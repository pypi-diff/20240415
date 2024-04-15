# Comparing `tmp/partcad-0.5.6.tar.gz` & `tmp/partcad-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partcad-0.5.6.tar", last modified: Mon Mar  4 10:56:27 2024, max compression
+gzip compressed data, was "partcad-0.5.8.tar", last modified: Wed Mar  6 07:20:03 2024, max compression
```

## Comparing `partcad-0.5.6.tar` & `partcad-0.5.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:27.441801 partcad-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-04 10:56:27.441801 partcad-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-04 10:56:07.000000 partcad-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-04 10:56:07.000000 partcad-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-04 10:56:07.000000 partcad-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 10:56:27.441801 partcad-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:27.429801 partcad-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:27.437801 partcad-0.5.6/src/partcad/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly_factory_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly_factory_assy.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/assembly_factory_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/logging_ansi_terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_3mf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_build123d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_cadquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_scad.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/part_factory_stl.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/plugin_export_png.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/plugin_export_png_reportlab.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    31696 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project_factory_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project_factory_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/project_factory_tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/render.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime_python_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime_python_conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime_python_none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/runtime_python_pypy.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/shape_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/shape_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/sync_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:27.437801 partcad-0.5.6/src/partcad/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrappers/cq_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrappers/wrapper_build123d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrappers/wrapper_cadquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrappers/wrapper_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-04 10:56:07.000000 partcad-0.5.6/src/partcad/wrappers/wrapper_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:27.441801 partcad-0.5.6/src/partcad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-04 10:56:27.000000 partcad-0.5.6/src/partcad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-04 10:56:27.000000 partcad-0.5.6/src/partcad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:56:27.000000 partcad-0.5.6/src/partcad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-04 10:56:27.000000 partcad-0.5.6/src/partcad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-04 10:56:27.000000 partcad-0.5.6/src/partcad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:03.945238 partcad-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-06 07:20:03.945238 partcad-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-06 07:19:40.000000 partcad-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-06 07:19:40.000000 partcad-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-06 07:19:40.000000 partcad-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 07:20:03.945238 partcad-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:03.933238 partcad-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:03.941238 partcad-0.5.8/src/partcad/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly_factory_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly_factory_assy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/assembly_factory_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/logging_ansi_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_3mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_build123d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_cadquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_scad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/part_factory_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/plugin_export_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/plugin_export_png_reportlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31696 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project_factory_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project_factory_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/project_factory_tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime_python_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime_python_conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime_python_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/runtime_python_pypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/shape_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/shape_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/sync_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:03.945238 partcad-0.5.8/src/partcad/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrappers/cq_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrappers/wrapper_build123d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrappers/wrapper_cadquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrappers/wrapper_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-06 07:19:40.000000 partcad-0.5.8/src/partcad/wrappers/wrapper_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:03.945238 partcad-0.5.8/src/partcad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-06 07:20:03.000000 partcad-0.5.8/src/partcad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-06 07:20:03.000000 partcad-0.5.8/src/partcad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 07:20:03.000000 partcad-0.5.8/src/partcad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-06 07:20:03.000000 partcad-0.5.8/src/partcad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-06 07:20:03.000000 partcad-0.5.8/src/partcad.egg-info/top_level.txt
```

### Comparing `partcad-0.5.6/PKG-INFO` & `partcad-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partcad
-Version: 0.5.6
+Version: 0.5.8
 Summary: Package manager for CAD models and a modelling framework
 Author-email: Roman Kuzmenko <openvmp@proton.me>
 Maintainer-email: Roman Kuzmenko <openvmp@proton.me>
 Project-URL: Homepage, https://github.com/openvmp/partcad
 Project-URL: Issues, https://github.com/openvmp/partcad/issues
 Keywords: cadquery,build123d,cad,design,openscad,step,stl
 Classifier: Programming Language :: Python :: 3
