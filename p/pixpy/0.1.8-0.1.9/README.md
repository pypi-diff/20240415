# Comparing `tmp/pixpy-0.1.8.tar.gz` & `tmp/pixpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixpy-0.1.8.tar", last modified: Fri Dec 16 22:21:23 2022, max compression
+gzip compressed data, was "pixpy-0.1.9.tar", last modified: Mon Jan  2 17:11:21 2023, max compression
```

## Comparing `pixpy-0.1.8.tar` & `pixpy-0.1.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.296848 pixpy-0.1.8/
--rw-r--r--   0 sasq       (501) staff       (20)     5422 2022-12-15 08:52:43.000000 pixpy-0.1.8/CMakeLists.txt
--rw-r--r--   0 sasq       (501) staff       (20)     1053 2022-11-26 12:55:33.000000 pixpy-0.1.8/LICENSE.md
--rw-r--r--   0 sasq       (501) staff       (20)      245 2022-12-15 08:52:43.000000 pixpy-0.1.8/MANIFEST.in
--rw-r--r--   0 sasq       (501) staff       (20)     6898 2022-12-16 22:21:23.296675 pixpy-0.1.8/PKG-INFO
--rw-r--r--   0 sasq       (501) staff       (20)     5520 2022-12-15 08:52:43.000000 pixpy-0.1.8/README.md
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.265586 pixpy-0.1.8/external/
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.269123 pixpy-0.1.8/external/lodepng/
--rw-r--r--   0 sasq       (501) staff       (20)   216665 2022-10-31 10:33:36.000000 pixpy-0.1.8/external/lodepng/lodepng.cpp
--rw-r--r--   0 sasq       (501) staff       (20)    79144 2022-10-31 10:33:36.000000 pixpy-0.1.8/external/lodepng/lodepng.h
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.270017 pixpy-0.1.8/external/pybind11/
--rw-r--r--   0 sasq       (501) staff       (20)    11687 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/CMakeLists.txt
--rw-r--r--   0 sasq       (501) staff       (20)     1684 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/LICENSE
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.265709 pixpy-0.1.8/external/pybind11/include/
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.274711 pixpy-0.1.8/external/pybind11/include/pybind11/
--rw-r--r--   0 sasq       (501) staff       (20)    23979 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/attr.h
--rw-r--r--   0 sasq       (501) staff       (20)     7069 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 sasq       (501) staff       (20)    65705 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/cast.h
--rw-r--r--   0 sasq       (501) staff       (20)     8458 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 sasq       (501) staff       (20)      120 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/common.h
--rw-r--r--   0 sasq       (501) staff       (20)     2096 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.276222 pixpy-0.1.8/external/pybind11/include/pybind11/detail/
--rw-r--r--   0 sasq       (501) staff       (20)    28251 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 sasq       (501) staff       (20)    50087 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 sasq       (501) staff       (20)     5491 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 sasq       (501) staff       (20)    17981 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 sasq       (501) staff       (20)    24651 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 sasq       (501) staff       (20)    42266 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 sasq       (501) staff       (20)     1625 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 sasq       (501) staff       (20)    32147 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 sasq       (501) staff       (20)    11792 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/embed.h
--rw-r--r--   0 sasq       (501) staff       (20)     4731 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/eval.h
--rw-r--r--   0 sasq       (501) staff       (20)     4695 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/functional.h
--rw-r--r--   0 sasq       (501) staff       (20)     7457 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/gil.h
--rw-r--r--   0 sasq       (501) staff       (20)     8862 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 sasq       (501) staff       (20)    79524 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 sasq       (501) staff       (20)     9051 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/operators.h
--rw-r--r--   0 sasq       (501) staff       (20)     2181 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/options.h
--rw-r--r--   0 sasq       (501) staff       (20)   126301 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 sasq       (501) staff       (20)    92159 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.276480 pixpy-0.1.8/external/pybind11/include/pybind11/stl/
--rw-r--r--   0 sasq       (501) staff       (20)     4185 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 sasq       (501) staff       (20)    15337 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/stl.h
--rw-r--r--   0 sasq       (501) staff       (20)    27013 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.280160 pixpy-0.1.8/external/pybind11/tools/
--rw-r--r--   0 sasq       (501) staff       (20)     2350 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 sasq       (501) staff       (20)     3105 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 sasq       (501) staff       (20)    10890 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 sasq       (501) staff       (20)      817 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 sasq       (501) staff       (20)     1423 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/check-style.sh
--rw-r--r--   0 sasq       (501) staff       (20)      952 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 sasq       (501) staff       (20)     1040 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 sasq       (501) staff       (20)     1031 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/libsize.py
--rwxr-xr-x   0 sasq       (501) staff       (20)     1282 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/make_changelog.py
--rw-r--r--   0 sasq       (501) staff       (20)      196 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 sasq       (501) staff       (20)    13487 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 sasq       (501) staff       (20)     6930 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 sasq       (501) staff       (20)     8955 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 sasq       (501) staff       (20)     8359 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 sasq       (501) staff       (20)       94 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/pyproject.toml
--rw-r--r--   0 sasq       (501) staff       (20)     1965 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/setup_global.py.in
--rw-r--r--   0 sasq       (501) staff       (20)     1139 2022-10-31 10:33:37.000000 pixpy-0.1.8/external/pybind11/tools/setup_main.py.in
--rw-r--r--   0 sasq       (501) staff       (20)      451 2022-12-16 21:43:43.000000 pixpy-0.1.8/pyproject.toml
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.266120 pixpy-0.1.8/python/
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.281761 pixpy-0.1.8/python/pixpy/
--rw-r--r--   0 sasq       (501) staff       (20)      138 2022-12-15 14:26:42.000000 pixpy-0.1.8/python/pixpy/__init__.py
--rw-r--r--   0 sasq       (501) staff       (20)    26388 2022-12-16 21:43:43.000000 pixpy-0.1.8/python/pixpy/__init__.pyi
--rw-r--r--   0 sasq       (501) staff       (20)       60 2022-12-12 15:21:44.000000 pixpy-0.1.8/python/pixpy/__main__.py
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.283055 pixpy-0.1.8/python/pixpy/color/
--rw-r--r--   0 sasq       (501) staff       (20)      654 2022-12-15 18:17:34.000000 pixpy-0.1.8/python/pixpy/color/__init__.pyi
--rw-r--r--   0 sasq       (501) staff       (20)     5082 2022-12-12 15:21:44.000000 pixpy-0.1.8/python/pixpy/editor.py
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.283462 pixpy-0.1.8/python/pixpy/event/
--rw-r--r--   0 sasq       (501) staff       (20)     1933 2022-12-15 18:17:34.000000 pixpy-0.1.8/python/pixpy/event/__init__.pyi
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.283765 pixpy-0.1.8/python/pixpy/key/
--rw-r--r--   0 sasq       (501) staff       (20)     1209 2022-12-15 18:17:34.000000 pixpy-0.1.8/python/pixpy/key/__init__.pyi
--rw-r--r--   0 sasq       (501) staff       (20)        0 2022-12-12 15:21:44.000000 pixpy-0.1.8/python/pixpy/py.typed
--rw-r--r--   0 sasq       (501) staff       (20)     5072 2022-12-15 08:52:43.000000 pixpy-0.1.8/python/pixpy/repl.py
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.282863 pixpy-0.1.8/python/pixpy.egg-info/
--rw-r--r--   0 sasq       (501) staff       (20)     6898 2022-12-16 22:21:23.000000 pixpy-0.1.8/python/pixpy.egg-info/PKG-INFO
--rw-r--r--   0 sasq       (501) staff       (20)     3427 2022-12-16 22:21:23.000000 pixpy-0.1.8/python/pixpy.egg-info/SOURCES.txt
--rw-r--r--   0 sasq       (501) staff       (20)        1 2022-12-16 22:21:23.000000 pixpy-0.1.8/python/pixpy.egg-info/dependency_links.txt
--rw-r--r--   0 sasq       (501) staff       (20)        1 2022-12-15 08:27:03.000000 pixpy-0.1.8/python/pixpy.egg-info/not-zip-safe
--rw-r--r--   0 sasq       (501) staff       (20)        6 2022-12-16 22:21:23.000000 pixpy-0.1.8/python/pixpy.egg-info/top_level.txt
--rw-r--r--   0 sasq       (501) staff       (20)       38 2022-12-16 22:21:23.296887 pixpy-0.1.8/setup.cfg
--rw-r--r--   0 sasq       (501) staff       (20)      406 2022-12-16 21:43:43.000000 pixpy-0.1.8/setup.py
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.292716 pixpy-0.1.8/src/
--rw-r--r--   0 sasq       (501) staff       (20)     1255 2022-11-09 19:29:58.000000 pixpy-0.1.8/src/colors.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     9632 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/context.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     2723 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/context.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     3254 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/eglutil.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     4817 2022-11-28 19:09:13.000000 pixpy-0.1.8/src/font.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     1639 2022-11-22 06:24:43.000000 pixpy-0.1.8/src/font.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     4489 2022-12-12 15:21:44.000000 pixpy-0.1.8/src/full_console.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     2348 2022-12-12 15:21:44.000000 pixpy-0.1.8/src/full_console.hpp
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.294489 pixpy-0.1.8/src/gl/
--rw-r--r--   0 sasq       (501) staff       (20)     3024 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/buffer.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1222 2022-11-06 10:49:43.000000 pixpy-0.1.8/src/gl/color.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     7162 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/functions.hpp
--rw-r--r--   0 sasq       (501) staff       (20)      474 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/gl.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     4151 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/program.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     3643 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/program_cache.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1502 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/gl/shader.hpp
--rw-r--r--   0 sasq       (501) staff       (20)    12268 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/gl/texture.hpp
--rw-r--r--   0 sasq       (501) staff       (20)   252470 2022-11-27 21:30:07.000000 pixpy-0.1.8/src/glad.h
--rw-r--r--   0 sasq       (501) staff       (20)    10425 2022-12-16 21:43:43.000000 pixpy-0.1.8/src/glfw_system.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     2309 2022-11-20 16:10:49.000000 pixpy-0.1.8/src/image.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     1353 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/image.hpp
--rw-r--r--   0 sasq       (501) staff       (20)    25544 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/jpeg_decoder.h
--rw-r--r--   0 sasq       (501) staff       (20)     1827 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/keycodes.h
--rw-r--r--   0 sasq       (501) staff       (20)      265 2022-11-01 18:30:42.000000 pixpy-0.1.8/src/machine.hpp
--rw-r--r--   0 sasq       (501) staff       (20)    11664 2022-11-09 19:29:58.000000 pixpy-0.1.8/src/pi_system.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     7919 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/pixel_console.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     2750 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/pixel_console.hpp
-drwxr-xr-x   0 sasq       (501) staff       (20)        0 2022-12-16 22:21:23.296280 pixpy-0.1.8/src/python/
--rw-r--r--   0 sasq       (501) staff       (20)     4261 2022-12-16 21:43:43.000000 pixpy-0.1.8/src/python/class_console.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     6534 2022-12-16 21:43:43.000000 pixpy-0.1.8/src/python/class_context.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1391 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/python/class_font.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     3294 2022-12-16 21:43:43.000000 pixpy-0.1.8/src/python/class_image.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1385 2022-12-12 15:21:44.000000 pixpy-0.1.8/src/python/class_screen.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1439 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/python/class_tileset.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     7327 2022-12-16 21:43:43.000000 pixpy-0.1.8/src/python/class_vec2.hpp
--rw-r--r--   0 sasq       (501) staff       (20)      811 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/python/mod_color.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     2666 2022-12-16 21:41:52.000000 pixpy-0.1.8/src/python/mod_event.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     1036 2022-12-02 15:01:01.000000 pixpy-0.1.8/src/python/mod_key.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     6291 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/python.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     4773 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/system.hpp
--rw-r--r--   0 sasq       (501) staff       (20)     4096 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/tile_set.cpp
--rw-r--r--   0 sasq       (501) staff       (20)     1314 2022-12-15 08:52:43.000000 pixpy-0.1.8/src/tile_set.hpp
--rw-r--r--   0 sasq       (501) staff       (20)  1730899 2022-10-31 10:33:37.000000 pixpy-0.1.8/src/unscii-16.h
--rw-r--r--   0 sasq       (501) staff       (20)     5690 2022-11-07 20:51:52.000000 pixpy-0.1.8/src/utf8.h
--rw-r--r--   0 sasq       (501) staff       (20)     5688 2022-12-12 15:21:44.000000 pixpy-0.1.8/src/vec2.hpp
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.433908 pixpy-0.1.9/
+-rw-r--r--   0 sasq       (501) staff       (20)     5451 2023-01-01 16:52:44.000000 pixpy-0.1.9/CMakeLists.txt
+-rw-r--r--   0 sasq       (501) staff       (20)     1053 2022-11-26 12:55:33.000000 pixpy-0.1.9/LICENSE.md
+-rw-r--r--   0 sasq       (501) staff       (20)      245 2022-12-15 08:52:43.000000 pixpy-0.1.9/MANIFEST.in
+-rw-r--r--   0 sasq       (501) staff       (20)     6898 2023-01-02 17:11:21.433753 pixpy-0.1.9/PKG-INFO
+-rw-r--r--   0 sasq       (501) staff       (20)     5520 2023-01-02 16:04:11.000000 pixpy-0.1.9/README.md
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.401186 pixpy-0.1.9/external/
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.404125 pixpy-0.1.9/external/lodepng/
+-rw-r--r--   0 sasq       (501) staff       (20)   216665 2022-10-31 10:33:36.000000 pixpy-0.1.9/external/lodepng/lodepng.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)    79144 2022-10-31 10:33:36.000000 pixpy-0.1.9/external/lodepng/lodepng.h
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.405025 pixpy-0.1.9/external/pybind11/
+-rw-r--r--   0 sasq       (501) staff       (20)    11687 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/CMakeLists.txt
+-rw-r--r--   0 sasq       (501) staff       (20)     1684 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/LICENSE
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.401300 pixpy-0.1.9/external/pybind11/include/
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.409468 pixpy-0.1.9/external/pybind11/include/pybind11/
+-rw-r--r--   0 sasq       (501) staff       (20)    23979 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 sasq       (501) staff       (20)     7069 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 sasq       (501) staff       (20)    65705 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 sasq       (501) staff       (20)     8458 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 sasq       (501) staff       (20)      120 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/common.h
+-rw-r--r--   0 sasq       (501) staff       (20)     2096 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.410850 pixpy-0.1.9/external/pybind11/include/pybind11/detail/
+-rw-r--r--   0 sasq       (501) staff       (20)    28251 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 sasq       (501) staff       (20)    50087 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 sasq       (501) staff       (20)     5491 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 sasq       (501) staff       (20)    17981 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 sasq       (501) staff       (20)    24651 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 sasq       (501) staff       (20)    42266 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 sasq       (501) staff       (20)     1625 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 sasq       (501) staff       (20)    32147 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 sasq       (501) staff       (20)    11792 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 sasq       (501) staff       (20)     4731 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 sasq       (501) staff       (20)     4695 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 sasq       (501) staff       (20)     7457 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 sasq       (501) staff       (20)     8862 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 sasq       (501) staff       (20)    79524 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 sasq       (501) staff       (20)     9051 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 sasq       (501) staff       (20)     2181 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/options.h
+-rw-r--r--   0 sasq       (501) staff       (20)   126301 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 sasq       (501) staff       (20)    92159 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.410998 pixpy-0.1.9/external/pybind11/include/pybind11/stl/
+-rw-r--r--   0 sasq       (501) staff       (20)     4185 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 sasq       (501) staff       (20)    15337 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 sasq       (501) staff       (20)    27013 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.414301 pixpy-0.1.9/external/pybind11/tools/
+-rw-r--r--   0 sasq       (501) staff       (20)     2350 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)     3105 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)    10890 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)      817 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 sasq       (501) staff       (20)     1423 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/check-style.sh
+-rw-r--r--   0 sasq       (501) staff       (20)      952 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 sasq       (501) staff       (20)     1040 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 sasq       (501) staff       (20)     1031 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/libsize.py
+-rwxr-xr-x   0 sasq       (501) staff       (20)     1282 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/make_changelog.py
+-rw-r--r--   0 sasq       (501) staff       (20)      196 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 sasq       (501) staff       (20)    13487 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)     6930 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 sasq       (501) staff       (20)     8955 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)     8359 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 sasq       (501) staff       (20)       94 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/pyproject.toml
+-rw-r--r--   0 sasq       (501) staff       (20)     1965 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 sasq       (501) staff       (20)     1139 2022-10-31 10:33:37.000000 pixpy-0.1.9/external/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 sasq       (501) staff       (20)      451 2023-01-02 16:03:43.000000 pixpy-0.1.9/pyproject.toml
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.401679 pixpy-0.1.9/python/
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.416090 pixpy-0.1.9/python/pixpy/
+-rw-r--r--   0 sasq       (501) staff       (20)      138 2022-12-15 14:26:42.000000 pixpy-0.1.9/python/pixpy/__init__.py
+-rw-r--r--   0 sasq       (501) staff       (20)    28242 2022-12-30 07:39:02.000000 pixpy-0.1.9/python/pixpy/__init__.pyi
+-rw-r--r--   0 sasq       (501) staff       (20)       60 2022-12-12 15:21:44.000000 pixpy-0.1.9/python/pixpy/__main__.py
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.417058 pixpy-0.1.9/python/pixpy/color/
+-rw-r--r--   0 sasq       (501) staff       (20)      654 2022-12-30 07:39:02.000000 pixpy-0.1.9/python/pixpy/color/__init__.pyi
+-rw-r--r--   0 sasq       (501) staff       (20)     5082 2022-12-12 15:21:44.000000 pixpy-0.1.9/python/pixpy/editor.py
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.417318 pixpy-0.1.9/python/pixpy/event/
+-rw-r--r--   0 sasq       (501) staff       (20)     1933 2022-12-30 07:39:02.000000 pixpy-0.1.9/python/pixpy/event/__init__.pyi
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.417546 pixpy-0.1.9/python/pixpy/key/
+-rw-r--r--   0 sasq       (501) staff       (20)     1209 2022-12-30 07:39:02.000000 pixpy-0.1.9/python/pixpy/key/__init__.pyi
+-rw-r--r--   0 sasq       (501) staff       (20)        0 2022-12-12 15:21:44.000000 pixpy-0.1.9/python/pixpy/py.typed
+-rw-r--r--   0 sasq       (501) staff       (20)     5072 2022-12-15 08:52:43.000000 pixpy-0.1.9/python/pixpy/repl.py
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.416928 pixpy-0.1.9/python/pixpy.egg-info/
+-rw-r--r--   0 sasq       (501) staff       (20)     6898 2023-01-02 17:11:21.000000 pixpy-0.1.9/python/pixpy.egg-info/PKG-INFO
+-rw-r--r--   0 sasq       (501) staff       (20)     3427 2023-01-02 17:11:21.000000 pixpy-0.1.9/python/pixpy.egg-info/SOURCES.txt
+-rw-r--r--   0 sasq       (501) staff       (20)        1 2023-01-02 17:11:21.000000 pixpy-0.1.9/python/pixpy.egg-info/dependency_links.txt
+-rw-r--r--   0 sasq       (501) staff       (20)        1 2023-01-02 16:01:27.000000 pixpy-0.1.9/python/pixpy.egg-info/not-zip-safe
+-rw-r--r--   0 sasq       (501) staff       (20)        6 2023-01-02 17:11:21.000000 pixpy-0.1.9/python/pixpy.egg-info/top_level.txt
+-rw-r--r--   0 sasq       (501) staff       (20)       38 2023-01-02 17:11:21.433942 pixpy-0.1.9/setup.cfg
+-rw-r--r--   0 sasq       (501) staff       (20)      406 2023-01-02 16:03:53.000000 pixpy-0.1.9/setup.py
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.426341 pixpy-0.1.9/src/
+-rw-r--r--   0 sasq       (501) staff       (20)     1255 2022-11-09 19:29:58.000000 pixpy-0.1.9/src/colors.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)    11493 2023-01-02 15:48:47.000000 pixpy-0.1.9/src/context.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     3340 2022-12-30 18:10:51.000000 pixpy-0.1.9/src/context.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     3254 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/eglutil.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     4817 2022-11-28 19:09:13.000000 pixpy-0.1.9/src/font.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1639 2022-11-22 06:24:43.000000 pixpy-0.1.9/src/font.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     4489 2022-12-12 15:21:44.000000 pixpy-0.1.9/src/full_console.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     2348 2022-12-12 15:21:44.000000 pixpy-0.1.9/src/full_console.hpp
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.430983 pixpy-0.1.9/src/gl/
+-rw-r--r--   0 sasq       (501) staff       (20)     3024 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/gl/buffer.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1222 2022-11-06 10:49:43.000000 pixpy-0.1.9/src/gl/color.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     7162 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/gl/functions.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)      474 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/gl/gl.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     4151 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/gl/program.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     3643 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/gl/program_cache.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1502 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/gl/shader.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)    11734 2023-01-02 11:38:01.000000 pixpy-0.1.9/src/gl/texture.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)   252470 2022-11-27 21:30:07.000000 pixpy-0.1.9/src/glad.h
+-rw-r--r--   0 sasq       (501) staff       (20)    11596 2023-01-02 11:38:01.000000 pixpy-0.1.9/src/glfw_system.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     2309 2022-11-20 16:10:49.000000 pixpy-0.1.9/src/image.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1353 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/image.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)    25544 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/jpeg_decoder.h
+-rw-r--r--   0 sasq       (501) staff       (20)     1827 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/keycodes.h
+-rw-r--r--   0 sasq       (501) staff       (20)      265 2022-11-01 18:30:42.000000 pixpy-0.1.9/src/machine.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)    11882 2023-01-01 19:26:42.000000 pixpy-0.1.9/src/pi_system.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     8003 2022-12-27 15:13:37.000000 pixpy-0.1.9/src/pixel_console.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     2769 2022-12-27 14:38:46.000000 pixpy-0.1.9/src/pixel_console.hpp
+drwxr-xr-x   0 sasq       (501) staff       (20)        0 2023-01-02 17:11:21.433439 pixpy-0.1.9/src/python/
+-rw-r--r--   0 sasq       (501) staff       (20)     4301 2022-12-26 21:48:10.000000 pixpy-0.1.9/src/python/class_console.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     7129 2023-01-01 18:56:52.000000 pixpy-0.1.9/src/python/class_context.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1391 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/python/class_font.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     3340 2022-12-30 06:57:27.000000 pixpy-0.1.9/src/python/class_image.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1989 2022-12-28 11:42:55.000000 pixpy-0.1.9/src/python/class_screen.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1411 2022-12-26 21:59:11.000000 pixpy-0.1.9/src/python/class_tileset.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     7327 2022-12-16 21:43:43.000000 pixpy-0.1.9/src/python/class_vec2.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)      811 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/python/mod_color.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     2666 2022-12-16 21:41:52.000000 pixpy-0.1.9/src/python/mod_event.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1036 2022-12-02 15:01:01.000000 pixpy-0.1.9/src/python/mod_key.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     6251 2022-12-30 06:36:35.000000 pixpy-0.1.9/src/python.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     4987 2022-12-28 09:42:32.000000 pixpy-0.1.9/src/system.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)     4096 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/tile_set.cpp
+-rw-r--r--   0 sasq       (501) staff       (20)     1314 2022-12-15 08:52:43.000000 pixpy-0.1.9/src/tile_set.hpp
+-rw-r--r--   0 sasq       (501) staff       (20)  1730899 2022-10-31 10:33:37.000000 pixpy-0.1.9/src/unscii-16.h
+-rw-r--r--   0 sasq       (501) staff       (20)     5237 2022-12-27 15:56:35.000000 pixpy-0.1.9/src/utf8.h
+-rw-r--r--   0 sasq       (501) staff       (20)     5688 2022-12-12 15:21:44.000000 pixpy-0.1.9/src/vec2.hpp
```

### Comparing `pixpy-0.1.8/CMakeLists.txt` & `pixpy-0.1.9/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 endif()
 
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
 include(ExternalProject)
 include(FetchContent)
 
