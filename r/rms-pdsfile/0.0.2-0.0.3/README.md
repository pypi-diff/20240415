# Comparing `tmp/rms-pdsfile-0.0.2.tar.gz` & `tmp/rms_pdsfile-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-pdsfile-0.0.2.tar", last modified: Thu Apr 11 22:19:12 2024, max compression
+gzip compressed data, was "rms_pdsfile-0.0.3.tar", last modified: Mon Apr 15 21:40:13 2024, max compression
```

## Comparing `rms-pdsfile-0.0.2.tar` & `rms_pdsfile-0.0.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/run-tests-and-opus.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.082759 rms-pdsfile-0.0.2/pdsfile/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 22:19:11.000000 rms-pdsfile-0.0.2/pdsfile/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.082759 rms-pdsfile-0.0.2/pdsfile/pds3file/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.086759 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/ASTROM_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COCIRS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/CORSS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/EBROCC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/GO_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/HSTxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJIR_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJNC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHxxxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RES_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RPX_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGIRIS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_20xx.py
--rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_28xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/rules/pytest_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.086759 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/
--rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23585 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24720 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/pytest_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57915 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased.py
--rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    33847 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pds4file/tests/test_pds4file_blackbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdscache.py
--rw-r--r--   0 runner    (1001) docker     (127)   230846 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdsfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/pdsviewable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pdsfile/preload_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 22:19:12.000000 rms-pdsfile-0.0.2/rms_pdsfile.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/run_tests_coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.078759 rms-pdsfile-0.0.2/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.090759 rms-pdsfile-0.0.2/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/scripts/automated_tests/pdsfile_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:12.094759 rms-pdsfile-0.0.2/validation/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsarchives.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdschecksums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsdata-sync.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsdependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsindexshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdsinfoshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/pdslinkshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/re-validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-11 22:19:05.000000 rms-pdsfile-0.0.2/validation/shelf-consistency-check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.479827 rms_pdsfile-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/run-tests-and-opus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/pdsfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/pdsfile/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/pdsfile/pds3file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.487827 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/ASTROM_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COCIRS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/CORSS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/EBROCC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/GO_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/HSTxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJIR_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJNC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHxxxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RES_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RPX_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGIRIS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_20xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_28xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/pytest_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23585 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24720 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/pytest_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57915 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33847 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/test_pds4file_blackbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230951 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdsfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdsviewable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/preload_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/run_tests_coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.479827 rms_pdsfile-0.0.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/scripts/automated_tests/pdsfile_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/validation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsarchives.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdschecksums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsdata-sync.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsdependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsindexshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsinfoshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdslinkshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/re-validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/shelf-consistency-check.py
```

### Comparing `rms-pdsfile-0.0.2/.github/workflows/publish_to_pypi.yml` & `rms_pdsfile-0.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/.github/workflows/publish_to_test_pypi.yml` & `rms_pdsfile-0.0.3/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/.github/workflows/run-tests-and-opus.yml` & `rms_pdsfile-0.0.3/.github/workflows/run-tests-and-opus.yml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/.github/workflows/run-tests.yml` & `rms_pdsfile-0.0.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/.gitignore` & `rms_pdsfile-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/CODE_OF_CONDUCT.md` & `rms_pdsfile-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/CONTRIBUTING.md` & `rms_pdsfile-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/LICENSE` & `rms_pdsfile-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/PKG-INFO` & `rms_pdsfile-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.2
+Version: 0.0.3
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms-pdsfile-0.0.2/README.md` & `rms_pdsfile-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/conftest.py` & `rms_pdsfile-0.0.3/conftest.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/__init__.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/ASTROM_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/ASTROM_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COCIRS_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COCIRS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COISS_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/CORSS_8xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/CORSS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COSP_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_0xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COUVIS_8xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_0xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/COVIMS_8xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/EBROCC_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/EBROCC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/GO_0xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/GO_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/HSTxx_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/HSTxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJIR_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJIR_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOJNC_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJNC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/JNOSP_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHSP_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/NHxxxx_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHxxxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RES_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RES_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/RPX_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RPX_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGIRIS_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGIRIS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VGISS_xxxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_0xxx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_20xx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_20xx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/VG_28xx.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_28xx.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/__init__.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/rules/pytest_support.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/helper.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pds3file_whitebox.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_whitebox.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py` & `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/__init__.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/__init__.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_iss.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_iss.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/cassini_vims.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_vims.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/pytest_support.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/tests/helper.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pds4file/tests/test_pds4file_blackbox.py` & `rms_pdsfile-0.0.3/pdsfile/pds4file/tests/test_pds4file_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pdscache.py` & `rms_pdsfile-0.0.3/pdsfile/pdscache.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/pdsfile.py` & `rms_pdsfile-0.0.3/pdsfile/pdsfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,15 +982,17 @@
                     cls.LOGGER.info('Pre-load not needed for ' + holdings)
                     continue
 
                 cls.LOCAL_PRELOADED.append(holdings)
                 cls.LOGGER.info('Pre-loading ' + holdings)
 
                 # Load volume info
-                cls.load_volume_info(holdings)
+                # PDS4 will ignore _volinfo directory
+                if cls.__name__ != 'Pds4File':
+                    cls.load_volume_info(holdings)
 
                 # Load directories starting from here
                 holdings_ = holdings.rstrip('/') + '/'
 
                 for c in cls.CATEGORY_LIST:
                     category_abspath = holdings_ + c
                     if not cls.os_path_exists(category_abspath):
```

### Comparing `rms-pdsfile-0.0.2/pdsfile/pdsviewable.py` & `rms_pdsfile-0.0.3/pdsfile/pdsviewable.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pdsfile/preload_and_cache.py` & `rms_pdsfile-0.0.3/pdsfile/preload_and_cache.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/pyproject.toml` & `rms_pdsfile-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/rms_pdsfile.egg-info/PKG-INFO` & `rms_pdsfile-0.0.3/rms_pdsfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.2
+Version: 0.0.3
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms-pdsfile-0.0.2/rms_pdsfile.egg-info/SOURCES.txt` & `rms_pdsfile-0.0.3/rms_pdsfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/run_tests_coverage.sh` & `rms_pdsfile-0.0.3/run_tests_coverage.sh`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/scripts/automated_tests/pdsfile_main_test.sh` & `rms_pdsfile-0.0.3/scripts/automated_tests/pdsfile_main_test.sh`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdsarchives.py` & `rms_pdsfile-0.0.3/validation/pdsarchives.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdschecksums.py` & `rms_pdsfile-0.0.3/validation/pdschecksums.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdsdata-sync.sh` & `rms_pdsfile-0.0.3/validation/pdsdata-sync.sh`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdsdependency.py` & `rms_pdsfile-0.0.3/validation/pdsdependency.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdsindexshelf.py` & `rms_pdsfile-0.0.3/validation/pdsindexshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdsinfoshelf.py` & `rms_pdsfile-0.0.3/validation/pdsinfoshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/pdslinkshelf.py` & `rms_pdsfile-0.0.3/validation/pdslinkshelf.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/re-validate.py` & `rms_pdsfile-0.0.3/validation/re-validate.py`

 * *Files identical despite different names*

### Comparing `rms-pdsfile-0.0.2/validation/shelf-consistency-check.py` & `rms_pdsfile-0.0.3/validation/shelf-consistency-check.py`

 * *Files identical despite different names*

