# Comparing `tmp/babelwidget-2023.9.tar.gz` & `tmp/babelwidget-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelwidget-2023.9.tar", last modified: Wed Oct 11 12:57:57 2023, max compression
+gzip compressed data, was "babelwidget-2024.1.tar", last modified: Mon Apr 15 11:14:03 2024, max compression
```

## Comparing `babelwidget-2023.9.tar` & `babelwidget-2024.1.tar`

### file list

```diff
@@ -1,51 +1,66 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 babelwidget-2023.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5305 2023-10-11 12:57:57.097864 babelwidget-2023.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-10-05 13:15:24.000000 babelwidget-2023.9/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelwidget-2023.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     4473 2023-10-05 13:22:38.000000 babelwidget-2023.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.094531 babelwidget-2023.9/babelwidget/
--rw-r--r--   0 eric      (1000) users      (984)     1596 2023-10-05 13:15:54.000000 babelwidget-2023.9/babelwidget/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.094531 babelwidget-2023.9/babelwidget/backend/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/babelwidget/backend/pyqt5/
--rw-r--r--   0 eric      (1000) users      (984)     2788 2023-10-06 08:03:57.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2381 2023-10-05 13:38:47.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     2040 2023-10-06 18:56:34.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     3239 2023-10-11 12:57:03.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/image.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1960 2023-10-09 14:33:45.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/menu.py
--rw-r--r--   0 eric      (1000) users      (984)     1708 2023-10-05 14:53:05.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/paragraph.py
--rw-r--r--   0 eric      (1000) users      (984)     2060 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2023-10-05 13:38:47.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt5/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/babelwidget/backend/pyqt6/
--rw-r--r--   0 eric      (1000) users      (984)     2898 2023-10-11 12:30:13.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2379 2023-10-05 13:39:00.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     2040 2023-10-06 18:56:26.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     3288 2023-10-11 12:57:00.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/image.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1960 2023-10-09 14:33:45.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/menu.py
--rw-r--r--   0 eric      (1000) users      (984)     1708 2023-10-05 14:53:30.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/paragraph.py
--rw-r--r--   0 eric      (1000) users      (984)     2059 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1968 2023-10-05 13:39:00.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-10-05 13:29:54.000000 babelwidget-2023.9/babelwidget/backend/pyqt6/widget/text.py
--rw-r--r--   0 eric      (1000) users      (984)     5081 2023-10-11 11:47:43.000000 babelwidget-2023.9/babelwidget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     7663 2023-10-05 14:02:22.000000 babelwidget-2023.9/babelwidget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-10-11 12:57:47.000000 babelwidget-2023.9/babelwidget/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/babelwidget.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5305 2023-10-11 12:57:57.000000 babelwidget-2023.9/babelwidget.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1399 2023-10-11 12:57:57.000000 babelwidget-2023.9/babelwidget.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-10-11 12:57:57.000000 babelwidget-2023.9/babelwidget.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       12 2023-10-11 12:57:57.000000 babelwidget-2023.9/babelwidget.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.094531 babelwidget-2023.9/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-10-11 12:57:57.097864 babelwidget-2023.9/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1912 2023-10-05 13:23:51.000000 babelwidget-2023.9/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 babelwidget-2023.9/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-10-11 12:57:57.097864 babelwidget-2023.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5858 2023-10-05 13:41:39.000000 babelwidget-2023.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.096332 babelwidget-2024.1/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 babelwidget-2024.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5305 2024-04-15 11:14:03.096332 babelwidget-2024.1/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-10-05 13:15:24.000000 babelwidget-2024.1/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelwidget-2024.1/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4473 2023-10-05 13:22:38.000000 babelwidget-2024.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.089666 babelwidget-2024.1/babelwidget/
+-rwx------   0 eric      (1000) users      (984)     1596 2023-10-05 13:15:54.000000 babelwidget-2024.1/babelwidget/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/
+-rwx------   0 eric      (1000) users      (984)     2647 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/builder.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/generic/
+-rwx------   0 eric      (1000) users      (984)     7639 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/generic/path_chooser.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/pyqt5/
+-rwx------   0 eric      (1000) users      (984)     2700 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     1859 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/function.py
+-rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/
+-rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/button.py
+-rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/choices.py
+-rwx------   0 eric      (1000) users      (984)     2143 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/image.py
+-rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/label.py
+-rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/text_line.py
+-rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt5/widget/unchanged.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/pyqt6/
+-rwx------   0 eric      (1000) users      (984)     2809 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     1859 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/function.py
+-rwx------   0 eric      (1000) users      (984)     2115 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.092999 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/
+-rwx------   0 eric      (1000) users      (984)     1777 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/button.py
+-rwx------   0 eric      (1000) users      (984)     2119 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/choices.py
+-rwx------   0 eric      (1000) users      (984)     2157 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/image.py
+-rwx------   0 eric      (1000) users      (984)     1755 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/label.py
+-rwx------   0 eric      (1000) users      (984)     1787 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1964 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1815 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1767 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1770 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/text_line.py
+-rwx------   0 eric      (1000) users      (984)     1780 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqt6/widget/unchanged.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.096332 babelwidget-2024.1/babelwidget/backend/pyqtx/
+-rwx------   0 eric      (1000) users      (984)     1678 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/button.py
+-rwx------   0 eric      (1000) users      (984)     2094 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/choices.py
+-rwx------   0 eric      (1000) users      (984)     3358 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/image.py
+-rwx------   0 eric      (1000) users      (984)     1612 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/label.py
+-rwx------   0 eric      (1000) users      (984)     3079 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/main.py
+-rwx------   0 eric      (1000) users      (984)     1841 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/menu.py
+-rwx------   0 eric      (1000) users      (984)     2136 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/path_chooser.py
+-rwx------   0 eric      (1000) users      (984)     1732 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/scroll_container.py
+-rwx------   0 eric      (1000) users      (984)     1627 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/text_box.py
+-rwx------   0 eric      (1000) users      (984)     1620 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/backend/pyqtx/text_line.py
+-rwx------   0 eric      (1000) users      (984)     5411 2024-04-15 11:10:59.000000 babelwidget-2024.1/babelwidget/main.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-04-15 11:13:04.000000 babelwidget-2024.1/babelwidget/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.096332 babelwidget-2024.1/babelwidget.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5305 2024-04-15 11:14:03.000000 babelwidget-2024.1/babelwidget.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1916 2024-04-15 11:14:03.000000 babelwidget-2024.1/babelwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-15 11:14:03.000000 babelwidget-2024.1/babelwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       12 2024-04-15 11:14:03.000000 babelwidget-2024.1/babelwidget.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.089666 babelwidget-2024.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:14:03.096332 babelwidget-2024.1/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1912 2023-10-05 13:23:51.000000 babelwidget-2024.1/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 babelwidget-2024.1/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-15 11:14:03.096332 babelwidget-2024.1/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5932 2023-11-07 14:56:02.000000 babelwidget-2024.1/setup.py
```

### Comparing `babelwidget-2023.9/PKG-INFO` & `babelwidget-2024.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelwidget
-Version: 2023.9
+Version: 2024.1
 Summary: A Meta Widget Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelwidget//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
