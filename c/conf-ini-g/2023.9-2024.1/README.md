# Comparing `tmp/conf-ini-g-2023.9.tar.gz` & `tmp/conf_ini_g-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-ini-g-2023.9.tar", last modified: Wed Aug 16 15:07:43 2023, max compression
+gzip compressed data, was "conf_ini_g-2024.1.tar", last modified: Mon Apr 15 11:17:02 2024, max compression
```

## Comparing `conf-ini-g-2023.9.tar` & `conf_ini_g-2024.1.tar`

### file list

```diff
@@ -1,108 +1,103 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/
--rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.9/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.590180 conf-ini-g-2023.9/conf_ini_g/
--rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.9/conf_ini_g/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.583513 conf-ini-g-2023.9/conf_ini_g/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.580180 conf-ini-g-2023.9/conf_ini_g/catalog/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.583513 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.583513 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.593513 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/
--rw-r--r--   0 eric      (1000) users      (984)     2529 2023-06-14 07:31:54.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2346 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.596846 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     1965 2023-06-02 15:09:21.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:29.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 14:56:56.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.596846 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/
--rw-r--r--   0 eric      (1000) users      (984)     2679 2023-06-14 07:32:27.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2344 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.600180 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     2010 2023-06-02 15:43:40.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:33.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2059 2023-06-02 14:30:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 15:01:41.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.606846 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3631 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     3814 2023-06-14 08:11:16.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     3859 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/directory.py
--rw-r--r--   0 eric      (1000) users      (984)     3387 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/multitype.py
--rw-r--r--   0 eric      (1000) users      (984)     2222 2023-06-14 07:01:24.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/none.py
--rw-r--r--   0 eric      (1000) users      (984)     6047 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     7923 2023-06-28 15:15:46.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2460 2023-06-14 08:11:16.000000 conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.583513 conf-ini-g-2023.9/conf_ini_g/catalog/specification/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.610180 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     2267 2023-06-06 07:02:20.000000 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     2472 2023-06-06 08:56:40.000000 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     4619 2023-06-06 12:27:27.000000 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/number.py
--rw-r--r--   0 eric      (1000) users      (984)     2929 2023-06-06 09:24:59.000000 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     4295 2023-08-16 15:00:48.000000 conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.610180 conf-ini-g-2023.9/conf_ini_g/extension/
--rw-r--r--   0 eric      (1000) users      (984)     3078 2023-06-05 12:39:31.000000 conf-ini-g-2023.9/conf_ini_g/extension/path.py
--rw-r--r--   0 eric      (1000) users      (984)     3505 2023-06-28 10:57:28.000000 conf-ini-g-2023.9/conf_ini_g/extension/python.py
--rw-r--r--   0 eric      (1000) users      (984)     5534 2023-08-16 14:47:08.000000 conf-ini-g-2023.9/conf_ini_g/extension/string.py
--rw-r--r--   0 eric      (1000) users      (984)     8515 2023-08-16 14:51:22.000000 conf-ini-g-2023.9/conf_ini_g/extension/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.610180 conf-ini-g-2023.9/conf_ini_g/instance/
--rw-r--r--   0 eric      (1000) users      (984)    11085 2023-06-28 14:04:38.000000 conf-ini-g-2023.9/conf_ini_g/instance/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.613513 conf-ini-g-2023.9/conf_ini_g/instance/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3353 2023-06-28 14:13:18.000000 conf-ini-g-2023.9/conf_ini_g/instance/parameter/base.py
--rw-r--r--   0 eric      (1000) users      (984)     4385 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/instance/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     4108 2023-06-14 08:11:16.000000 conf-ini-g-2023.9/conf_ini_g/instance/parameter/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.583513 conf-ini-g-2023.9/conf_ini_g/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.613513 conf-ini-g-2023.9/conf_ini_g/interface/console/
--rw-r--r--   0 eric      (1000) users      (984)     1635 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/interface/console/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     6498 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/interface/console/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.616846 conf-ini-g-2023.9/conf_ini_g/interface/screen/
--rw-r--r--   0 eric      (1000) users      (984)     4500 2023-06-14 07:31:17.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/backend.py
--rw-r--r--   0 eric      (1000) users      (984)    16586 2023-06-28 14:07:17.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.616846 conf-ini-g-2023.9/conf_ini_g/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     5671 2023-08-16 14:41:07.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     7884 2023-06-14 13:10:38.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/parameter/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     8811 2023-06-14 14:12:59.000000 conf-ini-g-2023.9/conf_ini_g/interface/screen/section.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.616846 conf-ini-g-2023.9/conf_ini_g/interface/storage/
--rw-r--r--   0 eric      (1000) users      (984)     6515 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/interface/storage/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.9/conf_ini_g/interface/storage/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.620180 conf-ini-g-2023.9/conf_ini_g/light/
--rw-r--r--   0 eric      (1000) users      (984)     4248 2023-06-29 15:29:36.000000 conf-ini-g-2023.9/conf_ini_g/light/config.py
--rw-r--r--   0 eric      (1000) users      (984)     3764 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/light/conversion.py
--rw-r--r--   0 eric      (1000) users      (984)     2595 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/light/ini.py
--rw-r--r--   0 eric      (1000) users      (984)     2071 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/light/xlsx.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.620180 conf-ini-g-2023.9/conf_ini_g/raw/
--rw-r--r--   0 eric      (1000) users      (984)     4519 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/raw/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.620180 conf-ini-g-2023.9/conf_ini_g/specification/
--rw-r--r--   0 eric      (1000) users      (984)     2820 2023-06-05 12:39:31.000000 conf-ini-g-2023.9/conf_ini_g/specification/base.py
--rw-r--r--   0 eric      (1000) users      (984)     7241 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/specification/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/conf_ini_g/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     2500 2023-06-06 08:53:53.000000 conf-ini-g-2023.9/conf_ini_g/specification/parameter/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     4177 2023-06-14 14:12:58.000000 conf-ini-g-2023.9/conf_ini_g/specification/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     6127 2023-06-26 13:28:55.000000 conf-ini-g-2023.9/conf_ini_g/specification/parameter/type.py
--rw-r--r--   0 eric      (1000) users      (984)     3437 2023-06-28 14:11:16.000000 conf-ini-g-2023.9/conf_ini_g/specification/parameter/unit.py
--rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.9/conf_ini_g/specification/parameter/value.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/conf_ini_g/specification/section/
--rw-r--r--   0 eric      (1000) users      (984)     9488 2023-06-06 15:35:51.000000 conf-ini-g-2023.9/conf_ini_g/specification/section/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.9/conf_ini_g/specification/section/unit.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-08-16 15:02:34.000000 conf-ini-g-2023.9/conf_ini_g/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.593513 conf-ini-g-2023.9/conf_ini_g.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-08-16 15:07:43.000000 conf-ini-g-2023.9/conf_ini_g.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     3454 2023-08-16 15:07:43.000000 conf-ini-g-2023.9/conf_ini_g.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-08-16 15:07:43.000000 conf-ini-g-2023.9/conf_ini_g.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       14 2023-08-16 15:07:43.000000 conf-ini-g-2023.9/conf_ini_g.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2023-08-16 15:07:43.000000 conf-ini-g-2023.9/conf_ini_g.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.586846 conf-ini-g-2023.9/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.9/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.9/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-08-16 15:07:43.630180 conf-ini-g-2023.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6360 2023-06-26 12:16:56.000000 conf-ini-g-2023.9/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/
+-rwx------   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf_ini_g-2024.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4554 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf_ini_g-2024.1/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf_ini_g-2024.1/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf_ini_g-2024.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/
+-rwx------   0 eric      (1000) users      (984)     1597 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/
+-rwx------   0 eric      (1000) users      (984)     3643 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/boolean.py
+-rwx------   0 eric      (1000) users      (984)     5727 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/callable.py
+-rwx------   0 eric      (1000) users      (984)     3833 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/choices.py
+-rwx------   0 eric      (1000) users      (984)    10756 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/collection.py
+-rwx------   0 eric      (1000) users      (984)     4036 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/directory.py
+-rwx------   0 eric      (1000) users      (984)     3616 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/multitype.py
+-rwx------   0 eric      (1000) users      (984)     2212 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/none.py
+-rwx------   0 eric      (1000) users      (984)     6879 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/path.py
+-rwx------   0 eric      (1000) users      (984)     2521 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/text_line.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/catalog/specification/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/
+-rwx------   0 eric      (1000) users      (984)     2701 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/boolean.py
+-rwx------   0 eric      (1000) users      (984)     3007 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/callable.py
+-rwx------   0 eric      (1000) users      (984)     3162 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/choices.py
+-rwx------   0 eric      (1000) users      (984)     4991 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/collection.py
+-rwx------   0 eric      (1000) users      (984)     4823 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/number.py
+-rwx------   0 eric      (1000) users      (984)     3250 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/extension/
+-rwx------   0 eric      (1000) users      (984)     3082 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/path.py
+-rwx------   0 eric      (1000) users      (984)     3731 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/python.py
+-rwx------   0 eric      (1000) users      (984)     2436 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/extension/string.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.416334 conf_ini_g-2024.1/conf_ini_g/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/console/
+-rwx------   0 eric      (1000) users      (984)     7001 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/console/config.py
+-rwx------   0 eric      (1000) users      (984)     1783 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     7519 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/config.py
+-rwx------   0 eric      (1000) users      (984)     1634 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/parameter.py
+-rwx------   0 eric      (1000) users      (984)     1598 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/storage/section.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/config/
+-rwx------   0 eric      (1000) users      (984)     3293 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/action.py
+-rwx------   0 eric      (1000) users      (984)     2471 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/advanced.py
+-rwx------   0 eric      (1000) users      (984)    16998 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/main.py
+-rwx------   0 eric      (1000) users      (984)     4113 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/config/title.py
+-rwx------   0 eric      (1000) users      (984)     1862 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/
+-rwx------   0 eric      (1000) users      (984)     5386 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     2235 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/type.py
+-rwx------   0 eric      (1000) users      (984)     2958 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/interface/window/section/
+-rwx------   0 eric      (1000) users      (984)     4039 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/section/collection.py
+-rwx------   0 eric      (1000) users      (984)     8783 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/interface/window/section/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/light/
+-rwx------   0 eric      (1000) users      (984)     4259 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/config.py
+-rwx------   0 eric      (1000) users      (984)     3763 2024-04-15 11:06:57.000000 conf_ini_g-2024.1/conf_ini_g/light/conversion.py
+-rwx------   0 eric      (1000) users      (984)     2607 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/ini.py
+-rwx------   0 eric      (1000) users      (984)     2102 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/light/xlsx.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/phase/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/generic/
+-rwx------   0 eric      (1000) users      (984)     4025 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/generic/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/
+-rwx------   0 eric      (1000) users      (984)     3294 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/config/
+-rwx------   0 eric      (1000) users      (984)    13255 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/config/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/
+-rwx------   0 eric      (1000) users      (984)     4284 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     3569 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/type.py
+-rwx------   0 eric      (1000) users      (984)     2445 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/unit.py
+-rwx------   0 eric      (1000) users      (984)     1853 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/
+-rwx------   0 eric      (1000) users      (984)     2390 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/controller.py
+-rwx------   0 eric      (1000) users      (984)     6306 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/generic.py
+-rwx------   0 eric      (1000) users      (984)     6543 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/specific.py
+-rwx------   0 eric      (1000) users      (984)     1845 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/specification/section/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/conf_ini_g/phase/typed/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/config/
+-rwx------   0 eric      (1000) users      (984)     7985 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/config/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/
+-rwx------   0 eric      (1000) users      (984)     1936 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/invalid.py
+-rwx------   0 eric      (1000) users      (984)     2833 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/main.py
+-rwx------   0 eric      (1000) users      (984)     2572 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/typed/section/
+-rwx------   0 eric      (1000) users      (984)     2705 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/typed/section/units.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g/phase/untyped/
+-rwx------   0 eric      (1000) users      (984)     1628 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/config.py
+-rwx------   0 eric      (1000) users      (984)     2637 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/parameter.py
+-rwx------   0 eric      (1000) users      (984)     2588 2024-04-15 11:10:03.000000 conf_ini_g-2024.1/conf_ini_g/phase/untyped/section.py
+-rwx------   0 eric      (1000) users      (984)     1616 2024-04-15 11:15:25.000000 conf_ini_g-2024.1/conf_ini_g/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/conf_ini_g.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4554 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2870 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       51 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2024-04-15 11:17:02.000000 conf_ini_g-2024.1/conf_ini_g.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.413001 conf_ini_g-2024.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:17:02.419668 conf_ini_g-2024.1/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf_ini_g-2024.1/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf_ini_g-2024.1/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-15 11:17:02.423001 conf_ini_g-2024.1/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     6607 2023-11-09 15:02:40.000000 conf_ini_g-2024.1/setup.py
```

### Comparing `conf-ini-g-2023.9/PKG-INFO` & `conf_ini_g-2024.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.9
+Version: 2024.1
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
@@ -12,14 +12,19 @@
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+Requires-Dist: babelwidget
+Requires-Dist: issue-manager
+Requires-Dist: openpyxl
+Requires-Dist: rich
+Requires-Dist: str-to-obj
 
 ..
    Copyright CNRS/Inria/UCA
    Contributor(s): Eric Debreuve (since 2021)
 
    eric.debreuve@cnrs.fr
```

### Comparing `conf-ini-g-2023.9/README-COPYRIGHT-utf8.txt` & `conf_ini_g-2024.1/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.9/README-LICENCE-utf8.txt` & `conf_ini_g-2024.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.9/README.rst` & `conf_ini_g-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.9/conf_ini_g/__init__.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,12 +25,18 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-# from conf_ini_g.specification.config import config_t
-# from conf_ini_g.specification.parameter.main import parameter_t
-# from conf_ini_g.specification.section.main import section_t
 
-from conf_ini_g.version import __version__
+from conf_ini_g.interface.constant import STD_ABBREVIATIONS
+
+
+def FormattedName(name: str, separator: str, /) -> str:
+    """"""
+    name_cmps = []
+    for component in name.split(separator):
+        name_cmps.append(STD_ABBREVIATIONS.get(component, component))
+
+    return " ".join(name_cmps).capitalize()
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/text_line.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,30 +25,44 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtCore as core
-import PyQt5.QtGui as visl
-import PyQt5.QtWidgets as wdgt
-
-ALIGNED_HCENTER = core.Qt.AlignmentFlag.AlignHCenter
-ALIGNED_LEFT = core.Qt.AlignmentFlag.AlignLeft
-ALIGNED_RIGHT = core.Qt.AlignmentFlag.AlignRight
-ALIGNED_TOP = core.Qt.AlignmentFlag.AlignTop
-BASE_PALETTE = visl.QPalette.Base
-COLOR_CYAN = visl.QColorConstants.Cyan
-DIALOG_ACCEPTATION = wdgt.QDialog.Accepted
-DIALOG_ACCEPT_OPEN = wdgt.QFileDialog.AcceptOpen
-DIALOG_ACCEPT_SAVE = wdgt.QFileDialog.AcceptSave
-DIALOG_AUTO_OVERWRITE = wdgt.QFileDialog.DontConfirmOverwrite
-DIALOG_MODE_ANY = wdgt.QFileDialog.AnyFile
-DIALOG_MODE_EXISTING_FILE = wdgt.QFileDialog.ExistingFile
-DIALOG_MODE_FOLDER = wdgt.QFileDialog.Directory
-FORMAT_RICH = core.Qt.TextFormat.RichText
-SELECTABLE_TEXT = core.Qt.TextInteractionFlag.TextSelectableByMouse
-SIZE_EXPANDING = wdgt.QSizePolicy.Expanding
-SIZE_FIXED = wdgt.QSizePolicy.Fixed
-SIZE_MINIMUM = wdgt.QSizePolicy.Minimum
-TAB_POSITION_EAST = wdgt.QTabWidget.East
+from __future__ import annotations
+
+import dataclasses as dtcl
+from typing import Any
+
+from babelwidget.main import backend_t
+from babelwidget.main import text_line_h as text_line_wgt_h
+from conf_ini_g.interface.window.parameter.value import value_wgt_a
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class text_line_t(value_wgt_a):
+    library_wgt: text_line_wgt_h
+
+    @classmethod
+    def NewForSpecification(
+        cls,
+        _: Any,
+        backend: backend_t,
+        /,
+    ) -> text_line_t:
+        """"""
+        output = cls(library_wgt=backend.text_line_t())
+        output.SetupValueChangedMessaging(output.library_wgt, "textChanged", backend)
+        return output
+
+    def Assign(self, value: Any | None, _: Any, /) -> None:
+        """"""
+        if value is None:
+            value = ""
+        else:
+            value = str(value)
+        self.library_wgt.setText(value)
+
+    def Text(self) -> str:
+        """"""
+        return self.library_wgt.Text()
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,32 +25,33 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
+import dataclasses as dtcl
+from typing import Any
+from typing import NamedTuple as named_tuple_t
+
+from rich.text import Text as text_t
+
+
+@dtcl.dataclass(init=False, repr=False, eq=False)  # Cannot have __init__ method.
+class controller_t(named_tuple_t):
+    section: str = None
+    parameter: str = None
+    # All controller values are equal in role. However, this one is called primary
+    # because it refers to the parameters of the section, as opposed to the parameters
+    # in the alternatives.
+    primary_value: Any = None
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
-
-
-class event_loop_t(wdgt.QApplication):
-    def Run(self) -> int:
+    def __str__(self) -> str:
         """"""
-        return self.exec_()
+        return text_t.from_markup(self.__rich__()).plain
 
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
+    def __rich__(self) -> str:
+        """"""
+        return (
+            f"[magenta]{type(self).__name__}[/]: "
+            f"[blue]{self.section}.{self.parameter}[/]={self.primary_value}"
+        )
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,24 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
+from conf_ini_g.interface.storage.section import INI_UNIT_SECTION
 
-import PyQt5.QtWidgets as wdgt
 
-
-class button_wgt_t(wdgt.QPushButton):
-    """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.clicked.connect(function)
-
-
-class dot_button_wgt_t(wdgt.QRadioButton):
+def IsUnitSection(section: str, /, *, possibly_fuzzy: bool = False) -> bool:
     """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.toggled.connect(function)
+    if possibly_fuzzy:
+        return section.lower() == INI_UNIT_SECTION.lower()
+    else:
+        return section == INI_UNIT_SECTION
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py` & `conf_ini_g-2024.1/conf_ini_g/light/xlsx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,24 +25,26 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
+from conf_ini_g.extension.path import any_path_h
+from conf_ini_g.phase.untyped.config import ini_config_h
+from openpyxl import load_workbook as WorkbookFromPath
 
-import PyQt5.QtWidgets as wdgt
 
-
-class choice_menu_wgt_t(wdgt.QComboBox):
+def NewConfigFromPath(path: any_path_h, /) -> ini_config_h:
     """"""
+    output = {}
 
-    def Text(self) -> str:
-        return self.currentText()
+    workbook = WorkbookFromPath(filename=path)
+    for name in workbook.sheetnames:
+        sheet = workbook[name]
+        contents = {}
+        for row in tuple(sheet.rows):  # TODO: Why tuple?
+            contents[row[0].value] = row[1].value
 
-    def ItemAt(self, index: int, /) -> str:
-        return self.itemText(index)
+        output[name] = contents
 
-    def SetFunction(self, function: Callable, /) -> None:
-        self.activated.connect(function)
-        # OR: self.currentTextChanged.connect(function)
+    return output
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py` & `conf_ini_g-2024.1/conf_ini_g/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,10 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
+__version__ = "2024.1"
 
-
-class label_wgt_t(wdgt.QLabel):
-    def Text(self) -> str:
-        """"""
-        return self.text()
+# TODO: Callable parameter still a WIP.
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py` & `conf_ini_g-2024.1/conf_ini_g/interface/storage/parameter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,18 +25,10 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
-
-library_wgt_t = wdgt.QWidget
-
-group_wgt_t = wdgt.QGroupBox
-stack_wgt_t = wdgt.QStackedWidget
-tabs_wgt_t = wdgt.QTabWidget
-
-hbox_lyt_t = wdgt.QHBoxLayout
-vbox_lyt_t = wdgt.QVBoxLayout
-grid_lyt_t = wdgt.QGridLayout
+INI_VALUE_ASSIGNMENT = "="
+INI_UNIT_SEPARATOR = ":IN:"
+INI_COMMENT_MARKER = "#"
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,26 +25,21 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtWidgets as wdgt
 
+class missing_required_value_t:
+    TEXT = "MISSING REQUIRED VALUE"
 
-class path_chooser_wgt_t(wdgt.QFileDialog):
-    """"""
-
-    def __init__(self, caption: str, /, *, extension_filter: str = None):
+    def __str__(self) -> str:
         """"""
-        if extension_filter is None:
-            extension_filter = "Any files (*)"
-        super().__init__(caption=caption, filter=extension_filter)
+        return self.__class__.TEXT
 
-    def SelectedFile(self) -> str:
+    def __rich__(self) -> str:
         """"""
-        return self.selectedFiles()[0]
+        return f"[red]{self.__class__.TEXT}[/]"
 
-    def RunAndGetClosingStatus(self) -> int:
-        """"""
-        return self.exec_()
+
+MISSING_REQUIRED_VALUE = missing_required_value_t()
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/none.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -27,23 +27,31 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-import PyQt5.QtWidgets as wdgt
+import dataclasses as dtcl
+from typing import Any
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
+from babelwidget.main import backend_t
+from babelwidget.main import label_h as label_wgt_h
+from conf_ini_g.interface.window.parameter.value import value_wgt_a
 
 
-class scroll_container_t(wdgt.QScrollArea):
-    """"""
+@dtcl.dataclass(repr=False, eq=False)
+class none_wgt_t(value_wgt_a):
+    library_wgt: label_wgt_h
 
     @classmethod
-    def NewForWidget(cls, widget: library_wgt_t, /) -> scroll_container_t:
+    def NewForSpecification(cls, _: Any, backend: backend_t, /) -> none_wgt_t:
         """"""
-        output = cls()
-        output.setWidget(widget)
-        output.setWidgetResizable(True)
+        return cls(library_wgt=backend.label_t("None"))
 
-        return output
+    def Assign(self, _: Any, __: Any, /) -> None:
+        """"""
+        pass
+
+    def Text(self) -> str:
+        """"""
+        return "None"
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py` & `conf_ini_g-2024.1/conf_ini_g/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
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
+from conf_ini_g.version import __version__
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py` & `conf_ini_g-2024.1/conf_ini_g/interface/storage/section.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,32 +25,9 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
 
-from conf_ini_g.catalog.interface.screen.library.pyqt6.widget.main import library_wgt_t
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
+INI_UNIT_SECTION = "UNITS"  # In uppercase
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py` & `conf_ini_g-2024.1/conf_ini_g/extension/string.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,24 +25,41 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
+import textwrap as text
+from typing import Sequence
 
-import PyQt6.QtWidgets as wdgt
 
