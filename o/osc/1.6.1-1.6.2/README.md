# Comparing `tmp/osc-1.6.1.tar.gz` & `tmp/osc-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-1.6.1.tar", last modified: Fri Feb 23 08:54:22 2024, max compression
+gzip compressed data, was "osc-1.6.2.tar", last modified: Mon Apr 15 08:44:08 2024, max compression
```

## Comparing `osc-1.6.1.tar` & `osc-1.6.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.251885 osc-1.6.1/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      481 2023-11-02 14:00:00.000000 osc-1.6.1/AUTHORS
--rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-11-02 14:00:00.000000 osc-1.6.1/COPYING
--rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-11-02 14:00:00.000000 osc-1.6.1/MANIFEST.in
--rw-r--r--   0 dmach     (1000) dmach     (1000)    17496 2024-02-23 08:37:31.000000 osc-1.6.1/NEWS
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1573 2024-02-23 08:54:22.251885 osc-1.6.1/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-11-02 14:00:00.000000 osc-1.6.1/README.md
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.235219 osc-1.6.1/osc/
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13384 2024-01-25 08:32:55.000000 osc-1.6.1/osc/OscConfigParser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2024-02-23 08:13:32.000000 osc-1.6.1/osc/__init__.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.238552 osc-1.6.1/osc/_private/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6142 2024-02-23 08:12:59.000000 osc-1.6.1/osc/_private/api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/api_build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/api_configuration.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/api_source.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1949 2023-11-22 07:48:32.000000 osc-1.6.1/osc/_private/common.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5725 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/project.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-11-02 14:00:00.000000 osc-1.6.1/osc/_private/request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8506 2024-02-23 08:12:59.000000 osc-1.6.1/osc/babysitter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    64709 2024-02-23 08:12:59.000000 osc-1.6.1/osc/build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3205 2024-01-25 08:32:55.000000 osc-1.6.1/osc/checker.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10119 2024-01-25 08:32:55.000000 osc-1.6.1/osc/cmdln.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   444180 2024-02-23 08:12:59.000000 osc-1.6.1/osc/commandline.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.238552 osc-1.6.1/osc/commands/
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-11-02 14:00:00.000000 osc-1.6.1/osc/commands/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      185 2023-11-02 14:00:00.000000 osc-1.6.1/osc/commands/repo.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2518 2023-11-02 14:00:00.000000 osc-1.6.1/osc/commands/repo_add.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1781 2023-11-02 14:00:00.000000 osc-1.6.1/osc/commands/repo_list.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1569 2023-11-02 14:00:00.000000 osc-1.6.1/osc/commands/repo_remove.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    70230 2024-02-23 08:12:59.000000 osc-1.6.1/osc/conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    26088 2024-01-25 08:32:55.000000 osc-1.6.1/osc/connection.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   335883 2024-02-23 08:12:59.000000 osc-1.6.1/osc/core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10569 2024-01-25 08:32:55.000000 osc-1.6.1/osc/credentials.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    17690 2024-02-23 08:12:59.000000 osc-1.6.1/osc/fetch.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.238552 osc-1.6.1/osc/git_scm/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      212 2023-11-02 14:00:00.000000 osc-1.6.1/osc/git_scm/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5019 2024-01-25 08:32:55.000000 osc-1.6.1/osc/git_scm/store.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1611 2023-11-02 14:00:00.000000 osc-1.6.1/osc/grabber.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2428 2024-01-25 08:32:55.000000 osc-1.6.1/osc/meter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5913 2024-01-25 08:32:55.000000 osc-1.6.1/osc/oscerr.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6915 2024-02-23 08:12:59.000000 osc-1.6.1/osc/oscssl.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.238552 osc-1.6.1/osc/output/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      165 2024-02-23 08:12:59.000000 osc-1.6.1/osc/output/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1619 2024-02-23 08:12:59.000000 osc-1.6.1/osc/output/input.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2519 2023-11-02 14:00:00.000000 osc-1.6.1/osc/output/key_value_table.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      746 2023-11-02 14:00:00.000000 osc-1.6.1/osc/output/tty.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      450 2023-11-02 14:00:00.000000 osc-1.6.1/osc/output/widechar.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-11-02 14:00:00.000000 osc-1.6.1/osc/py.typed
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10836 2024-01-25 08:32:55.000000 osc-1.6.1/osc/store.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.241885 osc-1.6.1/osc/util/
--rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/ar.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/archquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/cpio.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/debquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/git_version.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/helper.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13371 2024-01-25 08:32:55.000000 osc-1.6.1/osc/util/models.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5579 2024-01-25 08:32:55.000000 osc-1.6.1/osc/util/packagequery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/repodata.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/rpmquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/safewriter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      272 2023-11-02 14:00:00.000000 osc-1.6.1/osc/util/xdg.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2136 2024-02-23 08:12:59.000000 osc-1.6.1/osc/util/xml.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.251885 osc-1.6.1/osc.egg-info/
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1573 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2082 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/SOURCES.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/dependency_links.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/entry_points.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/requires.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2024-02-23 08:54:22.000000 osc-1.6.1/osc.egg-info/top_level.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1599 2024-02-23 08:54:22.251885 osc-1.6.1/setup.cfg
--rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-11-02 14:00:00.000000 osc-1.6.1/setup.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-02-23 08:54:22.251885 osc-1.6.1/tests/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test__private_api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test__private_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_addfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1196 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_commandline.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_commit.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    24396 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_config_parser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4960 2024-02-23 08:12:59.000000 osc-1.6.1/tests/test_core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_core_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_core_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      554 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_credentials.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_deletefiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_difffiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_doc_plugins.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1876 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_git_scm_store.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      865 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_grabber.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_helpers.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_init_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_init_project.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9375 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_models.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4136 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_output.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_package_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_prdiff.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_project_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_repairwc.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_results.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_revertfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_setlinkrev.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8585 2023-11-02 14:00:00.000000 osc-1.6.1/tests/test_store.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    15541 2024-02-23 08:12:59.000000 osc-1.6.1/tests/test_update.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2675 2024-01-25 08:32:55.000000 osc-1.6.1/tests/test_vc.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.489072 osc-1.6.2/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      481 2024-04-08 07:35:37.000000 osc-1.6.2/AUTHORS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2024-04-08 07:35:37.000000 osc-1.6.2/COPYING
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2024-04-08 07:35:37.000000 osc-1.6.2/MANIFEST.in
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    18474 2024-04-15 08:26:36.000000 osc-1.6.2/NEWS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1573 2024-04-15 08:44:08.489072 osc-1.6.2/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2024-04-08 07:35:37.000000 osc-1.6.2/README.md
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.472405 osc-1.6.2/osc/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13384 2024-04-08 07:35:37.000000 osc-1.6.2/osc/OscConfigParser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2024-04-15 08:26:36.000000 osc-1.6.2/osc/__init__.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.475738 osc-1.6.2/osc/_private/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6142 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/api_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/api_configuration.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2024-04-08 07:37:19.000000 osc-1.6.2/osc/_private/api_source.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1949 2024-04-08 07:37:19.000000 osc-1.6.2/osc/_private/common.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5725 2024-04-08 07:37:19.000000 osc-1.6.2/osc/_private/project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2024-04-08 07:35:37.000000 osc-1.6.2/osc/_private/request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8506 2024-04-08 07:37:19.000000 osc-1.6.2/osc/babysitter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    65590 2024-04-15 08:26:33.000000 osc-1.6.2/osc/build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3205 2024-04-08 07:35:37.000000 osc-1.6.2/osc/checker.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10119 2024-04-08 07:35:37.000000 osc-1.6.2/osc/cmdln.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   446010 2024-04-15 08:26:33.000000 osc-1.6.2/osc/commandline.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.475738 osc-1.6.2/osc/commands/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2024-04-08 07:35:37.000000 osc-1.6.2/osc/commands/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      185 2024-04-08 07:37:19.000000 osc-1.6.2/osc/commands/repo.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2518 2024-04-08 07:37:19.000000 osc-1.6.2/osc/commands/repo_add.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1781 2024-04-08 07:37:19.000000 osc-1.6.2/osc/commands/repo_list.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1569 2024-04-08 07:37:19.000000 osc-1.6.2/osc/commands/repo_remove.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    70230 2024-04-08 07:35:37.000000 osc-1.6.2/osc/conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    26088 2024-04-08 07:37:19.000000 osc-1.6.2/osc/connection.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   336318 2024-04-15 08:26:33.000000 osc-1.6.2/osc/core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11097 2024-04-15 08:26:33.000000 osc-1.6.2/osc/credentials.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    17690 2024-04-08 07:35:37.000000 osc-1.6.2/osc/fetch.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.475738 osc-1.6.2/osc/git_scm/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      212 2024-04-08 07:35:37.000000 osc-1.6.2/osc/git_scm/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5019 2024-04-08 07:35:37.000000 osc-1.6.2/osc/git_scm/store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1611 2024-04-08 07:35:37.000000 osc-1.6.2/osc/grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2428 2024-04-08 07:35:37.000000 osc-1.6.2/osc/meter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5913 2024-04-08 07:35:37.000000 osc-1.6.2/osc/oscerr.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6915 2024-04-08 07:35:37.000000 osc-1.6.2/osc/oscssl.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.479072 osc-1.6.2/osc/output/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      165 2024-04-08 07:37:19.000000 osc-1.6.2/osc/output/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1619 2024-04-08 07:35:37.000000 osc-1.6.2/osc/output/input.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2519 2024-04-08 07:35:37.000000 osc-1.6.2/osc/output/key_value_table.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      746 2024-04-08 07:37:19.000000 osc-1.6.2/osc/output/tty.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      450 2024-04-08 07:35:37.000000 osc-1.6.2/osc/output/widechar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2024-04-08 07:35:37.000000 osc-1.6.2/osc/py.typed
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10836 2024-04-08 07:35:37.000000 osc-1.6.2/osc/store.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.479072 osc-1.6.2/osc/util/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/ar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/archquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/cpio.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/debquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/git_version.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/helper.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13373 2024-04-15 08:26:33.000000 osc-1.6.2/osc/util/models.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5579 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/packagequery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/repodata.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/rpmquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/safewriter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      272 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/xdg.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2136 2024-04-08 07:35:37.000000 osc-1.6.2/osc/util/xml.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.489072 osc-1.6.2/osc.egg-info/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1573 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2082 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/SOURCES.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/dependency_links.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/entry_points.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/requires.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2024-04-15 08:44:08.000000 osc-1.6.2/osc.egg-info/top_level.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1599 2024-04-15 08:44:08.489072 osc-1.6.2/setup.cfg
+-rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2024-04-08 07:35:37.000000 osc-1.6.2/setup.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2024-04-15 08:44:08.489072 osc-1.6.2/tests/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test__private_api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test__private_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_addfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1196 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_commandline.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_commit.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    24396 2024-04-08 07:37:19.000000 osc-1.6.2/tests/test_conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_config_parser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4960 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_core_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_core_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      554 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_credentials.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_deletefiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_difffiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_doc_plugins.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1876 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_git_scm_store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      865 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_helpers.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_init_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_init_project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9375 2024-04-08 07:37:19.000000 osc-1.6.2/tests/test_models.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4136 2024-04-08 07:37:19.000000 osc-1.6.2/tests/test_output.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_package_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_prdiff.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_project_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_repairwc.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_results.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_revertfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_setlinkrev.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8585 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    15541 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_update.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2675 2024-04-08 07:35:37.000000 osc-1.6.2/tests/test_vc.py
```

### Comparing `osc-1.6.1/COPYING` & `osc-1.6.2/COPYING`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/NEWS` & `osc-1.6.2/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+- 1.6.2
+  - Command-line:
+    - Fix 'branch' command to allow using '--new-package' option on packages that do not exist
+    - Fix 'buildinfo' command to include obs:cli_debug_packages by default
+    - Fix 'buildinfo' command to send complete local build environment as the 'build' command does
+    - Allow `osc rpmlint` to infer prj/pkg from CWD
+    - Propagate exit code from the run() and do_() commandline methods
+    - Give a hint where a scmsync git is hosted
+    - Fix crash in 'updatepacmetafromspec' command when working with an incomplete spec
+  - Authentication:
+    - Cache password from SecretService to avoid spamming user with an accept dialog
+    - Never ask for credentials when displaying help
+  - Library:
+    - Support package linking of packages from scmsync projects
+    - Fix do_createrequest() function to return None instead of request id
+    - Replace invalid 'if' with 'elif' in BaseModel.dict()
+    - Fix crash when no prefered packages are defined
+
 - 1.6.1
   - Command-line:
     - Use busybox compatible commands for completion
     - Change 'wipe' command to use the new get_user_input() function
     - Fix error 500 in running 'meta attribute <prj>'
   - Configuration:
     - Fix resolving config symlink to the actual config file
```

