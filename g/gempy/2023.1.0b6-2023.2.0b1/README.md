# Comparing `tmp/gempy-2023.1.0b6.tar.gz` & `tmp/gempy-2023.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy-2023.1.0b6.tar", last modified: Fri Sep 15 11:10:27 2023, max compression
+gzip compressed data, was "gempy-2023.2.0b1.tar", last modified: Wed Nov 22 15:32:39 2023, max compression
```

## Comparing `gempy-2023.1.0b6.tar` & `gempy-2023.2.0b1.tar`

### file list

```diff
@@ -1,149 +1,135 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      611 2023-08-02 08:39:02.000000 gempy-2023.1.0b6/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13879 2023-08-02 08:45:53.000000 gempy-2023.1.0b6/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)       36 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/MANIFEST.in
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10337 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9647 2023-06-18 08:55:36.000000 gempy-2023.1.0b6/README.md
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.144810 gempy-2023.1.0b6/examples/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.144810 gempy-2023.1.0b6/examples/examples/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/examples/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.144810 gempy-2023.1.0b6/examples/examples/geometries/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/examples/geometries/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1535 2023-09-06 07:11:17.000000 gempy-2023.1.0b6/examples/examples/geometries/a01_horizontal_stratigraphic.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1503 2023-09-06 07:11:17.000000 gempy-2023.1.0b6/examples/examples/geometries/b02_fold.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1453 2023-09-06 13:07:14.000000 gempy-2023.1.0b6/examples/examples/geometries/c03_recumbent_fold.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1527 2023-09-06 13:07:48.000000 gempy-2023.1.0b6/examples/examples/geometries/d04_pinchout.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1822 2023-09-06 07:11:17.000000 gempy-2023.1.0b6/examples/examples/geometries/e05_fault.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1688 2023-09-06 07:11:17.000000 gempy-2023.1.0b6/examples/examples/geometries/f06_unconformity.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.144810 gempy-2023.1.0b6/examples/examples/geometries/foo/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/examples/geometries/foo/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5896 2023-07-24 12:39:37.000000 gempy-2023.1.0b6/examples/examples/geometries/foo/more_examples.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2266 2023-09-06 07:21:56.000000 gempy-2023.1.0b6/examples/examples/geometries/g07_combination.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/examples/real/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3904 2023-09-12 09:31:40.000000 gempy-2023.1.0b6/examples/examples/real/Alesmodel.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6310 2023-09-11 06:47:13.000000 gempy-2023.1.0b6/examples/examples/real/Claudius.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2064 2023-07-28 08:26:22.000000 gempy-2023.1.0b6/examples/examples/real/Greenstone.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6213 2023-07-28 08:26:22.000000 gempy-2023.1.0b6/examples/examples/real/Hecho.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4802 2023-07-28 13:16:45.000000 gempy-2023.1.0b6/examples/examples/real/Moureze.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4952 2023-06-18 08:55:36.000000 gempy-2023.1.0b6/examples/examples/real/Perth_basin.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/examples/real/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/integrations/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/integrations/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6388 2023-07-28 08:26:22.000000 gempy-2023.1.0b6/examples/integrations/gempy_export_MOOSE.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6605 2023-07-28 13:21:00.000000 gempy-2023.1.0b6/examples/integrations/gempy_export_perth_bassin_pflotran.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5855 2023-08-16 09:16:18.000000 gempy-2023.1.0b6/examples/integrations/gempy_striplog.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5924 2023-07-28 08:26:22.000000 gempy-2023.1.0b6/examples/integrations/gempy_subsurface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/tutorials/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/tutorials/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/tutorials/ch2-Geophysics/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-08-15 11:18:26.000000 gempy-2023.1.0b6/examples/tutorials/ch2-Geophysics/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4339 2023-09-08 10:47:35.000000 gempy-2023.1.0b6/examples/tutorials/ch2-Geophysics/ch2_1_gravity.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3773 2023-09-08 10:47:35.000000 gempy-2023.1.0b6/examples/tutorials/ch2-Geophysics/ch2_2_cell_selection.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/tutorials/ch4-Topology/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-08-15 11:18:26.000000 gempy-2023.1.0b6/examples/tutorials/ch4-Topology/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5029 2023-09-08 10:47:35.000000 gempy-2023.1.0b6/examples/tutorials/ch4-Topology/ch4-1-Topology.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/tutorials_/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-08-15 12:56:33.000000 gempy-2023.1.0b6/examples/tutorials_/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/examples/tutorials_/a_getting_started/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/examples/tutorials_/a_getting_started/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9221 2023-09-07 13:41:35.000000 gempy-2023.1.0b6/examples/tutorials_/a_getting_started/get_started.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2056 2023-09-12 08:16:22.000000 gempy-2023.1.0b6/gempy/API/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3325 2023-09-11 09:19:28.000000 gempy-2023.1.0b6/gempy/API/compute_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9439 2023-09-14 15:24:21.000000 gempy-2023.1.0b6/gempy/API/examples_generator.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4052 2023-09-11 07:12:59.000000 gempy-2023.1.0b6/gempy/API/faults_API.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/API/gp2_gp3_compatibility/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-26 13:17:15.000000 gempy-2023.1.0b6/gempy/API/gp2_gp3_compatibility/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1470 2023-08-02 09:14:03.000000 gempy-2023.1.0b6/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_input.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3583 2023-07-12 09:03:18.000000 gempy-2023.1.0b6/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2776 2023-09-12 08:17:25.000000 gempy-2023.1.0b6/gempy/API/grid_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      135 2023-08-17 07:41:03.000000 gempy-2023.1.0b6/gempy/API/implicit_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6474 2023-09-12 09:00:44.000000 gempy-2023.1.0b6/gempy/API/initialization_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3575 2023-09-12 09:00:44.000000 gempy-2023.1.0b6/gempy/API/io_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4283 2023-08-02 12:59:55.000000 gempy-2023.1.0b6/gempy/API/map_stack_to_surfaces_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      547 2023-09-04 13:52:48.000000 gempy-2023.1.0b6/gempy/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)       36 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/gempy/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2836 2023-07-27 12:12:28.000000 gempy-2023.1.0b6/gempy/core/color_generator.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/core/data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1351 2023-09-12 07:54:31.000000 gempy-2023.1.0b6/gempy/core/data/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      806 2023-09-11 08:08:14.000000 gempy-2023.1.0b6/gempy/core/data/_data_points_helpers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      190 2023-09-04 12:57:36.000000 gempy-2023.1.0b6/gempy/core/data/enumerators.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      414 2023-09-11 09:17:24.000000 gempy-2023.1.0b6/gempy/core/data/gempy_engine_config.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7724 2023-09-08 07:54:28.000000 gempy-2023.1.0b6/gempy/core/data/geo_model.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10366 2023-09-11 09:31:09.000000 gempy-2023.1.0b6/gempy/core/data/grid.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/core/data/grid_modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      107 2023-08-02 09:19:18.000000 gempy-2023.1.0b6/gempy/core/data/grid_modules/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    14738 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/gempy/core/data/grid_modules/diamond_square.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    25145 2023-09-14 08:23:26.000000 gempy-2023.1.0b6/gempy/core/data/grid_modules/grid_types.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5911 2023-09-12 08:17:53.000000 gempy-2023.1.0b6/gempy/core/data/grid_modules/topography.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      654 2023-08-16 07:59:09.000000 gempy-2023.1.0b6/gempy/core/data/importer_helper.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7117 2023-09-08 13:13:02.000000 gempy-2023.1.0b6/gempy/core/data/orientations.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3677 2023-09-11 08:15:09.000000 gempy-2023.1.0b6/gempy/core/data/structural_element.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    19469 2023-09-11 08:14:54.000000 gempy-2023.1.0b6/gempy/core/data/structural_frame.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3650 2023-09-11 07:12:33.000000 gempy-2023.1.0b6/gempy/core/data/structural_group.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5712 2023-09-08 13:03:28.000000 gempy-2023.1.0b6/gempy/core/data/surface_points.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12422 2023-08-15 14:08:07.000000 gempy-2023.1.0b6/gempy/core/data/xsolution.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 10:07:04.000000 gempy-2023.1.0b6/gempy/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy/modules/custom_implicit_functions/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-08-17 07:30:25.000000 gempy-2023.1.0b6/gempy/modules/custom_implicit_functions/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2177 2023-08-17 08:30:05.000000 gempy-2023.1.0b6/gempy/modules/custom_implicit_functions/ellipsoid_implicit_function.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/gempy/modules/data_manipulation/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-08-16 08:15:52.000000 gempy-2023.1.0b6/gempy/modules/data_manipulation/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12520 2023-09-14 10:54:44.000000 gempy-2023.1.0b6/gempy/modules/data_manipulation/manipulate_points.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1514 2023-08-16 11:17:55.000000 gempy-2023.1.0b6/gempy/modules/data_manipulation/manipulate_structural_frame.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2163 2023-09-08 10:39:19.000000 gempy-2023.1.0b6/gempy/modules/data_manipulation/orientations_from_surface_points.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/gempy/modules/geophysics/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-08 10:45:13.000000 gempy-2023.1.0b6/gempy/modules/geophysics/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5313 2023-09-04 13:10:15.000000 gempy-2023.1.0b6/gempy/modules/geophysics/geophysics.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/gempy/modules/grids/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 14:11:58.000000 gempy-2023.1.0b6/gempy/modules/grids/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4432 2023-09-14 08:36:36.000000 gempy-2023.1.0b6/gempy/modules/grids/create_topography.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1368 2023-09-14 08:23:26.000000 gempy-2023.1.0b6/gempy/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.154810 gempy-2023.1.0b6/gempy.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10337 2023-09-15 11:10:27.000000 gempy-2023.1.0b6/gempy.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4423 2023-09-15 11:10:27.000000 gempy-2023.1.0b6/gempy.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-09-15 11:10:27.000000 gempy-2023.1.0b6/gempy.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)      113 2023-09-15 11:10:27.000000 gempy-2023.1.0b6/gempy.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       20 2023-09-15 11:10:27.000000 gempy-2023.1.0b6/gempy.egg-info/top_level.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       79 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1514 2023-09-15 11:09:24.000000 gempy-2023.1.0b6/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.144810 gempy-2023.1.0b6/test/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_api/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/test/test_api/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2261 2023-09-04 09:54:31.000000 gempy-2023.1.0b6/test/test_api/test_backends.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2367 2023-09-04 09:57:45.000000 gempy-2023.1.0b6/test/test_api/test_fault_api.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1013 2023-09-04 13:58:01.000000 gempy-2023.1.0b6/test/test_api/test_gempy_legacy_comp.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1530 2023-09-04 10:57:25.000000 gempy-2023.1.0b6/test/test_api/test_initialization_and_compute_api.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5668 2023-09-04 13:58:38.000000 gempy-2023.1.0b6/test/test_api/test_model_construction_granular.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      248 2023-09-04 11:10:18.000000 gempy-2023.1.0b6/test/test_api/test_show_input_data.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_community_bugs/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/test/test_community_bugs/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      155 2023-09-04 11:17:05.000000 gempy-2023.1.0b6/test/test_community_bugs/test_community_bugs.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/test/test_core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      467 2023-07-11 12:03:33.000000 gempy-2023.1.0b6/test/test_core/test_color_generator.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2917 2023-09-04 10:53:42.000000 gempy-2023.1.0b6/test/test_core/test_transfoms.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_model_types/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy-2023.1.0b6/test/test_model_types/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2191 2023-09-06 12:13:12.000000 gempy-2023.1.0b6/test/test_model_types/test_example_models_I.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3438 2023-09-07 14:29:46.000000 gempy-2023.1.0b6/test/test_model_types/test_subduction.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-26 13:08:38.000000 gempy-2023.1.0b6/test/test_modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_modules/_geophysics_TO_UPDATE/
--rw-r--r--   0 leguark   (1000) leguark   (1000)       91 2023-09-04 13:05:00.000000 gempy-2023.1.0b6/test/test_modules/_geophysics_TO_UPDATE/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1483 2023-08-16 09:16:18.000000 gempy-2023.1.0b6/test/test_modules/_geophysics_TO_UPDATE/test_gravity.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      371 2023-09-08 10:47:35.000000 gempy-2023.1.0b6/test/test_modules/_geophysics_TO_UPDATE/test_grid_tz.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3697 2023-09-08 10:47:35.000000 gempy-2023.1.0b6/test/test_modules/_geophysics_TO_UPDATE/test_magnetics.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_modules/test_faults/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-09-04 09:29:47.000000 gempy-2023.1.0b6/test/test_modules/test_faults/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6241 2023-09-04 09:39:20.000000 gempy-2023.1.0b6/test/test_modules/test_faults/test_finite_faults.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1454 2023-09-14 13:16:25.000000 gempy-2023.1.0b6/test/test_modules/test_gempy_subsurface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 11:10:27.164810 gempy-2023.1.0b6/test/test_modules/test_grids/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-27 14:34:21.000000 gempy-2023.1.0b6/test/test_modules/test_grids/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1411 2023-09-04 09:46:33.000000 gempy-2023.1.0b6/test/test_modules/test_grids/test_custom_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8214 2023-08-02 09:04:35.000000 gempy-2023.1.0b6/test/test_modules/test_grids/test_diamond_square.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1594 2023-09-04 09:46:33.000000 gempy-2023.1.0b6/test/test_modules/test_grids/test_grids_I.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2190 2023-09-04 09:47:59.000000 gempy-2023.1.0b6/test/test_modules/test_grids/test_grids_sections.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      630 2023-10-11 08:27:11.000000 gempy-2023.2.0b1/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    14167 2023-10-11 08:27:11.000000 gempy-2023.2.0b1/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-10-11 08:27:11.000000 gempy-2023.2.0b1/MANIFEST.in
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12869 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11835 2023-11-15 08:14:26.000000 gempy-2023.2.0b1/README.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.311547 gempy-2023.2.0b1/examples/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/examples/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/examples/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/examples/geometries/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/examples/geometries/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1525 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/examples/examples/geometries/a01_horizontal_stratigraphic.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1493 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/examples/examples/geometries/b02_fold.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1443 2023-10-11 08:49:21.000000 gempy-2023.2.0b1/examples/examples/geometries/c03_recumbent_fold.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1517 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/examples/examples/geometries/d04_pinchout.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1812 2023-10-11 08:49:21.000000 gempy-2023.2.0b1/examples/examples/geometries/e05_fault.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1678 2023-10-11 08:49:21.000000 gempy-2023.2.0b1/examples/examples/geometries/f06_unconformity.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2256 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/examples/examples/geometries/g07_combination.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5431 2023-10-11 11:31:52.000000 gempy-2023.2.0b1/examples/examples/geometries/h08_more_examples.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/examples/real/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3896 2023-10-11 14:24:29.000000 gempy-2023.2.0b1/examples/examples/real/Alesmodel.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6399 2023-10-11 12:42:08.000000 gempy-2023.2.0b1/examples/examples/real/Claudius.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1491 2023-10-11 12:49:47.000000 gempy-2023.2.0b1/examples/examples/real/Greenstone.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5601 2023-10-11 08:49:21.000000 gempy-2023.2.0b1/examples/examples/real/Hecho.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4687 2023-11-22 12:08:33.000000 gempy-2023.2.0b1/examples/examples/real/Moureze.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2870 2023-11-22 12:31:36.000000 gempy-2023.2.0b1/examples/examples/real/Perth_basin.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/examples/real/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/integrations/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/integrations/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6388 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/integrations/gempy_export_MOOSE.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5924 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/integrations/gempy_subsurface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/tutorials/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/tutorials/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/tutorials/a_getting_started/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/tutorials/a_getting_started/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9211 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/examples/tutorials/a_getting_started/get_started.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/examples/tutorials/ch4-Topology/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/examples/tutorials/ch4-Topology/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5270 2023-10-11 08:52:02.000000 gempy-2023.2.0b1/examples/tutorials/ch4-Topology/ch4-1-Topology.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2296 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3570 2023-11-22 07:59:49.000000 gempy-2023.2.0b1/gempy/API/compute_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9618 2023-11-21 16:35:03.000000 gempy-2023.2.0b1/gempy/API/examples_generator.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4403 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/faults_API.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/API/gp2_gp3_compatibility/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/gp2_gp3_compatibility/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1509 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_input.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3583 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3299 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/grid_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      137 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/implicit_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6452 2023-11-10 13:27:56.000000 gempy-2023.2.0b1/gempy/API/initialization_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3575 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/io_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4283 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/API/map_stack_to_surfaces_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      549 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2913 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/color_generator.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/core/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1577 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      827 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/_data_points_helpers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2131 2023-11-22 08:31:15.000000 gempy-2023.2.0b1/gempy/core/data/core_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      199 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/enumerators.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      425 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/gempy_engine_config.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8146 2023-11-21 08:32:45.000000 gempy-2023.2.0b1/gempy/core/data/geo_model.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10364 2023-11-21 12:28:28.000000 gempy-2023.2.0b1/gempy/core/data/grid.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/core/data/grid_modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       95 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/grid_modules/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    15090 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/grid_modules/diamond_square.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11346 2023-11-22 08:30:22.000000 gempy-2023.2.0b1/gempy/core/data/grid_modules/grid_types.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6116 2023-10-11 14:22:35.000000 gempy-2023.2.0b1/gempy/core/data/grid_modules/topography.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      678 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/importer_helper.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7117 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/orientations.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3677 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/structural_element.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    20509 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/structural_frame.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4154 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/structural_group.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5712 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/surface_points.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12422 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/core/data/xsolution.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/modules/custom_implicit_functions/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/custom_implicit_functions/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2238 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/custom_implicit_functions/ellipsoid_implicit_function.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/modules/data_manipulation/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/data_manipulation/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12820 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/data_manipulation/manipulate_points.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1875 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/data_manipulation/manipulate_structural_frame.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2226 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/data_manipulation/orientations_from_surface_points.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy/modules/grids/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/grids/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4560 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/modules/grids/create_topography.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1368 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/gempy/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/gempy.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12869 2023-11-22 15:32:39.000000 gempy-2023.2.0b1/gempy.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3929 2023-11-22 15:32:39.000000 gempy-2023.2.0b1/gempy.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-11-22 15:32:39.000000 gempy-2023.2.0b1/gempy.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      107 2023-11-22 15:32:39.000000 gempy-2023.2.0b1/gempy.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       20 2023-11-22 15:32:39.000000 gempy-2023.2.0b1/gempy.egg-info/top_level.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       79 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2223 2023-11-22 15:32:27.000000 gempy-2023.2.0b1/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.311547 gempy-2023.2.0b1/test/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_api/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2261 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/test_backends.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2543 2023-11-21 16:24:08.000000 gempy-2023.2.0b1/test/test_api/test_fault_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1047 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/test_gempy_legacy_comp.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1585 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/test_initialization_and_compute_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5668 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/test_model_construction_granular.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      255 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_api/test_show_input_data.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_community_bugs/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_community_bugs/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      155 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_community_bugs/test_community_bugs.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      483 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_core/test_color_generator.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3005 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_core/test_transfoms.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_model_types/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_model_types/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2272 2023-11-21 16:36:20.000000 gempy-2023.2.0b1/test/test_model_types/test_example_models_I.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3531 2023-11-21 16:36:55.000000 gempy-2023.2.0b1/test/test_model_types/test_subduction.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_modules/_geophysics_TO_UPDATE/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       93 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/_geophysics_TO_UPDATE/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2577 2023-10-11 08:49:22.000000 gempy-2023.2.0b1/test/test_modules/_geophysics_TO_UPDATE/test_gravity.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_modules/test_faults/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_faults/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6427 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_faults/test_finite_faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1849 2023-11-21 16:20:18.000000 gempy-2023.2.0b1/test/test_modules/test_gempy_subsurface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:32:39.321547 gempy-2023.2.0b1/test/test_modules/test_grids/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_grids/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1468 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_grids/test_custom_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8362 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_grids/test_diamond_square.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1638 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_grids/test_grids_I.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2273 2023-10-11 08:27:12.000000 gempy-2023.2.0b1/test/test_modules/test_grids/test_grids_sections.py
```

### Comparing `gempy-2023.1.0b6/AUTHORS.rst` & `gempy-2023.2.0b1/AUTHORS.rst`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-.. _authors_ref:
-
-Authors
--------
-
-.. image:: https://img.shields.io/github/contributors/gempy-project/gempy_engine.svg?logo=github&logoColor=white
-   :target: https://github.com/gempy-projects/gempy_engine/graphs/contributors/
-
-
-The following is a list of authors who have made substantial contributions to
-the conception or design of this software; or the creation of new code used in
-this software; or have drafted the work or substantively revised it:
-
-- Miguel de la Varga, (`@leguark <https://github.com/leguark/>`_)
-- Alexander Zimmerman
-- Elisa Heim
-- Alexander Schaaf
-- Fabian Stamm
-- Florian Wellmann
+.. _authors_ref:
+
+Authors
+-------
+
+.. image:: https://img.shields.io/github/contributors/gempy-project/gempy_engine.svg?logo=github&logoColor=white
+   :target: https://github.com/gempy-projects/gempy_engine/graphs/contributors/
+
+
+The following is a list of authors who have made substantial contributions to
+the conception or design of this software; or the creation of new code used in
+this software; or have drafted the work or substantively revised it:
+
+- Miguel de la Varga, (`@leguark <https://github.com/leguark/>`_)
+- Alexander Zimmerman
+- Elisa Heim
+- Alexander Schaaf
+- Fabian Stamm
+- Florian Wellmann
```

### Comparing `gempy-2023.1.0b6/LICENSE` & `gempy-2023.2.0b1/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-Copyright (c) 2020-2023 The GemPy Engine Developers
-
-                      EUROPEAN UNION PUBLIC LICENCE v. 1.2
-                      EUPL © the European Union 2007, 2016
-
-This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
-below) which is provided under the terms of this Licence. Any use of the Work,
-other than as authorised under this Licence is prohibited (to the extent such
-use is covered by a right of the copyright holder of the Work).
-
-The Work is provided under the terms of this Licence when the Licensor (as
-defined below) has placed the following notice immediately following the
-copyright notice for the Work:
-
-        Licensed under the EUPL
-
-or has expressed by any other means his willingness to license under the EUPL.
-
-1. Definitions
-
-In this Licence, the following terms have the following meaning:
-
-- ‘The Licence’: this Licence.
-
-- ‘The Original Work’: the work or software distributed or communicated by the
-  Licensor under this Licence, available as Source Code and also as Executable
-  Code as the case may be.
-
-- ‘Derivative Works’: the works or software that could be created by the
-  Licensee, based upon the Original Work or modifications thereof. This Licence
-  does not define the extent of modification or dependence on the Original Work
-  required in order to classify a work as a Derivative Work; this extent is
-  determined by copyright law applicable in the country mentioned in Article 15.
-
-- ‘The Work’: the Original Work or its Derivative Works.
-
-- ‘The Source Code’: the human-readable form of the Work which is the most
-  convenient for people to study and modify.
-
-- ‘The Executable Code’: any code which has generally been compiled and which is
-  meant to be interpreted by a computer as a program.
-
-- ‘The Licensor’: the natural or legal person that distributes or communicates
-  the Work under the Licence.
-
-- ‘Contributor(s)’: any natural or legal person who modifies the Work under the
-  Licence, or otherwise contributes to the creation of a Derivative Work.
-
-- ‘The Licensee’ or ‘You’: any natural or legal person who makes any usage of
-  the Work under the terms of the Licence.
-
-- ‘Distribution’ or ‘Communication’: any act of selling, giving, lending,
-  renting, distributing, communicating, transmitting, or otherwise making
-  available, online or offline, copies of the Work or providing access to its
-  essential functionalities at the disposal of any other natural or legal
-  person.
-
-2. Scope of the rights granted by the Licence
-
-The Licensor hereby grants You a worldwide, royalty-free, non-exclusive,
-sublicensable licence to do the following, for the duration of copyright vested
-in the Original Work:
-
-- use the Work in any circumstance and for all usage,
-- reproduce the Work,
-- modify the Work, and make Derivative Works based upon the Work,
-- communicate to the public, including the right to make available or display
-  the Work or copies thereof to the public and perform publicly, as the case may
-  be, the Work,
-- distribute the Work or copies thereof,
-- lend and rent the Work or copies thereof,
-- sublicense rights in the Work or copies thereof.
-
-Those rights can be exercised on any media, supports and formats, whether now
-known or later invented, as far as the applicable law permits so.
-
-In the countries where moral rights apply, the Licensor waives his right to
-exercise his moral right to the extent allowed by law in order to make effective
-the licence of the economic rights here above listed.
-
-The Licensor grants to the Licensee royalty-free, non-exclusive usage rights to
-any patents held by the Licensor, to the extent necessary to make use of the
-rights granted on the Work under this Licence.
-
-3. Communication of the Source Code
-
-The Licensor may provide the Work either in its Source Code form, or as
-Executable Code. If the Work is provided as Executable Code, the Licensor
-provides in addition a machine-readable copy of the Source Code of the Work
-along with each copy of the Work that the Licensor distributes or indicates, in
-a notice following the copyright notice attached to the Work, a repository where
-the Source Code is easily and freely accessible for as long as the Licensor
-continues to distribute or communicate the Work.
-
-4. Limitations on copyright
-
-Nothing in this Licence is intended to deprive the Licensee of the benefits from
-any exception or limitation to the exclusive rights of the rights owners in the
-Work, of the exhaustion of those rights or of other applicable limitations
-thereto.
-
-5. Obligations of the Licensee
-
-The grant of the rights mentioned above is subject to some restrictions and
-obligations imposed on the Licensee. Those obligations are the following:
-
-Attribution right: The Licensee shall keep intact all copyright, patent or
-trademarks notices and all notices that refer to the Licence and to the
-disclaimer of warranties. The Licensee must include a copy of such notices and a
-copy of the Licence with every copy of the Work he/she distributes or
-communicates. The Licensee must cause any Derivative Work to carry prominent
-notices stating that the Work has been modified and the date of modification.
-
-Copyleft clause: If the Licensee distributes or communicates copies of the
-Original Works or Derivative Works, this Distribution or Communication will be
-done under the terms of this Licence or of a later version of this Licence
-unless the Original Work is expressly distributed only under this version of the
-Licence — for example by communicating ‘EUPL v. 1.2 only’. The Licensee
-(becoming Licensor) cannot offer or impose any additional terms or conditions on
-the Work or Derivative Work that alter or restrict the terms of the Licence.
-
-Compatibility clause: If the Licensee Distributes or Communicates Derivative
-Works or copies thereof based upon both the Work and another work licensed under
-a Compatible Licence, this Distribution or Communication can be done under the
-terms of this Compatible Licence. For the sake of this clause, ‘Compatible
-Licence’ refers to the licences listed in the appendix attached to this Licence.
-Should the Licensee's obligations under the Compatible Licence conflict with
-his/her obligations under this Licence, the obligations of the Compatible
-Licence shall prevail.
-
-Provision of Source Code: When distributing or communicating copies of the Work,
-the Licensee will provide a machine-readable copy of the Source Code or indicate
-a repository where this Source will be easily and freely available for as long
-as the Licensee continues to distribute or communicate the Work.
-
-Legal Protection: This Licence does not grant permission to use the trade names,
-trademarks, service marks, or names of the Licensor, except as required for
-reasonable and customary use in describing the origin of the Work and
-reproducing the content of the copyright notice.
-
-6. Chain of Authorship
-
-The original Licensor warrants that the copyright in the Original Work granted
-hereunder is owned by him/her or licensed to him/her and that he/she has the
-power and authority to grant the Licence.
-
-Each Contributor warrants that the copyright in the modifications he/she brings
-to the Work are owned by him/her or licensed to him/her and that he/she has the
-power and authority to grant the Licence.
-
-Each time You accept the Licence, the original Licensor and subsequent
-Contributors grant You a licence to their contributions to the Work, under the
-terms of this Licence.
-
-7. Disclaimer of Warranty
-
-The Work is a work in progress, which is continuously improved by numerous
-Contributors. It is not a finished work and may therefore contain defects or
-‘bugs’ inherent to this type of development.
-
-For the above reason, the Work is provided under the Licence on an ‘as is’ basis
-and without warranties of any kind concerning the Work, including without
-limitation merchantability, fitness for a particular purpose, absence of defects
-or errors, accuracy, non-infringement of intellectual property rights other than
-copyright as stated in Article 6 of this Licence.
-
-This disclaimer of warranty is an essential part of the Licence and a condition
-for the grant of any rights to the Work.
-
-8. Disclaimer of Liability
-
-Except in the cases of wilful misconduct or damages directly caused to natural
-persons, the Licensor will in no event be liable for any direct or indirect,
-material or moral, damages of any kind, arising out of the Licence or of the use
-of the Work, including without limitation, damages for loss of goodwill, work
-stoppage, computer failure or malfunction, loss of data or any commercial
-damage, even if the Licensor has been advised of the possibility of such damage.
-However, the Licensor will be liable under statutory product liability laws as
-far such laws apply to the Work.
-
-9. Additional agreements
-
-While distributing the Work, You may choose to conclude an additional agreement,
-defining obligations or services consistent with this Licence. However, if
-accepting obligations, You may act only on your own behalf and on your sole
-responsibility, not on behalf of the original Licensor or any other Contributor,
-and only if You agree to indemnify, defend, and hold each Contributor harmless
-for any liability incurred by, or claims asserted against such Contributor by
-the fact You have accepted any warranty or additional liability.
-
-10. Acceptance of the Licence
-
-The provisions of this Licence can be accepted by clicking on an icon ‘I agree’
-placed under the bottom of a window displaying the text of this Licence or by
-affirming consent in any other similar way, in accordance with the rules of
-applicable law. Clicking on that icon indicates your clear and irrevocable
-acceptance of this Licence and all of its terms and conditions.
-
-Similarly, you irrevocably accept this Licence and all of its terms and
-conditions by exercising any rights granted to You by Article 2 of this Licence,
-such as the use of the Work, the creation by You of a Derivative Work or the
-Distribution or Communication by You of the Work or copies thereof.
-
-11. Information to the public
-
-In case of any Distribution or Communication of the Work by means of electronic
-communication by You (for example, by offering to download the Work from a
-remote location) the distribution channel or media (for example, a website) must
-at least provide to the public the information requested by the applicable law
-regarding the Licensor, the Licence and the way it may be accessible, concluded,
-stored and reproduced by the Licensee.
-
-12. Termination of the Licence
-
-The Licence and the rights granted hereunder will terminate automatically upon
-any breach by the Licensee of the terms of the Licence.
-
-Such a termination will not terminate the licences of any person who has
-received the Work from the Licensee under the Licence, provided such persons
-remain in full compliance with the Licence.
-
-13. Miscellaneous
-
-Without prejudice of Article 9 above, the Licence represents the complete
-agreement between the Parties as to the Work.
-
-If any provision of the Licence is invalid or unenforceable under applicable
-law, this will not affect the validity or enforceability of the Licence as a
-whole. Such provision will be construed or reformed so as necessary to make it
-valid and enforceable.
-
-The European Commission may publish other linguistic versions or new versions of
-this Licence or updated versions of the Appendix, so far this is required and
-reasonable, without reducing the scope of the rights granted by the Licence. New
-versions of the Licence will be published with a unique version number.
-
-All linguistic versions of this Licence, approved by the European Commission,
-have identical value. Parties can take advantage of the linguistic version of
-their choice.
-
-14. Jurisdiction
-
-Without prejudice to specific agreement between parties,
-
-- any litigation resulting from the interpretation of this License, arising
-  between the European Union institutions, bodies, offices or agencies, as a
-  Licensor, and any Licensee, will be subject to the jurisdiction of the Court
-  of Justice of the European Union, as laid down in article 272 of the Treaty on
-  the Functioning of the European Union,
-
-- any litigation arising between other parties and resulting from the
-  interpretation of this License, will be subject to the exclusive jurisdiction
-  of the competent court where the Licensor resides or conducts its primary
-  business.
-
-15. Applicable Law
-
-Without prejudice to specific agreement between parties,
-
-- this Licence shall be governed by the law of the European Union Member State
-  where the Licensor has his seat, resides or has his registered office,
-
-- this licence shall be governed by Belgian law if the Licensor has no seat,
-  residence or registered office inside a European Union Member State.
-
-Appendix
-
-‘Compatible Licences’ according to Article 5 EUPL are:
-
-- GNU General Public License (GPL) v. 2, v. 3
-- GNU Affero General Public License (AGPL) v. 3
-- Open Software License (OSL) v. 2.1, v. 3.0
-- Eclipse Public License (EPL) v. 1.0
-- CeCILL v. 2.0, v. 2.1
-- Mozilla Public Licence (MPL) v. 2
-- GNU Lesser General Public Licence (LGPL) v. 2.1, v. 3
-- Creative Commons Attribution-ShareAlike v. 3.0 Unported (CC BY-SA 3.0) for
-  works other than software
-- European Union Public Licence (EUPL) v. 1.1, v. 1.2
-- Québec Free and Open-Source Licence — Reciprocity (LiLiQ-R) or Strong
-  Reciprocity (LiLiQ-R+).
-
-The European Commission may update this Appendix to later versions of the above
-licences without producing a new version of the EUPL, as long as they provide
-the rights granted in Article 2 of this Licence and protect the covered Source
-Code from exclusive appropriation.
-
-All other changes or additions to this Appendix require the production of a new
+Copyright (c) 2020-2023 The GemPy Engine Developers
+
+                      EUROPEAN UNION PUBLIC LICENCE v. 1.2
+                      EUPL © the European Union 2007, 2016
+
+This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
+below) which is provided under the terms of this Licence. Any use of the Work,
+other than as authorised under this Licence is prohibited (to the extent such
+use is covered by a right of the copyright holder of the Work).
+
+The Work is provided under the terms of this Licence when the Licensor (as
+defined below) has placed the following notice immediately following the
+copyright notice for the Work:
+
+        Licensed under the EUPL
+
+or has expressed by any other means his willingness to license under the EUPL.
+
+1. Definitions
+
+In this Licence, the following terms have the following meaning:
+
+- ‘The Licence’: this Licence.
+
+- ‘The Original Work’: the work or software distributed or communicated by the
+  Licensor under this Licence, available as Source Code and also as Executable
+  Code as the case may be.
+
+- ‘Derivative Works’: the works or software that could be created by the
+  Licensee, based upon the Original Work or modifications thereof. This Licence
+  does not define the extent of modification or dependence on the Original Work
+  required in order to classify a work as a Derivative Work; this extent is
+  determined by copyright law applicable in the country mentioned in Article 15.
+
+- ‘The Work’: the Original Work or its Derivative Works.
+
+- ‘The Source Code’: the human-readable form of the Work which is the most
+  convenient for people to study and modify.
+
+- ‘The Executable Code’: any code which has generally been compiled and which is
+  meant to be interpreted by a computer as a program.
+
+- ‘The Licensor’: the natural or legal person that distributes or communicates
+  the Work under the Licence.
+
+- ‘Contributor(s)’: any natural or legal person who modifies the Work under the
+  Licence, or otherwise contributes to the creation of a Derivative Work.
+
+- ‘The Licensee’ or ‘You’: any natural or legal person who makes any usage of
+  the Work under the terms of the Licence.
+
+- ‘Distribution’ or ‘Communication’: any act of selling, giving, lending,
+  renting, distributing, communicating, transmitting, or otherwise making
+  available, online or offline, copies of the Work or providing access to its
+  essential functionalities at the disposal of any other natural or legal
+  person.
+
+2. Scope of the rights granted by the Licence
+
+The Licensor hereby grants You a worldwide, royalty-free, non-exclusive,
+sublicensable licence to do the following, for the duration of copyright vested
+in the Original Work:
+
+- use the Work in any circumstance and for all usage,
+- reproduce the Work,
+- modify the Work, and make Derivative Works based upon the Work,
+- communicate to the public, including the right to make available or display
+  the Work or copies thereof to the public and perform publicly, as the case may
+  be, the Work,
+- distribute the Work or copies thereof,
+- lend and rent the Work or copies thereof,
+- sublicense rights in the Work or copies thereof.
+
+Those rights can be exercised on any media, supports and formats, whether now
+known or later invented, as far as the applicable law permits so.
+
+In the countries where moral rights apply, the Licensor waives his right to
+exercise his moral right to the extent allowed by law in order to make effective
+the licence of the economic rights here above listed.
+
+The Licensor grants to the Licensee royalty-free, non-exclusive usage rights to
+any patents held by the Licensor, to the extent necessary to make use of the
+rights granted on the Work under this Licence.
+
+3. Communication of the Source Code
+
+The Licensor may provide the Work either in its Source Code form, or as
+Executable Code. If the Work is provided as Executable Code, the Licensor
+provides in addition a machine-readable copy of the Source Code of the Work
+along with each copy of the Work that the Licensor distributes or indicates, in
+a notice following the copyright notice attached to the Work, a repository where
+the Source Code is easily and freely accessible for as long as the Licensor
+continues to distribute or communicate the Work.
+
+4. Limitations on copyright
+
+Nothing in this Licence is intended to deprive the Licensee of the benefits from
+any exception or limitation to the exclusive rights of the rights owners in the
+Work, of the exhaustion of those rights or of other applicable limitations
+thereto.
+
+5. Obligations of the Licensee
+
+The grant of the rights mentioned above is subject to some restrictions and
+obligations imposed on the Licensee. Those obligations are the following:
+
+Attribution right: The Licensee shall keep intact all copyright, patent or
+trademarks notices and all notices that refer to the Licence and to the
+disclaimer of warranties. The Licensee must include a copy of such notices and a
+copy of the Licence with every copy of the Work he/she distributes or
+communicates. The Licensee must cause any Derivative Work to carry prominent
+notices stating that the Work has been modified and the date of modification.
+
+Copyleft clause: If the Licensee distributes or communicates copies of the
+Original Works or Derivative Works, this Distribution or Communication will be
+done under the terms of this Licence or of a later version of this Licence
+unless the Original Work is expressly distributed only under this version of the
+Licence — for example by communicating ‘EUPL v. 1.2 only’. The Licensee
+(becoming Licensor) cannot offer or impose any additional terms or conditions on
+the Work or Derivative Work that alter or restrict the terms of the Licence.
+
+Compatibility clause: If the Licensee Distributes or Communicates Derivative
+Works or copies thereof based upon both the Work and another work licensed under
+a Compatible Licence, this Distribution or Communication can be done under the
+terms of this Compatible Licence. For the sake of this clause, ‘Compatible
+Licence’ refers to the licences listed in the appendix attached to this Licence.
+Should the Licensee's obligations under the Compatible Licence conflict with
+his/her obligations under this Licence, the obligations of the Compatible
+Licence shall prevail.
+
+Provision of Source Code: When distributing or communicating copies of the Work,
+the Licensee will provide a machine-readable copy of the Source Code or indicate
+a repository where this Source will be easily and freely available for as long
+as the Licensee continues to distribute or communicate the Work.
+
+Legal Protection: This Licence does not grant permission to use the trade names,
+trademarks, service marks, or names of the Licensor, except as required for
+reasonable and customary use in describing the origin of the Work and
+reproducing the content of the copyright notice.
+
+6. Chain of Authorship
+
+The original Licensor warrants that the copyright in the Original Work granted
+hereunder is owned by him/her or licensed to him/her and that he/she has the
+power and authority to grant the Licence.
+
+Each Contributor warrants that the copyright in the modifications he/she brings
+to the Work are owned by him/her or licensed to him/her and that he/she has the
+power and authority to grant the Licence.
+
+Each time You accept the Licence, the original Licensor and subsequent
+Contributors grant You a licence to their contributions to the Work, under the
+terms of this Licence.
+
+7. Disclaimer of Warranty
+
+The Work is a work in progress, which is continuously improved by numerous
+Contributors. It is not a finished work and may therefore contain defects or
+‘bugs’ inherent to this type of development.
+
+For the above reason, the Work is provided under the Licence on an ‘as is’ basis
+and without warranties of any kind concerning the Work, including without
+limitation merchantability, fitness for a particular purpose, absence of defects
+or errors, accuracy, non-infringement of intellectual property rights other than
+copyright as stated in Article 6 of this Licence.
+
+This disclaimer of warranty is an essential part of the Licence and a condition
+for the grant of any rights to the Work.
+
+8. Disclaimer of Liability
+
+Except in the cases of wilful misconduct or damages directly caused to natural
+persons, the Licensor will in no event be liable for any direct or indirect,
+material or moral, damages of any kind, arising out of the Licence or of the use
+of the Work, including without limitation, damages for loss of goodwill, work
+stoppage, computer failure or malfunction, loss of data or any commercial
+damage, even if the Licensor has been advised of the possibility of such damage.
+However, the Licensor will be liable under statutory product liability laws as
+far such laws apply to the Work.
+
+9. Additional agreements
+
+While distributing the Work, You may choose to conclude an additional agreement,
+defining obligations or services consistent with this Licence. However, if
+accepting obligations, You may act only on your own behalf and on your sole
+responsibility, not on behalf of the original Licensor or any other Contributor,
+and only if You agree to indemnify, defend, and hold each Contributor harmless
+for any liability incurred by, or claims asserted against such Contributor by
+the fact You have accepted any warranty or additional liability.
+
+10. Acceptance of the Licence
+
+The provisions of this Licence can be accepted by clicking on an icon ‘I agree’
+placed under the bottom of a window displaying the text of this Licence or by
+affirming consent in any other similar way, in accordance with the rules of
+applicable law. Clicking on that icon indicates your clear and irrevocable
+acceptance of this Licence and all of its terms and conditions.
+
+Similarly, you irrevocably accept this Licence and all of its terms and
+conditions by exercising any rights granted to You by Article 2 of this Licence,
+such as the use of the Work, the creation by You of a Derivative Work or the
+Distribution or Communication by You of the Work or copies thereof.
+
+11. Information to the public
+
+In case of any Distribution or Communication of the Work by means of electronic
+communication by You (for example, by offering to download the Work from a
+remote location) the distribution channel or media (for example, a website) must
+at least provide to the public the information requested by the applicable law
+regarding the Licensor, the Licence and the way it may be accessible, concluded,
+stored and reproduced by the Licensee.
+
+12. Termination of the Licence
+
+The Licence and the rights granted hereunder will terminate automatically upon
+any breach by the Licensee of the terms of the Licence.
+
+Such a termination will not terminate the licences of any person who has
+received the Work from the Licensee under the Licence, provided such persons
+remain in full compliance with the Licence.
+
+13. Miscellaneous
+
+Without prejudice of Article 9 above, the Licence represents the complete
+agreement between the Parties as to the Work.
+
+If any provision of the Licence is invalid or unenforceable under applicable
+law, this will not affect the validity or enforceability of the Licence as a
+whole. Such provision will be construed or reformed so as necessary to make it
+valid and enforceable.
+
+The European Commission may publish other linguistic versions or new versions of
+this Licence or updated versions of the Appendix, so far this is required and
+reasonable, without reducing the scope of the rights granted by the Licence. New
+versions of the Licence will be published with a unique version number.
+
+All linguistic versions of this Licence, approved by the European Commission,
+have identical value. Parties can take advantage of the linguistic version of
+their choice.
+
+14. Jurisdiction
+
+Without prejudice to specific agreement between parties,
+
+- any litigation resulting from the interpretation of this License, arising
+  between the European Union institutions, bodies, offices or agencies, as a
+  Licensor, and any Licensee, will be subject to the jurisdiction of the Court
+  of Justice of the European Union, as laid down in article 272 of the Treaty on
+  the Functioning of the European Union,
+
+- any litigation arising between other parties and resulting from the
+  interpretation of this License, will be subject to the exclusive jurisdiction
+  of the competent court where the Licensor resides or conducts its primary
+  business.
+
+15. Applicable Law
+
+Without prejudice to specific agreement between parties,
+
+- this Licence shall be governed by the law of the European Union Member State
+  where the Licensor has his seat, resides or has his registered office,
+
+- this licence shall be governed by Belgian law if the Licensor has no seat,
+  residence or registered office inside a European Union Member State.
+
+Appendix
+
+‘Compatible Licences’ according to Article 5 EUPL are:
+
+- GNU General Public License (GPL) v. 2, v. 3
+- GNU Affero General Public License (AGPL) v. 3
+- Open Software License (OSL) v. 2.1, v. 3.0
+- Eclipse Public License (EPL) v. 1.0
+- CeCILL v. 2.0, v. 2.1
+- Mozilla Public Licence (MPL) v. 2
+- GNU Lesser General Public Licence (LGPL) v. 2.1, v. 3
+- Creative Commons Attribution-ShareAlike v. 3.0 Unported (CC BY-SA 3.0) for
+  works other than software
+- European Union Public Licence (EUPL) v. 1.1, v. 1.2
+- Québec Free and Open-Source Licence — Reciprocity (LiLiQ-R) or Strong
+  Reciprocity (LiLiQ-R+).
+
+The European Commission may update this Appendix to later versions of the above
+licences without producing a new version of the EUPL, as long as they provide
+the rights granted in Article 2 of this Licence and protect the covered Source
+Code from exclusive appropriation.
+
+All other changes or additions to this Appendix require the production of a new
 EUPL version.