-
-class button_wgt_t(wdgt.QPushButton):
+def Flattened(string: str, /) -> str:
     """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.clicked.connect(function)
+    return text.dedent(string).replace("\n", "; ")
 
 
-class dot_button_wgt_t(wdgt.QRadioButton):
+def AlignedOnSeparator(
+    string: str | Sequence[str], separator: str, replacement: str, /
+) -> str | tuple[str, ...] | list[str]:
     """"""
-
-    def SetFunction(self, function: Callable, /) -> None:
-        self.toggled.connect(function)
+    if should_return_str := isinstance(string, str):
+        lines = string.splitlines()
+    else:
+        lines = string
+    indices = tuple(_lne.find(separator) for _lne in lines)
+    longest = max(indices)
+
+    output = (
+        (
+            _lne.replace(separator, (longest - _lgt) * " " + replacement, 1)
+            if _lgt > 0
+            else _lne
+        )
+        for _lne, _lgt in zip(lines, indices)
+    )
+    if should_return_str:
+        return "\n".join(output)
+    elif isinstance(string, tuple):
+        return tuple(output)
+    else:
+        return list(output)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/choices.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,27 +25,52 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
+import dataclasses as dtcl
+from typing import Annotated, Sequence
 
-import PyQt6.QtWidgets as wdgt
+from issue_manager import ISSUE_MANAGER
+from str_to_obj import annotation_t
+from str_to_obj.type.hint import annotated_hint_t
 
 
-class choice_menu_wgt_t(wdgt.QComboBox):
-    """"""
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class choices_t(annotation_t):
+    ACCEPTED_TYPES = (str,)
+    options: Sequence[str]
 
-    def Text(self) -> str:
+    def __post_init__(self) -> None:
         """"""
-        return self.currentText()
+        with ISSUE_MANAGER.AddedContextLevel("Choices Annotation"):
+            for option in self.options:
+                if not isinstance(option, str):
+                    ISSUE_MANAGER.Add(
+                        f'Invalid type of option "{option}"',
+                        actual=type(option).__name__,
+                        expected="str",
+                    )
 
-    def ItemAt(self, index: int, /) -> str:
+    @classmethod
+    def NewAnnotatedType(cls, options: Sequence[str], /) -> annotated_hint_t:
         """"""
-        return self.itemText(index)
+        return Annotated[str, cls(tuple(options))]
 
-    def SetFunction(self, function: Callable, /) -> None:
+    def ValueIsCompliant(self, value: str, /) -> list[str]:
         """"""
-        self.activated.connect(function)
-        # OR: self.currentTextChanged.connect(function)
+        issues = annotation_t.ValueIsCompliant(self, value)
+        if issues.__len__() > 0:
+            return issues
+
+        if (self.options.__len__() == 0) or (value in self.options):
+            # Options can be empty for a controlling parameter whose controlled section
+            # has not been specified. In a GUI context, such controlled section should
+            # have been populated programmatically.
+            return []
+
+        options = map(lambda _elm: f'"{_elm}"', self.options)
+        options = " or ".join(options)
+
+        return [f"Invalid choice: Actual={value}; Expected={options}."]
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py` & `conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/invalid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,25 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
 
+class invalid_value_t:
+    """
+    Do not use invalid_value_t = object, for example, otherwise isinstance returns True for anything.
+    """
 
-class label_wgt_t(wdgt.QLabel):
-    def Text(self) -> str:
+    TEXT = "INVALID VALUE"
+
+    def __str__(self) -> str:
+        """"""
+        return self.__class__.TEXT
+
+    def __rich__(self) -> str:
         """"""
-        return self.text()
+        return f"[red]{self.__class__.TEXT}[/]"
+
+
+INVALID_VALUE = invalid_value_t()
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py` & `conf_ini_g-2024.1/conf_ini_g/interface/constant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,18 +25,23 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
 
-library_wgt_t = wdgt.QWidget
+STD_ABBREVIATIONS = {
+    "fct": "function",
+    "mod": "module",
+    "n": "number of",
+    "o": "of",
+    "prm": "parameter",
+    "rng": "range",
+}
 
-group_wgt_t = wdgt.QGroupBox
-stack_wgt_t = wdgt.QStackedWidget
-tabs_wgt_t = wdgt.QTabWidget
 
-hbox_lyt_t = wdgt.QHBoxLayout
-vbox_lyt_t = wdgt.QVBoxLayout
-grid_lyt_t = wdgt.QGridLayout
+SECTION_COLOR = "green"
+PARAMETER_COLOR = "blue"
+
+
+PATH_SELECTOR_WIDTH = 100
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,26 +25,32 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
+import dataclasses as dtcl
 
+from conf_ini_g.phase.specification.parameter.main import parameter_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+from conf_ini_g.phase.untyped.section import STD_UNIT_CONVERSIONS
+from issue_manager import ISSUE_MANAGER
+
+
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class unit_t(parameter_t):
+    def __post_init__(self) -> None:
+        """
+        Unit parameter are never part of a specification. They can appear in INI
+        documents, and are therefore only instantiated programmatically.
+        """
+        self.type = type_t.NewFromTypeHint(float)
+
+        with ISSUE_MANAGER.AddedContextLevel(f'Unit "{self.name}"'):
+            if self.name in STD_UNIT_CONVERSIONS.keys():
+                ISSUE_MANAGER.Add("Redefinition of a standard unit")
 
-class path_chooser_wgt_t(wdgt.QFileDialog):
-    """"""
-
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
+    @property
+    def optional(self) -> bool:
         """"""
-        return self.exec()
+        return True
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,25 +25,30 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+from types import NoneType
+from typing import Sequence
 
-import PyQt6.QtWidgets as wdgt
+from babelwidget.main import backend_t
+from babelwidget.main import dropdown_choice_h as dropdown_choice_wgt_h
+from str_to_obj.type.hint_tree import hint_tree_t
 
-from conf_ini_g.catalog.interface.screen.library.pyqt6.widget.main import library_wgt_t
 
-
-class scroll_container_t(wdgt.QScrollArea):
+def TypeSelector(
+    hints: Sequence[hint_tree_t], backend: backend_t, /
+) -> dropdown_choice_wgt_h:
     """"""
+    output = backend.dropdown_choice_t()
 
-    @classmethod
-    def NewForWidget(cls, widget: library_wgt_t, /) -> scroll_container_t:
-        """"""
-        output = cls()
-        output.setWidget(widget)
-        output.setWidgetResizable(True)
+    for hint in hints:
+        # Here, it is important that hint trees cannot have an OR-node with an OR-node
+        # child so that hint.type has a valid value.
+        if hint is NoneType:
+            output.addItem("None")
+        else:
+            output.addItem(hint.type.__name__)
 
-        return output
+    return output
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py` & `conf_ini_g-2024.1/conf_ini_g/phase/untyped/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,14 +25,9 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt6.QtWidgets as wdgt
 
-
-class text_wgt_t(wdgt.QLineEdit):
-    def Text(self) -> str:
-        """"""
-        return self.text().strip()
+ini_config_h = dict[str, dict[str, str]]  # Without value interpretation
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/boolean.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/boolean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,72 +28,68 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+from typing import Any
 
-from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
-from conf_ini_g.interface.screen.backend import (
-    backend_t,
-    choices_dots_wgt_h,
-    library_wgt_h,
-)
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
+from babelwidget.main import backend_t
+from babelwidget.main import base_h as library_wgt_h
+from babelwidget.main import radio_choice_h as radio_choice_wgt_h
+from conf_ini_g.catalog.specification.annotation.boolean import boolean_t
+from conf_ini_g.interface.window.parameter.value import value_wgt_a
+from conf_ini_g.phase.specification.parameter.type import type_t
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class boolean_wgt_t:
+@dtcl.dataclass(repr=False, eq=False)
+class boolean_wgt_t(value_wgt_a):
     library_wgt: library_wgt_h
-    true_btn: choices_dots_wgt_h = dtcl.field(init=False, default=None)
+    true_btn: radio_choice_wgt_h | None = dtcl.field(init=False, default=None)
+    false_btn: radio_choice_wgt_h | None = dtcl.field(init=False, default=None)
 
     @classmethod
-    def NewWithDetails(
+    def NewForSpecification(
         cls,
-        value: bool | None,
-        value_type: type_t | boolean_t | None,
+        stripe: type_t | boolean_t | None,
         backend: backend_t,
-        _: parameter_t | None,
         /,
     ) -> boolean_wgt_t:
-        """
-        If value_type does not contain the necessary details, an exclamation point is added to the default values.
-        """
-        output = cls(library_wgt=backend.library_wgt_t())
+        """"""
+        output = cls(library_wgt=backend.base_t())
 
-        if value is None:
-            value = True
+        output.SetupValueChangedMessaging(output.true_btn, "released", backend)
 
-        if value_type is None:
-            labels = None
+        if stripe is None:
+            annotation = None
+        elif isinstance(stripe, type_t):
+            annotation = stripe.FirstAnnotationWithType(boolean_t)
+        else:
+            annotation = stripe
+        if annotation is None:
+            labels = ("True", "False")
         else:
-            if isinstance(value_type, type_t):
-                annotation = value_type.FirstAnnotationWithAttribute("mode")
-            else:
-                annotation = value_type
-            if annotation is None:
-                labels = None
-            else:
-                labels = getattr(annotation.mode, "value", None)
-        if labels is None:
-            labels = ("True!", "False!")
-
-        true_btn = backend.dot_button_wgt_t(labels[0], parent=output.library_wgt)
-        false_btn = backend.dot_button_wgt_t(labels[1], parent=output.library_wgt)
-        true_btn.setChecked(value)
-        false_btn.setChecked(not value)
+            labels = getattr(annotation.mode, "value", None)
+
+        true_btn = backend.radio_choice_t(labels[0], parent=output.library_wgt)
+        false_btn = backend.radio_choice_t(labels[1], parent=output.library_wgt)
 
         output.true_btn = true_btn
+        output.false_btn = false_btn
 
         layout = backend.hbox_lyt_t()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(true_btn)
         layout.addWidget(false_btn)
         output.library_wgt.setLayout(layout)
 
         return output
 
+    def Assign(self, value: bool, _: Any, /) -> None:
+        """"""
+        self.true_btn.setChecked(value)
+        self.false_btn.setChecked(not value)
+
     def Text(self) -> str:
         """"""
         return str(self.true_btn.isChecked())
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/choices.py` & `conf_ini_g-2024.1/conf_ini_g/phase/untyped/parameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,80 +25,43 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+from conf_ini_g.interface.storage.parameter import INI_UNIT_SEPARATOR
 
-import dataclasses as dtcl
-from typing import Any
 
-from conf_ini_g.catalog.specification.parameter.choices import choices_t
-from conf_ini_g.interface.screen.backend import backend_t, choices_list_wgt_h
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class choices_wgt_t:
-    library_wgt: choices_list_wgt_h
-
-    @classmethod
-    def NewWithDetails(
-        cls,
-        value: str | None,
-        value_type: type_t | choices_t | None,
-        backend: backend_t,
-        _: parameter_t | None,
-        /,
-    ) -> choices_wgt_t:
-        """
-        If value_type does not contain the necessary details, the initial value (if valid) is the only choice, or a unique
-        default choice ending with an exclamation point is added.
-        """
-        output = cls(library_wgt=backend.choice_menu_wgt_t())
-
-        value_is_valid = isinstance(value, str)
-        if value_is_valid:
-            value = value.strip()
-
-        if value_type is None:
-            choices = _DefaultChoices(value, value_is_valid)
-        else:
-            if isinstance(value_type, type_t):
-                annotation = value_type.FirstAnnotationWithAttribute("options")
-            else:
-                annotation = value_type
-            if annotation is None:
-                choices = _DefaultChoices(value, value_is_valid)
-            else:
-                choices = annotation.options
-
-        for choice in choices:
-            output.library_wgt.addItem(choice)
-        if value_is_valid:
-            output.library_wgt.setCurrentText(value)
-        else:
-            output.library_wgt.setCurrentIndex(0)
-
-        return output
-
-    def __getattr__(self, attribute: str, /) -> Any:
-        """
-        E.g., used for "SetFunction".
-        """
-        try:
-            output = super(choices_wgt_t, self).__getattr__(attribute)
-        except AttributeError:
-            output = getattr(self.library_wgt, attribute)
+def ValueUnitAndComment(
+    value_w_unit_w_comment: str,
+    comment_marker: str,
+    /,
+) -> tuple[str, str | None, str | None]:
+    """"""
+    value_w_unit, comment = _Pieces(value_w_unit_w_comment, comment_marker)
+    if (comment is not None) and (comment.__len__() == 0):
+        comment = None
+
+    value_as_str, unit = _Pieces(value_w_unit, INI_UNIT_SEPARATOR, from_left=False)
+    # if unit.__len__() == 0, do not make it None so that an invalid unit error is noticed later on
 
-        return output
+    return value_as_str, unit, comment
 
 
-def _DefaultChoices(value: str, value_is_valid: bool, /) -> tuple[str]:
+def _Pieces(
+    combined: str, separator: str, /, *, from_left: bool = True
+) -> tuple[str, str | None]:
     """"""
-    if value_is_valid:
-        return (value,)
+    if from_left:
+        where_separator = combined.find(separator)
     else:
-        return ("Default!",)
+        where_separator = combined.rfind(separator)
+
+    if where_separator != -1:
+        left = combined[:where_separator].strip()
+        right = combined[(where_separator + separator.__len__()) :].strip()
+    else:
+        left = combined
+        right = None
+
+    return left, right
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/directory.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/directory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -26,64 +26,66 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from pathlib import Path as path_t
-from types import NoneType
-from typing import Type
+from types import NoneType, UnionType
 
-from conf_ini_g.catalog.interface.screen.parameter.boolean import boolean_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.choices import choices_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.none import none_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.path import path_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.sequence import sequence_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.text import default_entry_wgt_t
-from conf_ini_g.catalog.specification.parameter.choices import choices_t
-from conf_ini_g.catalog.specification.parameter.number import number_t
-from conf_ini_g.extension.type import hint_node_t
-from conf_ini_g.interface.screen.backend import library_wgt_h
-from conf_ini_g.specification.parameter.annotation import annotation_t
-from conf_ini_g.specification.parameter.type import type_t
-
-_TYPE_WIDGET_TRANSLATOR: dict[type, Type[library_wgt_h]] = {
+from babelwidget.main import base_h as library_wgt_h
+from conf_ini_g.catalog.interface.window.parameter.boolean import boolean_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.callable import callable_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.choices import choices_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.collection import collection_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.none import none_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.path import path_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.text_line import text_line_t
+from conf_ini_g.catalog.specification.annotation.callable import callable_t
+from conf_ini_g.catalog.specification.annotation.choices import choices_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+from str_to_obj import annotation_t
+from str_to_obj.type.hint_tree import hint_tree_t
+
+# Widgets can be mapped from types or annotations. Since annotations are more specific
+# than types, they must be placed first to ensure they get a chance to be selected.
+_TYPE_WIDGET_TRANSLATOR: dict[type, type[library_wgt_h]] = {
+    # Annotations
+    callable_t: callable_wgt_t,
+    choices_t: choices_wgt_t,
+    # Types
     NoneType: none_wgt_t,
+    UnionType: choices_wgt_t,
     bool: boolean_wgt_t,
-    choices_t: choices_wgt_t,
-    int: default_entry_wgt_t,
-    list: sequence_wgt_t,
-    number_t: default_entry_wgt_t,
+    float: text_line_t,
+    int: text_line_t,
+    list: collection_wgt_t,
     path_t: path_wgt_t,
-    set: sequence_wgt_t,
-    tuple: sequence_wgt_t,
+    set: collection_wgt_t,
+    str: text_line_t,
+    tuple: collection_wgt_t,
 }
 
 
-def WidgetTypeForType(type_: type_t | hint_node_t, /) -> Type[library_wgt_h]:
+def ValueWidgetTypeForType(stripe: type_t | hint_tree_t, /) -> type[library_wgt_h]:
     """"""
-    if is_type_t := isinstance(type_, type_t):
-        base_hint = type_.base_hint
-    else:
-        base_hint = type_.type
+    base_hint = stripe.type
+    nnts = stripe.all_annotations
 
     for registered_type, widget_type in _TYPE_WIDGET_TRANSLATOR.items():
-        if (base_hint is registered_type) or (
-            is_type_t
-            and any(
-                issubclass(type(_nnt), registered_type) for _nnt in type_.annotations
-            )
+        if (base_hint is registered_type) or any(
+            issubclass(type(_nnt), registered_type) for _nnt in nnts
         ):
             return widget_type
 
-    return default_entry_wgt_t
+    return text_line_t
 
 
 def RegisterNewTranslation(
-    new_type: type | annotation_t, widget_type: Type[library_wgt_h], /
+    new_type: type | annotation_t, widget_type: type[library_wgt_h], /
 ) -> None:
     """"""
     if new_type in _TYPE_WIDGET_TRANSLATOR:
         # Raising an exception is adapted here since it is a developer-oriented function
         raise ValueError(
             f'{new_type.__name__}: Type already registered with "{_TYPE_WIDGET_TRANSLATOR[new_type]}" '
             f"in type-to-widget translations."
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/multitype.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/multitype.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -30,65 +30,67 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
 from typing import Any, Sequence
 
-from conf_ini_g.catalog.interface.screen.parameter.directory import WidgetTypeForType
-from conf_ini_g.extension.type import hint_node_t
-from conf_ini_g.interface.screen.backend import (
-    backend_t,
-    choices_list_wgt_h,
-    library_wgt_h,
-    stacked_wgt_h,
+from babelwidget.main import backend_t
+from babelwidget.main import base_h as library_wgt_h
+from babelwidget.main import dropdown_choice_h as dropdown_choice_wgt_h
+from babelwidget.main import stack_h as stack_wgt_h
+from conf_ini_g.catalog.interface.window.parameter.directory import (
+    ValueWidgetTypeForType,
 )
+from str_to_obj.type.hint_tree import hint_tree_t
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
+@dtcl.dataclass(repr=False, eq=False)
 class multitype_wgt_t:
-    library_wgt: stacked_wgt_h
-    controller_wgt: choices_list_wgt_h
-    values: tuple[library_wgt_h] = ()
+    hints: Sequence[hint_tree_t]
+    library_wgt: stack_wgt_h
+    type_selection_wgt: dropdown_choice_wgt_h
+    values: tuple[library_wgt_h] | None = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewForHints(
         cls,
-        value: Any,
-        hints: Sequence[hint_node_t],
-        controller: choices_list_wgt_h,
+        hints: Sequence[hint_tree_t],
+        controller: dropdown_choice_wgt_h,
         backend: backend_t,
         /,
     ) -> multitype_wgt_t:
         """"""
-        value_stack = backend.stack_wgt_t()
-        output = cls(library_wgt=value_stack, controller_wgt=controller)
+        value_stack = backend.stack_t()
+        controller.SetFunction(value_stack.setCurrentIndex)
+
+        output = cls(
+            hints=hints, library_wgt=value_stack, type_selection_wgt=controller
+        )
 
         values = []
-        initial_index = 0
         for t_idx, hint in enumerate(hints):
-            if isinstance(value, hint.type):
-                initial_index = t_idx
-                initial_value = value
-            else:
-                initial_value = None
-            widget_type = WidgetTypeForType(hint)
-            value_wgt = widget_type.NewWithDetails(
-                initial_value,
+            widget_type = ValueWidgetTypeForType(hint)
+            value_wgt = widget_type.NewForSpecification(
                 hint,
                 backend,
-                None,
             )
             values.append(value_wgt)
             value_stack.addWidget(value_wgt.library_wgt)
-
         output.values = tuple(values)
-        controller.SetFunction(value_stack.setCurrentIndex)
 
-        value_stack.setCurrentIndex(initial_index)
         value_stack.setSizePolicy(backend.SIZE_EXPANDING, backend.SIZE_FIXED)
 
         return output
 
+    def Assign(self, value: Any, stripe: Any, /) -> None:
+        """"""
+        type_idx = 0
+        for t_idx, hint in enumerate(self.hints):
+            if isinstance(value, hint.type):
+                type_idx = t_idx
+        self.type_selection_wgt.setCurrentIndex(type_idx)
+        self.values[type_idx].Assign(value, stripe)
+
     def Text(self) -> str:
         """"""
-        return self.values[self.controller_wgt.currentIndex()].Text()
+        return self.values[self.type_selection_wgt.currentIndex()].Text()
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/none.py` & `conf_ini_g-2024.1/conf_ini_g/phase/typed/section/units.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,31 +25,43 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+from conf_ini_g.interface.storage.parameter import INI_COMMENT_MARKER
+from conf_ini_g.interface.storage.section import INI_UNIT_SECTION
+from conf_ini_g.phase.specification.config.main import config_t as specification_t
+from conf_ini_g.phase.untyped.parameter import ValueUnitAndComment
+from conf_ini_g.phase.untyped.section import STD_UNIT_CONVERSIONS
+
+
+def InitialUnits(specification: specification_t, /) -> dict[str, float]:
+    """
+    Specification can override standard units.
+    """
+    units = dict(STD_UNIT_CONVERSIONS)
+    if INI_UNIT_SECTION in specification:
+        units.update(specification[INI_UNIT_SECTION].AsDict())
+
+    return units
+
+
+def UpdateUnits(
+    units: dict[str, float], name: str, value: str, /
+) -> tuple[float | None, list[str]]:
+    """"""
+    issues = []
+
+    if name in STD_UNIT_CONVERSIONS:
+        return None, [f'Standard unit "{name}" cannot be overriden.']
+
+    value, *_ = ValueUnitAndComment(value, INI_COMMENT_MARKER)
+    try:
+        value = float(value)
+    except ValueError:
+        return None, [f"/{INI_UNIT_SECTION}.{name}/ Invalid value: {value}."]
 
-import dataclasses as dtcl
-from typing import Any
+    units[name] = value
 
-from conf_ini_g.interface.screen.backend import backend_t, label_wgt_h
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class none_wgt_t:
-    library_wgt: label_wgt_h
-
-    @classmethod
-    def NewWithDetails(
-        cls, _: Any, __: type_t | None, backend: backend_t, ___: parameter_t | None, /
-    ) -> none_wgt_t:
-        """"""
-        return cls(library_wgt=backend.label_wgt_t("None"))
-
-    def Text(self) -> str:
-        """"""
-        return "None"
+    return value, issues
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/path.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/callable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,142 +28,129 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+import inspect as nspt
+import typing as h
+from importlib import util as mprt
 from pathlib import Path as pl_path_t
 
-from conf_ini_g.catalog.specification.parameter.path import path_t
-from conf_ini_g.interface.screen.backend import backend_t, library_wgt_h, text_wgt_h
-from conf_ini_g.interface.screen.parameter.path_chooser import (
-    NewSelectedInputDocument,
-    NewSelectedOutputDocument,
-    document_selection_fct_h,
-)
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-
-PATH_SELECTOR_WIDTH = 100
+from babelwidget.main import backend_t
+from babelwidget.main import base_h as library_wgt_h
+from conf_ini_g.catalog.interface.window.parameter.choices import choices_wgt_t
+from conf_ini_g.catalog.interface.window.parameter.path import path_wgt_t
+from conf_ini_g.catalog.specification.annotation.callable import callable_t
+from conf_ini_g.catalog.specification.annotation.path import path_t as path_annotation_t
+from conf_ini_g.interface.window.parameter.value import value_wgt_a
+from conf_ini_g.phase.specification.parameter.type import type_t
 
 
 @dtcl.dataclass(repr=False, eq=False)
-class path_wgt_t:
-    """
-    Cannot use slots (weak reference issue).
-    """
-
+class callable_wgt_t(value_wgt_a):
     library_wgt: library_wgt_h
     backend: backend_t
-    target_type: path_t.TARGET_TYPE = dtcl.field(init=False, default=None)
-    path: text_wgt_h = dtcl.field(init=False, default=None)
-    _NewSelectedDocument: document_selection_fct_h = dtcl.field(
-        init=False, default=None
-    )
+    kind: h.Literal["class", "function"]
+    path: path_wgt_t | None = dtcl.field(init=False, default=None)
+    choices: choices_wgt_t = dtcl.field(init=False, default=None)
 
     @classmethod
-    def NewWithDetails(
+    def NewForSpecification(
         cls,
-        value: pl_path_t | None,
-        value_type: type_t | path_t | None,
+        stripe: type_t | callable_t,
         backend: backend_t,
-        _: parameter_t | None,
         /,
-        *,
-        editable: bool = True,
-    ) -> path_wgt_t:
-        """
-        If value_type does not contain the necessary details, the target type is set to any and considered as input, and
-        the selection button label ends with an exclamation point.
-        """
-        output = cls(library_wgt=backend.library_wgt_t(), backend=backend)
-
-        if value is None:
-            value = ""
-        else:
-            value = str(value)
-
-        default_parameters = (path_t.TARGET_TYPE.any, True, True)
-        if value_type is None:
-            target_type, is_input, misses_details = default_parameters
-        else:
-            if isinstance(value_type, type_t):
-                annotation = value_type.FirstAnnotationWithAttribute(
-                    ("target_type", "is_input")
-                )
-            else:
-                annotation = value_type
+    ) -> callable_wgt_t:
+        """"""
+        if isinstance(stripe, type_t):
+            annotation = stripe.FirstAnnotationWithType(callable_t)
             if annotation is None:
-                target_type, is_input, misses_details = default_parameters
-            else:
-                target_type = annotation.target_type
-                is_input = annotation.is_input
-                misses_details = False
-
-        output.target_type = target_type
-        if is_input:
-            output._NewSelectedDocument = NewSelectedInputDocument
+                raise ValueError("No catalog provided.")
         else:
-            output._NewSelectedDocument = NewSelectedOutputDocument
+            annotation = stripe
+        kind = annotation.kind
+        choices = annotation.choices
+        allow_external = annotation.allow_external
+
+        choices_wgt = choices_wgt_t.NewForSpecification(
+            choices,
+            backend,
+        )
 
-        if target_type is path_t.TARGET_TYPE.document:
-            target_type_icon = "🗋"
-        elif target_type is path_t.TARGET_TYPE.folder:
-            target_type_icon = "📂"
-        else:
-            target_type_icon = "📂🗋"
-        if is_input:
-            selector_color = "green"
-        else:
-            selector_color = "red"
-        selector_label = f"...{target_type_icon}..."
-        if misses_details:
-            selector_label += "!"
-        if editable:
-            path = backend.text_wgt_t(value, parent=output.library_wgt)
-        else:
-            path = backend.label_wgt_t(value, parent=output.library_wgt)
-        path_selector = backend.button_wgt_t(selector_label, parent=output.library_wgt)
-        path_selector.SetFunction(output.SelectDocument)
-
-        output.path = path
-
-        path_selector.setStyleSheet(f"color: {selector_color};")
-        path_selector.setFixedWidth(PATH_SELECTOR_WIDTH)
-
-        layout = backend.hbox_lyt_t()
-        layout.setContentsMargins(0, 0, 0, 0)
-        layout.addWidget(path)
-        layout.addWidget(path_selector)
-        output.library_wgt.setLayout(layout)
+        if allow_external:
+            output = cls(
+                library_wgt=backend.base_t(),
+                backend=backend,
+                kind=kind,
+            )
+        else:
+            output = cls(
+                library_wgt=choices_wgt,
+                backend=backend,
+                kind=kind,
+            )
+        output.choices = choices_wgt
+
+        # TODO: Check that this is the correct emitter and signal.
+        output.SetupValueChangedMessaging(output.choices, "released", backend)
+
+        if allow_external:
+            path_wgt = path_wgt_t.NewForSpecification(
+                path_annotation_t(
+                    target_type=path_annotation_t.TARGET_TYPE.document, is_input=True
+                ),
+                backend,
+                PostAssignmentFunction=output._UpdateChoices,
+            )
+            output.path = path_wgt
+
+            layout = backend.hbox_lyt_t()
+            layout.setContentsMargins(0, 0, 0, 0)
+            layout.addWidget(path_wgt.library_wgt)
+            layout.addWidget(choices_wgt.library_wgt)
+            output.library_wgt.setLayout(layout)
 
         return output
 
-    def Text(self) -> str:
+    def _UpdateChoices(self, path: pl_path_t, /) -> None:
         """"""
-        return self.path.Text()
+        self.choices.library_wgt.clear()
 
-    def SelectDocument(self) -> None:
-        """"""
-        current_path = self.Text()
-        current_doc = pl_path_t(current_path).resolve()
+        spec = mprt.spec_from_file_location(path.stem, path)
+        module = spec.loader.load_module(spec.name)
+        if self.kind == "class":
+            condition = nspt.isclass
+        else:
+            condition = nspt.isfunction
+
+        for name, _ in nspt.getmembers(module, condition):
+            if not name.startswith("_"):
+                self.choices.library_wgt.addItem(name)
+
+    def SetFunction(self, function: h.Callable, /) -> None:
+        """
+        self.activated.connect(function): Responds only to GUI interaction, not
+        programmatic change.
+        """
+        self.choices.currentIndexChanged.connect(function)
 
-        if self.target_type is path_t.TARGET_TYPE.document:
-            title = "Select File"
-        elif self.target_type is path_t.TARGET_TYPE.folder:
-            title = "Select Folder"
+    def Assign(self, value: str, _: h.Any, /) -> None:
+        """"""
+        if callable_t.SEPARATOR in value:
+            path, choice = value.split(callable_t.SEPARATOR)
+            self.path.Assign(pl_path_t(path), None)
         else:
-            title = "Select File or Folder"
+            choice = value
+        self.choices.Assign(choice, None)
 
-        selection = self._NewSelectedDocument(
-            title,
-            title,
-            self.backend,
-            mode=self.target_type,
-            start_folder=current_doc.parent,
-            initial_selection=current_doc,
-        )
-        if selection is None:
-            return
+    def Text(self) -> str:
+        """"""
+        if self.path is None:
+            return self.choices.Text()
+
+        path = self.path.Text()
+        if path.__len__() > 0:
+            return f"{path}{callable_t.SEPARATOR}{self.choices.Text()}"
 
-        self.path.setText(str(selection))
+        return self.choices.Text()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/interface/screen/parameter/text.py` & `conf_ini_g-2024.1/conf_ini_g/phase/typed/parameter/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,44 +25,46 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
-import dataclasses as dtcl
 from typing import Any
 
-from conf_ini_g.interface.screen.backend import backend_t, text_wgt_h
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class default_entry_wgt_t:
-    library_wgt: text_wgt_h
-
-    @classmethod
-    def NewWithDetails(
-        cls,
-        value: Any | None,
-        _: type_t | None,
-        backend: backend_t,
-        __: parameter_t | None,
-        /,
-    ) -> default_entry_wgt_t:
-        """"""
-        output = cls(library_wgt=backend.text_wgt_t())
-
-        if value is None:
-            value = ""
-        else:
-            value = str(value)
-        output.library_wgt.setText(value)
-
-        return output
-
-    def Text(self) -> str:
-        """"""
-        return self.library_wgt.Text()
+from conf_ini_g.phase.specification.parameter.type import type_t
+from conf_ini_g.phase.typed.parameter.invalid import INVALID_VALUE, invalid_value_t
+from conf_ini_g.phase.typed.parameter.unit import ConvertedValue
+
+
+def TypedValue(
+    value: str,
+    expected_type: type_t,
+    /,
+    *,
+    unit: str | None = None,
+    units: dict[str, int | float | invalid_value_t] = None,
+) -> tuple[Any, list[str]]:
+    """
+    With unit consumed or not.
+    """
+    final_value, issues = expected_type.InterpretedValueOf(value)
+    if issues.__len__() > 0:
+        return INVALID_VALUE, [f"{value}: Invalid value: {', '.join(issues)}"]
+
+    if (units is None) or (unit is None):
+        return final_value, []
+
+    conversion_factor = units.get(unit, None)
+    if conversion_factor is None:
+        return INVALID_VALUE, [f"{unit}: Missing unit definition."]
+    if conversion_factor is INVALID_VALUE:
+        return INVALID_VALUE, [f"{unit}: Invalid unit value."]
+
+    converted, unconverted = ConvertedValue(final_value, conversion_factor)
+    if unconverted.__len__() > 0:
+        unconverted = ", ".join(unconverted)
+        return INVALID_VALUE, [
+            f"{unconverted}: Value(s) do(es) not support unit conversion."
+        ]
+
+    return converted, []
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/boolean.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/boolean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -27,30 +27,43 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from enum import Enum as enum_t
-from typing import Annotated
+from typing import Annotated, ClassVar
 
-from conf_ini_g.extension.type import annotated_hint_t
-from conf_ini_g.specification.parameter.annotation import annotation_t
+from str_to_obj import annotation_t
+from str_to_obj.type.hint import annotated_hint_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class boolean_t(annotation_t):
     class MODE(enum_t):
         # Always list true value first
         true_false = ("True", "False")
         yes_no = ("Yes", "No")
         on_off = ("On", "Off")
 
+    _MODES: ClassVar[tuple[str, ...]] = tuple(_elm for _elm in MODE.__members__.keys())
+
+    ACCEPTED_TYPES = (bool,)
     mode: enum_t = MODE.true_false
 
     @classmethod
-    def NewAnnotatedType(cls, mode: enum_t = None) -> annotated_hint_t:
+    def NewAnnotatedType(
+        cls, /, *, mode: enum_t | str | None = None
+    ) -> annotated_hint_t:
         """"""
         if mode is None:
             mode = cls.MODE.true_false
+        elif isinstance(mode, str):
+            if mode in cls._MODES:
+                mode = cls.MODE[mode].value
+            else:
+                valid = " or ".join(cls._MODES)
+                raise ValueError(
+                    f"Invalid boolean mode: Actual={mode}; Expected={valid}."
+                )
 
         return Annotated[bool, cls(mode=mode)]
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/choices.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/callable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -26,38 +26,50 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Annotated, Sequence
+from typing import Annotated, ClassVar, Literal, Sequence
 
-from conf_ini_g.extension.type import annotated_hint_t
-from conf_ini_g.specification.parameter.annotation import annotation_t
+from conf_ini_g.catalog.specification.annotation.choices import choices_t
+from str_to_obj import annotation_t
+from str_to_obj.type.hint import annotated_hint_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
-class choices_t(annotation_t):
-    options: Sequence[str] = None
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class callable_t(annotation_t):
+    ACCEPTED_TYPES = (str,)
+    DUMMY_ENTRY: ClassVar[str] = "Dummy entry"
+    SEPARATOR: ClassVar[str] = ":"
+    kind: Literal["class", "function"]
+    choices: choices_t | None = None
+    allow_external: bool = False
 
     @classmethod
-    def NewAnnotatedType(cls, options: Sequence[str], /) -> annotated_hint_t:
+    def NewAnnotatedType(
+        cls,
+        /,
+        *,
+        kind: Literal["class", "function"] = "function",
+        catalog: Sequence[str] | bool | None = None,
+        allow_external: bool = False,
+    ) -> annotated_hint_t:
         """"""
-        return Annotated[str, cls(tuple(options))]
-
-    def Issues(self) -> list[str]:
-        """"""
-        output = []
-
-        for option in self.options:
-            if not isinstance(option, str):
-                output.append(
-                    f"{type(option).__name__}: Invalid type of option {option} "
-                    f"in {self}; Expected=str"
+        if catalog is None:
+            annotation = cls(kind=kind, allow_external=allow_external)
+        elif isinstance(catalog, bool):
+            if catalog:
+                annotation = cls(
+                    kind=kind,
+                    choices=choices_t((cls.DUMMY_ENTRY,)),
+                    allow_external=allow_external,
                 )
+            else:
+                annotation = cls(kind=kind, allow_external=allow_external)
+        else:
+            annotation = cls(
+                kind=kind, choices=choices_t(catalog), allow_external=allow_external
+            )
 
-        return output
-
-    def ValueIsCompliant(self, value: str, /) -> bool:
-        """"""
-        return value in self.options
+        return Annotated[str, annotation]
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/number.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/number.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -26,96 +26,95 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Annotated, ClassVar
+from typing import ClassVar
 
-from conf_ini_g.extension.type import annotated_hint_t
-from conf_ini_g.specification.parameter.annotation import annotation_t
+from issue_manager import ISSUE_MANAGER
+from str_to_obj import annotation_t
 
 number_h = int | float
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class number_t(annotation_t):
     INFINITY_NEG: ClassVar[float] = -float("inf")
     INFINITY_POS: ClassVar[float] = float("inf")
     INFINITE_PRECISION: ClassVar[float] = 0.0
 
+    ACCEPTED_TYPES = (int, float)
     min: number_h = INFINITY_NEG
     max: number_h = INFINITY_POS
     min_inclusive: bool = True
     max_inclusive: bool = True
     precision: number_h = INFINITE_PRECISION
 
-    @classmethod
-    def NewAnnotatedType(cls, py_type: type, /, **kwargs) -> annotated_hint_t:
+    def __post_init__(self) -> None:
         """"""
-        if py_type in (int, float):
-            return Annotated[py_type, cls(**kwargs)]
+        stripe = self.__class__
 
-        raise TypeError(f"{py_type}: Invalid Python type; " f"Expected=int or float.")
+        with ISSUE_MANAGER.AddedContextLevel("Number Annotation"):
+            if (self.min != stripe.INFINITY_NEG) and not isinstance(
+                self.min, number_h.__args__
+            ):
+                ISSUE_MANAGER.Add(
+                    f"Invalid type for min value {self.min}",
+                    actual=type(self.min).__name__,
+                    expected=number_h,
+                )
+            if (self.max != stripe.INFINITY_POS) and not isinstance(
+                self.max, number_h.__args__
+            ):
+                ISSUE_MANAGER.Add(
+                    f"Invalid type for max value {self.max}",
+                    actual=type(self.max).__name__,
+                    expected=number_h,
+                )
+            if (self.precision != stripe.INFINITE_PRECISION) and not isinstance(
+                self.precision, number_h.__args__
+            ):
+                ISSUE_MANAGER.Add(
+                    f"Invalid type for precision {self.precision}",
+                    actual=type(self.precision).__name__,
+                    expected=number_h,
+                )
+            if self.precision < 0:
+                ISSUE_MANAGER.Add(f"Invalid, negative precision {self.precision}")
+            if (self.min > self.max) or (
+                (self.min == self.max)
+                and not (self.min_inclusive and self.max_inclusive)
+            ):
+                if self.min_inclusive:
+                    opening = "["
+                else:
+                    opening = "]"
+                if self.max_inclusive:
+                    closing = "]"
+                else:
+                    closing = "["
+                ISSUE_MANAGER.Add(
+                    f"Empty value interval {opening}{self.min},{self.max}{closing}"
+                )
 
-    def Issues(self) -> list[str]:
+    def ValueIsCompliant(self, value: number_h, /) -> list[str]:
         """"""
-        output = []
+        issues = annotation_t.ValueIsCompliant(self, value)
+        if issues.__len__() > 0:
+            return issues
 
-        self_class = self.__class__
-        if (self.min != self_class.INFINITY_NEG) and not isinstance(
-            self.min, number_h.__args__
-        ):
-            output.append(
-                f"{type(self.min)}: Invalid type for min value {self.min} "
-                f"in {self}; Expected={number_h}"
-            )
-        if (self.max != self_class.INFINITY_POS) and not isinstance(
-            self.max, number_h.__args__
-        ):
-            output.append(
-                f"{type(self.max)}: Invalid type for max value {self.max} "
-                f"in {self}; Expected={number_h}"
-            )
-        if (self.precision != self_class.INFINITE_PRECISION) and not isinstance(
-            self.precision, number_h.__args__
-        ):
-            output.append(
-                f"{type(self.precision)}: Invalid type for precision {self.precision} "
-                f"in {self}; Expected={number_h}"
-            )
-        if self.precision < 0:
-            output.append(f"{self.precision}: Negative precision in {self}")
-        if (self.min > self.max) or (
-            (self.min == self.max) and not (self.min_inclusive and self.max_inclusive)
-        ):
-            if self.min_inclusive:
-                opening = "["
-            else:
-                opening = "]"
-            if self.max_inclusive:
-                closing = "]"
-            else:
-                closing = "["
-            output.append(
-                f"{opening}{self.min},{self.max}{closing}: Empty value interval in {self}"
-            )
-
-        return output
-
-    def ValueIsCompliant(self, value: number_h, /) -> bool:
-        """"""
         if self.min <= value <= self.max:
             if ((value == self.min) and not self.min_inclusive) or (
                 (value == self.max) and not self.max_inclusive
             ):
-                return False
+                return [f"{value}: Value outside prescribed interval."]
 
             if (self.precision != self.__class__.INFINITE_PRECISION) and (
                 self.precision * int(value / self.precision) != value
             ):
-                return False
+                return [f"{value}: Value of higher precision than the prescribed one."]
 
-            return True
+            return []
         else:
-            return False
+            return [f"{value}: Value outside prescribed interval."]
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/path.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -30,49 +30,60 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from enum import Enum as enum_t
 from pathlib import Path as pl_path_t
 from typing import Annotated
 
-from conf_ini_g.extension.type import annotated_hint_t
-from conf_ini_g.specification.parameter.annotation import annotation_t
+from str_to_obj import annotation_t
+from str_to_obj.type.hint import annotated_hint_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class path_t(annotation_t):
-    """
-    Existence and target type validation are left to main program. Hence, ValueIsCompliant
-    is not overriden.
-    """
-
     class TARGET_TYPE(enum_t):
         document = 1
         folder = 2
         any = 3
 
+    ACCEPTED_TYPES = (pl_path_t,)
     target_type: enum_t
+    # TODO: Change this into input, output, or both.
     is_input: bool
 
     @classmethod
     def NewAnnotatedType(
         cls, target_type: TARGET_TYPE, is_input: bool, /
     ) -> annotated_hint_t:
         """"""
         return Annotated[pl_path_t, cls(target_type=target_type, is_input=is_input)]
 
-    def ValueIsCompliant(self, value: pl_path_t | None, /) -> bool:
-        """"""
+    def ValueIsCompliant(self, value: pl_path_t | None, /) -> list[str]:
+        """
+        None: Unspecified path.
+        """
+        issues = annotation_t.ValueIsCompliant(self, value)
+        if issues.__len__() > 0:
+            return issues
+
+        if value is None:
+            return []
+
         if not self.is_input:
-            return True
+            return []
 
-        if (value is not None) and value.exists():
+        if value.exists():
             if self.target_type is path_t.TARGET_TYPE.any:
-                return value.is_file() or value.is_dir()
+                if value.is_file() or value.is_dir():
+                    return []
+                else:
+                    return [f"{value}: Not a valid file or folder."]
 
             if (self.target_type is path_t.TARGET_TYPE.document) and value.is_file():
-                return True
+                return []
 
             if (self.target_type is path_t.TARGET_TYPE.folder) and value.is_dir():
-                return True
+                return []
 
-        return False
+        return [
+            f"{value}: Non-existent file or folder, or file for folder, or folder for file."
+        ]
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/catalog/specification/parameter/sequence.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/specification/annotation/collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -26,89 +26,95 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Annotated, Any, ClassVar, Sequence
+from typing import Any, ClassVar, Sequence
 
-from conf_ini_g.extension.type import annotated_hint_t, any_hint_h
-from conf_ini_g.specification.parameter.annotation import annotation_t
-from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+from issue_manager import ISSUE_MANAGER
+from str_to_obj import annotation_t
+from str_to_obj.type.hint import any_hint_h
 
 
-@dtcl.dataclass(repr=False, eq=False)
-class sequence_t(annotation_t):
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class collection_t(annotation_t):
+    # Items of any type but None
     ANY_ITEMS_TYPES: ClassVar[Any | tuple[Any, ...]] = Any
     ANY_LENGTH: ClassVar[tuple[int, ...]] = (0,)
 
-    # Any=Value of any type but None
-    items_types: any_hint_h | tuple[any_hint_h, ...] | type_t | tuple[
-        type_t, ...
-    ] = ANY_ITEMS_TYPES
+    ACCEPTED_TYPES = (list, set, tuple)
+    items_types: any_hint_h | tuple[any_hint_h, ...] | type_t | tuple[type_t, ...] = (
+        ANY_ITEMS_TYPES
+    )
     lengths: int | tuple[int, ...] = ANY_LENGTH
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """"""
+        original_item_types = self.items_types
+        original_lengths = self.lengths
+
         if isinstance(self.items_types, Sequence):
-            self.items_types = tuple(
-                type_t.NewFromType(_typ) for _typ in self.items_types
-            )
-        else:
-            self.items_types = type_t.NewFromType(self.items_types)
+            items_types = []
+            for stripe in self.items_types:
+                if isinstance(stripe, type_t):
+                    items_types.append(stripe)
+                else:
+                    items_types.append(type_t.NewFromTypeHint(stripe))
+            self.items_types = items_types
+        elif not isinstance(self.items_types, type_t):
+            self.items_types = type_t.NewFromTypeHint(self.items_types)
 
         if isinstance(self.lengths, int):
             self.lengths = (self.lengths,)
         else:
             self.lengths = tuple(sorted(self.lengths))
 
-    @classmethod
-    def NewAnnotatedType(
-        cls,
-        sequence_type: type,
-        items_types: any_hint_h | tuple[any_hint_h | None, ...] = ANY_ITEMS_TYPES,
-        lengths: tuple[int, ...] = ANY_LENGTH,
-    ) -> annotated_hint_t:
-        """"""
-        if sequence_type in (list, set, tuple):
-            return Annotated[
-                sequence_type, cls(items_types=items_types, lengths=lengths)
-            ]
-
-        raise ValueError(
-            f"{sequence_type.__name__}: Invalid sequence type; "
-            f"Expected=list, set or tuple."
-        )
-
-    def Issues(self) -> list[str]:
-        """"""
-        output = []
-
-        if self.lengths != self.__class__.ANY_LENGTH:
-            for length in self.lengths:
-                if (not isinstance(length, int)) or (length <= 0):
-                    output.append(
-                        f"{length}: Invalid sequence length in {self}; "
-                        f"Expected=strictly positive integer"
+        with ISSUE_MANAGER.AddedContextLevel("Collection Annotation"):
+            if isinstance(self.items_types, Sequence):
+                if max(self.lengths) > self.items_types.__len__():
+                    ISSUE_MANAGER.Add(
+                        f'Allowed length(s) ("{original_lengths}") must not exceed '
+                        f"the length of the item types sequence "
+                        f'("{original_item_types}")'
                     )
+            if self.lengths != self.__class__.ANY_LENGTH:
+                for length in self.lengths:
+                    if (not isinstance(length, int)) or (length < 0):
+                        ISSUE_MANAGER.Add(
+                            f"Invalid length in {self.lengths}",
+                            actual=length,
+                            expected="strictly positive integer",
+                        )
 
-        return output
-
-    def ValueIsCompliant(self, value: tuple, /) -> bool:
+    def ValueIsCompliant(self, value: tuple, /) -> list[str]:
         """"""
+        issues = annotation_t.ValueIsCompliant(self, value)
+        if issues.__len__() > 0:
+            return issues
+
         if (self.lengths != self.__class__.ANY_LENGTH) and (
             value.__len__() not in self.lengths
         ):
-            return False
+            return [
+                f"{value}: Sequence of invalid length; "
+                f"Expected={' or '.join(map(str, self.lengths))}."
+            ]
 
         if isinstance(self.items_types, Sequence):
             if value.__len__() > self.items_types.__len__():
-                return False
-
-            return all(
-                _typ.ValueIsCompliant(_elm)
-                for _typ, _elm in zip(self.items_types, value)
-            )
+                return [
+                    f"{value}: Sequence too long. Expected=At most {self.items_types.__len__()} element(s)."
+                ]
+
+            output = []
+            for stripe, element in zip(self.items_types, value):
+                output.extend(stripe.ValueIsCompliant(element))
+            return output
 
-        type_ = self.items_types
-        return all(type_.ValueIsCompliant(_elm) for _elm in value)
+        stripe: type_t = self.items_types
+        output = []
+        for element in value:
+            output.extend(stripe.ValueIsCompliant(element))
+        return output
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/extension/path.py` & `conf_ini_g-2024.1/conf_ini_g/extension/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -32,47 +32,47 @@
 from pathlib import Path as path_t
 
 any_path_h = str | path_t
 
 
 def ValidateInputPath(
     path: path_t, /, *, should_raise_on_error: bool = False
-) -> str | None:
+) -> list[str]:
     """"""
     if not path.exists():
         issue = f"{path}: Non-existing path."
         if should_raise_on_error:
             raise FileNotFoundError(issue)
         else:
-            return issue
+            return [issue]
 
     if path.is_dir():
         issue = f"{path}: Path is a folder; Expected=Path to an existing file."
         if should_raise_on_error:
             raise IsADirectoryError(issue)
         else:
-            return issue
+            return [issue]
 
-    return None
+    return []
 
 
 def ValidateOutputPath(
     path: path_t,
     /,
     *,
     should_overwrite: bool = False,
     should_raise_on_error: bool = False,
-) -> str | None:
+) -> list[str]:
     """"""
     if path.exists() and not should_overwrite:
         issue = f"{path}: Path exists and overwriting is not allowed."
         if should_raise_on_error:
             raise PermissionError(issue)
         else:
-            return issue
+            return [issue]
 
     if path.is_dir():
         if should_overwrite:
             document_qualification = ""
             document_property = ", existing or not"
         else:
             document_qualification = "non-existing "
@@ -80,10 +80,10 @@
         issue = (
             f"{path}: Path is a folder; "
             f"Expected=Path to a {document_qualification}file{document_property}."
         )
         if should_raise_on_error:
             raise IsADirectoryError(issue)
         else:
-            return issue
+            return [issue]
 
-    return None
+    return []
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/extension/python.py` & `conf_ini_g-2024.1/conf_ini_g/extension/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -33,45 +33,49 @@
 import inspect as nspt
 import sys as sstm
 from pathlib import Path as path_t
 
 
 def SpecificationPath(element: object, /, *, relative_to_home: bool = True) -> str:
     """"""
-    found = []
-    for module in sstm.modules.copy().values():
-        for attribute in dir(module):
-            # It can happen that "attribute" ends up not being an attribute of "module",
-            # for example with "single" in scipy.linalg.matfuncs. Hence, the default
-            # value in getattr. The getattr call can even fail, for example with
-            # "Viewer" in napari. Hence the try-expect.
-            try:
-                value = getattr(module, attribute, None)
-            except:
-                value = None
-            if (value is not None) and (value is element):
-                code = nspt.getsource(module)
-                tree = bstr.parse(code)
-                is_imported = False
-                for node in bstr.walk(tree):
-                    if isinstance(node, bstr.ImportFrom):
-                        for alias in node.names:
-                            if (
-                                (alias.asname is None) and (alias.name == attribute)
-                            ) or (
-                                (alias.asname is not None)
-                                and (alias.asname == attribute)
-                            ):
-                                is_imported = True
-                                break
-                if not is_imported:
-                    path = module.__file__
-                    if relative_to_home:
-                        path = str(path_t(path).relative_to(path_t.home()))
-                    found.append(path)
+    try:
+        found = [nspt.getfile(element)]
+    except TypeError:
+        found = []
+    if found.__len__() == 0:
+        for module in sstm.modules.copy().values():
+            for attribute in dir(module):
+                # It can happen that "attribute" ends up not being an attribute of
+                # "module", for example with "single" in scipy.linalg.matfuncs. Hence,
+                # the default value in getattr. The getattr call can even fail, for
+                # example with "Viewer" in napari. Hence the try-expect.
+                try:
+                    value = getattr(module, attribute, None)
+                except:
+                    value = None
+                if (value is not None) and (value is element):
+                    code = nspt.getsource(module)
+                    tree = bstr.parse(code)
+                    is_imported = False
+                    for node in bstr.walk(tree):
+                        if isinstance(node, bstr.ImportFrom):
+                            for alias in node.names:
+                                if (
+                                    (alias.asname is None) and (alias.name == attribute)
+                                ) or (
+                                    (alias.asname is not None)
+                                    and (alias.asname == attribute)
+                                ):
+                                    is_imported = True
+                                    break
+                    if not is_imported:
+                        path = module.__file__
+                        if relative_to_home:
+                            path = str(path_t(path).relative_to(path_t.home()))
+                        found.append(path)
 
     if (n_found := found.__len__()) == 0:
         output = "Unidentified specification file"
     elif n_found == 1:
         output = found[0]
     else:
         alternatives = ", ".join(found)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/instance/config.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/config/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,248 +25,319 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
 import dataclasses as dtcl
 import textwrap as text
 from typing import Any, Sequence
 
+from conf_ini_g.catalog.specification.annotation.callable import callable_t
+from conf_ini_g.catalog.specification.annotation.choices import choices_t
+from conf_ini_g.extension.python import SpecificationPath
+from conf_ini_g.interface.storage.parameter import INI_UNIT_SEPARATOR
+from conf_ini_g.interface.storage.section import INI_UNIT_SECTION
+from conf_ini_g.phase.specification.parameter.main import parameter_t
+from conf_ini_g.phase.specification.parameter.type import ANY_TYPE, type_t
+from conf_ini_g.phase.specification.parameter.unit import unit_t
+from conf_ini_g.phase.specification.parameter.value import MISSING_REQUIRED_VALUE
+from conf_ini_g.phase.specification.section.controller import controller_t
+from conf_ini_g.phase.specification.section.generic import section_t
+from conf_ini_g.phase.specification.section.specific import (
+    any_section_h,
+    controlled_section_t,
+    free_section_t,
+    parameters_t,
+)
+from conf_ini_g.phase.specification.section.unit import IsUnitSection
+from issue_manager import ISSUE_MANAGER
 from rich.text import Text as text_t
-
-from conf_ini_g.extension.path import any_path_h, path_t
-from conf_ini_g.extension.string import AlignedOnSeparator
-from conf_ini_g.extension.type import TypeAsRichStr
-from conf_ini_g.instance.parameter.main import instance_t
-from conf_ini_g.instance.parameter.unit import unit_instance_t
-from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-from conf_ini_g.raw.config import ini_config_h, raw_config_h
-from conf_ini_g.specification.config import config_t as specification_t
-from conf_ini_g.specification.parameter.unit import STD_UNIT_CONVERSIONS, unit_t
-from conf_ini_g.specification.parameter.value import MISSING_REQUIRED_VALUE
-from conf_ini_g.specification.section.main import controller_t
-from conf_ini_g.specification.section.unit import UNIT_SECTION, IsUnitSection
+from str_to_obj import ObjectFromStr
+from str_to_obj.interface.console import TypeAsRichStr
+from str_to_obj.type.hint import any_hint_h
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class config_t(dict[str, dict[str, instance_t | unit_instance_t]]):
-    specification: specification_t
-    ini_path: path_t | None = None
-
-    @classmethod
-    def NewFromINIConfig(
-        cls,
-        ini_config: ini_config_h,
-        specification: specification_t,
-        /,
-        *,
-        path: any_path_h = None,
-    ) -> tuple[config_t, list[str], Sequence[tuple[str, str]]]:
-        """"""
-        config = cls(specification=specification)
-
-        if path is not None:
-            config.ini_path = path_t(path)
-
-        issues, for_deferred_check = config._InstantiateFromINIConfig(ini_config)
-        config._ManageDefaults()
+class config_t(list[any_section_h]):
+    sections: dtcl.InitVar[Sequence[section_t]]
+    path: str = None
 
-        return config, issues, for_deferred_check
+    def __post_init__(self, sections: Sequence[section_t], /) -> None:
+        """
+        Raising exceptions is adapted here since execution cannot proceed without a
+        valid specification.
+        """
+        specific = []
+        for section in sections:
+            as_dict = dict(
+                (_elm.name, getattr(section, _elm.name))
+                for _elm in dtcl.fields(section)
+            )
+            if section.controller is None:
+                del as_dict["controller"]
+                del as_dict["alternatives"]
+                section = free_section_t(**as_dict)
+            else:
+                section = controlled_section_t(**as_dict)
+            specific.append(section)
 
-    def _InstantiateFromINIConfig(
-        self, ini_config: ini_config_h, /
-    ) -> tuple[list[str], Sequence[tuple[str, str]]]:
-        """"""
-        issues = []
-        for_deferred_check = []
+        self.extend(specific)
+        self.path = SpecificationPath(sections)
 
-        for section_name, parameters in ini_config.items():
-            if section_name not in self:
-                self[section_name] = {}
-
-            is_specified = section_name in self.specification
-            if (not is_specified) and IsUnitSection(section_name):
-                self.specification.AddUnitSection()
-                is_specified = True
-
-            if is_specified:
-                section_spec = self.specification[section_name]
-                for name, value in parameters.items():
-                    if name in section_spec:
-                        parameter_spec = section_spec[name]
-                    elif section_spec.is_growable:
-                        parameter_spec = section_spec.AddUnspecifiedParameter(name)
-                        for_deferred_check.append((section_name, name))
-                    else:
-                        parameter_spec = None
-                        issues.append(
-                            f"{section_name}.{name}: Attempt to add an unspecified "
-                            f"parameter to a section accepting none."
-                        )
-                    if parameter_spec is not None:
-                        if isinstance(parameter_spec, unit_t):
-                            instance = unit_instance_t()
-                        else:
-                            instance = instance_t()
-                        instance.SetStrValue(value, INI_COMMENT_MARKER)
-                        self[section_name][name] = instance
-            elif IsUnitSection(section_name, possibly_fuzzy=True):
-                issues.append(
-                    f"{section_name}: Unit section must respect the following case "
-                    f'"{UNIT_SECTION}".'
-                )
-            else:
-                issues.append(
-                    f"{section_name}: Invalid section; "
-                    f"Expected={self.specification.section_names}."
-                )
+        for section in specific:
+            if isinstance(section, free_section_t):
+                continue
 
-        return issues, for_deferred_check
+            controller = section.controller
+            if self.GetController(controller).type is ANY_TYPE:
+                choices = choices_t.NewAnnotatedType(section.controlling_values)
+                self.GetController(controller).type = type_t.NewFromTypeHint(choices)
 
-    def _ManageDefaults(self) -> None:
-        """"""
-        for section_spec in self.specification:
-            # Leave here, otherwise parameter_spec.name not in self[section_spec.name]
-            # below might fail.
-            if section_spec.name not in self:
-                self[section_spec.name] = {}
-
-            for parameter_spec in section_spec.all_parameters:
-                if parameter_spec.name not in self[section_spec.name]:
-                    if parameter_spec.optional:
-                        instance = instance_t(value=parameter_spec.default)
-                        self[section_spec.name][parameter_spec.name] = instance
-                    else:
-                        self[section_spec.name][
-                            parameter_spec.name
-                        ] = MISSING_REQUIRED_VALUE
+        _SignalIssues(self)
+        ISSUE_MANAGER.Report(with_time=True, how="rich")
 
-    def GetValueOfController(self, controller: controller_t, /) -> Any:
+    def AddUnitSection(self) -> None:
         """"""
-        return self[controller.section][controller.parameter].value
-
-    def AsRawConfig(self) -> tuple[raw_config_h, list[str]]:
+        section = free_section_t(
+            name=INI_UNIT_SECTION,
+            definition="Unit definitions",
+            description=f"Units can be used in any other section "
+            f"to specify a parameter value as follows: "
+            f"numerical_value{INI_UNIT_SEPARATOR}unit, e.g., 1.5'mm.",
+            basic=True,
+            optional=True,
+            category=INI_UNIT_SECTION,
+            is_growable=True,
+        )
+        self.append(section)
+
+    def AddPluginParameter(
+        self,
+        section: str | any_section_h,
+        name: str,
+        /,
+        *,
+        definition: str = "Programmatic plugin parameter",
+        description: str = "This parameter is not part of the specification. "
+        'It was added programmatically in a "plugin" way.',
+        basic: bool = True,
+        stripe: any_hint_h | type_t = None,
+        default: Any = MISSING_REQUIRED_VALUE,
+        controlling_value: str = None,
+    ) -> None:
         """