### Comparing `osc-1.6.1/PKG-INFO` & `osc-1.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.6.1
+Version: 1.6.2
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.6.1/README.md` & `osc-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/OscConfigParser.py` & `osc-1.6.2/osc/OscConfigParser.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/__init__.py` & `osc-1.6.2/osc/_private/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/api.py` & `osc-1.6.2/osc/_private/api.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/api_build.py` & `osc-1.6.2/osc/_private/api_build.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/api_source.py` & `osc-1.6.2/osc/_private/api_source.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/common.py` & `osc-1.6.2/osc/_private/common.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/package.py` & `osc-1.6.2/osc/_private/package.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/project.py` & `osc-1.6.2/osc/_private/project.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/_private/request.py` & `osc-1.6.2/osc/_private/request.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/babysitter.py` & `osc-1.6.2/osc/babysitter.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/build.py` & `osc-1.6.2/osc/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import getpass
 import glob
 import os
 import re
 import shutil
 import subprocess
 import sys
-
 from tempfile import NamedTemporaryFile, mkdtemp
+from typing import List
+from typing import Optional
 from urllib.parse import urlsplit
 from urllib.request import URLError, HTTPError
 from xml.etree import ElementTree as ET
 
 from . import conf
 from . import connection
 from . import core
@@ -477,15 +478,14 @@
         if not "repodata" in dirs:
             continue
         if "repomd.xml" in os.listdir(os.path.join(root, "repodata")):
             return root
     return None
 
 
