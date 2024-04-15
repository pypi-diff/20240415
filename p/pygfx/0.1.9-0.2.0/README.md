# Comparing `tmp/pygfx-0.1.9.tar.gz` & `tmp/pygfx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygfx-0.1.9.tar", last modified: Wed Apr 20 11:08:16 2022, max compression
+gzip compressed data, was "pygfx-0.2.0.tar", last modified: Mon Apr 15 14:50:12 2024, max compression
```

## Comparing `pygfx-0.1.9.tar` & `pygfx-0.2.0.tar`

### file list

```diff
@@ -1,101 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-04-20 11:08:07.000000 pygfx-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-04-20 11:08:16.576012 pygfx-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-04-20 11:08:07.000000 pygfx-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/cameras/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_orthographic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_perspective.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_orbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_panzoom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/geometries/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_box.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    10205 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_polyhedron.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_toroidal.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_box.py
--rw-r--r--   0 runner    (1001) docker     (121)    30183 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_gizmo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/linalg/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/cylindrical.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/euler.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/matrix3.py
--rw-r--r--   0 runner    (1001) docker     (121)    25021 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/matrix4.py
--rw-r--r--   0 runner    (1001) docker     (121)     9488 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/spherical.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/vector3.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/vector4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/materials/
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_background.py
--rw-r--r--   0 runner    (1001) docker     (121)     5461 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/objects/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15719 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14690 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_instanced.py
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_more.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/renderers/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/renderers/svg/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/_svgrenderer.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/linerender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/renderers/wgpu/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27254 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_blender.py
--rw-r--r--   0 runner    (1001) docker     (121)     9330 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_flusher.py
--rw-r--r--   0 runner    (1001) docker     (121)    21920 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_pipelinebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)    32563 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    26709 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_shadercomposer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/backgroundrender.py
--rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/imagerender.py
--rw-r--r--   0 runner    (1001) docker     (121)    28530 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/linerender.py
--rw-r--r--   0 runner    (1001) docker     (121)    30402 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/meshrender.py
--rw-r--r--   0 runner    (1001) docker     (121)    10356 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/pointsrender.py
--rw-r--r--   0 runner    (1001) docker     (121)    24215 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/volumerender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7355 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12125 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/_texture.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51540 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/_cmdata_mpl.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/cm.py
--rw-r--r--   0 runner    (1001) docker     (121)    12712 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/show.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/viewport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-04-20 11:08:16.576012 pygfx-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-04-20 11:08:07.000000 pygfx-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.555932 pygfx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-15 14:50:02.000000 pygfx-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-15 14:50:12.555932 pygfx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-15 14:50:02.000000 pygfx-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.523932 pygfx-0.2.0/pygfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.523932 pygfx-0.2.0/pygfx/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/__pyinstaller/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/__pyinstaller/hook-pygfx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/__pyinstaller/test_pygfx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.523932 pygfx-0.2.0/pygfx/cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/cameras/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/cameras/_orthographic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/cameras/_perspective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.527932 pygfx-0.2.0/pygfx/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26444 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/_fly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/_panzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/controllers/_trackball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.527932 pygfx-0.2.0/pygfx/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    25832 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   556216 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/NotoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   177004 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/NotoSansArabic-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   190960 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/NotoSansDevanagari-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   202972 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/NotoSansSymbols-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1609390 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/data_files/noto_default_index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.531932 pygfx-0.2.0/pygfx/geometries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_polyhedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35154 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/_toroidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/geometries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.535932 pygfx-0.2.0/pygfx/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_gizmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/helpers/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.535932 pygfx-0.2.0/pygfx/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30160 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/materials/_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.539932 pygfx-0.2.0/pygfx/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/_instanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21693 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/_lights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/objects/_more.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.539932 pygfx-0.2.0/pygfx/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.539932 pygfx-0.2.0/pygfx/renderers/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/svg/_svgrenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/svg/linerender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.539932 pygfx-0.2.0/pygfx/renderers/wgpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.539932 pygfx-0.2.0/pygfx/renderers/wgpu/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31807 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11495 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/mipmapsutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33525 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/shadowutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.543932 pygfx-0.2.0/pygfx/renderers/wgpu/shader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36527 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shader/_shaderlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shader/base1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shader/base2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.543932 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/backgroundshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/imageshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17813 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/lineshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53883 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/meshshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/pointsshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/textshader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25516 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/shaders/volumeshader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.543932 pygfx-0.2.0/pygfx/renderers/wgpu/wgsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/wgsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/wgsl/line.wgsl
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/renderers/wgpu/wgsl/points.wgsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.547932 pygfx-0.2.0/pygfx/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/resources/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/resources/_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/resources/_texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.547932 pygfx-0.2.0/pygfx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51540 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/_cmdata_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/cube_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/gallery_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/renderfunctionregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.551932 pygfx-0.2.0/pygfx/utils/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_fontfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_fontmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_shaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/text/_tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25675 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-15 14:50:02.000000 pygfx-0.2.0/pygfx/utils/viewport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.551932 pygfx-0.2.0/pygfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:50:12.000000 pygfx-0.2.0/pygfx.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-15 14:50:12.555932 pygfx-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-15 14:50:02.000000 pygfx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:50:12.551932 pygfx-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 14:50:02.000000 pygfx-0.2.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-15 14:50:02.000000 pygfx-0.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 14:50:02.000000 pygfx-0.2.0/tests/testutils.py
```

### Comparing `pygfx-0.1.9/LICENSE` & `pygfx-0.2.0/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2019, Almar Klein
+Copyright (c) 2019-2023, Almar Klein & Korijn van Golen
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pygfx-0.1.9/pygfx/__init__.py` & `pygfx-0.2.0/pygfx/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,22 +9,64 @@
 from .cameras import *
 from .helpers import *
 from .controllers import *
 
 from .renderers import *
 
 from .utils.color import Color
-from .utils.show import show
+from .utils.load import load_mesh, load_meshes, load_scene
+from .utils.show import show, Display
 from .utils.viewport import Viewport
-from .utils import cm
+from .utils.text import font_manager
+from .utils import cm, enums, logger
+from .utils.enums import *
 
+# Temp fix for pyinstaller to pick up pylinalg
+import pylinalg
 
-__version__ = "0.1.9"
+del pylinalg
+
+__version__ = "0.2.0"
 version_info = tuple(map(int, __version__.split(".")))
 
+__wgpu_version_range__ = "0.15.1", "0.16.0"
+__pylinalg_version_range__ = "0.4.1", "0.5.0"
+
+
+def _check_lib_version(libname, pipname, version_range):
+    import importlib  # noqa
+
+    lib = importlib.import_module(libname)
+
+    min_ver, max_ver = version_range
+    min_ver_info = tuple(map(int, min_ver.split(".")))
+    max_ver_info = tuple(map(int, max_ver.split(".")))
+    detected = f"Detected {lib.__version__}, need >={min_ver}, <{max_ver}."
+    if lib.version_info < min_ver_info:
+        logger.error(
+            f"Incompatible version of {libname}:\n    {detected}\n    To update, use e.g. `pip install -U {pipname}`."
+        )
+    elif lib.version_info >= max_ver_info:
+        logger.warning(f"Possible incompatible version of {libname}:\n    {detected}")
+
+
+_check_lib_version("wgpu", "wgpu", __wgpu_version_range__)
+_check_lib_version("pylinalg", "pylinalg", __pylinalg_version_range__)
+
+
+def _get_sg_image_scraper():
+    """Hook for sphinx so we can tell it how to generate the gallery."""
+    import sphinx_gallery.scrapers
+    from .utils.gallery_scraper import pygfx_scraper
+
+    # add webp as supported extension
+    sphinx_gallery.scrapers._KNOWN_IMG_EXTS += ("webp",)
+
+    return pygfx_scraper
+
 
 # Elements of this library are derived from three.js, original license
 # at time of writing copied here:
 # ---
 # The MIT License
 #
 # Copyright © 2010-2022 three.js authors
```

### Comparing `pygfx-0.1.9/pygfx/cameras/_base.py` & `pygfx-0.2.0/pygfx/cameras/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,82 @@
-from ..linalg import Matrix4, Vector3
+import numpy as np
+
 from ..objects._base import WorldObject
 
 
 class Camera(WorldObject):
     """Abstract base camera.
 
+    Camera's are world objects and be placed in the scene, but this is not required.
+
     The purpose of a camera is to define the viewpoint for rendering a scene.
-    This viewpoint consists of its position (in the world) and its projection.
+    This viewpoint consists of its position and orientation (in the world) and
+    its projection.
 
     In other words, it covers the projection of world coordinates to
     normalized device coordinates (NDC), by the (inverse of) the
     camera's own world matrix and the camera's projection transform.
     The former represent the camera's position, the latter is specific
     to the type of camera.
-
-    Note that we follow the NDC coordinate system of WGPU, where
-    x and y are in the range 0..1, z is in the range 0..1, and (-1, -1, 0)
-    represents the bottom left corner.
-
     """
 
+    _FORWARD_IS_MINUS_Z = True
+
     def __init__(self):
         super().__init__()
 
-        self.matrix_world_inverse = Matrix4()
-        self.projection_matrix = Matrix4()
-        self.projection_matrix_inverse = Matrix4()
+        self.projection_matrix = np.eye(4, dtype=float)
+        self.projection_matrix_inverse = np.eye(4, dtype=float)
 
     def set_view_size(self, width, height):
-        # In logical pixels
+        # In logical pixels, called by the renderer to set the viewport size
         pass
 
-    def update_matrix_world(self, *args, **kwargs):
-        super().update_matrix_world(*args, **kwargs)
-        self.matrix_world_inverse.get_inverse(self.matrix_world)
-
     def update_projection_matrix(self):
         raise NotImplementedError()
 
-    def show_object(
-        self, target: WorldObject, view_dir=(-1, -1, -1), distance_weight=2
-    ):
-        """Utility function to position and rotate the camera to ensure
-        a particular world object is in view.
-
-        Parameters:
-            target: WorldObject
-                The object to look at
-            view_dir: 3-tuple of float
-                Look at the object in this direction
-            distance_weight: float
-                The camera distance to the object's world position is
-                its bounding sphere radius multiplied by this weight
-
-        Returns:
-            pos: Vector3
-                The world coordinate the camera is looking at
+    def get_state(self):
+        """Get the state of the camera as a dict."""
+        return {}
+
+    def set_state(self, state):
+        """Set the state of the camera from a dict obtained with ``get_state``
+        from a camera of the same type.
         """
-        bsphere = target.get_world_bounding_sphere()
-        if bsphere is not None:
-            pos, distance = Vector3(*bsphere[:3]), bsphere[3]
-        else:
-            pos = target.get_world_position()
-            # whatever it is has no bounding sphere, so we just pick an
-            # arbitrary distance
-            distance = 100
-        distance *= distance_weight
-        self.position.copy(pos).add_scaled_vector(
-            Vector3(*view_dir).normalize().negate(), distance
-        )
-        self.look_at(pos)
-        return pos
+        pass
 
     @property
-    def flips_winding(self):
-        """Get whether the camera flips any dimensions causing the
-        winding of faces to be flipped. Note that if an even number of
-        dimensions are flipped, the winding is not affected.
-        """
-        return False
+    def view_matrix(self) -> np.ndarray:
+        return self.world.inverse_matrix
+
+    @property
+    def camera_matrix(self) -> np.ndarray:
+        return self.projection_matrix @ self.view_matrix
 
 
 class NDCCamera(Camera):
-    """A Camera operating in NDC coordinates: its projection matrix
-    is the identity transform (but its matrix_world can still be set).
+    """A Camera operating in NDC coordinates.
+
+    Its projection matrix is the identity transform (but its position and rotation can still be set).
 
     In the NDC coordinate system of WGPU (and pygfx), x and y are in
-    the range 0..1, z is in the range 0..1, and (-1, -1, 0) represents
-    the bottom left corner."""
+    the range -1..1, z is in the range 0..1, and (-1, -1, 0) represents
+    the bottom left corner.
+    """
 
     def update_projection_matrix(self):
-        eye = 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1
-        self.projection_matrix.set(*eye)
-        self.projection_matrix_inverse.set(*eye)
+        eye = np.eye(4)
+        self.projection_matrix = eye
+        self.projection_matrix_inverse = eye
 
 
 class ScreenCoordsCamera(Camera):
-    """A Camera operating in screen coordinates. The depth range is the same
-    as in NDC (0 to 1).
+    """A Camera operating in screen coordinates.
+
+    The depth range is the same as in NDC (0 to 1).
     """
 
     def __init__(self):
         super().__init__()
         self._width = 1
         self._height = 1
 
@@ -109,9 +84,10 @@
         self._width = width
         self._height = height
 
     def update_projection_matrix(self):
         sx, sy, sz = 2 / self._width, 2 / self._height, 1
         dx, dy, dz = -1, -1, 0
         m = sx, 0, 0, dx, 0, sy, 0, dy, 0, 0, sz, dz, 0, 0, 0, 1
-        self.projection_matrix.set(*m)
-        self.projection_matrix_inverse.get_inverse(self.projection_matrix)
+        proj_view = self.projection_matrix.ravel()
+        proj_view[:] = m
+        self.projection_matrix_inverse = np.linalg.inv(self.projection_matrix)
```

### Comparing `pygfx-0.1.9/pygfx/geometries/_toroidal.py` & `pygfx-0.2.0/pygfx/geometries/_toroidal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 import numpy as np
 
 from ._base import Geometry
 
 
-def klein_bottle_geometry(scale=1.0):
-    """The Klein bottle is a surface for which the inside and outside
+def klein_bottle_geometry(scale=1.0, stitch=False):
+    """Generate a Klein bottle.
+
+    The Klein bottle is a surface for which the inside and outside
     are the same, similar to a Möbius strip. In fact, a Klein bottle
     can be constructed by glueing together two Möbius strips.
 
-    More technically: the Klein bottle is an example of a non-orientable
-    surface; it is a two-dimensional manifold against which a system
-    for determining a normal vector cannot be consistently defined.
+    Parameters
+    ----------
+    scale : float
+        The scale of the bottle.
+    stitch : bool
+        Whether to stitch the ends together to produce a closed
+        manifold. If True, a mathematically correct Klein bottle is
+        produced. If False (default) an approximation is produced where
+        the ends of the bottle meet, but are not actually connected.
+
+    Returns
+    -------
+    klein_bottle : Geometry
+        A geometry object representing the requested klein bottle.
+        Mathematically, it is either an "orientable open manifold" or
+        a "non-orientable closed manifold", depending on the ``stitch``
+        parameter.
+
     """
 
     # This is an interesting object for mathematicians. For us it's
     # interesting because we can test whether our lighting etc. deals
     # correctly with objects for which the "inside" must also be shown.
 
     # The number of vertices is nxn
@@ -51,20 +68,37 @@
     # Replicate to all rectangles, add offsets
     indices = np.tile(indices, (n, n - 1, 1))
     gx, gy = np.meshgrid(
         np.arange(indices.shape[1], dtype=np.uint32),
         n * np.arange(indices.shape[0], dtype=np.uint32),
     )
     indices += (gx + gy).reshape(indices.shape[:2] + (1,))
-    # Stitch the ends together over one axis. We can't stitch the other ends
-    # together, since that's where the normals flip from "inside" to "outside".
+
+    # Stitch the faces at the tube's edge.
     indices[-1, :, 2:5] -= n * n
-    indices = indices.reshape((-1, 3))
+
+    if stitch:
+        # We can do the same for the tube's ends, and make this a closed
+        # manifold! Note that in doing that, we also make it
+        # not-orientable - the orientation of the faces (i.e. the
+        # winding) switches where we apply the stitch. Also note that
+        # in the current implementation we're left with n unused
+        # vertices.
+
+        # In the code below, i1 are one end of the tube, and i2 the
+        # other. Since the tube is inside-out, the matching pairs are
+        # on opposing sides.
+        for i in range(n):
+            i2 = n - 1 + i * n
+            i1 = (n // 2 - i) * n
+            i1 = i1 if i1 >= 0 else i1 + positions.shape[0]
+            indices[indices == i2] = i1
 
     # Create buffers for this geometry
+    indices = indices.reshape((-1, 3))
     return Geometry(indices=indices, positions=positions, texcoords=texcoords)
 
 
 def klein_bottle_surface(u, v):
     """
     http://paulbourke.net/geometry/toroidal/
 
@@ -81,36 +115,56 @@
     y = 16 * np.sin(u)
     y[half] = (16 * np.sin(u) + r * np.sin(u) * np.cos(v))[half]
     z = r * np.sin(v)
     return x, y, z
 
 
 def torus_knot_geometry(
-    scale=1.0, tube=0.4, tubular_segments=64, radial_segments=8, p=2, q=3
+    scale=1.0, tube=0.4, tubular_segments=64, radial_segments=8, p=2, q=3, stitch=False
 ):
-    """Create geometry representing a torus knot, the particular shape of which
-    is defined by a pair of coprime integers, p and q. If p and q are not coprime,
+    """Generate a torus knot.
+
+    Create geometry representing a torus knot, the particular shape of which is
+    defined by a pair of coprime integers, p and q. If p and q are not coprime,
     the result will be a torus link.
 
-    Arguments:
-        scale (float): the scale of the torus, default 1.
-        tube (float): the radius of the tube. Default 0.4.
-        tubular_segments (int): default is 64.
-        radial_segments (int): default is 8.
-        p (int): how many times the geometry winds around its axis of
-            rotational symmetry. Default 2.
-        q (int): how many times the geometry winds around a circle in
-            the interior of the torus. Default 3.
+    Parameters
+    ----------
+    scale : float
+        The scale of the torus, default 1.
+    tube : float
+        The radius of the tube. Default 0.4.
+    tubular_segments : int
+        default is 64.
+    radial_segments : int
+        default is 8.
+    p : int
+        How many times the geometry winds around its axis of
+        rotational symmetry. Default 2.
+    q : int
+        How many times the geometry winds around a circle in
+        the interior of the torus. Default 3.
+    stitch : bool
+        Whether to stitch the ends together to produce a closed
+        manifold. Default False. If False, the mesh is basically a
+        curved surface with the edges meeting to make it visually
+        closed, which works better for texturing. Set to True for a
+        mathematically closed object.
+
+    Returns
+    -------
+    torus : Geometry
+        A geometry object representing the requested torus.
+        Mathematically, it is an open orientable manifold, which can
+        be closed with the ``stitch`` parameter.
 
     """
 
-    # If we stitch, we have no duplicate vertices, but stitch the
-    # ends together with the indices, resulting in a fully closed object.
-    # However, texturing works better without such stitching.
-    stitch = False
+    # If we do not stitch, the two ends meet (i.e. duplicate vertices)
+    # to make the mesh look closed (while mathematically it is not).
 
     if stitch:
         tubular_verts = tubular_segments
         radial_verts = radial_segments
     else:
         tubular_verts = tubular_segments + 1
         radial_verts = radial_segments + 1
@@ -120,17 +174,19 @@
         0, p * 2 * np.pi, tubular_verts, endpoint=not stitch, dtype=np.float32
     )
     v = np.linspace(0, 2 * np.pi, radial_verts, endpoint=not stitch, dtype=np.float32)
 
     # Get positions along the torus' center, and a tiny step further
     pos1 = torus_knot_surface(u, p, q, scale)
     pos2 = torus_knot_surface(u + 0.01, p, q, scale)
+
     # Two vectors along the torus' centerline
-    vec1 = pos1 - pos2
-    vec2 = pos1 + pos2
+    vec1 = np.ndarray.astype(pos1 - pos2, np.float32, copy=False)
+    vec2 = np.ndarray.astype(pos1 + pos2, np.float32, copy=False)
+
     # Two vectors orthoginal to the torus' centerline
     vec3 = np.cross(vec1, vec2)
     vec4 = np.cross(vec3, vec1)
     # Normalize
     vec3 /= ((vec3[:, 0] ** 2 + vec3[:, 1] ** 2 + vec3[:, 2] ** 2) ** 0.5).reshape(
         -1, 1
     )
@@ -156,29 +212,32 @@
     # Create texcords
     # ty, tx = np.meshgrid(u / u[-1], v / v[-1])
     ty, tx = np.meshgrid(v / v[-1], u / u[-1])
     texcoords = np.column_stack((tx.flat, ty.flat))
 
     # Create indices
     # Two triangles onto the "top-left" rectangle (six vertices)
-    indices = np.array(
-        [radial_verts, 0, radial_verts + 1, radial_verts + 1, 0, 1],
-        np.uint32,
-    )
+    if stitch:
+        base_triangle = [radial_verts - 1, 0, radial_verts, radial_verts, 0, 1]
+    else:
+        base_triangle = [radial_verts, 0, radial_verts + 1, radial_verts + 1, 0, 1]
+    base_triangle = np.array(base_triangle, np.uint32)
+
     # Replicate to all rectangles, add offsets
-    indices = np.tile(indices, (tubular_segments, radial_segments, 1))
+    indices = np.tile(base_triangle, (tubular_segments, radial_segments, 1))
     gx, gy = np.meshgrid(
         np.arange(indices.shape[1], dtype=np.uint32),
         radial_verts * np.arange(indices.shape[0], dtype=np.uint32),
     )
     indices += (gx + gy).reshape(indices.shape[:2] + (1,))
-    # Stitch the ends together over both axii.
+
+    # Correct the faces at the tube's ends
     if stitch:
-        indices[-1, :, 1:4] -= radial_verts * tubular_verts
-        indices[:, -1, 2:5] -= radial_verts
+        indices[indices >= len(positions)] -= len(positions)
+
     indices = indices.reshape((-1, 3))
     # indices = np.fliplr(indices)  # Use this to change winding between CW and CCW
 
     return Geometry(
         indices=indices, positions=positions, normals=normals, texcoords=texcoords
     )
```

### Comparing `pygfx-0.1.9/pygfx/helpers/_box.py` & `pygfx-0.2.0/pygfx/helpers/_box.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import numpy as np
 
 from .. import Geometry, Line, LineSegmentMaterial
+from ..objects import WorldObject
 
 
 class BoxHelper(Line):
-    """A line box object. Commonly used to visualize bounding boxes.
+    """A WorldObject that shows a box-shaped wireframe.
 
-    Parameters:
-        size (float): The length of the box' edges (default 1).
-        thickness (float): the thickness of the lines (default 1 px).
-    """
+    Commonly used to visualize bounding boxes.
+
+    Parameters
+    ----------
+    size : float
+        The length of the box' edges in local space.
+    thickness : float
+        The thickness of the lines in (onscreen) pixels.
+    color : Color
+        The color of the box.
 
-    def __init__(self, size=1.0, thickness=1):
+    """
 
-        self._size = size
+    def __init__(self, size=1.0, thickness=1, color="white"):
+        self._size = float(size)
 
         positions = np.array(
             [
                 [0, 0, 0],  # bottom edges
                 [1, 0, 0],
                 [0, 0, 0],
                 [0, 0, 1],
@@ -41,91 +49,105 @@
                 [0, 1, 1],
                 [1, 0, 1],
                 [1, 1, 1],
             ],
             dtype="f4",
         )
         positions -= 0.5
+
         positions *= self._size
 
         geometry = Geometry(positions=positions)
-        material = LineSegmentMaterial(color=(1, 0, 0), thickness=thickness, aa=True)
+        material = LineSegmentMaterial(thickness=thickness, color=color, aa=True)
 
         super().__init__(geometry, material)
 
-    def set_transform_by_aabb(self, aabb):
-        """Set the position and scale attributes
-        based on a given bounding box.
-
-        Parameters:
-            aabb (ndarray): The position and scale attributes
-                will be configured such that the helper
-                will match the given bounding box. The array
-                is expected to have shape (2, 3), where the
-                two vectors represent the minimum and maximum
-                coordinates of the axis-aligned bounding box.
+    def set_transform_by_aabb(self, aabb, scale=1.0):
+        """Align with axis aligned bounding box.
+
+        The position and scale attributes will be configured such that the
+        helper will match the given bounding box.
+
+        Parameters
+        ----------
+        aabb : ndarray, [2, 3]
+            The bounding box to align with. The two vectors represent the
+            minimum and maximum coordinates of the axis-aligned bounding box.
+        scale : float
+            Scale multiplier of the final wireframe. Useful for adding margin to the
+            box.
+
         """
+
         aabb = np.asarray(aabb)
         if aabb.shape != (2, 3):
             raise ValueError(
                 "The given array does not appear to represent "
                 "an axis-aligned bounding box, ensure "
                 "the shape is (2, 3). Shape given: "
                 f"{aabb.shape}"
             )
 
         diagonal = aabb[1] - aabb[0]
         center = aabb[0] + diagonal * 0.5
-        scale = diagonal / self._size
+        full_scale = scale * diagonal / self._size
 
-        self.position.set(*center)
-        self.scale.set(*scale)
+        self.local.position = center
+        self.local.scale = full_scale
 
-    def set_transform_by_object(self, object, space="world"):
-        """Set the position and scale attributes
-        based on the bounding box of another object.
-
-        Parameters:
-            object (WorldObject): The position and scale attributes
-                will be configured such that the helper
-                will match the bounding box of the given object.
-            space (string, optional): If set to "world"
-                (the default) the world space bounding box will
-                be used as reference. If equal to "local", the
-                object's local space bounding box of its geometry
-                will be used instead.
+    def set_transform_by_object(self, object: WorldObject, space="world", scale=1.0):
+        """Align with WorldObject.
 
-        :Examples:
+        Set the position and scale attributes based on the bounding box of
+        another object.
+
+        Parameters
+        ----------
+        object : WorldObject
+            The object to wrap inside this wireframe.
+        space : str
+            If "world", the wire will be aligned to the world's axes. If
+            "local", the wire will be aligned to the local axes.
+        scale : float
+            Scale multiplier of the final wireframe. Useful for adding margin to the
+            box.
 
-        World-space bounding box visualization:
+        Examples
+        --------
 
-        .. code-block:: py
+        World-space bounding box visualization::
 
             box = gfx.BoxHelper()
             box.set_transform_by_object(mesh)
             scene.add(box)
 
-        Local-space bounding box visualization:
-
-        .. code-block:: py
+        Local-space bounding box visualization::
 
             box = gfx.BoxHelper()
             box.set_transform_by_object(mesh, space="local")
             mesh.add(box)
+
         """
+
         aabb = None
         if space not in {"world", "local"}:
             raise ValueError(
                 'Space argument must be either "world"'
                 f'or "local". Given value: {space}'
             )
         if space == "world":
             aabb = object.get_world_bounding_box()
         elif space == "local" and object.geometry is not None:
-            aabb = object.geometry.bounding_box()
+            aabb = object.geometry.get_bounding_box()
         if aabb is None:
             raise ValueError(
                 "No bounding box could be determined "
                 "for the given object, it (and its "
                 "children) may not define any geometry"
             )
-        self.set_transform_by_aabb(aabb)
+        self.set_transform_by_aabb(aabb, scale)
+
+    def get_world_bounding_box(self):
+        return None
+
+    def get_world_bounding_sphere(self):
+        return None
```

### Comparing `pygfx-0.1.9/pygfx/helpers/_gizmo.py` & `pygfx-0.2.0/pygfx/helpers/_gizmo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,114 @@
 """
 A transform gizmo to manipulate world objects.
 """
 
 import numpy as np
+import pylinalg as la
 
 from ..objects import Line, Mesh
 from ..geometries import Geometry, sphere_geometry, cone_geometry, box_geometry
 from ..materials import MeshBasicMaterial, LineMaterial
 from ..objects import WorldObject
-from ..linalg import Vector3, Quaternion
 from ..utils.viewport import Viewport
+from ..utils.transform import AffineTransform
 
 
 # Colors in hsluv space - https://www.hsluv.org/
 # With H: 0/120/240, S: 100, L: 50
 WHITE = "#ffffff"
 RED = "#ea0064"
 GREEN = "#3f8700"
 BLUE = "#007eb7"
 
 THICKNESS = 3
 
 
 class TransformGizmo(WorldObject):
-    """
-    A gizmo object that can be used to manipulate (i.e. transform) a world object.
+    """Gizmo to manipulate a WorldObject.
 
-    Aguments:
-        object (WorldObject): the object to transform with the gizmo.
-        screen_size (float): the approximate size of the widget in logical pixels. Default 100.
+    This Gizmo allows to interactively control WorldObjects with the mouse
+    inside a canvas. It can translate and rotate objects relative to the world
+    frame, local frame, or camera frame (screen space).
 
     To control the Gizmo:
-    * Click the center sphere to toggle between object-space, world-space and screen-space.
+
+    * Click the center sphere to toggle between object-space, world-space and
+      screen-space.
     * Grab the center sphere for uniform scaling.
     * Grab the cubes for one-directional scaling (only in object-space).
     * Grab the arrows to translate in one direction.
     * Grab the planes to translate in two directions.
     * Grab the spheres to rotate.
+
+    Parameters
+    ----------
+    object : WorldObject
+        The controlled world object.
+    screen_size : float
+        The approximate size of the widget in logical pixels. Default 100.
+
     """
 
     def __init__(self, object=None, screen_size=100):
         super().__init__()
+        self._object_to_control = None
 
         # We store these as soon as we get a call in ``add_default_event_handlers``
         self._viewport = None
         self._camera = None
+        self._ndc_to_screen = None
 
         # A dict that stores the state at the start of a drag. Or None.
         self._ref = None
+        self.gizmo_scale = np.ones(3, dtype=float)
 
-        # The (approximate) size of the gizmo on screen
+        # The radius (in pixels) the gizmo's screen-space bounding box should occupy
+        # (aka. the desired on-screen size of the gizmo)
         self._screen_size = float(screen_size)
 
+        # the extent of the gizmo measured along each cardinal direction
+        # expressed in the local frame
+        # order: right, up, forward, left, down, backward (first 3-tuple is
+        # along positive (x, y, z), second 3-tuple is along negative (x, y, z))
+        self._local_extents = None
+
         # Init
         self._create_elements()
         self.toggle_mode("object")  # object, world, screen
         self._highlight()
         self.set_object(object)
 
-    def set_object(self, object):
-        """Set the WorldObject to control with the gizmo."""
-        if object is None or isinstance(object, WorldObject):
-            self._object_to_control = object
-        else:
+    def set_object(self, object: WorldObject):
+        """Update the controlled object.
+
+        Parameters
+        ----------
+        object : WorldObject
+            The new controlled object.
+
+        """
+
+        if not isinstance(object, (WorldObject, None)):
             raise ValueError("The object must be None or a WorldObject instance.")
 
+        self._object_to_control = object
+
     def toggle_mode(self, mode=None):