-        Units are interpreted
+        See definition and description above.
         """
-        raw_config = {}
-        issues = []
-
-        unit_conversions = dict(STD_UNIT_CONVERSIONS)
-        if UNIT_SECTION in self.specification:
-            for unit_spec in self.specification[UNIT_SECTION]:
-                unit_name = unit_spec.name
-                expected_type = unit_spec.type
-                instance = self[UNIT_SECTION][unit_name]
-                if instance is MISSING_REQUIRED_VALUE:
-                    issues.append(f"{unit_name}: Missing required unit.")
-                else:
-                    unit_conversions[unit_name] = instance.TypedValue(expected_type)[0]
+        if isinstance(section, str):
+            section = self[section]
 
-        for section_spec in self.specification:
-            raw_section = {}
-
-            if (controller := section_spec.controller) is None:
-                parameters = section_spec
-            else:
-                controller_value = self[controller.section][controller.parameter].value
-                parameters = section_spec.ActiveParameters(controller_value)
-            for parameter_spec in parameters:
-                instance = self[section_spec.name][parameter_spec.name]
-                if instance is MISSING_REQUIRED_VALUE:
-                    value = None
-                    current_issues = ["Missing required parameter."]
-                else:
-                    value, current_issues = instance.TypedValue(
-                        parameter_spec.type, units=unit_conversions
-                    )
-
-                if current_issues.__len__() > 0:
-                    issues.extend(
-                        f"[{section_spec.name}.{parameter_spec.name}] {_iss}"
-                        for _iss in current_issues
-                    )
-                else:
-                    raw_section[parameter_spec.name] = value
+        parameter = parameter_t(
+            name=name,
+            definition=definition,
+            description=description,
+            basic=basic,
+            type=stripe,
+            default=default,
+        )
+        self._AddParameter(
+            section, parameter, controlling_value, config_t.AddPluginParameter.__name__
+        )
+
+    def AddRuntimeParameter(
+        self,
+        section: str | any_section_h,
+        name: str,
+        value: str | float,
+        /,
+        *,
+        controlling_value: str = None,
+    ) -> parameter_t:
+        """
+        See definition and description below.
+        The existence of such a method is justified by the fact that the parameter
+        created can be a "normal" parameter or a unit depending on the section.
 