-
 def get_prefer_pkgs(dirs, wanted_arch, type, cpio):
     paths = []
     repositories = []
 
     suffix = '*.rpm'
     if type in ('dsc', 'collax', 'livebuild'):
         suffix = '*.deb'
@@ -666,14 +666,84 @@
         cmd = su_wrapper(cmd)
 
     if not opts.userootforbuild:
         cmd.append('--norootforbuild')
     return run_external(cmd[0], *cmd[1:])
 
 
+def create_build_descr_data(
+    build_descr_path: Optional[str],
+    *,
+    build_type: Optional[str],
+    repo: Optional[str] = None,
+    arch: Optional[str] = None,
+    prefer_pkgs: Optional[List[str]] = None,
+    define: Optional[List[str]] = None,
+    define_with: Optional[List[str]] = None,
+    define_without: Optional[List[str]] = None,
+):
+    if build_descr_path:
+        build_descr_path = os.path.abspath(build_descr_path)
+        topdir = os.path.dirname(build_descr_path)
+    else:
+        topdir = None
+    result_data = []
+
+    if build_descr_path:
+        print(f"Using local file: {os.path.basename(build_descr_path)}", file=sys.stderr)
+        with open(build_descr_path, "rb") as f:
+            build_descr_data = f.read()
+
+        # HACK: there's no api to provide custom defines
+        # TODO: check if we're working with a spec?
+        defines: List[bytes] = []
+        for i in define or []:
+            defines.append(f"%define {i}".encode("utf-8"))
+        for i in define_with or []:
+            defines.append(f"%define _with_{i} 1".encode("utf-8"))
+        for i in define_without or []:
+            defines.append(f"%define _without_{i} 1".encode("utf-8"))
+        if defines:
+            build_descr_data = b"\n".join(defines) + b"\n\n" + build_descr_data
+
+        # build recipe must go first for compatibility with the older OBS versions
+        result_data.append((os.path.basename(build_descr_path).encode("utf-8"), build_descr_data))
+
+    if topdir:
+        buildenv_file = os.path.join(topdir, f"_buildenv.{repo}.{arch}")
+        if not os.path.isfile(buildenv_file):
+            buildenv_file = os.path.join(topdir, f"_buildenv")
+        if os.path.isfile(buildenv_file):
+            print(f"Using local file: {os.path.basename(buildenv_file)}", file=sys.stderr)
+            with open(buildenv_file, "rb") as f:
+                result_data.append((b"buildenv", f.read()))
+
+    if topdir:
+        service_file = os.path.join(topdir, "_service")
+        if os.path.isfile(service_file):
+            print("Using local file: _service", file=sys.stderr)
+            with open(service_file, "rb") as f:
+                result_data.append((b"_service", f.read()))
+
+    if not result_data and not prefer_pkgs:
+        return None, None
+
+    cpio_data = cpio.CpioWrite()
+    for key, value in result_data:
+        cpio_data.add(key, value)
+
+    if prefer_pkgs:
+        print("Scanning the following dirs for local preferred packages: {', '.join(dirs)}", file=sys.stderr)
+        prefer_pkgs_result = get_prefer_pkgs(prefer_pkgs, arch, build_type, cpio_data)
+    else:
+        prefer_pkgs_result = {}
+
+    return cpio_data.get(), prefer_pkgs_result
+
+
 def main(apiurl, store, opts, argv):
 
     repo = argv[0]
     arch = argv[1]
     build_descr = argv[2]
     xp = []
     build_root = None