+if (EXISTS /opt/vc)
+    set(RASPBERRY_PI 1)
+endif ()
+
 set(FT_REQUIRE_ZLIB OFF)
 set(FT_REQUIRE_BZIP2 OFF)
 set(FT_REQUIRE_PNG OFF)
 set(FT_REQUIRE_HARFBUZZ OFF)
 set(FT_REQUIRE_BROTLI OFF)
 
 set(FT_DISABLE_ZLIB ON CACHE BOOL "")
@@ -25,38 +29,36 @@
     URL https://download.savannah.gnu.org/releases/freetype/freetype-2.12.1.tar.gz)
 set(FT_DISABLE_ZLIB ON CACHE BOOL "")
 set(FT_DISABLE_BZIP2 ON CACHE BOOL "")
 set(FT_DISABLE_PNG ON CACHE BOOL "")
 set(FT_DISABLE_HARFBUZZ ON CACHE BOOL "")
 set(FT_DISABLE_BROTLI ON CACHE BOOL "")
 
-set(GLFW_BUILD_DOCS OFF CACHE BOOL "")
-FetchContent_Declare(glfw
-    GIT_REPOSITORY https://github.com/glfw/glfw)
+if (NOT RASPBERRY_PI)
+  set(GLFW_BUILD_DOCS OFF CACHE BOOL "")
+  FetchContent_Declare(glfw
+      GIT_REPOSITORY https://github.com/glfw/glfw)
 
-FetchContent_Populate(glfw)
-add_subdirectory(${glfw_SOURCE_DIR} ${glfw_BINARY_DIR} EXCLUDE_FROM_ALL)
+   FetchContent_Populate(glfw)
+   add_subdirectory(${glfw_SOURCE_DIR} ${glfw_BINARY_DIR} EXCLUDE_FROM_ALL)
+endif()
 
 FetchContent_Populate(freetype)
 add_subdirectory(${freetype_SOURCE_DIR} ${freetype_BINARY_DIR} EXCLUDE_FROM_ALL)
 
 #FetchContent_MakeAvailable(glfw freetype)
 add_library(Freetype::Freetype ALIAS freetype)
 
 set(CMAKE_EXPORT_COMPILE_COMMANDS 1)
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 #set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fsanitize=address -g")
 
 cmake_policy(SET CMP0072 NEW)
 
-if (EXISTS /opt/vc)
-    set(RASPBERRY_PI 1)
-endif ()
-
 # System wide directories and flags
 
 if (RASPBERRY_PI)
     set(VC /opt/vc)
     include_directories(SYSTEM
         ${VC}/include
         ${VC}/include/interface/vcos/pthreads
@@ -101,15 +103,15 @@
     -Wno-unused-function)
 
 set(MSVC_WARNINGS /W2 /wd4244)
 
 # GCC specific warnings
 set(GCC_WARNINGS -Wno-duplicated-branches -Wduplicated-cond -Wlogical-op
     -Wno-error=stringop-overflow
-    -Wcast-align -Wno-missing-field-initializers)
+    -Wno-missing-field-initializers)
 
 if ("${CMAKE_CXX_COMPILER_ID}" STREQUAL "GNU")
     set(WARNINGS ${WARNINGS} ${GCC_WARNINGS} ${GCC_CLANG_WARNINGS})
 elseif (CMAKE_CXX_COMPILER_ID MATCHES "Clang")
     set(WARNINGS ${WARNINGS} ${CLANG_WARNINGS} ${GCC_CLANG_WARNINGS})
 elseif ("${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC")
     set(WARNINGS ${WARNINGS} ${MSVC_WARNINGS})
```

### Comparing `pixpy-0.1.8/LICENSE.md` & `pixpy-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/PKG-INFO` & `pixpy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Graphics library
 Author-email: Jonas Minnberg <sasq64@gmail.com>
 License: Copyright 2022 Jonas Minnberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `pixpy-0.1.8/README.md` & `pixpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/lodepng/lodepng.cpp` & `pixpy-0.1.9/external/lodepng/lodepng.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/lodepng/lodepng.h` & `pixpy-0.1.9/external/lodepng/lodepng.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/CMakeLists.txt` & `pixpy-0.1.9/external/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/LICENSE` & `pixpy-0.1.9/external/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/attr.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/buffer_info.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/cast.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/chrono.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/complex.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/class.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/common.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/descr.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/init.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/internals.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/type_caster_base.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/detail/typeid.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/eigen.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/embed.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/eval.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/functional.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/gil.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/iostream.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/numpy.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/operators.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/options.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/pybind11.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/pytypes.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/stl/filesystem.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/stl.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/include/pybind11/stl_bind.h` & `pixpy-0.1.9/external/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/FindCatch.cmake` & `pixpy-0.1.9/external/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/FindEigen3.cmake` & `pixpy-0.1.9/external/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/FindPythonLibsNew.cmake` & `pixpy-0.1.9/external/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/JoinPaths.cmake` & `pixpy-0.1.9/external/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/check-style.sh` & `pixpy-0.1.9/external/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/cmake_uninstall.cmake.in` & `pixpy-0.1.9/external/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pixpy-0.1.9/external/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/libsize.py` & `pixpy-0.1.9/external/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/make_changelog.py` & `pixpy-0.1.9/external/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/pybind11Common.cmake` & `pixpy-0.1.9/external/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/pybind11Config.cmake.in` & `pixpy-0.1.9/external/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/pybind11NewTools.cmake` & `pixpy-0.1.9/external/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/pybind11Tools.cmake` & `pixpy-0.1.9/external/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/setup_global.py.in` & `pixpy-0.1.9/external/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/external/pybind11/tools/setup_main.py.in` & `pixpy-0.1.9/external/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy/__init__.pyi` & `pixpy-0.1.9/python/pixpy/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,18 @@
         Clear the console.
         """
     def get(self, arg0: Union[Int2, Tuple[int, int]]) -> int:
         """
         Get tile at position
         """
     def get_font_image(self) -> Image: ...
-    def get_image_for(self, tile: int) -> Image: ...
+    def get_image_for(self, tile: int) -> Image:
+        """
+        Get the image of a specific tile. Use to render the tile manually, or to copy another image into the tile.
+        """
     def get_tiles(self) -> typing.List[int]:
         """
         Get all the tiles and colors as an array of ints. Format is: [tile0, fg0, bg0, tile1, fg1, bg1 ...] etc.
         """
     def put(self, pos: Union[Int2, Tuple[int, int]], tile: int, fg: typing.Optional[int] = None, bg: typing.Optional[int] = None) -> None:
         """
         Put tile at position, optionally setting a specific foreground and/or background color
@@ -134,28 +137,32 @@
         Draw an (outline) circle
         """
     def clear(self, color: int = 0) -> None:
         """
         Clear the context using given color.
         """
     @typing.overload
-    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000)) -> None:
+    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000)) -> None:
         """
         Render an image. The image can either be aligned to its top left corner, or centered, in which case it can also be rotated.
         """
     @typing.overload
-    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000), rot: float = 0) -> None: ...
+    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), rot: float = 0) -> None: ...
     def filled_circle(self, center: Union[Float2, Tuple[float, float]], radius: float) -> None:
         """
         Draw a filled circle.
         """
     def filled_rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a filled rectangle.
         """
+    def flush(self) -> None:
+        """
+        Flush pixel operations
+        """
     @typing.overload
     def line(self, end: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a line between start and end.
 
         Draw a line from the end of the last line to the given position.
         """
@@ -174,14 +181,18 @@
         """
         Draw a convex polygon.
         """
     def rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a rectangle.
         """
+    def set_pixel(self, pos: Union[Int2, Tuple[int, int]], color: int) -> None:
+        """
+        Write a pixel into the image.
+        """
     @property
     def clip_size(self) -> Int2:
         """
         :type: Union[Int2, Tuple[int, int]]
         """
     @clip_size.setter
     def clip_size(self, arg1: Union[Int2, Tuple[int, int]]) -> None:
@@ -236,14 +247,19 @@
         Set the point size in fractional pixels.
         """
     @property
     def size(self) -> Float2:
         """
         :type: Union[Float2, Tuple[float, float]]
         """
+    @property
+    def target_size(self) -> Float2:
+        """
+        :type: Union[Float2, Tuple[float, float]]
+        """
     pass
 class Float2():
     @typing.overload
     def __add__(self, arg0: Union[Float2, Tuple[float, float]]) -> Float2: ...
     @typing.overload
     def __add__(self, arg0: Union[Int2, Tuple[int, int]]) -> Float2: ...
     @typing.overload
@@ -342,47 +358,63 @@
         """
     UNSCII_FONT: Font
     pass
 class Image():
     @typing.overload
     def __init__(self, size: Union[Float2, Tuple[float, float]]) -> None:
         """
-        Splits the image into as many _width_ * _height_ images as possible, first going left to right, then top to bottom.
+        Create an empty image of the given size.
+
+        Create an empty image of the given size.
+
+        Create an image from an array of 32-bit colors.
         """
     @typing.overload
     def __init__(self, width: int, height: int) -> None: ...
     @typing.overload
     def __init__(self, width: int, pixels: typing.List[int]) -> None: ...
-    def bind(self, unit: int = 0) -> None: ...
     def circle(self, center: Union[Float2, Tuple[float, float]], radius: float) -> None:
         """
         Draw an (outline) circle
         """
     def clear(self, color: int = 0) -> None:
         """
         Clear the context using given color.
         """
-    def copy_from(self, image: Image) -> None: ...
-    def copy_to(self, image: Image) -> None: ...
-    def crop(self, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: typing.Optional[Union[Float2, Tuple[float, float]]] = None) -> Image: ...
+    def copy_from(self, image: Image) -> None:
+        """
+        Render one image into another.
+        """
+    def copy_to(self, image: Image) -> None:
+        """
+        Render one image into another.
+        """
+    def crop(self, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: typing.Optional[Union[Float2, Tuple[float, float]]] = None) -> Image:
+        """
+        Crop an image. Returns a view into the old image.
+        """
     @typing.overload
-    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000)) -> None:
+    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000)) -> None:
         """
         Render an image. The image can either be aligned to its top left corner, or centered, in which case it can also be rotated.
         """
     @typing.overload
-    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000), rot: float = 0) -> None: ...
+    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), rot: float = 0) -> None: ...
     def filled_circle(self, center: Union[Float2, Tuple[float, float]], radius: float) -> None:
         """
         Draw a filled circle.
         """
     def filled_rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a filled rectangle.
         """
+    def flush(self) -> None:
+        """
+        Flush pixel operations
+        """
     @typing.overload
     def line(self, end: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a line between start and end.
 
         Draw a line from the end of the last line to the given position.
         """
@@ -401,15 +433,18 @@
         """
         Draw a convex polygon.
         """
     def rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a rectangle.
         """
-    def set_as_target(self) -> None: ...
+    def set_pixel(self, pos: Union[Int2, Tuple[int, int]], color: int) -> None:
+        """
+        Write a pixel into the image.
+        """
     @typing.overload
     def split(self, cols: int = -1, rows: int = -1, width: int = 8, height: int = 8) -> typing.List[Image]:
         """
         Splits the image into as many _width_ * _height_ images as possible, first going left to right, then top to bottom.
         """
     @typing.overload
     def split(self, size: Union[Float2, Tuple[float, float]]) -> typing.List[Image]: ...
@@ -474,22 +509,29 @@
     def point_size(self, arg1: float) -> None:
         """
         Set the point size in fractional pixels.
         """
     @property
     def pos(self) -> Float2:
         """
+        The position of this image in its texture. Will normally be (0, 0) unless this image was split or cropped from another image.
+
         :type: Union[Float2, Tuple[float, float]]
         """
     @property
     def size(self) -> Float2:
         """
         :type: Union[Float2, Tuple[float, float]]
         """
     @property
+    def target_size(self) -> Float2:
+        """
+        :type: Union[Float2, Tuple[float, float]]
+        """
+    @property
     def width(self) -> float:
         """
         :type: float
         """
     pass
 class Int2():
     @typing.overload
@@ -575,28 +617,32 @@
         Draw an (outline) circle
         """
     def clear(self, color: int = 0) -> None:
         """
         Clear the context using given color.
         """
     @typing.overload
-    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000)) -> None:
+    def draw(self, drawable: Console, top_left: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000)) -> None:
         """
         Render an image. The image can either be aligned to its top left corner, or centered, in which case it can also be rotated.
         """
     @typing.overload
-    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(-1.000000, -1.000000), rot: float = 0) -> None: ...
+    def draw(self, image: Image, top_left: typing.Optional[Union[Float2, Tuple[float, float]]] = None, center: typing.Optional[Union[Float2, Tuple[float, float]]] = None, size: Union[Float2, Tuple[float, float]] = Float2(0.000000, 0.000000), rot: float = 0) -> None: ...
     def filled_circle(self, center: Union[Float2, Tuple[float, float]], radius: float) -> None:
         """
         Draw a filled circle.
         """
     def filled_rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a filled rectangle.
         """
+    def flush(self) -> None:
+        """
+        Flush pixel operations
+        """
     @typing.overload
     def line(self, end: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a line between start and end.
 
         Draw a line from the end of the last line to the given position.
         """
@@ -616,14 +662,18 @@
         Draw a convex polygon.
         """
     def rect(self, top_left: Union[Float2, Tuple[float, float]], size: Union[Float2, Tuple[float, float]]) -> None:
         """
         Draw a rectangle.
         """
     def set_as_target(self) -> None: ...
+    def set_pixel(self, pos: Union[Int2, Tuple[int, int]], color: int) -> None:
+        """
+        Write a pixel into the image.
+        """
     def swap(self) -> None:
         """
         Synchronize with the frame rate of the display and swap buffers. This is normally the last thing you do in your render loop.
         """
     @property
     def clip_size(self) -> Int2:
         """
@@ -642,26 +692,41 @@
         pass
     @property
     def context(self) -> Context:
         """
         :type: Context
         """
     @property
+    def delta(self) -> float:
+        """
+        Time in seconds for last frame.
+
+        :type: float
+        """
+    @property
     def draw_color(self) -> int:
         """
         Set the draw color.
 
         :type: int
         """
     @draw_color.setter
     def draw_color(self, arg1: int) -> None:
         """
         Set the draw color.
         """
     @property
+    def fps(self) -> int:
+        """
+        :type: int
+        """
+    @fps.setter
+    def fps(self, arg1: int) -> None:
+        pass
+    @property
     def frame_counter(self) -> int:
         """
         :type: int
         """
     @property
     def height(self) -> int:
         """
@@ -688,19 +753,31 @@
         """
     @point_size.setter
     def point_size(self, arg1: float) -> None:
         """
         Set the point size in fractional pixels.
         """
     @property
+    def seconds(self) -> float:
+        """
+        Total seconds elapsed.
+
+        :type: float
+        """
+    @property
     def size(self) -> Float2:
         """
         :type: Union[Float2, Tuple[float, float]]
         """
     @property
+    def target_size(self) -> Float2:
+        """
+        :type: Union[Float2, Tuple[float, float]]
+        """
+    @property
     def width(self) -> int:
         """
         :type: int
         """
     pass
 class TileSet():
     @typing.overload
```

### Comparing `pixpy-0.1.8/python/pixpy/color/__init__.pyi` & `pixpy-0.1.9/python/pixpy/color/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy/editor.py` & `pixpy-0.1.9/python/pixpy/editor.py`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy/event/__init__.pyi` & `pixpy-0.1.9/python/pixpy/event/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy/key/__init__.pyi` & `pixpy-0.1.9/python/pixpy/key/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy/repl.py` & `pixpy-0.1.9/python/pixpy/repl.py`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/python/pixpy.egg-info/PKG-INFO` & `pixpy-0.1.9/python/pixpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Graphics library
 Author-email: Jonas Minnberg <sasq64@gmail.com>
 License: Copyright 2022 Jonas Minnberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `pixpy-0.1.8/python/pixpy.egg-info/SOURCES.txt` & `pixpy-0.1.9/python/pixpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/colors.hpp` & `pixpy-0.1.9/src/colors.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/context.cpp` & `pixpy-0.1.9/src/context.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -134,51 +134,51 @@
 {
     draw_filled(generate_circle(v, r, true), gl::Primitive::TriangleFan);
 }
 
 void Context::blit(gl::TexRef const& tex, Vec2f pos, Vec2f size)
 {
     tex.bind();
-    if (size.x < 0) {
+    if (size.x == 0) {
         size = {static_cast<float>(tex.width()),
                 static_cast<float>(tex.height())};
     }
     // auto vdata = generate_quad_with_uvs(pos.x, pos.y, size.x, size.y);
     auto vdata = generate_quad_with_uvs(pos, size);
     std::copy(tex.uvs().begin(), tex.uvs().end(), vdata.begin() + 8);
     draw_textured(vdata, gl::Primitive::TriangleFan);
 }
 
 void Context::draw(gl::TexRef const& tex, Vec2f center, Vec2f size, float rot)
 {
     tex.bind();
-    if (size.x < 0) {
+    if (size.x == 0) {
         size = {static_cast<float>(tex.width()),
                 static_cast<float>(tex.height())};
     }
     auto vdata = rotated_quad_with_uvs(center, size, rot);
     std::copy(tex.uvs().begin(), tex.uvs().end(), vdata.begin() + 8);
     draw_textured(vdata, gl::Primitive::TriangleFan);
 }
 
-Context::Context(Vec2f const& offs, Vec2f const& sz, GLuint fb)
-    : target{fb}, offset{offs}, target_size{sz}, fg{color::white},
+Context::Context(Vec2f _offset, Vec2f _view_size, Vec2f _target_size, GLuint fb)
+    : target{fb}, offset{_offset}, view_size{_view_size}, target_size{_target_size}, fg{color::white},
       colored{
           ProgramCache::get_instance()
               .get_program<ProgramCache::Colored, ProgramCache::NoTransform>()},
       textured{ProgramCache::get_instance()
                    .get_program<ProgramCache::Textured>()}, // NOLINT
       filled{ProgramCache::get_instance().get_program<>()} // NOLINT
 {
     // auto in_color = textured.getUniformLocation("in_color");
     // auto in_pos = textured.getAttribute("in_pos");
 }
 
 Context::Context(float w, float h, GLuint fb)
-    : Context(Vec2f{0, 0}, Vec2f{w, h}, fb)
+    : Context(Vec2f{0, 0}, Vec2f{w, h}, Vec2f{w,h}, fb)
 {
     static const std::array<float, 16> mat{1, 0, 0, 0, 0, 1, 0, 0,
                                            0, 0, 1, 0, 0, 0, 0, 1};
     gl::Color color = 0xffffffff;
     filled.setUniform("frag_color", color);
     filled.setUniform("in_transform", mat);
     textured.setUniform("frag_color", color);
@@ -208,15 +208,17 @@
     std::vector<float> data;
     for(unsigned i=0; i<count; i++) {
         auto&& p = to_screen(points[i]);
         data.push_back(p.x);
         data.push_back(p.y);
     }
 
+    glEnable(GL_CULL_FACE);
     draw_filled(data, gl::Primitive::TriangleFan);
+    glDisable(GL_CULL_FACE);
 
 }
 
 void Context::set_target() const
 {
     glBindFramebuffer(GL_FRAMEBUFFER, target);
     gl::setViewport({target_size.x * vpscale, target_size.y * vpscale});
@@ -304,9 +306,64 @@
 }
 void Context::flush()
 {
     if (!points.empty()) {
         draw_points();
         points.clear();
     }
+    flush_pixels();
+}
+void Context::set_pixel(int x, int y, uint32_t col)
+{
+    col = (col & 0x0000FFFF) << 16 | (col & 0xFFFF0000) >> 16;
+    col = (col & 0x00FF00FF) << 8 | (col & 0xFF00FF00) >> 8;
+
+    glBindFramebuffer(GL_FRAMEBUFFER, target);
+    int width = view_size.x;
+    int height = view_size.y;
+    if (pixels == nullptr) {
+        pixels = std::unique_ptr<uint32_t[]>(
+            new uint32_t[width * height]); // NOLINT
+        glReadPixels(0, 0, width, height, GL_RGBA, GL_UNSIGNED_BYTE,
+                     pixels.get());
+    }
+    dirty = true;
+    pixels[x + width * y] = col;
+}
+
+void Context::flush_pixels()
+{
+    if (dirty) {
+        // TODO: Better way of drawing to a FBO than creating a temporary
+        // texture and drawing a quad?
+
+        int width = view_size.x;
+        int height = view_size.y;
+        int x = offset.x;
+        int y = offset.y;
+
+        if (texture != nullptr)
+        {
+            texture->update(x, y, width, height, pixels.get());
+        }
+        else
+        {
+//        GLuint tex_id;
+//        glGenTextures(1, &tex_id);
+//        glBindTexture(GL_TEXTURE_2D, tex_id);
+//        glBindFramebuffer(GL_FRAMEBUFFER, target);
+//        glFramebufferTexture2D(GL_FRAMEBUFFER, GL_COLOR_ATTACHMENT0,
+//                               GL_TEXTURE_2D, tex_id, 0);
+//        glTexSubImage2D(GL_TEXTURE_2D, 0, x, y, w, h, GL_RGBA, GL_UNSIGNED_BYTE, pixels.get());
+//        glDeleteTextures(1, &tex_id);
+
+            auto tex = std::make_shared<gl::Texture>(width, height, pixels.get());
+            auto oldfg = fg;
+            fg = 0xffffffff;
+            blit(gl::TexRef{tex}, {0,0}, view_size);
+            fg = oldfg;
+        }
+        dirty = false;
+        pixels = nullptr;
+    }
 }
 } // namespace pix
```

### Comparing `pixpy-0.1.8/src/context.hpp` & `pixpy-0.1.9/src/context.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -10,24 +10,38 @@
 
 #include "vec2.hpp"
 
 namespace pix {
 
 class Context
 {
+    // The GL target frame buffer
     GLuint target = 0;
-    Vec2f offset{0, 0};
 
+    // The XY offset of our view into the framebuffer
+    Vec2f offset{0, 0};
+    // The size of our view into the framebuffer
+    Vec2f view_size{0, 0};
 public:
+    // Actual size of framebuffer
+    Vec2f target_size;
+
+    // Clip (scissor) area
     Vec2i clip_start{0,0};
     Vec2i clip_size{0,0};
 
-    Vec2f target_size;
+    std::shared_ptr<gl_wrap::Texture> texture;
+
+    // Viewport scale (for when window size != framebuffer size)
     float vpscale = 1.0F;
 
+    mutable bool dirty = false;
+
+    std::unique_ptr<uint32_t[]> pixels; // NOLINT
+
     float line_width = 1;
     float point_size = 2;
     gl_wrap::Color fg;
 
     std::vector<float> points;
 
 private:
@@ -65,20 +79,30 @@
 
     constexpr Vec2<float> to_screen(float x, float y) const
     {
         return to_screen(Vec2f{x, y});
     }
 
     Context(float w, float h, GLuint fb = 0);
-    Context(Vec2f const& offset, Vec2f const& size, GLuint fb = 0);
+    Context(Vec2f _offset, Vec2f _view_size, Vec2f _target_size, GLuint fb = 0);
 
-    Vec2f const& screen_size() { return target_size; }
+    Vec2f screen_size() const { return target_size; }
 
     void set_target() const;
 
+    void resize(Vec2f size, float scale)
+    {
+        target_size = size;
+        vpscale = scale;
+    }
+    void set_pixel(int x, int y, uint32_t col);
+
+    void flush_pixels();
+
+
     void set_color(gl_wrap::Color const& col);
 
     void circle(Vec2f const& v, float r);
     void filled_circle(Vec2f const& v, float r);
     void line(Vec2f from, Vec2f to);
     void line(Vec2f to);
     void filled_rect(Vec2f top_left, Vec2f size);
```

### Comparing `pixpy-0.1.8/src/eglutil.cpp` & `pixpy-0.1.9/src/eglutil.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/font.cpp` & `pixpy-0.1.9/src/font.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/font.hpp` & `pixpy-0.1.9/src/font.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/full_console.cpp` & `pixpy-0.1.9/src/full_console.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/full_console.hpp` & `pixpy-0.1.9/src/full_console.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/buffer.hpp` & `pixpy-0.1.9/src/gl/buffer.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/color.hpp` & `pixpy-0.1.9/src/gl/color.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/functions.hpp` & `pixpy-0.1.9/src/gl/functions.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/program.hpp` & `pixpy-0.1.9/src/gl/program.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/program_cache.hpp` & `pixpy-0.1.9/src/gl/program_cache.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/shader.hpp` & `pixpy-0.1.9/src/gl/shader.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/gl/texture.hpp` & `pixpy-0.1.9/src/gl/texture.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     void init()
     {
         // fmt::print("Created {}x{} = {}\n", width, height, (void*)this);
         glGenTextures(1, &tex_id);
         glBindTexture(GL_TEXTURE_2D, tex_id);
         glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);
-        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_LINEAR);
+        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);
         glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_CLAMP_TO_EDGE);
         glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_CLAMP_TO_EDGE);
     }
 
     template <typename T, size_t N>
     Texture(GLint w, GLint h, std::array<T, N> const& data,
             GLint target_format = GL_RGBA, GLint source_format = -1,
@@ -123,14 +123,15 @@
     }
 
     Texture(Texture const&) = delete;
     Texture(Texture&& other) noexcept { move_from(std::move(other)); }
 
     ~Texture()
     {
+
         if (tex_id != 0) { glDeleteTextures(1, &tex_id); }
         if (fb_id != 0) { glDeleteFramebuffers(1, &fb_id); }
     };
 
     Texture& operator=(Texture const&) = delete;
 
     Texture& operator=(Texture&& other) noexcept