-            raw_config[section_spec.name] = raw_section
+        value: float if unit.
 
-        return raw_config, issues
+        /!\ Cannot deal with str values with units.
+        """
+        if isinstance(section, str):
+            section = self[section]
 
-    def AsINIConfig(self) -> ini_config_h:
+        if IsUnitSection(section.name):
+            parameter_or_unit_t = unit_t
+            basic = True
+            converted = value
+            stripe = None  # Correctly set by the constructor.
+        else:
+            parameter_or_unit_t = parameter_t
+            basic = section.basic
+            converted, _ = ObjectFromStr(value)
+            stripe = type(converted)
+        definition = "Programmatic runtime parameter"
+        description = (
+            "This parameter is not part of the specification. "
+            "It was added programmatically because it was found in the INI document, "
+            "or passed as a command-line argument."
+        )
+        parameter = parameter_or_unit_t(
+            name=name,
+            definition=definition,
+            description=description,
+            basic=basic,
+            type=stripe,
+            default=converted,  # Just a trick to prevent error if basic is False.
+        )
+        self._AddParameter(
+            section, parameter, controlling_value, config_t.AddRuntimeParameter.__name__
+        )
+
+        return parameter
+
+    def _AddParameter(
+        self,
+        section: any_section_h,
+        parameter: parameter_t,
+        controlling_value: str,
+        caller: str,
+        /,
+    ) -> None:
         """"""
-        output = {}
-
-        for section_name, section in self.items():
-            section_spec = self.specification[section_name]
-            if (controller := section_spec.controller) is None:
-                raw_section = {_p_nme: _prm.Text() for _p_nme, _prm in section.items()}
+        if not section.is_growable:
+            raise RuntimeError(
+                f"{section.name}.{parameter.name}: "
+                f"Attempt to add an unspecified parameter to a section accepting none."
+            )
+
+        if isinstance(section, free_section_t):
+            section.append(parameter)
+            return
+
+        controller = section.controller
+        if controlling_value is None:
+            raise ValueError(
+                f"{caller}: A Controlling value must be passed for parameter "
+                f"{section.name}.{parameter.name}."
+            )
+
+        if controller.primary_value is None:
+            # controller_t is immutable, so it must be re-created.
+            section.controller = controller_t(
+                section=controller.section,
+                parameter=controller.parameter,
+                primary_value=controlling_value,
+            )
+            controller = section.controller
+            section[controlling_value] = parameters_t((parameter,))
+            should_update_controller_choices = True
+        elif controlling_value in section:
+            section[controlling_value].append(parameter)
+            should_update_controller_choices = False
+        else:
+            section[controlling_value] = parameters_t((parameter,))
+            should_update_controller_choices = True
+
+        if should_update_controller_choices:
+            nnts = self.GetController(controller).type.annotations
+            if nnts.__len__() > 0:
+                first_annotation = nnts[0]
             else:
-                controller_value = self.GetValueOfController(controller)
-                raw_section = {
-                    _p_spec.name: section[_p_spec.name].Text()
-                    for _p_spec in section_spec.ActiveParameters(controller_value)
-                }
+                first_annotation = None
+            if (first_annotation is None) or isinstance(first_annotation, choices_t):
+                choices = choices_t.NewAnnotatedType(section.controlling_values)
+                new_type = type_t.NewFromTypeHint(choices)
+            else:  # Must be callable_t.
+                callable_ = callable_t.NewAnnotatedType(
+                    kind=first_annotation.kind,
+                    catalog=section.controlling_values,
+                    allow_external=first_annotation.allow_external,
+                )
+                new_type = type_t.NewFromTypeHint(callable_)
+            self.GetController(controller).type = new_type
 
-            output[section_name] = raw_section
+    @property
+    def section_names(self) -> Sequence[str]:
+        """"""
+        return tuple(_sct.name for _sct in self)
 
-        return output
+    def GetController(self, controller: controller_t, /) -> parameter_t:
+        """"""
+        return self[controller.section][controller.parameter]
 
-    def Issues(self) -> list[str]:
+    def __contains__(self, key: str, /) -> bool:
         """"""
-        output = self.specification.Issues()
+        return any(_elm.name == key for _elm in self)
 
-        valid_units = list(STD_UNIT_CONVERSIONS.keys())
-        if UNIT_SECTION in self.specification:
-            valid_units.extend(_unt.name for _unt in self.specification[UNIT_SECTION])
-
-        for section in self.specification:
-            section_name = section.name
-
-            issues = []
-            for parameter in section:
-                if (instance := self[section.name].get(parameter.name)) is not None:
-                    issues.extend(
-                        f"[{section.name}.{parameter.name}] {_iss}"
-                        for _iss in instance.Issues()
-                    )
-                    # Unit validation cannot be done at the parameter level since the
-                    # unit section is needed.
-                    if ((unit := getattr(instance, "unit", None)) is not None) and (
-                        unit not in valid_units
-                    ):
-                        issues.append(
-                            f"{unit}: Invalid unit of parameter "
-                            f"{section_name}.{parameter.name}"
-                        )
+    def __getitem__(self, key: str, /) -> any_section_h:
+        """"""
+        for section in self:
+            if section.name == key:
+                return section
 
-            output.extend(issues)
+        raise KeyError(f"{key}: Not a section of config.")
 
-        return output
+    def AsDict(self) -> dict[str, dict[str, Any]]:
+        """"""
+        return {_sct.name: _sct.AsDict() for _sct in self}
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
         output = [
-            "[grey50]--- Specification[/]",
             TypeAsRichStr(self),
-            f"    [blue]ini_path[/]={self.ini_path}"
-            f"[yellow]:{type(self.ini_path).__name__}[/]",
-            text.indent(self.specification.__rich__(), "    "),
-            "[grey50]--- Instance[/]",
+            f"    [blue]path[/]={self.path}" f"[yellow]:{type(self.path).__name__}[/]",
         ]
 
-        for section_name, section in self.items():
-            output.append(f"{section_name}:")
-            for parameter_name, parameter in section.items():
-                output.append(f"    {parameter_name}@:@{parameter.__rich__()}")
-
-        output = AlignedOnSeparator(output, "@:@", ": ")
+        for section in self:
+            output.append(text.indent(section.__rich__(), "    "))
 
         return "\n".join(output)
+
+
+def _SignalIssues(self: config_t, /) -> None:
+    """"""
+    with ISSUE_MANAGER.AddedContextLevel(f'Specification "{self.path}"'):
+        if self.__len__() == 0:
+            ISSUE_MANAGER.Add(f"Empty specification")
+            return
+
+        names = self.section_names
+        if names.__len__() > set(names).__len__():
+            ISSUE_MANAGER.Add("Repeated section names")
+
+        for section in self:
+            if isinstance(section, controlled_section_t):
+                controller = section.controller
+                if controller.section not in self:
+                    ISSUE_MANAGER.Add(
+                        f"Unspecified parameter "
+                        f'"{controller.section}.{controller.parameter}" declared as '
+                        f'controller of section "{section.name}"'
+                    )
+                else:
+                    controller_section = self[controller.section]
+                    if isinstance(controller_section, controlled_section_t):
+                        ISSUE_MANAGER.Add(
+                            f'Section "{controller.section}" of parameter '
+                            f'"{controller.parameter}", which controls section '
+                            f'"{section.name}", is itself controlled'
+                        )
+                    if controller.parameter not in controller_section:
+                        ISSUE_MANAGER.Add(
+                            f"Unspecified parameter "
+                            f'"{controller.section}.{controller.parameter}" declared '
+                            f'as controller of section "{section.name}"'
+                        )
+                    else:
+                        controller_section: free_section_t
+                        controller_parameter = controller_section[controller.parameter]
+                        if controller_parameter.optional:
+                            ISSUE_MANAGER.Add(
+                                f"Optional parameter "
+                                f'"{controller.section}.{controller.parameter}" '
+                                f'declared as controller of section "{section.name}"'
+                            )
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/instance/parameter/base.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/value.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,84 +25,56 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+from __future__ import annotations
+
 import dataclasses as dtcl
 from abc import ABC as abstract_class_t
 from abc import abstractmethod
-from typing import Any
+from typing import Any, Callable
 
-from rich.text import Text as text_t
+from babelwidget.main import backend_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+from str_to_obj.type.annotation import annotation_t
 
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import INVALID_VALUE, invalid_value_t
 
+class _do_not_set_value:
+    pass
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class base_t(abstract_class_t):
-    value: str = None  # From INI document or interfaces
-    comment: str = None
 
-    @abstractmethod
-    def SetStrValue(
-        self,
-        value_w_unit_w_comment: str | Any,
-        comment_marker: str,
-        /,
-        *,
-        unit: str = None,
-    ) -> None:
-        """"""
-        ...
+DO_NOT_SET_VALUE = _do_not_set_value()
 
-    @abstractmethod
-    def TypedValue(
-        self,
-        expected_type: type_t,
-        /,
-        *,
-        units: dict[str, int | float | invalid_value_t] = None,
-    ) -> tuple[Any, list[str]]:
-        """"""
-        ...
 
-    @abstractmethod
-    def Text(self) -> str:
-        """"""
-        ...
+@dtcl.dataclass(repr=False, eq=False)
+class value_wgt_a(abstract_class_t):
+    _AcknowledgeValueChange: Callable | None = dtcl.field(init=False, default=None)
 
-    def Issues(self) -> list[str]:
+    def SetupValueChangedMessaging(
+        self, messenger: Any, message: str, backend: backend_t, /
+    ) -> None:
         """"""
-        if self.value is INVALID_VALUE:
-            return ["Invalid value"]
-
-        return []
+        backend.CreateMessageCanal(messenger, message, self.AcknowledgeValueChange)
 
-    def __str__(self) -> str:
+    def SetAcknowledgeValueChangeFunction(self, Function: Callable, /) -> None:
         """"""
-        return text_t.from_markup(self.__rich__()).plain
+        self._AcknowledgeValueChange = Function
 
-    def __rich__(self) -> str:
+    def AcknowledgeValueChange(self) -> None:
         """"""
-        return self.Text()
+        if self._AcknowledgeValueChange is not None:
+            self._AcknowledgeValueChange()
 
+    @classmethod
+    @abstractmethod
+    def NewForSpecification(
+        cls, stripe: type_t | annotation_t | None, backend: backend_t
+    ) -> value_wgt_a: ...
 
-def Pieces(
-    combined: str, separator: str, /, *, from_left: bool = True
-) -> tuple[str, str | None]:
-    """"""
-    if from_left:
-        where_separator = combined.find(separator)
-    else:
-        where_separator = combined.rfind(separator)
-
-    if where_separator != -1:
-        left = combined[:where_separator].strip()
-        right = combined[(where_separator + separator.__len__()) :].strip()
-    else:
-        left = combined
-        right = None
+    @abstractmethod
+    def Assign(self, value: Any, stripe: type_t | annotation_t | None, /) -> None: ...
 
-    return left, right
+    @abstractmethod
+    def Text(self) -> str: ...
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/instance/parameter/main.py` & `conf_ini_g-2024.1/conf_ini_g/phase/generic/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,95 +25,93 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
-from typing import Any
+from typing import Literal, get_args
 
-from conf_ini_g.instance.parameter.base import Pieces, base_t
-from conf_ini_g.instance.parameter.unit import ConvertedValue
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
-from conf_ini_g.specification.parameter.value import INVALID_VALUE, invalid_value_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class instance_t(base_t):
-    unit: str = None
-
-    def SetStrValue(
-        self,
-        value_w_unit_w_comment: str | Any,
-        comment_marker: str,
-        /,
-        *,
-        unit: str = None,
-    ) -> None:
-        """"""
-        value_as_str, inline_unit, comment = _ValueUnitAndComment(
-            value_w_unit_w_comment, comment_marker
-        )
-        if unit is None:
-            unit = inline_unit
+from conf_ini_g.extension.string import Flattened
+from conf_ini_g.interface.constant import PARAMETER_COLOR, SECTION_COLOR
+from conf_ini_g.phase.typed.config.main import typed_config_h
+from conf_ini_g.phase.untyped.config import ini_config_h
+
+any_dict_config_h = ini_config_h | typed_config_h
+color_modes_h = Literal["rich", "html", None]
 
-        self.value = value_as_str
-        self.unit = unit
-        self.comment = comment
-
-    def TypedValue(
-        self,
-        expected_type: type_t,
-        /,
-        *,
-        units: dict[str, int | float | invalid_value_t] = None,
-    ) -> tuple[Any, list[str]]:
-        """
-        With unit consumed or not.
-        """
-        final_value, success = expected_type.InterpretedValueOf(self.value)
-
-        if success:
-            if (units is None) or ((unit := self.unit) is None):
-                return final_value, []
-
-            conversion_factor = units.get(unit, None)
-            if conversion_factor is None:
-                return INVALID_VALUE, [f"{unit}: Missing unit definition."]
-            if conversion_factor is INVALID_VALUE:
-                return INVALID_VALUE, [f"{unit}: Invalid unit value."]
-
-            converted, unconverted = ConvertedValue(final_value, conversion_factor)
-            if unconverted.__len__() > 0:
-                unconverted = ", ".join(unconverted)
-                return INVALID_VALUE, [
-                    f"{unconverted}: Value(s) do(es) not support unit conversion."
-                ]
-
-            return converted, []
-
-        return INVALID_VALUE, [f"{self.value}: Invalid value."]
-
-    def Text(self) -> str:
-        """"""
-        if self.unit is None:
-            return str(self.value)  # str: Only useful when default value.
-
-        return f"{self.value}{UNIT_SEPARATOR}{self.unit}"
-
-
-def _ValueUnitAndComment(
-    value_w_unit_w_comment: str,
-    comment_marker: str,
+
+def AsStr(
+    config: any_dict_config_h,
     /,
-) -> tuple[str, str | None, str | None]:
+    *,
+    color: color_modes_h = None,
+    section_color: str = None,
+    parameter_color: str = None,
+) -> str:
     """"""
-    value_w_unit, comment = Pieces(value_w_unit_w_comment, comment_marker)
-    if (comment is not None) and (comment.__len__() == 0):
-        comment = None
+    output = []
+
+    if section_color is None:
+        section_color = SECTION_COLOR
+    if parameter_color is None:
+        parameter_color = PARAMETER_COLOR
+
+    if color is None:
+        section_color = ""
+        parameter_color = ""
+        color_reset = ""
+        newline = "\n"
+        indentation = " "
+        bracket_escape = ""
+    elif color == "rich":
+        section_color = f"[{section_color}]"
+        parameter_color = f"[{parameter_color}]"
+        color_reset = "[/]"
+        newline = "\n"
+        indentation = " "
+        bracket_escape = "\\"
+    elif color == "html":
+        section_color = f'<span style="color:{section_color}">'
+        parameter_color = f'<span style="color:{parameter_color}">'
+        color_reset = "</span>"
+        newline = "<br/>"
+        indentation = "&nbsp;"
+        bracket_escape = ""
+    else:
+        raise ValueError(
+            f"{color}: Invalid color mode; Expected=one of {get_args(color_modes_h)}."
+        )
+
+    longest = 0
+    for section, parameters in config.items():
+        if parameters.__len__() == 0:
+            continue
+
+        inner_output = []
+        lengths = []
+        for name, value in parameters.items():
+            length = name.__len__()
+            lengths.append(length)
+            longest = max(longest, length)
+
+            flattened = Flattened(str(value))
+            inner_output.append(f"{parameter_color}{name}{color_reset}@= {flattened}")
+
+        output.append(
+            (
+                f"{section_color}{bracket_escape}[{section}]{color_reset}",
+                inner_output,
+                lengths,
+            )
+        )
 
-    value_as_str, unit = Pieces(value_w_unit, UNIT_SEPARATOR, from_left=False)
-    # if unit.__len__() == 0, do not make it None so that an invalid unit error is noticed later on
+    output = (
+        f"{_sct}{newline}"
+        + newline.join(
+            _lne.replace("@", (longest - _lgt + 1) * indentation, 1)
+            for _lne, _lgt in zip(_prm, _lgs)
+        )
+        for _sct, _prm, _lgs in output
+    )
 
-    return value_as_str, unit, comment
+    return f"{newline}{newline}".join(output)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/instance/parameter/unit.py` & `conf_ini_g-2024.1/conf_ini_g/catalog/interface/window/parameter/choices.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,95 +25,80 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
-from pathlib import Path as path_t
-from typing import Any, Sequence
-
-from conf_ini_g.instance.parameter.base import Pieces, base_t
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import INVALID_VALUE
+from __future__ import annotations
 
+import dataclasses as dtcl
+from typing import Any
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class unit_instance_t(base_t):
-    def SetStrValue(
-        self,
-        value_w_comment: str | Any,
-        comment_marker: str,
+from babelwidget.main import backend_t
+from babelwidget.main import dropdown_choice_h as dropdown_choice_wgt_h
+from conf_ini_g.catalog.specification.annotation.choices import choices_t
+from conf_ini_g.interface.window.parameter.value import value_wgt_a
+from conf_ini_g.phase.specification.parameter.type import type_t
+
+INDEX_FOR_NONE = 0
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class choices_wgt_t(value_wgt_a):
+    library_wgt: dropdown_choice_wgt_h
+
+    @classmethod
+    def NewForSpecification(
+        cls,
+        stripe: type_t | choices_t,
+        backend: backend_t,
         /,
-        *,
-        _: str = None,
-    ) -> None:
+    ) -> choices_wgt_t:
         """
