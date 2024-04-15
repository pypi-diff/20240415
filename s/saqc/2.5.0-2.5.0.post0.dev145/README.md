# Comparing `tmp/saqc-2.5.0.tar.gz` & `tmp/saqc-2.5.0.post0.dev145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saqc-2.5.0.tar", last modified: Tue Sep  5 19:15:57 2023, max compression
+gzip compressed data, was "saqc-2.5.0.post0.dev145.tar", last modified: Mon Apr 15 19:29:23 2024, max compression
```

## Comparing `saqc-2.5.0.tar` & `saqc-2.5.0.post0.dev145.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:57.000620 saqc-2.5.0/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-07-08 08:06:22.000000 saqc-2.5.0/LICENSE.md
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.990620 saqc-2.5.0/LICENSES/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-07-08 08:06:22.000000 saqc-2.5.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7135 2023-09-05 19:15:57.000620 saqc-2.5.0/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6725 2023-09-05 18:37:08.000000 saqc-2.5.0/README.md
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      625 2023-09-05 18:37:08.000000 saqc-2.5.0/pyproject.toml
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.990620 saqc-2.5.0/saqc/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      665 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4439 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/__main__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      497 2023-09-05 19:15:57.000620 saqc-2.5.0/saqc/_version.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1604 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/constants.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.993953 saqc-2.5.0/saqc/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      414 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8452 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/core/core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16822 2023-08-27 08:20:27.000000 saqc-2.5.0/saqc/core/flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4555 2023-07-10 15:07:37.000000 saqc-2.5.0/saqc/core/frame.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18044 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/core/history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1180 2023-01-30 06:47:58.000000 saqc-2.5.0/saqc/core/mixins.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16349 2023-07-03 19:10:09.000000 saqc-2.5.0/saqc/core/register.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.993953 saqc-2.5.0/saqc/core/translation/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      466 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/core/translation/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7188 2023-07-03 12:52:30.000000 saqc-2.5.0/saqc/core/translation/basescheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6355 2023-05-24 06:55:14.000000 saqc-2.5.0/saqc/core/translation/dmpscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1534 2023-01-30 06:47:58.000000 saqc-2.5.0/saqc/core/translation/floatscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2766 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/core/translation/positionalscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      760 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/core/translation/simplescheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      252 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/exceptions.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.993953 saqc-2.5.0/saqc/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2023-03-30 19:15:16.000000 saqc-2.5.0/saqc/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6994 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/breaks.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13176 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/changepoints.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4995 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/constants.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7475 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/curvefit.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    29520 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/drift.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    22371 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8968 2023-05-24 06:55:17.000000 saqc-2.5.0/saqc/funcs/generic.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    22237 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/interpolation.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5784 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/noise.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    65386 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/outliers.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6511 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/pattern.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    17002 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4763 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/residuals.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6560 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20171 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/scores.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    17111 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/funcs/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1943 2023-05-24 06:55:17.000000 saqc-2.5.0/saqc/funcs/transformation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/saqc/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0/saqc/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    10946 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/lib/checking.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3237 2023-05-24 06:55:17.000000 saqc-2.5.0/saqc/lib/docs.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20101 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/lib/plotting.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7495 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/lib/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    21402 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/lib/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18895 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/lib/ts_operators.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      942 2023-04-19 15:26:39.000000 saqc-2.5.0/saqc/lib/types.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/saqc/parsing/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2023-04-05 11:41:00.000000 saqc-2.5.0/saqc/parsing/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2303 2023-05-24 06:55:14.000000 saqc-2.5.0/saqc/parsing/environ.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7576 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/parsing/reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5704 2023-06-07 07:36:11.000000 saqc-2.5.0/saqc/parsing/visitor.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      221 2023-09-05 18:37:08.000000 saqc-2.5.0/saqc/version.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.993953 saqc-2.5.0/saqc.egg-info/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7135 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2304 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/SOURCES.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/dependency_links.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/entry_points.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      140 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/requires.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       11 2023-09-05 19:15:56.000000 saqc-2.5.0/saqc.egg-info/top_level.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2023-09-05 19:15:57.000620 saqc-2.5.0/setup.cfg
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2188 2023-09-05 18:37:08.000000 saqc-2.5.0/setup.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/api/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/api/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      538 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/api/test_creation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/cli/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/cli/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3563 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/cli/test_integration.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11372 2023-07-03 18:54:50.000000 saqc-2.5.0/tests/core/test_core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11200 2023-07-10 15:05:55.000000 saqc-2.5.0/tests/core/test_flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      262 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/core/test_frame.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6164 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/core/test_history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4641 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/core/test_reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8524 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/core/test_translator.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1323 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/funcs/test_constants_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6995 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8907 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6300 2023-04-19 15:26:39.000000 saqc-2.5.0/tests/funcs/test_generic_api_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8689 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_generic_config_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7474 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_outlier_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1254 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/funcs/test_pattern_rec.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4715 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/funcs/test_proc_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    10260 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1151 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/funcs/test_tools.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/fuzzy/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/fuzzy/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4968 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/fuzzy/lib.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5991 2023-04-05 11:41:00.000000 saqc-2.5.0/tests/fuzzy/test_masking.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:56.997286 saqc-2.5.0/tests/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.5.0/tests/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2023-03-30 19:15:16.000000 saqc-2.5.0/tests/lib/test_periodicMask.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1766 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/lib/test_tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6990 2023-09-05 18:37:08.000000 saqc-2.5.0/tests/lib/test_ts_operators.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-09-05 19:15:57.000620 saqc-2.5.0/tests/misc/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      147 2023-07-10 15:07:37.000000 saqc-2.5.0/tests/misc/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      609 2023-07-10 15:07:37.000000 saqc-2.5.0/tests/misc/test_pickle.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      531 2023-03-30 19:15:16.000000 saqc-2.5.0/tests/test__main__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    86677 2023-09-05 17:35:53.000000 saqc-2.5.0/versioneer.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/LICENSE.md
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.384622 saqc-2.5.0.post0.dev145/LICENSES/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7472 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6725 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/README.md
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      625 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/pyproject.toml
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.384622 saqc-2.5.0.post0.dev145/saqc/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      665 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4329 2024-04-15 19:03:59.000000 saqc-2.5.0.post0.dev145/saqc/__main__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      510 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/saqc/_version.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1604 2024-01-31 22:57:39.000000 saqc-2.5.0.post0.dev145/saqc/constants.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.384622 saqc-2.5.0.post0.dev145/saqc/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      414 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/saqc/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13334 2024-04-15 19:03:59.000000 saqc-2.5.0.post0.dev145/saqc/core/core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16448 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/core/flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3801 2024-04-15 19:04:48.000000 saqc-2.5.0.post0.dev145/saqc/core/frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18572 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/saqc/core/history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1180 2023-01-30 06:47:58.000000 saqc-2.5.0.post0.dev145/saqc/core/mixins.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16349 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/core/register.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.387956 saqc-2.5.0.post0.dev145/saqc/core/translation/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      516 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3753 2024-04-09 14:51:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/annotationscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6332 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/basescheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6184 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/dmpscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2771 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/floatscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2830 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/positionalscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      759 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/core/translation/simplescheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      252 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/exceptions.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.387956 saqc-2.5.0.post0.dev145/saqc/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2023-03-30 19:15:16.000000 saqc-2.5.0.post0.dev145/saqc/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6975 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/funcs/breaks.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13176 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/funcs/changepoints.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5150 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/funcs/constants.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7459 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/funcs/curvefit.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    29551 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/drift.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    26958 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    10102 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/saqc/funcs/generic.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11189 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/interpolation.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5747 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/noise.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    65436 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/outliers.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6481 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/saqc/funcs/pattern.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    40952 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4769 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/funcs/residuals.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2872 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20565 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/scores.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    21068 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/funcs/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2174 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/funcs/transformation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.387956 saqc-2.5.0.post0.dev145/saqc/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/saqc/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12420 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/checking.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3240 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/docs.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20110 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/plotting.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7495 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/lib/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12873 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/selectionGUI.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    22151 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    17942 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/saqc/lib/ts_operators.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      948 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/lib/types.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/saqc/parsing/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/saqc/parsing/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2597 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/saqc/parsing/environ.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7576 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/parsing/reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5634 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/saqc/parsing/visitor.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      221 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/saqc/version.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/saqc.egg-info/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7472 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2357 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/SOURCES.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/dependency_links.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/entry_points.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      144 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/requires.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       11 2024-04-15 19:29:23.000000 saqc-2.5.0.post0.dev145/saqc.egg-info/top_level.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/setup.cfg
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1943 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/setup.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/api/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/api/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      538 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/tests/api/test_creation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/cli/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/cli/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3506 2024-04-15 19:03:59.000000 saqc-2.5.0.post0.dev145/tests/cli/test_integration.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16973 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/core/test_core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11075 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/tests/core/test_flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      262 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/tests/core/test_frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7002 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/core/test_history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4641 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/tests/core/test_reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9279 2024-04-15 19:11:53.000000 saqc-2.5.0.post0.dev145/tests/core/test_translator.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1323 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_constants_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11481 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8988 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6580 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_generic_api_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8689 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_generic_config_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7446 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_outlier_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1254 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_pattern_rec.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3706 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_proc_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    14370 2024-04-15 14:11:25.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1494 2024-04-15 19:04:14.000000 saqc-2.5.0.post0.dev145/tests/funcs/test_tools.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/fuzzy/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/fuzzy/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4940 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/fuzzy/lib.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5991 2023-04-05 11:41:00.000000 saqc-2.5.0.post0.dev145/tests/fuzzy/test_masking.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.391289 saqc-2.5.0.post0.dev145/tests/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.5.0.post0.dev145/tests/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2023-03-30 19:15:16.000000 saqc-2.5.0.post0.dev145/tests/lib/test_periodicMask.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1766 2023-09-05 18:37:08.000000 saqc-2.5.0.post0.dev145/tests/lib/test_tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7456 2024-04-15 14:09:58.000000 saqc-2.5.0.post0.dev145/tests/lib/test_ts_operators.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2024-04-15 19:29:23.394622 saqc-2.5.0.post0.dev145/tests/misc/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      147 2023-07-10 15:07:37.000000 saqc-2.5.0.post0.dev145/tests/misc/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      609 2023-07-10 15:07:37.000000 saqc-2.5.0.post0.dev145/tests/misc/test_pickle.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      531 2023-03-30 19:15:16.000000 saqc-2.5.0.post0.dev145/tests/test__main__.py
```

### Comparing `saqc-2.5.0/LICENSE.md` & `saqc-2.5.0.post0.dev145/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/LICENSES/GPL-3.0-or-later.txt` & `saqc-2.5.0.post0.dev145/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/PKG-INFO` & `saqc-2.5.0.post0.dev145/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: saqc
-Version: 2.5.0
-Summary: A timeseries data quality control and processing tool/framework
-Home-page: https://git.ufz.de/rdm-software/saqc
-Author: Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss
-Author-email: david.schaefer@ufz.de
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-License-File: LICENSES/GPL-3.0-or-later.txt
-
 <!--
 SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 <br>
@@ -70,15 +58,15 @@
 file listing the variables in the dataset and the routines to inspect,
 quality control and/or process them. The content of such a configuration
 could look like [this](https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/config.csv):
 
 ```
 varname    ; test
 #----------; ---------------------------------------------------------------------
-SM2        ; shift(freq="15Min")
+SM2        ; align(freq="15Min")
 'SM(1|2)+' ; flagMissing()
 SM1        ; flagRange(min=10, max=60)
 SM2        ; flagRange(min=10, max=40)
 SM2        ; flagZScore(window="30d", thresh=3.5, method='modified', center=False)
 Dummy      ; flagGeneric(field=["SM1", "SM2"], func=(isflagged(x) | isflagged(y)))
 ```
 
@@ -111,15 +99,15 @@
 data = pd.read_csv(
     "https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/data.csv",
     index_col=0, parse_dates=True,
 )
 
 qc = SaQC(data=data)
 qc = (qc
-      .shift("SM2", freq="15Min")
+      .align("SM2", freq="15Min")
       .flagMissing("SM(1|2)+", regex=True)
       .flagRange("SM1", min=10, max=60)
       .flagRange("SM2", min=10, max=40)
       .flagZScore("SM2", window="30d", thresh=3.5, method='modified', center=False)
       .flagGeneric(field=["SM1", "SM2"], target="Dummy", func=lambda x, y: (isflagged(x) | isflagged(y))))
 ```
```

### Comparing `saqc-2.5.0/README.md` & `saqc-2.5.0.post0.dev145/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: saqc
+Version: 2.5.0.post0.dev145
+Summary: A timeseries data quality control and processing tool/framework
+Home-page: https://git.ufz.de/rdm-software/saqc
+Author: Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss
+Author-email: david.schaefer@ufz.de
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+License-File: LICENSES/GPL-3.0-or-later.txt
+Requires-Dist: Click
+Requires-Dist: docstring_parser
+Requires-Dist: fancy-collections
+Requires-Dist: fastdtw
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numpy
+Requires-Dist: outlier-utils
+Requires-Dist: pyarrow
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: typing_extensions
+
 <!--
 SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 <br>
@@ -58,15 +82,15 @@
 file listing the variables in the dataset and the routines to inspect,
 quality control and/or process them. The content of such a configuration
 could look like [this](https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/config.csv):
 
 ```
 varname    ; test
 #----------; ---------------------------------------------------------------------
-SM2        ; shift(freq="15Min")
+SM2        ; align(freq="15Min")
 'SM(1|2)+' ; flagMissing()
 SM1        ; flagRange(min=10, max=60)
 SM2        ; flagRange(min=10, max=40)
 SM2        ; flagZScore(window="30d", thresh=3.5, method='modified', center=False)
 Dummy      ; flagGeneric(field=["SM1", "SM2"], func=(isflagged(x) | isflagged(y)))
 ```
 
@@ -99,15 +123,15 @@
 data = pd.read_csv(
     "https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/data.csv",
     index_col=0, parse_dates=True,
 )
 
 qc = SaQC(data=data)
 qc = (qc
-      .shift("SM2", freq="15Min")
+      .align("SM2", freq="15Min")
       .flagMissing("SM(1|2)+", regex=True)
       .flagRange("SM1", min=10, max=60)
       .flagRange("SM2", min=10, max=40)
       .flagZScore("SM2", window="30d", thresh=3.5, method='modified', center=False)
       .flagGeneric(field=["SM1", "SM2"], target="Dummy", func=lambda x, y: (isflagged(x) | isflagged(y))))
 ```
```

### Comparing `saqc-2.5.0/pyproject.toml` & `saqc-2.5.0.post0.dev145/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/__init__.py` & `saqc-2.5.0.post0.dev145/saqc/__init__.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/__main__.py` & `saqc-2.5.0.post0.dev145/saqc/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
-import json
 import logging
 from functools import partial
 from pathlib import Path
 
 import click
 import numpy as np
 import pandas as pd
@@ -142,31 +141,31 @@
             f = lambda j: j[str(json_field)]
         cr = cr.readJson(config, unpack=f)
     else:
         cr = cr.readCsv(config)
 
     saqc = cr.run()
 
-    data_result = saqc.data.to_pandas()
+    data_result = saqc.data
     flags_result = saqc.flags
-    if isinstance(flags_result, DictOfSeries):
-        flags_result = flags_result.to_pandas()
 
     if outfile:
-        data_result.columns = pd.MultiIndex.from_product(
-            [data_result.columns.tolist(), ["data"]]
-        )
-
-        if not isinstance(flags_result.columns, pd.MultiIndex):
-            flags_result.columns = pd.MultiIndex.from_product(
-                [flags_result.columns.tolist(), ["flags"]]
-            )
 
