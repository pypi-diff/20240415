# Comparing `tmp/pyvispr-2024.2.tar.gz` & `tmp/pyvispr-2024.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2024.2.tar", last modified: Thu Apr 11 14:04:11 2024, max compression
+gzip compressed data, was "pyvispr-2024.3.tar", last modified: Mon Apr 15 11:19:49 2024, max compression
```

## Comparing `pyvispr-2024.2.tar` & `pyvispr-2024.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.2/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-11 14:04:11.646021 pyvispr-2024.2/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.2/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.2/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.2/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.639354 pyvispr-2024.2/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.2/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.2/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/
--rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.2/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/catalog/factory/
--rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.2/pyvispr/catalog/factory/image_loader.py
--rwx------   0 eric      (1000) users      (984)    12213 2024-04-11 08:05:54.000000 pyvispr-2024.2/pyvispr/catalog/factory/image_viewer.py
--rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.2/pyvispr/catalog/factory/numexpr_calculator.py
--rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.2/pyvispr/catalog/factory/value.py
--rwx------   0 eric      (1000) users      (984)     2506 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/catalog/factory/value_viewer.py
--rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.2/pyvispr/catalog/installer.py
--rwx------   0 eric      (1000) users      (984)     4114 2024-04-11 12:31:33.000000 pyvispr-2024.2/pyvispr/catalog/parser.py
--rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.2/pyvispr/catalog/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/config/appearance/
--rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.2/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.2/pyvispr/config/appearance/behavior.py
--rwx------   0 eric      (1000) users      (984)     2586 2024-01-19 18:43:09.000000 pyvispr-2024.2/pyvispr/config/appearance/color.py
--rwx------   0 eric      (1000) users      (984)     1711 2023-12-13 13:08:28.000000 pyvispr-2024.2/pyvispr/config/appearance/geometry.py
--rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/config/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.2/pyvispr/constant/app.py
--rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.2/pyvispr/constant/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.2/pyvispr/constant/function.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.2/pyvispr/constant/path.py
--rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.2/pyvispr/constant/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/constant/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/constant/widget/function_header.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.2/pyvispr/constant/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.2/pyvispr/constant/widget/node.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/extension/
--rwx------   0 eric      (1000) users      (984)    11820 2024-04-11 13:59:35.000000 pyvispr-2024.2/pyvispr/extension/function.py
--rwx------   0 eric      (1000) users      (984)     2907 2024-04-11 10:11:11.000000 pyvispr-2024.2/pyvispr/extension/module.py
--rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.2/pyvispr/extension/qt6.py
--rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.2/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.642687 pyvispr-2024.2/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/flow/descriptive/
--rwx------   0 eric      (1000) users      (984)     7851 2024-04-11 14:03:03.000000 pyvispr-2024.2/pyvispr/flow/descriptive/node.py
--rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.2/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/flow/functional/
--rwx------   0 eric      (1000) users      (984)     6827 2024-04-11 08:16:26.000000 pyvispr-2024.2/pyvispr/flow/functional/graph.py
--rwx------   0 eric      (1000) users      (984)     4509 2023-12-12 21:43:02.000000 pyvispr-2024.2/pyvispr/flow/functional/link.py
--rwx------   0 eric      (1000) users      (984)    10835 2024-04-11 08:05:14.000000 pyvispr-2024.2/pyvispr/flow/functional/node_isolated.py
--rwx------   0 eric      (1000) users      (984)     3546 2024-04-11 08:19:29.000000 pyvispr-2024.2/pyvispr/flow/functional/node_linked.py
--rwx------   0 eric      (1000) users      (984)     2549 2024-04-10 14:37:49.000000 pyvispr-2024.2/pyvispr/flow/functional/socket.py
--rwx------   0 eric      (1000) users      (984)     2169 2024-04-10 16:31:30.000000 pyvispr-2024.2/pyvispr/flow/messenger.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/flow/visual/
--rwx------   0 eric      (1000) users      (984)    18732 2024-04-11 08:03:57.000000 pyvispr-2024.2/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.2/pyvispr/flow/visual/ii_value.py
--rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.2/pyvispr/flow/visual/link.py
--rwx------   0 eric      (1000) users      (984)    12954 2024-04-11 12:24:51.000000 pyvispr-2024.2/pyvispr/flow/visual/node.py
--rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/flow/visual/socket.py
--rwx------   0 eric      (1000) users      (984)     7968 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/flow/visual/whiteboard.py
--rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.639354 pyvispr-2024.2/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/interface/storage/
--rwx------   0 eric      (1000) users      (984)     2993 2024-04-10 14:07:15.000000 pyvispr-2024.2/pyvispr/interface/storage/loading.py
--rwx------   0 eric      (1000) users      (984)     3550 2024-04-10 14:07:15.000000 pyvispr-2024.2/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/interface/window/
--rwx------   0 eric      (1000) users      (984)    15868 2024-04-11 14:00:34.000000 pyvispr-2024.2/pyvispr/interface/window/installer.py
--rwx------   0 eric      (1000) users      (984)     1841 2023-12-13 13:55:15.000000 pyvispr-2024.2/pyvispr/interface/window/messenger.py
--rwx------   0 eric      (1000) users      (984)     7880 2024-04-11 10:10:11.000000 pyvispr-2024.2/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/interface/window/widget/
--rwx------   0 eric      (1000) users      (984)    16048 2024-04-11 13:33:15.000000 pyvispr-2024.2/pyvispr/interface/window/widget/function_header.py
--rwx------   0 eric      (1000) users      (984)     4147 2024-04-11 13:01:01.000000 pyvispr-2024.2/pyvispr/interface/window/widget/list.py
--rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.2/pyvispr/interface/window/widget/list_file.py
--rwx------   0 eric      (1000) users      (984)     2458 2024-01-19 20:05:03.000000 pyvispr-2024.2/pyvispr/interface/window/widget/list_function.py
--rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/interface/window/widget/list_module.py
--rwx------   0 eric      (1000) users      (984)     3818 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/interface/window/widget/list_node.py
--rwx------   0 eric      (1000) users      (984)     2412 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/interface/window/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.2/pyvispr/run.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr/runtime/
--rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.2/pyvispr/runtime/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.2/pyvispr/runtime/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1628 2024-04-10 14:44:17.000000 pyvispr-2024.2/pyvispr/runtime/messenger.py
--rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.2/pyvispr/runtime/socket.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-11 14:03:48.000000 pyvispr-2024.2/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-11 14:04:11.646021 pyvispr-2024.2/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2280 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-11 14:04:11.000000 pyvispr-2024.2/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-10 14:52:27.000000 pyvispr-2024.2/requirements.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-11 14:04:11.646021 pyvispr-2024.2/setup.cfg
--rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.2/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.3/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-15 11:19:49.366336 pyvispr-2024.3/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.3/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.3/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.3/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.359669 pyvispr-2024.3/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.3/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.3/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.3/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.3/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    15487 2024-04-15 11:08:52.000000 pyvispr-2024.3/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.3/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.3/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     5762 2024-04-13 15:12:28.000000 pyvispr-2024.3/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.3/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4114 2024-04-11 12:31:33.000000 pyvispr-2024.3/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.3/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.3/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.3/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2586 2024-01-19 18:43:09.000000 pyvispr-2024.3/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1711 2023-12-13 13:08:28.000000 pyvispr-2024.3/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.3/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.3/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.3/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.3/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.3/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.3/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.3/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11820 2024-04-11 13:59:35.000000 pyvispr-2024.3/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-11 10:11:11.000000 pyvispr-2024.3/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.3/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.3/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7851 2024-04-11 14:03:03.000000 pyvispr-2024.3/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.3/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     6827 2024-04-11 08:16:26.000000 pyvispr-2024.3/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4509 2023-12-12 21:43:02.000000 pyvispr-2024.3/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10964 2024-04-12 14:30:49.000000 pyvispr-2024.3/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     3621 2024-04-13 16:08:47.000000 pyvispr-2024.3/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2549 2024-04-10 14:37:49.000000 pyvispr-2024.3/pyvispr/flow/functional/socket.py
+-rwx------   0 eric      (1000) users      (984)     2169 2024-04-10 16:31:30.000000 pyvispr-2024.3/pyvispr/flow/messenger.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18732 2024-04-11 08:03:57.000000 pyvispr-2024.3/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.3/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.3/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13413 2024-04-15 11:07:24.000000 pyvispr-2024.3/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7968 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.359669 pyvispr-2024.3/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     2993 2024-04-10 14:07:15.000000 pyvispr-2024.3/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3550 2024-04-10 14:07:15.000000 pyvispr-2024.3/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    15868 2024-04-11 14:00:34.000000 pyvispr-2024.3/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     1841 2023-12-13 13:55:15.000000 pyvispr-2024.3/pyvispr/interface/window/messenger.py
+-rwx------   0 eric      (1000) users      (984)     7880 2024-04-11 10:10:11.000000 pyvispr-2024.3/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16048 2024-04-11 13:33:15.000000 pyvispr-2024.3/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-11 13:01:01.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2458 2024-01-19 20:05:03.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3818 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.3/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.3/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1628 2024-04-10 14:44:17.000000 pyvispr-2024.3/pyvispr/runtime/messenger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.3/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-15 11:18:11.000000 pyvispr-2024.3/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2280 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-10 14:52:27.000000 pyvispr-2024.3/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-15 11:19:49.366336 pyvispr-2024.3/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.3/setup.py
```

### Comparing `pyvispr-2024.2/PKG-INFO` & `pyvispr-2024.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.2
+Version: 2024.3
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
```

### Comparing `pyvispr-2024.2/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.3/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/README-LICENCE-utf8.txt` & `pyvispr-2024.3/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/README.rst` & `pyvispr-2024.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/documentation/wiki/description.asciidoc` & `pyvispr-2024.3/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/__init__.py` & `pyvispr-2024.3/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/factory/image_loader.py` & `pyvispr-2024.3/pyvispr/catalog/factory/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/factory/numexpr_calculator.py` & `pyvispr-2024.3/pyvispr/catalog/factory/numexpr_calculator.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/factory/value.py` & `pyvispr-2024.3/pyvispr/catalog/factory/value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/factory/value_viewer.py` & `pyvispr-2024.3/pyvispr/install.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,41 +25,25 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Any
+from sys import argv as cmd_line_args
+from sys import exit as Exit
 