-        value_w_unit_w_comment: can be an uninterpreted string coming from an INI
-        document, or can be an interpreted value coming from an interface.
+        If stripe does not contain the necessary details, the initial value (if valid) is the only choice, or a unique
+        default choice ending with an exclamation point is added.
         """
-        value_as_str, comment = _ValueAndComment(value_w_comment, comment_marker)
-        self.value = value_as_str
-        self.comment = comment
-
-    def TypedValue(
-        self, expected_type: type_t, /, *, units=None
-    ) -> tuple[Any, list[str]]:
-        """"""
-        final_value, success = expected_type.InterpretedValueOf(self.value)
+        output = cls(library_wgt=backend.dropdown_choice_t())
+
+        output.SetupValueChangedMessaging(output.library_wgt, "released", backend)
+
+        if isinstance(stripe, type_t):
+            annotation = stripe.FirstAnnotationWithType(choices_t)
+            if annotation is None:
+                raise ValueError("No choices provided.")
+        else:
+            annotation = stripe
 
-        if success:
-            return final_value, []
+        for choice in annotation.options:
+            output.library_wgt.addItem(choice)
 
-        return INVALID_VALUE, [f"{self.value}: Invalid value."]
+        return output
+
+    def Assign(self, value: str | None, _: Any, /) -> None:
+        """"""
+        if value is None:
+            where = INDEX_FOR_NONE
+        else:
+            choices = tuple(map(self.itemText, range(self.count())))
+            try:
+                where = choices.index(value)
+            except ValueError:
+                choices = " or ".join(choices)
+                raise ValueError(f"Invalid value: Actual={value}; Expected={choices}.")
+
+        self.setCurrentIndex(where)
 
     def Text(self) -> str:
         """"""
-        return self.value  # No need for "str" since units have no default values.
+        return self.library_wgt.currentText()
 
+    def __getattr__(self, attribute: str, /) -> Any:
+        """
+        E.g., used for "SetFunction".
+        """
+        try:
+            output = self.__getattribute__(attribute)
+        except AttributeError:
+            output = getattr(self.library_wgt, attribute)
 
-def ConvertedValue(
-    value: Any, conversion_factor: int | float, /
-) -> tuple[Any, list[str]]:
-    """"""
-    unconverted_values = []
-
-    if _ValueIsNotUnitCompatible(value):
-        converted = value
-    elif isinstance(value, (int, float)):
-        converted = conversion_factor * value
-    elif isinstance(value, Sequence):
-        converted = []
-        for element in value:
-            converted_elm, unconverted_elm = ConvertedValue(element, conversion_factor)
-            converted.append(converted_elm)
-            unconverted_values.extend(unconverted_elm)
-        converted = tuple(converted)
-    else:
-        converted = value
-        unconverted_values.append(str(value))
-
-    return converted, unconverted_values
-
-
-def _ValueAndComment(
-    value_w_comment: str,
-    comment_marker: str,
-    /,
-) -> tuple[str, str | None]:
-    """"""
-    value_as_str, comment = Pieces(value_w_comment, comment_marker)
-    if (comment is not None) and (comment.__len__() == 0):
-        comment = None
-
-    return value_as_str, comment
-
-
-def _ValueIsNotUnitCompatible(value: Any, /) -> bool:
-    """"""
-    return (
-        (value is None)
-        or isinstance(value, bool)
-        or isinstance(value, str)
-        or isinstance(value, path_t)
-    )
+        return output
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/console/__init__.py` & `conf_ini_g-2024.1/documentation/wiki/description.asciidoc`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-# Copyright CNRS/Inria/UNS
-# Contributor(s): Eric Debreuve (since 2021)
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
+// Copyright CNRS/Inria/UCA
+// Contributor(s): Eric Debreuve (since 2021)
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
 
-from conf_ini_g.interface.console.config import CommandLineParser, ParsedArguments
+:AUTHOR: Eric Debreuve
+:EMAIL: eric.debreuve@cnrs.fr
+
+:PROJECT_NAME: Conf-INI-g
+:SHORT_DESCRIPTION: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
+:KEYWORDS: app, application, configuration, INI, command-line, graphical interface
+
+:REPOSITORY_NAME: conf-ini-g
+:REPOSITORY_USER: eric.debreuve
+:REPOSITORY_SITE: src.koda.cnrs.fr
+:SINCE_YEAR: 2021
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/console/config.py` & `conf_ini_g-2024.1/conf_ini_g/interface/console/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -31,60 +31,64 @@
 
 import re as rgex
 from argparse import ArgumentParser as argument_parser_t
 from pathlib import Path as path_t
 from typing import Any, Iterator, Sequence
 
 from conf_ini_g.extension.string import Flattened
-from conf_ini_g.raw.config import raw_config_h
-from conf_ini_g.specification.config import config_t
-from conf_ini_g.specification.parameter.value import MISSING_REQUIRED_VALUE
+from conf_ini_g.phase.specification.config.main import config_t
+from conf_ini_g.phase.specification.parameter.value import MISSING_REQUIRED_VALUE
+from conf_ini_g.phase.untyped.config import ini_config_h
 
 parsed_arguments_h = dict[str, str]
 
 
-# Specified INI document file is stored in INI_DOCUMENT_VARIABLE
-INI_DOCUMENT_VARIABLE = "ini_path"
+# Specified INI document file is stored in _INI_DOCUMENT_VARIABLE
+_INI_DOCUMENT_VARIABLE = "ini_path"
 
-ADVANCED_MODE_OPTION = "advanced-mode"
-ADVANCED_MODE_VARIABLE = "advanced_mode"
+_ADVANCED_MODE_OPTION = "advanced-mode"
+_ADVANCED_MODE_VARIABLE = "advanced_mode"
 
-# Usage: {section_name}{SECTION_PARAMETER_SEPARATOR}{parameter_name}
-SECTION_PARAMETER_SEPARATOR = "-"
+# Usage: {section_name}{_SECTION_PARAMETER_SEPARATOR}{parameter_name}
+_SECTION_PARAMETER_SEPARATOR = "-"
 
 
 def CommandLineParser(
     description: str | None, specification: config_t, /
 ) -> argument_parser_t:
     """"""
     output = argument_parser_t(description=description, allow_abbrev=False)
-    # TODO: Why is this argument optional?
+    # This argument is optional because all parameters can be explicitly passed as
+    # arguments (CLI mode), or nothing can be passed at all (GUI mode).
     output.add_argument(
-        dest=INI_DOCUMENT_VARIABLE,
+        dest=_INI_DOCUMENT_VARIABLE,
         help="Path to INI configuration file",
         default=None,
         nargs="?",
         metavar="INI_config_file",
     )
 
+    # Default is a missing_required_value_t instance to avoid overwriting if in
+    # INI but not passed.
+    default = MISSING_REQUIRED_VALUE
+    options = []
     for section in specification:
         for parameter in section.all_parameters:
-            option = f"{section.name}{SECTION_PARAMETER_SEPARATOR}{parameter.name}"
-            if option == ADVANCED_MODE_OPTION:
+            option = f"{section.name}{_SECTION_PARAMETER_SEPARATOR}{parameter.name}"
+            if option == _ADVANCED_MODE_OPTION:
                 # Raising an exception is adapted here since execution has been launched from command line
                 raise ValueError(
                     f"{option}: Command-line option for parameter is identical to advanced mode option. "
                     f"Please change parameter specification (section name and/or parameter name)."
                 )
+            if option in options:
+                # This can happen in controlled sections whose alternatives share equally named parameters.
+                continue
 
-            attribute = f"{section.name}{SECTION_PARAMETER_SEPARATOR}{parameter.name}"
-
-            # Default is a missing_required_value_t instance to avoid overwriting if in
-            # INI but not passed.
-            default = MISSING_REQUIRED_VALUE
+            attribute = f"{section.name}{_SECTION_PARAMETER_SEPARATOR}{parameter.name}"
 
             if parameter.optional:
                 if isinstance(parameter.default, str):
                     delimiter = '"'
                 else:
                     delimiter = ""
                 type_and_value = (
@@ -92,77 +96,81 @@
                     f"Default: [green]{delimiter}{parameter.default}{delimiter}[/]"
                 )
             else:
                 type_and_value = str(default)
             flattened = Flattened(type_and_value)
             definition = f"{parameter.definition}. {flattened}"
 
-            # Type could be TypeHintOfAnnotated(cmd_line_type). However, to allow passing any of the allowed types,
+            # Type could be TypeOfAnnotatedHint(cmd_line_type). However, to allow passing any of the allowed types,
             # deferring type validation to functional config instantiation, this parameter is not passed.
             output.add_argument(
                 f"--{option}",
                 dest=attribute,
                 help=definition,
                 default=default,
                 metavar=attribute,
             )
+            options.append(option)
 
     output.add_argument(
-        f"--{ADVANCED_MODE_OPTION}",
-        dest=ADVANCED_MODE_VARIABLE,
+        f"--{_ADVANCED_MODE_OPTION}",
+        dest=_ADVANCED_MODE_VARIABLE,
         help="Toggle display of advanced sections and parameters",
         action="store_true",
     )
 
     return output
 
 
-def ParsedArguments(
+def CommandLineConfig(
     parser: argument_parser_t, /, *, arguments: Sequence[str] = None
-) -> tuple[path_t | None, bool, raw_config_h]:
+) -> tuple[ini_config_h, bool, path_t | None]:
     """"""
     parsed, unknowns = parser.parse_known_args(args=arguments)
     parsed = vars(parsed)
 
-    advanced_mode = parsed[ADVANCED_MODE_VARIABLE]
-    del parsed[ADVANCED_MODE_VARIABLE]
+    advanced_mode = parsed[_ADVANCED_MODE_VARIABLE]
+    del parsed[_ADVANCED_MODE_VARIABLE]
 
-    ini_path = parsed[INI_DOCUMENT_VARIABLE]
-    del parsed[INI_DOCUMENT_VARIABLE]
+    ini_path = parsed[_INI_DOCUMENT_VARIABLE]
+    del parsed[_INI_DOCUMENT_VARIABLE]
     if ini_path is not None:
-        ini_path = path_t(ini_path).resolve(strict=True)
+        try:
+            ini_path = path_t(ini_path).resolve(strict=True)
+        except (FileNotFoundError, RuntimeError):
+            raise FileNotFoundError(f"Nonexistent or invalid path: {ini_path}")
 
     pattern = rgex.compile(
-        r"--(\w+)" + SECTION_PARAMETER_SEPARATOR + r"(\w+)=(.+)", flags=rgex.ASCII
+        r"--(\w+)" + _SECTION_PARAMETER_SEPARATOR + r"(\w+)=(.+)", flags=rgex.ASCII
     )
     for unknown in unknowns:
         match = pattern.fullmatch(unknown)
         if match is None:
             # Raising an exception is adapted here since execution has been launched from command line
             raise ValueError(
                 f"{unknown}: Invalid option syntax; Expected=--SECTION-PARAMETER=VALUE"
             )
 
         section, parameter, value = match.groups()
-        parsed[f"{section}{SECTION_PARAMETER_SEPARATOR}{parameter}"] = value
+        parsed[f"{section}{_SECTION_PARAMETER_SEPARATOR}{parameter}"] = value
 
     raw_config = {}
     for sct_name, prm_name, value in _SectionParameterValueIterator(parsed):
         if sct_name in raw_config:
             raw_config[sct_name][prm_name] = value
         else:
             raw_config[sct_name] = {prm_name: value}
 
-    return ini_path, advanced_mode, raw_config
+    return raw_config, advanced_mode, ini_path
 
 
 def _SectionParameterValueIterator(
     arguments: parsed_arguments_h,
 ) -> Iterator[tuple[str, str, Any]]:
     """"""
     for prm_uid, value in arguments.items():
         # See CommandLineParser for why this can happen.
         if value is MISSING_REQUIRED_VALUE:
             continue
 
-        section, parameter = prm_uid.split(SECTION_PARAMETER_SEPARATOR)
+        section, parameter = prm_uid.split(_SECTION_PARAMETER_SEPARATOR)
         yield section, parameter, value
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/screen/config.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/config/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,153 +28,166 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+import inspect as nspt
 from pathlib import Path as pl_path_t
-from typing import Annotated, Any, Callable, Iterator, Sequence
+from typing import Any, Callable, Sequence
 
-from conf_ini_g.catalog.interface.screen.parameter.boolean import boolean_wgt_t
-from conf_ini_g.catalog.interface.screen.parameter.path import path_wgt_t
-from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
-from conf_ini_g.catalog.specification.parameter.path import path_t
-from conf_ini_g.catalog.specification.parameter.path import path_t as path_annotation_t
-from conf_ini_g.instance.config import config_t as config_instance_t
-from conf_ini_g.interface.screen.backend import (
-    backend_t,
-    button_wgt_h,
-    grid_lyt_h,
-    hbox_lyt_h,
-    library_wgt_h,
-    vbox_lyt_h,
+from babelwidget.backend.generic.path_chooser import NewSelectedOutputDocument
+from babelwidget.main import backend_t
+from babelwidget.main import base_h as library_wgt_h
+from conf_ini_g.interface.storage.config import INIConfig, SaveConfigToINIDocument
+from conf_ini_g.interface.window.config.action import ActionButtonsLayout
+from conf_ini_g.interface.window.config.advanced import AdvancedModeLayout
+from conf_ini_g.interface.window.config.title import TitleLayout
+from conf_ini_g.interface.window.section.collection import SectionsAndCategories
+from conf_ini_g.interface.window.section.main import (
+    any_section_h,
+    controlled_section_t,
+    free_section_t,
 )
-from conf_ini_g.interface.screen.parameter.path_chooser import NewSelectedOutputDocument
-from conf_ini_g.interface.screen.section import controlled_section_t, section_t
-from conf_ini_g.interface.storage.config import SaveRawConfigToINIDocument
-from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-from conf_ini_g.raw.config import AsStr, ini_config_h, raw_config_h
-from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.phase.generic.config import AsStr
+from conf_ini_g.phase.specification.config.main import config_t as specification_t
+from conf_ini_g.phase.specification.parameter.main import (
+    parameter_t as parameter_spec_t,
+)
+from conf_ini_g.phase.specification.section.specific import (
+    any_section_h as any_section_spec_h,
+)
+from conf_ini_g.phase.specification.section.specific import (
+    controlled_section_t as controlled_section_spec_t,
+)
+from conf_ini_g.phase.specification.section.specific import (
+    free_section_t as free_section_spec_t,
+)
+from conf_ini_g.phase.typed.config.main import (
+    TypedFromUntyped,
+    WithConsumedUnits,
+    typed_config_h,
+)
+from conf_ini_g.phase.untyped.config import ini_config_h
 
 
 @dtcl.dataclass(repr=False, eq=False)
-class config_t:
+class config_t(list[any_section_h]):
     """
     The class cannot use slots because it disables weak referencing, which is required.
     See error message below when using slots:
     TypeError: cannot create weak reference to 'config_t' object
     [...]
-    File "[...]conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py", line 41, in SetFunction
+    File "[...]conf_ini_g/catalog/interface/window/backend/pyqt5/widget/choices.py", line 41, in SetFunction
         self.clicked.connect(function)
-        │                    └ <bound method config_t.ToogleAdvancedMode of <conf_ini_g.interface.screen.config.config_t object at [...]>>
-        └ <conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices.dot_button_wgt_t object at [...]>
+        │                    └ <bound method config_t.ToggleAdvancedMode of <conf_ini_g.interface.window.config.config_t object at [...]>>
+        └ <conf_ini_g.catalog.interface.window.backend.pyqt5.widget.choices.radio_choice_wgt_h object at [...]>
 
     Widget might not cooperate well with list, in which case Python raises the
     following exception: TypeError: multiple bases have instance lay-out conflict
     To be safe, "sections" is a field instead of being part of the class definition.
