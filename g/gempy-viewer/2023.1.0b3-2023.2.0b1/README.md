# Comparing `tmp/gempy_viewer-2023.1.0b3.tar.gz` & `tmp/gempy_viewer-2023.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_viewer-2023.1.0b3.tar", last modified: Thu Sep 14 08:42:38 2023, max compression
+gzip compressed data, was "gempy_viewer-2023.2.0b1.tar", last modified: Wed Nov 22 15:21:36 2023, max compression
```

## Comparing `gempy_viewer-2023.1.0b3.tar` & `gempy_viewer-2023.2.0b1.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2023.1.0b3/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2023.1.0b3/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)      587 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2023.1.0b3/README.md
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      296 2023-09-14 07:59:45.000000 gempy_viewer-2023.1.0b3/gempy_viewer/API/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11053 2023-09-12 09:21:45.000000 gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_2d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7907 2023-09-07 13:51:17.000000 gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_2d_sections_api.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6085 2023-09-12 08:37:14.000000 gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_3d_API.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3774 2023-07-26 11:55:19.000000 gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_others.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/_plot.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/_visualization_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/decorators.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    60969 2023-07-28 08:27:07.000000 gempy_viewer-2023.1.0b3/gempy_viewer/DEP/visualization_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      291 2023-07-26 11:55:19.000000 gempy_viewer-2023.1.0b3/gempy_viewer/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1986 2023-08-15 08:19:47.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/data_to_show.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/plotting_2d_options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/scalar_data_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/section_data_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2023.1.0b3/gempy_viewer/core/slicer_data.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8755 2023-09-14 08:36:36.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_input_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2200 2023-08-02 14:06:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4922 2023-09-11 06:57:42.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      721 2023-08-02 09:04:35.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-07-25 08:34:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/helpers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7286 2023-08-17 15:14:16.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/multi_axis_manager.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4935 2023-09-05 13:03:44.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/plot_2d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4165 2023-09-14 07:57:05.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/visualization_2d.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    42120 2023-07-28 08:27:07.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/_vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4142 2023-09-08 14:04:29.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_input_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5588 2023-09-11 07:14:24.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1263 2023-08-15 09:14:11.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2987 2023-09-12 08:32:03.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/plot_3d_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5422 2023-09-07 08:53:32.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/vista.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6536 2023-06-18 07:52:19.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/vista_aux.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/vista_qt.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      579 2023-07-24 14:50:22.000000 gempy_viewer-2023.1.0b3/gempy_viewer/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      587 2023-09-14 08:42:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2116 2023-09-14 08:42:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-09-14 08:42:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       77 2023-09-14 08:42:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2023-09-14 08:42:38.000000 gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/top_level.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1073 2023-09-14 08:42:28.000000 gempy_viewer-2023.1.0b3/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/tests/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2023.1.0b3/tests/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2323 2023-08-04 09:04:24.000000 gempy_viewer-2023.1.0b3/tests/conftest.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-14 08:42:38.413742 gempy_viewer-2023.1.0b3/tests/test_plotting/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2023.1.0b3/tests/test_plotting/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7864 2023-09-14 08:03:39.000000 gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_2d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2715 2023-08-04 09:08:59.000000 gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_3d.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2851 2023-08-09 12:59:36.000000 gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_3d_legacy.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13407 2023-07-27 09:07:59.000000 gempy_viewer-2023.1.0b3/tests/test_plotting/test_vista.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.121505 gempy_viewer-2023.2.0b1/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      623 2023-06-19 10:23:48.000000 gempy_viewer-2023.2.0b1/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13874 2023-06-19 10:23:48.000000 gempy_viewer-2023.2.0b1/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      856 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1484 2023-07-26 10:50:13.000000 gempy_viewer-2023.2.0b1/README.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      296 2023-11-21 15:15:11.000000 gempy_viewer-2023.2.0b1/gempy_viewer/API/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10875 2023-10-10 11:45:51.000000 gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_2d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7967 2023-11-10 12:12:10.000000 gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_2d_sections_api.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6119 2023-11-21 15:10:45.000000 gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_3d_API.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3638 2023-11-21 16:20:52.000000 gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_others.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:59:27.000000 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    14538 2023-06-22 11:01:14.000000 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/_plot.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    54327 2023-06-22 10:59:32.000000 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/_visualization_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4308 2023-06-22 10:59:32.000000 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/decorators.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    60969 2023-07-28 08:27:07.000000 gempy_viewer-2023.2.0b1/gempy_viewer/DEP/visualization_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      337 2023-11-22 15:00:16.000000 gempy_viewer-2023.2.0b1/gempy_viewer/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:53:54.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1976 2023-09-27 08:52:01.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/data_to_show.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      479 2023-07-10 13:33:23.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/plotting_2d_options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      301 2023-07-26 12:29:31.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/scalar_data_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      496 2023-07-25 14:27:44.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/section_data_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      380 2023-07-25 14:27:44.000000 gempy_viewer-2023.2.0b1/gempy_viewer/core/slicer_data.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:05.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:45.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3921 2023-08-02 09:19:49.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_contours_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8773 2023-11-21 12:50:12.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_input_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2807 2023-11-08 12:18:06.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2983 2023-08-22 13:43:39.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4892 2023-10-11 11:42:21.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_topography_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      721 2023-08-02 09:04:35.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_traces_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      847 2023-11-08 11:53:57.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/helpers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7293 2023-11-08 07:54:32.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/multi_axis_manager.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5076 2023-11-22 08:30:22.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/plot_2d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12753 2023-06-18 07:52:19.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/plot_utils_DEP.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4242 2023-10-09 13:35:04.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/visualization_2d.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-22 10:54:58.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    42120 2023-07-28 08:27:07.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/_vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4222 2023-11-21 15:09:13.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_input_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5704 2023-11-21 16:31:05.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1321 2023-11-21 15:13:49.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3055 2023-11-21 15:14:27.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_topography_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1715 2023-09-08 13:45:29.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/plot_3d_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4569 2023-11-21 15:08:41.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/vista.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2523 2023-06-22 11:38:56.000000 gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/vista_qt.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      932 2023-11-21 16:16:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      856 2023-11-22 15:21:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2074 2023-11-22 15:21:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-11-22 15:21:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       83 2023-11-22 15:21:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2023-11-22 15:21:36.000000 gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/top_level.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-11-22 15:21:36.121505 gempy_viewer-2023.2.0b1/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1296 2023-11-22 15:20:52.000000 gempy_viewer-2023.2.0b1/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/tests/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-19 11:53:13.000000 gempy_viewer-2023.2.0b1/tests/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2313 2023-10-11 08:49:21.000000 gempy_viewer-2023.2.0b1/tests/conftest.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:21:36.111505 gempy_viewer-2023.2.0b1/tests/test_plotting/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:52:19.000000 gempy_viewer-2023.2.0b1/tests/test_plotting/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7864 2023-10-11 12:33:34.000000 gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_2d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2715 2023-08-04 09:08:59.000000 gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_3d.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2851 2023-08-09 12:59:36.000000 gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_3d_legacy.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13407 2023-07-27 09:07:59.000000 gempy_viewer-2023.2.0b1/tests/test_plotting/test_vista.py
```

### Comparing `gempy_viewer-2023.1.0b3/AUTHORS.rst` & `gempy_viewer-2023.2.0b1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/LICENSE` & `gempy_viewer-2023.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/README.md` & `gempy_viewer-2023.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_2d_API.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_2d_API.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ﻿from typing import Union, List, Optional
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from gempy.core.data import GeoModel
+from gempy.core.data.grid_modules import RegularGrid
 from gempy_viewer.API._plot_2d_sections_api import plot_sections
 from gempy_viewer.core.data_to_show import DataToShow
 from gempy_viewer.core.section_data_2d import SectionData2D
 from gempy_viewer.modules.plot_2d.multi_axis_manager import sections_iterator, orthogonal_sections_iterator
 from gempy_viewer.modules.plot_2d.visualization_2d import Plot2D
 
 
