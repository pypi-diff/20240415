# Comparing `tmp/VoigtFit-3.21.4.tar.gz` & `tmp/VoigtFit-3.21.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoigtFit-3.21.4.tar", last modified: Wed Apr  3 14:56:34 2024, max compression
+gzip compressed data, was "VoigtFit-3.21.5.1.tar", last modified: Mon Apr 15 14:56:34 2024, max compression
```

## Comparing `VoigtFit-3.21.4.tar` & `VoigtFit-3.21.5.1.tar`

### file list

```diff
@@ -1,55 +1,111 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.605471 VoigtFit-3.21.4/
--rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/AUTHORS.rst
--rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)     3135 2024-04-03 14:56:34.605229 VoigtFit-3.21.4/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.21.4/README.rst
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.591271 VoigtFit-3.21.4/VoigtFit/
--rw-r--r--   0 krogager   (501) staff       (20)        7 2024-04-03 14:50:24.000000 VoigtFit-3.21.4/VoigtFit/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1842 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/VoigtFit/__main__.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.594140 VoigtFit-3.21.4/VoigtFit/container/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/container/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/container/components.py
--rw-r--r--   0 krogager   (501) staff       (20)   105654 2023-12-11 16:42:50.000000 VoigtFit-3.21.4/VoigtFit/container/dataset.py
--rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/container/lines.py
--rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/container/regions.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.594993 VoigtFit-3.21.4/VoigtFit/funcs/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/funcs/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/funcs/limits.py
--rw-r--r--   0 krogager   (501) staff       (20)    13301 2023-12-11 17:16:18.000000 VoigtFit-3.21.4/VoigtFit/funcs/voigt.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.596438 VoigtFit-3.21.4/VoigtFit/io/
--rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/io/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)    16646 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/VoigtFit/io/fits_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/io/hdf5_save.py
--rw-r--r--   0 krogager   (501) staff       (20)    81493 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/VoigtFit/io/output.py
--rw-r--r--   0 krogager   (501) staff       (20)    31727 2023-12-11 16:17:40.000000 VoigtFit-3.21.4/VoigtFit/io/parse_input.py
--rw-r--r--   0 krogager   (501) staff       (20)    26196 2023-12-11 16:14:40.000000 VoigtFit-3.21.4/VoigtFit/main.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.599434 VoigtFit-3.21.4/VoigtFit/static/
--rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/Asplund2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.21.4/VoigtFit/static/Asplund2021.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/C_complexes.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/C_full_labels.txt
--rw-r--r--   0 krogager   (501) staff       (20)      561 2023-05-17 08:46:43.000000 VoigtFit-3.21.4/VoigtFit/static/Konstantopoulou2022.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/Lodders2009.dat
--rw-r--r--   0 krogager   (501) staff       (20)     5705 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/VoigtFit/static/input_template.txt
--rw-r--r--   0 krogager   (501) staff       (20)   168996 2024-04-03 14:49:41.000000 VoigtFit-3.21.4/VoigtFit/static/linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/static/telluric_em_abs.npz
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604274 VoigtFit-3.21.4/VoigtFit/utils/
--rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/utils/Asplund.py
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/utils/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)      638 2023-05-17 08:46:43.000000 VoigtFit-3.21.4/VoigtFit/utils/depletion.py
--rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.21.4/VoigtFit/utils/line_complexes.py
--rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.21.4/VoigtFit/utils/molecules.py
--rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.21.4/VoigtFit/utils/terminal_attributes.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604948 VoigtFit-3.21.4/VoigtFit.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)     3135 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     1178 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)      120 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)       54 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        9 2024-04-03 14:56:34.000000 VoigtFit-3.21.4/VoigtFit.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)       38 2024-04-03 14:56:34.605514 VoigtFit-3.21.4/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5234 2023-11-28 11:43:49.000000 VoigtFit-3.21.4/setup.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-03 14:56:34.604563 VoigtFit-3.21.4/tests/
--rw-r--r--   0 krogager   (501) staff       (20)     5372 2023-12-10 21:17:13.000000 VoigtFit-3.21.4/tests/test_voigtfit.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.041403 VoigtFit-3.21.5.1/
+-rw-r--r--   0 krogager   (501) staff       (20)      299 2023-11-28 11:43:49.000000 VoigtFit-3.21.5.1/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)      224 2023-12-11 17:39:26.000000 VoigtFit-3.21.5.1/.readthedocs.yaml
+-rw-r--r--   0 krogager   (501) staff       (20)      248 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/AUTHORS.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     1095 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)       90 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)     3137 2024-04-15 14:56:34.041117 VoigtFit-3.21.5.1/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2393 2022-05-03 11:48:30.000000 VoigtFit-3.21.5.1/README.rst
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.984305 VoigtFit-3.21.5.1/VoigtFit/
+-rw-r--r--   0 krogager   (501) staff       (20)        9 2024-04-15 14:54:02.000000 VoigtFit-3.21.5.1/VoigtFit/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1313 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1842 2023-11-28 11:43:49.000000 VoigtFit-3.21.5.1/VoigtFit/__main__.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.986813 VoigtFit-3.21.5.1/VoigtFit/container/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/container/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5401 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/container/components.py
+-rw-r--r--   0 krogager   (501) staff       (20)   105654 2023-12-11 16:42:50.000000 VoigtFit-3.21.5.1/VoigtFit/container/dataset.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4466 2022-07-21 13:29:16.000000 VoigtFit-3.21.5.1/VoigtFit/container/lines.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23426 2022-07-21 13:29:16.000000 VoigtFit-3.21.5.1/VoigtFit/container/regions.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.987467 VoigtFit-3.21.5.1/VoigtFit/funcs/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/funcs/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4009 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/funcs/limits.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13322 2024-04-14 13:47:24.000000 VoigtFit-3.21.5.1/VoigtFit/funcs/voigt.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.989292 VoigtFit-3.21.5.1/VoigtFit/io/
+-rw-r--r--   0 krogager   (501) staff       (20)       43 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/io/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16646 2023-12-10 21:17:13.000000 VoigtFit-3.21.5.1/VoigtFit/io/fits_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    16812 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/io/hdf5_save.py
+-rw-r--r--   0 krogager   (501) staff       (20)    81525 2024-04-15 14:53:15.000000 VoigtFit-3.21.5.1/VoigtFit/io/output.py
+-rw-r--r--   0 krogager   (501) staff       (20)    31727 2023-12-11 16:17:40.000000 VoigtFit-3.21.5.1/VoigtFit/io/parse_input.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26196 2023-12-11 16:14:40.000000 VoigtFit-3.21.5.1/VoigtFit/main.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.991861 VoigtFit-3.21.5.1/VoigtFit/static/
+-rw-r--r--   0 krogager   (501) staff       (20)     2116 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/static/Asplund2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2747 2022-07-21 13:05:22.000000 VoigtFit-3.21.5.1/VoigtFit/static/Asplund2021.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2435 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/static/C_complexes.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5437 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/static/C_full_labels.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      561 2023-05-17 08:46:43.000000 VoigtFit-3.21.5.1/VoigtFit/static/Konstantopoulou2022.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2750 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/static/Lodders2009.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     5705 2023-11-28 11:43:49.000000 VoigtFit-3.21.5.1/VoigtFit/static/input_template.txt
+-rw-r--r--   0 krogager   (501) staff       (20)   168996 2024-04-03 14:49:41.000000 VoigtFit-3.21.5.1/VoigtFit/static/linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)  2536616 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/static/telluric_em_abs.npz
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:33.996507 VoigtFit-3.21.5.1/VoigtFit/utils/
+-rw-r--r--   0 krogager   (501) staff       (20)     1285 2022-07-21 13:29:16.000000 VoigtFit-3.21.5.1/VoigtFit/utils/Asplund.py
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/utils/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)      638 2023-05-17 08:46:43.000000 VoigtFit-3.21.5.1/VoigtFit/utils/depletion.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2625 2022-07-21 13:29:16.000000 VoigtFit-3.21.5.1/VoigtFit/utils/line_complexes.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23052 2022-05-03 11:57:56.000000 VoigtFit-3.21.5.1/VoigtFit/utils/molecules.py
+-rw-r--r--   0 krogager   (501) staff       (20)      603 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/VoigtFit/utils/terminal_attributes.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.040679 VoigtFit-3.21.5.1/VoigtFit.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)     3137 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2480 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      120 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       54 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        9 2024-04-15 14:56:33.000000 VoigtFit-3.21.5.1/VoigtFit.egg-info/top_level.txt
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.000856 VoigtFit-3.21.5.1/docs/
+-rw-r--r--   0 krogager   (501) staff       (20)      640 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/Makefile
+-rw-r--r--   0 krogager   (501) staff       (20)    92631 2023-12-12 10:19:09.000000 VoigtFit-3.21.5.1/docs/VoigtFit_logo2.png
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.001445 VoigtFit-3.21.5.1/docs/_static/
+-rw-r--r--   0 krogager   (501) staff       (20)    15026 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/_static/custom.css
+-rw-r--r--   0 krogager   (501) staff       (20)       51 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/_static/requirements.readthedocs.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      592 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/api.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     5890 2023-12-12 10:31:52.000000 VoigtFit-3.21.5.1/docs/conf.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47401 2023-12-11 17:29:28.000000 VoigtFit-3.21.5.1/docs/documentation.rst
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.004473 VoigtFit-3.21.5.1/docs/figs/
+-rw-r--r--   0 krogager   (501) staff       (20)   109664 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/comp1.png
+-rw-r--r--   0 krogager   (501) staff       (20)   111986 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/comp2.png
+-rw-r--r--   0 krogager   (501) staff       (20)   138261 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/mask1.png
+-rw-r--r--   0 krogager   (501) staff       (20)   163341 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/mask2.png
+-rw-r--r--   0 krogager   (501) staff       (20)    98185 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/norm1.png
+-rw-r--r--   0 krogager   (501) staff       (20)   104670 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/norm2.png
+-rw-r--r--   0 krogager   (501) staff       (20)   974369 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/figs/vfit_thermal_output.png
+-rw-r--r--   0 krogager   (501) staff       (20)    11966 2024-04-14 13:47:24.000000 VoigtFit-3.21.5.1/docs/index.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     2745 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/install.rst
+-rw-r--r--   0 krogager   (501) staff       (20)     4966 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/physical_model_results.rst
+-rw-r--r--   0 krogager   (501) staff       (20)       82 2023-11-28 11:43:49.000000 VoigtFit-3.21.5.1/docs/requirements.txt
+-rw-r--r--   0 krogager   (501) staff       (20)   109592 2023-12-12 10:39:23.000000 VoigtFit-3.21.5.1/docs/voigtfit.ico
+-rw-r--r--   0 krogager   (501) staff       (20)      183 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/voigtfit_logo.rst
+-rw-r--r--   0 krogager   (501) staff       (20)    14554 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/docs/voigtfit_overview.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      131 2022-05-03 12:12:28.000000 VoigtFit-3.21.5.1/prep_dist
+-rw-r--r--   0 krogager   (501) staff       (20)       71 2022-05-03 12:11:00.000000 VoigtFit-3.21.5.1/pytest.ini
+-rw-r--r--   0 krogager   (501) staff       (20)       54 2023-02-15 13:18:30.000000 VoigtFit-3.21.5.1/requirements.txt
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.008715 VoigtFit-3.21.5.1/scripts/
+-rw-r--r--   0 krogager   (501) staff       (20)     4253 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/scripts/VoigtFit_example.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3170 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/scripts/make_synthetic_data.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6449 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/scripts/physical_model.py
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2024-04-15 14:56:34.041457 VoigtFit-3.21.5.1/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5234 2023-11-28 11:43:49.000000 VoigtFit-3.21.5.1/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.015183 VoigtFit-3.21.5.1/test_data/
+-rw-r--r--   0 krogager   (501) staff       (20)     2234 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/HI_input.pars
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.016904 VoigtFit-3.21.5.1/test_data/Q1313+1441/
+-rw-r--r--   0 krogager   (501) staff       (20)   360487 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/Q1313+1441/1313_UVB_1d.spec
+-rw-r--r--   0 krogager   (501) staff       (20)   682451 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/Q1313+1441/1313_VIS_1d.spec
+-rw-r--r--   0 krogager   (501) staff       (20)     4304 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/VoigtFit_example.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2844 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/input.pars
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.030319 VoigtFit-3.21.5.1/test_data/synthetic_testdata/
+-rw-r--r--   0 krogager   (501) staff       (20)      626 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/synpars.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      209 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/synpars_simple.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   494311 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/synspec.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   493933 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/synspec_simple.dat
+-rw-r--r--   0 krogager   (501) staff       (20)  6200068 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/thermal_model_2comp.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      477 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/synthetic_testdata/thermal_model_2comp.input
+-rw-r--r--   0 krogager   (501) staff       (20)   360455 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/test_UVB_1d.spec
+-rw-r--r--   0 krogager   (501) staff       (20)   682416 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/test_VIS_1d.spec
+-rw-r--r--   0 krogager   (501) staff       (20)     3673 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/test_input_comp.pars
+-rw-r--r--   0 krogager   (501) staff       (20)     3656 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/test_input_mask.pars
+-rw-r--r--   0 krogager   (501) staff       (20)     3659 2023-11-28 11:34:19.000000 VoigtFit-3.21.5.1/test_data/test_input_noint.pars
+-rw-r--r--   0 krogager   (501) staff       (20)     3717 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/test_input_norm.pars
+-rw-r--r--   0 krogager   (501) staff       (20)      994 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/test_data/thermal_model.pars
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-15 14:56:34.040317 VoigtFit-3.21.5.1/tests/
+-rw-r--r--   0 krogager   (501) staff       (20)  3720235 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/tests/test_2comp.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      454 2022-03-27 13:11:46.000000 VoigtFit-3.21.5.1/tests/test_2comp.input
+-rw-r--r--   0 krogager   (501) staff       (20)     5372 2023-12-10 21:17:13.000000 VoigtFit-3.21.5.1/tests/test_voigtfit.py
```

### Comparing `VoigtFit-3.21.4/LICENSE` & `VoigtFit-3.21.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/PKG-INFO` & `VoigtFit-3.21.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.21.4
+Version: 3.21.5.1
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VoigtFit-3.21.4/README.rst` & `VoigtFit-3.21.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/__init__.py` & `VoigtFit-3.21.5.1/VoigtFit/__init__.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/__main__.py` & `VoigtFit-3.21.5.1/VoigtFit/__main__.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/container/components.py` & `VoigtFit-3.21.5.1/VoigtFit/container/components.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/container/dataset.py` & `VoigtFit-3.21.5.1/VoigtFit/container/dataset.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/container/lines.py` & `VoigtFit-3.21.5.1/VoigtFit/container/lines.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/container/regions.py` & `VoigtFit-3.21.5.1/VoigtFit/container/regions.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/funcs/limits.py` & `VoigtFit-3.21.5.1/VoigtFit/funcs/limits.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/funcs/voigt.py` & `VoigtFit-3.21.5.1/VoigtFit/funcs/voigt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 to convert this to observed transmission and to convolve the
 observed spectrum with the instrumental profile.
 """
 
 __author__ = 'Jens-Kristian Krogager'
 
 import numpy as np
-from scipy.signal import fftconvolve, gaussian
-
+from scipy import signal
 import re
 
 # Regular Expression to match redshift parameter names:
 # ex: z0_FeII, z0_H2J0, z3_HI, z15_TiII
 z_matcher = re.compile('z[0-9]+_[A-Z][A-Z]?[0-9]?[a-z]?[I-Z]+[0-9]?[a-z]?')
 
 
@@ -229,17 +228,17 @@
         err_msg = "Invalid type of `kernel`: %r" % type(kernel)
         raise TypeError(err_msg)
 
     tau = evaluate_optical_depth(profile_wl, pars, lines, z_sys=z_sys)
     profile = np.exp(-tau)
 
     if isinstance(kernel, float):
-        LSF = gaussian(10*int(kernel) + 1, kernel)
+        LSF = signal.windows.gaussian(10*int(kernel) + 1, kernel)
         LSF = LSF/LSF.sum()
-        profile_broad = fftconvolve(profile, LSF, 'same')
+        profile_broad = signal.fftconvolve(profile, LSF, 'same')
         # Interpolate onto the data grid:
         profile_obs = np.interp(x, profile_wl, profile_broad)
 
     else:
         profile_broad = convolve(profile, kernel)
         if kernel_nsub > 1:
             # Interpolate onto the data grid:
@@ -393,16 +392,16 @@
         the resolution element: `width` = FWHM / 2.35482
 
     Returns
     -------
     profile_obs : array, shape(N)
         The convolved version of `profile`.
     """