+
+    _widget: Both an access for interacting with widgets, and a reference keeper to
+    prevent autonomous widgets from loosing their "liveness".
     """
 
-    sections: dict[str, section_t | controlled_section_t] = dtcl.field(
-        init=False, default=None
-    )
-    instance: config_instance_t
+    specification: specification_t
+    ini_path: pl_path_t | None
+    UpdateHistory: Callable[[pl_path_t | str], None] | None
+    #
     backend: backend_t
     library_wgt: library_wgt_h
-    _action_button: button_wgt_h = dtcl.field(init=False, default=None)
-    Action: Callable[[raw_config_h], None] = None
-    _reference_keeper: tuple[library_wgt_h, ...] = None
+    #
+    Action: Callable[[typed_config_h], None] = None
+    #
+    _widget: dict[str, library_wgt_h] = dtcl.field(init=False, default_factory=dict)
 
     @classmethod
-    def NewFromConfig(
+    def NewForSpecification(
         cls,
         title: str | None,
-        instance: config_instance_t,
+        specification: specification_t,
+        ini_path: pl_path_t | None,
         backend: backend_t,
         /,
         *,
+        history: Sequence[str] | None = None,
+        UpdateHistory: Callable[[pl_path_t | str], None] | None = None,
+        action: tuple[str, Callable[[typed_config_h], None]] = None,
         advanced_mode: bool = False,
-        action: tuple[str, Callable[[raw_config_h], None]] = None,
     ) -> config_t:
         """"""
+        if ini_path is not None:
+            if UpdateHistory is not None:
+                UpdateHistory(ini_path)
+            as_str = str(ini_path)
+            if history is None:
+                history = (as_str,)
+            elif as_str not in history:
+                history = list(history)
+                history.append(as_str)
+
         if action is None:
             kwargs = {}
         else:
             kwargs = {"Action": action[1]}
+
         output = cls(
-            instance=instance,
+            specification=specification,
+            ini_path=ini_path,
             backend=backend,
-            library_wgt=backend.library_wgt_t(),
+            library_wgt=backend.base_t(),
+            UpdateHistory=UpdateHistory,
             **kwargs,
         )
 
         # --- Top-level widgets
-        title_lyt, widget_1 = _TitleLayout(title, instance, output)
-        advanced_mode_lyt, widget_2 = _AdvancedModeLayout(advanced_mode, output)
-        button_lyt, widgets = _ActionButtonsLayout(
-            output, action, instance.ini_path is not None
+        (
+            title_lyt,
+            ini_path_wgt,
+            history_button,
+            history_menu,
+            close_button,
+        ) = TitleLayout(
+            title,
+            specification,
+            history,
+            backend,
+            ini_path,
+            output.UpdateWithNewINI,
+            output.library_wgt.close,
+        )
+        advanced_mode_lyt, adv_mode_wgt = AdvancedModeLayout(
+            advanced_mode, backend, output.ToggleAdvancedMode
+        )
+        button_lyt, action_button, action_wgts = ActionButtonsLayout(
+            action,
+            ini_path is not None,
+            backend,
+            output.ShowInINIFormat,
+            output.SaveConfig,
+            output.LaunchAction,
+            output.library_wgt.close,
         )
-        output._reference_keeper = (widget_1, widget_2, *widgets)
+        output._widget["ini_path"] = ini_path_wgt
+        output._widget["history_button"] = history_button
+        output._widget["history_menu"] = history_menu
+        output._widget["adv_mode"] = adv_mode_wgt
+        output._widget["action"] = action_button
+        output._widget["action_buttons"] = action_wgts
+        output._widget["close"] = close_button
 
         # --- Sections
-        categories = {}
-        sections = {}
-        controlled_sections = []
-
-        for section_spec in instance.specification:
-            if (controller := section_spec.controller) is None:
-                section = section_t.NewForSection(
-                    section_spec, instance[section_spec.name], backend
-                )
-            else:
-                section = controlled_section_t.NewForSection(
-                    section_spec,
-                    controller,
-                    instance.GetValueOfController(controller),
-                    instance[section_spec.name],
-                    backend,
-                )
-                if section is not None:
-                    controlled_sections.append((section, section_spec))
-            if section is None:
-                continue
-
-            sections[section_spec.name] = section
-
-            if (category := section_spec.category) not in categories:
-                contents = backend.library_wgt_t()
-                scroll_area = backend.scroll_container_t.NewForWidget(contents)
-                layout = backend.vbox_lyt_t()
-                contents.setLayout(layout)
-                categories[category] = (layout, scroll_area)
-
-            layout = categories[category][0]
-            layout.addWidget(section.library_wgt)
-
-        output.sections = sections
-
-        if categories.__len__() > 1:
-            category_selector = backend.tabs_wgt_t()
-            for category, (_, scroll_area) in categories.items():
-                category_selector.addTab(scroll_area, category)
-        else:
-            category = tuple(categories.keys())[0]
-            category_selector = categories[category][1]
-
-        for section, section_spec in controlled_sections:
-            controller = section_spec.controller
-            parameter = output[controller.section].parameters[controller.parameter]
-            value_wgt = parameter.value
-            if hasattr(value_wgt, "SetFunction"):
-                value_wgt.SetFunction(section.page_stack.setCurrentIndex)
-            else:
-                backend.ShowErrorMessage(
-                    f"{controller.section}.{controller.parameter}: "
-                    f'Controller has no "SetFunction" method; Disabling control.'
-                )
+        sections, controlled_sections, category_selector = SectionsAndCategories(
+            specification, None, backend
+        )
+        output.extend(sections)
+        output._AssociateSectionsAndControllers(controlled_sections)
+        output._widget["category_selector"] = category_selector
 
         # --- Layout...
         layout = backend.grid_lyt_t()
         if title_lyt is None:
             first_available_row = 0
         else:
             layout.addLayout(title_lyt, 0, 0, 1, 1)
@@ -182,267 +195,243 @@
         layout.addWidget(category_selector, first_available_row, 0, 1, 1)
         layout.addLayout(advanced_mode_lyt, first_available_row + 1, 0, 1, 1)
         layout.addLayout(button_lyt, first_available_row + 2, 0, 1, 1)
 
         output.library_wgt.setLayout(layout)
         # --- ...Layout
 
-        output.ToogleAdvancedMode(advanced_mode)
-
         return output
 
-    def ToogleAdvancedMode(self, advanced_mode: bool, /) -> None:
+    def _AssociateSectionsAndControllers(
+        self,
+        controlled_sections: Sequence[
+            tuple[controlled_section_t, controlled_section_spec_t]
+        ],
+        /,
+    ) -> None:
+        """"""
+        for section, section_spec in controlled_sections:
+            controller = section_spec.controller
+            # Controller section cannot be controlled, so active parameters are in fact
+            # all the parameters.
+            parameter = self[controller.section].active_parameters[controller.parameter]
+            value_wgt = parameter.value
+            if hasattr(value_wgt, "SetFunction"):
+                value_wgt.SetFunction(section.page_stack.setCurrentIndex)
+            else:
+                self.backend.ShowErrorMessage(
+                    f"{controller.section}.{controller.parameter}: "
+                    f'Controller has no "SetFunction" method; Disabling control.'
+                )
+
+    def ReassignCloseButtonTarget(self) -> None:
         """"""
-        for section_name, section in self.sections.items():
-            section_spec = self.instance.specification[section_name]
+        current = self.library_wgt
+        while current is not None:
+            main_window = current
+            current = current.parent()
+
+        self._widget["close"].SetFunction(main_window.close)
+
+    def SetValues(
+        self, config: typed_config_h, units: dict[tuple[str, str], tuple[str, float]], /
+    ) -> None:
+        """"""
+        for section in self:
+            sct_name = section.spec_name
+            if isinstance(section, free_section_t):
+                for parameter in section:
+                    prm_name = parameter.spec_name
+                    parameter_spec = self.specification[sct_name][prm_name]
+                    typed_section = config[sct_name]
+                    if prm_name in typed_section:
+                        parameter.value.Assign(
+                            typed_section[prm_name], parameter_spec.type
+                        )
+                        unit = units.get((sct_name, prm_name), None)
+                        if unit is not None:
+                            parameter.unit.setText(unit[0])
+                    elif parameter_spec.optional:
+                        parameter.value.Assign(
+                            parameter_spec.default, parameter_spec.type
+                        )
+            else:
+                for controlling_value, parameters in section.items():
+                    for parameter in parameters:
+                        prm_name = parameter.spec_name
+                        parameter_spec = self.specification[sct_name][
+                            controlling_value
+                        ][prm_name]
+                        typed_section = config[sct_name]
+                        if prm_name in typed_section:
+                            parameter.value.Assign(
+                                typed_section[prm_name], parameter_spec.type
+                            )
+                            unit = units.get((sct_name, prm_name), None)
+                            if unit is not None:
+                                parameter.unit.setText(unit[0])
+                        elif parameter_spec.optional:
+                            parameter.value.Assign(
+                                parameter_spec.default, parameter_spec.type
+                            )
+
+    def ToggleAdvancedMode(self, advanced_mode: bool, /) -> None:
+        """"""
+        for section in self:
+            section_spec = self.specification[section.spec_name]
             if section_spec.basic:
                 should_check_parameters = True
             elif advanced_mode:
                 section.library_wgt.setVisible(True)
                 should_check_parameters = True
             else:
                 section.library_wgt.setVisible(False)
                 should_check_parameters = False
 
             if should_check_parameters:
-                if (controller := section_spec.controller) is None:
-                    parameter_specs = section_spec
-                else:
-                    controller_text = (
-                        self[controller.section].parameters[controller.parameter].Text()
-                    )
-                    parameter_specs = section_spec.ActiveParameters(controller_text)
-                for parameter, parameter_spec in zip(
-                    section.active_parameters.values(), parameter_specs
-                ):
+                parameters = section.active_parameters
+                parameter_specs = self._ActiveParameterSpcOfSection(section_spec)
+                for parameter, parameter_spec in zip(parameters, parameter_specs):
                     if not parameter_spec.basic:
                         if advanced_mode:
-                            parameter.setVisible(True)
+                            parameter.SetVisible(True)
                         else:
-                            parameter.setVisible(False)
+                            parameter.SetVisible(False)
 
-    def SynchronizeInstance(self) -> list[str]:
+    def UpdateWithNewINI(self, ini_path: pl_path_t | str, /) -> None:
         """"""
-        for section_name, section in self.sections.items():
-            section_spec = self.instance.specification[section_name]
-            if (controller := section_spec.controller) is None:
-                parameter_specs = section_spec
-            else:
-                controller_text = (
-                    self[controller.section].parameters[controller.parameter].Text()
-                )
-                parameter_specs = section_spec.ActiveParameters(controller_text)
-            for parameter, parameter_spec in zip(
-                section.active_parameters.values(), parameter_specs
-            ):
-                if parameter.unit is None:
-                    unit_kwarg = {}
-                else:
-                    unit_kwarg = {"unit": parameter.unit.Text()}
-                instance = self.instance[section_spec.name][parameter_spec.name]
-                instance.SetStrValue(
-                    parameter.Text(),
-                    INI_COMMENT_MARKER,
-                    **unit_kwarg,
-                )
+        if isinstance(ini_path, str):
+            ini_path = pl_path_t(ini_path)
 
-        return self.instance.Issues()
+        config_ini = INIConfig(ini_path)
+        config_typed, config_units, config_comments, issues = TypedFromUntyped(
+            config_ini, None, self.specification
+        )
+        if issues.__len__() > 0:
+            self.backend.ShowErrorMessage("\n".join(issues), parent=self.library_wgt)
+            return
 
-    def AsINIConfig(self) -> ini_config_h | None:
+        category_selector = self._widget["category_selector"]
+        if isinstance(category_selector, self.backend.tabs_t):
+            # Note: idx^th layout: category_selector.widget(t_idx).widget().layout().
+            while category_selector.count() > 0:
+                category_selector.removeTab(0)
+        else:
+            layout = category_selector.widget().layout()
+            while layout.count() > 0:
+                layout.itemAt(0).widget().setParent(None)
+
+        self.clear()
+        sections, controlled_sections, _ = SectionsAndCategories(
+            self.specification, category_selector, self.backend
+        )
+        self.extend(sections)
+        self._AssociateSectionsAndControllers(controlled_sections)
+        self.SetValues(config_typed, config_units)
+        self.ToggleAdvancedMode(self._widget["adv_mode"].true_btn.isChecked())
+
+        self._widget["ini_path"].Assign(ini_path, None)
+        self._widget["history_button"].setEnabled(True)
+        if str(ini_path) not in (
+            _elm.text() for _elm in self._widget["history_menu"].actions()
+        ):
+            self._widget["history_menu"].addAction(str(ini_path))
+
+        if self.UpdateHistory is not None:
+            self.UpdateHistory(ini_path)
+
+    def _ActiveParameterSpcOfSection(
+        self, section_spec: any_section_spec_h, /
+    ) -> Sequence[parameter_spec_t]:
         """"""
-        issues = self.SynchronizeInstance()
-        if issues.__len__() == 0:
-            output = self.instance.AsINIConfig()
+        if isinstance(section_spec, free_section_spec_t):
+            output = section_spec
         else:
-            output = None
-            self.backend.ShowErrorMessage("\n".join(issues), parent=self)
+            controller = section_spec.controller
+            controller = self[controller.section].active_parameters[
+                controller.parameter
+            ]
+            output = section_spec.ActiveParameters(controller.Text())
 
         return output
 
-    def ShowInINIFormat(self) -> None:
+    def AsINI(self) -> ini_config_h:
+        """"""
+        return {_elm.spec_name: _elm.AsINI() for _elm in self}
+
+    def LaunchAction(self) -> None:
         """"""
-        config = self.AsINIConfig()
-        if config is None:
+        config_full, units_full, _, issues = TypedFromUntyped(
+            self.AsINI(), None, self.specification
+        )
+        if issues.__len__() > 0:
+            self.backend.ShowErrorMessage("\n".join(issues), parent=self.library_wgt)
             return
 
-        config = AsStr(config, in_html_format=True)
+        typed_config, issues = WithConsumedUnits(config_full, units_full)
+        if issues.__len__() > 0:
+            self.backend.ShowErrorMessage("\n".join(issues), parent=self.library_wgt)
+            return
+
+        self.setEnabled(False)
+        self.backend.qt_core_app_t.processEvents()
+        try:
+            self.Action(typed_config)
+        except Exception as exception:
+            trace = nspt.trace()[-1]
+            context = "\n".join(trace.code_context)
+            self.backend.ShowErrorMessage(
+                f"{trace.filename}@{trace.lineno}:{trace.function}\n"
+                f"{context}\n"
+                f"{exception}",
+                parent=self.library_wgt,
+            )
+        self.setEnabled(True)
+
+    def ShowInINIFormat(self) -> None:
+        """"""
+        config = AsStr(self.AsINI(), color="html")
         self.backend.ShowMessage("INI Config", "<tt>" + config + "<tt/>")
 
     def SaveConfig(self, new_ini: bool, /) -> None:
         """"""
         if new_ini:
             path = NewSelectedOutputDocument(
                 "Save Config As",
                 "Save Config As",
                 self.backend,
-                mode=path_t.TARGET_TYPE.document,
+                mode="document",
                 valid_types={"Config files": ("ini", "INI")},
             )
         else:
-            path = self.instance.ini_path  # Will overwrite current INI document
+            path = self.ini_path  # Will overwrite current INI document
 
         if path is not None:
-            config = self.AsINIConfig()
-            error = SaveRawConfigToINIDocument(config, path)
-            if error is None:
-                self.instance.ini_path = path
+            config = self.AsINI()
+            issues = SaveConfigToINIDocument(config, path)
+            if issues.__len__() > 0:
+                self.backend.ShowErrorMessage("\n".join(issues), parent=self)
             else:
-                self.backend.ShowErrorMessage(error, parent=self)
-
-    def LaunchAction(self) -> None:
-        """"""
-        issues = self.SynchronizeInstance()
-        if issues.__len__() == 0:
-            raw_config, issues = self.instance.AsRawConfig()
-            if issues.__len__() == 0:
-                self._action_button.setEnabled(False)
-                try:
-                    self.Action(raw_config)
-                except Exception as exception:
-                    self.backend.ShowErrorMessage(
-                        str(exception), parent=self.library_wgt
-                    )
-                self._action_button.setEnabled(True)
-            else:
-                self.backend.ShowErrorMessage(
-                    "\n".join(issues), parent=self.library_wgt
-                )
-        else:
-            self.backend.ShowErrorMessage("\n".join(issues), parent=self.library_wgt)
+                self.ini_path = path
 
     def __getattr__(self, attribute: str, /) -> Any:
         """
         E.g., used for "show".
         """
         try:
-            output = super().__getattr__(attribute)
+            output = super().__getattribute__(attribute)
         except AttributeError:
             output = getattr(self.library_wgt, attribute)
 
         return output
 
     def __contains__(self, key: str, /) -> bool:
         """"""
-        return key in self.sections
+        return any(_elm.spec_name == key for _elm in self)
 
-    def __getitem__(self, key: str, /) -> section_t | controlled_section_t:
+    def __getitem__(self, key: str, /) -> any_section_h:
         """"""
-        return self.sections[key]
-
-    def __iter__(self) -> Iterator[str]:
-        """"""
-        return self.sections.keys()
-
-
-def _TitleLayout(
-    title: str | None, instance: config_instance_t, config: config_t, /
-) -> tuple[vbox_lyt_h, path_wgt_t]:
-    """"""
-    layout = config.backend.vbox_lyt_t()
-
-    if title is None:
-        title = "Conf-INI-g"
-    title = (
-        f'<h1 style="color: blue">{title}</h1>'
-        f"<b><font face=monospace>SPEC:</font></b> {instance.specification.spec_path}"
-    )
-    title_wgt = config.backend.label_wgt_t(title)
-    title_wgt.setAlignment(config.backend.ALIGNED_LEFT)
-
-    if instance.ini_path is None:
-        ini_path_wgt = path_layout = None
-    else:
-        ini_path_wgt = path_wgt_t.NewWithDetails(
-            pl_path_t(instance.ini_path),
-            path_annotation_t(
-                target_type=path_annotation_t.TARGET_TYPE.document, is_input=True
-            ),
-            config.backend,
-            None,
-            editable=False,
-        )
-        label_wgt = config.backend.label_wgt_t(
-            "<b><font face=monospace>INI: </font></b>"
-        )
-        label_wgt.setSizePolicy(config.backend.SIZE_FIXED, config.backend.SIZE_FIXED)
-        path_layout = config.backend.hbox_lyt_t()
-        path_layout.addWidget(label_wgt)
-        path_layout.addWidget(ini_path_wgt.library_wgt)
-
-    layout.addWidget(title_wgt)
-    if path_layout is not None:
-        layout.addLayout(path_layout)
-
-    return layout, ini_path_wgt
-
-
-def _AdvancedModeLayout(
-    advanced_mode: bool, config: config_t, /
-) -> tuple[hbox_lyt_h, boolean_wgt_t]:
-    """"""
-    layout = config.backend.hbox_lyt_t()
-
-    annotated_type = Annotated[bool, boolean_t(mode=boolean_t.MODE.on_off)]
-    value_type = type_t.NewFromType(annotated_type)
-    boolean = boolean_wgt_t.NewWithDetails(
-        advanced_mode,
-        value_type,
-        config.backend,
-        None,
-    )
-    boolean.true_btn.SetFunction(config.ToogleAdvancedMode)
-
-    layout.addWidget(config.backend.label_wgt_t("<i>Advanced Mode</i>"))
-    layout.addWidget(boolean.library_wgt)
-
-    return layout, boolean
-
-
-def _ActionButtonsLayout(
-    config: config_t,
-    action: tuple[str, Callable[[raw_config_h], None]] | None,
-    has_ini_document: bool,
-    /,
-) -> tuple[grid_lyt_h, Sequence[button_wgt_h, ...]]:
-    """"""
-    layout = config.backend.grid_lyt_t()
-
-    buttons = []
-    geometries = []
-
-    button = config.backend.button_wgt_t("Show in INI format")
-    button.SetFunction(config.ShowInINIFormat)
-    buttons.append(button)
-    geometries.append((0, 0, 1, 2))
-
-    button = config.backend.button_wgt_t("Save Config As")
-    button.SetFunction(lambda: config.SaveConfig(True))
-    buttons.append(button)
-    if has_ini_document:
-        geometries.append((1, 0, 1, 1))
-
-        button = config.backend.button_wgt_t("Save/Overwrite Config")
-        button.SetFunction(lambda: config.SaveConfig(False))
-        buttons.append(button)
-        geometries.append((1, 1, 1, 1))
-    else:
-        geometries.append((1, 0, 1, 2))
-
-    if action is None:
-        label = "Close"
-        Function = config.library_wgt.close
-    else:
-        label = action[0]
-        Function = config.LaunchAction
-
-    button = config.backend.button_wgt_t(label)
-    button.SetFunction(Function)
-    buttons.append(button)
-    geometries.append((2, 0, 1, 2))
-
-    config._action_button = button
-
-    for button, geometry in zip(buttons, geometries):
-        layout.addWidget(button, *geometry)
-    layout.setContentsMargins(0, 0, 0, 0)
+        for section in self:
+            if section.spec_name == key:
+                return section
 
-    return layout, buttons
+        raise KeyError(f"{key}: Not a section of config.")
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/screen/generic.py` & `conf_ini_g-2024.1/conf_ini_g/light/ini.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,24 +25,40 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-STD_ABBREVIATIONS = {
-    "fct": "function",
-    "mod": "module",
-    "n": "number of",
-    "o": "of",
-    "prm": "parameter",
-    "rng": "range",
-}
+from configparser import ConfigParser as config_t
+from configparser import ExtendedInterpolation
 
+from conf_ini_g.extension.path import any_path_h
+from conf_ini_g.phase.untyped.config import ini_config_h
 
-def FormattedName(name: str, separator: str) -> str:
+_DEFAULT_OPTIONS = (
+    ("delimiters", ("=",)),
+    ("comment_prefixes", ("#",)),
+    ("inline_comment_prefixes", ("#",)),
+    ("interpolation", ExtendedInterpolation()),
+)
+
+
+def NewConfigFromPath(path: any_path_h, /, **kwargs) -> ini_config_h:
     """"""
-    name_cmps = []
-    for component in name.split(separator):
-        name_cmps.append(STD_ABBREVIATIONS.get(component, component))
+    options = kwargs.copy()
+    for name, value in _DEFAULT_OPTIONS:
+        if name not in options:
+            options[name] = value
+
+    config = config_t(**options)
+    config.optionxform = lambda option: option  # To avoid automatic lowercasing
+    config.read(path)
 
-    return " ".join(name_cmps).capitalize()
+    # config.sections(): Does not include the default section named configparser.DEFAULTSECT
+    return {_nme: dict(config[_nme]) for _nme in config.sections()}
+    # return {
+    #     _nme: {
+    #         _prm: _vle for _prm, _vle in config[_nme].items()
+    #     }
+    #     for _nme in config.sections()
+    # }
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/screen/parameter/main.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/parameter/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,126 +28,116 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
-from types import NoneType, UnionType
-from typing import Sequence
+from types import UnionType
 
-from conf_ini_g.catalog.interface.screen.parameter.directory import WidgetTypeForType
-from conf_ini_g.catalog.interface.screen.parameter.multitype import multitype_wgt_t
-from conf_ini_g.extension.type import hint_node_t
-from conf_ini_g.instance.parameter.main import instance_t
-from conf_ini_g.interface.screen.backend import (
-    backend_t,
-    choices_list_wgt_h,
-    label_wgt_h,
-    library_wgt_h,
-    text_wgt_h,
+from babelwidget.main import backend_t
+from babelwidget.main import base_h as library_wgt_h
+from babelwidget.main import dropdown_choice_h as dropdown_choice_wgt_h
+from babelwidget.main import label_h as label_wgt_h
+from babelwidget.main import text_line_h as text_line_wgt_h
+from conf_ini_g.catalog.interface.window.parameter.directory import (
+    ValueWidgetTypeForType,
 )
-from conf_ini_g.interface.screen.generic import FormattedName
-from conf_ini_g.specification.parameter.main import parameter_t as parameter_spec_t
-from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
+from conf_ini_g.catalog.interface.window.parameter.multitype import multitype_wgt_t
+from conf_ini_g.interface.storage.parameter import INI_UNIT_SEPARATOR
+from conf_ini_g.interface.window.generic import FormattedName
+from conf_ini_g.interface.window.parameter.type import TypeSelector
+from conf_ini_g.phase.specification.parameter.main import (
+    parameter_t as parameter_spec_t,
+)
+from conf_ini_g.phase.specification.parameter.type import type_t
+from str_to_obj.type.hint_tree import hint_tree_t
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
+@dtcl.dataclass(repr=False, eq=False)
 class parameter_t:
     """
     In order to leave the section widget put the name, type, and input widgets of each parameter in columns,
     parameter_t is not a container widget. Instead, it just stores its component widgets for later addition to a layout.
     """
 
+    spec_name: str
     name: label_wgt_h = dtcl.field(init=False, default=None)
-    type: label_wgt_h | choices_list_wgt_h = dtcl.field(init=False, default=None)
+    type: label_wgt_h | dropdown_choice_wgt_h = dtcl.field(init=False, default=None)
     value: library_wgt_h = dtcl.field(init=False, default=None)
-    unit: text_wgt_h = dtcl.field(init=False, default=None)
+    unit: text_line_wgt_h = dtcl.field(init=False, default=None)
     comment: str = dtcl.field(init=False, default=None)
 
     @classmethod
-    def NewForParameter(
+    def NewForSpecification(
         cls,
         parameter_spec: parameter_spec_t,
-        instance: instance_t,
         backend: backend_t,
         /,
     ) -> parameter_t:
         """"""
-        output = cls()
+        output = cls(spec_name=parameter_spec.name)
 
         formatted_name = FormattedName(parameter_spec.name, " ")
-        comment = f"{formatted_name}\n{parameter_spec.definition}.\n\n{parameter_spec.description}."
-        if instance.comment is not None:
-            comment += f"\n\n{instance.comment}."
-        output.name = backend.label_wgt_t(formatted_name)
+        comment = (
+            f"{formatted_name}\n{parameter_spec.definition}.\n\n"
+            f"{parameter_spec.description}."
+        )
+        output.name = backend.label_t(formatted_name)
         output.name.setToolTip(comment)
         output.comment = comment
 
-        type_ = parameter_spec.type
-        value, issues = instance.TypedValue(type_)
-        if issues.__len__() > 0:
-            value = None
-        if isinstance(type_.hint, hint_node_t) and (type_.hint.type is UnionType):
-            hint_options = type_.hint.elements
-            type_wgt = _TypeSelector(hint_options, backend)
-            value_wgt = multitype_wgt_t.NewForHints(
-                value,
-                hint_options,
-                type_wgt,
-                backend,
-            )
-        else:
-            type_wgt = backend.label_wgt_t(type_.template_as_str)
-            widget_type = WidgetTypeForType(type_)
-            value_wgt = widget_type.NewWithDetails(
-                value,
-                type_,
-                backend,
-                parameter_spec,
-            )
-        output.type = type_wgt
-        output.value = value_wgt
+        stripe = parameter_spec.type
+        output.type, output.value = TypeAndValueWidgetsForType(stripe, backend)
 
-        if (unit := getattr(instance, "unit", None)) is not None:
-            output.unit = backend.text_wgt_t(unit)
+        output.unit = backend.text_line_t()
 
         name_style = "padding-right: 5px;"
         if parameter_spec.optional:
             name_style += "color: gray;"
         output.name.setStyleSheet(name_style)
         output.type.setStyleSheet(name_style)
 
         return output
 
     def SetVisible(self, visible: bool, /) -> None:
         """"""
         self.name.setVisible(visible)
         self.type.setVisible(visible)
+        self.value.library_wgt.setVisible(visible)
         if self.unit is not None:
             self.unit.setVisible(visible)
 
     def Text(self) -> str:
         """"""
         text = self.value.Text()
-
         if self.unit is None:
             return text
 
-        return f"{text}{UNIT_SEPARATOR}{self.unit.Text()}"
+        unit = self.unit.Text()
+        if unit.__len__() > 0:
+            return f"{text}{INI_UNIT_SEPARATOR}{unit}"
 
+        return text
 
-def _TypeSelector(
-    hints: Sequence[hint_node_t], backend: backend_t, /
-) -> choices_list_wgt_h:
-    """"""
-    output = backend.choice_menu_wgt_t()
 
-    for hint in hints:
-        # Here, it is important that hint trees cannot have an OR-node with an OR-node
-        # child so that hint.type has a valid value.
-        if hint is NoneType:
-            output.addItem("None")
-        else:
-            output.addItem(hint.type.__name__)
+def TypeAndValueWidgetsForType(
+    stripe: type_t | hint_tree_t, backend: backend_t, /
+) -> tuple[type[library_wgt_h], type[library_wgt_h]]:
+    """"""
+    if isinstance(stripe, hint_tree_t) and (stripe.type is UnionType):
+        hint_options = stripe.elements
+        type_wgt = TypeSelector(hint_options, backend)
+        value_wgt = multitype_wgt_t.NewForHints(
+            hint_options,
+            type_wgt,
+            backend,
+        )
+    else:
+        type_wgt = backend.label_t(stripe.template_as_str)
+        widget_type = ValueWidgetTypeForType(stripe)
+        value_wgt = widget_type.NewForSpecification(
+            stripe,
+            backend,
+        )
 
-    return output
+    return type_wgt, value_wgt
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/screen/section.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/section/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,208 +28,212 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
+import itertools as ittl
 from typing import ClassVar, Iterator, Sequence
 
-from conf_ini_g.instance.parameter.main import instance_t
-from conf_ini_g.interface.screen.backend import (
-    backend_t,
-    grid_lyt_h,
-    group_wgt_h,
-    label_wgt_h,
-    stack_wgt_h,
+from babelwidget.main import backend_t, grid_lyt_h
+from babelwidget.main import group_h as group_wgt_h
+from babelwidget.main import label_h as label_wgt_h
+from babelwidget.main import stack_h as stack_wgt_h
+from conf_ini_g.interface.storage.section import INI_UNIT_SECTION
+from conf_ini_g.interface.window.generic import FormattedName
+from conf_ini_g.interface.window.parameter.main import parameter_t
+from conf_ini_g.phase.specification.parameter.main import (
+    parameter_t as parameter_spec_t,
+)
+from conf_ini_g.phase.specification.section.controller import controller_t
+from conf_ini_g.phase.specification.section.specific import (
+    any_section_h as any_section_spec_h,
+)
+from conf_ini_g.phase.specification.section.specific import (
+    controlled_section_t as controlled_section_spec_t,
+)
+from conf_ini_g.phase.specification.section.specific import (
+    free_section_t as free_section_spec_t,
 )
-from conf_ini_g.interface.screen.generic import FormattedName
-from conf_ini_g.interface.screen.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.main import parameter_t as parameter_spec_t
-from conf_ini_g.specification.section.main import controller_t
-from conf_ini_g.specification.section.main import section_t as section_spec_t
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class _base_t:  # Cannot be abstracted
+@dtcl.dataclass(repr=False, eq=False)
+class _section_t:  # Cannot be abstracted.
     HEADER_NAMES: ClassVar[tuple[str]] = (
         "Parameter",
         "Type(s)",
         "Value",
         "Unit",
     )
     HEADER_STYLE: ClassVar[str] = "background-color: darkgray; padding-left: 5px;"
 
-    library_wgt: group_wgt_h
+    spec_name: str
     formatted_name: str
+    library_wgt: group_wgt_h
 
     @classmethod
     def NewWithName(
         cls, name: str, backend: backend_t, /, *, controller: controller_t = None
-    ) -> _base_t:
+    ) -> _section_t:
         """"""
         if controller is None:
             controller = ""
         else:
-            controller = f" ⮜ {controller.section}.{controller.parameter}"
+            controller = (
+                f" ⮜ {FormattedName(controller.section, ' ')}."
+                f"{FormattedName(controller.parameter, ' ')}"
+            )
         formatted_name = FormattedName(name, " ") + controller
 
-        output = cls(library_wgt=backend.group_wgt_t(), formatted_name=formatted_name)
+        output = cls(
+            spec_name=name, formatted_name=formatted_name, library_wgt=backend.group_t()
+        )
         output.library_wgt.setTitle(formatted_name)
 
         return output
 
     @classmethod
     def Headers(cls, backend: backend_t, /) -> Sequence[label_wgt_h]:
         """"""
         output = []
 
         for text in cls.HEADER_NAMES:
-            header = backend.label_wgt_t(f'<font color="blue">{text}</font>')
+            header = backend.label_t(f'<font color="blue">{text}</font>')
             header.setStyleSheet(cls.HEADER_STYLE)
             output.append(header)
 
         return output
 
     @property
-    def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
+    def active_parameters(self) -> Sequence[parameter_t]:
         """"""
         raise NotImplementedError
 
-    @property
-    def active_parameters(self) -> dict[str, parameter_t]:
+    def AsINI(self) -> dict[str, str]:
         """"""
-        raise NotImplementedError
+        return {_elm.spec_name: _elm.Text() for _elm in self.active_parameters}
 
+
+@dtcl.dataclass(init=False, repr=False, eq=False)
+class parameters_t(list[parameter_t]):
     def __contains__(self, key: str, /) -> bool:
         """"""
-        return any(key in _set.keys() for _set in self.all_parameters)
+        return any(_elm.spec_name == key for _elm in self)
 
     def __getitem__(self, key: str, /) -> parameter_t:
         """"""
-        for parameter_set in self.all_parameters:
-            if key in parameter_set:
-                return parameter_set[key]
-
-        raise KeyError(f"{key}: Not a parameter of section {self.formatted_name}.")
+        for parameter in self:
+            if parameter.spec_name == key:
+                return parameter
 
-    def __iter__(self) -> Iterator[parameter_t]:
-        """"""
-        for parameter_set in self.all_parameters:
-            for parameter in parameter_set:
-                yield parameter
+        raise KeyError(f"{key}: Not a valid parameter.")
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class section_t(_base_t):
-    parameters: dict[str, parameter_t] = dtcl.field(init=False, default=None)
-
+@dtcl.dataclass(repr=False, eq=False)
+class free_section_t(_section_t, parameters_t):
     @classmethod
-    def NewForSection(
+    def NewForSpecification(
         cls,
-        section_spec: section_spec_t,
-        instances: dict[str, instance_t],
+        section_spec: free_section_spec_t,
         backend: backend_t,
         /,
-    ) -> section_t | None:
+    ) -> free_section_t | None:
         """"""
         output = cls.NewWithName(section_spec.name, backend)
 
-        parameters, parameter_names, layout = _ParametersFromSpecifications(
-            section_spec, instances, backend
+        parameters, _, layout = _SectionParameters(
+            section_spec, section_spec.name == INI_UNIT_SECTION, backend
         )
         if parameters.__len__() == 0:
             return None
 
-        output.parameters = dict(zip(parameter_names, parameters))
+        output.extend(parameters)
 
         for h_idx, header in enumerate(cls.Headers(backend)):
             layout.addWidget(header, 0, h_idx)
         output.library_wgt.setLayout(layout)
 
         return output
 
     @property
-    def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
+    def all_parameters(self) -> parameters_t:
         """"""
-        return (self.parameters,)
+        return self
 
     @property
-    def active_parameters(self) -> dict[str, parameter_t]:
+    def active_parameters(self) -> parameters_t:
         """"""
-        return self.parameters
+        return self
 
 
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class controlled_section_t(_base_t):
-    parameter_sets: list[dict[str, parameter_t]] = dtcl.field(init=False, default=None)
+@dtcl.dataclass(repr=False, eq=False)
+class controlled_section_t(_section_t, dict[str, parameters_t]):
+    controlling_values: list[str] = dtcl.field(init=False, default=None)
     page_stack: stack_wgt_h = dtcl.field(init=False, default=None)
 
     @classmethod
-    def NewForSection(
+    def NewForSpecification(
         cls,
-        section_spec: section_spec_t,
+        section_spec: controlled_section_spec_t,
         controller: controller_t,
-        controller_value: str,
-        instances: dict[str, instance_t],
         backend: backend_t,
         /,
     ) -> controlled_section_t | None:
         """"""
         output = cls.NewWithName(section_spec.name, backend, controller=controller)
 
-        parameter_sets = []
-        page_stack = backend.stack_wgt_t()
-        for parameter_specs in (section_spec, *section_spec.alternatives.values()):
-            parameters, parameter_names, layout = _ParametersFromSpecifications(
-                parameter_specs, instances, backend
-            )
+        controlling_values = []
+        page_stack = backend.stack_t()
+        for controlling_value, parameter_specs in section_spec.items():
+            parameters, _, layout = _SectionParameters(parameter_specs, False, backend)
             if parameters.__len__() == 0:
                 continue
 
-            parameter_sets.append(dict(zip(parameter_names, parameters)))
+            controlling_values.append(controlling_value)
+            output[controlling_value] = parameters_t(parameters)
 
             for h_idx, header in enumerate(cls.Headers(backend)):
                 layout.addWidget(header, 0, h_idx)
-            page = backend.library_wgt_t()
+            page = backend.base_t()
             page.setLayout(layout)
             page_stack.addWidget(page)
 
-        if parameter_sets.__len__() == 0:
+        if output.__len__() == 0:
             return None
 
-        output.parameter_sets = parameter_sets
+        output.controlling_values = controlling_values
         output.page_stack = page_stack
 
-        controlling_values = section_spec.controlling_values
-        page_stack.setCurrentIndex(controlling_values.index(controller_value))
-
         # Curiously, the stacked widget cannot be simply declared as child of instance;
         # This must be specified through a layout.
         layout = backend.hbox_lyt_t()
         layout.addWidget(page_stack)
         layout.setContentsMargins(0, 0, 0, 0)
         output.library_wgt.setLayout(layout)
 
         return output
 
     @property
-    def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
+    def all_parameters(self) -> parameters_t:
         """"""
-        return self.parameter_sets
+        return parameters_t(ittl.chain(*self.values()))
 
     @property
-    def active_parameters(self) -> dict[str, parameter_t]:
+    def active_parameters(self) -> parameters_t:
         """"""
-        return self.parameter_sets[self.page_stack.currentIndex()]
+        return self[self.controlling_values[self.page_stack.currentIndex()]]
+
 
+any_section_h = free_section_t | controlled_section_t
 
-def _ParametersFromSpecifications(
-    specifications: section_spec_t | Iterator[parameter_spec_t],
-    instances: dict[str, instance_t],
+
+def _SectionParameters(
+    specifications: any_section_spec_h | Iterator[parameter_spec_t],
+    section_is_unit: bool,
     backend: backend_t,
     /,
 ) -> tuple[Sequence[parameter_t], Sequence[str], grid_lyt_h]:
     """"""
     parameters = []
     parameter_names = []
 
@@ -238,20 +242,18 @@
     layout.setColumnStretch(0, 4)
     layout.setColumnStretch(1, 1)
     layout.setColumnStretch(2, 8)
     layout.setColumnStretch(3, 1)
     layout.setContentsMargins(0, 0, 0, 0)
 
     for row, parameter_spec in enumerate(specifications, start=1):
-        parameter = parameter_t.NewForParameter(
-            parameter_spec, instances[parameter_spec.name], backend
-        )
+        parameter = parameter_t.NewForSpecification(parameter_spec, backend)
         parameters.append(parameter)
         parameter_names.append(parameter_spec.name)
 
         layout.addWidget(parameter.name, row, 0, alignment=backend.ALIGNED_RIGHT)
         layout.addWidget(parameter.type, row, 1)
         layout.addWidget(parameter.value.library_wgt, row, 2, 1, 2 - 1)
-        if parameter.unit is not None:
+        if not (section_is_unit or (parameter.unit is None)):
             layout.addWidget(parameter.unit, row, 3)
 
     return parameters, parameter_names, layout
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/storage/config.py` & `conf_ini_g-2024.1/conf_ini_g/interface/storage/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,47 +25,47 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import configparser as cfpr
 import sys as sstm
-from argparse import ArgumentParser as argument_parser_t
 
-from conf_ini_g.extension.path import (
-    ValidateInputPath,
-    ValidateOutputPath,
-    any_path_h,
-    path_t,
+from conf_ini_g.extension.path import ValidateOutputPath, any_path_h, path_t
+from conf_ini_g.interface.storage.parameter import (
+    INI_COMMENT_MARKER,
+    INI_VALUE_ASSIGNMENT,
 )
-from conf_ini_g.extension.string import AsInterpretedObject
-from conf_ini_g.raw.config import AsStr, INIConfigFromINIDocument, any_raw_config_h
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.section.main import section_t
-from conf_ini_g.specification.section.unit import IsUnitSection
+from conf_ini_g.phase.generic.config import AsStr, any_dict_config_h
+from conf_ini_g.phase.specification.parameter.main import parameter_t
+from conf_ini_g.phase.specification.section.generic import section_t
+from conf_ini_g.phase.specification.section.unit import IsUnitSection
+from conf_ini_g.phase.untyped.config import ini_config_h
+from str_to_obj import ObjectFromStr
 
-SECTIONS = "SECTIONS"
+_SECTIONS = "SECTIONS"
 
 
 def DraftSpecificationFromINIDocument(path: any_path_h, /) -> str | None:
     """"""
-    ini_config = INIConfigFromINIDocument(path)
+    ini_config = INIConfig(path)
     if ini_config is None:
         return None
 
     sections = []
     for section_name, parameters in ini_config.items():
         # possibly_fuzzy=True: in case the raw config is not valid in that respect
         if IsUnitSection(section_name, possibly_fuzzy=True):
             continue
 
         parameters_as_lst = []
         for parameter_name, value_as_str in parameters.items():
-            value, _ = AsInterpretedObject(value_as_str)
+            value, _ = ObjectFromStr(value_as_str)
             parameter = (
                 f"{parameter_t.__name__}(\n"
                 f'                name="{parameter_name}",\n'
                 f"                type={type(value).__name__},\n"
                 f"            )"
             )
             parameters_as_lst.append(parameter)
@@ -79,107 +79,132 @@
             f"        ]\n"
             f"    )"
         )
         sections.append(section)
 
     imports = (
         f"# To use this specification file:\n"
-        f"#     1. import the object {SECTIONS}\n"
+        f"#     1. import the object {_SECTIONS}\n"
         f"#     2. instantiate a conf_ini_g.specification.config.config_t from it\n"
         f"from conf_ini_g.specification.parameter.main "
         f"import {parameter_t.__name__}\n"
         f"from conf_ini_g.specification.section.main import {section_t.__name__}\n"
     )
 
-    return imports + f"\n{SECTIONS} = (\n" + ",\n".join(sections) + ",\n)\n"
+    return imports + f"\n{_SECTIONS} = (\n" + ",\n".join(sections) + ",\n)\n"
 
 
-def SaveRawConfigToINIDocument(
-    config: any_raw_config_h,
+def INIConfig(ini_path: any_path_h | None, /) -> ini_config_h:
+    """"""
+    if ini_path is None:
+        ini_config = {}
+    else:
+        ini_config = cfpr.ConfigParser(
+            delimiters=INI_VALUE_ASSIGNMENT,
+            comment_prefixes=INI_COMMENT_MARKER,
+            empty_lines_in_values=False,
+            interpolation=None,
+        )
+        ini_config.optionxform = lambda option: option
+        # Returns DEFAULT <Section: DEFAULT> if path does not exist or is a folder.
+        ini_config.read(ini_path, encoding=sstm.getfilesystemencoding())
+
+    output = {
+        section: {parameter: value for parameter, value in parameters.items()}
+        for section, parameters in ini_config.items()
+        if section != cfpr.DEFAULTSECT
+    }
+
+    return output
+
+
+def SaveConfigToINIDocument(
+    config: any_dict_config_h,
     path: any_path_h,
     /,
     *,
     should_overwrite: bool = False,
     should_raise_on_error: bool = False,
-) -> str | None:
+) -> list[str]:
     """"""
     path = path_t(path)
-    error = ValidateOutputPath(
+    issues = ValidateOutputPath(
         path,
         should_overwrite=should_overwrite,
         should_raise_on_error=should_raise_on_error,
     )
-    if error is not None:
-        return error
+    if issues.__len__() > 0:
+        return issues
 
     encoding = sstm.getfilesystemencoding()
 
     with path.open("w", encoding=encoding) as ini_writer:
         print(AsStr(config), file=ini_writer)
         print(f"", file=ini_writer)
 
-    return None
-
-
-if __name__ == "__main__":
-    """
-    Run with: python -m conf_ini_g.interface.storage.config
-    from package base folder.
-    """
-    main_encoding = sstm.getfilesystemencoding()
-
-    parser = argument_parser_t(
-        prog="python -m conf_ini_g.interface.storage.config",
-        description="Display or save a draft config specification "
-        "based on an INI file.",
-        allow_abbrev=False,
-    )
-    # type=argparse.FileType() => automatic file opening
-    parser.add_argument(
-        dest="ini_path",
-        help="Input: Path to INI configuration file",
-        metavar="INI_config_file",
-    )
-    # type=argparse.FileType('w', encoding=main_encoding) => automatic creation of file
-    parser.add_argument(
-        dest="draft_specification",
-        help="Output: Path to draft config specification file. "
-        "If not passed, specification is displayed in console.",
-        default=None,
-        nargs="?",
-        metavar="draft_spec_file",
-    )
-    parser.add_argument(
-        "--overwrite",
-        dest="should_overwrite",
-        action="store_true",
-        help="Allows overwriting of draft config specification file.",
-    )
+    return []
 
-    arguments = parser.parse_args()
-    ini_path = path_t(arguments.ini_path)
-    draft_path = arguments.draft_specification
-    main_should_overwrite = arguments.should_overwrite
-
-    if (issue := ValidateInputPath(ini_path)) is not None:
-        print(issue + "\n")
-        parser.print_help()
-        sstm.exit(-1)
-
-    if draft_path is not None:
-        draft_path = path_t(draft_path)
-        issue = ValidateOutputPath(draft_path, should_overwrite=main_should_overwrite)
-        if issue is not None:
-            print(issue + "\n")
-            parser.print_help()
-            sstm.exit(-1)
-
-    draft = DraftSpecificationFromINIDocument(ini_path)
-    if draft is None:
-        print(f"{ini_path}: Not a valid INI document")
-        sstm.exit(-1)
 
-    if draft_path is None:
-        print(draft)
-    else:
-        with draft_path.open("w", encoding=main_encoding) as draft_writer:
-            draft_writer.write(draft)
+# if __name__ == "__main__":
+#     """
+#     Run with: python -m conf_ini_g.interface.storage.config
+#     from package base folder.
+#     """
+#     main_encoding = sstm.getfilesystemencoding()
+#
+#     parser = argument_parser_t(
+#         prog="python -m conf_ini_g.interface.storage.config",
+#         description="Display or save a draft config specification "
+#         "based on an INI file.",
+#         allow_abbrev=False,
+#     )
+#     # type=argparse.FileType() => automatic file opening
+#     parser.add_argument(
+#         dest="ini_path",
+#         help="Input: Path to INI configuration file",
+#         metavar="INI_config_file",
+#     )
+#     # type=argparse.FileType('w', encoding=main_encoding) => automatic creation of file
+#     parser.add_argument(
+#         dest="draft_specification",
+#         help="Output: Path to draft config specification file. "
+#         "If not passed, specification is displayed in console.",
+#         default=None,
+#         nargs="?",
+#         metavar="draft_spec_file",
+#     )
+#     parser.add_argument(
+#         "--overwrite",
+#         dest="should_overwrite",
+#         action="store_true",
+#         help="Allows overwriting of draft config specification file.",
+#     )
+#
+#     arguments = parser.parse_args()
+#     ini_path = path_t(arguments.ini_path)
+#     draft_path = arguments.draft_specification
+#     main_should_overwrite = arguments.should_overwrite
+#
+#     issues_ = ValidateInputPath(ini_path)
+#     if issues_.__len__() > 0:
+#         print("\n".join(issues_) + "\n")
+#         parser.print_help()
+#         sstm.exit(-1)
+#
+#     if draft_path is not None:
+#         draft_path = path_t(draft_path)
+#         issues_ = ValidateOutputPath(draft_path, should_overwrite=main_should_overwrite)
+#         if issues_.__len__() > 0:
+#             print("\n".join(issues_) + "\n")
+#             parser.print_help()
+#             sstm.exit(-1)
+#
+#     draft = DraftSpecificationFromINIDocument(ini_path)
+#     if draft is None:
+#         print(f"{ini_path}: Not a valid INI document")
+#         sstm.exit(-1)
+#
+#     if draft_path is None:
+#         print(draft)
+#     else:
+#         with draft_path.open("w", encoding=main_encoding) as draft_writer:
+#             draft_writer.write(draft)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/interface/storage/constant.py` & `conf_ini_g-2024.1/conf_ini_g/interface/window/config/advanced.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,8 +25,31 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-INI_COMMENT_MARKER = "#"
+from typing import Annotated, Callable
+
+from babelwidget.main import backend_t, hbox_lyt_h
+from conf_ini_g.catalog.interface.window.parameter.boolean import boolean_wgt_t
+from conf_ini_g.catalog.specification.annotation.boolean import boolean_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+
+
+def AdvancedModeLayout(
+    advanced_mode: bool, backend: backend_t, ToggleAdvancedMode: Callable, /
+) -> tuple[hbox_lyt_h, boolean_wgt_t]:
+    """"""
+    layout = backend.hbox_lyt_t()
+
+    annotated_type = Annotated[bool, boolean_t(mode=boolean_t.MODE.on_off)]
+    stripe = type_t.NewFromTypeHint(annotated_type)
+    boolean = boolean_wgt_t.NewForSpecification(stripe, backend)
+    boolean.Assign(advanced_mode, None)
+    boolean.true_btn.SetFunction(ToggleAdvancedMode)
+
+    layout.addWidget(backend.label_t("<i>Advanced Mode</i>"))
+    layout.addWidget(boolean.library_wgt)
+
+    return layout, boolean
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/light/config.py` & `conf_ini_g-2024.1/conf_ini_g/light/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -31,23 +31,22 @@
 
 from __future__ import annotations
 
 import inspect as nspt
 import sys as sstm
 from typing import Callable
 