@@ -143,95 +144,85 @@
     {
         glActiveTexture(GL_TEXTURE0 + unit);
         glBindTexture(GL_TEXTURE_2D, tex_id);
     }
 
     void set_target()
     {
-        if (fb_id == 0) {
-            // glActiveTexture(GL_TEXTURE0);
-            glBindTexture(GL_TEXTURE_2D, tex_id);
-            glGenFramebuffers(1, &fb_id);
-            glBindFramebuffer(GL_FRAMEBUFFER, fb_id);
-            glFramebufferTexture2D(GL_FRAMEBUFFER, GL_COLOR_ATTACHMENT0,
-                                   GL_TEXTURE_2D, tex_id, 0);
-        } else {
+        if(!alloc_framebuffer()) {
             glBindFramebuffer(GL_FRAMEBUFFER, fb_id);
         }
         setViewport({width, height});
     }
 
     GLuint get_target()
     {
+        alloc_framebuffer();
+        return fb_id;
+    }
+
+    bool alloc_framebuffer()
+    {
         if (fb_id == 0) {
-            // glActiveTexture(GL_TEXTURE0);
             glBindTexture(GL_TEXTURE_2D, tex_id);
             glGenFramebuffers(1, &fb_id);
             glBindFramebuffer(GL_FRAMEBUFFER, fb_id);
             glFramebufferTexture2D(GL_FRAMEBUFFER, GL_COLOR_ATTACHMENT0,
                                    GL_TEXTURE_2D, tex_id, 0);
+            gl_check("glFrameBufferTexture2d");
+            return true;
         }
-        return fb_id;
+        return false;
     }
 
     std::vector<std::byte> read_pixels(int x = 0, int y = 0, int w = -1,
                                        int h = -1)
     {
         if (w < 0) { w = width; }
         if (h < 0) { h = height; }
 
-        GLuint fb = 0;
-        if (fb_id == 0) {
-            glGenFramebuffers(1, &fb);
-            glBindFramebuffer(GL_FRAMEBUFFER, fb);
-            glFramebufferTexture2D(GL_FRAMEBUFFER, GL_COLOR_ATTACHMENT0,
-                                   GL_TEXTURE_2D, tex_id, 0);
-            gl_check("glFrameBufferTexture2d");
-            setViewport({width, height});
-        } else {
-            set_target();
-        }
+        set_target();
         std::vector<std::byte> data(width * height * 4);
         auto type = GL_UNSIGNED_BYTE;
         glReadPixels(x, height - y - h, w, h, format, type, data.data());
         gl_check("glReadPixels");
         glBindFramebuffer(GL_FRAMEBUFFER, 0);
         return data;
     }
 
     template <typename T>
     void update(T const* ptr, GLint source_format = -1,
-                GLenum type = GL_UNSIGNED_BYTE)
+                GLenum type = GL_UNSIGNED_BYTE) const
     {
         if (source_format < 0) {
             constexpr static std::array translate{0, GL_ALPHA, 0, GL_RGB,
                                                   GL_RGBA};
             source_format = translate[sizeof(T)];
         }
         glBindTexture(GL_TEXTURE_2D, tex_id);
         glTexSubImage2D(GL_TEXTURE_2D, 0, 0, 0, width, height, source_format,
                         type, ptr);
     }
 
     template <typename T>
     void update(int x, int y, int w, int h, T const* ptr,
-                GLint source_format = -1, GLenum type = GL_UNSIGNED_BYTE)
+                GLint source_format = -1, GLenum type = GL_UNSIGNED_BYTE) const
     {
         if (source_format < 0) {
             constexpr static std::array translate{0, GL_ALPHA, 0, GL_RGB,
                                                   GL_RGBA};
             source_format = translate[sizeof(T)];
         }
         glBindTexture(GL_TEXTURE_2D, tex_id);
         glTexSubImage2D(GL_TEXTURE_2D, 0, x, y, w, h, source_format, type, ptr);
     }
 
     std::pair<float, float> size() const
     {
-        return {(float)width, (float)height};
+        return {static_cast<float>(width), (float)height};
     }
 };
 
 struct TexRef
 {
     std::shared_ptr<void> data;
     std::shared_ptr<Texture> tex;
@@ -239,15 +230,15 @@
 private:
     std::array<float, 8> _uvs{0.F, 1.F, 1.F, 1.F, 1.F, 0.F, 0.F, 0.F};
 
 public:
     // Constructors
     TexRef() = default;
     TexRef(int w, int h) : tex{std::make_shared<Texture>(w, h)} {}
-    TexRef(std::pair<int, int> size)
+    explicit TexRef(std::pair<int, int> size)
         : tex{std::make_shared<Texture>(size.first, size.second)}
     {
     }
     explicit TexRef(std::shared_ptr<Texture> const& t) : tex(t) {}
     TexRef(std::shared_ptr<Texture> const& t, std::array<float, 8> const& u)
         : tex(t), _uvs(u)
     {
@@ -263,15 +254,15 @@
     };
 
     operator bool() const { return tex != nullptr; }
 
     void copy_from(gl_wrap::TexRef const& src) const
     {
         using gl_wrap::ProgramCache;
-        GLint fb;
+        GLint fb = 0;
         glGetIntegerv(GL_FRAMEBUFFER_BINDING, &fb);
         auto old = gl_wrap::getViewport();
         set_target();
         src.bind();
         float dx = 0;
         float dy = 0;
         // Transform UVs to clip space
@@ -309,18 +300,21 @@
 
     void set_target() const { tex->set_target(); }
 
     GLuint get_target() const { return tex->get_target(); }
 
     void copy_to(TexRef const& target) const { target.copy_from(*this); }
 
-    float ytou(double yy) { return static_cast<float>(1.0 - yy / tex->height); }
-    float xtov(double xx) { return static_cast<float>(xx / tex->width); }
+    float ytou(double yy) const
+    {
+        return static_cast<float>(1.0 - yy / tex->height);
+    }
+    float xtov(double xx) const { return static_cast<float>(xx / tex->width); }
 
-    TexRef crop(double x, double y, double w, double h)
+    TexRef crop(double x, double y, double w, double h) const
     {
         float u0 = xtov(this->x() + x);
         float v0 = ytou(this->y() + y);
         float u1 = u0 + static_cast<float>(w / tex->width);
         float v1 = v0 - static_cast<float>(h / tex->height);
         // printf("%f %f %f %f => %f %f %f %f\n", x, y, w, h, u0, v0, u1, v1);
         return {tex, std::array{u0, v0, u1, v0, u1, v1, u0, v1}};
```

### Comparing `pixpy-0.1.8/src/glad.h` & `pixpy-0.1.9/src/glad.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/glfw_system.cpp` & `pixpy-0.1.9/src/glfw_system.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -18,64 +18,107 @@
 #include <unordered_set>
 
 namespace fs = std::filesystem;
 
 using namespace std::chrono_literals;
 
 static bool swapped = false;
-
+
 class GLFWWindow : public Screen
 {
+    int frame_counter = 0;
+    int fps = 60;
+    using clk = std::chrono::steady_clock;
+    clk::time_point last_end{};
+    clk::time_point real_t{};
+    clk::time_point first{};
+    clk::duration frame_time = std::chrono::microseconds(1000000 / 60);
+    clk::duration delta = std::chrono::microseconds(1000000 / 60);
+
 public:
     GLFWwindow* window = nullptr;
 
-    explicit GLFWWindow(GLFWwindow* win) : window(win) { update_scale(); }
+    explicit GLFWWindow(GLFWwindow* win) : window(win)
+    {
+        update_scale();
+        first = clk::now();
+    }
 
     void update_scale()
     {
         int fw = 0;
         int fh = 0;
         glfwGetFramebufferSize(window, &fw, &fh);
         log("fb size %d %d\n", fw, fh);
 
         int w = 0;
         int h = 0;
         glfwGetWindowSize(window, &w, &h);
         log("win size %d %d\n", w, h);
-        scale = static_cast<float>(fw) / w;
+        scale = static_cast<float>(fw) / static_cast<float>(w);
     }
 
     ~GLFWWindow() override
     {
         if (window != nullptr) { glfwDestroyWindow(window); }
     }
 
     float scale = 1.0F;
     float get_scale() override
     {
         update_scale();
         return scale;
     }
 
-    using clk = std::chrono::steady_clock;
-    clk::time_point last{};
-    clk::duration frame_time = std::chrono::microseconds(1000000 / 60);
-
     void swap() override
     {
         glfwSwapBuffers(window);
         clk::time_point t = clk::now();
-        auto d = t - last;
+        auto d = t - real_t;
         swapped = true;
-        // printf("Frame time %.3f\n", d.count() / 1000000.0);
-        if (d + 1ms < frame_time) {
-            // printf("Sleeping %lld\n", (frame_time - d).count());
-            std::this_thread::sleep_for(frame_time - d - 1ms);
+        if (frame_time != 0us) {
+            if (d + 1ms < frame_time) {
+                //printf("Sleeping %dms\n", to_ms(frame_time - d)- 1);
+                std::this_thread::sleep_for(frame_time - d - 1ms);
+            }
+        }
+        t = clk::now();
+        //printf("Actually slept %dms\n", to_ms(t - real_t));
+        if (frame_counter > 0) {
+            delta = t - real_t;
         }
-        last = t;
+        real_t = t;
+        frame_counter++;
+    }
+    void set_fps(int fps) override
+    {
+        this->fps = fps;
+        if (fps == 0) {
+            frame_time = 0us;
+        } else {
+            frame_time = 1000000us / fps;
+        }
+    }
+
+    static inline constexpr int to_ms(clk::duration d)
+    {
+        return duration_cast<std::chrono::milliseconds>(d).count();
+    }
+
+    static inline constexpr double to_sec(clk::duration d)
+    {
+        return static_cast<double>(duration_cast<std::chrono::microseconds>(d)
+            .count()) /
+            1000'000.0;
+    }
+    Time get_time() const override
+    {
+        auto secs = to_sec(real_t - first);
+        auto f = to_sec(delta);
+        return {secs, frame_counter, f, fps};
     }
 
     void set_target() override
     {
         glBindFramebuffer(GL_FRAMEBUFFER, 0);
         auto [w, h] = get_size();
         glViewport(0, 0, w, h);
@@ -170,14 +213,16 @@
             return nullptr;
         }
         // printf("GL %d.%d\n", GLAD_VERSION_MAJOR(version),
         // GLAD_VERSION_MINOR(version));
 #endif
         glfwSwapInterval(1);
         // printf("%s\n", glGetString(GL_VERSION));
+        glDisable(GL_CULL_FACE);
+        glCullFace(GL_BACK);
         glEnable(GL_BLEND);
         glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA);
         glBindFramebuffer(GL_FRAMEBUFFER, 0);
 
         system = this;
         glfwSetCharCallback(window, [](GLFWwindow*, unsigned int codepoint) {
             system->char_was_pressed(codepoint);
@@ -233,17 +278,15 @@
         auto s = utf8::utf8_encode(
             std::u32string(1, static_cast<char32_t>(codepoint)));
         event_queue.emplace_back(TextEvent{s, 0});
     }
 
     std::optional<std::pair<int, int>> new_size;
 
-    void resized(int w, int h) { 
-        new_size = {w, h};
-    }
+    void resized(int w, int h) { new_size = {w, h}; }
 
     void key_was_pressed(int key, int /* scancode */, int action, int mods)
     {
         auto down = (action != GLFW_RELEASE);
         if (key >= 0x20 && key <= 0x7f) {
             auto c = static_cast<uint32_t>(std::tolower(key));
             if (down) {
```

### Comparing `pixpy-0.1.8/src/image.cpp` & `pixpy-0.1.9/src/image.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/image.hpp` & `pixpy-0.1.9/src/image.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/jpeg_decoder.h` & `pixpy-0.1.9/src/jpeg_decoder.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/keycodes.h` & `pixpy-0.1.9/src/keycodes.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/pi_system.cpp` & `pixpy-0.1.9/src/pi_system.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #include "keycodes.h"
-#include "player_linux.h"
 #include "system.hpp"
 
-#include <fmt/format.h>
-
 #include <EGL/egl.h>
 #include <GLES2/gl2.h>
 #include <bcm_host.h>
 #include <cctype>
+#include <chrono>
 #include <deque>
 #include <fcntl.h>
 #include <filesystem>
 #include <linux/input.h>
 #include <unordered_map>
 #include <vector>
 
+using namespace std::chrono_literals;
 namespace fs = std::filesystem;
 
+using std::chrono::duration_cast;
+
 class display_exception : public std::exception
 {
 public:
     explicit display_exception(const std::string& msg) : msg(msg) {}
     const char* what() const noexcept override { return msg.c_str(); }
 
 private:
@@ -38,28 +39,55 @@
 
 class PiScreen : public Screen
 {
     EGLDisplay eglDisplay;
     EGLSurface eglSurface;
     int width;
     int height;
+    int frame_counter = 0;
+    int fps = 60;
+    using clk = std::chrono::steady_clock;
+    clk::time_point real_t{};
+    clk::time_point first{};
+    clk::duration delta = std::chrono::microseconds(1000000 / 60);
 
 public:
     PiScreen(EGLDisplay d, EGLSurface s, int w, int h)
         : eglDisplay(d), eglSurface(s), width(w), height(h)
     {
     }
+
+    static inline constexpr double to_sec(clk::duration d)
+    {
+        return static_cast<double>(duration_cast<std::chrono::microseconds>(d)
+            .count()) /
+            1000'000.0;
+    }
+
+    Time get_time() const override
+    {
+        auto secs = to_sec(real_t - first);
+        auto f = to_sec(delta);
+        return {secs, frame_counter, f, fps};
+    }
+
     void swap() override
     {
         if (eglDisplay != EGL_NO_DISPLAY) {
             eglSwapBuffers(eglDisplay, eglSurface);
             // eglQuerySurface(eglDisplay, eglSurface, EGL_WIDTH, &screenWidth);
             // eglQuerySurface(eglDisplay, eglSurface, EGL_HEIGHT,
             // &screenHeight);
         }
+        auto t = clk::now();
+        if (frame_counter > 0) {
+            delta = t - real_t;
+        }
+        real_t = t;
+        frame_counter++;
     }
     std::pair<int, int> get_size() const override { return {width, height}; }
 };
 
 class PiSystem : public System
 {
     EGL_DISPMANX_WINDOW_T nativewindow{};
@@ -67,21 +95,19 @@
     EGLConfig eglConfig{};
     EGLContext eglContext{};
     EGLDisplay eglDisplay{};
     EGLSurface eglSurface{};
 
     std::vector<int> fdv;
 
-    std::unique_ptr<LinuxPlayer> player;
-
     int32_t display_width{};
     int32_t display_height{};
 
 public:
-    std::shared_ptr<Screen> init_screen(Settings const&) override
+    std::shared_ptr<Screen> init_screen(Screen::Settings const&) override
     {
         bcm_host_init();
 
         DISPMANX_ELEMENT_HANDLE_T dispman_element = 0;
         DISPMANX_DISPLAY_HANDLE_T dispman_display = 0;
         DISPMANX_UPDATE_HANDLE_T dispman_update = 0;
         VC_RECT_T dst_rect;
@@ -131,14 +157,16 @@
         nativewindow.width = display_width;
         nativewindow.height = display_height;
         vc_dispmanx_update_submit_sync(dispman_update);
 
         initEGL(eglConfig, eglContext, eglDisplay, eglSurface, &nativewindow);
         return std::make_shared<PiScreen>(eglDisplay, eglSurface, display_width,
                                           display_height);
+
+        glColorMask(true, true, true, false);
     }
 
     std::vector<int> letters = {
         KEY_A, KEY_B, KEY_C, KEY_D, KEY_E, KEY_F, KEY_G, KEY_H, KEY_I,
         KEY_J, KEY_K, KEY_L, KEY_M, KEY_N, KEY_O, KEY_P, KEY_Q, KEY_R,
         KEY_S, KEY_T, KEY_U, KEY_V, KEY_W, KEY_X, KEY_Y, KEY_Z,
     };
@@ -284,21 +312,21 @@
                                 mods = 0;
                                 if (k == KEY_ESC && shift_down) {
                                     putEvent(QuitEvent{});
                                 } else {
                                     if (shift_down) mods |= 1;
                                     auto it = mappings.find(k | (mods << 24));
                                     if (it != mappings.end()) {
-                                        fmt::print("Converted to {:x} > {:x}\n",
-                                                   k, it->second);
+                                        //fmt::print("Converted to {:x} > {:x}\n",
+                                        //           k, it->second);
                                         k = it->second;
                                         putEvent(KeyEvent{k, mods, 0});
                                     } else {
-                                        fmt::print("Unhandled key {:x}\n",
-                                                   ptr->code);
+                                        //fmt::print("Unhandled key {:x}\n",
+                                        //           ptr->code);
                                     }
                                 }
                             }
                         } else if (ptr->type != 0) {
                             // fmt::print("TYPE {} CODE {} VALUE {}\n",
                             // ptr->type, ptr->code, ptr->value);
                         }
@@ -306,33 +334,13 @@
                         rc -= sizeof(struct input_event);
                     }
                 }
             }
         }
         return events;
     }
-
-    void init_audio(Settings const&) override
-    {
-        return;
-        player = std::make_unique<LinuxPlayer>(44100);
-    }
-
-    void
-    set_audio_callback(std::function<void(float*, size_t)> const& fcb) override
-    {
-        return;
-        player->play([fcb](int16_t* data, size_t sz) {
-            std::array<float, 32768> fa; // NOLINT
-            fcb(fa.data(), sz);
-            for (size_t i = 0; i < sz; i++) {
-                auto f = std::clamp(fa[i], -1.0F, 1.0F);
-                data[i] = static_cast<int16_t>(f * 32767.0);
-            }
-        });
-    }
 };
 
 std::unique_ptr<System> create_pi_system()
 {
     return std::make_unique<PiSystem>();
 }
```

### Comparing `pixpy-0.1.8/src/pixel_console.cpp` & `pixpy-0.1.9/src/pixel_console.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     : font_ptr{std::make_shared<TileSet>(ftfont)}, font{*font_ptr}, cols(w),
       rows(h)
 
 {
     init();
 }
 */
-PixConsole::PixConsole(int w, int h, std::shared_ptr<TileSet> const& _font)
-    : font{_font},  cols{w}, rows{h}
+PixConsole::PixConsole(int _cols, int _rows, std::shared_ptr<TileSet> const& _tile_set)
+    : tile_set{_tile_set},  cols{_cols}, rows{_rows}
 {
     init();
 }
 
 void PixConsole::init()
 {
     uvdata.resize(cols * rows);
@@ -80,23 +80,23 @@
                           gl::FragmentShader{fragment_shader});
 
     program.setUniform("in_tex", 0);
     program.setUniform("uv_tex", 1);
     program.setUniform("col_tex", 2);
 
     program.setUniform("console_size", std::pair<float, float>(cols, rows));
-    program.setUniform("uv_scale", font->get_uvscale());
+    program.setUniform("uv_scale", tile_set->get_uvscale());
 
     uv_texture.update(uvdata.data());
     col_texture.update(coldata.data());
 }
 
 template <typename T> std::pair<T, T> PixConsole::get_char_size() const
 {
-    return {static_cast<T>(font->char_width), static_cast<T>(font->char_height)};
+    return {static_cast<T>(tile_set->char_width), static_cast<T>(tile_set->char_height)};
 }
 
 template std::pair<float, float> PixConsole::get_char_size() const;
 template std::pair<int, int> PixConsole::get_char_size() const;
 
 
 std::pair<int, int> PixConsole::text(int x, int y, std::string const& t,
@@ -120,15 +120,15 @@
     for (auto c : text32) {
         if (c == 10) {
             x = 0;
             y++;
             continue;
         }
 
-        uvdata[x + cols * y] = font->get_offset(c) | w0;
+        uvdata[x + cols * y] = tile_set->get_offset(c) | w0;
         coldata[x + cols * y] = w1;
         x++;
         if (x >= cols) {
             x = 0;
             y++;
         }
     }
@@ -136,50 +136,50 @@
     return {x, y};
 }
 
 void PixConsole::put_char(int x, int y, char32_t c)
 {
     uv_dirty = col_dirty = true;
     auto& u = uvdata[x + cols * y];
-    u = (u & 0xffff0000) | font->get_offset(c);
+    u = (u & 0xffff0000) | tile_set->get_offset(c);
 }
 
 void PixConsole::put(int x, int y, uint32_t fg, uint32_t bg, char32_t c)
 {
     uv_dirty = col_dirty = true;
     auto [w0, w1] = make_col(fg, bg);
-    uvdata[x + cols * y] = font->get_offset(c) | w0;
+    uvdata[x + cols * y] = tile_set->get_offset(c) | w0;
     coldata[x + cols * y] = w1;
 }
 
 uint32_t PixConsole::get_char(int x, int y)
 {
     uint32_t uv = uvdata[x + cols * y] & 0xffff;
-    return font->get_char_from_uv(uv);
+    return tile_set->get_char_from_uv(uv);
 }
 
 std::vector<uint32_t> PixConsole::get_tiles()
 {
     std::vector<uint32_t> result(cols*rows*3);
     for(int i=0; i<cols*rows; i++) {
         uint32_t uv = uvdata[i] & 0xffff;
         auto fg = ((coldata[i] & 0xff000000)>>16) | (uvdata[i] & 0xffff0000);
         auto bg = coldata[i] & 0xffffff;
-        result[i*3] = font->get_char_from_uv(uv);
+        result[i*3] = tile_set->get_char_from_uv(uv);
         result[i*3+1] = fg;
         result[i*3+2] = bg;
     }
     return result;
 }
 
 void PixConsole::set_tiles(std::vector<uint32_t> const& data)
 {
     for(int i=0; i<cols*rows; i++) {
         auto [w0,w1] = make_col(data[i*3+1], data[i*3+2]);
-        uvdata[i] = font->get_offset(data[i*3]) | w0;
+        uvdata[i] = tile_set->get_offset(data[i*3]) | w0;
         coldata[i] = w1;
     }
     uv_dirty = true;
     col_dirty = true;
 }
 
 void PixConsole::put_color(int x, int y, uint32_t fg, uint32_t bg)
@@ -190,15 +190,15 @@
     coldata[x + cols * y] = w1;
 }
 
 void PixConsole::fill(uint32_t fg, uint32_t bg)
 {
     uv_dirty = col_dirty = true;
     auto [w0, w1] = make_col(fg, bg);
-    w0 |= font->char_uvs[' '];
+    w0 |= tile_set->char_uvs[' '];
     for (size_t i = 0; i < uvdata.size(); i++) {
         uvdata[i] = w0;
         coldata[i] = w1;
     }
 }
 
 void PixConsole::fill(uint32_t bg)
