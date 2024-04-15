# Comparing `tmp/regipy-4.1.1.tar.gz` & `tmp/regipy-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regipy-4.1.1.tar", last modified: Thu Mar  7 11:49:26 2024, max compression
+gzip compressed data, was "regipy-4.2.0.tar", last modified: Mon Apr 15 18:45:25 2024, max compression
```

## Comparing `regipy-4.1.1.tar` & `regipy-4.2.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.342558 regipy-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-07 11:49:22.000000 regipy-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 11:49:22.000000 regipy-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-07 11:49:26.342558 regipy-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-03-07 11:49:22.000000 regipy-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.330559 regipy-4.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-07 11:49:22.000000 regipy-4.1.1/docs/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-07 11:49:22.000000 regipy-4.1.1/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.330559 regipy-4.1.1/regipy/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25515 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/hive_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.334559 regipy-4.1.1/regipy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.334559 regipy-4.1.1/regipy/plugins/amcache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/amcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/amcache/amcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.334559 regipy-4.1.1/regipy/plugins/bcd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/bcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/bcd/boot_entry_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.334559 regipy-4.1.1/regipy/plugins/ntuser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/installed_programs_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/network_drives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/shellbags_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/tsclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/typed_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/typed_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/user_assist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/winrar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/winscp_saved_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/ntuser/word_wheel_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/plugin_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.338559 regipy-4.1.1/regipy/plugins/sam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/sam/local_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.338559 regipy-4.1.1/regipy/plugins/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/security/domain_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.338559 regipy-4.1.1/regipy/plugins/software/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/image_file_execution_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/installed_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/last_logon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/printdemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/profilelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/software/uac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.342558 regipy-4.1.1/regipy/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/active_controlset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/bam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/bootkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/computer_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.342558 regipy-4.1.1/regipy/plugins/system/external/
--rwxr-xr-x   0 runner    (1001) docker     (127)    17390 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/external/ShimCacheParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/host_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/network_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/safeboot_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/shimcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/timezone_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/usbstor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/system/wdigest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.342558 regipy-4.1.1/regipy/plugins/usrclass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/usrclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/usrclass/shellbags_usrclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/regdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)    26690 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/security_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-07 11:49:22.000000 regipy-4.1.1/regipy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:49:26.342558 regipy-4.1.1/regipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 11:49:26.000000 regipy-4.1.1/regipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 11:49:26.342558 regipy-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-07 11:49:22.000000 regipy-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 18:45:17.000000 regipy-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 18:45:17.000000 regipy-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-15 18:45:25.427455 regipy-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-15 18:45:17.000000 regipy-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.415455 regipy-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 18:45:17.000000 regipy-4.2.0/docs/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-15 18:45:17.000000 regipy-4.2.0/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/hive_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/amcache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/amcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/amcache/amcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.419455 regipy-4.2.0/regipy/plugins/bcd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/bcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/bcd/boot_entry_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/ntuser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/installed_programs_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/network_drives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/shellbags_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/tsclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/typed_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/typed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/user_assist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/winrar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/winscp_saved_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/ntuser/word_wheel_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/plugin_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/sam/local_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/security/domain_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.423455 regipy-4.2.0/regipy/plugins/software/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/image_file_execution_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/installed_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/last_logon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/printdemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/profilelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/software/uac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/active_controlset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/bam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/bootkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/computer_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/system/external/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17390 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/external/ShimCacheParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/host_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/safeboot_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/shimcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/timezone_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/usbstor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/system/wdigest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy/plugins/usrclass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/usrclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/usrclass/shellbags_usrclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/regdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26690 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/security_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-15 18:45:17.000000 regipy-4.2.0/regipy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:45:25.427455 regipy-4.2.0/regipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 18:45:25.000000 regipy-4.2.0/regipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:45:25.427455 regipy-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-15 18:45:17.000000 regipy-4.2.0/setup.py
```

### Comparing `regipy-4.1.1/LICENSE` & `regipy-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/PKG-INFO` & `regipy-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 4.1.1
+Version: 4.2.0
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,16 @@
 Requires-Dist: pytest-flake8; extra == "test"
 Provides-Extra: cli
 Requires-Dist: click>=7.0.0; extra == "cli"
 Requires-Dist: tabulate; extra == "cli"
 Provides-Extra: full
 Requires-Dist: click>=7.0.0; extra == "full"
 Requires-Dist: tabulate; extra == "full"