@@ -894,67 +964,24 @@
             with open(filename, encoding="utf-8") as f:
                 for line in f:
                     extra_pkgs.append(line.rstrip('\n'))
 
     if xp:
         extra_pkgs += xp
 
-    prefer_pkgs = {}
-    build_descr_data = open(build_descr, 'rb').read()
-
-    # XXX: dirty hack but there's no api to provide custom defines
-    if opts.without:
-        s = ''
-        for i in opts.without:
-            s += "%%define _without_%s 1\n" % i
-        build_descr_data = s.encode() + build_descr_data
-    if opts._with:
-        s = ''
-        for i in opts._with:
-            s += "%%define _with_%s 1\n" % i
-        build_descr_data = s.encode() + build_descr_data
-    if opts.define:
-        s = ''
-        for i in opts.define:
-            s += "%%define %s\n" % i
-        build_descr_data = s.encode() + build_descr_data
-
-    cpiodata = None
-    servicefile = os.path.join(os.path.dirname(build_descr), "_service")
-    if not os.path.isfile(servicefile):
-        servicefile = os.path.join(os.path.dirname(build_descr), "_service")
-        if not os.path.isfile(servicefile):
-            servicefile = None
-        else:
-            print('Using local _service file')
-    buildenvfile = os.path.join(os.path.dirname(build_descr), "_buildenv." + repo + "." + arch)
-    if not os.path.isfile(buildenvfile):
-        buildenvfile = os.path.join(os.path.dirname(build_descr), "_buildenv")
-        if not os.path.isfile(buildenvfile):
-            buildenvfile = None
-        else:
-            print('Using local buildenv file: %s' % os.path.basename(buildenvfile))
-    if buildenvfile or servicefile:
-        if not cpiodata:
-            cpiodata = cpio.CpioWrite()
-
-    if opts.prefer_pkgs:
-        print('Scanning the following dirs for local packages: %s' % ', '.join(opts.prefer_pkgs))
-        if not cpiodata:
-            cpiodata = cpio.CpioWrite()
-        prefer_pkgs = get_prefer_pkgs(opts.prefer_pkgs, arch, build_type, cpiodata)
-
-    if cpiodata:
-        cpiodata.add(os.path.basename(build_descr.encode()), build_descr_data)
-        # buildenv must come last for compatibility reasons...
-        if buildenvfile:
-            cpiodata.add(b"buildenv", open(buildenvfile, 'rb').read())
-        if servicefile:
-            cpiodata.add(b"_service", open(servicefile, 'rb').read())
-        build_descr_data = cpiodata.get()
+    build_descr_data, prefer_pkgs = create_build_descr_data(
+        build_descr,
+        build_type=build_type,
+        repo=repo,
+        arch=arch,
+        prefer_pkgs=opts.prefer_pkgs,
+        define=opts.define,
+        define_with=opts._with,
+        define_without=opts.without,
+    )
 
     # special handling for overlay and rsync-src/dest
     specialcmdopts = []
     if opts.rsyncsrc or opts.rsyncdest:
         if not opts.rsyncsrc or not opts.rsyncdest:
             raise oscerr.WrongOptions('When using --rsync-{src,dest} both parameters have to be specified.')
         myrsyncsrc = os.path.abspath(os.path.expanduser(os.path.expandvars(opts.rsyncsrc)))