@@ -92,15 +93,15 @@
         cell_number = ['mid']
     direction = [] if direction is None else direction
 
     if type(cell_number) != list:
         cell_number = [cell_number]
 
     if type(direction) != list:
-        direction = [direction]
+        direction = [direction] * len(cell_number)
 
     if n_axis is None:
         n_axis = len(section_names) + len(cell_number)
 
     if type(series_n) is int:
         series_n = [series_n] * n_axis
 
@@ -149,14 +150,15 @@
         n_axis=n_axis,
         n_columns=n_columns,
         ve=ve,
         projection_distance=kwargs.get('projection_distance', 0.2 * model.transform.isometric_scale)
     )
 
     section_data_list.extend(orthogonal_section_data_list)
+    p.section_data_list = section_data_list
 
     plot_sections(
         gempy_model=model,
         sections_data=section_data_list,
         data_to_show=data_to_show,
         ve=ve,
         series_n=series_n,
@@ -193,15 +195,15 @@
         section_names=section_names
     )
     
     plot.fig.show()
     return pst
 
 
-def plot_topology(geo_model, edges, centroids, direction="y", scale=True,
+def plot_topology(regular_grid: RegularGrid, edges, centroids, direction="y", ax=None, scale=True,
                   label_kwargs=None, edge_kwargs=None):
     """Plot the topology adjacency graph in 2-D.
 
         Args:
             geo_model ([type]): GemPy geomodel instance.
             edges (Set[Tuple[int, int]]): Set of topology edges.
             centroids (Dict[int, Array[int, 3]]): Dictionary of topology id's and
@@ -210,43 +212,43 @@
                 Defaults to "y".
             label_kwargs (dict, optional): Keyword arguments for topology labels.
                 Defaults to None.
             edge_kwargs (dict, optional): Keyword arguments for topology edges.
                 Defaults to None.
 
         """
-    res = geo_model._grid.regular_grid.resolution
+    if ax is None:
+        fig, ax = plt.subplots(figsize=(10, 10))
+        
+    res = regular_grid.resolution
     if direction == "y":
         c1, c2 = (0, 2)
-        e1 = geo_model._grid.regular_grid.extent[1] - geo_model._grid.regular_grid.extent[0]
-        e2 = geo_model._grid.regular_grid.extent[5] - geo_model._grid.regular_grid.extent[4]
-        d1 = geo_model._grid.regular_grid.extent[0]
-        d2 = geo_model._grid.regular_grid.extent[4]
-        # if len(list(centroids.items())[0][1]) == 2:
-        #     c1, c2 = (0, 1)
+        e1 = regular_grid.extent[1] - regular_grid.extent[0]
+        e2 = regular_grid.extent[5] - regular_grid.extent[4]
+        d1 = regular_grid.extent[0]
+        d2 = regular_grid.extent[4]
+        # ? (miguel, Oct 23) When is this condition used?
+        if len(list(centroids.items())[0][1]) == 2:
+            c1, c2 = (0, 1)
         r1 = res[0]
         r2 = res[2]
     elif direction == "x":
         c1, c2 = (1, 2)
-        e1 = geo_model._grid.regular_grid.extent[3] - geo_model._grid.regular_grid.extent[2]
-        e2 = geo_model._grid.regular_grid.extent[5] - geo_model._grid.regular_grid.extent[4]
-        d1 = geo_model._grid.regular_grid.extent[2]
-        d2 = geo_model._grid.regular_grid.extent[4]
-        # if len(list(centroids.items())[0][1]) == 2:
-        #     c1, c2 = (0, 1)
+        e1 = regular_grid.extent[3] - regular_grid.extent[2]
+        e2 = regular_grid.extent[5] - regular_grid.extent[4]
+        d1 = regular_grid.extent[2]
+        d2 = regular_grid.extent[4]
         r1 = res[1]
         r2 = res[2]
     elif direction == "z":
         c1, c2 = (0, 1)
-        e1 = geo_model._grid.regular_grid.extent[1] - geo_model._grid.regular_grid.extent[0]
-        e2 = geo_model._grid.regular_grid.extent[3] - geo_model._grid.regular_grid.extent[2]
-        d1 = geo_model._grid.regular_grid.extent[0]
-        d2 = geo_model._grid.regular_grid.extent[2]
-        # if len(list(centroids.items())[0][1]) == 2:
-        #     c1, c2 = (0, 1)
+        e1 = regular_grid.extent[1] - regular_grid.extent[0]
+        e2 = regular_grid.extent[3] - regular_grid.extent[2]
+        d1 = regular_grid.extent[0]
+        d2 = regular_grid.extent[2]
         r1 = res[0]
         r2 = res[1]
 
     tkw = {
         "color"              : "white",
         "fontsize"           : 13,
         "ha"                 : "center",
@@ -270,16 +272,18 @@
     for a, b in edges:
         # plot edges
         x = np.array([centroids[a][c1], centroids[b][c1]])
         y = np.array([centroids[a][c2], centroids[b][c2]])
         if scale:
             x = x * e1 / r1 + d1
             y = y * e2 / r2 + d2
-        plt.plot(x, y, **lkw)
+        ax.plot(x, y, **lkw)
 
     for node in np.unique(list(edges)):
         x = centroids[node][c1]
         y = centroids[node][c2]
         if scale:
             x = x * e1 / r1 + d1
             y = y * e2 / r2 + d2
-        plt.text(x, y, str(node), **tkw)
+        ax.text(x, y, str(node), **tkw)
+    
+    plt.show()
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_2d_sections_api.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_2d_sections_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
                 orientations=gempy_model.orientations.df.copy(),
                 points=gempy_model.surface_points.df.copy(),
                 slicer_data=section_data.slicer_data
             )
 
         if data_to_show.show_lith[e] is True:
             _is_filled = True
-            cmap = kwargs_lithology.get('cmap', get_geo_model_cmap(gempy_model.structural_frame.elements_colors))
-            norm = kwargs_lithology.get('norm', get_geo_model_norm(gempy_model.structural_frame.number_of_elements))
+            cmap = kwargs_lithology.pop('cmap', get_geo_model_cmap(gempy_model.structural_frame.elements_colors))
+            norm = kwargs_lithology.pop('norm', get_geo_model_norm(gempy_model.structural_frame.number_of_elements))
             
             match section_data.section_type:
                 case SectionType.SECTION:
                     plot_section_area(
                         gempy_model=gempy_model,
                         ax=temp_ax,
                         section_name=section_data.section_name,
@@ -61,24 +61,25 @@
                 case SectionType.ORTHOGONAL:
                     if override_regular_grid is None:
                         block_to_plot = gempy_model.solutions.raw_arrays.lith_block
                         cmap = cmap
                         norm = norm
                     else:
                         block_to_plot = override_regular_grid
-                        cmap = kwargs_lithology.get('cmap', None)
-                        norm = kwargs_lithology.get('norm', None)
+                        # cmap = kwargs_lithology.pop('cmap', None)
+                        # norm = kwargs_lithology.pop('norm', None)
 
                     plot_regular_grid_area(
                         ax=temp_ax,
                         slicer_data=section_data.slicer_data,
                         block=block_to_plot,  # * Only used for orthogonal sections
                         resolution=gempy_model.grid.regular_grid.resolution,
                         cmap=cmap,
                         norm=norm,
+                        imshow_kwargs=kwargs_lithology
                     )
                 case _:
                     raise ValueError(f'Unknown section type: {section_data.section_type}')
         if data_to_show.show_scalar[e] is True:
             _is_filled = True
             match section_data.section_type:
                 case SectionType.SECTION:
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_3d_API.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_3d_API.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 ﻿import matplotlib.pyplot as plt
 import numpy as np
 
 from gempy.core.data import GeoModel
 from gempy_viewer.core.data_to_show import DataToShow
 from gempy_viewer.core.scalar_data_type import ScalarDataType, TopographyDataType
 from gempy_viewer.modules.plot_2d.plot_2d_utils import get_geo_model_cmap
-from gempy_viewer.modules.plot_3d.drawer_input_3d import plot_data
-from gempy_viewer.modules.plot_3d.drawer_structured_grid_3d import plot_structured_grid
-from gempy_viewer.modules.plot_3d.drawer_surfaces_3d import plot_surfaces
-from gempy_viewer.modules.plot_3d.drawer_topography_3d import plot_topography_3d
-from gempy_viewer.modules.plot_3d.plot_3d_utils import set_scalar_bar
 from gempy_viewer.modules.plot_3d.vista import GemPyToVista
 
 try:
     import pyvista as pv
     from gempy_viewer.modules.plot_3d._vista import Vista as Vista
 
     PYVISTA_IMPORT = True
@@ -40,15 +35,23 @@
         kwargs_plot_data=None,
         kwargs_plotter=None,
         kwargs_plot_surfaces=None,
         image=False,
         show=True,
         **kwargs
 ) -> GemPyToVista:
+    
     """Plot 3-D geomodel."""
+
+    from gempy_viewer.modules.plot_3d.drawer_input_3d import plot_data
+    from gempy_viewer.modules.plot_3d.drawer_structured_grid_3d import plot_structured_grid
+    from gempy_viewer.modules.plot_3d.drawer_surfaces_3d import plot_surfaces
+    from gempy_viewer.modules.plot_3d.drawer_topography_3d import plot_topography_3d
+    from gempy_viewer.modules.plot_3d.plot_3d_utils import set_scalar_bar
+    
     # * Grab from kwargs all the show arguments and create the proper class. This is for backwards compatibility
     can_show_results = model.solutions is not None  # and model.solutions.lith_block.shape[0] != 0
     data_to_show = DataToShow(
         n_axis=1,
         show_data=kwargs.get('show_data', True),
         _show_results=kwargs.get('show_results', can_show_results),
         show_surfaces=kwargs.get('show_surfaces', True),
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/API/_plot_others.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/API/_plot_others.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,17 @@
     the potential field method.
     Tested on Ubuntu 16
 
     Created on 10/11/2019
 
     @author: Alex Schaaf, Elisa Heim, Miguel de la Varga
 """
-# This is for sphenix to find the packages
-# sys.path.append( path.dirname( path.dirname( path.abspath(__file__) ) ) )
-
 import matplotlib.pyplot as plt
-import pandas as pn
+
+from gempy_viewer.optional_dependencies import require_pandas
 
 try:
     import mplstereonet
 
     mplstereonet_import = True
 except ImportError:
     mplstereonet_import = False
@@ -47,19 +45,18 @@
     from collections import OrderedDict
 
     if litho is None:
         litho = self.model._orientations.df['surface'].unique()
 
     if single_plots is False:
         fig, ax = mplstereonet.subplots(figsize=(5, 5))
+        pn = require_pandas()
         df_sub2 = pn.DataFrame()
         for i in litho:
-            df_sub2 = df_sub2.append(self.model._orientations.df[
-                                         self.model._orientations.df[
-                                             'surface'] == i])
+            df_sub2 = df_sub2.append(self.model._orientations.df[ self.model._orientations.df[ 'surface'] == i])
 
     for formation in litho:
         if single_plots:
             fig = plt.figure(figsize=(5, 5))
             ax = fig.add_subplot(111, projection='stereonet')
             ax.set_title(formation, y=1.1)
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/DEP/_plot.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/DEP/_plot.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/DEP/_visualization_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/DEP/_visualization_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/DEP/decorators.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/DEP/decorators.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/DEP/visualization_3d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/DEP/visualization_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/core/data_to_show.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/core/data_to_show.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     show_topography: Union[bool, list] = False
     show_section_traces: Union[bool, list] = True
     show_values: Union[bool, list] = False
     show_block: Union[bool, list] = False
     
     def __post_init__(self):
         if self.show_results is False:
-            self.show_lith = [False]
-            self.show_values = [False]
-            self.show_block = [False]
-            self.show_scalar = [False]
-            self.show_boundaries = [False]
+            self.show_lith = False
+            self.show_values = False
+            self.show_block = False
+            self.show_scalar = False
+            self.show_boundaries = False
 
 
         if type(self.show_data) is bool:
             self.show_data = [self.show_data] * self.n_axis
         if type(self.show_lith) is bool:
             self.show_lith = [self.show_lith] * self.n_axis
         if type(self.show_values) is bool:
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_contours_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_contours_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_input_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_input_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ﻿import copy
 import warnings
 
 import numpy as np
-import pandas as pd
 from matplotlib import pyplot as plt
 
 from gempy_viewer.core.slicer_data import SlicerData
 from gempy.core.data.grid_modules import RegularGrid, Sections
 from gempy.core.data.grid_modules import Topography
 from .plot_2d_utils import slice_cross_section
 from .visualization_2d import Plot2D
@@ -74,15 +73,15 @@
     except AttributeError:
         pass
     # endregion
 
 
 # TODO: This could be public and the slice just a class yes!
 def draw_data(ax, surface_points_colors: list[str], orientations_colors: list[str],
-              orientations: pd.DataFrame, points: pd.DataFrame, slicer_data: SlicerData):
+              orientations: 'pd.DataFrame', points: 'pd.DataFrame', slicer_data: SlicerData):
     
     _draw_surface_points(ax, points, slicer_data, surface_points_colors)
     _draw_orientations(ax, orientations, orientations_colors, slicer_data)
 
 
 def _draw_orientations(ax, orientations, orientations_colors, slicer_data):
     sel_ori = orientations[slicer_data.select_projected_o]
@@ -208,22 +207,23 @@
         select_projected_o=select_projected_o
     )
 
     return slicer_data
 
 
 def _projection_params_topography(topography: Topography, orientations, points, projection_distance, topography_compression: int = 5000):
-    import scipy.spatial.distance as dd
-    
+    from gempy_viewer.optional_dependencies import require_scipy
+    scipy = require_scipy()
+    dd = scipy.spatial.distance
     decimation_aux = int(topography.values.shape[0] / topography_compression)
     tpp = topography.values[::decimation_aux + 1, :]
-    cdist_sp = scipy.spatial.distance.dd.cdist(
+    cdist_sp = dd.cdist(
         XA=tpp,
         XB=points[['X', 'Y', 'Z']])
     cartesian_point_dist = (cdist_sp < projection_distance).sum(axis=0).astype(bool)
-    cdist_ori = scipy.spatial.distance.dd.cdist(
+    cdist_ori = dd.cdist(
         XA=tpp,
         XB=orientations[['X', 'Y', 'Z']]
     )
     cartesian_ori_dist = (cdist_ori < projection_distance).sum(axis=0).astype(bool)
     x, y, Gx, Gy = 'X', 'Y', 'G_x', 'G_y'
     return Gx, Gy, cartesian_ori_dist, cartesian_point_dist, x, y
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_regular_grid_2d.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,47 @@
 from gempy.core.data import GeoModel, Grid
 from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
 from gempy_viewer.core.slicer_data import SlicerData
 
 
 # TODO: This name seems bad. This is plotting area basically?
 def plot_regular_grid_area(ax, slicer_data: SlicerData, block: np.ndarray, resolution: iter,
-                      cmap: mcolors.Colormap, norm: mcolors.Normalize):
+                      cmap: mcolors.Colormap, norm: mcolors.Normalize, imshow_kwargs: dict = None):
+    if imshow_kwargs is None:
+        imshow_kwargs = dict()
+
+    plot_grid = imshow_kwargs.pop('plot_grid', False)
     
     plot_block = block.reshape(resolution)
     image = plot_block[
         slicer_data.regular_grid_x_idx,
         slicer_data.regular_grid_y_idx,
         slicer_data.regular_grid_z_idx].T
 
-    ax.imshow(
+    
+    im = ax.imshow(
         image,
         origin='lower',
         zorder=-100,
         cmap=cmap,
         norm=norm,
-        extent=[*ax.get_xlim(), *ax.get_ylim()]
+        extent=[*ax.get_xlim(), *ax.get_ylim()],
+        **imshow_kwargs
     )
+
+    if plot_grid:
+        ticks_x = np.linspace(ax.get_xlim()[0], ax.get_xlim()[1], image.shape[1] + 1)
+        ticks_y = np.linspace(ax.get_ylim()[0], ax.get_ylim()[1], image.shape[0] + 1)
+        ax.set_xticks(ticks_x, minor=True)
+        ax.set_yticks(ticks_y, minor=True)
+        ax.grid(which="minor",linestyle='-', linewidth='3', color='grey', alpha=0.7)
+    
+    ax.figure.colorbar(im, ax=ax, shrink=0.5)
     
-    return ax
+    return im
 
 
 def plot_section_area(gempy_model: GeoModel, ax, section_name: str, cmap: mcolors.Colormap, norm: mcolors.Normalize):
     image = _prepare_section_image(gempy_model, section_name)
     ax.imshow(
         image,
         origin='lower',
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_scalar_field_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_topography_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_topography_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,18 @@
         fill_contour=False,
         contour=True,
         section_name=None,
         cell_number=None,
         direction='y',
         block=None,
         **kwargs):
-    
     # Check topography in model 
     if gempy_model.grid.topography is None:
         raise ValueError('Cannot plot topography, no topography in model')
-    
+
     hillshade = kwargs.get('hillshade', True)
     azdeg = kwargs.get('azdeg', 0)
     altdeg = kwargs.get('altdeg', 0)
     cmap = kwargs.get('cmap', 'terrain')
 
     section_name, cell_number, direction = check_default_section(ax, section_name, cell_number, direction)
 
@@ -50,33 +49,33 @@
     topo_super_res = skimage.transform.resize(
         topo.values_2d,
         (1600, 1600),
         order=3,
         mode='edge',
         anti_aliasing=True, preserve_range=False)
     values = topo_super_res[:, :, 2].T
-    
+
     if height_contours is True:
         CS = ax.contour(
             values,
             extent=(topo.extent[:4]),
             colors='k',
             linestyles='solid',
             origin='lower'
         )
         ax.clabel(CS, inline=1, fontsize=10, fmt='%d')
-        
+
     if fill_contour is True:
         CS2 = ax.contourf(
             values,
             extent=topo.extent[:4],
             cmap=cmap
         )
         add_colorbar(axes=ax, label='elevation [m]', cs=CS2)
-        
+
     if hillshade is True:
         from matplotlib.colors import LightSource
 
         ls = LightSource(
             azdeg=azdeg,
             altdeg=altdeg
         )
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/drawer_traces_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/drawer_traces_2d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/helpers.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/helpers.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/multi_axis_manager.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/multi_axis_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,16 @@
 
     # ax.set_aspect('equal')
 
     # Adding some properties to the axes to make easier to plot
     ax.cell_number = cell_number
     ax.direction = direction
     ax.tick_params(axis='x', labelrotation=30)
+
+   
     plot_2d.axes = np.append(plot_2d.axes, ax)
     plot_2d.fig.tight_layout()
 
     return ax
 
 
 def _setup_orthogonal_section(ax, cell_number, direction, gempy_grid):
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/plot_2d_utils.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/plot_2d_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ﻿from typing import Sequence
 
 import numpy as np
 import matplotlib.colors as mcolors
 
 from gempy.core.data import Grid
+from gempy.core.data.core_utils import calculate_line_coordinates_2points, interpolate_zvals_at_xy
 from gempy.core.data.grid_modules import grid_types
 from gempy.core.data.grid_modules import Sections, RegularGrid
 
 
 def slice_cross_section(regular_grid: grid_types.RegularGrid, direction: str, cell_number: int or str):
     """
     Slice the 3D array (blocks or scalar field) in the specific direction selected in the plot functions
@@ -96,16 +97,16 @@
         :param resx: resolution of the defined section
         :param method: interpolation method, 'interp2d' for cubic scipy.interpolate.interp2d
                                          'spline' for scipy.interpolate.RectBivariateSpline
 
     Returns:
         :return: returns x,y,z values of the topography along the section
     """
-    xy = grid.sections.calculate_line_coordinates_2points(p1, p2, resx)
-    z = grid.sections.interpolate_zvals_at_xy(xy, grid.topography, method)
+    xy = calculate_line_coordinates_2points(p1, p2, resx)
+    z = interpolate_zvals_at_xy(xy, grid.topography, method)
     return xy[:, 0], xy[:, 1], z
 
 
 def calculate_p1p2(regular_grid: RegularGrid, direction, cell_number):
     if direction == 'y':
         cell_number = int(regular_grid.resolution[1] / 2) if cell_number == 'mid' else cell_number
 
@@ -129,8 +130,9 @@
     if reverse:
         return mcolors.ListedColormap(elements_colors).reversed()
     else:
         return mcolors.ListedColormap(elements_colors)
 
 
 def get_geo_model_norm(number_elements: int) -> mcolors.Normalize:
-    return mcolors.Normalize(vmin=0.5, vmax=number_elements + 0.5)
+    # return mcolors.Normalize(vmin=0.5, vmax=number_elements + 0.5)
+    return mcolors.Normalize(vmin=0, vmax=number_elements + 0.01)
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/plot_utils_DEP.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/plot_utils_DEP.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_2d/visualization_2d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_2d/visualization_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 Module with classes and methods to visualized structural geology data and potential fields of the regional modelling based on
 the potential field method.
 
 @author: Miguel de la Varga
 """
 
 import warnings
+from typing import Optional
 
 import matplotlib
 import matplotlib.pyplot as plt
 
 plt.style.use(['seaborn-v0_8-white', 'seaborn-v0_8-talk'])
 
 warnings.filterwarnings("ignore", message="No contour levels were found")
 
 
 # ! Missing a function? Check gempy_legacy
 class Plot2D:
     # _color_lot: dict
     axes: list[plt.Axes]
+    section_data_list: Optional[list] = list()
 
     def __init__(self):
         # TODO: Moving this to plotting options
         self.axes = list()
 
     @staticmethod
     def remove(ax):
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/_vista.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/_vista.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_input_3d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_input_3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿import numpy as np
-import pyvista as pv
 
 from gempy.core.data import GeoModel
 from gempy.core.data.orientations import OrientationsTable
 from gempy.core.data.surface_points import SurfacePointsTable
 from gempy_viewer.modules.plot_2d.plot_2d_utils import get_geo_model_cmap
 from gempy_viewer.modules.plot_3d.vista import GemPyToVista
+from gempy_viewer.optional_dependencies import require_pyvista
 
 
 def plot_data(gempy_vista: GemPyToVista, 
               model: GeoModel,
               arrows_factor: float,
               **kwargs):
     plot_surface_points(
@@ -44,15 +44,16 @@
     mapping_dict = {value: i for i, value in enumerate(unique_values_order)}  # Use a dictionary to map the original numbers to new values
     mapped_array = np.vectorize(mapping_dict.get)(ids)  # Map the original array to the new values
 
     # Selecting the surfaces to plot
     xyz = surface_points.xyz
     if transfromed_data := False:  # TODO: Expose this to user
         xyz = surface_points.model_transform.apply(xyz)
-        
+
+    pv = require_pyvista()
     poly = pv.PolyData(xyz)
     poly['id'] = mapped_array
 
     cmap = get_geo_model_cmap(
         elements_colors=np.array(elements_colors),
         reverse=False)
 
@@ -79,15 +80,16 @@
     
     if orientations_xyz.shape[0] == 0:
         return
     if transfromed_data := False:
         orientations_xyz = orientations.model_transform.apply(orientations_xyz)
         orientations_grads = orientations.model_transform.transform_gradient(orientations_grads)
         arrows_factor /=  orientations.model_transform.isometric_scale
-        
+
+    pv = require_pyvista()
     poly = pv.PolyData(orientations_xyz)
     
     ids = orientations.ids
     if ids.shape[0] == 0:
         return
     unique_values, first_indices = np.unique(ids, return_index=True)  # Find the unique elements and their first indices
     unique_values_order = unique_values[np.argsort(first_indices)]  # Sort the unique values by their first appearance in `a`
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 ﻿from typing import Union, Optional
 
 import numpy as np
-import pyvista as pv
 from matplotlib import colors as mcolors
-from pyvista import PolyData
 
 from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
 from gempy_viewer.core.scalar_data_type import ScalarDataType
 from gempy.core.data.grid_modules import RegularGrid, Topography
 from gempy_viewer.modules.plot_3d.vista import GemPyToVista
+from gempy_viewer.optional_dependencies import require_pyvista
 
 
 def plot_structured_grid(
         gempy_vista: GemPyToVista,
         regular_grid: RegularGrid,
         scalar_data_type: ScalarDataType,
         solution: RawArraysSolution,
         cmap: Union[mcolors.Colormap or str],
         active_scalar_field: Optional[str] = None,
-        opacity=.25,
+        opacity=.5,
         **kwargs
 ):
+    pv = require_pyvista()
     structured_grid: pv.StructuredGrid | pv.PolyData = create_regular_mesh(gempy_vista, regular_grid)
 
     # Set the scalar field-Activate it-getting cmap?
     structured_grid = set_scalar_data(
         structured_grid=structured_grid,
         data=solution,
         resolution = regular_grid.resolution,
         scalar_data_type=scalar_data_type
     )
 
     structured_grid = set_active_scalar_fields(
         structured_grid=structured_grid,
         active_scalar_field=active_scalar_field
     )
-    topography_polydata: PolyData = gempy_vista.surface_poly.get('topography', None)
+    topography_polydata: pv.PolyData = gempy_vista.surface_poly.get('topography', None)
     if topography_polydata is not None:
         structured_grid = structured_grid.clip_surface(
             surface=topography_polydata,
             value=-10,
             crinkle=False,
             invert=True
         )
@@ -51,15 +51,15 @@
         opacity=opacity,  # BUG pass this as an argument
         **kwargs
     )
 
 
 def add_regular_grid_mesh(
         gempy_vista: GemPyToVista,
-        structured_grid: pv.StructuredGrid,
+        structured_grid: 'pv.StructuredGrid',
         cmap: Union[mcolors.Colormap or str],
         opacity: float,
         **kwargs
 ):
     gempy_vista.regular_grid_actor = gempy_vista.p.add_mesh(
         mesh=structured_grid,
         cmap=cmap,
@@ -69,50 +69,52 @@
         interpolate_before_map=True,
         opacity=opacity,
         clim=(0, cmap.N - 1),
         **kwargs
     )
 
 
-def create_regular_mesh(gempy_vista: GemPyToVista, regular_grid: RegularGrid) -> pv.StructuredGrid:
+def create_regular_mesh(gempy_vista: GemPyToVista, regular_grid: RegularGrid) -> "pv.StructuredGrid":
     gempy_vista._grid_values = regular_grid.values
 
     if False:
         grid_3d = regular_grid.values.reshape(*regular_grid.resolution, 3).T
         regular_grid_mesh = pv.StructuredGrid(*grid_3d)
     else:
         x = np.linspace(regular_grid.extent[0], regular_grid.extent[1], regular_grid.resolution[0] + 1)
         y = np.linspace(regular_grid.extent[2], regular_grid.extent[3], regular_grid.resolution[1] + 1)
         z = np.linspace(regular_grid.extent[4], regular_grid.extent[5], regular_grid.resolution[2] + 1)
 
         x, y, z = np.meshgrid(x, y, z, indexing='ij')
+        pv = require_pyvista()
         regular_grid_mesh = pv.StructuredGrid( x , y, z ) 
     return regular_grid_mesh
 
 
-def _mask_topography(structured_grid: pv.StructuredGrid, topography: Topography) -> pv.StructuredGrid:
+def _mask_topography(structured_grid: "pv.StructuredGrid", topography: Topography) -> "pv.StructuredGrid":
     # ? Obsolete? I am using pyvista clipping and seems to do the job very good.
     threshold = -100
     structured_grid.active_scalars[topography.topography_mask.ravel(order='C')] = threshold - 1
 
     # ? Is this messing up the data type?
+    pv = require_pyvista()
     structured_grid: pv.StructuredGrid = structured_grid.threshold(
         value=threshold,
         method="upper"
     )
 
     return structured_grid
 
 
 def set_scalar_data(
         data: RawArraysSolution,
-        structured_grid: pv.StructuredGrid,
+        structured_grid: "pv.StructuredGrid",
         resolution: np.ndarray,
         scalar_data_type: ScalarDataType,
-) -> pv.StructuredGrid:
+) -> "pv.StructuredGrid":
     
     def _convert_sol_array_to_fortran_order(array: np.ndarray) -> np.ndarray:
         return array.reshape(*resolution, order='C').ravel(order='F')
     # Substitute the madness of the previous if with match
     match scalar_data_type:
         case ScalarDataType.LITHOLOGY | ScalarDataType.ALL:
             structured_grid.cell_data['id'] = _convert_sol_array_to_fortran_order(data.lith_block - 1)
@@ -127,15 +129,15 @@
                 structured_grid[scalar_field_ + str(e)] = _convert_sol_array_to_fortran_order(data.values_matrix[e])
         case _:
             raise ValueError(f'Unknown scalar data type: {scalar_data_type}')
 
     return structured_grid  # , cmap
 
 
-def set_active_scalar_fields(structured_grid: pv.StructuredGrid, active_scalar_field: Optional[str]) -> pv.StructuredGrid:
+def set_active_scalar_fields(structured_grid: "pv.StructuredGrid", active_scalar_field: Optional[str]) -> "pv.StructuredGrid":
     if active_scalar_field is None:
         active_scalar_field = structured_grid.array_names[0]
 
     if active_scalar_field == 'lith':
         active_scalar_field = 'id'
 
     # Set the scalar field active
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-﻿import pyvista as pv
-import numpy as np
+﻿import numpy as np
 
 from gempy.core.data.structural_element import StructuralElement
 from gempy_viewer.modules.plot_3d.vista import GemPyToVista
-
+from ...optional_dependencies import require_pyvista
 
 
 def plot_surfaces(
         gempy_vista: GemPyToVista,
         structural_elements_with_solution: list[StructuralElement],
         **kwargs
 ):
+    pv = require_pyvista()
     # ! If the order of the meshes does not match the order of scalar_field_at_surface points we need to reorder them in 'multi_scalar_dual_contouring.py'
     
     topography_mesh = gempy_vista.surface_poly.get('topography', None)
     
     for element in structural_elements_with_solution:
         vertices_ = element.vertices
         edges_ = element.edges
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/drawer_topography_3d.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/drawer_topography_3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 ﻿from typing import Optional
 
 import numpy as np
-import pyvista as pv
-from vtkmodules.util.numpy_support import numpy_to_vtk
 import matplotlib.colors as mcolors
 
 from gempy.core.data.grid_modules import Topography
 from gempy_viewer.core.scalar_data_type import TopographyDataType
 from gempy_engine.core.data.raw_arrays_solution import RawArraysSolution
 from gempy_viewer.modules.plot_3d.vista import GemPyToVista
+from ...optional_dependencies import require_pyvista
 
 
 def plot_topography_3d(
         gempy_vista: GemPyToVista,
         topography: Topography,
         solution: Optional[RawArraysSolution],
         topography_scalar_type: TopographyDataType,
         elements_colors: list[str],
         contours=True,
         **kwargs
 ):
+    pv = require_pyvista()
+    from vtkmodules.util.numpy_support import numpy_to_vtk
+    
     rgb = False
 
     xx, yy = np.meshgrid(topography.y, topography.x)
 
     grid = pv.StructuredGrid(yy, xx, topography.values_2d[:, :, 2])
     polydata = grid.extract_surface()
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/plot_3d_utils.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/plot_3d_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/vista.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/vista.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,40 +25,33 @@
 """
 from __future__ import annotations
 
 import warnings
 from typing import Union, List, Optional
 
 import numpy as np
-import pyvista as pv
 
-# TODO Check if this is necessary if it is implemented in the API
-try:
-    import pyvistaqt as pvqt
-
-    PYVISTA_IMPORT = True
-except ImportError:
-    PYVISTA_IMPORT = False
-
-from gempy_viewer.modules.plot_3d.vista_aux import WidgetsCallbacks, RenderChanges
 import matplotlib
 
 warnings.filterwarnings("ignore",
                         message='.*Conversion of the second argument of issubdtype *.',
                         append=True)
 try:
     import vtk
     from vtk.util.numpy_support import numpy_to_vtk
 
     VTK_IMPORT = True
 except ImportError:
     VTK_IMPORT = False
 
+from gempy_viewer.optional_dependencies import require_pyvista
+
 
-class GemPyToVista(WidgetsCallbacks, RenderChanges):
+
+class GemPyToVista:
 
     def __init__(self, extent: Union[np.ndarray | list[float]], plotter_type: str = 'basic',
                  live_updating=False, pyvista_bounds_kwargs: Optional[dict] = None, **kwargs):
         """GemPy 3-D visualization using pyVista.
 
         Args:
             model (gp.Model): Geomodel instance with solutions.
@@ -68,43 +61,35 @@
                 a look-up table. Defaults to None.
             live_updating (bool, optional): Toggles real-time updating of the
                 plot. Defaults to False.
             **kwargs:
 
         """
 
+        pv = require_pyvista()
+        
         if pyvista_bounds_kwargs is None:
             pyvista_bounds_kwargs = {}
-            
+
         # Override default notebook value
         pv.set_plot_theme("document")
         kwargs['notebook'] = kwargs.get('notebook', False)
 
-        # Model properties
-        # self.model = model
-        # self.extent = model._grid.regular_grid.extent if extent is None else extent
-
         # plotting options
         self.live_updating = live_updating
 
         # Choosing plotter
         if plotter_type == 'basic':
             self.p = pv.Plotter(**kwargs)
             self.p.view_isometric(negative=False)
         elif plotter_type == 'notebook':
             raise NotImplementedError
             # self.p = pv.PlotterITK()
         elif plotter_type == 'background':
-            # TODO: Move this to the module to require optional dependencies
-            try:
-                self.p = pv.BackgroundPlotter(**kwargs)
-            except pv.QtDeprecationError:
-                from pyvistaqt import BackgroundPlotter
-                self.p = BackgroundPlotter(**kwargs)
-            self.p.view_isometric(negative=False)
+            raise NotImplementedError
         else:
             raise AttributeError('Plotter type must be basic, background or notebook.')
 
         self.plotter_type = plotter_type
 
         # Default camera and bounds
         self.set_bounds(extent, **pyvista_bounds_kwargs)
@@ -131,23 +116,17 @@
         nv = numpy_to_vtk(col, array_type=3)
         self._cmaps = {'viridis': nv}
 
         # Topology properties
         self.topo_edges = None
         self.topo_ctrs = None
 
-
     def set_bounds(self, extent: List[float], **kwargs):
-
-        # kwargs.setdefault('location', 'furthest')
-        # kwargs.setdefault('grid', False)
-        # kwargs.setdefault('use_2d', False)
-
         self.p.show_bounds(bounds=extent, **kwargs)
-    
+
     @property
     def scalar_bar_arguments(self):
         sargs = dict(
             title_font_size=20,
             label_font_size=16,
             shadow=True,
             italic=True,
@@ -155,11 +134,7 @@
             height=0.25,
             vertical=True,
             position_x=0.15,
             title="id",
             fmt="%.0f",
         )
         return sargs
-
-
-
-
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/modules/plot_3d/vista_qt.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/modules/plot_3d/vista_qt.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer/optional_dependencies.py` & `gempy_viewer-2023.2.0b1/gempy_viewer/optional_dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,28 @@
 def require_pyvista():
     try:
         import pyvista as pv
     except ImportError:
         raise ImportError("The pyvista package is required to run this function.")
     return pv
 
+def require_scipy():
+    try:
+        import scipy
+    except ImportError:
+        raise ImportError("The scipy package is required to run this function.")
+    return scipy
 
 def require_skimage():
     try:
         import skimage
     except ImportError:
         raise ImportError("The skimage package is required to run this function.")
     return skimage
-    
+    
+
+def require_pandas():
+    try:
+        import pandas as pd
+    except ImportError:
+        raise ImportError("The pandas package is required to run this function.")
+    return pd
```

### Comparing `gempy_viewer-2023.1.0b3/gempy_viewer.egg-info/SOURCES.txt` & `gempy_viewer-2023.2.0b1/gempy_viewer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 gempy_viewer/modules/plot_3d/_vista.py
 gempy_viewer/modules/plot_3d/drawer_input_3d.py
 gempy_viewer/modules/plot_3d/drawer_structured_grid_3d.py
 gempy_viewer/modules/plot_3d/drawer_surfaces_3d.py
 gempy_viewer/modules/plot_3d/drawer_topography_3d.py
 gempy_viewer/modules/plot_3d/plot_3d_utils.py
 gempy_viewer/modules/plot_3d/vista.py
-gempy_viewer/modules/plot_3d/vista_aux.py
 gempy_viewer/modules/plot_3d/vista_qt.py
 tests/__init__.py
 tests/conftest.py
 tests/test_plotting/__init__.py
 tests/test_plotting/test_plot_2d.py
 tests/test_plotting/test_plot_3d.py
 tests/test_plotting/test_plot_3d_legacy.py
```

### Comparing `gempy_viewer-2023.1.0b3/setup.py` & `gempy_viewer-2023.2.0b1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 ﻿# setup.py for gempy_viewer. Requierements are numpy and matplotlib
 
 from setuptools import setup, find_packages
+import gempy 
 
-version = "2023.1.0b3"
-
+version = gempy.__version__
+# 
+# with open("gempy_viewer/__init__.py", "r") as f:
+#     for line in f:
+#         if line.startswith("__version__"):
+#             version = line.split("=")[1].strip().strip("'")
+#             break
+# 
 
 def read_requirements(file_name):
     with open(file_name, "r", encoding="utf-8") as f:
         return [line.strip() for line in f.readlines()]
 
 
 setup(
```

### Comparing `gempy_viewer-2023.1.0b3/tests/conftest.py` & `gempy_viewer-2023.2.0b1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def _one_fault_model_generator():
     data_path = 'https://raw.githubusercontent.com/cgre-aachen/gempy_data/master/'
     path_to_data = data_path + "/data/input_data/jan_models/"
     geo_data = gp.create_geomodel(
         project_name='fault',
         extent=[0, 2000, 0, 2000, 0, 1000],
         resolution=[20, 5, 20],
-        number_octree_levels=4,
+        refinement=4,
         importer_helper=ImporterHelper(
             path_to_surface_points=path_to_data + "model5_surface_points.csv",
             path_to_orientations=path_to_data + "model5_orientations.csv",
             hash_surface_points="8fe9250462c3e65080818a84d29925378664f6be46301dcdb42ed4047aa3fe6f",
             hash_orientations="58d1d28be0c52dfdcedf36c9adc3b231e67d6923554159d6484dba589b0bfc5e",
         )
     )
```

### Comparing `gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_2d.py` & `gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             section_dict={'section_SW-NE': ([250, 250], [1750, 1750], [100, 100]),
                           'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])}
         )
 
         gp.set_topography_from_random(
             grid=one_fault_model_no_interp.grid,
             fractal_dimension=1.2,
-            d_z=np.array([600, 2000]),
+            d_z=np.array([600, 1000]),
             topography_resolution=np.array([60, 60])
         )
 
         gpv.plot_2d(
             model=one_fault_model_no_interp,
             section_names=['section_SW-NE', 'section_NW-SE', 'topography'],
             show_topography=True,
@@ -84,15 +84,15 @@
             section_dict={'section_SW-NE': ([250, 250], [1750, 1750], [100, 100]),
                           'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])}
         )
 
         gp.set_topography_from_random(
             grid=one_fault_model_no_interp.grid,
             fractal_dimension=1.2,
-            d_z=np.array([600, 2000]),
+            d_z=np.array([600, 1000]),
             topography_resolution=np.array([60, 60])
         )
 
         gpv.plot_2d(
             model=one_fault_model_no_interp,
             section_names=['section_SW-NE', 'section_NW-SE', 'topography'],
             direction=['x'], cell_number=['mid'],
@@ -161,15 +161,15 @@
             section_dict={'section_SW-NE': ([250, 250], [1750, 1750], [100, 100]),
                           'section_NW-SE': ([250, 1750], [1750, 250], [100, 100])}
         )
 
         gp.set_topography_from_random(
             grid=one_fault_model.grid,
             fractal_dimension=1.2,
-            d_z=np.array([600, 2000]),
+            d_z=np.array([600, 1000]),
             topography_resolution=np.array([60, 60])
         )
 
         gp.compute_model(one_fault_model)
         return one_fault_model
 
     def test_plot_2d_solutions_default(self, one_fault_model_topo_solution_octrees):
```

### Comparing `gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_3d.py` & `gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_3d.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/tests/test_plotting/test_plot_3d_legacy.py` & `gempy_viewer-2023.2.0b1/tests/test_plotting/test_plot_3d_legacy.py`

 * *Files identical despite different names*

### Comparing `gempy_viewer-2023.1.0b3/tests/test_plotting/test_vista.py` & `gempy_viewer-2023.2.0b1/tests/test_plotting/test_vista.py`

 * *Files identical despite different names*