-Requires-Dist: libfwsi-python>=20220123; extra == "full"
+Requires-Dist: libfwsi-python>=20240315; extra == "full"
+Requires-Dist: libfwps-python>=20240310; extra == "full"
 
 
 .. image:: https://travis-ci.com/mkorman90/regipy.svg?branch=master
     :target: https://travis-ci.com/mkorman90/regipy
 
 regipy
 ==========
```

### Comparing `regipy-4.1.1/README.md` & `regipy-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/docs/PLUGINS.md` & `regipy-4.2.0/docs/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/docs/README.rst` & `regipy-4.2.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/cli.py` & `regipy-4.2.0/regipy/cli.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/cli_utils.py` & `regipy-4.2.0/regipy/cli_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/constants.py` & `regipy-4.2.0/regipy/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ShellBags Known GUIDs
 KNOWN_GUIDS = {
-    "008ca0b1-55b4-4c56-b8a8-4de4b299d3bE": "Account Pictures",
+    "008ca0b1-55b4-4c56-b8a8-4de4b299d3be": "Account Pictures",
     "00bcfc5a-ed94-4e48-96a1-3f6217f21990": "RoamingTiles",
     "00c6d95f-329c-409a-81d7-c46c66ea7f33": "Default Location",
     "00f2886f-cd64-4fc9-8ec5-30ef6cdbe8c3": "Scanners and Cameras",
     "0139d44e-6afe-49f2-8690-3dafcae6ffb8": "Programs",
     "0142e4d0-fb7a-11dc-ba4a-000ffe7ab428": "Biometric Devices (Biometrics)",
     "018d5c66-4533-4307-9b53-224de2ed1fe6": "OneDrive",
     "025a5937-a6be-4686-a844-36fe4bec8b6d": "Power Options",
@@ -158,15 +158,15 @@
     "679f85cb-0220-4080-b29b-5540cc05aab6": "Home Folder",
     "67ca7650-96e6-4fdd-bb43-a8e774f73a57": "Home Group Control Panel (Home Group)",
     "692f0339-cbaa-47e6-b5b5-3b84db604e87": "Extensions Manager Folder",
     "69d2cf90-fc33-4fb7-9a0c-ebb0f0fcb43c": "Slide Shows",
     "6c8eec18-8d75-41b2-a177-8831d59d2d50": "Mouse",
     "6dfd7c5c-2451-11d3-a299-00c04f8ef6af": "Folder Options",
     "6f0cd92b-2e97-45d1-88ff-b0d186b8dedd": "Network Connections",
-    "7007acc7-3202-11d1-aad2-00805fc1270e": "Network Connections (Network and Dial-up Connections)",
+    "7007acc7-3202-11d1-aad2-00805fc1270e": "Network Connections",
     "708e1662-b832-42a8-bbe1-0a77121e3908": "Tree property value folder",
     "71689ac1-cc88-45d0-8a22-2943c3e7dfb3": "Music Search Results",
     "71d99464-3b6b-475c-b241-e15883207529": "Sync Results Folder",
     "724ef170-a42d-4fef-9f26-b60e846fba4f": "Administrative tools",
     "725be8f7-668e-4c7b-8f90-46bdb0936430": "Keyboard",
     "72b36e70-8700-42d6-a7f7-c9ab3323ee51": "Search Connector Folder",
     "74246bfc-4c96-11d0-abef-0020af6b0b7a": "Device Manager",
@@ -271,15 +271,15 @@
     "b5947d7f-b489-4fde-9e77-23780cc610d1": "Virtual Machines",
     "b689b0d0-76d3-4cbb-87f7-585d0e0ce070": "Games folder",
     "b6ebfb86-6907-413c-9af7-4fc2abf07cc5": "Public Pictures",
     "b7534046-3ecb-4c18-be4e-64cd4cb7d6ac": "Recycle Bin",
     "b7bede81-df94-4682-a7d8-57a52620b86f": "Screenshots",
     "b94237e7-57ac-4347-9151-b08c6c32d1f7": "CommonTemplates",
     "b97d20bb-f46a-4c97-ba10-5e3608430854": "Startup",
-    "b98a2bea-7d42-4558-8bd1-832f41bac6fd": "Backup And Restore (Backup and Restore Center)",
+    "b98a2bea-7d42-4558-8bd1-832f41bac6fd": "Backup And Restore (Windows 7)",
     "bb06c0e4-d293-4f75-8a90-cb05b6477eee": "System",
     "bb64f8a7-bee7-4e1a-ab8d-7d8273f7fdb6": "Action Center Control Panel",
     "bc476f4c-d9d7-4100-8d4e-e043f6dec409": "Microsoft Browser Architecture",
     "bc48b32f-5910-47f5-8570-5074a8a5636a": "Sync Results Delegate Folder",
     "bcb5256f-79f6-4cee-b725-dc34e402fd46": "ImplicitAppShortcuts",
     "bcbd3057-ca5c-4622-b42d-bc56db0ae516": "Programs",
     "bd7a2e7b-21cb-41b2-a086-b309680c6b7e": "Client Side Cache Folder",
@@ -384,8 +384,42 @@
     "f86fa3ab-70d2-4fc7-9c99-fcbf05467f3a": "Videos",
     "3dfdf296-dbec-4fb4-81d1-6a3438bcf4de": "Music",
     "e31ea727-12ed-4702-820c-4b6445f28e1a": "Dropbox",
     "4a8fcd9f-623c-4283-96f0-10f41846a98a": "Box Sync",
     "fbf23b42-e3f0-101b-8488-00aa003e56f8": "Internet Explorer",
     "00020d75-0000-0000-c000-000000000046": "Inbox",
     "00020d76-0000-0000-c000-000000000046": "Inbox",
+    "0": "All Control Panel Items",
+    "1": "Appearance and Personalization",
+    "2": "Hardware and Sound",
+    "3": "Network and Internet",
+    "4": "Sounds, Speech, and Audio Devices",
+    "5": "System and Security",
+    "6": "Clock, Language, and Region",
+    "7": "Ease of Access",
+    "8": "Programs",
+    "9": "User Accounts",
+    "10": "Security Center",
+    "11": "Mobile PC",
+    "0ddd015d-b06c-45d5-8c4c-f59713854639": "Local Pictures",
+    "a0c69a99-21c8-4671-8703-7934162fcf1d": "Local Music",
+    "7d83ee9b-2244-4e70-b1f5-5393042af1e4": "Local Downloads",
+    "35286a68-3c57-41a1-bbb1-0eae73d76c95": "Local Videos",
+    "f42ee2d3-909f-4907-8871-4c22fc0bf756": "Local Documents",
+    "5ed4f38c-d3ff-4d61-b506-6820320aebfe": "All Settings",
+    "1bef2128-2f96-4500-ba7c-098dc0049cb2": "CLSID_DBFolderBoth",
+    "00021400-0000-0000-c000-000000000046": "Desktop",
+    "3936e9e4-d92c-4eee-a85a-bc16d5ea0819": "Frequent folders",
+    "45e8e0e8-7ae9-41ad-a9e8-594972716684": "Pictures",
+    "f5fb2c77-0e2f-4a16-a381-3e560c68bc83": "Removable Drives",
+    "0e5aae11-a475-4c5b-ab00-c66de400274e": "Shell File System Folder",
+    "f3364ba0-65b9-11ce-a9ba-00aa004ae837": "Shell File System Folder",
+    "5e5f29ce-e0a8-49d3-af32-7a7bdc173478": "This PC",
+    "e44e5d18-0652-4508-a4e2-8a090067bcb0": "Default Programs",
+    "e88865ea-0e1c-4e20-9aa6-edcd0212c87c": "Gallery",
+    "b2b4a4d1-2754-4140-a2eb-9a76d9d7cdc6": "Linux",
+    "2559a1f8-21d7-11d4-bdaf-00c04f60b9f0": "Windows Search",
+    "e342f0fe-ff1c-4c41-be37-a0271fc90396": "Intel Rapid Storage Technology",
+    "0bbca823-e77d-419e-9a44-5adec2c8eeb0": "NVIDIA Control Panel",
+    "8e0c279d-0bd1-43c3-9ebd-31c3dc5b8a77": "Windows To Go",
+    "00028b00-0000-0000-c000-000000000046": "Microsoft Network",
 }