```

### Comparing `babelwidget-2023.9/README-COPYRIGHT-utf8.txt` & `babelwidget-2024.1/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelwidget-2023.9/README-LICENCE-utf8.txt` & `babelwidget-2024.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelwidget-2023.9/README.rst` & `babelwidget-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `babelwidget-2023.9/babelwidget/__init__.py` & `babelwidget-2024.1/babelwidget/__init__.py`

 * *Files identical despite different names*

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/constant.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/constant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -29,14 +29,16 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt5.QtCore as core
 import PyQt5.QtGui as visl
 import PyQt5.QtWidgets as wdgt
 
+EXECUTE = "exec_"
+
 ALIGNED_CENTER = core.Qt.AlignmentFlag.AlignCenter
 ALIGNED_HCENTER = core.Qt.AlignmentFlag.AlignHCenter
 ALIGNED_LEFT = core.Qt.AlignmentFlag.AlignLeft
 ALIGNED_RIGHT = core.Qt.AlignmentFlag.AlignRight
 ALIGNED_TOP = core.Qt.AlignmentFlag.AlignTop
 BASE_PALETTE = visl.QPalette.Base
 DIALOG_ACCEPTATION = wdgt.QDialog.Accepted
@@ -51,12 +53,7 @@
 SELECTABLE_TEXT = core.Qt.TextInteractionFlag.TextSelectableByMouse
 SIZE_EXPANDING = wdgt.QSizePolicy.Expanding
 SIZE_FIXED = wdgt.QSizePolicy.Fixed
 SIZE_MINIMUM = wdgt.QSizePolicy.Minimum
 TAB_POSITION_EAST = wdgt.QTabWidget.East
 WIDGET_TYPE = core.Qt.WindowType.Widget
 WORD_NO_WRAP = visl.QTextOption.WrapMode.NoWrap
