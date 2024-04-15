# Comparing `tmp/zfs_autobackup-3.2b1.tar.gz` & `tmp/zfs_autobackup-3.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zfs_autobackup-3.2b1.tar", last modified: Tue Aug 16 07:14:30 2022, max compression
+gzip compressed data, was "zfs_autobackup-3.3b3.tar", last modified: Mon Apr 15 09:43:34 2024, max compression
```

## Comparing `zfs_autobackup-3.2b1.tar` & `zfs_autobackup-3.3b3.tar`

### file list

```diff
@@ -1,36 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4998 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4998 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 07:14:30.000000 zfs_autobackup-3.2b1/zfs_autobackup/
--rw-r--r--   0 runner    (1001) docker     (121)    11712 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsAutoverify.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/TreeHasher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsAuto.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/LogStub.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/LogConsole.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/CachedProperty.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsPool.py
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/Thinner.py
--rw-r--r--   0 runner    (1001) docker     (121)    43182 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ExecuteNode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/compressors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/CliBase.py
--rw-r--r--   0 runner    (1001) docker     (121)    10633 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsNode.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        3 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ThinnerRule.py
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/BlockHasher.py
--rw-r--r--   0 runner    (1001) docker     (121)    25867 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsAutobackup.py
--rw-r--r--   0 runner    (1001) docker     (121)     7530 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/CmdPipe.py
--rw-r--r--   0 runner    (1001) docker     (121)    11023 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/ZfsCheck.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       91 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/zfs_autobackup/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-08-16 07:14:13.000000 zfs_autobackup-3.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:43:34.198589 zfs_autobackup-3.3b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-15 09:43:34.198589 zfs_autobackup-3.3b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:43:34.198589 zfs_autobackup-3.3b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:43:34.194589 zfs_autobackup-3.3b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_blockhasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_cmdpipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_destroymissing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21844 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_executenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_externalfailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_sendrecvpipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_thinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_treehasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35892 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_zfsautobackup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_zfsautobackup31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_zfsautobackup32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_zfscheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/tests/test_zfsnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:43:34.198589 zfs_autobackup-3.3b3/zfs_autobackup/
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/BlockHasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/CachedProperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/CliBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/CmdPipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ExecuteNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/LogConsole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/LogStub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/Thinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ThinnerRule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/TreeHasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsAuto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27108 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsAutobackup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsAutoverify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/ZfsPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        3 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/compressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-15 09:43:26.000000 zfs_autobackup-3.3b3/zfs_autobackup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:43:34.198589 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:43:34.000000 zfs_autobackup-3.3b3/zfs_autobackup.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup.egg-info/PKG-INFO` & `zfs_autobackup-3.3b3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,68 @@
-Metadata-Version: 2.1
-Name: zfs-autobackup
-Version: 3.2b1
-Summary: ZFS autobackup is used to periodicly backup ZFS filesystems to other locations. It tries to be the most friendly to use and easy to debug ZFS backup tool.
-Home-page: https://github.com/psy0rz/zfs_autobackup
-Author: Edwin Eefting
-Author-email: edwin@datux.nl
-License: UNKNOWN
-Description: 
-        # ZFS autobackup
-        
-        [![Tests](https://github.com/psy0rz/zfs_autobackup/workflows/Regression%20tests/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions?query=workflow%3A%22Regression+tests%22) [![Coverage Status](https://coveralls.io/repos/github/psy0rz/zfs_autobackup/badge.svg)](https://coveralls.io/github/psy0rz/zfs_autobackup)  [![Python Package](https://github.com/psy0rz/zfs_autobackup/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/zfs-autobackup/)
-        [![CodeQL](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml)
-        
-        ## Introduction
-        
-        ZFS-autobackup tries to be the most reliable and easiest to use tool, while having all the features.
-        
-        You can either use it as a **backup** tool, **replication** tool or **snapshot** tool.
-        
-        You can select what to backup by setting a custom `ZFS property`. This makes it easy to add/remove specific datasets, or just backup your whole pool.
-        
-        Other settings are just specified on the commandline: Simply setup and test your zfs-autobackup command and  fix all the issues you might encounter. When you're done you can just copy/paste your command to a cron or script.
-        
-        Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or error. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
-        
-        An important feature that's missing from other tools is a reliable `--test` option: This allows you to see what zfs-autobackup will do and tune your parameters. It will do everything, except make changes to your system.
-        
-        ## Features
-        
-        * Works across operating systems: Tested with **Linux**, **FreeBSD/FreeNAS** and **SmartOS**.
-        * Low learning curve: no complex daemons or services, no additional software or networking needed. (Only read this page)   
-        * Plays nicely with existing replication systems. (Like Proxmox HA)
-        * Automatically selects filesystems to backup by looking at a simple ZFS property. 
-        * Creates consistent snapshots. (takes all snapshots at once, atomicly.)
-        * Multiple backups modes:
-          * Backup local data on the same server.
-          * "push" local data to a backup-server via SSH.
-          * "pull" remote data from a server via SSH and backup it locally.
-          * "pull+push": Zero trust between source and target.
-        * Can be scheduled via simple cronjob or run directly from commandline.
-        * ZFS encryption support: Can decrypt / encrypt or even re-encrypt datasets during transfer.
-        * Supports sending with compression. (Using pigz, zstd etc)
-        * IO buffering to speed up transfer.
-        * Bandwidth rate limiting.
-        * Multiple backups from and to the same datasets are no problem.
-        * Resillient to errors.
-        * Ability to manually 'finish' failed backups to see whats going on.
-        * Easy to debug and has a test-mode. Actual unix commands are printed.
-        * Uses progressive thinning for older snapshots.
-        * Uses zfs-holds on important snapshots to prevent accidental deletion.
-        * Automatic resuming of failed transfers.
-        * Easy migration from other zfs backup systems to zfs-autobackup.
-        * Gracefully handles datasets that no longer exist on source.
-        * Complete and clean logging. 
-        * Easy installation:
-          * Just install zfs-autobackup via pip.
-          * Only needs to be installed on one side.
-          * Written in python and uses zfs-commands, no special 3rd party dependency's or compiled libraries needed.
-          * No annoying config files or properties. 
-        
-        ## Getting started
-        
-        Please look at our wiki to [Get started](https://github.com/psy0rz/zfs_autobackup/wiki).
-        
-        # Sponsor list
-        
-        This project was sponsorred by:
-        
-        * JetBrains (Provided me with a license for their whole professional product line, https://www.jetbrains.com/pycharm/ )
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
+
+# ZFS autobackup
+
+[![Tests](https://github.com/psy0rz/zfs_autobackup/workflows/Regression%20tests/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions?query=workflow%3A%22Regression+tests%22) [![Coverage Status](https://coveralls.io/repos/github/psy0rz/zfs_autobackup/badge.svg)](https://coveralls.io/github/psy0rz/zfs_autobackup)  [![Python Package](https://github.com/psy0rz/zfs_autobackup/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/zfs-autobackup/)
+[![CodeQL](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml)
+
+## Introduction
+
+ZFS-autobackup tries to be the most reliable and easiest to use tool, while having all the features.
+
+You can either use it as a **backup** tool, **replication** tool or **snapshot** tool.
+
+You can select what to backup by setting a custom `ZFS property`. This makes it easy to add/remove specific datasets, or just backup your whole pool.
+
+Other settings are just specified on the commandline: Simply setup and test your zfs-autobackup command and  fix all the issues you might encounter. When you're done you can just copy/paste your command to a cron or script.
+
+Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or errors. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
+
+An important feature that's missing from other tools is a reliable `--test` option: This allows you to see what zfs-autobackup will do and tune your parameters. It will do everything, except make changes to your system.
+
+## Features
+
+* Works across operating systems: Tested with **Linux**, **FreeBSD/FreeNAS** and **SmartOS**.
+* Low learning curve: no complex daemons or services, no additional software or networking needed. 
+* Plays nicely with existing replication systems. (Like Proxmox HA)
+* Automatically selects filesystems to backup by looking at a simple ZFS property. 
+* Creates consistent snapshots. (takes all snapshots at once, atomicly.)
+* Multiple backups modes:
+  * Backup local data on the same server.
+  * "push" local data to a backup-server via SSH.
+  * "pull" remote data from a server via SSH and backup it locally.
+  * "pull+push": Zero trust between source and target.
+* Can be scheduled via simple cronjob or run directly from commandline.
+* Also supports complex backup geometries.
+* ZFS encryption support: Can decrypt / encrypt or even re-encrypt datasets during transfer.
+* Supports sending with compression. (Using pigz, zstd etc)
+* IO buffering to speed up transfer.
+* Bandwidth rate limiting.
+* Multiple backups from and to the same datasets are no problem.
+* Resillient to errors.
+* Ability to manually 'finish' failed backups to see whats going on.
+* Easy to debug and has a test-mode. Actual unix commands are printed.
+* Uses progressive thinning for older snapshots.
+* Uses zfs-holds on important snapshots to prevent accidental deletion.
+* Automatic resuming of failed transfers.
+* Easy migration from other zfs backup systems to zfs-autobackup.
+* Gracefully handles datasets that no longer exist on source.
+* Complete and clean logging.
+* All code is regression tested against actual ZFS environments.
+* Easy installation:
+  * Just install zfs-autobackup via pip.
+  * Only needs to be installed on one side.
+  * Written in python and uses zfs-commands, no special 3rd party dependency's or compiled libraries needed.
+  * No annoying config files or properties. 
+
+## Getting started
+
+Please look at our wiki to [Get started](https://github.com/psy0rz/zfs_autobackup/wiki).
+
+Or read the [Full manual](https://github.com/psy0rz/zfs_autobackup/wiki/Manual)
+
+# Sponsor list
+
+This project was sponsored by:
+
+* JetBrains 
+* https://rsync.net
+* [DatuX](https://www.datux.nl)
```

### Comparing `zfs_autobackup-3.2b1/PKG-INFO` & `zfs_autobackup-3.3b3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 Metadata-Version: 2.1
 Name: zfs_autobackup
-Version: 3.2b1
+Version: 3.3b3
 Summary: ZFS autobackup is used to periodicly backup ZFS filesystems to other locations. It tries to be the most friendly to use and easy to debug ZFS backup tool.
 Home-page: https://github.com/psy0rz/zfs_autobackup
 Author: Edwin Eefting
 Author-email: edwin@datux.nl
-License: UNKNOWN
-Description: 
-        # ZFS autobackup
-        
-        [![Tests](https://github.com/psy0rz/zfs_autobackup/workflows/Regression%20tests/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions?query=workflow%3A%22Regression+tests%22) [![Coverage Status](https://coveralls.io/repos/github/psy0rz/zfs_autobackup/badge.svg)](https://coveralls.io/github/psy0rz/zfs_autobackup)  [![Python Package](https://github.com/psy0rz/zfs_autobackup/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/zfs-autobackup/)
-        [![CodeQL](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml)
-        
-        ## Introduction
-        
-        ZFS-autobackup tries to be the most reliable and easiest to use tool, while having all the features.
-        
-        You can either use it as a **backup** tool, **replication** tool or **snapshot** tool.
-        
-        You can select what to backup by setting a custom `ZFS property`. This makes it easy to add/remove specific datasets, or just backup your whole pool.
-        
-        Other settings are just specified on the commandline: Simply setup and test your zfs-autobackup command and  fix all the issues you might encounter. When you're done you can just copy/paste your command to a cron or script.
-        
-        Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or error. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
-        
-        An important feature that's missing from other tools is a reliable `--test` option: This allows you to see what zfs-autobackup will do and tune your parameters. It will do everything, except make changes to your system.
-        
-        ## Features
-        
-        * Works across operating systems: Tested with **Linux**, **FreeBSD/FreeNAS** and **SmartOS**.
-        * Low learning curve: no complex daemons or services, no additional software or networking needed. (Only read this page)   
-        * Plays nicely with existing replication systems. (Like Proxmox HA)
-        * Automatically selects filesystems to backup by looking at a simple ZFS property. 
-        * Creates consistent snapshots. (takes all snapshots at once, atomicly.)
-        * Multiple backups modes:
-          * Backup local data on the same server.
-          * "push" local data to a backup-server via SSH.
-          * "pull" remote data from a server via SSH and backup it locally.
-          * "pull+push": Zero trust between source and target.
-        * Can be scheduled via simple cronjob or run directly from commandline.
-        * ZFS encryption support: Can decrypt / encrypt or even re-encrypt datasets during transfer.
-        * Supports sending with compression. (Using pigz, zstd etc)
-        * IO buffering to speed up transfer.
-        * Bandwidth rate limiting.
-        * Multiple backups from and to the same datasets are no problem.
-        * Resillient to errors.
-        * Ability to manually 'finish' failed backups to see whats going on.
-        * Easy to debug and has a test-mode. Actual unix commands are printed.
-        * Uses progressive thinning for older snapshots.
-        * Uses zfs-holds on important snapshots to prevent accidental deletion.
-        * Automatic resuming of failed transfers.
-        * Easy migration from other zfs backup systems to zfs-autobackup.
-        * Gracefully handles datasets that no longer exist on source.
-        * Complete and clean logging. 
-        * Easy installation:
-          * Just install zfs-autobackup via pip.
-          * Only needs to be installed on one side.
-          * Written in python and uses zfs-commands, no special 3rd party dependency's or compiled libraries needed.
-          * No annoying config files or properties. 
-        
-        ## Getting started
-        
-        Please look at our wiki to [Get started](https://github.com/psy0rz/zfs_autobackup/wiki).
-        
-        # Sponsor list
-        
-        This project was sponsorred by:
-        
-        * JetBrains (Provided me with a license for their whole professional product line, https://www.jetbrains.com/pycharm/ )
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: colorama
+Requires-Dist: argparse
+
+
+# ZFS autobackup
+
+[![Tests](https://github.com/psy0rz/zfs_autobackup/workflows/Regression%20tests/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions?query=workflow%3A%22Regression+tests%22) [![Coverage Status](https://coveralls.io/repos/github/psy0rz/zfs_autobackup/badge.svg)](https://coveralls.io/github/psy0rz/zfs_autobackup)  [![Python Package](https://github.com/psy0rz/zfs_autobackup/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/zfs-autobackup/)
+[![CodeQL](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml)
+
+## Introduction
+
+ZFS-autobackup tries to be the most reliable and easiest to use tool, while having all the features.
+
+You can either use it as a **backup** tool, **replication** tool or **snapshot** tool.
+
+You can select what to backup by setting a custom `ZFS property`. This makes it easy to add/remove specific datasets, or just backup your whole pool.
+
+Other settings are just specified on the commandline: Simply setup and test your zfs-autobackup command and  fix all the issues you might encounter. When you're done you can just copy/paste your command to a cron or script.
+
+Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or errors. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
+
+An important feature that's missing from other tools is a reliable `--test` option: This allows you to see what zfs-autobackup will do and tune your parameters. It will do everything, except make changes to your system.
+
+## Features
+
+* Works across operating systems: Tested with **Linux**, **FreeBSD/FreeNAS** and **SmartOS**.
+* Low learning curve: no complex daemons or services, no additional software or networking needed. 
+* Plays nicely with existing replication systems. (Like Proxmox HA)
+* Automatically selects filesystems to backup by looking at a simple ZFS property. 
+* Creates consistent snapshots. (takes all snapshots at once, atomicly.)
+* Multiple backups modes:
+  * Backup local data on the same server.
+  * "push" local data to a backup-server via SSH.
+  * "pull" remote data from a server via SSH and backup it locally.
+  * "pull+push": Zero trust between source and target.
+* Can be scheduled via simple cronjob or run directly from commandline.
+* Also supports complex backup geometries.
+* ZFS encryption support: Can decrypt / encrypt or even re-encrypt datasets during transfer.
+* Supports sending with compression. (Using pigz, zstd etc)
+* IO buffering to speed up transfer.
+* Bandwidth rate limiting.
+* Multiple backups from and to the same datasets are no problem.
+* Resillient to errors.
+* Ability to manually 'finish' failed backups to see whats going on.
+* Easy to debug and has a test-mode. Actual unix commands are printed.
+* Uses progressive thinning for older snapshots.
+* Uses zfs-holds on important snapshots to prevent accidental deletion.
+* Automatic resuming of failed transfers.
+* Easy migration from other zfs backup systems to zfs-autobackup.
+* Gracefully handles datasets that no longer exist on source.
+* Complete and clean logging.
+* All code is regression tested against actual ZFS environments.
+* Easy installation:
+  * Just install zfs-autobackup via pip.
+  * Only needs to be installed on one side.
+  * Written in python and uses zfs-commands, no special 3rd party dependency's or compiled libraries needed.
+  * No annoying config files or properties. 
+
+## Getting started
+
+Please look at our wiki to [Get started](https://github.com/psy0rz/zfs_autobackup/wiki).
+
+Or read the [Full manual](https://github.com/psy0rz/zfs_autobackup/wiki/Manual)
+
+# Sponsor list
+
+This project was sponsored by:
+
+* JetBrains 
+* https://rsync.net
+* [DatuX](https://www.datux.nl)
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsAutoverify.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsAutoverify.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         #     compare_trees_tar(source_snapshot.zfs_node, source_mnt, target_snapshot.zfs_node, target_mnt)
         elif method == 'find':
             compare_trees_find(source_snapshot.zfs_node, source_mnt, target_snapshot.zfs_node, target_mnt)
         else:
             raise(Exception("program errror, unknown method"))
 
     finally:
-        source_snapshot.unmount()
-        target_snapshot.unmount()
+        source_snapshot.unmount(source_mnt)
+        target_snapshot.unmount(target_mnt)
 
 
 # def hash_dev(node, dev):
 #     """calculate md5sum of a device on a node"""
 #
 #     node.debug("Hashing volume {} ".format(dev))
 #
@@ -182,15 +182,15 @@
 
             try:
                 # determine corresponding target_dataset
                 target_name = self.make_target_name(source_dataset)
                 target_dataset = target_node.get_dataset(target_name)
 
                 # find common snapshots to  verify
-                source_snapshot = source_dataset.find_common_snapshot(target_dataset)
+                source_snapshot = source_dataset.find_common_snapshot(target_dataset, True)
                 target_snapshot = target_dataset.find_snapshot(source_snapshot)
 
                 if source_snapshot is None or target_snapshot is None:
                     raise(Exception("Cant find common snapshot"))
 
                 target_snapshot.verbose("Verifying...")
 
@@ -235,20 +235,19 @@
                                   snapshot_time_format=self.snapshot_time_format, hold_name=self.hold_name, logger=self,
                                   ssh_config=self.args.ssh_config,
                                   ssh_to=self.args.ssh_source, readonly=self.args.test,
                                   debug_output=self.args.debug_output, description=description)
 
             ################# select source datasets
             self.set_title("Selecting")
-            source_datasets = source_node.selected_datasets(property_name=self.property_name,
+            ( source_datasets, excluded_datasets) = source_node.selected_datasets(property_name=self.property_name,
                                                             exclude_received=self.args.exclude_received,
                                                             exclude_paths=self.exclude_paths,
-                                                            exclude_unchanged=self.args.exclude_unchanged,
-                                                            min_change=0)
-            if not source_datasets:
+                                                            exclude_unchanged=self.args.exclude_unchanged)
+            if not source_datasets and not excluded_datasets:
                 self.print_error_sources()
                 return 255
 
             # create target_node
             self.set_title("Target settings")
             target_node = ZfsNode(utc=self.args.utc,
                                   snapshot_time_format=self.snapshot_time_format, hold_name=self.hold_name,
@@ -303,14 +302,15 @@
 
 
 
 
 def cli():
     import sys
 
+    raise(Exception("This program is incomplete, dont use it yet."))
     signal(SIGPIPE, sigpipe_handler)
     failed = ZfsAutoverify(sys.argv[1:], False).run()
     sys.exit(min(failed,255))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/TreeHasher.py` & `zfs_autobackup-3.3b3/zfs_autobackup/TreeHasher.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsAuto.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsAuto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import sys
 
 from .CliBase import CliBase
+from .util import datetime_now
 
 
 class ZfsAuto(CliBase):
     """Common Base class for ZfsAutobackup and ZfsAutoverify ."""
 
     def __init__(self, argv, print_arguments=True):
 
@@ -42,27 +43,31 @@
         self.exclude_paths = []
         if args.ssh_source == args.ssh_target:
             if args.target_path:
                 # target and source are the same, make sure to exclude target_path
                 self.verbose("NOTE: Source and target are on the same host, excluding target-path from selection.")
                 self.exclude_paths.append(args.target_path)
             else:
-                if not args.exclude_received:
-                    self.verbose("NOTE: Source and target are on the same host, adding --exclude-received to commandline.")
+                if not args.exclude_received and not args.include_received:
+                    self.verbose("NOTE: Source and target are on the same host, adding --exclude-received to commandline. (use --include-received to overrule)")
                     args.exclude_received = True
 
         if args.test:
             self.warning("TEST MODE - SIMULATING WITHOUT MAKING ANY CHANGES")
 
         #format all the names
         self.property_name = args.property_format.format(args.backup_name)
         self.snapshot_time_format = args.snapshot_format.format(args.backup_name)
         self.hold_name = args.hold_format.format(args.backup_name)
 
+        dt = datetime_now(args.utc)
+
         self.verbose("")
+        self.verbose("Current time {}           : {}".format(args.utc and "UTC" or "   ", dt.strftime("%Y-%m-%d %H:%M:%S")))
+
         self.verbose("Selecting dataset property : {}".format(self.property_name))
         self.verbose("Snapshot format            : {}".format(self.snapshot_time_format))
         self.verbose("Timezone                   : {}".format("UTC" if args.utc else "Local"))
 
         return args
 
     def get_parser(self):
@@ -94,19 +99,22 @@
         group.add_argument('--hold-format', metavar='FORMAT', default="zfs_autobackup:{}",
                             help='ZFS hold string format. Default: %(default)s')
         group.add_argument('--strip-path', metavar='N', default=0, type=int,
                            help='Number of directories to strip from target path.')
 
         group=parser.add_argument_group("Selection options")
         group.add_argument('--ignore-replicated', action='store_true', help=argparse.SUPPRESS)
-        group.add_argument('--exclude-unchanged', action='store_true',
-                            help='Exclude datasets that have no changes since any last snapshot. (Useful in combination with proxmox HA replication)')
+        group.add_argument('--exclude-unchanged', metavar='BYTES', default=0, type=int,
+                            help='Exclude datasets that have less than BYTES data changed since any last snapshot. (Use with proxmox HA replication)')
         group.add_argument('--exclude-received', action='store_true',
                             help='Exclude datasets that have the origin of their autobackup: property as "received". '
                                  'This can avoid recursive replication between two backup partners.')
+        group.add_argument('--include-received', action='store_true',
+                            help=argparse.SUPPRESS)
+
 
         return parser
 
     def print_error_sources(self):
         self.error(
             "No source filesystems selected, please do a 'zfs set autobackup:{0}=true' on the source datasets "
             "you want to select.".format(
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/LogStub.py` & `zfs_autobackup-3.3b3/zfs_autobackup/LogStub.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/LogConsole.py` & `zfs_autobackup-3.3b3/zfs_autobackup/LogConsole.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         else:
             print("! " + txt, file=sys.stderr)
         sys.stderr.flush()
 
     def warning(self, txt):
         self.clear_progress()
         if self.colorama:
-            print(colorama.Fore.YELLOW + colorama.Style.BRIGHT + "  NOTE: " + txt + colorama.Style.RESET_ALL)
+            print(colorama.Fore.YELLOW + colorama.Style.NORMAL + "  NOTE: " + txt + colorama.Style.RESET_ALL)
         else:
             print("  NOTE: " + txt)
         sys.stdout.flush()
 
     def verbose(self, txt):
         if self.show_verbose:
             self.clear_progress()
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/CachedProperty.py` & `zfs_autobackup-3.3b3/zfs_autobackup/CachedProperty.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsPool.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsPool.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/Thinner.py` & `zfs_autobackup-3.3b3/zfs_autobackup/Thinner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 
 from .ThinnerRule import ThinnerRule
 
 
 class Thinner:
     """progressive thinner (universal, used for cleaning up snapshots)"""
 
@@ -33,28 +32,26 @@
         if self.always_keep:
             ret.append("Keep the last {} snapshot{}.".format(self.always_keep, self.always_keep != 1 and "s" or ""))
         for rule in self.rules:
             ret.append(rule.human_str)
 
         return ret
 
-    def thin(self, objects, keep_objects=None, now=None):
+    def thin(self, objects, keep_objects, now):
         """thin list of objects with current schedule rules. objects: list of
         objects to thin. every object should have timestamp attribute.
 
             return( keeps, removes )
 
         Args:
             objects: list of objects to check (should have a timestamp attribute)
             keep_objects: objects to always keep (if they also are in the in the normal objects list)
             now: if specified, use this time as current time
         """
 
-        if not keep_objects:
-            keep_objects = []
 
         # always keep a number of the last objets?
         if self.always_keep:
             # all of them
             if len(objects) <= self.always_keep:
                 return objects, []
 
@@ -64,17 +61,14 @@
             always_keep_objects = []
 
         # determine time blocks
         time_blocks = {}
         for rule in self.rules:
             time_blocks[rule.period] = {}
 
-        if not now:
-            now = int(time.time())
-
         keeps = []
         removes = []
 
         # traverse objects
         for thisobject in objects:
             # important they are ints!
             timestamp = int(thisobject.timestamp)
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsDataset.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsDataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,21 @@
     def error(self, txt):
         """
         Args:
             :type txt: str
         """
         self.zfs_node.error("{}: {}".format(self.name, txt))
 
+    def warning(self, txt):
+        """
+        Args:
+            :type txt: str
+        """
+        self.zfs_node.warning("{}: {}".format(self.name, txt))
+
     def debug(self, txt):
         """
         Args:
             :type txt: str
         """
         self.zfs_node.debug("{}: {}".format(self.name, txt))
 
@@ -77,16 +84,16 @@
 
     def lstrip_path(self, count):
         """return name with first count components stripped
 
         Args:
             :type count: int
         """
-        components=self.split_path()
-        if count>len(components):
+        components = self.split_path()
+        if count > len(components):
             raise Exception("Trying to strip too much from path ({} items from {})".format(count, self.name))
 
         return "/".join(components[count:])
 
     def rstrip_path(self, count):
         """return name with last count components stripped
 
@@ -114,30 +121,33 @@
         return snapshot_name
 
     @property
     def is_snapshot(self):
         """true if this dataset is a snapshot"""
         return self.name.find("@") != -1
 
-    def is_selected(self, value, source, inherited, exclude_received, exclude_paths, exclude_unchanged, min_change):
+    def is_selected(self, value, source, inherited, exclude_received, exclude_paths, exclude_unchanged):
         """determine if dataset should be selected for backup (called from
         ZfsNode)
 
         Args:
-            :type exclude_paths: list of str
+            :type exclude_paths: list[str]
             :type value: str
             :type source: str
             :type inherited: bool
             :type exclude_received: bool
-            :type exclude_unchanged: bool
-            :type min_change: bool
+            :type exclude_unchanged: int
 
             :param value: Value of the zfs property ("false"/"true"/"child"/parent/"-")
             :param source: Source of the zfs property ("local"/"received", "-")
             :param inherited: True of the value/source was inherited from a higher dataset.
+
+        Returns: True : Selected
+                 False: Excluded
+                 None: No property found
         """
 
         # sanity checks
         if source not in ["local", "received", "-"]:
             # probably a program error in zfs-autobackup or new feature in zfs
             raise (Exception(
                 "{} autobackup-property has illegal source: '{}' (possible BUG)".format(self.name, source)))
@@ -145,15 +155,15 @@
         if value not in ["false", "true", "child", "parent", "-"]:
             # user error
             raise (Exception(
                 "{} autobackup-property has illegal value: '{}'".format(self.name, value)))
 
         # non specified, ignore
         if value == "-":
-            return False
+            return None
 
         # only select childs of this dataset, ignore
         if value == "child" and not inherited:
             return False
 
         # only select parent, no childs, ignore
         if value == "parent" and inherited:
@@ -175,36 +185,36 @@
                 return False
 
         if source == "received":
             if exclude_received:
                 self.verbose("Excluded (dataset already received)")
                 return False
 
-        if exclude_unchanged and not self.is_changed(min_change):
-            self.verbose("Excluded (unchanged since last snapshot)")
+        if not self.is_changed(exclude_unchanged):
+            self.verbose("Excluded (by --exclude-unchanged)")
             return False
 
         self.verbose("Selected")
         return True
 
-
-    @CachedProperty
+    @property
     def parent(self):
         """get zfs-parent of this dataset. for snapshots this means it will get
         the filesystem/volume that it belongs to. otherwise it will return the
         parent according to path
 
         we cache this so everything in the parent that is cached also stays.
 
         returns None if there is no parent.
+        :rtype: ZfsDataset | None
         """
         if self.is_snapshot:
             return self.zfs_node.get_dataset(self.filesystem_name)
         else:
-            stripped=self.rstrip_path(1)
+            stripped = self.rstrip_path(1)
             if stripped:
                 return self.zfs_node.get_dataset(stripped)
             else:
                 return None
 
     # NOTE: unused for now
     # def find_prev_snapshot(self, snapshot, also_other_snapshots=False):
@@ -243,40 +253,54 @@
         while index is not None and index < len(self.snapshots) - 1:
             index = index + 1
             if also_other_snapshots or self.snapshots[index].is_ours():
                 return self.snapshots[index]
         return None
 
     @CachedProperty
+    def exists_check(self):
+        """check on disk if it exists"""
+        self.debug("Checking if dataset exists")
+        return (len(self.zfs_node.run(tab_split=True, cmd=["zfs", "list", self.name], readonly=True,
+                                      valid_exitcodes=[0, 1],
+                                      hide_errors=True)) > 0)
+
+    @property
     def exists(self):
-        """check if dataset exists. Use force to force a specific value to be
-        cached, if you already know. Useful for performance reasons
+        """returns True if dataset should exist.
+           Use force_exists to force a specific value, if you already know. Useful for performance and test reasons
         """
 
         if self.force_exists is not None:
-            self.debug("Checking if filesystem exists: was forced to {}".format(self.force_exists))
+            if self.force_exists:
+                self.debug("Dataset should exist")
+            else:
+                self.debug("Dataset should not exist")
             return self.force_exists
         else:
-            self.debug("Checking if filesystem exists")
-
-        return (self.zfs_node.run(tab_split=True, cmd=["zfs", "list", self.name], readonly=True, valid_exitcodes=[0, 1],
-                                  hide_errors=True) and True)
+            return self.exists_check
 
-    def create_filesystem(self, parents=False):
+    def create_filesystem(self, parents=False, unmountable=True):
         """create a filesystem
 
         Args:
             :type parents: bool
         """
-        if parents:
-            self.verbose("Creating filesystem and parents")
-            self.zfs_node.run(["zfs", "create", "-p", self.name])
-        else:
-            self.verbose("Creating filesystem")
-            self.zfs_node.run(["zfs", "create", self.name])
+
+        # recurse up
+        if parents and self.parent and not self.parent.exists:
+            self.parent.create_filesystem(parents, unmountable)
+
+        cmd = ["zfs", "create"]
+
+        if unmountable:
+            cmd.extend(["-o", "canmount=off"])
+
+        cmd.append(self.name)
+        self.zfs_node.run(cmd)
 
         self.force_exists = True
 
     def destroy(self, fail_exception=False, deferred=False, verbose=True):
         """destroy the dataset. by default failures are not an exception, so we
         can continue making backups
 
@@ -311,17 +335,14 @@
     def properties(self):
         """all zfs properties"""
 
         cmd = [
             "zfs", "get", "-H", "-o", "property,value", "-p", "all", self.name
         ]
 
-        if not self.exists:
-            return {}
-
         self.debug("Getting zfs properties")
 
         ret = {}
         for pair in self.zfs_node.run(tab_split=True, cmd=cmd, readonly=True, valid_exitcodes=[0]):
             if len(pair) == 2:
                 ret[pair[0]] = pair[1]
 
@@ -334,15 +355,14 @@
             :type min_changed_bytes: int
         """
         self.debug("Checking if dataset is changed")
 
         if min_changed_bytes == 0:
             return True
 
-
         if int(self.properties['written']) < min_changed_bytes:
             return False
         else:
             return True
 
     def is_ours(self):
         """return true if this snapshot name has format"""
@@ -351,15 +371,15 @@
         except ValueError as e:
             return False
 
         return True
 
     @property
     def holds(self):
-        """get list of holds for dataset"""
+        """get list[holds] for dataset"""
 
         output = self.zfs_node.run(["zfs", "holds", "-H", self.name], valid_exitcodes=[0], tab_split=True,
                                    readonly=True)
         return map(lambda fields: fields[1], output)
 
     def is_hold(self):
         """did we hold this snapshot?"""
@@ -394,23 +414,23 @@
             # we must adjust for that here.
             if self.zfs_node.utc:
                 seconds = (dt - datetime(1970, 1, 1)).total_seconds()
             else:
                 seconds = time.mktime(dt.timetuple())
         return seconds
 
-    def from_names(self, names):
-        """convert a list of names to a list ZfsDatasets for this zfs_node
+    def from_names(self, names, force_exists=None):
+        """convert a list[names] to a list ZfsDatasets for this zfs_node
 
         Args:
-            :type names: list of str
+            :type names: list[str]
         """
         ret = []
         for name in names:
-            ret.append(self.zfs_node.get_dataset(name))
+            ret.append(self.zfs_node.get_dataset(name, force_exists))
 
         return ret
 
     # def add_virtual_snapshot(self, snapshot):
     #     """pretend a snapshot exists (usefull in test mode)"""
     #
     #     # NOTE: we could just call self.snapshots.append() but this would trigger a zfs list which is not always needed.
@@ -421,30 +441,33 @@
     #     else:
     #         # self.snapshots will add it when requested
     #         print ("ADDED VIRT")
     #         self._virtual_snapshots.append(snapshot)
 
     @CachedProperty
     def snapshots(self):
-        """get all snapshots of this dataset"""
+        """get all snapshots of this dataset
+        :rtype: ZfsDataset
+        """
 
+        #FIXME: dont check for existance. (currenlty needed for _add_virtual_snapshots)
         if not self.exists:
             return []
 
         self.debug("Getting snapshots")
 
         cmd = [
             "zfs", "list", "-d", "1", "-r", "-t", "snapshot", "-H", "-o", "name", self.name
         ]
 
-        return self.from_names(self.zfs_node.run(cmd=cmd, readonly=True))
+        return self.from_names(self.zfs_node.run(cmd=cmd, readonly=True), force_exists=True)
 
     @property
     def our_snapshots(self):
-        """get list of snapshots creates by us of this dataset"""
+        """get list[snapshots] creates by us of this dataset"""
         ret = []
         for snapshot in self.snapshots:
             if snapshot.is_ours():
                 ret.append(snapshot)
 
         return ret
 
@@ -531,15 +554,15 @@
 
         self.debug("Getting all recursive datasets under us")
 
         names = self.zfs_node.run(tab_split=False, readonly=True, valid_exitcodes=[0], cmd=[
             "zfs", "list", "-r", "-t", types, "-o", "name", "-H", self.name
         ])
 
-        return self.from_names(names[1:])
+        return self.from_names(names[1:], force_exists=True)
 
     @CachedProperty
     def datasets(self, types="filesystem,volume"):
         """get all (non-snapshot) datasets directly under us
 
         Args:
             :type types: str
@@ -547,89 +570,92 @@
 
         self.debug("Getting all datasets under us")
 
         names = self.zfs_node.run(tab_split=False, readonly=True, valid_exitcodes=[0], cmd=[
             "zfs", "list", "-r", "-t", types, "-o", "name", "-H", "-d", "1", self.name
         ])
 
-        return self.from_names(names[1:])
+        return self.from_names(names[1:], force_exists=True)
 
-    def send_pipe(self, features, prev_snapshot, resume_token, show_progress, raw, send_properties, write_embedded, send_pipes, zfs_compressed):
+    def send_pipe(self, features, prev_snapshot, resume_token, show_progress, raw, send_properties, write_embedded,
+                  send_pipes, zfs_compressed):
         """returns a pipe with zfs send output for this snapshot
 
         resume_token: resume sending from this token. (in that case we don't
         need to know snapshot names)
 
         Args:
             :param send_pipes: output cmd array that will be added to actual zfs send command. (e.g. mbuffer or compression program)
-            :type send_pipes: list of str
-            :type features: list of str
+            :type send_pipes: list[str]
+            :type features: list[str]
             :type prev_snapshot: ZfsDataset
             :type resume_token: str
             :type show_progress: bool
             :type raw: bool
         """
         # build source command
         cmd = []
 
         cmd.extend(["zfs", "send", ])
 
         # all kind of performance options:
         if 'large_blocks' in features and "-L" in self.zfs_node.supported_send_options:
-            cmd.append("--large-block")  # large block support (only if recordsize>128k which is seldomly used)
+            # large block support (only if recordsize>128k which is seldomly used)
+            cmd.append("-L")  # --large-block
 
         if write_embedded and 'embedded_data' in features and "-e" in self.zfs_node.supported_send_options:
-            cmd.append("--embed")  # WRITE_EMBEDDED, more compact stream
+            cmd.append("-e")  # --embed; WRITE_EMBEDDED, more compact stream
 
         if zfs_compressed and "-c" in self.zfs_node.supported_send_options:
-            cmd.append("--compressed")  # use compressed WRITE records
+            cmd.append("-c")  # --compressed; use compressed WRITE records
 
         # raw? (send over encrypted data in its original encrypted form without decrypting)
         if raw:
             cmd.append("--raw")
 
         # progress output
         if show_progress:
-            cmd.append("--verbose")
-            cmd.append("--parsable")
+            cmd.append("-v")  # --verbose
+            cmd.append("-P")  # --parsable
 
         # resume a previous send? (don't need more parameters in that case)
         if resume_token:
             cmd.extend(["-t", resume_token])
 
         else:
             # send properties
             if send_properties:
-                cmd.append("--props")
+                cmd.append("-p")  # --props
 
             # incremental?
             if prev_snapshot:
                 cmd.extend(["-i", "@" + prev_snapshot.snapshot_name])
 
             cmd.append(self.name)
 
         cmd.extend(send_pipes)
 
         output_pipe = self.zfs_node.run(cmd, pipe=True, readonly=True)
 
         return output_pipe
 
-    def recv_pipe(self, pipe, features, recv_pipes, filter_properties=None, set_properties=None, ignore_exit_code=False, force=False):
+    def recv_pipe(self, pipe, features, recv_pipes, filter_properties=None, set_properties=None, ignore_exit_code=False,
+                  force=False):
         """starts a zfs recv for this snapshot and uses pipe as input
 
         note: you can it both on a snapshot or filesystem object. The
         resulting zfs command is the same, only our object cache is invalidated
         differently.
 
         Args:
             :param recv_pipes: input cmd array that will be prepended to actual zfs recv command. (e.g. mbuffer or decompression program)
             :type pipe: subprocess.pOpen
-            :type features: list of str
-            :type filter_properties: list of str
-            :type set_properties: list of str
+            :type features: list[str]
+            :type filter_properties: list[str]
+            :type set_properties: list[str]
             :type ignore_exit_code: bool
         """
 
         if set_properties is None:
             set_properties = []
 
         if filter_properties is None:
@@ -638,15 +664,15 @@
         # build target command
         cmd = []
 
         cmd.extend(recv_pipes)
 
         cmd.extend(["zfs", "recv"])
 
-        # don't mount filesystem that is received
+        # don't let zfs recv mount everything thats received (even with canmount=noauto!)
         cmd.append("-u")
 
         for property_ in filter_properties:
             cmd.extend(["-x", property_])
 
         for property_ in set_properties:
             cmd.extend(["-o", property_])
@@ -668,71 +694,107 @@
             valid_exitcodes = []
         else:
             valid_exitcodes = [0]
 
         # self.zfs_node.reset_progress()
         self.zfs_node.run(cmd, inp=pipe, valid_exitcodes=valid_exitcodes)
 
-        # invalidate cache, but we at least know we exist now
+        # invalidate cache
         self.invalidate()
 
         # in test mode we assume everything was ok and it exists
         if self.zfs_node.readonly:
             self.force_exists = True
 
         # check if transfer was really ok (exit codes have been wrong before due to bugs in zfs-utils and some
         # errors should be ignored, thats where the ignore_exitcodes is for.)
         if not self.exists:
             self.error("error during transfer")
             raise (Exception("Target doesn't exist after transfer, something went wrong."))
 
+        # at this point we're sure the actual dataset exists
+        self.parent.force_exists = True
+
+    def automount(self):
+        """Mount the dataset as if one did a zfs mount -a, but only for this dataset
+        Failure to mount doesnt result in an exception, but outputs errors to STDERR.
+
+        """
+
+        self.debug("Auto mounting")
+
+        if self.properties['type'] != "filesystem":
+            return
+
+        if self.properties['canmount'] != 'on':
+            return
+
+        if self.properties['mountpoint'] == 'legacy':
+            return
+
+        if self.properties['mountpoint'] == 'none':
+            return
+
+        if self.properties['encryption'] != 'off' and self.properties['keystatus'] == 'unavailable':
+            return
+
+        self.zfs_node.run(["zfs", "mount", self.name], valid_exitcodes=[0,1])
+
     def transfer_snapshot(self, target_snapshot, features, prev_snapshot, show_progress,
                           filter_properties, set_properties, ignore_recv_exit_code, resume_token,
                           raw, send_properties, write_embedded, send_pipes, recv_pipes, zfs_compressed, force):
         """transfer this snapshot to target_snapshot. specify prev_snapshot for
         incremental transfer
 
         connects a send_pipe() to recv_pipe()
 
         Args:
-            :type send_pipes: list of str
-            :type recv_pipes: list of str
+            :type send_pipes: list[str]
+            :type recv_pipes: list[str]
             :type target_snapshot: ZfsDataset
-            :type features: list of str
+            :type features: list[str]
             :type prev_snapshot: ZfsDataset
             :type show_progress: bool
-            :type filter_properties: list of str
-            :type set_properties: list of str
+            :type filter_properties: list[str]
+            :type set_properties: list[str]
             :type ignore_recv_exit_code: bool
             :type resume_token: str
             :type raw: bool
         """
 
         if set_properties is None:
             set_properties = []
         if filter_properties is None:
             filter_properties = []
 
         self.debug("Transfer snapshot to {}".format(target_snapshot.filesystem_name))
 
         if resume_token:
-            target_snapshot.verbose("resuming")
+            self.verbose("resuming")
 
         # initial or increment
         if not prev_snapshot:
-            target_snapshot.verbose("receiving full".format(self.snapshot_name))
+            self.verbose("-> {} (new)".format(target_snapshot.filesystem_name))
         else:
             # incremental
-            target_snapshot.verbose("receiving incremental".format(self.snapshot_name))
+            self.verbose("-> {}".format(target_snapshot.filesystem_name))
 
         # do it
         pipe = self.send_pipe(features=features, show_progress=show_progress, prev_snapshot=prev_snapshot,
-                              resume_token=resume_token, raw=raw, send_properties=send_properties, write_embedded=write_embedded, send_pipes=send_pipes, zfs_compressed=zfs_compressed)
+                              resume_token=resume_token, raw=raw, send_properties=send_properties,
+                              write_embedded=write_embedded, send_pipes=send_pipes, zfs_compressed=zfs_compressed)
         target_snapshot.recv_pipe(pipe, features=features, filter_properties=filter_properties,
-                                  set_properties=set_properties, ignore_exit_code=ignore_recv_exit_code, recv_pipes=recv_pipes, force=force)
+                                  set_properties=set_properties, ignore_exit_code=ignore_recv_exit_code,
+                                  recv_pipes=recv_pipes, force=force)
+
+        # try to automount it, if its the initial transfer
+        if not prev_snapshot:
+            # in test mode it doesnt actually exist, so dont try to mount it/read properties
+            if not target_snapshot.zfs_node.readonly:
+                target_snapshot.parent.automount()
 
     def abort_resume(self):
         """abort current resume state"""
         self.debug("Aborting resume")
         self.zfs_node.run(["zfs", "recv", "-A", self.name])
 
     def rollback(self):
@@ -766,24 +828,24 @@
                 snapshot = self.zfs_node.get_dataset(self.filesystem_name + "@" + snapshot_name)
                 snapshot.debug("resume token belongs to this snapshot")
                 return snapshot
 
         return None
 
     def thin_list(self, keeps=None, ignores=None):
-        """determines list of snapshots that should be kept or deleted based on
+        """determines list[snapshots] that should be kept or deleted based on
         the thinning schedule. cull the herd!
 
         returns: ( keeps, obsoletes )
 
         Args:
-            :param keeps: list of snapshots to always keep (usually the last)
+            :param keeps: list[snapshots] to always keep (usually the last)
             :param ignores: snapshots to completely ignore (usually incompatible target snapshots that are going to be destroyed anyway)
-            :type keeps: list of ZfsDataset
-            :type ignores: list of ZfsDataset
+            :type keeps: list[ZfsDataset]
+            :type ignores: list[ZfsDataset]
         """
 
         if ignores is None:
             ignores = []
         if keeps is None:
             keeps = []
 
@@ -802,31 +864,37 @@
         for obsolete in obsoletes:
             if skip_holds and obsolete.is_hold():
                 obsolete.verbose("Keeping (common snapshot)")
             else:
                 obsolete.destroy()
                 self.snapshots.remove(obsolete)
 
-    def find_common_snapshot(self, target_dataset):
+    def find_common_snapshot(self, target_dataset, guid_check):
         """find latest common snapshot between us and target returns None if its
         an initial transfer
 
         Args:
+            :type guid_check: bool
             :type target_dataset: ZfsDataset
         """
+
         if not target_dataset.snapshots:
             # target has nothing yet
             return None
         else:
             for source_snapshot in reversed(self.snapshots):
-                if target_dataset.find_snapshot(source_snapshot):
-                    source_snapshot.debug("common snapshot")
-                    return source_snapshot
-            target_dataset.error("Cant find common snapshot with source.")
-            raise (Exception("You probably need to delete the target dataset to fix this."))
+                target_snapshot = target_dataset.find_snapshot(source_snapshot)
+                if target_snapshot:
+                    if guid_check and source_snapshot.properties['guid'] != target_snapshot.properties['guid']:
+                        target_snapshot.warning("Common snapshot has invalid guid, ignoring.")
+                    else:
+                        target_snapshot.debug("common snapshot")
+                        return source_snapshot
+            # target_dataset.error("Cant find common snapshot with source.")
+            raise (Exception("Cant find common snapshot with target."))
 
     def find_start_snapshot(self, common_snapshot, also_other_snapshots):
         """finds first snapshot to send :rtype: ZfsDataset or None if we cant
         find it.
 
         Args:
             :type common_snapshot: ZfsDataset
@@ -845,40 +913,43 @@
                     start_snapshot = self.find_next_snapshot(start_snapshot, also_other_snapshots)
         else:
             # normal situation: start_snapshot is the one after the common snapshot
             start_snapshot = self.find_next_snapshot(common_snapshot, also_other_snapshots)
 
         return start_snapshot
 
-    def find_incompatible_snapshots(self, common_snapshot):
-        """returns a list of snapshots that is incompatible for a zfs recv onto
+    def find_incompatible_snapshots(self, common_snapshot, raw):
+        """returns a list[snapshots] that is incompatible for a zfs recv onto
         the common_snapshot. all direct followup snapshots with written=0 are
         compatible.
 
+        in raw-mode nothing is compatible. issue #219
+
         Args:
             :type common_snapshot: ZfsDataset
+            :type raw: bool
         """
 
         ret = []
 
         if common_snapshot and self.snapshots:
             followup = True
             for snapshot in self.snapshots[self.find_snapshot_index(common_snapshot) + 1:]:
-                if not followup or int(snapshot.properties['written']) != 0:
+                if raw or not followup or int(snapshot.properties['written']) != 0:
                     followup = False
                     ret.append(snapshot)
 
         return ret
 
     def get_allowed_properties(self, filter_properties, set_properties):
         """only returns lists of allowed properties for this dataset type
 
         Args:
-            :type filter_properties: list of str
-            :type set_properties: list of str
+            :type filter_properties: list[str]
+            :type set_properties: list[str]
         """
 
         allowed_filter_properties = []
         allowed_set_properties = []
         illegal_properties = self.ILLEGAL_PROPERTIES[self.properties['type']]
         for set_property in set_properties:
             (property_, value) = set_property.split("=")
@@ -902,27 +973,28 @@
         """
 
         self.debug("Creating virtual target snapshots")
         snapshot = source_start_snapshot
         while snapshot:
             # create virtual target snapsho
             # NOTE: with force_exist we're telling the dataset it doesnt exist yet. (e.g. its virtual)
-            virtual_snapshot = self.zfs_node.get_dataset(self.filesystem_name + "@" + snapshot.snapshot_name, force_exists=False)
+            virtual_snapshot = self.zfs_node.get_dataset(self.filesystem_name + "@" + snapshot.snapshot_name,
+                                                         force_exists=False)
             self.snapshots.append(virtual_snapshot)
             snapshot = source_dataset.find_next_snapshot(snapshot, also_other_snapshots)
 
     def _pre_clean(self, common_snapshot, target_dataset, source_obsoletes, target_obsoletes, target_keeps):
         """cleanup old stuff before starting snapshot syncing
 
         Args:
             :type common_snapshot: ZfsDataset
             :type target_dataset: ZfsDataset
-            :type source_obsoletes: list of ZfsDataset
-            :type target_obsoletes: list of ZfsDataset
-            :type target_keeps: list of ZfsDataset
+            :type source_obsoletes: list[ZfsDataset]
+            :type target_obsoletes: list[ZfsDataset]
+            :type target_keeps: list[ZfsDataset]
         """
 
         # on source: destroy all obsoletes before common. (since we cant send them anyways)
         # But after common, only delete snapshots that target also doesn't want
         if common_snapshot:
             before_common = True
         else:
@@ -936,54 +1008,56 @@
                 target_snapshot = target_dataset.find_snapshot(source_snapshot)
                 if (source_snapshot in source_obsoletes) and (before_common or (target_snapshot not in target_keeps)):
                     source_snapshot.destroy()
 
         # on target: destroy everything thats obsolete, except common_snapshot
         for target_snapshot in target_dataset.snapshots:
             if (target_snapshot in target_obsoletes) \
-                    and ( not common_snapshot or (target_snapshot.snapshot_name != common_snapshot.snapshot_name)):
+                    and (not common_snapshot or (target_snapshot.snapshot_name != common_snapshot.snapshot_name)):
                 if target_snapshot.exists:
                     target_snapshot.destroy()
 
     def _validate_resume_token(self, target_dataset, start_snapshot):
         """validate and get (or destory) resume token
 
         Args:
             :type target_dataset: ZfsDataset
             :type start_snapshot: ZfsDataset
         """
 
-        if 'receive_resume_token' in target_dataset.properties:
-            if start_snapshot==None:
+        if target_dataset.exists and 'receive_resume_token' in target_dataset.properties:
+            if start_snapshot == None:
                 target_dataset.verbose("Aborting resume, its obsolete.")
                 target_dataset.abort_resume()
             else:
                 resume_token = target_dataset.properties['receive_resume_token']
                 # not valid anymore
                 resume_snapshot = self.get_resume_snapshot(resume_token)
                 if not resume_snapshot or start_snapshot.snapshot_name != resume_snapshot.snapshot_name:
                     target_dataset.verbose("Aborting resume, its no longer valid.")
                     target_dataset.abort_resume()
                 else:
                     return resume_token
 
-    def _plan_sync(self, target_dataset, also_other_snapshots):
+    def _plan_sync(self, target_dataset, also_other_snapshots, guid_check, raw):
         """plan where to start syncing and what to sync and what to keep
 
         Args:
-            :rtype: ( ZfsDataset, ZfsDataset, list of ZfsDataset, list of ZfsDataset, list of ZfsDataset, list of ZfsDataset )
+            :rtype: ( ZfsDataset, ZfsDataset, list[ZfsDataset], list[ZfsDataset], list[ZfsDataset], list[ZfsDataset] )
             :type target_dataset: ZfsDataset
             :type also_other_snapshots: bool
+            :type guid_check: bool
+            :type raw: bool
         """
 
         # determine common and start snapshot
         target_dataset.debug("Determining start snapshot")
-        common_snapshot = self.find_common_snapshot(target_dataset)
+        common_snapshot = self.find_common_snapshot(target_dataset, guid_check=guid_check)
         start_snapshot = self.find_start_snapshot(common_snapshot, also_other_snapshots)
-        incompatible_target_snapshots = target_dataset.find_incompatible_snapshots(common_snapshot)
+        incompatible_target_snapshots = target_dataset.find_incompatible_snapshots(common_snapshot, raw)
 
         # let thinner decide whats obsolete on source
         source_obsoletes = []
         if self.our_snapshots:
             source_obsoletes = self.thin_list(keeps=[self.our_snapshots[-1]])[1]
 
         # let thinner decide keeps/obsoletes on target, AFTER the transfer would be done (by using virtual snapshots)
@@ -997,58 +1071,76 @@
         return common_snapshot, start_snapshot, source_obsoletes, target_obsoletes, target_keeps, incompatible_target_snapshots
 
     def handle_incompatible_snapshots(self, incompatible_target_snapshots, destroy_incompatible):
         """destroy incompatbile snapshots on target before sync, or inform user
         what to do
 
         Args:
-            :type incompatible_target_snapshots: list of ZfsDataset
+            :type incompatible_target_snapshots: list[ZfsDataset]
             :type destroy_incompatible: bool
         """
 
         if incompatible_target_snapshots:
             if not destroy_incompatible:
                 for snapshot in incompatible_target_snapshots:
                     snapshot.error("Incompatible snapshot")
-                raise (Exception("Please destroy incompatible snapshots or use --destroy-incompatible."))
+                raise (Exception("Please destroy incompatible snapshots on target, or use --destroy-incompatible."))
             else:
                 for snapshot in incompatible_target_snapshots:
                     snapshot.verbose("Incompatible snapshot")
-                    snapshot.destroy()
+                    snapshot.destroy(fail_exception=True)
                     self.snapshots.remove(snapshot)
 
+                if len(incompatible_target_snapshots) > 0:
+                    self.rollback()
 
     def sync_snapshots(self, target_dataset, features, show_progress, filter_properties, set_properties,
                        ignore_recv_exit_code, holds, rollback, decrypt, encrypt, also_other_snapshots,
-                       no_send, destroy_incompatible, send_pipes, recv_pipes, zfs_compressed, force):
+                       no_send, destroy_incompatible, send_pipes, recv_pipes, zfs_compressed, force, guid_check):
         """sync this dataset's snapshots to target_dataset, while also thinning
         out old snapshots along the way.
 
         Args:
-            :type send_pipes: list of str
-            :type recv_pipes: list of str
+            :type send_pipes: list[str]
+            :type recv_pipes: list[str]
             :type target_dataset: ZfsDataset
-            :type features: list of str
+            :type features: list[str]
             :type show_progress: bool
-            :type filter_properties: list of str
-            :type set_properties: list of str
+            :type filter_properties: list[str]
+            :type set_properties: list[str]
             :type ignore_recv_exit_code: bool
             :type holds: bool
             :type rollback: bool
             :type decrypt: bool
             :type also_other_snapshots: bool
             :type no_send: bool
-            :type destroy_incompatible: bool
+            :type guid_check: bool
         """
 
-        self.verbose("sending to {}".format(target_dataset))
+        # self.verbose("-> {}".format(target_dataset))
+
+        # defaults for these settings if there is no encryption stuff going on:
+        send_properties = True
+        raw = False
+        write_embedded = True
+
+        # source dataset encrypted?
+        if self.properties.get('encryption', 'off') != 'off':
+            # user wants to send it over decrypted?
+            if decrypt:
+                # when decrypting, zfs cant send properties
+                send_properties = False
+            else:
+                # keep data encrypted by sending it raw (including properties)
+                raw = True
 
         (common_snapshot, start_snapshot, source_obsoletes, target_obsoletes, target_keeps,
          incompatible_target_snapshots) = \
-            self._plan_sync(target_dataset=target_dataset, also_other_snapshots=also_other_snapshots)
+            self._plan_sync(target_dataset=target_dataset, also_other_snapshots=also_other_snapshots,
+                            guid_check=guid_check, raw=raw)
 
         # NOTE: we do this because we dont want filesystems to fillup when backups keep failing.
         # Also usefull with no_send to still cleanup stuff.
         self._pre_clean(
             common_snapshot=common_snapshot, target_dataset=target_dataset,
             target_keeps=target_keeps, target_obsoletes=target_obsoletes, source_obsoletes=source_obsoletes)
 
@@ -1058,51 +1150,38 @@
         # now actually transfer the snapshots, if we want
         if no_send:
             return
 
         # check if we can resume
         resume_token = self._validate_resume_token(target_dataset, start_snapshot)
 
-        # rollback target to latest?
-        if rollback:
-            target_dataset.rollback()
-
-        #defaults for these settings if there is no encryption stuff going on:
-        send_properties = True
-        raw = False
-        write_embedded = True
-
-        (active_filter_properties, active_set_properties) = self.get_allowed_properties(filter_properties, set_properties)
-
-        # source dataset encrypted?
-        if self.properties.get('encryption', 'off')!='off':
-            # user wants to send it over decrypted?
-            if decrypt:
-                # when decrypting, zfs cant send properties
-                send_properties=False
-            else:
-                # keep data encrypted by sending it raw (including properties)
-                raw=True
+        (active_filter_properties, active_set_properties) = self.get_allowed_properties(filter_properties,
+                                                                                        set_properties)
 
         # encrypt at target?
         if encrypt and not raw:
             # filter out encryption properties to let encryption on the target take place
-            active_filter_properties.extend(["keylocation","pbkdf2iters","keyformat", "encryption"])
-            write_embedded=False
-
+            active_filter_properties.extend(["keylocation", "pbkdf2iters", "keyformat", "encryption"])
+            write_embedded = False
 
         # now actually transfer the snapshots
         prev_source_snapshot = common_snapshot
         source_snapshot = start_snapshot
+        do_rollback = rollback
         while source_snapshot:
             target_snapshot = target_dataset.find_snapshot(source_snapshot)  # still virtual
 
             # does target actually want it?
             if target_snapshot not in target_obsoletes:
 
+                # do the rollback, one time at first transfer
+                if do_rollback:
+                    target_dataset.rollback()
+                    do_rollback = False
+
                 source_snapshot.transfer_snapshot(target_snapshot, features=features,
                                                   prev_snapshot=prev_source_snapshot, show_progress=show_progress,
                                                   filter_properties=active_filter_properties,
                                                   set_properties=active_set_properties,
                                                   ignore_recv_exit_code=ignore_recv_exit_code,
                                                   resume_token=resume_token, write_embedded=write_embedded, raw=raw,
                                                   send_properties=send_properties, send_pipes=send_pipes,
@@ -1147,23 +1226,22 @@
 
         cmd = [
             "mount", "-tzfs", self.name, mount_point
         ]
 
         self.zfs_node.run(cmd=cmd, valid_exitcodes=[0])
 
-    def unmount(self):
+    def unmount(self, mount_point):
 
         self.debug("Unmounting")
 
         cmd = [
-            "umount", self.name
+            "umount", mount_point
         ]
 
-
         self.zfs_node.run(cmd=cmd, valid_exitcodes=[0])
 
     def clone(self, name):
         """clones this snapshot and returns ZfsDataset of the clone"""
 
         self.debug("Cloning to {}".format(name))
 
@@ -1196,8 +1274,7 @@
         cmd = [
             "zfs", "inherit", prop, self.name
         ]
 
         self.zfs_node.run(cmd=cmd, valid_exitcodes=[0])
 
         self.invalidate()
-
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ExecuteNode.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ExecuteNode.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/compressors.py` & `zfs_autobackup-3.3b3/zfs_autobackup/compressors.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/CliBase.py` & `zfs_autobackup-3.3b3/zfs_autobackup/CliBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class CliBase(object):
     """Base class for all cli programs
     Overridden in subclasses that add stuff for the specific programs."""
 
     # also used by setup.py
-    VERSION = "3.2-beta1"
+    VERSION = "3.3-beta.3"
     HEADER = "{} v{} - (c)2022 E.H.Eefting (edwin@datux.nl)".format(os.path.basename(sys.argv[0]), VERSION)
 
     def __init__(self, argv, print_arguments=True):
 
         self.parser=self.get_parser()
         self.args = self.parse_args(argv)
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsNode.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsNode.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .ExecuteNode import ExecuteNode
 from .Thinner import Thinner
 from .CachedProperty import CachedProperty
 from .ZfsPool import ZfsPool
 from .ZfsDataset import ZfsDataset
 from .ExecuteNode import ExecuteError
+from .util import datetime_now
 
 
 class ZfsNode(ExecuteNode):
     """a node that contains zfs datasets. implements global (systemwide/pool wide) zfs commands"""
 
     def __init__(self, logger, utc=False, snapshot_time_format="", hold_name="", ssh_config=None, ssh_to=None, readonly=False,
                  description="",
@@ -55,15 +56,16 @@
         self._progress_start_time = time.time()
 
         ExecuteNode.__init__(self, ssh_config=ssh_config, ssh_to=ssh_to, readonly=readonly, debug_output=debug_output)
 
     def thin(self, objects, keep_objects):
         # NOTE: if thinning is disabled with --no-thinning, self.__thinner will be none.
         if self.__thinner is not None:
-            return self.__thinner.thin(objects, keep_objects)
+
+            return self.__thinner.thin(objects, keep_objects, datetime_now(self.utc).timestamp())
         else:
             return (keep_objects, [])
 
     @CachedProperty
     def supported_send_options(self):
         """list of supported options, for optimizing sends"""
         # not every zfs implementation supports them all
@@ -231,30 +233,32 @@
             for cmd in post_snapshot_cmds:
                 self.verbose("Running post-snapshot-cmd")
                 try:
                     self.run(cmd=shlex.split(cmd), readonly=False)
                 except Exception as e:
                     pass
 
-    def selected_datasets(self, property_name, exclude_received, exclude_paths, exclude_unchanged, min_change):
+    def selected_datasets(self, property_name, exclude_received, exclude_paths, exclude_unchanged):
         """determine filesystems that should be backed up by looking at the special autobackup-property, systemwide
 
-           returns: list of ZfsDataset
+           returns: ( list of selected ZfsDataset, list of excluded ZfsDataset)
         """
 
         self.debug("Getting selected datasets")
 
         # get all source filesystems that have the backup property
         lines = self.run(tab_split=True, readonly=True, cmd=[
             "zfs", "get", "-t", "volume,filesystem", "-o", "name,value,source", "-H",
             property_name
         ])
 
+
         # The returnlist of selected ZfsDataset's:
         selected_filesystems = []
+        excluded_filesystems = []
 
         # list of sources, used to resolve inherited sources
         sources = {}
 
         for line in lines:
             (name, value, raw_source) = line
             dataset = self.get_dataset(name, force_exists=True)
@@ -266,13 +270,18 @@
                 inherited_from = re.sub("^inherited from ", "", raw_source)
                 source = sources[inherited_from]
             else:
                 inherited = False
                 source = raw_source
 
             # determine it
-            if dataset.is_selected(value=value, source=source, inherited=inherited, exclude_received=exclude_received,
-                                   exclude_paths=exclude_paths, exclude_unchanged=exclude_unchanged,
-                                   min_change=min_change):
+            selected=dataset.is_selected(value=value, source=source, inherited=inherited, exclude_received=exclude_received,
+                                   exclude_paths=exclude_paths, exclude_unchanged=exclude_unchanged)
+
+            if selected==True:
                 selected_filesystems.append(dataset)
+            elif selected==False:
+                excluded_filesystems.append(dataset)
+            #returns None when no property is set.
+
 
-        return selected_filesystems
+        return ( selected_filesystems, excluded_filesystems)
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ThinnerRule.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ThinnerRule.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/BlockHasher.py` & `zfs_autobackup-3.3b3/zfs_autobackup/BlockHasher.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsAutobackup.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsAutobackup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import time
 
 import argparse
-from datetime import datetime
 from signal import signal, SIGPIPE
-from .util import output_redir, sigpipe_handler
+from .util import output_redir, sigpipe_handler, datetime_now
 
 from .ZfsAuto import ZfsAuto
 
 from . import compressors
 from .ExecuteNode import ExecuteNode
 from .Thinner import Thinner
 from .ZfsDataset import ZfsDataset
@@ -29,23 +27,23 @@
 
         if not args.no_holds:
             self.verbose("Hold name                  : {}".format(self.hold_name))
 
         if args.allow_empty:
             args.min_change = 0
 
-        if args.destroy_incompatible:
-            args.rollback = True
+        # if args.destroy_incompatible:
+        #     args.rollback = True
 
         if args.resume:
-            self.warning("The --resume option isn't needed anymore (its autodetected now)")
+            self.warning("The --resume option isn't needed anymore (it's autodetected now)")
 
         if args.raw:
             self.warning(
-                "The --raw option isn't needed anymore (its autodetected now). Also see --encrypt and --decrypt.")
+                "The --raw option isn't needed anymore (it's autodetected now). Also see --encrypt and --decrypt.")
 
         if args.compress and args.ssh_source is None and args.ssh_target is None:
             self.warning("Using compression, but transfer is local.")
 
         if args.compress and args.zfs_compressed:
             self.warning("Using --compress with --zfs-compressed, might be inefficient.")
 
@@ -63,66 +61,70 @@
                            help='Run COMMAND before snapshotting (can be used multiple times.')
         group.add_argument('--post-snapshot-cmd', metavar="COMMAND", default=[], action='append',
                            help='Run COMMAND after snapshotting (can be used multiple times.')
         group.add_argument('--min-change', metavar='BYTES', type=int, default=1,
                            help='Only create snapshot if enough bytes are changed. (default %('
                                 'default)s)')
         group.add_argument('--allow-empty', action='store_true',
-                           help='If nothing has changed, still create empty snapshots. (Faster. Same as --min-change=0)')
+                           help='If nothing has changed, still create empty snapshots. (Same as --min-change=0)')
         group.add_argument('--other-snapshots', action='store_true',
                            help='Send over other snapshots as well, not just the ones created by this tool.')
         group.add_argument('--set-snapshot-properties', metavar='PROPERTY=VALUE,...', type=str,
                            help='List of properties to set on the snapshot.')
+        group.add_argument('--no-guid-check', action='store_true',
+                           help='Dont check guid of common snapshots. (faster)')
 
 
         group = parser.add_argument_group("Transfer options")
         group.add_argument('--no-send', action='store_true',
-                           help='Don\'t transfer snapshots (useful for cleanups, or if you want a serperate send-cronjob)')
+                           help='Don\'t transfer snapshots (useful for cleanups, or if you want a separate send-cronjob)')
         group.add_argument('--no-holds', action='store_true',
                            help='Don\'t hold snapshots. (Faster. Allows you to destroy common snapshot.)')
         group.add_argument('--clear-refreservation', action='store_true',
-                           help='Filter "refreservation" property. (recommended, safes space. same as '
+                           help='Filter "refreservation" property. (recommended, saves space. same as '
                                 '--filter-properties refreservation)')
         group.add_argument('--clear-mountpoint', action='store_true',
                            help='Set property canmount=noauto for new datasets. (recommended, prevents mount '
                                 'conflicts. same as --set-properties canmount=noauto)')
         group.add_argument('--filter-properties', metavar='PROPERTY,...', type=str,
                            help='List of properties to "filter" when receiving filesystems. (you can still restore '
                                 'them with zfs inherit -S)')
         group.add_argument('--set-properties', metavar='PROPERTY=VALUE,...', type=str,
                            help='List of propererties to override when receiving filesystems. (you can still restore '
                                 'them with zfs inherit -S)')
         group.add_argument('--rollback', action='store_true',
                            help='Rollback changes to the latest target snapshot before starting. (normally you can '
                                 'prevent changes by setting the readonly property on the target_path to on)')
         group.add_argument('--force', '-F', action='store_true',
-                           help='Use zfs -F option to force overwrite/rollback. (Usefull with --strip-path=1, but use with care)')
+                           help='Use zfs -F option to force overwrite/rollback. (Useful with --strip-path=1, but use with care)')
         group.add_argument('--destroy-incompatible', action='store_true',
-                           help='Destroy incompatible snapshots on target. Use with care! (implies --rollback)')
+                           help='Destroy incompatible snapshots on target. Use with care! (also does rollback of dataset)')
         group.add_argument('--ignore-transfer-errors', action='store_true',
                            help='Ignore transfer errors (still checks if received filesystem exists. useful for '
                                 'acltype errors)')
 
         group.add_argument('--decrypt', action='store_true',
                            help='Decrypt data before sending it over.')
         group.add_argument('--encrypt', action='store_true',
                            help='Encrypt data after receiving it.')
 
         group.add_argument('--zfs-compressed', action='store_true',
                            help='Transfer blocks that already have zfs-compression as-is.')
 
-        group = parser.add_argument_group("ZFS send/recv pipes")
+        group = parser.add_argument_group("Data transfer options")
         group.add_argument('--compress', metavar='TYPE', default=None, nargs='?', const='zstd-fast',
                            choices=compressors.choices(),
                            help='Use compression during transfer, defaults to zstd-fast if TYPE is not specified. ({})'.format(
                                ", ".join(compressors.choices())))
         group.add_argument('--rate', metavar='DATARATE', default=None,
-                           help='Limit data transfer rate (e.g. 128K. requires mbuffer.)')
+                           help='Limit data transfer rate in Bytes/sec (e.g. 128K. requires mbuffer.)')
         group.add_argument('--buffer', metavar='SIZE', default=None,
                            help='Add zfs send and recv buffers to smooth out IO bursts. (e.g. 128M. requires mbuffer)')
+        parser.add_argument('--buffer-chunk-size', metavar="BUFFERCHUNKSIZE", default=None,
+                            help='Tune chunk size when mbuffer is used. (requires mbuffer.)')
         group.add_argument('--send-pipe', metavar="COMMAND", default=[], action='append',
                            help='pipe zfs send output through COMMAND (can be used multiple times)')
         group.add_argument('--recv-pipe', metavar="COMMAND", default=[], action='append',
                            help='pipe zfs recv input through COMMAND (can be used multiple times)')
 
         group = parser.add_argument_group("Thinner options")
         group.add_argument('--no-thinning', action='store_true', help="Do not destroy any snapshots.")
@@ -138,22 +140,26 @@
         parser.add_argument('--resume', action='store_true', help=argparse.SUPPRESS)
         parser.add_argument('--raw', action='store_true', help=argparse.SUPPRESS)
 
         return parser
 
     # NOTE: this method also uses self.args. args that need extra processing are passed as function parameters:
     def thin_missing_targets(self, target_dataset, used_target_datasets):
-        """thin target datasets that are missing on the source."""
+        """thin target datasets that are missing on the source.
+        :type used_target_datasets: list[ZfsDataset]
+        :type target_dataset: ZfsDataset
+        """
 
         self.debug("Thinning obsolete datasets")
         missing_datasets = [dataset for dataset in target_dataset.recursive_datasets if
                             dataset not in used_target_datasets]
 
         count = 0
         for dataset in missing_datasets:
+            self.debug("analyse missing {}".format(dataset))
 
             count = count + 1
             if self.args.progress:
                 self.progress("Analysing missing {}/{}".format(count, len(missing_datasets)))
 
             try:
                 dataset.debug("Missing on source, thinning")
@@ -163,15 +169,19 @@
                 dataset.error("Error during thinning of missing datasets ({})".format(str(e)))
 
         # if self.args.progress:
         #     self.clear_progress()
 
     # NOTE: this method also uses self.args. args that need extra processing are passed as function parameters:
     def destroy_missing_targets(self, target_dataset, used_target_datasets):
-        """destroy target datasets that are missing on the source and that meet the requirements"""
+        """destroy target datasets that are missing on the source and that meet the requirements
+        :type used_target_datasets: list[ZfsDataset]
+        :type target_dataset: ZfsDataset
+
+        """
 
         self.debug("Destroying obsolete datasets")
 
         missing_datasets = [dataset for dataset in target_dataset.recursive_datasets if
                             dataset not in used_target_datasets]
 
         count = 0
@@ -185,19 +195,19 @@
                 # cant do anything without our own snapshots
                 if not dataset.our_snapshots:
                     if dataset.datasets:
                         # its not a leaf, just ignore
                         dataset.debug("Destroy missing: ignoring")
                     else:
                         dataset.verbose(
-                            "Destroy missing: has no snapshots made by us. (please destroy manually)")
+                            "Destroy missing: has no snapshots made by us (please destroy manually).")
                 else:
                     # past the deadline?
                     deadline_ttl = ThinnerRule("0s" + self.args.destroy_missing).ttl
-                    now = int(time.time())
+                    now = datetime_now(self.args.utc).timestamp()
                     if dataset.our_snapshots[-1].timestamp + deadline_ttl > now:
                         dataset.verbose("Destroy missing: Waiting for deadline.")
                     else:
 
                         dataset.debug("Destroy missing: Removing our snapshots.")
 
                         # remove all our snaphots, except last, to safe space in case we fail later on
@@ -230,19 +240,30 @@
         # if self.args.progress:
         #     self.clear_progress()
 
     def get_send_pipes(self, logger):
         """determine the zfs send pipe"""
 
         ret = []
+        _mbuffer = False
+        _buffer = "16M"
+        _cs = "128k"
+        _rate = False
 
         # IO buffer
         if self.args.buffer:
             logger("zfs send buffer        : {}".format(self.args.buffer))
-            ret.extend([ExecuteNode.PIPE, "mbuffer", "-q", "-s128k", "-m" + self.args.buffer])
+            _mbuffer = True
+            _buffer = self.args.buffer
+
+        # IO chunk size
+        if self.args.buffer_chunk_size:
+            logger("zfs send chunk size    : {}".format(self.args.buffer_chunk_size))
+            _mbuffer = True
+            _cs = self.args.buffer_chunk_size
 
         # custom pipes
         for send_pipe in self.args.send_pipe:
             ret.append(ExecuteNode.PIPE)
             ret.extend(send_pipe.split(" "))
             logger("zfs send custom pipe   : {}".format(send_pipe))
 
@@ -252,15 +273,22 @@
             cmd = compressors.compress_cmd(self.args.compress)
             ret.extend(cmd)
             logger("zfs send compression   : {}".format(" ".join(cmd)))
 
         # transfer rate
         if self.args.rate:
             logger("zfs send transfer rate : {}".format(self.args.rate))
-            ret.extend([ExecuteNode.PIPE, "mbuffer", "-q", "-s128k", "-m16M", "-R" + self.args.rate])
+            _mbuffer = True
+            _rate = self.args.rate
+
+        if _mbuffer:
+            cmd = [ExecuteNode.PIPE, "mbuffer", "-q", "-s{}".format(_cs), "-m{}".format(_buffer)]
+            if _rate:
+                cmd.append("-R{}".format(self.args.rate))
+            ret.extend(cmd)
 
         return ret
 
     def get_recv_pipes(self, logger):
 
         ret = []
 
@@ -274,19 +302,27 @@
         # custom pipes
         for recv_pipe in self.args.recv_pipe:
             ret.extend(recv_pipe.split(" "))
             ret.append(ExecuteNode.PIPE)
             logger("zfs recv custom pipe   : {}".format(recv_pipe))
 
         # IO buffer
-        if self.args.buffer:
+        if self.args.buffer or self.args.buffer_chunk_size:
+            _cs = "128k"
+            _buffer = "16M"
             # only add second buffer if its usefull. (e.g. non local transfer or other pipes active)
             if self.args.ssh_source != None or self.args.ssh_target != None or self.args.recv_pipe or self.args.send_pipe or self.args.compress != None:
                 logger("zfs recv buffer        : {}".format(self.args.buffer))
-                ret.extend(["mbuffer", "-q", "-s128k", "-m" + self.args.buffer, ExecuteNode.PIPE])
+
+                if self.args.buffer_chunk_size:
+                    _cs = self.args.buffer_chunk_size
+                if self.args.buffer:
+                    _buffer = self.args.buffer
+
+                ret.extend(["mbuffer", "-q", "-s{}".format(_cs), "-m{}".format(_buffer), ExecuteNode.PIPE])
 
         return ret
 
     def make_target_name(self, source_dataset):
         """make target_name from a source_dataset"""
         stripped=source_dataset.lstrip_path(self.args.strip_path)
         if stripped!="":
@@ -338,14 +374,15 @@
 
                 # ensure parents exists
                 # TODO: this isnt perfect yet, in some cases it can create parents when it shouldn't.
                 if not self.args.no_send \
                         and target_dataset.parent \
                         and target_dataset.parent not in target_datasets \
                         and not target_dataset.parent.exists:
+                    target_dataset.debug("Creating unmountable parents")
                     target_dataset.parent.create_filesystem(parents=True)
 
                 # determine common zpool features (cached, so no problem we call it often)
                 source_features = source_node.get_pool(source_dataset).features
                 target_features = target_node.get_pool(target_dataset).features
                 common_features = source_features and target_features
 
@@ -356,27 +393,23 @@
                                               ignore_recv_exit_code=self.args.ignore_transfer_errors,
                                               holds=not self.args.no_holds, rollback=self.args.rollback,
                                               also_other_snapshots=self.args.other_snapshots,
                                               no_send=self.args.no_send,
                                               destroy_incompatible=self.args.destroy_incompatible,
                                               send_pipes=send_pipes, recv_pipes=recv_pipes,
                                               decrypt=self.args.decrypt, encrypt=self.args.encrypt,
-                                              zfs_compressed=self.args.zfs_compressed, force=self.args.force)
+                                              zfs_compressed=self.args.zfs_compressed, force=self.args.force, guid_check=not self.args.no_guid_check)
             except Exception as e:
-                # if self.args.progress:
-                #     self.clear_progress()
 
                 fail_count = fail_count + 1
                 source_dataset.error("FAILED: " + str(e))
                 if self.args.debug:
                     self.verbose("Debug mode, aborting on first error")
                     raise
 
-        # if self.args.progress:
-        #     self.clear_progress()
 
         target_path_dataset = target_node.get_dataset(self.args.target_path)
         if not self.args.no_thinning:
             self.thin_missing_targets(target_dataset=target_path_dataset, used_target_datasets=target_datasets)
 
         if self.args.destroy_missing is not None:
             self.destroy_missing_targets(target_dataset=target_path_dataset, used_target_datasets=target_datasets)
@@ -439,28 +472,26 @@
                                   snapshot_time_format=self.snapshot_time_format, hold_name=self.hold_name, logger=self,
                                   ssh_config=self.args.ssh_config,
                                   ssh_to=self.args.ssh_source, readonly=self.args.test,
                                   debug_output=self.args.debug_output, description=description, thinner=source_thinner)
 
             ################# select source datasets
             self.set_title("Selecting")
-            source_datasets = source_node.selected_datasets(property_name=self.property_name,
+            ( source_datasets, excluded_datasets) = source_node.selected_datasets(property_name=self.property_name,
                                                             exclude_received=self.args.exclude_received,
                                                             exclude_paths=self.exclude_paths,
-                                                            exclude_unchanged=self.args.exclude_unchanged,
-                                                            min_change=self.args.min_change)
-            if not source_datasets:
+                                                            exclude_unchanged=self.args.exclude_unchanged)
+            if not source_datasets and not excluded_datasets:
                 self.print_error_sources()
                 return 255
 
             ################# snapshotting
             if not self.args.no_snapshot:
                 self.set_title("Snapshotting")
-                dt = datetime.utcnow() if self.args.utc else datetime.now()
-                snapshot_name = dt.strftime(self.snapshot_time_format)
+                snapshot_name = datetime_now(self.args.utc).strftime(self.snapshot_time_format)
                 source_node.consistent_snapshot(source_datasets, snapshot_name,
                                                 min_changed_bytes=self.args.min_change,
                                                 pre_snapshot_cmds=self.args.pre_snapshot_cmd,
                                                 post_snapshot_cmds=self.args.post_snapshot_cmd,
                                                 set_snapshot_properties=self.set_snapshot_properties_list())
 
             ################# sync
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/CmdPipe.py` & `zfs_autobackup-3.3b3/zfs_autobackup/CmdPipe.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/ZfsCheck.py` & `zfs_autobackup-3.3b3/zfs_autobackup/ZfsCheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self.debug("Create temporary mount point {}".format(mnt))
         self.node.run(["mkdir", mnt])
         snapshot.mount(mnt)
         return mnt
 
     def cleanup_zfs_filesystem(self, snapshot):
         mnt = "/tmp/" + tmp_name()
-        snapshot.unmount()
+        snapshot.unmount(mnt)
         self.debug("Cleaning up temporary mount point")
         self.node.run(["rmdir", mnt], hide_errors=True, valid_exitcodes=[])
 
     # NOTE: https://www.google.com/search?q=Mount+Path+Limit+freebsd
     # Freebsd has limitations regarding path length, so we have to clone it so the part stays sort
     def prepare_zfs_volume(self, snapshot):
         """clone volume, waits and tries to findout /dev path to the volume, in a compatible way. (linux/freebsd/smartos)"""
@@ -102,15 +102,15 @@
 
                 # fake it in testmode
                 if self.args.test:
                     return location
 
             time.sleep(1)
 
-        raise (Exception("Timeout while waiting for /dev entry to appear. (looking in: {})".format(locations)))
+        raise (Exception("Timeout while waiting for /dev entry to appear. (looking in: {}). Hint: did you forget to load the encryption key?".format(locations)))
 
     def cleanup_zfs_volume(self, snapshot):
         """destroys temporary volume snapshot"""
         clone_name = get_tmp_clone_name(snapshot)
         clone = snapshot.zfs_node.get_dataset(clone_name)
         clone.destroy(deferred=True, verbose=False)
```

### Comparing `zfs_autobackup-3.2b1/zfs_autobackup/util.py` & `zfs_autobackup-3.3b3/zfs_autobackup/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-# root@psyt14s:/home/psy/zfs_autobackup# ls -lh /home/psy/Downloads/carimage.zip
-# -rw-rw-r-- 1 psy psy 990M Nov 26  2020 /home/psy/Downloads/carimage.zip
-# root@psyt14s:/home/psy/zfs_autobackup# time sha1sum /home/psy/Downloads/carimage.zip
-# a682e1a36e16fe0d0c2f011104f4a99004f19105  /home/psy/Downloads/carimage.zip
-#
-# real	0m2.558s
-# user	0m2.105s
-# sys	0m0.448s
-# root@psyt14s:/home/psy/zfs_autobackup# time python3 -m zfs_autobackup.ZfsCheck
-#
-# real	0m1.459s
-# user	0m0.993s
-# sys	0m0.462s
 
 # NOTE: surprisingly sha1 in via python3 is faster than the native sha1sum utility, even in the way we use below!
 import os
 import platform
 import sys
+from datetime import datetime
 
 
 def tmp_name(suffix=""):
     """create temporary name unique to this process and node. always retruns the same result during the same execution"""
 
     #we could use uuids but those are ugly and confusing
     name="{}-{}-{}".format(
@@ -44,22 +32,32 @@
     devnull = os.open(os.devnull, os.O_WRONLY)
     os.dup2(devnull, sys.stdout.fileno())
     os.dup2(devnull, sys.stderr.fileno())
 
 def sigpipe_handler(sig, stack):
     #redir output so we dont get more SIGPIPES during cleanup. (which my try to write to stdout)
     output_redir()
-    deb('redir')
+    #deb('redir')
 
 # def check_output():
 #     """make sure stdout still functions. if its broken, this will trigger a SIGPIPE which will be handled by the sigpipe_handler."""
 #     try:
 #         print(" ")
 #         sys.stdout.flush()
 #     except Exception as e:
 #         pass
 
 # def deb(txt):
 #     with open('/tmp/debug.log', 'a') as fh:
 #         fh.write("DEB: "+txt+"\n")
 
 
+# This should be the only source of trueth for the current datetime.
+# This function will be mocked during unit testing.
+
+
+datetime_now_mock=None
+def datetime_now(utc):
+    if datetime_now_mock is None:
+        return( datetime.utcnow() if utc else datetime.now())
+    else:
+        return datetime_now_mock
```

### Comparing `zfs_autobackup-3.2b1/LICENSE` & `zfs_autobackup-3.3b3/LICENSE`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/setup.py` & `zfs_autobackup-3.3b3/setup.py`

 * *Files identical despite different names*

### Comparing `zfs_autobackup-3.2b1/README.md` & `zfs_autobackup-3.3b3/zfs_autobackup.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: zfs_autobackup
+Version: 3.3b3
+Summary: ZFS autobackup is used to periodicly backup ZFS filesystems to other locations. It tries to be the most friendly to use and easy to debug ZFS backup tool.
+Home-page: https://github.com/psy0rz/zfs_autobackup
+Author: Edwin Eefting
+Author-email: edwin@datux.nl
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: colorama
+Requires-Dist: argparse
+
 
 # ZFS autobackup
 
 [![Tests](https://github.com/psy0rz/zfs_autobackup/workflows/Regression%20tests/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions?query=workflow%3A%22Regression+tests%22) [![Coverage Status](https://coveralls.io/repos/github/psy0rz/zfs_autobackup/badge.svg)](https://coveralls.io/github/psy0rz/zfs_autobackup)  [![Python Package](https://github.com/psy0rz/zfs_autobackup/workflows/Upload%20Python%20Package/badge.svg)](https://pypi.org/project/zfs-autobackup/)
 [![CodeQL](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/psy0rz/zfs_autobackup/actions/workflows/codeql-analysis.yml)
 
 ## Introduction
@@ -10,53 +27,59 @@
 
 You can either use it as a **backup** tool, **replication** tool or **snapshot** tool.
 
 You can select what to backup by setting a custom `ZFS property`. This makes it easy to add/remove specific datasets, or just backup your whole pool.
 
 Other settings are just specified on the commandline: Simply setup and test your zfs-autobackup command and  fix all the issues you might encounter. When you're done you can just copy/paste your command to a cron or script.
 
-Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or error. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
+Since it's using ZFS commands, you can see what it's actually doing by specifying `--debug`. This also helps a lot if you run into some strange problem or errors. You can just copy-paste the command that fails and play around with it on the commandline. (something I missed in other tools)
 
 An important feature that's missing from other tools is a reliable `--test` option: This allows you to see what zfs-autobackup will do and tune your parameters. It will do everything, except make changes to your system.
 
 ## Features
 
 * Works across operating systems: Tested with **Linux**, **FreeBSD/FreeNAS** and **SmartOS**.
-* Low learning curve: no complex daemons or services, no additional software or networking needed. (Only read this page)   
+* Low learning curve: no complex daemons or services, no additional software or networking needed. 
 * Plays nicely with existing replication systems. (Like Proxmox HA)
 * Automatically selects filesystems to backup by looking at a simple ZFS property. 
 * Creates consistent snapshots. (takes all snapshots at once, atomicly.)
 * Multiple backups modes:
   * Backup local data on the same server.
   * "push" local data to a backup-server via SSH.
   * "pull" remote data from a server via SSH and backup it locally.
   * "pull+push": Zero trust between source and target.
 * Can be scheduled via simple cronjob or run directly from commandline.
+* Also supports complex backup geometries.
 * ZFS encryption support: Can decrypt / encrypt or even re-encrypt datasets during transfer.
 * Supports sending with compression. (Using pigz, zstd etc)
 * IO buffering to speed up transfer.
 * Bandwidth rate limiting.
 * Multiple backups from and to the same datasets are no problem.
 * Resillient to errors.
 * Ability to manually 'finish' failed backups to see whats going on.
 * Easy to debug and has a test-mode. Actual unix commands are printed.
 * Uses progressive thinning for older snapshots.
 * Uses zfs-holds on important snapshots to prevent accidental deletion.
 * Automatic resuming of failed transfers.
 * Easy migration from other zfs backup systems to zfs-autobackup.
 * Gracefully handles datasets that no longer exist on source.
-* Complete and clean logging. 
+* Complete and clean logging.
+* All code is regression tested against actual ZFS environments.
 * Easy installation:
   * Just install zfs-autobackup via pip.
   * Only needs to be installed on one side.
   * Written in python and uses zfs-commands, no special 3rd party dependency's or compiled libraries needed.
   * No annoying config files or properties. 
 
 ## Getting started
 
 Please look at our wiki to [Get started](https://github.com/psy0rz/zfs_autobackup/wiki).
 
+Or read the [Full manual](https://github.com/psy0rz/zfs_autobackup/wiki/Manual)
+
 # Sponsor list
 
-This project was sponsorred by:
+This project was sponsored by:
 
-* JetBrains (Provided me with a license for their whole professional product line, https://www.jetbrains.com/pycharm/ )
+* JetBrains 
+* https://rsync.net
+* [DatuX](https://www.datux.nl)
```