```

### Comparing `regipy-4.1.1/regipy/exceptions.py` & `regipy-4.2.0/regipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/hive_types.py` & `regipy-4.2.0/regipy/hive_types.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/__init__.py` & `regipy-4.2.0/regipy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/amcache/amcache.py` & `regipy-4.2.0/regipy/plugins/amcache/amcache.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/bcd/boot_entry_list.py` & `regipy-4.2.0/regipy/plugins/bcd/boot_entry_list.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/classes_installer.py` & `regipy-4.2.0/regipy/plugins/ntuser/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/installed_programs_ntuser.py` & `regipy-4.2.0/regipy/plugins/ntuser/installed_programs_ntuser.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/network_drives.py` & `regipy-4.2.0/regipy/plugins/ntuser/network_drives.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/persistence.py` & `regipy-4.2.0/regipy/plugins/ntuser/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/shellbags_ntuser.py` & `regipy-4.2.0/regipy/plugins/ntuser/shellbags_ntuser.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,46 +47,71 @@
 
         elif isinstance(shell_item, pyfwsi.network_location):
             item_type = "Network Location"
 
         elif isinstance(shell_item, pyfwsi.root_folder):
             item_type = "Root Folder"
 
+        elif isinstance(shell_item, pyfwsi.control_panel_category):
+            item_type = "Control Panel Category"
+
+        elif isinstance(shell_item, pyfwsi.control_panel_item):
+            item_type = "Control Panel Item"
+
+        elif isinstance(shell_item, pyfwsi.users_property_view):
+            item_type = "Users Property View"
+
         else:
             item_type = 'unknown'
 
         return item_type
 
     @staticmethod