@@ -213,15 +213,15 @@
 void PixConsole::clear_area(int32_t x, int32_t y, int32_t w, int32_t h,
                             uint32_t fg, uint32_t bg)
 {
     uv_dirty = col_dirty = true;
     if (w == -1) { w = cols; }
     if (h == -1) { h = rows; }
     auto [w0, w1] = make_col(fg, bg);
-    w0 |= font->char_uvs[' '];
+    w0 |= tile_set->char_uvs[' '];
     for (int32_t yy = 0; yy < h; yy++) {
         for (int32_t xx = 0; xx < w; xx++) {
             auto offs = (xx + x) + (yy + y) * cols;
             uvdata[offs] = w0;
             coldata[offs] = w1;
         }
     }
@@ -251,15 +251,15 @@
 {
     if (uv_dirty) { uv_texture.update(uvdata.data()); }
     if (col_dirty) { col_texture.update(coldata.data()); }
     uv_dirty = col_dirty = false;
     glDisable(GL_BLEND);
     col_texture.bind(2);
     uv_texture.bind(1);
-    font->tile_texture->bind(0);
+    tile_set->tile_texture->bind(0);
 
     program.use();
 
     std::array vertexData{x0,  y0,  x1,  y0,  x1,  y1,  x0,  y1,
                           0.F, 0.F, 1.F, 0.F, 1.F, 1.F, 0.F, 1.F};
     gl::ArrayBuffer<GL_STREAM_DRAW> vbo{vertexData};
 
@@ -275,9 +275,9 @@
     uv.disable();
 
     glEnable(GL_BLEND);
 }
 
 std::pair<int, int> PixConsole::get_pixel_size() const
 {
-    return {cols * font->char_width, rows * font->char_height};
+    return {cols * tile_set->char_width, rows * tile_set->char_height};
 }
```

### Comparing `pixpy-0.1.8/src/pixel_console.hpp` & `pixpy-0.1.9/src/pixel_console.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class PixConsole
 {
     static std::string vertex_shader;
     static std::string fragment_shader;
 
     gl_wrap::Program program;
 
-    std::shared_ptr<TileSet> font;
+    std::shared_ptr<TileSet> tile_set;
 
     int cols;
     int rows;
 
     gl_wrap::Texture uv_texture;
     gl_wrap::Texture col_texture;
 
@@ -41,31 +41,31 @@
             fg & 0xffff0000, ((bg & 0xff) << 16) | (bg & 0xff00) | (bg >> 16) |
                                  ((fg << 16) & 0xff000000)};
     }
 
     void init();
 
 public:
-    PixConsole(int cols, int rows, std::shared_ptr<TileSet> const& font);
+    PixConsole(int _cols, int _rows, std::shared_ptr<TileSet> const& _tile_set);
 
     std::vector<uint32_t> get_tiles();
     void set_tiles(std::vector<uint32_t> const& data);
 
     std::pair<int, int> get_size() const { return {cols, rows}; }
     template <typename T = int> std::pair<T, T> get_char_size() const;
     std::pair<int, int> get_pixel_size() const;
 
     std::shared_ptr<gl_wrap::Texture> get_font_texture() const
     {
-        return font->tile_texture;
+        return tile_set->tile_texture;
     }
 
     gl_wrap::TexRef get_texture_for_char(char32_t c)
     {
-        return font->get_texture_for_char(c);
+        return tile_set->get_texture_for_char(c);
     }
 
     std::pair<int, int> text(int x, int y, std::string const& t,
                              uint32_t fg = 0xffffffff, uint32_t bg = 0);
     std::pair<int, int> text(int x, int y, std::u32string const& t,
                              uint32_t fg = 0xffffffff, uint32_t bg = 0);
     std::pair<int, int> text(std::pair<int, int> pos,
```

### Comparing `pixpy-0.1.8/src/python/class_console.hpp` & `pixpy-0.1.9/src/python/class_console.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     auto fcon = std::make_shared<FullConsole>(con, Machine::get_instance().sys);
 
     return fcon;
 }
 
 inline void add_console_class(py::module_ const& mod)
 {
+    using namespace pybind11::literals;
     // Console
     py::class_<FullConsole, std::shared_ptr<FullConsole>>(mod, "Console")
         .def(py::init<>(&make_console), "cols"_a = 80, "rows"_a = 50,
              "font_file"_a = "", "tile_size"_a = Vec2i{0, 0},
              "font_size"_a = 16,
              "Create a new Console holding cols*row tiles. Optionally set a "
              "backing font. If `tile_size` is not provided it will be derived "
```

### Comparing `pixpy-0.1.8/src/python/class_context.hpp` & `pixpy-0.1.9/src/python/class_context.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 #include <optional>
 #include <pybind11/detail/common.h>
 #include <pybind11/pybind11.h>
 
 #include <string>
 #include <tuple>
 
-using namespace pybind11::literals;
-
 namespace py = pybind11;
 namespace gl = gl_wrap;
 
 inline std::shared_ptr<pix::Context> make_context(Vec2f size)
 {
     if (size.x == 0 && size.y == 0) {
         size = Vec2f{Machine::get_instance().screen->get_size()};
@@ -30,35 +28,39 @@
 {
     if (tr.data != nullptr) {
         return static_cast<pix::Context*>(tr.data.get());
     }
 
     auto* context = new pix::Context(
         {static_cast<float>(tr.x()), static_cast<float>(tr.y())},
+        {static_cast<float>(tr.width()), static_cast<float>(tr.height())},
         {static_cast<float>(tr.tex->width), static_cast<float>(tr.tex->height)},
         tr.get_target());
     tr.data = std::shared_ptr<void>(static_cast<void*>(context), [](void* ptr) {
         delete static_cast<pix::Context*>(ptr);
     });
+    context->texture = tr.tex;
     return context;
 }
 
-inline pix::Context* context_from(Screen& screen)
+inline pix::Context* context_from(Screen& /*screen*/)
 {
     return Machine::get_instance().context.get();
 }
 
 inline pix::Context* context_from(pix::Context& context)
 {
     return &context;
 }
 
 template <typename T, typename... O>
 inline void add_draw_functions(pybind11::class_<T, O...>& cls)
 {
+    using namespace pybind11::literals;
+
     cls.def(
         "circle",
         [](T& self, Vec2f const& center, float r) {
             context_from(self)->circle(center, r);
         },
         "center"_a, "radius"_a, "Draw an (outline) circle");
 
@@ -80,15 +82,15 @@
         "line", [](T& self, Vec2f const& to) { context_from(self)->line(to); },
         "end"_a,
         "Draw a line from the end of the last line to the given position.");
 
     cls.def(
         "polygon",
         [](T& self, std::vector<Vec2f> const& points) {
-          context_from(self)->draw_polygon(points.data(), points.size());
+            context_from(self)->draw_polygon(points.data(), points.size());
         },
         "points"_a, "Draw a convex polygon.");
     cls.def(
         "plot",
         [](T& self, Vec2f const& to, uint32_t color) {
             context_from(self)->plot(to, gl_wrap::Color(color));
         },
@@ -136,27 +138,27 @@
             } else if (xy) {
                 ctx->blit(tr, *xy, size);
             } else {
                 ctx->blit(tr, {0, 0}, size);
             }
         },
         "image"_a, "top_left"_a = std::nullopt, "center"_a = std::nullopt,
-        "size"_a = Vec2f{-1, -1}, "rot"_a = 0,
+        "size"_a = Vec2f{0, 0}, "rot"_a = 0,
         "Render an image. The image can either be aligned to its top left "
         "corner, or centered, in which case it can also be rotated.");
     cls.def(
         "draw",
         [](T& self, FullConsole& con, Vec2f const& xy, Vec2f const& size) {
             con.render(context_from(self), xy, size);
         },
-        "drawable"_a, "top_left"_a = Vec2f{0, 0}, "size"_a = Vec2f{-1, -1});
+        "drawable"_a, "top_left"_a = Vec2f{0, 0}, "size"_a = Vec2f{0, 0});
     cls.def(
         "clear",
         [](T& self, uint32_t color) { context_from(self)->clear(color); },
-        "color"_a = color::transp, "Clear the context using given color.");
+        "color"_a = color::black, "Clear the context using given color.");
     cls.def_property(
         "draw_color", [](T& self) { return context_from(self)->fg.to_rgba(); },
         [](T& self, uint32_t color) { context_from(self)->set_color(color); },
         "Set the draw color.");
     cls.def_property(
         "point_size", [](T& self) { return context_from(self)->point_size; },
         [](T& self, float lw) { context_from(self)->point_size = lw; },
@@ -171,14 +173,27 @@
         "clip_top_left", [](T& self) { return context_from(self)->clip_start; },
         [](T& self, Vec2i xy) { context_from(self)->clip_start = xy; });
     cls.def_property(
         "clip_size", [](T& self) { return context_from(self)->clip_size; },
         [](T& self, Vec2i xy) { context_from(self)->clip_size = xy; });
     cls.def_property_readonly(
         "size", [](T& self) { return context_from(self)->target_size; });