```

### Comparing `osc-1.6.1/osc/checker.py` & `osc-1.6.2/osc/checker.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/cmdln.py` & `osc-1.6.2/osc/cmdln.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/commandline.py` & `osc-1.6.2/osc/commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import textwrap
 import tempfile
 import time
 import traceback
 from functools import cmp_to_key
 from operator import itemgetter
 from pathlib import Path
+from tempfile import NamedTemporaryFile
 from typing import List
 from urllib.parse import urlsplit
 from urllib.error import HTTPError
 
 from . import _private
 from . import build as osc_build
 from . import cmdln
@@ -239,15 +240,15 @@
         pass
 
     def run(self, args):
         cmd = getattr(args, "_selected_command", None)
         if not cmd:
             self.parser.error("Please specify a command")
         self.post_parse_args(args)
-        cmd.run(args)
+        return cmd.run(args)
 
     def load_command(self, cls, module_prefix):
         mod_cls_name = f"{module_prefix}.{cls.__name__}"
         parent_name = getattr(cls, "parent", None)
         if parent_name:
             # allow relative references to classes in the the same module/directory
             if "." not in parent_name:
@@ -406,14 +407,18 @@
         self.add_argument(
             "--no-keyring",
             action="store_true",
             help="disable usage of desktop keyring system",
         )
 
     def post_parse_args(self, args):
+        if args.command == "help":
+            # HACK: never ask for credentials when displaying help
+            return
+
         # apiurl hasn't been specified by the user
         # we need to set it here because the 'default' option of an argument doesn't support lazy evaluation
         if args.apiurl is None:
             try:
                 # try reading the apiurl from the working copy
                 args.apiurl = osc_store.Store(Path.cwd()).apiurl
             except oscerr.NoWorkingCopy:
@@ -492,18 +497,18 @@
             def run(self, args):
                 sig = inspect.signature(self.func)
                 arg_names = list(sig.parameters.keys())
                 if arg_names == ["subcmd", "opts"]:
                     # handler doesn't take positional args via *args
                     if args.positional_args:
                         self.parser.error(f"unrecognized arguments: " + " ".join(args.positional_args))
-                    self.func(args.command, args)
+                    return self.func(args.command, args)
                 else:
                     # handler takes positional args via *args
-                    self.func(args.command, args, *args.positional_args)
+                    return self.func(args.command, args, *args.positional_args)
 
         return LegacyCommandWrapper
 
     def load_legacy_commands(self):
         # lazy links of attributes that would normally be initialized in the instance of Osc class
         class LegacyOsc(Osc):  # pylint: disable=used-before-assignment
             # pylint: disable=no-self-argument
@@ -551,15 +556,16 @@
         Initialize OscMainCommand, load all commands and run the selected command.
         """
         cmd = cls()
         cmd.load_commands()
         cmd.load_legacy_commands()
         if run:
             args = cmd.parse_args(args=argv)
-            cmd.run(args)
+            exit_code = cmd.run(args)
+            sys.exit(exit_code)
         else:
             args = None
         return cmd, args
 
 
 def get_parser():
     """
@@ -2817,15 +2823,14 @@
         f = http_POST(u, data=xml)
 
         root = ET.parse(f).getroot()
         rid = root.get('id')
         for srid in supersede:
             change_request_state(apiurl, srid, 'superseded',
                                  f'superseded by {rid}', rid)
-        return rid
 
     @cmdln.option('-m', '--message', metavar='TEXT',
                   help='specify message TEXT')
     @cmdln.option('-r', '--role', metavar='role',
                   help='specify user role (default: maintainer)')
     @cmdln.alias("reqbugownership")
     @cmdln.alias("requestbugownership")
@@ -5773,14 +5778,15 @@
         arg_list = args[:]
 
         for arg in arg_list:
             if is_project_dir(arg):
                 prj = Project(arg, progress_obj=self.download_progress)
                 if prj.scm_url:
                     print("Please use git to update project", prj.name)
+                    print("This git repository is hosted at", prj.scm_url)
                     continue
 
                 if conf.config['do_package_tracking']:
                     prj.update(expand_link=opts.expand_link,
                                unexpand_link=opts.unexpand_link)
                     args.remove(arg)
                 else:
@@ -5837,14 +5843,15 @@
 #                if [ i for i in p.filenamelist+p.filenamelist_unvers if p.status(i) != ' ' and p.status(i) != '?']:
 #                    print >>sys.stderr, 'osc: cannot expand/unexpand because your working ' \
 #                                        'copy has local modifications.\nPlease revert/commit them ' \
 #                                        'and try again.'
 #                    sys.exit(1)
             if p.scm_url:
                 print("Please use git to update package", p.name)
+                print("This git repository is hosted at", p.scm_url)
                 continue
 
             if not rev:
                 if opts.expand_link:
                     rev = p.latest_rev(expand=True)
                     if p.islink() and not p.isexpanded():
                         print('Expanding to rev', rev)