-import PyQt6.QtWidgets as wdgt
-from pyvispr.extension.qt6 import ExecuteApp, QtApp
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from PyQt6.QtWidgets import QApplication
+from pyvispr.interface.window.installer import installer_wdw_t
 
 
-def pyVisprValueViewer(value: Any, /) -> None:
+def Main() -> None:
     """"""
-    app, should_exec = QtApp()
-    value_viewer = value_viewer_t(value, wdgt.QApplication.activeWindow())
-    value_viewer.show()
-    ExecuteApp(app, should_exec)
+    app = QApplication(cmd_line_args)
+    window = installer_wdw_t.New()
+    window.show()
+    Exit(app.exec())
 
 
-class value_viewer_t(wdgt.QMainWindow):
-    def __init__(self, value: Any, wdw: wdgt.QWidget, /) -> None:
-        """"""
-        super().__init__(wdw)
-
-        viewer = wdgt.QTextEdit(str(value))
-        done = wdgt.QPushButton("Done")
-
-        layout = wdgt.QVBoxLayout()
-        layout.addWidget(viewer)
-        layout.addWidget(done)
-
-        central = wdgt.QWidget()
-        central.setLayout(layout)
-        self.setCentralWidget(central)
-
-        self.setWindowTitle("pyVispr Value Viewer")
-
-        CreateMessageCanal(done, "clicked", self.close)
+if __name__ == "__main__":
+    #
+    Main()
```

### Comparing `pyvispr-2024.2/pyvispr/catalog/installer.py` & `pyvispr-2024.3/pyvispr/catalog/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/parser.py` & `pyvispr-2024.3/pyvispr/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/catalog/type.py` & `pyvispr-2024.3/pyvispr/catalog/type.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/config/appearance/backend.py` & `pyvispr-2024.3/pyvispr/config/appearance/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/config/appearance/behavior.py` & `pyvispr-2024.3/pyvispr/config/appearance/behavior.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/config/appearance/color.py` & `pyvispr-2024.3/pyvispr/config/appearance/color.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.3/pyvispr/config/appearance/geometry.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/config/path.py` & `pyvispr-2024.3/pyvispr/config/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/app.py` & `pyvispr-2024.3/pyvispr/constant/app.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/catalog.py` & `pyvispr-2024.3/pyvispr/constant/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/function.py` & `pyvispr-2024.3/pyvispr/constant/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/path.py` & `pyvispr-2024.3/pyvispr/constant/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/socket.py` & `pyvispr-2024.3/pyvispr/constant/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/widget/function_header.py` & `pyvispr-2024.3/pyvispr/constant/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/widget/list.py` & `pyvispr-2024.3/pyvispr/constant/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/constant/widget/node.py` & `pyvispr-2024.3/pyvispr/constant/widget/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/extension/function.py` & `pyvispr-2024.3/pyvispr/extension/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/extension/module.py` & `pyvispr-2024.3/pyvispr/extension/module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/extension/qt6.py` & `pyvispr-2024.3/pyvispr/extension/qt6.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/extension/string_.py` & `pyvispr-2024.3/pyvispr/extension/string_.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/descriptive/node.py` & `pyvispr-2024.3/pyvispr/flow/descriptive/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.3/pyvispr/flow/descriptive/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/functional/graph.py` & `pyvispr-2024.3/pyvispr/flow/functional/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/functional/link.py` & `pyvispr-2024.3/pyvispr/flow/functional/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.3/pyvispr/flow/functional/node_isolated.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+import traceback as tbck
 import typing as h
 from enum import Enum as enum_t
 
 from json_any import JsonStringOf
 from logger_36 import LOGGER
 from pyvispr.constant.socket import OUTPUT_SET, OUTPUT_UNSET
 from pyvispr.flow.descriptive.node import node_t as description_t