+    cls.def_property_readonly(
+        "target_size", [](T& self) { return context_from(self)->target_size; });
+    cls.def(
+        "set_pixel",
+        [](T& self, Vec2i pos, uint32_t color) {
+            context_from(self)->set_pixel(pos.x, pos.y, color);
+        },
+        "pos"_a, "color"_a, "Write a pixel into the image.");
+    cls.def(
+        "flush", [](T& self) { context_from(self)->flush(); },
+        "Flush pixel operations");
 }
 inline auto add_context_class(py::module_ const& mod)
 {
+    using namespace pybind11::literals;
+
     return py::class_<pix::Context, std::shared_ptr<pix::Context>>(mod,
                                                                    "Context")
         .def(py::init<>(&make_context), "size"_a = Vec2f{0, 0});
 }
```

### Comparing `pixpy-0.1.8/src/python/class_font.hpp` & `pixpy-0.1.9/src/python/class_font.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/python/class_image.hpp` & `pixpy-0.1.9/src/python/class_image.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #include <pybind11/detail/common.h>
 #include <pybind11/pybind11.h>
 
 #include <memory>
 #include <string>
 #include <tuple>
 
-using namespace pybind11::literals;
-
 namespace py = pybind11;
 namespace gl = gl_wrap;
 
 inline std::vector<gl::TexRef> split_wh(gl::TexRef img, int cols, int rows,
                                         int w, int h)
 {
     if (cols < 0) { cols = static_cast<int>(img.width() / w); }
@@ -31,15 +29,16 @@
     return img.split(static_cast<int>(cols), static_cast<int>(rows));
 }
 
 inline gl::TexRef image_from_vec2(Vec2f const& v)
 {
     return {static_cast<int>(v.x), static_cast<int>(v.y)};
 }