-
-
-def Color(name: str, /) -> visl.QColorConstants:
-    """"""
-    return getattr(visl.QColorConstants, name)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/main.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/label.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,33 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
-from PyQt5.QtCore import QCoreApplication as qt_core_app_t
-
-from babelwidget.backend.pyqt5.widget.main import library_wgt_t
-
-
-class event_loop_t(wdgt.QApplication):
-    def Run(self) -> int:
-        """"""
-        return self.exec_()
-
-
-def ShowMessage(title: str, message: str, /, *, parent: library_wgt_t = None) -> None:
-    """"""
-    dialog = wdgt.QMessageBox(parent=parent)
-    dialog.setWindowTitle(title)
-    dialog.setText("<b>" + title + "</b>")
-    dialog.setInformativeText(message)
-    dialog.setStandardButtons(wdgt.QMessageBox.StandardButton.Close)
-    dialog.setDefaultButton(wdgt.QMessageBox.StandardButton.Close)
-    dialog.exec_()
-
-
-def ShowErrorMessage(message: str, /, *, parent: library_wgt_t = None) -> None:
-    """"""
-    wdgt.QMessageBox.critical(parent, "Error", message)
+import PyQt6.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.label import Text
+
+label_t = NewClass(
+    "label_t",
+    wdgt.QLabel,
+    method=Text,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/button.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,24 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
+import typing as h
 
-import PyQt5.QtWidgets as wdgt
 
-
-class button_wgt_t(wdgt.QPushButton):
+def NewWithFunction(cls, Function: h.Callable, /) -> h.Any:
     """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.clicked.connect(function)
+    output = cls()
+    output.triggered.connect(lambda _nty: Function(_nty.text()))
+    return output
 
 
-class dot_button_wgt_t(wdgt.QRadioButton):
+def ItemAt(self, index: int, /) -> str:
     """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.toggled.connect(function)
+    return self.actions()[index].text()
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/choices.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/label.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,25 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
-
 import PyQt5.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.label import Text
 
-
-class choice_menu_wgt_t(wdgt.QComboBox):
-    def Text(self) -> str:
-        return self.currentText()
-
-    def ItemAt(self, index: int, /) -> str:
-        return self.itemText(index)
-
-    def SetFunction(self, function: Callable, /) -> None:
-        """
-        self.activated.connect(function): Responds only to GUI interaction, not
-        programmatic change.
-        """
-        self.currentIndexChanged.connect(function)
+label_t = NewClass(
+    "label_t",
+    wdgt.QLabel,
+    method=Text,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/image.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,60 +25,73 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtGui as visl
-import PyQt5.QtWidgets as wdgt
-from numpy import ndarray as n_array_t
-from PyQt5.QtCore import QPoint as point_t
+import typing as h
 
-SIZE_FIXED = wdgt.QSizePolicy.Fixed
 
+def __init__Function(size_policy, /) -> h.Callable:
+    """"""
 
-class image_wgt_t(wdgt.QLabel):
     def __init__(self, *args, **kwargs) -> None:
         """"""
-        super().__init__(*args, **kwargs)
-        self.setSizePolicy(SIZE_FIXED, SIZE_FIXED)
+        super(self.__class__, self).__init__(*args, **kwargs)
+        self.setSizePolicy(size_policy, size_policy)
         self.setScaledContents(True)
         # Must be kept alive in instance.
         self.q_image = None
 
+    return __init__
+
+
+def SetImageFunction(module, n_array_t, img_format, /):
+    """"""
+
     def SetImage(self, rgb_image: n_array_t, /) -> None:
         """
         QImage call taken from:
         https://github.com/baoboa/pyqt5/blob/master/examples/widgets/imageviewer.py
         """
-        self.q_image = visl.QImage(
+        self.q_image = module.QImage(
             rgb_image.data,
             rgb_image.shape[1],
             rgb_image.shape[0],
             3 * rgb_image.shape[1],
-            visl.QImage.Format_RGB888,
+            img_format,
         )
-        self.setPixmap(visl.QPixmap.fromImage(self.q_image))
+        self.setPixmap(module.QPixmap.fromImage(self.q_image))
+
+    return SetImage
+
+
+def DrawPointsFunction(module, n_array_t, point_t, /):
+    """"""
 
     def DrawPoints(
         self,
         points: tuple[n_array_t, n_array_t],
         color: tuple[int, int, int],
         /,
         *,
         bbox_width: int = 1,
         bbox_height: int = 1,
     ) -> None:
         """"""
         contour_qpoints = tuple(point_t(point[1], point[0]) for point in zip(*points))
-        pixmap = visl.QPixmap(self.pixmap())
+        pixmap = module.QPixmap(self.pixmap())
 
-        painter = visl.QPainter()
+        painter = module.QPainter()
         painter.begin(pixmap)
-        painter.setPen(visl.QPen(visl.QColor(*color)))  # Must be after call to begin
+        painter.setPen(
+            module.QPen(module.QColor(*color))
+        )  # Must be after call to begin
         for point in contour_qpoints:
             # TODO: Check why -1's are necessary.
             painter.drawPoint(point.x() + bbox_width - 1, point.y() + bbox_height - 1)
         painter.end()
 
         self.setPixmap(pixmap)
+
+    return DrawPoints
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/label.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,11 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
 
-
-class label_wgt_t(wdgt.QLabel):
-    def Text(self) -> str:
-        """"""
-        return self.text()
+def Text(self) -> str:
+    """"""
+    return self.text()
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/main.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/unchanged.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -27,16 +27,16 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt5.QtWidgets as wdgt
 
-library_wgt_t = wdgt.QWidget
+base_t = wdgt.QWidget
 
-group_wgt_t = wdgt.QGroupBox
-stack_wgt_t = wdgt.QStackedWidget
-tabs_wgt_t = wdgt.QTabWidget
+group_t = wdgt.QGroupBox
+stack_t = wdgt.QStackedWidget
+tabs_t = wdgt.QTabWidget
 
 hbox_lyt_t = wdgt.QHBoxLayout
 vbox_lyt_t = wdgt.QVBoxLayout
 grid_lyt_t = wdgt.QGridLayout
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/menu.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/button.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,23 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
-import typing as h
-
-import PyQt5.QtWidgets as wdgt
-
-
-class menu_wgt_t(wdgt.QMenu):
-    @classmethod
-    def NewWithFunction(cls, Function: h.Callable, /) -> menu_wgt_t:
-        output = cls()
-        output.triggered.connect(lambda _nty: Function(_nty.text()))
-        return output
-
-    def ItemAt(self, index: int, /) -> str:
-        return self.actions()[index].text()
+import PyQt6.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.button import SetFunction
+
+button_t = NewClass(
+    "button_t",
+    wdgt.QPushButton,
+    method=SetFunction,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/paragraph.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/text_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,11 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
 
-
-class paragraph_wgt_t(wdgt.QTextEdit):
-    def Text(self) -> str:
-        """"""
-        return self.toPlainText().strip()
+def Text(self) -> str:
+    """"""
+    return self.toPlainText().strip()
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/path_chooser.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/path_chooser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,26 +25,31 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
+import typing as h
 
 
-class path_chooser_wgt_t(wdgt.QFileDialog):
+def __init__(self, caption: str, /, *, extension_filter: str = None):
     """"""
+    if extension_filter is None:
+        extension_filter = "Any files (*)"
+    super(self.__class__, self).__init__(caption=caption, filter=extension_filter)
 
-    def __init__(self, caption: str, /, *, extension_filter: str = None):
-        """"""
-        if extension_filter is None:
-            extension_filter = "Any files (*)"
-        super().__init__(caption=caption, filter=extension_filter)
 
-    def SelectedFile(self) -> str:
-        """"""
-        return self.selectedFiles()[0]
+def SelectedFile(self) -> str:
+    """"""
+    return self.selectedFiles()[0]
+
+
+def RunAndGetClosingStatusFunction(execute: str, /) -> h.Callable:
+    """"""
 
     def RunAndGetClosingStatus(self) -> int:
         """"""
-        return self.exec_()
+        Execute = getattr(self, execute)
+        return Execute()
+
+    return RunAndGetClosingStatus
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/scroll_container.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,25 +25,12 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+import PyQt6.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.menu import ItemAt, NewWithFunction
 
-import PyQt5.QtWidgets as wdgt
-
-from babelwidget.backend.pyqt5.widget.main import library_wgt_t
-
-
-class scroll_container_t(wdgt.QScrollArea):
-    """"""
-
-    @classmethod
-    def NewForWidget(cls, widget: library_wgt_t, /) -> scroll_container_t:
-        """"""
-        output = cls()
-        output.setWidget(widget)
-        output.setWidgetResizable(True)
-
-        return output
+menu_t = NewClass("menu_t", wdgt.QMenu, method=ItemAt, class_method=NewWithFunction)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt5/widget/text.py` & `babelwidget-2024.1/babelwidget/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
-
-
-class text_wgt_t(wdgt.QLineEdit):
-    def Text(self) -> str:
-        """"""
-        return self.text().strip()
+__version__ = "2024.1"
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/constant.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/constant.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -29,14 +29,16 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt6.QtCore as core
 import PyQt6.QtGui as visl
 import PyQt6.QtWidgets as wdgt
 
+EXECUTE = "exec"
+
 ALIGNED_CENTER = core.Qt.AlignmentFlag.AlignCenter
 ALIGNED_HCENTER = core.Qt.AlignmentFlag.AlignHCenter
 ALIGNED_LEFT = core.Qt.AlignmentFlag.AlignLeft
 ALIGNED_RIGHT = core.Qt.AlignmentFlag.AlignRight
 ALIGNED_TOP = core.Qt.AlignmentFlag.AlignTop
 BASE_PALETTE = visl.QPalette.ColorRole.Base
 DIALOG_ACCEPTATION = wdgt.QDialog.DialogCode.Accepted
@@ -51,12 +53,7 @@
 SELECTABLE_TEXT = core.Qt.TextInteractionFlag.TextSelectableByMouse
 SIZE_EXPANDING = wdgt.QSizePolicy.Policy.Expanding
 SIZE_FIXED = wdgt.QSizePolicy.Policy.Fixed
 SIZE_MINIMUM = wdgt.QSizePolicy.Policy.Minimum
 TAB_POSITION_EAST = wdgt.QTabWidget.TabPosition.East
 WIDGET_TYPE = core.Qt.WindowType.Widget
 WORD_NO_WRAP = visl.QTextOption.WrapMode.NoWrap
-
-
-def Color(name: str, /) -> visl.QColorConstants:
-    """"""
-    return getattr(visl.QColorConstants, name)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/main.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/button.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,33 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
-from PyQt6.QtCore import QCoreApplication as qt_core_app_t
-
-from babelwidget.backend.pyqt6.widget.main import library_wgt_t
-
-
-class event_loop_t(wdgt.QApplication):
-    def Run(self) -> int:
-        """"""
-        return self.exec()
-
-
-def ShowMessage(title: str, message: str, /, *, parent: library_wgt_t = None) -> None:
-    """"""
-    dialog = wdgt.QMessageBox(parent=parent)
-    dialog.setWindowTitle(title)
-    dialog.setText("<b>" + title + "</b>")
-    dialog.setInformativeText(message)
-    dialog.setStandardButtons(wdgt.QMessageBox.StandardButton.Close)
-    dialog.setDefaultButton(wdgt.QMessageBox.StandardButton.Close)
-    dialog.exec()
-
-
-def ShowErrorMessage(message: str, /, *, parent: library_wgt_t = None) -> None:
-    """"""
-    wdgt.QMessageBox.critical(parent, "Error", message)
+import PyQt5.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.button import SetFunction
+
+button_t = NewClass(
+    "button_t",
+    wdgt.QPushButton,
+    method=SetFunction,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/button.py` & `babelwidget-2024.1/documentation/wiki/description.asciidoc`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-# Copyright CNRS/Inria/UNS
-# Contributor(s): Eric Debreuve (since 2023)
-#
-# eric.debreuve@cnrs.fr
-#
-# This software is governed by the CeCILL  license under French law and
-# abiding by the rules of distribution of free software.  You can  use,
-# modify and/ or redistribute the software under the terms of the CeCILL
-# license as circulated by CEA, CNRS and INRIA at the following URL
-# "http://www.cecill.info".
-#
-# As a counterpart to the access to the source code and  rights to copy,
-# modify and redistribute granted by the license, users are provided only
-# with a limited warranty  and the software's author,  the holder of the
-# economic rights,  and the successive licensors  have only  limited
-# liability.
-#
-# In this respect, the user's attention is drawn to the risks associated
-# with loading,  using,  modifying and/or developing or reproducing the
-# software by the user in light of its specific status of free software,
-# that may mean  that it is complicated to manipulate,  and  that  also
-# therefore means  that it is reserved for developers  and  experienced
-# professionals having in-depth computer knowledge. Users are therefore
-# encouraged to load and test the software's suitability as regards their
-# requirements in conditions enabling the security of their systems and/or
-# data to be ensured and,  more generally, to use and operate it in the
-# same conditions as regards security.
-#
-# The fact that you are presently reading this means that you have had
-# knowledge of the CeCILL license and that you accept its terms.
-
-from typing import Callable
-
-import PyQt6.QtWidgets as wdgt
-
-
-class button_wgt_t(wdgt.QPushButton):
-    """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.clicked.connect(function)
-
-
-class dot_button_wgt_t(wdgt.QRadioButton):
-    """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.toggled.connect(function)
+// Copyright CNRS/Inria/UCA
+// Contributor(s): Eric Debreuve (since 2023)
+//
+// eric.debreuve@cnrs.fr
+//
+// This software is governed by the CeCILL  license under French law and
+// abiding by the rules of distribution of free software.  You can  use,
+// modify and/ or redistribute the software under the terms of the CeCILL
+// license as circulated by CEA, CNRS and INRIA at the following URL
+// "http://www.cecill.info".
+//
+// As a counterpart to the access to the source code and  rights to copy,
+// modify and redistribute granted by the license, users are provided only
+// with a limited warranty  and the software's author,  the holder of the
+// economic rights,  and the successive licensors  have only  limited
+// liability.
+//
+// In this respect, the user's attention is drawn to the risks associated
+// with loading,  using,  modifying and/or developing or reproducing the
+// software by the user in light of its specific status of free software,
+// that may mean  that it is complicated to manipulate,  and  that  also
+// therefore means  that it is reserved for developers  and  experienced
+// professionals having in-depth computer knowledge. Users are therefore
+// encouraged to load and test the software's suitability as regards their
+// requirements in conditions enabling the security of their systems and/or
+// data to be ensured and,  more generally, to use and operate it in the
+// same conditions as regards security.
+//
+// The fact that you are presently reading this means that you have had
+// knowledge of the CeCILL license and that you accept its terms.
+
+:AUTHOR: Eric Debreuve
+:EMAIL: eric.debreuve@cnrs.fr
+
+:PROJECT_NAME: BabelWidget
+:SHORT_DESCRIPTION: A Meta Widget Library That Speaks Several Backends
+:KEYWORDS: app, application, development, graphical interface
+
+:REPOSITORY_NAME: babelwidget
+:REPOSITORY_USER: eric.debreuve
+:REPOSITORY_SITE: src.koda.cnrs.fr
+:SINCE_YEAR: 2023
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/choices.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/text_box.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,25 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
-
 import PyQt6.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.text_box import Text
 
-
-class choice_menu_wgt_t(wdgt.QComboBox):
-    def Text(self) -> str:
-        return self.currentText()
-
-    def ItemAt(self, index: int, /) -> str:
-        return self.itemText(index)
-
-    def SetFunction(self, function: Callable, /) -> None:
-        """
-        self.activated.connect(function): Responds only to GUI interaction, not
-        programmatic change.
-        """
-        self.currentIndexChanged.connect(function)
+text_box_t = NewClass(
+    "text_box_t",
+    wdgt.QTextEdit,
+    method=Text,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/label.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/button.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,14 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
 
+import typing as h
 
-class label_wgt_t(wdgt.QLabel):
-    def Text(self) -> str:
-        """"""
-        return self.text()
+
+def SetFunction(self, function: h.Callable, /) -> None:
+    """"""
+    self.clicked.connect(function)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/main.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/unchanged.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -27,16 +27,16 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt6.QtWidgets as wdgt
 
-library_wgt_t = wdgt.QWidget
+base_t = wdgt.QWidget
 
-group_wgt_t = wdgt.QGroupBox
-stack_wgt_t = wdgt.QStackedWidget
-tabs_wgt_t = wdgt.QTabWidget
+group_t = wdgt.QGroupBox
+stack_t = wdgt.QStackedWidget
+tabs_t = wdgt.QTabWidget
 
 hbox_lyt_t = wdgt.QHBoxLayout
 vbox_lyt_t = wdgt.QVBoxLayout
 grid_lyt_t = wdgt.QGridLayout
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/menu.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/text_box.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,23 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
-import typing as h
-
-import PyQt6.QtWidgets as wdgt
-
-
-class menu_wgt_t(wdgt.QMenu):
-    @classmethod
-    def NewWithFunction(cls, Function: h.Callable, /) -> menu_wgt_t:
-        output = cls()
-        output.triggered.connect(lambda _nty: Function(_nty.text()))
-        return output
-
-    def ItemAt(self, index: int, /) -> str:
-        return self.actions()[index].text()
+import PyQt5.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.text_box import Text
+
+text_box_t = NewClass(
+    "text_box_t",
+    wdgt.QTextEdit,
+    method=Text,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/paragraph.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/text_line.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
+import PyQt5.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.text_line import Text
 
-
-class paragraph_wgt_t(wdgt.QTextEdit):
-    def Text(self) -> str:
-        """"""
-        return self.toPlainText().strip()
+text_line_t = NewClass(
+    "text_line_t",
+    wdgt.QLineEdit,
+    method=Text,
+)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/path_chooser.py` & `babelwidget-2024.1/babelwidget/backend/pyqtx/scroll_container.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,26 +25,17 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
+import typing as h
 
 
-class path_chooser_wgt_t(wdgt.QFileDialog):
+def NewForWidget(cls, widget, /) -> h.Any:
     """"""
+    output = cls()
+    output.setWidget(widget)
+    output.setWidgetResizable(True)
 
-    def __init__(self, caption: str, /, *, extension_filter: str = None):
-        """"""
-        if extension_filter is None:
-            extension_filter = "Any files (*)"
-        super().__init__(caption=caption, filter=extension_filter)
-
-    def SelectedFile(self) -> str:
-        """"""
-        return self.selectedFiles()[0]
-
-    def RunAndGetClosingStatus(self) -> int:
-        """"""
-        return self.exec()
+    return output
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/scroll_container.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/widget/menu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,25 +25,12 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+import PyQt5.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.menu import ItemAt, NewWithFunction
 
-import PyQt6.QtWidgets as wdgt
-
-from babelwidget.backend.pyqt6.widget.main import library_wgt_t
-
-
-class scroll_container_t(wdgt.QScrollArea):
-    """"""
-
-    @classmethod
-    def NewForWidget(cls, widget: library_wgt_t, /) -> scroll_container_t:
-        """"""
-        output = cls()
-        output.setWidget(widget)
-        output.setWidgetResizable(True)
-
-        return output
+menu_t = NewClass("menu_t", wdgt.QMenu, method=ItemAt, class_method=NewWithFunction)
```

### Comparing `babelwidget-2023.9/babelwidget/backend/pyqt6/widget/text.py` & `babelwidget-2024.1/babelwidget/backend/pyqt5/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
+import typing as h
 
+import PyQt5.QtCore as core
 
-class text_wgt_t(wdgt.QLineEdit):
-    def Text(self) -> str:
-        """"""
-        return self.text().strip()
+NewMessage = core.pyqtSignal
+
+
+def CreateMessageCanal(
+    messenger: core.QObject, message: str, AcknowledgeMessage: h.Callable, /
+) -> None:
+    """"""
+    signal: core.pyqtBoundSignal = getattr(messenger, message)
+    signal.connect(AcknowledgeMessage)
```

### Comparing `babelwidget-2023.9/babelwidget/path_chooser.py` & `babelwidget-2024.1/babelwidget/backend/generic/path_chooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2018)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -36,15 +36,15 @@
 
 """
 valid_types: {"Type": "extension", "Type": ("extension", "extension",...), ...}
 filter: "Image files (*.png *.xpm *.jpg);Text files (*.txt);Any files (*)"
 """
 
 
-path_chooser_wgt_h = TypeVar("path_chooser_wgt_h")
+path_chooser_h = TypeVar("path_chooser_h")
 valid_types_h = dict[str, str | Sequence[str]]
 document_selection_fct_h = Callable[..., path_t | None]
 
 
 def NewSelectedInputDocument(
     title: str,
     caption: str,
@@ -189,28 +189,26 @@
     title: str,
     caption: str,
     extension_filter: str,
     start_folder: str | path_t,
     initial_selection: str | path_t,
     backend: backend_t,
     /,
-) -> path_chooser_wgt_h:
+) -> path_chooser_h:
     """"""
-    output = backend.path_chooser_wgt_t(caption, extension_filter=extension_filter)
+    output = backend.path_chooser_t(caption, extension_filter=extension_filter)
     output.setWindowTitle(title)
     if start_folder is not None:
         output.setDirectory(str(start_folder))
     if initial_selection is not None:
         output.selectFile(str(initial_selection))
 
     return output
 
 
-def _SelectedDocument(
-    dialog: path_chooser_wgt_h, backend: backend_t, /
-) -> path_t | None:
+def _SelectedDocument(dialog: path_chooser_h, backend: backend_t, /) -> path_t | None:
     """"""
     status = dialog.RunAndGetClosingStatus()
     if status == backend.DIALOG_ACCEPTATION:
         return path_t(dialog.SelectedFile())
 
     return None
```

### Comparing `babelwidget-2023.9/babelwidget/version.py` & `babelwidget-2024.1/babelwidget/backend/pyqt6/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UCA
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2023)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,8 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.9"
+import typing as h
+
+import PyQt6.QtCore as core
+
+NewMessage = core.pyqtSignal
+
+
+def CreateMessageCanal(
+    messenger: core.QObject, message: str, AcknowledgeMessage: h.Callable, /
+) -> None:
+    """"""
+    signal: core.pyqtBoundSignal = getattr(messenger, message)
+    signal.connect(AcknowledgeMessage)
```

### Comparing `babelwidget-2023.9/babelwidget.egg-info/PKG-INFO` & `babelwidget-2024.1/babelwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelwidget
-Version: 2023.9
+Version: 2024.1
 Summary: A Meta Widget Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelwidget//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelwidget/
```

### Comparing `babelwidget-2023.9/babelwidget.egg-info/SOURCES.txt` & `babelwidget-2024.1/babelwidget.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,38 +2,51 @@
 README-COPYRIGHT-utf8.txt
 README-LICENCE-utf8.txt
 README.rst
 pyproject.toml
 setup.py
 babelwidget/__init__.py
 babelwidget/main.py
-babelwidget/path_chooser.py
 babelwidget/version.py
 babelwidget.egg-info/PKG-INFO
 babelwidget.egg-info/SOURCES.txt
 babelwidget.egg-info/dependency_links.txt
 babelwidget.egg-info/top_level.txt
+babelwidget/backend/builder.py
+babelwidget/backend/generic/path_chooser.py
 babelwidget/backend/pyqt5/constant.py
+babelwidget/backend/pyqt5/function.py
 babelwidget/backend/pyqt5/main.py
 babelwidget/backend/pyqt5/widget/button.py
 babelwidget/backend/pyqt5/widget/choices.py
 babelwidget/backend/pyqt5/widget/image.py
 babelwidget/backend/pyqt5/widget/label.py
-babelwidget/backend/pyqt5/widget/main.py
 babelwidget/backend/pyqt5/widget/menu.py
-babelwidget/backend/pyqt5/widget/paragraph.py
 babelwidget/backend/pyqt5/widget/path_chooser.py
 babelwidget/backend/pyqt5/widget/scroll_container.py
-babelwidget/backend/pyqt5/widget/text.py
+babelwidget/backend/pyqt5/widget/text_box.py
+babelwidget/backend/pyqt5/widget/text_line.py
+babelwidget/backend/pyqt5/widget/unchanged.py
 babelwidget/backend/pyqt6/constant.py
+babelwidget/backend/pyqt6/function.py
 babelwidget/backend/pyqt6/main.py
 babelwidget/backend/pyqt6/widget/button.py
 babelwidget/backend/pyqt6/widget/choices.py
 babelwidget/backend/pyqt6/widget/image.py
 babelwidget/backend/pyqt6/widget/label.py
-babelwidget/backend/pyqt6/widget/main.py
 babelwidget/backend/pyqt6/widget/menu.py
-babelwidget/backend/pyqt6/widget/paragraph.py
 babelwidget/backend/pyqt6/widget/path_chooser.py
 babelwidget/backend/pyqt6/widget/scroll_container.py
-babelwidget/backend/pyqt6/widget/text.py
+babelwidget/backend/pyqt6/widget/text_box.py
+babelwidget/backend/pyqt6/widget/text_line.py
+babelwidget/backend/pyqt6/widget/unchanged.py
+babelwidget/backend/pyqtx/button.py
+babelwidget/backend/pyqtx/choices.py
+babelwidget/backend/pyqtx/image.py
+babelwidget/backend/pyqtx/label.py
+babelwidget/backend/pyqtx/main.py
+babelwidget/backend/pyqtx/menu.py
+babelwidget/backend/pyqtx/path_chooser.py
+babelwidget/backend/pyqtx/scroll_container.py
+babelwidget/backend/pyqtx/text_box.py
+babelwidget/backend/pyqtx/text_line.py
 documentation/wiki/description.asciidoc
```

### Comparing `babelwidget-2023.9/documentation/wiki/description.asciidoc` & `babelwidget-2024.1/babelwidget/backend/pyqt6/widget/choices.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-// Copyright CNRS/Inria/UCA
-// Contributor(s): Eric Debreuve (since 2023)
-//
-// eric.debreuve@cnrs.fr
-//
-// This software is governed by the CeCILL  license under French law and
-// abiding by the rules of distribution of free software.  You can  use,
-// modify and/ or redistribute the software under the terms of the CeCILL
-// license as circulated by CEA, CNRS and INRIA at the following URL
-// "http://www.cecill.info".
-//
-// As a counterpart to the access to the source code and  rights to copy,
-// modify and redistribute granted by the license, users are provided only
-// with a limited warranty  and the software's author,  the holder of the
-// economic rights,  and the successive licensors  have only  limited
-// liability.
-//
-// In this respect, the user's attention is drawn to the risks associated
-// with loading,  using,  modifying and/or developing or reproducing the
-// software by the user in light of its specific status of free software,
-// that may mean  that it is complicated to manipulate,  and  that  also
-// therefore means  that it is reserved for developers  and  experienced
-// professionals having in-depth computer knowledge. Users are therefore
-// encouraged to load and test the software's suitability as regards their
-// requirements in conditions enabling the security of their systems and/or
-// data to be ensured and,  more generally, to use and operate it in the
-// same conditions as regards security.
-//
-// The fact that you are presently reading this means that you have had
-// knowledge of the CeCILL license and that you accept its terms.
+# Copyright CNRS/Inria/UniCA
+# Contributor(s): Eric Debreuve (since 2023)
+#
+# eric.debreuve@cnrs.fr
+#
+# This software is governed by the CeCILL  license under French law and
+# abiding by the rules of distribution of free software.  You can  use,
+# modify and/ or redistribute the software under the terms of the CeCILL
+# license as circulated by CEA, CNRS and INRIA at the following URL
+# "http://www.cecill.info".
+#
+# As a counterpart to the access to the source code and  rights to copy,
+# modify and redistribute granted by the license, users are provided only
+# with a limited warranty  and the software's author,  the holder of the
+# economic rights,  and the successive licensors  have only  limited
+# liability.
+#
+# In this respect, the user's attention is drawn to the risks associated
+# with loading,  using,  modifying and/or developing or reproducing the
+# software by the user in light of its specific status of free software,
+# that may mean  that it is complicated to manipulate,  and  that  also
+# therefore means  that it is reserved for developers  and  experienced
+# professionals having in-depth computer knowledge. Users are therefore
+# encouraged to load and test the software's suitability as regards their
+# requirements in conditions enabling the security of their systems and/or
+# data to be ensured and,  more generally, to use and operate it in the
+# same conditions as regards security.
+#
+# The fact that you are presently reading this means that you have had
+# knowledge of the CeCILL license and that you accept its terms.
 
-:AUTHOR: Eric Debreuve
-:EMAIL: eric.debreuve@cnrs.fr
 
-:PROJECT_NAME: BabelWidget
-:SHORT_DESCRIPTION: A Meta Widget Library That Speaks Several Backends
-:KEYWORDS: app, application, development, graphical interface
+import PyQt6.QtWidgets as wdgt
+from babelwidget.backend.builder import NewClass
+from babelwidget.backend.pyqtx.choices import (
+    ItemAtSEPARATORDropdown,
+    SetFunctionSEPARATORDropdown,
+    SetFunctionSEPARATORRadio,
+    TextSEPARATORDropdown,
+)
 
-:REPOSITORY_NAME: babelwidget
-:REPOSITORY_USER: eric.debreuve
-:REPOSITORY_SITE: src.koda.cnrs.fr
-:SINCE_YEAR: 2023
+radio_choice_t = NewClass(
+    "radio_choice_t",
+    wdgt.QRadioButton,
+    method=SetFunctionSEPARATORRadio,
+)
+
+dropdown_choice_t = NewClass(
+    "dropdown_choice_t",
+    wdgt.QComboBox,
+    method=(
+        SetFunctionSEPARATORDropdown,
+        TextSEPARATORDropdown,
+        ItemAtSEPARATORDropdown,
+    ),
+)
```

### Comparing `babelwidget-2023.9/setup.py` & `babelwidget-2024.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,20 @@
 PYPI_AUDIENCE = "Science/Research"         # https://pypi.org/classifiers/    Intended Audience::*  # /!\ REMOVE THE PREFIX
 PYPI_STATUS = "4 - Beta"                   # https://pypi.org/classifiers/    Development Status::*  # /!\ REMOVE THE PREFIX
 
 IMPORT_NAME = "babelwidget"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.backend",
+    f"{IMPORT_NAME}.backend.generic",
     f"{IMPORT_NAME}.backend.pyqt5",
     f"{IMPORT_NAME}.backend.pyqt5.widget",
     f"{IMPORT_NAME}.backend.pyqt6",
     f"{IMPORT_NAME}.backend.pyqt6.widget",
+    f"{IMPORT_NAME}.backend.pyqtx",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
 )
 ENTRY_POINTS = {}
```