-        """Toggle between modes. If the mode is omitted, will move to the next mode.
-        Must be one of "object", "world", or "screen".
+        """Switch the reference frame.
+
+        Parameters
+        ----------
+        mode : str
+            The reference frame to switch to. Must be one of  ``"object"``
+            (local frame), ``"world"`` (world frame), or ``"screen"`` (camera
+            frame). If None the next mode (following this order) is selected.
+
         """
+
         modes = "object", "world", "screen"
         if not mode:
             mode = {"object": "world", "world": "screen"}.get(self._mode, "object")
         if mode not in modes:
             raise ValueError(f"Invalid mode '{mode}', must be one of {modes}.")
         self._mode = mode
         self._on_mode_switch()  # The gizmo looks a bit different in each mode
@@ -85,17 +121,17 @@
 
         # --- the parts that are at the center
 
         # Create screen translate handle
         sphere_geo = sphere_geometry(0.07)
         scale_uniform = Mesh(
             sphere_geo,
-            MeshBasicMaterial(color=WHITE),
+            MeshBasicMaterial(color=WHITE, pick_write=True),
         )
-        scale_uniform.scale.set(1.5, 1.5, 1.5)
+        scale_uniform.local.scale = (1.5, 1.5, 1.5)
 
         # --- the parts that are fully in one dimension
 
         # Create lines
         line_geo = Geometry(positions=[(0, 0, 0), (halfway, 0, 0)])
         line_x = Line(
             line_geo,
@@ -111,45 +147,45 @@
         )
 
         # Create 1D translate handles
         cone_geo = cone_geometry(0.1, 0.17)
         cone_geo.positions.data[:] = cone_geo.positions.data[:, ::-1]  # xyz->zyx
         translate_x = Mesh(
             cone_geo,
-            MeshBasicMaterial(color=RED),
+            MeshBasicMaterial(color=RED, pick_write=True),
         )
         translate_y = Mesh(
             cone_geo,
-            MeshBasicMaterial(color=GREEN),
+            MeshBasicMaterial(color=GREEN, pick_write=True),
         )
         translate_z = Mesh(
             cone_geo,
-            MeshBasicMaterial(color=BLUE),
+            MeshBasicMaterial(color=BLUE, pick_write=True),
         )
-        translate_x.position.set(1, 0, 0)
-        translate_y.position.set(0, 1, 0)
-        translate_z.position.set(0, 0, 1)
+        translate_x.local.position = (1, 0, 0)
+        translate_y.local.position = (0, 1, 0)
+        translate_z.local.position = (0, 0, 1)
 
         # Create scale handles
         cube_geo = box_geometry(0.1, 0.1, 0.1)
         scale_x = Mesh(
             cube_geo,
-            MeshBasicMaterial(color=RED),
+            MeshBasicMaterial(color=RED, pick_write=True),
         )
         scale_y = Mesh(
             cube_geo,
-            MeshBasicMaterial(color=GREEN),
+            MeshBasicMaterial(color=GREEN, pick_write=True),
         )
         scale_z = Mesh(
             cube_geo,
-            MeshBasicMaterial(color=BLUE),
+            MeshBasicMaterial(color=BLUE, pick_write=True),
         )
-        scale_x.position.set(halfway, 0, 0)
-        scale_y.position.set(0, halfway, 0)
-        scale_z.position.set(0, 0, halfway)
+        scale_x.local.position = (halfway, 0, 0)
+        scale_y.local.position = (0, halfway, 0)
+        scale_z.local.position = (0, 0, halfway)
 
         # --- the parts that are in a plane
 
         # Create arcs
         t = np.linspace(0, np.pi / 2, 64)
         arc_positions = np.stack([0 * t, np.sin(t), np.cos(t)], 1).astype(np.float32)
         arc_geo = Geometry(positions=arc_positions * halfway)
@@ -161,70 +197,72 @@
             arc_geo,
             LineMaterial(thickness=THICKNESS, color=GREEN),
         )
         arc_xy = Line(
             arc_geo,
             LineMaterial(thickness=THICKNESS, color=BLUE),
         )
-        arc_zx.scale.y = -1
-        arc_xy.scale.z = -1
 
         # Create in-plane translate handles
         plane_geo = box_geometry(0.01, 0.15, 0.15)
         translate_yz = Mesh(
             plane_geo,
-            MeshBasicMaterial(color=RED),
+            MeshBasicMaterial(color=RED, pick_write=True),
         )
         translate_zx = Mesh(
             plane_geo,
-            MeshBasicMaterial(color=GREEN),
+            MeshBasicMaterial(color=GREEN, pick_write=True),
         )
         translate_xy = Mesh(
             plane_geo,
-            MeshBasicMaterial(color=BLUE),
+            MeshBasicMaterial(color=BLUE, pick_write=True),
         )
         inside_arc = 0.4 * halfway
-        translate_yz.position.set(0, inside_arc, inside_arc)
-        translate_zx.position.set(inside_arc, 0, inside_arc)
-        translate_xy.position.set(inside_arc, inside_arc, 0)
+        translate_yz.local.position = (0, inside_arc, inside_arc)
+        translate_zx.local.position = (inside_arc, 0, inside_arc)
+        translate_xy.local.position = (inside_arc, inside_arc, 0)
 
         # Create rotation handles
         # These are positioned on each mode switch
         rotate_yz = Mesh(
             sphere_geo,
-            MeshBasicMaterial(color=RED),
+            MeshBasicMaterial(color=RED, pick_write=True),
         )
         rotate_zx = Mesh(
             sphere_geo,
-            MeshBasicMaterial(color=GREEN),
+            MeshBasicMaterial(color=GREEN, pick_write=True),
         )
         rotate_xy = Mesh(
             sphere_geo,
-            MeshBasicMaterial(color=BLUE),
+            MeshBasicMaterial(color=BLUE, pick_write=True),
         )
 
         # --- post-process
 
         # Rotate objects to their correct orientation
-        for ob in [line_y, translate_y, scale_y, arc_zx, translate_zx, rotate_zx]:
-            ob.rotation.set_from_axis_angle(Vector3(0, 0, 1), np.pi / 2)
-        for ob in [line_z, translate_z, scale_z, arc_xy, translate_xy, rotate_xy]:
-            ob.rotation.set_from_axis_angle(Vector3(0, -1, 0), np.pi / 2)
+        ob: WorldObject
+        for ob in [line_y, translate_y, scale_y, translate_zx, rotate_zx]:
+            ob.local.rotation = la.quat_from_axis_angle((0, 0, 1), np.pi / 2)
+        for ob in [line_z, translate_z, scale_z, translate_xy, rotate_xy]:
+            ob.local.rotation = la.quat_from_axis_angle((0, -1, 0), np.pi / 2)
+
+        arc_xy.local.rotation = la.quat_from_axis_angle((0, 1, 0), np.pi / 2)
+        arc_zx.local.rotation = la.quat_from_axis_angle((0, 0, 1), -np.pi / 2)
 
-        # Store the objectss
+        # Store the objects
         self._center_sphere = scale_uniform
         self._line_children = line_x, line_y, line_z
         self._arc_children = arc_yz, arc_zx, arc_xy
         self._translate1_children = translate_x, translate_y, translate_z
         self._translate2_children = translate_yz, translate_zx, translate_xy
         self._translate_children = self._translate1_children + self._translate2_children
         self._scale_children = scale_x, scale_y, scale_z
         self._rotate_children = rotate_yz, rotate_zx, rotate_xy
 
-        # Lines and arcs are never apaque. That way they're also not
+        # Lines and arcs are never opaque. That way they're also not
         # pickable, so they won't be "in the way".
         for ob in self._line_children + self._arc_children:
             ob.material.opacity = 0.6
 
         # Assign dimensions
         scale_uniform.dim = None
         for triplet in [
@@ -244,40 +282,45 @@
         self.add(*self._line_children)
         self.add(*self._arc_children)
         self.add(self._center_sphere)
         self.add(*self._translate_children)
         self.add(*self._scale_children)
         self.add(*self._rotate_children)
 
+        # work out local extent
+        self._local_extents = np.empty((6, 3), dtype=float)
+        scales = self.get_bounding_box().ravel()  # we know our bb is not None
+        self._local_extents[:3] = np.diag(scales[3:])
+        self._local_extents[3:] = np.diag(scales[:3])
+
     def _on_mode_switch(self):
         """When the mode is changed, some adjustments are made."""
 
         # Note: the elements are affected by the mode in various ways.
         # Much of that (e.g. visibility) is already handled in the
         # _update_xx functions, so we don't have to do that here.
 
         # Update position of rotation handles
         rotate_yz, rotate_zx, rotate_xy = self._rotate_children
         halfway = self._halfway
         on_arc = halfway * 2**0.5 / 2
-        if self._mode == "screen":
-            rotate_yz.position.set(0, on_arc, 0)
-            rotate_zx.position.set(on_arc, 0, 0)
-            rotate_xy.position.set(on_arc, on_arc, 0)
-        else:
-            rotate_yz.position.set(0, on_arc, on_arc)
-            rotate_zx.position.set(on_arc, 0, on_arc)
-            rotate_xy.position.set(on_arc, on_arc, 0)
+        rotate_yz.local.position = (0, on_arc, on_arc)
+        rotate_zx.local.position = (on_arc, 0, on_arc)
+        rotate_xy.local.position = (on_arc, on_arc, 0)
 
     def _highlight(self, object=None):
         """Change the appearance during interaction for visual feedback
         on what is being manipulated.
         """
         # Reset thickness of all lines
-        for ob in self._line_children + self._arc_children:
+        for ob in self._line_children:
+            if ob.material.thickness != THICKNESS:
+                ob.material.thickness = THICKNESS
+
+        for ob in self._arc_children:
             if ob.material.thickness != THICKNESS:
                 ob.material.thickness = THICKNESS
 
         # Set thickness of lines corresponding to the object
         if object:
             lines = []
             dim = object.dim
@@ -288,231 +331,221 @@
                     lines.append(self._arc_children[dim])
                 else:  # translate1 or scale
                     lines.append(self._line_children[dim])
             else:  # translate2
                 lines.append(self._line_children[dim[0]])
                 lines.append(self._line_children[dim[1]])
             for ob in lines:
-                ob.material.thickness = THICKNESS * 1.75
+                ob.material.thickness *= 1.75
 
-    # %% Updating before each draw
+    def update_gizmo(self, event):
+        if event.type != "before_render":
+            return
 
-    def update_matrix_world(self, *args, **kwargs):
-        """We overload this method, which gets called by the renderer
-        just before rendering. This allows us to prep the gizmo just
-        in time.
-        """
         # Note that we almost always update the transform (scale,
         # rotation, position) which means the matrix changed, and so
         # does the world_matrix of all children. In effect the uniforms
         # of all elements need updating anyway, so any other changes
         # to wobject properties (e.g. visibility) are "free" - no need
         # to only update if it actually changes.
         if not self._object_to_control:
             self.visible = False
         elif self._viewport and self._camera:
             self.visible = True
+            self._update_ndc_screen_transform()
             self._update_directions()
-            self._update_scale()
+            self._update_gizmo_transform()
             self._update_visibility()
-        super().update_matrix_world(*args, **kwargs)
+
+    def _update_ndc_screen_transform(self):
+        # Note: screen origin is at top left corner of NDC with Y-axis pointing down
+        x_dim, y_dim = self._viewport.logical_size
+        screen_space = AffineTransform()
+        screen_space.position = (-1, 1, 0)
+        screen_space.scale = (2 / x_dim, -2 / y_dim, 1)
+        self._ndc_to_screen = screen_space.inverse_matrix
+        self._screen_to_ndc = screen_space.matrix
 
     def _update_directions(self):
-        """Calculate the x/y/z reference directions, which depend on
-        mode and camera. Calculate these for world-space, ndc-space and
-        screen-space.
         """
+        Calculate how much 1 unit of translation in the draggable space (aka
+        mode) translates the object in world and screen space.
 
-        camera = self._camera
-        scene_size = self._viewport.logical_size
-        world_pos = self._object_to_control.position
-        ndc_pos = world_pos.clone().project(camera)
+        """
 
-        # Calculate direction pairs (world_directions, ndc_directions)
-        base_directions = Vector3(1, 0, 0), Vector3(0, 1, 0), Vector3(0, 0, 1)
+        # work out the transforms between the spaces
+        camera = self._camera
         if self._mode == "object":
-            # The world direction is derived from the object
-            rot = self._object_to_control.rotation.clone()
-            world_directions = [vec.apply_quaternion(rot) for vec in base_directions]
-            # Calculate ndc directions from here
-            ndc_directions = [
-                world_pos.clone().add(vec).project(camera).sub(ndc_pos)
-                for vec in world_directions
-            ]
+            # local space is draggable
+            local_to_world = self._object_to_control.world.matrix
+            local_to_ndc = camera.camera_matrix @ local_to_world
+            local_to_screen = self._ndc_to_screen @ local_to_ndc
         elif self._mode == "world":
-            # The world direction is the base direction
-            rot = Quaternion()  # null rotation
-            world_directions = base_directions
-            # Calculate ndc directions from here
-            ndc_directions = [
-                world_pos.clone().add(vec).project(camera).sub(ndc_pos)
-                for vec in world_directions
-            ]
+            # world space is draggable
+            local_to_world = np.eye(4)
+            local_to_ndc = camera.camera_matrix @ local_to_world
+            local_to_screen = self._ndc_to_screen @ local_to_ndc
         elif self._mode == "screen":
-            # The screen direction is the base_direction
-            rot = Quaternion().set_from_rotation_matrix(camera.matrix_world)
-            screen_directions = [
-                vec.multiply_scalar(self._screen_size) for vec in base_directions
-            ]
-            # Convert to world directions
-            ndc_directions = [
-                Vector3(vec.x / scene_size[0] * 2, vec.y / scene_size[1] * 2, -vec.z)
-                for vec in screen_directions
-            ]
-            world_directions = [
-                ndc_pos.clone().add(vec).unproject(camera).sub(world_pos)
-                for vec in ndc_directions
-            ]
+            # camera space is draggable
+            local_to_world = camera.world.matrix
+            local_to_ndc = camera.projection_matrix
+            local_to_screen = self._ndc_to_screen @ local_to_ndc
         else:  # This cannot happen, in theory
-            raise RuntimeError(f"Unexpected mode: '{self._mode}'")
+            raise RuntimeError(f"Unexpected mode: `{self._mode}`")
 
-        # Calculate screen directions from ndc_directions (also re-calculate for screen mode)
-        # These represent how much one "step" moves on screen.
-        # Note how for ndc_directions we have a valid z, but for screen_directions z is 0.
-        screen_directions = [
-            Vector3(vec.x * scene_size[0] / 2, -vec.y * scene_size[1] / 2, 0)
-            for vec in ndc_directions
-        ]
-
-        # Store direction lists, to be used during a drag operation.
-        self._world_directions = world_directions
-        self._ndc_directions = ndc_directions
-        self._screen_directions = screen_directions
-
-        # Apply rotation
-        self.rotation = rot
+        # points referring to local coordinate axes and origin
+        local_points = np.zeros((4, 3))
+        local_points[1:, :] = np.eye(3)
+        if self._mode == "screen":
+            # reference frame has a z-offset from screen origin
+            object_to_ndc = camera.camera_matrix @ self._object_to_control.world.matrix
+            depth = la.vec_transform((0, 0, 0), object_to_ndc)[2]
+
+            local_points[3, 2] = -1  # camera has inverted Z axis
+            local_points[:, 2] -= depth
+
+        # express unit vectors and origin in the various frames
+        world_points = la.vec_transform(local_points, local_to_world)
+        ndc_points = la.vec_transform(local_points, local_to_ndc)
+        screen_points = la.vec_transform(local_points, local_to_screen)
+
+        # store the directions for future use
+        self._world_directions = world_points[1:] - world_points[0]
+        self._ndc_directions = ndc_points[1:] - ndc_points[0]
+        self._screen_directions = screen_points[1:] - screen_points[0]
 