```

### Comparing `gempy-2023.1.0b6/PKG-INFO` & `gempy-2023.2.0b1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,227 +1,219 @@
-Metadata-Version: 2.1
-Name: gempy
-Version: 2023.1.0b6
-Summary: An Open-source, Python-based 3-D structural geological modeling software.
-Home-page: https://github.com/cgre-aachen/gempy
-Author: Miguel de la Varga, Alexander Zimmerman, Elisa Heim, Alexander Schaaf, Fabian Stamm, Florian Wellmann, Jan Niederau, Andrew Annex
-Author-email: miguel@terranigma-solutions.com
-License: EUPL-1.2
-Keywords: geology,3-D modeling,structural geology,uncertainty
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: opt
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# <p align="center"><img src="docs/readme_images/header_combined_slim.png" width="1000"></p>
-
-> Open-source, implicit 3D structural geological modeling in Python.
-
-[![PyPI](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/)
-[![PyPI](https://img.shields.io/badge/pypi-1.0-blue.svg)](https://pypi.org/project/gempy/)
-[![license: LGPL v3](https://img.shields.io/badge/license-LGPL%20v3-blue.svg)](https://github.com/cgre-aachen/gempy/blob/master/LICENSE)
-[![Documentation Status](https://assets.readthedocs.org/static/projects/badges/passing-flat.svg)](http://docs.gempy.org)
-[![Travis Build](https://travis-ci.org/cgre-aachen/gempy.svg?branch=master)](https://travis-ci.org/github/cgre-aachen/gempy/branches)
-[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/cgre-aachen/gempy/master)
-[![DOI](https://zenodo.org/badge/96211155.svg)](https://zenodo.org/badge/latestdoi/96211155)
-[![DOCKER](https://img.shields.io/docker/cloud/automated/leguark/gempy.svg)](https://cloud.docker.com/repository/docker/leguark/gempy)
-
-## Overview
-
-[GemPy](https://www.gempy.org/) is a Python-based, **open-source geomodeling library**. It is
-capable of constructing complex **3D geological models** of folded
-structures, fault networks and unconformities, based on the underlying
-powerful **implicit representation** approach. 
-
-## Installation
-
-We provide the latest release version of GemPy via PyPi package services. We highly recommend using PyPi,
-
-`$ pip install gempy`
-
-as it will take care of automatically installing all the required dependencies - except in windows that requires one extra step.
-
-Windows does not have a gcc compilers pre-installed. The easiest way to get a aesara compatible compiler is by using 
-the aesara conda installation. Therefore the process would be the following:
-
-`$ conda install aesara`
-
-`$ pip install gempy`
-
-For more information, refer to the [installation documentation](https://docs.gempy.org/installation.html).
-
-## Requirements
-
-The following versions are required/strongly recommended for the main dependencies of GemPy (as of June 2023):
-- python>=3.10
-- pandas>=2.0
-- matplotlib>=3.7
-- pyvista>=0.39
-
-## Resources
-
-After installation, you can either check the [notebook tutorials](https://docs.gempy.org/getting_started/get_started.html#sphx-glr-getting-started-get-started-py) 
-or the [video introduction](https://www.youtube.com/watch?v=n0btC5Zilyc) to get started.
-
-Go to the [documentation site](http://docs.gempy.org/) for further information and enjoy the [tutorials and examples](https://www.gempy.org/tutorials).
-
-For questions and support, please use [discussions](https://github.com/cgre-aachen/gempy/discussions).
-
-If you find a bug or have a feature request, create an [issue](https://github.com/cgre-aachen/gempy/issues).
-
-Follow these [guidelines](https://github.com/cgre-aachen/gempy/blob/WIP_readme-update-march21/CONTRIBUTING.md) to contribute to GemPy.
-
-<a name="ref"></a>
-## References 
-
-* de la Varga, M., Schaaf, A., and Wellmann, F. (2019). [GemPy 1.0: open-source stochastic geological modeling and inversion](https://gmd.copernicus.org/articles/12/1/2019/gmd-12-1-2019.pdf), Geosci. Model Dev., 12, 1-32.
-* Wellmann, F., & Caumon, G. (2018). [3-D Structural geological models: Concepts, methods, and uncertainties.](https://hal.univ-lorraine.fr/hal-01921494/file/structural_models_for_geophysicsHAL.pdf) In Advances in Geophysics (Vol. 59, pp. 1-121). Elsevier.
-* Calcagno, P., Chilès, J. P., Courrioux, G., & Guillen, A. (2008). [Geological modelling from field data and geological knowledge: Part I. Modelling method coupling 3D potential-field interpolation and geological rules](https://www.sciencedirect.com/science/article/abs/pii/S0031920108001258). Physics of the Earth and Planetary Interiors, 171(1-4), 147-157.
-* Lajaunie, C., Courrioux, G., & Manuel, L. (1997). [Foliation fields and 3D cartography in geology: principles of a method based on potential interpolation](https://link.springer.com/article/10.1007/BF02775087). Mathematical Geology, 29(4), 571-584.
-
-## Publications using GemPy
-
-
-* Schaaf, A., de la Varga, M., Wellmann, F., & Bond, C. E. (2021). [Constraining stochastic 3-D structural geological models with topology information using approximate Bayesian computation in GemPy 2.1](https://gmd.copernicus.org/articles/14/3899/2021/gmd-14-3899-2021.html). Geosci. Model Dev., 14(6), 3899-3913. doi:10.5194/gmd-14-3899-2021
-* Güdük, N., de la Varga, M. Kaukolinna, J. and Wellmann, F. (2021). [Model-Based Probabilistic Inversion Using Magnetic Data: A Case Study on the Kevitsa Deposit](https://www.mdpi.com/2076-3263/11/4/150), _Geosciences_, 11(4):150. https://doi.org/10.3390/geosciences11040150.
-* Stamm, F. A., de la Varga, M., and Wellmann, F. (2019). [Actors, actions, and uncertainties: optimizing decision-making based on 3-D structural geological models](https://se.copernicus.org/articles/10/2015/2019/se-10-2015-2019.html), Solid Earth, 10, 2015–2043.
-* Wellmann, F., Schaaf, A., de la Varga, M., & von Hagke, C. (2019). [From Google Earth to 3D Geology Problem 2: Seeing Below the Surface of the Digital Earth](
-https://www.sciencedirect.com/science/article/pii/B9780128140482000156).
-In Developments in Structural Geology and Tectonics (Vol. 5, pp. 189-204). Elsevier.
-
-A continuously growing list of gempy-applications (e.g. listing real-world models) can be found [here](https://hackmd.io/@Japhiolite/B1juPvCxc).
-
-## Gallery
-
-### Geometries
-
-<p>
-<table>
-<tr>
-
-  <td>
-  <a href="https://docs.gempy.org/examples/geometries/1_horizontal_stratigraphic.html#sphx-glr-examples-geometries-1-horizontal-stratigraphic-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model1_nodata.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/examples/geometries/2_fold.html#sphx-glr-examples-geometries-2-fold-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model2_nodata.png" width="300" />
-  </a>
-  </td>
-  
-   <td>
-  <a href="https://docs.gempy.org/examples/geometries/3_recumbent_fold.html#sphx-glr-examples-geometries-3-recumbent-fold-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model3_nodata.png" width="300" />
-  </a>
-  </td>
-
-</tr>
-<tr>
-
-  <td>
-  <a href="https://docs.gempy.org/examples/geometries/4_pinchout.html#sphx-glr-examples-geometries-4-pinchout-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model4_nodata.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/examples/geometries/5_fault.html#sphx-glr-examples-geometries-5-fault-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model5_nodata.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/examples/geometries/6_unconformity.html#sphx-glr-examples-geometries-6-unconformity-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model6_nodata.png" width="300" />
-  </a>
-  </td>
-
-</tr>
-</table>
-</p>
-
-### Features
-
-<p>
-<table>
-<tr>
-
-  <td>
-  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_3b_cross_sections.html#sphx-glr-tutorials-ch1-fundamentals-ch1-3b-cross-sections-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/sectiontest.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_7_3d_visualization.html#sphx-glr-tutorials-ch1-fundamentals-ch1-7-3d-visualization-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/data_vis.png" width="300" />
-  </a>
-  </td>
-  
-   <td>
-  <a href="https://docs.gempy.org/examples/geometries/7_combination.html#sphx-glr-examples-geometries-7-combination-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/scalarfield.png" width="300" />
-  </a>
-  </td>
-
-</tr>
-<tr>
-
-  <td>
-  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_3b_cross_sections.html#sphx-glr-tutorials-ch1-fundamentals-ch1-3b-cross-sections-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/geomap.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/tutorials/ch4-Topology/ch4-1-Topology.html#sphx-glr-tutorials-ch4-topology-ch4-1-topology-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/topology.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/tutorials/ch4-Topology/ch4-1-Topology.html#sphx-glr-tutorials-ch4-topology-ch4-1-topology-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/topology_matrix.png" width="300" />
-  </a>
-  </td>
-
-</tr>
-</table>
-</p>
-
-
-### Case studies
-
-<p>
-<table>
-<tr>
-
-  <td>
-  <a href="https://docs.gempy.org/examples/real/Alesmodel.html#sphx-glr-examples-real-alesmodel-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/alesmodel.png" width="300" />
-  </a>
-  </td>
-  
-  <td>
-  <a href="https://docs.gempy.org/examples/real/Perth_basin.html#sphx-glr-examples-real-perth-basin-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/perthmodel.png" width="300" />
-  </a>
-  </td>
-  
-   <td>
-  <a href="https://docs.gempy.org/examples/real/Greenstone.html#sphx-glr-examples-real-greenstone-py">
-  <img alt="colormapped image plot thumbnail" src="docs/readme_images/greenstonemodel.png" width="300" />
-  </a>
-  </td>
-
-</tr>
-</table>
-</p>
+# <p align="center"><img src="docs/readme_images/header_combined_slim.png" width="1000"></p>
+
+> Open-source, implicit 3D structural geological modeling in Python.
+
+[![PyPI](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31013/)
+[![PyPI](https://img.shields.io/badge/pypi-1.0-blue.svg)](https://pypi.org/project/gempy/)
+[![license: EUPL v1.2](https://img.shields.io/badge/license-EUPL%20v1.2-blue.svg)](https://github.com/cgre-aachen/gempy/blob/master/LICENSE)
+[![Documentation Status](https://assets.readthedocs.org/static/projects/badges/passing-flat.svg)](http://docs.gempy.org)
+[![DOI](https://zenodo.org/badge/96211155.svg)](https://zenodo.org/badge/latestdoi/96211155)
+
+## What's New: GemPy v3 Pre-release!
+
+GemPy v3 is gearing up for its official launch. Our team is diligently working on refining the documentation and adding the final touches. Delve into the exciting new features in the [What's New in GemPy v3](WhatsNewGemPy3.md). Experience GemPy v3 firsthand by installing the pre-release version from PyPi:
+
+`$ pip install gempy --pre`
+
+In the meantime, you can explore the updated documentation [here](https://gempy-project.github.io/temp_gp3_docs/).
+
+## Overview
+
+[GemPy](https://www.gempy.org/) is a Python-based, **open-source geomodeling library**. It is
+capable of constructing complex **3D geological models** of folded
+structures, fault networks and unconformities, based on the underlying
+powerful **implicit representation** approach. 
+
+## Installation
+
+We provide the latest release version of GemPy via PyPi package services. We highly recommend using PyPi,
+
+`$ pip install gempy`
+
+
+## Requirements
+
+The following versions are required/strongly recommended for the main dependencies of GemPy (as of June 2023):
+- python <= 3.10 (required by aesara)
+- numpy
+ 
+## Resources
+
+After installation, you can either check the [notebook tutorials](https://docs.gempy.org/getting_started/get_started.html#sphx-glr-getting-started-get-started-py) 
+or the [video introduction](https://www.youtube.com/watch?v=n0btC5Zilyc) to get started.
+
+Go to the [documentation site](http://docs.gempy.org/) for further information and enjoy the [tutorials and examples](https://www.gempy.org/tutorials).
+
+For questions and support, please use [discussions](https://github.com/cgre-aachen/gempy/discussions).
+
+If you find a bug or have a feature request, create an [issue](https://github.com/cgre-aachen/gempy/issues).
+
+Follow these [guidelines](https://github.com/cgre-aachen/gempy/blob/WIP_readme-update-march21/CONTRIBUTING.md) to contribute to GemPy.
+
+<a name="ref"></a>
+## References 
+
+* de la Varga, M., Schaaf, A., and Wellmann, F. (2019). [GemPy 1.0: open-source stochastic geological modeling and inversion](https://gmd.copernicus.org/articles/12/1/2019/gmd-12-1-2019.pdf), Geosci. Model Dev., 12, 1-32.
+* Wellmann, F., & Caumon, G. (2018). [3-D Structural geological models: Concepts, methods, and uncertainties.](https://hal.univ-lorraine.fr/hal-01921494/file/structural_models_for_geophysicsHAL.pdf) In Advances in Geophysics (Vol. 59, pp. 1-121). Elsevier.
+* Calcagno, P., Chilès, J. P., Courrioux, G., & Guillen, A. (2008). [Geological modelling from field data and geological knowledge: Part I. Modelling method coupling 3D potential-field interpolation and geological rules](https://www.sciencedirect.com/science/article/abs/pii/S0031920108001258). Physics of the Earth and Planetary Interiors, 171(1-4), 147-157.
+* Lajaunie, C., Courrioux, G., & Manuel, L. (1997). [Foliation fields and 3D cartography in geology: principles of a method based on potential interpolation](https://link.springer.com/article/10.1007/BF02775087). Mathematical Geology, 29(4), 571-584.
+
+## Publications using GemPy
+
+
+
+* Brisson, S., Wellmann, F., Chudalla, N., von Harten, J., & von Hagke, C. (2023). [Estimating uncertainties in 3-D models of complex fold-and-thrust belts: A case study of the Eastern Alps triangle zone](https://www.sciencedirect.com/science/article/pii/S2590197423000046). Applied Computing and Geosciences, 18, 100115.
+
+* Liang, Z., de la Varga, M., & Wellmann, F. (2023). [Kernel method for gravity forward simulation in implicit probabilistic geologic modeling](https://pubs.geoscienceworld.org/geophysics/article/88/3/G43/621596/Kernel-method-for-gravity-forward-simulation-in?casa_token=VjCR7rYOkKoAAAAA:W81L1AXgW_j9GiYPciBvLIdL8Zo66IzYVYiU6Ri8xLgIjbzTmpcDE74rzmAwnokX_71_XKg). Geophysics, 88(3), G43-G55.
+
+* Kong, S., Oh, J., Yoon, D., Ryu, D. W., & Kwon, H. S. (2023). [Integrating Deep Learning and Deterministic Inversion for Enhancing Fault Detection in Electrical Resistivity Surveys](https://www.mdpi.com/2076-3417/13/10/6250). Applied Sciences, 13(10), 6250.
+
+* Thomas, A. T., Micallef, A., Duan, S., & Zou, Z. (2023). [Characteristics and controls of an offshore freshened groundwater system in the Shengsi region, East China Sea](https://www.frontiersin.org/articles/10.3389/feart.2023.1198215/full). Frontiers in Earth Science, 11, 1198215.
+
+* Haehnel, P., Freund, H., Greskowiak, J. & Massmann, G. (2023) [Development of a three-dimensional hydrogeological model for the island of Norderney (Germany) using GemPy](https://doi.org/10.1002/gdj3.208). Geoscience Data Journal, 00, 1–17. 
+
+* Jüstel, A., de la Varga, M., Chudalla, N., Wagner, J. D., Back, S., & Wellmann, F. (2023). [From Maps to Models-Tutorials for structural geological modeling using GemPy and GemGIS](https://jose.theoj.org/papers/10.21105/jose.00185). Journal of Open Source Education, 6(66), 185.
+
+* Sehsah, H., Eldosouky, A. M., & Pham, L. T. (2022). [Incremental Emplacement of the Sierra Nevada Batholith Constrained by U-Pb Ages and Potential Field Data](https://www.journals.uchicago.edu/doi/full/10.1086/722724?casa_token=pkl8XXrtyokAAAAA:YeIh1t-qwt6AT8yz_vTj4OQapaR1_nZUjS3Az_77VZXlpyfGu0cN5DSzrz6NNjoj4Qv5iud4rdc). The Journal of Geology, 130(5), 381-391.
+
+* Schaaf, A., de la Varga, M., Wellmann, F., & Bond, C. E. (2021). [Constraining stochastic 3-D structural geological models with topology information using approximate Bayesian computation in GemPy 2.1](https://gmd.copernicus.org/articles/14/3899/2021/gmd-14-3899-2021.html). Geosci. Model Dev., 14(6), 3899-3913. doi:10.5194/gmd-14-3899-2021
+* Güdük, N., de la Varga, M. Kaukolinna, J. and Wellmann, F. (2021). [Model-Based Probabilistic Inversion Using Magnetic Data: A Case Study on the Kevitsa Deposit](https://www.mdpi.com/2076-3263/11/4/150), _Geosciences_, 11(4):150. https://doi.org/10.3390/geosciences11040150.
+
+* Wu, J., & Sun, B. (2021). [Discontinuous mechanical analysis of manifold element strain of rock slope based on open source Gempy](https://www.e3s-conferences.org/articles/e3sconf/abs/2021/24/e3sconf_caes2021_03084/e3sconf_caes2021_03084.html). In E3S Web of Conferences (Vol. 248, p. 03084). EDP Sciences.
+
+* Stamm, F. A., de la Varga, M., and Wellmann, F. (2019). [Actors, actions, and uncertainties: optimizing decision-making based on 3-D structural geological models](https://se.copernicus.org/articles/10/2015/2019/se-10-2015-2019.html), Solid Earth, 10, 2015–2043.
+* Wellmann, F., Schaaf, A., de la Varga, M., & von Hagke, C. (2019). [From Google Earth to 3D Geology Problem 2: Seeing Below the Surface of the Digital Earth](
+https://www.sciencedirect.com/science/article/pii/B9780128140482000156).
+In Developments in Structural Geology and Tectonics (Vol. 5, pp. 189-204). Elsevier.
+
+Please let us know if your publication is missing!
+
+A continuously growing list of gempy-applications (e.g. listing real-world models) can be found [here](https://hackmd.io/@Japhiolite/B1juPvCxc).
+
+## Gallery
+
+### Geometries
+
+<p>
+<table>
+<tr>
+
+  <td>
+  <a href="https://docs.gempy.org/examples/geometries/1_horizontal_stratigraphic.html#sphx-glr-examples-geometries-1-horizontal-stratigraphic-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model1_nodata.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/examples/geometries/2_fold.html#sphx-glr-examples-geometries-2-fold-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model2_nodata.png" width="300" />
+  </a>
+  </td>
+  
+   <td>
+  <a href="https://docs.gempy.org/examples/geometries/3_recumbent_fold.html#sphx-glr-examples-geometries-3-recumbent-fold-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model3_nodata.png" width="300" />
+  </a>
+  </td>
+
+</tr>
+<tr>
+
+  <td>
+  <a href="https://docs.gempy.org/examples/geometries/4_pinchout.html#sphx-glr-examples-geometries-4-pinchout-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model4_nodata.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/examples/geometries/5_fault.html#sphx-glr-examples-geometries-5-fault-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model5_nodata.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/examples/geometries/6_unconformity.html#sphx-glr-examples-geometries-6-unconformity-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/model6_nodata.png" width="300" />
+  </a>
+  </td>
+
+</tr>
+</table>
+</p>
+
+### Features
+
+<p>
+<table>
+<tr>
+
+  <td>
+  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_3b_cross_sections.html#sphx-glr-tutorials-ch1-fundamentals-ch1-3b-cross-sections-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/sectiontest.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_7_3d_visualization.html#sphx-glr-tutorials-ch1-fundamentals-ch1-7-3d-visualization-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/data_vis.png" width="300" />
+  </a>
+  </td>
+  
+   <td>
+  <a href="https://docs.gempy.org/examples/geometries/7_combination.html#sphx-glr-examples-geometries-7-combination-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/scalarfield.png" width="300" />
+  </a>
+  </td>
+
+</tr>
+<tr>
+
+  <td>
+  <a href="https://docs.gempy.org/tutorials/ch1_fundamentals/ch1_3b_cross_sections.html#sphx-glr-tutorials-ch1-fundamentals-ch1-3b-cross-sections-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/geomap.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/tutorials/ch4-Topology/ch4-1-Topology.html#sphx-glr-tutorials-ch4-topology-ch4-1-topology-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/topology.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/tutorials/ch4-Topology/ch4-1-Topology.html#sphx-glr-tutorials-ch4-topology-ch4-1-topology-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/topology_matrix.png" width="300" />
+  </a>
+  </td>
+
+</tr>
+</table>
+</p>
+
+
+### Case studies
+
+<p>
+<table>
+<tr>
+
+  <td>
+  <a href="https://docs.gempy.org/examples/real/Alesmodel.html#sphx-glr-examples-real-alesmodel-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/alesmodel.png" width="300" />
+  </a>
+  </td>
+  
+  <td>
+  <a href="https://docs.gempy.org/examples/real/Perth_basin.html#sphx-glr-examples-real-perth-basin-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/perthmodel.png" width="300" />
+  </a>
+  </td>
+  
+   <td>
+  <a href="https://docs.gempy.org/examples/real/Greenstone.html#sphx-glr-examples-real-greenstone-py">
+  <img alt="colormapped image plot thumbnail" src="docs/readme_images/greenstonemodel.png" width="300" />
+  </a>
+  </td>
+
+</tr>
+</table>
+</p>
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/a01_horizontal_stratigraphic.py` & `gempy-2023.2.0b1/examples/examples/geometries/a01_horizontal_stratigraphic.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Generate the model
 # Define the path to data
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 # Create a GeoModel instance
 data = gp.create_geomodel(
     project_name='horizontal',
     extent=[0, 1000, 0, 1000, 0, 1000],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
         path_to_orientations=data_path + "/data/input_data/jan_models/model1_orientations.csv",
         path_to_surface_points=data_path + "/data/input_data/jan_models/model1_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/b02_fold.py` & `gempy-2023.2.0b1/examples/examples/geometries/f06_unconformity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """
-Model 2 - Anticline
-===================
+Model 6 - Unconformity
+======================
 
-This script demonstrates how to create a geological model of an anticline structure using GemPy,
-a Python-based, open-source library for implicit geological modeling.
+This script creates an unconformity cutting an anticline structure using GemPy,
+an open-source, Python-based library for building implicit geological models.
 """
 
-# Import necessary libraries
+# Importing necessary libraries
 import gempy as gp
 import gempy_viewer as gpv
-
+from gempy_engine.core.data.stack_relation_type import StackRelationType
 
 # sphinx_gallery_thumbnail_number = 2
 
 
 # %%
 # Generate the model
 # Define the path to data
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 path_to_data = data_path + "/data/input_data/jan_models/"
 # Create a GeoModel instance
-data: gp.data.GeoModel = gp.create_geomodel(
-    project_name='fold',
+data = gp.create_geomodel(
+    project_name='unconformity',
     extent=[0, 1000, 0, 1000, 0, 1000],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
-        path_to_orientations=path_to_data + "model2_orientations.csv",
-        path_to_surface_points=path_to_data + "model2_surface_points.csv"
+        path_to_orientations=path_to_data + "model6_orientations.csv",
+        path_to_surface_points=path_to_data + "model6_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
     gempy_model=data,
-    mapping_object={"Strat_Series": ('rock2', 'rock1')}
+    mapping_object={
+        "Strat_Series1": 'rock3',
+        "Strat_Series2": ('rock2', 'rock1')
+    }
 )
+# Define the structural relation
+data.structural_frame.structural_groups[0].structural_relation = StackRelationType.ERODE
+
 # Compute the geological model
 gp.compute_model(data)
 geo_data = data
 
 # %%
-# Plot the initial geological model in the y direction without results
+# Plot the initial geological model in the y direction
 gpv.plot_2d(geo_data, direction=['y'], show_results=False)
 
-# Plot the result of the model in the y and x direction with data and scalar
-gpv.plot_2d(geo_data, direction='y', show_data=True, show_scalar=False)
-gpv.plot_2d(geo_data, direction='x', show_data=True, show_scalar=True)
+# %%
+# Plot the result of the model in the y and x directions with data
+gpv.plot_2d(geo_data, direction='y', show_data=True)
+gpv.plot_2d(geo_data, direction='x', show_data=True)
+
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/c03_recumbent_fold.py` & `gempy-2023.2.0b1/examples/examples/geometries/c03_recumbent_fold.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 path_to_data = data_path + "/data/input_data/jan_models/"
 # Create a GeoModel instance
 data = gp.create_geomodel(
     project_name='recumbent',
     extent=[0, 1000, 0, 1000, 0, 1000],
     resolution=[50, 50, 50],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
         path_to_orientations=path_to_data + "model3_orientations.csv",
         path_to_surface_points=path_to_data + "model3_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/d04_pinchout.py` & `gempy-2023.2.0b1/examples/examples/geometries/b02_fold.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 """
-Model 4 - Pinchout
-==================
+Model 2 - Anticline
+===================
 
-This script demonstrates how to create a geological model with a layer of varying thickness (pinchout) using GemPy,
+This script demonstrates how to create a geological model of an anticline structure using GemPy,
 a Python-based, open-source library for implicit geological modeling.
 """
 
 # Import necessary libraries
 import gempy as gp
 import gempy_viewer as gpv
 
 
-# sphinx_gallery_thumbnail_number = 3
+# sphinx_gallery_thumbnail_number = 2
 
 
 # %%
 # Generate the model
 # Define the path to data
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 path_to_data = data_path + "/data/input_data/jan_models/"
 # Create a GeoModel instance
-data = gp.create_geomodel(
-    project_name='pinchout',
+data: gp.data.GeoModel = gp.create_geomodel(
+    project_name='fold',
     extent=[0, 1000, 0, 1000, 0, 1000],
-    resolution=[50, 50, 50],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
-        path_to_orientations=path_to_data + "model4_orientations.csv",
-        path_to_surface_points=path_to_data + "model4_surface_points.csv"
+        path_to_orientations=path_to_data + "model2_orientations.csv",
+        path_to_surface_points=path_to_data + "model2_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
     gempy_model=data,
     mapping_object={"Strat_Series": ('rock2', 'rock1')}
 )
 # Compute the geological model
 gp.compute_model(data)
 geo_data = data
 
 # %%
-# Plot the initial geological model in the y direction
+# Plot the initial geological model in the y direction without results
 gpv.plot_2d(geo_data, direction=['y'], show_results=False)
 
-# Plot the result of the model in the x and y direction with data
-gpv.plot_2d(geo_data, direction=['x'], show_data=True)
-gpv.plot_2d(geo_data, direction=['y'], show_data=True)
-
-# %%
-gpv.plot_3d(geo_data, show_surfaces=True)
+# Plot the result of the model in the y and x direction with data and scalar
+gpv.plot_2d(geo_data, direction='y', show_data=True, show_scalar=False)
+gpv.plot_2d(geo_data, direction='x', show_data=True, show_scalar=True)
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/e05_fault.py` & `gempy-2023.2.0b1/examples/examples/geometries/e05_fault.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Define the path to data
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 path_to_data = data_path + "/data/input_data/jan_models/"
 # Create a GeoModel instance
 data = gp.create_geomodel(
     project_name='fault',
     extent=[0, 1000, 0, 1000, 0, 1000],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
         path_to_orientations=path_to_data + "model5_orientations.csv",
         path_to_surface_points=path_to_data + "model5_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/f06_unconformity.py` & `gempy-2023.2.0b1/examples/examples/geometries/g07_combination.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 """
-Model 6 - Unconformity
+Model 7 - Combination
 ======================
 
-This script creates an unconformity cutting an anticline structure using GemPy,
+This script creates a folded domain featuring an unconformity and a fault using GemPy,
 an open-source, Python-based library for building implicit geological models.
 """
 
 # Importing necessary libraries
+import numpy as np
 import gempy as gp
 import gempy_viewer as gpv
 from gempy_engine.core.data.stack_relation_type import StackRelationType
 
 # sphinx_gallery_thumbnail_number = 2
 
-
-# %%
 # Generate the model
 # Define the path to data
 data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
 path_to_data = data_path + "/data/input_data/jan_models/"
 # Create a GeoModel instance
 data = gp.create_geomodel(
-    project_name='unconformity',
-    extent=[0, 1000, 0, 1000, 0, 1000],
-    number_octree_levels=6,
+    project_name='combination',
+    extent=[0, 2500, 0, 1000, 0, 1000],
+    refinement=6,
+    resolution=[20, 20, 20],
     importer_helper=gp.data.ImporterHelper(
-        path_to_orientations=path_to_data + "model6_orientations.csv",
-        path_to_surface_points=path_to_data + "model6_surface_points.csv"
+        path_to_orientations=path_to_data + "model7_orientations.csv",
+        path_to_surface_points=path_to_data + "model7_surface_points.csv"
     )
 )
 # Map geological series to surfaces
 gp.map_stack_to_surfaces(
     gempy_model=data,
     mapping_object={
-        "Strat_Series1": 'rock3',
-        "Strat_Series2": ('rock2', 'rock1')
+        "Fault_Series" : ('fault'),
+        "Strat_Series1": ('rock3'),
+        "Strat_Series2": ('rock2', 'rock1'),
     }
 )
 # Define the structural relation
-data.structural_frame.structural_groups[0].structural_relation = StackRelationType.ERODE
-
+data.structural_frame.structural_groups[0].structural_relation = StackRelationType.FAULT
+data.structural_frame.fault_relations = np.array(
+    [[0, 1, 1],
+     [0, 0, 0],
+     [0, 0, 0]]
+)
 # Compute the geological model
+data.interpolation_options.number_octree_levels_surface = 5
 gp.compute_model(data)
-geo_data = data
+data.structural_frame
 
 # %%
 # Plot the initial geological model in the y direction
-gpv.plot_2d(geo_data, direction=['y'], show_results=False)
+gpv.plot_2d(data, direction=['y'], show_results=False)
 
 # %%
-# Plot the result of the model in the y and x directions with data
-gpv.plot_2d(geo_data, direction='y', show_data=True)
-gpv.plot_2d(geo_data, direction='x', show_data=True)
+# Plot the result of the model in the y and x directions with data and boundaries
+gpv.plot_2d(data, direction='y', show_data=True, show_boundaries=True)
+gpv.plot_2d(data, direction='x', show_data=True)
+
+# Plot the blocks accounting for fault blocks
+gpv.plot_2d(
+    model=data,
+    override_regular_grid=data.solutions.raw_arrays.litho_faults_block,
+    show_data=True, kwargs_lithology={'cmap': 'Set1', 'norm': None}
+)
 
+# %%
+# The 3D plot is commented out due to a bug.
+gpv.plot_3d(data)
```

### Comparing `gempy-2023.1.0b6/examples/examples/geometries/foo/more_examples.py` & `gempy-2023.2.0b1/examples/examples/geometries/h08_more_examples.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 -----------------------------------------
 
 """
 
 # %%
 # Importing gempy
 import gempy as gp
+import gempy_viewer as gpv
 
 # Aux imports
 import numpy as np
-import pandas as pn
-import matplotlib
-import aesara
+import os
 
 # %%
 # Choose a model and load the corresponding data set in the line below
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 # 
 # Model 1: Discordant layering
 # 
@@ -32,110 +31,112 @@
 # 
 # Model 8: Similar to Model 5
 # 
 # Model 9: Parallel flat dipping layers
 # 
 
 # %%
-data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
+
+data_path = os.path.abspath('../..')
 
 
 # %%
-def create_example(name_model, interpolator=None, save_pickle=False, plot_section=True):
+def create_example(name_model, plot_section=True):
     """
     Create an inter_data from one of the examples data_set
     
     Attr:
         name_model (str): name of the model that you want to generate. It has to be in ['Model 1' ,'Model 2', 'Model 3', 'Model 4','Model 5' 'Model 6','Model 7',
                           'Model 8', 'Model 9']
         save_pickle (bool, str): Save to a pickle the interp_data object. You can pass the path as a string otherwse
                                 the default name will be given
         plot_section (bool)
     
     """
-    name_list = np.array(['Model 1', 'Model 2', 'Model 3', 'Model 4', 'Model 5', 'Model 6', 'Model 7',
-                          'Model 8', 'Model 9'])
+    name_list = np.array(['Model 1', 'Model 2', 'Model 3', 'Model 4', 'Model 5', 'Model 6', 'Model 7', 'Model 8', 'Model 9'])
     assert name_model in name_list, 'Name model must be in the following list: ' + str(name_list)
     # Extract number of the model
     n_model = name_model[-1]
 
-    # Load right gempy geodata
-    geo_data = gp.create_data_legacy(name_model, extent=[0, 2000, 0, 2000, 0, 1600], resolution=[50, 50, 50],
-                                     path_o=data_path + "/data/input_data/lisa_models/foliations" + n_model + ".csv",
-                                     path_i=data_path + "/data/input_data/lisa_models/interfaces" + n_model + ".csv")
+    # # Load right gempy geodata
+    geo_data: gp.data.GeoModel = gp.create_geomodel(
+        project_name=name_model,
+        extent=[0, 2000, 0, 2000, 0, 1600],
+        resolution=[50, 50, 50],
+        refinement=6,  # * For this model is better not to use octrees because we want to see what is happening in the scalar fields
+        importer_helper=gp.data.ImporterHelper(
+            path_to_orientations=data_path + "/data/input_data/lisa_models/foliations" + n_model + ".csv",
+            path_to_surface_points=data_path + "/data/input_data/lisa_models/interfaces" + n_model + ".csv",
+        )
+    )
 
     # Set the right sequential pile
     subset_list_1 = np.array(['Model 1'])
     subset_list_2 = np.array(['Model 5', 'Model 8'])
     subset_list_3 = np.array(['Model 2', 'Model 3', 'Model 9', 'Model 6'])
     subset_list_4 = np.array(['Model 7'])
+    
     ### Model 1 - Discordant layering ###
     if name_model in subset_list_1:
-        gp.map_series_to_surfaces(geo_data, {"Strat_Series_1": ('Sandstone', 'Siltstone', 'Shale'),
-                                             "Strat_Series_2": ('Sandstone2', 'Siltstone2', 'Shale2')},
-                                  )
+        gp.map_stack_to_surfaces(
+            gempy_model=geo_data,
+            mapping_object={
+                "Strat_Series_1": ('Sandstone', 'Siltstone', 'Shale'),
+                "Strat_Series_2": ('Sandstone2', 'Siltstone2', 'Shale2')
+            },
+        )
     ### Model 5 - One normal Fault ###
     ### Model 8 - ###
     elif name_model in subset_list_2:
-        gp.map_series_to_surfaces(geo_data, {"Fault_Series": 'Main_Fault',
-                                             "Strat_Series": (
-                                             'Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')},
-                                  )
-        geo_data.set_is_fault(['Fault_Series'])
+        gp.map_stack_to_surfaces(
+            gempy_model=geo_data,
+            mapping_object={
+            "Fault_Series": 'Main_Fault',
+            "Strat_Series": ('Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')
+            },
+        )
+        
+        gp.set_is_fault(geo_data, ['Fault_Series'])
+        
     elif name_model in subset_list_3:
         ### Model 2 - Aufwölbung (durch Salzstock?) ###
         ### Model 3+9 - Parallele NNE Schichtung ohne Verwerfung ###
         ### Model 6 - Mulde ###
-        gp.map_series_to_surfaces(geo_data, {
-            "Strat_Series": ('Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')},
-                                  )
-
+        gp.map_stack_to_surfaces(
+            gempy_model=geo_data,
+            mapping_object={
+            "Strat_Series": ('Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')
+            },
+        )
     elif name_model in subset_list_4:
         ### Model 7 - Graben ###
-        gp.map_series_to_surfaces(geo_data, {"Fault_1": 'Fault_1', "Fault_2": 'Fault_2',
-                                             "Strat_Series": (
-                                             'Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')},
-                                  )
-        geo_data.set_is_fault(['Fault_1', 'Fault_2'])
-
+        gp.map_stack_to_surfaces(
+            gempy_model=geo_data,
+            mapping_object={
+            "Fault_1": 'Fault_1', "Fault_2": 'Fault_2',
+            "Strat_Series": ('Sandstone', 'Siltstone', 'Shale', 'Sandstone_2', 'Schist', 'Gneiss')
+            },
+        )
+        
+        gp.set_is_fault(geo_data, ['Fault_1', 'Fault_2'])
     else:
         print('You would never reach this point. Look for the bug')
 
     # Interpolation and Computation
-    if interpolator is None:
-        interp_data = gp.set_interpolator(geo_data, aesara_optimizer='fast_run')
-    else:
-        interp_data = interpolator
-        geo_data.set_aesara_function(interpolator)
-    sol = gp.compute_model(geo_data)
+    sol = gp.compute_model(
+        gempy_model=geo_data,
+        engine_config=gp.data.GemPyEngineConfig(backend=gp.data.AvailableBackends.PYTORCH)
+    )
 
     if plot_section is True:
         # 2D Plot
-        gp.plot_2d(geo_data, cell_number=25,
-                             direction='y', show_data=True)
-        gp.plot_3d(geo_data, image=True)
-
-    if save_pickle is not False:
-        if type(save_pickle) is str:
-            gp.save_model_to_pickle(geo_data, save_pickle)
-        else:
-            gp.save_model_to_pickle(geo_data, 'lisa-' + str(n_model))
-
-    gp.save_model(geo_data)
-
-    return interp_data
-
-
-# %% 
-def generate_all_models(list_of_models):
-    for e, n in enumerate(list_of_models):
-        if e == 0:
-            interp = create_example(n, None, save_pickle=False, plot_section=True)
-        else:
-            create_example(n, interp, save_pickle=False, plot_section=True)
+        gpv.plot_2d(geo_data, cell_number=['mid'], direction='y', show_data=True)
+        gpv.plot_3d(geo_data, image=False)
+
+    return geo_data.structural_frame
 
 
 # %%
 # Discordant layering 1
 # =====================
 
 create_example('Model 1')
@@ -178,13 +179,12 @@
 
 # %%
 # Horizontal tilted
 # =================
 
 create_example('Model 9')
 
-
 # %%
 
 # generate_all_models(['Model 1', 'Model 2', 'Model 3',
 #                     'Model 5', 'Model 6', 'Model 7',
 #                     'Model 8', 'Model 9'])
```

### Comparing `gempy-2023.1.0b6/examples/examples/real/Alesmodel.py` & `gempy-2023.2.0b1/examples/examples/real/Alesmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 path_dem = data_path + "/data/input_data/AlesModel/_cropped_DEM_coarse.tif"
 
 # %% 
 geo_model: gp.data.GeoModel = gp.create_geomodel(
     project_name='Claudius',
     extent=[729550.0, 751500.0, 1913500.0, 1923650.0, -1800.0, 800.0],
     resolution=[100, 100, 100],
-    number_octree_levels=6,
+    refinement=6,
     importer_helper=gp.data.ImporterHelper(
         path_to_orientations=path_orient,
         path_to_surface_points=path_interf,
     )
 )
 
 # %% 
@@ -98,15 +98,15 @@
 # ~~~~~~~~~~
 # 
 
 # %% 
 gp.set_topography_from_file(
     grid=geo_model.grid,
     filepath=path_dem,
-    crop_to_extent=[729550.0, 751500.0, 1913500.0, 1923650.0]
+    crop_to_extent=[729550.0, 751500.0, 1_913_500.0, 1923650.0]
 )
 
 
 gpv.plot_3d(geo_model, show_topography=True, ve=1, image=True)
 
 # %%
 carbo = geo_model.structural_frame.get_group_by_name("Carbon_Series")
@@ -136,9 +136,9 @@
 gpv.plot_2d(geo_model, show_topography=False, section_names=['topography'], show_lith=True)
 
 # %% 
 gpv.plot_2d(geo_model, cell_number=[4], direction=['y'], show_topography=True, show_data=True)
 gpv.plot_2d(geo_model, cell_number=[-4], direction=['y'], show_topography=True, show_data=True)
 
 # %%
-# sphinx_gallery_thumbnail_number = 5
-gpv.plot_3d(geo_model, show_lith=True, show_topography=False, kwargs_plot_structured_grid={'opacity': 0.5})
+# sphinx_gallery_thumbnail_number = -1
+gpv.plot_3d(geo_model, show_lith=True, show_topography=True, kwargs_plot_structured_grid={'opacity': 0.8})
```

### Comparing `gempy-2023.1.0b6/examples/examples/real/Claudius.py` & `gempy-2023.2.0b1/examples/examples/real/Claudius.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # we can directly tidy the data in gempy style:
 # 
 
 # %% 
 
 data_path = os.path.abspath('../../data/input_data/Claudius')
 
-reduce_data_by = 5
+reduce_data_by = 30
 
 dfs = []
 for letter in 'ABCD':
     dfs.append(
         pn.read_csv(
             filepath_or_buffer=f"{data_path}/{letter}Points.csv",
             sep=';',
@@ -129,15 +129,15 @@
     orientations=orientations_table
 )
 
 geo_model: gp.data.GeoModel = gp.create_geomodel(
     project_name='Claudius',
     extent=[548800, 552500, 7816600, 7822000, -11010, -8400],
     resolution=[38, 55, 30],
-    number_octree_levels=1,
+    refinement=5,
     structural_frame=structural_frame
 )
 
 group_fault = gp.data.StructuralGroup(
     name='Fault1',
     elements=[geo_model.structural_frame.structural_elements.pop(-2)],
     structural_relation=gp.data.StackRelationType.FAULT,
@@ -198,16 +198,16 @@
 # We will need to separate with surface belong to each series:
 # 
 
 gp.map_stack_to_surfaces(
     gempy_model=geo_model,
     mapping_object={
         'Default series': ('0', '60', '250'),
-        'Fault'         : 'Claudius_fault',
-        'Uncomformity'  : '330',
+        'Fault': 'Claudius_fault',
+        'Uncomformity': '330',
     }
 )
 # %%
 # So far we did not specify which series/faults are actula faults:
 # 
 
 # %%
@@ -216,18 +216,25 @@
     fault_groups=[geo_model.structural_frame.get_group_by_name('Fault')]
 )
 
 geo_model.structural_frame
 
 # %%
 geo_model.interpolation_options.kernel_options.range = 1
-gp.compute_model(geo_model, gp.data.GemPyEngineConfig(use_gpu=True))
+gp.compute_model(
+    geo_model,
+    gp.data.GemPyEngineConfig(
+        backend=gp.data.AvailableBackends.numpy,
+        use_gpu=False,
+        dtype='float64'
+    )
+)
 
 # %% 
-sect = [35]
+sect = ['mid']
 
 gpv.plot_2d(geo_model, cell_number=sect, series_n=1, show_scalar=True, direction='x')
 
 # %% 
 gpv.plot_2d(geo_model, cell_number=sect, show_data=True, direction='x')
 
 # %%
```

### Comparing `gempy-2023.1.0b6/examples/examples/real/Greenstone.py` & `gempy-2023.2.0b1/examples/examples/real/Perth_basin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,117 @@
 """
-Greenstone.
-===========
+Perth basin.
+============
 """
+import os
 
-# Importing gempy
+# Importing GemPy
 import gempy as gp
+import gempy_viewer as gpv
 
-# Aux imports
-import numpy as np
-import matplotlib.pyplot as plt
-import os
+# Importing auxiliary libraries
+import matplotlib
 
-print(gp.__version__)
+matplotlib.rcParams['figure.figsize'] = (20.0, 10.0)
+os.environ["aesara_FLAGS"] = "mode=FAST_RUN,device=cuda"
 
-# %% 
-geo_model = gp.create_model('Greenstone')
+# %%
+cwd = os.getcwd()
+if 'examples' not in cwd:
+    data_path = os.getcwd() + '/examples'
+else:
+    data_path = cwd + '/../..'
+
+# %% 
+geo_model: gp.data.GeoModel = gp.create_geomodel(
+    project_name='Perth_Basin',
+    extent=[337000, 400000, 6640000, 6710000, -18000, 1000],
+    resolution=[100, 100, 100],
+    refinement=4,
+    importer_helper=gp.data.ImporterHelper(
+        path_to_orientations=data_path + "/data/input_data/perth_basin/Paper_GU2F_sc_faults_topo_Foliations.csv",
+        path_to_surface_points=data_path + "/data/input_data/perth_basin/Paper_GU2F_sc_faults_topo_Points.csv",
+    )
+)
 
 # %%
+geo_model.structural_frame
 
-data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
+# %% 
+del_surfaces = ['Cadda', 'Woodada_Kockatea', 'Cattamarra']
+for s in del_surfaces:
+    gp.remove_element_by_name(geo_model, s)
+
+geo_model.structural_frame
+
+# %% 
+gp.map_stack_to_surfaces(
+    gempy_model=geo_model,
+    mapping_object={
+        "fault_Abrolhos_Transfer": ["Abrolhos_Transfer"],
+        "fault_Coomallo": ["Coomallo"],
+        "fault_Eneabba_South": ["Eneabba_South"],
+        "fault_Hypo_fault_W": ["Hypo_fault_W"],
+        "fault_Hypo_fault_E": ["Hypo_fault_E"],
+        "fault_Urella_North": ["Urella_North"],
+        "fault_Darling": ["Darling"],
+        "fault_Urella_South": ["Urella_South"],
+        "Sedimentary_Series": ['Cretaceous', 'Yarragadee', 'Eneabba', 'Lesueur', 'Permian']
+    }
+)
 
-# Importing the data from csv files and settign extent and resolution
-geo_model = gp.init_data(geo_model, [696000, 747000, 6863000, 6930000, -20000, 200], [50, 50, 50],
-                         path_o=data_path + "/data/input_data/tut_SandStone/SandStone_Foliations.csv",
-                         path_i=data_path + "/data/input_data/tut_SandStone/SandStone_Points.csv")
+# %%
+# Select which series are faults
+# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+# 
 
-# %% 
-gp.plot_2d(geo_model, direction=['z'])
+gp.set_is_fault(
+    geo_model,
+    fault_groups=[
+        "fault_Abrolhos_Transfer",
+        "fault_Coomallo",
+        "fault_Eneabba_South",
+        "fault_Hypo_fault_W",
+        "fault_Hypo_fault_E",
+        "fault_Urella_North",
+        "fault_Darling",
+        "fault_Urella_South"
+    ],
+)
 
-# %% 
-gp.map_stack_to_surfaces(geo_model, {"EarlyGranite_Series": 'EarlyGranite',
-                                     "BIF_Series": ('SimpleMafic2', 'SimpleBIF'),
-                                     "SimpleMafic_Series": 'SimpleMafic1', 'Basement': 'basement'})
 
 # %% 
-geo_model.add_surface_values([2.61, 2.92, 3.1, 2.92, 2.61])
+# gp.set_fault_relation(geo_model, fr)
 
-# %% 
-gp.set_interpolator(geo_model,
-                    compile_aesara=True,
-                    aesara_optimizer='fast_compile',
-                    verbose=[])
+print(geo_model.structural_frame.fault_relations)
 
 # %% 
-gp.compute_model(geo_model, set_solutions=True)
+# %matplotlib inline
+gpv.plot_2d(geo_model, direction=['z'])
 
 # %% 
-gp.plot_2d(geo_model, cell_number=[-1], direction=['z'], show_data=False)
+gp.set_topography_from_random(geo_model.grid)
 
 # %% 
-gp.plot_2d(geo_model, cell_number=[25], direction='x')
+gpv.plot_3d(geo_model)
 
 # %% 
-geo_model.solutions.values_matrix
+gp.compute_model(
+    gempy_model=geo_model,
+    engine_config= gp.data.GemPyEngineConfig(
+        backend=gp.data.AvailableBackends.PYTORCH,
+        dtype="float64",
+    )
+)
 
 # %% 
-p2d = gp.plot_2d(geo_model, cell_number=[25], block=geo_model.solutions.values_matrix,
-           direction=['y'], show_data=True,
-           kwargs_regular_grid={'cmap': 'viridis', 'norm':None})
+gpv.plot_2d(geo_model, cell_number="mid")
 
-# %%
-# sphinx_gallery_thumbnail_number = 5
-gp.plot_3d(geo_model)
+# %% 
+gpv.plot_2d(geo_model, cell_number="mid", series_n=-1, show_scalar=True)
 
 # %% 
-np.save('greenstone_ver', geo_model.solutions.vertices)
-np.save('greenstone_edges', geo_model.solutions.edges)
+gpv.plot_2d(geo_model, cell_number=[12], direction=["y"], show_data=True, show_topography=True)
 
 # %%
-# Saving the model
-# ~~~~~~~~~~~~~~~~
-# 
-
-# %% 
-# gp.save_model(geo_model, path=os.pardir + '/data/gempy_models')
-gp.save_model(geo_model)
+# sphinx_gallery_thumbnail_number = 6
+gpv.plot_3d(geo_model, show_topography=True)
```

### Comparing `gempy-2023.1.0b6/examples/examples/real/Hecho.py` & `gempy-2023.2.0b1/examples/examples/real/Hecho.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,234 +1,226 @@
 """
 Hecho
 ~~~~~
 
 """
+import os
 
+import numpy as np
 # %% 
-# These two lines are necessary only if gempy is not installed
-import sys, os
-import urllib
-
-os.environ["aesara_FLAGS"] = "mode=FAST_RUN,device=cpu"
-# Importing gempy
-import gempy as gp
 
 # Aux imports
-import numpy as np
 import pandas as pn
-import matplotlib.pyplot as plt
 
+# Importing gempy
+import gempy as gp
+import gempy_viewer as gpv
 
 # %%
 # Loading surface points from repository:
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 # 
 # With pandas we can do it directly from the web and with the right args
 # we can directly tidy the data in gempy style:
 # 
 
 # %% 
+
+data_path = os.path.abspath('../../data/input_data/Hecho')
 dfs = []
-data_amount = 'Full'
 
 # First stratigraphic data
 for letter in range(1, 10):
-
-    try:
-        dfs.append(pn.read_csv('https://raw.githubusercontent.com/Loop3D/ImplicitBenchmark/master'
-                               f'/Hecho/{data_amount}/H' +
-                               str(letter) + '.csv', sep=';',
-                               names=['X', 'Y', 'Z', 'surface', '_'], header=0))
-    except urllib.error.HTTPError as e:
-        print(e, letter)
+    dfs.append(pn.read_csv(
+        filepath_or_buffer=data_path + '/H' + str(letter) + '.csv',
+        sep=';',
+        names=['X', 'Y', 'Z', 'surface', '_'],
+        header=0
+    ))
 
 # Also faults
 for f in range(1, 4):
-    fault_df = pn.read_csv('https://raw.githubusercontent.com/Loop3D/ImplicitBenchmark/master/Hecho/F' +
-                           str(f) + 'Line.csv',
-                           sep=';', names=['X', 'Y', 'Z'], header=0)
+    fault_df = pn.read_csv(
+        filepath_or_buffer=data_path + '/F' + str(f) + 'Line.csv',
+        sep=';',
+        names=['X', 'Y', 'Z'],
+        header=0
+    )
     fault_df['surface'] = 'f' + str(f)
     dfs.append(fault_df)
 
 # We put all the surfaces points together because is how gempy likes it:
 surface_points = pn.concat(dfs, sort=True)
 surface_points.reset_index(inplace=True, drop=False)
 surface_points.tail()
 
 # %%
 # Now we do the same with the orientations:
 # 
 
 # %% 
-orientations = pn.read_csv('https://raw.githubusercontent.com/Loop3D/ImplicitBenchmark/master/Hecho/Sparse/Dips.csv',
-                           sep=';',
-                           names=['X', 'Y', 'Z', 'G_x', 'G_z', '_'], header=0)
+orientations = pn.read_csv(
+    filepath_or_buffer=data_path + '/Dips.csv',
+    sep=';',
+    names=['X', 'Y', 'Z', 'G_x', 'G_z', '_'],
+    header=0
+)
 # Orientation needs to belong to a surface. This is mainly to categorize to which series belong and to
 # use the same color
 orientations['surface'] = 0
 
 # We fill the laking direction with a dummy value:
 orientations['G_y'] = 0
 
-# Drop unecesary data point
-orientations.drop([1, 3, 4], inplace=True)
-orientations
+# Replace -99999.00000 with NaN
+orientations.replace(-99999.00000, np.nan, inplace=True)
+
+# Drop irrelevant columns
+orientations.drop(columns=['_'], inplace=True)
+
+# Remove rows containing NaN
+orientations.dropna(inplace=True)
+
 
 # %%
 # Data initialization:
 # ~~~~~~~~~~~~~~~~~~~~
 # 
 # Suggested size of the axis-aligned modeling box: Origin: 0 -0.5 0
 # Maximum: 16 0.5 4.5
 # 
 # Suggested resolution: 0.05m (grid size 321 x 21 x 91)
 # 
+# %%
 
-# %% 
-geo_model = gp.create_model('Moureze')
-geo_model = gp.init_data(geo_model, extent=[0, 16, -0.5, 0.5, 0, 4.5], resolution=[321, 21, 91],
-                         surface_points_df=surface_points, orientations_df=orientations,
-                         surface_name='surface',
-                         add_basement=True)
-
-# %% 
-geo_model.orientations.df.at[5, 'surface']
-
-# %% 
-geo_model.orientations.df
+surface_points_table: gp.data.SurfacePointsTable = gp.data.SurfacePointsTable.from_arrays(
+    x=surface_points['X'].values,
+    y=surface_points['Y'].values,
+    z=surface_points['Z'].values,
+    names=surface_points['surface'].values.astype(str)
+)
+
+orientations_table: gp.data.OrientationsTable = gp.data.OrientationsTable.from_arrays(
+    x=orientations['X'].values,
+    y=orientations['Y'].values,
+    z=orientations['Z'].values,
+    G_x=orientations['G_x'].values,
+    G_y=orientations['G_y'].values,
+    G_z=orientations['G_z'].values,
+    names=orientations['surface'].values.astype(str),
+    name_id_map=surface_points_table.name_id_map  # ! Make sure that ids and names are shared
+)
+
+structural_frame: gp.data.StructuralFrame = gp.data.StructuralFrame.from_data_tables(
+    surface_points=surface_points_table,
+    orientations=orientations_table
+)
+
+geo_model: gp.data.GeoModel = gp.create_geomodel(
+    project_name='Moureze',
+    extent=[0, 16, -0.5, 0.5, 0, 4.5],
+    resolution=[321, 21, 91],
+    refinement=4,
+    structural_frame=structural_frame
+)
+
+gp.set_section_grid(
+    grid=geo_model.grid,
+    section_dict={
+        'section': ([0, 0], [16, 0], [321, 91])
+    },
+)
 
 # %%
 # We need an orientation per series/fault. The faults does not have
 # orientation so the easiest is to create an orientation from the surface
 # points availablle:
 # 
 
 # %% 
 f_names = ['f1', 'f2', 'f3']
 for fn in f_names:
-    fault_idx = geo_model.surface_points.df.index[geo_model.surface_points.df['surface'] == fn]
-    gp.set_orientation_from_surface_points(geo_model, fault_idx)
+    element = geo_model.structural_frame.get_element_by_name(fn)
+    new_orientations = gp.create_orientations_from_surface_points_coords(
+        xyz_coords=element.surface_points.xyz
+    )
+    gp.add_orientations(
+        geo_model=geo_model,
+        x=new_orientations.data['X'],
+        y=new_orientations.data['Y'],
+        z=new_orientations.data['Z'],
+        pole_vector=new_orientations.grads,
+        elements_names=fn
+    )
 
 # %%
 # Now we can see how the data looks so far:
 # 
 
 # %% 
-gp.plot_2d(geo_model)
+gpv.plot_2d(geo_model)
 
 # %%
 # By default all surfaces belong to one unique series.
 # 
 
 # %% 
-geo_model.surfaces
-
-# %% 
-geo_model.orientations.df.dtypes
+geo_model.structural_frame
 
 # %%
 # We will need to separate with surface belong to each series:
 # 
 
 # %% 
-gp.map_stack_to_surfaces(geo_model, {'Fault1': 'f1', 'Fault2': 'f2', 'Fault3': 'f3'})
+gp.map_stack_to_surfaces(
+    gempy_model=geo_model,
+    mapping_object={'Fault1': 'f1', 'Fault2': 'f2', 'Fault3': 'f3'}
+)
 
 # %%
 # However if we want the faults to offset the “Default series”, they will
 # need to be more recent (higher on the pile). We can modify the order by:
 # 
 
 # %% 
-geo_model.modify_order_series(4, 'Default series')
 
 # %%
 # Lastly, so far we did not specify which series/faults are actula faults:
 # 
 
 # %% 
-geo_model.set_is_fault(['Fault1', 'Fault2', 'Fault3'])
-
-# %%
-# Now we are good to go:
-# 
-
-# %% 
-gp.set_interpolator(geo_model, aesara_optimizer='fast_run', dtype='float64')
+gp.set_is_fault(
+    frame=geo_model,
+    fault_groups=['Fault1', 'Fault2', 'Fault3']
+)
 
 # %%
 # The default range is always the diagonal of the extent. Since in this
 # model data is very close we will need to reduce the range to 5-10% of
 # that value:
 # 
 
 # %%
-new_range = geo_model.get_additional_data().loc[('Kriging', 'range'), 'values'] * 0.2
-geo_model.modify_kriging_parameters('range', new_range)
-
-
+geo_model.interpolation_options.kernel_options.range *= 0.2
 # %% 
-gp.compute_model(geo_model, sort_surfaces=True, compute_mesh=False)
+gp.compute_model(geo_model, gp.data.GemPyEngineConfig(use_gpu=True, dtype='float64'))
 
 # %%
 # Time
 # ~~~~
 # 
 # -  GTX 2080 164 ms ± 2.03 ms per loop (mean ± std. dev. of 7 runs, 1
 #    loop each)
 # 
 
 # %% 
-gp.plot_2d(geo_model, cell_number=[10], series_n=3, show_scalar=True)
-
-# %% 
-gp.plot_2d(geo_model, cell_number=[10], show_data=True)
-
-# %%
-# sphinx_gallery_thumbnail_number = 3
-gp.plot_3d(geo_model, kwargs_plot_structured_grid={'opacity': 8})
-
-
-# %%
-# Export data:
-# ~~~~~~~~~~~~
-# 
-# The solution is stored in a numpy array of the following shape. Axis 0
-# are the scalar fields of each correspondent series/faults in the
-# following order (except basement):
-# 
-
-# %% 
-geo_model.series
-
-# %%
-# For the surfaces, there are two numpy arrays, one with vertices and the
-# other with triangles. Axis 0 is each surface in the order:
-# 
-
-# %% 
-geo_model.surfaces
+gpv.plot_2d(geo_model, cell_number=[10], series_n=3, show_scalar=True)
 
 # %% 
-np.save('Hecho_scalar', geo_model.solutions.scalar_field_matrix)
-
-
-# %%
-def write_property_to_gocad_voxet(propertyfilename, propertyvalues):
-    """
-    This function writes a numpy array into the right format for a gocad
-    voxet property file. This assumet there is a property already added to the .vo file,
-    and is just updating the file.
-    propertyfile - string giving the path to the file to write
-    propertyvalues - numpy array nz,ny,nx ordering and in float format
-    """
-    propertyvalues = propertyvalues.astype('>f4')  # big endian
-    #     array = propertyvalues.newbyteorder()
-    propertyvalues.tofile(propertyfilename)
-
+gpv.plot_2d(geo_model, cell_number=[10], show_data=True)
 
 # %%
-write_property_to_gocad_voxet(f'hecho_sf_gempy_{data_amount}',
-                              geo_model.solutions.scalar_field_matrix[3].reshape([321, 21, 91]).ravel('F'))
+gpv.plot_2d(geo_model, section_names=['section'], show_data=True)
 
 # %%
-4
+# sphinx_gallery_thumbnail_number = 3
+gpv.plot_3d(geo_model, kwargs_plot_structured_grid={'opacity': .2})
```

### Comparing `gempy-2023.1.0b6/examples/integrations/gempy_export_MOOSE.py` & `gempy-2023.2.0b1/examples/integrations/gempy_export_MOOSE.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/examples/integrations/gempy_striplog.py` & `gempy-2023.2.0b1/examples/integrations/gempy_subsurface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,244 +1,177 @@
 """
-Transform 2019: Integrating Striplog and GemPy
-==============================================
-
+GemPy - Subsurface Link
+=======================
 """
 
-# %% 
-# ! pip install welly striplog
-
-# %% 
-# Authors: M. de la Varga, Evan Bianco, Brian Burnham and Dieter Werthmüller
-# Importing GemPy
-import gempy as gp
-
-# Importing auxiliary libraries
+import pooch
 import numpy as np
-import pandas as pn
-import matplotlib.pyplot as plt
-import os
-import welly
-from welly import Location, Project
-import glob
-from striplog import Striplog, Legend, Decor
-
-pn.set_option('precision', 2)
-
-# %%
-# Creating striplog object
-# -----------------------------
-# 
-
-# %% 
-# get well header coordinates
-well_heads = {'alpha': {'kb_coords': (0, 0, 0)},
-              'beta': {'kb_coords': (10, 10, 0)},
-              'gamma': {'kb_coords': (12, 0, 0)},
-              'epsilon': {'kb_coords': (20, 0, 0)}}
+import pandas as pd
 
-# %% 
-# Reading tops file
-cwd = os.getcwd()
-if 'examples' not in cwd:
-    data_path = os.getcwd() + '/examples'
-else:
-    data_path = cwd + '/..'
+import subsurface as sb
+from subsurface.reader import read_netcdf
 
-print(data_path+'/data/input_data/striplog_integration/*.tops')
-topsfiles = glob.glob(data_path+'/data/input_data/striplog_integration/*.tops')
-topsfiles
+data_url = "https://raw.githubusercontent.com/softwareunderground/subsurface/main" \
+           "/examples/tutorials/wells_unstructured.nc"
 
-# %% 
-# Creating striplog object
-my_striplogs = []
+data_hash = "206290db4e563e379361725349ebf4a02628f4700d361599aedff37fab9cf5b9"
+borehole_unstructured_data_file = pooch.retrieve(url=data_url,
+                                                 known_hash=data_hash)
 
-for file in topsfiles:
-    with open(file) as f:
-        text = f.read()
-        striplog = Striplog.from_csv(text=text)
-        my_striplogs.append(striplog)
+unstruct = read_netcdf.read_unstruct(borehole_unstructured_data_file)
+unstruct
 
-striplog_dict = {'alpha': my_striplogs[1],
-                 'beta': my_striplogs[2],
-                 'gamma': my_striplogs[3],
-                 'epsilon': my_striplogs[0]}
+# %%
+element = sb.LineSet(unstruct)
+lines_mesh = sb.visualization.to_pyvista_line(element, radius=50)
 
-striplog_dict['alpha'][0]
+# Plot default LITH
+sb.visualization.pv_plot([lines_mesh])
 
-# %% 
-# Plot striplog
-f, a = plt.subplots(ncols=4, sharey=True)
 
-for e, log in enumerate(striplog_dict.items()):
-    log[1].plot(ax=a[e], legend=None)
-f.tight_layout()
-plt.show()
+# %% md
+# Findig the boreholes bases
+# --------------------------
+# GemPy interpolates the bottom of a unit, therefore we need to be able to extract those points to be able tointerpolate them.
+# xarray, pandas and numpy are using the same type of memory representation what makes possible to use the same or at least similar methods to manipulate the data to our will.
+# Lets find the base points of each well:
 
 # %%
-# Striplog to pandas df of bottoms
-rows = []
-for wellname in striplog_dict.keys():
-    for i, interval in enumerate(striplog_dict[wellname]):
-        surface_name = interval.primary.lith
-        surface_base = interval.base.middle
-        x, y = well_heads[wellname]['kb_coords'][:-1]
-        series = 1
-        rows.append([x, y, surface_base, surface_name, series, wellname])
 
-column_names = ['X', 'Y', 'Z', 'surface', 'series', 'wellname']
-df = pn.DataFrame(rows, columns=column_names)
-df
+# Creating references to the xarray.DataArray
+cells_attr = unstruct.data.cell_attrs
+cells = unstruct.data.cells
+vertex = unstruct.data.vertex
+# Find vertex points at the boundary of two units
+# Marking each vertex
+bool_prop_change = cells_attr.values[1:] != cells_attr.values[:-1]
+# Getting the index of the vertex
+args_prop_change = np.where(bool_prop_change)[0]
+# Getting the attr values at those points
+vals_prop_change = cells_attr[args_prop_change]
+vals_prop_change.to_pandas()
 
 # %%
-# GemPy model
-# ----------------
-# 
+# Getting the vertex values at those points
+vertex_args_prop_change = cells[args_prop_change, 1]
+interface_points = vertex[vertex_args_prop_change]
+interface_points
 
-# %% 
-# Create gempy model object
-geo_model = gp.create_model('welly_integration')
 
-extent = [-100, 300, -100, 200, -150, 0]
-res = [60, 60, 60]
+# %%
+# Creating a new UnstructuredData
+interf_us= sb.UnstructuredData.from_array(vertex=interface_points.values, cells="points",
+                                          cells_attr=vals_prop_change.to_pandas())
+interf_us
 
-# Initializting model using the striplog df
-gp.init_data(geo_model, extent, res, surface_points_df=df)
+# %% md
+# This new UnstructuredData object instead containing data that represent lines, contain point data at the bottom of each
+# unit. We can plot it very similar as before:
 
-# %% 
-geo_model.surface_points.df.head()
+element = sb.PointSet(interf_us)
+point_mesh = sb.visualization.to_pyvista_points(element)
+sb.visualization.pv_plot([lines_mesh, point_mesh])
 
-# %% 
-geo_model.surfaces
+# %% md
+# GemPy: Initialize model
+# -----------------------
+# The first step to create a GemPy model is create a gempy.
 
-# %% 
-dec_list = []
-for e, i in enumerate(striplog_dict['alpha']):
-    dec_list.append(Decor({'_colour': geo_model.surfaces.df.loc[e, 'color'],
-                           'width': None,
-                           'component': i.primary,
-                           'hatch': None}))
+# %%
 
+import gempy as gp
+geo_model = gp.create_model("getting started")
+geo_model.set_regular_grid(extent=[275619, 323824, 3914125, 3961793, -3972.6, 313.922], resolution=[50,50,50])
+gp.set_interpolator(geo_model, aesara_optimizer='fast_compile', verbose=[])
 
-# %% 
-# welly plot with gempy colors
-# Create Decor list
-dec_list = []
-for e, i in enumerate(striplog_dict['alpha']):
-    dec_list.append(Decor({'_colour': geo_model.surfaces.df.loc[e, 'color'],
-                           'width': None,
-                           'component': i.primary,
-                           'hatch': None}))
+# %% md
+# Making a model step by step.
+# ----------------------------
 
-# Create legend
-legend = Legend(dec_list)
-legend
+# The temptation at this point is to bring all the points into gempy and just interpolate. However, often that strategy
+# results in ill posed problems due to noise or irregularities in the data. gempy has been design to being able to
+# iterate rapidly and therefore a much better workflow use to be creating the model step by step.
+#
+# To do that, lets define a function that we can pass the name of the formation and get the assotiated vertex. Grab from
+# the interf_us the XYZ coordinates of the first layer:
 
-# %% 
-# Plot striplogs:
-f, a = plt.subplots(ncols=4, sharey=True)
+# %%
+def get_interface_coord_from_surfaces(surface_names: list, verbose=False):
+    df = pd.DataFrame(columns=["X", "Y", "Z", "surface"])
 
-for e, log in enumerate(striplog_dict.items()):
-    log[1].plot(ax=a[e], legend=legend)
-f.tight_layout()
-plt.show()
+    for e, surface_name in enumerate(surface_names):
+        # The properties in subsurface start at 1
+        val_property = formations.index(surface_name) + 1
+        # Find the cells with the surface id
+        args_from_first_surface = np.where(vals_prop_change == val_property)[0]
+        if verbose: print(args_from_first_surface)
+        # Find the vertex
+        points_from_first_surface = interface_points[args_from_first_surface]
+        if verbose: print(points_from_first_surface)
 
-# %% 
-# Modifying the coordinates to make more sense
-geo_model.surface_points.df[['X', 'Y']] = geo_model.surface_points.df[['X', 'Y']] * 10
-geo_model.surface_points.df['Z'] *= -1
+        # xarray.DataArray to pandas.DataFrame
+        surface_pandas = points_from_first_surface.to_pandas()
 
-# %% 
-# Delete points of the basement surface since we are intepolating bottoms (that surface wont exit).
-geo_model.delete_surface_points_basement()
+        # Add formation column
+        surface_pandas["surface"] = surface_name
+        df = df.append(surface_pandas)
 
-# %% 
-# Adding an arbitrary orientation. Remember gempy need an orientation per series
-geo_model.set_default_orientation()
-geo_model.modify_orientations(0, X=-500)
+    return df.reset_index()
 
-# %% 
-gp.plot_2d(geo_model)
+# %% md
+# Surfaces
+# ++++++++
 
+formations = ["topo", "etchegoin", "macoma", "chanac", "mclure",
+              "santa_margarita", "fruitvale",
+              "round_mountain", "olcese", "freeman_jewett", "vedder", "eocene",
+              "cretaceous",
+              "basement", "null"]
 
 # %%
-gp.set_interpolator(geo_model)
-
-# %% 
-gp.compute_model(geo_model)
+geo_model.add_features("Formations")
+one_formation_every = 3
+geo_model.add_surfaces(formations[0:4*one_formation_every:one_formation_every])
 
-# %% 
+geo_model.map_stack_to_surfaces({"Formations": ["etchegoin", "macoma", "chanac", "mclure"],
+                                 "Default series": ["topo"]},
+                                set_series=False)
 
-p2d = gp.plot_2d(geo_model, cell_number=[30], show_data=True, show=True)
 
 # %%
-gp.plot_3d(geo_model)
-
+gempy_surface_points = get_interface_coord_from_surfaces(formations[0:3*one_formation_every:one_formation_every])
 
 # %%
-# Pinch out model
-# ------------------
-# 
-# As we can see the 3D model generated above does not honor the forth well
-# lets fix it. First lets add an unconformity: between the yellow and
-# green layer:
-# 
+geo_model.set_surface_points(gempy_surface_points, update_surfaces=False)
+geo_model.update_to_interpolator()
 
-# %% 
-geo_model.add_features('Unconformity')
 
-# %%
-# Now we set the green layer in the second series
-# 
-
-# %% 
-geo_model.map_stack_to_surfaces({'Uncomformity': ['brian', 'evan', 'dieter']})
-geo_model.add_surfaces('basement')
+# %% md
+# Adding orientations
+# -------------------
 
 # %%
-# Lastly we need to add a dummy orientation to the new series:
-# 
-
-# %% 
-geo_model.add_orientations(-500, 0, -100, 'dieter', [0, 0, 1])
+# find neighbours
+neighbours = gp.select_nearest_surfaces_points(geo_model, geo_model._surface_points.df, 2)
 
-# %%
-# Now we can compute:
-# 
+# calculate all fault orientations
+gp.set_orientation_from_neighbours_all(geo_model, neighbours)
 
-# %% 
-gp.compute_model(geo_model)
+# %% md
+# Using the flag to subsurface, the result of the interpolation will get stored in `subsurface` data objects. In the
+# future exporting to subsurface will be the default behaviour.
 
-# %% 
-p = gp.plot_2d(geo_model, cell_number=[30], show_data=True)
-f, a = plt.subplots(ncols=4, sharey=True)
+# %%
+gp.compute_model(geo_model, to_subsurface=True)
 
-for e, log in enumerate(striplog_dict.items()):
-    log[1].plot(ax=a[e], legend=legend)
-f.tight_layout()
-plt.show()
+# %%
+p3d = gp.plot_3d(geo_model)
 
 # %%
-# Getting better but not quite there yet. Since the yellow does not show
-# up in the last well the pinch out has to happen somewhere before so lets
-# add an artifial point to get that shape:
-# 
+geo_model.solutions.s_regular_grid
 
-# %% 
-geo_model.add_surface_points(200, 0, -75, 'evan');
+# %%
+geo_model.solutions.meshes
 
-# %% 
-gp.compute_model(geo_model)
-p = gp.plot_2d(geo_model, cell_number=[30], show_data=True)
-f, a = plt.subplots(ncols=4, sharey=True)
 
-for e, log in enumerate(striplog_dict.items()):
-    log[1].plot(ax=a[e], legend=legend)
-f.tight_layout()
-plt.show()
 
-# %%
-# sphinx_gallery_thumbnail_number = 7
-gp.plot_3d(geo_model)
 
-# %%
-# gp.save_model(geo_model)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gempy-2023.1.0b6/examples/tutorials_/a_getting_started/get_started.py` & `gempy-2023.2.0b1/examples/tutorials/a_getting_started/get_started.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # appropriate. 
 
 # %%
 geo_model: gp.data.GeoModel = gp.create_geomodel(
     project_name='Model1',
     extent=[0, 791, -200, 200, -582, 0],
     resolution=[50, 50, 50],
-    number_octree_levels=4,
+    refinement=4,
     structural_frame=gp.data.StructuralFrame.initialize_default_structure()
 )
 geo_model
 
 # %%
 # Creating a figure:
 # ~~~~~~~~~~~~~~~~~~
```

### Comparing `gempy-2023.1.0b6/gempy/API/__init__.py` & `gempy-2023.2.0b1/gempy/API/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .map_stack_to_surfaces_API import map_stack_to_surfaces
 
 # Grid API
 from .grid_API import (
     set_active_grid,
     set_custom_grid,
     set_section_grid,
+    set_centered_grid,
     set_topography_from_random,
     set_topography_from_file,
     set_topography_from_subsurface_structured_grid
 )
 
 # Examples generator
 from .examples_generator import generate_example_model
@@ -48,19 +49,24 @@
     create_orientations_from_surface_points_coords
 )
 
 # Data manipulation: structural frame
 from ..modules.data_manipulation.manipulate_structural_frame import (
     add_structural_group,
     remove_structural_group_by_index,
-    remove_structural_group_by_name
+    remove_structural_group_by_name,
+    remove_element_by_name
 )
 
+# Geophysics
+from gempy_engine.modules.geophysics.gravity_gradient import calculate_gravity_gradient
+
 __all__ = [
     'create_data_legacy', 'create_geomodel', 'compute_model', 'compute_model_at', 'map_stack_to_surfaces',
     'set_section_grid', 'set_active_grid', 'set_topography_from_random', 'set_topography_from_file', 'set_topography_from_subsurface_structured_grid',
-    'set_custom_grid',
+    'set_custom_grid', 'set_centered_grid',
     'generate_example_model', 'set_fault_relation', 'set_is_fault', 'set_is_finite_fault',
     'add_surface_points', 'add_orientations', 'delete_surface_points', 'delete_orientations',
     'create_orientations_from_surface_points_coords', 'modify_surface_points', 'modify_orientations',
-    'add_structural_group', 'remove_structural_group_by_index', 'remove_structural_group_by_name'
+    'add_structural_group', 'remove_structural_group_by_index', 'remove_structural_group_by_name', 'remove_element_by_name',
+    'calculate_gravity_gradient'
 ]
```

### Comparing `gempy-2023.1.0b6/gempy/API/compute_API.py` & `gempy-2023.2.0b1/gempy/API/compute_API.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,31 @@
     """
     engine_config = engine_config or GemPyEngineConfig(
         backend=AvailableBackends.numpy,
         use_gpu=False,
     )
 
     match engine_config.backend:
-        case AvailableBackends.numpy | AvailableBackends.tensorflow:
+        case AvailableBackends.numpy | AvailableBackends.PYTORCH:
 
             BackendTensor.change_backend_gempy(
                 engine_backend=engine_config.backend,
                 use_gpu=engine_config.use_gpu,
                 dtype=engine_config.dtype
             )
 
+            # TODO: To decide what to do with this.
+            interpolation_input = gempy_model.interpolation_input
+            gempy_model.taped_interpolation_input = interpolation_input
+
             gempy_model.solutions = gempy_engine.compute_model(
-                interpolation_input=gempy_model.interpolation_input,
+                interpolation_input=interpolation_input,
                 options=gempy_model.interpolation_options,
-                data_descriptor=gempy_model.input_data_descriptor
+                data_descriptor=gempy_model.input_data_descriptor,
+                geophysics_input=gempy_model.geophysics_input,
             )
 
         case AvailableBackends.aesara | AvailableBackends.legacy:
             gempy_model.legacy_model = _legacy_compute_model(gempy_model)
         case _:
             raise ValueError(f'Backend {engine_config} not supported')
```

### Comparing `gempy-2023.1.0b6/gempy/API/examples_generator.py` & `gempy-2023.2.0b1/gempy/API/examples_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 
 def _generate_2_5d_model(compute_model: bool) -> gp.data.GeoModel:
     geo_model: gp.data.GeoModel = gp.create_geomodel(
         project_name='Model1',
         extent=[0, 791, -200, 200, -582, 0],
         resolution=[50, 50, 50],
-        number_octree_levels=1,
+        refinement=1,
         structural_frame=gp.data.StructuralFrame.initialize_default_structure()
     )
-    
+
     gp.add_surface_points(
         geo_model=geo_model,
         x=[223, 458, 612],
         y=[0.01, 0, 0],
         z=[-94, -197, -14],
         elements_names='surface1'
     )
@@ -44,15 +44,15 @@
         y=[1],
         z=[-300],
         elements_names=['surface1'],
         pole_vector=[[0, 0, 1]]
     )
 
     geo_model.update_transform(gp.data.GlobalAnisotropy.NONE)  # * Remove the auto anisotropy for this 2.5D model
-    
+
     element2 = gp.data.StructuralElement(
         name='surface2',
         color=next(geo_model.structural_frame.color_generator),
         surface_points=gp.data.SurfacePointsTable.from_arrays(
             x=np.array([225, 459]),
             y=np.array([0, 0]),
             z=np.array([-269, -279]),
@@ -102,27 +102,25 @@
         elements=[element_fault],
         structural_relation=gp.data.StackRelationType.FAULT,
         fault_relations=gp.data.FaultsRelationSpecialCase.OFFSET_ALL
     )
 
     geo_model.structural_frame.insert_group(0, group_fault)  # * We are placing it already in the right place so we do not need to map anything
 
-
     gp.set_topography_from_random(
         grid=geo_model.grid,
         fractal_dimension=1.9,
         d_z=np.array([-150, 0]),
         topography_resolution=np.array([50, 40])
     )
-    
+
     if compute_model:
         gp.compute_model(geo_model)
-    
-    return geo_model
 
+    return geo_model
 
 
 def _generate_horizontal_stratigraphic_model(compute_model: bool) -> gp.data.GeoModel:
     """
     Function to create a geological model of horizontally stacked layers,
     map the geological series to surfaces, and compute the geological model.
     """
@@ -162,15 +160,15 @@
     data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
     path_to_data = data_path + "/data/input_data/jan_models/"
 
     # Create a GeoModel instance
     geo_data: gp.data.GeoModel = gp.create_geomodel(
         project_name='fold',
         extent=[0, 1000, 0, 1000, 0, 1000],
-        number_octree_levels=5,
+        refinement=5,
         importer_helper=gp.data.ImporterHelper(
             path_to_orientations=path_to_data + "model2_orientations.csv",
             path_to_surface_points=path_to_data + "model2_surface_points.csv"
         )
     )
 
     # Map geological series to surfaces
@@ -218,48 +216,49 @@
     # Define fault groups
     geo_data.structural_frame.structural_groups[0].structural_relation = StackRelationType.FAULT
     geo_data.structural_frame.fault_relations = np.array([[0, 1], [0, 0]])
     gp.set_is_fault(
         frame=geo_data,
         fault_groups=['Fault_Series']
     )
-    
+
     if compute_model:
         # Compute the geological model
         gp.compute_model(geo_data)
 
     return geo_data
 
 
-def _generate_combination_model(compute_model:bool) -> gp.data.GeoModel:
+def _generate_combination_model(compute_model: bool) -> gp.data.GeoModel:
     """
     Function to create a model with a folded domain featuring an unconformity and a fault,
     map the geological series to surfaces, and compute the geological model.
     """
     # Define the path to data
     data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
     path_to_data = data_path + "/data/input_data/jan_models/"
 
     # Create a GeoModel instance
     geo_data = gp.create_geomodel(
         project_name='combination',
         extent=[0, 2500, 0, 1000, 0, 1000],
-        number_octree_levels=4,
+        refinement=4,
         resolution=[125, 50, 50],
         importer_helper=gp.data.ImporterHelper(
             path_to_orientations=path_to_data + "model7_orientations.csv",
             path_to_surface_points=path_to_data + "model7_surface_points.csv"
         )
     )
+    geo_data.interpolation_options.number_octree_levels_surface = 4 
 
     # Map geological series to surfaces
     gp.map_stack_to_surfaces(
         gempy_model=geo_data,
         mapping_object={
-            "Fault_Series" : ('fault'),
+            "Fault_Series": ('fault'),
             "Strat_Series1": ('rock3'),
             "Strat_Series2": ('rock2', 'rock1'),
         }
     )
 
     # Define the structural relation
     geo_data.structural_frame.structural_groups[0].structural_relation = StackRelationType.FAULT
@@ -267,10 +266,15 @@
         [[0, 1, 1],
          [0, 0, 0],
          [0, 0, 0]]
     )
 
     # Compute the geological model
     if compute_model:
-        gp.compute_model(geo_data)
+        gp.compute_model(
+            gempy_model=geo_data,
+            engine_config=gp.data.GemPyEngineConfig(
+                backend=gp.data.AvailableBackends.numpy
+            )
+        )
 
     return geo_data
```

### Comparing `gempy-2023.1.0b6/gempy/API/faults_API.py` & `gempy-2023.2.0b1/gempy/API/faults_API.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,109 @@
-﻿from typing import Union
-import numpy as np
-
-from gempy_engine.core.data.stack_relation_type import StackRelationType
-from gempy.core.data import GeoModel, StructuralFrame
-from gempy.core.data.structural_group import StructuralGroup, FaultsRelationSpecialCase
-
-
-def set_is_fault(frame: Union[GeoModel, StructuralFrame], fault_groups: Union[list[str], list[StructuralGroup]],
-                 change_color: bool = True) -> StructuralFrame:
-    """
-    Sets given groups as fault in the structural frame of the GeoModel. It can optionally change the color of these groups.
-
-    Args:
-        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
-        fault_groups (Union[list[str], list[StructuralGroup]]): Groups to be set as faults.
-        change_color (bool, optional): If True, changes the color of the fault groups. Defaults to True.
-
-    Returns:
-        StructuralFrame: The updated StructuralFrame object.
-    """
-    if isinstance(frame, GeoModel):
-        frame = frame.structural_frame
-
-    frame = _find_and_set_fields(
-        frame=frame,
-        fault_groups=fault_groups,
-        faults_relation_type=FaultsRelationSpecialCase.OFFSET_FORMATIONS,
-        stack_relation_type=StackRelationType.FAULT,
-        change_color=change_color
-    )
-
-    # * TODO: Set the fault colors
-
-    return frame
-
-
-def unset_is_fault(frame: Union[GeoModel, StructuralFrame], fault_groups: Union[list[str], list[StructuralGroup]]) -> StructuralFrame:
-    """
-    Unsets given groups as fault in the structural frame of the GeoModel.
-
-    Args:
-        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
-        fault_groups (Union[list[str], list[StructuralGroup]]): Groups to be unset as faults.
-
-    Returns:
-        StructuralFrame: The updated StructuralFrame object.
-    """
-    if isinstance(frame, GeoModel):
-        frame = frame.structural_frame
-
-    frame = _find_and_set_fields(
-        frame=frame,
-        fault_groups=fault_groups,
-        faults_relation_type=FaultsRelationSpecialCase.OFFSET_NONE,
-        stack_relation_type=StackRelationType.ERODE,
-        change_color=False
-    )
-
-    return frame
-
-
-def set_fault_relation(frame: Union[GeoModel, StructuralFrame], rel_matrix: np.ndarray) -> StructuralFrame:
-    """
-    Sets the fault relations in the structural frame of the GeoModel.
-
-    Args:
-        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
-        rel_matrix (np.ndarray): Fault relation matrix to be set.
-
-    Returns:
-        StructuralFrame: The updated StructuralFrame object.
-    """
-    
-    if isinstance(frame, GeoModel):
-        frame = frame.structural_frame
-
-    frame.fault_relations = rel_matrix
-    return frame
-
-
-def set_is_finite_fault(self, series_fault=None, toggle: bool = True):
-    """"""
-    raise NotImplementedError
-    s = self._faults.set_is_finite_fault(series_fault,
-                                         toggle)  # change df in Fault obj
-    # change shared aesara variable for infinite factor
-    self._interpolator.set_aesara_shared_is_finite()
-    return s
-
-
-# TODO: Move to a faults module
-def _find_and_set_fields(frame: StructuralFrame, fault_groups: list[StructuralGroup],
-                         faults_relation_type: FaultsRelationSpecialCase, stack_relation_type: StackRelationType,
-                         change_color: bool) -> StructuralFrame:
-    for index, group in enumerate(fault_groups):
-        if isinstance(group, str):
-            group = next((g for g in frame.structural_groups if g.name == group), None)
-        if isinstance(group, StructuralGroup):
-            group.structural_relation = stack_relation_type
-            group.fault_relations = faults_relation_type  # * Set the default fault relations
-            if change_color:
-                for element in group.elements:
-                    element.color = '#527682'
-        else:
-            raise ValueError(f"Could not find group '{group}' in structural frame.")
-    return frame
+﻿from typing import Union
+import numpy as np
+
+from gempy_engine.core.data.stack_relation_type import StackRelationType
+from gempy.core.data import GeoModel, StructuralFrame
+from gempy.core.data.structural_group import StructuralGroup, FaultsRelationSpecialCase
+
+
+def set_is_fault(frame: Union[GeoModel, StructuralFrame], fault_groups: Union[list[str], list[StructuralGroup]],
+                 faults_relation_type: FaultsRelationSpecialCase = FaultsRelationSpecialCase.OFFSET_FORMATIONS,
+                 change_color: bool = True) -> StructuralFrame:
+    """
+    Sets given groups as fault in the structural frame of the GeoModel. It can optionally change the color of these groups.
+
+    Args:
+        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
+        fault_groups (Union[list[str], list[StructuralGroup]]): Groups to be set as faults.
+        faults_relation_type (FaultsRelationSpecialCase, optional): Faults relation type to be set. Defaults to FaultsRelationSpecialCase.OFFSET_FORMATIONS.
+        change_color (bool, optional): If True, changes the color of the fault groups. Defaults to True.
+
+    Returns:
+        StructuralFrame: The updated StructuralFrame object.
+    """
+    if isinstance(frame, GeoModel):
+        frame = frame.structural_frame
+
+    frame = _find_and_set_fields(
+        frame=frame,
+        fault_groups=fault_groups,
+        faults_relation_type=faults_relation_type,
+        stack_relation_type=StackRelationType.FAULT,
+        change_color=change_color
+    )
+
+    # * TODO: Set the fault colors
+
+    return frame
+
+
+def unset_is_fault(frame: Union[GeoModel, StructuralFrame], fault_groups: Union[list[str], list[StructuralGroup]]) -> StructuralFrame:
+    """
+    Unsets given groups as fault in the structural frame of the GeoModel.
+
+    Args:
+        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
+        fault_groups (Union[list[str], list[StructuralGroup]]): Groups to be unset as faults.
+
+    Returns:
+        StructuralFrame: The updated StructuralFrame object.
+    """
+    if isinstance(frame, GeoModel):
+        frame = frame.structural_frame
+
+    frame = _find_and_set_fields(
+        frame=frame,
+        fault_groups=fault_groups,
+        faults_relation_type=FaultsRelationSpecialCase.OFFSET_NONE,
+        stack_relation_type=StackRelationType.ERODE,
+        change_color=False
+    )
+
+    return frame
+
+
+def set_fault_relation(frame: Union[GeoModel, StructuralFrame], rel_matrix: np.ndarray) -> StructuralFrame:
+    """
+    Sets the fault relations in the structural frame of the GeoModel.
+
+    Args:
+        frame (Union[GeoModel, StructuralFrame]): GeoModel or its StructuralFrame to be modified.
+        rel_matrix (np.ndarray): Fault relation matrix to be set.
+
+    Returns:
+        StructuralFrame: The updated StructuralFrame object.
+    """
+
+    if isinstance(frame, GeoModel):
+        frame = frame.structural_frame
+
+    frame.fault_relations = rel_matrix
+    return frame
+
+
+def set_is_finite_fault(self, series_fault=None, toggle: bool = True):
+    """"""
+    raise NotImplementedError
+    s = self._faults.set_is_finite_fault(series_fault,
+                                         toggle)  # change df in Fault obj
+    # change shared aesara variable for infinite factor
+    self._interpolator.set_aesara_shared_is_finite()
+    return s
+
+
+# TODO: Move to a faults module
+def _find_and_set_fields(frame: StructuralFrame, fault_groups: list[StructuralGroup],
+                         faults_relation_type: FaultsRelationSpecialCase, stack_relation_type: StackRelationType,
+                         change_color: bool) -> StructuralFrame:
+    for index, group in enumerate(fault_groups):
+        if isinstance(group, str):
+            group = next((g for g in frame.structural_groups if g.name == group), None)
+        if isinstance(group, StructuralGroup):
+            group.structural_relation = stack_relation_type
+            group.fault_relations = faults_relation_type  # * Set the default fault relations
+            if change_color:
+                for element in group.elements:
+                    element.color = '#527682'
+        else:
+            raise ValueError(f"Could not find group '{group}' in structural frame.")
+    return frame
```

### Comparing `gempy-2023.1.0b6/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_output.py` & `gempy-2023.2.0b1/gempy/API/gp2_gp3_compatibility/gp3_to_gp2_output.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/API/grid_API.py` & `gempy-2023.2.0b1/gempy/API/grid_API.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,96 @@
-﻿from typing import Union, Sequence
-
-import numpy as np
-
-from gempy.core.data import Grid
-from gempy.core.data.grid import GridTypes
-from gempy.core.data.grid_modules import CustomGrid
-from gempy.core.data.grid_modules.topography import Topography
-from gempy.modules.grids.create_topography import create_random_topography
-from gempy.optional_dependencies import require_subsurface
-
-
-def set_section_grid(grid: Grid, section_dict: dict):
-    if grid.sections is None:
-        grid.create_section_grid(section_dict=section_dict)
-    else:
-        grid.sections.set_sections(section_dict,
-                                   regular_grid=grid.regular_grid)
-
-    set_active_grid(grid, [GridTypes.SECTIONS])
-    return grid.sections
-
-
-def set_topography_from_random(grid: Grid, fractal_dimension: float = 2.0, d_z: Union[Sequence, None] = None,
-                               topography_resolution: Union[Sequence, None] = None):
-    if topography_resolution is None:
-        topography_resolution = grid.regular_grid.resolution
-
-    random_topography: np.ndarray = create_random_topography(
-        extent=grid.regular_grid.extent,
-        resolution=topography_resolution,
-        dz=d_z,
-        fractal_dimension=fractal_dimension
-    )
-    
-    grid.topography = Topography(
-        regular_grid=grid.regular_grid,
-        values_2d=random_topography
-    )
-
-    set_active_grid(grid, [GridTypes.TOPOGRAPHY])
-    return grid.topography
-
-
-def set_topography_from_subsurface_structured_grid(grid: Grid, struct: 'import subsurface'):
-    grid.topography = Topography.from_subsurface_structured_data(struct, grid.regular_grid)
-    set_active_grid(grid, [GridTypes.TOPOGRAPHY])
-    return grid.topography
-
-
-def set_topography_from_file(grid: Grid, filepath: str, crop_to_extent: Union[Sequence, None] = None):
-    ss = require_subsurface()
-    struct: ss.StructuredData = ss.reader.read_structured_topography(
-        path=filepath,
-        crop_to_extent=crop_to_extent
-    )
-    return set_topography_from_subsurface_structured_grid(grid, struct)
-
-
-def set_custom_grid(grid: Grid, xyz_coord: np.ndarray):
-    custom_grid = CustomGrid(xyx_coords=xyz_coord)
-    grid.custom_grid = custom_grid
-    
-    set_active_grid(grid, [GridTypes.CUSTOM])
-    return grid.custom_grid
-
-
-def set_topography_from_gdal():
-    raise NotImplementedError("This is not implemented yet")
-
-
-def set_topography_from_array():
-    raise NotImplementedError("This is not implemented yet")
-
-
-def set_active_grid(grid: Grid, grid_type: list[GridTypes], reset: bool = False):
-    if reset is True:
-        grid.deactivate_all_grids()
-    for grid_type in grid_type:
-        grid.active_grids_bool[grid_type.value] = True
-
-    print(f'Active grids: {grid.grid_types[grid.active_grids_bool]}')
-
-    return grid
+﻿from typing import Union, Sequence
+
+import numpy as np
+
+from gempy.core.data import Grid
+from gempy.core.data.grid import GridTypes
+from gempy.core.data.grid_modules import CustomGrid
+from gempy.core.data.grid_modules.topography import Topography
+from gempy.modules.grids.create_topography import create_random_topography
+from gempy.optional_dependencies import require_subsurface
+
+
+def set_section_grid(grid: Grid, section_dict: dict):
+    if grid.sections is None:
+        grid.create_section_grid(section_dict=section_dict)
+    else:
+        grid.sections.set_sections(section_dict,
+                                   regular_grid=grid.regular_grid)
+
+    set_active_grid(grid, [GridTypes.SECTIONS])
+    return grid.sections
+
+
+def set_topography_from_random(grid: Grid, fractal_dimension: float = 2.0, d_z: Union[Sequence, None] = None,
+                               topography_resolution: Union[Sequence, None] = None):
+    if topography_resolution is None:
+        topography_resolution = grid.regular_grid.resolution
+
+    random_topography: np.ndarray = create_random_topography(
+        extent=grid.regular_grid.extent,
+        resolution=topography_resolution,
+        dz=d_z,
+        fractal_dimension=fractal_dimension
+    )
+    
+    grid.topography = Topography(
+        regular_grid=grid.regular_grid,
+        values_2d=random_topography
+    )
+
+    set_active_grid(grid, [GridTypes.TOPOGRAPHY])
+    return grid.topography
+
+
+def set_topography_from_subsurface_structured_grid(grid: Grid, struct: 'import subsurface'):
+    grid.topography = Topography.from_subsurface_structured_data(struct, grid.regular_grid)
+    set_active_grid(grid, [GridTypes.TOPOGRAPHY])
+    return grid.topography
+
+
+def set_topography_from_file(grid: Grid, filepath: str, crop_to_extent: Union[Sequence, None] = None):
+    ss = require_subsurface()
+    struct: ss.StructuredData = ss.reader.read_structured_topography(
+        path=filepath,
+        crop_to_extent=crop_to_extent
+    )
+    return set_topography_from_subsurface_structured_grid(grid, struct)
+
+
+def set_custom_grid(grid: Grid, xyz_coord: np.ndarray):
+    custom_grid = CustomGrid(xyx_coords=xyz_coord)
+    grid.custom_grid = custom_grid
+    
+    set_active_grid(grid, [GridTypes.CUSTOM])
+    return grid.custom_grid
+
+
+def set_centered_grid(grid: Grid, centers: np.ndarray, resolution: Sequence[float], radius: Union[float, Sequence[float]]):
+    from gempy_engine.core.data.centered_grid import CenteredGrid
+    centered_grid = CenteredGrid(
+        centers=centers,
+        resolution=resolution,
+        radius=radius
+    )
+    grid.centered_grid = centered_grid
+    set_active_grid(grid, [GridTypes.CENTERED])
+    return grid.centered_grid
+
+
+def set_topography_from_gdal():
+    raise NotImplementedError("This is not implemented yet")
+
+
+def set_topography_from_array():
+    raise NotImplementedError("This is not implemented yet")
+
+
+def set_active_grid(grid: Grid, grid_type: list[GridTypes], reset: bool = False):
+    if reset is True:
+        grid.deactivate_all_grids()
+    for grid_type in grid_type:
+        grid.active_grids_bool[grid_type.value] = True
+
+    print(f'Active grids: {grid.grid_types[grid.active_grids_bool]}')
+
+    return grid
```

### Comparing `gempy-2023.1.0b6/gempy/API/initialization_API.py` & `gempy-2023.2.0b1/gempy/API/initialization_API.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,44 +16,48 @@
 
 
 def create_geomodel(
         *,
         project_name: str = 'default_project',
         extent: Union[list, ndarray] = None,
         resolution: Union[list, ndarray] = None,
-        number_octree_levels: int = 1,
+        refinement: int = 1,
         structural_frame: StructuralFrame = None,
         importer_helper: ImporterHelper = None,
 ) -> GeoModel:  # ? Do I need to pass pandas read kwargs?
     """
     Creates a GeoModel instance.
 
     This function initializes a GeoModel object, including its grid and interpolation options.
 
     Args:
         project_name (str, optional): The name of the project. Defaults to 'default_project'.
         extent (Union[list, ndarray], optional): The 3D extent of the grid. Defaults to None.
         resolution (Union[list, ndarray], optional): The resolution of the grid. Defaults to None.
-        number_octree_levels (int, optional): The number of octree levels for the dual contouring interpolation method. Defaults to 1.
+        refinement (int, optional): Defaults to 1.
         structural_frame (StructuralFrame, optional): The structural frame of the GeoModel. Defaults to None.
         importer_helper (ImporterHelper, optional): Helper object to import structural elements. Defaults to None.
 
     Returns:
         GeoModel: The initialized GeoModel object.
     """
+    # init resolutions well
+    if resolution is None:
+        resolution = np.array([20, 20, 20])
+    
     grid: Grid = Grid(
         extent=extent,
-        resolution=resolution or np.array([20, 20, 20])
+        resolution=resolution
     )
 
     interpolation_options: InterpolationOptions = InterpolationOptions(
         range=5,
         c_o=10,
-        dual_contouring=True,
-        number_octree_levels=number_octree_levels,
+        mesh_extraction=True,
+        number_octree_levels=refinement,
     )
     
     match (structural_frame, importer_helper):
         case (None, None):
             # ? For now my gut feeling is that is better to pass the structural frame explicitly
             raise ValueError("Either structural_frame or importer_helper must be provided. You can use StructuralFrame.initialize_default_structure() to create a default structural frame.")
             structural_frame = StructuralFrame.initialize_default_structure()
```

### Comparing `gempy-2023.1.0b6/gempy/API/io_API.py` & `gempy-2023.2.0b1/gempy/API/io_API.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/API/map_stack_to_surfaces_API.py` & `gempy-2023.2.0b1/gempy/API/map_stack_to_surfaces_API.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/__init__.py` & `gempy-2023.2.0b1/gempy/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 from .API import *
 from .API import implicit_functions
 
 # * Assert at least pyton 3.10
 assert sys.version_info[0] >= 3 and sys.version_info[1] >= 10, "GemPy requires Python 3.10 or higher"
 
-__version__ = '2023.2.0'
+__version__ = '2023.2.0b1'
 
 if __name__ == '__main__':
     pass
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/__init__.py` & `gempy-2023.2.0b1/gempy/core/data/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from .structural_element import StructuralElement
 from .orientations import OrientationsTable
 from .surface_points import SurfacePointsTable
 from .grid import Grid, Topography, GridTypes
 from .importer_helper import ImporterHelper
 from .gempy_engine_config import GemPyEngineConfig
 from .structural_group import FaultsRelationSpecialCase
+from ..color_generator import ColorsGenerator
 
 from gempy_engine.core.data.stack_relation_type import StackRelationType
 from gempy_engine.core.data.options import InterpolationOptions
 from gempy_engine.core.data.solutions import Solutions
 from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
 from gempy_engine.core.data.transforms import GlobalAnisotropy, Transform
 from gempy_engine.core.data.kernel_classes.faults import FaultsData, FiniteFaultData
+from gempy_engine.config import AvailableBackends
+from gempy_engine.core.data.geophysics_input import GeophysicsInput
 
 
 __all__ = [
     # From gempy
     'GeoModel', 'StructuralFrame', 'StructuralGroup', 'StructuralElement', 'OrientationsTable', 'SurfacePointsTable',
     'Grid', 'Topography', 'GridTypes',
-    'ImporterHelper', 'GemPyEngineConfig', 'FaultsRelationSpecialCase',
+    'ImporterHelper', 'GemPyEngineConfig', 'FaultsRelationSpecialCase', 'ColorsGenerator',
     # From gempy engine
     'StackRelationType', 'InterpolationOptions', 'Solutions', 'RawArraysSolution', 'GlobalAnisotropy', 'Transform',
-    'FaultsData', 'FiniteFaultData'
+    'FaultsData', 'FiniteFaultData', 'AvailableBackends', 'GeophysicsInput'
 ]
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/geo_model.py` & `gempy-2023.2.0b1/gempy/core/data/geo_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,192 @@
-﻿import pprint
-import warnings
-from dataclasses import dataclass, field
-from typing import Sequence, Optional
-
-import numpy as np
-
-import gempy_engine.core.data.grid
-from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
-from gempy_engine.core.data import InterpolationOptions
-from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
-from gempy_engine.core.data.interpolation_input import InterpolationInput
-from .orientations import OrientationsTable
-from .structural_frame import StructuralFrame
-from gempy_engine.core.data.transforms import Transform, GlobalAnisotropy
-from .grid import Grid
-
-"""
-TODO:
-    - [ ] StructuralFrame will all input points chunked on Elements. Here I will need a property to put all
-    together to feed to InterpolationInput
-
-"""
-
-
-@dataclass
-class GeoModelMeta:
-    """
-    Container for metadata associated with a GeoModel.
-
-    Attributes:
-        name (str): Name of the geological model.
-        creation_date (str): Date of creation of the model.
-        last_modification_date (str): Last modification date of the model.
-        owner (str): Owner of the geological model.
-    """
-
-    name: str
-    creation_date: str
-    last_modification_date: str
-    owner: str
-
-
-@dataclass(init=False)
-class GeoModel:
-    """
-    Class representing a geological model.
-
-    """
-
-    meta: GeoModelMeta  #: Meta-information about the geological model, like its name, creation and modification dates, and owner.
-    structural_frame: StructuralFrame  #: The structural information of the geological model.
-    grid: Grid  #: The general grid used in the geological model.
-
-    # region GemPy engine data types
-    interpolation_options: InterpolationOptions  #: The interpolation options provided by the user.
-
-    transform: Transform = None  #: The transformation used in the geological model for input points.
-    
-    interpolation_grid: gempy_engine.core.data.grid.Grid = None  #: Optional grid used for interpolation. Can be seen as a cache field.
-    _interpolationInput: InterpolationInput = None  #: Input data for interpolation. Fed by the structural frame and can be seen as a cache field.
-    _input_data_descriptor: InputDataDescriptor = None  #: Descriptor of the input data. Fed by the structural frame and can be seen as a cache field.
-
-    # endregion
-    _solutions: gempy_engine.core.data.solutions.Solutions = field(init=False, default=None)  #: The computed solutions of the geological model. 
-
-    legacy_model: "gpl.Project" = None  #: Legacy model (if available). Allows for backward compatibility.
-
-    def __init__(self, name: str, structural_frame: StructuralFrame, grid: Grid,
-                 interpolation_options: InterpolationOptions):
-        # TODO: Fill the arguments properly
-        self.meta = GeoModelMeta(
-            name=name,
-            creation_date=None,
-            last_modification_date=None,
-            owner=None
-        )
-
-        self.structural_frame = structural_frame  # ? This could be Optional
-
-        self.grid = grid
-        self.interpolation_options = interpolation_options
-        self.transform = Transform.from_input_points(
-            surface_points=self.surface_points,
-            orientations=self.orientations
-        )
-
-    def __repr__(self):
-        # TODO: Improve this
-        return pprint.pformat(self.__dict__)
-
-    def update_transform(self, auto_anisotropy: GlobalAnisotropy = GlobalAnisotropy.CUBE, anisotropy_limit: Optional[np.ndarray] = None):
-        self.transform = Transform.from_input_points(
-            surface_points=self.surface_points,
-            orientations=self.orientations
-        )
-        
-        self.transform.apply_anisotropy(anisotropy_type=auto_anisotropy, anisotropy_limit=anisotropy_limit)
-            
-
-    @property
-    def solutions(self):
-        return self._solutions
-
-    @solutions.setter
-    def solutions(self, value):
-        self._solutions = value
-        for e, group in enumerate(self.structural_frame.structural_groups):
-            group.solution = RawArraysSolution(  # ? Maybe I need to add more fields, but I am not sure yet
-                scalar_field_matrix=self._solutions.raw_arrays.scalar_field_matrix[e],
-                block_matrix=self._solutions.raw_arrays.block_matrix[e],
-            )
-
-        for e, element in enumerate(self.structural_frame.structural_elements[:-1]):  # * Ignore basement
-
-            dc_mesh = self._solutions.dc_meshes[e] if self._solutions.dc_meshes is not None else None
-            # TODO: These meshes are in the order of the scalar field
-            element.vertices = (self.transform.apply_inverse(dc_mesh.vertices) if dc_mesh is not None else None)
-            element.edges = (dc_mesh.edges if dc_mesh is not None else None)
-
-    @property
-    def surface_points(self):
-        """This is a copy! Returns a SurfacePointsTable for all surface points across the structural elements"""
-        surface_points_table = self.structural_frame.surface_points
-        if self.transform is not None:
-            surface_points_table.model_transform = self.transform
-        return surface_points_table
-    
-    @surface_points.setter
-    def surface_points(self, value):
-        self.structural_frame.surface_points = value
-
-    @property
-    def orientations(self) -> OrientationsTable:
-        """This is a copy! Returns a OrientationsTable for all orientations across the structural elements"""
-        orientations_table = self.structural_frame.orientations
-        if self.transform is not None:
-            orientations_table.model_transform = self.transform
-        return orientations_table
-    
-    @orientations.setter
-    def orientations(self, value):
-        self.structural_frame.orientations = value
-
-    @property
-    def interpolation_input(self):
-        if self.structural_frame.is_dirty is False:
-            return self._interpolationInput
-        n_octree_lvl = self.interpolation_options.number_octree_levels
-
-        compute_octrees: bool = n_octree_lvl > 1
-
-        # * Set regular grid to the octree resolution. ? Probably a better way to do this would be to make regular_grid resolution a property
-        if compute_octrees:
-            octree_leaf_resolution = np.array([2 ** n_octree_lvl] * 3)
-
-            resolution_not_set = self.grid.regular_grid.resolution is not None
-            resolution_is_octree_resolution = np.allclose(self.grid.regular_grid.resolution, octree_leaf_resolution)
-
-            if resolution_not_set and not resolution_is_octree_resolution:
-                warnings.warn(
-                    message="You are using octrees and passing a regular grid. The resolution of the regular grid will be overwritten",
-                    category=UserWarning
-                )
-
-            self.grid.regular_grid.set_regular_grid(
-                extent=self.grid.regular_grid.extent,
-                resolution=octree_leaf_resolution
-            )
-
-        self._interpolationInput = InterpolationInput.from_structural_frame(
-            structural_frame=self.structural_frame,
-            grid=self.grid,
-            transform=self.transform,
-            octrees=compute_octrees
-        )
-
-        return self._interpolationInput
-
-    @property
-    def input_data_descriptor(self) -> InputDataDescriptor:
-        # TODO: This should have the exact same dirty logic as interpolation_input
-        return self.structural_frame.input_data_descriptor
-
-    def add_surface_points(self, X: Sequence[float], Y: Sequence[float], Z: Sequence[float],
-                           surface: Sequence[str], nugget: Optional[Sequence[float]] = None) -> None:
-        raise NotImplementedError("This method is deprecated. Use `gp.add_surface_points` instead")
+﻿import pprint
+import warnings
+from dataclasses import dataclass, field
+from typing import Sequence, Optional
+
+import numpy as np
+
+import gempy_engine.core.data.grid
+from gempy_engine.core.data import Solutions
+from gempy_engine.core.data.geophysics_input import GeophysicsInput
+from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
+from gempy_engine.core.data import InterpolationOptions
+from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
+from gempy_engine.core.data.interpolation_input import InterpolationInput
+from .orientations import OrientationsTable
+from .structural_frame import StructuralFrame
+from gempy_engine.core.data.transforms import Transform, GlobalAnisotropy
+from .grid import Grid
+
+"""
+TODO:
+    - [ ] StructuralFrame will all input points chunked on Elements. Here I will need a property to put all
+    together to feed to InterpolationInput
+
+"""
+
+
+@dataclass
+class GeoModelMeta:
+    """
+    Container for metadata associated with a GeoModel.
+
+    Attributes:
+        name (str): Name of the geological model.
+        creation_date (str): Date of creation of the model.
+        last_modification_date (str): Last modification date of the model.
+        owner (str): Owner of the geological model.
+    """
+
+    name: str
+    creation_date: str
+    last_modification_date: str
+    owner: str
+
+
+@dataclass(init=False)
+class GeoModel:
+    """
+    Class representing a geological model.
+
+    """
+
+    meta: GeoModelMeta  #: Meta-information about the geological model, like its name, creation and modification dates, and owner.
+    structural_frame: StructuralFrame  #: The structural information of the geological model.
+    grid: Grid  #: The general grid used in the geological model.
+
+    # region GemPy engine data types
+    interpolation_options: InterpolationOptions  #: The interpolation options provided by the user.
+    geophysics_input: GeophysicsInput = None  #: The geophysics input of the geological model.
+    
+    transform: Transform = None  #: The transformation used in the geological model for input points.
+    
+    interpolation_grid: gempy_engine.core.data.grid.Grid = None  #: Optional grid used for interpolation. Can be seen as a cache field.
+    _interpolationInput: InterpolationInput = None  #: Input data for interpolation. Fed by the structural frame and can be seen as a cache field.
+    _input_data_descriptor: InputDataDescriptor = None  #: Descriptor of the input data. Fed by the structural frame and can be seen as a cache field.
+
+    # endregion
+    _solutions: gempy_engine.core.data.solutions.Solutions = field(init=False, default=None)  #: The computed solutions of the geological model. 
+
+    legacy_model: "gpl.Project" = None  #: Legacy model (if available). Allows for backward compatibility.
+
+    def __init__(self, name: str, structural_frame: StructuralFrame, grid: Grid,
+                 interpolation_options: InterpolationOptions):
+        # TODO: Fill the arguments properly
+        self.meta = GeoModelMeta(
+            name=name,
+            creation_date=None,
+            last_modification_date=None,
+            owner=None
+        )
+
+        self.structural_frame = structural_frame  # ? This could be Optional
+
+        self.grid = grid
+        self.interpolation_options = interpolation_options
+        self.transform = Transform.from_input_points(
+            surface_points=self.surface_points,
+            orientations=self.orientations
+        )
+
+    def __repr__(self):
+        # TODO: Improve this
+        return pprint.pformat(self.__dict__)
+
+    def update_transform(self, auto_anisotropy: GlobalAnisotropy = GlobalAnisotropy.NONE, anisotropy_limit: Optional[np.ndarray] = None):
+        self.transform = Transform.from_input_points(
+            surface_points=self.surface_points,
+            orientations=self.orientations
+        )
+        
+        self.transform.apply_anisotropy(anisotropy_type=auto_anisotropy, anisotropy_limit=anisotropy_limit)
+            
+
+    @property
+    def solutions(self) -> Solutions:
+        return self._solutions
+
+    @solutions.setter
+    def solutions(self, value):
+        self._solutions = value
+        for e, group in enumerate(self.structural_frame.structural_groups):
+            group.kriging_solution = RawArraysSolution(  # ? Maybe I need to add more fields, but I am not sure yet
+                scalar_field_matrix=self._solutions.raw_arrays.scalar_field_matrix[e],
+                block_matrix=self._solutions.raw_arrays.block_matrix[e],
+            )
+
+        for e, element in enumerate(self.structural_frame.structural_elements[:-1]):  # * Ignore basement
+
+            dc_mesh = self._solutions.dc_meshes[e] if self._solutions.dc_meshes is not None else None
+            # TODO: These meshes are in the order of the scalar field
+            element.vertices = (self.transform.apply_inverse(dc_mesh.vertices) if dc_mesh is not None else None)
+            element.edges = (dc_mesh.edges if dc_mesh is not None else None)
+
+    @property
+    def surface_points(self):
+        """This is a copy! Returns a SurfacePointsTable for all surface points across the structural elements"""
+        surface_points_table = self.structural_frame.surface_points
+        if self.transform is not None:
+            surface_points_table.model_transform = self.transform
+        return surface_points_table
+    
+    @surface_points.setter
+    def surface_points(self, value):
+        self.structural_frame.surface_points = value
+
+    @property
+    def orientations(self) -> OrientationsTable:
+        """This is a copy! Returns a OrientationsTable for all orientations across the structural elements"""
+        orientations_table = self.structural_frame.orientations
+        if self.transform is not None:
+            orientations_table.model_transform = self.transform
+        return orientations_table
+    
+    @orientations.setter
+    def orientations(self, value):
+        self.structural_frame.orientations = value
+
+    @property
+    def interpolation_input(self):
+        if self.structural_frame.is_dirty is False:
+            return self._interpolationInput
+        n_octree_lvl = self.interpolation_options.number_octree_levels
+
+        compute_octrees: bool = n_octree_lvl > 1
+
+        # * Set regular grid to the octree resolution. ? Probably a better way to do this would be to make regular_grid resolution a property
+        if compute_octrees:
+            octree_leaf_resolution = np.array([2 ** n_octree_lvl] * 3)
+
+            resolution_set = self.grid.regular_grid.resolution is not None
+            resolution_is_octree_resolution = np.allclose(self.grid.regular_grid.resolution, octree_leaf_resolution)
+
+            if resolution_set and not resolution_is_octree_resolution:
+                warnings.warn(
+                    message="You are using refinement and passing a regular grid. The resolution of the regular grid will be overwritten",
+                    category=UserWarning
+                )
+
+            self.grid.regular_grid.set_regular_grid(
+                extent=self.grid.regular_grid.extent,
+                resolution=octree_leaf_resolution
+            )
+
+        self._interpolationInput = InterpolationInput.from_structural_frame(
+            structural_frame=self.structural_frame,
+            grid=self.grid,
+            transform=self.transform,
+            octrees=compute_octrees
+        )
+
+        return self._interpolationInput
+
+    @property
+    def input_data_descriptor(self) -> InputDataDescriptor:
+        # TODO: This should have the exact same dirty logic as interpolation_input
+        return self.structural_frame.input_data_descriptor
+
+    def add_surface_points(self, X: Sequence[float], Y: Sequence[float], Z: Sequence[float],
+                           surface: Sequence[str], nugget: Optional[Sequence[float]] = None) -> None:
+        raise NotImplementedError("This method is deprecated. Use `gp.add_surface_points` instead")
+
+
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/grid.py` & `gempy-2023.2.0b1/gempy/core/data/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.centered_grid_active = False
 
         # Init basic grid empty
         self.regular_grid = self.create_regular_grid(set_active=False, **kwargs)
         self.regular_grid_active = False
 
         # Init optional sections
-        self.sections = grid_types.Sections(regular_grid=self.regular_grid)
+        self.sections = None
 
         self.update_grid_values()
 
     def __str__(self):
         grid_summary = [f"{g_type} (active: {getattr(self, g_type + '_grid_active')}): {len(getattr(self, g_type + '_grid').values)} points"
                         for g_type in self.grid_types]
         grid_summary_str = "\n".join(grid_summary)
@@ -99,27 +99,29 @@
         RegularGrid Docs
         """
         self.regular_grid = grid_types.RegularGrid(extent, resolution, **kwargs)
         if set_active is True:
             self.set_active('regular')
         return self.regular_grid
 
-    def create_custom_grid(self, custom_grid: np.ndarray):
+    # ? DEP?
+    def create_custom_grid_(self, custom_grid: np.ndarray):
         """
         Set a new regular grid and activate it.
 
         Args:
             custom_grid (np.array): [s0]
 
         """
         self.custom_grid = grid_types.CustomGrid(custom_grid)
         self.set_active('custom')
 
     # ! (miguel, Sep 2023) This has to change a lot
-    def create_topography(self, source='random', **kwargs):
+    # ? DEP? 
+    def create_topography_(self, source='random', **kwargs):
         """Create a topography grid and activate it.
 
         Args:
             source:
                 * 'gdal':  Load topography from a raster file.
                 * 'random': Generate random topography (based on a fractal grid).
                 * 'saved': Load topography that was saved with the topography.save() function.
@@ -168,14 +170,15 @@
         self.set_active('topography')
 
     def create_section_grid(self, section_dict):
         self.sections = grid_types.Sections(regular_grid=self.regular_grid, section_dict=section_dict)
         self.set_active('sections')
         return self.sections
 
+    # ? DEP?
     def create_centered_grid(self, centers, radius, resolution=None):
         """Initialize gravity grid. Deactivate the rest of the grids"""
         self.centered_grid = grid_types.CenteredGrid(centers, radius, resolution)
         # self.active_grids = np.zeros(4, dtype=bool)
         self.set_active('centered')
 
     def deactivate_all_grids(self):
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/grid_modules/diamond_square.py` & `gempy-2023.2.0b1/gempy/core/data/grid_modules/diamond_square.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-"""Implementation of Diamond-Square algorithm
-
-This algorithm is often used for random topography generation, following Fournier et al., 1982
-see https://en.wikipedia.org/wiki/Diamond-square_algorithm.
-
-Fournier, Alain; Fussell, Don; Carpenter, Loren (June 1982). "Computer rendering of stochastic models".
-Communications of the ACM. 25 (6): 371–384.
-
-Here the description from the wikipedia page:
-
-+++ begin Wikipedia +++
-
-The diamond-square algorithm begins with a 2D square array of width and
-height 2n + 1. The four corner points of the array must first be set to initial values. The diamond and square steps
-are then performed alternately until all array values have been set.
-
-The diamond step: For each square in the array, set the midpoint of that square to be the average of the four corner
-points plus a random value.
-
-The square step: For each diamond in the array, set the midpoint of that diamond to be the average of the four corner
-points plus a random value.
-
-At each iteration, the magnitude of the random value should be reduced.
-
-During the square steps, points located on the edges of the array will have only three adjacent values set rather
-than four. There are a number of ways to handle this complication - the simplest being to take the average of just
-the three adjacent values. Another option is to 'wrap around', taking the fourth value from the other side of the
-array. When used with consistent initial corner values this method also allows generated fractals to be stitched
-together without discontinuities.
-
-+++ end Wikipedia +++
-
-The implementations (in Python) I could find online were either difficult to understand or had many case
-selections, especially at edges. Here is a fully vectorized implementation, using padding at edges, to avoid
-all these case selections for a more straight-forward implementation (I hope).
-
-This implementation is also adjusted to work on non-square start matrices, and on reduced hierarchies with
-more initial (internal) points.
-
-Created on 10.04.2020
-
-@author: Florian Wellmann
-
-"""
-import numpy as np
-import matplotlib.pyplot as plt
-
-
-class DiaomondSquare(object):
-
-    def __init__(self, size: tuple = (16, 16), roughness: float = 0.5, z_min: float = 0, z_max:
-                 float = 1, r_type: chr = 'default', **kwds):
-        """Implementation of vectorized Diaomnd-Square algorithm for random topography generation
-
-        Args:
-            size (int, int): shape of grid to interpolate; note: the standard diamond-square algorithm
-                operates on a square grid with side length 2**n+1. This implementation is adjusted to non-square
-                grids with (2**n+1, 2**m+1). If the input size (int, int) is not matching to the ideal dimension,
-                the next bigger size is taken and the grid finally cut (lower left corner is kept);
-            roughness: roughness parameter, [0,1]: 0: deterministic interpolation, 1: very rough and bumpy (in standard
-                randomisation method - other options available in self.random_func())
-            z_min: minimum height of surface
-            z_max: maximum height of surface
-            seed: seed for random function to enable reproducibility and testing
-            r_type: 'basic', 'level_scale' (See below for details)
-            
-        Options for the randomization function (self.r_type) are:
-        - 'default': standard reduction
-        - 'level_scale' : uniform distribution between z_min, z_max, scaled by (level + 1)
-
-        """
-        self.size = size
-        # Create mesh with optimal size (2**n+1, 2**m+1)
-        # If the input size `self.size` does not match to these dimensions, then the next larger suitable
-        # size is chosen.
-        self.n = np.ceil(np.log2(self.size[0] - 1)).astype('int8')
-        self.m = np.ceil(np.log2(self.size[1] - 1)).astype('int8')
-        self.grid = np.zeros((2 ** self.n + 1, 2 ** self.m + 1))
-        self.roughness = roughness
-        self.z_min = z_min
-        self.z_max = z_max
-        if 'seed' in kwds:
-            np.random.seed(kwds['seed'])
-        self.base_rand_range = 1
-        self.r_type = r_type
-
-    def random_func(self, i, level_shape):
-        """Define random function to adjust range for subsequent steps
-
-        The random function type is defined on class level (self.r_type)
-        """
-
-        if self.r_type == 'default':
-            if self.roughness > 0:
-                rand_range = self.base_rand_range * 2 ** (- (1 - self.roughness) * i)
-                return np.random.uniform(-rand_range, rand_range, level_shape)
-            else:
-                return 0.
-
-        if self.r_type == 'long_range':
-            if self.roughness > 0:
-                rand_range = self.base_rand_range * 16 ** (- (1 - self.roughness) * i)
-                return np.random.uniform(-rand_range, rand_range, level_shape)
-            else:
-                return 0.
-
-        elif self.r_type == 'level_scale':
-            if self.roughness > 0:
-                return np.random.uniform(self.z_min, self.z_max,
-                                         level_shape) / (1 + i)
-            else:
-                return 0.
-
-        elif self.r_type == 'deterministic':
-            # No randomization at all - deterministic interpolation result
-            return 0.
-
-        else:
-            raise NotImplementedError("Random function type %s not implemented" % self.r_type)
-
-    def random_initialization(self, level='highest', verbose: bool=False):
-        """Initialize cells on speicifc hierarchy with random values
-
-        Args:
-            level = 'hightest', int : hierarchy level for interpolation (default: highest)
-            verbose: verbose output (default: False)
-
-        With highest hierarchy, we refer here to the largest diamond-square step, i.e. the corner points
-        for a square grid; Or, more formally: the diamond points for `min(self.n, self.m)`
-        """
-        if level == 'highest':
-            m_pow_max = min(self.n, self.m)
-        else:
-            m_pow_max = level
-
-        step_size = int(2 ** m_pow_max)
-        if verbose:
-            print("Initialize on step size %d" % step_size)
-
-        level_shape = self.grid[::step_size, ::step_size].shape
-
-        self.grid[::step_size, ::step_size] = np.random.uniform(0, 1, level_shape)  # self.random_func(0, level_shape)
-
-    def interpolate(self, level='highest'):
-        """Perform diamond-square interpolation
-
-        Args:
-            level = 'hightest', int : hierarchy level for interpolation (default: highest)
-
-        This step follows the conventional procedure:
-        Iterate over hierarchies and repeat:
-        2) Perform Diamond interpolation step
-        3) Perform Square interpolation step
-        4) Reduce roughness factor
-        """
-        if level == 'highest':
-            # determine highest hierarchy level (determined by shorter rectangle side)
-            m_pow_max = min(self.n, self.m)
-        else:
-            m_pow_max = level
-
-        for i, m_pow in enumerate(np.arange(m_pow_max)[::-1]):
-            self.perform_diamond_step(i, m_pow)
-            self.perform_square_step(i, m_pow)
-
-    def reset_grid(self):
-        """Reset grid back to zero values"""
-        self.grid[:, :] = 0
-
-    def perform_diamond_step(self, i: int, m_pow: int):
-        """Perform one diamond interpolation step on hierarchy m_pow
-
-        Note: for more details on the vectorized selection, see self.get_selection_diamond()
-        """
-        step_size = int(2 ** m_pow)
-
-        # Diamond step
-        # ----------------
-
-        # get shape of this step
-        level_shape = self.grid[step_size::2 * step_size, step_size::2 * step_size].shape
-
-        self.grid[step_size::2 * step_size, step_size::2 * step_size] = \
-            (self.grid[:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] +
-             self.grid[:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] +
-             self.grid[2 * step_size::2 * step_size, :-2 * step_size:2 * step_size] +
-             self.grid[2 * step_size::2 * step_size, 2 * step_size::2 * step_size]) / \
-            4. + \
-            self.random_func(i, level_shape)
-
-        # np.random.uniform(-rand_range, rand_range, level_shape)
-
-        # self.d * 2**()
-        # self.roughness ** i * (np.random.random(step_shape) - 0.5)
-
-        # (np.random.random(step_shape) - 0.5) * i * self.roughness
-
-    def perform_square_step(self, i: int, m_pow: int):
-        """Perform one square interpolation step on hierarchy m_pow
-
-        Note: for more details on the vectorized selection, see self.get_selection_square()
-        """
-        step_size = int(2 ** m_pow)
-
-        # pad cells with zero value
-        z_pad = np.pad(self.grid, step_size, mode='constant')
-
-        # also create a grid for division to divide only by 3 on borders
-        grid_div = np.ones_like(self.grid[1:-1, 1:-1]) * 4.
-        grid_div = np.pad(grid_div, step_size + 1, mode='constant', constant_values=3.)
-
-        # Checkerboard odd
-        # ----------------
-
-        # get shape of this step
-        level_shape = grid_div[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size].shape
-
-        z_pad[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = \
-            (z_pad[step_size::2 * step_size, step_size:-2 * step_size:2 * step_size] +
-             z_pad[step_size::2 * step_size, 3 * step_size:-step_size:2 * step_size] +
-             z_pad[:-step_size:2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] +
-             z_pad[2 * step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size]) / \
-            grid_div[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] + \
-            self.random_func(i, level_shape)
-
-        # np.random.uniform(-rand_range, rand_range, level_shape)
-
-        #    self.roughness ** i * (np.random.random(step_shape) - 0.5)
-
-        # (np.random.random(step_shape) - 0.5) * i * self.roughness
-
-        # Checkerboard even
-        # -----------------
-
-        # get shape of this step
-        level_shape = z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size].shape
-
-        # check-even, values to interpolate:
-        z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = \
-            (z_pad[2 * step_size:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] +
-             z_pad[2 * step_size:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] +
-             z_pad[step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] +
-             z_pad[3 * step_size::2 * step_size, step_size:-step_size:2 * step_size]) / \
-            grid_div[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] + \
-            self.random_func(i, level_shape)
-
-        # np.random.uniform(-rand_range, rand_range, level_shape)
-
-        # self.roughness ** i * (np.random.random(step_shape) - 0.5)
-
-        # (np.random.random(step_shape) - 0.5) * i * self.roughness
-
-        # assign results back to self.grid
-        self.grid = z_pad[step_size:-step_size, step_size:-step_size]
-
-    def get_selection_diamond(self, m_pow: int):
-        """get selected points for diamond step on grid z on hierarchy m
-
-        This method is mostly implemented for testing and visualization purposes.
-        """
-
-        step_size = int(2 ** m_pow)
-
-        z = np.zeros_like(self.grid, dtype='int8')
-
-        # points to interpolate
-        z[step_size::2 * step_size, step_size::2 * step_size] = 1
-
-        # top left
-        z[:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] = 2
-
-        # top right
-        z[:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] = 2
-
-        # bottom left
-        z[2 * step_size::2 * step_size, :-2 * step_size:2 * step_size] = 2
-
-        # bottom right
-        z[2 * step_size::2 * step_size, 2 * step_size::2 * step_size] = 2
-
-        return z
-
-    def get_selection_square(self, m_pow: int):
-        """Plot selected points for square step on grid z on hierarchy m
-
-        This method is mostly implemented for testing and visualization purposes.
-        """
-        z = np.zeros_like(self.grid, dtype='int8')
-        step_size = int(2 ** m_pow)
-
-        # pad cells with zero value
-        z_pad = np.pad(z, step_size, mode='constant')
-
-        # Checkerboard odd
-        # ----------------
-
-        # check-odd, values to interpolate:
-        z_pad[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 1
-
-        # check-odd, left
-        z_pad[step_size::2 * step_size, step_size:-2 * step_size:2 * step_size] = 2
-
-        # check-odd, right
-        z_pad[step_size::2 * step_size, 3 * step_size:-step_size:2 * step_size] = 2
-
-        # check-odd, top
-        z_pad[:-step_size:2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 2
-
-        # check-odd, bottom
-        z_pad[2 * step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 2
-
-        # Checkerboard even
-        # -----------------
-
-        # check-even, values to interpolate:
-        z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = 1
-
-        # check-even, left:
-        z_pad[2 * step_size:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] = 2
-
-        # check-even, right:
-        z_pad[2 * step_size:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] = 2
-
-        # check-even, top:
-        z_pad[step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = 2
-
-        # check-even, bottom:
-        z_pad[3 * step_size::2 * step_size, step_size:-step_size:2 * step_size] = 2
-
-        return z_pad
-
-    def plot_diamond_and_square(self, pad=False):
-        """Plot selected points for diamond and square step for all hierarchies side by side"""
-
-        m_pow_max = min(self.n, self.m)
-
-        shape_ratio = self.n / self.m
-
-        f, axes = plt.subplots(2, m_pow_max, figsize=(12, 12 * shape_ratio / m_pow_max * 2))
-
-        for i, m_pow in enumerate(np.arange(m_pow_max)[::-1]):
-            m = 2 ** m_pow
-            # z_zero = np.zeros_like(self.grid)
-            z_diamond = self.get_selection_diamond(m_pow)
-            z_square = self.get_selection_square(m_pow)
-            if pad:
-                z_pad = np.pad(z_diamond, m, mode='constant')
-                axes[0, i].imshow(z_pad, cmap='viridis', vmin=0, vmax=2)
-                axes[1, i].imshow(z_square, cmap='viridis', vmin=0, vmax=2)
-            else:
-                axes[0, i].imshow(z_diamond, cmap='viridis', vmin=0, vmax=2)
-                axes[1, i].imshow(z_square[m:-m, m:-m], cmap='viridis', vmin=0, vmax=2)
+"""Implementation of Diamond-Square algorithm
+
+This algorithm is often used for random topography generation, following Fournier et al., 1982
+see https://en.wikipedia.org/wiki/Diamond-square_algorithm.
+
+Fournier, Alain; Fussell, Don; Carpenter, Loren (June 1982). "Computer rendering of stochastic models".
+Communications of the ACM. 25 (6): 371–384.
+
+Here the description from the wikipedia page:
+
++++ begin Wikipedia +++
+
+The diamond-square algorithm begins with a 2D square array of width and
+height 2n + 1. The four corner points of the array must first be set to initial values. The diamond and square steps
+are then performed alternately until all array values have been set.
+
+The diamond step: For each square in the array, set the midpoint of that square to be the average of the four corner
+points plus a random value.
+
+The square step: For each diamond in the array, set the midpoint of that diamond to be the average of the four corner
+points plus a random value.
+
+At each iteration, the magnitude of the random value should be reduced.
+
+During the square steps, points located on the edges of the array will have only three adjacent values set rather
+than four. There are a number of ways to handle this complication - the simplest being to take the average of just
+the three adjacent values. Another option is to 'wrap around', taking the fourth value from the other side of the
+array. When used with consistent initial corner values this method also allows generated fractals to be stitched
+together without discontinuities.
+
++++ end Wikipedia +++
+
+The implementations (in Python) I could find online were either difficult to understand or had many case
+selections, especially at edges. Here is a fully vectorized implementation, using padding at edges, to avoid
+all these case selections for a more straight-forward implementation (I hope).
+
+This implementation is also adjusted to work on non-square start matrices, and on reduced hierarchies with
+more initial (internal) points.
+
+Created on 10.04.2020
+
+@author: Florian Wellmann
+
+"""
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+class DiaomondSquare(object):
+
+    def __init__(self, size: tuple = (16, 16), roughness: float = 0.5, z_min: float = 0, z_max:
+                 float = 1, r_type: chr = 'default', **kwds):
+        """Implementation of vectorized Diaomnd-Square algorithm for random topography generation
+
+        Args:
+            size (int, int): shape of grid to interpolate; note: the standard diamond-square algorithm
+                operates on a square grid with side length 2**n+1. This implementation is adjusted to non-square
+                grids with (2**n+1, 2**m+1). If the input size (int, int) is not matching to the ideal dimension,
+                the next bigger size is taken and the grid finally cut (lower left corner is kept);
+            roughness: roughness parameter, [0,1]: 0: deterministic interpolation, 1: very rough and bumpy (in standard
+                randomisation method - other options available in self.random_func())
+            z_min: minimum height of surface
+            z_max: maximum height of surface
+            seed: seed for random function to enable reproducibility and testing
+            r_type: 'basic', 'level_scale' (See below for details)
+            
+        Options for the randomization function (self.r_type) are:
+        - 'default': standard reduction
+        - 'level_scale' : uniform distribution between z_min, z_max, scaled by (level + 1)
+
+        """
+        self.size = size
+        # Create mesh with optimal size (2**n+1, 2**m+1)
+        # If the input size `self.size` does not match to these dimensions, then the next larger suitable
+        # size is chosen.
+        self.n = np.ceil(np.log2(self.size[0] - 1)).astype('int8')
+        self.m = np.ceil(np.log2(self.size[1] - 1)).astype('int8')
+        self.grid = np.zeros((2 ** self.n + 1, 2 ** self.m + 1))
+        self.roughness = roughness
+        self.z_min = z_min
+        self.z_max = z_max
+        if 'seed' in kwds:
+            np.random.seed(kwds['seed'])
+        self.base_rand_range = 1
+        self.r_type = r_type
+
+    def random_func(self, i, level_shape):
+        """Define random function to adjust range for subsequent steps
+
+        The random function type is defined on class level (self.r_type)
+        """
+
+        if self.r_type == 'default':
+            if self.roughness > 0:
+                rand_range = self.base_rand_range * 2 ** (- (1 - self.roughness) * i)
+                return np.random.uniform(-rand_range, rand_range, level_shape)
+            else:
+                return 0.
+
+        if self.r_type == 'long_range':
+            if self.roughness > 0:
+                rand_range = self.base_rand_range * 16 ** (- (1 - self.roughness) * i)
+                return np.random.uniform(-rand_range, rand_range, level_shape)
+            else:
+                return 0.
+
+        elif self.r_type == 'level_scale':
+            if self.roughness > 0:
+                return np.random.uniform(self.z_min, self.z_max,
+                                         level_shape) / (1 + i)
+            else:
+                return 0.
+
+        elif self.r_type == 'deterministic':
+            # No randomization at all - deterministic interpolation result
+            return 0.
+
+        else:
+            raise NotImplementedError("Random function type %s not implemented" % self.r_type)
+
+    def random_initialization(self, level='highest', verbose: bool=False):
+        """Initialize cells on speicifc hierarchy with random values
+
+        Args:
+            level = 'hightest', int : hierarchy level for interpolation (default: highest)
+            verbose: verbose output (default: False)
+
+        With highest hierarchy, we refer here to the largest diamond-square step, i.e. the corner points
+        for a square grid; Or, more formally: the diamond points for `min(self.n, self.m)`
+        """
+        if level == 'highest':
+            m_pow_max = min(self.n, self.m)
+        else:
+            m_pow_max = level
+
+        step_size = int(2 ** m_pow_max)
+        if verbose:
+            print("Initialize on step size %d" % step_size)
+
+        level_shape = self.grid[::step_size, ::step_size].shape
+
+        self.grid[::step_size, ::step_size] = np.random.uniform(0, 1, level_shape)  # self.random_func(0, level_shape)
+
+    def interpolate(self, level='highest'):
+        """Perform diamond-square interpolation
+
+        Args:
+            level = 'hightest', int : hierarchy level for interpolation (default: highest)
+
+        This step follows the conventional procedure:
+        Iterate over hierarchies and repeat:
+        2) Perform Diamond interpolation step
+        3) Perform Square interpolation step
+        4) Reduce roughness factor
+        """
+        if level == 'highest':
+            # determine highest hierarchy level (determined by shorter rectangle side)
+            m_pow_max = min(self.n, self.m)
+        else:
+            m_pow_max = level
+
+        for i, m_pow in enumerate(np.arange(m_pow_max)[::-1]):
+            self.perform_diamond_step(i, m_pow)
+            self.perform_square_step(i, m_pow)
+
+    def reset_grid(self):
+        """Reset grid back to zero values"""
+        self.grid[:, :] = 0
+
+    def perform_diamond_step(self, i: int, m_pow: int):
+        """Perform one diamond interpolation step on hierarchy m_pow
+
+        Note: for more details on the vectorized selection, see self.get_selection_diamond()
+        """
+        step_size = int(2 ** m_pow)
+
+        # Diamond step
+        # ----------------
+
+        # get shape of this step
+        level_shape = self.grid[step_size::2 * step_size, step_size::2 * step_size].shape
+
+        self.grid[step_size::2 * step_size, step_size::2 * step_size] = \
+            (self.grid[:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] +
+             self.grid[:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] +
+             self.grid[2 * step_size::2 * step_size, :-2 * step_size:2 * step_size] +
+             self.grid[2 * step_size::2 * step_size, 2 * step_size::2 * step_size]) / \
+            4. + \
+            self.random_func(i, level_shape)
+
+        # np.random.uniform(-rand_range, rand_range, level_shape)
+
+        # self.d * 2**()
+        # self.roughness ** i * (np.random.random(step_shape) - 0.5)
+
+        # (np.random.random(step_shape) - 0.5) * i * self.roughness
+
+    def perform_square_step(self, i: int, m_pow: int):
+        """Perform one square interpolation step on hierarchy m_pow
+
+        Note: for more details on the vectorized selection, see self.get_selection_square()
+        """
+        step_size = int(2 ** m_pow)
+
+        # pad cells with zero value
+        z_pad = np.pad(self.grid, step_size, mode='constant')
+
+        # also create a grid for division to divide only by 3 on borders
+        grid_div = np.ones_like(self.grid[1:-1, 1:-1]) * 4.
+        grid_div = np.pad(grid_div, step_size + 1, mode='constant', constant_values=3.)
+
+        # Checkerboard odd
+        # ----------------
+
+        # get shape of this step
+        level_shape = grid_div[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size].shape
+
+        z_pad[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = \
+            (z_pad[step_size::2 * step_size, step_size:-2 * step_size:2 * step_size] +
+             z_pad[step_size::2 * step_size, 3 * step_size:-step_size:2 * step_size] +
+             z_pad[:-step_size:2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] +
+             z_pad[2 * step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size]) / \
+            grid_div[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] + \
+            self.random_func(i, level_shape)
+
+        # np.random.uniform(-rand_range, rand_range, level_shape)
+
+        #    self.roughness ** i * (np.random.random(step_shape) - 0.5)
+
+        # (np.random.random(step_shape) - 0.5) * i * self.roughness
+
+        # Checkerboard even
+        # -----------------
+
+        # get shape of this step
+        level_shape = z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size].shape
+
+        # check-even, values to interpolate:
+        z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = \
+            (z_pad[2 * step_size:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] +
+             z_pad[2 * step_size:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] +
+             z_pad[step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] +
+             z_pad[3 * step_size::2 * step_size, step_size:-step_size:2 * step_size]) / \
+            grid_div[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] + \
+            self.random_func(i, level_shape)
+
+        # np.random.uniform(-rand_range, rand_range, level_shape)
+
+        # self.roughness ** i * (np.random.random(step_shape) - 0.5)
+
+        # (np.random.random(step_shape) - 0.5) * i * self.roughness
+
+        # assign results back to self.grid
+        self.grid = z_pad[step_size:-step_size, step_size:-step_size]
+
+    def get_selection_diamond(self, m_pow: int):
+        """get selected points for diamond step on grid z on hierarchy m
+
+        This method is mostly implemented for testing and visualization purposes.
+        """
+
+        step_size = int(2 ** m_pow)
+
+        z = np.zeros_like(self.grid, dtype='int8')
+
+        # points to interpolate
+        z[step_size::2 * step_size, step_size::2 * step_size] = 1
+
+        # top left
+        z[:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] = 2
+
+        # top right
+        z[:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] = 2
+
+        # bottom left
+        z[2 * step_size::2 * step_size, :-2 * step_size:2 * step_size] = 2
+
+        # bottom right
+        z[2 * step_size::2 * step_size, 2 * step_size::2 * step_size] = 2
+
+        return z
+
+    def get_selection_square(self, m_pow: int):
+        """Plot selected points for square step on grid z on hierarchy m
+
+        This method is mostly implemented for testing and visualization purposes.
+        """
+        z = np.zeros_like(self.grid, dtype='int8')
+        step_size = int(2 ** m_pow)
+
+        # pad cells with zero value
+        z_pad = np.pad(z, step_size, mode='constant')
+
+        # Checkerboard odd
+        # ----------------
+
+        # check-odd, values to interpolate:
+        z_pad[step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 1
+
+        # check-odd, left
+        z_pad[step_size::2 * step_size, step_size:-2 * step_size:2 * step_size] = 2
+
+        # check-odd, right
+        z_pad[step_size::2 * step_size, 3 * step_size:-step_size:2 * step_size] = 2
+
+        # check-odd, top
+        z_pad[:-step_size:2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 2
+
+        # check-odd, bottom
+        z_pad[2 * step_size::2 * step_size, 2 * step_size:-2 * step_size:2 * step_size] = 2
+
+        # Checkerboard even
+        # -----------------
+
+        # check-even, values to interpolate:
+        z_pad[2 * step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = 1
+
+        # check-even, left:
+        z_pad[2 * step_size:-2 * step_size:2 * step_size, :-2 * step_size:2 * step_size] = 2
+
+        # check-even, right:
+        z_pad[2 * step_size:-2 * step_size:2 * step_size, 2 * step_size::2 * step_size] = 2
+
+        # check-even, top:
+        z_pad[step_size:-2 * step_size:2 * step_size, step_size:-step_size:2 * step_size] = 2
+
+        # check-even, bottom:
+        z_pad[3 * step_size::2 * step_size, step_size:-step_size:2 * step_size] = 2
+
+        return z_pad
+
+    def plot_diamond_and_square(self, pad=False):
+        """Plot selected points for diamond and square step for all hierarchies side by side"""
+
+        m_pow_max = min(self.n, self.m)
+
+        shape_ratio = self.n / self.m
+
+        f, axes = plt.subplots(2, m_pow_max, figsize=(12, 12 * shape_ratio / m_pow_max * 2))
+
+        for i, m_pow in enumerate(np.arange(m_pow_max)[::-1]):
+            m = 2 ** m_pow
+            # z_zero = np.zeros_like(self.grid)
+            z_diamond = self.get_selection_diamond(m_pow)
+            z_square = self.get_selection_square(m_pow)
+            if pad:
+                z_pad = np.pad(z_diamond, m, mode='constant')
+                axes[0, i].imshow(z_pad, cmap='viridis', vmin=0, vmax=2)
+                axes[1, i].imshow(z_square, cmap='viridis', vmin=0, vmax=2)
+            else:
+                axes[0, i].imshow(z_diamond, cmap='viridis', vmin=0, vmax=2)
+                axes[1, i].imshow(z_square[m:-m, m:-m], cmap='viridis', vmin=0, vmax=2)
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/grid_modules/topography.py` & `gempy-2023.2.0b1/gempy/core/data/grid_modules/topography.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import warnings
-from typing import Optional
-
-import numpy as np
-
-from gempy.core.data.grid_modules.grid_types import RegularGrid
-from gempy.modules.grids.create_topography import _LoadDEMArtificial
-
-from gempy.optional_dependencies import require_skimage
-
-
-class Topography:
-    """
-    Object to include topography in the model.
-
-    Notes:
-        This always assumes that the topography we pass fits perfectly the extent
-
-    """
-
-    def __init__(self, regular_grid: RegularGrid, values_2d: Optional[np.ndarray] = None):
-
-        self._mask_topo = None
-        self._regular_grid = regular_grid
-
-        # Values (n, 3)
-        self.values = np.zeros((0, 3))
-
-        # Values (n, n, 3)
-        self.values_2d = np.zeros((0, 0, 3))
-
-        # Shape original
-        self.raster_shape = tuple()
-
-        # Topography Resolution
-        self.resolution = np.zeros((0, 3))
-
-        # Source for the
-        self.source = None
-
-        # Coords
-        self._x = None
-        self._y = None
-
-        if values_2d is not None:
-            self.set_values(values_2d)
-
-    @classmethod
-    def from_subsurface_structured_data(cls, structured_data: 'subsurface.StructuredData', regular_grid: RegularGrid):
-        """Creates a topography object from a subsurface structured data object
-
-        Args:
-            structured_data (subsurface.StructuredData): Structured data object
-
-        Returns:
-            :class:`gempy.core.grid_modules.topography.Topography`
-
-        """
-
-        # Generate meshgrid for x and y coordinates
-        ds = structured_data.data
-        x_vals, y_vals = np.meshgrid(ds['x'], ds['y'], indexing='ij')
-
-        # Reshape arrays for stacking
-        x_vals = x_vals[:, :, np.newaxis]  # shape (73, 34, 1)
-        y_vals = y_vals[:, :, np.newaxis]  # shape (73, 34, 1)
-        topography_vals = ds['topography'].values[:, :, np.newaxis]  # shape (73, 34, 1)
-        # Stack along the last dimension
-        result = np.concatenate([x_vals, y_vals, topography_vals], axis=2)  # shape (73, 34, 3)
-
-        return cls(regular_grid=regular_grid, values_2d=result)
-
-    @property
-    def extent(self):
-        return self._regular_grid.extent
-
-    @property
-    def regular_grid_resolution(self):
-        return self._regular_grid.resolution
-
-    @property
-    def x(self):
-        if self._x is not None:
-            return self._x
-        else:
-            val = self.values[:, 0]
-            val.sort()
-            return np.unique(val)
-
-    @property
-    def y(self):
-        if self._y is not None:
-            return self._y
-        else:
-            val = self.values[:, 1]
-            val.sort()
-            return np.unique(val)
-
-    def set_values(self, values_2d: np.ndarray):
-        """General method to set topography
-
-        Args:
-            values_2d (numpy.ndarray[float,float, 3]): array with the XYZ values
-             in 2D
-
-        Returns:
-            :class:`gempy.core.grid_modules.topography.Topography`
-
-
-        """
-        # Original topography data
-        self.values_2d = values_2d
-        self.resolution = values_2d.shape[:2]
-
-        # n,3 array
-        self.values = values_2d.reshape((-1, 3), order='C')
-        return self
-
-    @property
-    def topography_mask(self):
-        """This method takes a topography grid of the same extent as the regular
-         grid and creates a mask of voxels
-
-        """
-
-        # * Check if the topography is the same as the cached one and if so, return the cached mask
-        if self._mask_topo is not None:
-            return self._mask_topo
-
-        # interpolate topography values to the regular grid
-        skimage = require_skimage()
-        regular_grid_topo = skimage.transform.resize(
-            image=self.values_2d,
-            output_shape=(self.regular_grid_resolution[0], self.regular_grid_resolution[1]),
-            mode='constant',
-            anti_aliasing=False,
-            preserve_range=True
-        )
-
-        # Adjust the topography to be lower by half a voxel height
-        # Assumes your voxel heights are uniform and can be calculated as the total height divided by resolution
-        voxel_height = self._regular_grid.dz * 2
-        regular_grid_topo = regular_grid_topo - voxel_height
-
-        # Reshape the Z values of the regular grid to 3d
-        values_3d = self._regular_grid.values[:, 2].reshape(self.regular_grid_resolution)
-        if regular_grid_topo.ndim == 3:
-            regular_grid_topo_z = regular_grid_topo[:, :, [2]]
-        elif regular_grid_topo.ndim == 2:
-            regular_grid_topo_z = regular_grid_topo
-        else:
-            raise ValueError()
-        mask = np.greater(values_3d[:, :, :], regular_grid_topo_z)
-
-        self._mask_topo = mask
-        return self._mask_topo
-
-    def resize_topo(self):
-        skimage = require_skimage()
-        regular_grid_topo = skimage.transform.resize(
-            self.values_2d,
-            (self.regular_grid_resolution[0], self.regular_grid_resolution[1]),
-            mode='constant',
-            anti_aliasing=False, preserve_range=True)
-
-        return regular_grid_topo
-
-    def load_random_hills(self, **kwargs):
-        warnings.warn('This function is deprecated. Use load_from_random instead', DeprecationWarning)
-        if 'extent' in kwargs:
-            self.extent = kwargs.pop('extent')
-
-        if 'resolution' in kwargs:
-            self.regular_grid_resolution = kwargs.pop('resolution')
-
-        dem = _LoadDEMArtificial(extent=self.extent,
-                                 resolution=self.regular_grid_resolution, **kwargs)
-
-        self._x, self._y = dem.x, dem.y
-        self.set_values(dem.get_values())
-
-    def save(self, path):
-        np.save(path, self.values_2d)
-
-    def load(self, path):
-        self.set_values(np.load(path))
-        self._x, self._y = None, None
-        return self.values
-
-    def load_from_saved(self, *args, **kwargs):
-        self.load(*args, **kwargs)
+import warnings
+from typing import Optional
+
+import numpy as np
+
+from gempy.core.data.grid_modules.grid_types import RegularGrid
+from gempy.modules.grids.create_topography import _LoadDEMArtificial
+
+from gempy.optional_dependencies import require_skimage
+
+
+class Topography:
+    """
+    Object to include topography in the model.
+
+    Notes:
+        This always assumes that the topography we pass fits perfectly the extent
+
+    """
+
+    def __init__(self, regular_grid: RegularGrid, values_2d: Optional[np.ndarray] = None):
+
+        self._mask_topo = None
+        self._regular_grid = regular_grid
+
+        # Values (n, 3)
+        self.values = np.zeros((0, 3))
+
+        # Values (n, n, 3)
+        self.values_2d = np.zeros((0, 0, 3))
+
+        # Shape original
+        self.raster_shape = tuple()
+
+        # Topography Resolution
+        self.resolution = np.zeros((0, 3))
+
+        # Source for the
+        self.source = None
+
+        # Coords
+        self._x = None
+        self._y = None
+
+        if values_2d is not None:
+            self.set_values(values_2d)
+
+    @classmethod
+    def from_subsurface_structured_data(cls, structured_data: 'subsurface.StructuredData', regular_grid: RegularGrid):
+        """Creates a topography object from a subsurface structured data object
+
+        Args:
+            structured_data (subsurface.StructuredData): Structured data object
+
+        Returns:
+            :class:`gempy.core.grid_modules.topography.Topography`
+
+        """
+
+        # Generate meshgrid for x and y coordinates
+        ds = structured_data.data
+        x_vals, y_vals = np.meshgrid(ds['x'], ds['y'], indexing='ij')
+
+        # Reshape arrays for stacking
+        x_vals = x_vals[:, :, np.newaxis]  # shape (73, 34, 1)
+        y_vals = y_vals[:, :, np.newaxis]  # shape (73, 34, 1)
+        topography_vals = ds['topography'].values[:, :, np.newaxis]  # shape (73, 34, 1)
+        # Stack along the last dimension
+        result = np.concatenate([x_vals, y_vals, topography_vals], axis=2)  # shape (73, 34, 3)
+
+        return cls(regular_grid=regular_grid, values_2d=result)
+
+    @property
+    def extent(self):
+        return self._regular_grid.extent
+
+    @property
+    def regular_grid_resolution(self):
+        return self._regular_grid.resolution
+
+    @property
+    def x(self):
+        if self._x is not None:
+            return self._x
+        else:
+            val = self.values[:, 0].copy()
+            val.sort()
+            return np.unique(val)
+
+    @property
+    def y(self):
+        if self._y is not None:
+            return self._y
+        else:
+            val = self.values[:, 1].copy()
+            val.sort()
+            return np.unique(val)
+
+    def set_values(self, values_2d: np.ndarray):
+        """General method to set topography
+
+        Args:
+            values_2d (numpy.ndarray[float,float, 3]): array with the XYZ values
+             in 2D
+
+        Returns:
+            :class:`gempy.core.grid_modules.topography.Topography`
+
+
+        """
+        # Original topography data
+        self.values_2d = values_2d
+        self.resolution = values_2d.shape[:2]
+
+        # n,3 array
+        self.values = values_2d.reshape((-1, 3), order='C')
+        return self
+
+    @property
+    def topography_mask(self):
+        """This method takes a topography grid of the same extent as the regular
+         grid and creates a mask of voxels
+
+        """
+
+        # * Check if the topography is the same as the cached one and if so, return the cached mask
+        if self._mask_topo is not None:
+            return self._mask_topo
+
+        # interpolate topography values to the regular grid
+        skimage = require_skimage()
+        regular_grid_topo = skimage.transform.resize(
+            image=self.values_2d,
+            output_shape=(self.regular_grid_resolution[0], self.regular_grid_resolution[1]),
+            mode='constant',
+            anti_aliasing=False,
+            preserve_range=True
+        )
+
+        # Adjust the topography to be lower by half a voxel height
+        # Assumes your voxel heights are uniform and can be calculated as the total height divided by resolution
+        voxel_height = self._regular_grid.dz * 2
+        regular_grid_topo = regular_grid_topo - voxel_height
+
+        # Reshape the Z values of the regular grid to 3d
+        values_3d = self._regular_grid.values[:, 2].reshape(self.regular_grid_resolution)
+        if regular_grid_topo.ndim == 3:
+            regular_grid_topo_z = regular_grid_topo[:, :, [2]]
+        elif regular_grid_topo.ndim == 2:
+            regular_grid_topo_z = regular_grid_topo
+        else:
+            raise ValueError()
+        mask = np.greater(values_3d[:, :, :], regular_grid_topo_z)
+
+        self._mask_topo = mask
+        return self._mask_topo
+
+    def resize_topo(self):
+        skimage = require_skimage()
+        regular_grid_topo = skimage.transform.resize(
+            self.values_2d,
+            (self.regular_grid_resolution[0], self.regular_grid_resolution[1]),
+            mode='constant',
+            anti_aliasing=False, preserve_range=True)
+
+        return regular_grid_topo
+
+    def load_random_hills(self, **kwargs):
+        warnings.warn('This function is deprecated. Use load_from_random instead', DeprecationWarning)
+        if 'extent' in kwargs:
+            self.extent = kwargs.pop('extent')
+
+        if 'resolution' in kwargs:
+            self.regular_grid_resolution = kwargs.pop('resolution')
+
+        dem = _LoadDEMArtificial(extent=self.extent,
+                                 resolution=self.regular_grid_resolution, **kwargs)
+
+        self._x, self._y = dem.x, dem.y
+        self.set_values(dem.get_values())
+
+    def save(self, path):
+        np.save(path, self.values_2d)
+
+    def load(self, path):
+        self.set_values(np.load(path))
+        self._x, self._y = None, None
+        return self.values
+
+    def load_from_saved(self, *args, **kwargs):
+        self.load(*args, **kwargs)
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/importer_helper.py` & `gempy-2023.2.0b1/gempy/core/data/importer_helper.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-﻿from dataclasses import dataclass
-from typing import Optional
-
-
-@dataclass
-class ImporterHelper:
-    path_to_surface_points: Optional[str] 
-    path_to_orientations: Optional[str]
-    
-    hash_surface_points: Optional[str] = None
-    hash_orientations: Optional[str] = None
-    
-    coord_x_name: Optional[str] = "X"
-    coord_y_name: Optional[str] = "Y"
-    coord_z_name: Optional[str] = "Z"
-    surface_name: Optional[str] = "formation"
-    
-    gx_name: Optional[str] = "G_x"
-    gy_name: Optional[str] = "G_y"
-    gz_name: Optional[str] = "G_z"
-    
-    pandas_reader_kwargs: Optional[dict] = None
-    
-    
+﻿from dataclasses import dataclass
+from typing import Optional
+
+
+@dataclass
+class ImporterHelper:
+    path_to_surface_points: Optional[str] 
+    path_to_orientations: Optional[str]
+    
+    hash_surface_points: Optional[str] = None
+    hash_orientations: Optional[str] = None
+    
+    coord_x_name: Optional[str] = "X"
+    coord_y_name: Optional[str] = "Y"
+    coord_z_name: Optional[str] = "Z"
+    surface_name: Optional[str] = "formation"
+    
+    gx_name: Optional[str] = "G_x"
+    gy_name: Optional[str] = "G_y"
+    gz_name: Optional[str] = "G_z"
+    
+    pandas_reader_kwargs: Optional[dict] = None
+    
+    
     # ? Add here pandas reader options
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/orientations.py` & `gempy-2023.2.0b1/gempy/core/data/orientations.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/core/data/structural_element.py` & `gempy-2023.2.0b1/gempy/core/data/structural_element.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/core/data/structural_frame.py` & `gempy-2023.2.0b1/gempy/core/data/structural_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,21 +32,29 @@
     def get_element_by_name(self, element_name: str) -> StructuralElement:
         elements: Generator = (group.get_element_by_name(element_name) for group in self.structural_groups)
         valid_elements: Generator = (element for element in elements if element is not None)
         element = next(valid_elements, None)
         if element is None:
             raise ValueError(f"Element with name {element_name} not found in the structural frame.")
         return element
-
+    
     def get_group_by_name(self, group_name: str) -> StructuralGroup:
         groups: Generator = (group for group in self.structural_groups if group.name == group_name)
         group = next(groups, None)
         if group is None:
             raise ValueError(f"Group with name {group_name} not found in the structural frame.")
         return group
+    
+    def get_group_by_element(self, element: StructuralElement) -> StructuralGroup:
+        groups: Generator = (group for group in self.structural_groups if element in group.elements)
+        group = next(groups, None)
+        if group is None:
+            raise ValueError(f"Element {element.name} not found in any group in the structural frame.")
+        return group
+        
 
     def append_group(self, group: StructuralGroup):
         self.structural_groups.append(group)
 
     def insert_group(self, index: int, group: StructuralGroup):
         self.structural_groups.insert(index, group)
 
@@ -153,14 +161,19 @@
     def structural_elements(self) -> list[StructuralElement]:
         """Returns a list of all structural elements across the structural groups."""
         elements = []
         for group in self.structural_groups:
             elements.extend(group.elements)
         elements.append(self._basement_element)
         return elements
+    
+    @property
+    def n_elements(self) -> int:
+        """Returns the total number of elements in the structural frame."""
+        return len(self.structural_elements)
 
     @property
     def _basement_element(self) -> StructuralElement:
         basement = StructuralElement(
             name="basement",
             surface_points=SurfacePointsTable(data=np.zeros(0, dtype=SurfacePointsTable.dt)),
             orientations=OrientationsTable(data=np.zeros(0, dtype=OrientationsTable.dt)),
@@ -215,14 +228,24 @@
                 group.fault_relations = FaultsRelationSpecialCase.OFFSET_ALL
                 group.structural_relation = StackRelationType.FAULT
             elif not any_younger_groups_affected:
                 group.fault_relations = FaultsRelationSpecialCase.OFFSET_NONE
             else:  # * A specific set of groups are affected
                 group.fault_relations = [g for j, g in enumerate(self.structural_groups) if affected_groups[j]]
                 group.structural_relation = StackRelationType.FAULT
+    
+    @property
+    def group_is_fault(self) -> list[bool]:
+        """Returns a list of booleans indicating if each structural element is a fault."""
+        return [group.is_fault for group in self.structural_groups]
+    
+    @property
+    def group_is_lithology(self) -> list[bool]:
+        """Returns a list of booleans indicating if each structural element is a lithology."""
+        return [group.is_lithology for group in self.structural_groups]
 
     @property
     def input_data_descriptor(self):
         """Returns a descriptor for the input data, detailing the relations and faults between groups."""
         # TODO: This should have the exact same dirty logic as interpolation_input
 
         self._validate_faults_relations()
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/structural_group.py` & `gempy-2023.2.0b1/gempy/core/data/structural_group.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,110 @@
-﻿import pprint
-from abc import ABC
-from dataclasses import dataclass, field
-from enum import Enum, auto
-from typing import Optional, Union, Generator
-
-from gempy_engine.core.data.kernel_classes.faults import FaultsData
-from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
-from gempy_engine.core.data.stack_relation_type import StackRelationType
-from gempy.core.data.structural_element import StructuralElement
-
-
-class FaultsRelationSpecialCase(Enum):
-    OFFSET_FORMATIONS = auto()
-    OFFSET_NONE = auto()
-    OFFSET_ALL = auto()
-    
-    
-@dataclass
-class StructuralGroup(ABC):
-    """
-    An abstract base class that represents a structural group within a geological model.
-    
-    """
-    name: str  #: The name of the structural group.
-    
-    elements: list[StructuralElement] = field(repr=False)  #: A list of structural elements within the group.
-    structural_relation: StackRelationType  #: The type of relation between the structural elements in the group.
-
-    #: Relations with other groups in terms of faults.
-    fault_relations: Optional[Union[list["StructuralGroup"], FaultsRelationSpecialCase]] = field(default=None, repr=False)
-    faults_input_data: Optional[FaultsData] = field(default=None, repr=False)
-    
-    solution: Optional[RawArraysSolution] = field(init=False, default=None, repr=False)  #: Solution related to this group from geological computations.
-    
-    
-    def __post_init__(self):
-        if not isinstance(self.elements, list):
-            raise TypeError("elements must be a list of StructuralElement objects.")
-        for e in self.elements:
-            if not isinstance(e, StructuralElement):
-                raise TypeError("elements must be a list of StructuralElement objects.")
-        
-    def __repr__(self):
-        elements_repr = ',\n'.join([repr(e) for e in self.elements])
-        return f"StructuralGroup(\n" \
-               f"\tname={self.name},\n" \
-               f"\tstructural_relation={self.structural_relation},\n" \
-               f"\telements=[\n{elements_repr}\n]\n)"
-
-    def _repr_html_(self):
-        elements_html = '<br>'.join([e._repr_html_() for e in self.elements])
-        html = f"""
-    <table style="border-left:1.2px solid black;>
-      <tr><th colspan="2"><b>StructuralGroup:</b></th></tr>
-      <tr><td>Name:</td><td>{self.name}</td></tr>
-      <tr><td>Structural Relation:</td><td>{self.structural_relation}</td></tr>
-      <tr><td>Elements:</td><td>{elements_html}</td></tr>
-    </table>
-        """
-        return html
-    
-    def append_element(self, element: StructuralElement):
-        self.elements.append(element)
-
-    @property
-    def id(self):
-        raise NotImplementedError
-    
-    @property
-    def number_of_points(self) -> int:
-        return sum([element.number_of_points for element in self.elements])
-    
-    @property
-    def number_of_orientations(self) -> int:
-        return sum([element.number_of_orientations for element in self.elements])
-    
-    @property
-    def number_of_elements(self) -> int:
-        return len(self.elements)
-    
-    def get_element_by_name(self, element_name: str) -> StructuralElement | None:
-        matched_elements: Generator = (element for element in self.elements if element.name == element_name)
-        return next(matched_elements, None)
-
-
-# ? I think these two subclasses are not necessary
-@dataclass
-class Stack(StructuralGroup): 
-    def __int__(self, name: str, elements: list[StructuralElement]):
-        super().__init__(name, elements)
-        
-    def __repr__(self):
-        return pprint.pformat(self.__dict__)
-
-
-@dataclass
-class Fault(StructuralGroup): 
-    pass
+﻿import pprint
+from abc import ABC
+from dataclasses import dataclass, field
+from enum import Enum, auto
+from typing import Optional, Union, Generator
+
+from gempy_engine.core.data.kernel_classes.faults import FaultsData
+from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
+from gempy_engine.core.data.stack_relation_type import StackRelationType
+from gempy.core.data.structural_element import StructuralElement
+
+
+class FaultsRelationSpecialCase(Enum):
+    OFFSET_FORMATIONS = auto()
+    OFFSET_NONE = auto()
+    OFFSET_ALL = auto()
+    
+    
+@dataclass
+class StructuralGroup(ABC):
+    """
+    An abstract base class that represents a structural group within a geological model.
+    
+    """
+    name: str  #: The name of the structural group.
+    
+    elements: list[StructuralElement] = field(repr=False)  #: A list of structural elements within the group.
+    structural_relation: StackRelationType  #: The type of relation between the structural elements in the group.
+
+    #: Relations with other groups in terms of faults.
+    fault_relations: Optional[Union[list["StructuralGroup"], FaultsRelationSpecialCase]] = field(default=None, repr=False)
+    faults_input_data: Optional[FaultsData] = field(default=None, repr=False)
+    
+    solution: Optional[RawArraysSolution] = field(init=False, default=None, repr=False)  #: Solution related to this group from geological computations.
+    
+    
+    def __post_init__(self):
+        if not isinstance(self.elements, list):
+            raise TypeError("elements must be a list of StructuralElement objects.")
+        for e in self.elements:
+            if not isinstance(e, StructuralElement):
+                raise TypeError("elements must be a list of StructuralElement objects.")
+        
+    def __repr__(self):
+        elements_repr = ',\n'.join([repr(e) for e in self.elements])
+        return f"StructuralGroup(\n" \
+               f"\tname={self.name},\n" \
+               f"\tstructural_relation={self.structural_relation},\n" \
+               f"\telements=[\n{elements_repr}\n]\n)"
+
+    def _repr_html_(self):
+        elements_html = '<br>'.join([e._repr_html_() for e in self.elements])
+        html = f"""
+    <table style="border-left:1.2px solid black;>
+      <tr><th colspan="2"><b>StructuralGroup:</b></th></tr>
+      <tr><td>Name:</td><td>{self.name}</td></tr>
+      <tr><td>Structural Relation:</td><td>{self.structural_relation}</td></tr>
+      <tr><td>Elements:</td><td>{elements_html}</td></tr>
+    </table>
+        """
+        return html
+    
+    def append_element(self, element: StructuralElement):
+        self.elements.append(element)
+    
+    def remove_element(self, element: StructuralElement):
+        self.elements.remove(element)
+
+    @property
+    def id(self):
+        raise NotImplementedError
+    
+    @property
+    def is_fault(self)-> bool:
+        return self.structural_relation == StackRelationType.FAULT
+    
+    @property
+    def is_lithology(self)-> bool:
+        return self.structural_relation == StackRelationType.ERODE or self.structural_relation == StackRelationType.ONLAP
+    
+    @property
+    def number_of_points(self) -> int:
+        return sum([element.number_of_points for element in self.elements])
+    
+    @property
+    def number_of_orientations(self) -> int:
+        return sum([element.number_of_orientations for element in self.elements])
+    
+    @property
+    def number_of_elements(self) -> int:
+        return len(self.elements)
+    
+    def get_element_by_name(self, element_name: str) -> StructuralElement | None:
+        matched_elements: Generator = (element for element in self.elements if element.name == element_name)
+        return next(matched_elements, None)
+
+
+# ? I think these two subclasses are not necessary
+@dataclass
+class Stack(StructuralGroup): 
+    def __int__(self, name: str, elements: list[StructuralElement]):
+        super().__init__(name, elements)
+        
+    def __repr__(self):
+        return pprint.pformat(self.__dict__)
+
+
+@dataclass
+class Fault(StructuralGroup): 
+    pass
```

### Comparing `gempy-2023.1.0b6/gempy/core/data/surface_points.py` & `gempy-2023.2.0b1/gempy/core/data/surface_points.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/core/data/xsolution.py` & `gempy-2023.2.0b1/gempy/core/data/xsolution.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy/modules/data_manipulation/manipulate_points.py` & `gempy-2023.2.0b1/gempy/modules/data_manipulation/manipulate_points.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-﻿from typing import Sequence, Optional, Union
-
-import numpy as np
-
-from gempy.core.data import GeoModel, StructuralFrame, SurfacePointsTable, StructuralElement, OrientationsTable
-from gempy.core.data.orientations import DEFAULT_ORI_NUGGET
-from gempy.core.data.surface_points import DEFAULT_SP_NUGGET
-
-
-def add_surface_points(geo_model: GeoModel, x: Sequence[float], y: Sequence[float], z: Sequence[float],
-                       elements_names: Sequence[str], nugget: Optional[Sequence[float]] = None) -> StructuralFrame:
-    elements_names = _validate_args(elements_names, x, y, z)
-
-    # If nugget is not provided, create a Sequence filled with the default value
-    if nugget is None:
-        nugget = [DEFAULT_SP_NUGGET] * len(x)
-
-    # Ensure nugget also has the same length as the other Sequences
-    if len(nugget) != len(x):
-        raise ValueError("The length of the nugget Sequence does not match the lengths of other input Sequences.")
-
-    # * Split the sequences according to the elements_names
-    x = np.array(x)
-    y = np.array(y)
-    z = np.array(z)
-    elements_names = np.array(elements_names)
-    nugget = np.array(nugget)
-
-    unique_names = np.unique(elements_names)
-    grouped_data = {}
-
-    for name in unique_names:
-        mask = (elements_names == name)
-        grouped_data[name] = {
-            'x'     : x[mask],
-            'y'     : y[mask],
-            'z'     : z[mask],
-            'nugget': nugget[mask]
-        }
-
-    # * Loop per element_name
-    for element_name, data in grouped_data.items():
-        formatted_data, _ = SurfacePointsTable._data_from_arrays(
-            x=data['x'],
-            y=data['y'],
-            z=data['z'],
-            names=[element_name] * len(data['x']),
-            nugget=data['nugget'],
-            name_id_map=None
-        )
-
-        element: StructuralElement = geo_model.structural_frame.get_element_by_name(element_name)
-        element.surface_points.data = np.concatenate([
-            element.surface_points.data,
-            formatted_data
-        ])
-
-    return geo_model.structural_frame
-
-
-def delete_surface_points():
-    raise NotImplementedError
-
-
-def add_orientations(geo_model: GeoModel, x: Sequence[float], y: Sequence[float], z: Sequence[float],
-                     elements_names: Sequence[str], pole_vector: Optional[Sequence[np.ndarray]] = None,
-                     orientation: Optional[Sequence[np.ndarray]] = None,
-                     nugget: Optional[Sequence[float]] = None) -> StructuralFrame:
-    if pole_vector is None and orientation is None:
-        raise ValueError("Either pole_vector or orientation must be provided.")
-
-    if orientation:  # Convert orientation to pole_vector (or gradient)
-        pole_vector = convert_orientation_to_pole_vector(
-            azimuth=orientation[:, 0],
-            dip=orientation[:, 1],
-            polarity=orientation[:, 2]
-        )
-
-    elements_names = _validate_args(elements_names, x, y, z, pole_vector)
-
-    if nugget is None:  # If nugget is not provided, create a Sequence filled with the default value
-        nugget = [DEFAULT_ORI_NUGGET] * len(x)
-
-    # Ensure nugget also has the same length as the other Sequences
-    if len(nugget) != len(x):
-        raise ValueError("The length of the nugget Sequence does not match the lengths of other input Sequences.")
-
-    # * Split the sequences according to the elements_names
-    x = np.array(x)
-    y = np.array(y)
-    z = np.array(z)
-    elements_names = np.array(elements_names)
-    pole_vector = np.array(pole_vector)
-    nugget = np.array(nugget)
-
-    unique_names = np.unique(elements_names)
-    grouped_data = {}
-
-    for name in unique_names:
-        mask = (elements_names == name)
-        grouped_data[name] = {
-            'x'          : x[mask],
-            'y'          : y[mask],
-            'z'          : z[mask],
-            'pole_vector': pole_vector[mask],
-            'nugget'     : nugget[mask]
-        }
-
-    # * Loop per element_name
-    for element_name, data in grouped_data.items():
-        formatted_data, _ = OrientationsTable._data_from_arrays(
-            x=data['x'],
-            y=data['y'],
-            z=data['z'],
-            G_x=data['pole_vector'][..., 0],
-            G_y=data['pole_vector'][..., 1],
-            G_z=data['pole_vector'][..., 2],
-            names=[element_name] * len(data['x']),
-            nugget=data['nugget'],
-        )
-
-        element: StructuralElement = geo_model.structural_frame.get_element_by_name(element_name)
-        element.orientations.data = np.concatenate([
-            element.orientations.data,
-            formatted_data
-        ])
-
-    return geo_model.structural_frame
-
-
-def modify_orientations(geo_model: GeoModel, slice: Optional[Union[int, slice]] = None,
-                        **orientation_field: Union[float, np.ndarray]) -> StructuralFrame:
-    """
-    Modifies specified fields of all orientations in the structural frame. The keys of the orientation_field 
-    dictionary should match the field names in the orientations (e.g., "X", "Y", "Z", "G_x", "G_y", "G_z", "nugget").
-    
-    Args:
-        geo_model (GeoModel): The GeoModel instance to modify.
-        slice (Optional[Union[int, slice]]): The slice of orientations to modify. If None, all orientations will be modified.
-        
-    Keyword Args:
-        X (Union[float, np.ndarray]): X coordinates of the orientations.
-        Y (Union[float, np.ndarray]): Y coordinates of the orientations.
-        Z (Union[float, np.ndarray]): Z coordinates of the orientations.
-        azimuth (Union[float, np.ndarray]): Azimuth angles of the orientations.
-        dip (Union[float, np.ndarray]): Dip angles of the orientations.
-        polarity (Union[float, np.ndarray]): Polarity values of the orientations.
-        G_x (Union[float, np.ndarray]): X component of the gradient vector.
-        G_y (Union[float, np.ndarray]): Y component of the gradient vector.
-        G_z (Union[float, np.ndarray]): Z component of the gradient vector.
-        nugget (Union[float, np.ndarray]): Nugget value of the orientations.
-            
-    Returns:
-        StructuralFrame: The modified structural frame.
-    """
-
-    orientations = geo_model.structural_frame.orientations
-
-    # If no slice is provided, target all rows; else, target specified slice
-    target_rows = slice if slice is not None else np.s_[:]
-
-    # Extract provided orientation fields without modifying the dictionary
-    azimuth = orientation_field.pop('azimuth', None)
-    dip = orientation_field.pop('dip', None)
-    polarity = orientation_field.pop('polarity', None)
-
-    # Update all the other fields
-    for key, value in orientation_field.items():
-        if isinstance(value, np.ndarray) and len(value) != len(orientations.data[target_rows]):
-            raise ValueError(f"Length mismatch: Expected size {len(orientations.data[target_rows])} for field {key}, but got {len(value)}.")
-        orientations.data[key][target_rows] = value
-
-    # Check if azimuth, dip, or polarity are provided
-    any_polar_fields = azimuth is not None or dip is not None or polarity is not None
-    all_polar_fields = azimuth is not None and dip is not None and polarity is not None
-
-    match (any_polar_fields, all_polar_fields):
-        case (True, True):
-            # All polar fields provided, convert to gradients
-            gx, gy, gz = convert_orientation_to_pole_vector(np.asarray(azimuth), np.asarray(dip), np.asarray(polarity))
-            orientations.data['G_x'][target_rows] = gx
-            orientations.data['G_y'][target_rows] = gy
-            orientations.data['G_z'][target_rows] = gz
-
-        case (True, False):
-            # Some polar fields missing, compute missing fields from gradients
-            prev_azimuth, prev_dip, prev_polarity = compute_adp_from_gradients(
-                orientations.data['G_x'],
-                orientations.data['G_y'],
-                orientations.data['G_z']
-            )
-            azimuth = np.asarray(azimuth) if azimuth is not None else prev_azimuth
-            dip = np.asarray(dip) if dip is not None else prev_dip
-            polarity = np.asarray(polarity) if polarity is not None else prev_polarity
-
-            gradients = convert_orientation_to_pole_vector(azimuth, dip, polarity)
-            orientations.data['G_x'][target_rows] = gradients[:, 0]
-            orientations.data['G_y'][target_rows] = gradients[:, 1]
-            orientations.data['G_z'][target_rows] = gradients[:, 2]
-
-        case (_, _):
-            pass
-
-    geo_model.orientations = orientations
-    return geo_model.structural_frame
-
-
-def modify_surface_points(geo_model: GeoModel,
-                          slice: Optional[Union[int, slice]] = None,
-                          elements_names: Optional[Sequence[str]] = None,
-                          **surface_points_field: Union[float, np.ndarray]) -> StructuralFrame:
-    """
-    Modifies specified fields of all surface points in the structural frame. The keys of the surface_points_field 
-    dictionary should match the field names in the surface points (e.g., "X", "Y", "Z", "nugget").
-    
-    Args:
-        geo_model (GeoModel): The GeoModel instance to modify.
-        slice (Optional[Union[int, slice]]): The slice of surface points to modify. If None, all surface points will be modified.
-        
-    Keyword Args:
-        X (Union[float, np.ndarray]): X coordinates of the surface points.
-        Y (Union[float, np.ndarray]): Y coordinates of the surface points.
-        Z (Union[float, np.ndarray]): Z coordinates of the surface points.
-        nugget (Union[float, np.ndarray]): Nugget value of the surface points.
-            
-    Returns:
-        StructuralFrame: The modified structural frame.
-    """
-    surface_points = geo_model.structural_frame.surface_points
-    
-    if elements_names is not None:
-        ids = [surface_points.name_id_map[element] for element in elements_names] 
-        slice = np.s_[np.isin(surface_points.data['id'], ids)]
-    
-
-    # If no slice is provided, target all rows; else, target specified slice
-    target_rows = slice if slice is not None else np.s_[:]
-
-    for key, value in surface_points_field.items():
-        if isinstance(value, np.ndarray) and len(value) != len(surface_points.data[target_rows]):
-            raise ValueError(f"Length mismatch: Expected size {len(surface_points.data[target_rows])} for field {key}, but got {len(value)}.")
-
-        surface_points.data[key][target_rows] = value
-
-    geo_model.surface_points = surface_points
-    return geo_model.structural_frame
-
-
-def delete_orientations():
-    raise NotImplementedError
-
-
-def convert_orientation_to_pole_vector(azimuth: Sequence[float], dip: Sequence[float], polarity: Sequence[float]) -> Sequence[np.ndarray]:
-    # Convert sequences to numpy arrays for vectorized operations
-    azimuth = np.array(azimuth)
-    dip = np.array(dip)
-    polarity = np.array(polarity)
-
-    # Calculate gradient components
-    G_x = np.sin(np.deg2rad(dip)) * np.sin(np.deg2rad(azimuth)) * polarity
-    G_y = np.sin(np.deg2rad(dip)) * np.cos(np.deg2rad(azimuth)) * polarity
-    G_z = np.cos(np.deg2rad(dip)) * polarity
-
-    # Combine gradient components into an array of vectors
-    gradients = np.vstack([G_x, G_y, G_z]).T
-
-    return gradients
-
-
-def compute_adp_from_gradients(G_x: np.ndarray, G_y: np.ndarray, G_z: np.ndarray) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-    # Calculate polarity (here assumed to be 1 for all, but you can adapt if needed)
-    polarity = np.ones_like(G_x)
-
-    # Calculate dip
-    dip = np.rad2deg(np.nan_to_num(np.arccos(G_z / polarity)))
-
-    # Calculate azimuth
-    azimuth = np.rad2deg(np.nan_to_num(np.arctan2(G_x / polarity, G_y / polarity)))
-
-    # Shift values from [-pi, 0] to [pi,2*pi]
-    azimuth[azimuth < 0] += 360
-
-    # Adjust azimuth where dip is nearly zero, because if dip is zero, azimuth is undefined
-    azimuth[dip < 0.001] = 0
-
-    return azimuth, dip, polarity
-
-
-def _validate_args(elements_names, *args):
-    if isinstance(elements_names, str):
-        elements_names = np.array([elements_names] * len(args[0]))
-    elif isinstance(elements_names, Sequence) or isinstance(elements_names, np.ndarray):
-        pass
-    else:
-        raise TypeError(f"Names should be a string or a NumPy array, not {type(elements_names)}")
-    # Ensure all provided Sequences have the same length
-    lengths = {len(arg) for arg in args}
-    if len(lengths) != 1:
-        raise ValueError("All input Sequences must have the same length.")
-    return elements_names
+﻿from typing import Sequence, Optional, Union
+
+import numpy as np
+
+from gempy.core.data import GeoModel, StructuralFrame, SurfacePointsTable, StructuralElement, OrientationsTable
+from gempy.core.data.orientations import DEFAULT_ORI_NUGGET
+from gempy.core.data.surface_points import DEFAULT_SP_NUGGET
+
+
+def add_surface_points(geo_model: GeoModel, x: Sequence[float], y: Sequence[float], z: Sequence[float],
+                       elements_names: Sequence[str], nugget: Optional[Sequence[float]] = None) -> StructuralFrame:
+    elements_names = _validate_args(elements_names, x, y, z)
+
+    # If nugget is not provided, create a Sequence filled with the default value
+    if nugget is None:
+        nugget = [DEFAULT_SP_NUGGET] * len(x)
+
+    # Ensure nugget also has the same length as the other Sequences
+    if len(nugget) != len(x):
+        raise ValueError("The length of the nugget Sequence does not match the lengths of other input Sequences.")
+
+    # * Split the sequences according to the elements_names
+    x = np.array(x)
+    y = np.array(y)
+    z = np.array(z)
+    elements_names = np.array(elements_names)
+    nugget = np.array(nugget)
+
+    unique_names = np.unique(elements_names)
+    grouped_data = {}
+
+    for name in unique_names:
+        mask = (elements_names == name)
+        grouped_data[name] = {
+            'x'     : x[mask],
+            'y'     : y[mask],
+            'z'     : z[mask],
+            'nugget': nugget[mask]
+        }
+
+    # * Loop per element_name
+    for element_name, data in grouped_data.items():
+        formatted_data, _ = SurfacePointsTable._data_from_arrays(
+            x=data['x'],
+            y=data['y'],
+            z=data['z'],
+            names=[element_name] * len(data['x']),
+            nugget=data['nugget'],
+            name_id_map=None
+        )
+
+        element: StructuralElement = geo_model.structural_frame.get_element_by_name(element_name)
+        element.surface_points.data = np.concatenate([
+            element.surface_points.data,
+            formatted_data
+        ])
+
+    return geo_model.structural_frame
+
+
+def delete_surface_points():
+    raise NotImplementedError
+
+
+def add_orientations(geo_model: GeoModel, x: Sequence[float], y: Sequence[float], z: Sequence[float],
+                     elements_names: Sequence[str], pole_vector: Optional[Sequence[np.ndarray]] = None,
+                     orientation: Optional[Sequence[np.ndarray]] = None,
+                     nugget: Optional[Sequence[float]] = None) -> StructuralFrame:
+    if pole_vector is None and orientation is None:
+        raise ValueError("Either pole_vector or orientation must be provided.")
+
+    if orientation:  # Convert orientation to pole_vector (or gradient)
+        pole_vector = convert_orientation_to_pole_vector(
+            azimuth=orientation[:, 0],
+            dip=orientation[:, 1],
+            polarity=orientation[:, 2]
+        )
+
+    elements_names = _validate_args(elements_names, x, y, z, pole_vector)
+
+    if nugget is None:  # If nugget is not provided, create a Sequence filled with the default value
+        nugget = [DEFAULT_ORI_NUGGET] * len(x)
+
+    # Ensure nugget also has the same length as the other Sequences
+    if len(nugget) != len(x):
+        raise ValueError("The length of the nugget Sequence does not match the lengths of other input Sequences.")
+
+    # * Split the sequences according to the elements_names
+    x = np.array(x)
+    y = np.array(y)
+    z = np.array(z)
+    elements_names = np.array(elements_names)
+    pole_vector = np.array(pole_vector)
+    nugget = np.array(nugget)
+
+    unique_names = np.unique(elements_names)
+    grouped_data = {}
+
+    for name in unique_names:
+        mask = (elements_names == name)
+        grouped_data[name] = {
+            'x'          : x[mask],
+            'y'          : y[mask],
+            'z'          : z[mask],
+            'pole_vector': pole_vector[mask],
+            'nugget'     : nugget[mask]
+        }
+
+    # * Loop per element_name
+    for element_name, data in grouped_data.items():
+        formatted_data, _ = OrientationsTable._data_from_arrays(
+            x=data['x'],
+            y=data['y'],
+            z=data['z'],
+            G_x=data['pole_vector'][..., 0],
+            G_y=data['pole_vector'][..., 1],
+            G_z=data['pole_vector'][..., 2],
+            names=[element_name] * len(data['x']),
+            nugget=data['nugget'],
+        )
+
+        element: StructuralElement = geo_model.structural_frame.get_element_by_name(element_name)
+        element.orientations.data = np.concatenate([
+            element.orientations.data,
+            formatted_data
+        ])
+
+    return geo_model.structural_frame
+
+
+def modify_orientations(geo_model: GeoModel, slice: Optional[Union[int, slice]] = None,
+                        **orientation_field: Union[float, np.ndarray]) -> StructuralFrame:
+    """
+    Modifies specified fields of all orientations in the structural frame. The keys of the orientation_field 
+    dictionary should match the field names in the orientations (e.g., "X", "Y", "Z", "G_x", "G_y", "G_z", "nugget").
+    
+    Args:
+        geo_model (GeoModel): The GeoModel instance to modify.
+        slice (Optional[Union[int, slice]]): The slice of orientations to modify. If None, all orientations will be modified.
+        
+    Keyword Args:
+        X (Union[float, np.ndarray]): X coordinates of the orientations.
+        Y (Union[float, np.ndarray]): Y coordinates of the orientations.
+        Z (Union[float, np.ndarray]): Z coordinates of the orientations.
+        azimuth (Union[float, np.ndarray]): Azimuth angles of the orientations.
+        dip (Union[float, np.ndarray]): Dip angles of the orientations.
+        polarity (Union[float, np.ndarray]): Polarity values of the orientations.
+        G_x (Union[float, np.ndarray]): X component of the gradient vector.
+        G_y (Union[float, np.ndarray]): Y component of the gradient vector.
+        G_z (Union[float, np.ndarray]): Z component of the gradient vector.
+        nugget (Union[float, np.ndarray]): Nugget value of the orientations.
+            
+    Returns:
+        StructuralFrame: The modified structural frame.
+    """
+
+    orientations = geo_model.structural_frame.orientations
+
+    # If no slice is provided, target all rows; else, target specified slice
+    target_rows = slice if slice is not None else np.s_[:]
+
+    # Extract provided orientation fields without modifying the dictionary
+    azimuth = orientation_field.pop('azimuth', None)
+    dip = orientation_field.pop('dip', None)
+    polarity = orientation_field.pop('polarity', None)
+
+    # Update all the other fields
+    for key, value in orientation_field.items():
+        if isinstance(value, np.ndarray) and len(value) != len(orientations.data[target_rows]):
+            raise ValueError(f"Length mismatch: Expected size {len(orientations.data[target_rows])} for field {key}, but got {len(value)}.")
+        orientations.data[key][target_rows] = value
+
+    # Check if azimuth, dip, or polarity are provided
+    any_polar_fields = azimuth is not None or dip is not None or polarity is not None
+    all_polar_fields = azimuth is not None and dip is not None and polarity is not None
+
+    match (any_polar_fields, all_polar_fields):
+        case (True, True):
+            # All polar fields provided, convert to gradients
+            gx, gy, gz = convert_orientation_to_pole_vector(np.asarray(azimuth), np.asarray(dip), np.asarray(polarity))
+            orientations.data['G_x'][target_rows] = gx
+            orientations.data['G_y'][target_rows] = gy
+            orientations.data['G_z'][target_rows] = gz
+
+        case (True, False):
+            # Some polar fields missing, compute missing fields from gradients
+            prev_azimuth, prev_dip, prev_polarity = compute_adp_from_gradients(
+                orientations.data['G_x'],
+                orientations.data['G_y'],
+                orientations.data['G_z']
+            )
+            azimuth = np.asarray(azimuth) if azimuth is not None else prev_azimuth
+            dip = np.asarray(dip) if dip is not None else prev_dip
+            polarity = np.asarray(polarity) if polarity is not None else prev_polarity
+
+            gradients = convert_orientation_to_pole_vector(azimuth, dip, polarity)
+            orientations.data['G_x'][target_rows] = gradients[:, 0]
+            orientations.data['G_y'][target_rows] = gradients[:, 1]
+            orientations.data['G_z'][target_rows] = gradients[:, 2]
+
+        case (_, _):
+            pass
+
+    geo_model.orientations = orientations
+    return geo_model.structural_frame
+
+
+def modify_surface_points(geo_model: GeoModel,
+                          slice: Optional[Union[int, slice]] = None,
+                          elements_names: Optional[Sequence[str]] = None,
+                          **surface_points_field: Union[float, np.ndarray]) -> StructuralFrame:
+    """
+    Modifies specified fields of all surface points in the structural frame. The keys of the surface_points_field 
+    dictionary should match the field names in the surface points (e.g., "X", "Y", "Z", "nugget").
+    
+    Args:
+        geo_model (GeoModel): The GeoModel instance to modify.
+        slice (Optional[Union[int, slice]]): The slice of surface points to modify. If None, all surface points will be modified.
+        
+    Keyword Args:
+        X (Union[float, np.ndarray]): X coordinates of the surface points.
+        Y (Union[float, np.ndarray]): Y coordinates of the surface points.
+        Z (Union[float, np.ndarray]): Z coordinates of the surface points.
+        nugget (Union[float, np.ndarray]): Nugget value of the surface points.
+            
+    Returns:
+        StructuralFrame: The modified structural frame.
+    """
+    surface_points = geo_model.structural_frame.surface_points
+    
+    if elements_names is not None:
+        ids = [surface_points.name_id_map[element] for element in elements_names] 
+        slice = np.s_[np.isin(surface_points.data['id'], ids)]
+    
+
+    # If no slice is provided, target all rows; else, target specified slice
+    target_rows = slice if slice is not None else np.s_[:]
+
+    for key, value in surface_points_field.items():
+        if isinstance(value, np.ndarray) and len(value) != len(surface_points.data[target_rows]):
+            raise ValueError(f"Length mismatch: Expected size {len(surface_points.data[target_rows])} for field {key}, but got {len(value)}.")
+
+        surface_points.data[key][target_rows] = value
+
+    geo_model.surface_points = surface_points
+    return geo_model.structural_frame
+
+
+def delete_orientations():
+    raise NotImplementedError
+
+
+def convert_orientation_to_pole_vector(azimuth: Sequence[float], dip: Sequence[float], polarity: Sequence[float]) -> Sequence[np.ndarray]:
+    # Convert sequences to numpy arrays for vectorized operations
+    azimuth = np.array(azimuth)
+    dip = np.array(dip)
+    polarity = np.array(polarity)
+
+    # Calculate gradient components
+    G_x = np.sin(np.deg2rad(dip)) * np.sin(np.deg2rad(azimuth)) * polarity
+    G_y = np.sin(np.deg2rad(dip)) * np.cos(np.deg2rad(azimuth)) * polarity
+    G_z = np.cos(np.deg2rad(dip)) * polarity
+
+    # Combine gradient components into an array of vectors
+    gradients = np.vstack([G_x, G_y, G_z]).T
+
+    return gradients
+
+
+def compute_adp_from_gradients(G_x: np.ndarray, G_y: np.ndarray, G_z: np.ndarray) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+    # Calculate polarity (here assumed to be 1 for all, but you can adapt if needed)
+    polarity = np.ones_like(G_x)
+
+    # Calculate dip
+    dip = np.rad2deg(np.nan_to_num(np.arccos(G_z / polarity)))
+
+    # Calculate azimuth
+    azimuth = np.rad2deg(np.nan_to_num(np.arctan2(G_x / polarity, G_y / polarity)))
+
+    # Shift values from [-pi, 0] to [pi,2*pi]
+    azimuth[azimuth < 0] += 360
+
+    # Adjust azimuth where dip is nearly zero, because if dip is zero, azimuth is undefined
+    azimuth[dip < 0.001] = 0
+
+    return azimuth, dip, polarity
+
+
+def _validate_args(elements_names, *args):
+    if isinstance(elements_names, str):
+        elements_names = np.array([elements_names] * len(args[0]))
+    elif isinstance(elements_names, Sequence) or isinstance(elements_names, np.ndarray):
+        pass
+    else:
+        raise TypeError(f"Names should be a string or a NumPy array, not {type(elements_names)}")
+    # Ensure all provided Sequences have the same length
+    lengths = {len(arg) for arg in args}
+    if len(lengths) != 1:
+        raise ValueError("All input Sequences must have the same length.")
+    return elements_names
```

### Comparing `gempy-2023.1.0b6/gempy/modules/data_manipulation/orientations_from_surface_points.py` & `gempy-2023.2.0b1/gempy/modules/data_manipulation/orientations_from_surface_points.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-﻿from typing import Optional
-
-import numpy as np
-from numpy.linalg import svd
-
-from gempy.core.data import SurfacePointsTable, OrientationsTable
-
-
-def create_orientations_from_surface_points_coords(xyz_coords: np.ndarray,
-                                                   subset: Optional[np.ndarray] = None,
-                                                   element_name: Optional[str] = "Generated") -> OrientationsTable:
-    # Initialize the arrays
-    center = np.empty((len(subset) if subset is not None else 1, 3))
-    normal = np.empty((len(subset) if subset is not None else 1, 3))
-
-    if subset is None:
-        center[0], normal[0] = _plane_fit(xyz_coords)
-    else:
-        for idx, i in enumerate(subset):
-            center[idx], normal[idx] = _plane_fit(xyz_coords[i])
-
-    orientations = OrientationsTable.from_arrays(
-        x=center[:, 0],
-        y=center[:, 1],
-        z=center[:, 2],
-        G_x=normal[:, 0],
-        G_y=normal[:, 1],
-        G_z=normal[:, 2],
-        names=[element_name]
-    )
-    return orientations
-
-
-def _plane_fit(point_list):
-    """
-    Fit plane to points in PointSet
-    Fit an d-dimensional plane to the points in a point set.
-    adjusted from: http://stackoverflow.com/questions/12299540/plane-fitting-to-4-or-more-xyz-points
-
-    Args:
-        point_list (array_like): array of points XYZ
-
-    Returns:
-        Return a point, p, on the plane (the point-cloud centroid),
-        and the normal, n.
-    """
-
-    points = point_list.T
-
-    points = np.reshape(points, (np.shape(points)[0], -1))  # Collapse trialing dimensions
-    assert points.shape[0] <= points.shape[1], "There are only {} points in {} dimensions.".format(points.shape[1],
-                                                                                                   points.shape[0])
-    ctr = points.mean(axis=1)
-    x = points - ctr[:, np.newaxis]
-    M = np.dot(x, x.T)  # Could also use np.cov(x) here.
-
-    # ctr = Point(x=ctr[0], y=ctr[1], z=ctr[2], type='utm', zone=self.points[0].zone)
-    normal = svd(M)[0][:, -1]
-    # return ctr, svd(M)[0][:, -1]
-    if normal[2] < 0:
-        normal = - normal
-
-    return ctr, normal
+﻿from typing import Optional
+
+import numpy as np
+from numpy.linalg import svd
+
+from gempy.core.data import SurfacePointsTable, OrientationsTable
+
+
+def create_orientations_from_surface_points_coords(xyz_coords: np.ndarray,
+                                                   subset: Optional[np.ndarray] = None,
+                                                   element_name: Optional[str] = "Generated") -> OrientationsTable:
+    # Initialize the arrays
+    center = np.empty((len(subset) if subset is not None else 1, 3))
+    normal = np.empty((len(subset) if subset is not None else 1, 3))
+
+    if subset is None:
+        center[0], normal[0] = _plane_fit(xyz_coords)
+    else:
+        for idx, i in enumerate(subset):
+            center[idx], normal[idx] = _plane_fit(xyz_coords[i])
+
+    orientations = OrientationsTable.from_arrays(
+        x=center[:, 0],
+        y=center[:, 1],
+        z=center[:, 2],
+        G_x=normal[:, 0],
+        G_y=normal[:, 1],
+        G_z=normal[:, 2],
+        names=[element_name]
+    )
+    return orientations
+
+
+def _plane_fit(point_list):
+    """
+    Fit plane to points in PointSet
+    Fit an d-dimensional plane to the points in a point set.
+    adjusted from: http://stackoverflow.com/questions/12299540/plane-fitting-to-4-or-more-xyz-points
+
+    Args:
+        point_list (array_like): array of points XYZ
+
+    Returns:
+        Return a point, p, on the plane (the point-cloud centroid),
+        and the normal, n.
+    """
+
+    points = point_list.T
+
+    points = np.reshape(points, (np.shape(points)[0], -1))  # Collapse trialing dimensions
+    assert points.shape[0] <= points.shape[1], "There are only {} points in {} dimensions.".format(points.shape[1],
+                                                                                                   points.shape[0])
+    ctr = points.mean(axis=1)
+    x = points - ctr[:, np.newaxis]
+    M = np.dot(x, x.T)  # Could also use np.cov(x) here.
+
+    # ctr = Point(x=ctr[0], y=ctr[1], z=ctr[2], type='utm', zone=self.points[0].zone)
+    normal = svd(M)[0][:, -1]
+    # return ctr, svd(M)[0][:, -1]
+    if normal[2] < 0:
+        normal = - normal
+
+    return ctr, normal
```

### Comparing `gempy-2023.1.0b6/gempy/modules/grids/create_topography.py` & `gempy-2023.2.0b1/gempy/modules/grids/create_topography.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-"""
-This file is part of gempy.
-
-Created on 16.04.2019
-
-@author: Elisa Heim
-"""
-from typing import Optional
-
-import numpy as np
-
-from gempy.optional_dependencies import require_scipy
-
-
-def create_random_topography(extent: np.array, resolution: np.array, dz: Optional[np.array] = None,
-                             fractal_dimension: Optional[float] = 2.0) -> np.array:
-    dem = _LoadDEMArtificial(
-        extent=extent,
-        resolution=resolution,
-        d_z=dz,
-        fd=fractal_dimension
-    )
-
-    return dem.get_values()
-
-
-class _LoadDEMArtificial:  # * Cannot think of a good reason to be a class
-
-    def __init__(self, grid=None, fd=2.0, extent=None, resolution=None, d_z=None):
-        """Class to create a random topography based on a fractal grid algorithm.
-
-        Args:
-            fd:         fractal dimension, defaults to 2.0
-            d_z:        maximum height difference. If none, last 20% of the model in z direction
-            extent:     extent in xy direction. If none, geo_model.grid.extent
-            resolution: desired resolution of the topography array. If none, geo_model.grid.resolution
-        """
-        self.values_2d = np.array([])
-        self.resolution = grid.resolution[:2] if resolution is None else resolution
-
-        assert all(np.asarray(self.resolution) >= 2), 'The regular grid needs to be at least of size 2 on all directions.'
-        self.extent = grid.extent if extent is None else extent
-
-        if d_z is None:
-            self.d_z = np.array([self.extent[5] - (self.extent[5] - self.extent[4]) * 1 / 5, self.extent[5]])
-            print(self.d_z)
-        else:
-            self.d_z = d_z
-
-        topo = self.fractalGrid(fd, n=self.resolution.max())
-        topo = np.interp(topo, (topo.min(), topo.max()), self.d_z)
-
-        self.dem_zval = topo[:self.resolution[0], :self.resolution[1]]  # crop fractal grid with resolution
-        self.create_topo_array()
-
-    @staticmethod
-    def fractalGrid(fd, n=256):
-        """
-        Modified after https://github.com/samthiele/pycompass/blob/master/examples/3_Synthetic%20Examples.ipynb
-
-        Generate isotropic fractal surface image using
-        spectral synthesis method [1, p.]
-        References:
-        1. Yuval Fisher, Michael McGuire,
-        The Science of Fractal Images, 1988
-
-        (cf. http://shortrecipes.blogspot.com.au/2008/11/python-isotropic-fractal-surface.html)
-        **Arguments**:
-         -fd = the fractal dimension
-         -N = the size of the fractal surface/image
-
-        """
-        h = 1 - (fd - 2)
-        # X = np.zeros((N, N), complex)
-        a = np.zeros((n, n), complex)
-        powerr = -(h + 1.0) / 2.0
-
-        for i in range(int(n / 2) + 1):
-            for j in range(int(n / 2) + 1):
-                phase = 2 * np.pi * np.random.rand()
-
-                if i != 0 or j != 0:
-                    rad = (i * i + j * j) ** powerr * np.random.normal()
-                else:
-                    rad = 0.0
-
-                a[i, j] = complex(rad * np.cos(phase), rad * np.sin(phase))
-
-                if i == 0:
-                    i0 = 0
-                else:
-                    i0 = n - i
-
-                if j == 0:
-                    j0 = 0
-                else:
-                    j0 = n - j
-
-                a[i0, j0] = complex(rad * np.cos(phase), -rad * np.sin(phase))
-
-                a.imag[int(n / 2)][0] = 0.0
-                a.imag[0, int(n / 2)] = 0.0
-                a.imag[int(n / 2)][int(n / 2)] = 0.0
-
-        for i in range(1, int(n / 2)):
-            for j in range(1, int(n / 2)):
-                phase = 2 * np.pi * np.random.rand()
-                rad = (i * i + j * j) ** powerr * np.random.normal()
-                a[i, n - j] = complex(rad * np.cos(phase), rad * np.sin(phase))
-                a[n - i, j] = complex(rad * np.cos(phase), -rad * np.sin(phase))
-
-        scipy = require_scipy()
-        itemp = scipy.fftpack.ifft2(a)
-        itemp = itemp - itemp.min()
-
-        return itemp.real / itemp.real.max()
-
-    def create_topo_array(self):
-        """for masking the lith block"""
-        x = np.linspace(self.extent[0], self.extent[1], self.resolution[0])
-        y = np.linspace(self.extent[2], self.extent[3], self.resolution[1])
-        self.x = x
-        self.y = y
-        xx, yy = np.meshgrid(x, y, indexing='ij')
-        self.values_2d = np.dstack([xx, yy, self.dem_zval])
-
-    def get_values(self):
-        return self.values_2d
+"""
+This file is part of gempy.
+
+Created on 16.04.2019
+
+@author: Elisa Heim
+"""
+from typing import Optional
+
+import numpy as np
+
+from gempy.optional_dependencies import require_scipy
+
+
+def create_random_topography(extent: np.array, resolution: np.array, dz: Optional[np.array] = None,
+                             fractal_dimension: Optional[float] = 2.0) -> np.array:
+    dem = _LoadDEMArtificial(
+        extent=extent,
+        resolution=resolution,
+        d_z=dz,
+        fd=fractal_dimension
+    )
+
+    return dem.get_values()
+
+
+class _LoadDEMArtificial:  # * Cannot think of a good reason to be a class
+
+    def __init__(self, grid=None, fd=2.0, extent=None, resolution=None, d_z=None):
+        """Class to create a random topography based on a fractal grid algorithm.
+
+        Args:
+            fd:         fractal dimension, defaults to 2.0
+            d_z:        maximum height difference. If none, last 20% of the model in z direction
+            extent:     extent in xy direction. If none, geo_model.grid.extent
+            resolution: desired resolution of the topography array. If none, geo_model.grid.resolution
+        """
+        self.values_2d = np.array([])
+        self.resolution = grid.resolution[:2] if resolution is None else resolution
+
+        assert all(np.asarray(self.resolution) >= 2), 'The regular grid needs to be at least of size 2 on all directions.'
+        self.extent = grid.extent if extent is None else extent
+
+        if d_z is None:
+            self.d_z = np.array([self.extent[5] - (self.extent[5] - self.extent[4]) * 1 / 5, self.extent[5]])
+            print(self.d_z)
+        else:
+            self.d_z = d_z
+
+        topo = self.fractalGrid(fd, n=self.resolution.max())
+        topo = np.interp(topo, (topo.min(), topo.max()), self.d_z)
+
+        self.dem_zval = topo[:self.resolution[0], :self.resolution[1]]  # crop fractal grid with resolution
+        self.create_topo_array()
+
+    @staticmethod
+    def fractalGrid(fd, n=256):
+        """
+        Modified after https://github.com/samthiele/pycompass/blob/master/examples/3_Synthetic%20Examples.ipynb
+
+        Generate isotropic fractal surface image using
+        spectral synthesis method [1, p.]
+        References:
+        1. Yuval Fisher, Michael McGuire,
+        The Science of Fractal Images, 1988
+
+        (cf. http://shortrecipes.blogspot.com.au/2008/11/python-isotropic-fractal-surface.html)
+        **Arguments**:
+         -fd = the fractal dimension
+         -N = the size of the fractal surface/image
+
+        """
+        h = 1 - (fd - 2)
+        # X = np.zeros((N, N), complex)
+        a = np.zeros((n, n), complex)
+        powerr = -(h + 1.0) / 2.0
+
+        for i in range(int(n / 2) + 1):
+            for j in range(int(n / 2) + 1):
+                phase = 2 * np.pi * np.random.rand()
+
+                if i != 0 or j != 0:
+                    rad = (i * i + j * j) ** powerr * np.random.normal()
+                else:
+                    rad = 0.0
+
+                a[i, j] = complex(rad * np.cos(phase), rad * np.sin(phase))
+
+                if i == 0:
+                    i0 = 0
+                else:
+                    i0 = n - i
+
+                if j == 0:
+                    j0 = 0
+                else:
+                    j0 = n - j
+
+                a[i0, j0] = complex(rad * np.cos(phase), -rad * np.sin(phase))
+
+                a.imag[int(n / 2)][0] = 0.0
+                a.imag[0, int(n / 2)] = 0.0
+                a.imag[int(n / 2)][int(n / 2)] = 0.0
+
+        for i in range(1, int(n / 2)):
+            for j in range(1, int(n / 2)):
+                phase = 2 * np.pi * np.random.rand()
+                rad = (i * i + j * j) ** powerr * np.random.normal()
+                a[i, n - j] = complex(rad * np.cos(phase), rad * np.sin(phase))
+                a[n - i, j] = complex(rad * np.cos(phase), -rad * np.sin(phase))
+
+        scipy = require_scipy()
+        itemp = scipy.fftpack.ifft2(a)
+        itemp = itemp - itemp.min()
+
+        return itemp.real / itemp.real.max()
+
+    def create_topo_array(self):
+        """for masking the lith block"""
+        x = np.linspace(self.extent[0], self.extent[1], self.resolution[0])
+        y = np.linspace(self.extent[2], self.extent[3], self.resolution[1])
+        self.x = x
+        self.y = y
+        xx, yy = np.meshgrid(x, y, indexing='ij')
+        self.values_2d = np.dstack([xx, yy, self.dem_zval])
+
+    def get_values(self):
+        return self.values_2d
```

### Comparing `gempy-2023.1.0b6/gempy/optional_dependencies.py` & `gempy-2023.2.0b1/gempy/optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/gempy.egg-info/SOURCES.txt` & `gempy-2023.2.0b1/gempy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,37 +9,30 @@
 examples/examples/geometries/a01_horizontal_stratigraphic.py
 examples/examples/geometries/b02_fold.py
 examples/examples/geometries/c03_recumbent_fold.py
 examples/examples/geometries/d04_pinchout.py
 examples/examples/geometries/e05_fault.py
 examples/examples/geometries/f06_unconformity.py
 examples/examples/geometries/g07_combination.py
-examples/examples/geometries/foo/__init__.py
-examples/examples/geometries/foo/more_examples.py
+examples/examples/geometries/h08_more_examples.py
 examples/examples/real/Alesmodel.py
 examples/examples/real/Claudius.py
 examples/examples/real/Greenstone.py
 examples/examples/real/Hecho.py
 examples/examples/real/Moureze.py
 examples/examples/real/Perth_basin.py
 examples/examples/real/__init__.py
 examples/integrations/__init__.py
 examples/integrations/gempy_export_MOOSE.py
-examples/integrations/gempy_export_perth_bassin_pflotran.py
-examples/integrations/gempy_striplog.py
 examples/integrations/gempy_subsurface.py
 examples/tutorials/__init__.py
-examples/tutorials/ch2-Geophysics/__init__.py
-examples/tutorials/ch2-Geophysics/ch2_1_gravity.py
-examples/tutorials/ch2-Geophysics/ch2_2_cell_selection.py
+examples/tutorials/a_getting_started/__init__.py
+examples/tutorials/a_getting_started/get_started.py
 examples/tutorials/ch4-Topology/__init__.py
 examples/tutorials/ch4-Topology/ch4-1-Topology.py
-examples/tutorials_/__init__.py
-examples/tutorials_/a_getting_started/__init__.py
-examples/tutorials_/a_getting_started/get_started.py
 gempy/__init__.py
 gempy/optional_dependencies.py
 gempy.egg-info/PKG-INFO
 gempy.egg-info/SOURCES.txt
 gempy.egg-info/dependency_links.txt
 gempy.egg-info/requires.txt
 gempy.egg-info/top_level.txt
@@ -55,14 +48,15 @@
 gempy/API/gp2_gp3_compatibility/__init__.py
 gempy/API/gp2_gp3_compatibility/gp3_to_gp2_input.py
 gempy/API/gp2_gp3_compatibility/gp3_to_gp2_output.py
 gempy/core/__init__.py
 gempy/core/color_generator.py
 gempy/core/data/__init__.py
 gempy/core/data/_data_points_helpers.py
+gempy/core/data/core_utils.py
 gempy/core/data/enumerators.py
 gempy/core/data/gempy_engine_config.py
 gempy/core/data/geo_model.py
 gempy/core/data/grid.py
 gempy/core/data/importer_helper.py
 gempy/core/data/orientations.py
 gempy/core/data/structural_element.py
@@ -77,16 +71,14 @@
 gempy/modules/__init__.py
 gempy/modules/custom_implicit_functions/__init__.py
 gempy/modules/custom_implicit_functions/ellipsoid_implicit_function.py
 gempy/modules/data_manipulation/__init__.py
 gempy/modules/data_manipulation/manipulate_points.py
 gempy/modules/data_manipulation/manipulate_structural_frame.py
 gempy/modules/data_manipulation/orientations_from_surface_points.py
-gempy/modules/geophysics/__init__.py
-gempy/modules/geophysics/geophysics.py
 gempy/modules/grids/__init__.py
 gempy/modules/grids/create_topography.py
 test/test_api/__init__.py
 test/test_api/test_backends.py
 test/test_api/test_fault_api.py
 test/test_api/test_gempy_legacy_comp.py
 test/test_api/test_initialization_and_compute_api.py
@@ -100,16 +92,14 @@
 test/test_model_types/__init__.py
 test/test_model_types/test_example_models_I.py
 test/test_model_types/test_subduction.py
 test/test_modules/__init__.py
 test/test_modules/test_gempy_subsurface.py
 test/test_modules/_geophysics_TO_UPDATE/__init__.py
 test/test_modules/_geophysics_TO_UPDATE/test_gravity.py
-test/test_modules/_geophysics_TO_UPDATE/test_grid_tz.py
-test/test_modules/_geophysics_TO_UPDATE/test_magnetics.py
 test/test_modules/test_faults/__init__.py
 test/test_modules/test_faults/test_finite_faults.py
 test/test_modules/test_grids/__init__.py
 test/test_modules/test_grids/test_custom_grid.py
 test/test_modules/test_grids/test_diamond_square.py
 test/test_modules/test_grids/test_grids_I.py
 test/test_modules/test_grids/test_grids_sections.py
```

### Comparing `gempy-2023.1.0b6/setup.py` & `gempy-2023.2.0b1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 from setuptools import setup, find_packages
 
-version = '2023.1.0b6'
+
+with open("gempy/__init__.py", "r") as f:
+    for line in f:
+        if line.startswith("__version__"):
+            version = line.split("=")[1].strip().strip("'")
+            break
+
 
 
 def read_requirements(file_name):
+    requirements = []
     with open(file_name, "r", encoding="utf-8") as f:
-        return [line.strip() for line in f.readlines()]
+        for line in f:
+            # Strip whitespace and ignore comments
+            line = line.strip()
+            if line.startswith("#") or not line:
+                continue
+
+            # Handle -r directive
+            if line.startswith("-r "):
+                referenced_file = line.split()[1]  # Extract the file name
+                requirements.extend(read_requirements(referenced_file))  # Recursively read referenced file
+            else:
+                requirements.append(line)
+
+    return requirements
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gempy',
     version=version,
     packages=find_packages(exclude=('test', 'docs', 'examples')),
-    install_requires=read_requirements("requirements.txt"),
+    install_requires=read_requirements("requirements/requirements.txt"),
     extras_require={
-        "dev": read_requirements("dev-requirements.txt"),
-        "opt": read_requirements("optional-requirements.txt"),
+        "opt": read_requirements("requirements/optional-requirements.txt"),
+        "base": read_requirements("requirements/base-requirements.txt"),
     },
     url='https://github.com/cgre-aachen/gempy',
     license='EUPL-1.2',
     author='Miguel de la Varga, Alexander Zimmerman, Elisa Heim, Alexander Schaaf, Fabian Stamm, Florian Wellmann, Jan Niederau, Andrew Annex',
-    author_email='miguel@terranigma-solutions.com',
+    author_email='gempy@terranigma-solutions.com',
     description='An Open-source, Python-based 3-D structural geological modeling software.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['geology', '3-D modeling', 'structural geology', 'uncertainty'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `gempy-2023.1.0b6/test/test_api/test_backends.py` & `gempy-2023.2.0b1/test/test_api/test_backends.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/test/test_api/test_gempy_legacy_comp.py` & `gempy-2023.2.0b1/test/test_api/test_gempy_legacy_comp.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-﻿import gempy as gp
-import gempy_viewer
-from gempy.core.data import Solutions
-from gempy.API.gp2_gp3_compatibility.gp3_to_gp2_input import gempy3_to_gempy2
-from gempy.optional_dependencies import require_gempy_legacy
-from test.test_api.test_initialization_and_compute_api import _create_data
-
-# Skip pytest if legacy is not installed
-try:
-    require_gempy_legacy()
-except ImportError:
-    import pytest
-    pytest.skip("Legacy is not installed.", allow_module_level=True)
-
-
-
-def test_compare_numpy_with_legacy():
-    geo_data = _create_data()
-
-    gp.map_stack_to_surfaces(
-        gempy_model=geo_data,
-        mapping_object={"Strat_Series": ('rock2', 'rock1')}
-    )
-
-    sol: Solutions = gp.compute_model(geo_data)
-
-    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=True, show_boundaries=False)
-
-    legacy_model = gempy3_to_gempy2(geo_data)
-
-    gl = require_gempy_legacy()
-    gl.set_interpolator(legacy_model)
-    gl.compute_model(legacy_model)
-    gl.plot_2d(legacy_model, direction=['y'])
+﻿import gempy as gp
+import gempy_viewer
+from gempy.core.data import Solutions
+from gempy.API.gp2_gp3_compatibility.gp3_to_gp2_input import gempy3_to_gempy2
+from gempy.optional_dependencies import require_gempy_legacy
+from test.test_api.test_initialization_and_compute_api import _create_data
+
+# Skip pytest if legacy is not installed
+try:
+    require_gempy_legacy()
+except ImportError:
+    import pytest
+    pytest.skip("Legacy is not installed.", allow_module_level=True)
+
+
+
+def test_compare_numpy_with_legacy():
+    geo_data = _create_data()
+
+    gp.map_stack_to_surfaces(
+        gempy_model=geo_data,
+        mapping_object={"Strat_Series": ('rock2', 'rock1')}
+    )
+
+    sol: Solutions = gp.compute_model(geo_data)
+
+    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=True, show_boundaries=False)
+
+    legacy_model = gempy3_to_gempy2(geo_data)
+
+    gl = require_gempy_legacy()
+    gl.set_interpolator(legacy_model)
+    gl.compute_model(legacy_model)
+    gl.plot_2d(legacy_model, direction=['y'])
```

### Comparing `gempy-2023.1.0b6/test/test_api/test_initialization_and_compute_api.py` & `gempy-2023.2.0b1/test/test_api/test_initialization_and_compute_api.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-﻿from pprint import pprint
-
-import gempy as gp
-import gempy_viewer
-from gempy.core.data import GeoModel
-
-from gempy_engine.core.data.solutions import Solutions
-
-
-def test_api_create_data():
-    geo_data = _create_data()
-
-    pprint(geo_data)
-    return geo_data
-
-
-def _create_data():
-    data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
-    geo_data: GeoModel = gp.create_geomodel(
-        project_name='horizontal',
-        extent=[0, 1000, 0, 1000, 0, 1000],
-        resolution=[50, 5, 50],
-        importer_helper=gp.data.ImporterHelper(
-            path_to_surface_points=data_path + "/data/input_data/jan_models/model1_surface_points.csv",
-            path_to_orientations=data_path + "/data/input_data/jan_models/model1_orientations.csv"
-        )
-    )
-    return geo_data
-
-
-def test_map_stack_to_surfaces():
-    geo_data = _create_data()
-
-    gp.map_stack_to_surfaces(
-        gempy_model=geo_data,
-        mapping_object={"Strat_Series": ('rock2', 'rock1')}
-    )
-
-    pprint(geo_data.structural_frame)
-
-
-def test_api_compute_model():
-    geo_data = _create_data()
-
-    gp.map_stack_to_surfaces(
-        gempy_model=geo_data,
-        mapping_object={"Strat_Series": ('rock2', 'rock1')}
-    )
-
-    gempy_viewer.plot_2d(geo_data, direction=['y'])
-
-    sol: Solutions = gp.compute_model(geo_data)
-
-    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=True, show_boundaries=True, show_lith=False)
-    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=False, show_scalar=True)
+﻿from pprint import pprint
+
+import gempy as gp
+import gempy_viewer
+from gempy.core.data import GeoModel
+
+from gempy_engine.core.data.solutions import Solutions
+
+
+def test_api_create_data():
+    geo_data = _create_data()
+
+    pprint(geo_data)
+    return geo_data
+
+
+def _create_data():
+    data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
+    geo_data: GeoModel = gp.create_geomodel(
+        project_name='horizontal',
+        extent=[0, 1000, 0, 1000, 0, 1000],
+        resolution=[50, 5, 50],
+        importer_helper=gp.data.ImporterHelper(
+            path_to_surface_points=data_path + "/data/input_data/jan_models/model1_surface_points.csv",
+            path_to_orientations=data_path + "/data/input_data/jan_models/model1_orientations.csv"
+        )
+    )
+    return geo_data
+
+
+def test_map_stack_to_surfaces():
+    geo_data = _create_data()
+
+    gp.map_stack_to_surfaces(
+        gempy_model=geo_data,
+        mapping_object={"Strat_Series": ('rock2', 'rock1')}
+    )
+
+    pprint(geo_data.structural_frame)
+
+
+def test_api_compute_model():
+    geo_data = _create_data()
+
+    gp.map_stack_to_surfaces(
+        gempy_model=geo_data,
+        mapping_object={"Strat_Series": ('rock2', 'rock1')}
+    )
+
+    gempy_viewer.plot_2d(geo_data, direction=['y'])
+
+    sol: Solutions = gp.compute_model(geo_data)
+
+    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=True, show_boundaries=True, show_lith=False)
+    gempy_viewer.plot_2d(geo_data, direction=['y'], show_data=False, show_scalar=True)
```

### Comparing `gempy-2023.1.0b6/test/test_api/test_model_construction_granular.py` & `gempy-2023.2.0b1/test/test_api/test_model_construction_granular.py`

 * *Files identical despite different names*

### Comparing `gempy-2023.1.0b6/test/test_core/test_transfoms.py` & `gempy-2023.2.0b1/test/test_core/test_transfoms.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-﻿from gempy.core.data import GeoModel
-from gempy_engine.core.data.transforms import Transform
-from test.test_api.test_initialization_and_compute_api import _create_data
-import numpy as np
-import matplotlib.pyplot as plt
-
-
-def test_transform_1():
-    geo_data: GeoModel = _create_data()
-    print(geo_data.transform)
-    transformed_xyz = geo_data.transform.apply(geo_data.surface_points.xyz)
-    print(transformed_xyz)
-    return
-
-
-# Assuming you have your Transform class defined above this.
-
-def plot_points(points, title):
-    fig = plt.figure()
-    ax = fig.add_subplot(111, projection='3d')
-    ax.scatter(points[:, 0], points[:, 1], points[:, 2], c='r', marker='o')
-    ax.set_xlabel('X')
-    ax.set_ylabel('Y')
-    ax.set_zlabel('Z')
-    ax.set_title(title)
-    plt.show()
-
-
-def test_transform_operations_scale_move():
-    transform = Transform(
-        position=np.array([1, 2, 3]),
-        rotation=np.array([0, 0, 0]),
-        scale=np.array([2, 2, 2]))
-
-    original_points = np.array([
-        [0, 0, 0],
-        [1, 1, 1],
-        [-1, -1, -1]
-    ])
-
-    transformed_points = transform.apply(original_points)
-    inv_transformed_points = transform.apply_inverse(transformed_points)
-    fig = plt.figure()
-    ax = fig.add_subplot(111, projection='3d')
-
-    # Original points
-    ax.scatter(original_points[:, 0], original_points[:, 1], original_points[:, 2], c='r', marker='o', label='Original')
-    # Transformed points
-    ax.scatter(transformed_points[:, 0], transformed_points[:, 1], transformed_points[:, 2], c='g', marker='^', label='Transformed')
-    # Inverse transformed points
-    ax.scatter(inv_transformed_points[:, 0], inv_transformed_points[:, 1], inv_transformed_points[:, 2], c='b', marker='x', label='Inv Transformed')
-
-    ax.legend()
-    plt.show()
-
-    assert np.allclose(original_points, inv_transformed_points)
-
-
-
-def test_transform_operations_rotate():
-
-    transform = Transform(
-        position=np.array([0, 0, 0]),
-        rotation=np.array([45, 45, 45]),
-        scale=np.array([1, 1, 1]))
-
-    original_points = np.array([
-        [0, 0, 0],
-        [1, 1, 1],
-        [-1, -1, -1]
-    ])
-
-    transformed_points = transform.apply(original_points)
-    inv_transformed_points = transform.apply_inverse(transformed_points)
-
-    fig = plt.figure()
-    ax = fig.add_subplot(111, projection='3d')
-    # Original points
-    ax.scatter(original_points[:, 0], original_points[:, 1], original_points[:, 2], c='r', marker='o', label='Original')
-    # Transformed points
-    ax.scatter(transformed_points[:, 0], transformed_points[:, 1], transformed_points[:, 2], c='g', marker='^', label='Transformed')
-    # Inverse transformed points
-    ax.scatter(inv_transformed_points[:, 0], inv_transformed_points[:, 1], inv_transformed_points[:, 2], c='b', marker='x', label='Inv Transformed')
-
-    ax.legend()
-    plt.show()
-
-    assert np.allclose(original_points, inv_transformed_points)
+﻿from gempy.core.data import GeoModel
+from gempy_engine.core.data.transforms import Transform
+from test.test_api.test_initialization_and_compute_api import _create_data
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+def test_transform_1():
+    geo_data: GeoModel = _create_data()
+    print(geo_data.transform)
+    transformed_xyz = geo_data.transform.apply(geo_data.surface_points.xyz)
+    print(transformed_xyz)
+    return
+
+
+# Assuming you have your Transform class defined above this.
+
+def plot_points(points, title):
+    fig = plt.figure()
+    ax = fig.add_subplot(111, projection='3d')
+    ax.scatter(points[:, 0], points[:, 1], points[:, 2], c='r', marker='o')
+    ax.set_xlabel('X')
+    ax.set_ylabel('Y')
+    ax.set_zlabel('Z')
+    ax.set_title(title)
+    plt.show()
+
+
+def test_transform_operations_scale_move():
+    transform = Transform(
+        position=np.array([1, 2, 3]),
+        rotation=np.array([0, 0, 0]),
+        scale=np.array([2, 2, 2]))
+
+    original_points = np.array([
+        [0, 0, 0],
+        [1, 1, 1],
+        [-1, -1, -1]
+    ])
+
+    transformed_points = transform.apply(original_points)
+    inv_transformed_points = transform.apply_inverse(transformed_points)
+    fig = plt.figure()
+    ax = fig.add_subplot(111, projection='3d')
+
+    # Original points
+    ax.scatter(original_points[:, 0], original_points[:, 1], original_points[:, 2], c='r', marker='o', label='Original')
+    # Transformed points
+    ax.scatter(transformed_points[:, 0], transformed_points[:, 1], transformed_points[:, 2], c='g', marker='^', label='Transformed')
+    # Inverse transformed points
+    ax.scatter(inv_transformed_points[:, 0], inv_transformed_points[:, 1], inv_transformed_points[:, 2], c='b', marker='x', label='Inv Transformed')
+
+    ax.legend()
+    plt.show()
+
+    assert np.allclose(original_points, inv_transformed_points)
+
+
+
+def test_transform_operations_rotate():
+
+    transform = Transform(
+        position=np.array([0, 0, 0]),
+        rotation=np.array([45, 45, 45]),
+        scale=np.array([1, 1, 1]))
+
+    original_points = np.array([
+        [0, 0, 0],
+        [1, 1, 1],
+        [-1, -1, -1]
+    ])
+
+    transformed_points = transform.apply(original_points)
+    inv_transformed_points = transform.apply_inverse(transformed_points)
+
+    fig = plt.figure()
+    ax = fig.add_subplot(111, projection='3d')
+    # Original points
+    ax.scatter(original_points[:, 0], original_points[:, 1], original_points[:, 2], c='r', marker='o', label='Original')
+    # Transformed points
+    ax.scatter(transformed_points[:, 0], transformed_points[:, 1], transformed_points[:, 2], c='g', marker='^', label='Transformed')
+    # Inverse transformed points
+    ax.scatter(inv_transformed_points[:, 0], inv_transformed_points[:, 1], inv_transformed_points[:, 2], c='b', marker='x', label='Inv Transformed')
+
+    ax.legend()
+    plt.show()
+
+    assert np.allclose(original_points, inv_transformed_points)
```

### Comparing `gempy-2023.1.0b6/test/test_model_types/test_subduction.py` & `gempy-2023.2.0b1/test/test_model_types/test_subduction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-﻿import os
-
-import gempy as gp
-import gempy_viewer as gpv
-
-
-def test_subduction():
-    data_path = os.path.abspath('../../examples')
-
-    geo_model: gp.data.GeoModel = gp.create_geomodel(
-        project_name='Onlap_relations',
-        extent=[-200, 1000, -500, 500, -1000, 0],
-        resolution=[50, 50, 50],
-        number_octree_levels=5,
-        importer_helper=gp.data.ImporterHelper(
-            path_to_orientations=data_path + "/data/input_data/tut-ch1-4/tut_ch1-4_orientations.csv",
-            path_to_surface_points=data_path + "/data/input_data/tut-ch1-4/tut_ch1-4_points.csv",
-        )
-    )
-
-    gp.add_structural_group(
-        model=geo_model,
-        group_index=0,
-        structural_group_name="seafloor_series",
-        elements=[geo_model.structural_frame.get_element_by_name("seafloor")],
-        structural_relation=gp.data.StackRelationType.ERODE,
-    )
-
-    gp.add_structural_group(
-        model=geo_model,
-        group_index=1,
-        structural_group_name="right_series",
-        elements=[
-            geo_model.structural_frame.get_element_by_name("rock1"),
-            geo_model.structural_frame.get_element_by_name("rock2"),
-        ],
-        structural_relation=gp.data.StackRelationType.ONLAP
-    )
-
-    gp.add_structural_group(
-        model=geo_model,
-        group_index=2,
-        structural_group_name="onlap_series",
-        elements=[geo_model.structural_frame.get_element_by_name("onlap_surface")],
-        structural_relation=gp.data.StackRelationType.ERODE
-    )
-
-    gp.add_structural_group(
-        model=geo_model,
-        group_index=3,
-        structural_group_name="left_series",
-        elements=[geo_model.structural_frame.get_element_by_name("rock3")],
-        structural_relation=gp.data.StackRelationType.BASEMENT
-    )
-
-    gp.remove_structural_group_by_name(model=geo_model, group_name="default_formation")
-   
-   
-    # %%
-    from gempy_engine.core.data.options import DualContouringMaskingOptions
-    geo_model.interpolation_options.dual_contouring_masking_options = DualContouringMaskingOptions.INTERSECT
-    s = gp.compute_model(geo_model)
-
-    gpv.plot_2d(geo_model)
-    
-    # %% 
-    gpv.plot_3d(
-        model=geo_model,
-        show_surfaces=True,
-        show_data=True,
-        image=False,
-        show_topography=True,
-        kwargs_plot_structured_grid={'opacity': 0.1}
-    )
-
-    # %%
-    # ! White are True, black are False
-    if False:
-        p = gpv.plot_2d(
-            model=geo_model,
-            cell_number=2,
-            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[0],
-            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
-        )
-        gpv.plot_2d(
-            model=geo_model,
-            cell_number=2,
-            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[1],
-            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
-        )
-
-        gpv.plot_2d(
-            model=geo_model,
-            cell_number=2,
-            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[2],
-            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
-        )
-
-        gpv.plot_2d(
-            model=geo_model,
-            cell_number=2,
-            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[3],
-            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
-        )
+﻿import os
+
+import gempy as gp
+import gempy_viewer as gpv
+
+
+def test_subduction():
+    data_path = os.path.abspath('../../examples')
+
+    geo_model: gp.data.GeoModel = gp.create_geomodel(
+        project_name='Onlap_relations',
+        extent=[-200, 1000, -500, 500, -1000, 0],
+        resolution=[50, 50, 50],
+        refinement=5,
+        importer_helper=gp.data.ImporterHelper(
+            path_to_orientations=data_path + "/data/input_data/tut-ch1-4/tut_ch1-4_orientations.csv",
+            path_to_surface_points=data_path + "/data/input_data/tut-ch1-4/tut_ch1-4_points.csv",
+        )
+    )
+
+    gp.add_structural_group(
+        model=geo_model,
+        group_index=0,
+        structural_group_name="seafloor_series",
+        elements=[geo_model.structural_frame.get_element_by_name("seafloor")],
+        structural_relation=gp.data.StackRelationType.ERODE,
+    )
+
+    gp.add_structural_group(
+        model=geo_model,
+        group_index=1,
+        structural_group_name="right_series",
+        elements=[
+            geo_model.structural_frame.get_element_by_name("rock1"),
+            geo_model.structural_frame.get_element_by_name("rock2"),
+        ],
+        structural_relation=gp.data.StackRelationType.ONLAP
+    )
+
+    gp.add_structural_group(
+        model=geo_model,
+        group_index=2,
+        structural_group_name="onlap_series",
+        elements=[geo_model.structural_frame.get_element_by_name("onlap_surface")],
+        structural_relation=gp.data.StackRelationType.ERODE
+    )
+
+    gp.add_structural_group(
+        model=geo_model,
+        group_index=3,
+        structural_group_name="left_series",
+        elements=[geo_model.structural_frame.get_element_by_name("rock3")],
+        structural_relation=gp.data.StackRelationType.BASEMENT
+    )
+
+    gp.remove_structural_group_by_name(model=geo_model, group_name="default_formation")
+   
+   
+    # %%
+    from gempy_engine.core.data.options import MeshExtractionMaskingOptions
+    geo_model.interpolation_options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.INTERSECT
+    s = gp.compute_model(geo_model)
+
+    gpv.plot_2d(geo_model)
+    
+    # %% 
+    gpv.plot_3d(
+        model=geo_model,
+        show_surfaces=True,
+        show_data=True,
+        image=True,
+        show_topography=True,
+        kwargs_plot_structured_grid={'opacity': 0.1}
+    )
+
+    # %%
+    # ! White are True, black are False
+    if False:
+        p = gpv.plot_2d(
+            model=geo_model,
+            cell_number=2,
+            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[0],
+            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
+        )
+        gpv.plot_2d(
+            model=geo_model,
+            cell_number=2,
+            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[1],
+            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
+        )
+
+        gpv.plot_2d(
+            model=geo_model,
+            cell_number=2,
+            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[2],
+            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
+        )
+
+        gpv.plot_2d(
+            model=geo_model,
+            cell_number=2,
+            override_regular_grid=geo_model.solutions.raw_arrays.mask_matrix_squeezed[3],
+            show_data=True, kwargs_lithology={'cmap': 'gray', 'norm': None}
+        )
```

### Comparing `gempy-2023.1.0b6/test/test_modules/test_faults/test_finite_faults.py` & `gempy-2023.2.0b1/test/test_modules/test_faults/test_finite_faults.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import numpy as np
-import pytest
-
-import gempy as gp
-import gempy_viewer as gpv
-from gempy.core.data.enumerators import ExampleModel
-from gempy_viewer.optional_dependencies import require_pyvista
-from test.conftest import TEST_SPEED, TestSpeed
-
-center = np.array([500, 500, 500])
-radius = np.array([500, 100, 200]) / 2
-k = np.array([1, 1, 1]) * 1
-
-PLOT = False
-# TODO: Add the approval test check
-
-
-@pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
-def test_finite_fault_scalar_field_on_fault():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ONE_FAULT,
-        compute_model=False
-    )
-
-    regular_grid = geo_model.grid.regular_grid
-
-    # TODO: Extract grid from the model
-    scaled_center = geo_model.transform.apply(center.reshape(1, -1))[0]
-    scaled_radius = geo_model.transform.scale_points(radius.reshape(1, -1))[0]
-    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
-        center=scaled_center,
-        radius=scaled_radius,
-        max_slope=k  # * This controls the speed of the transition
-    )
-
-    transform = gp.data.Transform(
-        position=np.array([0, 0, 0]),
-        rotation=np.array([0, 60, 0]),
-        scale=np.ones(3)
-    )
-
-    faults_data = gp.data.FaultsData(
-        fault_values_everywhere=np.zeros(0),
-        fault_values_on_sp=np.zeros(0),
-        thickness=None,
-        fault_values_ref=np.zeros(0),
-        fault_values_rest=np.zeros(0),
-        finite_fault_data=gp.data.FiniteFaultData(
-            implicit_function=scalar_funtion,
-            implicit_function_transform=transform,
-            pivot=scaled_center,
-        )
-    )
-
-    geo_model.structural_frame.structural_groups[0].faults_input_data = faults_data
-    gp.compute_model(geo_model)
-
-    # TODO: Try to do this afterwards
-    # scalar_fault = scalar_funtion(regular_grid.values)
-
-    if plot_pyvista := True:
-        plot3d = gpv.plot_3d(
-            geo_model,
-            show_lith=False,
-            show=False
-        )
-        scalar_block_for_viz = _apply(
-            regular_grid=regular_grid,
-            scalar_funtion=gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
-                center=center,
-                radius=radius,
-                max_slope=k  # * This controls the speed of the transition
-            ),
-            transform=transform
-        )
-        _plot_scalar_field(regular_grid, scalar_block_for_viz, plot3d.p, background_field=False)
-        
-        
-def test_finite_fault_scalar_field():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ONE_FAULT,
-        compute_model=False
-    )
-
-    regular_grid = geo_model.grid.regular_grid
-
-    # TODO: Extract grid from the model
-    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
-        center=center,
-        radius=radius,
-        max_slope=k  # * This controls the speed of the transition
-    )
-
-    transform = gp.data.Transform(
-        position=np.array([0, 0, 0]),
-        rotation=np.array([0, 0, 30]),
-        scale=np.ones(3)
-    )
-
-    transformed_points = transform.apply_inverse_with_pivot(
-        points=regular_grid.values,
-        pivot=center
-    )
-    scalar_block = scalar_funtion(transformed_points)
-
-    # TODO: Try to do this afterwards
-    # scalar_fault = scalar_funtion(regular_grid.values)
-
-    if plot_pyvista := True:
-        _plot_scalar_field(regular_grid, scalar_block)
-
-
-@pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
-def test_finite_fault_scalar_field_on_fault_ZERO():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ONE_FAULT,
-        compute_model=True
-    )
-
-    regular_grid = geo_model.grid.regular_grid
-
-    # TODO: Extract grid from the model
-    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
-        center=center,
-        radius=radius,
-        max_slope=k  # * This controls the speed of the transition
-    )
-
-    transform = gp.data.Transform(
-        position=np.array([0, 0, 0]),
-        rotation=np.array([0, 0, 30]),
-        scale=np.ones(3)
-    )
-
-    transformed_points = transform.apply_inverse_with_pivot(
-        points=regular_grid.values,
-        pivot=center
-    )
-    
-    scalar_block = scalar_funtion(transformed_points)
-
-    # TODO: Try to do this afterwards
-    # scalar_fault = scalar_funtion(regular_grid.values)
-
-    if plot_pyvista := True:
-        plot3d = gpv.plot_3d(
-            geo_model,
-            show=False
-        )
-        _plot_scalar_field(regular_grid, scalar_block, plot3d.p)
-
-
-def _apply(regular_grid, scalar_funtion, transform):
-    transformed_points = transform.apply_inverse_with_pivot(
-        points=regular_grid.values,  # ! This depends on the octree
-        pivot=center
-    )
-    scalar_block = scalar_funtion(transformed_points)
-    return scalar_block
-
-
-def _plot_scalar_field(regular_grid, scalar_block, plotter=None, background_field=True):
-    if not PLOT:
-        return
-    
-    pv = require_pyvista()
-    p = plotter or pv.Plotter()
-    regular_grid_values = regular_grid.values_vtk_format
-    grid_3d = regular_grid_values.reshape(*(regular_grid.resolution + 1), 3).T
-    regular_grid_mesh = pv.StructuredGrid(*grid_3d)
-    regular_grid_mesh["lith"] = scalar_block
-    if True:
-        area_of_effect = regular_grid_mesh.threshold([.000000001, 1.1])
-        p.add_mesh(area_of_effect, show_edges=True, opacity=.4)
-
-        area_of_effect_2 = regular_grid_mesh.threshold([.2, 1.1])
-        p.add_mesh(area_of_effect_2, show_edges=True, opacity=.8)
-    if background_field:
-        p.add_mesh(regular_grid_mesh, show_edges=False, opacity=.2)
-    p.show_bounds(bounds=regular_grid.extent)
-    # * Add the fault
-    if False:
-        dual_mesh = pv.PolyData(fault_mesh.vertices, np.insert(fault_mesh.edges, 0, 3, axis=1).ravel())
-        dual_mesh["bar"] = scalar_fault
-        p.add_mesh(dual_mesh, opacity=1, silhouette=True, show_edges=True)
-    p.show()
+import numpy as np
+import pytest
+
+import gempy as gp
+import gempy_viewer as gpv
+from gempy.core.data.enumerators import ExampleModel
+from gempy_viewer.optional_dependencies import require_pyvista
+from test.conftest import TEST_SPEED, TestSpeed
+
+center = np.array([500, 500, 500])
+radius = np.array([500, 100, 200]) / 2
+k = np.array([1, 1, 1]) * 1
+
+PLOT = False
+# TODO: Add the approval test check
+
+
+@pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
+def test_finite_fault_scalar_field_on_fault():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ONE_FAULT,
+        compute_model=False
+    )
+
+    regular_grid = geo_model.grid.regular_grid
+
+    # TODO: Extract grid from the model
+    scaled_center = geo_model.transform.apply(center.reshape(1, -1))[0]
+    scaled_radius = geo_model.transform.scale_points(radius.reshape(1, -1))[0]
+    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
+        center=scaled_center,
+        radius=scaled_radius,
+        max_slope=k  # * This controls the speed of the transition
+    )
+
+    transform = gp.data.Transform(
+        position=np.array([0, 0, 0]),
+        rotation=np.array([0, 60, 0]),
+        scale=np.ones(3)
+    )
+
+    faults_data = gp.data.FaultsData(
+        fault_values_everywhere=np.zeros(0),
+        fault_values_on_sp=np.zeros(0),
+        thickness=None,
+        fault_values_ref=np.zeros(0),
+        fault_values_rest=np.zeros(0),
+        finite_fault_data=gp.data.FiniteFaultData(
+            implicit_function=scalar_funtion,
+            implicit_function_transform=transform,
+            pivot=scaled_center,
+        )
+    )
+
+    geo_model.structural_frame.structural_groups[0].faults_input_data = faults_data
+    gp.compute_model(geo_model)
+
+    # TODO: Try to do this afterwards
+    # scalar_fault = scalar_funtion(regular_grid.values)
+
+    if plot_pyvista := True:
+        plot3d = gpv.plot_3d(
+            geo_model,
+            show_lith=False,
+            show=False
+        )
+        scalar_block_for_viz = _apply(
+            regular_grid=regular_grid,
+            scalar_funtion=gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
+                center=center,
+                radius=radius,
+                max_slope=k  # * This controls the speed of the transition
+            ),
+            transform=transform
+        )
+        _plot_scalar_field(regular_grid, scalar_block_for_viz, plot3d.p, background_field=False)
+        
+        
+def test_finite_fault_scalar_field():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ONE_FAULT,
+        compute_model=False
+    )
+
+    regular_grid = geo_model.grid.regular_grid
+
+    # TODO: Extract grid from the model
+    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
+        center=center,
+        radius=radius,
+        max_slope=k  # * This controls the speed of the transition
+    )
+
+    transform = gp.data.Transform(
+        position=np.array([0, 0, 0]),
+        rotation=np.array([0, 0, 30]),
+        scale=np.ones(3)
+    )
+
+    transformed_points = transform.apply_inverse_with_pivot(
+        points=regular_grid.values,
+        pivot=center
+    )
+    scalar_block = scalar_funtion(transformed_points)
+
+    # TODO: Try to do this afterwards
+    # scalar_fault = scalar_funtion(regular_grid.values)
+
+    if plot_pyvista := True:
+        _plot_scalar_field(regular_grid, scalar_block)
+
+
+@pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
+def test_finite_fault_scalar_field_on_fault_ZERO():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ONE_FAULT,
+        compute_model=True
+    )
+
+    regular_grid = geo_model.grid.regular_grid
+
+    # TODO: Extract grid from the model
+    scalar_funtion: callable = gp.implicit_functions.ellipsoid_3d_factory(  # * This paints the 3d regular grid
+        center=center,
+        radius=radius,
+        max_slope=k  # * This controls the speed of the transition
+    )
+
+    transform = gp.data.Transform(
+        position=np.array([0, 0, 0]),
+        rotation=np.array([0, 0, 30]),
+        scale=np.ones(3)
+    )
+
+    transformed_points = transform.apply_inverse_with_pivot(
+        points=regular_grid.values,
+        pivot=center
+    )
+    
+    scalar_block = scalar_funtion(transformed_points)
+
+    # TODO: Try to do this afterwards
+    # scalar_fault = scalar_funtion(regular_grid.values)
+
+    if plot_pyvista := True:
+        plot3d = gpv.plot_3d(
+            geo_model,
+            show=False
+        )
+        _plot_scalar_field(regular_grid, scalar_block, plot3d.p)
+
+
+def _apply(regular_grid, scalar_funtion, transform):
+    transformed_points = transform.apply_inverse_with_pivot(
+        points=regular_grid.values,  # ! This depends on the octree
+        pivot=center
+    )
+    scalar_block = scalar_funtion(transformed_points)
+    return scalar_block
+
+
+def _plot_scalar_field(regular_grid, scalar_block, plotter=None, background_field=True):
+    if not PLOT:
+        return
+    
+    pv = require_pyvista()
+    p = plotter or pv.Plotter()
+    regular_grid_values = regular_grid.values_vtk_format
+    grid_3d = regular_grid_values.reshape(*(regular_grid.resolution + 1), 3).T
+    regular_grid_mesh = pv.StructuredGrid(*grid_3d)
+    regular_grid_mesh["lith"] = scalar_block
+    if True:
+        area_of_effect = regular_grid_mesh.threshold([.000000001, 1.1])
+        p.add_mesh(area_of_effect, show_edges=True, opacity=.4)
+
+        area_of_effect_2 = regular_grid_mesh.threshold([.2, 1.1])
+        p.add_mesh(area_of_effect_2, show_edges=True, opacity=.8)
+    if background_field:
+        p.add_mesh(regular_grid_mesh, show_edges=False, opacity=.2)
+    p.show_bounds(bounds=regular_grid.extent)
+    # * Add the fault
+    if False:
+        dual_mesh = pv.PolyData(fault_mesh.vertices, np.insert(fault_mesh.edges, 0, 3, axis=1).ravel())
+        dual_mesh["bar"] = scalar_fault
+        p.add_mesh(dual_mesh, opacity=1, silhouette=True, show_edges=True)
+    p.show()
```

### Comparing `gempy-2023.1.0b6/test/test_modules/test_gempy_subsurface.py` & `gempy-2023.2.0b1/test/test_modules/test_gempy_subsurface.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,51 @@
-﻿import gempy as gp
-import gempy_viewer as gpv
-from gempy.core.data.enumerators import ExampleModel
-import numpy as np
-import subsurface as ss
-import pandas as pd
-
-
-def test_gempy_to_subsurface():
-    model = gp.generate_example_model(ExampleModel.ANTICLINE, compute_model=True)
-    if False:
-        gpv.plot_3d(model)
-
-    vertex: list[np.ndarray] = model.solutions.raw_arrays.vertices
-    simplex_list: list[np.ndarray] = model.solutions.raw_arrays.edges
-
-    idx_max = 0
-    for simplex_array in simplex_list:
-        simplex_array += idx_max
-        idx_max = simplex_array.max() + 1
-
-    id_array = [np.full(v.shape[0], i + 1) for i, v in enumerate(vertex)]
-
-    concatenated_id_array = np.concatenate(id_array)
-    meshes: ss.UnstructuredData = ss.UnstructuredData.from_array(
-        vertex=np.concatenate(vertex),
-        cells=np.concatenate(simplex_list),
-        vertex_attr=pd.DataFrame({'id': concatenated_id_array})
-    )
-
-    trisurf = ss.TriSurf(meshes)
-    pyvista_mesh = ss.visualization.to_pyvista_mesh(trisurf)
-    ss.visualization.pv_plot([pyvista_mesh], image_2d=False)
-
-
-def test_gempy_to_subsurface_II():
-    model = gp.generate_example_model(ExampleModel.ANTICLINE, compute_model=True)
-    meshes: ss.UnstructuredData = model.solutions.raw_arrays.meshes_to_subsurface()
-
-    trisurf = ss.TriSurf(meshes)
-    pyvista_mesh = ss.visualization.to_pyvista_mesh(trisurf)
-    ss.visualization.pv_plot([pyvista_mesh], image_2d=False)
+﻿import gempy as gp
+import gempy_viewer as gpv
+from gempy.core.data.enumerators import ExampleModel
+import numpy as np
+import subsurface as ss
+import pandas as pd
+
+
+def test_gempy_to_subsurface():
+    model = gp.generate_example_model(ExampleModel.ANTICLINE, compute_model=True)
+    if False:
+        gpv.plot_3d(model)
+
+    vertex: list[np.ndarray] = model.solutions.raw_arrays.vertices
+    simplex_list: list[np.ndarray] = model.solutions.raw_arrays.edges
+
+    idx_max = 0
+    for simplex_array in simplex_list:
+        simplex_array += idx_max
+        idx_max = simplex_array.max() + 1
+
+    id_array = [np.full(v.shape[0], i + 1) for i, v in enumerate(vertex)]
+
+    concatenated_id_array = np.concatenate(id_array)
+    meshes: ss.UnstructuredData = ss.UnstructuredData.from_array(
+        vertex=np.concatenate(vertex),
+        cells=np.concatenate(simplex_list),
+        vertex_attr=pd.DataFrame({'id': concatenated_id_array})
+    )
+
+    trisurf = ss.TriSurf(meshes)
+    pyvista_mesh = ss.visualization.to_pyvista_mesh(trisurf)
+    ss.visualization.pv_plot([pyvista_mesh], image_2d=True)
+
+
+def test_gempy_to_subsurface_II():
+    model = gp.generate_example_model(ExampleModel.ANTICLINE, compute_model=True)
+    meshes: ss.UnstructuredData = model.solutions.raw_arrays.meshes_to_subsurface()
+
+    trisurf = ss.TriSurf(meshes)
+    pyvista_mesh = ss.visualization.to_pyvista_mesh(trisurf)
+    ss.visualization.pv_plot([pyvista_mesh], image_2d=True)
+
+
+def test_gempy_to_subsurface_III():
+    model = gp.generate_example_model(ExampleModel.ANTICLINE, compute_model=True)
+    meshes: ss.UnstructuredData = model.solutions.meshes_to_unstruct()
+
+    trisurf = ss.TriSurf(meshes)
+    pyvista_mesh = ss.visualization.to_pyvista_mesh(trisurf)
+    ss.visualization.pv_plot([pyvista_mesh], image_2d=True)
```

### Comparing `gempy-2023.1.0b6/test/test_modules/test_grids/test_custom_grid.py` & `gempy-2023.2.0b1/test/test_modules/test_grids/test_custom_grid.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-﻿import numpy as np
-import pytest
-
-from test.conftest import TEST_SPEED, TestSpeed
-import gempy as gp
-from gempy.core.data.enumerators import ExampleModel
-
-pytestmark = pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
-
-xyz_coord = np.array(
-    [[0, 0, 0],
-     [1000, 0, 0],
-     [0, 1000, 0],
-     [1000, 1000, 0],
-     [0, 0, 1000],
-     [1000, 0, 1000],
-     [0, 1000, 1000],
-     [1000, 1000, 1000]]
-)
-
-
-def test_custom_grid():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ANTICLINE,
-        compute_model=False
-    )
-
-    geo_model.interpolation_options.number_octree_levels = 2
-
-    gp.set_custom_grid(
-        grid=geo_model.grid,
-        xyz_coord=xyz_coord
-    )
-
-    sol: gp.data.Solutions = gp.compute_model(geo_model)
-    np.testing.assert_array_equal(
-        sol.raw_arrays.custom,
-        np.array([3., 3., 3., 3., 1., 1., 1., 1.])
-    )
-
-
-def test_compute_at():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ANTICLINE,
-        compute_model=False
-    )
-
-    geo_model.interpolation_options.number_octree_levels = 2
-    sol: np.ndarray = gp.compute_model_at(
-        gempy_model=geo_model,
-        at=xyz_coord
-    )
-    
-    np.testing.assert_array_equal(
-        sol,
-        np.array([3., 3., 3., 3., 1., 1., 1., 1.])
-    )
+﻿import numpy as np
+import pytest
+
+from test.conftest import TEST_SPEED, TestSpeed
+import gempy as gp
+from gempy.core.data.enumerators import ExampleModel
+
+pytestmark = pytest.mark.skipif(TEST_SPEED.value < TestSpeed.SECONDS.value, reason="Global test speed below this test value.")
+
+xyz_coord = np.array(
+    [[0, 0, 0],
+     [1000, 0, 0],
+     [0, 1000, 0],
+     [1000, 1000, 0],
+     [0, 0, 1000],
+     [1000, 0, 1000],
+     [0, 1000, 1000],
+     [1000, 1000, 1000]]
+)
+
+
+def test_custom_grid():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ANTICLINE,
+        compute_model=False
+    )
+
+    geo_model.interpolation_options.number_octree_levels = 2
+
+    gp.set_custom_grid(
+        grid=geo_model.grid,
+        xyz_coord=xyz_coord
+    )
+
+    sol: gp.data.Solutions = gp.compute_model(geo_model)
+    np.testing.assert_array_equal(
+        sol.raw_arrays.custom,
+        np.array([3., 3., 3., 3., 1., 1., 1., 1.])
+    )
+
+
+def test_compute_at():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ANTICLINE,
+        compute_model=False
+    )
+
+    geo_model.interpolation_options.number_octree_levels = 2
+    sol: np.ndarray = gp.compute_model_at(
+        gempy_model=geo_model,
+        at=xyz_coord
+    )
+    
+    np.testing.assert_array_equal(
+        sol,
+        np.array([3., 3., 3., 3., 1., 1., 1., 1.])
+    )
```

### Comparing `gempy-2023.1.0b6/test/test_modules/test_grids/test_diamond_square.py` & `gempy-2023.2.0b1/test/test_modules/test_grids/test_diamond_square.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import gempy.core.data.grid_modules.diamond_square
-import pytest  # to add fixtures and to test error raises
-import numpy as np  # as another testing environment
-
-
-def test_class_nocrash():
-    """Simply check if class can be instantiated"""
-    gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
-
-
-def test_grid_generation():
-    """Test grid generation and extension for non-suitable grid sizes"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
-    assert ds.grid.shape == (5, 5)
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(8, 10))
-    assert ds.grid.shape == (9, 17)
-
-
-def test_diamond_selection():
-    """Test selection of diamond positions"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
-    z = ds.get_selection_diamond(1)
-    assert np.all(z == np.array([[2, 0, 0, 0, 2],
-                                 [0, 0, 0, 0, 0],
-                                 [0, 0, 1, 0, 0],
-                                 [0, 0, 0, 0, 0],
-                                 [2, 0, 0, 0, 2]]))
-    z = ds.get_selection_diamond(0)
-    assert np.all(z == np.array([[2, 0, 2, 0, 2],
-                                 [0, 1, 0, 1, 0],
-                                 [2, 0, 2, 0, 2],
-                                 [0, 1, 0, 1, 0],
-                                 [2, 0, 2, 0, 2]]))
-
-
-def test_square_selection():
-    """Test selection of diamond positions"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
-    z = ds.get_selection_square(0)
-    assert np.all(z == np.array([[0, 0, 2, 0, 2, 0, 0],
-                                 [0, 2, 1, 2, 1, 2, 0],
-                                 [2, 1, 2, 1, 2, 1, 2],
-                                 [0, 2, 1, 2, 1, 2, 0],
-                                 [2, 1, 2, 1, 2, 1, 2],
-                                 [0, 2, 1, 2, 1, 2, 0],
-                                 [0, 0, 2, 0, 2, 0, 0]]))
-    z = ds.get_selection_square(1)
-    assert np.all(z == np.array([[0, 0, 0, 0, 2, 0, 0, 0, 0],
-                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
-                                 [0, 0, 2, 0, 1, 0, 2, 0, 0],
-                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
-                                 [2, 0, 1, 0, 2, 0, 1, 0, 2],
-                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
-                                 [0, 0, 2, 0, 1, 0, 2, 0, 0],
-                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
-                                 [0, 0, 0, 0, 2, 0, 0, 0, 0]]))
-
-
-def test_random_initialization():
-    """Test random initialization of corner points"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 6), seed=52062)
-    ds.random_initialization()
-    m_pow_max = min(ds.n, ds.m)
-    step_size = int(2 ** m_pow_max)
-    np.testing.assert_array_almost_equal(ds.grid[::step_size, ::step_size],
-                                         np.array([[0.35127005, 0.55476571, 0.93745213],
-                                                   [0.66668382, 0.85215985, 0.53222795]]))
-
-
-def test_random_initialization_level():
-    """Test random initialization on lower level"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
-    level = 3
-    ds.random_initialization(level=level)
-    step_size = int(2 ** level)
-    np.testing.assert_array_almost_equal(ds.grid[::step_size, ::step_size],
-                                         np.array([[0.35127005, 0.55476571, 0.93745213, 0.66668382, 0.85215985],
-                                                   [0.53222795, 0.55800027, 0.20974513, 0.74837501, 0.64394326],
-                                                   [0.0359961, 0.22723278, 0.56347804, 0.13438884, 0.32613594],
-                                                   [0.20868763, 0.03116471, 0.1498014, 0.20755495, 0.86021482],
-                                                   [0.64707457, 0.44744272, 0.36504945, 0.52473407, 0.27948164]]))
-
-def test_reset_grid():
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 6), seed=52062)
-    ds.random_initialization()
-    ds.reset_grid()
-    np.testing.assert_array_almost_equal(ds.grid,
-                                         np.array([[0., 0., 0., 0., 0., 0., 0., 0., 0.],
-                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
-                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
-                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
-                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.]]))
-
-
-def test_random_func():
-    """Test random function implementation"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
-    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
-                                         np.array([-0.14872995, 0.05476571]))
-    # testing for correct default implementation
-    ds.r_type = 'default'
-    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
-                                         np.array([0.43745213, 0.16668382]))
-    # testing long-range correlation
-    ds.r_type = 'long_range'
-    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
-                                         np.array([0.04401998, 0.00402849]))
-    # testing level-scale correlation
-    ds.r_type = 'level_scale'
-    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
-                                         np.array([0.18600009, 0.06991504]))
-    # testing deterministic implementation (no random value)
-    ds.r_type = 'deterministic'
-    assert ds.random_func(2, 2) == 0.0
-
-
-def test_random_func_raises_error():
-    """Test if random function raises NonImplementedError correctly"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
-    ds.r_type = 'fail'
-
-    with pytest.raises(NotImplementedError):
-        ds.random_func(2, 2)
-
-
-def test_interpolate():
-    """Test interpolation step itself"""
-    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(9, 9), seed=52062)
-    ds.interpolate()
-    np.testing.assert_array_almost_equal(ds.grid,
-                                         np.array([[0., 0.2951411, 0.21781267, 0.29361906, 0.01037812,
-                                                    -0.0376406, -0.59889259, 0.01136296, 0.],
-                                                   [-0.13102895, -0.07079394, 0.40240191, -0.24139454, -0.64535709,
-                                                    -0.25358984, -0.20811689, -0.38977623, -0.02280871],
-                                                   [-0.32311967, -0.08246826, 0.03236034, -0.72313104, -0.6863271,
-                                                    -0.09742037, 0.16154592, -0.41643384, -0.23968483],
-                                                   [-0.53344647, -0.09313507, -0.66247738, -0.42849468, -0.06519284,
-                                                    -0.50628043, -0.31159035, 0.53516982, 0.07387422],
-                                                   [0.23421434, 0.32817758, -0.45156142, -0.24627659, -0.2974599,
-                                                    0.16071127, 0.36261452, 0.62070397, 0.60516641],
-                                                   [-0.20172896, -0.05668301, -0.26331217, -0.22196496, 0.42029741,
-                                                    0.35078669, 0.77129922, 0.38999358, 0.95701668],
-                                                   [-0.41296032, -0.04377428, -0.23235603, 0.60954786, 0.72643437,
-                                                    0.37788456, 0.62211967, 0.16198846, 0.61709021],
-                                                   [0.00192109, -0.28399285, 0.28596529, 0.54081866, 1.00235637,
-                                                    0.25454729, 0.1248549, 0.85789169, 0.23511424],
-                                                   [0., -0.54507578, -0.33592062, 0.62216544, 0.77575097,
-                                                    0.5338132, 0.22007596, 0.02926128, 0.]]))
+import gempy.core.data.grid_modules.diamond_square
+import pytest  # to add fixtures and to test error raises
+import numpy as np  # as another testing environment
+
+
+def test_class_nocrash():
+    """Simply check if class can be instantiated"""
+    gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
+
+
+def test_grid_generation():
+    """Test grid generation and extension for non-suitable grid sizes"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
+    assert ds.grid.shape == (5, 5)
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(8, 10))
+    assert ds.grid.shape == (9, 17)
+
+
+def test_diamond_selection():
+    """Test selection of diamond positions"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
+    z = ds.get_selection_diamond(1)
+    assert np.all(z == np.array([[2, 0, 0, 0, 2],
+                                 [0, 0, 0, 0, 0],
+                                 [0, 0, 1, 0, 0],
+                                 [0, 0, 0, 0, 0],
+                                 [2, 0, 0, 0, 2]]))
+    z = ds.get_selection_diamond(0)
+    assert np.all(z == np.array([[2, 0, 2, 0, 2],
+                                 [0, 1, 0, 1, 0],
+                                 [2, 0, 2, 0, 2],
+                                 [0, 1, 0, 1, 0],
+                                 [2, 0, 2, 0, 2]]))
+
+
+def test_square_selection():
+    """Test selection of diamond positions"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 5))
+    z = ds.get_selection_square(0)
+    assert np.all(z == np.array([[0, 0, 2, 0, 2, 0, 0],
+                                 [0, 2, 1, 2, 1, 2, 0],
+                                 [2, 1, 2, 1, 2, 1, 2],
+                                 [0, 2, 1, 2, 1, 2, 0],
+                                 [2, 1, 2, 1, 2, 1, 2],
+                                 [0, 2, 1, 2, 1, 2, 0],
+                                 [0, 0, 2, 0, 2, 0, 0]]))
+    z = ds.get_selection_square(1)
+    assert np.all(z == np.array([[0, 0, 0, 0, 2, 0, 0, 0, 0],
+                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
+                                 [0, 0, 2, 0, 1, 0, 2, 0, 0],
+                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
+                                 [2, 0, 1, 0, 2, 0, 1, 0, 2],
+                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
+                                 [0, 0, 2, 0, 1, 0, 2, 0, 0],
+                                 [0, 0, 0, 0, 0, 0, 0, 0, 0],
+                                 [0, 0, 0, 0, 2, 0, 0, 0, 0]]))
+
+
+def test_random_initialization():
+    """Test random initialization of corner points"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 6), seed=52062)
+    ds.random_initialization()
+    m_pow_max = min(ds.n, ds.m)
+    step_size = int(2 ** m_pow_max)
+    np.testing.assert_array_almost_equal(ds.grid[::step_size, ::step_size],
+                                         np.array([[0.35127005, 0.55476571, 0.93745213],
+                                                   [0.66668382, 0.85215985, 0.53222795]]))
+
+
+def test_random_initialization_level():
+    """Test random initialization on lower level"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
+    level = 3
+    ds.random_initialization(level=level)
+    step_size = int(2 ** level)
+    np.testing.assert_array_almost_equal(ds.grid[::step_size, ::step_size],
+                                         np.array([[0.35127005, 0.55476571, 0.93745213, 0.66668382, 0.85215985],
+                                                   [0.53222795, 0.55800027, 0.20974513, 0.74837501, 0.64394326],
+                                                   [0.0359961, 0.22723278, 0.56347804, 0.13438884, 0.32613594],
+                                                   [0.20868763, 0.03116471, 0.1498014, 0.20755495, 0.86021482],
+                                                   [0.64707457, 0.44744272, 0.36504945, 0.52473407, 0.27948164]]))
+
+def test_reset_grid():
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(5, 6), seed=52062)
+    ds.random_initialization()
+    ds.reset_grid()
+    np.testing.assert_array_almost_equal(ds.grid,
+                                         np.array([[0., 0., 0., 0., 0., 0., 0., 0., 0.],
+                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
+                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
+                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.],
+                                                   [0., 0., 0., 0., 0., 0., 0., 0., 0.]]))
+
+
+def test_random_func():
+    """Test random function implementation"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
+    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
+                                         np.array([-0.14872995, 0.05476571]))
+    # testing for correct default implementation
+    ds.r_type = 'default'
+    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
+                                         np.array([0.43745213, 0.16668382]))
+    # testing long-range correlation
+    ds.r_type = 'long_range'
+    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
+                                         np.array([0.04401998, 0.00402849]))
+    # testing level-scale correlation
+    ds.r_type = 'level_scale'
+    np.testing.assert_array_almost_equal(ds.random_func(2, 2),
+                                         np.array([0.18600009, 0.06991504]))
+    # testing deterministic implementation (no random value)
+    ds.r_type = 'deterministic'
+    assert ds.random_func(2, 2) == 0.0
+
+
+def test_random_func_raises_error():
+    """Test if random function raises NonImplementedError correctly"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(33, 33), seed=52062)
+    ds.r_type = 'fail'
+
+    with pytest.raises(NotImplementedError):
+        ds.random_func(2, 2)
+
+
+def test_interpolate():
+    """Test interpolation step itself"""
+    ds = gempy.core.data.grid_modules.diamond_square.DiaomondSquare(size=(9, 9), seed=52062)
+    ds.interpolate()
+    np.testing.assert_array_almost_equal(ds.grid,
+                                         np.array([[0., 0.2951411, 0.21781267, 0.29361906, 0.01037812,
+                                                    -0.0376406, -0.59889259, 0.01136296, 0.],
+                                                   [-0.13102895, -0.07079394, 0.40240191, -0.24139454, -0.64535709,
+                                                    -0.25358984, -0.20811689, -0.38977623, -0.02280871],
+                                                   [-0.32311967, -0.08246826, 0.03236034, -0.72313104, -0.6863271,
+                                                    -0.09742037, 0.16154592, -0.41643384, -0.23968483],
+                                                   [-0.53344647, -0.09313507, -0.66247738, -0.42849468, -0.06519284,
+                                                    -0.50628043, -0.31159035, 0.53516982, 0.07387422],
+                                                   [0.23421434, 0.32817758, -0.45156142, -0.24627659, -0.2974599,
+                                                    0.16071127, 0.36261452, 0.62070397, 0.60516641],
+                                                   [-0.20172896, -0.05668301, -0.26331217, -0.22196496, 0.42029741,
+                                                    0.35078669, 0.77129922, 0.38999358, 0.95701668],
+                                                   [-0.41296032, -0.04377428, -0.23235603, 0.60954786, 0.72643437,
+                                                    0.37788456, 0.62211967, 0.16198846, 0.61709021],
+                                                   [0.00192109, -0.28399285, 0.28596529, 0.54081866, 1.00235637,
+                                                    0.25454729, 0.1248549, 0.85789169, 0.23511424],
+                                                   [0., -0.54507578, -0.33592062, 0.62216544, 0.77575097,
+                                                    0.5338132, 0.22007596, 0.02926128, 0.]]))
```

### Comparing `gempy-2023.1.0b6/test/test_modules/test_grids/test_grids_I.py` & `gempy-2023.2.0b1/test/test_modules/test_grids/test_grids_I.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-﻿import pytest
-
-import gempy as gp
-import gempy_viewer as gpv
-from gempy.core.data.enumerators import ExampleModel
-from gempy_engine.modules.octrees_topology.octrees_topology_interface import ValueType
-from gempy_engine.plugins.plotting.helper_functions import plot_block_and_input_2d
-from test.conftest import TEST_SPEED, TestSpeed
-
-
-pytestmark = pytest.mark.skipif(TEST_SPEED.value < TestSpeed.MINUTES.value, reason="Global test speed below this test value.")
-
-
-def  test_octree():
-    geo_model: gp.data.GeoModel = gp.generate_example_model(
-        example_model=ExampleModel.ANTICLINE,
-        compute_model=False
-    ) 
-    
-    geo_model.interpolation_options.number_octree_levels = 4
-    gp.compute_model(geo_model)
-
-    plot_block_and_input_2d(
-        stack_number=0,
-        interpolation_input=geo_model.interpolation_input,
-        outputs=geo_model.solutions.octrees_output,
-        structure=geo_model.structural_frame.input_data_descriptor.stack_structure,
-        value_type=ValueType.ids
-    )
-    
-    gpv.plot_3d(geo_model, show_data=True, show_boundaries=True, show_lith=False, image=True)
-    
-    geo_model.interpolation_options.number_octree_levels = 2
-    gp.compute_model(geo_model)
-
-    plot_block_and_input_2d(
-        stack_number=0,
-        interpolation_input=geo_model.interpolation_input,
-        outputs=geo_model.solutions.octrees_output,
-        structure=geo_model.structural_frame.input_data_descriptor.stack_structure,
-        value_type=ValueType.ids
-    )
-
-    gpv.plot_3d(geo_model, show_data=True, show_boundaries=True, show_lith=False, image=True)
+﻿import pytest
+
+import gempy as gp
+import gempy_viewer as gpv
+from gempy.core.data.enumerators import ExampleModel
+from gempy_engine.modules.octrees_topology.octrees_topology_interface import ValueType
+from gempy_engine.plugins.plotting.helper_functions import plot_block_and_input_2d
+from test.conftest import TEST_SPEED, TestSpeed
+
+
+pytestmark = pytest.mark.skipif(TEST_SPEED.value < TestSpeed.MINUTES.value, reason="Global test speed below this test value.")
+
+
+def  test_octree():
+    geo_model: gp.data.GeoModel = gp.generate_example_model(
+        example_model=ExampleModel.ANTICLINE,
+        compute_model=False
+    ) 
+    
+    geo_model.interpolation_options.number_octree_levels = 4
+    gp.compute_model(geo_model)
+
+    plot_block_and_input_2d(
+        stack_number=0,
+        interpolation_input=geo_model.interpolation_input,
+        outputs=geo_model.solutions.octrees_output,
+        structure=geo_model.structural_frame.input_data_descriptor.stack_structure,
+        value_type=ValueType.ids
+    )
+    
+    gpv.plot_3d(geo_model, show_data=True, show_boundaries=True, show_lith=False, image=True)
+    
+    geo_model.interpolation_options.number_octree_levels = 2
+    gp.compute_model(geo_model)
+
+    plot_block_and_input_2d(
+        stack_number=0,
+        interpolation_input=geo_model.interpolation_input,
+        outputs=geo_model.solutions.octrees_output,
+        structure=geo_model.structural_frame.input_data_descriptor.stack_structure,
+        value_type=ValueType.ids
+    )
+
+    gpv.plot_3d(geo_model, show_data=True, show_boundaries=True, show_lith=False, image=True)
```

