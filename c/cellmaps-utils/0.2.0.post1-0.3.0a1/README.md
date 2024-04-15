# Comparing `tmp/cellmaps_utils-0.2.0.post1.tar.gz` & `tmp/cellmaps_utils-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.2.0.post1.tar", last modified: Wed Feb 28 22:25:38 2024, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.3.0a1.tar", last modified: Mon Apr 15 16:40:46 2024, max compression
```

## Comparing `cellmaps_utils-0.2.0.post1.tar` & `cellmaps_utils-0.3.0a1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.831871 cellmaps_utils-0.2.0.post1/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-14 17:52:02.000000 cellmaps_utils-0.2.0.post1/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)      603 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5713 2024-02-28 22:25:38.832027 cellmaps_utils-0.2.0.post1/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3318 2024-02-28 22:23:22.000000 cellmaps_utils-0.2.0.post1/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.820849 cellmaps_utils-0.2.0.post1/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      284 2024-02-28 22:24:04.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)    10959 2023-09-01 00:16:37.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/apmstool.py
--rw-r--r--   0 churas     (504) staff       (20)     2150 2023-09-01 00:16:37.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/basecmdtool.py
--rw-r--r--   0 churas     (504) staff       (20)     4303 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/cellmaps_utilscmd.py
--rw-r--r--   0 churas     (504) staff       (20)     5535 2023-12-22 18:02:22.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)    18061 2023-09-01 00:16:37.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/crisprtool.py
--rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    23380 2023-09-01 00:16:37.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/iftool.py
--rw-r--r--   0 churas     (504) staff       (20)     8281 2023-10-05 22:24:13.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/music_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    35908 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/provenance.py
--rw-r--r--   0 churas     (504) staff       (20)    13341 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils/tabletool.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.822967 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5713 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1256 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       64 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2024-02-28 22:25:38.000000 cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.828799 cellmaps_utils-0.2.0.post1/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.812619 cellmaps_utils-0.2.0.post1/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.812737 cellmaps_utils-0.2.0.post1/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.829918 cellmaps_utils-0.2.0.post1/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.2.0.post1/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.2.0.post1/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.2.0.post1/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1187 2023-12-22 18:02:22.000000 cellmaps_utils-0.2.0.post1/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5985 2023-08-17 22:56:58.000000 cellmaps_utils-0.2.0.post1/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-09-01 00:17:50.000000 cellmaps_utils-0.2.0.post1/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1064 2024-02-28 22:24:04.000000 cellmaps_utils-0.2.0.post1/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)      123 2023-11-02 21:07:52.000000 cellmaps_utils-0.2.0.post1/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      826 2023-12-22 18:02:22.000000 cellmaps_utils-0.2.0.post1/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)     8820 2023-12-22 18:02:22.000000 cellmaps_utils-0.2.0.post1/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2024-02-28 22:25:38.832486 cellmaps_utils-0.2.0.post1/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2410 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-02-28 22:25:38.831605 cellmaps_utils-0.2.0.post1/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.2.0.post1/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1015 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/tests/test_basecommandlinetool.py
--rw-r--r--   0 churas     (504) staff       (20)      836 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/tests/test_helloworldcommand.py
--rw-r--r--   0 churas     (504) staff       (20)     6483 2023-12-22 18:02:22.000000 cellmaps_utils-0.2.0.post1/tests/test_integation_provenance.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.2.0.post1/tests/test_logutils.py
--rw-r--r--   0 churas     (504) staff       (20)    34840 2024-02-20 22:35:20.000000 cellmaps_utils-0.2.0.post1/tests/test_provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.455752 cellmaps_utils-0.3.0a1/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-14 17:52:02.000000 cellmaps_utils-0.3.0a1/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)      692 2024-04-15 16:39:05.000000 cellmaps_utils-0.3.0a1/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5846 2024-04-15 16:40:46.456040 cellmaps_utils-0.3.0a1/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3318 2024-03-13 21:17:30.000000 cellmaps_utils-0.3.0a1/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.434502 cellmaps_utils-0.3.0a1/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      280 2024-04-15 16:36:22.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    10959 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/apmstool.py
+-rw-r--r--   0 churas     (504) staff       (20)     2150 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/basecmdtool.py
+-rw-r--r--   0 churas     (504) staff       (20)     4303 2024-02-20 22:35:20.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/cellmaps_utilscmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     5535 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)    18061 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/crisprtool.py
+-rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    23380 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/iftool.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-10-05 22:24:13.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/music_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    35908 2024-02-20 22:35:20.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/provenance.py
+-rw-r--r--   0 churas     (504) staff       (20)    13341 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/cellmaps_utils/tabletool.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.437067 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5846 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1256 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       63 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2024-04-15 16:40:46.000000 cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.448571 cellmaps_utils-0.3.0a1/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.425781 cellmaps_utils-0.3.0a1/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.425943 cellmaps_utils-0.3.0a1/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.450501 cellmaps_utils-0.3.0a1/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.3.0a1/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.3.0a1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.3.0a1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1187 2023-12-22 18:02:22.000000 cellmaps_utils-0.3.0a1/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6020 2024-03-13 21:17:40.000000 cellmaps_utils-0.3.0a1/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-09-01 00:17:50.000000 cellmaps_utils-0.3.0a1/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1064 2024-03-13 21:17:30.000000 cellmaps_utils-0.3.0a1/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)      123 2023-11-02 21:07:52.000000 cellmaps_utils-0.3.0a1/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      826 2023-12-22 18:02:22.000000 cellmaps_utils-0.3.0a1/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)     8820 2023-12-22 18:02:22.000000 cellmaps_utils-0.3.0a1/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2024-04-15 16:40:46.456834 cellmaps_utils-0.3.0a1/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2409 2024-04-15 16:33:58.000000 cellmaps_utils-0.3.0a1/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2024-04-15 16:40:46.454666 cellmaps_utils-0.3.0a1/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.3.0a1/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1015 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/tests/test_basecommandlinetool.py
+-rw-r--r--   0 churas     (504) staff       (20)      836 2024-02-20 22:35:20.000000 cellmaps_utils-0.3.0a1/tests/test_helloworldcommand.py
+-rw-r--r--   0 churas     (504) staff       (20)     6483 2024-04-15 16:33:26.000000 cellmaps_utils-0.3.0a1/tests/test_integation_provenance.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.3.0a1/tests/test_logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)    34840 2024-02-20 22:35:20.000000 cellmaps_utils-0.3.0a1/tests/test_provenance.py
```

### Comparing `cellmaps_utils-0.2.0.post1/CONTRIBUTING.rst` & `cellmaps_utils-0.3.0a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/LICENSE` & `cellmaps_utils-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/PKG-INFO` & `cellmaps_utils-0.3.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_utils
-Version: 0.2.0.post1
+Version: 0.3.0a1
 Summary: Contains utilities needed by Cell Maps tools
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Cell Maps team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =============================
         Cell Maps Pipeline Utilities