-        out = pd.concat([data_result, flags_result], axis=1).sort_index(
-            axis=1, level=0, sort_remaining=False
+        out = DictOfSeries()
+        for k in data_result.keys():
+            flagscol = flags_result[k]
+            if isinstance(flagscol, pd.Series):
+                flagscol = flagscol.rename("flags")
+            out[k] = pd.concat([data_result[k].rename("data"), flagscol], axis=1)
+
+        writeData(
+            writer,
+            out.to_pandas(
+                fill_value=-9999 if scheme == "positional" else np.nan,
+                multiindex=True,
+            ),
+            outfile,
         )
 
-        writeData(writer, out, outfile)
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `saqc-2.5.0/saqc/constants.py` & `saqc-2.5.0.post0.dev145/saqc/constants.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/core/core.py` & `saqc-2.5.0.post0.dev145/saqc/core/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import contextlib
 import warnings
 from copy import copy as shallowcopy
 from copy import deepcopy
-from typing import Any, Hashable, MutableMapping
+from functools import partial
+from typing import Any, Hashable, Iterable, MutableMapping
 
 import numpy as np
 import pandas as pd
 
 from saqc.core.flags import Flags, _HistAccess, initFlagsLike
 from saqc.core.frame import DictOfSeries
 from saqc.core.history import History
@@ -26,15 +28,15 @@
     SimpleScheme,
     TranslationScheme,
 )
 from saqc.funcs import FunctionsMixin
 
 # warnings
 pd.set_option("mode.chained_assignment", "warn")
-pd.options.mode.copy_on_write = False
+pd.set_option("mode.copy_on_write", True)
 np.seterr(invalid="ignore")
 
 
 TRANSLATION_SCHEMES = {
     "simple": SimpleScheme,
     "float": FloatScheme,
     "dmp": DmpScheme,
@@ -48,21 +50,33 @@
         "_flags",
         "_scheme",
         "_attrs",
     }
 
     def __init__(
         self,
-        data=None,
-        flags=None,
+        data: (
+            pd.Series
+            | pd.DataFrame
+            | DictOfSeries
+            | list[pd.Series | pd.DataFrame | DictOfSeries]
+            | None
+        ) = None,
+        flags: (
+            pd.DataFrame
+            | DictOfSeries
+            | Flags
+            | list[pd.DataFrame | DictOfSeries | Flags]
+            | None
+        ) = None,
         scheme: str | TranslationScheme = "float",
     ):
+        self.scheme: TranslationScheme = scheme
         self._data: DictOfSeries = self._initData(data)
         self._flags: Flags = self._initFlags(flags)
-        self._scheme: TranslationScheme = self._initTranslationScheme(scheme)
         self._attrs: dict = {}
         self._validate(reason="init")
 
     def _construct(self, **attributes) -> "SaQC":
         """
         Construct a new `SaQC`-Object from `self` and optionally inject
         attributes with any chechking and overhead.
@@ -72,63 +86,191 @@
         **attributes: any of the `SaQC` data attributes with name and value
 
         Note
         ----
         For internal usage only! Setting values through `injectables` has
         the potential to mess up certain invariants of the constructed object.
         """
-        out = SaQC(data=DictOfSeries(), flags=Flags(), scheme=self._scheme)
+        out = self.__class__(data=DictOfSeries(), flags=Flags(), scheme=self._scheme)
         out.attrs = self._attrs
         for k, v in attributes.items():
             if k not in self._attributes:
                 raise AttributeError(f"SaQC has no attribute {repr(k)}")
             setattr(out, k, v)
         return out
 
     def _validate(self, reason=None):
         if not self._data.columns.equals(self._flags.columns):
-            msg = "Consistency broken. data and flags have not the same columns."
+            msg = "Data and flags don't contain the same columns."
             if reason:
                 msg += f" This was most likely caused by: {reason}"
             raise RuntimeError(msg)
+        return self
 
     @property
     def attrs(self) -> dict[Hashable, Any]:
         """
         Dictionary of global attributes of this dataset.
         """
         return self._attrs
 
     @attrs.setter
     def attrs(self, value: dict[Hashable, Any]) -> None:
         self._attrs = dict(value)
 
     @property
-    def data(self) -> MutableMapping:
+    def data(self) -> DictOfSeries:
         data = self._data
         data.attrs = self._attrs.copy()
         return data
 
     @property
-    def flags(self) -> MutableMapping:
+    def flags(self) -> DictOfSeries:
         flags = self._scheme.toExternal(self._flags, attrs=self._attrs)
         flags.attrs = self._attrs.copy()
         return flags
 
     @property
+    def scheme(self) -> TranslationScheme:
+        return self._scheme
+
+    @scheme.setter
+    def scheme(self, scheme: str | TranslationScheme) -> None:
+        if isinstance(scheme, str) and scheme in TRANSLATION_SCHEMES:
+            scheme = TRANSLATION_SCHEMES[scheme]()
+        if not isinstance(scheme, TranslationScheme):
+            raise TypeError(
+                f"expected one of the following translation schemes '{TRANSLATION_SCHEMES.keys()} "
+                f"or an initialized Translator object, got '{scheme}'"
+            )
+        self._scheme = scheme
+
+    @property
     def _history(self) -> _HistAccess:
         return self._flags.history
 
+    @property
+    def columns(self) -> pd.Index:
+        return self._data.columns
+
+    def __len__(self):
+        return len(self.columns)
+
+    def __contains__(self, item):
+        return item in self.columns
+
+    def _get_keys(self, key: str | Iterable[str] | slice):
+        if isinstance(key, str):
+            key = [key]
+        elif isinstance(key, slice):
+            sss = self.columns.slice_locs(key.start, key.stop, key.step)
+            key = self.columns[slice(*sss)]
+        keys = pd.Index(key)
+        if keys.has_duplicates:
+            raise NotImplementedError(
+                "selecting the same key multiple times is not supported yet."
+            )
+        return keys
+
+    def __delitem__(self, key):
+        if key not in self.columns:
+            raise KeyError(key)
+        with self._atomicWrite():
+            del self._data[key]
+            del self._flags[key]
+
+    def __getitem__(self, key: str | slice | Iterable[str]) -> SaQC:
+        keys = self._get_keys(key)
+        if not_found := keys.difference(self.columns).tolist():
+            raise KeyError(f"{not_found} not in columns")
+        # data = self._data[key] should work, but fails with key=[]
+        # because of slice_dict issue #GH2 - empty list selection fails.
+        # As long as flags/history have no slicing support we stick to
+        # the loop.
+        data = DictOfSeries()
+        flags = Flags()
+        for k in keys:
+            data[k] = self._data[k].copy()
+            flags.history[k] = self._flags.history[k].copy()
+        new = self._construct(_data=data, _flags=flags)
+        return new._validate("a bug, pls report")
+
+    def __setitem__(
+        self,
+        key: str | slice | Iterable[str],
+        value: (
+            SaQC
+            | pd.Series
+            | pd.DataFrame
+            | DictOfSeries
+            | dict[Any, pd.Series]
+            | Iterable[pd.Series]
+        ),
+    ):
+        keys = self._get_keys(key)
+        if isinstance(value, SaQC):
+            pass
+        elif isinstance(value, pd.Series):
+            value = [value]
+        elif isinstance(value, (pd.DataFrame, DictOfSeries)):
+            value = [value[k] for k in value.keys()]
+        else:
+            if isinstance(value, dict):
+                value = value.values()
+            value = list(value)
+            for s in value:
+                if not isinstance(s, pd.Series):
+                    raise TypeError(
+                        f"all items of value must be of type "
+                        f"pd.Series, but got {type(s)}"
+                    )
+
+        if len(keys) != len(value):
+            raise ValueError(
+                f"Length mismatch, expected {len(keys)} elements, "
+                f"but value has {len(value)} elements"
+            )
+        with self._atomicWrite():
+            if isinstance(value, SaQC):
+                for k, c in zip(keys, value.columns):
+                    self._data[k] = value._data[c].copy()
+                    self._flags.history[k] = value._flags.history[c].copy()
+            else:
+                for i, k in enumerate(keys):
+                    self._data[k] = value[i]
+                    self._flags.history[k] = History(value[i].index)
+
+    @contextlib.contextmanager
+    def _atomicWrite(self):
+        """
+        Context manager to realize writing in an all-or-nothing style.
+
+        This is helpful for writing data and flags at once or resetting
+        all changes on errors.
+        It is also useful for updating multiple columns "at once".
+        """
+        # shallow copies
+        data = self._data.copy()
+        flags = self._flags.copy(deep=False)
+        try:
+            yield
+            # when we get here, everything has gone well,
+            # and we accept all changes on data and flags
+            data = self._data
+            flags = self._flags
+        finally:
+            self._data = data
+            self._flags = flags
+
     def __getattr__(self, key):
         """
         All failing attribute accesses are redirected to __getattr__.
         We use this mechanism to make the registered functions appear
         as `SaQC`-methods without actually implementing them.
         """
-        from functools import partial
 
         if key not in FUNC_MAP:
             raise AttributeError(f"SaQC has no attribute {repr(key)}")
         return partial(FUNC_MAP[key], self)
 
     def copy(self, deep=True):
         copyfunc = deepcopy if deep else shallowcopy
@@ -244,9 +386,9 @@
 
     def _castToFlags(self, flags):
         if isinstance(flags, pd.DataFrame):
             for idx in [flags.index, flags.columns]:
                 if isinstance(idx, pd.MultiIndex):
                     raise TypeError("'flags' should not have MultiIndex")
         if not isinstance(flags, Flags):
-            flags = Flags(flags)
+            flags = Flags(self._scheme.toInternal(flags))
         return flags
```

### Comparing `saqc-2.5.0/saqc/core/flags.py` & `saqc-2.5.0.post0.dev145/saqc/core/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     The flags can be accessed via ``__getitem__`` and ``__setitem__``, in real life known as the `[]`-operator.
 
     For the curious:
         Under the hood, the series are stored in a `history`, which allows the advanced user to retrieve all flags
         once was set in this object, but in the most cases this is irrelevant. For simplicity one can safely assume,
         that this class works just stores the flag-series one sets.
 
-    See Also
+    See also
     --------
     initFlagsLike : create a Flags instance, with same dimensions as a reference object.
     History : class that actually store the flags
 
     Examples
     --------
 
@@ -228,15 +228,17 @@
                 result[k] = item
                 continue
             if not isinstance(item, pd.Series):
                 raise TypeError(
                     f"cannot init from '{type(data).__name__}' of '{type(item).__name__}'"
                 )
 
-            result[k] = History(item.index).append(item)
+            result[k] = History(item.index).append(
+                item, meta={"func": "importedFlags", "args": (), "kwargs": {}}
+            )
 
         return result
 
     @staticmethod
     def _validateHistForFlags(history: History, colname=None):
         if history.empty:
             return history
@@ -317,20 +319,18 @@
     def __contains__(self, item):
         return item in self.columns
 
     # ----------------------------------------------------------------------
     # item access
 
     @overload
-    def __getitem__(self, key: str) -> pd.Series:
-        ...
+    def __getitem__(self, key: str) -> pd.Series: ...
 
     @overload
-    def __getitem__(self, key: list | pd.Index) -> Flags:
-        ...
+    def __getitem__(self, key: list | pd.Index) -> Flags: ...
 
     def __getitem__(self, key: str | list | pd.Index) -> pd.Series | Flags:
         if isinstance(key, str):
             return self._data[key].squeeze()
 
         if isinstance(key, slice):
             key = self.columns[key]
@@ -353,15 +353,15 @@
 
     def __setitem__(self, key: SelectT, value: ValueT):
         # force-KW is only internally available
 
         if isinstance(key, tuple):
             if len(key) != 2:
                 raise KeyError(
-                    "a single 'column' or a tuple of 'mask, column' must be passt"
+                    "a single 'column' or a tuple of 'mask, column' must be passed"
                 )
             mask, key = key
 
             tmp = pd.Series(np.nan, index=self._data[key].index, dtype=float)
 
             # make a mask from an index, because it seems
             # that passing an index is a very common workflow
@@ -429,15 +429,15 @@
         history.
 
         Returns
         -------
         history : History
             Accessor for the flags history
 
-        See Also
+        See also
         --------
         saqc.core.History : History storage class.
         """
         return _HistAccess(self)
 
     # ----------------------------------------------------------------------
     # copy
@@ -470,32 +470,14 @@
         memo, default None
             Standard signature. Unused
         """
         return self.copy(deep=True)
 
     # ----------------------------------------------------------------------
     # transformation and representation
-
-    def toDios(self) -> DictOfSeries:
-        """
-        Transform the flags container to a ``DictOfSeries``.
-
-        .. deprecated:: 2.4
-           use `saqc.DictOfSeries(obj)` instead.
-
-        Returns
-        -------
-        DictOfSeries
-        """
-        warnings.warn(
-            "toDios is deprecated, use `saqc.DictOfSeries(obj)` instead.",
-            category=DeprecationWarning,
-        )
-        return DictOfSeries(self).copy()
-
     def toFrame(self) -> pd.DataFrame:
         """
         Transform the flags container to a ``pd.DataFrame``.
 
         Returns
         -------
         pd.DataFrame
```

### Comparing `saqc-2.5.0/saqc/core/frame.py` & `saqc-2.5.0.post0.dev145/saqc/core/frame.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import Any, Hashable, Mapping
 
 import pandas as pd
 from fancy_collections import DictOfPandas
 
 
 class DictOfSeries(DictOfPandas):
-    _key_types = (str, int, float)
-    _value_types = (pd.Series,)
+    _key_types = (str, int, float, tuple)
+    _value_types = (pd.Series, pd.DataFrame)
 
     def __init__(self, *args, **kwargs):
         # data is needed to prevent an
         # AttributeError on repr during
         # Errors within __init__
         self.data = {}
         self._attrs = None
@@ -31,49 +31,30 @@
             self._attrs = {}
         return self._attrs
 
     @attrs.setter
     def attrs(self, value: Mapping[Hashable, Any]) -> None:
         self._attrs = dict(value)
 
-    def flatten(self, promote_index: bool = False) -> DictOfSeries:
+    def astype(self, dtype: str | type) -> DictOfSeries:
         """
-        Return a copy.
-        DictOfPandas compatibility
-        """
-        return self.copy()
-
-    def index_of(self, method="union") -> pd.Index:
-        """Return an index with indices from all columns.
-
-        .. deprecated:: 2.4
-           use `DictOfSeries.union_index()` and `DictOfSeries.shared_index()` instead.
+        Cast a DictOfSeries object to the specified ``dtype``
 
         Parameters
         ----------
-        method : string, default 'all'
-            * 'union' : return the union of all indices from all columns
-            * 'shared' : return only indices that are present in every column
-            * 'all' : alias for 'union'
-            * 'intersection' : alias for 'shared'
-
-        See also
-        --------
-        DictOfSeries.to_pandas: convert a DictOfSeries to a pandas.DataFrame
+        dtype: data type to cast the entire object to.
 
         Returns
         -------
-        index: pd.Index
-            A duplicate-free index
+        DictOfSeries
         """
-        if method in ["union", "all"]:
-            return self.union_index()
-        elif method in ["intersection", "shared"]:
-            return self.shared_index()
-        raise ValueError("method must be one of 'shared' or 'union'.")
+        out = DictOfSeries()
+        for k, v in self.data.items():
+            out[k] = v.astype(dtype)
+        return out
 
 
 DictOfSeries.empty.__doc__ = """
 Indicator whether DictOfSeries is empty.
 
 True if DictOfSeries is entirely empty (no items) or all
 items are empty themselves.
@@ -162,10 +143,10 @@
 2   NaN  22.0   NaN
 4   NaN   NaN  33.0
 7   NaN   NaN  33.0
 
 or is dropped if `how='inner'`
 
 >>> di.to_pandas(how='inner')   # doctest: +NORMALIZE_WHITESPACE
-      a     b     c
-1  11.0  22.0  33.0
+    a   b   c
+1  11  22  33
 """
```

### Comparing `saqc-2.5.0/saqc/core/history.py` & `saqc-2.5.0.post0.dev145/saqc/core/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_float_dtype
 
 from saqc import UNFLAGGED
 
+AGGRGEGATIONS = {
+    "last": lambda x: x.ffill(axis=1).iloc[:, -1],
+    "max": lambda x: x.max(axis=1),
+    "min": lambda x: x.min(axis=1),
+}
+AGGREGATION = "last"
+
 
 class History:
     """
     Saqc internal storage for the history of a (single) flags column.
 
     The flag-history (FH) stores the history of a flags column. Each time
     ``append`` is called a new column is appended to the FH. The column
@@ -34,23 +41,33 @@
     [1] https://git.ufz.de/rdm-software/saqc/-/issues/143
 
     Parameters
     ----------
     index: pd.Index
         A index that fit the flags to be insert.
 
-    See Also
+    See also
     --------
     createHistoryFromData: function to create History from existing data
     """
 
     def __init__(self, index: pd.Index | None):
         self._hist = pd.DataFrame(index=index)
         self._meta = []
 
+    def __getitem__(self, key) -> History:
+        if not isinstance(key, tuple):
+            # we got a single indexer like hist[3:-4]
+            key = (key, slice(None))
+        rows, cols = key
+        out = History(index=None)
+        out._hist = self._hist.iloc[rows, cols]
+        out._meta = self._meta[cols]
+        return out
+
     @property
     def hist(self):
         return self._hist.astype(float, copy=True)
 
     @hist.setter
     def hist(self, value: pd.DataFrame) -> None:
         self._validateHist(value)
@@ -141,15 +158,17 @@
         # all following code must handle a passed empty series
 
         # ensure continuous increasing columns
         assert 0 <= pos <= len(self.columns)
         self._hist[pos] = s.astype("category")
         return self
 
-    def append(self, value: pd.Series | History, meta: dict | None = None) -> History:
+    def append(
+        self, value: pd.Series | History, meta: dict[str, Any] | None = None
+    ) -> History:
         """
         Create a new FH column and insert given pd.Series to it.
 
         Parameters
         ----------
         value : pd.Series or History
             The data to append. Must have dtype float and the index must
@@ -300,15 +319,15 @@
         2   -inf
         dtype: float64
         """
         hist = self._hist.iloc[:, slice(start, end)].astype(float)
         if hist.empty:
             result = pd.Series(data=np.nan, index=self._hist.index, dtype=float)
         else:
-            result = hist.ffill(axis=1).iloc[:, -1]
+            result = AGGRGEGATIONS[AGGREGATION](hist)
         if not raw:
             result = result.fillna(UNFLAGGED)
         result.name = None
         return result
 
     def reindex(
         self, index: pd.Index, fill_value_last: float = UNFLAGGED, copy: bool = True
```

### Comparing `saqc-2.5.0/saqc/core/mixins.py` & `saqc-2.5.0.post0.dev145/saqc/core/mixins.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/core/register.py` & `saqc-2.5.0.post0.dev145/saqc/core/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
     - `flags[field]` gets squeezed (only one history column append per call) if needed
 
     Notes
     -----
     For full control over masking, demasking and squeezing or to implement
     a multivariate function (multiple in- or outputs) use the `@register` decorator.
 
-    See Also
+    See also
     --------
         resister: generalization of of this function
     """
     if kwargs:
         raise ValueError("use '@register' to pass keywords")
     return register(mask=["field"], demask=["field"], squeeze=["field"])
 
@@ -468,14 +468,14 @@
     - no squeezing of flags
 
     Notes
     -----
     For full control over masking, demasking and squeezing or to implement
     a multivariate function (multiple in- or outputs) use the `@register` decorator.
 
-    See Also
+    See also
     --------
         resister: generalization of of this function
     """
     if kwargs:
         raise ValueError("use '@register' to pass keywords")
     return register(mask=[], demask=[], squeeze=[])
```

### Comparing `saqc-2.5.0/saqc/core/translation/basescheme.py` & `saqc-2.5.0.post0.dev145/saqc/core/translation/basescheme.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Any, Dict
 
-import numpy as np
 import pandas as pd
 
-from saqc import BAD, FILTER_ALL, GOOD, UNFLAGGED
+from saqc import BAD, FILTER_ALL, UNFLAGGED
 from saqc.core import DictOfSeries, Flags
 from saqc.lib.types import ExternalFlag
 
 ForwardMap = Dict[ExternalFlag, float]
 BackwardMap = Dict[float, ExternalFlag]
 
 
@@ -145,15 +144,16 @@
         """
         if isinstance(flags, pd.Series):
             flags = flags.to_frame()
 
         out = DictOfSeries()
         expected = pd.Index(trans_map.values())
         for field in flags.columns:
-            out[field] = flags[field].replace(trans_map)
+            with pd.option_context("future.no_silent_downcasting", True):
+                out[field] = flags[field].replace(trans_map).infer_objects()
             diff = pd.Index(out[field]).difference(expected)
             if not diff.empty:
                 raise ValueError(
                     f"following flag values could not be "
                     f"translated: {diff.drop_duplicates().to_list()}"
                 )
         return out
@@ -211,36 +211,7 @@
         Returns
         -------
         pd.DataFrame
         """
         out = self._translate(flags, self._backward)
         out.attrs = attrs or {}
         return out
-
-
-class FloatScheme(TranslationScheme):
-
-    """
-    Acts as the default Translator, provides a changeable subset of the
-    internal float flags
-    """
-
-    DFILTER_DEFAULT: float = FILTER_ALL
-
-    def __call__(self, flag: float | int) -> float:
-        try:
-            return float(flag)
-        except (TypeError, ValueError, OverflowError):
-            raise ValueError(f"invalid flag, expected a numerical value, got: {flag}")
-
-    def toInternal(self, flags: pd.DataFrame | DictOfSeries) -> Flags:
-        try:
-            return Flags(flags.astype(float))
-        except (TypeError, ValueError, OverflowError):
-            raise ValueError(
-                f"invalid flag(s), expected a collection of numerical values, got: {flags}"
-            )
-
-    def toExternal(self, flags: Flags, attrs: dict | None = None) -> DictOfSeries:
-        out = DictOfSeries(flags)
-        out.attrs = attrs or {}
-        return out
```

### Comparing `saqc-2.5.0/saqc/core/translation/dmpscheme.py` & `saqc-2.5.0.post0.dev145/saqc/core/translation/dmpscheme.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from functools import reduce
 
 import numpy as np
 import pandas as pd
 
 from saqc import BAD, DOUBTFUL, GOOD, UNFLAGGED
 from saqc.core import Flags, History
+from saqc.core.frame import DictOfSeries
 from saqc.core.translation.basescheme import BackwardMap, ForwardMap, MappingScheme
 from saqc.lib.tools import getUnionIndex
 
 _QUALITY_CAUSES = [
     "",
     "BATTERY_LOW",
     "BELOW_MINIMUM",
@@ -37,15 +38,14 @@
     "quality_flag",
     "quality_cause",
     "quality_comment",
 ]
 
 
 class DmpScheme(MappingScheme):
-
     """
     Implements the translation from and to the flagging scheme implemented in
     the UFZ - Datamanagementportal
     """
 
     ARGUMENTS = {"comment": "", "cause": "OTHER"}
 
@@ -65,62 +65,73 @@
         DOUBTFUL: "DOUBTFUL",
         BAD: "BAD",
     }
 
     def __init__(self):
         super().__init__(forward=self._FORWARD, backward=self._BACKWARD)
 
-    def toHistory(self, field_flags: pd.DataFrame):
+    def toHistory(self, flags: pd.DataFrame):
         """
         Translate a single field of external ``Flags`` to a ``History``
         """
-        field_history = History(field_flags.index)
+        history = History(flags.index)
+
+        for (flag, cause, comment), values in flags.groupby(_QUALITY_LABELS):
+            if cause == "" and comment == "":
+                continue
 
-        for (flag, cause, comment), values in field_flags.groupby(_QUALITY_LABELS):
             try:
                 comment = json.loads(comment)
             except json.decoder.JSONDecodeError:
                 comment = {"test": "unknown", "comment": ""}
 
-            histcol = pd.Series(np.nan, index=field_flags.index)
-            histcol.loc[values.index] = self(flag)
+            column = pd.Series(np.nan, index=flags.index)
+            column.loc[values.index] = self(flag)
 
             meta = {
                 "func": comment["test"],
                 "kwargs": {"comment": comment["comment"], "cause": cause},
             }
-            field_history.append(histcol, meta=meta)
-        return field_history
+            history.append(column, meta=meta)
+        return history
 
-    def toInternal(self, df: pd.DataFrame) -> Flags:
+    def toInternal(self, flags: pd.DataFrame | DictOfSeries) -> Flags:
         """
         Translate from 'external flags' to 'internal flags'
 
         Parameters
         ----------
         df : pd.DataFrame
             The external flags to translate
 
         Returns
         -------
         Flags object
         """
 
-        self.validityCheck(df)
+        if isinstance(flags, pd.DataFrame):
+            flags = DictOfSeries(flags)
+
+        self.validityCheck(flags)
 
         data = {}
 
-        for field in df.columns.get_level_values(0).drop_duplicates():
-            data[str(field)] = self.toHistory(df[field])
+        if isinstance(flags, pd.DataFrame):
+            fields = flags.columns.get_level_values(0).drop_duplicates()
+        else:
+            fields = flags.keys()
+
+        for field in fields:
+            data[str(field)] = self.toHistory(flags[field])
 
         return Flags(data)
 
     def toExternal(
         self, flags: Flags, attrs: dict | None = None, **kwargs
-    ) -> pd.DataFrame:
+    ) -> DictOfSeries:
         """
         Translate from 'internal flags' to 'external flags'
 
         Parameters
         ----------
         flags : The external flags to translate
 
@@ -129,18 +140,15 @@
 
         Returns
         -------
         translated flags
         """
         tflags = super().toExternal(flags, attrs=attrs)
 
-        out = pd.DataFrame(
-            index=getUnionIndex(tflags),
-            columns=pd.MultiIndex.from_product([flags.columns, _QUALITY_LABELS]),
-        )
+        out = DictOfSeries()
 
         for field in tflags.columns:
             df = pd.DataFrame(
                 {
                     "quality_flag": tflags[field],
                     "quality_cause": "",
                     "quality_comment": "",
@@ -160,44 +168,38 @@
                         "comment": keywords.get("comment", self.ARGUMENTS["comment"]),
                     }
                 )
                 cause = keywords.get("cause", self.ARGUMENTS["cause"])
                 df.loc[valid, "quality_comment"] = comment
                 df.loc[valid, "quality_cause"] = cause
 
-            out[field] = df.reindex(out.index)
+            out[field] = df
 
         self.validityCheck(out)
         return out
 
     @classmethod
-    def validityCheck(cls, df: pd.DataFrame) -> None:
+    def validityCheck(cls, flags: DictOfSeries) -> None:
         """
         Check wether the given causes and comments are valid.
 
         Parameters
         ----------
         df : external flags
         """
+        for df in flags.values():
 
-        cols = df.columns
-        if not isinstance(cols, pd.MultiIndex):
-            raise TypeError("DMP-Flags need multi-index columns")
-
-        if not cols.get_level_values(1).isin(_QUALITY_LABELS).all(axis=None):
-            raise TypeError(
-                f"DMP-Flags expect the labels {list(_QUALITY_LABELS)} in the secondary level"
-            )
+            if not df.columns.isin(_QUALITY_LABELS).all(axis=None):
+                raise TypeError(
+                    f"DMP-Flags expect the labels {list(_QUALITY_LABELS)} in the secondary level"
+                )
 
-        for field in df.columns.get_level_values(0):
-            # we might have NaN injected by DictOfSeries -> DataFrame conversions
-            field_df = df[field].dropna(how="all", axis="index")
-            flags = field_df["quality_flag"]
-            causes = field_df["quality_cause"]
-            comments = field_df["quality_comment"]
+            flags = df["quality_flag"]
+            causes = df["quality_cause"]
+            comments = df["quality_comment"]
 
             if not flags.isin(cls._FORWARD.keys()).all(axis=None):
                 raise ValueError(
                     f"invalid quality flag(s) found, only the following values are supported: {set(cls._FORWARD.keys())}"
                 )
 
             if not causes.isin(_QUALITY_CAUSES).all(axis=None):
```

### Comparing `saqc-2.5.0/saqc/core/translation/positionalscheme.py` & `saqc-2.5.0.post0.dev145/saqc/core/translation/positionalscheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 from saqc.constants import BAD, DOUBTFUL, GOOD, UNFLAGGED
 from saqc.core import Flags, History
+from saqc.core.frame import DictOfSeries
 from saqc.core.translation.basescheme import BackwardMap, ForwardMap, MappingScheme
 
 
 class PositionalScheme(MappingScheme):
-
     """
     Implements the translation from and to the flagging scheme implemented by CHS
     """
 
     DFILTER_DEFAULT = DOUBTFUL + 1
 
     _FORWARD: ForwardMap = {
@@ -65,37 +65,36 @@
                 index=field_flags.index,
             ).astype(int)
 
             # the exploded values form the History of `field`
             fflags = super()._translate(df, self._FORWARD)
             field_history = History(field_flags.index)
             for _, s in fflags.items():
-                field_history.append(s)
+                field_history.append(s.replace(UNFLAGGED, np.nan))
             data[str(field)] = field_history
-
         return Flags(data)
 
-    def toExternal(self, flags: Flags, **kwargs) -> pd.DataFrame:
+    def toExternal(self, flags: Flags, **kwargs) -> DictOfSeries:
         """
         Translate from 'internal flags' to 'external flags'
 
         Parameters
         ----------
         flags : pd.DataFrame
             The external flags to translate
 
         Returns
         -------
-        pd.DataFrame
+        DictOfSeries
         """
-        out = {}
+        out = DictOfSeries()
         for field in flags.columns:
             thist = flags.history[field].hist.replace(self._BACKWARD).astype(float)
             # concatenate the single flag values
             ncols = len(thist.columns)
             init = 9 * 10**ncols
             bases = 10 ** np.arange(ncols - 1, -1, -1)
 
             tflags = init + (thist * bases).sum(axis=1)
-            out[field] = tflags
+            out[field] = tflags.fillna(-9999).astype(int)
 
-        return pd.DataFrame(out).fillna(-9999).astype(int)
+        return out
```

### Comparing `saqc-2.5.0/saqc/core/translation/simplescheme.py` & `saqc-2.5.0.post0.dev145/saqc/core/translation/simplescheme.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy as np
 
 from saqc.constants import BAD, GOOD, UNFLAGGED
 from saqc.core.translation import MappingScheme
 
 
 class SimpleScheme(MappingScheme):
-
     """
     Acts as the default Translator, provides a changeable subset of the
     internal float flags
     """
 
     _FORWARD = {
         "UNFLAGGED": UNFLAGGED,
```

### Comparing `saqc-2.5.0/saqc/funcs/__init__.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/funcs/breaks.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/breaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,17 @@
 
         Notes
         -----
         A series of values :math:`x_k,x_{k+1},...,x_{k+n}`, with associated
         timestamps :math:`t_k,t_{k+1},...,t_{k+n}`, is considered to be isolated, if:
 
         1. :math:`t_{k+1} - t_n <` `group_window`
-        2. None of the :math:`x_j` with :math:`0 < t_k - t_j <` `gap_window`,
-            is valid (preceeding gap).
-        3. None of the :math:`x_j` with :math:`0 < t_j - t_(k+n) <` `gap_window`,
-            is valid (succeding gap).
+        2. None of the :math:`x_j` with :math:`0 < t_k - t_j <` `gap_window`, is valid (preceding gap).
+        3. None of the :math:`x_j` with :math:`0 < t_j - t_(k+n) <` `gap_window`, is valid (succeeding gap).
+
         """
         validateWindow(gap_window, name="gap_window", allow_int=False)
         validateWindow(group_window, name="group_window", allow_int=False)
 
         dat = self._data[field].dropna()
         if dat.empty:
             return self
@@ -142,32 +141,32 @@
     ) -> "SaQC":
         """
         Flag jumps and drops in data.
 
         Flag data where the mean of its values significantly changes (where the data "jumps" from one
         value level to another).
         Value changes are detected by comparing the mean for two adjacent rolling windows. Whenever
-        the difference between the mean in the two windows exceeds py:attr:`thresh`, the value between
+        the difference between the mean in the two windows exceeds :py:attr:`thresh` , the value between
         the windows is flagged.
 
         Parameters
         ----------
         thresh :
             Threshold value by which the mean of data has to jump, to trigger flagging.
 
         window :
             Size of the two moving windows. This determines the number of observations used for
             calculating the mean in every window. The window size should be big enough to yield enough
             samples for a reliable mean calculation, but it should also not be arbitrarily big, since
             it also limits the density of jumps that can be detected.
             More precisely: Jumps that are not distanced to each other by more than three fourth (3/4)
-            of the selected py:attr:`window` size, will not be detected reliably.
+            of the selected :py:attr:`window` size, will not be detected reliably.
 
         min_periods :
-            The minimum number of observations in py:attr:`window` required to calculate a valid mean value.
+            The minimum number of observations in :py:attr:`window` required to calculate a valid mean value.
 
         Examples
         --------
 
         Below picture gives an abstract interpretation of the parameter interplay in case of a positive
         value jump, initialising a new mean level.
```

### Comparing `saqc-2.5.0/saqc/funcs/changepoints.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/changepoints.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/funcs/constants.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,37 +47,38 @@
          - (2): abs(y(t + i) - (t + j)) < `thresh`, for all i,j in [0, 1, ..., n]
 
         Parameters
         ----------
         thresh :
             Maximum total change allowed per window.
 
+        window :
+            Size of the moving window. This determines the number of observations used
+            for calculating the absolute change per window.
+            Each window will either contain a fixed number of periods (integer defined window),
+            or will have a fixed temporal extension (offset defined window).
+
         min_periods :
             Minimum number of observations in window required to generate
-            a flag. Must be an integer greater or equal `2`, because a
+            a flag. This can be used to exclude underpopulated *offset* defined windows from
+            flagging. (Integer defined windows will always contain exactly *window* samples).
+            Must be an integer greater or equal `2`, because a
             single value would always be considered constant.
             Defaults to `2`.
-
-        window :
-            Size of the moving window. This is the number of observations used
-            for calculating the statistic. Each window will be a fixed size.
-            If it is an offset then this will be the time period of each window.
-            Each window will be a variable sized based on the observations included
-            in the time-period.
         """
         d: pd.Series = self._data[field]
         validateWindow(window, index=d.index)
         validateMinPeriods(min_periods, minimum=2, optional=False)
 
         # 1. find starting points of consecutive constant values as a boolean mask
         # 2. fill the whole window with True's
         rolling = d.rolling(window=window, min_periods=min_periods)
         starting_points_mask = rolling.max() - rolling.min() <= thresh
 
-        removeRollingRamps(starting_points_mask, window=window, inplace=True)
+        starting_points_mask = removeRollingRamps(starting_points_mask, window=window)
 
         # mimic forward rolling by roll over inverse [::-1]
         rolling = starting_points_mask[::-1].rolling(
             window=window, min_periods=min_periods
         )
         # mimic any()
         mask = (rolling.sum()[::-1] > 0) & d.notna()
```

### Comparing `saqc-2.5.0/saqc/funcs/curvefit.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/curvefit.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from saqc.core import DictOfSeries, Flags, register
 from saqc.lib.checking import (
     validateChoice,
     validateMinPeriods,
     validateValueBounds,
     validateWindow,
 )
-from saqc.lib.tools import extractLiteral, getFreqDelta
+from saqc.lib.tools import getFreqDelta
 from saqc.lib.ts_operators import (
     butterFilter,
     polyRoller,
     polyRollerIrregular,
     polyRollerNoMissing,
 )
```

### Comparing `saqc-2.5.0/saqc/funcs/drift.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import functools
 import inspect
 import warnings