-    LSF = gaussian(10*int(width)+1, width)
+    LSF = signal.windows.gaussian(10*int(width)+1, width)
     LSF = LSF/LSF.sum()
     # Add padding to avoid edge effects of the convolution:
     pad = np.ones(5*int(width))
     P_padded = np.concatenate((pad, profile, pad))
-    profile_broad = fftconvolve(P_padded, LSF, 'same')
+    profile_broad = signal.fftconvolve(P_padded, LSF, 'same')
     # Remove padding:
     profile_obs = profile_broad[5*int(width):-5*int(width)]
     return profile_obs
```

### Comparing `VoigtFit-3.21.4/VoigtFit/io/fits_input.py` & `VoigtFit-3.21.5.1/VoigtFit/io/fits_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/io/hdf5_save.py` & `VoigtFit-3.21.5.1/VoigtFit/io/hdf5_save.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/io/output.py` & `VoigtFit-3.21.5.1/VoigtFit/io/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import os
 from os.path import splitext
 from matplotlib.lines import Line2D
 import matplotlib.pyplot as plt
 import matplotlib.backends.backend_pdf
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-from scipy.signal import fftconvolve, gaussian
+from scipy.signal import fftconvolve
+from scipy.signal.windows import gaussian
 from scipy.ndimage import gaussian_filter1d
 from scipy.interpolate import RectBivariateSpline as spline2d
 import numpy as np
 import re
 
 from ..utils import Asplund
 from ..utils import molecules