@@ -117,14 +117,20 @@
         
         
         
         =======
         History
         =======
         
+        0.3.0 (2024-04-15)
+        -------------------
+        
+        * Bumped fairscape-cli dependency to ``0.2.0``
+        
+        
         0.2.0 (2024-02-20)
         ------------------
         
         * Bumped fairscape-cli dependency to ``0.1.14`` to support schemas
         
         * Added support for ``schema`` to **data_dict** parameter in ``ProvenanceUtil.register_dataset()``
```

### Comparing `cellmaps_utils-0.2.0.post1/README.rst` & `cellmaps_utils-0.3.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/apmstool.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/apmstool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/basecmdtool.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/basecmdtool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/cellmaps_utilscmd.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/cellmaps_utilscmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/constants.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/crisprtool.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/crisprtool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/iftool.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/iftool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/logutils.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/provenance.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/provenance.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils/tabletool.py` & `cellmaps_utils-0.3.0a1/cellmaps_utils/tabletool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-utils
-Version: 0.2.0.post1
+Version: 0.3.0a1
 Summary: Contains utilities needed by Cell Maps tools
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Cell Maps team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =============================
         Cell Maps Pipeline Utilities
@@ -117,14 +117,20 @@
         
         
         
         =======
         History
         =======
         
+        0.3.0 (2024-04-15)
+        -------------------
+        
+        * Bumped fairscape-cli dependency to ``0.2.0``
+        
+        
         0.2.0 (2024-02-20)
         ------------------
         
         * Bumped fairscape-cli dependency to ``0.1.14`` to support schemas
         
         * Added support for ``schema`` to **data_dict** parameter in ``ProvenanceUtil.register_dataset()``
```

### Comparing `cellmaps_utils-0.2.0.post1/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.3.0a1/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/Makefile` & `cellmaps_utils-0.3.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/cellmaps_utils.rst` & `cellmaps_utils-0.3.0a1/docs/cellmaps_utils.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/conf.py` & `cellmaps_utils-0.3.0a1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.intersphinx',
               'sphinx.ext.autosectionlabel',
-              'sphinx.ext.viewcode']
+              'sphinx.ext.viewcode',
+              'sphinx_copybutton']
 
 # intersphinx mapping
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None),
                        "requests": ("https://requests.readthedocs.io/en/latest/", None),
                        "networkx": ("http://networkx.org/documentation/stable/", None),
                        "pandas": ("https://pandas.pydata.org/docs/", None),
                        "numpy": ("https://numpy.org/doc/stable/", None)
```

### Comparing `cellmaps_utils-0.2.0.post1/docs/index.rst` & `cellmaps_utils-0.3.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/installation.rst` & `cellmaps_utils-0.3.0a1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/make.bat` & `cellmaps_utils-0.3.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/newrelease.rst` & `cellmaps_utils-0.3.0a1/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/pypircfile.rst` & `cellmaps_utils-0.3.0a1/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/usage.rst` & `cellmaps_utils-0.3.0a1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/docs/versioningscheme.rst` & `cellmaps_utils-0.3.0a1/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/setup.py` & `cellmaps_utils-0.3.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 
-requirements = ['fairscape-cli==0.1.14',
+requirements = ['fairscape-cli==0.2.0',
                 'scipy',
                 'scikit-learn',
                 'pandas',
                 'numpy',
                 'dill',
                 'tqdm']
```

### Comparing `cellmaps_utils-0.2.0.post1/tests/test_basecommandlinetool.py` & `cellmaps_utils-0.3.0a1/tests/test_basecommandlinetool.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/tests/test_helloworldcommand.py` & `cellmaps_utils-0.3.0a1/tests/test_helloworldcommand.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/tests/test_integation_provenance.py` & `cellmaps_utils-0.3.0a1/tests/test_integation_provenance.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/tests/test_logutils.py` & `cellmaps_utils-0.3.0a1/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.2.0.post1/tests/test_provenance.py` & `cellmaps_utils-0.3.0a1/tests/test_provenance.py`

 * *Files identical despite different names*