-from rich.text import Text as text_t
-
 from conf_ini_g.extension.path import any_path_h, path_t
 from conf_ini_g.extension.string import AlignedOnSeparator
-from conf_ini_g.extension.type import NameValueTypeAsRichStr, TypeAsRichStr
-from conf_ini_g.raw.config import ini_config_h
-from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.phase.specification.parameter.type import type_t
+from conf_ini_g.phase.untyped.config import ini_config_h
+from rich.text import Text as text_t
+from str_to_obj.interface.console import NameValueTypeAsRichStr, TypeAsRichStr
 
-SECTION_PARAMETER_SEPARATOR = "__"
+_SECTION_PARAMETER_SEPARATOR = "__"
 
 
 class config_t:
     path: path_t
     _types: dict[str, type_t]
 
     @classmethod
@@ -60,15 +59,15 @@
         output = cls()
 
         if (path is not None) and isinstance(path, str):
             path = path_t(path)
 
         output.path = path
         output._types = {
-            _nme: type_t.NewFromType(_hnt)
+            _nme: type_t.NewFromTypeHint(_hnt)
             for _nme, _hnt in nspt.get_annotations(cls).items()
         }
 
         issues = []
         for s_name, section in ini_config.items():
             for p_name, value in section.items():
                 issues.extend(output.Set(_FullName(s_name, p_name), value))
@@ -79,42 +78,42 @@
             sstm.exit(1)
 
         return output
 
     def Set(self, name: str, value: str, /) -> list[str]:
         """"""
         expected_type = self._types[name]
-        typed_value, success = expected_type.InterpretedValueOf(value)
-        if success:
-            setattr(self, name, typed_value)
-            return []
-
-        return [
-            f"{value}: "
-            f'Invalid value of parameter "{name}"; '
-            f"Expected={expected_type.template_as_str}."
-        ]
+        typed_value, issues = expected_type.InterpretedValueOf(value)
+
+        if issues.__len__() > 0:
+            return [
+                f"{value}: "
+                f'Invalid value of parameter "{name}": {", ".join(issues)}.'
+            ]
+
+        setattr(self, name, typed_value)
+        return []
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
         output = [TypeAsRichStr(self)]
 
         AllButCallable = lambda _elm: not isinstance(_elm, Callable)
         for name, value in nspt.getmembers(self, AllButCallable):
             if name[0] != "_":
-                name = name.replace(SECTION_PARAMETER_SEPARATOR, ".", 1)
+                name = name.replace(_SECTION_PARAMETER_SEPARATOR, ".", 1)
                 output.append(
                     "    " + NameValueTypeAsRichStr(name, value, separator="@=@")
                 )
 
         output = AlignedOnSeparator(output, "@=@", " = ")
 
         return "\n".join(output)
 
 
 def _FullName(section: str, parameter: str, /) -> str:
     """"""
-    return f"{section.strip().lower().replace(' ', '_')}{SECTION_PARAMETER_SEPARATOR}{parameter.strip().lower()}"
+    return f"{section.strip().lower().replace(' ', '_')}{_SECTION_PARAMETER_SEPARATOR}{parameter.strip().lower()}"
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/light/conversion.py` & `conf_ini_g-2024.1/conf_ini_g/light/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from configparser import ConfigParser as config_parser_t
 
-from openpyxl import Workbook as workbook_t
-
 from conf_ini_g.extension.path import any_path_h, path_t
 from conf_ini_g.light.ini import NewConfigFromPath as NewConfigFromINIPath
 from conf_ini_g.light.xlsx import NewConfigFromPath as NewConfigFromXLSXPath
+from openpyxl import Workbook as workbook_t
 
 
 def INItoXLSX(
     ini_path: any_path_h, xlsx_path: any_path_h, /, *, should_overwrite: bool = False
 ) -> None:
     """"""
     ini_path, xlsx_path = _AsPaths(ini_path, xlsx_path)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/raw/config.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/parameter/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,107 +25,82 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import configparser as cfpr
-import sys as sstm
+import dataclasses as dtcl
+import textwrap as text
 from typing import Any
 
-from conf_ini_g.extension.path import any_path_h
-from conf_ini_g.extension.string import Flattened
-from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-
-ini_config_h = dict[str, dict[str, str]]  # Without value interpretation
-raw_config_h = dict[str, dict[str, Any]]  # With interpreted values, and possibly units
-any_raw_config_h = ini_config_h | raw_config_h
-
-
-INI_VALUE_ASSIGNMENT = "="
-
-
-def INIConfigFromINIDocument(
-    path: any_path_h,
-    /,
-    *,
-    arguments: raw_config_h = None,
-) -> ini_config_h | None:
-    """"""
-    ini_config = cfpr.ConfigParser(
-        delimiters=INI_VALUE_ASSIGNMENT,
-        comment_prefixes=INI_COMMENT_MARKER,
-        empty_lines_in_values=False,
-        interpolation=None,
-    )
-    ini_config.optionxform = lambda option: option
-    try:
-        # Returns DEFAULT <Section: DEFAULT> if path does not exist or is a folder
-        ini_config.read(path, encoding=sstm.getfilesystemencoding())
-    except cfpr.MissingSectionHeaderError:
-        return None
-
-    output = {
-        section: {parameter: value for parameter, value in parameters.items()}
-        for section, parameters in ini_config.items()
-        if section != cfpr.DEFAULTSECT
-    }
-    if arguments is not None:
-        for sct_name, parameters in arguments.items():
-            if sct_name not in output:
-                output[sct_name] = {}
-            for prm_name, value in parameters.items():
-                output[sct_name][prm_name] = value
-
-    if output.__len__() == 0:
-        return None
-
-    return output
-
-
-def AsStr(config: any_raw_config_h, /, *, in_html_format: bool = False) -> str:
-    """"""
-    output = []
-
-    if in_html_format:
-        section_color = '<span style="color:green">'
-        parameter_color = '<span style="color:blue">'
-        color_reset = "</span>"
-        newline = "<br/>"
-        indentation = "&nbsp;"
-    else:
-        section_color = "[green]"
-        parameter_color = "[blue]"
-        color_reset = "[/]"
-        newline = "\n"
-        indentation = " "
-
-    longest = 0
-    for section, parameters in config.items():
-        if parameters.__len__() == 0:
-            continue
-
-        inner_output = []
-        lengths = []
-        for name, value in parameters.items():
-            length = name.__len__()
-            lengths.append(length)
-            longest = max(longest, length)
-
-            flattened = Flattened(str(value))
-            inner_output.append(f"{parameter_color}{name}{color_reset}@= {flattened}")
-
-        output.append(
-            (f"{section_color}[{section}]{color_reset}", inner_output, lengths)
-        )
-
-    output = (
-        f"{_sct}{newline}"
-        + newline.join(
-            _lne.replace("@", (longest - _lgt + 1) * indentation, 1)
-            for _lne, _lgt in zip(_prm, _lgs)
-        )
-        for _sct, _prm, _lgs in output
-    )
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.phase.specification.base import base_t
+from conf_ini_g.phase.specification.parameter.type import ANY_TYPE, type_t
+from conf_ini_g.phase.specification.parameter.value import MISSING_REQUIRED_VALUE
+from issue_manager import ISSUE_MANAGER
+from str_to_obj import CastValue
+from str_to_obj.interface.console import NameValueTypeAsRichStr, TypeAsRichStr
+from str_to_obj.type.hint import any_hint_h
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class parameter_t(base_t):
+    """
+    type:
+        At instantiation time:
+            - any_hint_h, if passed
+            - type_t (ANY_TYPE), if not.
+        After __post_init__: type_t
+    """
+
+    type: any_hint_h | type_t = ANY_TYPE
+    default: Any = MISSING_REQUIRED_VALUE
+
+    def __post_init__(self) -> None:
+        """"""
+        if not isinstance(self.type, type_t):
+            self.type = type_t.NewFromTypeHint(self.type)
+
+        with ISSUE_MANAGER.AddedContextLevel(
+            f'Specification of {type(self).__name__} "{self.name}"'
+        ):
+            if self.optional:
+                if self.default is MISSING_REQUIRED_VALUE:
+                    ISSUE_MANAGER.Add(
+                        "Invalid default value",
+                        actual=MISSING_REQUIRED_VALUE,
+                        expected="an explicit value",
+                    )
+                else:
+                    converted, issues = CastValue(self.default, self.type)
+                    if issues.__len__() > 0:
+                        issues = ", ".join(issues)
+                        ISSUE_MANAGER.Add(f"Invalid default value: {issues}")
+                    else:
+                        self.default = converted
+            else:
+                if not self.basic:
+                    ISSUE_MANAGER.Add("Parameter is not basic but not optional")
+                if self.default is not MISSING_REQUIRED_VALUE:
+                    ISSUE_MANAGER.Add(
+                        "Mandatory parameter with an explicit default value"
+                    )
+
+    @property
+    def optional(self) -> bool:
+        """"""
+        return self.default is not MISSING_REQUIRED_VALUE
+
+    def __rich__(self) -> str:
+        """"""
+        output = [
+            TypeAsRichStr(self),
+            *text.indent(super().__rich__(), "    ").splitlines(),
+            f"    [blue]Template[/]@=@{self.type.__rich__()}",
+            f"    {NameValueTypeAsRichStr('Default', self.default, separator='@=@')}",
+            f"    [blue]Optional[/]@=@{self.optional}",
+        ]
 