@@ -254,15 +255,17 @@
         try:
             if anonymous_args is None:
                 output = self.description.Function()
             else:
                 output = self.description.Function(*anonymous_args, **named_args)
         except Exception as exception:
             output = _FakeOutputs(self.description.n_outputs, None)
-            LOGGER.error(f"Error while running {self.unique_name}:\n{exception}")
+            lines = tbck.format_exception(exception)
+            as_str = "\n".join(lines[:1] + lines[2:])
+            LOGGER.error(f"Error while running {self.unique_name}:\n{as_str}")
 
         return output
 
     def SetInputValue(self, name: str, value: h.Any, /) -> None:
         """"""
         self.inputs[name].value = value
```

### Comparing `pyvispr-2024.2/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.3/pyvispr/flow/functional/node_linked.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,24 @@
 import dataclasses as dtcl
 
 from pyvispr.flow.functional.link import outbound_links_t
 from pyvispr.flow.functional.node_isolated import node_t as base_t
 from pyvispr.flow.functional.node_isolated import state_e
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
+@dtcl.dataclass(repr=False, eq=False)
 class node_t(base_t):
     """
     links[idx]: Outbound links of node of index idx in list "nodes":
         - None if node has no outbound links.
         - If not None, dictionary with:
             - key=name of output and...
             - value=list of alternating target nodes and name of target inputs.
+
+    Cannot be sloted because of QThread issue with weak reference (see visual.graph).
     """
 
     links: outbound_links_t = dtcl.field(init=False, default_factory=outbound_links_t)
 
     def AddLink(self, output_name: str, target: node_t, input_name: str, /) -> None:
         """"""
         self.links.Add(
```

### Comparing `pyvispr-2024.2/pyvispr/flow/functional/socket.py` & `pyvispr-2024.3/pyvispr/flow/functional/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/messenger.py` & `pyvispr-2024.3/pyvispr/flow/messenger.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/graph.py` & `pyvispr-2024.3/pyvispr/flow/visual/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/ii_value.py` & `pyvispr-2024.3/pyvispr/flow/visual/ii_value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/link.py` & `pyvispr-2024.3/pyvispr/flow/visual/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/node.py` & `pyvispr-2024.3/pyvispr/flow/visual/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     NEEDS_RUNNING,
     TOP_OF_BOTTOM_BUTTONS,
     WIDTH_OF_LATERAL_BUTTONS,
 )
 from pyvispr.flow.descriptive.socket import assignment_e
 from pyvispr.flow.functional.node_linked import node_t as functional_t
 from pyvispr.flow.visual.ii_value import invalid_ii_value_t