+    def _check_known_guids(guid):
+        if guid in KNOWN_GUIDS:
+            path_segment = KNOWN_GUIDS[guid]
+        else:
+            path_segment = '{{{0:s}}}'.format(guid)
+        return path_segment
+
+    @staticmethod
+    def _get_entry_string(fwps_record):
+        if fwps_record.entry_name:
+            entry_string = fwps_record.entry_name
+        else:
+            entry_string = f'{fwps_record.entry_type:d}'
+        return entry_string
+
+    @staticmethod
     def _parse_shell_item_path_segment(self, shell_item):
         """Parses a shell item path segment.
         Args:
           shell_item (pyfwsi.item): shell item.
         Returns:
           str: shell item path segment.
         """
 
         try:
             import pyfwsi
+            import pyfwps
         except ModuleNotFoundError as ex:
             logger.exception(f"Plugin `shellbag_plugin` has missing modules, install regipy using"
                              f" `pip install regipy[full]` in order to install plugin dependencies. "
                              f"This might take some time... ")
             raise ex
 
         path_segment = None
+        full_path = None
+        location_description = None
 
         if isinstance(shell_item, pyfwsi.volume):
             if shell_item.name:
                 path_segment = shell_item.name
             elif shell_item.identifier:
-                if shell_item.identifier in KNOWN_GUIDS:
-                    path_segment = KNOWN_GUIDS[shell_item.identifier]
-                else:
-                    path_segment = '{{{0:s}}}'.format(shell_item.identifier)
+                path_segment = self._check_known_guids(shell_item.identifier)
 
         elif isinstance(shell_item, pyfwsi.file_entry):
             long_name = ''
             for extension_block in shell_item.extension_blocks:
                 if isinstance(extension_block, pyfwsi.file_entry_extension):
                     long_name = extension_block.long_name
 