-    return f"{newline}{newline}".join(output)
+        output = AlignedOnSeparator(output, "@=@", " = ")
+
+        return "\n".join(output)
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/specification/base.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -28,46 +28,52 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import string as strg
 
+from issue_manager import ISSUE_MANAGER
 from rich.text import Text as text_t
 
-WORD_SEPARATOR = "_"
-VALID_CHARACTERS = strg.ascii_letters + strg.digits + WORD_SEPARATOR
+# Must not be <space> to allow assignment through command-line arguments.
+_WORD_SEPARATOR = "_"
+_VALID_CHARACTERS = strg.ascii_letters + strg.digits + _WORD_SEPARATOR
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(repr=False, eq=False)  # Do not use slots here, only on last class.
 class base_t:
     name: str
     definition: str = "No Definition Provided"
     description: str = "No Description Provided"
     basic: bool = True
 
-    def Issues(self) -> list[str]:
+    def __post_init__(self) -> None:
         """"""
-        output = []
-
-        if any(_chr not in VALID_CHARACTERS for _chr in self.name):
-            output.append(
-                f"{self.name}: Name contains invalid characters; "
-                f"Valid={VALID_CHARACTERS}"
-            )
-        if not isinstance(self.definition, str):
-            output.append(
-                f'{self.definition}: Not a valid string for definition of "{self.name}"'
-            )
-        if not isinstance(self.description, str):
-            output.append(
-                f'{self.description}: Not a valid string for description of "{self.name}"'
-            )
-
-        return output
+        with ISSUE_MANAGER.AddedContextLevel(
+            f'Specification of {type(self).__name__} "{self.name}"'
+        ):
+            if any(_chr not in _VALID_CHARACTERS for _chr in self.name):
+                ISSUE_MANAGER.Add(
+                    "Name contains invalid characters",
+                    actual=self.name,
+                    expected=f"name with characters from: {_VALID_CHARACTERS}",
+                )
+            if not isinstance(self.definition, str):
+                ISSUE_MANAGER.Add(
+                    f"Invalid type of definition",
+                    actual=type(self.definition).__name__,
+                    expected="str",
+                )
+            if not isinstance(self.description, str):
+                ISSUE_MANAGER.Add(
+                    f"Invalid type of description",
+                    actual=type(self.description).__name__,
+                    expected="str",
+                )
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/specification/config.py` & `conf_ini_g-2024.1/conf_ini_g/phase/specification/section/generic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,168 +25,125 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
 import dataclasses as dtcl
-import textwrap as text
-from typing import Sequence
-
-from rich import print as rprint
-from rich.text import Text as text_t
 
-from conf_ini_g.catalog.specification.parameter.choices import choices_t
-from conf_ini_g.extension.python import SpecificationPath
-from conf_ini_g.extension.type import TypeAsRichStr
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
-from conf_ini_g.specification.section.main import section_t
-from conf_ini_g.specification.section.unit import UNIT_SECTION
-
-
-@dtcl.dataclass(init=False, repr=False, eq=False)
-class config_t(list[section_t]):
-    spec_path: str = None
-
-    def __init__(self, sections: Sequence[section_t], /) -> None:
-        """
-        Raising exceptions is adapted here since execution cannot proceed without a
-        valid specification.
-        """
-        list.__init__(self, sections)
-        self._SetControllerChoices()  # After __init__ so that self iterator is usable
-        self.spec_path = SpecificationPath(sections)
-
-        issues = self.Issues()
-        if issues.__len__() > 0:
-            rprint(
-                self.spec_path,
-                "[red]Invalid specification[/]",
-                "\n".join(issues),
-                sep="\n",
-            )
-            raise ValueError
+from conf_ini_g.phase.specification.base import base_t
+from conf_ini_g.phase.specification.parameter.main import parameter_t
+from conf_ini_g.phase.specification.section.controller import controller_t
+from issue_manager import ISSUE_MANAGER
+
+
+@dtcl.dataclass(repr=False, eq=False)
+class section_t(base_t):
+    category: str = "Main"
+    optional: bool = False
+    is_growable: bool = False  # True by default if no parameters are specified.
+    parameters: list[parameter_t] | None = None
+    controller: controller_t = None
+    alternatives: dict[str, list[parameter_t]] = None
 
-    def _SetControllerChoices(self) -> None:
+    def __post_init__(self) -> None:
         """"""
-        for section in self:
-            if (controller := section.controller) is None:
-                continue
-
-            controlling_parameter = self[controller.section][controller.parameter]
-            controlling_parameter.type = type_t.NewFromType(
-                choices_t.NewAnnotatedType(section.controlling_values)
-            )
+        if self.parameters is None:
+            self.is_growable = True
 
-    def AddUnitSection(self) -> None:
-        """"""
-        section = section_t(
-            name=UNIT_SECTION,
-            definition="Unit definitions",
-            description=f"Units can be used in any other section "
-            f"to specify a parameter value as follows: "
-            f"numerical_value{UNIT_SEPARATOR}unit, e.g., 1.5'mm.",
-            basic=True,
-            optional=True,
-            category=UNIT_SECTION,
-            is_growable=True,
-        )
-        self.append(section)
+        _SignalIssues(self)
 
     @property
-    def section_names(self) -> Sequence[str]:
-        """"""
-        return tuple(_sct.name for _sct in self)
-
-    def Issues(self) -> list[str]:
-        """"""
-        output = []
-
-        if self.__len__() == 0:
-            output.append("spec_path: Empty specification")
-            return output
-
-        names = self.section_names
-        if names.__len__() > set(names).__len__():
-            output.append("Specification with repeated section names")
-
-        for section in self:
-            if not isinstance(section, section_t):
-                output.append(
-                    f"{type(section).__name__}: Invalid section type; Expected={section_t.__name__}."
-                )
-                continue
-
-            output.extend(section.Issues())
-            if section.controller is not None:
-                if section.controller.section not in self:
-                    output.append(
-                        f"{section.controller.section}: "
-                        f'Unspecified section declared as controller of section "{section.name}"'
+    def controlling_values(self) -> tuple[str, ...]:
+        """
+        Call only on controlled sections.
+        """
+        if self.controller.primary_value is None:
+            # The controlling values are not mentioned in the specification. They will
+            # be set programmatically later on.
+            return ()
+
+        if self.alternatives is None:
+            # The controlling values are not mentioned in the specification. They are
+            # being set programmatically.
+            return (self.controller.primary_value,)
+
+        return (self.controller.primary_value,) + tuple(self.alternatives.keys())
+
+
+def _SignalIssues(self) -> None:
+    """"""
+    with ISSUE_MANAGER.AddedContextLevel(
+        f'Specification of {type(self).__name__} "{self.name}"'
+    ):
+        if self.parameters is not None:
+            valid_name_sets = [tuple(_prm.name for _prm in self.parameters)]
+            if self.alternatives is not None:
+                for parameters in self.alternatives.values():
+                    valid_name_sets.append(tuple(_prm.name for _prm in parameters))
+            for valid_name_set in valid_name_sets:
+                if valid_name_set.__len__() > set(valid_name_set).__len__():
+                    ISSUE_MANAGER.Add(
+                        "Repeated parameter names (possibly in alternatives)"
                     )
-                else:
-                    controller_section = self[section.controller.section]
-                    if controller_section.controller is not None:
-                        output.append(
-                            f"{section.controller.section}: "
-                            f'Section controlling "{section.name}" is itself controlled'
-                        )
-                    if section.controller.parameter not in controller_section:
-                        output.append(
-                            f"{section.controller.section}.{section.controller.parameter}: "
-                            f'Unspecified parameter declared as controller of section "{section.name}"'
-                        )
-                    else:
-                        controller_parameter = controller_section[
-                            section.controller.parameter
-                        ]
-                        if controller_parameter.optional:
-                            output.append(
-                                f"{section.controller.section}.{section.controller.parameter}: "
-                                f'Optional parameter declared as controller of section "{section.name}"'
-                            )
 
-        return output
+        basic = self.basic
+        optional = self.optional
 
-    def _Item(self, key: str | int, /) -> section_t | None:
-        """"""
-        if isinstance(key, int):
-            return list.__getitem__(self, key)
-
-        for section in self:
-            if section.name == key:
-                return section
-
-        return None
-
-    def __contains__(self, key: str, /) -> bool:
-        """"""
-        return self._Item(key) is not None
-
-    def __getitem__(self, key: str | int, /) -> section_t:
-        """"""
-        item = self._Item(key)
-        if item is None:
-            raise KeyError(f"{key}: Not a section of config.")
-
-        return item
+        if not (basic or optional):
+            ISSUE_MANAGER.Add("Section is not basic but not optional")
 
-    def __str__(self) -> str:
-        """"""
-        return text_t.from_markup(self.__rich__()).plain
-
-    def __rich__(self) -> str:
-        """"""
-        output = [
-            TypeAsRichStr(self),
-            f"    [blue]spec_path[/]={self.spec_path}"
-            f"[yellow]:{type(self.spec_path).__name__}[/]",
-        ]
+        if (
+            (self.controller is None)
+            and (not optional)
+            and ((self.parameters is None) or (self.parameters.__len__() == 0))
+        ):
+            ISSUE_MANAGER.Add("Empty mandatory section")
+
+        if self.parameters is not None:
+            n_parameters = 0
+            n_basic_prms = 0
+            for parameter in self.parameters:
+                n_parameters += 1
+                if parameter.basic:
+                    n_basic_prms += 1
+
+                if parameter.basic and not basic:
+                    ISSUE_MANAGER.Add(
+                        f'Basic parameter "{parameter.name}" in advanced section'
+                    )
+                if optional and not parameter.optional:
+                    ISSUE_MANAGER.Add(
+                        f'Mandatory parameter "{parameter.name}" in optional section'
+                    )
 
-        for section in self:
-            output.append(text.indent(section.__rich__(), "    "))
+            if (n_parameters == 0) and not self.is_growable:
+                ISSUE_MANAGER.Add("Empty section not accepting runtime parameters")
+            if basic and (n_parameters > 0) and (n_basic_prms == 0):
+                ISSUE_MANAGER.Add("Basic section without any basic parameters")
+
+        if self.controller is None:
+            if self.alternatives is not None:
+                ISSUE_MANAGER.Add("Uncontrolled section with alternatives")
+        else:
+            if self.controller.section == self.name:
+                ISSUE_MANAGER.Add("Section controlled by itself")
+            controlling_values = self.controlling_values
+            if controlling_values.__len__() > set(controlling_values).__len__():
+                ISSUE_MANAGER.Add(
+                    "Controlled section with duplicated controlling values"
+                )
+            if self.parameters is not None:
+                for parameter in self.parameters:
+                    if not parameter.optional:
+                        ISSUE_MANAGER.Add(
+                            f'Mandatory parameter "{parameter.name}" in '
+                            f"controlled section"
+                        )
 
-        return "\n".join(output)
+            if self.controller.primary_value is None:
+                if self.alternatives is not None:
+                    ISSUE_MANAGER.Add("Controlled section without primary value")
+                # else: This will be set programmatically later on.
+            elif self.alternatives is None:
+                ISSUE_MANAGER.Add("Controlled section without alternatives")
```

### Comparing `conf-ini-g-2023.9/conf_ini_g/specification/parameter/unit.py` & `conf_ini_g-2024.1/conf_ini_g/phase/untyped/section.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright CNRS/Inria/UNS
+# Copyright CNRS/Inria/UniCA
 # Contributor(s): Eric Debreuve (since 2021)
 #
 # eric.debreuve@cnrs.fr
 #
 # This software is governed by the CeCILL  license under French law and
 # abiding by the rules of distribution of free software.  You can  use,
 # modify and/ or redistribute the software under the terms of the CeCILL
@@ -25,22 +25,16 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
 from math import pi as PI
 
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-
-UNIT_SEPARATOR = ":IN:"
-
 _STD_UNIT_CONVERSIONS = (
     # unit, unit name, parent unit (None if none), conversion factor (1.0 if None)
     ("si", "site", None, 1.0),  # Synonym for sample, pixel, voxel...
     #
     ("km", "kilometer", "m", 1000.0),
     ("m", "meter", "si", 1.0),
     ("cm", "centimeter", "m", 1.0e-2),
@@ -61,31 +55,7 @@
     ("mn", "minute", "s", 60.0),
     ("s", "second", "si", 1.0),
     ("ms", "millisecond", "s", 1.0e-3),
     ("us", "microsecond", "s", 1.0e-6),
     ("ns", "nanosecond", "s", 1.0e-9),
 )
 STD_UNIT_CONVERSIONS = {_elm[0]: _elm[-1] for _elm in _STD_UNIT_CONVERSIONS}
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class unit_t(parameter_t):
-    def __post_init__(self) -> None:
-        """
-        Unit parameter are never part of a specification. They can appear in INI
-        documents, and are therefore only instantiated programmatically.
-        """
-        self.type = type_t.NewFromType(float)
-
-    def Issues(self) -> list[str]:
-        """"""
-        if self.name in STD_UNIT_CONVERSIONS.keys():
-            return [
-                f"{self.name}: Redefinition of a standard unit; Please use another unit name."
-            ]
-
-        return []
-
-    @property
-    def optional(self) -> bool:
-        """"""
-        return True
```

### Comparing `conf-ini-g-2023.9/conf_ini_g.egg-info/PKG-INFO` & `conf_ini_g-2024.1/conf_ini_g.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.9
+Version: 2024.1
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
@@ -12,14 +12,19 @@
 Classifier: Topic :: Software Development
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+Requires-Dist: babelwidget
+Requires-Dist: issue-manager
+Requires-Dist: openpyxl
+Requires-Dist: rich
+Requires-Dist: str-to-obj
 
 ..
    Copyright CNRS/Inria/UCA
    Contributor(s): Eric Debreuve (since 2021)
 
    eric.debreuve@cnrs.fr
```

### Comparing `conf-ini-g-2023.9/conf_ini_g.egg-info/SOURCES.txt` & `conf_ini_g-2024.1/conf_ini_g.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,71 +7,64 @@
 conf_ini_g/__init__.py
 conf_ini_g/version.py
 conf_ini_g.egg-info/PKG-INFO
 conf_ini_g.egg-info/SOURCES.txt
 conf_ini_g.egg-info/dependency_links.txt
 conf_ini_g.egg-info/requires.txt
 conf_ini_g.egg-info/top_level.txt
-conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
-conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
-conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
-conf_ini_g/catalog/interface/screen/parameter/boolean.py
-conf_ini_g/catalog/interface/screen/parameter/choices.py
-conf_ini_g/catalog/interface/screen/parameter/directory.py
-conf_ini_g/catalog/interface/screen/parameter/multitype.py
-conf_ini_g/catalog/interface/screen/parameter/none.py
-conf_ini_g/catalog/interface/screen/parameter/path.py
-conf_ini_g/catalog/interface/screen/parameter/sequence.py
-conf_ini_g/catalog/interface/screen/parameter/text.py
-conf_ini_g/catalog/specification/parameter/boolean.py
-conf_ini_g/catalog/specification/parameter/choices.py
-conf_ini_g/catalog/specification/parameter/number.py
-conf_ini_g/catalog/specification/parameter/path.py
-conf_ini_g/catalog/specification/parameter/sequence.py
+conf_ini_g/catalog/interface/window/parameter/boolean.py
+conf_ini_g/catalog/interface/window/parameter/callable.py
+conf_ini_g/catalog/interface/window/parameter/choices.py
+conf_ini_g/catalog/interface/window/parameter/collection.py
+conf_ini_g/catalog/interface/window/parameter/directory.py
+conf_ini_g/catalog/interface/window/parameter/multitype.py
+conf_ini_g/catalog/interface/window/parameter/none.py
+conf_ini_g/catalog/interface/window/parameter/path.py
+conf_ini_g/catalog/interface/window/parameter/text_line.py
+conf_ini_g/catalog/specification/annotation/boolean.py
+conf_ini_g/catalog/specification/annotation/callable.py
+conf_ini_g/catalog/specification/annotation/choices.py
+conf_ini_g/catalog/specification/annotation/collection.py
+conf_ini_g/catalog/specification/annotation/number.py
+conf_ini_g/catalog/specification/annotation/path.py
 conf_ini_g/extension/path.py
 conf_ini_g/extension/python.py
 conf_ini_g/extension/string.py
-conf_ini_g/extension/type.py
-conf_ini_g/instance/config.py
-conf_ini_g/instance/parameter/base.py
-conf_ini_g/instance/parameter/main.py
-conf_ini_g/instance/parameter/unit.py
-conf_ini_g/interface/console/__init__.py
+conf_ini_g/interface/constant.py
 conf_ini_g/interface/console/config.py
-conf_ini_g/interface/screen/backend.py
-conf_ini_g/interface/screen/config.py
-conf_ini_g/interface/screen/generic.py
-conf_ini_g/interface/screen/section.py
-conf_ini_g/interface/screen/parameter/main.py
-conf_ini_g/interface/screen/parameter/path_chooser.py
 conf_ini_g/interface/storage/config.py
-conf_ini_g/interface/storage/constant.py
+conf_ini_g/interface/storage/parameter.py
+conf_ini_g/interface/storage/section.py
+conf_ini_g/interface/window/generic.py
+conf_ini_g/interface/window/config/action.py
+conf_ini_g/interface/window/config/advanced.py
+conf_ini_g/interface/window/config/main.py
+conf_ini_g/interface/window/config/title.py
+conf_ini_g/interface/window/parameter/main.py
+conf_ini_g/interface/window/parameter/type.py
+conf_ini_g/interface/window/parameter/value.py
+conf_ini_g/interface/window/section/collection.py
+conf_ini_g/interface/window/section/main.py
 conf_ini_g/light/config.py
 conf_ini_g/light/conversion.py
 conf_ini_g/light/ini.py
 conf_ini_g/light/xlsx.py
-conf_ini_g/raw/config.py
-conf_ini_g/specification/base.py
-conf_ini_g/specification/config.py
-conf_ini_g/specification/parameter/annotation.py
-conf_ini_g/specification/parameter/main.py
-conf_ini_g/specification/parameter/type.py
-conf_ini_g/specification/parameter/unit.py
-conf_ini_g/specification/parameter/value.py
-conf_ini_g/specification/section/main.py
-conf_ini_g/specification/section/unit.py
+conf_ini_g/phase/generic/config.py
+conf_ini_g/phase/specification/base.py
+conf_ini_g/phase/specification/config/main.py
+conf_ini_g/phase/specification/parameter/main.py
+conf_ini_g/phase/specification/parameter/type.py
+conf_ini_g/phase/specification/parameter/unit.py
+conf_ini_g/phase/specification/parameter/value.py
+conf_ini_g/phase/specification/section/controller.py
+conf_ini_g/phase/specification/section/generic.py
+conf_ini_g/phase/specification/section/specific.py
+conf_ini_g/phase/specification/section/unit.py
+conf_ini_g/phase/typed/config/main.py
+conf_ini_g/phase/typed/parameter/invalid.py
+conf_ini_g/phase/typed/parameter/main.py
+conf_ini_g/phase/typed/parameter/unit.py
+conf_ini_g/phase/typed/section/units.py
+conf_ini_g/phase/untyped/config.py
+conf_ini_g/phase/untyped/parameter.py
+conf_ini_g/phase/untyped/section.py
 documentation/wiki/description.asciidoc
```

### Comparing `conf-ini-g-2023.9/setup.py` & `conf_ini_g-2024.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import re as rgex
 from pathlib import Path as path_t
 
 from setuptools import setup
 
-
 HERE = path_t(__file__).parent.resolve()
 DOCUMENTATION_HOME = HERE / "documentation" / "wiki" / "description.asciidoc"
 
 
 def DescriptionFromDocumentation(documentation: path_t, /) -> dict[str, str]:
     """"""
     output = {}
@@ -70,36 +69,38 @@
 PYPI_STATUS = "4 - Beta"
 
 IMPORT_NAME = "conf_ini_g"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
     f"{IMPORT_NAME}.catalog.interface",
-    f"{IMPORT_NAME}.catalog.interface.screen",
-    f"{IMPORT_NAME}.catalog.interface.screen.library",
-    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5",
-    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5.widget",
-    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt6",
-    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt6.widget",
-    f"{IMPORT_NAME}.catalog.interface.screen.parameter",
+    f"{IMPORT_NAME}.catalog.interface.window",
+    f"{IMPORT_NAME}.catalog.interface.window.parameter",
     f"{IMPORT_NAME}.catalog.specification",
-    f"{IMPORT_NAME}.catalog.specification.parameter",
+    f"{IMPORT_NAME}.catalog.specification.annotation",
     f"{IMPORT_NAME}.extension",
-    f"{IMPORT_NAME}.instance",
-    f"{IMPORT_NAME}.instance.parameter",
     f"{IMPORT_NAME}.interface",
     f"{IMPORT_NAME}.interface.console",
-    f"{IMPORT_NAME}.interface.screen",
-    f"{IMPORT_NAME}.interface.screen.parameter",
     f"{IMPORT_NAME}.interface.storage",
+    f"{IMPORT_NAME}.interface.window",
+    f"{IMPORT_NAME}.interface.window.config",
+    f"{IMPORT_NAME}.interface.window.parameter",
+    f"{IMPORT_NAME}.interface.window.section",
     f"{IMPORT_NAME}.light",
-    f"{IMPORT_NAME}.raw",
-    f"{IMPORT_NAME}.specification",
-    f"{IMPORT_NAME}.specification.parameter",
-    f"{IMPORT_NAME}.specification.section",
+    f"{IMPORT_NAME}.phase",
+    f"{IMPORT_NAME}.phase.generic",
+    f"{IMPORT_NAME}.phase.specification",
+    f"{IMPORT_NAME}.phase.specification.config",
+    f"{IMPORT_NAME}.phase.specification.parameter",
+    f"{IMPORT_NAME}.phase.specification.section",
+    f"{IMPORT_NAME}.phase.typed",
+    f"{IMPORT_NAME}.phase.typed.config",
+    f"{IMPORT_NAME}.phase.typed.parameter",
+    f"{IMPORT_NAME}.phase.typed.section",
+    f"{IMPORT_NAME}.phase.untyped",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
     f"{IMPORT_NAME}.test",
 )
 ENTRY_POINTS = {}
 
@@ -128,16 +129,18 @@
                 folders.append(node)
     folders = sorted(folders)
 
     packages = sorted(PACKAGES)
     if packages != folders:
         raise ValueError(
             f"Mismatch between declared and found packages:\n"
-            f"    - Declared=\n      {packages};\n"
-            f"    - Found=\n      {folders}."
+            f"    - Declared=\n      {packages}\n"
+            f"    - Found=\n      {folders}\n"
+            f"    - Undeclared=\n      {set(folders).difference(packages)}\n"
+            f"    - Nonexistent=\n      {set(packages).difference(folders)}"
         )
 
 
 def Version():
     """"""
     contents = {}
     with open(HERE / IMPORT_NAME / "version.py") as accessor:
@@ -180,11 +183,14 @@
             "Source": repository_url,
         },
         #
         packages=PACKAGES,
         entry_points=ENTRY_POINTS,
         python_requires=f">={PY_VERSION}",
         install_requires=[
-            "rich",
+            "babelwidget",
+            "issue-manager",
             "openpyxl",
+            "rich",
+            "str-to-obj",
         ],
     )
```