+from pyvispr.interface.window.messenger import CreateMessageCanal
 from pyvispr.runtime.backend import SCREEN_BACKEND
 from pyvispr.runtime.socket import VALUE_NOT_SET, value_not_set_t
 from str_to_obj import annotation_t
 
 
 class ii_widget_p(wdgt.QWidget):
     def Assign(
@@ -283,14 +284,23 @@
                 interactive_inputs[name] = value_wgt
                 n_widgets += 1
 
                 layout.addWidget(wdgt.QLabel(name), i_idx, 0, 1, 1)
                 layout.addWidget(type_wgt, i_idx, 1, 1, 1)
                 layout.addWidget(value_wgt.library_wgt, i_idx, 2, 1, 1)
 
+                if isinstance(value_wgt.library_wgt, wdgt.QStackedWidget):
+                    widgets = (_elm for _elm in value_wgt.values)
+                else:
+                    widgets = (value_wgt,)
+                for widget in widgets:
+                    widget.SetAcknowledgeValueChangeFunction(
+                        self.functional.InvalidateOutputValues
+                    )
+
         if n_widgets > 0:
             self.interactive_inputs = interactive_inputs
 
             widget = wdgt.QWidget()
             widget.setLayout(layout)
             widget.setStyleSheet(f"background-color: {color_e.deepskyblue.name()};")
```

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/socket.py` & `pyvispr-2024.3/pyvispr/flow/visual/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.3/pyvispr/flow/visual/whiteboard.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/install.py` & `pyvispr-2024.3/pyvispr/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from sys import argv as cmd_line_args
 from sys import exit as Exit
 
 from PyQt6.QtWidgets import QApplication
-from pyvispr.interface.window.installer import installer_wdw_t
+from pyvispr.interface.window.runner import runner_wdw_t
 
 
 def Main() -> None:
     """"""
     app = QApplication(cmd_line_args)
-    window = installer_wdw_t.New()
+    window = runner_wdw_t.New()
     window.show()
     Exit(app.exec())
 
 
 if __name__ == "__main__":
     #
     Main()
```

### Comparing `pyvispr-2024.2/pyvispr/interface/storage/loading.py` & `pyvispr-2024.3/pyvispr/interface/storage/loading.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.3/pyvispr/interface/storage/stowing.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/installer.py` & `pyvispr-2024.3/pyvispr/interface/window/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/messenger.py` & `pyvispr-2024.3/pyvispr/interface/window/messenger.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/runner.py` & `pyvispr-2024.3/pyvispr/interface/window/runner.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/function_header.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/list_file.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/list_file.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/list_function.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/list_function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/list_module.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/list_module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/list_node.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/list_node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.3/pyvispr/interface/window/widget/menu.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/run.py` & `pyvispr-2024.3/pyvispr/runtime/socket.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,25 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from sys import argv as cmd_line_args
-from sys import exit as Exit
 
-from PyQt6.QtWidgets import QApplication
-from pyvispr.interface.window.runner import runner_wdw_t
+class assign_when_importing_t:
+    pass
 
 
-def Main() -> None:
-    """"""
-    app = QApplication(cmd_line_args)
-    window = runner_wdw_t.New()
-    window.show()
-    Exit(app.exec())
+ASSIGN_WHEN_ACTIVATING = assign_when_importing_t()
 
 
-if __name__ == "__main__":
-    #
-    Main()
+class value_not_set_t:
+    pass
+
+
+VALUE_NOT_SET = value_not_set_t()
```

### Comparing `pyvispr-2024.2/pyvispr/runtime/backend.py` & `pyvispr-2024.3/pyvispr/runtime/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/runtime/catalog.py` & `pyvispr-2024.3/pyvispr/runtime/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/runtime/messenger.py` & `pyvispr-2024.3/pyvispr/runtime/messenger.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/pyvispr/runtime/socket.py` & `pyvispr-2024.3/pyvispr/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,20 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-
-class assign_when_importing_t:
-    pass
-
-
-ASSIGN_WHEN_ACTIVATING = assign_when_importing_t()
-
-
-class value_not_set_t:
-    pass
-
-
-VALUE_NOT_SET = value_not_set_t()
+__version__ = "2024.3"
```

### Comparing `pyvispr-2024.2/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.3/pyvispr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.2
+Version: 2024.3
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
```

### Comparing `pyvispr-2024.2/pyvispr.egg-info/SOURCES.txt` & `pyvispr-2024.3/pyvispr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.2/setup.py` & `pyvispr-2024.3/setup.py`

 * *Files identical despite different names*