@@ -94,27 +119,88 @@
                 path_segment = long_name
             elif shell_item.name:
                 path_segment = shell_item.name
 
         elif isinstance(shell_item, pyfwsi.network_location):
             if shell_item.location:
                 path_segment = shell_item.location
+            if shell_item.description:
+                location_description = shell_item.description
+                if shell_item.comments:
+                    location_description += f', {shell_item.comments}'
 
         elif isinstance(shell_item, pyfwsi.root_folder):
             if shell_item.shell_folder_identifier in KNOWN_GUIDS:
                 path_segment = KNOWN_GUIDS[shell_item.shell_folder_identifier]
             elif hasattr(shell_item, 'identifier') and shell_item.identifier in KNOWN_GUIDS:
                 path_segment = KNOWN_GUIDS[shell_item.identifier]
             else:
                 path_segment = '{{{0:s}}}'.format(shell_item.shell_folder_identifier)
 
+        elif isinstance(shell_item, pyfwsi.users_property_view):
+            # Users property view
+            if shell_item.delegate_folder_identifier in KNOWN_GUIDS:
+                path_segment = KNOWN_GUIDS[shell_item.delegate_folder_identifier]
+            elif hasattr(shell_item, 'identifier') and shell_item.identifier in KNOWN_GUIDS:
+                path_segment = KNOWN_GUIDS[shell_item.identifier]
+
+            # Variable: Users property view
+            elif shell_item.property_store_data:
+                fwps_store = pyfwps.store()
+                fwps_store.copy_from_byte_stream(shell_item.property_store_data)
+
+                for fwps_set in iter(fwps_store.sets):
+                    if fwps_set.identifier == 'b725f130-47ef-101a-a5f1-02608c9eebac':
+                        for fwps_record in iter(fwps_set.records):
+                            entry_string = self._get_entry_string(fwps_record)
+
+                            # PKEY_DisplayName: {b725f130-47ef-101a-a5f1-02608c9eebac}/10
+                            if entry_string == '10':
+                                if fwps_record.value_type == 0x0001:
+                                    value_string = '<VT_NULL>'
+                                elif fwps_record.value_type in (0x0003, 0x0013, 0x0014, 0x0015):
+                                    value_string = str(fwps_record.get_data_as_integer())
+                                elif fwps_record.value_type in (0x0008, 0x001e, 0x001f):
+                                    value_string = fwps_record.get_data_as_string()
+                                elif fwps_record.value_type == 0x000b:
+                                    value_string = str(fwps_record.get_data_as_boolean())
+                                elif fwps_record.value_type == 0x0040:
+                                    filetime = fwps_record.get_data_as_integer()
+                                    value_string = self._FormatFiletimeValue(filetime)
+                                elif fwps_record.value_type == 0x0042:
+                                    # TODO: add support
+                                    value_string = '<VT_STREAM>'
+                                elif fwps_record.value_type == 0x0048:
+                                    value_string = fwps_record.get_data_as_guid()
+                                elif fwps_record.value_type & 0xf000 == 0x1000:
+                                    # TODO: add support
+                                    value_string = '<VT_VECTOR>'
+                                else:
+                                    value_string = None
+
+                                path_segment = value_string
+
+                    elif fwps_set.identifier == '28636aa6-953d-11d2-b5d6-00c04fd918d0':
+                        for fwps_record in iter(fwps_set.records):
+                            entry_string = self._get_entry_string(fwps_record)
+
+                            # PKEY_ParsingPath: {28636aa6-953d-11d2-b5d6-00c04fd918d0}/30
+                            if entry_string == '30':
+                                full_path = fwps_record.get_data_as_string()
+
+        elif isinstance(shell_item, pyfwsi.control_panel_category):
+            path_segment = self._check_known_guids(str(shell_item.identifier))
+
+        elif isinstance(shell_item, pyfwsi.control_panel_item):
+            path_segment = self._check_known_guids(shell_item.identifier)
+
         if path_segment is None:
             path_segment = '<UNKNOWN: 0x{0:02x}>'.format(shell_item.class_type)
 