```

### Comparing `partcad-0.5.6/README.md` & `partcad-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/pyproject.toml` & `partcad-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "partcad"
-version = "0.5.6"
+version = "0.5.8"
 description = "Package manager for CAD models and a modelling framework"
 readme = "README.md"
 keywords = ["cadquery", "build123d", "cad", "design", "openscad", "step", "stl"]
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 authors = [
   {name = "Roman Kuzmenko", email = "openvmp@proton.me" }
```

### Comparing `partcad-0.5.6/src/partcad/__init__.py` & `partcad-0.5.8/src/partcad/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .project_factory_local import ProjectFactoryLocal
 from .project_factory_git import ProjectFactoryGit
 from .project_factory_tar import ProjectFactoryTar
 from .user_config import user_config
 from .plugins import plugins
 from .plugin_export_png_reportlab import PluginExportPngReportlab
 from .logging_ansi_terminal import init as logging_ansi_terminal_init
+from .logging_ansi_terminal import fini as logging_ansi_terminal_fini
 from . import logging
 from . import utils
 
 __all__ = [
     "config",
     "context",
     "shape",
@@ -44,8 +45,8 @@
     "assembly_factory",
     "assembly_factory_python",
     "scene",
     "main_cli",
     "plugins",
 ]
 
-__version__: str = "0.5.6"
+__version__: str = "0.5.8"
```

### Comparing `partcad-0.5.6/src/partcad/assembly.py` & `partcad-0.5.8/src/partcad/assembly.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/assembly_config.py` & `partcad-0.5.8/src/partcad/assembly_config.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/assembly_factory.py` & `partcad-0.5.8/src/partcad/assembly_factory.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/assembly_factory_alias.py` & `partcad-0.5.8/src/partcad/assembly_factory_alias.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/assembly_factory_assy.py` & `partcad-0.5.8/src/partcad/assembly_factory_assy.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/assembly_factory_file.py` & `partcad-0.5.8/src/partcad/assembly_factory_file.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/context.py` & `partcad-0.5.8/src/partcad/context.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/factory.py` & `partcad-0.5.8/src/partcad/factory.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/globals.py` & `partcad-0.5.8/src/partcad/globals.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 from .context import Context
 from .assembly import Assembly
 from .assembly_factory_assy import AssemblyFactoryAssy
 from .assembly_factory_alias import AssemblyFactoryAlias
 from .part import Part
 from . import consts
 from . import factory
-
-# from . import logging as pc_logging
+from . import logging as pc_logging
 
 global _partcad_context
 _partcad_context = None
 _partcad_context_lock = threading.Lock()
 
 factory.register("assembly", "assy", AssemblyFactoryAssy)
 factory.register("assembly", "alias", AssemblyFactoryAlias)
@@ -96,11 +95,12 @@
     else:
         template_name = "init-public.yaml"
     src_path = os.path.join(
         os.path.dirname(__file__), "template", template_name
     )
 
     if os.path.exists(dst_path):
+        pc_logging.error("File already exists: %s" % dst_path)
         return False
     shutil.copyfile(src_path, dst_path)
 
     return True
```

### Comparing `partcad-0.5.6/src/partcad/logging.py` & `partcad-0.5.8/src/partcad/logging.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/logging_ansi_terminal.py` & `partcad-0.5.8/src/partcad/logging_ansi_terminal.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part.py` & `partcad-0.5.8/src/partcad/part.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_config.py` & `partcad-0.5.8/src/partcad/part_config.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory.py` & `partcad-0.5.8/src/partcad/part_factory.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_3mf.py` & `partcad-0.5.8/src/partcad/part_factory_3mf.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_alias.py` & `partcad-0.5.8/src/partcad/part_factory_alias.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_build123d.py` & `partcad-0.5.8/src/partcad/part_factory_build123d.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_cadquery.py` & `partcad-0.5.8/src/partcad/part_factory_cadquery.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_enrich.py` & `partcad-0.5.8/src/partcad/part_factory_enrich.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_file.py` & `partcad-0.5.8/src/partcad/part_factory_file.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_python.py` & `partcad-0.5.8/src/partcad/part_factory_python.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_scad.py` & `partcad-0.5.8/src/partcad/part_factory_scad.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_step.py` & `partcad-0.5.8/src/partcad/part_factory_step.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/part_factory_stl.py` & `partcad-0.5.8/src/partcad/part_factory_stl.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/plugin_export_png_reportlab.py` & `partcad-0.5.8/src/partcad/plugin_export_png_reportlab.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project.py` & `partcad-0.5.8/src/partcad/project.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project_config.py` & `partcad-0.5.8/src/partcad/project_config.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project_factory.py` & `partcad-0.5.8/src/partcad/project_factory.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project_factory_git.py` & `partcad-0.5.8/src/partcad/project_factory_git.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project_factory_local.py` & `partcad-0.5.8/src/partcad/project_factory_local.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/project_factory_tar.py` & `partcad-0.5.8/src/partcad/project_factory_tar.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/render.py` & `partcad-0.5.8/src/partcad/render.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime.py` & `partcad-0.5.8/src/partcad/runtime.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime_python.py` & `partcad-0.5.8/src/partcad/runtime_python.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime_python_all.py` & `partcad-0.5.8/src/partcad/runtime_python_all.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime_python_conda.py` & `partcad-0.5.8/src/partcad/runtime_python_conda.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime_python_none.py` & `partcad-0.5.8/src/partcad/runtime_python_none.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/runtime_python_pypy.py` & `partcad-0.5.8/src/partcad/runtime_python_pypy.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/shape.py` & `partcad-0.5.8/src/partcad/shape.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/shape_config.py` & `partcad-0.5.8/src/partcad/shape_config.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/sync_threads.py` & `partcad-0.5.8/src/partcad/sync_threads.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/user_config.py` & `partcad-0.5.8/src/partcad/user_config.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/utils.py` & `partcad-0.5.8/src/partcad/utils.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/wrappers/cq_serialize.py` & `partcad-0.5.8/src/partcad/wrappers/cq_serialize.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/wrappers/wrapper_build123d.py` & `partcad-0.5.8/src/partcad/wrappers/wrapper_build123d.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/wrappers/wrapper_cadquery.py` & `partcad-0.5.8/src/partcad/wrappers/wrapper_cadquery.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/wrappers/wrapper_common.py` & `partcad-0.5.8/src/partcad/wrappers/wrapper_common.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad/wrappers/wrapper_step.py` & `partcad-0.5.8/src/partcad/wrappers/wrapper_step.py`

 * *Files identical despite different names*

### Comparing `partcad-0.5.6/src/partcad.egg-info/PKG-INFO` & `partcad-0.5.8/src/partcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partcad
-Version: 0.5.6
+Version: 0.5.8
 Summary: Package manager for CAD models and a modelling framework
 Author-email: Roman Kuzmenko <openvmp@proton.me>
 Maintainer-email: Roman Kuzmenko <openvmp@proton.me>
 Project-URL: Homepage, https://github.com/openvmp/partcad
 Project-URL: Issues, https://github.com/openvmp/partcad/issues
 Keywords: cadquery,build123d,cad,design,openscad,step,stl
 Classifier: Programming Language :: Python :: 3
```

### Comparing `partcad-0.5.6/src/partcad.egg-info/SOURCES.txt` & `partcad-0.5.8/src/partcad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