```

### Comparing `VoigtFit-3.21.4/VoigtFit/io/parse_input.py` & `VoigtFit-3.21.5.1/VoigtFit/io/parse_input.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/main.py` & `VoigtFit-3.21.5.1/VoigtFit/main.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/Asplund2009.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/Asplund2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/Asplund2021.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/Asplund2021.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/C_complexes.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/C_complexes.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/C_full_labels.txt` & `VoigtFit-3.21.5.1/VoigtFit/static/C_full_labels.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/Konstantopoulou2022.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/Konstantopoulou2022.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/Lodders2009.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/Lodders2009.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/input_template.txt` & `VoigtFit-3.21.5.1/VoigtFit/static/input_template.txt`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/linelist.dat` & `VoigtFit-3.21.5.1/VoigtFit/static/linelist.dat`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/static/telluric_em_abs.npz` & `VoigtFit-3.21.5.1/VoigtFit/static/telluric_em_abs.npz`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/utils/Asplund.py` & `VoigtFit-3.21.5.1/VoigtFit/utils/Asplund.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/utils/depletion.py` & `VoigtFit-3.21.5.1/VoigtFit/utils/depletion.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/utils/line_complexes.py` & `VoigtFit-3.21.5.1/VoigtFit/utils/line_complexes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/utils/molecules.py` & `VoigtFit-3.21.5.1/VoigtFit/utils/molecules.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit/utils/terminal_attributes.py` & `VoigtFit-3.21.5.1/VoigtFit/utils/terminal_attributes.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/VoigtFit.egg-info/PKG-INFO` & `VoigtFit-3.21.5.1/VoigtFit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoigtFit
-Version: 3.21.4
+Version: 3.21.5.1
 Summary: Voigt Profile Fitting in Python
 Home-page: https://github.com/jkrogager/VoigtFit
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: voigtfit absorption analysis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VoigtFit-3.21.4/setup.py` & `VoigtFit-3.21.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `VoigtFit-3.21.4/tests/test_voigtfit.py` & `VoigtFit-3.21.5.1/tests/test_voigtfit.py`

 * *Files identical despite different names*