@@ -6202,15 +6209,31 @@
 
         usage:
             osc rpmlintlog project package repository arch
         """
         apiurl = self.get_api_url()
         args = slash_split(args)
 
-        if len(args) == 4:
+        if len(args) <= 3:
+            project = store_read_project(Path.cwd())
+            package = store_read_package(Path.cwd())
+            if len(args) == 1:
+                repository, arch = self._find_last_repo_arch(args[0], fatal=False)
+                if repository is None:
+                    # no local build with this repo was done
+                    print('failed to guess arch, using hostarch')
+                    repository = args[0]
+                    arch = osc_build.hostarch
+            elif len(args) == 2:
+                repository, arch = args
+            elif len(args) == 3:
+                raise oscerr.WrongArgs('Too many arguments.')
+            else:  # len(args) = 0 case
+                self.print_repos()
+        elif len(args) == 4:
             project, package, repository, arch = args
         else:
             raise oscerr.WrongArgs('please provide project package repository arch.')
 
         print(decode_it(get_rpmlint_log(apiurl, project, package, repository, arch)))
 
     @cmdln.alias('bl')
@@ -6622,14 +6645,16 @@
                   help='verbose output of build dependencies')
     @cmdln.option('-M', '--multibuild-package', metavar='FLAVOR',
                   help=HELP_MULTIBUILD_ONE)
     @cmdln.option('-x', '--extra-pkgs', metavar='PAC', action='append',
                   help='Add this package when computing the buildinfo')
     @cmdln.option('-p', '--prefer-pkgs', metavar='DIR', action='append',
                   help='Prefer packages from this directory when installing the build-root')
+    @cmdln.option('--nodebugpackages', '--no-debug-packages', action='store_true',
+                  help='Skip installation of additional debug packages for CLI builds (specified in obs:cli_debug_packages in project metadata)')
     def do_buildinfo(self, subcmd, opts, *args):
         """
         Shows the build info
 
         Shows the build "info" which is used in building a package.
         This command is mostly used internally by the 'build' subcommand.
         It needs to be called from within a package directory.
@@ -6681,36 +6706,58 @@
             if len(args) == 5:
                 build_descr = args[4]
         else:
             raise oscerr.WrongArgs('Too many arguments.')
 
         apiurl = self.get_api_url()
 
-        build_descr_data = None
-        if build_descr is not None:
-            build_descr_data = open(build_descr, 'rb').read()
-        if opts.prefer_pkgs and build_descr_data is None:
-            raise oscerr.WrongArgs('error: a build description is needed if \'--prefer-pkgs\' is used')
-        elif opts.prefer_pkgs:
-            print(f"Scanning the following dirs for local packages: {', '.join(opts.prefer_pkgs)}")
-            cpiodata = cpio.CpioWrite()
-            prefer_pkgs = osc_build.get_prefer_pkgs(opts.prefer_pkgs, arch,
-                                                    os.path.splitext(build_descr)[1],
-                                                    cpiodata)
-            cpiodata.add(os.path.basename(build_descr.encode()), build_descr_data)
-            build_descr_data = cpiodata.get()
+        # TODO: refactor retrieving build type in build.py and use it here or directly in create_build_descr_data()
+        if build_descr:
+            build_type = os.path.splitext(build_descr)[1]
+        else:
+            build_type = None
+
+        build_descr_data, prefer_pkgs = osc_build.create_build_descr_data(
+            build_descr,
+            build_type=build_type,
+            repo=repository,
+            arch=arch,
+            prefer_pkgs=opts.prefer_pkgs,
+            # define=,
+            # define_with=,
+            # define_without=,
+        )
 
         if opts.multibuild_package:
             package = package + ":" + opts.multibuild_package
 