-inline gl::TexRef image_from_pixels(int width, std::vector<uint32_t> pixels)
+inline gl::TexRef image_from_pixels(int width,
+                                    std::vector<uint32_t> const& pixels)
 {
     auto tex = std::make_shared<gl::Texture>(
         width, static_cast<int>(pixels.size()) / width, pixels);
     return gl::TexRef{tex};
 }
 
 inline gl::TexRef crop(gl::TexRef img, std::optional<Vec2f> xy_,
@@ -49,14 +48,15 @@
     auto d = Vec2f{img.width(), img.height()} - xy;
     auto size = size_.value_or(d);
     return img.crop(xy.x, xy.y, size.x, size.y);
 }
 
 inline auto add_image_class(py::module_ const& mod)
 {
+    using namespace pybind11::literals;
 
     // Image
     return py::class_<gl_wrap::TexRef>(mod, "Image")
         .def(py::init<int32_t, int32_t>(), "width"_a, "height"_a,
              "Create an empty image of the given size.")
         .def(py::init<>(&image_from_vec2), "size"_a,
              "Create an empty image of the given size.")
```

### Comparing `pixpy-0.1.8/src/python/class_tileset.hpp` & `pixpy-0.1.9/src/python/class_tileset.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 
 #include <filesystem>
 #include <memory>
 #include <string>
 #include <tuple>
 
 namespace py = pybind11;
-using namespace pybind11::literals;
-namespace fs = std::filesystem;
 
 inline std::shared_ptr<TileSet> make_tileset(std::string const& font_file,
                                              int size)
 {
     return std::make_shared<TileSet>(font_file, size);
 }
 
 inline std::shared_ptr<TileSet> make_tileset2(Vec2f size)
 {
     return std::make_shared<TileSet>(std::pair{size.x, size.y});
 }
 inline void add_tileset_class(py::module_ const& mod)
 {
+    using namespace pybind11::literals;
     py::class_<TileSet, std::shared_ptr<TileSet>>(mod, "TileSet")
         .def(py::init<>(&make_tileset), "font_file"_a, "size"_a,
              "Create a TileSet from a ttf font with the given size. The tile "
              "size will be derived from the font size.")
         .def(py::init<>(&make_tileset2), "tile_size"_a,
              "Create a tileset with the given tile size.")
         .def("get_image_for", &TileSet::get_texture_for_char,
```

### Comparing `pixpy-0.1.8/src/python/class_vec2.hpp` & `pixpy-0.1.9/src/python/class_vec2.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/python/mod_color.hpp` & `pixpy-0.1.9/src/python/mod_color.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/python/mod_event.hpp` & `pixpy-0.1.9/src/python/mod_event.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/python/mod_key.hpp` & `pixpy-0.1.9/src/python/mod_key.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/python.cpp` & `pixpy-0.1.9/src/python.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
 
     m.context = std::make_shared<pix::Context>(realw, realh, 0);
     m.context->vpscale = m.screen->get_scale();
 
     m.sys->add_listener([](AnyEvent const& e) {
         if (std::holds_alternative<ResizeEvent>(e)) {
             auto [w, h] = m.screen->get_size();
-            m.context->target_size = Vec2f(w, h);
-            m.context->vpscale = m.screen->get_scale();
+            m.context->resize(Vec2f(w,h), m.screen->get_scale());
         }
         return System::Propagate::Pass;
     });
 
     m.sys->init_input();
     return m.screen;
 }
```

### Comparing `pixpy-0.1.8/src/system.hpp` & `pixpy-0.1.9/src/system.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -98,16 +98,26 @@
     {
         ScreenType screen = ScreenType::Window;
         std::string title = "pix";
         int display_width = 1600;
         int display_height = 1200;
     };
 
+    struct Time
+    {
+        double seconds{};
+        int frame_counter{};
+        double delta{};
+        int fps{};
+    };
+
     virtual ~Screen() = default;
     virtual void swap() {}
+    virtual void set_fps(int fps) {}
+    virtual Time get_time() const { return {}; }
     virtual void set_target(){};
     virtual float get_scale() { return 1.0F; }
     virtual std::pair<int, int> get_size() const { return {-1, -1}; }
 };
 
 class Input
 {};
```

### Comparing `pixpy-0.1.8/src/tile_set.cpp` & `pixpy-0.1.9/src/tile_set.cpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/tile_set.hpp` & `pixpy-0.1.9/src/tile_set.hpp`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/unscii-16.h` & `pixpy-0.1.9/src/unscii-16.h`

 * *Files identical despite different names*

### Comparing `pixpy-0.1.8/src/utf8.h` & `pixpy-0.1.9/src/utf8.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 #pragma once
 
+#include <array>
 #include <cstdint>
 #include <string>
 #include <string_view>
 #include <vector>
 
 // Copyright (c) 2008-2009 Bjoern Hoehrmann <bjoern@hoehrmann.de>
 // See http://bjoern.hoehrmann.de/utf-8/decoder/dfa/ for details.
 
-//#define UTF8_ACCEPT 0
-//#define UTF8_REJECT 1
-
 namespace utf8 {
 
 inline uint32_t decode(uint32_t* state, uint32_t* codep, char byte)
 {
-    static const uint8_t utf8d[] = {
+    static constexpr std::array<uint8_t, 400> utf8d = {
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0, // 00..1f
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0, // 20..3f
         0,   0,   0,   0,   0,   0,   0,   0,   0,   0,   0,
@@ -53,103 +51,90 @@
         1,   1,   1,   1,   1,   1,   1,   1,   1,   1,   1,
         1,   3,   1,   3,   1,   1,   1,   1,   1,   1, // s5..s6
         1,   3,   1,   1,   1,   1,   1,   3,   1,   3,   1,
         1,   1,   1,   1,   1,   1,   3,   1,   1,   1,   1,
         1,   1,   1,   1,   1,   1,   1,   1,   1,   1, // s7..s8
     };
 
-    uint32_t type = utf8d[(unsigned char)byte];
+    uint32_t type = utf8d[static_cast<unsigned char>(byte)];
 
-    *codep = (*state != 0) ? (byte & 0x3fu) | (*codep << 6)
-                                     : (0xff >> type) & (byte);
+    *codep = (*state != 0) ? (byte & 0x3fU) | (*codep << 6)
+                           : (0xff >> type) & (byte);
 
     *state = utf8d[256 + *state * 16 + type];
     return *state;
 }
 
 inline size_t utf8_decode(const std::string& utf8, uint32_t* target)
 {
-    uint32_t codepoint;
+    uint32_t codepoint = 0;
     uint32_t state = 0;
     auto* ptr = target;
 
     for (auto s : utf8) {
-        if (!decode(&state, &codepoint, s)) {
-            if (codepoint <= 0xffff)
-                *ptr++ = codepoint;
+        if (decode(&state, &codepoint, s) == 0U) {
+            if (codepoint <= 0xffff) { *ptr++ = codepoint; }
         }
     }
     return ptr - target;
 }
 
 inline std::u32string utf8_decode(std::string_view txt)
 {
     std::u32string result;
     using C = std::u32string::value_type;
 
-    uint32_t codepoint;
+    uint32_t codepoint = 0;
     uint32_t state = 0;
 
     for (auto s : txt) {
-        if (!decode(&state, &codepoint, s)) {
-                result.push_back((C)codepoint);
+        if (decode(&state, &codepoint, s) == 0U) {
+            result.push_back(static_cast<C>(codepoint));
         }
     }
     return result;
 }
 
-/* inline std::string utf8_encode(std::string_view txt) */
-/* { */
-/*     std::string out; */
-/*     const uint8_t* s = (uint8_t*)txt.data(); */
-/*     for (size_t i = 0; i < txt.length(); i++) { */
-/*         uint8_t c = s[i]; */
-/*         if (c <= 0x7f) */
-/*             out.push_back(c); */
-/*         else { */
-/*             out.push_back(0xC0 | (c >> 6)); */
-/*             out.push_back(0x80 | (c & 0x3F)); */
-/*         } */
-/*     } */
-/*     return out; */
-/* } */
-
 inline std::string utf8_encode(const std::vector<char32_t>& s)
 {
     std::string out;
+    const auto push = [&](char32_t c) constexpr {
+        out.push_back(static_cast<char>(c));
+    };
+
     for (auto c : s) {
-        if (c < 0x80)
-            out.push_back(c & 0xff);
-        else if (c < 0x800) {
-            out.push_back(0xC0 | ((c >> 6) & 0x1f));
-            out.push_back(0x80 | (c & 0x3f));
+        if (c < 0x80) {
+            push(c & 0xff);
+        } else if (c < 0x800) {
+            push(0xC0 | ((c >> 6) & 0x1f));
+            push(0x80 | (c & 0x3f));
         } else if (c < 0x10000) {
-            out.push_back(0xE0 | ((c >> 12) & 0xf));
-            out.push_back(0x80 | ((c >> 6) & 0x3f));
-            out.push_back(0x80 | (c & 0x3f));
+            push(0xE0 | ((c >> 12) & 0xf));
+            push(0x80 | ((c >> 6) & 0x3f));
+            push(0x80 | (c & 0x3f));
         } else {
-            out.push_back(0xF0 | ((c >> 18) & 0x07));
-            out.push_back(0x80 | ((c >> 12) & 0x3f));
-            out.push_back(0x80 | ((c >> 6) & 0x3f));
-            out.push_back(0x80 | (c & 0x3f));
+            push(0xF0 | ((c >> 18) & 0x07));
+            push(0x80 | ((c >> 12) & 0x3f));
+            push(0x80 | ((c >> 6) & 0x3f));
+            push(0x80 | (c & 0x3f));
         }
     }
     return out;
 }
 
 inline std::string utf8_encode(const std::u32string& s)
 {
     std::string out;
     const auto push = [&](char32_t c) constexpr {
         out.push_back(static_cast<char>(c));
     };
     for (auto c : s) {
-        if (c < 0x80)
+        if (c < 0x80) {
             push(c & 0xff);
-        else if (c < 0x800) {
+        } else if (c < 0x800) {
             push(0xC0 | ((c >> 6) & 0x1f));
             push(0x80 | (c & 0x3f));
         } else if (c < 0x10000) {
             push(0xE0 | ((c >> 12) & 0xf));
             push(0x80 | ((c >> 6) & 0x3f));
             push(0x80 | (c & 0x3f));
         } else {
@@ -157,8 +142,8 @@
             push(0x80 | ((c >> 12) & 0x3f));
             push(0x80 | ((c >> 6) & 0x3f));
             push(0x80 | (c & 0x3f));
         }
     }
     return out;
 }
-} // namespace utils
+} // namespace utf8
```

### Comparing `pixpy-0.1.8/src/vec2.hpp` & `pixpy-0.1.9/src/vec2.hpp`

 * *Files identical despite different names*