-        return path_segment
+        return path_segment, full_path, location_description
 
     def iter_sk(self, key, reg_path, base_path='', path=''):
         try:
             import pyfwsi
         except ModuleNotFoundError as ex:
             logger.exception(f"Plugin `shellbag_plugin` has missing modules, install regipy using"
                              f" `pip install regipy[full]` in order to install plugin dependencies. "
@@ -136,15 +222,15 @@
             if re.match("\d+", v.name):
                 slot = v.name
                 byte_stream = v.value
                 shell_items = pyfwsi.item_list()
                 shell_items.copy_from_byte_stream(byte_stream, ascii_codepage=CODEPAGE)
                 for item in shell_items.items:
                     shell_type = self._get_shell_item_type(item)
-                    value = self._parse_shell_item_path_segment(self, item)
+                    value, full_path, location_description = self._parse_shell_item_path_segment(self, item)
                     if not path:
                         path = value
                         base_path = ''
                     else:
                         path += f'\\{value}'
 
                     creation_time = None
@@ -180,14 +266,16 @@
                     entry = {'value': value,
                              'slot': slot,
                              'reg_path': reg_path,
                              'value_name': value_name,
                              'node_slot': node_slot,
                              'shell_type': shell_type,
                              'path': path,
+                             'full path': full_path if full_path else None,
+                             'location description': location_description if location_description else None,
                              'creation_time': creation_time,
                              'access_time': access_time,
                              'modification_time': modification_time,
                              'last_write': last_write,
                              'mru_order': mru_order,
                              'mru_order_location': mru_order_location,
                              }
```

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/tsclient.py` & `regipy-4.2.0/regipy/plugins/ntuser/tsclient.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/typed_paths.py` & `regipy-4.2.0/regipy/plugins/ntuser/typed_paths.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/typed_urls.py` & `regipy-4.2.0/regipy/plugins/ntuser/typed_urls.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/user_assist.py` & `regipy-4.2.0/regipy/plugins/ntuser/user_assist.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/winrar.py` & `regipy-4.2.0/regipy/plugins/ntuser/winrar.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/winscp_saved_sessions.py` & `regipy-4.2.0/regipy/plugins/ntuser/winscp_saved_sessions.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/ntuser/word_wheel_query.py` & `regipy-4.2.0/regipy/plugins/ntuser/word_wheel_query.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/plugin.py` & `regipy-4.2.0/regipy/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/plugin_template.py` & `regipy-4.2.0/regipy/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/sam/local_sid.py` & `regipy-4.2.0/regipy/plugins/sam/local_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/security/domain_sid.py` & `regipy-4.2.0/regipy/plugins/security/domain_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/classes_installer.py` & `regipy-4.2.0/regipy/plugins/software/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/image_file_execution_options.py` & `regipy-4.2.0/regipy/plugins/software/image_file_execution_options.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/installed_programs.py` & `regipy-4.2.0/regipy/plugins/software/installed_programs.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/last_logon.py` & `regipy-4.2.0/regipy/plugins/software/last_logon.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/persistence.py` & `regipy-4.2.0/regipy/plugins/software/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/printdemon.py` & `regipy-4.2.0/regipy/plugins/software/printdemon.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/profilelist.py` & `regipy-4.2.0/regipy/plugins/software/profilelist.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/tracing.py` & `regipy-4.2.0/regipy/plugins/software/tracing.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/software/uac.py` & `regipy-4.2.0/regipy/plugins/software/uac.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/active_controlset.py` & `regipy-4.2.0/regipy/plugins/system/active_controlset.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/bam.py` & `regipy-4.2.0/regipy/plugins/system/bam.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/bootkey.py` & `regipy-4.2.0/regipy/plugins/system/bootkey.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/computer_name.py` & `regipy-4.2.0/regipy/plugins/system/computer_name.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/external/ShimCacheParser.py` & `regipy-4.2.0/regipy/plugins/system/external/ShimCacheParser.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/host_domain_name.py` & `regipy-4.2.0/regipy/plugins/system/host_domain_name.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/network_data.py` & `regipy-4.2.0/regipy/plugins/system/network_data.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/routes.py` & `regipy-4.2.0/regipy/plugins/system/routes.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/safeboot_configuration.py` & `regipy-4.2.0/regipy/plugins/system/safeboot_configuration.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/services.py` & `regipy-4.2.0/regipy/plugins/system/services.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/shimcache.py` & `regipy-4.2.0/regipy/plugins/system/shimcache.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/timezone_data.py` & `regipy-4.2.0/regipy/plugins/system/timezone_data.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/usbstor.py` & `regipy-4.2.0/regipy/plugins/system/usbstor.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/system/wdigest.py` & `regipy-4.2.0/regipy/plugins/system/wdigest.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/plugins/utils.py` & `regipy-4.2.0/regipy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/recovery.py` & `regipy-4.2.0/regipy/recovery.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/regdiff.py` & `regipy-4.2.0/regipy/regdiff.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/registry.py` & `regipy-4.2.0/regipy/registry.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/security_utils.py` & `regipy-4.2.0/regipy/security_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/structs.py` & `regipy-4.2.0/regipy/structs.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy/utils.py` & `regipy-4.2.0/regipy/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/regipy.egg-info/PKG-INFO` & `regipy-4.2.0/regipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 4.1.1
+Version: 4.2.0
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,16 @@
 Requires-Dist: pytest-flake8; extra == "test"
 Provides-Extra: cli
 Requires-Dist: click>=7.0.0; extra == "cli"
 Requires-Dist: tabulate; extra == "cli"
 Provides-Extra: full
 Requires-Dist: click>=7.0.0; extra == "full"
 Requires-Dist: tabulate; extra == "full"
-Requires-Dist: libfwsi-python>=20220123; extra == "full"
+Requires-Dist: libfwsi-python>=20240315; extra == "full"
+Requires-Dist: libfwps-python>=20240310; extra == "full"
 
 
 .. image:: https://travis-ci.com/mkorman90/regipy.svg?branch=master
     :target: https://travis-ci.com/mkorman90/regipy
 
 regipy
 ==========
```

### Comparing `regipy-4.1.1/regipy.egg-info/SOURCES.txt` & `regipy-4.2.0/regipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regipy-4.1.1/setup.py` & `regipy-4.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
           tests_require=test_requirements,
           extras_require={
               'test': test_requirements,
               'cli': ['click>=7.0.0', 'tabulate'],
               'full': [
                  'click>=7.0.0',
                  'tabulate',
-                 'libfwsi-python>=20220123'
+                 'libfwsi-python>=20240315',
+                 'libfwps-python>=20240310'
               ],
           },
           include_package_data=True,
           keywords='Python, Python3, registry, windows registry, registry parser',
           classifiers=['Development Status :: 5 - Production/Stable',
                        'Intended Audience :: Developers',
                        'Natural Language :: English',
```