-from typing import TYPE_CHECKING, Callable, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Callable, Literal, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 from scipy.spatial.distance import pdist
-from typing_extensions import Literal
 
 from saqc import BAD
 from saqc.core import DictOfSeries, Flags, flagging, register
 from saqc.funcs.changepoints import _getChangePoints
 from saqc.lib.checking import (
     validateCallable,
     validateChoice,
@@ -306,21 +305,24 @@
 
         Examples
         --------
         Some examples of meaningful driftmodels.
 
         Linear drift modell (no free parameters).
 
+        .. doctest::
 
-        >>> Model = lambda t, origin, target: origin + t*target
+            >>> Model = lambda t, origin, target: origin + t*target
 
         exponential drift model (exponential raise!)
 
-        >>> expFunc = lambda t, a, b, c: a + b * (np.exp(c * x) - 1)
-        >>> Model = lambda t, p, origin, target: expFunc(t, (target - origin) / (np.exp(abs(c)) - 1), abs(c))
+        .. doctest::
+
+            >>> expFunc = lambda t, a, b, c: a + b * (np.exp(c * x) - 1)
+            >>> Model = lambda t, p, origin, target: expFunc(t, (target - origin) / (np.exp(abs(c)) - 1), abs(c))
 
         Exponential and linear driftmodels are part of the ``ts_operators`` library, under the names
         ``expDriftModel`` and ``linearDriftModel``.
 
         """
         if isinstance(model, str):
             model = DRIFT_MODELS.get(model, None)
@@ -356,15 +358,15 @@
         shift_targets = drift_grouper.aggregate(lambda x: x[:cal_range].mean()).shift(
             -1
         )
 
         for k, group in drift_grouper:
             data_series = group[field]
             data_fit, data_shiftTarget = _driftFit(
-                data_series, shift_targets.loc[k, :][0], cal_range, model
+                data_series, shift_targets.loc[k, :].iloc[0], cal_range, model
             )
             data_fit = pd.Series(data_fit, index=group.index)
             data_shiftTarget = pd.Series(data_shiftTarget, index=group.index)
             data_shiftVektor = data_shiftTarget - data_fit
             shiftedData = data_series + data_shiftVektor
             to_correct[shiftedData.index] = shiftedData
```

### Comparing `saqc-2.5.0/saqc/funcs/flagtools.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/flagtools.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,56 +13,71 @@
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from saqc import BAD, FILTER_ALL, UNFLAGGED
 from saqc.core import DictOfSeries, flagging, register
+from saqc.core.flags import Flags
 from saqc.core.history import History
 from saqc.lib.checking import validateChoice, validateWindow
-from saqc.lib.tools import initializeTargets, isflagged, isunflagged, toSequence
+from saqc.lib.tools import (
+    initializeTargets,
+    isflagged,
+    isunflagged,
+    multivariateParameters,
+    toSequence,
+)
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
 class FlagtoolsMixin:
     @flagging()
     def flagDummy(self: "SaQC", field: str, **kwargs) -> "SaQC":
         """
         Function does nothing but returning data and flags.
+
+        Parameters
+        ----------
+
         """
         return self
 
     @register(mask=[], demask=[], squeeze=["field"])
     def forceFlags(self: "SaQC", field: str, flag: float = BAD, **kwargs) -> "SaQC":
         """
         Set whole column to a flag value.
 
-        See Also
+        Parameters
+        ----------
+
+        See also
         --------
         clearFlags : set whole column to UNFLAGGED
         flagUnflagged : set flag value at all unflagged positions
+
         """
         self._flags[:, field] = flag
         return self
 
     @register(mask=[], demask=[], squeeze=["field"])
     def clearFlags(self: "SaQC", field: str, **kwargs) -> "SaQC":
         """
-        Set whole column to UNFLAGGED.
+        Assign UNFLAGGED value to all periods in field.
 
         Notes
         -----
         This function ignores the ``dfilter`` keyword, because the data
         is not relevant for processing.
         A warning is triggered if the ``flag`` keyword is given, because
         the flags are always set to `UNFLAGGED`.
 
-        See Also
+        See also
         --------
         forceFlags : set whole column to a flag value
         flagUnflagged : set flag value at all unflagged positions
         """
         # NOTE: do we really need this?
         if "flag" in kwargs:
             kwargs = {**kwargs}  # copy
@@ -72,28 +87,93 @@
         return self.forceFlags(field, flag=UNFLAGGED, **kwargs)
 
     @register(mask=[], demask=[], squeeze=["field"])
     def flagUnflagged(self: "SaQC", field: str, flag: float = BAD, **kwargs) -> "SaQC":
         """
         Function sets a flag at all unflagged positions.
 
-        See Also
-        --------
-        clearFlags : set whole column to UNFLAGGED
-        forceFlags : set whole column to a flag value
+        Parameters
+        ----------
 
         Notes
         -----
         This function ignores the ``dfilter`` keyword, because the
         data is not relevant for processing.
+
+        See also
+        --------
+        clearFlags : set whole column to UNFLAGGED
+        forceFlags : set whole column to a flag value
+
         """
+
         unflagged = self._flags[field].isna() | (self._flags[field] == UNFLAGGED)
         self._flags[unflagged, field] = flag
         return self
 
+    @flagging()
+    def setFlags(
+        self,
+        field: str,
+        data: str | list | np.ndarray | pd.Series,
+        override: bool = False,
+        flag: float = BAD,
+        **kwargs,
+    ) -> "SaQC":
+        """
+        Include flags listed in external data.
+
+        Parameters
+        ----------
+
+        data :
+            Determines which timestamps to set flags at, depending on the passed type:
+
+            * 1-d `array` or `List` of timestamps or `pandas.Index`: flag `field` with `flag` at every timestamp in `f_data`
+            * 2-d `array` or List of tuples: for all elements `t[k]` out of f_data:
+              flag `field` with `flag` at every timestamp in between `t[k][0]` and `t[k][1]`
+            * pd.Series: flag `field` with `flag` in between any index and data value of the passed series
+            * str: use the variable timeseries `f_data` as flagging template
+            * pd.Series: flag `field` with `flag` in between any index and data value of the passed series
+            * 1-d `array` or `List` of timestamps: flag `field` with `flag` at every timestamp in `f_data`
+            * 2-d `array` or List of tuples: for all elements `t[k]` out of f_data:
+              flag `field` with `flag` at every timestamp in between `t[k][0]` and `t[k][1]`
+        override :
+            determines if flags shall be assigned although the value in question already has a flag assigned.
+        """
+        to_flag = pd.Series(False, index=self._data[field].index)
+
+        # check if f_data is meant to denote timestamps:
+        if (isinstance(data, (list, np.ndarray, pd.Index))) and not isinstance(
+            data[0], (tuple, np.ndarray)
+        ):
+            set_idx = pd.DatetimeIndex(data).intersection(to_flag.index)
+            to_flag[set_idx] = True
+        else:  # f_data denotes intervals:
+            if isinstance(data, (str, pd.Series)):
+                if isinstance(data, str):
+                    flags_data = self._data[data]
+                else:
+                    flags_data = data
+                intervals = flags_data.items()
+            else:
+                intervals = data
+            for s in intervals:
+                to_flag[s[0] : s[1]] = True
+
+        # elif isinstance(f_data, list):
+        if not override:
+
+            to_flag &= isunflagged(self._flags[field], thresh=kwargs["dfilter"])
+            # to_flag &= (self._flags[field] < flag) & (
+            #     self._flags[field] >= kwargs["dfilter"]
+            # )
+        self._flags[to_flag.values, field] = flag
+        return self
+
     @register(mask=["field"], demask=["field"], squeeze=["field"])
     def flagManual(
         self: "SaQC",
         field: str,
         mdata: str | pd.Series | np.ndarray | list | pd.DataFrame | DictOfSeries,
         method: Literal[
             "left-open", "right-open", "closed", "plain", "ontime"
@@ -104,14 +184,17 @@
         **kwargs,
     ) -> "SaQC":
         """
         Include flags listed in external data.
 
         The method allows to integrate pre-existing flagging information.
 
+            .. deprecated:: 2.6.0
+               Deprecated Function. See :py:meth:`~saqc.SaQC.setFlags`.
+
         Parameters
         ----------
         mdata :
             Determines which values or intervals will be flagged. Supported input types:
 
             * ``pd.Series``: Needs a datetime index and values of type:
 
@@ -211,14 +294,19 @@
            2000-01-31    False
            2000-02-01     True
            2000-02-02     True
            2000-03-01     True
            2000-05-01     True
            dtype: bool
         """
+        warnings.warn(
+            "`flagManual` is deprecated and will be removed in version 2.8 of saqc. "
+            "Please use `setFlags` for similar functionality.",
+            DeprecationWarning,
+        )
         validateChoice(
             method, "method", ["left-open", "right-open", "closed", "plain", "ontime"]
         )
         validateChoice(mformat, "mformat", ["start-end", "mflag"])
 
         dat = self._data[field]
         # internal not-mflag-value -> cant go for np.nan
@@ -276,46 +364,46 @@
             if method == "closed":
                 mdata[mdata.ffill() == mflag] = mflag
                 mdata.replace({not_mflag: mflag}, inplace=True)
         else:
             raise ValueError(method)
 
         mask = mdata == mflag
-        mask = mask.reindex(dat.index).fillna(False)
+        mask = mask.reindex(dat.index, fill_value=False)  # .fillna(False)
 
         self._flags[mask, field] = flag
         return self
 
     @register(
         mask=[],
         demask=[],
         squeeze=[],
         handles_target=True,  # function defines a target parameter, so it needs to handle it
+        multivariate=True,
     )
     def transferFlags(
         self: "SaQC",
         field: str,
         target: str | None = None,
         squeeze: bool = False,
         overwrite: bool = False,
         **kwargs,
     ) -> "SaQC":
         """
         Transfer Flags of one variable to another.
 
+        Parameters
+        ----------
+
         squeeze :
             Squeeze the history into a single column if ``True``, function specific flag information is lost.
 
         overwrite :
             Overwrite existing flags if ``True``.
 
-        See Also
-        --------
-        * :py:meth:`saqc.SaQC.flagGeneric`
-        * :py:meth:`saqc.SaQC.concatFlags`
 
         Examples
         --------
         First, generate some data with some flags:
 
         .. doctest:: exampleTransfer
 
@@ -344,46 +432,74 @@
         .. doctest:: exampleTransfer
 
            >>> qc = qc.transferFlags(['a','a'], ['b', 'c'], overwrite=True)
            >>> qc.flags.to_pandas()
                   a      b      c
            0   -inf   -inf   -inf
            1  255.0  255.0  255.0
-        """
-        history = self._flags.history[field]
 
-        if target is None:
-            target = field
+        See also
+        --------
+        * :py:meth:`saqc.SaQC.flagGeneric`
+        * :py:meth:`saqc.SaQC.concatFlags`
 
-        if overwrite is False:
-            mask = isflagged(self._flags[target], thresh=kwargs["dfilter"])
-            history._hist[mask] = np.nan
+        """
 
-        # append a dummy column
+        fields, targets, broadcasting = multivariateParameters(field, target)
         meta = {
             "func": f"transferFlags",
             "args": (),
             "kwargs": {
                 "field": field,
                 "target": target,
                 "squeeze": squeeze,
                 "overwrite": overwrite,
                 **kwargs,
             },
         }
 
-        if squeeze:
-            flags = history.squeeze(raw=True)
-            # init an empty history to which we later append the squeezed flags
-            history = History(index=history.index)
-        else:
-            flags = pd.Series(np.nan, index=history.index, dtype=float)
+        for field, target in zip(fields, targets):
+            # initialize non existing targets
+            if target not in self._data:
+                self._data[target] = pd.Series(np.nan, index=self._data[field].index)
+                self._flags._data[target] = History(self._data[target].index)
+            if not self._data[field].index.equals(self._data[target].index):
+                raise ValueError(
+                    f"All Field and Target indices must match!\n"
+                    f"Indices of {field} and {target} seem to be not congruent within the context of the given\n"
+                    f"- fields: {fields}\n "
+                    f"- and targets: {targets}"
+                )
+            history = self._flags.history[field].copy(deep=True)
 
-        history.append(flags, meta)
-        self._flags.history[target].append(history)
+            if overwrite is False:
+                mask = isflagged(self._flags[target], thresh=kwargs["dfilter"])
+                history._hist[mask] = np.nan
+
+            if squeeze:
+                # add squeezed flags
+                flags = history.squeeze(raw=True)
+                history = History(index=history.index).append(flags, meta)
+            elif broadcasting is False:
+                # add an empty flags
+                flags = pd.Series(np.nan, index=history.index, dtype=float)
+                history.append(flags, meta)
+            # else:
+            #    broadcasting -> multiple fields will be written to one target
+            #    only add the fields' histories and add an empty column later
+
+            self._flags.history[target].append(history)
+
+        if broadcasting and not squeeze:
+            # add one final history column
+            # all targets are identical, if we broadcast fields -> target
+            target = targets[0]
+            history = self._flags.history[target]
+            flags = pd.Series(np.nan, index=history.index, dtype=float)
+            self._flags.history[target].append(flags, meta)
 
         return self
 
     @flagging()
     def propagateFlags(
         self: "SaQC",
         field: str,
@@ -517,15 +633,15 @@
         """
         Flag all values, if all the given ``field`` values are already flagged.
 
         Parameters
         ----------
         group:
             A collection of ``SaQC`` objects. Flag checks are performed on all ``SaQC`` objects
-            based on the variables specified in :py:attr:`field`. Whenever all monitored variables
+            based on the variables specified in ``field``. Whenever all monitored variables
             are flagged, the associated timestamps will receive a flag.
         """
         return _groupOperation(
             saqc=self,
             field=field,
             target=target,
             func=operator.and_,
@@ -662,10 +778,10 @@
             mask = func(mask, flagged)
 
     targets = _flatten(targets)
     saqc = initializeTargets(saqc, _flatten(fields), targets, mask.index)
 
     # write flags
     for t in targets:
-        saqc._flags[mask, t] = flag
+        saqc._flags[mask & isunflagged(saqc._flags[t], thresh=dfilter), t] = flag
 
     return saqc
```

### Comparing `saqc-2.5.0/saqc/funcs/generic.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,16 +21,17 @@
     from saqc import SaQC
 
 
 class GenericFunction(Protocol):
     __name__: str
     __globals__: dict[str, Any]
 
-    def __call__(self, *args: pd.Series) -> pd.Series | pd.DataFrame | DictOfSeries:
-        ...  # pragma: no cover
+    def __call__(
+        self, *args: pd.Series
+    ) -> pd.Series | pd.DataFrame | DictOfSeries: ...  # pragma: no cover
 
 
 def _flagSelect(field: str, flags: Flags, label: str | None = None) -> pd.Series:
     if label is None:
         return flags[field]
 
     h_meta = flags.history[field].meta
@@ -59,31 +60,51 @@
     globs = {
         "isflagged": lambda data, label=None: isflagged(
             _flagSelect(data.name, flags, label), thresh=dfilter
         ),
         **ENVIRONMENT,
     }
 
+    # some function don't have a globals attribute (e.g. np.sum)
+    if not hasattr(func, "__globals__"):
+        func.__globals__ = {}
     func.__globals__.update(globs)
 
     if isinstance(data, pd.Series):
         data = data.to_frame()
 
     # set series.name, because `isflagged` relies on it
     cols = []
     for c in data.columns:
         data[c].name = c
         cols.append(data[c])
     return func(*cols)
 
 
+def _inferBroadcast(obj, trg_shape) -> pd.DataFrame:
+    # simple single value broadcasting
+    if pd.api.types.is_scalar(obj):
+        return np.full(trg_shape, obj)
+    return obj
+
+
+def _inferDF(obj, cols, index):
+    # infer dataframe if result is numpy array of fitting shape
+    if isinstance(obj, np.ndarray):
+        lc = len(cols)
+        li = len(index)
+        if (obj.shape == (li, lc)) or (obj.shape == (li,)):
+            return pd.DataFrame(obj, columns=cols, index=index)
+    return obj
+
+
 def _castResult(obj) -> DictOfSeries:
     # Note: the actual keys aka. column names
     # we use here to create a DictOfSeries
-    # are never used, and only exists temporary.
+    # are never used and only exist temporarily.
 
     if isinstance(obj, pd.Series):
         return DictOfSeries({"0": obj})
     if pd.api.types.is_dict_like(obj):
         # includes pd.Series and
         # everything with keys and __getitem__
         return DictOfSeries(obj)
@@ -146,15 +167,18 @@
         1970-01-01         1         2              3
         """
 
         fields = toSequence(field)
         targets = fields if target is None else toSequence(target)
 
         dchunk, fchunk = self._data[fields].copy(), self._flags[fields].copy()
+        trg_idx = dchunk[dchunk.columns[0]].index
         result = _execGeneric(fchunk, dchunk, func, dfilter=dfilter)
+        result = _inferBroadcast(result, (len(trg_idx), len(targets)))
+        result = _inferDF(result, cols=targets, index=trg_idx)
         result = _castResult(result)
 
         # update data & flags
         for i, col in enumerate(targets):
             datacol = result[result.columns[i]]
             self._data[col] = datacol
 
@@ -226,29 +250,33 @@
         """
 
         fields = toSequence(field)
         targets = fields if target is None else toSequence(target)
         dfilter = kwargs.get("dfilter", BAD)
 
         dchunk, fchunk = self._data[fields].copy(), self._flags[fields].copy()
+        trg_idx = dchunk[dchunk.columns[0]].index
         result = _execGeneric(fchunk, dchunk, func, dfilter=dfilter)
+        result = _inferBroadcast(result, (len(trg_idx), len(targets)))
+        result = _inferDF(result, cols=targets, index=trg_idx)
         result = _castResult(result)
 
-        if len(targets) != len(result.columns):
+        if len(result.columns) > 1 and len(targets) != len(result.columns):
             raise ValueError(
                 f"the generic function returned {len(result.columns)} field(s), "
                 f"but {len(targets)} target(s) were given"
             )
 
         if not result.empty and not isAllBoolean(result):
             raise TypeError(f"generic expression does not return a boolean array")
 
         # update flags & data
         for i, col in enumerate(targets):
-            mask = result[result.columns[i]]
+            # broadcast one column results to all targets
+            mask = result[result.columns[i if len(result.columns) > 1 else 0]]
 
             # make sure the column exists
             if col not in self._flags:
                 self._flags[col] = pd.Series(np.nan, index=mask.index)
 
             # respect existing flags
             mask = isunflagged(self._flags[col], thresh=dfilter) & mask
```

### Comparing `saqc-2.5.0/saqc/funcs/interpolation.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,656 +3,530 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
+import pickle
+import tkinter as tk
 import warnings
-from typing import TYPE_CHECKING, Callable, Tuple, Union
+from typing import TYPE_CHECKING
 
+import matplotlib as mpl
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
-from saqc import UNFLAGGED
-from saqc.core import register
-from saqc.core.history import History
-from saqc.lib.checking import (
-    isValidChoice,
-    validateCallable,
-    validateChoice,
-    validateMinPeriods,
-    validateValueBounds,
-    validateWindow,
-)
-from saqc.lib.tools import isflagged
-from saqc.lib.ts_operators import interpolateNANs, shift2Freq
+from saqc import BAD, FILTER_NONE, UNFLAGGED
+from saqc.core import processing, register
+from saqc.lib.checking import validateChoice
+from saqc.lib.docs import DOC_TEMPLATES
+from saqc.lib.plotting import makeFig
+from saqc.lib.selectionGUI import MplScroller, SelectionOverlay
+from saqc.lib.tools import periodicMask
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
-# TODO: remove, when `interpolateIndex` and `interpolateInvalid are removed`
-INTERPOLATION_METHODS = Literal[
-    "linear",
-    "time",
-    "nearest",
-    "zero",
-    "slinear",
-    "quadratic",
-    "cubic",
-    "spline",
-    "barycentric",
-    "polynomial",
-    "krogh",
-    "piecewise_polynomial",
-    "spline",
-    "pchip",
-    "akima",
-]
-
-
-def _resampleOverlapping(data: pd.Series, freq: str, fill_value):
-    """TODO: docstring needed"""
-    dtype = data.dtype
-    end = data.index[-1].ceil(freq)
-    data = data.resample(freq).max()
-    data = data.combine(data.shift(1, fill_value=fill_value), max)
-    if end not in data:
-        data.loc[end] = fill_value
-    return data.fillna(fill_value).astype(dtype)
+_MPL_DEFAULT_BACKEND = mpl.get_backend()
+_TEST_MODE = False
 
 
-class InterpolationMixin:
-    @register(
-        mask=["field"],
-        demask=["field"],
-        squeeze=[],  # func handles history by itself
-    )
-    def interpolateByRolling(
+class ToolsMixin:
+    @register(mask=[], demask=[], squeeze=[], multivariate=True)
+    def flagByClick(
         self: "SaQC",
-        field: str,
-        window: str | int,
-        func: Callable[[pd.Series], float] = np.median,
-        center: bool = True,
-        min_periods: int = 0,
-        flag: float = UNFLAGGED,
+        field: str | list[str],
+        max_gap: str | None = None,
+        gui_mode: Literal["GUI", "overlay"] = "GUI",
+        selection_marker_kwargs: dict | None = None,
+        dfilter: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        Replace NaN by the aggregation result of the surrounding window.
+        Pop up GUI for adding or removing flags by selection of points in the data plot.
+
+        * Left click and Drag the selection area over the points you want to add to selection.
+
+        * Right clack and drag the selection area over the points you want to remove from selection
+
+        * press 'shift' to switch between rectangle and span selector
+
+        * press 'enter' or click "Assign Flags" to assign flags to the selected points and end session
+
+        * press 'escape' or click "Discard" to end Session without assigneing flags to selection
+
+        * activate the sliders attached to each axes to bind the respective variable. When using the
+          span selector, points from all bound variables will be added synchronously.
+
+
+        Note, that you can only mark already flagged values, if `dfilter` is set accordingly.
+
+        Note, that you can use `flagByClick` to "unflag" already flagged values, when setting `dfilter` above the flag to
+        "unset", and setting `flag` to a flagging level associated with your "unflagged" level.
 
         Parameters
         ----------
-        window :
-            The size of the window, the aggregation is computed from.
-            An integer define the number of periods to be used, a string
-            is interpreted as an offset. ( see `pandas.rolling` for more
-            information). Integer windows may result in screwed aggregations
-            if called on none-harmonized or irregular data.
-
-        func : default median
-            The function used for aggregation.
-
-        center :
-            Center the window around the value. Can only be used with
-            integer windows, otherwise it is silently ignored.
-
-        min_periods :
-            Minimum number of valid (not np.nan) values that have to be
-            available in a window for its aggregation to be
-            computed.
-        """
-        validateWindow(window)
-        validateCallable(func, "func")
-        validateMinPeriods(min_periods)
-
-        datcol = self._data[field]
-        roller = datcol.rolling(window=window, center=center, min_periods=min_periods)
-        try:
-            func_name = func.__name__
-            if func_name[:3] == "nan":
-                func_name = func_name[3:]
-            rolled = getattr(roller, func_name)()
-        except AttributeError:
-            rolled = roller.apply(func)
-
-        na_mask = datcol.isna()
-        interpolated = na_mask & rolled.notna()
-        datcol[na_mask] = rolled[na_mask]
-        self._data[field] = datcol
-
-        flagcol = pd.Series(np.nan, index=self._flags[field].index)
-        flagcol.loc[interpolated] = np.nan if flag is None else flag
-
-        meta = {
-            "func": "interpolateByRolling",
-            "args": (field,),
-            "kwargs": {
-                "window": window,
-                "func": func,
-                "center": center,
-                "min_periods": min_periods,
-                "flag": flag,
-                **kwargs,
-            },
-        }
-        self._flags.history[field].append(flagcol, meta)
+        max_gap :
+            If ``None``, all data points will be connected, resulting in long linear
+            lines, in case of large data gaps. ``NaN`` values will be removed before
+            plotting. If an offset string is passed, only points that have a distance
+            below ``max_gap`` are connected via the plotting line.
+        gui_mode :
+            * ``"GUI"`` (default), spawns TK based pop-up GUI, enabling scrolling and binding for subplots
+            * ``"overlay"``, spawns matplotlib based pop-up GUI. May be less conflicting, but does not support
+              scrolling or binding.
+        """
+        data, flags = self._data.copy(), self._flags.copy()
+
+        flag = kwargs.get("flag", BAD)
+        scrollbar = True if gui_mode == "GUI" else False
+        selection_marker_kwargs = selection_marker_kwargs or {}
+
+        if not scrollbar:
+            plt.rcParams["toolbar"] = "toolmanager"
+
+        if not _TEST_MODE:
+            plt.close("all")
+            mpl.use(_MPL_DEFAULT_BACKEND)
+        else:
+            mpl.use("Agg")
+
+        # make base figure, the gui will wrap
+        fig = makeFig(
+            data=data,
+            field=field,
+            flags=flags,
+            level=UNFLAGGED,
+            mode="subplots",
+            max_gap=max_gap,
+            history="valid",
+            xscope=None,
+            ax_kwargs={"ncols": 1},
+            scatter_kwargs={},
+            plot_kwargs={},
+        )
 
+        overlay_data = []
+        for f in field:
+            overlay_data.extend([(data[f][flags[f] < dfilter]).dropna()])
+
+        if scrollbar:  # spawn TK based GUI
+            root = tk.Tk()
+            scroller = MplScroller(root, fig=fig)
+            root.protocol("WM_DELETE_WINDOW", scroller.assignAndQuitFunc())
+            scroller.pack(side="top", fill="both", expand=True)
+
+        else:  # only use figure window overlay
+            scroller = None
+
+        selector = SelectionOverlay(
+            fig.axes,
+            data=overlay_data,
+            selection_marker_kwargs=selection_marker_kwargs,
+            parent=scroller,
+        )
+        if _TEST_MODE & scrollbar:
+            root.after(2000, root.destroy)
+            # return self
+
+        if scrollbar:
+            root.attributes("-fullscreen", True)
+            root.mainloop()
+            if not _TEST_MODE:
+                root.destroy()
+        else:  # show figure if only overlay is used
+            plt.show(block=not _TEST_MODE)
+            plt.rcParams["toolbar"] = "toolbar2"
+
+        # disconnect mouse events when GUI is closed
+        selector.disconnect()
+
+        # assign flags only if selection was confirmed by user
+        if selector.confirmed:
+            for k in range(selector.N):
+                to_flag = selector.index[k][selector.marked[k]]
+
+                new_col = pd.Series(np.nan, index=self._flags[field[k]].index)
+                new_col.loc[to_flag] = flag
+                self._flags.history[field[k]].append(
+                    new_col, {"func": "flagByClick", "args": (), "kwargs": kwargs}
+                )
         return self
 
     @register(
-        mask=["field"],
+        mask=[],
         demask=[],
-        squeeze=[],  # func handles history by itself
+        squeeze=[],
+        handles_target=True,
+        docstring={"target": DOC_TEMPLATES["target"]},
     )
-    def interpolate(
+    def copyField(
         self: "SaQC",
         field: str,
-        method: INTERPOLATION_METHODS = "time",
-        order: int = 2,
-        limit: int | str | None = None,
-        extrapolate: Literal["forward", "backward", "both"] | None = None,
-        flag: float = UNFLAGGED,
+        target: str,
+        overwrite: bool = False,
         **kwargs,
     ) -> "SaQC":
         """
-        Fill NaN and flagged values using an interpolation method.
-
-        .. deprecated:: 2.4.0
-           Use :py:meth:`~saqc.SaQC.align` instead.
+        Make a copy of the data and flags of `field`.
 
         Parameters
         ----------
-        method :
-            Interpolation technique to use. One of:
-
-            * ‘linear’: Ignore the index and treat the values as equally spaced.
-            * ‘time’: Works on daily and higher resolution data to interpolate given length of interval.
-            * ‘index’, ‘values’: Use the actual numerical values of the index.
-            * ‘pad’: Fill in NaNs using existing values.
-            * ‘nearest’, ‘zero’, ‘slinear’, ‘quadratic’, ‘cubic’, ‘spline’, ‘barycentric’, ‘polynomial’:
-                 Passed to scipy.interpolate.interp1d. These methods use the numerical values of the index.
-                 Both ‘polynomial’ and ‘spline’ require that you also specify an order (int), e.g.
-                 ``qc.interpolate(method='polynomial', order=5)``.
-            * ‘krogh’, ‘spline’, ‘pchip’, ‘akima’, ‘cubicspline’:
-                 Wrappers around the SciPy interpolation methods of similar names.
-            * ‘from_derivatives’: Refers to scipy.interpolate.BPoly.from_derivatives
-
-        order :
-            Order of the interpolation method, ignored if not supported
-            by the chosen ``method``
-
-        limit :
-            Maximum number of missing values to interpolate. Only gaps
-            smaller than ``limit`` will be filled. The gap size can be
-            given as a number of values (integer) or a temporal extensions
-            (offset string). With ``None``, all missing values will be
-            interpolated.
-
-        extrapolate :
-            Use parameter to perform extrapolation instead of interpolation
-            onto the trailing and/or leading chunks of NaN values in data series.
-
-            * 'None' (default) - perform interpolation
-            * 'forward'/'backward' - perform forward/backward extrapolation
-            * 'both' - perform forward and backward extrapolation
+        overwrite :
+            overwrite target, if already existant.
 
-        Examples
-        --------
-        See some examples of the keyword interplay below:
+        """
+        if field == target:
+            return self
 
-        Lets generate some dummy data:
+        if target in self._flags.columns.union(self._data.columns):
+            if not overwrite:
+                raise ValueError(f"{target}: already exist")
+            self = self.dropField(field=target)
 
-        .. doctest:: interpolate
+        self._data[target] = self._data[field].copy()
+        self._flags.history[target] = self._flags.history[field].copy()
 
-           >>> data = pd.DataFrame({'data':np.array([np.nan, 0, np.nan, np.nan, np.nan, 4, 5, np.nan, np.nan, 8, 9, np.nan, np.nan])}, index=pd.date_range('2000',freq='1H', periods=13))
-           >>> data
-                                data
-           2000-01-01 00:00:00   NaN
-           2000-01-01 01:00:00   0.0
-           2000-01-01 02:00:00   NaN
-           2000-01-01 03:00:00   NaN
-           2000-01-01 04:00:00   NaN
-           2000-01-01 05:00:00   4.0
-           2000-01-01 06:00:00   5.0
-           2000-01-01 07:00:00   NaN
-           2000-01-01 08:00:00   NaN
-           2000-01-01 09:00:00   8.0
-           2000-01-01 10:00:00   9.0
-           2000-01-01 11:00:00   NaN
-           2000-01-01 12:00:00   NaN
-
-        Use :py:meth:`~saqc.SaQC.interpolate` to do linear interpolation
-        of up to 2 consecutive missing values:
-
-        .. doctest:: interpolate
-
-           >>> qc = saqc.SaQC(data)
-           >>> qc = qc.interpolate("data", limit=3, method='time')
-           >>> qc.data # doctest:+NORMALIZE_WHITESPACE
-                               data |
-           ======================== |
-           2000-01-01 00:00:00  NaN |
-           2000-01-01 01:00:00  0.0 |
-           2000-01-01 02:00:00  NaN |
-           2000-01-01 03:00:00  NaN |
-           2000-01-01 04:00:00  NaN |
-           2000-01-01 05:00:00  4.0 |
-           2000-01-01 06:00:00  5.0 |
-           2000-01-01 07:00:00  6.0 |
-           2000-01-01 08:00:00  7.0 |
-           2000-01-01 09:00:00  8.0 |
-           2000-01-01 10:00:00  9.0 |
-           2000-01-01 11:00:00  NaN |
-           2000-01-01 12:00:00  NaN |
-           <BLANKLINE>
-
-
-        Use :py:meth:`~saqc.SaQC.interpolate` to do linear extrapolaiton
-        of up to 1 consecutive missing values:
-
-        .. doctest:: interpolate
-
-           >>> qc = saqc.SaQC(data)
-           >>> qc = qc.interpolate("data", limit=2, method='time', extrapolate='both')
-           >>> qc.data # doctest:+NORMALIZE_WHITESPACE
-                               data |
-           ======================== |
-           2000-01-01 00:00:00  0.0 |
-           2000-01-01 01:00:00  0.0 |
-           2000-01-01 02:00:00  NaN |
-           2000-01-01 03:00:00  NaN |
-           2000-01-01 04:00:00  NaN |
-           2000-01-01 05:00:00  4.0 |
-           2000-01-01 06:00:00  5.0 |
-           2000-01-01 07:00:00  NaN |
-           2000-01-01 08:00:00  NaN |
-           2000-01-01 09:00:00  8.0 |
-           2000-01-01 10:00:00  9.0 |
-           2000-01-01 11:00:00  NaN |
-           2000-01-01 12:00:00  NaN |
-           <BLANKLINE>
-        """
-        if limit is not None:
-            validateWindow(limit, "limit")
-
-        validateValueBounds(order, "order", left=0, strict_int=True)
-        validateChoice(
-            extrapolate, "extrapolate", ["forward", "backward", "both", None]
-        )
+        return self
 
-        if "freq" in kwargs:
-            # the old interpolate version
-            warnings.warn(
-                f"The method `interpolate` is deprecated and will be removed "
-                f"in version 2.7 of saqc. To achieve the same behaviour "
-                f"please use: `qc.align(field={field}, freq={kwargs['freq']}, "
-                f"method={method}, order={order}, flag={flag})`",
-                DeprecationWarning,
-            )
-            return self.align(
-                field=field,
-                freq=kwargs.pop("freq", method),
-                method=method,
-                order=order,
-                flag=flag,
-                **kwargs,
-            )
+    @processing()
+    def dropField(self: "SaQC", field: str, **kwargs) -> "SaQC":
+        """
+        Drops field from the data and flags.
+        """
+        del self._data[field]
+        del self._flags[field]
+        return self
 
-        inter_data = interpolateNANs(
-            self._data[field],
-            method,
-            order=order,
-            gap_limit=limit,
-            extrapolate=extrapolate,
-        )
+    @processing()
+    def renameField(self: "SaQC", field: str, new_name: str, **kwargs) -> "SaQC":
+        """
+        Rename field in data and flags.
 
-        interpolated = self._data[field].isna() & inter_data.notna()
-        self._data[field] = inter_data
-        new_col = pd.Series(np.nan, index=self._flags[field].index)
-        new_col.loc[interpolated] = np.nan if flag is None else flag
-
-        # todo kwargs must have all passed args except data,field,flags
-        self._flags.history[field].append(
-            new_col, {"func": "interpolateInvalid", "args": (), "kwargs": kwargs}
-        )
+        Parameters
+        ----------
+        new_name :
+            String, field is to be replaced with.
+        """
+        self._data[new_name] = self._data[field]
+        self._flags.history[new_name] = self._flags.history[field]
+        del self._data[field]
+        del self._flags[field]
         return self
 
-    @register(mask=["field"], demask=[], squeeze=[])
-    def align(
+    @register(mask=[], demask=[], squeeze=["field"])
+    def selectTime(
         self: "SaQC",
         field: str,
-        freq: str,
-        method: INTERPOLATION_METHODS = "time",
-        order: int = 2,
-        extrapolate: Literal["forward", "backward", "both"] | None = None,
-        overwrite: bool = False,
+        mode: Literal["periodic", "selection_field"],
+        selection_field: str | None = None,
+        start: str | None = None,
+        end: str | None = None,
+        closed: bool = True,
         **kwargs,
     ) -> "SaQC":
         """
-        Convert time series to specified frequency. Values affected by
-        frequency changes will be inteprolated using the given method.
+        Realizes masking within saqc.
+
+        Due to some inner saqc mechanics, it is not straight forwardly possible to exclude
+        values or datachunks from flagging routines. This function replaces flags with UNFLAGGED
+        value, wherever values are to get masked. Furthermore, the masked values get replaced by
+        np.nan, so that they dont effect calculations.
+
+        Here comes a recipe on how to apply a flagging function only on a masked chunk of the variable field:
+
+        1. dublicate "field" in the input data (`copyField`)
+        2. mask the dublicated data (this, `selectTime`)
+        3. apply the tests you only want to be applied onto the masked data chunks (a saqc function)
+        4. project the flags, calculated on the dublicated and masked data onto the original field data (`concateFlags` or `flagGeneric`)
+        5. drop the dublicated data (`dropField`)
+
+        To see an implemented example, checkout flagSeasonalRange in the saqc.functions module
 
         Parameters
         ----------
-        freq :
-            Target frequency.
+        mode :
+            The masking mode.
+            - "periodic": parameters "period_start", "end" are evaluated to generate a periodical mask
+            - "mask_var": data[mask_var] is expected to be a boolean valued timeseries and is used as mask.
+
+        selection_field :
+            Only effective if mode == "mask_var"
+            Fieldname of the column, holding the data that is to be used as mask. (must be boolean series)
+            Neither the series` length nor its labels have to match data[field]`s index and length. An inner join of the
+            indices will be calculated and values get masked where the values of the inner join are ``True``.
+
+        start :
+            Only effective if mode == "seasonal"
+            String denoting starting point of every period. Formally, it has to be a truncated instance of "mm-ddTHH:MM:SS".
+            Has to be of same length as `end` parameter.
+            See examples section below for some examples.
+
+        end :
+            Only effective if mode == "periodic"
+            String denoting starting point of every period. Formally, it has to be a truncated instance of "mm-ddTHH:MM:SS".
+            Has to be of same length as `end` parameter.
+            See examples section below for some examples.
 
-        method :
-            Interpolation technique to use. One of:
+        closed :
+            Wheather or not to include the mask defining bounds to the mask.
 
-            * ``'nshift'``: shift grid points to the nearest time stamp
-                in the range = +/- 0.5 * ``freq``
-            * ``'bshift'``: shift grid points to the first succeeding
-                time stamp (if any)
-            * ``'fshift'``: shift grid points to the last preceeding time
-                stamp (if any)
-            * ``'linear'``: Ignore the index and treat the values as equally
-                spaced.
-            * ``'time'``, ``'index'``, 'values': Use the actual numerical
-                values of the index.
-            * ``'pad'``: Fill in NaNs using existing values.
-            * ``'spline'``, ``'polynomial'``:
-                Passed to ``scipy.interpolate.interp1d``. These methods
-                use the numerical values of the index.  An ``order`` must be
-                specified, e.g. ``qc.interpolate(method='polynomial', order=5)``.
-            * ``'nearest'``, ``'zero'``, ``'slinear'``, ``'quadratic'``, ``'cubic'``, ``'barycentric'``:
-                Passed to ``scipy.interpolate.interp1d``. These methods use
-                the numerical values of the index.
-            * ``'krogh'``, ``'spline'``, ``'pchip'``, ``'akima'``, ``'cubicspline'``:
-                Wrappers around the SciPy interpolation methods of similar
-                names.
-            * ``'from_derivatives'``: Refers to ``scipy.interpolate.BPoly.from_derivatives``
-
-        order :
-            Order of the interpolation method, ignored if not supported
-            by the chosen ``method``
-
-        extrapolate :
-            Use parameter to perform extrapolation instead of interpolation
-            onto the trailing and/or leading chunks of NaN values in data series.
-
-            * ``None`` (default) - perform interpolation
-            * ``'forward'``/``'backward'`` - perform forward/backward extrapolation
-            * ``'both'`` - perform forward and backward extrapolation
+        Examples
+        --------
+        The `period_start` and `end` parameters provide a conveniant way to generate seasonal / date-periodic masks.
+        They have to be strings of the forms:
 
-        overwrite :
-           If set to True, existing flags will be cleared
-        """
+        * "mm-ddTHH:MM:SS"
+        * "ddTHH:MM:SS"
+        * "HH:MM:SS"
+        * "MM:SS" or "SS"
 
-        # TODO:
-        # - should we keep `extrapolate`
+        (mm=month, dd=day, HH=hour, MM=minute, SS=second)
+        Single digit specifications have to be given with leading zeros.
+        `period_start` and `seas   on_end` strings have to be of same length (refer to the same periodicity)
+        The highest date unit gives the period.
+        For example:
 
-        validateWindow(freq, "freq", allow_int=False)
-        validateValueBounds(order, "order", left=0, strict_int=True)
-        validateChoice(
-            extrapolate, "extrapolate", ["forward", "backward", "both", None]
-        )
+        .. doctest::
 
-        if self._data[field].empty:
-            return self
+           >>> start = "01T15:00:00"
+           >>> end = "13T17:30:00"
 
-        if method in ("fshift", "bshift", "nshift"):
-            datacol, history = _shift(
-                saqc=self, field=field, freq=freq, method=method, **kwargs
-            )
+        Will result in all values sampled between 15:00 at the first and  17:30 at the 13th of every month get masked
+
+        .. doctest::
+
+           >>> start = "01:00"
+           >>> end = "04:00"
+
+        All the values between the first and 4th minute of every hour get masked.
+
+        .. doctest::
+
+           >>> start = "01-01T00:00:00"
+           >>> end = "01-03T00:00:00"
+
+        Mask january and february of evcomprosed in theery year. masking is inclusive always, so in this case the mask will
+        include 00:00:00 at the first of march. To exclude this one, pass:
+
+        .. doctest::
+
+           >>> start = "01-01T00:00:00"
+           >>> end = "02-28T23:59:59"
+
+        To mask intervals that lap over a seasons frame, like nights, or winter, exchange sequence of season start and
+        season end. For example, to mask night hours between 22:00:00 in the evening and 06:00:00 in the morning, pass:
+
+        >> start = "22:00:00"
+        >> end = "06:00:00"
+
+        """
+        validateChoice(mode, "mode", ["periodic", "selection_field"])
+
+        datcol_idx = self._data[field].index
+
+        if mode == "periodic":
+            mask = periodicMask(datcol_idx, start, end, closed)
+        elif mode == "selection_field":
+            idx = self._data[selection_field].index.intersection(datcol_idx)
+            mask = self._data[selection_field].loc[idx]
         else:
-            datacol, history = _interpolate(
-                saqc=self,
-                field=field,
-                freq=freq,
-                method=method,
-                order=order,
-                extrapolate=extrapolate,
-                dfilter=kwargs["dfilter"],
+            raise ValueError(
+                "Keyword passed as masking mode is unknown ({})!".format(mode)
             )
 
-        meta = {
-            "func": "align",
-            "args": (field,),
-            "kwargs": {
-                "freq": freq,
-                "method": method,
-                "order": order,
-                "extrapolate": extrapolate,
-                **kwargs,
-            },
-        }
-        flagcol = pd.Series(UNFLAGGED if overwrite else np.nan, index=history.index)
-        history.append(flagcol, meta)
-        self._data[field] = datacol
-        self._flags.history[field] = history
+        mask = mask.reindex(self._data[field].index, fill_value=False).astype(bool)
+        self._data[field].loc[mask] = np.nan
+        self._flags[mask, field] = UNFLAGGED
         return self
 
-    # ============================================================
-    ### Deprecated functions
-    # ============================================================
-
-    @register(mask=["field"], demask=[], squeeze=[])
-    def interpolateIndex(
+    @register(
+        mask=[],
+        demask=[],
+        squeeze=[],
+        multivariate=True,
+    )
+    def plot(
         self: "SaQC",
-        field: str,
-        freq: str,
-        method: INTERPOLATION_METHODS,
-        order: int = 2,
-        limit: int | None = 2,
-        extrapolate: Literal["forward", "backward", "both"] = None,
+        field: str | list[str],
+        path: str | None = None,
+        max_gap: str | None = None,
+        mode: Literal["subplots", "oneplot"] | str = "oneplot",
+        history: Literal["valid", "complete"] | list[str] | None = "valid",
+        xscope: slice | str | None = None,
+        yscope: tuple | list[tuple] | dict | None = None,
+        store_kwargs: dict | None = None,
+        ax: mpl.axes.Axes | None = None,
+        ax_kwargs: dict | None = None,
+        marker_kwargs: dict | None = None,
+        plot_kwargs: dict | None = None,
+        dfilter: float = FILTER_NONE,
         **kwargs,
     ) -> "SaQC":
         """
-        Function to interpolate the data at regular (equidistant)
-        timestamps also known as or grid points.
+        Plot data and flags or store plot to file.
 
-            .. deprecated:: 2.4.0
-               Use :py:meth:`~saqc.SaQC.align` instead.
+        There are two modes, 'interactive' and 'store', which are determined through the
+        ``save_path`` keyword. In interactive mode (default) the plot is shown at runtime
+        and the program execution stops until the plot window is closed manually. In
+        store mode the generated plot is stored to disk and no manually interaction is
+        needed.
 
         Parameters
         ----------
-        freq :
-            An Offset String, interpreted as the frequency of
-            the grid you want to interpolate your data to.
-
-        method :
-            The interpolation method you want to apply.
-
-        order :
-            If your selected interpolation method can be performed at
-            different 'orders' - here you pass the desired order.
-
-        limit :
-            Upper limit of missing index values (with respect to ``freq``)
-            to fill. The limit can either be expressed as the number of
-            consecutive missing values (integer) or temporal extension
-            of the gaps to be filled (Offset String). If ``None`` is passed,
-            no limit is set.
-
-        extrapolate :
-            Use parameter to perform extrapolation instead of interpolation
-            onto the trailing and/or leading chunks of NaN values in data
-            series.
-
-            * ``None`` (default) - perform interpolation
-            * ``'forward'``/``'backward'`` - perform forward/backward extrapolation
-            * ``'both'`` - perform forward and backward extrapolation
-        """
-        call = (
-            f'qc.align(field="{field}", freq="{freq}", method="{method}", '
-            f'order={order}, extrapolate="{extrapolate}")'
-        )
-        if limit != 2:
-            call = (
-                f'qc.interpolate(field="{field}", method="{method}", '
-                f'order="{order}", limit="{limit}", extrapolate="{extrapolate}")'
-            )
-        warnings.warn(
-            f"The method interpolateIndex is deprectated and will be removed with SaQC==3.0. Use `{call}` instead",
-            DeprecationWarning,
-        )
+        path :
+            If ``None`` is passed, interactive mode is entered; plots are shown immediatly
+            and a user need to close them manually before execution continues.
+            If a filepath is passed instead, store-mode is entered and
+            the plot is stored unter the passed location.
+
+        max_gap :
+            If ``None``, all data points will be connected, resulting in long linear
+            lines, in case of large data gaps. ``NaN`` values will be removed before
+            plotting. If an offset string is passed, only points that have a distance
+            below ``max_gap`` are connected via the plotting line.
+
+        mode :
+           How to process multiple variables to be plotted:
+
+           * `"oneplot"` : plot all variables with their flags in one axis (default)
+           * `"subplots"` : generate subplot grid where each axis contains one variable plot with associated flags
+           * `"biplot"` : plotting first and second variable in field against each other in a scatter plot  (point cloud).
+
+        history :
+            Discriminate the plotted flags with respect to the tests they originate from.
+
+            * ``"valid"``: Only plot flags, that are not overwritten by subsequent tests.
+              Only list tests in the legend, that actually contributed flags to the overall
+              result.
+            * ``None``: Just plot the resulting flags for one variable, without any historical
+              and/or meta information.
+            * list of strings: List of tests. Plot flags from the given tests, only.
+            * ``complete`` (not recommended, deprecated): Plot all the flags set by any test, independently from them being removed or modified by
+              subsequent modifications. (this means: plotted flags do not necessarily match with flags ultimately
+              assigned to the data)
+
+        xscope :
+            Determine a chunk of the data to be plotted. ``xscope`` can be anything,
+            that is a valid argument to the ``pandas.Series.__getitem__`` method.
+
+        yscope :
+             Either a tuple of 2 scalars that determines all plots' y-view limits, or a list of those
+             tuples, determining the different variables y-view limits (must match number of variables)
+             or a dictionary with variables as keys and the y-view tuple as values.
+
+        ax :
+            If not ``None``, plot into the given ``matplotlib.Axes`` instance, instead of a
+            newly created ``matplotlib.Figure``. This option offers a possibility to integrate
+            ``SaQC`` plots into custom figure layouts.
+
+        store_kwargs :
+            Keywords to be passed on to the ``matplotlib.pyplot.savefig`` method, handling
+            the figure storing. To store an pickle object of the figure, use the option
+            ``{"pickle": True}``, but note that all other ``store_kwargs`` are ignored then.
+            To reopen a pickled figure execute: ``pickle.load(open(savepath, "w")).show()``
+
+        ax_kwargs :
+            Axis keywords. Change axis specifics. Those are passed on to the
+            `matplotlib.axes.Axes.set <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html>`_
+            method and can have the options listed there.
+            The following options are `saqc` specific:
+
+            * ``"xlabel"``: Either single string, that is to be attached to all x-axis´, or
+              a List of labels, matching the number of variables to plot in length, or a dictionary, directly
+              assigning labels to certain fields - defaults to ``None`` (no labels)
+            * ``"ylabel"``: Either single string, that is to be attached to all y-axis´, or
+              a List of labels, matching the number of variables to plot in length, or a dictionary, directly
+              assigning labels to certain fields - defaults to ``None`` (no labels)
+            * ``"title"``: Either a List of labels, matching the number of variables to plot in length, or a dictionary, directly
+              assigning labels to certain variables - defaults to ``None`` (every plot gets titled the plotted variables name)
+            * ``"fontsize"``: (float) Adjust labeling and titeling fontsize
+            * ``"nrows"``, ``"ncols"``: shape of the subplot matrix the plots go into: If both are assigned, a subplot
+              matrix of shape `nrows` x `ncols` is generated. If only one is assigned, the unassigned dimension is 1.
+              defaults to plotting into subplot matrix with 2 columns and the necessary number of rows to fit the
+              number of variables to plot.
+
+        marker_kwargs :
+            Keywords to modify flags marker appearance. The markers are set via the
+            `matplotlib.pyplot.scatter <https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html>`_
+            method and can have the options listed there.
+            The following options are `saqc` specific:
+
+            * ``"cycleskip"``: (int) start the cycle of shapes that are assigned any flag-type with a certain lag - defaults to ``0`` (no skip)
+
+        plot_kwargs :
+            Keywords to modify the plot appearance. The plotting is delegated to
+            `matplotlib.pyplot.plot <https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html>`_, all options listed there are available. Additionally the following saqc specific configurations are possible:
+
+            * ``"alpha"``: Either a scalar float in *[0,1]*, that determines all plots' transparencies, or
+              a list of floats, matching the number of variables to plot.
+
+            * ``"linewidth"``: Either single float in *[0,1]*, that determines the thickness of all plotted,
+              or a list of floats, matching the number of variables to plot.
 
-        # HINT: checking is delegated to called functions
 
-        out = self.align(
-            field=field,
-            freq=freq,
-            method=method,
-            order=order,
-            extrapolate=extrapolate,
-            **kwargs,
-        )
-        if limit != 2:
-            out = out.interpolate(
-                field=field,
-                freq=freq,
-                method=method,
-                order=order,
-                limit=limit,
-                extrapolate=extrapolate,
-                **kwargs,
-            )
-        return out
 
-    @register(
-        mask=["field"],
-        demask=["field"],
-        squeeze=[],  # func handles history by itself
-    )
-    def interpolateInvalid(
-        self: "SaQC",
-        field: str,
-        method: INTERPOLATION_METHODS,
-        order: int = 2,
-        limit: int | None = None,
-        extrapolate: Literal["forward", "backward", "both"] | None = None,
-        flag: float = UNFLAGGED,
-        **kwargs,
-    ) -> "SaQC":
-        """
-        .. deprecated:: 2.4.0
-           Use :py:meth:`~saqc.SaQC.interpolate` instead.
+        Notes
+        -----
+
+        * Check/modify the module parameter `saqc.lib.plotting.SCATTER_KWARGS` to see/modify global marker defaults
+        * Check/modify the module parameter `saqc.lib.plotting.PLOT_KWARGS` to see/modify global plot line defaults
         """
-        warnings.warn(
-            "The method `intepolateInvalid` is deprecated and will be removed "
-            "with version 2.7 of saqc. To achieve the same behavior, please "
-            f"use `qc.interpolate(field={field}, method={method}, order={order}, "
-            f"limit={limit}, extrapolate={extrapolate}, flag={flag})`",
-            DeprecationWarning,
-        )
+        data, flags = self._data.copy(), self._flags.copy()
 
-        # HINT: checking is delegated to called function
-        return self.interpolate(
-            field=field,
-            method=method,
-            order=order,
-            limit=limit,
-            extrapolate=extrapolate,
-            flag=flag,
-            **kwargs,
-        )
+        level = kwargs.get("flag", UNFLAGGED)
 
+        if dfilter < np.inf:
+            for f in field:
+                data[f].loc[flags[f] >= dfilter] = np.nan
+
+        store_kwargs = store_kwargs or {}
+        ax_kwargs = ax_kwargs or {}
+        marker_kwargs = marker_kwargs or {}
+        plot_kwargs = plot_kwargs or {}
+
+        if (
+            (yscope is not None)
+            and (len(yscope) == 2)
+            and not isinstance(yscope[0], (list, tuple))
+        ):
+            yscope = tuple(yscope)
+        if yscope is not None:
 
-def _shift(
-    saqc: "SaQC",
-    field: str,
-    freq: str,
-    method: Literal["fshift", "bshift", "nshift"] = "nshift",
-    **kwargs,
-) -> Tuple[pd.Series, History]:
-    """
-    Shift data points and flags to a regular frequency grid.
-
-    Parameters
-    ----------
-    field :
-        The fieldname of the column, holding the data-to-be-shifted.
-
-    freq :
-        Offset string. Sampling rate of the target frequency.
-
-    method :
-        Method to propagate values:
-
-        * 'nshift' : shift grid points to the nearest time stamp in the range = +/- 0.5 * ``freq``
-        * 'bshift' : shift grid points to the first succeeding time stamp (if any)
-        * 'fshift' : shift grid points to the last preceding time stamp (if any)
-
-    Returns
-    -------
-    saqc.SaQC
-    """
-    validateChoice(method, "method", ["fshift", "bshift", "nshift"])
-    validateWindow(freq, "freq", allow_int=False)
-
-    datcol = saqc._data[field]
-    if datcol.empty:
-        return saqc
-
-    # do the shift
-    datcol = shift2Freq(datcol, method, freq, fill_value=np.nan)
-
-    # do the shift on the history
-    kws = dict(method=method, freq=freq)
-
-    history = saqc._flags.history[field].apply(
-        index=datcol.index,
-        func_handle_df=True,
-        func=shift2Freq,
-        func_kws={**kws, "fill_value": np.nan},
-    )
+            ax_kwargs.update({"ylim": yscope})
 
-    return datcol, history
+        if not path:
+            mpl.use(_MPL_DEFAULT_BACKEND)
+        else:
+            plt.close("all")  # supress matplotlib deprecation warning
+            mpl.use("Agg")
 
+        fig = makeFig(
+            data=data,
+            field=field,
+            flags=flags,
+            level=level,
+            mode=mode,
+            max_gap=max_gap,
+            history=history,
+            xscope=xscope,
+            ax=ax,
+            ax_kwargs=ax_kwargs,
+            scatter_kwargs=marker_kwargs,
+            plot_kwargs=plot_kwargs,
+        )
 
-def _interpolate(
-    saqc: "SaQC",
-    field: str,
-    freq: str,
-    method: str,
-    order: int | None,
-    dfilter: float,
-    extrapolate: Literal["forward", "backward", "both", None] = None,
-) -> Tuple[pd.Series, History]:
-    """TODO: Docstring"""
-
-    validateChoice(extrapolate, "extrapolate", ["forward", "backward", "both", None])
-    validateWindow(freq, "freq", allow_int=False)
-    if order is not None:
-        validateValueBounds(order, "order", 0, strict_int=True)
-
-    datcol = saqc._data[field].copy()
-
-    start, end = datcol.index[0].floor(freq), datcol.index[-1].ceil(freq)
-    grid_index = pd.date_range(start=start, end=end, freq=freq, name=datcol.index.name)
-
-    flagged = isflagged(saqc._flags[field], dfilter)
-
-    # drop all points that hold no relevant grid information
-    datcol = datcol[~flagged].dropna()
-
-    # account for annoying case of subsequent frequency aligned values,
-    # that differ exactly by the margin of 2*freq
-    gaps = datcol.index[1:] - datcol.index[:-1] == 2 * pd.Timedelta(freq)
-    gaps = datcol.index[1:][gaps]
-    gaps = gaps.intersection(grid_index).shift(-1, freq)
-
-    # prepare grid interpolation:
-    datcol = datcol.reindex(datcol.index.union(grid_index))
-
-    # do the grid interpolation
-    inter_data = interpolateNANs(
-        data=datcol,
-        method=method,
-        order=order,
-        gap_limit=2,
-        extrapolate=extrapolate,
-    )
-    # override falsely interpolatet values:
-    inter_data[gaps] = np.nan
-    inter_data = inter_data[grid_index]
-
-    history = saqc._flags.history[field].apply(
-        index=inter_data.index,
-        func=_resampleOverlapping,
-        func_kws=dict(freq=freq, fill_value=np.nan),
-    )
-    return inter_data, history
+        if ax is None and not path:
+            plt.show()
+
+        if path:
+            if store_kwargs.pop("pickle", False):
+                with open(path, "wb") as f:
+                    pickle.dump(fig, f)
+            else:
+                fig.savefig(path, **store_kwargs)
+
+        return self
```

### Comparing `saqc-2.5.0/saqc/funcs/noise.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/noise.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 import pandas as pd
 from scipy.stats import median_abs_deviation
 
 from saqc.constants import BAD
 from saqc.core.register import flagging
 from saqc.lib.checking import (
     isCallable,
-    validateChoice,
+    validateFuncSelection,
     validateMinPeriods,
     validateWindow,
 )
 from saqc.lib.tools import isunflagged, statPass
-
-STATS_DICT = {"std": np.std, "var": np.var, "mad": median_abs_deviation}
+from saqc.parsing.environ import ENV_OPERATORS
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
 class NoiseMixin:
     def flagByStatLowPass(
         self: "SaQC",
         field: str,
         window: str | pd.Timedelta,
         thresh: float,
-        func: Literal["std", "var", "mad"]
-        | Callable[[np.ndarray, pd.Series], float] = "std",
+        func: (
+            Literal["std", "var", "mad"] | Callable[[np.ndarray, pd.Series], float]
+        ) = "std",
         sub_window: str | pd.Timedelta | None = None,
         sub_thresh: float | None = None,
         min_periods: int | None = None,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
@@ -50,21 +50,26 @@
 
         Flag data chunks of length ``window`` if
 
         1. they excexceed ``thresh`` with regard to ``func`` and
         2. all (maybe overlapping) sub-chunks of the data chunks with length ``sub_window``,
            exceed ``sub_thresh`` with regard to ``func``
 
+            .. deprecated:: 2.5.0
+               Deprecated Function. See :py:meth:`~saqc.SaQC.flagByScatterLowpass`.
+
         Parameters
         ----------
         func :
             Either a String value, determining the aggregation function applied on every chunk.
+
             * 'std': standard deviation
             * 'var': variance
             * 'mad': median absolute deviation
+
             Or a Callable function mapping 1 dimensional arraylikes onto scalars.
 
         window :
             Window (i.e. chunk) size.
 
         thresh :
             Threshold. A given chunk is flagged, if the return value of ``func`` excceeds ``thresh``.
@@ -99,16 +104,17 @@
 
     @flagging()
     def flagByScatterLowpass(
         self: "SaQC",
         field: str,
         window: str | pd.Timedelta,
         thresh: float,
-        func: Literal["std", "var", "mad"]
-        | Callable[[np.ndarray, pd.Series], float] = "std",
+        func: (
+            Literal["std", "var", "mad"] | Callable[[np.ndarray, pd.Series], float]
+        ) = "std",
         sub_window: str | pd.Timedelta | None = None,
         sub_thresh: float | None = None,
         min_periods: int | None = None,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
@@ -119,18 +125,20 @@
         1. they excexceed ``thresh`` with regard to ``func`` and
         2. all (maybe overlapping) sub-chunks of the data chunks with length ``sub_window``,
            exceed ``sub_thresh`` with regard to ``func``
 
         Parameters
         ----------
         func :
-            Either a string, determining the aggregation function applied on every chunk
+            Either a string, determining the aggregation function applied on every chunk:
+
             * 'std': standard deviation
             * 'var': variance
             * 'mad': median absolute deviation
+
             Or a Callable, mapping 1 dimensional array likes onto scalars.
 
         window :
             Window (i.e. chunk) size.
 
         thresh :
             Threshold. A given chunk is flagged, if the return value of ``func`` excceeds ``thresh``.
@@ -142,27 +150,23 @@
         sub_thresh :
             Threshold. A given sub chunk is flagged, if the return value of ``func` excceeds ``sub_thresh``.
 
         min_periods :
             Minimum number of values needed in a chunk to perfom the test.
             Ignored if ``window`` is an integer.
         """
-        if (not isCallable(func)) and (func not in ["std", "var", "mad"]):
-            raise TypeError(
-                f"Parameter 'func' must either be of type 'Callable' or one out of ['std', 'var', 'mad']. Got {func}."
-            )
-
+        validateFuncSelection(func, allow_operator_str=True)
         validateWindow(window, allow_int=False)
         validateMinPeriods(min_periods)
         if sub_window is not None:
             validateWindow(sub_window, "sub_window", allow_int=False)
             sub_window = pd.Timedelta(sub_window)
 
-        if not isCallable(func):
-            func = STATS_DICT[func]
+        if isinstance(func, str):
+            func = ENV_OPERATORS[func]
 
         to_set = statPass(
             datcol=self._data[field],
             stat=func,
             winsz=pd.Timedelta(window),
             thresh=thresh,
             comparator=operator.gt,
```

### Comparing `saqc-2.5.0/saqc/funcs/outliers.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/outliers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from typing_extensions import Literal
 
 from saqc import BAD, UNFLAGGED
 from saqc.core import DictOfSeries, Flags, flagging, register
 from saqc.lib.checking import (
     isCallable,
     isFloatLike,
-    validateCallable,
     validateChoice,
     validateFraction,
     validateFrequency,
+    validateFuncSelection,
     validateMinPeriods,
     validateValueBounds,
     validateWindow,
 )
 from saqc.lib.docs import DOC_TEMPLATES
 from saqc.lib.rolling import windowRoller
 from saqc.lib.tools import getFreqDelta, isflagged, toSequence
@@ -64,15 +64,14 @@
     def flagLOF(
         self: "SaQC",
         field: Sequence[str],
         n: int = 20,
         thresh: Literal["auto"] | float = 1.5,
         algorithm: Literal["ball_tree", "kd_tree", "brute", "auto"] = "ball_tree",
         p: int = 1,
-        density: Literal["auto"] | float | Callable = "auto",
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
         Flag values where the Local Outlier Factor (LOF) exceeds cutoff.
 
         Parameters
@@ -95,17 +94,15 @@
             The threshold for flagging the calculated LOF. A LOF of around
             ``1`` is considered normal and most likely corresponds to
             inlier points.
 
             * The "automatic" threshing introduced with the publication
               of the algorithm defaults to ``1.5``.
             * In this implementation, :py:attr:`thresh` defaults (``'auto'``)
-              to flagging the scores with a modified 3-sigma rule, resulting
-              in a :py:attr:`thresh` `` > 1.5`` which usually mitigates
-              over-flagging compared to the literature recommendation.
+              to flagging the scores with a modified 3-sigma rule.
 
         algorithm :
             Algorithm used for calculating the :py:attr:`n`-nearest neighbors.
 
         p :
             Degree of the metric ("Minkowski"), according to which the
             distance to neighbors is determined. Most important values are:
@@ -140,27 +137,26 @@
           of the points distances to its :py:attr:`n`-nearest neighbors,
           measured with regard to the minkowski metric of degree :py:attr:`p`
           (usually euclidean).
         * To derive a binary label for every point (outlier: *yes*, or *no*),
           the scores are cut off at a level, determined by :py:attr:`thresh`.
 
         """
-        self._validateLOF(algorithm, n, p, density)
+        self._validateLOF(algorithm, n, p, 1.0)
         if thresh != "auto" and not isFloatLike(thresh):
             raise ValueError(f"'thresh' must be 'auto' or a float, not {thresh}")
 
         fields = toSequence(field)
         field_ = str(uuid.uuid4())
         qc = self.assignLOF(
             field=fields,
             target=field_,
             n=n,
             algorithm=algorithm,
             p=p,
-            density=density,
         )
         s = qc.data[field_]
         if thresh == "auto":
             s = pd.concat([s, (-s - 2)])
             s_mask = (s - s.mean() / s.std())[: len(s) // 2].abs() > 3
         else:
             s_mask = s < abs(thresh)
@@ -177,14 +173,16 @@
         field: str,
         n: int = 20,
         thresh: Literal["auto"] | float = 1.5,
         algorithm: Literal["ball_tree", "kd_tree", "brute", "auto"] = "ball_tree",
         p: int = 1,
         density: Literal["auto"] | float = "auto",
         fill_na: bool = True,
+        slope_correct: bool = True,
+        min_offset: float = None,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
         Flag "univariate" Local Outlier Factor (LOF) exceeding cutoff.
 
         The function is a wrapper around a usual LOF implementation, aiming
@@ -230,14 +228,15 @@
         algorithm :
             Algorithm used for calculating the :py:attr:`n`-nearest neighbors
             needed for LOF calculation.
 
         p :
             Degree of the metric ("Minkowski"), according to which distance
             to neighbors is determined. Most important values are:
+
             * ``1`` - Manhatten Metric
             * ``2`` - Euclidian Metric
 
         density :
             How to calculate the temporal distance/density for the variable
             to flag.
 
@@ -245,18 +244,22 @@
               equal to the median of the absolute diff of the variable to flag.
             * ``float`` - introduces linear density with an increment
               equal to :py:attr:`density`
 
         fill_na :
             If True, NaNs in the data are filled with a linear interpolation.
 
-        See Also
-        --------
-        :ref:`introduction to outlier detection with
-            saqc <cookbooks/OutlierDetection:Outlier Detection>`
+        slope_correct :
+            if True, a correction is applied, that removes outlier cluster that actually
+            just seem to be steep slopes
+
+        min_offset :
+            If set, only those outlier cluster will be flagged, that are preceeded and succeeeded
+            by sufficiently large value "jumps". Defaults to estimating the sufficient value jumps from
+            the median over the absolute step sizes between data points.
 
         Notes
         -----
 
         * The :py:meth:`~saqc.SaQC.flagUniLOF` function calculates an
           univariate Local Outlier Factor (UniLOF) - score for every
           point in the one dimensional input data series. The *UniLOF*
@@ -343,14 +346,17 @@
            :context: close-figs
            :include-source: False
            :class: center
 
            qc = qc.flagUniLOF('sac254_raw')
            qc.plot('sac254_raw')
 
+        See also
+        --------
+        :ref:`introduction to outlier detection with saqc <cookbooks/OutlierDetection:Outlier Detection>`
         """
         self._validateLOF(algorithm, n, p, density)
         if thresh != "auto" and not isFloatLike(thresh):
             raise ValueError(f"'thresh' must be 'auto' or a float, not {thresh}")
 
         tmp_field = str(uuid.uuid4())
         qc = self.assignUniLOF(
@@ -364,16 +370,55 @@
         )
         s = qc.data[tmp_field]
         if thresh == "auto":
             _s = pd.concat([s, (-s - 2)])
             s_mask = ((_s - _s.mean()) / _s.std()).iloc[: int(s.shape[0])].abs() > 3
         else:
             s_mask = s < -abs(thresh)
-
         s_mask = ~isflagged(qc._flags[field], kwargs["dfilter"]) & s_mask
+
+        if slope_correct:
+            g_mask = s_mask.diff()
+            g_mask = g_mask.cumsum()
+            dat = self._data[field]
+            od_groups = dat.interpolate("linear").groupby(by=g_mask)
+            first_vals = od_groups.first()
+            last_vals = od_groups.last()
+            max_vals = od_groups.max()
+            min_vals = od_groups.min()
+            if min_offset is None:
+                if density == "auto":
+                    d_diff = dat.diff()
+                    eps = d_diff.abs().median()
+                    if eps == 0:
+                        eps = d_diff[d_diff != 0].abs().median()
+                else:
+                    eps = density
+                eps = 3 * eps
+            else:
+                eps = min_offset
+            up_slopes = (min_vals + eps >= last_vals.shift(1)) & (
+                max_vals - eps <= first_vals.shift(-1)
+            )
+            down_slopes = (max_vals - eps <= last_vals.shift(1)) & (
+                min_vals + eps >= first_vals.shift(-1)
+            )
+            slopes = up_slopes | down_slopes
+            odd_return_pred = (max_vals > last_vals.shift(1)) & (
+                min_vals < last_vals.shift(1)
+            )
+            odd_return_succ = (max_vals > first_vals.shift(-1)) & (
+                min_vals < first_vals.shift(-1)
+            )
+            returns = odd_return_succ | odd_return_pred
+            corrections = returns | slopes
+            for s_id in corrections[corrections].index:
+                correct_idx = od_groups.get_group(s_id).index
+                s_mask[correct_idx] = False
+
         qc._flags[s_mask, field] = flag
         qc = qc.dropField(tmp_field)
         return qc
 
     @flagging()
     def flagRange(
         self: "SaQC",
@@ -511,15 +556,15 @@
     )
     def flagMVScores(
         self: "SaQC",
         field: Sequence[str],
         trafo: Callable[[pd.Series], pd.Series] = lambda x: x,
         alpha: float = 0.05,
         n: int = 10,
-        func: Callable[[pd.Series], float] = np.sum,
+        func: Callable[[pd.Series], float] | str = "sum",
         iter_start: float = 0.5,
         window: int | str | None = None,
         min_periods: int = 11,
         stray_range: str | None = None,
         drop_flagged: bool = False,  # TODO: still a case ?
         thresh: float = 3.5,
         min_periods_r: int = 1,
@@ -530,14 +575,17 @@
         The algorithm implements a 3-step outlier detection procedure for
         simultaneously flagging of higher dimensional data (dimensions > 3).
 
         In [1], the procedure is introduced and exemplified with an application on
         hydrological data. See the notes section for an overview over the algorithms
         basic steps.
 
+            .. deprecated:: 2.6.0
+               Deprecated Function. Please refer to :py:meth:`~saqc.SaQC.flagByStray`.
+
         Parameters
         ----------
         trafo :
             Transformation to be applied onto every column before scoring. For more
             fine-grained control, the data could also be transformed before
             :py:meth:`~saqc.SaQC.flagMVScores` is called.
 
@@ -674,14 +722,25 @@
                 To alter the size of the reduction window, use the parameter
                 `min_periods_r`. Changes readily apply.
                 This warning will be removed in saqc version 2.7.
                 """,
                 DeprecationWarning,
             )
 
+        warnings.warn(
+            """
+                flagMVScores is deprecated and will be removed with Version 2.8.
+                To replicate the function, transform the different fields involved
+                via explicit applications of some transformations, than calculate the
+                kNN scores via `saqc.SaQC.assignkNScores` and finally assign the STRAY
+                algorithm via `saqc.SaQC.flagByStray`.
+                """,
+            DeprecationWarning,
+        )
+
         # Hint: checking is delegated to the called functions
 
         fields = toSequence(field)
 
         qc = self
         fields_ = []
         for f in fields:
@@ -739,44 +798,18 @@
         raise_factor: float = 2.0,
         slope: float | None = None,
         weight: float = 0.8,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
-        The function flags raises and drops in value courses, that exceed a certain
-        threshold within a certain timespan.
-
-        The parameter variety of the function is owned to the intriguing case of
-        values, that "return" from outlierish or anomalious value levels and thus
-        exceed the threshold, while actually being usual values.
-
-        Notes
-        -----
-        The dataset is NOT supposed to be harmonized to a time series with an
-        equidistant requency grid.
-
-        The value :math:`x_{k}` of a time series :math:`x` with associated
-        timestamps :math:`t_i`, is flagged a raise, if:
-
-        1. There is any value :math:`x_{s}`, preceeding :math:`x_{k}` within
-           :py:attr:`raise_window` range, so that
-           :math:`M = |x_k - x_s | >`  :py:attr:`thresh` :math:`> 0`
+        The function flags raises and drops in value courses, that exceed a certain threshold within a certain timespan.
 
-        2. The weighted average :math:`\\mu^{*}` of the values, preceding
-           :math:`x_{k}` within :py:attr:`average_window` range indicates,
-           that :math:`x_{k}` does not return from an "outlierish" value
-           course, meaning that
-           :math:`x_k > \\mu^* + ( M` / :py:attr:`raise_factor` :math:`)`
-
-        3. Additionally, if :py:attr:`slope` is not ``None``, :math:`x_{k}`
-           is checked or being sufficiently divergent from its very predecessor
-           :math:`x_{k-1}`, meaning that, it is additionally checked if:
-           * :math:`x_k - x_{k-1} >` :py:attr:`slope`
-           * :math:`t_k - t_{k-1} >` :py:attr:`weight` :math:`\\times` :py:attr:`freq`
+        .. deprecated:: 2.6.0
+           Function is deprecated since its not humanly parameterisable. Also more suitable alternatives are available. Depending on use case, use: :py:meth:`~saqc.SaQC.flagUniLOF`, :py:meth:`~saqc.SaQC.flagZScore`, :py:meth:`~saqc.SaQC.flagJumps` instead.
 
         Parameters
         ----------
         thresh :
             The threshold, for the total rise (:py:attr:`thresh` ``> 0``),
             or total drop (:py:attr:`thresh` ``< 0``), value courses must
             not exceed within a timespan of length :py:attr:`raise_window`.
@@ -799,15 +832,49 @@
             See condition (2).
 
         slope :
             See condition (3).
 
         weight :
             See condition (3).
+
+        Notes
+        -----
+        The dataset is NOT supposed to be harmonized to a time series with an
+        equidistant requency grid.
+
+        The value :math:`x_{k}` of a time series :math:`x` with associated
+        timestamps :math:`t_i`, is flagged a raise, if:
+
+        1. There is any value :math:`x_{s}`, preceeding :math:`x_{k}` within
+           :py:attr:`raise_window` range, so that
+           :math:`M = |x_k - x_s | >`  :py:attr:`thresh` :math:`> 0`
+
+        2. The weighted average :math:`\\mu^{*}` of the values, preceding
+           :math:`x_{k}` within :py:attr:`average_window` range indicates,
+           that :math:`x_{k}` does not return from an "outlierish" value
+           course, meaning that
+           :math:`x_k > \\mu^* + ( M` / :py:attr:`raise_factor` :math:`)`
+
+        3. Additionally, if :py:attr:`slope` is not ``None``, :math:`x_{k}`
+           is checked or being sufficiently divergent from its very predecessor
+           :math:`x_{k-1}`, meaning that, it is additionally checked if:
+           * :math:`x_k - x_{k-1} >` :py:attr:`slope`
+           * :math:`t_k - t_{k-1} >` :py:attr:`weight` :math:`\\times` :py:attr:`freq`
         """
+
+        warnings.warn(
+            "The function flagRaise is deprecated with no 100% exact replacement function."
+            "When looking for changes in the value course, the use of flagRaise can be replicated and more "
+            "easily aimed for, via the method flagJump.\n"
+            "When looking for raises to outliers or plateaus, use one of: "
+            "flagZScore (outliers), flagUniLOF (outliers and small plateaus) or flagOffset (plateaus)",
+            DeprecationWarning,
+        )
+
         validateWindow(raise_window, "raise_window", allow_int=False)
         validateWindow(freq, "freq", allow_int=False)
         validateWindow(average_window, "average_window", allow_int=False, optional=True)
 
         # prepare input args
         dataseries = self._data[field].dropna()
         raise_window_td = pd.Timedelta(raise_window)
@@ -903,14 +970,18 @@
         **kwargs,
     ) -> "SaQC":
         """
         Flag outiers using the modified Z-score outlier detection method.
 
         See references [1] for more details on the algorithm.
 
+            .. deprecated:: 2.6.0
+               Deprecated Function. Please refer to :py:meth:`~saqc.SaQC.flagZScore`.
+
+
         Note
         ----
         Data needs to be sampled at a regular equidistant time grid.
 
         Parameters
         ----------
         window :
@@ -970,14 +1041,15 @@
 
         Notes
         -----
         This definition of a "spike" not only includes one-value outliers, but also plateau-ish value courses.
 
         Values :math:`x_n, x_{n+1}, .... , x_{n+k}` of a timeseries :math:`x` with
         associated timestamps :math:`t_n, t_{n+1}, .... , t_{n+k}` are considered spikes, if:
+
         1. :math:`|x_{n-1} - x_{n + s}| >` :py:attr:`thresh`, for all :math:`s \\in [0,1,2,...,k]`
         2. if :py:attr:`thresh_relative` > 0, :math:`x_{n + s} > x_{n - 1}*(1+` :py:attr:`thresh_relative` :math:`)`
         3. if :py:attr:`thresh_relative` < 0, :math:`x_{n + s} < x_{n - 1}*(1+` :py:attr:`thresh_relative` :math:`)`
         4. :math:`|x_{n-1} - x_{n+k+1}| <` :py:attr:`tolerance`
         5. :math:`|t_{n-1} - t_{n+k+1}| <` :py:attr:`window`
 
 
@@ -1013,24 +1085,24 @@
         .. plot::
            :context:
            :include-source: False
 
            import matplotlib
            import saqc
            import pandas as pd
-           data = pd.DataFrame({'data':np.array([5,5,8,16,17,7,4,4,4,1,1,4])}, index=pd.date_range('2000',freq='1H', periods=12))
+           data = pd.DataFrame({'data':np.array([5,5,8,16,17,7,4,4,4,1,1,4])}, index=pd.date_range('2000',freq='1h', periods=12))
 
 
         Lets generate a simple, regularly sampled timeseries with an hourly sampling rate and generate an
         :py:class:`saqc.SaQC` instance from it.
 
         .. doctest:: flagOffsetExample
 
            >>> import saqc
-           >>> data = pd.DataFrame({'data':np.array([5,5,8,16,17,7,4,4,4,1,1,4])}, index=pd.date_range('2000',freq='1H', periods=12))
+           >>> data = pd.DataFrame({'data':np.array([5,5,8,16,17,7,4,4,4,1,1,4])}, index=pd.date_range('2000',freq='1h', periods=12))
            >>> data
                                 data
            2000-01-01 00:00:00     5
            2000-01-01 01:00:00     5
            2000-01-01 02:00:00     8
            2000-01-01 03:00:00    16
            2000-01-01 04:00:00    17
@@ -1046,59 +1118,59 @@
         Now we are applying :py:meth:`~saqc.SaQC.flagOffset` and try to flag offset courses, that dont extend
         longer than *6 hours* in time (:py:attr:`window`) and that have an initial value jump higher than ``2``
         (:py:attr:`thresh`), and that do return to the initial value level within a tolerance of ``1.5``
         (:py:attr:`tolerance`).
 
         .. doctest:: flagOffsetExample
 
-           >>> qc = qc.flagOffset("data", thresh=2, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, tolerance=1.5, window='6h')
            >>> qc.plot('data')  # doctest: +SKIP
 
         .. plot::
            :context: close-figs
            :include-source: False
 
            >>> qc = saqc.SaQC(data)
-           >>> qc = qc.flagOffset("data", thresh=2, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, tolerance=1.5, window='6h')
            >>> qc.plot('data')  # doctest: +SKIP
 
         Note, that both, negative and positive jumps are considered starting points of negative or positive
         offsets. If you want to impose the additional condition, that the initial jump must exceed
         +90%* of the value level, you can additionally set the :py:attr:`thresh_relative` parameter:
 
         .. doctest:: flagOffsetExample
 
-           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=.9, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=.9, tolerance=1.5, window='6h')
            >>> qc.plot('data') # doctest:+SKIP
 
         .. plot::
            :context: close-figs
            :include-source: False
 
            >>> qc = saqc.SaQC(data)
-           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=.9, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=.9, tolerance=1.5, window='6h')
            >>> qc.plot('data')  # doctest: +SKIP
 
         Now, only positive jumps, that exceed a value gain of +90%* are considered starting points of offsets.
 
         In the same way, you can aim for only negative offsets, by setting a negative relative threshold.
         The below example only flags offsets, that fall off by at least *50%* in value, with an absolute
         value drop of at least 2.
 
         .. doctest:: flagOffsetExample
 
-           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=-.5, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=-.5, tolerance=1.5, window='6h')
            >>> qc.plot('data') # doctest:+SKIP
 
         .. plot::
            :context: close-figs
            :include-source: False
 
            >>> qc = saqc.SaQC(data)
-           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=-.5, tolerance=1.5, window='6H')
+           >>> qc = qc.flagOffset("data", thresh=2, thresh_relative=-.5, tolerance=1.5, window='6h')
            >>> qc.plot('data')  # doctest: +SKIP
         """
         validateWindow(window)
         if thresh is None and thresh_relative is None:
             raise ValueError(
                 "At least one of parameters 'thresh' and 'thresh_relative' "
                 "has to be given. Got 'thresh'=None, 'thresh_relative'=None "
@@ -1163,29 +1235,19 @@
         pedantic: bool = False,
         flag: float = BAD,
         **kwargs,
     ) -> "SaQC":
         """
         Flag outliers using the Grubbs algorithm.
 
-        See [1] for more information on the grubbs tests definition.
-
-        The (two-sided) test gets applied to data chunks of size :py:attr:`window`. The
-        tests will be iterated chunkwise until no more outliers are detected.
-
-        Note
-        ----
-        * The data is expected to be normally distributed!
-        * The test performs poorly for small data chunks, resulting in considerable
-          overflagging. Select :py:attr:`window` such that every data chunk contains at
-          least 8 values and also adjust the :py:attr:`min_periods` values accordingly.
+        .. deprecated:: 2.6.0
+           Use :py:meth:`~saqc.SaQC.flagUniLOF` or :py:meth:`~saqc.SaQC.flagZScore` instead.
 
         Parameters
         ----------
-
         window :
             Size of the testing window.
             If an integer, the fixed number of observations used for each window.
             If an offset string the time period of each window.
 
         alpha :
             Level of significance, the grubbs test is to be performed at. Must be between 0 and 1.
@@ -1201,14 +1263,22 @@
 
         References
         ----------
         introduction to the grubbs test:
 
         [1] https://en.wikipedia.org/wiki/Grubbs%27s_test_for_outliers
         """
+
+        warnings.warn(
+            "The function flagByGrubbs is deprecated due to its inferior performance, with "
+            "no 100% exact replacement function. When looking for outliers use one of: "
+            "flagZScore, flagUniLOF",
+            DeprecationWarning,
+        )
+
         validateWindow(window)
         validateFraction(alpha, "alpha")
         validateMinPeriods(min_periods, optional=False)
 
         datcol = self._data[field].copy()
         rate = getFreqDelta(datcol.index)
 
@@ -1263,93 +1333,14 @@
         return self
 
     @register(
         mask=["field"],
         demask=["field"],
         squeeze=["field"],
         multivariate=True,
-        handles_target=False,
-        docstring={"field": DOC_TEMPLATES["field"]},
-    )
-    def flagCrossStatistics(
-        self: "SaQC",
-        field: Sequence[str],
-        thresh: float,
-        method: Literal["modZscore", "Zscore"] = "modZscore",
-        flag: float = BAD,
-        **kwargs,
-    ) -> "SaQC":
-        """
-        Function checks for outliers relatively to the "horizontal" input data axis.
-
-        Notes
-        -----
-        The input variables dont necessarily have to be aligned. If the variables are unaligned, scoring
-        and flagging will only be performed on the subset of indices shared among all input variables.
-
-        For :py:attr:`field` :math:`=[f_1,f_2,...,f_N]` and timestamps :math:`[t_1,t_2,...,t_K]`,
-        the following steps are taken for outlier detection:
-
-        1. All timestamps :math:`t_i`, where there is one :math:`f_k`, with :math:`data[f_K]` having no
-           entry at :math:`t_i`, are excluded from the following process (inner join of the :math:`f_i` fields.)
-        2. for every :math:`0 <= i <= K`, the value
-           :math:`m_j = median(\\{data[f_1][t_i], data[f_2][t_i], ..., data[f_N][t_i]\\})` is calculated
-        3. for every :math:`0 <= i <= K`, the set
-           :math:`\\{data[f_1][t_i] - m_j, data[f_2][t_i] - m_j, ..., data[f_N][t_i] - m_j\\}` is tested for
-           outliers with the specified algorithm (:py:attr:`method` parameter).
-
-        Parameters
-        ----------
-        thresh :
-            Threshold which the outlier score of an value must exceed, for being flagged an outlier.
-
-        method :
-            Method used for calculating the outlier scores.
-
-            * ``'modZscore'``: Median based "sigma"-ish approach. See References [1].
-            * ``'Zscore'``: Score values by how many times the standard deviation they differ from the
-              median. See References [1].
-
-
-        References
-        ----------
-        [1] https://www.itl.nist.gov/div898/handbook/eda/section3/eda35h.htm
-        """
-        new_method_string = {
-            "modZscore": "modified",
-            "Zscore": "standard",
-            np.mean: "standard",
-            np.median: "modified",
-        }
-        call = (
-            f"qc.flagZScore(field={field}, window=1, "
-            f"method={new_method_string[method]}, "
-            f"thresh={thresh}, axis=1)"
-        )
-        warnings.warn(
-            f"The method `flagCrossStatistics` is deprecated and will "
-            f"be removed in verion 2.7 of saqc. To achieve the same behavior "
-            f"use:`{call}`",
-            DeprecationWarning,
-        )
-
-        return self.flagZScore(
-            field=field,
-            window=1,
-            method=new_method_string[method],
-            thresh=thresh,
-            axis=1,
-            flag=flag,
-        )
-
-    @register(
-        mask=["field"],
-        demask=["field"],
-        squeeze=["field"],
-        multivariate=True,
         docstring={"field": DOC_TEMPLATES["field"]},
     )
     def flagZScore(
         self: "SaQC",
         field: Sequence[str],
         method: Literal["standard", "modified"] = "standard",
         window: str | int | None = None,
```

### Comparing `saqc-2.5.0/saqc/funcs/pattern.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 # SPDX-License-Identifier: GPL-3.0-or-later
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import dtw
+import fastdtw
 import pandas as pd
 
 from saqc import BAD
 from saqc.core import flagging
 from saqc.lib.rolling import removeRollingRamps
 
 if TYPE_CHECKING:
@@ -23,15 +23,15 @@
     """
     Calculate the DTW-distance of data to pattern in a rolling calculation.
 
     The data is compared to pattern in a rolling window.
     The size of the rolling window is determined by the timespan defined
     by the first and last timestamp of the reference data's datetime index.
 
-    For details see the linked functions in the `See Also` section.
+    For details see the linked functions in the `See also` section.
 
     Parameters
     ----------
     data :
         Data series. Must have datetime-like index, and must be regularly sampled.
 
     reference :
@@ -55,29 +55,29 @@
     distance : pd.Series
 
     Notes
     -----
     The data must be regularly sampled, otherwise a ValueError is raised.
     NaNs in the data will be dropped before dtw distance calculation.
 
-    See Also
+    See also
     --------
     flagPatternByDTW : flag data by DTW
     """
     if reference.hasnans or reference.empty:
         raise ValueError("reference must not have nan's and must not be empty.")
 
     winsz: pd.Timedelta = reference.index.max() - reference.index.min()
     reference = reference.to_numpy()
 
     def isPattern(chunk):
         if forward:
-            return dtw.accelerated_dtw(chunk[::-1], reference, "euclidean")[0]
+            return fastdtw.fastdtw(chunk[::-1], reference)[0]
         else:
-            return dtw.accelerated_dtw(chunk, reference, "euclidean")[0]
+            return fastdtw.fastdtw(chunk, reference)[0]
 
     # generate distances, excluding NaNs
     nonas = data.dropna()
     rollover = nonas[::-1] if forward else nonas
     arr = rollover.rolling(winsz, closed="both").apply(isPattern, raw=True).to_numpy()
     distances = pd.Series(arr[::-1] if forward else arr, index=nonas.index)
     removeRollingRamps(distances, window=winsz, inplace=True)
```

### Comparing `saqc-2.5.0/saqc/funcs/residuals.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/residuals.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ) -> "SaQC":
         """
         Fits a polynomial model to the data and calculate the residuals.
 
         The residual  is calculated by fitting a polynomial of degree `order` to a data
         slice of size `window`, that has x at its center.
 
-        Note, that calculating the residuals tends to be quite costy, because a function
+        Note, that calculating the residuals tends to be quite costly, because a function
         fitting is performed for every sample. To improve performance, consider the
         following possibilities:
 
         In case your data is sampled at an equidistant frequency grid:
 
         (1) If you know your data to have no significant number of missing values,
         or if you do not want to calculate residuals for windows containing missing values
@@ -86,15 +86,15 @@
         return self
 
     @register(mask=["field"], demask=[], squeeze=[])
     def calculateRollingResiduals(
         self: "SaQC",
         field: str,
         window: str | int,
-        func: Callable[[pd.Series], np.ndarray] = np.mean,
+        func: Callable[[pd.Series], np.ndarray] | str = "mean",
         min_periods: int = 0,
         center: bool = True,
         **kwargs,
     ) -> "SaQC":
         """
         Calculate the diff of a rolling-window function and the data.
```

### Comparing `saqc-2.5.0/saqc/funcs/scores.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/scores.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 import pandas as pd
 from sklearn.neighbors import LocalOutlierFactor
 from typing_extensions import Literal
 
 from saqc import UNFLAGGED
 from saqc.core import register
 from saqc.lib.checking import (
-    validateCallable,
     validateChoice,
+    validateFuncSelection,
     validateMinPeriods,
     validateWindow,
 )
 from saqc.lib.docs import DOC_TEMPLATES
 from saqc.lib.tools import getApply, toSequence
 from saqc.lib.ts_operators import kNN
+from saqc.parsing.environ import ENV_OPERATORS, ENV_TRAFOS
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
 def _kNNApply(vals, n_neighbors, func=np.sum, **kwargs):
     dist, *_ = kNN(vals, n_neighbors=n_neighbors, **kwargs)
@@ -120,17 +121,21 @@
         Function to calculate the scaling for every window
     center
         Weather or not to center the target value in the scoring window. If `False`, the
         target value is the last value in the window.
     min_periods
         Minimum number of valid meassurements in a scoring window, to consider the resulting score valid.
     """
+    validateFuncSelection(model_func, "model_func", allow_operator_str=True)
+    if isinstance(model_func, str):
+        model_func = ENV_OPERATORS[model_func]
+    validateFuncSelection(norm_func, "norm_func", allow_operator_str=True)
+    if isinstance(norm_func, str):
+        norm_func = ENV_OPERATORS[norm_func]
     validateWindow(window, optional=True)
-    validateCallable(model_func, "model_func")
-    validateCallable(norm_func, "norm_func")
     validateMinPeriods(min_periods, optional=True)
 
     if data.empty:
         return data, data, data
     if min_periods is None:
         min_periods = 0
 
@@ -162,24 +167,24 @@
         docstring={"field": DOC_TEMPLATES["field"], "target": DOC_TEMPLATES["target"]},
     )
     def assignKNNScore(
         self: "SaQC",
         field: Sequence[str],
         target: str,
         n: int = 10,
-        func: Callable[[pd.Series], float] = np.sum,
+        func: Callable[[pd.Series], float] | str = "sum",
         freq: float | str | None = np.inf,
         min_periods: int = 2,
         algorithm: Literal["ball_tree", "kd_tree", "brute", "auto"] = "ball_tree",
         metric: str = "minkowski",
         p: int = 2,
         **kwargs,
     ) -> "SaQC":
         """
-        Score datapoints by an aggregation of the dictances to their k nearest neighbors.
+        Score datapoints by an aggregation of the distances to their `k` nearest neighbors.
 
         The function is a wrapper around the NearestNeighbors method from pythons sklearn library (See reference [1]).
 
         The steps taken to calculate the scores are as follows:
 
         1. All the timeseries, given through ``field``, are combined to one feature space by an *inner* join on their
            date time indexes. thus, only samples, that share timestamps across all ``field`` will be included in the
@@ -234,18 +239,20 @@
             The keyword just gets passed on to the underlying sklearn method.
             See reference [1] for more information on the algorithm.
 
         References
         ----------
         [1] https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.NearestNeighbors.html
         """
+        validateFuncSelection(func, allow_operator_str=True)
+        if isinstance(func, str):
+            func = ENV_OPERATORS[func]
         validateChoice(
             algorithm, "algorithm", ["ball_tree", "kd_tree", "brute", "auto"]
         )
-        validateCallable(func, "func")
 
         if isinstance(target, list):
             if len(target) > 1:
                 raise ValueError(
                     f"'target' must be of length 1. {target} was passed instead."
                 )
             target = target[0]
@@ -275,32 +282,32 @@
         return self
 
     @register(mask=["field"], demask=[], squeeze=[])
     def assignZScore(
         self: "SaQC",
         field: str,
         window: str | None = None,
-        norm_func: Callable = np.nanstd,
-        model_func: Callable = np.nanmean,
+        norm_func: Callable | str = "std",
+        model_func: Callable | str = "mean",
         center: bool = True,
         min_periods: int | None = None,
         **kwargs,
     ) -> "SaQC":
         """
         Calculate (rolling) Zscores.
 
         See the Notes section for a detailed overview of the calculation
 
         Parameters
         ----------
         window :
-            Size of the window. Either determined via an Offset String, denoting the windows temporal extension or
-            by an integer, denoting the windows number of periods.
-            `NaN` measurements also count as periods.
-            If `None` is passed, All data points share the same scoring window, which than equals the whole
+            Size of the window. can be determined as:
+            * Offset String, denoting the windows temporal extension
+            * Integer, denoting the windows number of periods.
+            * `None` (default), All data points share the same scoring window, which than equals the whole
             data.
         model_func : default std
             Function to calculate the center moment in every window.
         norm_func : default mean
             Function to calculate the scaling for every window
         center :
             Weather or not to center the target value in the scoring window. If `False`, the
@@ -312,17 +319,17 @@
         -----
         Steps of calculation:
 
         1. Consider a window :math:`W` of successive points :math:`W = x_{1},...x_{w}`
         containing the value :math:`y_{K}` wich is to be checked.
         (The index of :math:`K` depends on the selection of the parameter `center`.)
 
-        2. The "moment" :math:`M` for the window gets calculated via :math:`M=` `model_func(:math:`W`)
+        2. The "moment" :math:`M` for the window gets calculated via :math:`M=` model_func(:math:`W`)
 
-        3. The "scaling" :math:`N` for the window gets calculated via :math:`N=` `norm_func(:math:`W`)
+        3. The "scaling" :math:`N` for the window gets calculated via :math:`N=` norm_func(:math:`W`)
 
         4. The "score" :math:`S` for the point :math:`x_{k}`gets calculated via :math:`S=(x_{k} - M) / N`
         """
 
         if min_periods is None:
             min_periods = 0
 
@@ -360,31 +367,34 @@
         Assign Local Outlier Factor (LOF).
 
         Parameters
         ----------
         n :
             Number of periods to be included into the LOF calculation. Defaults to `20`, which is a value found to be
             suitable in the literature.
-
-            * `n` determines the "locality" of an observation (its `n` nearest neighbors) and sets the upper limit of
-              values of an outlier clusters (i.e. consecutive outliers). Outlier clusters of size greater than `n/2`
-              may not be detected reliably.
-            * The larger `n`, the lesser the algorithm's sensitivity to local outliers and small or singleton outliers
-              points. Higher values greatly increase numerical costs.
-
         freq :
             Determines the segmentation of the data into partitions, the kNN algorithm is
             applied onto individually.
         algorithm :
             Algorithm used for calculating the `n`-nearest neighbors needed for LOF calculation.
         p :
             Degree of the metric ("Minkowski"), according to wich distance to neighbors is determined.
             Most important values are:
+
             * `1` - Manhatten Metric
             * `2` - Euclidian Metric
+
+        Notes
+        -----
+
+        * `n` determines the "locality" of an observation (its `n` nearest neighbors) and sets the upper limit of
+          values of an outlier clusters (i.e. consecutive outliers). Outlier clusters of size greater than `n/2`
+          may not be detected reliably.
+        * The larger `n`, the lesser the algorithm's sensitivity to local outliers and small or singleton outliers
+          points. Higher values greatly increase numerical costs.
         """
         from saqc.funcs.outliers import OutliersMixin
 
         validateMinPeriods(min_periods)
         OutliersMixin._validateLOF(algorithm, n, p, 1.0)
 
         if isinstance(target, list):
@@ -453,14 +463,15 @@
 
         algorithm :
             Algorithm used for calculating the `n`-nearest neighbors needed for LOF calculation.
 
         p :
             Degree of the metric ("Minkowski"), according to wich distance to neighbors is determined.
             Most important values are:
+
             * `1` - Manhatten Metric
             * `2` - Euclidian Metric
 
         density :
             How to calculate the temporal distance/density for the variable-to-be-flagged.
 
             * float - introduces linear density with an increment equal to `density`
@@ -470,15 +481,15 @@
         fill_na :
             If True, NaNs in the data are filled with a linear interpolation.
 
         Notes
         -----
         Algorithm steps for uniLOF flagging of variable `x`:
 
-        1. The temporal density `dt(x)` is calculated according o the `density` parameter.
+        1. The temporal density `dt(x)` is calculated according to the `density` parameter.
         2. LOF scores `LOF(x)` are calculated for the concatenation [`x`, `dt(x)`]
         3. `x` is flagged where `LOF(x)` exceeds the threshold determined by the parameter `thresh`.
 
         Examples
         --------
 
         """
@@ -492,30 +503,31 @@
             filled = vals.isna()
             vals = vals.interpolate("linear")
             filled = filled & vals.notna()
         else:
             filled = pd.Series(False, index=vals.index)
 
         if density == "auto":
-            density = vals.diff().abs().median()
+            v_diff = vals.diff()
+            density = v_diff.abs().median()
             if density == 0:
-                density = vals.diff().abs().mean()
+                density = v_diff[v_diff != 0].abs().median()
         elif isinstance(density, Callable):
             density = density(vals)
         if isinstance(density, pd.Series):
             density = density.values
 
         d_var = pd.Series(np.arange(len(vals)) * density, index=vals.index)
         na_bool_ser = vals.isna() | d_var.isna()
         na_idx = na_bool_ser.index[na_bool_ser.values]
         # notna_bool = vals.notna()
         val_no = (~na_bool_ser).sum()
-        if 1 < val_no < n:
-            n = val_no
-        elif val_no <= 1:
+        if 2 < val_no <= n:
+            n = val_no - 2
+        elif val_no <= 2:
             return self
 
         d_var = d_var.drop(na_idx, axis=0).values
         vals = vals.drop(na_idx, axis=0).values
         vals_extended = np.array(
             list(vals[::-1][-n:]) + list(vals) + list(vals[::-1][:n])
         )
```

### Comparing `saqc-2.5.0/saqc/funcs/transformation.py` & `saqc-2.5.0.post0.dev145/saqc/funcs/transformation.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from saqc.core import register
+from saqc.lib.checking import validateFuncSelection
+from saqc.parsing.environ import ENV_TRAFOS
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
 class TransformationMixin:
     @register(mask=["field"], demask=[], squeeze=[])
     def transform(
         self: "SaQC",
         field: str,
-        func: Callable[[pd.Series | np.ndarray], pd.Series],
+        func: Callable[[pd.Series | np.ndarray], pd.Series] | str,
         freq: float | str | None = None,
         **kwargs,
     ) -> "SaQC":
         """
         Transform data by applying a custom function on data chunks of variable size. Existing flags are preserved.
 
         Parameters
@@ -38,14 +40,18 @@
         freq :
             Size of the data window. The transformation is applied on each window individually
 
             * ``None``: Apply transformation on the entire data set at once
             * ``int`` : Apply transformation on successive data chunks of the given length. Must be grater than 0.
             * Offset String : Apply transformation on successive data chunks of the given temporal extension.
         """
+        validateFuncSelection(func, allow_trafo_str=True)
+        if isinstance(func, str):
+            func = ENV_TRAFOS[func]
+
         val_ser = self._data[field].copy()
         # partitioning
         if not freq:
             freq = len(val_ser)
 
         if isinstance(freq, str):
             grouper = pd.Grouper(freq=freq)
```

### Comparing `saqc-2.5.0/saqc/lib/checking.py` & `saqc-2.5.0.post0.dev145/saqc/lib/checking.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,36 +7,38 @@
 from typing import Any, Collection, Iterable, Literal, TypeVar, get_origin
 
 import numpy as np
 import pandas as pd
 
 T = TypeVar("T")
 
+
 # ====================================================================
 # `isSomething`-Checks: must not raise Exceptions by checking the value (but
 # might rise Exceptions on wrong usage) and should return a boolean
 # value
 # ====================================================================
-
-
+#
+# Module should not have no saqc dependencies
+#
 def isBoolLike(obj: Any, optional: bool = False) -> bool:
     """Return True if obj is a boolean or one of the integers 0 or 1.
     If optional is True, `None` also is considered a valid boolean.
     """
     return (
-        isinstance(obj, bool)
+        pd.api.types.is_bool(obj)
         or optional
         and obj is None
-        or isinstance(obj, int)
+        or pd.api.types.is_integer(obj)
         and obj in [0, 1]
     )
 
 
 def isFloatLike(obj: Any) -> bool:
-    return isinstance(obj, (float, int))
+    return pd.api.types.is_float(obj) or pd.api.types.is_integer(obj)
 
 
 def isIterable(obj: Any) -> bool:
     if isinstance(obj, Iterable) or pd.api.types.is_iterator(obj):
         return True
     try:
         iter(obj)
@@ -97,20 +99,38 @@
         or fixed_only
         and isFixedFrequencyOffset(obj)
         or allow_str
         and isFrequencyString(obj, fixed_only=fixed_only)
     )
 
 
+def isValidFuncSelection(
+    obj: Any,
+    allow_callable: bool = True,
+    allow_operator_str: bool = False,
+    allow_trafo_str: bool = False,
+):
+    from saqc.parsing.environ import ENV_OPERATORS, ENV_TRAFOS
+
+    return (
+        allow_callable
+        and callable(obj)
+        or allow_operator_str
+        and obj in ENV_OPERATORS.keys()
+        or allow_trafo_str
+        and obj in ENV_TRAFOS.keys()
+    )
+
+
 def isValidWindow(obj: Any, allow_int: bool = True, allow_str: bool = True) -> bool:
     return (
         isinstance(obj, pd.Timedelta)
         or isFixedFrequencyOffset(obj)
         or allow_int
-        and isinstance(obj, int)
+        and pd.api.types.is_integer(obj)
         and isInBounds(obj, 0)
         or allow_str
         and isTimedeltaString(obj)
     )
 
 
 def isValidChoice(value: T, choices: Collection[T]) -> bool:
@@ -196,15 +216,15 @@
     if _isLiteral(choices):
         choices = extractLiteral(choices)
     if not isValidChoice(value, choices):
         raise ValueError(f"{name!r} must be one of {set(choices)}, not {value!r}")
 
 
 def isIntOrInf(obj: int | float) -> bool:
-    return isinstance(obj, int) or isinstance(obj, float) and np.isinf(obj)
+    return pd.api.types.is_integer(obj) or pd.api.types.is_float(obj) and np.isinf(obj)
 
 
 def validateValueBounds(
     value: int | float,
     name: str,
     left: int | float = -np.inf,
     right: int | float = np.inf,
@@ -255,14 +275,42 @@
         types.append("an offset-string")
     msg = f"{name!r} must be {joinExt(', ', types, ' or ')}, not {value!r}"
 
     if not isValidFrequency(value, allow_str=allow_str, fixed_only=fixed_only):
         raise ValueError(msg)
 
 
+def validateFuncSelection(
+    value: Any,
+    name: str = "func",
+    allow_callable: bool = True,
+    allow_operator_str: bool = False,
+    allow_trafo_str: bool = False,
+):
+    """
+    Validate Function selection to be either a Callable or a kex fro the environments Dictionaries.
+    """
+    from saqc.lib.tools import joinExt
+    from saqc.parsing.environ import ENV_OPERATORS, ENV_TRAFOS
+
+    is_valid = isValidFuncSelection(
+        value,
+        allow_callable=allow_callable,
+        allow_trafo_str=allow_trafo_str,
+        allow_operator_str=allow_operator_str,
+    )
+
+    msg_c = ["of type callable"] * allow_callable
+    msg_op = [f"a string out of {ENV_OPERATORS.keys()}"] * allow_operator_str
+    msg_tr = [f"a string out of {ENV_TRAFOS.keys()}"] * allow_trafo_str
+    msg = joinExt(", ", msg_c + msg_op + msg_tr, " or ")
+    if not is_valid:
+        raise ValueError(f"Parameter '{name}' must be {msg}. Got '{value}' instead.")
+
+
 def validateWindow(
     value: int | str | pd.offsets.BaseOffset | pd.Timedelta,
     name: str = "window",
     allow_int: bool = True,
     allow_str: bool = True,
     optional: bool = False,
     index: pd.Index | None = None,
```

### Comparing `saqc-2.5.0/saqc/lib/docs.py` & `saqc-2.5.0.post0.dev145/saqc/lib/docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
-from typing import Any, TypedDict
+from typing import TypedDict
 
-from docstring_parser import DocstringParam, DocstringReturns, compose, parse
+from docstring_parser import (
+    DocstringParam,
+    DocstringReturns,
+    DocstringStyle,
+    compose,
+    parse,
+)
 
 
 class ParamDict(TypedDict):
     typehint: str | None
     description: str | None
     optional: bool | None
 
@@ -46,65 +52,65 @@
         "description": "The flag value the function uses to mark observations. Defaults to the ``BAD`` value of the translation scheme.",
         "typehint": "Any",
         "optional": True,
     },
 }
 
 
-class FunctionParam(DocstringParam):
-    def __init__(
-        self, name: str, typehint: str, description: str, optional: bool = False
-    ):
-        super().__init__(
-            args=["param", name],
-            description=description,
-            arg_name=name,
-            type_name=typehint,
-            is_optional=optional,
-            default=None,
-        )
+def toParameter(
+    name: str, typehint: str, description: str, optional: bool = False
+) -> DocstringParam:
+    return DocstringParam(
+        args=["param", name],
+        description=description,
+        arg_name=name,
+        type_name=typehint,
+        is_optional=optional,
+        default=None,
+    )
 
 
 def docurator(func, defaults: dict[str, ParamDict] | None = None):
     if defaults is None:
         defaults = {}
 
     docstring_return = DocstringReturns(
         args=["returns"],
         description="the updated SaQC object",
         type_name="saqc.SaQC",
         is_generator=False,
         return_name="SaQC",
     )
 
-    tree = parse(func.__doc__)
+    tree = parse(func.__doc__, style=DocstringStyle.NUMPYDOC)
 
     if tree.returns:
         raise ValueError(
             f"'{func.__name__}' function doctstring should not provide a returns section"
         )
 
     # rewrite parameters
-    meta = [FunctionParam(**{**COMMON["field"], **defaults.get("field", {})})]
+    meta = [toParameter(**{**COMMON["field"], **defaults.get("field", {})})]
     for p in tree.params:
         if p.arg_name in COMMON:
             raise ValueError(
                 f"'{func.__name__}' function docstring should not provide a parameter description for '{p.arg_name}'"
             )
         meta.append(p)
 
     # additional parameters
     for p in ("target", "dfilter", "flag"):
-        meta.append(FunctionParam(**{**COMMON[p], **defaults.get(p, {})}))
+        meta.append(toParameter(**{**COMMON[p], **defaults.get(p, {})}))
 
     # return sections
     meta.append(docstring_return)
 
     # everyhing else the docstring provides
     for m in tree.meta:
         if not isinstance(m, DocstringParam):
             meta.append(m)
 
     tree.meta = meta
 
     func.__doc__ = compose(tree)
+
     return func
```

### Comparing `saqc-2.5.0/saqc/lib/plotting.py` & `saqc-2.5.0.post0.dev145/saqc/lib/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         na_mask,
         plot_kwargs,
         ax_kwargs,
         scatter_kwargs,
         mode,
     )
 
-    # readability formattin fo the x-tick labels:
+    # readability formattin for the x-tick labels:
     fig.autofmt_xdate()
     return fig
 
 
 def _instantiateAxesContext(
     plot_kwargs, scatter_kwargs, ax_kwargs, var_num, var_name, mode
 ):
@@ -274,15 +274,15 @@
     )
     # skip through cycles on to the desired start
     for k in range(0, cyclestart):
         next(_scatter_kwargs["color"])
         next(_scatter_kwargs["marker"])
 
     # assign variable specific labels/titles
-    for axis_spec in ["xlabel", "ylabel", "title"]:
+    for axis_spec in ["xlabel", "ylabel", "title", "ylim"]:
         spec = _ax_kwargs.get(axis_spec, None)
         if isinstance(spec, list):
             _ax_kwargs[axis_spec] = spec[var_num]
         elif isinstance(spec, dict):
             _ax_kwargs[axis_spec] = spec.get(var_name, None)
 
     title = _ax_kwargs.get("title", "" if mode != "subplots" else None)
```

### Comparing `saqc-2.5.0/saqc/lib/rolling.py` & `saqc-2.5.0.post0.dev145/saqc/lib/rolling.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/lib/tools.py` & `saqc-2.5.0.post0.dev145/saqc/lib/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,15 +173,32 @@
             s = start_replacer(x.index)
             e = end_replacer(x.index)
             x[s:e] = False
             x[s:s] = True
             x[e:e] = True
             return x
 
-    freq = "1" + "mmmhhhdddMMMYYY"[len(season_start)]
+    freq = (
+        "1",
+        "m",
+        "m",
+        "m",
+        "h",
+        "h",
+        "h",
+        "d",
+        "d",
+        "d",
+        "M",
+        "M",
+        "M",
+        "YE",
+        "YE",
+        "YE",
+    )[len(season_start)]
     out = mask.groupby(pd.Grouper(freq=freq)).transform(_selector)
     if invert:
         out = ~out
     return out
 
 
 def isQuoted(string):
@@ -397,15 +414,15 @@
     If yes, the according timedelta value is returned,
 
     If no, ``None`` is returned.
 
     (``None`` will also be returned for pd.RangeIndex type.)
 
     """
-    delta = getattr(index, "window", None)
+    delta = getattr(index, "freq", None)
     if delta is None and not index.empty:
         i = pd.date_range(index[0], index[-1], len(index))
         if i.equals(index):
             return i[1] - i[0]
     return delta
 
 
@@ -550,15 +567,15 @@
 def initializeTargets(
     saqc,
     fields: Sequence[str],
     targets: Sequence[str],
     index: pd.Index,
 ):
     """
-    Initialize all targets based on field.
+    Initialize all targets based on fields.
 
     Note
     ----
     The following behavior is implemented:
     1. n 'field', n 'target', n > 0     -> direct copy
     2. n 'field', m 'target' mit n != m -> empty targets
     """
@@ -648,7 +665,25 @@
         raise TypeError("'sep' must be string")
     if not isinstance(sep, str):
         raise TypeError("'last_sep' must be string or None")
     iterable = list(iterable)  # ensure __len__ and __getitem__
     if len(iterable) < 2:
         return sep.join(iterable)
     return f"{sep.join(iterable[:-1])}{last_sep}{iterable[-1]}"
+
+
+def multivariateParameters(
+    field: str | list[str], target: str | list[str] | None = None
+) -> tuple[list[str], list[str], bool]:
+    fields = toSequence(field)
+    targets = fields if target is None else toSequence(target)
+    broadcasting = False
+
+    if len(targets) == 1:
+        targets = targets * len(fields)
+        broadcasting = True
+    if len(targets) != len(fields):
+        raise ValueError(
+            "expected a single 'target' or the same number of 'field' and 'target' values"
+        )
+
+    return fields, targets, broadcasting
```

### Comparing `saqc-2.5.0/saqc/lib/ts_operators.py` & `saqc-2.5.0.post0.dev145/saqc/lib/ts_operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,33 @@
 import numpy as np
 import numpy.polynomial.polynomial as poly
 import pandas as pd
 from scipy.signal import butter, filtfilt
 from scipy.stats import iqr, median_abs_deviation
 from sklearn.neighbors import NearestNeighbors
 
-from saqc.lib.checking import validateChoice, validateWindow
 from saqc.lib.tools import getFreqDelta
 
 
+def mad(series):
+    return median_abs_deviation(series, nan_policy="omit")
+
+
+def clip(series, lower=None, upper=None):
+    return series.clip(lower=lower, upper=upper)
+
+
+def cv(series: pd.Series) -> pd.Series:
+    """
+    calculates the coefficient of variation on a min-max scaled time series
+    """
+    series_ = (series - series.min()) / (series.max() - series.min())
+    return series_.std() / series_.mean()
+
+
 def identity(ts):
     """
     Returns the input.
 
     Parameters
     ----------
     ts : pd.Series
@@ -174,26 +189,26 @@
         return pd.Series(data=0.5, index=ts.index)
     else:
         return (ts - ts_min) / (ts.max() - ts_min)
 
 
 def standardizeByMean(ts):
     # standardization with mean and probe variance
-    return (ts - np.mean(ts)) / np.std(ts, ddof=1)
+    return (ts - np.nanmean(ts)) / np.nanstd(ts, ddof=1)
 
 
 def standardizeByMedian(ts):
     # standardization with median (MAD)
     # NO SCALING
-    return (ts - np.median(ts)) / median_abs_deviation(ts, nan_policy="omit")
+    return (ts - np.nanmedian(ts)) / median_abs_deviation(ts, nan_policy="omit")
 
 
 def standardizeByIQR(ts):
     # standardization with median and inter quantile range
-    return (ts - np.median(ts)) / iqr(ts, nan_policy="omit")
+    return (ts - np.nanmedian(ts)) / iqr(ts, nan_policy="omit")
 
 
 def kNN(in_arr, n_neighbors, algorithm="ball_tree", metric="minkowski", p=2):
     # k-nearest-neighbor search
 
     nbrs = NearestNeighbors(
         n_neighbors=n_neighbors, algorithm=algorithm, metric=metric, p=p
@@ -225,36 +240,74 @@
     exceeded: bool
         True if more than allowed consecutive NaNs appear, False otherwise.
     """
     s = arr.shape[0]
     if s <= max_consec:
         return False
     views = np.lib.stride_tricks.sliding_window_view(
-        arr, window_shape=min(s, max_consec + 1)
+        arr, window_shape=min([s, max_consec + 1])
     )
     return bool(views.all(axis=1).any())
 
 
-def validationTrafo(data, max_nan_total, max_nan_consec):
+def validationTrafo(data, max_nan_total, max_nan_consec, trafo=True):
     # data has to be boolean. False=Valid Value, True=invalid Value function returns
     # True-array of input array size for invalid input arrays False array for valid
     # ones
-    data = data.copy()
-    if max_nan_total is np.inf and max_nan_consec is np.inf:
-        return data
+    if trafo:
+        data = data.copy()
 
-    if data.sum() > max_nan_total:
+    if max_nan_total == np.inf and max_nan_consec == np.inf:
+        value = False
+    elif data.sum() > max_nan_total:
         value = True
-    elif max_nan_consec is np.inf:
+    elif min(max_nan_consec, max_nan_total) > data.sum():
         value = False
     else:
         value = _exceedConsecutiveNanLimit(np.asarray(data), max_nan_consec)
 
-    data[:] = value
-    return data
+    if trafo:
+        data[:] = value
+        return data
+    else:
+        return value
+
+
+def isValid(
+    data: pd.Series, max_nan_total: int = None, max_nan_consec: int = None
+) -> bool:
+    """
+    The function checks for input data having not more than ``max_nan_total`` NaN values in total,
+    and not more than ``max_nan_consec`` consecutive NaN values.
+
+    Parameters
+    ----------
+    data :
+        input data Series to check
+
+    max_nan_total :
+        Total maximum number of NaN values allowed in `data` .
+
+    max_nan_consec :
+        Maximum chunk length of consecutive NaN values allowed in `data`.
+
+    Returns
+    -------
+    out :
+        False if ``data`` is conflicting with the NaN-limit conditions and True otherwise.
+
+    """
+    if (max_nan_total is not None) and (data.isna().sum() > max_nan_total):
+        return False
+    elif (max_nan_consec is not None) and (
+        data.rolling(max_nan_consec + 1, min_periods=max_nan_consec + 1).count().min()
+        == 0
+    ):
+        return False
+    return True
 
 
 def stdQC(data, max_nan_total=np.inf, max_nan_consec=np.inf):
     return np.nanstd(
         data[~validationTrafo(data.isna(), max_nan_total, max_nan_consec)], ddof=1
     )
 
@@ -332,16 +385,14 @@
     :param extrapolate:             Str or None. Default None. If True:
                                     If a data chunk not contains enough values for interpolation of the order "order",
                                     the highest order possible will be selected for that chunks interpolation.
 
     :return:
     """
 
-    # TODO: IMAO, this code desperately needs a refactoring/rewrite --palmb
-
     gap_check = np.nan if isinstance(gap_limit, str) else gap_limit
     data = pd.Series(data, copy=True)
     limit_area = None if extrapolate else "inside"
     if gap_check is None:
         # if there is actually no limit set to the gaps to-be interpolated,
         # generate a dummy mask for the gaps
         gap_mask = pd.Series(True, index=data.index, name=data.name)
@@ -409,114 +460,14 @@
             },
         )
     # finally reinsert the dropped data gaps
     data = data.reindex(pre_index)
     return data
 
 
-def aggregate2Freq(
-    data: pd.Series,
-    method,
-    freq,
-    agg_func,
-    fill_value=np.nan,
-    max_invalid_total=None,
-    max_invalid_consec=None,
-):
-    """
-    The function aggregates values to an equidistant frequency grid with func.
-    Timestamps that gets no values projected, get filled with the fill-value. It
-    also serves as a replacement for "invalid" intervals.
-    """
-    validateChoice(method, "method", ["nagg", "bagg", "fagg"])
-    validateWindow(freq, "freq", allow_int=False)
-
-    methods = {
-        # offset, closed, label
-        "nagg": lambda f: (f / 2, "left", "left"),
-        "bagg": lambda _: (pd.Timedelta(0), "left", "left"),
-        "fagg": lambda _: (pd.Timedelta(0), "right", "right"),
-    }
-    # filter data for invalid patterns (since filtering is expensive we pre-check if
-    # it is demanded)
-    if max_invalid_total is not None or max_invalid_consec is not None:
-        if pd.isna(fill_value):
-            temp_mask = data.isna()
-        else:
-            temp_mask = data == fill_value
-
-        temp_mask = temp_mask.groupby(pd.Grouper(freq=freq)).transform(
-            validationTrafo,
-            max_nan_total=max_invalid_total,
-            max_nan_consec=max_invalid_consec,
-        )
-        data[temp_mask] = fill_value
-
-    freq = pd.Timedelta(freq)
-    offset, closed, label = methods[method](freq)
-
-    resampler = data.resample(
-        freq, closed=closed, label=label, origin="start_day", offset=offset
-    )
-
-    # count valid values
-    counts = resampler.count()
-
-    # native methods of resampling (median, mean, sum, ..) are much faster than apply
-    try:
-        check_name = re.sub("^nan", "", agg_func.__name__)
-        # a nasty special case: if function "count" was passed, we not want empty
-        # intervals to be replaced by fill_value:
-        if check_name == "count":
-            data = counts.copy()
-            counts[:] = np.nan
-        else:
-            data = getattr(resampler, check_name)()
-    except AttributeError:
-        data = resampler.apply(agg_func)
-
-    # we custom fill bins that have no value
-    data[counts == 0] = fill_value
-
-    # undo the temporary shift, to mimic centering the frequency
-    if method == "nagg":
-        data.index += offset
-
-    return data
-
-
-def shift2Freq(
-    data: Union[pd.Series, pd.DataFrame],
-    method: Literal["fshift", "bshift", "nshift"],
-    freq: str,
-    fill_value,
-):
-    """
-    shift timestamps backwards/forwards in order to align them with an equidistant
-    frequency grid. Resulting Nan's are replaced with the fill-value.
-    """
-    validateWindow(freq, "freq", allow_int=False)
-    validateChoice(method, "method", ["fshift", "bshift", "nshift"])
-    methods = {
-        "fshift": lambda freq: ("ffill", pd.Timedelta(freq)),
-        "bshift": lambda freq: ("bfill", pd.Timedelta(freq)),
-        "nshift": lambda freq: ("nearest", pd.Timedelta(freq) / 2),
-    }
-    direction, tolerance = methods[method](freq)
-    target_ind = pd.date_range(
-        start=pd.Timestamp(data.index[0]).floor(freq),
-        end=pd.Timestamp(data.index[-1]).ceil(freq),
-        freq=freq,
-        name=data.index.name,
-    )
-    return data.reindex(
-        target_ind, method=direction, tolerance=tolerance, fill_value=fill_value
-    )
-
-
 def butterFilter(
     x, cutoff, nyq=0.5, filter_order=2, fill_method="linear", filter_type="lowpass"
 ):
     """
     Applies butterworth filter.
     `x` is expected to be regularly sampled.
 
@@ -600,7 +551,39 @@
 
 def linearInterpolation(data, inter_limit=2):
     return interpolateNANs(data, "time", gap_limit=inter_limit)
 
 
 def polynomialInterpolation(data, inter_limit=2, inter_order=2):
     return interpolateNANs(data, "polynomial", gap_limit=inter_limit, order=inter_order)
+
+
+def climatologicalMean(data):
+    """
+    The true daily mean as defined by WMO standard:
+    true daily mean = val@6:30 + val@12:30 + 2*val@20:30, NaN if one val is missing.
+    """
+    d = data[
+        ((data.index.hour == 6) & (data.index.minute == 30))
+        | ((data.index.hour == 12) & (data.index.minute == 30))
+    ]
+    d = pd.concat([d, 2 * data[((data.index.hour == 20) & (data.index.minute == 30))]])
+    d = d[d.index.second == 0]
+    rs = d.resample("1D")
+    res = rs.mean()
+    invalid = rs.count() < 3
+    res[invalid] = np.nan
+    return res
+
+
+def trueDailyMean(data):
+    dat = pd.Series(data.values, index=data.index.shift(1, "10min"))
+    dat = dat.reindex(
+        pd.date_range(
+            dat.index[0].date(), dat.index[-1].date() + pd.Timedelta("1D"), freq="1h"
+        )
+    )
+    rs = dat.resample("1D")
+    res = rs.mean()
+    valid = rs.apply(func=isValid, **{"max_nan_consec": 2}).astype(bool)
+    res[~valid] = np.nan
+    return res
```

### Comparing `saqc-2.5.0/saqc/lib/types.py` & `saqc-2.5.0.post0.dev145/saqc/lib/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 ArrayLike = TypeVar("ArrayLike", np.ndarray, pd.Series, pd.DataFrame)
 
 ExternalFlag = Union[str, float, int]
 
 
 # needed for deeper type hinting magic
 class CurveFitter(Protocol):
-    def __call__(self, data: np.ndarray, *params: float) -> np.ndarray:
-        ...  # pragma: no cover
+    def __call__(
+        self, data: np.ndarray, *params: float
+    ) -> np.ndarray: ...  # pragma: no cover
 
 
 class Comparable(Protocol):
     @abc.abstractmethod
     def __gt__(self: CompT, other: CompT) -> bool:
         pass
```

### Comparing `saqc-2.5.0/saqc/parsing/reader.py` & `saqc-2.5.0.post0.dev145/saqc/parsing/reader.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/saqc/parsing/visitor.py` & `saqc-2.5.0.post0.dev145/saqc/parsing/visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # -*- coding: utf-8 -*-
 
 import ast
 import importlib
 
-import numpy as np
-
 from saqc.core.register import FUNC_MAP
 from saqc.parsing.environ import ENVIRONMENT
 
 
 class ConfigExpressionParser(ast.NodeVisitor):
     """
     Generic configuration functions will be rewritten as lambda functions
@@ -24,21 +22,20 @@
 
     The main purpose of this class is to identify all variables used in
     a given generic function and to check that it does not violate the
     restrictions imposed onto generic functions.
     """
 
     SUPPORTED = (
-        ast.Str,
+        ast.Constant,
         ast.Expression,
         ast.UnaryOp,
         ast.BinOp,
         ast.BitOr,
         ast.BitAnd,
-        ast.Num,
         ast.Compare,
         ast.Add,
         ast.Sub,
         ast.Mult,
         ast.Div,
         ast.Pow,
         ast.Mod,
@@ -82,18 +79,16 @@
             raise TypeError(f"invalid expression: '{node}'")
         return super().generic_visit(node)
 
 
 class ConfigFunctionParser(ast.NodeVisitor):
     SUPPORTED_NODES = (
         ast.Call,
-        ast.Num,
-        ast.Str,
+        ast.Constant,
         ast.keyword,
-        ast.NameConstant,
         ast.UnaryOp,
         ast.Name,
         ast.Load,
         ast.Expression,
         ast.Subscript,
         ast.Index,
         ast.USub,
```

### Comparing `saqc-2.5.0/saqc.egg-info/PKG-INFO` & `saqc-2.5.0.post0.dev145/saqc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: saqc
-Version: 2.5.0
+Version: 2.5.0.post0.dev145
 Summary: A timeseries data quality control and processing tool/framework
 Home-page: https://git.ufz.de/rdm-software/saqc
 Author: Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss
 Author-email: david.schaefer@ufz.de
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: LICENSES/GPL-3.0-or-later.txt
+Requires-Dist: Click
+Requires-Dist: docstring_parser
+Requires-Dist: fancy-collections
+Requires-Dist: fastdtw
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numpy
+Requires-Dist: outlier-utils
+Requires-Dist: pyarrow
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: typing_extensions
 
 <!--
 SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
@@ -70,15 +82,15 @@
 file listing the variables in the dataset and the routines to inspect,
 quality control and/or process them. The content of such a configuration
 could look like [this](https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/config.csv):
 
 ```
 varname    ; test
 #----------; ---------------------------------------------------------------------
-SM2        ; shift(freq="15Min")
+SM2        ; align(freq="15Min")
 'SM(1|2)+' ; flagMissing()
 SM1        ; flagRange(min=10, max=60)
 SM2        ; flagRange(min=10, max=40)
 SM2        ; flagZScore(window="30d", thresh=3.5, method='modified', center=False)
 Dummy      ; flagGeneric(field=["SM1", "SM2"], func=(isflagged(x) | isflagged(y)))
 ```
 
@@ -111,15 +123,15 @@
 data = pd.read_csv(
     "https://git.ufz.de/rdm-software/saqc/raw/develop/docs/resources/data/data.csv",
     index_col=0, parse_dates=True,
 )
 
 qc = SaQC(data=data)
 qc = (qc
-      .shift("SM2", freq="15Min")
+      .align("SM2", freq="15Min")
       .flagMissing("SM(1|2)+", regex=True)
       .flagRange("SM1", min=10, max=60)
       .flagRange("SM2", min=10, max=40)
       .flagZScore("SM2", window="30d", thresh=3.5, method='modified', center=False)
       .flagGeneric(field=["SM1", "SM2"], target="Dummy", func=lambda x, y: (isflagged(x) | isflagged(y))))
 ```
```

### Comparing `saqc-2.5.0/saqc.egg-info/SOURCES.txt` & `saqc-2.5.0.post0.dev145/saqc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
-versioneer.py
 LICENSES/GPL-3.0-or-later.txt
 saqc/__init__.py
 saqc/__main__.py
 saqc/_version.py
 saqc/constants.py
 saqc/exceptions.py
 saqc/version.py
@@ -20,14 +19,15 @@
 saqc/core/core.py
 saqc/core/flags.py
 saqc/core/frame.py
 saqc/core/history.py
 saqc/core/mixins.py
 saqc/core/register.py
 saqc/core/translation/__init__.py
+saqc/core/translation/annotationscheme.py
 saqc/core/translation/basescheme.py
 saqc/core/translation/dmpscheme.py
 saqc/core/translation/floatscheme.py
 saqc/core/translation/positionalscheme.py
 saqc/core/translation/simplescheme.py
 saqc/funcs/__init__.py
 saqc/funcs/breaks.py
@@ -48,14 +48,15 @@
 saqc/funcs/tools.py
 saqc/funcs/transformation.py
 saqc/lib/__init__.py
 saqc/lib/checking.py
 saqc/lib/docs.py
 saqc/lib/plotting.py
 saqc/lib/rolling.py
+saqc/lib/selectionGUI.py
 saqc/lib/tools.py
 saqc/lib/ts_operators.py
 saqc/lib/types.py
 saqc/parsing/__init__.py
 saqc/parsing/environ.py
 saqc/parsing/reader.py
 saqc/parsing/visitor.py
```

### Comparing `saqc-2.5.0/setup.py` & `saqc-2.5.0.post0.dev145/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,39 +24,32 @@
     raise RuntimeError(v["error"])
 
 if v["dirty"]:
     raise ValueError(
         f"The repository you build is dirty. Please commit changes first {v}."
     )
 
-if "dev" in v["version"] and name == "saqc":
-    raise ValueError(
-        f"An saqc release must have version in the format X.Y.Z, "
-        f"which requires a git tag on the same commit. Please set "
-        f"a tag, then build again. {v}"
-    )
-
 
 setup(
     name=name,
     version=versioneer.get_version(),  # keep this line as it is
     cmdclass=versioneer.get_cmdclass(),  # keep this line as it is
     author="Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss",
     author_email="david.schaefer@ufz.de",
     description="A timeseries data quality control and processing tool/framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ufz.de/rdm-software/saqc",
     packages=find_packages(exclude=("tests", "docs")),
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=[
         "Click",
-        "dtw",
         "docstring_parser",
         "fancy-collections",
+        "fastdtw",
         "matplotlib>=3.4",
         "numpy",
         "outlier-utils",
         "pyarrow",
         "pandas>=2.0.0",
         "scikit-learn",
         "scipy",
```

### Comparing `saqc-2.5.0/tests/api/test_creation.py` & `saqc-2.5.0.post0.dev145/tests/api/test_creation.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/cli/test_integration.py` & `saqc-2.5.0.post0.dev145/tests/cli/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,54 +7,50 @@
 
 import pytest
 from click.testing import CliRunner
 
 FLOAT = [
     ",Battery,Battery,SM1,SM1,SM2,SM2\n",
     ",data,flags,data,flags,data,flags\n",
-    "Date,,,,,,\n",
     "2016-04-01 00:00:00,nan,nan,nan,nan,29.3157,-inf\n",
     "2016-04-01 00:05:48,3573.0,-inf,32.685,-inf,nan,nan\n",
     "2016-04-01 00:15:00,nan,nan,nan,nan,29.3157,-inf\n",
     "2016-04-01 00:20:42,3572.0,-inf,32.7428,-inf,nan,nan\n",
     "2016-04-01 00:30:00,nan,nan,nan,nan,29.3679,255.0\n",
     "2016-04-01 00:35:37,3572.0,-inf,32.6186,-inf,nan,nan\n",
     "2016-04-01 00:45:00,nan,nan,nan,nan,29.3679,-inf\n",
 ]
 
 SIMPLE = [
     ",Battery,Battery,SM1,SM1,SM2,SM2\n",
     ",data,flags,data,flags,data,flags\n",
-    "Date,,,,,,\n",
     "2016-04-01 00:00:00,nan,nan,nan,nan,29.3157,UNFLAGGED\n",
     "2016-04-01 00:05:48,3573.0,UNFLAGGED,32.685,UNFLAGGED,nan,nan\n",
     "2016-04-01 00:15:00,nan,nan,nan,nan,29.3157,UNFLAGGED\n",
     "2016-04-01 00:20:42,3572.0,UNFLAGGED,32.7428,UNFLAGGED,nan,nan\n",
     "2016-04-01 00:30:00,nan,nan,nan,nan,29.3679,BAD\n",
     "2016-04-01 00:35:37,3572.0,UNFLAGGED,32.6186,UNFLAGGED,nan,nan\n",
     "2016-04-01 00:45:00,nan,nan,nan,nan,29.3679,UNFLAGGED\n",
 ]
 
 POSITIONAL = [
     ",Battery,Battery,SM1,SM1,SM2,SM2\n",
     ",data,flags,data,flags,data,flags\n",
-    "Date,,,,,,\n",
-    "2016-04-01 00:00:00,nan,-9999,nan,-9999,29.3157,90000\n",
-    "2016-04-01 00:05:48,3573.0,9,32.685,90,nan,-9999\n",
-    "2016-04-01 00:15:00,nan,-9999,nan,-9999,29.3157,90000\n",
-    "2016-04-01 00:20:42,3572.0,9,32.7428,90,nan,-9999\n",
-    "2016-04-01 00:30:00,nan,-9999,nan,-9999,29.3679,90002\n",
-    "2016-04-01 00:35:37,3572.0,9,32.6186,90,nan,-9999\n",
-    "2016-04-01 00:45:00,nan,-9999,nan,-9999,29.3679,90000\n",
+    "2016-04-01 00:00:00,-9999,-9999,-9999.0,-9999,29.3157,90000\n",
+    "2016-04-01 00:05:48,3573,9,32.685,90,-9999.0,-9999\n",
+    "2016-04-01 00:15:00,-9999,-9999,-9999.0,-9999,29.3157,90000\n",
+    "2016-04-01 00:20:42,3572,9,32.7428,90,-9999.0,-9999\n",
+    "2016-04-01 00:30:00,-9999,-9999,-9999.0,-9999,29.3679,90002\n",
+    "2016-04-01 00:35:37,3572,9,32.6186,90,-9999.0,-9999\n",
+    "2016-04-01 00:45:00,-9999,-9999,-9999.0,-9999,29.3679,90000\n",
 ]
 
 DMP = [
     ",Battery,Battery,Battery,Battery,SM1,SM1,SM1,SM1,SM2,SM2,SM2,SM2\n",
     ",data,quality_flag,quality_cause,quality_comment,data,quality_flag,quality_cause,quality_comment,data,quality_flag,quality_cause,quality_comment\n",
-    "Date,,,,,,,,,,,,\n",
     "2016-04-01 00:00:00,nan,nan,nan,nan,nan,nan,nan,nan,29.3157,NIL,,\n",
     "2016-04-01 00:05:48,3573.0,NIL,,,32.685,NIL,,,nan,nan,nan,nan\n",
     "2016-04-01 00:15:00,nan,nan,nan,nan,nan,nan,nan,nan,29.3157,NIL,,\n",
     "2016-04-01 00:20:42,3572.0,NIL,,,32.7428,NIL,,,nan,nan,nan,nan\n",
     '2016-04-01 00:30:00,nan,nan,nan,nan,nan,nan,nan,nan,29.3679,BAD,OTHER,"{""test"": ""flagZScore"", ""comment"": """"}"\n',
     "2016-04-01 00:35:37,3572.0,NIL,,,32.6186,NIL,,,nan,nan,nan,nan\n",
     "2016-04-01 00:45:00,nan,nan,nan,nan,nan,nan,nan,nan,29.3679,NIL,,\n",
@@ -81,9 +77,9 @@
         outfile,
         "--scheme",
         scheme,
     ]
     result = CliRunner().invoke(saqc.__main__.main, args)
     assert result.exit_code == 0, result.output
     with open(outfile, "r") as f:
-        result = f.readlines()[:10]
+        result = f.readlines()[:9]
         assert result == expected
```

### Comparing `saqc-2.5.0/tests/core/test_flags.py` & `saqc-2.5.0.post0.dev145/tests/core/test_flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         is_equal(copy, flags)
 
     assert deep is not shallow
     is_equal(deep, shallow)
 
     # the underling series data is the same
     for c in shallow.columns:
-        assert shallow._data[c].index is flags._data[c].index
+        assert shallow._data[c].index.equals(flags._data[c].index)
 
     # the underling series data was copied
     for c in deep.columns:
         assert deep._data[c].index is not flags._data[c].index
 
 
 @pytest.mark.parametrize("data", testdata)
@@ -192,14 +192,21 @@
         assert all(flags.history[c].squeeze() == 8888.0)
         assert all(flags.history[c].squeeze() == flags[c])
 
         # check if deep-copied correctly
         new[:] = 7777.0
         assert all(flags.history[c].squeeze() == 8888.0)
 
+        # check auto generated meta entries
+        assert flags.history[c].meta[0] == {
+            "func": "importedFlags",
+            "args": (),
+            "kwargs": {},
+        }
+
 
 @pytest.mark.parametrize("data", testdata)
 def test_set_flags_with_mask(
     data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]
 ):
     flags = Flags(data)
 
@@ -285,23 +292,14 @@
 
     for c in flags.columns:
         assert df[c].index.equals(flags[c].index)
         assert df[c].equals(flags[c])  # respects nan's
 
 
 @pytest.mark.parametrize("data", testdata)
-def test_to_dios(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
-    flags = Flags(data)
-    with pytest.deprecated_call():
-        result = flags.toDios()
-        assert isinstance(result, DictOfSeries)
-        _validate_flags_equals_frame(flags, result)
-
-
-@pytest.mark.parametrize("data", testdata)
 def test_toFrame(data: Union[pd.DataFrame, DictOfSeries, Dict[str, pd.Series]]):
     flags = Flags(data)
     df = flags.toFrame()
 
     assert isinstance(df, pd.DataFrame)
     _validate_flags_equals_frame(flags, df)
```

### Comparing `saqc-2.5.0/tests/core/test_history.py` & `saqc-2.5.0.post0.dev145/tests/core/test_history.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.api.types import is_categorical_dtype, is_float_dtype
 
-from saqc.core.history import History, createHistoryFromData
+from saqc.core.history import AGGREGATION, History, createHistoryFromData
 from tests.common import dummyHistory
 
 # see #GH143 combined backtrack
 # (adjusted to current implementation)
 example1 = (
     # flags
     np.array(
@@ -95,23 +95,23 @@
     """
     Check if two FH are (considered) equal, namely have equal 'hist'
     """
     return hist1.hist.equals(hist2.hist)
 
 
 @pytest.mark.parametrize("data", data + [None])
-def test_init(data: np.array):
+def test_init(data: np.ndarray):
     # init
     df = pd.DataFrame(data, dtype=float)
     hist = History(df.index)
     check_invariants(hist)
 
 
 @pytest.mark.parametrize("data", data + [None])
-def test_createHistory(data: np.array):
+def test_createHistory(data: np.ndarray):
     # init
     df = pd.DataFrame(data, dtype=float)
     meta = [{}] * len(df.columns)
     hist = createHistoryFromData(df, meta)
 
     check_invariants(hist)
 
@@ -139,15 +139,15 @@
         assert copy.meta is not hist.meta
         assert is_equal(copy, hist)
 
     assert deep is not shallow
     assert is_equal(deep, shallow)
 
     # underling pandas data was only copied with deep=True
-    assert shallow.hist.index is hist.hist.index
+    assert shallow.hist.index.equals(hist.hist.index)
     assert deep.hist.index is not hist.hist.index
 
 
 @pytest.mark.parametrize("copy", [True, False])
 @pytest.mark.parametrize("data", data + [None])
 def test_reindex_trivial_cases(data, copy):
     df = pd.DataFrame(data, dtype=float)
@@ -236,7 +236,29 @@
     ],
 )
 def test_append_force(__hist, s, max_val):
     hist = __hist
     hist.append(s)
     check_invariants(hist)
     assert all(hist.squeeze() == max_val)
+
+
+@pytest.mark.parametrize(
+    "col, expected",
+    [
+        (pd.Series(0, index=range(6), dtype=float), {"last": 0, "min": 0, "max": 0}),
+        (pd.Series(1, index=range(6), dtype=float), {"last": 1, "min": 0, "max": 1}),
+        (pd.Series(6, index=range(6), dtype=float), {"last": 6, "min": 0, "max": 6}),
+        (pd.Series(4, index=range(6), dtype=float), {"last": 4, "min": 0, "max": 6}),
+    ],
+)
+def test_aggregations(col, expected, hist=History(index=pd.Index(range(6)))):
+    import saqc.core.history
+
+    hist.append(col)
+    check_invariants(hist)
+    for aggregation in ["last", "min", "max"]:
+        saqc.core.history.AGGREGATION = aggregation
+        assert (hist.squeeze() == expected[aggregation]).all()
+
+    # reset to not disturb the other tests...
+    saqc.core.history.AGGREGATION = "last"
```

### Comparing `saqc-2.5.0/tests/core/test_reader.py` & `saqc-2.5.0.post0.dev145/tests/core/test_reader.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/core/test_translator.py` & `saqc-2.5.0.post0.dev145/tests/core/test_translator.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import json
 from typing import Dict, Sequence, Union
 
 import numpy as np
 import pandas as pd
 import pytest
 
-from saqc import BAD, DOUBTFUL, FILTER_NONE, UNFLAGGED, SaQC
-from saqc.core import Flags
+from saqc.constants import BAD, DOUBTFUL, FILTER_NONE, UNFLAGGED
+from saqc.core import Flags, SaQC
 from saqc.core.translation import DmpScheme, MappingScheme, PositionalScheme
+from saqc.core.translation.floatscheme import AnnotatedFloatScheme
 from tests.common import initData
 
 
 def _genTranslators():
     for dtype in (str, float, int):
         flags = {
             dtype(-2): UNFLAGGED,
@@ -89,46 +90,45 @@
     history2 = flags.history["var2"]
     history2.meta[-1].update(
         {"func": "flagFoo", "kwargs": {"cause": "BELOW_OR_ABOVE_MIN_MAX"}}
     )
 
     tflags = scheme.toExternal(flags)
 
-    assert set(tflags.columns.get_level_values(1)) == {
-        "quality_flag",
-        "quality_comment",
-        "quality_cause",
-    }
+    for df in tflags.values():
+        assert set(df.columns) == {
+            "quality_flag",
+            "quality_comment",
+            "quality_cause",
+        }
 
-    assert (tflags.loc[:, ("var1", "quality_flag")] == "DOUBTFUL").all(axis=None)
+    assert (tflags["var1"]["quality_flag"] == "DOUBTFUL").all(axis=None)
     assert (
-        tflags.loc[:, ("var1", "quality_comment")]
+        tflags["var1"]["quality_comment"]
         == '{"test": "flagBar", "comment": "I did it"}'
     ).all(axis=None)
 
-    assert (tflags.loc[:, ("var1", "quality_cause")] == "OTHER").all(axis=None)
+    assert (tflags["var1"]["quality_cause"] == "OTHER").all(axis=None)
 
-    assert (tflags.loc[:, ("var2", "quality_flag")] == "BAD").all(axis=None)
+    assert (tflags["var2"]["quality_flag"] == "BAD").all(axis=None)
     assert (
-        tflags.loc[:, ("var2", "quality_comment")]
-        == '{"test": "flagFoo", "comment": ""}'
+        tflags["var2"]["quality_comment"] == '{"test": "flagFoo", "comment": ""}'
     ).all(axis=None)
-    assert (tflags.loc[:, ("var2", "quality_cause")] == "BELOW_OR_ABOVE_MIN_MAX").all(
-        axis=None
-    )
+    assert (tflags["var2"]["quality_cause"] == "BELOW_OR_ABOVE_MIN_MAX").all(axis=None)
 
     assert (
-        tflags.loc[flags["var3"] == BAD, ("var3", "quality_comment")]
+        tflags["var3"].loc[flags["var3"] == BAD, "quality_comment"]
         == '{"test": "unknown", "comment": ""}'
     ).all(axis=None)
-    assert (tflags.loc[flags["var3"] == BAD, ("var3", "quality_cause")] == "OTHER").all(
+    assert (tflags["var3"].loc[flags["var3"] == BAD, "quality_cause"] == "OTHER").all(
+        axis=None
+    )
+    assert (tflags["var3"].loc[flags["var3"] == UNFLAGGED, "quality_cause"] == "").all(
         axis=None
     )
-    mask = flags["var3"] == UNFLAGGED
-    assert (tflags.loc[mask, ("var3", "quality_cause")] == "").all(axis=None)
 
 
 def test_positionalTranslator():
     scheme = PositionalScheme()
     flags = _genFlags({"var1": np.zeros(100), "var2": np.zeros(50)})
     flags[1::3, "var1"] = BAD
     flags[1::3, "var1"] = DOUBTFUL
@@ -150,48 +150,51 @@
     flags = saqc.flags
 
     for field in flags.keys():
         assert flags[field].astype(str).str.match("^9[012]*$").all()
 
     round_trip = scheme.toExternal(scheme.toInternal(flags))
 
-    assert (flags.values == round_trip.values).all()
-    assert (flags.index == round_trip.index).all()
     assert (flags.columns == round_trip.columns).all()
+    for col in flags.columns:
+        assert (flags[col] == round_trip[col]).all()
+        assert (flags[col].index == round_trip[col].index).all()
 
 
 def test_dmpTranslatorIntegration():
     data = initData(1)
     col = data.columns[0]
 
     scheme = DmpScheme()
     saqc = SaQC(data=data, scheme=scheme)
     saqc = saqc.flagMissing(col).flagRange(col, min=3, max=10)
     flags = saqc.flags
 
-    qflags = flags.xs("quality_flag", axis="columns", level=1)
-    qfunc = flags.xs("quality_comment", axis="columns", level=1).map(
-        lambda v: json.loads(v)["test"] if v else ""
-    )
-    qcause = flags.xs("quality_cause", axis="columns", level=1)
+    qflags = pd.DataFrame({k: v["quality_flag"] for k, v in flags.items()})
+    qfunc = pd.DataFrame({k: v["quality_comment"] for k, v in flags.items()})
+    qcause = pd.DataFrame({k: v["quality_cause"] for k, v in flags.items()})
 
     assert qflags.isin(scheme._forward.keys()).all(axis=None)
-    assert qfunc.isin({"", "flagMissing", "flagRange"}).all(axis=None)
+    assert (
+        qfunc.map(lambda v: json.loads(v)["test"] if v else "")
+        .isin({"", "flagMissing", "flagRange"})
+        .all(axis=None)
+    )
     assert (qcause[qflags[col] == "BAD"] == "OTHER").all(axis=None)
 
     round_trip = scheme.toExternal(scheme.toInternal(flags))
 
-    assert round_trip.xs("quality_flag", axis="columns", level=1).equals(qflags)
-
-    assert round_trip.xs("quality_comment", axis="columns", level=1).equals(
-        flags.xs("quality_comment", axis="columns", level=1)
+    assert pd.DataFrame({k: v["quality_flag"] for k, v in round_trip.items()}).equals(
+        qflags
     )
-
-    assert round_trip.xs("quality_cause", axis="columns", level=1).equals(
-        flags.xs("quality_cause", axis="columns", level=1)
+    assert pd.DataFrame(
+        {k: v["quality_comment"] for k, v in round_trip.items()}
+    ).equals(qfunc)
+    assert pd.DataFrame({k: v["quality_cause"] for k, v in round_trip.items()}).equals(
+        qcause
     )
 
 
 def test_dmpValidCombinations():
     data = initData(1)
     col = data.columns[0]
 
@@ -271,7 +274,27 @@
     tflags1 = scheme.toExternal(flags1).astype(str)
     tflags2 = scheme.toExternal(flags2).astype(str)
 
     for k in flags2.columns:
         expected = tflags1[k].str.slice(start=1) * 2
         got = tflags2[k].str.slice(start=1)
         assert expected.equals(got)
+
+
+def test_annotatedFloatScheme():
+    data = initData(1)
+    col = data.columns[0]
+
+    scheme = AnnotatedFloatScheme()
+    saqc = SaQC(data=data, scheme=scheme)
+    saqc = saqc.setFlags(col, data=data[col].index[::4], flag=DOUBTFUL).flagRange(
+        col, min=3, max=10, flag=BAD
+    )
+    flags = saqc.flags
+
+    assert flags[col]["flag"].isin({DOUBTFUL, BAD, UNFLAGGED}).all(axis=None)
+    assert flags[col]["func"].isin({"", "setFlags", "flagRange"}).all(axis=None)
+
+    round_trip = scheme.toExternal(scheme.toInternal(flags))
+    assert tuple(round_trip.keys()) == tuple(flags.keys())
+    for key in flags.keys():
+        assert round_trip[key].equals(flags[key])
```

### Comparing `saqc-2.5.0/tests/funcs/test_constants_detection.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_constants_detection.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/funcs/test_functions.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     data = pd.Series(0, index=pd.date_range("2000", "2001", freq="1D"), name="data")
     noise = [-1, 1] * 10
     data[100:120] = noise
     data[200:210] = noise[:10]
     data = DictOfSeries(data=data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagByScatterLowpass(
-        "data", "20D", 0.999, "std", "5D", 0.999, 0, flag=BAD
+        "data", "20D", 0.999, np.std, "5D", 0.999, 0, flag=BAD
     )
     assert (qc.flags["data"].iloc[:100] == UNFLAGGED).all()
     assert (qc.flags["data"].iloc[100:120] == BAD).all()
     assert (qc.flags["data"].iloc[121:] == UNFLAGGED).all()
 
 
 def test_flagRange(data, field):
@@ -48,15 +48,15 @@
     qc = SaQC(data, flags)
     qc = qc.flagRange(field, min=min, max=max, flag=BAD)
     flagged = qc.flags[field] > UNFLAGGED
     expected = (data[field] < min) | (data[field] > max)
     assert all(flagged == expected)
 
 
-def test_flagSeasonalRange(data, field):
+def test_selectTime(data, field):
     data[field].iloc[::2] = 0
     data[field].iloc[1::2] = 50
     nyears = len(data[field].index.year.unique())
 
     tests = [
         (
             {
@@ -175,27 +175,29 @@
     kwargs_list = [
         dict(mdata=mdata, mflag="a", method="plain", mformat="mflag", flag=BAD),
         dict(mdata=mdata, mflag="a", method="ontime", mformat="mflag", flag=BAD),
         dict(mdata=shrinked, mflag="a", method="ontime", mformat="mflag", flag=BAD),
     ]
 
     for kw in kwargs_list:
-        qc = SaQC(data, flags).flagManual(field, **kw)
+        with pytest.deprecated_call():
+            qc = SaQC(data, flags).flagManual(field, **kw)
         isflagged = qc._flags[field] > UNFLAGGED
         assert isflagged[isflagged].index.equals(index_exp)
 
     # flag not exist in mdata
-    qc = SaQC(data, flags).flagManual(
-        field,
-        mdata=mdata,
-        mflag="i do not exist",
-        method="ontime",
-        mformat="mflag",
-        flag=BAD,
-    )
+    with pytest.deprecated_call():
+        qc = SaQC(data, flags).flagManual(
+            field,
+            mdata=mdata,
+            mflag="i do not exist",
+            method="ontime",
+            mformat="mflag",
+            flag=BAD,
+        )
     isflagged = qc._flags[field] > UNFLAGGED
     assert isflagged[isflagged].index.equals(pd.DatetimeIndex([]))
 
     # check closure methods
     index = pd.date_range(start="2016-01-01", end="2018-12-31", periods=11)
     mdata = pd.Series(0, index=index)
     mdata.loc[index[[1, 5, 6, 7, 9, 10]]] = 1
@@ -216,57 +218,56 @@
     flag_intervals = [
         (m_index[1], m_index[2]),
         (m_index[5], m_index[8]),
         (m_index[9], dat.index.shift(freq="1h")[-1]),
     ]
     bound_drops = {"right-open": [1], "left-open": [0], "closed": []}
     for method in ["right-open", "left-open", "closed"]:
-        qc = qc.flagManual(
-            field,
-            mdata=mdata,
-            mflag=1,
-            method=method,
-            mformat="mflag",
-            flag=BAD,
-        )
+        with pytest.deprecated_call():
+            qc = qc.flagManual(
+                field,
+                mdata=mdata,
+                mflag=1,
+                method=method,
+                mformat="mflag",
+                flag=BAD,
+            )
         isflagged = qc._flags[field] > UNFLAGGED
         for flag_i in flag_intervals:
             f_i = isflagged[slice(flag_i[0], flag_i[-1])].index
             check_i = f_i.drop(
                 [flag_i[k] for k in bound_drops[method]], errors="ignore"
             )
             assert isflagged[check_i].all()
             unflagged = isflagged[f_i.difference(check_i)]
             if not unflagged.empty:
                 assert ~unflagged.all()
 
 
-@pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_1")])
-def test_flagDriftFromNorm(dat):
-    data = dat(periods=200, peak_level=5, name="field1")[0]
-    data["field2"] = dat(periods=200, peak_level=10, name="field2")[0]["field2"]
-    data["field3"] = dat(periods=200, peak_level=100, name="field3")[0]["field3"]
+def test_flagDriftFromNorm(course_1):
+    data = course_1(periods=200, peak_level=5, name="field1")[0]
+    data["field2"] = course_1(periods=200, peak_level=10, name="field2")[0]["field2"]
+    data["field3"] = course_1(periods=200, peak_level=100, name="field3")[0]["field3"]
 
     fields = ["field1", "field2", "field3"]
 
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagDriftFromNorm(
         field=fields,
         window="200min",
         spread=5,
         flag=BAD,
     )
     assert all(qc._flags["field3"] > UNFLAGGED)
 
 
-@pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_1")])
-def test_flagDriftFromReference(dat):
-    data = dat(periods=200, peak_level=5, name="field1")[0]
-    data["field2"] = dat(periods=200, peak_level=10, name="field2")[0]["field2"]
-    data["field3"] = dat(periods=200, peak_level=100, name="field3")[0]["field3"]
+def test_flagDriftFromReference(course_1):
+    data = course_1(periods=200, peak_level=5, name="field1")[0]
+    data["field2"] = course_1(periods=200, peak_level=10, name="field2")[0]["field2"]
+    data["field3"] = course_1(periods=200, peak_level=100, name="field3")[0]["field3"]
 
     fields = ["field1", "field2", "field3"]
 
     flags = initFlagsLike(data)
 
     qc = SaQC(data, flags).flagDriftFromReference(
         field=fields,
```

### Comparing `saqc-2.5.0/tests/funcs/test_generic_api_functions.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_generic_api_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "targets, func",
     [
         (["tmp"], lambda x, y: pd.Series(True, index=x.index.union(y.index))),
         (
             ["tmp1", "tmp2"],
             lambda x, y: [pd.Series(True, index=x.index.union(y.index))] * 2,
         ),
+        (["tmp1", "tmp2"], lambda x, y: pd.Series(True, index=x.index.union(y.index))),
     ],
 )
 def test_writeTargetFlagGeneric(data, targets, func):
     saqc = SaQC(data=data)
     saqc = saqc.flagGeneric(field=data.columns, target=targets, func=func, flag=BAD)
     for target in targets:
         assert saqc._flags.history[target].hist.iloc[0].tolist() == [BAD]
@@ -76,15 +77,19 @@
     )
 
     res = saqc.flagGeneric(field=fields, func=func, flag=flag, dfilter=FILTER_NONE)
     for field in fields:
         histcol1 = res._flags.history[field].hist[1]
         assert (histcol1 == flag).all()
         assert (data[field] == res.data[field]).all(axis=None)
-        assert res._flags.history[field].meta[0] == {}
+        assert res._flags.history[field].meta[0] == {
+            "args": (),
+            "func": "importedFlags",
+            "kwargs": {},
+        }
 
 
 @pytest.mark.parametrize(
     "data, targets, func, expected_data",
     [
         (
             DictOfSeries(dict(a=pd.Series([1.0, 2.0]), b=pd.Series([10.0, 20.0]))),
@@ -161,15 +166,19 @@
 
     res = saqc.processGeneric(field=fields, func=func, dfilter=dfilter, label="generic")
     assert expected_data == res.data
     # check that the histories got appended
     for field in fields:
         assert (res._flags.history[field].hist[0] == 127.0).all()
         assert res._flags.history[field].hist[1].isna().all()
-        assert res._flags.history[field].meta[0] == {}
+        assert res._flags.history[field].meta[0] == {
+            "args": (),
+            "func": "importedFlags",
+            "kwargs": {},
+        }
 
 
 def test_label():
     dat = pd.DataFrame(
         {"data1": [1, 1, 5, 2, 1], "data2": [1, 1, 2, 3, 4], "data3": [1, 1, 2, 3, 4]},
         index=pd.date_range("2000", "2005", periods=5),
     )
```

### Comparing `saqc-2.5.0/tests/funcs/test_generic_config_functions.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_generic_config_functions.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/funcs/test_outlier_detection.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_outlier_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 def test_flagMad(spiky_data):
     data = spiky_data[0]
     field, *_ = data.columns
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagZScore(
-        field, window="1H", method="modified", thresh=3.5, flag=BAD
+        field, window="1h", method="modified", thresh=3.5, flag=BAD
     )
     flag_result = qc.flags[field]
     test_sum = (flag_result.iloc[spiky_data[1]] == BAD).sum()
     assert test_sum == len(spiky_data[1])
 
 
 def test_flagSpikesBasic(spiky_data):
@@ -48,26 +48,19 @@
         field, thresh=60, tolerance=10, window="20min", flag=BAD
     )
     flag_result = qc.flags[field]
     test_sum = (flag_result.iloc[spiky_data[1]] == BAD).sum()
     assert test_sum == len(spiky_data[1])
 
 
+@pytest.mark.filterwarnings("ignore::DeprecationWarning")
 @pytest.mark.slow
-@pytest.mark.parametrize(
-    "dat",
-    [
-        # see test/functs/fixtures.py for the 'course_N'
-        pytest.lazy_fixture("course_1"),
-        pytest.lazy_fixture("course_2"),
-        pytest.lazy_fixture("course_3"),
-        pytest.lazy_fixture("course_4"),
-    ],
-)
-def test_flagSpikesLimitRaise(dat):
+@pytest.mark.parametrize("dat", ["course_1", "course_2", "course_3", "course_4"])
+def test_flagSpikesLimitRaise(dat, request):
+    dat = request.getfixturevalue(dat)
     data, characteristics = dat()
     field, *_ = data.columns
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagRaise(
         field,
         thresh=2,
         freq="10min",
@@ -76,67 +69,68 @@
     )
     assert np.all(qc.flags[field][characteristics["raise"]] > UNFLAGGED)
     assert not np.any(qc.flags[field][characteristics["return"]] > UNFLAGGED)
     assert not np.any(qc.flags[field][characteristics["drop"]] > UNFLAGGED)
 
 
 # see test/functs/fixtures.py for the 'course_N'
-@pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_3")])
-def test_flagMVScores(dat):
+def test_flagMVScores(course_3):
     def _check(fields, flags, characteristics):
         for field in fields:
             isflagged = flags[field] > UNFLAGGED
             assert isflagged[characteristics["raise"]].all()
             assert not isflagged[characteristics["return"]].any()
             assert not isflagged[characteristics["drop"]].any()
 
-    data1, characteristics = dat(
+    data1, characteristics = course_3(
         periods=1000, initial_level=5, final_level=15, out_val=50
     )
-    data2, characteristics = dat(
+    data2, characteristics = course_3(
         periods=1000, initial_level=20, final_level=1, out_val=30
     )
     fields = ["field1", "field2"]
     s1, s2 = data1["data"], data2["data"]
     s1 = pd.Series(data=s1.values, index=s1.index)
     s2 = pd.Series(data=s2.values, index=s1.index)
     data = DictOfSeries(field1=s1, field2=s2)
     flags = initFlagsLike(data)
-    qc = SaQC(data, flags).flagMVScores(
-        field=fields,
-        trafo=np.log,
-        iter_start=0.95,
-        n=10,
-        flag=BAD,
-    )
+    qc = SaQC(data, flags)
+    qc = qc.processGeneric("field1", func=lambda x: np.log(x))
+    qc = qc.processGeneric("field2", func=lambda x: np.log(x))
+    qc = qc.assignKNNScore(
+        ["field1", "field2"],
+        target="kNNScores",
+    )
+    qc = qc.flagByStray("kNNScores", iter_start=0.95)
+    qc = qc.transferFlags("kNNScores", target="field1")
+    qc = qc.transferFlags("kNNScores", target="field2")
+
     _check(fields, qc.flags, characteristics)
 
 
-@pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_3")])
-def test_grubbs(dat):
-    data, char_dict = dat(
+def test_grubbs(course_3):
+    data, char_dict = course_3(
         freq="10min",
         periods=45,
         initial_level=0,
         final_level=0,
         crowd_size=1,
         crowd_spacing=3,
         out_val=-10,
     )
     flags = initFlagsLike(data)
-    qc = SaQC(data, flags).flagByGrubbs("data", window=20, min_periods=15, flag=BAD)
+    qc = SaQC(data, flags).flagUniLOF("data", density=0.4)
     assert np.all(qc.flags["data"][char_dict["drop"]] > UNFLAGGED)
 
 
-@pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_2")])
 @pytest.mark.parametrize(
     "parameters",
     [("standard", 1), ("modified", 1), ("modified", 3), ("standard", "3h")],
 )
-def test_flagCrossStatistics(dat, parameters):
+def test_flagCrossStatistics(parameters):
     fields = [f"data{i}" for i in range(6)]
     data = pd.DataFrame(
         0, columns=fields, index=pd.date_range("2000", freq="1h", periods=10)
     )
     bad_idx = (np.random.randint(0, 10), np.random.randint(0, 6))
     data.iloc[bad_idx[0], bad_idx[1]] = 10
     flags = initFlagsLike(data)
```

### Comparing `saqc-2.5.0/tests/funcs/test_pattern_rec.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_pattern_rec.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/funcs/test_proc_functions.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_proc_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,38 +41,14 @@
         center=False,
         min_periods=3,
         interpol_flag=UNFLAGGED,
     )
     assert qc.data[field][characteristics["missing"]].isna().all()
 
 
-def test_interpolate(course_5):
-    data, characteristics = course_5(periods=10, nan_slice=[5])
-    field = data.columns[0]
-    data = DictOfSeries(data)
-    flags = initFlagsLike(data)
-    qc = SaQC(data, flags)
-
-    qc_lin = qc.interpolate(field, method="linear")
-    qc_poly = qc.interpolate(field, method="polynomial")
-    assert qc_lin.data[field][characteristics["missing"]].notna().all()
-    assert qc_poly.data[field][characteristics["missing"]].notna().all()
-
-    data, characteristics = course_5(periods=10, nan_slice=[5, 6, 7])
-
-    qc = SaQC(data, flags)
-    qc_lin_1 = qc.interpolate(field, method="linear", limit=2)
-    qc_lin_2 = qc.interpolate(field, method="linear", limit=3)
-    qc_lin_3 = qc.interpolate(field, method="linear", limit=4)
-
-    assert qc_lin_1.data[field][characteristics["missing"]].isna().all()
-    assert qc_lin_2.data[field][characteristics["missing"]].isna().all()
-    assert qc_lin_3.data[field][characteristics["missing"]].notna().all()
-
-
 def test_transform(course_5):
     data, characteristics = course_5(periods=10, nan_slice=[5, 6])
     field = data.columns[0]
     data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags)
 
@@ -93,29 +69,29 @@
     data, _ = course_5(freq="1min", periods=30, nan_slice=[1, 11, 12, 22, 24, 26])
     field = data.columns[0]
     data = DictOfSeries(data)
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).resample(
         field,
         "10min",
-        np.mean,
+        "mean",
         maxna=2,
         maxna_group=1,
     )
     assert ~np.isnan(qc.data[field].iloc[0])
     assert np.isnan(qc.data[field].iloc[1])
     assert np.isnan(qc.data[field].iloc[2])
 
 
 def test_interpolateGrid(course_5, course_3):
     data, _ = course_5()
     data_grid, _ = course_3()
     data["grid"] = data_grid["data"]
     flags = initFlagsLike(data)
-    SaQC(data, flags).align("data", "1h", "time", grid_field="grid", limit=10)
+    SaQC(data, flags).align("data", "1h", "time")
 
 
 @pytest.mark.slow
 def test_offsetCorrecture():
     data = pd.Series(0, index=pd.date_range("2000", freq="1d", periods=100), name="dat")
     data.iloc[30:40] = -100
     data.iloc[70:80] = 100
```

### Comparing `saqc-2.5.0/tests/funcs/test_tools.py` & `saqc-2.5.0.post0.dev145/tests/funcs/test_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,29 @@
         .flagRange("data", max=300)
     )
 
     # not interactive, no storing
     outfile = str(Path(tmp_path, "test.png"))  # the filesystem's temp dir
 
     d_saqc = d_saqc.plot(field="data", path=outfile)
-    d_saqc = d_saqc.plot(field="data", path=outfile, history="valid", stats=True)
-    with pytest.deprecated_call():
-        d_saqc = d_saqc.plot(field="data", path=outfile, history="complete")
+    d_saqc = d_saqc.plot(
+        field="data", path=outfile, history="valid", yscope=[(-50, 1000)]
+    )
 
     d_saqc = d_saqc.plot(
-        field="data", path=outfile, ax_kwargs={"ylabel": "data is data"}, stats=True
+        field="data",
+        path=outfile,
+        ax_kwargs={"ylabel": "data is data"},
+        yscope=(100, 150),
+    )
+
+
+@pytest.mark.filterwarnings("ignore::UserWarning")
+def test_flagByClick():
+    saqc.funcs.tools._TEST_MODE = True
+    data = pd.DataFrame(
+        {f"d{k}": np.random.randint(0, 100, 100) for k in range(10)},
+        index=pd.date_range("2000", freq="1d", periods=100),
     )
+    qc = saqc.SaQC(data)
+    qc = qc.flagByClick(data.columns, gui_mode="overlay")
+    qc = qc.flagByClick(data.columns)
```

### Comparing `saqc-2.5.0/tests/fuzzy/lib.py` & `saqc-2.5.0.post0.dev145/tests/fuzzy/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,21 +100,21 @@
 
 @composite
 def daterangeIndexes(draw, min_size=0, max_size=100):
     min_date = pd.Timestamp("1900-01-01").to_pydatetime()
     max_date = pd.Timestamp("2099-12-31").to_pydatetime()
     start = draw(datetimes(min_value=min_date, max_value=max_date))
     periods = draw(integers(min_value=min_size, max_value=max_size))
-    freq = draw(sampled_from(["D", "H", "T", "min", "S", "L", "ms", "U", "us", "N"]))
+    freq = draw(sampled_from(["D", "h", "min", "s", "ms", "us", "ns"]))
     return pd.date_range(start, periods=periods, freq=freq)
 
 
 @composite
 def frequencyStrings(draw, _):
-    freq = draw(sampled_from(["D", "H", "T", "min", "S", "L", "ms", "U", "us", "N"]))
+    freq = draw(sampled_from(["D", "h", "min", "s", "ms", "us", "ns"]))
     mult = draw(integers(min_value=1, max_value=10))
     value = f"{mult}{freq}"
     return value
 
 
 @composite
 def dataFieldFlags(draw):
```

### Comparing `saqc-2.5.0/tests/fuzzy/test_masking.py` & `saqc-2.5.0.post0.dev145/tests/fuzzy/test_masking.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/lib/test_periodicMask.py` & `saqc-2.5.0.post0.dev145/tests/lib/test_periodicMask.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/lib/test_tools.py` & `saqc-2.5.0.post0.dev145/tests/lib/test_tools.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/lib/test_ts_operators.py` & `saqc-2.5.0.post0.dev145/tests/lib/test_ts_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,7 +250,24 @@
     ],
 )
 def test_interpolatNANs(limit, extrapolate, data, expected):
     got = tsops.interpolateNANs(
         pd.Series(data), gap_limit=limit, method="linear", extrapolate=extrapolate
     )
     assert got.equals(pd.Series(expected, dtype=float))
+
+
+@pytest.mark.parametrize(
+    "func,expected",
+    [
+        (tsops.trueDailyMean, [71.0, 212.0, np.nan, np.nan]),
+        (tsops.climatologicalMean, [np.nan, 312.0]),
+    ],
+)
+def test_wmoFuncs(func, expected):
+    data = pd.Series(
+        np.arange(288), index=pd.date_range("2000", freq="10min", periods=288)
+    )
+    data["2000-01-01 06:30:00"] = np.nan
+    data.iloc[150:154] = np.nan
+    m = func(data)
+    assert ((m.values == expected) | m.isna()).all()
```

### Comparing `saqc-2.5.0/tests/misc/test_pickle.py` & `saqc-2.5.0.post0.dev145/tests/misc/test_pickle.py`

 * *Files identical despite different names*

### Comparing `saqc-2.5.0/tests/test__main__.py` & `saqc-2.5.0.post0.dev145/tests/test__main__.py`

 * *Files identical despite different names*