-        print(decode_it(get_buildinfo(apiurl,
-                                      project, package, repository, arch,
-                                      specfile=build_descr_data,
-                                      debug=opts.debug_dependencies,
-                                      addlist=opts.extra_pkgs)))
+        extra_pkgs = opts.extra_pkgs.copy() if opts.extra_pkgs else []
+
+        if os.path.exists("/usr/lib/build/queryconfig") and not opts.nodebugpackages:
+            with NamedTemporaryFile(mode="w+b", prefix="obs_buildconfig_") as bc_file:
+                # print('Getting buildconfig from server and store to %s' % bc_filename)
+                bc = get_buildconfig(apiurl, project, repository)
+                bc_file.write(bc)
+                bc_file.flush()
+
+                debug_pkgs = decode_it(return_external("/usr/lib/build/queryconfig", "--dist", bc_file.name, "substitute", "obs:cli_debug_packages"))
+                if debug_pkgs:
+                    extra_pkgs.extend(debug_pkgs.strip().split(" "))
+
+        buildinfo = get_buildinfo(
+            apiurl,
+            project,
+            package,
+            repository,
+            arch,
+            specfile=build_descr_data,
+            debug=opts.debug_dependencies,
+            addlist=extra_pkgs,
+        )
+        print(decode_it(buildinfo))
 
     def do_buildconfig(self, subcmd, opts, *args):
         """
         Shows the build config
 
         Shows the build configuration which is used in building a package.
         This command is mostly used internally by the 'build' command.
@@ -7071,15 +7118,15 @@
     @cmdln.option('--noinit', '--no-init', action='store_true',
                   help='Skip initialization of build root and start with build immediately.')
     @cmdln.option('--nochecks', '--no-checks', action='store_true',
                   help='Do not run build checks on the resulting packages.')
     @cmdln.option('--no-verify', '--noverify', action='store_true',
                   help='Skip signature verification (via pgp keys) of packages used for build. (Global config in oscrc: no_verify)')
     @cmdln.option('--nodebugpackages', '--no-debug-packages', action='store_true',
-                  help='Skip installation of additional debug packages for CLI builds')
+                  help='Skip installation of additional debug packages for CLI builds (specified in obs:cli_debug_packages in project metadata)')
     @cmdln.option("--skip-local-service-run", "--noservice", "--no-service", default=False, action="store_true",
                   help="Skip run of local source services as specified in _service file.")
     @cmdln.option('-p', '--prefer-pkgs', metavar='DIR', action='append',
                   help='Prefer packages from this directory when installing the build-root')
     @cmdln.option('-k', '--keep-pkgs', metavar='DIR',
                   help='Save built packages into this directory')
     @cmdln.option('-M', '--multibuild-package', metavar='FLAVOR',
```

### Comparing `osc-1.6.1/osc/commands/repo_add.py` & `osc-1.6.2/osc/commands/repo_add.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/commands/repo_list.py` & `osc-1.6.2/osc/commands/repo_list.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/commands/repo_remove.py` & `osc-1.6.2/osc/commands/repo_remove.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/conf.py` & `osc-1.6.2/osc/conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/connection.py` & `osc-1.6.2/osc/connection.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/core.py` & `osc-1.6.2/osc/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -4371,16 +4371,18 @@
         m = re.compile(tag_pat % tag, re.I | re.M).search(''.join(lines))
         if m and m.group('val'):
             spec_data[tag] = m.group('val').strip()
 
     section_pat = r'^%s\s*?$'
     for section in sections:
         m = re.compile(section_pat % section, re.I | re.M).search(''.join(lines))
-        if m:
-            start = lines.index(m.group() + '\n') + 1
+        if m is None:
+            spec_data[section] = ""
+            continue
+        start = lines.index(m.group() + '\n') + 1
         data = []
         for line in lines[start:]:
             if line.startswith('%'):
                 break
             data.append(line)
         spec_data[section] = data
 
@@ -5834,20 +5836,25 @@
         if disable_publish:
             elm = root.find('publish')
             if not elm:
                 elm = ET.SubElement(root, 'publish')
             elm.clear()
             ET.SubElement(elm, 'disable')
 
+        root.remove('scmsync')
+
         dst_meta = ET.tostring(root, encoding=ET_ENCODING)
 
     if meta_change:
+        root = ET.fromstring(''.join(dst_meta))
+        for scmsync in root.findall('scmsync'):
+            root.remove(scmsync)
         edit_meta('pkg',
                   path_args=(dst_project, dst_package),
-                  data=dst_meta)
+                  data=ET.tostring(root, encoding=ET_ENCODING))
     # create the _link file
     # but first, make sure not to overwrite an existing one
     if '_link' in meta_get_filelist(apiurl, dst_project, dst_package):
         if force:
             print('forced overwrite of existing _link file', file=sys.stderr)
         else:
             print(file=sys.stderr)
@@ -6115,31 +6122,37 @@
     """
     Branch a package (via API call)
     """
 
     # BEGIN: Error out on branching scmsync packages; this should be properly handled in the API
 
     # read src_package meta
-    m = b"".join(show_package_meta(apiurl, src_project, src_package))
-    root = ET.fromstring(m)
+    try:
+        m = b"".join(show_package_meta(apiurl, src_project, src_package))
+        root = ET.fromstring(m)
+    except HTTPError as e:
+        if e.code == 404 and missingok:
+            root = None
+        else:
+            raise
 
     devel_project = None
     devel_package = None
-    if not nodevelproject:
+    if root is not None and not nodevelproject:
         devel_node = root.find("devel")
         if devel_node is not None:
             devel_project = devel_node.get("project")
             devel_package = devel_node.get("package", src_package)
         if devel_project:
             # replace src_package meta with devel_package meta because we're about branch from devel
             m = b"".join(show_package_meta(apiurl, devel_project, devel_package))
             root = ET.fromstring(m)
 
     # error out if we're branching a scmsync package (we'd end up with garbage anyway)
-    if root.find("scmsync") is not None:
+    if root is not None and root.find("scmsync") is not None:
         msg = "Cannot branch a package with <scmsync> set."
         if devel_project:
             raise oscerr.PackageError(devel_project, devel_package, msg)
         raise oscerr.PackageError(src_project, src_package, msg)
 
     # END: Error out on branching scmsync packages; this should be properly handled in the API
```

### Comparing `osc-1.6.1/osc/credentials.py` & `osc-1.6.2/osc/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,14 +185,18 @@
         return 3
 
     def create(self, cp):
         return TransientCredentialsManager(cp, None)
 
 
 class KeyringCredentialsManager(AbstractCredentialsManager):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._password = None
+
     def _process_options(self, options):
         if options is None:
             raise RuntimeError('options may not be None')
         self._backend_cls_name = options
 
     def _load_backend(self):
         try:
@@ -205,22 +209,27 @@
     @classmethod
     def create(cls, cp, options):
         if not has_keyring_support():
             return None
         return super().create(cp, options)
 
     def _get_password(self, url, user, apiurl=None):
-        self._load_backend()
-        return keyring.get_password(urlsplit(url)[1], user)
+        if self._password is None:
+            self._load_backend()
+            self._password = keyring.get_password(urlsplit(url)[1], user)
+            # TODO: this works fine on the command-line but a long-running process using osc library would start failing after changing the password in the keyring
+            # TODO: implement retrieving the password again after basic auth fails; sufficiently inform user about what's being done
+        return self._password
 
     def set_password(self, url, user, password):
         self._load_backend()
         keyring.set_password(urlsplit(url)[1], user, password)
         config_value = f"{self._qualified_name()}:{self._backend_cls_name}"
         self._cp.set(url, self.config_entry, config_value)
+        self._password = password
 
     def delete_password(self, url, user):
         self._load_backend()
         service = urlsplit(url)[1]
         data = keyring.get_password(service, user)
         if data is None:
             return
```

### Comparing `osc-1.6.1/osc/fetch.py` & `osc-1.6.2/osc/fetch.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/git_scm/store.py` & `osc-1.6.2/osc/git_scm/store.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/grabber.py` & `osc-1.6.2/osc/grabber.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/meter.py` & `osc-1.6.2/osc/meter.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/oscerr.py` & `osc-1.6.2/osc/oscerr.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/oscssl.py` & `osc-1.6.2/osc/oscssl.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/output/input.py` & `osc-1.6.2/osc/output/input.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/output/key_value_table.py` & `osc-1.6.2/osc/output/key_value_table.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/output/tty.py` & `osc-1.6.2/osc/output/tty.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/store.py` & `osc-1.6.2/osc/store.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/ar.py` & `osc-1.6.2/osc/util/ar.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/archquery.py` & `osc-1.6.2/osc/util/archquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/cpio.py` & `osc-1.6.2/osc/util/cpio.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/debquery.py` & `osc-1.6.2/osc/util/debquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/git_version.py` & `osc-1.6.2/osc/util/git_version.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/helper.py` & `osc-1.6.2/osc/util/helper.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/models.py` & `osc-1.6.2/osc/util/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,13 +380,13 @@
         result = {}
         for name, field in self.__fields__.items():
             if field.exclude:
                 continue
             value = getattr(self, name)
             if value is not None and field.is_model:
                 result[name] = value.dict()
-            if value is not None and field.is_model_list:
+            elif value is not None and field.is_model_list:
                 result[name] = [i.dict() for i in value]
             else:
                 result[name] = value
 
         return result
```

### Comparing `osc-1.6.1/osc/util/packagequery.py` & `osc-1.6.2/osc/util/packagequery.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/repodata.py` & `osc-1.6.2/osc/util/repodata.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/rpmquery.py` & `osc-1.6.2/osc/util/rpmquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/safewriter.py` & `osc-1.6.2/osc/util/safewriter.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc/util/xml.py` & `osc-1.6.2/osc/util/xml.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/osc.egg-info/PKG-INFO` & `osc-1.6.2/osc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.6.1
+Version: 1.6.2
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.6.1/osc.egg-info/SOURCES.txt` & `osc-1.6.2/osc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/setup.cfg` & `osc-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test__private_api.py` & `osc-1.6.2/tests/test__private_api.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test__private_package.py` & `osc-1.6.2/tests/test__private_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_addfiles.py` & `osc-1.6.2/tests/test_addfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_build.py` & `osc-1.6.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_commandline.py` & `osc-1.6.2/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_commit.py` & `osc-1.6.2/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_conf.py` & `osc-1.6.2/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_config_parser.py` & `osc-1.6.2/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_core.py` & `osc-1.6.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_core_package.py` & `osc-1.6.2/tests/test_core_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_core_request.py` & `osc-1.6.2/tests/test_core_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_credentials.py` & `osc-1.6.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_deletefiles.py` & `osc-1.6.2/tests/test_deletefiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_difffiles.py` & `osc-1.6.2/tests/test_difffiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_doc_plugins.py` & `osc-1.6.2/tests/test_doc_plugins.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_git_scm_store.py` & `osc-1.6.2/tests/test_git_scm_store.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_grabber.py` & `osc-1.6.2/tests/test_grabber.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_helpers.py` & `osc-1.6.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_init_package.py` & `osc-1.6.2/tests/test_init_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_init_project.py` & `osc-1.6.2/tests/test_init_project.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_models.py` & `osc-1.6.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_output.py` & `osc-1.6.2/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_package_status.py` & `osc-1.6.2/tests/test_package_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_prdiff.py` & `osc-1.6.2/tests/test_prdiff.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_project_status.py` & `osc-1.6.2/tests/test_project_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_repairwc.py` & `osc-1.6.2/tests/test_repairwc.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_request.py` & `osc-1.6.2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_results.py` & `osc-1.6.2/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_revertfiles.py` & `osc-1.6.2/tests/test_revertfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_setlinkrev.py` & `osc-1.6.2/tests/test_setlinkrev.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_store.py` & `osc-1.6.2/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_update.py` & `osc-1.6.2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `osc-1.6.1/tests/test_vc.py` & `osc-1.6.2/tests/test_vc.py`

 * *Files identical despite different names*