-    def _update_scale(
+    def _update_gizmo_transform(
         self,
     ):
-        """Update the scale of the gizmo so it gets the correct
-        (approximate) size on screen.
         """
 
-        # During interaction we don't adjust the scale, this way:
+        Set the gizmo's transform to keep it in sync with the object it is
+        tracking while accounting for the gizmo's mode.
+
+        Position: Set to match the tracked object.
+        Rotation: Set to indicate translation directions of the current mode.
+        Scale: Set to have the target on-screen size.
+
+        Note: This function also flips the directions of the gizmo's local axes
+        so that handles always point towards the camera.
+        """
+
+        self.world.position = self._object_to_control.world.position
+
+        # negative/flipped scale on 2 axes registers as 180° rotation. This will
+        # be undone by the rotation update below and will sometimes flip the
+        # gizmo during rotation updates. Instead, reset scale and restore the
+        # desired scale after the rotation update.
+        self.world.scale = 1
+
+        if self._mode == "object":
+            self.world.rotation = self._object_to_control.world.rotation
+        elif self._mode == "world":
+            self.world.rotation = np.array((0, 0, 0, 1))
+        else:  # self._mode == "screen"
+            self.world.rotation = self._camera.world.rotation
+
+        # During interaction we don't update gzimo scale and axis flip, this way:
         # * During a rotation the gizmo does not flip,
         #   making it easier to see how much was rotated.
         # * During a translation the gizmo keeps its "world size",
         #   so that the perspective helps you see how the gizmo has moved.
         if self._ref:
+            self.world.scale = self.gizmo_scale
             return
 
-        camera = self._camera
-        scene_size = self._viewport.logical_size
-        world_pos = self._object_to_control.position
-        ndc_pos = world_pos.clone().project(camera)
-
-        # Get how our direction vectors express on screen
-        ndc_sx = self._screen_size * 2 / scene_size[0]
-        ndc_sy = self._screen_size * 2 / scene_size[1]
-        vec1 = (
-            ndc_pos.clone().add(Vector3(ndc_sx, 0, 0)).unproject(camera).sub(world_pos)
-        )
-        vec2 = (
-            ndc_pos.clone().add(Vector3(0, ndc_sy, 0)).unproject(camera).sub(world_pos)
-        )
-        scale_scalar = 0.5 * (vec1.length() + vec2.length())
-
-        # Determine the scale of this object, so that it gets the intended size on screen.
-        scale = [scale_scalar, scale_scalar, scale_scalar]
-
-        # Determine any flips so that the gizmo faces the camera. Note
-        # that this checks whether the vector in question points away
-        # from the camera.
-        # -----------------------#  So on a view like this, where the widget
-        #      | g               #  is on the left, the red leg might still
-        # r ___|                 #  just point towards the camera, even though
-        #     /                  #  it might not "feel" this way because the
-        #    b                   #  blue leg may partly obscure elements of the
-        # -----------------------#  red leg.
-        for dim, vec in enumerate(self._ndc_directions):
-            if vec.z > 0:
-                scale[dim] = -scale[dim]
+        # size on screen for scale=1
+        local_to_screen = (
+            self._ndc_to_screen @ self._camera.camera_matrix @ self.world.matrix
+        )
+        screen_extents = la.vec_transform(self._local_extents, local_to_screen)
+        origin_screen = la.vec_transform((0, 0, 0), local_to_screen)
+        screen_directions = screen_extents - origin_screen
+
+        # radius of bounding circle (in screen space) and scaling to set to
+        # desired radius (aka _screen_size)
+        size_1_radius = np.max(np.linalg.norm(screen_directions[:, :2], axis=-1))
+        self.gizmo_scale[:] = self._screen_size / size_1_radius
+
+        # if required, flip axes so that handles always point towards the camera
+        eps = 1e-10
+        should_flip = screen_directions[:3, 2] > eps
+        self.gizmo_scale *= 1 - 2 * should_flip
 
-        # Apply scale
-        self.scale = Vector3(*scale)
+        self.world.scale = self.gizmo_scale
 
     def _update_visibility(self):
         """Depending on the mode and the orientation of the camera,
         some elements are made invisible.
         """
 
-        screen_directions = self._screen_directions
-
-        # The scaled screen direction matches the size of the widget on screen.
-        scale_scalar = abs(self.scale.x)
-        scaled_screen_directions = [
-            vec.clone().multiply_scalar(scale_scalar) for vec in screen_directions
-        ]
-
-        # Determine what directions are orthogonal to the view plane
-        show_direction = [True, True, True]
-        for dim, vec in enumerate(scaled_screen_directions):
-            size = (vec.x**2 + vec.y**2) ** 0.5
-            show_direction[dim] = size > 30  # in pixels
-
-        # Also determine whether in-plane elements (arcs and translate2 handles) become hard to see
-        show_direction2 = [True, True, True]
-        for dim, vec in enumerate(screen_directions):
-            dims = [(1, 2), (2, 0), (0, 1)][dim]
-            vec1 = screen_directions[dims[0]].clone().normalize()
-            vec2 = screen_directions[dims[1]].clone().normalize()
-            show_direction2[dim] = abs(vec1.dot(vec2)) < 0.9
+        # compute the viewing angle onto the gizmo's coordinate planes
+        screen_normal = la.vec_transform((0, 0, -1), self._camera.world.matrix)
+        screen_normal = la.vec_normalize(screen_normal)
+        plane_normal = (
+            la.vec_transform(np.eye(3), self.world.matrix) - self.world.position
+        )
+        plane_normal = la.vec_normalize(plane_normal)
+        cos_angle = np.sum(plane_normal * screen_normal, axis=-1)
+        viewing_angle = np.pi / 2 - np.arccos(np.clip(np.abs(cos_angle), 0, 1))
+
+        # compute the size of the gizmo's axes on screen
+        gizmo_to_screen = (
+            self._ndc_to_screen @ self._camera.camera_matrix @ self.world.matrix
+        )
+        origin_screen = la.vec_transform((0, 0, 0), gizmo_to_screen)
+        axes_screen = la.vec_transform(np.eye(3), gizmo_to_screen) - origin_screen
+        ax_size = np.linalg.norm(axes_screen[:, :2], axis=-1)
+
+        # check which handles should be shown
+        show_1d_translation = ax_size > 30
+        show_1d_scaling = ax_size > 30
+        show_2d_translation = viewing_angle > deg_to_rad(15)
 
         if self._mode == "screen":
-            # Show x and y lines and translate1 handles
-            for dim, visible in enumerate([True, True, False]):
-                self._line_children[dim].visible = visible
-                self._translate1_children[dim].visible = visible
-            # Show only the xy translate2 handle
-            for dim, visible in enumerate([False, False, True]):
-                self._translate2_children[dim].visible = visible
-                self._arc_children[dim].visible = visible
-        else:
-            # Lines and arcs are always shown
-            for dim in (0, 1, 2):
-                self._arc_children[dim].visible = True
-                self._line_children[dim].visible = True
-            # The translate1 and scale handles depend on their angle to the camera
-            for dim in (0, 1, 2):
-                self._translate1_children[dim].visible = show_direction[dim]
-                self._scale_children[dim].visible = show_direction[dim]
-            # The translate2 handles depend on two angles to the camera
-            for dim in (0, 1, 2):
-                dim1, dim2 = [(1, 2), (2, 0), (0, 1)][dim]
-                visible = (
-                    show_direction[dim1]
-                    and show_direction[dim2]
-                    and show_direction2[dim]
-                )
-                self._translate2_children[dim].visible = visible
+            show_1d_translation[2] = False
+            show_2d_translation[:] = (False, False, True)
 
         # Per-dimension scaling is only possible in object-mode
         if self._mode != "object":
-            for ob in self._scale_children[:3]:
-                ob.visible = False
+            show_1d_scaling[:] = False
+
+        # set the visibility
+        # Note: uniform scale and rotations are always visible
+        for dim in (0, 1, 2):
+            self._translate1_children[dim].visible = show_1d_translation[dim]
+            self._scale_children[dim].visible = show_1d_scaling[dim]
+            self._translate2_children[dim].visible = show_2d_translation[dim]
 
     # %% Event handling
 
     def add_default_event_handlers(self, viewport, camera):
+        """Register Gizmo callbacks."""
+
         # Store objects that we need outside the event handling. In
         # contrast to e.g. a controller, the Gizmo also needs to do
         # some calculation at draw time (or right before a draw, to be
         # precise), and for these calculations it needs the viewport
-        # cand camera.
+        # and camera.
         viewport = Viewport.from_viewport_or_renderer(viewport)
         self._viewport = viewport
         self._camera = camera
 
         self.add_event_handler(
-            self.process_event, "pointer_down", "pointer_move", "pointer_up", "wheel"
+            self.process_event,
+            "pointer_down",
+            "pointer_move",
+            "pointer_up",
+            "wheel",
         )
 
+        viewport.renderer.add_event_handler(self.update_gizmo, "before_render")
+
     def process_event(self, event):
-        """The event handler."""
+        """Callback to handle gizmo-related events."""
 
         # No interaction if there is no object to control
         if not self._object_to_control:
             return
 
         # Triage over event type
         type = event.type
@@ -536,15 +569,15 @@
             elif ob in self._scale_children:
                 self._handle_start("scale", event, ob)
             elif ob in self._rotate_children:
                 self._handle_start("rotate", event, ob)
             # Highlight the object
             self._highlight(ob)
             self._viewport.renderer.request_draw()
-            self.set_pointer_capture(event.pointer_id)
+            self.set_pointer_capture(event.pointer_id, event.root)
 
         elif type == "pointer_up":
             if not self._ref:
                 return
             if self._ref["dim"] is None and self._ref["maxdist"] < 3:
                 self.toggle_mode()  # clicked on the center sphere
             self._ref = None
@@ -569,190 +602,154 @@
             elif self._ref["kind"] == "scale":
                 self._handle_scale_move(event)
             elif self._ref["kind"] == "rotate":
                 self._handle_rotate_move(event)
             # Keep viz up to date
             self._viewport.renderer.request_draw()
 
-    def _handle_start(self, kind, event, ob):
+    def _handle_start(self, kind, event, ob: WorldObject):
         """Initiate a drag. We create a snapshot of the relevant state at this point."""
-        sign = np.sign
-        this_pos = self._object_to_control.position.clone()
-        ob_pos = ob.get_world_position().clone()
+        this_pos = self._object_to_control.world.position
+        ob_pos = ob.world.position
         self._ref = {
             "kind": kind,
-            "event_pos": (event.x, event.y),
+            "event_pos": np.array((event.x, event.y)),
             "dim": ob.dim,
             "maxdist": 0,
             # Transform at time of start
-            "scale": self._object_to_control.scale.clone(),
-            "rot": self._object_to_control.rotation.clone(),
+            "pos": self._object_to_control.world.position,
+            "scale": self._object_to_control.world.scale,
+            "rot": self._object_to_control.world.rotation,
             "world_pos": ob_pos,
-            "world_offset": ob_pos.clone().sub(this_pos),
-            "ndc_pos": ob_pos.clone().project(self._camera),
+            "world_offset": ob_pos - this_pos,
+            "ndc_pos": la.vec_transform(ob_pos, self._camera.camera_matrix),
             # Gizmo direction state at start-time of drag
-            "flips": [sign(self.scale.x), sign(self.scale.y), sign(self.scale.z)],
-            "world_directions": [vec.clone() for vec in self._world_directions],
-            "ndc_directions": [vec.clone() for vec in self._ndc_directions],
-            "screen_directions": [vec.clone() for vec in self._screen_directions],
+            "flips": np.sign(self.world.scale),
+            "world_directions": self._world_directions.copy(),
+            "ndc_directions": self._ndc_directions.copy(),
+            "screen_directions": self._screen_directions.copy(),
         }
 
     def _handle_translate_move(self, event):
         """Translate action, either using a translate1 or translate2 handle."""
-        # Get dimensions to translate in
-        dim = self._ref["dim"]
 
-        # Get how the mouse has moved
-        screen_moved = Vector3(
-            event.x - self._ref["event_pos"][0],
-            event.y - self._ref["event_pos"][1],
-            0,
-        )
-        scene_size = self._viewport.logical_size
-        ndc_moved = screen_moved.clone().multiply(
-            Vector3(2 / scene_size[0], -2 / scene_size[1], 0)
-        )
-
-        # Init new position
-        new_position = self._ref["world_pos"].clone()
-        new_position.sub(self._ref["world_offset"])
-
-        if isinstance(dim, int):
-            # For 1D movement we can project the screen movement to the world-direction.
-            # Sample directions
-            world_dir = self._ref["world_directions"][dim]
-            ndc_dir = self._ref["ndc_directions"][dim].clone()
-            screen_dir = self._ref["screen_directions"][dim].clone()
-            # Calculate how many times the screen_dir matches the moved direction
-            factor = get_scale_factor(screen_dir, screen_moved)
-            # Calculate position by moving ndc_pos in that direction
-            ndc_pos = self._ref["ndc_pos"].clone().add_scaled_vector(ndc_dir, factor)
-            position = ndc_pos.unproject(self._camera)
-            # The found position has roundoff errors, let's align it with the world_dir
-            world_move = position.clone().sub(self._ref["world_pos"])
-            factor = get_scale_factor(world_dir, world_move)
-            new_position.add_scaled_vector(world_move, 1)  # world_dir, factor)
+        world_to_screen = self._ndc_to_screen @ self._camera.camera_matrix
+        screen_to_world = np.linalg.inv(world_to_screen)
+
+        if isinstance(self._ref["dim"], int):
+            travel_directions = (self._ref["dim"],)
         else:
-            # For 2d movement we project the cursor vector onto the plane defined
-            # by the two world directions.
-            dims = dim  # tuple of 2 ints
-            # Get reference world pos and the world vectors. Imagine this a plane.
-            world_pos = self._ref["world_pos"].clone()
-            world_dir1 = self._ref["world_directions"][dims[0]]
-            world_dir2 = self._ref["world_directions"][dims[1]]
-            # Get the line (in world coords) to move things to
-            ndc_pos = self._ref["ndc_pos"].clone()
-            ndc_pos1 = ndc_pos.add_scaled_vector(ndc_moved, 1)
-            ndc_pos2 = ndc_pos1.clone().add(Vector3(0, 0, 1))
-            cursor_world_pos1 = ndc_pos1.unproject(self._camera)
-            cursor_world_pos2 = ndc_pos2.unproject(self._camera)
-            # Get where line intersects plane, expressed in factors of the world dirs
-            factor1, factor2 = get_line_plane_intersection(
-                cursor_world_pos1, cursor_world_pos2, world_pos, world_dir1, world_dir2
+            travel_directions = self._ref["dim"]
+
+        screen_travel = np.array(
+            (
+                event.x - self._ref["event_pos"][0],
+                event.y - self._ref["event_pos"][1],
             )
-            new_position.add_scaled_vector(world_dir1, factor1)
-            new_position.add_scaled_vector(world_dir2, factor2)
+        )
 
-        # Apply
-        self._object_to_control.position = new_position.clone()
-        self.position = new_position.clone()
+        # units dragged along gizmo axes
+        screen_directions = self._ref["screen_directions"][travel_directions, :]
+        if len(screen_directions) == 1:
+            # translate 1D: only count movement along translation axis
+            units_traveled = get_scale_factor(screen_directions[..., :2], screen_travel)
+        else:
+            # translate 2D: change basis from screen to gizmo axes
+            screen_to_axes = np.linalg.inv(screen_directions[..., :2].T)
+            units_traveled = screen_to_axes @ screen_travel
+
+        # pixel units to world units
+        # Note: location of translation matters because perspective cameras have
+        # shear, i.e., we need to account for start
+        start = la.vec_transform(self._ref["world_pos"], world_to_screen)
+        end = start + screen_directions.T @ units_traveled
+        end_world = la.vec_transform(end, screen_to_world)
+        world_units_traveled = end_world - self._ref["world_pos"]
+
+        self._object_to_control.world.position = self._ref["pos"] + world_units_traveled
 
     def _handle_scale_move(self, event):
         """Scale action."""
         # Get dimension
         dim = self._ref["dim"]
 
         # Get how the mouse has moved
-        screen_moved = Vector3(
-            event.x - self._ref["event_pos"][0],
-            event.y - self._ref["event_pos"][1],
-            0,
+        screen_moved = np.array(
+            (
+                event.x - self._ref["event_pos"][0],
+                event.y - self._ref["event_pos"][1],
+                0,
+            )
         )
 
         if dim is None:
             # Uniform scale
-            ref_vec = Vector3(1, -1, 0)
-            npixels = get_scale_factor(ref_vec, screen_moved)
-            scale = 2 ** (npixels / 100)
-            scale = Vector3(scale, scale, scale)
+            ref_vec = np.array((1, -1, 0))
+            factor = get_scale_factor(ref_vec, screen_moved)
+            scale = 2 ** (factor / 100)
+            scale = np.array((scale, scale, scale))
         else:
             # Get how much the mouse has moved in the ref direction
             screen_dir = self._ref["screen_directions"][dim]
             factor = get_scale_factor(screen_dir, screen_moved)
-            factor *= self._ref["flips"][dim]
-            npixels = factor * screen_dir.length()
+
+            # we flip gizmo axis to point towards the user. As a result,
+            # users expect the direction of positive scaling to flip, too
+            is_flipped = self.local.scale[dim] < 0
+            factor *= 1 - 2 * (is_flipped)
+
+            npixels = factor * np.linalg.norm(screen_dir)
             # Calculate the relative scale
             scale = [1, 1, 1]
             scale[dim] = 2 ** (npixels / 100)
-            scale = Vector3(*scale)
+            scale = np.array(scale)
 
         # Apply
-        self._object_to_control.scale = self._ref["scale"].clone().multiply(scale)
+        self._object_to_control.local.scale = scale * self._ref["scale"]
 
     def _handle_rotate_move(self, event):
         """Rotate action."""
-        # Get dimension around which to rotate, and the *other* dimensions
-        dim = self._ref["dim"]
-        dims = [(1, 2), (2, 0), (0, 1)][dim]
 
-        # Get how the mouse has moved
-        screen_moved = Vector3(
-            event.x - self._ref["event_pos"][0],
-            event.y - self._ref["event_pos"][1],
-            0,
-        )
-
-        # Calculate axis of rotation
-        world_dir = self._ref["world_directions"][dim]
-        axis = world_dir.clone().normalize()
-
-        # Calculate the vector between the two arrows that span the arc.
-        # We need to flip the sign in the right places to make this work.
-        screen_dir1 = self._ref["screen_directions"][dims[0]].clone()
-        screen_dir2 = self._ref["screen_directions"][dims[1]].clone()
-        flip1, flip2 = self._ref["flips"][dims[0]], self._ref["flips"][dims[1]]
-        screen_dir1.multiply_scalar(flip1)
-        screen_dir2.multiply_scalar(flip2)
-        screen_vec = screen_dir2.sub(screen_dir1)
-
-        # Now we can calculate how far the mouse moved in *that* direction.
-        factor = get_scale_factor(screen_vec, screen_moved)
-        factor = factor * flip1 * flip2
-        angle = factor * 2
+        local_to_screen = (
+            self._ndc_to_screen @ self._camera.camera_matrix @ self.world.matrix
+        )
+        object_screen = la.vec_transform((0, 0, 0), local_to_screen)[:2]
 
-        # Apply
-        rot = Quaternion().set_from_axis_angle(axis, angle)
-        self._object_to_control.rotation = rot.multiply(self._ref["rot"])
+        # amount of cursor rotation around gizmo origin (CCW is positive)
+        start_direction = self._ref["event_pos"] - object_screen
+        start_angle = np.arctan2(start_direction[1], start_direction[0])
+        current_direction = np.array((event.x, event.y)) - object_screen
+        current_angle = np.arctan2(current_direction[1], current_direction[0])
+        cursor_rotation = current_angle - start_angle
+
+        # axis around which the object rotates
+        dim = self._ref["dim"]
+        world_axis = self._ref["world_directions"][dim]
+
+        # the cursor rotation is measured around the camera's forward direction
+        # (CCW is positive) we need to mirror it if the rotation axis points
+        # points the other way (when CW is positive)
+        ndc_axis = self._ref["ndc_directions"][dim]
+        is_mirrored = 2 * int(ndc_axis[2] > 0) - 1
+        cursor_rotation *= is_mirrored
+
+        initial_rotation = self._ref["rot"]
+        rotation = la.quat_from_axis_angle(world_axis, cursor_rotation)
+        self._object_to_control.world.rotation = la.quat_mul(rotation, initial_rotation)
 
 
 def get_scale_factor(vec1, vec2):
-    """Calculate how many times vec2 fits onto vec1. Basically a dot
-    product and a division by their norms.
     """
-    factor = vec2.clone().normalize().dot(vec1.clone().normalize())
-    factor *= vec2.length() / vec1.length()
-    return factor
-
+    Vector project vec2 onto vec1. Aka, figure out how long vec2
+    is when measured along vec1.
 
-def get_line_plane_intersection(a0, a1, p0, v1, v2):
-    """Get the intersection point of a line onto a plane.
-    Args a0 and a1 represent two points on a line. Arg p0 is a point
-    on a plane, and v1 and v2 two in-plane vectors. The intersection
-    is expressed in factors of v1 and v2.
+    This is used, for example, to work out how many units the cursor has
+    traveled along a given direction.
     """
-    # Get the vector from a0 to a1
-    av = a1.clone().sub(a0)
 
-    # Get how often this vector must be applied from a0 to get to the plane
-    # https://en.wikipedia.org/wiki/Line%E2%80%93plane_intersection
-    n = v1.clone().normalize().cross(v2.clone().normalize())
-    nom = p0.clone().sub(a0).dot(n)
-    denom = av.clone().dot(n)
-    at = nom / denom
-
-    # So the point where the line intersects the plane is ...
-    p1 = a0.clone().add_scaled_vector(av, at)
-
-    # But let's re-express that in a factor of v1 and v2, so that
-    # we really only move in these directions.
-    v3 = p1.clone().sub(p0)
-    return get_scale_factor(v1, v3), get_scale_factor(v2, v3)
+    # Note: implementing it like this saves a couple square-roots from
+    # normalizing
+    return np.sum(vec2 * vec1, axis=-1) / np.sum(vec1**2, axis=-1)
+
+
+def deg_to_rad(degrees):
+    return degrees / 360 * (2 * np.pi)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygfx-0.1.9/pygfx/materials/_background.py` & `pygfx-0.2.0/pygfx/materials/_background.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,50 @@
+from ..resources import Texture
 from ._base import Material
 from ..utils import Color
 
-# todo: in ThreeJS you can simply set a CubeTexture as the scene.background
-# we could do that, and the scene could use these objects automatically.
-# Or just leave it like this. I kinda like it.
-
 
 class BackgroundMaterial(Material):
-    """A background material that draws the background is a uniform color
+    """Solid/Gradient background color.
+
+    A background material that draws the background is a uniform color
     or in a gradient. The positional arguments are passed to ``set_colors()``.
+
+    Parameters
+    ----------
+    colors : list
+        A list of 0, 1, 2, or 4 colors to use in the background. If zero,
+        defaults to monochrome black. If one, the background will be monochrome
+        using the given color. If two, the background will be a gradient from
+        bottom to top using the given colors. If four, the background will be a
+        gradient with each corner set to a different color. The value at a given
+        position is then based on the relative distance of that position to each
+        corner.
+    kwargs : Any
+        Additional kwargs are passed to the base constructor
+        (:class:`pygfx.materials.Material`).
+
     """
 
     uniform_type = dict(
+        Material.uniform_type,
         color_bottom_left="4xf4",
         color_bottom_right="4xf4",
         color_top_left="4xf4",
         color_top_right="4xf4",
     )
 
     def __init__(self, *colors, **kwargs):
         super().__init__(**kwargs)
         self.set_colors(*colors)
 
     def set_colors(self, *colors):
         """Set the background colors. If one color is given, it will be used
         as a uniform color. If two colors are given, it will be used for
-        the botton and top. If four colors are given, it will be used for the
+        the bottom and top. If four colors are given, it will be used for the
         four corners.
         """
         colors = [Color(c) for c in colors]
         if len(colors) == 0:
             self.color_bottom_left = (0, 0, 0, 1)
             self.color_bottom_right = (0, 0, 0, 1)
             self.color_top_left = (0, 0, 0, 1)
@@ -90,25 +105,48 @@
     @color_top_right.setter
     def color_top_right(self, color):
         self.uniform_buffer.data["color_top_right"] = Color(color)
         self.uniform_buffer.update_range(0, 1)
 
 
 class BackgroundImageMaterial(BackgroundMaterial):
-    """A background material that displays an image. If map is a 2D
+    """Image/Skybox background.
+
+    A background material that displays an image. If map is a 2D
     texture view, it is used as a static background. If it is a cube
     texture view, (on a NxMx6 texture) it is used as a skybox.
-    Use the Background object's transform to orient the image.
+
+    Parameters
+    ----------
+    map : Texture
+        If map is a 2D texture, it is used as static background image. If map is
+        a cube texture, it is used as a skybox.
+    kwargs : Any
+        Additional kwargs are passed to the base constructor
+        (:class:`pygfx.materials.Material`).
+
     """
 
     def __init__(self, map=None, **kwargs):
         super().__init__(**kwargs)
         self.map = map
 
     @property
     def map(self):
         """The texture map specifying the background image"""
-        return self._map
+        return self._store.map
 
     @map.setter
     def map(self, map):
-        self._map = map
+        assert map is None or isinstance(map, Texture)
+        self._store.map = map
+
+
+class BackgroundSkyboxMaterial(BackgroundImageMaterial):
+    """Skybox background.
+
+    A cube image background, resulting in a skybox.
+
+    """
+
+    def __init__(self, map=None, **kwargs):
+        super().__init__(map=map, **kwargs)
```

### Comparing `pygfx-0.1.9/pygfx/materials/_mesh.py` & `pygfx-0.2.0/pygfx/geometries/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,283 +1,212 @@
-from ._base import Material
-from ..resources import TextureView
-from ..utils import unpack_bitfield
-from ..utils.color import Color
+import numpy as np
+import pylinalg as la
 
+from ..utils.trackable import Trackable
+from ..resources import Resource, Buffer, Texture
 
-class MeshBasicMaterial(Material):
-    """A material for drawing geometries in a simple shaded (flat or
-    wireframe) way. This material is not affected by lights.
-    """
-
-    uniform_type = dict(
-        color="4xf4",
-        wireframe="f4",
-    )
-
-    def __init__(
-        self,
-        color=(1, 1, 1, 1),
-        vertex_colors=False,
-        map=None,
-        wireframe=False,
-        wireframe_thickness=1,
-        side="BOTH",
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-
-        self.color = color
-        self._vertex_colors = bool(vertex_colors)
-        self.map = map
-        self.wireframe = wireframe
-        self.wireframe_thickness = wireframe_thickness
-        self.side = side
-
-    def _wgpu_get_pick_info(self, pick_value):
-        # This should match with the shader
-        values = unpack_bitfield(
-            pick_value, wobject_id=20, index=26, coord1=6, coord2=6, coord3=6
-        )
-        return {
-            "face_index": values["index"],
-            "face_coord": (
-                values["coord1"] / 64,
-                values["coord2"] / 64,
-                values["coord3"] / 64,
-            ),
-        }
-
-    @property
-    def color(self):
-        """The uniform color of the mesh, as an rgba tuple.
-        This value is ignored if a texture map is used.
-        """
-        return Color(self.uniform_buffer.data["color"])
 
-    @color.setter
-    def color(self, color):
-        color = Color(color)
-        if (color[3] >= 1) != (self.uniform_buffer.data["color"][3] >= 1):
-            self._bump_rev()  # rebuild pipeline if this becomes opaque/transparent
-        self.uniform_buffer.data["color"] = color
-        self.uniform_buffer.update_range(0, 1)
-
-    @property
-    def vertex_colors(self):
-        """Whether to use the vertex colors provided in the geometry."""
-        return self._vertex_colors
-
-    @vertex_colors.setter
-    def vertex_colors(self, value):
-        value = bool(value)
-        if value != self._vertex_colors:
-            self._vertex_colors = value
-            self._bump_rev()
-
-    @property
-    def map(self):
-        """The texture map specifying the color for each texture coordinate.
-        The dimensionality of the map can be 1D, 2D or 3D, but should match the
-        number of columns in the geometry's texcoords.
-        """
-        return self._map
+class Geometry(Trackable):
+    """Generic container for Geometry data.
 
-    @map.setter
-    def map(self, map):
-        assert map is None or isinstance(map, TextureView)
-        self._map = map
-
-    @property
-    def side(self):
-        """Defines which side of faces will be rendered: "FRONT", "BACK", or "BOTH".
-        By default this is "BOTH". Setting to "FRONT" or "BACK" will only render
-        faces from that side, hiding the other. A feature also known as culling.
-
-        Which side of the mesh is the front is determined by the winding of the faces.
-        Counter-clockwise (CCW) winding is assumed. If this is not the case,
-        adjust your geometry (using e.g. ``np.fliplr()`` on ``geometry.indices``).
-        """
-        return self._side
+    Parameters
+    ----------
+    kwargs : dict
+        A dict of attributes to define on the geometry object. Keys must match
+        the naming convention described in the implementation details section of
+        the :mod:`Geometries module <pygfx.geometries>`. If they don't they will
+        become optional attributes. Values must either be `Resources` or
+        ArrayLike.
 
-    @side.setter
-    def side(self, value):
-        side = str(value).upper()
-        if side in ("FRONT", "BACK", "BOTH"):
-            self._side = side
-        else:
-            raise ValueError(f"Unexpected side: '{value}'")
-        self._bump_rev()
+    Example
+    -------
 
-    @property
-    def wireframe(self):
-        """Render geometry as a wireframe. Default is False (i.e. render as polygons)."""
-        return self.uniform_buffer.data["wireframe"] > 0
-
-    @wireframe.setter
-    def wireframe(self, value):
-        is_wiremode = bool(value)
-        was_wiremode = self.uniform_buffer.data["wireframe"] > 0
-        if was_wiremode == is_wiremode:
-            return
-        # Set uniform
-        # We use a trick to make negative values indicate no-wireframe mode
-        thickness = self.wireframe_thickness
-        if is_wiremode:
-            self.uniform_buffer.data["wireframe"] = thickness
-        else:
-            self.uniform_buffer.data["wireframe"] = -thickness
-        # Trigger a pipleine rebuild if the mode changes
-        self.uniform_buffer.update_range(0, 1)
-        self._bump_rev()
-
-    @property
-    def wireframe_thickness(self):
-        """The thickness of the lines when rendering as a wireframe."""
-        return abs(float(self.uniform_buffer.data["wireframe"])) or 1
-
-    @wireframe_thickness.setter
-    def wireframe_thickness(self, value):
-        value = max(0.01, float(value))
-        if self.uniform_buffer.data["wireframe"] > 0:
-            self.uniform_buffer.data["wireframe"] = value
-        else:
-            self.uniform_buffer.data["wireframe"] = -value
-        self.uniform_buffer.update_range(0, 1)
+    .. code-block:: py
 
+        g = Geometry(positions=[[1, 2], [2, 4], [3, 5], [4, 1]])
+        g.positions.data  # numpy array
 
-# todo: MeshLambertMaterial? In ThreeJS this material uses Gouroud shading with the Lambertian light model.
-
-
-class MeshPhongMaterial(MeshBasicMaterial):
-    """A material affected by light, diffuse and with specular
-    highlights. This material uses the Blinn-Phong reflectance model.
-    If the specular color is turned off, Lambertian shading is obtained.
     """
 
-    # For reference:
-    #
-    # Lambertion shading, or Lambertian reflection, is a model to
-    # calculate the diffuse component of a lit surface. Using this by
-    # itself produces a matte look. All the below use a Lambertion term.
-    #
-    # Gouraud shading means doing the light-math in the vertex shader
-    # and interpolating the final color over the face, often resulting
-    # in a somewhat "interpolated" look. Back in the day this mattered
-    # for performance, but it's silly now.
-    #
-    # Phong shading means interpolating the normals and doing the
-    # light-math for each fragment.
-    #
-    # The Phong reflection model refers to the combination of ambient,
-    # diffuse and specular lights, and the way that these are
-    # calculated.
-    #
-    # The Blinn-Phong reflection model, also called the modified Phong
-    # reflection model, is a tweak to how the reflection is calculated,
-    # using a halfway factor, that was intended mostly as a performance
-    # optimization, but apparently is a more accurate approximation of
-    # how light behaves, or so they say.
-    #
-    # Flat shading refers to using the same color for the whole face.
-    # This is what you get if the geometry has indices that do not share
-    # vertices. But we can also obtain it by calculating the face normal
-    # using derivatives of the world pos.
-
-    uniform_type = dict(
-        emissive_color="4xf4",
-        shininess="f4",
-    )
-
-    def __init__(self, shininess=30, emissive=(0, 0, 0, 0), **kwargs):
-        super().__init__(**kwargs)
-        self.emissive = emissive
-        self.shininess = shininess
-
-    @property
-    def emissive(self):
-        """The emissive (light) color of the mesh, as an rgba tuple.
-        This color is added to the final color and is unaffected by lighting.
-        The alpha channel of this color is ignored.
-        """
-        return self.uniform_buffer.data["emissive_color"]
-
-    @emissive.setter
-    def emissive(self, color):
-        self.uniform_buffer.data["emissive_color"] = color
-        self.uniform_buffer.update_range(0, 1)
-
-    @property
-    def shininess(self):
-        """How shiny the specular highlight is; a higher value gives a sharper highlight.
-        Default is 30.
-        """
-        return float(self.uniform_buffer.data["shininess"])
-
-    @shininess.setter
-    def shininess(self, value):
-        self.uniform_buffer.data["shininess"] = value
-        self.uniform_buffer.update_range(0, 1)
-
-
-class MeshFlatMaterial(MeshPhongMaterial):
-    """A material that applies lighting per-face (non-interpolated).
-    This gives a "pixelated" look, but can also be usefull if one wants
-    to show the (size of) the triangle faces. The shading and
-    reflectance model is the same as for ``MeshPhongMaterial``.
-    """
-
-
-# todo: MeshStandardMaterial(MeshBasicMaterial):
-# A standard physically based material, using Metallic-Roughness workflow.
-
-
-# todo: MeshToonMaterial(MeshBasicMaterial):
-# A cartoon-style mesh material.
-
-
-class MeshNormalMaterial(MeshBasicMaterial):
-    """A material that maps the normal vectors to RGB colors."""
-
-
-class MeshNormalLinesMaterial(MeshBasicMaterial):
-    """A material that shows surface normals as lines sticking out of the mesh."""
-
-    def _wgpu_get_pick_info(self, pick_value):
-        return {}  # No picking for normal lines
+    def __init__(self, **kwargs):
+        super().__init__()
 
+        self._aabb = None
+        self._aabb_rev = None
+        self._bsphere = None
+        self._bsphere_rev = None
+
+        for name, val in kwargs.items():
+            # Get resource object
+            if isinstance(val, Resource):
+                resource = val
+            else:
+                # Convert literal arrays to numpy arrays (buffers and textures require memoryview compatible data).
+                if isinstance(val, list):
+                    dtype = "int32" if name == "indices" else "float32"
+                    val = np.array(val, dtype=dtype)
+                # Create texture or buffer
+                if name == "grid":
+                    dim = val.ndim
+                    if dim > 2 and val.shape[-1] <= 4:
+                        dim -= 1  # last array dim is probably (a subset of) rgba
+                    resource = Texture(val, dim=dim)
+                else:
+                    resource = Buffer(val)
+
+            # Checks
+            if isinstance(resource, Buffer):
+                format = resource.format
+                if name == "indices":
+                    # Make no assumptions about shape. Shader will need to validate.
+                    # For meshes will be Nx3 or Nx4, but other dtypes may support
+                    # multidimensional stuff for fancy graphics.
+                    pass
+                elif name == "positions":
+                    if not format.startswith("3x"):
+                        raise ValueError("Expected Nx3 data for positions")
+                elif name == "normals":
+                    if not format.startswith("3x"):
+                        raise ValueError("Expected Nx3 data for normals")
+                elif name == "texcoords":
+                    if not ("x" not in format or format.startswith(("1x", "2x", "3x"))):
+                        raise ValueError("Expected Nx1, Nx2 or Nx3 data for texcoords")
+                elif name == "colors":
+                    if not format.startswith(("3x", "4x")):
+                        raise ValueError("Expected Nx3 or Nx4 data for colors")
+                elif name == "sizes":
+                    if not ("x" not in format):
+                        raise ValueError("Expected array of scalars for sizes")
+                else:
+                    pass  # Unknown attribute - no checks
+
+            # Store
+            setattr(self, name, resource)
+
+    def __setattr__(self, key, new_value):
+        if not key.startswith("_"):
+            if isinstance(new_value, Trackable) or key in self._store:
+                return setattr(self._store, key, new_value)
+        object.__setattr__(self, key, new_value)
+
+    def __getattribute__(self, key):
+        if not key.startswith("_"):
+            if key in self._store:
+                return getattr(self._store, key)
+        return object.__getattribute__(self, key)
+
+    def __dir__(self):
+        x = object.__dir__(self)
+        x.extend(dict.keys(self._store))
+        return x
+
+    def get_bounding_box(self):
+        """Compute the axis-aligned bounding box.
+
+        Computes the aabb based on either positions or the shape of the grid
+        buffer. If both are present, the bounding box will be computed based on
+        the positions buffer.
+
+        Returns
+        -------
+        aabb : ndarray, [2, 3] or None
+            The axis-aligned bounding box given by the "smallest" (lowest value)
+            and "largest" (highest value) corners. Is None when the geometry has
+            no finite positions.
+
+        """
+        if hasattr(self, "positions"):
+            if self._aabb_rev == self.positions.rev:
+                return self._aabb
+            aabb = None
+            # Get positions and check expected shape
+            pos = self.positions.data
+            if pos.ndim == 2 and pos.shape[1] in (2, 3):
+                # Select finite positions
+                finite_mask = np.isfinite(pos).all(axis=1)
+                if finite_mask.sum() > 0:
+                    # Construct aabb
+                    pos_finite = pos[finite_mask]
+                    aabb = np.array(
+                        [pos_finite.min(axis=0), pos_finite.max(axis=0)], np.float32
+                    )
+                    # If positions contains xy, but not z, assume z=0
+                    if aabb.shape[1] == 2:
+                        aabb = np.column_stack([aabb, np.zeros((2, 1), np.float32)])
+            self._aabb = aabb
+            self._aabb_rev = self.positions.rev
+            return self._aabb
+
+        elif hasattr(self, "grid"):
+            if self._aabb_rev == self.grid.rev:
+                return self._aabb
+            # account for multi-channel image data
+            grid_shape = self.grid.data.shape[: self.grid.dim]
+            # create aabb in index/data space
+            aabb = np.array([np.zeros_like(grid_shape), grid_shape[::-1]], dtype="f8")
+            # convert to local image space by aligning
+            # center of voxel index (0, 0, 0) with origin (0, 0, 0)
+            aabb -= 0.5
+            # ensure coordinates are 3D
+            # NOTE: important we do this last, we don't want to apply
+            # the -0.5 offset to the z-coordinate of 2D images
+            if aabb.shape[1] == 2:
+                aabb = np.hstack([aabb, [[0], [0]]])
+            self._aabb = aabb
+            self._aabb_rev = self.grid.rev
+            return self._aabb
+        else:
+            return None
 
-class MeshSliceMaterial(MeshBasicMaterial):
-    """A material that displays a slice of the mesh."""
+    def get_bounding_sphere(self):
+        """Compute a bounding sphere.
 
-    uniform_type = dict(
-        plane="4xf4",
-        thickness="f4",
-    )
+        Uses the geometry's axis-aligned bounding box, to estimate a sphere
+        which contains the geometry.
 
-    def __init__(self, plane=(0, 0, 1, 0), thickness=2.0, **kwargs):
-        super().__init__(**kwargs)
-        self.plane = plane
-        self.thickness = thickness
+        Returns
+        -------
+        sphere : ndarray, [4] or None
+            A sphere given by it's center and radius. Format: ``(x, y, z, radius)``.
+            Is None when the geometry has no finite positions.
+
+        Notes
+        -----
+        Since the sphere wraps the geometry's bounding box, it typically won't
+        be the minimally binding sphere.
 
-    @property
-    def plane(self):
-        """The plane to slice at, represented with 4 floats ``(a, b, c, d)``,
-        which make up the equation: ``ax + by + cz + d = 0`` The plane
-        definition applies to the world space (of the scene).
         """
-        return self.uniform_buffer.data["plane"]
 
-    @plane.setter
-    def plane(self, plane):
-        self.uniform_buffer.data["plane"] = plane
-        self.uniform_buffer.update_range(0, 1)
-
-    @property
-    def thickness(self):
-        """The thickness of the line to draw the edge of the mesh."""
-        return self.uniform_buffer.data["thickness"]
-
-    @thickness.setter
-    def thickness(self, thickness):
-        self.uniform_buffer.data["thickness"] = thickness
-        self.uniform_buffer.update_range(0, 1)
+        if hasattr(self, "positions"):
+            if self._bsphere_rev == self.positions.rev:
+                return self._bsphere
+            bsphere = None
+            # Get positions and check expected shape
+            pos = self.positions.data
+            if pos.ndim == 2 and pos.shape[1] in (2, 3):
+                # Select finite positions
+                finite_mask = np.isfinite(pos).all(axis=1)
+                if finite_mask.sum() > 0:
+                    # Construct aabb
+                    pos_finite = pos[finite_mask]
+                    center = pos_finite.mean(axis=0)
+                    distances = np.linalg.norm(pos_finite - center, axis=0)
+                    radius = float(distances.max())
+                    if len(center) == 2:
+                        bsphere = np.array(
+                            [center[0], center[1], 0.0, radius], np.float32
+                        )
+                    else:
+                        bsphere = np.array(
+                            [center[0], center[1], center[1], radius], np.float32
+                        )
+            self._bsphere = bsphere
+            self._bsphere_rev = self.positions.rev
+            return self._bsphere
+
+        else:
+            if self._bsphere_rev == self._aabb_rev:
+                return self._bsphere
+            aabb = self.get_bounding_box()
+            self._bsphere = None if aabb is None else la.aabb_to_sphere(aabb)
+            self._bsphere_rev = self._aabb_rev
+            return self._bsphere
```

### Comparing `pygfx-0.1.9/pygfx/objects/_base.py` & `pygfx-0.2.0/pygfx/utils/text/_atlas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,451 +1,429 @@
-import random
-import weakref
 import threading
 
 import numpy as np
 
-from ._events import EventTarget
-from ..linalg import Vector3, Matrix4, Quaternion
-from ..linalg.utils import transform_aabb, aabb_to_sphere
-from ..resources import Resource, Buffer
-from ..utils import array_from_shadertype
+from ...resources import Texture, Buffer
 
 
-class IdProvider:
-    """Object for internal use to manage world object id's."""
-
-    def __init__(self):
-        self._ids_in_use = set([0])
-        self._map = weakref.WeakValueDictionary()
-        self._lock = threading.RLock()
-
-    def claim_id(self, wobject):
-        """Used by wobjects to claim an id."""
-        # We don't simply count up, but keep a pool of ids. This is
-        # because an application *could* create and discard objects at
-        # a high rate, so we want to be able to re-use these ids.
-        #
-        # Some numbers:
-        # * 4_294_967_296 (2**32) max number for u32
-        # * 2_147_483_647 (2**31 -1) max number for i32.
-        # *    16_777_216 max integer that can be stored exactly in f32
-        # *     4_000_000 max integer that survives being passed as a varying (in my tests)
-        # *     1_048_575 is ~1M is 2**20 seems like a good max scene objects.
-        # *    67_108_864 is ~50M is 2**26 seems like a good max vertex count.
-        #                 which leaves 64-20-26=18 bits for any other picking info.
-
-        # Max allowed id, inclusive
-        id_max = 1_048_575  # 2*20-1
-
-        # The max number of ids. This is a bit less to avoid choking
-        # when there are few free id's left.
-        max_items = 1_000_000
-
-        with self._lock:
-            if len(self._ids_in_use) >= max_items:
-                raise RuntimeError("Max number of objects reached.")
-            id = 0
-            while id in self._ids_in_use:
-                id = random.randint(1, id_max)
-            self._ids_in_use.add(id)
-            self._map[id] = wobject
-
-        return id
-
-    def release_id(self, wobject, id):
-        """Release an id associated with a wobject."""
-        with self._lock:
-            self._ids_in_use.discard(id)
-            self._map.pop(id, None)
+def generate_size_table(max_size=8192):
+    # 8192 is the default wgpu max texture size
+    size = 0
+    ref_area = 256
+    while size < max_size:
+        while size * size < ref_area:
+            size += 8
+        size = min(size, max_size)
+        yield (size, size * size, ref_area)
+        ref_area *= 2
+
+
+# A table of predefined atlas sizes, resulting in ± factor-of-two increasing area.
+# Each item in the table is a tuple (size, area, ref_area).
+# Sizes are rounded to multiples of 8.
+SIZES = list(generate_size_table())
+
+
+def get_suitable_size(approximate_area):
+    """Get the atlas size such that it has about the given area."""
+    for i in range(1, len(SIZES)):
+        size2, area2, _ = SIZES[i]
+        if area2 >= approximate_area:
+            size1, area1, _ = SIZES[i - 1]
+            diff1 = np.abs(area1 - approximate_area)
+            diff2 = np.abs(area2 - approximate_area)
+            return size1 if diff1 < diff2 else size2
+    else:
+        return SIZES[-1][0]
 
-    def get_object_from_id(self, id):
-        """Return the wobject associated with an id, or None."""
-        return self._map.get(id)
 
+class RectPacker:
+    """
+    This Python code was copied from the Vispy project.
+    The algorithm is based on the article by Jukka Jylänki : "A Thousand Ways
+    to Pack the Bin - A Practical Approach to Two-Dimensional Rectangle Bin
+    Packing", February 27, 2010. More precisely, this is an implementation of
+    the Skyline Bottom-Left algorithm based on C++ sources provided by Jukka
+    Jylänki at: http://clb.demon.fi/files/RectangleBinPack/.
+    """
 
-id_provider = IdProvider()
-
-
-class ResourceContainer:
-    """Base class for WorldObject, Geometry and Material."""
-
-    def __init__(self):
-        self._resource_parents = weakref.WeakSet()
-        self._rev = 0
-
-    @property
-    def rev(self):
-        """Monotonically increasing integer that gets bumped when any
-        of its buffers or textures are set. (Not when updates are made
-        to these resources themselves).
+    # Note: this could be extended to keep track of waste-space in a
+    # separate data structure (a.k.a. waste map improvement). Similarly,
+    # we could track freed regions for re-use. Right now we keep things
+    # simple, and repack to re-claim freed regions.
+
+    def _reset_packer(self):
+        self._atlas_nodes = [(0, 0, self._array.shape[1])]
+
+    def _select_region(self, width, height):
+        """Find a free region of given size and allocate it.
+        Returns the newly allocated region as (x, y, w, h), or None on failure.
         """
-        return self._rev
-
-    # NOTE: we could similarly let bumping of a resource's rev bump a
-    # data_rev here. But it is not clear whether the (minor?) increase
-    # in performance is worth the added complexity.
-
-    def _bump_rev(self):
-        """Bump the rev (and that of any "resource parents"), to trigger a pipeline rebuild."""
-        self._rev += 1
-        for x in self._resource_parents:
-            x._rev += 1
-
-    def __setattr__(self, name, value):
-        super().__setattr__(name, value)
-        if isinstance(value, ResourceContainer):
-            value._resource_parents.add(self)
-            self._bump_rev()
-        elif isinstance(value, Resource):
-            self._bump_rev()
-
-
-class WorldObject(EventTarget, ResourceContainer):
-    """The base class for objects present in the "world", i.e. the scene graph.
-
-    Each WorldObject has geometry to define it's data, and material to define
-    its appearance. The object itself is only responsible for defining object
-    hierarchies (parent / children) and its position and orientation in the world.
 
-    This is considered a base class. Use Group to collect multiple world objects
-    into a single empty world object.
-    """
+        # Find best place to fit it
+        best_height = best_width = np.inf
+        best_index = -1
+        for i in range(len(self._atlas_nodes)):
+            y = self._fit_region(i, width, height)
+            if y >= 0:
+                node = self._atlas_nodes[i]
+                if y + height < best_height or (
+                    y + height == best_height and node[2] < best_width
+                ):
+                    best_height = y + height
+                    best_index = i
+                    best_width = node[2]
+                    region = node[0], y, width, height
+        if best_index == -1:
+            return None
+
+        # Create the node and update the data structure
+        node = region[0], region[1] + height, width
+        self._atlas_nodes.insert(best_index, node)
+        i = best_index + 1
+        while i < len(self._atlas_nodes):
+            node = self._atlas_nodes[i]
+            prev_node = self._atlas_nodes[i - 1]
+            if node[0] < prev_node[0] + prev_node[2]:
+                shrink = prev_node[0] + prev_node[2] - node[0]
+                x, y, w = self._atlas_nodes[i]
+                self._atlas_nodes[i] = x + shrink, y, w - shrink
+                if self._atlas_nodes[i][2] <= 0:
+                    del self._atlas_nodes[i]
+                    i -= 1
+                else:
+                    break
+            else:
+                break
+            i += 1
 
-    # The uniform type describes the structured info for this object, which represents
-    # every "propery" that a renderer would need to know in order to visualize it.
-    # Put larger items first for alignment, also note that host-sharable structs
-    # align at power-of-two only, so e.g. vec3 needs padding.
-    # todo: rename uniform to info or something?
-
-    uniform_type = dict(
-        world_transform="4x4xf4",
-        world_transform_inv="4x4xf4",
-        id="i4",
-    )
-
-    _v = Vector3()
-    _m = Matrix4()
-    _q = Quaternion()
-
-    def __init__(
-        self,
-        geometry=None,
-        material=None,
-        *,
-        visible=True,
-        render_order=0,
-        render_mask="auto",
-    ):
-        super().__init__()
-
-        self.geometry = geometry
-        self.material = material
-
-        # Init visibility and render props
-        self.visible = visible
-        self.render_order = render_order
-        self.render_mask = render_mask
-
-        # Init parent and children
-        self._parent_ref = None
-        self._children = []
-
-        self.position = Vector3()
-        self.rotation = Quaternion()
-        self.scale = Vector3(1, 1, 1)
-        self._transform_hash = ()
-
-        self.up = Vector3(0, 1, 0)
-
-        self._matrix = Matrix4()
-        self._matrix_auto_update = True
-        self._matrix_world = Matrix4()
-        self._matrix_world_dirty = True
-
-        # Compose complete uniform type
-        self.uniform_type = {}
-        for cls in reversed(self.__class__.mro()):
-            self.uniform_type.update(getattr(cls, "uniform_type", {}))
-        self.uniform_buffer = Buffer(array_from_shadertype(self.uniform_type))
-
-        # Set id
-        self._id = id_provider.claim_id(self)
-        self.uniform_buffer.data["id"] = self._id
+        # Merge nodes
+        i = 0
+        while i < len(self._atlas_nodes) - 1:
+            node = self._atlas_nodes[i]
+            next_node = self._atlas_nodes[i + 1]
+            if node[1] == next_node[1]:
+                self._atlas_nodes[i] = node[0], node[1], node[2] + next_node[2]
+                del self._atlas_nodes[i + 1]
+            else:
+                i += 1
 
-    def __del__(self):
-        id_provider.release_id(self, self.id)
+        return region
 
-    @property
-    def id(self):
-        """An integer id smaller than 2**31 (read-only)."""
-        return self._id
+    def _fit_region(self, index, width, height):
+        """Test if region (width, height) fit into self._atlas_nodes[index].
+        Returns y on success, or -1 on failure."""
+        node = self._atlas_nodes[index]
+        x, y = node[0], node[1]
+        shape = self._array.shape
+        width_left = width
+        if x + width > shape[1]:
+            return -1
+        i = index
+        while width_left > 0:
+            node = self._atlas_nodes[i]
+            y = max(y, node[1])
+            if y + height > shape[0]:
+                return -1
+            width_left -= node[2]
+            i += 1
+        return y
+
+
+class GlyphAtlas(RectPacker):
+    """A global atlas for glyphs (thread-safe).
+
+    This object allows allocating regions, which are packed into a large
+    internal array. When the internal array is full, it is resized and
+    repacked. This means that packed regions are moved to a new location
+    (defragmentation). Therefore the actual location must be looked up
+    via the infos array. The internal array is also reduced when the
+    capacity is much larger than needed.
+    """
 
-    @property
-    def visible(self):
-        """Wheter is object is rendered or not. Default True."""
-        return self._visible
-
-    @visible.setter
-    def visible(self, visible):
-        self._visible = bool(visible)
+    def __init__(self, initial_infos_size=1024, initial_array_size=1024):
+        self._lock = threading.RLock()
 
-    @property
-    def render_order(self):
-        """This value allows the default rendering order of scene graph
-        objects to be controlled. Default 0. See ``Renderer.sort_objects``
-        for details.
+        # Keep track of the index for each glyph
+        self._hash2index = {}  # hash -> index
+        self._index2hash = {}
+
+        # Indices monotonically increase, but can also be reused from freed regions
+        self._index_counter = 0
+        self._free_indices = set()
+
+        # Stats
+        # The allocated_area represents the sum of areas that the packer has allocated,
+        # not including the areas of freed regions. The free_area consists of regions
+        # that were once allocated. The waste space in the atlas due to inefficient
+        # packing is not counted.
+        self._region_count = 0
+        self._allocated_area = 0
+        self._free_area = 0
+
+        # Props to influence the behavior
+        self.clear_free_regions = False
+        self.downscale_ratio = 0.25
+
+        # The per-glyph information (used in the shader)
+        self._info_dtype = [
+            ("origin", np.int32, 2),
+            ("size", np.int32, 2),
+            ("offset", np.float32, 2),
+        ]
+
+        # Init arrays
+        self._infos = self._array = np.zeros((0,), np.void)
+        self._initial_array_size = get_suitable_size(initial_array_size**2)
+        self._set_new_infos_array(initial_infos_size)
+        self._set_new_glyphs_array(self._initial_array_size)
+
+    @property
+    def region_count(self):
+        """The number of regions allocated (excluding freed)."""
+        return self._region_count
+
+    @property
+    def total_area(self):
+        """The total area that the atlas could potentially hold."""
+        shape = self._array.shape
+        return shape[1] * shape[0]
+
+    @property
+    def allocated_area(self):
+        """The allocated area (excluding the area of freed regions)."""
+        return self._allocated_area
+
+    def _set_new_infos_array(self, size):
+        """Create a new array to store per-glyph info."""
+        assert size > 0 and size > self._infos.shape[0]
+
+        # Allocate new infos array
+        infos1 = self._infos
+        infos2 = np.zeros((size,), self._info_dtype)
+        self._infos = infos2
+
+        # Make a copy
+        infos2[: infos1.shape[0]] = infos1
+
+    def _set_new_glyphs_array(self, size):
+        """Pack all glyphs up in a new array. If the size is unchanged,
+        repacks the glyphs in the current array.
         """
-        return self._render_order
-
-    @render_order.setter
-    def render_order(self, value):
-        self._render_order = float(value)
+        assert size > 0
 
-    @property
-    def render_mask(self):
-        """Indicates in what render passes to render this object:
-
-        * "auto": try to determine the best approach (default).
-        * "opaque": only in the opaque render pass.
-        * "transparent": only in the transparent render pass(es).
-        * "all": render in both opaque and transparent render passses.
-
-        If "auto" (the default), the renderer attempts to determine
-        whether all fragments will be either opaque or all transparent,
-        and only apply the needed render passes. If this cannot be
-        determined, it falls back to "all".
-
-        Some objects may contain both transparent and opaque fragments,
-        and should be rendered in all passes - the object's contribution
-        to each pass is determined on a per-fragment basis.
-
-        For clarity, rendering objects in all passes even though they
-        are fully opaque/transparent yields correct results and is
-        generally the "safest" option. The only cost is performance.
-        Rendering transparent fragments in the opaque pass makes them
-        invisible. Rendering opaque fragments in the transparent pass
-        blends them as if they are transparent with an alpha of 1.
+        if size == self._array.shape[0]:
+            # Keep the array, we'll repack only
+            array1 = self._array.copy()
+            array2 = self._array
+            array2.fill(0)
+        else:
+            # Create new array
+            array1 = self._array
+            array2 = np.zeros((size, size), np.uint8)
+            self._array = array2
+
+        # We're going to pack it up fresh
+        self._reset_packer()
+
+        # Copy all rect regions to their new location
+        allocated_area = 0
+        for index in range(self._index_counter):
+            info = self._infos[index]
+            x1, y1 = info["origin"]
+            w1, h1 = info["size"]
+            if not w1 or not h1:
+                continue  # freed region
+            x2, y2, w2, h2 = self._select_region(w1, h1)
+            info["origin"] = x2, y2
+            array2[y2 : y2 + h2, x2 : x2 + w2] = array1[y1 : y1 + h1, x1 : x1 + w1]
+            allocated_area += w2 * h2
+
+        assert allocated_area == self._allocated_area
+
+        self._free_area = 0
+        self._allocated_area = allocated_area
+        self._free_indices.clear()
+
+    def allocate_region(self, w, h):
+        """Allocate a region of the given size. Returns the index for
+        the new region. The internal array may be repacked and/or
+        resized if necessary.
         """
-        return self._render_mask
-
-    @render_mask.setter
-    def render_mask(self, value):
-        value = "auto" if value is None else value
-        assert isinstance(value, str), "render_mask should be string"
-        value = value.lower()
-        options = ("opaque", "transparent", "auto", "all")
-        if value not in options:
-            raise ValueError(
-                f"WorldObject.render_mask must be one of {options} not {value!r}"
-            )
-        self._render_mask = value
-        # Trigger a pipeline redraw, because this info is used in that code path
-        self._bump_rev()
+        with self._lock:
+            # Select a region
+            rect = self._select_region(w, h)
 
-    @property
-    def geometry(self):
-        """The object's geometry, the data that defines (the shape of) this object."""
-        return self._geometry
-
-    @geometry.setter
-    def geometry(self, geometry):
-        self._geometry = geometry
+            # If the array is full the above returns None. If so, resize and try again.
+            if rect is None:
+                # If one third or more is empty, we repack only
+                if self._free_area and self._free_area >= 0.5 * self._allocated_area:
+                    self._set_new_glyphs_array(self._array.shape[0])
+                    rect = self._select_region(w, h)
+                # Increase size until we have enough space. Note that the requested
+                # region might simply require more than double the original size.
+                new_size = 0
+                while rect is None:
+                    new_size = get_suitable_size(self.total_area * 2)
+                    if new_size**2 == self.total_area:
+                        # You'd have to stretch things *a lot*, but this can happen in theory
+                        raise RuntimeError(
+                            "Glyph atlas is out of space and cannot be larger."
+                        )
+                    self._set_new_glyphs_array(new_size)
+                    rect = self._select_region(w, h)
+
+            # Select an index
+            if self._free_indices:
+                # Reuse an index that was previously freed.
+                # Note that we only re-use the index (and thus the slot in the infos array),
+                # but not the slot in the glyph array. Therefore _free_area does not change.
+                index = self._free_indices.pop()
+            else:
+                # Create a new index
+                index = self._index_counter
+                self._index_counter += 1
+                # Make sure that the per-glyph arrays are large enough
+                while index >= self._infos.shape[0]:
+                    self._set_new_infos_array(self._infos.shape[0] * 2)
+
+            # Store the rectangle
+            info = self._infos[index]
+            info["origin"] = rect[:2]
+            info["size"] = rect[2:]
+            info["offset"] = 0, 0  # set to zero just in case
+
+            # Bookkeeping
+            self._region_count += 1
+            self._allocated_area += w * h
 
-    @property
-    def material(self):
-        """Wheter is object is rendered or not. Default True."""
-        return self._material
-
-    @material.setter
-    def material(self, material):
-        self._material = material
+            return index
 
-    @property
-    def parent(self):
-        """Object's parent in the scene graph (read-only).
-        An object can have at most one parent.
-        """
-        return self._parent_ref and self._parent_ref()
+    def set_region(self, index, region):
+        """Set the region data for index."""
+        with self._lock:
+            info = self._infos[index]
+            x, y = info["origin"]
+            w, h = info["size"]
+            self._array[y : y + h, x : x + w] = region
 
-    @property
-    def children(self):
-        """The child objects of this wold object (read-only tuple).
-        Use ``.add()`` and ``.remove()`` to change this list.
-        """
-        return tuple(self._children)
+    def get_region(self, index):
+        """Return a copy of the region corresponding to index."""
+        with self._lock:
+            info = self._infos[index]
+            x, y = info["origin"]
+            w, h = info["size"]
+            return self._array[y : y + h, x : x + w].copy()
 
-    def add(self, *objects, before=None):
-        """Adds object as child of this object. Any number of
-        objects may be added. Any current parent on an object passed
-        in here will be removed, since an object can have at most one
-        parent.
-        If ``before`` argument is given (and present in children), then
-        the items are inserted before the given element.
-        """
-        idx = len(self._children)
-        if before:
-            try:
-                idx = self._children.index(before)
-            except ValueError:
-                pass
-        for obj in objects:
-            # orphan if needed
-            if obj._parent_ref is not None:
-                obj._parent_ref().remove(obj)
-            # attach to scene graph
-            obj._parent_ref = weakref.ref(self)
-            self._children.insert(idx, obj)
-            idx += 1
-            # flag world matrix as dirty
-            obj._matrix_world_dirty = True
-        return self
-
-    def remove(self, *objects):
-        """Removes object as child of this object. Any number of objects may be removed.
-        If a given object is not a child, it is ignored.
-        """
-        for obj in objects:
+    def get_index_from_hash(self, hash):
+        """Get the glyph index from the hash, or None on failure."""
+        with self._lock:
             try:
-                self._children.remove(obj)
-                obj._parent_ref = None
-            except ValueError:
-                pass
-        return self
-
-    def traverse(self, callback, skip_invisible=False):
-        """Executes the callback on this object and all descendants.
-
-        If ``skip_invisible`` is given and True, objects whose
-        ``visible`` property is False - and their children - are
-        skipped. Note that modifying the scene graph inside the callback
-        is discouraged.
+                return self._hash2index[hash]
+            except KeyError:
+                return None
+
+    def store_region_with_hash(self, hash, region, offset=(0, 0)):
+        """Set the region corresponding to the given hash, and return the index."""
+        with self._lock:
+            # Sanitize
+            assert isinstance(region, np.ndarray)
+            assert hash not in self._hash2index
+
+            # Reserve a slot
+            w, h = region.shape[1], region.shape[0]
+            index = self.allocate_region(w, h)
+
+            # Store
+            self.set_region(index, region)
+            self._infos[index]["offset"] = offset
+
+            # Bookkeeping
+            self._hash2index[hash] = index
+            self._index2hash[index] = hash
+
+            return index
+
+    def free_region(self, index):
+        """Free up a region slot."""
+        # We mask the index to only use the first 24 bits. In pygfx we use
+        # the upper 8 bits to store font-prop info for the shader.
+        index = int(index) & 0x0FFF
+        with self._lock:
+            # Zero out the region data
+            if self.clear_free_regions:
+                self.set_region(index, 0)
+            # Free in data structure
+            assert index < self._index_counter, "Invalid index to free"
+            info = self._infos[index]
+            x, y = info["origin"]
+            w, h = info["size"]
+            info["size"] = 0, 0
+            self._free_indices.add(index)
+            # Bookkeeping
+            self._region_count -= 1
+            self._free_area += w * h
+            self._allocated_area -= w * h
+            # Clear hash data
+            hash = self._index2hash.pop(index, None)
+            if hash is not None:
+                self._hash2index.pop(hash)
+            # Reduce size?
+            if self.downscale_ratio:
+                total_area = self._allocated_area + self._free_area
+                if self._allocated_area <= self.downscale_ratio * total_area:
+                    current_size = self._array.shape[0]
+                    if current_size > self._initial_array_size:
+                        new_size = get_suitable_size(self.total_area / 2)
+                        new_size = max(new_size, self._initial_array_size)
+                        if new_size != current_size:
+                            self._set_new_glyphs_array(new_size)
+
+
+class PygfxGlyphAtlas(GlyphAtlas):
+    """A textured pygfx-specific subclass of the GlyphAtlas."""
+
+    @property
+    def texture(self):
+        """The texture for the atlas. The Shared object exposes this object
+        in a trackable way.
         """
-        if skip_invisible and not self._visible:
-            return
-        callback(self)
-        for child in self._children:
-            child.traverse(callback, skip_invisible)
-
-    def update_matrix(self):
-        p, r, s = self.position, self.rotation, self.scale
-        hash = p.x, p.y, p.z, r.x, r.y, r.z, r.w, s.x, s.y, s.z
-        if hash != self._transform_hash:
-            self._transform_hash = hash
-            self._matrix.compose(self.position, self.rotation, self.scale)
-            self._matrix_world_dirty = True
+        return self._texture
 
     @property
-    def matrix(self):
-        """The (settable) transformation matrix."""
-        return self._matrix
-
-    @matrix.setter
-    def matrix(self, matrix):
-        self._matrix.copy(matrix)
-        self._matrix.decompose(self.position, self.rotation, self.scale)
-        self._matrix_world_dirty = True
+    def info_buffer(self):
+        """A buffer containing the info for the glyphs (origin, size, offset)."""
+        return self._infos_buffer
+
+    def _set_new_glyphs_array(self, *args):
+        # Do the normal behavior
+        array = self._array
+        super()._set_new_glyphs_array(*args)
+        # Create resource object if needed
+        if self._array is not array:
+            self._texture = Texture(self._array, dim=2)
+        # Schedule an update. Note that the infos array is updated due to repacking.
+        w, h = self._array.shape[1], self._array.shape[0]
+        self._texture.update_range((0, 0, 0), (w, h, 1))
+        self._infos_buffer.update_range(0, self._infos.shape[0])
+
+    def _set_new_infos_array(self, *args):
+        # Do the normal behavior
+        infos = self._infos
+        super()._set_new_infos_array(*args)
+        # Create resource object if needed
+        if self._infos is not infos:
+            self._infos_buffer = Buffer(self._infos)
+        # Schedule an update
+        self._infos_buffer.update_range(0, self._infos.shape[0])
 
-    @property
-    def matrix_world(self):
-        """The world matrix (local matrix composed with any parent matrices)."""
-        return self._matrix_world
+    def set_region(self, index, glyph):
+        with self._lock:
+            super().set_region(index, glyph)
+            info = self._infos[index]
+            x, y = info["origin"]
+            w, h = info["size"]
+            self._texture.update_range((x, y, 0), (w, h, 1))
+            self._infos_buffer.update_range(index, index + 1)
 
-    @property
-    def matrix_auto_update(self):
-        """Whether or not the matrix auto-updates."""
-        return self._matrix_auto_update
-
-    @matrix_auto_update.setter
-    def matrix_auto_update(self, value):
-        self._matrix_auto_update = bool(value)
 
-    @property
-    def matrix_world_dirty(self):
-        """Whether or not the matrix needs updating (readonly)."""
-        return self._matrix_world_dirty
-
-    def apply_matrix(self, matrix):
-        if self._matrix_auto_update:
-            self.update_matrix()
-        self._matrix.premultiply(matrix)
-        self._matrix.decompose(self.position, self.rotation, self.scale)
-        self._matrix_world_dirty = True
-
-    def update_matrix_world(
-        self, force=False, update_children=True, update_parents=False
-    ):
-        if update_parents and self.parent:
-            self.parent.update_matrix_world(
-                force=force, update_children=False, update_parents=True
-            )
-        if self._matrix_auto_update:
-            self.update_matrix()
-        if self._matrix_world_dirty or force:
-            if self.parent is None:
-                self._matrix_world.copy(self._matrix)
-            else:
-                self._matrix_world.multiply_matrices(
-                    self.parent._matrix_world, self._matrix
-                )
-            self.uniform_buffer.data[
-                "world_transform"
-            ].flat = self._matrix_world.elements
-            tmp_inv_matrix = Matrix4().get_inverse(self._matrix_world)
-            self.uniform_buffer.data[
-                "world_transform_inv"
-            ].flat = tmp_inv_matrix.elements
-            self.uniform_buffer.update_range(0, 1)
-            self._matrix_world_dirty = False
-            for child in self._children:
-                child._matrix_world_dirty = True
-        if update_children:
-            for child in self._children:
-                child.update_matrix_world()
-
-    def look_at(self, target: Vector3):
-        self.update_matrix_world(update_parents=True, update_children=False)
-        self._v.set_from_matrix_position(self._matrix_world)
-        self._m.look_at(self._v, target, self.up)
-        self.rotation.set_from_rotation_matrix(self._m)
-        if self.parent:
-            self._m.extract_rotation(self.parent._matrix_world)
-            self._q.set_from_rotation_matrix(self._m)
-            self.rotation.premultiply(self._q.inverse())
-
-    def get_world_position(self):
-        self.update_matrix_world(update_parents=True, update_children=False)
-        self._v.set_from_matrix_position(self._matrix_world)
-        return self._v.clone()
-
-    def get_world_bounding_box(self):
-        self.update_matrix_world(update_parents=True, update_children=True)
-        return self._get_world_bounding_box()
-
-    def _get_world_bounding_box(self):
-        boxes = []
-        if self._geometry:
-            aabb = self._geometry.bounding_box()
-            aabb_world = transform_aabb(aabb, self._matrix_world.to_ndarray())
-            boxes.append(aabb_world)
-        if self._children:
-            boxes.extend(
-                [
-                    b
-                    for b in (c.get_world_bounding_box() for c in self._children)
-                    if b is not None
-                ]
-            )
-        if len(boxes) == 1:
-            return boxes[0]
-        if boxes:
-            boxes = np.array(boxes)
-            return np.array([boxes[:, 0].min(axis=0), boxes[:, 1].max(axis=0)])
-
-    def get_world_bounding_sphere(self):
-        aabb = self.get_world_bounding_box()
-        if aabb is not None:
-            return aabb_to_sphere(aabb)
-
-    def _wgpu_get_pick_info(self, pick_value):
-        # In most cases the material handles this.
-        return self.material._wgpu_get_pick_info(pick_value)
+glyph_atlas = PygfxGlyphAtlas()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygfx-0.1.9/pygfx/objects/_events.py` & `pygfx-0.2.0/pygfx/objects/_events.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 from enum import Enum
 from time import perf_counter_ns
 from typing import Union
-from weakref import ref, WeakValueDictionary
+from weakref import ref
 
 from wgpu.gui.base import log_exception
 
 
 CLICK_DEBOUNCE = 500  # in milliseconds
 
 
@@ -26,22 +26,41 @@
     WHEEL = "wheel"
     # Window
     CLOSE = "close"
     RESIZE = "resize"
 
 
 class Event:
-    """Event base class for creating events.
+    """Event base class.
 
     If a target is set, an event can bubble up through a hierarchy
     of targets, connected through a ``parent`` property.
     To prevent an event from bubbling up, use ``stop_propagation``.
 
     It is also possible to cancel events, which will stop any further
     handling of the event (also by the same target).
+
+    Parameters
+    ----------
+    type : Union[str, EventType]
+        The name of the event.
+    bubbles : bool
+        If True, the event bubbles up through the scene tree.
+    target : EventTarget
+        The object onto which the event was dispatched.
+    root : RootEventHandler
+        A reference to the root event handler.
+    time_stamp : float
+        The time at which the event was created (in ms). Might not be an actual
+        time stamp so please only use this for relative time measurements.
+    cancelled : bool
+        A boolean value indicating whether the event is cancelled.
+    event_type : str
+        Unused.
+
     """
 
     def __init__(
         self,
         type: Union[str, EventType],
         *,
         bubbles=True,
@@ -114,21 +133,77 @@
         self._update_current_target(target)
 
     def _update_current_target(self, target):
         self._current_target = target
 
 
 class KeyboardEvent(Event):
+    """Keyboard button press.
+
+    Parameters
+    ----------
+    args : Any
+        Positional arguments are forwarded to the :class:`base class
+        <pygfx.objects.Event>`.
+    key : str
+        The key that was pressed.
+    modifiers : list
+        The modifiers that were pressed while the key was pressed.
+    kwargs : Any
+        Additional keyword arguments are forward to the :class:`base class
+        <pygfx.objects.Event>`.
+
+    """
+
     def __init__(self, *args, key, modifiers=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.key = key
         self.modifiers = modifiers or ()
 
 
 class PointerEvent(Event):
+    """Mouse/Touch Event.
+
+    Parameters
+    ----------
+    args : Any
+        Positional arguments are forwarded to the :class:`base class
+        <pygfx.objects.Event>`.
+    x : int
+        The x position of the cursor or touch in screen space (px).
+    y : int
+        Thy y position of the cursor or touch in screen space (px).
+    button : int
+        The integer value of the button being pushed.
+    buttons : str
+        The string name of the button being pushed.
+    modifiers : list
+        The modifiers that were pressed while the key was pressed.
+    ntouches : int
+        The total number of synchronous touches.
+    touches : list
+        A list of all currently occurring touches.
+    pick_info : dict
+        Values of pickable fields. The exact content is specific to the
+        WorldObject triggering the event.
+    clicks : int
+        The total number of synchronous clicks.
+    pointer_id : Any
+        The value set by `set_pointer_capture()`.
+    kwargs : Any
+        Additional keyword arguments are forward to the :class:`base class
+        <pygfx.objects.Event>`.
+
+    Notes
+    -----
+    The values of this event follow the convention used by jupyter rfb. You can read
+    about them `here <https://jupyter-rfb.readthedocs.io/en/stable/events.html>`_.
+
+    """
+
     def __init__(
         self,
         *args,
         x,
         y,
         button=0,
         buttons=None,
@@ -172,49 +247,95 @@
             root=self.root,
         )
         values.update(kwargs)
         return PointerEvent(**values)
 
 
 class WheelEvent(PointerEvent):
+    """Scrolling of the mouse wheel.
+
+    Parameters
+    ----------
+    args : Any
+        Positional arguments are forwarded to the :class:`base class
+        <pygfx.objects.Event>`.
+    dx : float
+        The amount (in rad) by which the wheel was turned around the x-axis.
+    dy : float
+        The amount (in rad) by which the wheel was turned around the y-axis.
+    kwargs : Any
+        Additional keyword arguments are forward to the :class:`base class
+        <pygfx.objects.Event>`.
+
+    """
+
     def __init__(self, *args, dx, dy, **kwargs):
         super().__init__(*args, **kwargs)
         self.dx = dx
         self.dy = dy
 
 
 class WindowEvent(Event):
+    """Window resize event
+
+    Parameters
+    ----------
+    args : Any
+        Positional arguments are forwarded to the :class:`base class
+        <pygfx.objects.Event>`.
+    width : int
+        The new width of the application window in screen space (px).
+    height : int
+        The new height of the application window in screen space (px).
+    pixel_ratio : float
+        The new ratio between logical pixels and physical pixels.
+    kwargs : Any
+        Additional keyword arguments are forward to the :class:`base class
+        <pygfx.objects.Event>`.
+
+    """
+
     def __init__(self, *args, width=None, height=None, pixel_ratio=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.width = width
         self.height = height
         self.pixel_ratio = pixel_ratio
 
 
 class EventTarget:
-    """Mixin class that enables event handlers to be attached to objects
+    """Targetable object mixin.
+
+    Mixin class that enables event handlers to be attached to objects
     of the mixed-in class.
+
+    Parameters
+    ----------
+    args : Any
+        Arguments are forwarded to allow multiple inheritance.
+    kwargs : Any
+        Kwargs are forwarded to allow multiple inheritance.
+
     """
 
-    pointer_captures = WeakValueDictionary()
+    pointer_captures = {}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._event_handlers = defaultdict(set)
 
     def add_event_handler(self, *args):
         """Register an event handler.
 
         Arguments:
             callback (callable): The event handler. Must accept a
                 single event argument.
             *types (list of strings): A list of event types.
 
         For the available event types, see
-        https://jupyter-rfb.readthedocs.io/en/latest/events.html
+        https://jupyter-rfb.readthedocs.io/en/stable/events.html
 
         Can also be used as a decorator.
 
         Example:
 
         .. code-block:: py
 
@@ -269,119 +390,141 @@
         event_type = event.type
         for callback in self._event_handlers[event_type].copy():
             if event.cancelled:
                 break
             with log_exception(f"Error during handling {event_type} event"):
                 callback(event)
 
-    def set_pointer_capture(self, pointer_id):
+    def set_pointer_capture(self, pointer_id, event_root):
         """Register this object to capture any other pointer events,
         until ``release_pointer_capture`` is called or an ``pointer_up``
         event is encountered.
 
         Arguments:
             pointer_id: id of pointer to capture (mouse, touch, etc.)
+            event_root: the event root that this pointer is captured on
         """
-        EventTarget.pointer_captures[pointer_id] = self
+        EventTarget.pointer_captures[pointer_id] = (
+            ref(self),
+            (event_root and ref(event_root)) or None,
+        )
 
     def release_pointer_capture(self, pointer_id):
         """Release the pointer capture for the object that was registered
         to the given pointer_id.
 
         Arguments:
             pointer_id: id of pointer to release (mouse, touch, etc.)
         """
         EventTarget.pointer_captures.pop(pointer_id, None)
 
 
 class RootEventHandler(EventTarget):
-    """Root event handler for the Pygfx event system."""
+    """Pygfx event handler.
+
+    Root event handler for the Pygfx event system.
 
-    # Dictionary to track clicks, keyed on pointer_id
-    click_tracker = {}
-    # Dictionary to track targets, keyed on pointer_id
-    target_tracker = {}
+    """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        # Dictionary to track clicks, keyed on pointer_id
+        self._click_tracker = {}
+        # Dictionary to track targets, keyed on pointer_id
+        self._target_tracker = {}
 
     def dispatch_event(self, event: Event):
         """Dispatch the given event.
 
-        This method will dispatch an event by looking for the right target
-        to handle the event. When a target is set on the event, then that
-        target will be the first object that gets to handle the event.
-        From there it will ask its parents one-by-one to handle the event
-        as long as the event bubbles / propagates up or is not cancelled.
+        This method will dispatch an event by looking for the right target to
+        handle the event. When a target is set on the event, then that target
+        will be the first object that gets to handle the event. From there it
+        will ask its parents one-by-one to handle the event as long as the event
+        bubbles / propagates up or is not cancelled.
 
-        The RootEventHandler object will serve as a virtual root for the
-        tree hierarchy.
+        The RootEventHandler object will serve as a virtual root for the tree
+        hierarchy.
 
         Whenever an object has captured the pointer (for a specific pointer_id)
         then that object will get all pointer related events until the object
         releases the capture or a ``pointer_up`` event is encountered.
 
         This method will also keep track of ``pointer_down`` and ``pointer_up``
         events in order to generate and dispatch ``click`` and ``double_click``
         events.
 
-        Arguments:
-            event: Event object to dispatch
+        Parameters
+        ----------
+        event : Event
+            The event to dispatch.
+
         """
         pointer_id = getattr(event, "pointer_id", None)
 
         # Check for captured pointer events
         if pointer_id is not None and pointer_id in EventTarget.pointer_captures:
-            captured_target = EventTarget.pointer_captures.get(pointer_id)
-            # Encountered an event with pointer_id while there is a
-            # capture active, so don't bubble, and retarget the event
-            # to the captured target
-            event._retarget(captured_target)
-            event.stop_propagation()
+            captured_target_ref, event_root_ref = EventTarget.pointer_captures[
+                pointer_id
+            ]
+            captured_target, event_root = (
+                captured_target_ref(),
+                event_root_ref and event_root_ref(),
+            )
+            # If the pointer was captured in the context of another root event
+            # handler, then let's not handle this event. It will be handled by
+            # the appropriate RootEventHandler
+            if event_root and event_root is not self:
+                return
+
+            if captured_target:
+                # Encountered an event with pointer_id while there is a
+                # capture active, so don't bubble, and retarget the event
+                # to the captured target
+                event._retarget(captured_target)
+                event.stop_propagation()
 
         # Current target is either something that was under the pointer, or nothing
         # in which case we set the target to the root event handler (self)
         target = event.target or self
 
         # Update the target tracker on all `pointer_move` events
         if event.type == EventType.POINTER_MOVE:
             # Get the previous target for this pointer (if any)
-            previous_target_ref = RootEventHandler.target_tracker.get(pointer_id)
+            previous_target_ref = self._target_tracker.get(pointer_id)
             previous_target = (previous_target_ref and previous_target_ref()) or None
             # Check if the target has changed since the previous move event
             if previous_target is not target:
                 # Update the current target for this pointer
-                RootEventHandler.target_tracker[pointer_id] = (
-                    target and ref(target)
-                ) or None
+                self._target_tracker[pointer_id] = (target and ref(target)) or None
                 if previous_target is not None:
                     # Dispatch a `pointer_leave` event for the previous target
                     ev = event.copy(type="pointer_leave", target=previous_target)
                     self.dispatch_event(ev)
                 # Dispatch a `pointer_enter` event for the new target
                 ev = event.copy(type="pointer_enter")
                 self.dispatch_event(ev)
 
         # Dispatch the event to target and bubble up the hierarchy
         while target:
             # Update the current target
             event._update_current_target(target)
             target.handle_event(event)
+            # During handling of the event, the target might capture the pointer events
             if pointer_id is not None and pointer_id in EventTarget.pointer_captures:
                 event._retarget(target)
                 event.stop_propagation()
                 if event.type == EventType.POINTER_UP:
                     captured_target.release_pointer_capture(pointer_id)
             if not event.bubbles or event.cancelled or target is self:
                 break
             target = target.parent or self
 
         # Update the click tracker on all `pointer_down` events
         if event.type == EventType.POINTER_DOWN:
-            tracked_click = RootEventHandler.click_tracker.get(pointer_id)
+            tracked_click = self._click_tracker.get(pointer_id)
             # Check if the `pointer_id` is already tracked, targets
             # the same target and is within the DEBOUNCE time.
             # Bump the count and update the time_stamp if that is the case.
             # Otherwise, restart counting.
             if (
                 tracked_click
                 and (
@@ -391,25 +534,25 @@
                     or (tracked_click["target"] is None and event.target is None)
                 )
                 and event.time_stamp - tracked_click["time_stamp"] < CLICK_DEBOUNCE
             ):
                 tracked_click["count"] += 1
                 tracked_click["time_stamp"] = event.time_stamp
             else:
-                RootEventHandler.click_tracker[pointer_id] = {
+                self._click_tracker[pointer_id] = {
                     "count": 1,
                     "time_stamp": event.time_stamp,
                     "target": (event.target and ref(event.target)) or None,
                 }
         # On all ``pointer_up`` events, see if the event is on the same target
         # as for the ``pointer_down``. If so, then a ``click`` event is dispatched.
         # When the counter for the click is at 2, then a ``double_click`` event
         # is dispatched.
         elif event.type == EventType.POINTER_UP:
-            tracked_click = RootEventHandler.click_tracker.get(pointer_id)
+            tracked_click = self._click_tracker.get(pointer_id)
             if tracked_click and (
                 tracked_click["target"] is not None
                 and tracked_click["target"]() is not None
                 and tracked_click["target"]() is event.target
                 or (tracked_click["target"] is None and event.target is None)
             ):
                 ev = event.copy(type="click", clicks=tracked_click["count"])
```

### Comparing `pygfx-0.1.9/pygfx/objects/_instanced.py` & `pygfx-0.2.0/pygfx/objects/_instanced.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,49 +2,74 @@
 
 from ._base import id_provider
 from . import Mesh
 from ..resources import Buffer
 
 
 class InstancedMesh(Mesh):
-    """An instanced mesh with a matrix for each instance."""
+    """Display a mesh multiple times using instances.
+
+    An instanced mesh with a matrix for each instance.
+
+    Parameters
+    ----------
+    geometry : Geometry
+        The mesh's geometry data.
+    material : Material
+        The material with which to render the mesh.
+    count : int
+        The number of instances to create.
+    kwargs : Any
+        Additional kwargs get forwarded to the :class:`base class
+        <pygfx.objects.Mesh>`.
+
+    """
 
     def __init__(self, geometry, material, count, **kwargs):
         super().__init__(geometry, material, **kwargs)
         count = int(count)
         # Create array of `count` instance_info objects
         dtype = np.dtype(
             [
                 ("matrix", np.float32, (4, 4)),
                 ("id", np.uint32),
                 ("_12_bytes_padding", np.uint8, (12,)),
             ]
         )
         instance_infos = np.zeros(count, dtype)
-        self.instance_infos = Buffer(instance_infos, nitems=count)
+        self._store.instance_buffer = Buffer(instance_infos, nitems=count)
         # Set ids
         self._idmap = {}
         for instance_index in range(count):
             id = id_provider.claim_id(self)
             self._idmap[id] = instance_index
             instance_infos[instance_index]["id"] = id
         # Init eye matrices
         for i in range(4):
             instance_infos["matrix"][:, i, i] = 1
 
     def __del__(self):
         super().__del__()
-        instance_infos = self.instance_infos.data
+        instance_infos = self._store["instance_buffer"].data
         for i in range(len(instance_infos)):
             id_provider.release_id(self, instance_infos[i]["id"])
 
+    @property
+    def instance_buffer(self):
+        return self._store.instance_buffer
+
     def set_matrix_at(self, index: int, matrix):
         """set the matrix for the instance at the given index."""
         matrix = np.array(matrix).reshape(4, 4)
-        self.instance_infos.data["matrix"][index] = matrix
+        self._store["instance_buffer"].data["matrix"][index] = matrix.T
+        self._store["instance_buffer"].update_range(index, 1)
+
+    def get_matrix_at(self, index: int):
+        """get the matrix for the instance at the given index."""
+        return self._store["instance_buffer"].data["matrix"][index].T
 
     def _wgpu_get_pick_info(self, pick_value):
         info = self.material._wgpu_get_pick_info(pick_value)
         # The id maps to one of our instances
         id = pick_value & 1048575  # 2**20-1
         info["instance_index"] = self._idmap.get(id)
         return info
```

### Comparing `pygfx-0.1.9/pygfx/renderers/_base.py` & `pygfx-0.2.0/pygfx/utils/renderfunctionregistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from ..objects import WorldObject
 from ..materials import Material
 
 
 class Renderer:
-    """Base class for all renderers. The purpose of a renderer is to
-    render (i.e. draw) a scene to a canvas.
-    """
+    """Renderer base class."""
 
     pass
 
 
 class RenderFunctionRegistry:
-    """A registry for render functions capable of rendering specific
+    """Storage for available rendering functions.
+
+    A registry for render functions capable of rendering specific
     object-material combinations. This registry allows for a scalable
     plugin-like system for a renderer's capabilities.
+
     """
 
     def __init__(self):
         self._store = {}
         self._known_classes = set([WorldObject, Material])
 
     def register(self, wobject_cls, material_cls, func):
```

### Comparing `pygfx-0.1.9/pygfx/renderers/svg/_svgrenderer.py` & `pygfx-0.2.0/pygfx/renderers/svg/_svgrenderer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,73 @@
 import os
 import io
+import pylinalg as la
 
-from .. import Renderer, RenderFunctionRegistry
+from ...utils.renderfunctionregistry import RenderFunctionRegistry
 
 from ...objects import WorldObject
 from ...cameras import Camera
-from ...linalg import Matrix4, Vector3
+from .. import Renderer
 
 
 registry = RenderFunctionRegistry()
 
 
 def register_svg_render_function(wobject_cls, material_cls):
-    """Decorator to register an SVG render function."""
+    """Decorator for SVG rendering functions.
+
+    Parameters
+    ----------
+    wobject_cls : WorldObject
+        The world object that this function knows how to render.
+    material_cls : Material
+        The world object that this function knows how to render.
+
+    """
 
     def _register_svg_render_function(f):
         registry.register(wobject_cls, material_cls, f)
         return f
 
     return _register_svg_render_function
 
 
 class SvgRenderer(Renderer):
-    """A renderer that generates an SVG."""
+    """Turns scenes into SVG images.
+
+    Notice: this renderer is just an experimental stub for now.
+
+    Parameters
+    ----------
+    width : int
+        The width of the resulting image.
+    height : int
+        The height of the resulting image.
+    filename : str
+        The name of the location to which to write the image.
+
+    """
 
     def __init__(self, width, height, filename):
         self._width = width
         self._height = height
 
         # todo: also support writing to file-like object
         if filename.startswith("~"):
             filename = os.path.expanduser(filename)
         self._filename = filename
 
     def render(self, scene: WorldObject, camera: Camera):
         """Render the scene to a file."""
 
         # Ensure that matrices are up-to-date
-        scene.update_matrix_world()
-        camera.update_matrix_world()  # camera may not be a member of the scene
         camera.update_projection_matrix()
 
         # Get the sorted list of objects to render (guaranteed to be visible and having a material)
-        proj_screen_matrix = Matrix4().multiply_matrices(
-            camera.projection_matrix, camera.matrix_world_inverse
-        )
-        q = self.get_render_list(scene, proj_screen_matrix)
+        q = self.get_render_list(scene, camera.camera_matrix)
 
         # Init the svg file
         f = io.StringIO()
         f.write(
             f"<svg width='{self._width}' height='{self._height}' xmlns='http://www.w3.org/2000/svg'>\n"
         )
 
@@ -65,31 +83,26 @@
                         f.write(line)
 
         # Finish the svg file and write actual file handle.
         f.write("\n</svg>\n")
         with open(self._filename, "wb") as f2:
             f2.write(f.getvalue().encode())
 
-    def get_render_list(self, scene: WorldObject, proj_screen_matrix: Matrix4):
+    def get_render_list(self, scene: WorldObject, proj_screen_matrix):
         """Given a scene object, get a list of objects to render."""
 
         # start by gathering everything that is visible and has a material
         q = []
 
         def visit(wobject):
             nonlocal q
             if wobject.visible and hasattr(wobject, "material"):
                 q.append(wobject)
 
         scene.traverse(visit)
 
         # next, sort them from back-to-front
         def sort_func(wobject: WorldObject):
-            z = (
-                Vector3()
-                .set_from_matrix_position(wobject.matrix_world)
-                .apply_matrix4(proj_screen_matrix)
-                .z
-            )
+            z = la.vec_transform(wobject.world.position, proj_screen_matrix)[2]
             return wobject.render_order, z
 
         return list(sorted(q, key=sort_func))
```

### Comparing `pygfx-0.1.9/pygfx/renderers/svg/linerender.py` & `pygfx-0.2.0/pygfx/renderers/svg/linerender.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.9/pygfx/renderers/wgpu/_flusher.py` & `pygfx-0.2.0/pygfx/renderers/wgpu/engine/flusher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+"""
+The flusher is responsible for rendering the renderers internal image
+to the canvas.
+"""
+
 import wgpu
 import numpy as np
 
+from .utils import GpuCache, hash_from_value
+from .shared import get_shared
+
+# This cache enables sharing some gpu objects between code that uses
+# full-quad shaders. The gain here won't be large in general, but can
+# still be worthwhile in situations where many canvases are created,
+# such as in Jupyter notebooks, or e.g. when generating screenshots.
+# It should also reduce the required work during canvas resizing.
+FULL_QUAD_CACHE = GpuCache("full_quad_objects")
+
 
 FULL_QUAD_SHADER = """
     struct VertexInput {
         @builtin(vertex_index) index: u32,
     };
     struct Varyings {
         @location(0) texcoord: vec2<f32>,
@@ -12,183 +27,222 @@
     };
     struct FragmentOutput {
         @location(0) color: vec4<f32>,
     };
 
     BINDINGS_CODE
 
-    @stage(vertex)
+    @vertex
     fn vs_main(in: VertexInput) -> Varyings {
         var positions = array<vec2<f32>,4>(
             vec2<f32>(0.0, 1.0), vec2<f32>(0.0, 0.0), vec2<f32>(1.0, 1.0), vec2<f32>(1.0, 0.0)
         );
         let pos = positions[in.index];
         var varyings: Varyings;
         varyings.texcoord = vec2<f32>(pos.x, 1.0 - pos.y);
         varyings.position = vec4<f32>(pos * 2.0 - 1.0, 0.0, 1.0);
         return varyings;
     }
 
-    @stage(fragment)
+    @fragment
     fn fs_main(varyings: Varyings) -> FragmentOutput {
         var out : FragmentOutput;
         let texcoord = varyings.texcoord;  // for textureSample
         let texindex = vec2<i32>(varyings.position.xy);  // for textureLoad
 
         FRAGMENT_CODE
 
         return out;
     }
 """
 
 
-def _create_pipeline(device, binding_layouts, bindings, targets, wgsl):
+def create_full_quad_pipeline(targets, binding_layout, bindings_code, fragment_code):
+    device = get_shared().device
+
+    # Get bind group layout
+    key1 = hash_from_value(binding_layout)
+    bind_group_layout = FULL_QUAD_CACHE.get(key1)
+    if bind_group_layout is None:
+        bind_group_layout = device.create_bind_group_layout(entries=binding_layout)
+        FULL_QUAD_CACHE.set(key1, bind_group_layout)
+
+    # Get render pipeline
+    key2 = hash_from_value([bind_group_layout, targets, bindings_code, fragment_code])
+    render_pipeline = FULL_QUAD_CACHE.get(key2)
+    if render_pipeline is None:
+        wgsl = FULL_QUAD_SHADER
+        wgsl = wgsl.replace("BINDINGS_CODE", bindings_code)
+        wgsl = wgsl.replace("FRAGMENT_CODE", fragment_code)
+        shader_module = device.create_shader_module(code=wgsl)
+
+        pipeline_layout = device.create_pipeline_layout(
+            bind_group_layouts=[bind_group_layout]
+        )
+
+        render_pipeline = device.create_render_pipeline(
+            layout=pipeline_layout,
+            vertex={
+                "module": shader_module,
+                "entry_point": "vs_main",
+                "buffers": [],
+            },
+            primitive={
+                "topology": wgpu.PrimitiveTopology.triangle_strip,
+                "strip_index_format": wgpu.IndexFormat.uint32,
+            },
+            depth_stencil=None,
+            multisample=None,
+            fragment={
+                "module": shader_module,
+                "entry_point": "fs_main",
+                "targets": targets,
+            },
+        )
 
-    shader_module = device.create_shader_module(code=wgsl)
+        # Bind shader module object to the lifetime of the pipeline object
+        render_pipeline._gfx_module = shader_module
 
-    bind_group_layout = device.create_bind_group_layout(entries=binding_layouts)
-    pipeline_layout = device.create_pipeline_layout(
-        bind_group_layouts=[bind_group_layout]
-    )
-    bind_group = device.create_bind_group(layout=bind_group_layout, entries=bindings)
-
-    render_pipeline = device.create_render_pipeline(
-        layout=pipeline_layout,
-        vertex={
-            "module": shader_module,
-            "entry_point": "vs_main",
-            "buffers": [],
-        },
-        primitive={
-            "topology": wgpu.PrimitiveTopology.triangle_strip,
-            "strip_index_format": wgpu.IndexFormat.uint32,
-        },
-        depth_stencil=None,
-        multisample=None,
-        fragment={
-            "module": shader_module,
-            "entry_point": "fs_main",
-            "targets": targets,
-        },
-    )
+        FULL_QUAD_CACHE.set(key2, render_pipeline)
 
-    return bind_group, render_pipeline
+    return render_pipeline
 
 
 # %%%%%%%%%%
 
 
 class RenderFlusher:
     """
     Utility to flush (render) the current state of a renderer into a texture.
     """
 
-    # todo: Once we also have the depth here, we can support things like fog
-
-    def __init__(self, device):
-        self._device = device
-        self._pipelines = {}
-
-        dtype = [("size", "float32", (2,)), ("sigma", "float32"), ("support", "int32")]
+    def __init__(self, target_format):
+        self._device = get_shared().device
+        self._target_format = target_format
+
+        dtype = [
+            ("size", "float32", (2,)),
+            ("sigma", "float32"),
+            ("support", "int32"),
+            ("gamma", "float32"),
+            ("_padding", "float32"),
+        ]
         self._uniform_data = np.zeros((), dtype=dtype)
         self._uniform_buffer = self._device.create_buffer(
             size=self._uniform_data.nbytes,
             usage=wgpu.BufferUsage.UNIFORM | wgpu.BufferUsage.COPY_DST,
         )
 
-    def render(self, src_color_tex, src_depth_tex, dst_color_tex, dst_format):
-        """Render the (internal) result of the renderer into a texture."""
-        # NOTE: cannot actually use src_depth_tex as a sample texture (BindingCollision)
+        self._render_pipeline = None
+        self._bind_group = None
+        self._bind_group_hash = None
+
+    def render(
+        self,
+        src_color_tex,
+        src_depth_tex,
+        dst_color_tex,
+        gamma=1.0,
+        filter_strength=1.0,
+    ):
+        """Render the (internal) result of the renderer to a texture view."""
+
+        # NOTE: src_depth_tex is not used yet, see #492
+        # NOTE: cannot actually use src_depth_tex as a sample texture (BindingCollision)?
         assert src_depth_tex is None
-        assert isinstance(src_color_tex, wgpu.base.GPUTextureView)
-        assert isinstance(dst_color_tex, wgpu.base.GPUTextureView)
+        assert isinstance(src_color_tex, wgpu.GPUTextureView)
+        assert isinstance(dst_color_tex, wgpu.GPUTextureView)
 
-        # Recreate pipeline? Use ._internal as a true identifier of the texture view
-        hash = src_color_tex.size, src_color_tex._internal
-        stored_hash = self._pipelines.get(dst_format, ["invalidhash"])[0]
-        if hash != stored_hash:
-            bind_group, render_pipeline = self._create_pipeline(
-                src_color_tex, dst_format
+        # Make sure we have the render_pipeline
+        if self._render_pipeline is None:
+            self._render_pipeline = self._create_pipeline()
+
+        # Same for bind group. Needs to be recreated when the source texture changes.
+        hash = id(src_color_tex._internal)
+        if self._bind_group is None or hash != self._bind_group_hash:
+            self._bind_group_hash = hash
+            self._bind_group = self._create_bind_group(
+                self._render_pipeline.get_bind_group_layout(0), src_color_tex
             )
-            self._pipelines[dst_format] = hash, bind_group, render_pipeline
 
-        self._update_uniforms(src_color_tex, dst_color_tex)
-        return self._render(dst_color_tex, dst_format)
+        # Ready to go!
+        self._update_uniforms(src_color_tex, dst_color_tex, gamma, filter_strength)
+        return self._render(dst_color_tex)
 
-    def _update_uniforms(self, src_color_tex, dst_color_tex):
+    def _update_uniforms(self, src_color_tex, dst_color_tex, gamma, filter_strength):
         # Get factor between texture sizes
         factor_x = src_color_tex.size[0] / dst_color_tex.size[0]
         factor_y = src_color_tex.size[1] / dst_color_tex.size[1]
         factor = (factor_x + factor_y) / 2
 
-        if factor > 1:
-            # The src has higher res, we can do ssaa.
-            sigma = 0.5 * factor
-            support = min(5, int(sigma * 3))
+        if factor == 1:
+            # With equal res, we smooth a tiny bit. A bit less crisp, but also less flicker.
+            ref_sigma = 0.5
+        elif factor > 1:
+            # With src a higher res, we will do SSAA.
+            ref_sigma = 0.5 * factor
         else:
-            # The src has lower res, interpolate + smooth.
-            # Smoothing a bit more helps reduce the blockiness.
-            sigma = 1
-            support = 2
+            # With src a lower res, the output is interpolated. But we also smooth to reduce blockiness.
+            ref_sigma = 0.5
 
+        # Determine kernel sigma and support
+        sigma = ref_sigma * float(filter_strength)
+        support = int(sigma * 3)  # is limited in shader
+
+        # Compose
         self._uniform_data["size"] = src_color_tex.size[:2]
         self._uniform_data["sigma"] = sigma
         self._uniform_data["support"] = support
+        self._uniform_data["gamma"] = gamma
 
-    def _render(self, dst_color_tex, dst_format):
-        device = self._device
-        _, bind_group, render_pipeline = self._pipelines[dst_format]
-
-        command_encoder = device.create_command_encoder()
-
-        tmp_buffer = device.create_buffer_with_data(
-            data=self._uniform_data,
-            usage=wgpu.BufferUsage.COPY_SRC,
-        )
-        command_encoder.copy_buffer_to_buffer(
-            tmp_buffer, 0, self._uniform_buffer, 0, self._uniform_data.nbytes
+        # Sync to gpu
+        self._device.queue.write_buffer(
+            self._uniform_buffer, 0, self._uniform_data, 0, self._uniform_data.nbytes
         )
 
+    def _render(self, dst_color_tex):
+        command_encoder = self._device.create_command_encoder()
+
         render_pass = command_encoder.begin_render_pass(
             color_attachments=[
                 {
                     "view": dst_color_tex,
                     "resolve_target": None,
                     "clear_value": (0, 0, 0, 0),
                     "load_op": wgpu.LoadOp.clear,
                     "store_op": wgpu.StoreOp.store,
                 }
             ],
             depth_stencil_attachment=None,
         )
-        render_pass.set_pipeline(render_pipeline)
-        render_pass.set_bind_group(0, bind_group, [], 0, 99)
+        render_pass.set_pipeline(self._render_pipeline)
+        render_pass.set_bind_group(0, self._bind_group, [], 0, 99)
         render_pass.draw(4, 1)
         render_pass.end()
 
         return [command_encoder.finish()]
 
-    def _create_pipeline(self, src_texture_view, dst_format):
-        device = self._device
-
+    def _create_pipeline(self):
         bindings_code = """
             struct Render {
                 size: vec2<f32>,
                 sigma: f32,
                 support: i32,
+                gamma: f32,
             };
             @group(0) @binding(0)
             var<uniform> u_render: Render;
             @group(0) @binding(1)
             var r_color: texture_2d<f32>;
         """
 
         fragment_code = """
             // Get info about the smoothing
-            let sigma = u_render.sigma;
+            // The limits here may give the compiler info on max iters of the loop below.
+            let sigma = max(0.1, u_render.sigma);
             let support = min(5, u_render.support);
 
             // The reference index is the subpixel index in the source texture that
             // represents the location of this fragment.
             let ref_index = texcoord * u_render.size;
 
             // For the sampling, we work with integer coords. Also use min/max for the edges.
@@ -208,22 +262,19 @@
                     let dist = length(ref_index - vec2<f32>(index) - 0.5);
                     let t = dist / sigma;
                     let w = exp(-0.5 * t * t);
                     val = val + textureLoad(r_color, index, 0) * w;
                     weight = weight + w;
                 }
             }
-            out.color = val / weight;
+            let gamma3 = vec3<f32>(u_render.gamma);
+            out.color = vec4<f32>(pow(val.rgb / weight, gamma3), val.a / weight);
         """
 
-        wgsl = FULL_QUAD_SHADER
-        wgsl = wgsl.replace("BINDINGS_CODE", bindings_code)
-        wgsl = wgsl.replace("FRAGMENT_CODE", fragment_code)
-
-        binding_layouts = [
+        binding_layout = [
             {
                 "binding": 0,
                 "visibility": wgpu.ShaderStage.FRAGMENT,
                 "buffer": {"type": wgpu.BufferBindingType.uniform},
             },
             {
                 "binding": 1,
@@ -232,29 +283,17 @@
                     "sample_type": wgpu.TextureSampleType.unfilterable_float,
                     "view_dimension": wgpu.TextureViewDimension.d2,
                     "multisampled": False,
                 },
             },
         ]
 
-        bindings = [
-            {
-                "binding": 0,
-                "resource": {
-                    "buffer": self._uniform_buffer,
-                    "offset": 0,
-                    "size": self._uniform_data.nbytes,
-                },
-            },
-            {"binding": 1, "resource": src_texture_view},
-        ]
-
         targets = [
             {
-                "format": dst_format,
+                "format": self._target_format,
                 "blend": {
                     "alpha": (
                         wgpu.BlendFactor.src_alpha,
                         wgpu.BlendFactor.one_minus_src_alpha,
                         wgpu.BlendOperation.add,
                     ),
                     "color": (
@@ -262,8 +301,27 @@
                         wgpu.BlendFactor.one_minus_src_alpha,
                         wgpu.BlendOperation.add,
                     ),
                 },
             },
         ]
 
-        return _create_pipeline(device, binding_layouts, bindings, targets, wgsl)
+        return create_full_quad_pipeline(
+            targets, binding_layout, bindings_code, fragment_code
+        )
+
+    def _create_bind_group(self, bind_group_layout, src_texture_view):
+        # This must match the binding_layout above
+        bind_group_entries = [
+            {
+                "binding": 0,
+                "resource": {
+                    "buffer": self._uniform_buffer,
+                    "offset": 0,
+                    "size": self._uniform_data.nbytes,
+                },
+            },
+            {"binding": 1, "resource": src_texture_view},
+        ]
+        return self._device.create_bind_group(
+            layout=bind_group_layout, entries=bind_group_entries
+        )
```

### Comparing `pygfx-0.1.9/pygfx/renderers/wgpu/_renderer.py` & `pygfx-0.2.0/pygfx/renderers/wgpu/engine/renderer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,298 +1,288 @@
+"""
+The main renderer class. This class wraps a canvas or texture and it
+manages the rendering process.
+"""
+
 import time
 import weakref
-import logging
 
 import numpy as np
-import wgpu.backends.rs
+import wgpu
+import pylinalg as la
 
-from .. import Renderer
-from ...linalg import Matrix4, Vector3
-from ...objects import (
-    id_provider,
+from ....objects._base import id_provider
+from ....objects import (
     KeyboardEvent,
     RootEventHandler,
     PointerEvent,
     WheelEvent,
     WindowEvent,
     WorldObject,
 )
-from ...cameras import Camera
-from ...resources import Buffer, Texture, TextureView
-from ...utils import array_from_shadertype, Color
-
-from . import _blender as blender_module
-from ._flusher import RenderFlusher
-from ._pipelinebuilder import ensure_pipeline
-from ._update import update_buffer, update_texture, update_texture_view
-
-
-logger = logging.getLogger("pygfx")
-
-
-# Definition uniform struct with standard info related to transforms,
-# provided to each shader as uniform at slot 0.
-# todo: a combined transform would be nice too, for performance
-# todo: same for ndc_to_world transform (combined inv transforms)
-stdinfo_uniform_type = dict(
-    cam_transform="4x4xf4",
-    cam_transform_inv="4x4xf4",
-    projection_transform="4x4xf4",
-    projection_transform_inv="4x4xf4",
-    physical_size="2xf4",
-    logical_size="2xf4",
-    flipped_winding="i4",  # A bool, really
-)
+from ....cameras import Camera
+from ....resources import Texture
+from ....resources._base import resource_update_registry
+from ....utils import Color
+
+from ... import Renderer
+from . import blender as blender_module
+from .flusher import RenderFlusher
+from .pipeline import get_pipeline_container_group
+from .update import update_resource, ensure_wgpu_object
+from .shared import get_shared
+from .environment import get_environment
+from .shadowutil import render_shadow_maps
+from .mipmapsutil import generate_texture_mipmaps
+from .utils import GfxTextureView
 
 
 def _get_sort_function(camera: Camera):
     """Given a scene object, get a function to sort wobject-tuples"""
 
-    def sort_func(wobject_tuple: WorldObject):
-        wobject = wobject_tuple[0]
-        z = (
-            Vector3()
-            .set_from_matrix_position(wobject.matrix_world)
-            .apply_matrix4(proj_screen_matrix)
-            .z
-        )
+    def sort_func(wobject: WorldObject):
+        z = la.vec_transform(wobject.world.position, camera.camera_matrix)[2]
         return wobject.render_order, z
 
-    proj_screen_matrix = Matrix4().multiply_matrices(
-        camera.projection_matrix, camera.matrix_world_inverse
-    )
-
     return sort_func
 
 
-class SharedData:
-    """An object to store global data to share between multiple wgpu renderers.
-
-    Since renderers don't render simultaneously, they can share certain
-    resources. This safes memory, but more importantly, resources that
-    get used in wobject pipelines should be shared to avoid having to
-    constantly recompose the pipelines of wobjects that are rendered by
-    multiple renderers.
-    """
-
-    def __init__(self, canvas):
-
-        # Create adapter and device objects - there should be just one per canvas.
-        # Having a global device provides the benefit that we can draw any object
-        # anywhere.
-        # We could pass the canvas to request_adapter(), so we get an adapter that is
-        # at least compatible with the first canvas that a renderer is create for.
-        # However, passing the object has been shown to prevent the creation of
-        # a canvas (on Linux + wx), so, we never pass it for now.
-        self.adapter = wgpu.request_adapter(
-            canvas=None, power_preference="high-performance"
-        )
-        self.device = self.adapter.request_device(
-            required_features=[], required_limits={}
-        )
-
-        # Create a uniform buffer for std info
-        self.stdinfo_buffer = Buffer(array_from_shadertype(stdinfo_uniform_type))
-        self.stdinfo_buffer._wgpu_usage |= wgpu.BufferUsage.UNIFORM
-
-        # A cache for shader objects
-        self.shader_cache = {}
+class WgpuRenderer(RootEventHandler, Renderer):
+    """Turns Scenes into rasterized images using wgpu.
 
+    The current implementation supports various ``blend_modes`` which control how
+    transparency is handled during the rendering process. The following modes exist:
 
-class WgpuRenderer(RootEventHandler, Renderer):
-    """Object used to render scenes using wgpu.
+        * "default" or None: Select the default: currently this is "ordered2".
+        * "opaque": single-pass approach that ignores transparency.
+        * "ordered1": single-pass approach that blends fragments (using alpha
+          blending). Can only produce correct results if fragments are drawn
+          from back to front.
+        * "ordered2": two-pass approach that first processes all opaque
+          fragments and then blends transparent fragments (using alpha blending)
+          with depth-write disabled. The visual results are usually better than
+          ordered1, but still depend on the drawing order.
+        * "weighted": two-pass approach for order independent transparency based
+          on alpha weights.
+        * "weighted_depth": two-pass approach for order independent transparency
+          based on alpha weights and depth [1]. Note that the depth range
+          affects the (quality of the) visual result.
+        * "weighted_plus": three-pass approach for order independent
+          transparency, in which the front-most transparent layer is rendered
+          correctly, while transparent layers behind it are blended using alpha
+          weights.
+
+    Parameters
+    ----------
+    target : WgpuCanvas or Texture
+        The target to render to. It is also used to determine the size of the
+        render buffer.
+    pixel_ratio : float, optional
+        The ratio between the number of pixels in the render buffer versus the
+        number of pixels in the display buffer. If None, this will be 1 for
+        high-res canvases and 2 otherwise. If greater than 1, SSAA
+        (supersampling anti-aliasing) is applied while converting a render
+        buffer to a display buffer. If smaller than 1, pixels from the render
+        buffer are replicated while converting to a display buffer. This has
+        positive performance implications.
+    pixel_filter : float, optional
+        The strength of the filter when copying the result to the target/canvas.
+    show_fps : bool
+        Whether to display the frames per second. Beware that
+        depending on the GUI toolkit, the canvas may impose a frame rate limit.
+    blend_mode : str
+        The method for handling transparency. If None, use ``"ordered2"``.
+    sort_objects : bool
+        If True, sort objects by depth before rendering. The sorting
+        uses a hierarchical index based on the object's (1) ``render_order``,
+        (2) distance to the camera (based on the local frame's origin), (3) the
+        position in the scene graph (flattened depth-first). If False, the
+        rendering order is based on the objects ``render_order`` and position
+        in the scene graph only.
+    enable_events : bool
+        If True, forward wgpu events to pygfx's event system.
+    gamma_correction : float
+        The gamma correction to apply in the final render stage. Typically a
+        number between 0.0 and 2.0. A value of 1.0 indicates no correction.
+
+    References
+    ----------
+    [1] Morgan McGuire and Louis Bavoil, Weighted Blended Order-Independent Transparency, Journal of Computer Graphics Techniques (JCGT), vol. 2, no. 2, 122-141, 2013
 
-    The purpose of a renderer is to render (i.e. draw) a scene to a
-    canvas or texture. It also provides picking, defines the
-    anti-aliasing parameters, and any post processing effects.
-
-    A renderer is directly associated with its target and can only render
-    to that target. Different renderers can render to the same target though.
-
-    It provides a ``.render()`` method that can be called one or more
-    times to render scenes. This creates a visual representation that
-    is stored internally, and is finally rendered into its render target
-    (the canvas or texture).
-                                  __________
-                                 | blender  |
-        [scenes] -- render() --> |  state   | -- flush() --> [target]
-                                 |__________|
-
-    The internal representation is managed by the blender object. The
-    internal render textures are typically at a higher resolution to
-    reduce aliasing (SSAA). The blender has auxilary buffers such as a
-    depth buffer, pick buffer, and buffers for transparent fragments.
-    Depending on the blend mode, a single render call may consist of
-    multiple passes (to deal with semi-transparent fragments).
-
-    The flush-step resolves the internal representation into the target
-    texture or canvas, averaging neighbouring fragments for anti-aliasing.
-
-    Parameters:
-        target (WgpuCanvas or Texture): The target to render to, and what
-            determines the size of the render buffer.
-        pixel_ratio (float, optional): How large the physical size of the render
-            buffer is in relation to the target's physical size, for antialiasing.
-            See the corresponding property for details.
-        show_fps (bool): Whether to display the frames per second. Beware that
-            depending on the GUI toolkit, the canvas may impose a frame rate limit.
     """
 
-    _shared = None
-
     _wobject_pipelines_collection = weakref.WeakValueDictionary()
 
     def __init__(
         self,
         target,
         *args,
         pixel_ratio=None,
+        pixel_filter=None,
         show_fps=False,
         blend_mode="default",
         sort_objects=False,
         enable_events=True,
+        gamma_correction=1.0,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # Check and normalize inputs
-        if not isinstance(target, (Texture, TextureView, wgpu.gui.WgpuCanvasBase)):
+        if not isinstance(target, (Texture, GfxTextureView, wgpu.gui.WgpuCanvasBase)):
             raise TypeError(
-                f"Render target must be a canvas or texture (view), not a {target.__class__.__name__}"
+                f"Render target must be a Canvas or Texture, not a {target.__class__.__name__}"
             )
         self._target = target
-
-        # Process other inputs
         self.pixel_ratio = pixel_ratio
-        self._show_fps = bool(show_fps)
+        self.pixel_filter = pixel_filter
 
-        # Make sure we have a shared object (the first renderer create it)
-        canvas = target if isinstance(target, wgpu.gui.WgpuCanvasBase) else None
-        if WgpuRenderer._shared is None:
-            WgpuRenderer._shared = SharedData(canvas)
+        # Make sure we have a shared object (the first renderer creates the instance)
+        self._shared = get_shared()
+        self._device = self._shared.device
 
         # Init counter to auto-clear
         self._renders_since_last_flush = 0
 
         # Get target format
+        self.gamma_correction = gamma_correction
+        self._gamma_correction_srgb = 1.0
         if isinstance(target, wgpu.gui.WgpuCanvasBase):
             self._canvas_context = self._target.get_context()
-            self._target_tex_format = self._canvas_context.get_preferred_format(
+            # Select output format. We currently don't have a way of knowing
+            # what formats are available, so if not srgb, we gamma-correct in shader.
+            target_format = self._canvas_context.get_preferred_format(
                 self._shared.adapter
             )
+            if not target_format.endswith("srgb"):
+                self._gamma_correction_srgb = 1 / 2.2  # poor man's srgb
             # Also configure the canvas
             self._canvas_context.configure(
-                device=self._shared.device,
-                format=self._target_tex_format,
-                usage=wgpu.TextureUsage.RENDER_ATTACHMENT,
+                device=self._device,
+                format=target_format,
             )
         else:
-            self._target_tex_format = self._target.format
+            target_format = self._target.format
             # Also enable the texture for render and display usage
             self._target._wgpu_usage |= wgpu.TextureUsage.RENDER_ATTACHMENT
             self._target._wgpu_usage |= wgpu.TextureUsage.TEXTURE_BINDING
 
         # Prepare render targets.
         self.blend_mode = blend_mode
         self.sort_objects = sort_objects
 
         # Prepare object that performs the final render step into a texture
-        self._flusher = RenderFlusher(self._shared.device)
+        self._flusher = RenderFlusher(target_format)
 
         # Initialize a small buffer to read pixel info into
         # Make it 256 bytes just in case (for bytes_per_row)
-        self._pixel_info_buffer = self._shared.device.create_buffer(
+        self._pixel_info_buffer = self._device.create_buffer(
             size=16,
             usage=wgpu.BufferUsage.COPY_DST | wgpu.BufferUsage.MAP_READ,
         )
 
+        # Init fps measurements
+        self._show_fps = bool(show_fps)
+        now = time.perf_counter()
+        self._fps = {"start": now, "count": 0}
+
         if enable_events:
             self.enable_events()
 
     @property
     def device(self):
-        """A reference to the used wgpu device."""
-        return self._shared.device
+        """A reference to the global wgpu device."""
+        return self._device
 
     @property
     def target(self):
         """The render target. Can be a canvas, texture or texture view."""
         return self._target
 
     @property
     def pixel_ratio(self):
         """The ratio between the number of internal pixels versus the logical pixels on the canvas.
 
         This can be used to configure the size of the render texture
-        relative to the canvas' logical size. By default (value is None) the
-        used pixel ratio follows the screens pixel ratio on high-res
-        displays, and is 2 otherwise.
+        relative to the canvas' *logical* size. Can be set to None to
+        set the default. By default the pixel_ratio is 2 on "regular"
+        screens, and the same as the screen pixel ratio on HiDPI screens
+        (usually also 2).
 
         If the used pixel ratio causes the render texture to be larger
-        than the physical size of the canvas, SSAA is applied, resulting
-        in a smoother final image with less jagged edges. Alternatively,
-        this value can be set to e.g. 0.5 to lower* the resolution (e.g.
-        for performance during interaction).
+        than the physical size of the canvas, SSAA (super sampling
+        antialiasing) is applied, resulting in a smoother final image
+        with less jagged edges. Alternatively, this value can be set
+        to e.g. 0.5 to *lower* the resolution.
         """
-        return self._pixel_ratio
+        if self._pixel_ratio is not None:
+            return self._pixel_ratio
+        elif isinstance(self._target, wgpu.gui.WgpuCanvasBase):
+            target_pixel_ratio = self._target.get_pixel_ratio()
+            if target_pixel_ratio > 1.0:
+                return target_pixel_ratio
+        # Default
+        return 2.0
 
     @pixel_ratio.setter
     def pixel_ratio(self, value):
+        if not value:
+            value = None
         if value is None:
             self._pixel_ratio = None
         elif isinstance(value, (int, float)):
-            self._pixel_ratio = None if value <= 0 else float(value)
+            self._pixel_ratio = abs(float(value))
         else:
             raise TypeError(
                 f"Rendered.pixel_ratio expected None or number, not {value}"
             )
 
     @property
+    def pixel_filter(self):
+        """The strength of the filter applied to the final pixels.
+
+        The renderer renders everything to an internal texture, which,
+        depending on the `pixel_ratio`, may have a differens size than
+        the target (i.e. canvas). In the process of rendering the result
+        to the target, a filter is applied, resulting in SSAA if the
+        size was larger, and a smoothing effect otherwise.
+
+        When the `pixel_filter` is 1.0, the default optimal filter is
+        used. Higher values result in more blur. Can be set to 0 to
+        disable the filter.
+        """
+        return self._pixel_filter
+
+    @pixel_filter.setter
+    def pixel_filter(self, value):
+        if value is None:
+            value = 1.0
+        self._pixel_filter = max(0.0, float(value))
+
+    @property
     def rect(self):
         """The rectangular viewport for the renderer area."""
         return (0, 0) + self.logical_size
 
     @property
     def logical_size(self):
         """The size of the render target in logical pixels."""
         target = self._target
         if isinstance(target, wgpu.gui.WgpuCanvasBase):
             return target.get_logical_size()
         elif isinstance(target, Texture):
             return target.size[:2]  # assuming pixel-ratio 1
-        elif isinstance(target, TextureView):
-            return target.texture.size[:2]  # assuming pixel-ratio 1
         else:
             raise TypeError(f"Unexpected render target {target.__class__.__name__}")
 
     @property
     def physical_size(self):
         """The physical size of the internal render texture."""
-
-        # Get physical size of the target
-        target = self._target
-        if isinstance(target, wgpu.gui.WgpuCanvasBase):
-            target_psize = target.get_physical_size()
-        elif isinstance(target, Texture):
-            target_psize = target.size[:2]
-        elif isinstance(target, TextureView):
-            target_psize = target.texture.size[:2]
-        else:
-            raise TypeError(f"Unexpected render target {target.__class__.__name__}")
-
-        # Determine the pixel ratio of the render texture
-        if self._pixel_ratio:
-            pixel_ratio = self._pixel_ratio
-        else:
-            target_lsize = self.logical_size
-            pixel_ratio = target_psize[0] / target_lsize[0]
-            if pixel_ratio <= 1:
-                pixel_ratio = 2.0  # use 2 on non-hidpi displays
-
-        # Determine the physical size of the internal render textures
+        pixel_ratio = self.pixel_ratio
+        target_lsize = self.logical_size
         return tuple(max(1, int(pixel_ratio * x)) for x in target_lsize)
 
     @property
     def blend_mode(self):
         """The method for handling transparency:
 
         * "default" or None: Select the default: currently this is "ordered2".
@@ -304,15 +294,15 @@
           visual results are usually better than ordered1, but still depend on the drawing order.
         * "weighted": two-pass approach that for order independent transparency,
           using alpha weights.
         * "weighted_depth": two-pass approach for order independent transparency,
           with weights based on alpha and depth (McGuire 2013). Note that the depth
           range affects the (quality of the) visual result.
         * "weighted_plus": three-pass approach for order independent transparency,
-          in wich the front-most transparent layer is rendered correctly, while
+          in which the front-most transparent layer is rendered correctly, while
           transparent layers behind it are blended using alpha weights.
         """
         return self._blend_mode
 
     @blend_mode.setter
     def blend_mode(self, value):
         # Massage and check the input
@@ -341,42 +331,54 @@
         self._set_wobject_pipelines()
         # If our target is a canvas, request a new draw
         if isinstance(self._target, wgpu.gui.WgpuCanvasBase):
             self._target.request_draw()
 
     @property
     def sort_objects(self):
-        """Whether to sort world objects before rendering. Default False.
+        """Whether to sort world objects by depth before rendering. Default False.
 
         * ``True``: the render order is defined by 1) the object's ``render_order``
           property; 2) the object's distance to the camera; 3) the position object
           in the scene graph (based on a depth-first search).
-        * ``False``: don't sort, the render order is defined by the scene graph alone.
+        * ``False``: don't sort, the render order is only defined by the
+          ``render_order`` and scene graph position.
         """
         return self._sort_objects
 
     @sort_objects.setter
     def sort_objects(self, value):
         self._sort_objects = bool(value)
 
+    @property
+    def gamma_correction(self):
+        """The gamma correction applied in the final composition step."""
+        return self._gamma_correction
+
+    @gamma_correction.setter
+    def gamma_correction(self, value):
+        self._gamma_correction = 1.0 if value is None else float(value)
+        if isinstance(self._target, wgpu.gui.WgpuCanvasBase):
+            self._target.request_draw()
+
     def _set_wobject_pipelines(self):
         # Each WorldObject has associated with it a wobject_pipeline:
         # a dict that contains the wgpu pipeline objects. This
         # wobject_pipeline is also associated with the blend_mode,
         # because the blend mode affects the pipelines.
         #
         # Each renderer has ._wobject_pipelines, a dict that maps
         # wobject -> wobject_pipeline. This dict is a WeakKeyDictionary -
         # when the wobject is destroyed, the associated pipeline is
         # collected as well.
         #
         # Renderers with the same blend mode can safely share these
         # wobject_pipeline dicts. Therefore, we make use of a global
         # collection. Since this global collection is a
-        # WeakValueDictionary, if all renderes stop using a certain
+        # WeakValueDictionary, if all renderers stop using a certain
         # blend mode, the associated pipelines are removed as well.
         #
         # In a diagram:
         #
         # _wobject_pipelines_collection -> _wobject_pipelines -> wobject_pipeline
         #        global                         renderer              wobject
         #   WeakValueDictionary              WeakKeyDictionary         dict
@@ -389,15 +391,14 @@
 
     def render(
         self,
         scene: WorldObject,
         camera: Camera,
         *,
         rect=None,
-        viewport=None,
         clear_color=None,
         flush=True,
     ):
         """Render a scene with the specified camera as the viewpoint.
 
         Parameters:
             scene (WorldObject): The scene to render, a WorldObject that
@@ -408,25 +409,14 @@
                 expressed in logical pixels, a.k.a. the viewport.
             clear_color (bool, optional): Whether to clear the color buffer
                 before rendering. By default this is True on the first
                 call to ``render()`` after a flush, and False otherwise.
             flush (bool, optional): Whether to flush the rendered result into
                 the target (texture or canvas). Default True.
         """
-        device = self.device
-
-        now = time.perf_counter()  # noqa
-        if self._show_fps:
-            if not hasattr(self, "_fps"):
-                self._fps = now, now, 1
-            elif now > self._fps[0] + 1:
-                print(f"FPS: {self._fps[2]/(now - self._fps[0]):0.1f}")
-                self._fps = now, now, 1
-            else:
-                self._fps = self._fps[0], now, self._fps[2] + 1
 
         # Define whether to clear color.
         if clear_color is None:
             clear_color = self._renders_since_last_flush == 0
         clear_color = bool(clear_color)
         self._renders_since_last_flush += 1
 
@@ -442,25 +432,15 @@
         logical_size = self.logical_size
         physical_size = self.physical_size
         if not all(i > 0 for i in logical_size):
             return
         pixel_ratio = physical_size[1] / logical_size[1]
 
         # Update the render targets
-        self._blender.ensure_target_size(device, physical_size)
-
-        # todo: 11-04-2022 - remove viewport arg and this backwards compat logic in the next release
-        if viewport is not None:
-            if not hasattr(self, "_warned_for_viewport_arg"):
-                self._warned_for_viewport_arg = True
-                logger.warning(
-                    "render(viewport=xx) is deprecated, use rect=xx instead."
-                )
-            if not rect:
-                rect = viewport
+        self._blender.ensure_target_size(physical_size)
 
         # Get viewport in physical pixels
         if not rect:
             scene_lsize = logical_size
             scene_psize = physical_size
             physical_viewport = 0, 0, physical_size[0], physical_size[1], 0, 1
         elif len(rect) == 4:
@@ -469,185 +449,231 @@
             physical_viewport = tuple(physical_viewport) + (0, 1)
             scene_psize = physical_viewport[2], physical_viewport[3]
         else:
             raise ValueError(
                 "The viewport rect must be None or 4 elements (x, y, w, h)."
             )
 
+        # Allow objects to prepare just in time. When doing multiple
+        # render calls, we don't want to spam. The clear_color flag is
+        # a good indicator to detect the first render call.
+        if clear_color:
+            ev = WindowEvent(
+                "before_render",
+                target=None,
+                root=self,
+                width=logical_size[0],
+                height=logical_size[1],
+                pixel_ratio=self.pixel_ratio,
+            )
+            self.dispatch_event(ev)
+
         # Ensure that matrices are up-to-date
-        scene.update_matrix_world()
         camera.set_view_size(*scene_lsize)
-        camera.update_matrix_world()  # camera may not be a member of the scene
         camera.update_projection_matrix()
 
+        # Prepare the shared object
+        self._shared.pre_render_hook()
+
         # Update stdinfo uniform buffer object that we'll use during this render call
         self._update_stdinfo_buffer(camera, scene_psize, scene_lsize)
 
-        # Get the list of objects to render, as they appear in the scene graph
+        # Get environment
+        environment = get_environment(self, scene)
+
+        # Flatten the scenegraph, categorised by render_order
+        wobject_dict = {}
+        scene.traverse(
+            lambda ob: wobject_dict.setdefault(ob.render_order, []).append(ob), True
+        )
+
+        # Produce a sorted list of world objects
         wobject_list = []
-        scene.traverse(wobject_list.append, True)
+        if self._sort_objects:
+            depth_sort_func = _get_sort_function(camera)
+            for render_order in sorted(wobject_dict.keys()):
+                wobjects = wobject_dict[render_order]
+                wobjects.sort(key=depth_sort_func)
+                wobject_list.extend(wobjects)
+        else:
+            for render_order in sorted(wobject_dict.keys()):
+                wobject_list.extend(wobject_dict[render_order])
 
-        # Ensure each wobject has pipeline info, and filter objects that we cannot render
-        wobject_tuples = []
-        any_has_changed = False
+        # Collect all pipeline container objects
+        compute_pipeline_containers = []
+        render_pipeline_containers = []
         for wobject in wobject_list:
             if not wobject.material:
                 continue
-            wobject_pipeline, has_changed = ensure_pipeline(self, wobject)
-            if wobject_pipeline:
-                any_has_changed |= has_changed
-                wobject_tuples.append((wobject, wobject_pipeline))
+            container_group = get_pipeline_container_group(wobject, environment)
+            compute_pipeline_containers.extend(container_group.compute_containers)
+            render_pipeline_containers.extend(container_group.render_containers)
+            # Enable pipelines to update data on the CPU. This usually includes
+            # baking data into buffers. This is CPU intensive, but in practice
+            # it is only used by a few materials.
+            for func in container_group.bake_functions:
+                func(wobject, camera, logical_size)
+
+        # Update *all* buffers and textures that have changed
+        for resource in resource_update_registry.get_syncable_resources(flush=True):
+            update_resource(resource)
 
         # Command buffers cannot be reused. If we want some sort of re-use we should
         # look into render bundles. See https://github.com/gfx-rs/wgpu-native/issues/154
         # If we do get this to work, we should trigger a new recording
-        # when the wobject's children, visibile, render_order, or render_pass changes.
-
-        # Sort objects
-        if self.sort_objects:
-            sort_func = _get_sort_function(camera)
-            wobject_tuples.sort(key=sort_func)
+        # when the wobject's children, visible, render_order, or render_pass changes.
 
         # Record the rendering of all world objects, or re-use previous recording
         command_buffers = []
         command_buffers += self._render_recording(
-            wobject_tuples, physical_viewport, clear_color
+            environment,
+            wobject_list,
+            compute_pipeline_containers,
+            render_pipeline_containers,
+            physical_viewport,
+            clear_color,
         )
-        command_buffers += self._blender.perform_combine_pass(self._shared.device)
-        command_buffers
+        command_buffers += self._blender.perform_combine_pass()
 
         # Collect commands and submit
-        device.queue.submit(command_buffers)
+        self._device.queue.submit(command_buffers)
 
         if flush:
             self.flush()
 
-    def flush(self):
-        """Render the result into the target texture view. This method is
-        called automatically unless you use ``.render(..., flush=False)``.
+    def flush(self, target=None):
+        """Render the result into the target. This method is called
+        automatically unless you use ``.render(..., flush=False)``.
         """
 
-        # Note: we could, in theory, allow specifying a custom target here.
+        # Print FPS
+        now = time.perf_counter()  # noqa
+        if self._show_fps:
+            if self._fps["count"] == 0:
+                print(f"Time to first draw: {now-self._fps['start']:0.2f}")
+                self._fps["start"] = now
+                self._fps["count"] = 1
+            elif now > self._fps["start"] + 1:
+                fps = self._fps["count"] / (now - self._fps["start"])
+                print(f"FPS: {fps:0.1f}")
+                self._fps["start"] = now
+                self._fps["count"] = 1
+            else:
+                self._fps["count"] += 1
 
-        if isinstance(self._target, wgpu.gui.WgpuCanvasBase):
-            raw_texture_view = self._canvas_context.get_current_texture()
+        need_mipmaps = False
+        if target is None:
+            target = self._target
+
+        # Get the wgpu texture view.
+        if isinstance(target, wgpu.gui.WgpuCanvasBase):
+            wgpu_tex_view = self._canvas_context.get_current_texture().create_view()
+        elif isinstance(target, Texture):
+            need_mipmaps = target.generate_mipmaps
+            wgpu_tex_view = getattr(target, "_wgpu_default_view", None)
+            if wgpu_tex_view is None:
+                wgpu_tex_view = ensure_wgpu_object(GfxTextureView(target))
+                target._wgpu_default_view = wgpu_tex_view
+        elif isinstance(target, GfxTextureView):
+            need_mipmaps = target.texture.generate_mipmaps
+            wgpu_tex_view = ensure_wgpu_object(target)
         else:
-            if isinstance(self._target, Texture):
-                texture_view = self._target.get_view()
-            elif isinstance(self._target, TextureView):
-                texture_view = self._target
-            update_texture(self._shared.device, texture_view.texture)
-            update_texture_view(self._shared.device, texture_view)
-            raw_texture_view = texture_view._wgpu_texture_view[1]
+            raise TypeError("Unexpected target type.")
 
         # Reset counter (so we can auto-clear the first next draw)
         self._renders_since_last_flush = 0
 
         command_buffers = self._flusher.render(
             self._blender.color_view,
             None,
-            raw_texture_view,
-            self._target_tex_format,
+            wgpu_tex_view,
+            self._gamma_correction * self._gamma_correction_srgb,
+            self._pixel_filter,
         )
-        self.device.queue.submit(command_buffers)
+        self._device.queue.submit(command_buffers)
+
+        if need_mipmaps:
+            generate_texture_mipmaps(target)
 
     def _render_recording(
         self,
-        wobject_tuples,
+        environment,
+        wobject_list,
+        compute_pipeline_containers,
+        render_pipeline_containers,
         physical_viewport,
         clear_color,
     ):
-
         # You might think that this is slow for large number of world
         # object. But it is actually pretty good. It does iterate over
         # all world objects, and over stuff in each object. But that's
         # it, really.
         # todo: we may be able to speed this up with render bundles though
 
-        command_encoder = self.device.create_command_encoder()
+        command_encoder = self._device.create_command_encoder()
         blender = self._blender
+        if clear_color:
+            blender.clear()
+        else:
+            blender.clear_depth()
 
         # ----- compute pipelines
 
         compute_pass = command_encoder.begin_compute_pass()
 
-        for wobject, wobject_pipeline in wobject_tuples:
-            for pinfo in wobject_pipeline.get("compute_pipelines", ()):
-                compute_pass.set_pipeline(pinfo["pipeline"])
-                for bind_group_id, bind_group in enumerate(pinfo["bind_groups"]):
-                    compute_pass.set_bind_group(
-                        bind_group_id, bind_group, [], 0, 999999
-                    )
-                compute_pass.dispatch_workgroups(*pinfo["index_args"])
+        for compute_pipeline_container in compute_pipeline_containers:
+            compute_pipeline_container.dispatch(compute_pass, environment)
 
         compute_pass.end()
 
         # ----- render pipelines
 
-        for pass_index in range(blender.get_pass_count()):
+        # -- process shadow maps
+        lights = (
+            environment.lights["point_lights"]
+            + environment.lights["spot_lights"]
+            + environment.lights["directional_lights"]
+        )
+        render_shadow_maps(lights, wobject_list, command_encoder)
 
-            color_attachments = blender.get_color_attachments(pass_index, clear_color)
+        for pass_index in range(blender.get_pass_count()):
+            color_attachments = blender.get_color_attachments(pass_index)
             depth_attachment = blender.get_depth_attachment(pass_index)
             render_mask = blender.passes[pass_index].render_mask
             if not color_attachments:
                 continue
 
             render_pass = command_encoder.begin_render_pass(
                 color_attachments=color_attachments,
-                depth_stencil_attachment={
-                    **depth_attachment,
-                    "stencil_load_op": wgpu.LoadOp.load,
-                    "stencil_store_op": wgpu.StoreOp.store,
-                },
+                depth_stencil_attachment=depth_attachment,
                 occlusion_query_set=None,
             )
             render_pass.set_viewport(*physical_viewport)
 
-            for wobject, wobject_pipeline in wobject_tuples:
-                if not (render_mask & wobject_pipeline["render_mask"]):
-                    continue
-                for pinfo in wobject_pipeline["render_pipelines"]:
-                    render_pass.set_pipeline(pinfo["pipelines"][pass_index])
-                    for slot, vbuffer in pinfo["vertex_buffers"].items():
-                        render_pass.set_vertex_buffer(
-                            slot,
-                            vbuffer._wgpu_buffer[1],
-                            vbuffer.vertex_byte_range[0],
-                            vbuffer.vertex_byte_range[1],
-                        )
-                    for bind_group_id, bind_group in enumerate(pinfo["bind_groups"]):
-                        render_pass.set_bind_group(bind_group_id, bind_group, [], 0, 99)
-                    # Draw with or without index buffer
-                    if pinfo["index_buffer"] is not None:
-                        ibuffer = pinfo["index_buffer"]
-                        render_pass.set_index_buffer(ibuffer, 0, ibuffer.size)
-                        render_pass.draw_indexed(*pinfo["index_args"])
-                    else:
-                        render_pass.draw(*pinfo["index_args"])
+            for render_pipeline_container in render_pipeline_containers:
+                render_pipeline_container.draw(
+                    render_pass, environment, pass_index, render_mask
+                )
 
             render_pass.end()
 
         return [command_encoder.finish()]
 
-    def _update_stdinfo_buffer(self, camera, physical_size, logical_size):
+    def _update_stdinfo_buffer(self, camera: Camera, physical_size, logical_size):
         # Update the stdinfo buffer's data
-        stdinfo_data = self._shared.stdinfo_buffer.data
-        stdinfo_data["cam_transform"].flat = camera.matrix_world_inverse.elements
-        stdinfo_data["cam_transform_inv"].flat = camera.matrix_world.elements
-        stdinfo_data["projection_transform"].flat = camera.projection_matrix.elements
-        stdinfo_data[
-            "projection_transform_inv"
-        ].flat = camera.projection_matrix_inverse.elements
+        stdinfo_data = self._shared.uniform_buffer.data
+        stdinfo_data["cam_transform"] = camera.world.inverse_matrix.T
+        stdinfo_data["cam_transform_inv"] = camera.world.matrix.T
+        stdinfo_data["projection_transform"] = camera.projection_matrix.T
+        stdinfo_data["projection_transform_inv"] = camera.projection_matrix_inverse.T
         # stdinfo_data["ndc_to_world"].flat = np.linalg.inv(stdinfo_data["cam_transform"] @ stdinfo_data["projection_transform"])
         stdinfo_data["physical_size"] = physical_size
         stdinfo_data["logical_size"] = logical_size
-        stdinfo_data["flipped_winding"] = camera.flips_winding
         # Upload to GPU
-        self._shared.stdinfo_buffer.update_range(0, 1)
-        update_buffer(self._shared.device, self._shared.stdinfo_buffer)
+        self._shared.uniform_buffer.update_range(0, 1)
 
     # Picking
 
     def get_pick_info(self, pos):
         """Get information about the given window location. The given
         pos is a 2D point in logical pixels (with the origin at the
         top-left). Returns a dict with fields:
@@ -670,22 +696,25 @@
         # Prevent out of range and picking before first draw
         out_of_range = not (0 <= float_pos[0] <= 1 and 0 <= float_pos[1] <= 1)
         blender_zero_size = self._blender.size == (0, 0)
         if out_of_range or blender_zero_size:
             return {"rgba": Color(0, 0, 0, 0), "world_object": None}
 
         # Sample
-        encoder = self.device.create_command_encoder()
+        encoder = self._device.create_command_encoder()
         self._copy_pixel(encoder, self._blender.color_tex, float_pos, 0)
         self._copy_pixel(encoder, self._blender.pick_tex, float_pos, 8)
-        queue = self.device.queue
-        queue.submit([encoder.finish()])
+        self._device.queue.submit([encoder.finish()])
 
         # Collect data from the buffer
-        data = self._pixel_info_buffer.map_read()
+        self._pixel_info_buffer.map("read")
+        try:
+            data = self._pixel_info_buffer.read_mapped()
+        finally:
+            self._pixel_info_buffer.unmap()
         color = Color(x / 255 for x in tuple(data[0:4].cast("B")))
         pick_value = tuple(data[8:16].cast("Q"))[0]
         wobject_id = pick_value & 1048575  # 2**20-1
         wobject = id_provider.get_object_from_id(wobject_id)
         # Note: the position in world coordinates is not included because
         # it depends on the camera, but we don't "own" the camera.
 
@@ -696,15 +725,14 @@
 
         if wobject:
             pick_info = wobject._wgpu_get_pick_info(pick_value)
             info.update(pick_info)
         return info
 
     def _copy_pixel(self, encoder, render_texture, float_pos, buf_offset):
-
         # Map position to the texture index
         w, h, d = render_texture.size
         x = max(0, min(w - 1, int(float_pos[0] * w)))
         y = max(0, min(h - 1, int(float_pos[1] * h)))
 
         # Note: bytes_per_row must be a multiple of 256.
         encoder.copy_texture_to_buffer(
@@ -722,21 +750,20 @@
             copy_size=(1, 1, 1),
         )
 
     def snapshot(self):
         """Create a snapshot of the currently rendered image."""
 
         # Prepare
-        device = self._shared.device
         texture = self._blender.color_tex
         size = texture.size
         bytes_per_pixel = 4
 
         # Note, with queue.read_texture the bytes_per_row limitation does not apply.
-        data = device.queue.read_texture(
+        data = self._device.queue.read_texture(
             {
                 "texture": texture,
                 "mip_level": 0,
                 "origin": (0, 0, 0),
             },
             {
                 "offset": 0,
```

### Comparing `pygfx-0.1.9/pygfx/renderers/wgpu/imagerender.py` & `pygfx-0.2.0/pygfx/renderers/wgpu/shaders/imageshader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,26 @@
 import wgpu  # only for flags/enums
 
-from . import register_wgpu_render_function
-from ._shadercomposer import Binding, WorldObjectShader
-from ._utils import to_texture_format
-from ...objects import Image
-from ...materials import ImageBasicMaterial
-from ...resources import Texture, TextureView
+from ....objects import Image
+from ....materials import ImageBasicMaterial
+from ....resources import Texture
+
+from .. import (
+    register_wgpu_render_function,
+    WorldObjectShader,
+    Binding,
+    RenderMask,
+    to_texture_format,
+    GfxSampler,
+    GfxTextureView,
+)
 
 
 vertex_and_fragment = wgpu.ShaderStage.VERTEX | wgpu.ShaderStage.FRAGMENT
 
-
-def handle_colormap(geometry, material, shader):
-    if isinstance(material.map, Texture):
-        raise TypeError("material.map is a Texture, but must be a TextureView")
-    elif not isinstance(material.map, TextureView):
-        raise TypeError("material.map must be a TextureView")
-    # Dimensionality
-    shader["colormap_dim"] = view_dim = material.map.view_dim
-    if material.map.view_dim not in ("1d", "2d", "3d"):
-        raise ValueError("Unexpected colormap texture dimension")
-    # Texture dim matches image channels
-    if int(view_dim[0]) != shader["img_nchannels"]:
-        raise ValueError(
-            f"Image channels {shader['img_nchannels']} does not match material.map {view_dim}"
-        )
-    # Sampling type
-    fmt = to_texture_format(material.map.format)
-    if "norm" in fmt or "float" in fmt:
-        shader["colormap_format"] = "f32"
-    elif "uint" in fmt:
-        shader["colormap_format"] = "u32"
-    else:
-        shader["colormap_format"] = "i32"
-    # Channels
-    shader["colormap_nchannels"] = len(fmt) - len(fmt.lstrip("rgba"))
-    # Return bindinhs
-    return [
-        Binding("s_colormap", "sampler/filtering", material.map, "FRAGMENT"),
-        Binding("t_colormap", "texture/auto", material.map, "FRAGMENT"),
-    ]
-
-
-@register_wgpu_render_function(Image, ImageBasicMaterial)
-def image_renderer(render_info):
-    """Render function capable of rendering images."""
-
-    wobject = render_info.wobject
-    geometry = wobject.geometry
-    material = wobject.material  # noqa
-    shader = ImageShader(render_info, climcorrection="")
-
-    bindings = [
-        Binding("u_stdinfo", "buffer/uniform", render_info.stdinfo_uniform),
-        Binding("u_wobject", "buffer/uniform", wobject.uniform_buffer),
-        Binding("u_material", "buffer/uniform", material.uniform_buffer),
-    ]
-
-    topology = wgpu.PrimitiveTopology.triangle_strip
-    n = 4
-
-    # Collect texture and sampler
-    if geometry.grid is None:
-        raise ValueError("Image.geometry must have a grid (texture).")
-    else:
-        if isinstance(geometry.grid, TextureView):
-            view = geometry.grid
-        elif isinstance(geometry.grid, Texture):
-            view = geometry.grid.get_view(filter="linear")
-        else:
-            raise TypeError("Image.geometry.grid must be a Texture or TextureView")
-        if view.view_dim.lower() != "2d":
-            raise TypeError("Image.geometry.grid must a 2D texture (view)")
-        # Sampling type
-        fmt = to_texture_format(geometry.grid.format)
-        if "norm" in fmt or "float" in fmt:
-            shader["img_format"] = "f32"
-            if "unorm" in fmt:
-                shader["climcorrection"] = " * 255.0"
-            elif "snorm" in fmt:
-                shader["climcorrection"] = " * 255.0 - 128.0"
-        elif "uint" in fmt:
-            shader["img_format"] = "u32"
-        else:
-            shader["img_format"] = "i32"
-        # Channels
-        shader["img_nchannels"] = len(fmt) - len(fmt.lstrip("rgba"))
-
-    bindings.append(Binding("s_img", "sampler/filtering", view, "FRAGMENT"))
-    bindings.append(Binding("t_img", "texture/auto", view, vertex_and_fragment))
-
-    # If a colormap is applied ...
-    if material.map is not None:
-        bindings.extend(handle_colormap(geometry, material, shader))
-
-    # Let the shader generate code for our bindings
-    for i, binding in enumerate(bindings):
-        shader.define_binding(0, i, binding)
-
-    # Get in what passes this needs rendering
-    suggested_render_mask = 3
-    if material.opacity < 1:
-        suggested_render_mask = 2
-    if material.map is not None:
-        if shader["colormap_nchannels"] in (1, 3):
-            suggested_render_mask = 1
-    else:
-        if shader["img_nchannels"] in (1, 3):
-            suggested_render_mask = 1
-
-    # Put it together!
-    return [
-        {
-            "suggested_render_mask": suggested_render_mask,
-            "render_shader": shader,
-            "primitive_topology": topology,
-            "indices": (range(n), range(1)),
-            "vertex_buffers": {},
-            "bindings0": bindings,
-        }
-    ]
-
-
 sampled_value_to_color = """
         fn sampled_value_to_color(value_rgba: vec4<f32>) -> vec4<f32> {
 
             // Make it the correct dimension
             $$ if img_nchannels == 1
                 let value_raw = value_rgba.r;
             $$ elif img_nchannels == 2
@@ -159,15 +54,15 @@
 
             return color;
         }
 """
 
 
 class BaseImageShader(WorldObjectShader):
-    def image_helpers(self):
+    def code_image_helpers(self):
         return (
             sampled_value_to_color
             + """
         struct ImGeometry {
             indices: array<i32,6>,
             positions: array<vec3<f32>,4>,
             texcoords: array<vec2<f32>,4>,
@@ -206,33 +101,123 @@
                 return vec4<f32>(textureLoad(t_img, texcoords_u, 0));
             $$ endif
         }
     """
         )
 
 
+@register_wgpu_render_function(Image, ImageBasicMaterial)
 class ImageShader(BaseImageShader):
+    type = "render"
+
+    def get_bindings(self, wobject, shared):
+        geometry = wobject.geometry
+        material = wobject.material  # noqa
+
+        bindings = [
+            Binding("u_stdinfo", "buffer/uniform", shared.uniform_buffer),
+            Binding("u_wobject", "buffer/uniform", wobject.uniform_buffer),
+            Binding("u_material", "buffer/uniform", material.uniform_buffer),
+        ]
+
+        self["climcorrection"] = ""
+
+        # Collect texture and sampler
+        if geometry.grid is None:
+            raise ValueError("Image.geometry must have a grid (texture).")
+        else:
+            if not isinstance(geometry.grid, Texture):
+                raise TypeError("Image.geometry.grid must be a Texture.")
+            if geometry.grid.dim != 2:
+                raise TypeError("Image.geometry.grid must a 2D texture")
+            tex_view = GfxTextureView(geometry.grid)
+            sampler = GfxSampler(material.interpolation, "clamp")
+            self["colorspace"] = geometry.grid.colorspace
+            # Sampling type
+            fmt = to_texture_format(geometry.grid.format)
+            if "norm" in fmt or "float" in fmt:
+                self["img_format"] = "f32"
+                if "unorm" in fmt:
+                    self["climcorrection"] = " * 255.0"
+                elif "snorm" in fmt:
+                    self["climcorrection"] = " * 255.0 - 128.0"
+            elif "uint" in fmt:
+                self["img_format"] = "u32"
+            else:
+                self["img_format"] = "i32"
+            # Channels
+            self["img_nchannels"] = len(fmt) - len(fmt.lstrip("rgba"))
+
+        bindings.append(Binding("s_img", "sampler/filtering", sampler, "FRAGMENT"))
+        bindings.append(Binding("t_img", "texture/auto", tex_view, vertex_and_fragment))
+
+        # If a colormap is applied ...
+        if material.map is not None:
+            bindings.extend(
+                self.define_img_colormap(material.map, material.map_interpolation)
+            )
+            self["colorspace"] = material.map.colorspace
+
+        bindings = {i: b for i, b in enumerate(bindings)}
+        self.define_bindings(0, bindings)
+
+        return {
+            0: bindings,
+        }
+
+    def get_pipeline_info(self, wobject, shared):
+        return {
+            "primitive_topology": wgpu.PrimitiveTopology.triangle_strip,
+            "cull_mode": wgpu.CullMode.none,
+        }
+
+    def get_render_info(self, wobject, shared):
+        material = wobject.material
+
+        render_mask = 0
+        if wobject.render_mask:
+            render_mask = wobject.render_mask
+        elif material.is_transparent:
+            render_mask = RenderMask.transparent
+        else:
+            # Determine what passes are needed
+            if material.map is not None:
+                if self["colormap_nchannels"] in (1, 3):
+                    render_mask |= RenderMask.opaque
+                else:
+                    render_mask |= RenderMask.all
+            else:
+                if self["img_nchannels"] in (1, 3):
+                    render_mask |= RenderMask.opaque
+                else:
+                    render_mask |= RenderMask.all
+
+        return {
+            "indices": (4, 1),
+            "render_mask": render_mask,
+        }
+
     def get_code(self):
         return (
-            self.get_definitions()
-            + self.common_functions()
-            + self.image_helpers()
-            + self.vertex_shader()
-            + self.fragment_shader()
+            self.code_definitions()
+            + self.code_common()
+            + self.code_image_helpers()
+            + self.code_vertex()
+            + self.code_fragment()
         )
 
-    def vertex_shader(self):
+    def code_vertex(self):
         return """
 
         struct VertexInput {
             @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        @stage(vertex)
+        @vertex
         fn vs_main(in: VertexInput) -> Varyings {
 
             var geo = get_im_geometry();
 
             // Select what face we're at
             let index = i32(in.vertex_index);
             let i0 = geo.indices[index];
@@ -246,35 +231,41 @@
             varyings.position = vec4<f32>(ndc_pos);
             varyings.world_pos = vec3<f32>(world_pos.xyz);
             varyings.texcoord = vec2<f32>(geo.texcoords[i0]);
             return varyings;
         }
         """
 
-    def fragment_shader(self):
+    def code_fragment(self):
         return """
 
-        @stage(fragment)
+        @fragment
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             let sizef = vec2<f32>(textureDimensions(t_img));
             let value = sample_im(varyings.texcoord.xy, sizef);
             let color = sampled_value_to_color(value);
-            let albeido = color.rgb;
 
-            let final_color = vec4<f32>(albeido, color.a * u_material.opacity);
+            // Move to physical colorspace (linear photon count) so we can do math
+            $$ if colorspace == 'srgb'
+                let physical_color = srgb2physical(color.rgb);
+            $$ else
+                let physical_color = color.rgb;
+            $$ endif
+            let opacity = color.a * u_material.opacity;
+            let out_color = vec4<f32>(physical_color, opacity);
 
             // Wrap up
             apply_clipping_planes(varyings.world_pos);
-            var out = get_fragment_output(varyings.position.z, final_color);
+            var out = get_fragment_output(varyings.position.z, out_color);
 
             $$ if write_pick
             // The wobject-id must be 20 bits. In total it must not exceed 64 bits.
             out.pick = (
                 pick_pack(u32(u_wobject.id), 20) +
-                pick_pack(u32(varyings.texcoord.x * 4194304.0), 22) +
-                pick_pack(u32(varyings.texcoord.y * 4194304.0), 22)
+                pick_pack(u32(varyings.texcoord.x * 4194303.0), 22) +
+                pick_pack(u32(varyings.texcoord.y * 4194303.0), 22)
             );
             $$ endif
 
             return out;
         }
         """
```

### Comparing `pygfx-0.1.9/pygfx/renderers/wgpu/meshrender.py` & `pygfx-0.2.0/pygfx/renderers/wgpu/shaders/volumeshader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,756 +1,632 @@
 import wgpu  # only for flags/enums
 
-from . import register_wgpu_render_function
-from ._shadercomposer import Binding, WorldObjectShader
-from .pointsrender import handle_colormap
-from ...objects import Mesh, InstancedMesh
-from ...materials import (
-    MeshBasicMaterial,
-    MeshPhongMaterial,
-    MeshFlatMaterial,
-    MeshNormalMaterial,
-    MeshNormalLinesMaterial,
-    MeshSliceMaterial,
+from ....objects import Volume
+from ....materials import VolumeSliceMaterial, VolumeRayMaterial
+from ....resources import Texture
+
+from .. import (
+    register_wgpu_render_function,
+    WorldObjectShader,
+    Binding,
+    RenderMask,
+    to_texture_format,
+    GfxSampler,
+    GfxTextureView,
 )
-from ...resources import Buffer
-from ...utils import normals_from_vertices
 
+from .imageshader import sampled_value_to_color
 
-@register_wgpu_render_function(Mesh, MeshBasicMaterial)
-def mesh_renderer(render_info):
-    """Render function capable of rendering meshes."""
-    wobject = render_info.wobject
-    geometry = wobject.geometry
-    material = wobject.material  # noqa
-
-    # Initialize
-    topology = wgpu.PrimitiveTopology.triangle_list
-    shader = MeshShader(
-        render_info,
-        lighting="",
-        colormap_format="f32",
-        instanced=False,
-        wireframe=material.wireframe,
-        vertex_color_channels=0,
-    )
-
-    # We're assuming the presence of an index buffer for now
-    assert getattr(geometry, "indices", None)
-    n = geometry.indices.data.size
-
-    # Normals. Usually it'd be given. If not, we'll calculate it from the vertices.
-    if getattr(geometry, "normals", None) is not None:
-        normal_buffer = geometry.normals
-    else:
-        normal_data = normals_from_vertices(
-            geometry.positions.data, geometry.indices.data
-        )
-        normal_buffer = Buffer(normal_data)
 
-    # We're using storage buffers for everything; no vertex nor index buffers.
-    vertex_buffers = {}
-    index_buffer = None
-
-    # Init bindings
-    bindings = [
-        Binding("u_stdinfo", "buffer/uniform", render_info.stdinfo_uniform),
-        Binding("u_wobject", "buffer/uniform", wobject.uniform_buffer),
-        Binding("u_material", "buffer/uniform", material.uniform_buffer),
-        Binding("s_indices", "buffer/read_only_storage", geometry.indices, "VERTEX"),
-        Binding(
-            "s_positions", "buffer/read_only_storage", geometry.positions, "VERTEX"
-        ),
-        Binding("s_normals", "buffer/read_only_storage", normal_buffer, "VERTEX"),
-    ]
-    bindings1 = []  # non-auto-generated bindings
-
-    # Per-vertex color, colormap, or a plane color?
-    shader["color_mode"] = "uniform"
-    if material.vertex_colors:
-        shader["color_mode"] = "vertex"
-        shader["vertex_color_channels"] = nchannels = geometry.colors.data.shape[1]
-        if nchannels not in (1, 2, 3, 4):
-            raise ValueError(f"Geometry.colors needs 1-4 columns, not {nchannels}")
-        bindings.append(
-            Binding("s_colors", "buffer/read_only_storage", geometry.colors, "VERTEX")
-        )
-    elif material.map is not None:
-        shader["color_mode"] = "map"
-        bindings.extend(handle_colormap(geometry, material, shader))
-
-    # Triage based on material
-    if isinstance(material, MeshNormalMaterial):
-        # Special simple fragment shader
-        shader["color_mode"] = "normal"
-        shader["colormap_dim"] = ""  # disable texture if there happens to be one
-    elif isinstance(material, MeshNormalLinesMaterial):
-        # Special simple vertex shader with plain fragment shader
-        topology = wgpu.PrimitiveTopology.line_list
-        shader.vertex_shader = shader.vertex_shader_normal_lines
-        index_buffer = None
-        n = geometry.positions.nitems * 2
-        shader["color_mode"] = "uniform"
-        shader["lighting"] = ""
-        shader["wireframe"] = False
-    elif isinstance(material, MeshFlatMaterial):
-        shader["lighting"] = "flat"
-    elif isinstance(material, MeshPhongMaterial):
-        shader["lighting"] = "phong"
-    else:
-        pass  # simple lighting
-
-    # Instanced meshes have an extra storage buffer that we add manually
-    n_instances = 1
-    if isinstance(wobject, InstancedMesh):
-        shader["instanced"] = True
-        bindings1.append(
-            Binding(
-                "s_instance_infos",
-                "buffer/read_only_storage",
-                wobject.instance_infos,
-                "VERTEX",
-            )
-        )
-        n_instances = wobject.instance_infos.nitems
+vertex_and_fragment = wgpu.ShaderStage.VERTEX | wgpu.ShaderStage.FRAGMENT
 
-    # Determine culling
-    if material.side == "FRONT":
-        cull_mode = wgpu.CullMode.back
-    elif material.side == "BACK":
-        cull_mode = wgpu.CullMode.front
-    else:  # material.side == "BOTH"
-        cull_mode = wgpu.CullMode.none
-
-    # Let the shader generate code for our bindings
-    for i, binding in enumerate(bindings):
-        shader.define_binding(0, i, binding)
-
-    # Determine in what render passes this objects must be rendered
-    suggested_render_mask = 3
-    if material.opacity < 1:
-        suggested_render_mask = 2
-    elif shader["color_mode"] == "vertex":
-        if shader["vertex_color_channels"] in (1, 3):
-            suggested_render_mask = 1
-    elif shader["color_mode"] == "map":
-        if shader["colormap_nchannels"] in (1, 3):
-            suggested_render_mask = 1
-    elif shader["color_mode"] == "normal":
-        suggested_render_mask = 1
-    elif shader["color_mode"] == "uniform":
-        suggested_render_mask = 1 if material.color[3] >= 1 else 2
-    else:
-        raise RuntimeError(f"Unexpected color mode {shader['color_mode']}")
-
-    # Put it together!
-    return [
-        {
-            "suggested_render_mask": suggested_render_mask,
-            "render_shader": shader,
-            "primitive_topology": topology,
-            "cull_mode": cull_mode,
-            "indices": (range(n), range(n_instances)),
-            "index_buffer": index_buffer,
-            "vertex_buffers": vertex_buffers,
-            "bindings0": bindings,
-            "bindings1": bindings1,
-        }
-    ]
 
+class BaseVolumeShader(WorldObjectShader):
+    def get_bindings(self, wobject, shared):
+        geometry = wobject.geometry
+        material = wobject.material  # noqa
+
+        bindings = [
+            Binding("u_stdinfo", "buffer/uniform", shared.uniform_buffer),
+            Binding("u_wobject", "buffer/uniform", wobject.uniform_buffer),
+            Binding("u_material", "buffer/uniform", material.uniform_buffer),
+        ]
+
+        # Collect texture and sampler
+        if geometry.grid is None:
+            raise ValueError("Volume.geometry must have a grid (texture).")
+        if not isinstance(geometry.grid, Texture):
+            raise TypeError("Volume.geometry.grid must be a Texture")
+        if geometry.grid.dim != 3:
+            raise TypeError("Volume.geometry.grid must a 3D texture (view)")
+
+        tex_view = GfxTextureView(geometry.grid)
+        sampler = GfxSampler(material.interpolation, "clamp")
+        self["colorspace"] = geometry.grid.colorspace
+
+        # Sampling type
+        self["climcorrection"] = ""
+        fmt = to_texture_format(geometry.grid.format)
+        if "norm" in fmt or "float" in fmt:
+            self["img_format"] = "f32"
+            if "unorm" in fmt:
+                self["climcorrection"] = " * 255.0"
+            elif "snorm" in fmt:
+                self["climcorrection"] = " * 255.0 - 128.0"
+        elif "uint" in fmt:
+            self["img_format"] = "u32"
+        else:
+            self["img_format"] = "i32"
+
+        # Channels
+        self["img_nchannels"] = len(fmt) - len(fmt.lstrip("rgba"))
+
+        bindings.append(Binding("s_img", "sampler/filtering", sampler, "FRAGMENT"))
+        bindings.append(Binding("t_img", "texture/auto", tex_view, vertex_and_fragment))
+
+        # If a colormap is applied ...
+        if material.map is not None:
+            bindings.extend(
+                self.define_img_colormap(material.map, material.map_interpolation)
+            )
+            self["colorspace"] = material.map.colorspace
 
-class MeshShader(WorldObjectShader):
-    def get_code(self):
-        return (
-            self.get_definitions()
-            + self.common_functions()
-            + self.helpers()
-            + self.vertex_shader()
-            + self.fragment_shader()
-        )
+        bindings = {i: b for i, b in enumerate(bindings)}
+        self.define_bindings(0, bindings)
 
-    def vertex_shader(self):
-        return """
+        return {
+            0: bindings,
+        }
 
-        struct VertexInput {
-            @builtin(vertex_index) vertex_index : u32,
-            $$ if instanced
-            @builtin(instance_index) instance_index : u32,
-            $$ endif
+    def code_volume_helpers(self):
+        return (
+            sampled_value_to_color
+            + """
+        struct VolGeometry {
+            indices: array<i32,36>,
+            positions: array<vec3<f32>,8>,
+            texcoords: array<vec3<f32>,8>,
         };
 
-        $$ if instanced
-        struct InstanceInfo {
-            transform: mat4x4<f32>,
-            id: u32,
-        };
-        @group(1) @binding(0)
-        var<storage,read> s_instance_infos: array<InstanceInfo>;
-        $$ endif
+        fn get_vol_geometry() -> VolGeometry {
+            let size = textureDimensions(t_img);
+            var geo: VolGeometry;
+
+            geo.indices = array<i32,36>(
+                0, 1, 2,   3, 2, 1,   4, 5, 6,   7, 6, 5,   6, 7, 3,   2, 3, 7,
+                1, 0, 4,   5, 4, 0,   5, 0, 7,   2, 7, 0,   1, 4, 3,   6, 3, 4,
+            );
 
+            let pos1 = vec3<f32>(-0.5);
+            let pos2 = vec3<f32>(size) + pos1;
+            geo.positions = array<vec3<f32>,8>(
+                vec3<f32>(pos2.x, pos1.y, pos2.z),
+                vec3<f32>(pos2.x, pos1.y, pos1.z),
+                vec3<f32>(pos2.x, pos2.y, pos2.z),
+                vec3<f32>(pos2.x, pos2.y, pos1.z),
+                vec3<f32>(pos1.x, pos1.y, pos1.z),
+                vec3<f32>(pos1.x, pos1.y, pos2.z),
+                vec3<f32>(pos1.x, pos2.y, pos1.z),
+                vec3<f32>(pos1.x, pos2.y, pos2.z),
+            );
 
-        @stage(vertex)
-        fn vs_main(in: VertexInput) -> Varyings {
+            geo.texcoords = array<vec3<f32>,8>(
+                vec3<f32>(1.0, 0.0, 1.0),
+                vec3<f32>(1.0, 0.0, 0.0),
+                vec3<f32>(1.0, 1.0, 1.0),
+                vec3<f32>(1.0, 1.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 1.0),
+                vec3<f32>(0.0, 1.0, 0.0),
+                vec3<f32>(0.0, 1.0, 1.0),
+            );
 
-            // Select what face we're at
-            let index = i32(in.vertex_index);
-            let face_index = index / 3;
-            var sub_index = index % 3;
+            return geo;
+        }
 
-            // If the camera flips a dimension, it flips the face winding.
-            // We can correct for this by adjusting the order (sub_index) here.
-            sub_index = select(sub_index, -1 * (sub_index - 1) + 1, u_stdinfo.flipped_winding > 0);
-
-            // Sample
-            let ii = load_s_indices(face_index);
-            let i0 = i32(ii[sub_index]);
-
-            // Get world transform
-            $$ if instanced
-                let instance_info = s_instance_infos[in.instance_index];
-                let world_transform = u_wobject.world_transform * instance_info.transform;
+        fn sample_vol(texcoord: vec3<f32>, sizef: vec3<f32>) -> vec4<f32> {
+            $$ if img_format == 'f32'
+                return textureSample(t_img, s_img, texcoord.xyz);
             $$ else
-                let world_transform = u_wobject.world_transform;
-            $$ endif
-
-            // Get vertex position
-            let raw_pos = load_s_positions(i0);
-            let world_pos = world_transform * vec4<f32>(raw_pos, 1.0);
-            var ndc_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * world_pos;
-
-            // For the wireframe we also need the ndc_pos of the other vertices of this face
-            $$ if wireframe
-                $$ for i in (1, 2, 3)
-                    let raw_pos{{ i }} = load_s_positions(i32(ii[{{ i - 1 }}]));
-                    let world_pos{{ i }} = world_transform * vec4<f32>(raw_pos{{ i }}, 1.0);
-                    let ndc_pos{{ i }} = u_stdinfo.projection_transform * u_stdinfo.cam_transform * world_pos{{ i }};
-                $$ endfor
-                let depth_offset = -0.0001;  // to put the mesh slice atop a mesh
-                ndc_pos.z = ndc_pos.z + depth_offset;
-            $$ endif
-
-            // Prepare output
-            var varyings: Varyings;
-
-            // Set position
-            varyings.world_pos = vec3<f32>(world_pos.xyz / world_pos.w);
-            varyings.position = vec4<f32>(ndc_pos.xyz, ndc_pos.w);
-
-            // Per-vertex colors
-            $$ if vertex_color_channels == 1
-            let cvalue = load_s_colors(i0);
-            varyings.color = vec4<f32>(cvalue, cvalue, cvalue, 1.0);
-            $$ elif vertex_color_channels == 2
-            let cvalue = load_s_colors(i0);
-            varyings.color = vec4<f32>(cvalue.r, cvalue.r, cvalue.r, cvalue.g);
-            $$ elif vertex_color_channels == 3
-            varyings.color = vec4<f32>(load_s_colors(i0), 1.0);
-            $$ elif vertex_color_channels == 4
-            varyings.color = vec4<f32>(load_s_colors(i0));
+                let texcoords_u = vec3<i32>(texcoord.xyz * sizef);
+                return vec4<f32>(textureLoad(t_img, texcoords_u, 0));
             $$ endif
+        }
 
-            // Set texture coords
-            $$ if colormap_dim == '1d'
-            varyings.texcoord = f32(load_s_texcoords(i0));
-            $$ elif colormap_dim == '2d'
-            varyings.texcoord = vec2<f32>(load_s_texcoords(i0));
-            $$ elif colormap_dim == '3d'
-            varyings.texcoord = vec3<f32>(load_s_texcoords(i0));
-            $$ endif
+    """
+        )
 
-            // Set the normal
-            let raw_normal = load_s_normals(i0);
-            let world_pos_n = world_transform * vec4<f32>(raw_pos + raw_normal, 1.0);
-            let world_normal = normalize(world_pos_n - world_pos).xyz;
-            varyings.normal = vec3<f32>(world_normal);
-
-            // Vectors for lighting, all in world coordinates
-            let view_vec = normalize(ndc_to_world_pos(vec4<f32>(0.0, 0.0, 1.0, 1.0)));
-            varyings.view = vec3<f32>(view_vec);
-            varyings.light = vec3<f32>(view_vec);
-
-            // Set wireframe barycentric-like coordinates
-            $$ if wireframe
-                $$ for i in (1, 2, 3)
-                    let p{{ i }} = (ndc_pos{{ i }}.xy / ndc_pos{{ i }}.w) * u_stdinfo.logical_size * 0.5;
-                $$ endfor
-                let dist1 = abs((p3.x - p2.x) * (p2.y - p1.y) - (p2.x - p1.x) * (p3.y - p2.y)) / distance(p2, p3);
-                let dist2 = abs((p3.x - p1.x) * (p1.y - p2.y) - (p1.x - p2.x) * (p3.y - p1.y)) / distance(p1, p3);
-                let dist3 = abs((p1.x - p2.x) * (p2.y - p3.y) - (p2.x - p3.x) * (p1.y - p2.y)) / distance(p2, p1);
-                var arr_wireframe_coords = array<vec3<f32>, 3>(
-                    vec3<f32>(dist1, 0.0, 0.0), vec3<f32>(0.0, dist2, 0.0), vec3<f32>(0.0, 0.0, dist3)
-                );
-                varyings.wireframe_coords = vec3<f32>(arr_wireframe_coords[sub_index]);  // in logical pixels
-            $$ endif
 
-            // Set varyings for picking. We store the face_index, and 3 weights
-            // that indicate how close the fragment is to each vertex (barycentric
-            // coordinates). This allows the selection of the nearest vertex or edge.
-            $$ if instanced
-                let pick_id = instance_info.id;
-            $$ else
-                let pick_id = u_wobject.id;
-            $$ endif
+@register_wgpu_render_function(Volume, VolumeSliceMaterial)
+class VolumeSliceShader(BaseVolumeShader):
+    type = "render"
+
+    def get_pipeline_info(self, wobject, shared):
+        return {
+            "primitive_topology": wgpu.PrimitiveTopology.triangle_list,
+            "cull_mode": wgpu.CullMode.none,
+        }
 
-            varyings.pick_id = u32(pick_id);
-            varyings.pick_idx = u32(face_index);
-            var arr_pick_coords = array<vec3<f32>, 3>(vec3<f32>(1.0, 0.0, 0.0), vec3<f32>(0.0, 1.0, 0.0), vec3<f32>(0.0, 0.0, 1.0));
-            varyings.pick_coords = vec3<f32>(arr_pick_coords[sub_index]);
+    def get_render_info(self, wobject, shared):
+        material = wobject.material
 
-            return varyings;
+        render_mask = 0
+        if wobject.render_mask:
+            render_mask = wobject.render_mask
+        elif material.is_transparent:
+            render_mask = RenderMask.transparent
+        else:
+            # Determine what passes are needed
+            if material.map is not None:
+                if self["colormap_nchannels"] in (1, 3):
+                    render_mask |= RenderMask.opaque
+                else:
+                    render_mask |= RenderMask.all
+            else:
+                if self["img_nchannels"] in (1, 3):
+                    render_mask |= RenderMask.opaque
+                else:
+                    render_mask |= RenderMask.all
+
+        return {
+            "indices": (12, 1),
+            "render_mask": render_mask,
         }
 
-    """
+    def get_code(self):
+        return (
+            self.code_definitions()
+            + self.code_common()
+            + self.code_volume_helpers()
+            + self.code_vertex()
+            + self.code_fragment()
+        )
 
-    def vertex_shader_normal_lines(self):
+    def code_vertex(self):
         return """
 
         struct VertexInput {
             @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        @stage(vertex)
+        @vertex
         fn vs_main(in: VertexInput) -> Varyings {
-            let index = i32(in.vertex_index);
-            let r = index % 2;
-            let i0 = (index - r) / 2;
 
-            let raw_pos = load_s_positions(i0);
-            let raw_normal = load_s_normals(i0);
+            // Our geometry is implicitly defined by the volume dimensions.
+            var geo = get_vol_geometry();
 
-            let world_pos1 = u_wobject.world_transform * vec4<f32>(raw_pos, 1.0);
-            let world_pos2 = u_wobject.world_transform * vec4<f32>(raw_pos + raw_normal, 1.0);
+            // This layout is like this:
+            //
+            //   Vertices       Planes (right, left, back, front, top, bottom)
+            //                            0      1    2      3     4     5
+            //
+            //    5----0        0: 0231        +----+
+            //   /|   /|        1: 7546       /|24 /|
+            //  7----2 |        2: 5014      +----+ |0
+            //  | 4--|-1        3: 2763     1| +--|-+
+            //  |/   |/         4: 0572      |/35 |/
+            //  6----3          5: 3641      +----+
 
-            // The normal is sized in world coordinates
-            let world_normal = normalize(world_pos2 - world_pos1);
+            let plane = u_material.plane.xyzw;  // ax + by + cz + d
+            let n = plane.xyz;
 
-            let amplitude = 1.0;
-            let world_pos = world_pos1 + f32(r) * world_normal * amplitude;
-            let ndc_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * world_pos;
+            // Define edges (using vertex indices), and their matching plane
+            // indices (each edge touches two planes). Note that these need to
+            // match the above figure, and that needs to match with the actual
+            // BoxGeometry implementation!
+            var edges = array<vec2<i32>,12>(
+                vec2<i32>(0, 2), vec2<i32>(2, 3), vec2<i32>(3, 1), vec2<i32>(1, 0),
+                vec2<i32>(4, 6), vec2<i32>(6, 7), vec2<i32>(7, 5), vec2<i32>(5, 4),
+                vec2<i32>(5, 0), vec2<i32>(1, 4), vec2<i32>(2, 7), vec2<i32>(6, 3),
+            );
+            var ed2pl = array<vec2<i32>,12>(
+                vec2<i32>(0, 4), vec2<i32>(0, 3), vec2<i32>(0, 5), vec2<i32>(0, 2),
+                vec2<i32>(1, 5), vec2<i32>(1, 3), vec2<i32>(1, 4), vec2<i32>(1, 2),
+                vec2<i32>(2, 4), vec2<i32>(2, 5), vec2<i32>(3, 4), vec2<i32>(3, 5),
+            );
 
-            var varyings: Varyings;
-            varyings.world_pos = vec3<f32>(world_pos.xyz / world_pos.w);
-            varyings.position = vec4<f32>(ndc_pos);
+            // Init intersection info
+            var intersect_flags = array<i32,12>(0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0);
+            var intersect_positions = array<vec3<f32>,12>(
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+            );
+            var intersect_texcoords = array<vec3<f32>,12>(
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0), vec3<f32>(0.0, 0.0, 0.0),
+            );
+
+            // Intersect the 12 edges
+            for (var i:i32=0; i<12; i=i+1) {
+                let edge = edges[i];
+                let p1_raw = geo.positions[ edge[0] ];
+                let p2_raw = geo.positions[ edge[1] ];
+                let p1_p = u_wobject.world_transform * vec4<f32>(p1_raw, 1.0);
+                let p2_p = u_wobject.world_transform * vec4<f32>(p2_raw, 1.0);
+                let p1 = p1_p.xyz / p1_p.w;
+                let p2 = p2_p.xyz / p2_p.w;
+                let tc1 = geo.texcoords[ edge[0] ];
+                let tc2 = geo.texcoords[ edge[1] ];
+                let u = p2 - p1;
+                let t = -(plane.x * p1.x + plane.y * p1.y + plane.z * p1.z + plane.w) / dot(n, u);
+                let intersects:bool = t > 0.0 && t < 1.0;
+                intersect_flags[i] = select(0, 1, intersects);
+                intersect_positions[i] = mix(p1, p2, vec3<f32>(t, t, t));
+                intersect_texcoords[i] = mix(tc1, tc2, vec3<f32>(t, t, t));
+            }
 
-            // Stub varyings, because the mesh varyings are based on face index
-            varyings.pick_id = u32(u_wobject.id);
-            varyings.pick_idx = u32(0);
-            varyings.pick_coords = vec3<f32>(0.0);
+            // Init six vertices
+            var vertices = array<vec3<f32>,6>(
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+            );
+            var texcoords = array<vec3<f32>,6>(
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+                vec3<f32>(0.0, 0.0, 0.0),
+            );
 
+            // Find first intersection point. This can be any valid intersection.
+            // In ed2pl[i][0], the 0 could also be a one. It would mean that we'd
+            // move around the box in the other direction.
+            var plane_index: i32 = 0;
+            var i:i32;
+            for (i=0; i<12; i=i+1) {
+                if (intersect_flags[i] == 1) {
+                    plane_index = ed2pl[i][0];
+                    vertices[0] = intersect_positions[i];
+                    texcoords[0] = intersect_texcoords[i];
+                    break;
+                }
+            }
+
+            // From there take (at most) 5 steps
+            let i_start: i32 = i;
+            var i_last: i32 = i;
+            var max_iter: i32 = 6;
+            for (var iter:i32=1; iter<max_iter; iter=iter+1) {
+                for (var i:i32=0; i<12; i=i+1) {
+                    if (i != i_last && intersect_flags[i] == 1) {
+                        if (ed2pl[i][0] == plane_index) {
+                            vertices[iter] = intersect_positions[i];
+                            texcoords[iter] = intersect_texcoords[i];
+                            plane_index = ed2pl[i][1];
+                            i_last = i;
+                            break;
+                        } else if (ed2pl[i][1] == plane_index) {
+                            vertices[iter] = intersect_positions[i];
+                            texcoords[iter] = intersect_texcoords[i];
+                            plane_index = ed2pl[i][0];
+                            i_last = i;
+                            break;
+                        }
+                    }
+                }
+                if (i_last == i_start) {
+                    max_iter = iter;
+                    break;
+                }
+            }
+
+            // Make the rest degenerate triangles
+            for (var i:i32=max_iter; i<6; i=i+1) {
+                vertices[i] = vertices[0];
+            }
+
+            // Now select the current vertex. We mimic a triangle fan with a triangle list.
+            // This works whether the number of vertices/intersections is 3, 4, 5, and 6.
+            let index = i32(in.vertex_index);
+            var indexmap = array<i32,12>(0, 1, 2, 0, 2, 3, 0, 3, 4, 0, 4, 5);
+            let world_pos = vertices[ indexmap[index] ];
+            let ndc_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * vec4<f32>(world_pos, 1.0);
+
+            var varyings : Varyings;
+            varyings.position = vec4<f32>(ndc_pos);
+            varyings.world_pos = vec3<f32>(world_pos);
+            varyings.texcoord = vec3<f32>(texcoords[ indexmap[index] ]);
             return varyings;
         }
         """
 
-    def fragment_shader(self):
+    def code_fragment(self):
         return """
 
-        @stage(fragment)
-        fn fs_main(varyings: Varyings, @builtin(front_facing) is_front: bool) -> FragmentOutput {
-
-            $$ if color_mode == 'vertex'
-                let color_value = varyings.color;
-                let albeido = color_value.rgb;
-            $$ elif color_mode == 'map'
-                let color_value = sample_colormap(varyings.texcoord);
-                let albeido = color_value.rgb;  // no more colormap
-            $$ elif color_mode == 'normal'
-                let albeido = normalize(varyings.normal.xyz) * 0.5 + 0.5;
-                let color_value = vec4<f32>(albeido, 1.0);
-            $$ else
-                let color_value = u_material.color;
-                let albeido = color_value.rgb;
-            $$ endif
-
-            // Lighting
-            $$ if lighting
-                let world_pos = varyings.world_pos;
-                let lit_color = lighting_{{ lighting }}(is_front, varyings.world_pos, varyings.normal, varyings.light, varyings.view, albeido);
+        @fragment
+        fn fs_main(varyings: Varyings) -> FragmentOutput {
+            let sizef = vec3<f32>(textureDimensions(t_img));
+            let value = sample_vol(varyings.texcoord.xyz, sizef);
+            let color = sampled_value_to_color(value);
+
+            // Move to physical colorspace (linear photon count) so we can do math
+            $$ if colorspace == 'srgb'
+                let physical_color = srgb2physical(color.rgb);
             $$ else
-                let lit_color = albeido;
+                let physical_color = color.rgb;
             $$ endif
-
-            $$ if wireframe
-                let distance_from_edge = min(varyings.wireframe_coords.x, min(varyings.wireframe_coords.y, varyings.wireframe_coords.z));
-                if (distance_from_edge > 0.5 * u_material.wireframe) {
-                    discard;
-                }
-            $$ endif
-
-            let final_color = vec4<f32>(lit_color, color_value.a * u_material.opacity);
+            let opacity = color.a * u_material.opacity;
+            let out_color = vec4<f32>(physical_color, opacity);
 
             // Wrap up
-
             apply_clipping_planes(varyings.world_pos);
-            var out = get_fragment_output(varyings.position.z, final_color);
+            var out = get_fragment_output(varyings.position.z, out_color);
 
             $$ if write_pick
             // The wobject-id must be 20 bits. In total it must not exceed 64 bits.
             out.pick = (
-                pick_pack(varyings.pick_id, 20) +
-                pick_pack(varyings.pick_idx, 26) +
-                pick_pack(u32(varyings.pick_coords.x * 64.0), 6) +
-                pick_pack(u32(varyings.pick_coords.y * 64.0), 6) +
-                pick_pack(u32(varyings.pick_coords.z * 64.0), 6)
+                pick_pack(u32(u_wobject.id), 20) +
+                pick_pack(u32(varyings.texcoord.x * 16383.0), 14) +
+                pick_pack(u32(varyings.texcoord.y * 16383.0), 14) +
+                pick_pack(u32(varyings.texcoord.z * 16383.0), 14)
             );
             $$ endif
 
             return out;
         }
 
         """
 
-    def helpers(self):
-        return """
-
-        $$ if lighting
-        fn lighting_phong(
-            is_front: bool,
-            world_pos: vec3<f32>,
-            normal: vec3<f32>,
-            light: vec3<f32>,
-            view: vec3<f32>,
-            albeido: vec3<f32>,
-        ) -> vec3<f32> {
-            let light_color = vec3<f32>(1.0, 1.0, 1.0);
-
-            // Light parameters
-            let ambient_factor = 0.1;
-            let diffuse_factor = 0.7;
-            let specular_factor = 0.3;
-            let shininess = u_material.shininess;
-
-            // Base vectors
-            var normal: vec3<f32> = normalize(normal);
-            let view = normalize(view);
-            let light = normalize(light);
-
-            // Maybe flip the normal - otherwise backfacing faces are not lit
-            // See pygfx/issues/#105 for details
-            normal = select(normal, -normal, is_front);
-
-            // Ambient
-            let ambient_color = light_color * ambient_factor;
-
-            // Diffuse (blinn-phong reflection model)
-            let lambert_term = clamp(dot(light, normal), 0.0, 1.0);
-            let diffuse_color = diffuse_factor * light_color * lambert_term;
-
-            // Specular
-            let halfway = normalize(light + view);  // halfway vector
-            var specular_term = pow(clamp(dot(halfway,  normal), 0.0, 1.0), shininess);
-            specular_term = select(0.0, specular_term, shininess > 0.0);
-            let specular_color = specular_factor * specular_term * light_color;
-
-            // Emissive color is additive and unaffected by lights
-            let emissive_color = u_material.emissive_color.rgb;
-
-            // Put together
-            return albeido * (ambient_color + diffuse_color) + specular_color + emissive_color;
-        }
-
-        fn lighting_flat(
-            is_front: bool,
-            world_pos: vec3<f32>,
-            normal: vec3<f32>,
-            light: vec3<f32>,
-            view: vec3<f32>,
-            albeido: vec3<f32>,
-        ) -> vec3<f32> {
-
-            let u = dpdx(world_pos);
-            let v = dpdy(world_pos);
-            var normal = normalize(cross(u, v));
-
-            // The normal calculated above may not be oriented correctly.
-            // We have two flags: is_front and u_stdinfo.flipped_winding.
-            // Note that lighting_phong() also applies the is_front flag.
-            // Below code means: flip the normal if the XOR of these two flags is true.
-            normal = select(normal, -normal, (select(0, 1, is_front) + u_stdinfo.flipped_winding) == 1);
 
-            // The rest is the same as phong
-            return lighting_phong(is_front, world_pos, normal, light, view, albeido);
+@register_wgpu_render_function(Volume, VolumeRayMaterial)
+class VolumeRayShader(BaseVolumeShader):
+    type = "render"
+
+    def get_bindings(self, wobject, shared):
+        self["mode"] = wobject.material.render_mode
+        return super().get_bindings(wobject, shared)
+
+    def get_pipeline_info(self, wobject, shared):
+        return {
+            "primitive_topology": wgpu.PrimitiveTopology.triangle_list,
+            "cull_mode": wgpu.CullMode.front,  # the back planes are the ref
         }
-        $$ endif
-
-        """
 
+    def get_render_info(self, wobject, shared):
+        material = wobject.material
 
-@register_wgpu_render_function(Mesh, MeshSliceMaterial)
-def meshslice_renderer(render_info):
-    """Render function capable of rendering mesh slices."""
-
-    # It would technically be possible to implement colormapping or
-    # per-vertex colors, but its a tricky dance to get the per-vertex
-    # data (e.g. texcoords) into a varying. And because the visual
-    # result is a line, its likely that in most use-cases a uniform
-    # color is preferred anyway. So for now we don't implement that.
-
-    wobject = render_info.wobject
-    geometry = wobject.geometry
-    material = wobject.material  # noqa
-
-    # Initialize
-    topology = wgpu.PrimitiveTopology.triangle_list
-    shader = MeshSliceShader(render_info)
-
-    # We're assuming the presence of an index buffer for now
-    assert getattr(geometry, "indices", None)
-    n = (geometry.indices.data.size // 3) * 6
-    n_instances = 1
-
-    bindings = {}
-
-    # Init uniform bindings
-    bindings[0] = Binding("u_stdinfo", "buffer/uniform", render_info.stdinfo_uniform)
-    bindings[1] = Binding("u_wobject", "buffer/uniform", wobject.uniform_buffer)
-    bindings[2] = Binding("u_material", "buffer/uniform", material.uniform_buffer)
-
-    # Init storage buffer bindings
-    bindings[3] = Binding(
-        "s_indices", "buffer/read_only_storage", geometry.indices, "VERTEX"
-    )
-    bindings[4] = Binding(
-        "s_positions", "buffer/read_only_storage", geometry.positions, "VERTEX"
-    )
-
-    # Let the shader generate code for our bindings
-    for i, binding in bindings.items():
-        shader.define_binding(0, i, binding)
-
-    # As long as we don't use alpha for aa in the frag shader, we can use a render_mask of 1 or 2.
-    only_color_and_opacity_determine_fragment_alpha = True
-    suggested_render_mask = 3
-    if only_color_and_opacity_determine_fragment_alpha:
-        is_opaque = material.opacity >= 1 and material.color[3] >= 1
-        suggested_render_mask = 1 if is_opaque else 2
-
-    # Put it together!
-    return [
-        {
-            "suggested_render_mask": suggested_render_mask,
-            "render_shader": shader,
-            "primitive_topology": topology,
-            "indices": (range(n), range(n_instances)),
-            "index_buffer": None,
-            "vertex_buffers": {},
-            "bindings0": bindings,
+        render_mask = wobject.render_mask
+        if not render_mask:
+            if material.is_transparent:
+                render_mask = RenderMask.transparent
+            elif self["img_nchannels"] in (1, 3):
+                render_mask = RenderMask.opaque
+            else:
+                render_mask = RenderMask.all
+
+        return {
+            "indices": (36, 1),
+            "render_mask": render_mask,
         }
-    ]
-
 
-class MeshSliceShader(WorldObjectShader):
     def get_code(self):
         return (
-            self.get_definitions()
-            + self.common_functions()
-            + self.vertex_shader()
-            + self.fragment_shader()
+            self.code_definitions()
+            + self.code_common()
+            + self.code_volume_helpers()
+            + self.code_render_function()
+            + self.code_vertex()
+            + self.code_fragment()
         )
 
-    def vertex_shader(self):
+    def code_vertex(self):
         return """
 
         struct VertexInput {
             @builtin(vertex_index) vertex_index : u32,
         };
 
-
-        @stage(vertex)
+        @vertex
         fn vs_main(in: VertexInput) -> Varyings {
 
-            // This vertex shader uses VertexId and storage buffers instead of
-            // vertex buffers. It creates 6 vertices for each face in the mesh,
-            // drawn with triangle-list. For the faces that cross the plane, we
-            // draw a (thick) line segment with round caps (we need 6 verts for that).
-            // Other faces become degenerate triangles.
-
-            let screen_factor = u_stdinfo.logical_size.xy / 2.0;
-            let l2p = u_stdinfo.physical_size.x / u_stdinfo.logical_size.x;
-            let thickness = u_material.thickness;  // in logical pixels
+            // Our geometry is implicitly defined by the volume dimensions.
+            var geo = get_vol_geometry();
 
-            // Get the face index, and sample the vertex indices
+            // Select what face we're at
             let index = i32(in.vertex_index);
-            let segment_index = index % 6;
-            let face_index = (index - segment_index) / 6;
-            let ii = vec3<i32>(load_s_indices(face_index));
-
-            // Vertex positions of this face, in local object coordinates
-            let pos1a = load_s_positions(ii[0]);
-            let pos2a = load_s_positions(ii[1]);
-            let pos3a = load_s_positions(ii[2]);
-            let pos1b = u_wobject.world_transform * vec4<f32>(pos1a, 1.0);
-            let pos2b = u_wobject.world_transform * vec4<f32>(pos2a, 1.0);
-            let pos3b = u_wobject.world_transform * vec4<f32>(pos3a, 1.0);
-            let pos1 = pos1b.xyz / pos1b.w;
-            let pos2 = pos2b.xyz / pos2b.w;
-            let pos3 = pos3b.xyz / pos3b.w;
+            let i0 = geo.indices[index];
 
-            // Get the plane definition
-            let plane = u_material.plane.xyzw;  // ax + by + cz + d
-            let n = plane.xyz;  // not necessarily a unit vector
+            // Sample position, and convert to world pos, and then to ndc
+            let data_pos = vec4<f32>(geo.positions[i0], 1.0);
+            let world_pos = u_wobject.world_transform * data_pos;
+            let ndc_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * world_pos;
 
-            // Intersect the plane with pos 1 and 2
-            var p: vec3<f32>;
-            var u: vec3<f32>;
-            p = pos1.xyz;
-            u = pos2.xyz - pos1.xyz;
-            let t1 = -(plane.x * p.x + plane.y * p.y + plane.z * p.z + plane.w) / dot(n, u);
-            // Intersect the plane with pos 2 and 3
-            p = pos2.xyz;
-            u = pos3.xyz - pos2.xyz;
-            let t2 = -(plane.x * p.x + plane.y * p.y + plane.z * p.z + plane.w) / dot(n, u);
-            // Intersect the plane with pos 3 and 1
-            p = pos3.xyz;
-            u = pos1.xyz - pos3.xyz;
-            let t3 = -(plane.x * p.x + plane.y * p.y + plane.z * p.z + plane.w) / dot(n, u);
-
-            // Selectors
-
-            let b1 = select(0, 4, (t1 > 0.0) && (t1 < 1.0));
-            let b2 = select(0, 2, (t2 > 0.0) && (t2 < 1.0));
-            let b3 = select(0, 1, (t3 > 0.0) && (t3 < 1.0));
-            let pos_index = b1 + b2 + b3;
-
-            // The big triage
-            var the_pos: vec4<f32>;
-            var the_coord: vec2<f32>;
-            var segment_length: f32;
-            var pick_idx = u32(0u);
-            var pick_coords = vec3<f32>(0.0);
-
-            if (pos_index < 3) {//   (pos_index < 3) {  // or dot(n, u) == 0.0
-                // Just return the same vertex, resulting in degenerate triangles
-                the_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * vec4<f32>(pos1, 1.0);
-                the_coord = vec2<f32>(0.0, 0.0);
-                segment_length = 0.0;
-
-            } else {
-                // Get the positions where the frame intersects the plane
-                let pos00: vec3<f32> = pos1;
-                let pos12: vec3<f32> = mix(pos1, pos2, vec3<f32>(t1, t1, t1));
-                let pos23: vec3<f32> = mix(pos2, pos3, vec3<f32>(t2, t2, t2));
-                let pos31: vec3<f32> = mix(pos3, pos1, vec3<f32>(t3, t3, t3));
-                // b1+b2+b3     000    001    010    011    100    101    110    111
-                var positions_a = array<vec3<f32>, 8>(pos00, pos00, pos00, pos23, pos00, pos12, pos12, pos12);
-                var positions_b = array<vec3<f32>, 8>(pos00, pos00, pos00, pos31, pos00, pos31, pos23, pos23);
-                // Select the two positions that define the line segment
-                let pos_a = positions_a[pos_index];
-                let pos_b = positions_b[pos_index];
-
-                // Same for face weights
-                let fw00 = vec3<f32>(0.5, 0.5, 0.5);
-                let fw12 = mix(vec3<f32>(1.0, 0.0, 0.0), vec3<f32>(0.0, 1.0, 0.0), vec3<f32>(t1, t1, t1));
-                let fw23 = mix(vec3<f32>(0.0, 1.0, 0.0), vec3<f32>(0.0, 0.0, 1.0), vec3<f32>(t2, t2, t2));
-                let fw31 = mix(vec3<f32>(0.0, 0.0, 1.0), vec3<f32>(1.0, 0.0, 0.0), vec3<f32>(t3, t3, t3));
-                var fws_a = array<vec3<f32>, 8>(fw00, fw00, fw00, fw23, fw00, fw12, fw12, fw12);
-                var fws_b = array<vec3<f32>, 8>(fw00, fw00, fw00, fw31, fw00, fw31, fw23, fw23);
-                let fw_a = fws_a[pos_index];
-                let fw_b = fws_b[pos_index];
-
-                // Go from local coordinates to NDC
-                var npos_a: vec4<f32> = u_stdinfo.projection_transform * u_stdinfo.cam_transform * vec4<f32>(pos_a, 1.0);
-                var npos_b: vec4<f32> = u_stdinfo.projection_transform * u_stdinfo.cam_transform * vec4<f32>(pos_b, 1.0);
-                // Don't forget to "normalize"!
-                // todo: omitting this step diminish the thickness with distance, but it that the way?
-                npos_a = npos_a / npos_a.w;
-                npos_b = npos_b / npos_b.w;
-
-                // And to logical pixel coordinates (don't worry about offset)
-                let ppos_a = npos_a.xy * screen_factor;
-                let ppos_b = npos_b.xy * screen_factor;
-
-                // Get the segment vector, its length, and how much it scales because of thickness
-                let v0 = ppos_b - ppos_a;
-                segment_length = length(v0);  // in logical pixels;
-                let segment_factor = (segment_length + thickness) / segment_length;
-
-                // Get the (orthogonal) unit vectors that span the segment
-                let v1 = normalize(v0);
-                let v2 = vec2<f32>(v1.y, -v1.x);
-
-                // Get the vector, in local logical pixels for the segment's square
-                let pvec_local = 0.5 * vec2<f32>(segment_length + thickness, thickness);
-
-                // Select one of the four corners of the segment rectangle
-                var vecs = array<vec2<f32>, 6>(
-                    vec2<f32>(-1.0, -1.0),
-                    vec2<f32>( 1.0,  1.0),
-                    vec2<f32>(-1.0,  1.0),
-                    vec2<f32>( 1.0,  1.0),
-                    vec2<f32>(-1.0, -1.0),
-                    vec2<f32>( 1.0, -1.0),
-                );
-                let the_vec = vecs[segment_index];
-
-                // Construct the position, also make sure zw scales correctly
-                let pvec = the_vec.x * pvec_local.x * v1 + the_vec.y * pvec_local.y * v2;
-                let z_range = (npos_b.z - npos_a.z) * segment_factor;
-                let the_pos_p = 0.5 * (ppos_a + ppos_b) + pvec;
-                let the_pos_z = 0.5 * (npos_a.z + npos_b.z) + the_vec.x * z_range * 0.5;
-                let depth_offset = -0.0001;  // to put the mesh slice atop a mesh
-                the_pos = vec4<f32>(the_pos_p / screen_factor, the_pos_z + depth_offset, 1.0);
-
-                // Define the local coordinate in physical pixels
-                the_coord = the_vec * pvec_local;
-
-                // Picking info
-                pick_idx = u32(face_index);
-                let mixval = the_vec.x * 0.5 + 0.5;
-                pick_coords = vec3<f32>(mix(fw_a, fw_b, vec3<f32>(mixval, mixval, mixval)));
-            }
+            // Prepare inverse matrix
+            let ndc_to_data = u_wobject.world_transform_inv * u_stdinfo.cam_transform_inv * u_stdinfo.projection_transform_inv;
 
-            // Shader output
             var varyings: Varyings;
-            varyings.position = vec4<f32>(the_pos);
-            varyings.world_pos = vec3<f32>(ndc_to_world_pos(the_pos));
-            varyings.dist2center = vec2<f32>(the_coord * l2p);
-            varyings.segment_length = f32(segment_length * l2p);
-            varyings.segment_width = f32(thickness * l2p);
-            varyings.pick_idx = u32(pick_idx);
-            varyings.pick_coords = vec3<f32>(pick_coords);
+
+            // Store values for fragment shader
+            varyings.position = vec4<f32>(ndc_pos);
+            varyings.world_pos = vec3<f32>(world_pos.xyz);
+
+            // The position on the face of the cube. We can say that it's the back face,
+            // because we cull the front faces.
+            // These positions are in data positions (voxels) rather than texcoords (0..1),
+            // because distances make more sense in this space. In the fragment shader we
+            // can consider it an isotropic volume, because any position, rotation,
+            // and scaling of the volume is part of the world transform.
+            varyings.data_back_pos = vec4<f32>(data_pos);
+
+            // We calculate the NDC positions for the near and front clipping planes,
+            // and transform these back to data coordinates. From these positions
+            // we can construct the view vector in the fragment shader, which is then
+            // resistant to perspective transforms. It also makes that if the camera
+            // is inside the volume, only the part in front in rendered.
+            // Note that the w component for these positions should be left intact.
+            let ndc_pos1 = vec4<f32>(ndc_pos.xy, -ndc_pos.w, ndc_pos.w);
+            let ndc_pos2 = vec4<f32>(ndc_pos.xy, ndc_pos.w, ndc_pos.w);
+            varyings.data_near_pos = vec4<f32>(ndc_to_data * ndc_pos1);
+            varyings.data_far_pos = vec4<f32>(ndc_to_data * ndc_pos2);
+
             return varyings;
         }
         """
 
-    def fragment_shader(self):
+    def code_fragment(self):
         return """
-
-        @stage(fragment)
+        @fragment
         fn fs_main(varyings: Varyings) -> FragmentOutput {
-            var out: FragmentOutput;
 
-            // Discart fragments that are too far from the centerline. This makes round caps.
-            // Note that we operate in physical pixels here.
-            let distx = max(0.0, abs(varyings.dist2center.x) - 0.5 * varyings.segment_length);
-            let dist = length(vec2<f32>(distx, varyings.dist2center.y));
-            if (dist > varyings.segment_width * 0.5) {
-                discard;
-            }
+            // Get size of the volume
+            let sizef = vec3<f32>(textureDimensions(t_img));
 
-            // No aa. This is something we need to decide on. See line renderer.
-            // Making this < 1 would affect the suggested_render_mask.
-            let alpha = 1.0;
-
-            // Set color
-            let color = u_material.color;
-            let final_color = vec4<f32>(color.rgb, min(1.0, color.a) * alpha);
+            // Determine the stepsize as a float in pixels.
+            // This value should be between ~ 0.1 and 1. Smaller values yield better
+            // results at the cost of performance. With larger values you may miss
+            // small structures (and corners of larger structures) because the step
+            // may skip over them.
+            // We could make this a user-facing property. But for now we scale between
+            // 0.1 and 0.8 based on the (sqrt of the) volume size.
+            let relative_step_size = clamp(sqrt(max(sizef.x, max(sizef.y, sizef.z))) / 20.0, 0.1, 0.8);
+
+            // Positions in data coordinates
+            let back_pos = varyings.data_back_pos.xyz / varyings.data_back_pos.w;
+            let far_pos = varyings.data_far_pos.xyz / varyings.data_far_pos.w;
+            let near_pos = varyings.data_near_pos.xyz / varyings.data_near_pos.w;
+
+            // Calculate unit vector pointing in the view direction through this fragment.
+            let view_ray = normalize(far_pos - near_pos);
+
+            // Calculate the (signed) distance, from back_pos to the first voxel
+            // that must be sampled, expressed in data coords (voxels).
+            var dist = dot(near_pos - back_pos, view_ray);
+            dist = max(dist, min((-0.5 - back_pos.x) / view_ray.x, (sizef.x - 0.5 - back_pos.x) / view_ray.x));
+            dist = max(dist, min((-0.5 - back_pos.y) / view_ray.y, (sizef.y - 0.5 - back_pos.y) / view_ray.y));
+            dist = max(dist, min((-0.5 - back_pos.z) / view_ray.z, (sizef.z - 0.5 - back_pos.z) / view_ray.z));
+
+            // Now we have the starting position. This is typically on a front face,
+            // but it can also be incide the volume (on the near plane).
+            let front_pos = back_pos + view_ray * dist;
+
+            // Decide how many steps to take. If we'd not cul the front faces,
+            // that would still happen here because nsteps would be negative.
+            let nsteps = i32(-dist / relative_step_size + 0.5);
+            if( nsteps < 1 ) { discard; }
+
+            // Get starting position and step vector in texture coordinates.
+            let start_coord = (front_pos + vec3<f32>(0.5, 0.5, 0.5)) / sizef;
+            let step_coord = ((back_pos - front_pos) / sizef) / f32(nsteps);
+
+            // Render
+            let render_out = render_func(sizef, nsteps, start_coord, step_coord);
+
+            // Get world and ndc pos from the calculatex texture coordinate
+            let data_pos = render_out.coord * sizef - vec3<f32>(0.5, 0.5, 0.5);
+            let world_pos = u_wobject.world_transform * vec4<f32>(data_pos, 1.0);
+            let ndc_pos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * world_pos;
 
-            // Wrap up
+            // Maybe we did the work for nothing
+            apply_clipping_planes(world_pos.xyz);
 
-            apply_clipping_planes(varyings.world_pos);
-            var out = get_fragment_output(varyings.position.z, final_color);
+            // Get fragment output. Note that the depth arg only affects the
+            // blending - setting the depth attribute actually sets the fragment depth.
+            let depth = ndc_pos.z / ndc_pos.w;
+            var out = get_fragment_output(depth, render_out.color);
+            out.depth = depth;
 
             $$ if write_pick
             // The wobject-id must be 20 bits. In total it must not exceed 64 bits.
             out.pick = (
                 pick_pack(u32(u_wobject.id), 20) +
-                pick_pack(varyings.pick_idx, 26) +
-                pick_pack(u32(varyings.pick_coords.x * 64.0), 6) +
-                pick_pack(u32(varyings.pick_coords.y * 64.0), 6) +
-                pick_pack(u32(varyings.pick_coords.z * 64.0), 6)
+                pick_pack(u32(render_out.coord.x * 16383.0), 14) +
+                pick_pack(u32(render_out.coord.y * 16383.0), 14) +
+                pick_pack(u32(render_out.coord.z * 16383.0), 14)
             );
             $$ endif
+            return out;
+        }
+        """
+
+    def code_render_function(self):
+        # Triage over different render modes. Only one mode so far :)
+        f = getattr(self, "render_mode_" + self.kwargs["mode"].lower(), "mip")
+
+        preamble = """
+        struct RenderOutput {
+            color: vec4<f32>,
+            coord: vec3<f32>,
+        };
+        """
+
+        return preamble + f()
+
+    def render_mode_mip(self):
+        # Ideas for improvement:
+        # * We could textureLoad() the 27 voxels surrounding the initial location
+        #   and sample from that in the refinement step. Less texture loads and we
+        #   could do linear interpolation also for formats like i16.
+        # * Create helper textures at a lower resolution (e.g. min, max) so we can
+        #   skip along the ray much faster. By taking smaller steps where needed,
+        #   it will be both faster and more accurate.
+
+        return """
+        fn render_func(sizef: vec3<f32>, nsteps: i32, start_coord: vec3<f32>, step_coord: vec3<f32>) -> RenderOutput {
+
+            let nstepsf = f32(nsteps);
+
+            // Primary loop. The purpose is to find the approximate location where
+            // the maximum is.
+            var the_ref = -999999.0;
+            var the_coord = start_coord;
+            var the_value : vec4<f32>;
+            for (var iter=0.0; iter<nstepsf; iter=iter+1.0) {
+                let coord = start_coord + iter * step_coord;
+                let value = sample_vol(coord, sizef);
+                let reff = value.r;
+                if (reff > the_ref) {
+                    the_ref = reff;
+                    the_coord = coord;
+                    the_value = value;
+                }
+            }
+
+            // Secondary loop to close in on a more accurate position using
+            // a divide-by-two approach.
+            var substep_coord = step_coord;
+            for (var iter2=0; iter2<4; iter2=iter2+1) {
+                substep_coord = substep_coord * 0.5;
+                let coord1 = the_coord - substep_coord;
+                let coord2 = the_coord + substep_coord;
+                let value1 = sample_vol(coord1, sizef);
+                let value2 = sample_vol(coord2, sizef);
+                let ref1 = value1.r;
+                let ref2 = value2.r;
+                if (ref1 >= the_ref) {  // deliberate larger-equal
+                    the_ref = ref1;
+                    the_coord = coord1;
+                    the_value = value1;
+                } else if (ref2 > the_ref) {
+                    the_ref = ref2;
+                    the_coord = coord2;
+                    the_value = value2;
+                }
+            }
+
+            // Colormapping
+            let color = sampled_value_to_color(the_value);
+            // Move to physical colorspace (linear photon count) so we can do math
+            $$ if colorspace == 'srgb'
+                let physical_color = srgb2physical(color.rgb);
+            $$ else
+                let physical_color = color.rgb;
+            $$ endif
+            let opacity = color.a * u_material.opacity;
+            let out_color = vec4<f32>(physical_color, opacity);
 
+            // Produce result
+            var out: RenderOutput;
+            out.color = out_color;
+            out.coord = the_coord;
             return out;
         }
         """
```

### Comparing `pygfx-0.1.9/pygfx/resources/_texture.py` & `pygfx-0.2.0/pygfx/resources/_texture.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,124 @@
 import numpy as np
 
-from ._buffer import Resource, STRUCT_FORMAT_ALIASES
+from ._base import Resource, get_item_format_from_memoryview
 
 
 class Texture(Resource):
-    """A base texture wrapper that can be implemented for numpy, ctypes arrays,
-    or any other kind of array.
+    """Texture object containing structured 1D, 2D or 3D data.
+
+    Can be used to represent e.g. image data or colormaps. Can also
+    serve as a render target (for the renderer). Supports texture
+    stacks, cube textures, and mipmapping.
 
     Parameters:
-        data (array, optional): Array data of any type that supports the
-            buffer-protocol, (e.g. a bytes or numpy array). If not given
-            or None, nbytes and nitems must be provided. The data is
-            copied if it's float64 or not contiguous.
-        dim (int): The dimensionality of the array (1, 2 or 3).
-        size (3-tuple): The extent ``(width, height, depth)`` of the array.
-            If not given or None, it is derived from dim and the shape of
-            the data. By creating a 2D array with ``depth > 1``, a view can
-            be created with format 'd2_array' or 'cube'.
-        format (str): the format of texture. By default this is automatically
-            set from the data. This must be a pygfx format specifier, e.g. "3xf4",
-            but can also be a format specific to the render backend if necessary
-            (e.g. from ``wgpu.TextureFormat``).
+        data : array, optional
+            Array data of any type that supports the buffer-protocol, (e.g. a
+            bytes or numpy array). If None, nbytes and size must be provided.
+            The dtype must be compatible with the rendering backend.
+        dim : int
+            The dimensionality of the array (1, 2 or 3).
+        size : tuple, [3]
+            The extent ``(width, height, depth)`` of the array. If None, it is
+            derived from `dim` and the shape of the data. The texture can also
+            represent a stack of images by setting `dim=2` and `depth > 1`,
+            or a cube image by setting `dim=2` and `depth==6`.
+        format : str
+            A format string describing the texture layout. If None, this is
+            derived from the data. This must be a pygfx format
+            specifier, e.g. "3xf4", but can also be a format specific to the
+            render backend (e.g. from ``wgpu.TextureFormat``).
+        colorspace : str
+            If this data is used as color, it is interpreted to be in this
+            colorspace. Can be "srgb" or "physical". Default "srgb".
+        generate_mipmaps : bool
+            If True, automatically generates mipmaps when transferring data to
+            the GPU.
+
     """
 
-    def __init__(self, data=None, *, dim, size=None, format=None):
-        self._rev = 0
+    def __init__(
+        self,
+        data=None,
+        *,
+        dim,
+        size=None,
+        format=None,
+        colorspace="srgb",
+        generate_mipmaps=False,
+    ):
+        super().__init__()
+        Resource._rev += 1
+        self._rev = Resource._rev
         # The dim specifies the texture dimension
         assert dim in (1, 2, 3)
-        self._dim = int(dim)
-        # The size specifies the size on the GPU (width, height, depth)
-        self._size = ()
-        self._format = None if format is None else str(format)
-        self._nbytes = 0
+        self._store.dim = int(dim)
         # The actual data (optional)
         self._data = None
-        self._pending_uploads = []  # list of (offset, size) tuples
+        self._format = None
+        self._gfx_pending_uploads = []  # list of (offset, size) tuples
 
         # Backends-specific attributes for internal use
+        self._wgpu_object = None
         self._wgpu_usage = 0
+        self._wgpu_mip_level_count = 1
+
+        self._colorspace = (colorspace or "srgb").lower()
+        assert self._colorspace in ("srgb", "physical")
+
+        self._generate_mipmaps = bool(generate_mipmaps)
 
         size = None if size is None else (int(size[0]), int(size[1]), int(size[2]))
 
         if data is not None:
-            mem = memoryview(data)
-            if mem.format == "d":
-                raise ValueError("Float64 data is not supported, use float32 instead.")
             self._data = data
-            self._mem = mem
-            self._nbytes = mem.nbytes
-            self._size = self._size_from_data(mem, dim, size)
-            self.update_range((0, 0, 0), self._size)
+            self._mem = mem = memoryview(data)
+            self._store.nbytes = mem.nbytes
+            self._store.size = self._size_from_data(mem, dim, size)
+            subformat = get_item_format_from_memoryview(mem)
+            if subformat is None:
+                raise ValueError(
+                    f"Unsupported dtype/format for texture data: {mem.format}"
+                )
+            shape = mem.shape
+            collapsed_size = [x for x in self.size if x > 1]
+            if len(shape) == len(collapsed_size) + 1:
+                nchannels = shape[-1]
+            else:
+                if not len(shape) == len(collapsed_size):
+                    raise ValueError(
+                        "Incompatible data shape for image data, there must be > 1 pixel to draw per channel"
+                    )
+                nchannels = 1
+            if not (1 <= nchannels <= 4):
+                raise ValueError(
+                    f"Expected 1-4 texture color channels, got {nchannels}."
+                )
+            self._format = (f"{nchannels}x" + subformat).lstrip("1x")
+            self.update_range((0, 0, 0), self.size)
         elif size is not None and format is not None:
-            self._size = size
+            self._store.size = size
+            self._store.nbytes = 0
         else:
             raise ValueError(
                 "Texture must be instantiated with either data or size and format."
             )
 
+        if format is not None:
+            self._format = str(format)
+
     @property
     def rev(self):
         """An integer that is increased when update_range() is called."""
         return self._rev
 
-    def get_view(self, **kwargs):
-        """Get a new view on the this texture."""
-        return TextureView(self, **kwargs)
-
     @property
     def dim(self):
         """The dimensionality of the texture (1, 2, or 3)."""
-        return self._dim
+        return self._store.dim
 
     @property
     def data(self):
         """The data for this texture. Can be None if the data only
         exists on the GPU.
 
         Note: the data is the same reference that was given to
@@ -87,36 +132,42 @@
         the data only exists on the GPU.
         """
         return self._mem
 
     @property
     def nbytes(self):
         """Get the number of bytes in the texture."""
-        return self._nbytes
+        return self._store.nbytes
 
     @property
     def size(self):
         """The size of the texture as (width, height, depth).
         (always a 3-tuple, regardless of the dimension).
         """
-        return self._size
+        return self._store.size
 
     @property
     def format(self):
         """The texture format as a string. Usually a pygfx format specifier
         (e.g. u2 for scalar uint16, or 3xf4 for RGB float32),
-        but can also be a overriden to a backend-specific format.
+        but can also be a overridden to a backend-specific format.
         """
-        if self._format is not None:
-            return self._format
-        elif self.data is not None:
-            self._format = format_from_memoryview(self.mem, self.size)
-            return self._format
-        else:
-            raise ValueError("Texture has no data nor format.")
+        return self._format
+
+    @property
+    def colorspace(self):
+        """If this data is used as color, it is interpreted to be in this colorspace.
+        Can be "srgb" or "physical". Default "srgb".
+        """
+        return self._colorspace
+
+    @property
+    def generate_mipmaps(self):
+        """Whether to automatically generate mipmaps when uploading to the GPU."""
+        return self._generate_mipmaps
 
     def update_range(self, offset, size):
         """Mark a certain range of the data for upload to the GPU.
         The offset and (sub) size should be (width, height, depth)
         tuples. Numpy users beware that an arrays shape is (height, width)!
         """
         # Check input
@@ -133,23 +184,25 @@
         # Apply - consider that texture arrays want to be uploaded per-texture
         # todo: avoid duplicates by merging with existing pending uploads
         if self.dim == 1:
             for z in range(size[2]):
                 for y in range(size[1]):
                     offset2 = offset[0], y, z
                     size2 = size[0], 1, 1
-                    self._pending_uploads.append((offset2, size2))
+                    self._gfx_pending_uploads.append((offset2, size2))
         elif self.dim == 2:
             for z in range(size[2]):
                 offset2 = offset[0], offset[1], z
                 size2 = size[0], size[1], 1
-                self._pending_uploads.append((offset2, size2))
+                self._gfx_pending_uploads.append((offset2, size2))
         else:
-            self._pending_uploads.append((offset, size))
-        self._rev += 1
+            self._gfx_pending_uploads.append((offset, size))
+        Resource._rev += 1
+        self._rev = Resource._rev
+        self._gfx_mark_for_sync()
 
     def _size_from_data(self, data, dim, size):
         # Check if shape matches dimension
         shape = data.shape
 
         if size:
             # Get version of size with trailing ones stripped
@@ -172,16 +225,21 @@
             elif dim == 2:
                 return shape[1], shape[0], 1
             else:  # dim == 3:
                 return shape[2], shape[1], shape[0]
 
     def _get_subdata(self, offset, size, pixel_padding=None):
         """Return subdata as a contiguous array."""
-        # If this is a full range, this is easy
-        if offset == 0 and size == self.nitems and self.mem.contiguous:
+        # If this is a full range, this is easy (and fast)
+        if (
+            offset == (0, 0, 0)
+            and size == self.size
+            and self.mem.c_contiguous
+            and pixel_padding is None
+        ):
             return self.mem
         # Get a numpy array, because memoryviews do not support nd slicing
         if isinstance(self.data, np.ndarray):
             arr = self.data
         elif not self.mem.c_contiguous:
             raise ValueError(
                 "Non-contiguous texture data is only supported for numpy array."
@@ -195,133 +253,11 @@
             slices.append(slice(offset[d], offset[d] + size[d]))
         sub_arr = arr[tuple(slices)]
         if pixel_padding is not None:
             padding = np.ones(sub_arr.shape[:3] + (1,), dtype=sub_arr.dtype)
             sub_arr = np.concatenate([sub_arr, pixel_padding * padding], -1)
         return memoryview(np.ascontiguousarray(sub_arr))
 
-
-def format_from_memoryview(mem, size):
-
-    formatmap = {
-        "b": "i1",
-        "B": "u1",
-        "h": "i2",
-        "H": "u2",
-        "i": "i4",
-        "U": "u4",
-        "e": "f2",
-        "f": "f4",
-    }
-
-    format = str(mem.format)
-    format = STRUCT_FORMAT_ALIASES.get(format, format)
-    # Process channels
-    shape = mem.shape
-    collapsed_size = [x for x in size if x > 1]
-    if len(shape) == len(collapsed_size) + 1:
-        nchannels = shape[-1]
-    else:
-        assert len(shape) == len(collapsed_size)
-        nchannels = 1
-    assert 1 <= nchannels <= 4
-    if format in ("d", "float64"):
-        raise TypeError("GPU's don't support float64 texture formats.")
-    elif format not in formatmap:
-        raise TypeError(
-            f"Cannot convert {format!r} to texture format. Maybe specify format?"
+    def get_view(self, *args, **kwargs):
+        raise DeprecationWarning(
+            "Texture.get_view() is removed, TextureView is no longer public API: just use plain textures."
         )
-    format = f"{nchannels}x" + formatmap[format]
-    return format.lstrip("1x")
-
-
-# mipmaps: every texture can have a certain number of mipmap levels. Each
-# next level is half the size of the previous level. I think we can design our
-# API to target level 0 by default and allow a way to upload data to other levels.
-# arrays: a d2_array view can be be created from a d2 texture with dept > 1
-# cube: a special kind3 of array texture, with six 2D textures.
-# cube_array: I suppose you'd have an array of 6xn textures in this case?
-
-
-class TextureView(Resource):
-    """A view on a texture.
-
-    The view defines the sampling behavior and can specify a selection/different
-    view on the texture.
-
-    Passing no more than ``address_mode`` and ``filter`` will create a
-    default view on the texture with the given sampling parameters.
-
-    Parameters:
-        address_mode (str): How to sample beyond the edges. Use "clamp",
-            "mirror" or "repeat". Default "clamp".
-            Can also use e.g. "clamp,clamp,repeat" to specify for u, v and w.
-        filter (str): Interpolation filter. Use "nearest" or "linear".
-            Default "nearest". Can also use e.g. "linear,linear,nearest" to set
-            mag, min and mipmap filters.
-        format (str): Omit or pass None to use the texture's format.
-        view_dim (str): Omit or pass None to use the texture's format. Or e.g.
-            get a "2d" slice view from a 3d texture, or e.g. "cube" or "2d-array".
-        aspect (str): Omit or pass None to use the default.
-        mip_range (range): A range object to specify what mip levels to view.
-        layer_range (range): A range object to specify what array layers to view.
-    """
-
-    def __init__(
-        self,
-        texture,
-        *,
-        address_mode="clamp",
-        filter="nearest",
-        format=None,
-        view_dim=None,
-        aspect=None,
-        mip_range=None,
-        layer_range=None,
-    ):
-        self._rev = 1
-        assert isinstance(texture, Texture)
-        self._texture = texture
-        # Sampler parameters
-        self._address_mode = address_mode
-        self._filter = filter
-        # Texture view parameters
-        self._format = format
-        self._view_dim = view_dim
-        self._aspect = aspect
-        self._mip_range = mip_range or range(1)
-        self._layer_range = layer_range or range(1)
-        self._is_default_view = all(
-            x is None for x in [format, view_dim, aspect, mip_range, layer_range]
-        )
-
-    @property
-    def rev(self):
-        # This is not actually increased anywhere, but it's added for consistency
-        return self._rev
-
-    @property
-    def texture(self):
-        """The Texture object holding the data for this texture view."""
-        return self._texture
-
-    @property
-    def format(self):
-        """The texture format."""
-        return self._format or self.texture.format
-
-    @property
-    def view_dim(self):
-        """The dimensionality of this view: "1d", "2d" or "3d"."""
-        return self._view_dim or f"{self.texture.dim}d"
-
-    @property
-    def address_mode(self):
-        """How to sample beyond the edges. Use "clamp",
-        "mirror" or "repeat". Default "clamp".
-        """
-        return self._address_mode
-
-    @property
-    def filter(self):
-        """Interpolation filter. Use "nearest" or "linear"."""
-        return self._filter
```

### Comparing `pygfx-0.1.9/pygfx/utils/_cmdata_mpl.py` & `pygfx-0.2.0/pygfx/utils/_cmdata_mpl.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.9/pygfx/utils/color.py` & `pygfx-0.2.0/pygfx/utils/color.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Provides utilities to deal with color."""
 
 # Possible improvements:
 #
-# * Support for HSL colorspace:
-#   * Accept CSS compatible "hsl(...)" and "hsla(...)"
-#   * Color.hsl property
-#   * Color.from_hsl() classmethod
-# * Support for HSV color space?
+# Colorspaces
 # * Support for HSLuv, a colorspace with uniform brightness https://www.hsluv.org/
-# * Color.__add__ another color or a scalar.
-# * Color.__mul__ another color or a scalar.
+#
+# CSS:
+# * Support "rgb(100%, 50%, 0%)"
+# * Support "hsl(...)" and "hsla(...)"
+#
+# Other:
 # * Color.lerp(color, t) linear interpolate towards other color.
-# * Color.lerpHSL(color, t) same as lerp but interpolate in HSL space.
-# * Color.lighter(factor) and Color.darker(factort)
-
-# todo Color.__eq__
-# todo: Support "rgb(100%, 50%, 0%)"
+# * Color.lerpHSL(color, t) same as lerp but interpolate in HSL / HSLuv space.
+# * Color.lighter(factor) and Color.darker(factor)
 
 
 import ctypes
+import colorsys
 
 
 F4 = ctypes.c_float * 4
 
 
 def _float_from_css_value(v, i):
     v = v.strip()
@@ -31,55 +29,60 @@
     elif i < 3:
         return float(v) / 255
     else:
         return float(v)
 
 
 class Color:
-    """An object representing a color.
+    """A representation of color (in the sRGB colorspace).
 
-    Internally the color is stored using 4 32-bit floats (rgba).
-    It can be instantiated in a variety of ways. E.g. by providing
-    the color components as values between 0 and 1:
+    Internally the color is stored using 4 32-bit floats (rgba). It can be
+    instantiated in a variety of ways. E.g. by providing the color components as
+    values between 0 and 1:
 
-    * `Color(r, g, b, a)` providing rgba values.
-    * `Color(r, g, b)` providing rgb, alpha is 1.
-    * `Color(gray, a)` grayscale intensity and alpha.
-    * `Color(gray)` grayscale intensity.
+        * `Color(r, g, b, a)` providing rgba values.
+        * `Color(r, g, b)` providing rgb, alpha is 1.
+        * `Color(gray, a)` grayscale intensity and alpha.
+        * `Color(gray)` grayscale intensity.
 
-    The above variations can also be supplied as a single tuple/list,
-    or anything that :
+    The above variations can also be supplied as a single tuple/list, or
+    anything that:
 
-    * `Color((r, g, b))`.
+        * `Color((r, g, b))`.
 
     Named colors:
 
-    * `Color("red")` base color names.
-    * `Color("cornflowerblue")` CSS color names.
-    * `Color("m")` Matlab color chars.
+        * `Color("red")` base color names.
+        * `Color("cornflowerblue")` CSS color names.
+        * `Color("m")` Matlab color chars.
 
     Hex colors:
 
-    * `Color("#ff0000")` the commmon hex format.
-    * `Color("#ff0000ff")` the hex format that includes alpha.
-    * `Color("#ff0")` the short form hex format.
-    * `Color("#ff0f")` the short form hex format that includes alpha.
+        * `Color("#ff0000")` the common hex format.
+        * `Color("#ff0000ff")` the hex format that includes alpha.
+        * `Color("#ff0")` the short form hex format.
+        * `Color("#ff0f")` the short form hex format that includes alpha.
 
     CSS color functions:
 
-    * `Color("rgb(255, 0, 0)")`.
-    * `Color("rgba(255, 0, 0, 1.0)")`.
+        * `Color("rgb(255, 0, 0)")`.
+        * `Color("rgba(255, 0, 0, 1.0)")`.
+
+    Parameters
+    ----------
+    args : tuple, int, str
+        The color specification. Check the docstring of this function for
+        details on available format options.
 
     """
 
     # Internally, the color is a ctypes float array
     __slots__ = ["_val"]
 
     def __init__(self, *args):
-
         if len(args) == 1:
             color = args[0]
             if isinstance(color, (int, float)):
                 self._set_from_tuple(args)
             elif isinstance(color, str):
                 self._set_from_str(color)
             else:
@@ -91,39 +94,63 @@
 
     def __repr__(self):
         # A precision of 4 decimals, i.e. 10001 possible values for each color.
         # We truncate zeros, but make sure the value does not end with a dot.
         f = lambda v: f"{v:0.4f}".rstrip("0").ljust(3, "0")  # noqa: stfu
         return f"Color({f(self.r)}, {f(self.g)}, {f(self.b)}, {f(self.a)})"
 
+    @property
+    def __array_interface__(self):
+        # Numpy can wrap our memory in an array without copying
+        readonly = True
+        ptr = ctypes.addressof(self._val)
+        x = dict(version=3, shape=(4,), typestr="<f4", data=(ptr, readonly))
+        return x
+
     def __len__(self):
         return 4
 
     def __getitem__(self, index):
         return self._val[index]
 
     def __iter__(self):
         return self.rgba.__iter__()
 
-    @property
-    def __array_interface__(self):
-        # Numpy can wrap our memory in an array without copying
-        readonly = True
-        ptr = ctypes.addressof(self._val)
-        x = dict(version=3, shape=(4,), typestr="<f4", data=(ptr, readonly))
-        return x
+    def __eq__(self, other):
+        if not isinstance(other, Color):
+            other = Color(other)
+        return all(self._val[i] == other._val[i] for i in range(4))
+
+    def __add__(self, other):
+        return Color(
+            self.r + other.r,
+            self.g + other.g,
+            self.b + other.b,
+            self.a,
+        )
 
-    def _set_from_rgba(self, r, g, b, a):
-        self._val = F4(
-            max(0.0, min(1.0, float(r))),
-            max(0.0, min(1.0, float(g))),
-            max(0.0, min(1.0, float(b))),
-            max(0.0, min(1.0, float(a))),
+    def __mul__(self, factor):
+        if not isinstance(factor, (float, int)):
+            raise TypeError("Can only multiple a color with a scalar.")
+        return Color(
+            self.r * factor,
+            self.g * factor,
+            self.b * factor,
+            self.a,
         )
 
+    def __truediv__(self, factor):
+        if not isinstance(factor, (float, int)):
+            raise TypeError("Can only multiple a color with a scalar.")
+        return self.__mul__(1 / factor)
+
+    def _set_from_rgba(self, r, g, b, a):
+        a = max(0.0, min(1.0, float(a)))
+        self._val = F4(float(r), float(g), float(b), a)
+
     def _set_from_tuple(self, color):
         color = tuple(float(c) for c in color)
         if len(color) == 4:
             self._set_from_rgba(*color)
         elif len(color) == 3:
             self._set_from_rgba(*color, 1)
         elif len(color) == 2:
@@ -213,52 +240,123 @@
     @property
     def b(self):
         """The blue value."""
         return self._val[2]
 
     @property
     def a(self):
-        """The alpha (transparency) value."""
+        """The alpha (transparency) value, between 0 and 1."""
         return self._val[3]
 
     @property
     def gray(self):
         """Return the grayscale intensity."""
         # Calculate with the weighted (a.k.a. luminosity) method, same as Matlab
         r, g, b = self.rgb
         return 0.2989 * r + 0.5870 * g + 0.1140 * b
 
     @property
     def hex(self):
-        """The CSS hex string, e.g. "#00ff00". The alpha channel is ignored."""
-        r = int(self.r * 255 + 0.5)
-        b = int(self.b * 255 + 0.5)
-        g = int(self.g * 255 + 0.5)
+        """The CSS hex string, e.g. "#00ff00". The alpha channel is ignored.
+        Values are clipped to 00 an ff.
+        """
+        c = self.clip()
+        r = int(c.r * 255 + 0.5)
+        b = int(c.b * 255 + 0.5)
+        g = int(c.g * 255 + 0.5)
         i = (r << 16) + (g << 8) + b
         return "#" + hex(i)[2:].rjust(6, "0")
 
     @property
     def hexa(self):
-        """The hex string including alpha, e.g. "#00ff00ff"."""
-        r = int(self.r * 255 + 0.5)
-        b = int(self.b * 255 + 0.5)
-        g = int(self.g * 255 + 0.5)
-        a = int(self.a * 255 + 0.5)
+        """The hex string including alpha, e.g. "#00ff00ff".
+        Values are clipped to 00 an ff.
+        """
+        c = self.clip()
+        r = int(c.r * 255 + 0.5)
+        b = int(c.b * 255 + 0.5)
+        g = int(c.g * 255 + 0.5)
+        a = int(c.a * 255 + 0.5)
         i = (r << 24) + (g << 16) + (b << 8) + a
         return "#" + hex(i)[2:].rjust(8, "0")
 
     @property
     def css(self):
         """The CSS color string, e.g. "rgba(0,255,0,0.5)"."""
         r, g, b, a = self.rgba
         if a == 1:
             return f"rgb({int(255*r+0.5)},{int(255*g+0.5)},{int(255*b+0.5)})"
         else:
             return f"rgba({int(255*r+0.5)},{int(255*g+0.5)},{int(255*b+0.5)},{a:0.3f})"
 
+    def clip(self):
+        """Return a new Color with the values clipped between 0 and 1."""
+        return Color(max(0.0, min(1.0, x)) for x in self.rgba)
+
+    @classmethod
+    def from_physical(cls, r, g, b, a=1):
+        """Create a Color object from a color in the physical colorspace.
+
+        With the physical colorspace we mean what is sometimes called
+        Linear-sRGB. It has the same gamut as sRGB, but where sRGB is
+        linear w.r.t. human perception, Linear-sRGB is linear w.r.t.
+        lumen and photon counts. Calculations on colors in pygfx's shaders
+        are done in the physical colorspace.
+        """
+        return Color(_physical2srgb(r), _physical2srgb(g), _physical2srgb(b), a)
+
+    def to_physical(self):
+        """Get the color represented in the physical colorspace, as 3 floats."""
+        return _srgb2physical(self.r), _srgb2physical(self.g), _srgb2physical(self.b)
+
+    @classmethod
+    def from_hsv(cls, hue, saturation, value):
+        """Create a Color object from an a color in the HSV (a.k.a. HSB) colorspace.
+
+        HSV stands for hue, saturation, value (aka brightness). The hue
+        component indicates the color tone. Values go from red (0) to
+        green (0.333) to blue (0.666) and back to red (1). The
+        satutation indicates vividness, with 0 meaning gray and 1
+        meaning the primary color. The value/brightness indicates goes
+        from 0 (black) to 1 (white).
+        """
+        return Color(colorsys.hsv_to_rgb(hue, saturation, value))
+
+    def to_hsv(self):
+        """Get the color represented in the HSV colorspace, as 3 floats."""
+        return colorsys.rgb_to_hsv(*self.rgb)
+
+    @classmethod
+    def from_hsl(cls, hue, saturation, lightness):
+        """Create a Color object from an a color in the HSL colorspace.
+
+        The HSL colorspace is similar to the HSV colorspace, except the
+        "value" is replaced with "lightness". This lightness scales the
+        color differently, e.g. a lightness of 1 always represents full
+        white.
+        """
+        return Color(colorsys.hls_to_rgb(hue, lightness, saturation))
+
+    def to_hsl(self):
+        """Get the color represented in the HSL colorspace, as 3 floats."""
+        hue, lightness, saturation = colorsys.rgb_to_hls(*self.rgb)
+        return hue, saturation, lightness
+
+
+def _srgb2physical(c):
+    # The simplified version has a maximum error less than 1%, but that's still
+    # two steps in the range 0..255.
+    # return c ** 2.2
+    return c / 12.92 if c <= 0.04045 else ((c + 0.055) / 1.055) ** 2.4
+
+
+def _physical2srgb(c):
+    # return c ** (1 / 2.2)
+    return c * 12.92 if c <= 0.0031308 else c ** (1 / 2.4) * 1.055 - 0.055
+
 
 NAMED_COLORS = {
     # CSS Level 1
     "black": "#000000",
     "silver": "#C0C0C0",
     "gray": "#808080",
     "white": "#FFFFFF",
```

### Comparing `pygfx-0.1.9/pygfx/utils/viewport.py` & `pygfx-0.2.0/pygfx/utils/viewport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from ..renderers import Renderer
 
 
 class Viewport:
-    """Defines a rectangular area on a renderer."""
+    """A rectangular area on a renderer.
+
+    Parameters
+    ----------
+    renderer : Renderer
+        The renderer on which the viewport should be defined.
+    rect : tuple, [4]
+        The viewport rect (x, y, w, h). If None, it is set to the full size of
+        the renderer's canvas.
+
+    """
 
     def __init__(self, renderer, rect=None):
         if not isinstance(renderer, Renderer):
             raise TypeError("Viewport first arg must be a Renderer.")
         self._renderer = renderer
         self.rect = rect
 
@@ -57,12 +67,12 @@
             return self._rect
 
     def is_inside(self, x, y):
         """Get whether the given position is inside the viewport rect."""
         vp = self.rect
         return vp[0] <= x <= vp[0] + vp[2] and vp[1] <= y <= vp[1] + vp[3]
 
-    def render(self, scene, camera):
+    def render(self, scene, camera, flush=False):
         """A shorthand for ``renderer.render(scene, camera)`` at the appropriate
-        viewport. Does not flush.
+        viewport. Does not flush by default.
         """
-        self.renderer.render(scene, camera, rect=self.rect, flush=False)
+        self.renderer.render(scene, camera, rect=self.rect, flush=flush)
```

### Comparing `pygfx-0.1.9/pygfx.egg-info/SOURCES.txt` & `pygfx-0.2.0/pygfx.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,84 +2,125 @@
 README.md
 setup.cfg
 setup.py
 pygfx/__init__.py
 pygfx.egg-info/PKG-INFO
 pygfx.egg-info/SOURCES.txt
 pygfx.egg-info/dependency_links.txt
+pygfx.egg-info/entry_points.txt
 pygfx.egg-info/requires.txt
 pygfx.egg-info/top_level.txt
 pygfx.egg-info/zip-safe
+pygfx/__pyinstaller/__init__.py
+pygfx/__pyinstaller/conftest.py
+pygfx/__pyinstaller/hook-pygfx.py
+pygfx/__pyinstaller/test_pygfx.py
 pygfx/cameras/__init__.py
 pygfx/cameras/_base.py
 pygfx/cameras/_orthographic.py
 pygfx/cameras/_perspective.py
 pygfx/controllers/__init__.py
 pygfx/controllers/_base.py
+pygfx/controllers/_fly.py
 pygfx/controllers/_orbit.py
 pygfx/controllers/_panzoom.py
+pygfx/controllers/_trackball.py
+pygfx/data_files/Humor-Sans.ttf
+pygfx/data_files/NotoSans-Regular.ttf
+pygfx/data_files/NotoSansArabic-Regular.ttf
+pygfx/data_files/NotoSansDevanagari-Regular.ttf
+pygfx/data_files/NotoSansSymbols-Regular.ttf
+pygfx/data_files/__init__.py
+pygfx/data_files/noto_default_index.json
 pygfx/geometries/__init__.py
 pygfx/geometries/_base.py
 pygfx/geometries/_box.py
 pygfx/geometries/_compat.py
 pygfx/geometries/_cylinder.py
 pygfx/geometries/_plane.py
 pygfx/geometries/_polyhedron.py
 pygfx/geometries/_sphere.py
+pygfx/geometries/_text.py
 pygfx/geometries/_toroidal.py
 pygfx/geometries/utils.py
 pygfx/helpers/__init__.py
 pygfx/helpers/_axes.py
 pygfx/helpers/_box.py
 pygfx/helpers/_gizmo.py
 pygfx/helpers/_grid.py
-pygfx/linalg/__init__.py
-pygfx/linalg/cylindrical.py
-pygfx/linalg/euler.py
-pygfx/linalg/matrix3.py
-pygfx/linalg/matrix4.py
-pygfx/linalg/quaternion.py
-pygfx/linalg/spherical.py
-pygfx/linalg/utils.py
-pygfx/linalg/vector3.py
-pygfx/linalg/vector4.py
+pygfx/helpers/_lights.py
+pygfx/helpers/_stats.py
 pygfx/materials/__init__.py
 pygfx/materials/_background.py
 pygfx/materials/_base.py
+pygfx/materials/_compat.py
 pygfx/materials/_image.py
 pygfx/materials/_line.py
 pygfx/materials/_mesh.py
 pygfx/materials/_points.py
+pygfx/materials/_text.py
 pygfx/materials/_volume.py
 pygfx/objects/__init__.py
 pygfx/objects/_base.py
 pygfx/objects/_events.py
 pygfx/objects/_instanced.py
+pygfx/objects/_lights.py
 pygfx/objects/_more.py
 pygfx/renderers/__init__.py
-pygfx/renderers/_base.py
 pygfx/renderers/svg/__init__.py
 pygfx/renderers/svg/_svgrenderer.py
 pygfx/renderers/svg/linerender.py
 pygfx/renderers/wgpu/__init__.py
-pygfx/renderers/wgpu/_blender.py
-pygfx/renderers/wgpu/_flusher.py
-pygfx/renderers/wgpu/_pipelinebuilder.py
-pygfx/renderers/wgpu/_renderer.py
-pygfx/renderers/wgpu/_shadercomposer.py
-pygfx/renderers/wgpu/_update.py
-pygfx/renderers/wgpu/_utils.py
-pygfx/renderers/wgpu/backgroundrender.py
-pygfx/renderers/wgpu/imagerender.py
-pygfx/renderers/wgpu/linerender.py
-pygfx/renderers/wgpu/meshrender.py
-pygfx/renderers/wgpu/pointsrender.py
-pygfx/renderers/wgpu/volumerender.py
+pygfx/renderers/wgpu/engine/__init__.py
+pygfx/renderers/wgpu/engine/blender.py
+pygfx/renderers/wgpu/engine/environment.py
+pygfx/renderers/wgpu/engine/flusher.py
+pygfx/renderers/wgpu/engine/mipmapsutil.py
+pygfx/renderers/wgpu/engine/pipeline.py
+pygfx/renderers/wgpu/engine/renderer.py
+pygfx/renderers/wgpu/engine/shadowutil.py
+pygfx/renderers/wgpu/engine/shared.py
+pygfx/renderers/wgpu/engine/update.py
+pygfx/renderers/wgpu/engine/utils.py
+pygfx/renderers/wgpu/shader/__init__.py
+pygfx/renderers/wgpu/shader/_shaderlib.py
+pygfx/renderers/wgpu/shader/base1.py
+pygfx/renderers/wgpu/shader/base2.py
+pygfx/renderers/wgpu/shaders/__init__.py
+pygfx/renderers/wgpu/shaders/backgroundshader.py
+pygfx/renderers/wgpu/shaders/imageshader.py
+pygfx/renderers/wgpu/shaders/lineshader.py
+pygfx/renderers/wgpu/shaders/meshshader.py
+pygfx/renderers/wgpu/shaders/pointsshader.py
+pygfx/renderers/wgpu/shaders/textshader.py
+pygfx/renderers/wgpu/shaders/volumeshader.py
+pygfx/renderers/wgpu/wgsl/__init__.py
+pygfx/renderers/wgpu/wgsl/line.wgsl
+pygfx/renderers/wgpu/wgsl/points.wgsl
 pygfx/resources/__init__.py
+pygfx/resources/_base.py
 pygfx/resources/_buffer.py
 pygfx/resources/_texture.py
 pygfx/utils/__init__.py
 pygfx/utils/_cmdata_mpl.py
+pygfx/utils/_dirs.py
 pygfx/utils/cm.py
 pygfx/utils/color.py
+pygfx/utils/cube_camera.py
+pygfx/utils/enums.py
+pygfx/utils/gallery_scraper.py
+pygfx/utils/load.py
+pygfx/utils/renderfunctionregistry.py
 pygfx/utils/show.py
-pygfx/utils/viewport.py
+pygfx/utils/trackable.py
+pygfx/utils/transform.py
+pygfx/utils/viewport.py
+pygfx/utils/text/__init__.py
+pygfx/utils/text/_atlas.py
+pygfx/utils/text/_fontfinder.py
+pygfx/utils/text/_fontmanager.py
+pygfx/utils/text/_sdf.py
+pygfx/utils/text/_shaper.py
+pygfx/utils/text/_tokenizers.py
+tests/test_basics.py
+tests/test_data.py
+tests/testutils.py
```

