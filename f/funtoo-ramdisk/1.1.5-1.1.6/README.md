# Comparing `tmp/funtoo-ramdisk-1.1.5.tar.gz` & `tmp/funtoo_ramdisk-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-ramdisk-1.1.5.tar", last modified: Fri Sep 15 19:56:28 2023, max compression
+gzip compressed data, was "funtoo_ramdisk-1.1.6.tar", last modified: Mon Apr 15 03:23:13 2024, max compression
```

## Comparing `funtoo-ramdisk-1.1.5.tar` & `funtoo_ramdisk-1.1.6.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2023-08-15 04:16:10.000000 funtoo-ramdisk-1.1.5/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7654 2023-09-15 19:56:19.000000 funtoo-ramdisk-1.1.5/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2023-09-15 19:55:45.000000 funtoo-ramdisk-1.1.5/MANIFEST.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15306 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2023-09-04 02:26:28.000000 funtoo-ramdisk-1.1.5/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-09-15 19:56:00.000000 funtoo-ramdisk-1.1.5/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.276242 funtoo-ramdisk-1.1.5/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2023-09-04 19:29:55.000000 funtoo-ramdisk-1.1.5/bin/ramdisk
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.276242 funtoo-ramdisk-1.1.5/doc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7107 2023-09-15 19:56:25.000000 funtoo-ramdisk-1.1.5/doc/manpage.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7113 2023-09-15 02:14:14.000000 funtoo-ramdisk-1.1.5/doc/manpage.rst.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7655 2023-09-15 19:56:25.000000 funtoo-ramdisk-1.1.5/doc/ramdisk.8
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-08-14 21:32:25.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6117 2023-09-03 03:13:02.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/args.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2023-09-14 18:35:49.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/config_files.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1926 2023-09-03 03:11:26.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/const.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11414 2023-09-04 19:29:55.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/initramfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2023-09-03 02:54:20.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/kernel.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2023-09-02 19:02:38.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/log.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15870 2023-09-04 01:51:39.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/modules.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      830 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugin_base.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugins/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugins/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugins/btrfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugins/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      464 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugins/lvm.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-08-15 04:57:00.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/etc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      300 2023-08-20 04:33:45.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/etc/initrd.defaults
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5637 2023-09-04 00:37:25.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/etc/initrd.scripts
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2023-08-21 01:31:42.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/initramfs.cpio
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2569 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/linuxrc
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/modules.autoload
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/modules.copy
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2023-09-02 18:33:14.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/utilities.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-09-15 19:56:25.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk/version.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15306 2023-09-15 19:56:28.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1162 2023-09-15 19:56:28.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-09-15 19:56:28.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2023-09-15 19:56:28.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2023-09-15 19:56:28.000000 funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      724 2023-09-15 02:05:23.000000 funtoo-ramdisk-1.1.5/make.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-09-15 19:56:28.280242 funtoo-ramdisk-1.1.5/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2023-09-15 19:56:25.000000 funtoo-ramdisk-1.1.5/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2023-09-15 02:11:39.000000 funtoo-ramdisk-1.1.5/setup.py.in
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8429 2024-04-15 03:22:39.000000 funtoo_ramdisk-1.1.6/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/MANIFEST.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16081 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-04-15 03:15:29.000000 funtoo_ramdisk-1.1.6/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/bin/ramdisk
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/doc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7107 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/doc/manpage.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7113 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/doc/manpage.rst.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7642 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/doc/ramdisk.8
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6309 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/args.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/config_files.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/const.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12096 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/initramfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/kernel.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/log.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15949 2024-04-15 03:11:58.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/modules.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1167 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugin_base.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/btrfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      782 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugins/lvm.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      319 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.defaults
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6059 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.scripts
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      645 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      117 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/initramfs.cpio
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2174 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/linuxrc
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.autoload
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.copy
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/utilities.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk/version.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:23:13.453779 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16081 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1374 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2024-04-15 03:23:13.000000 funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      721 2024-04-15 03:17:25.000000 funtoo_ramdisk-1.1.6/make.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-04-15 03:23:13.463770 funtoo_ramdisk-1.1.6/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2024-04-15 03:23:08.000000 funtoo_ramdisk-1.1.6/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.6/setup.py.in
```

### Comparing `funtoo-ramdisk-1.1.5/ChangeLog.rst` & `funtoo_ramdisk-1.1.6/ChangeLog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+funtoo-ramdisk 1.1.6
+--------------------
+
+Released on April 14, 2024.
+
+This is a maintenance and minor features release.
+
+* Various minor bug fixes.
+
+* Change ``--enable`` to ``--plugins`` since it's more
+  self-explanatory.
+
+* Continue to flesh out the plugin system. I added support for
+  plugins to have an activation script which will get executed
+  on startup. This is a work in progress and I still need to
+  add support for listing needed modules for a plugin which
+  will get loaded automatically.
+
+* Fix a bug in argument parsing where the code was not scanning
+  for invalid options which could result in odd parsing behavior.
+
+* Start adding support for udev. This is not yet completed but
+  the plugin system for this has been incorporated into the
+  linuxrc.
+
+
 funtoo-ramdisk 1.1.5
 --------------------
 
 Released on September 15, 2023.
 
 This is a packaging fix for the manpage.
```

### Comparing `funtoo-ramdisk-1.1.5/PKG-INFO` & `funtoo_ramdisk-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.5
+Version: 1.1.6
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.5
+:Version: 1.1.6
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -127,15 +127,15 @@
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
                         ``ramdisk list kernels`` to display available options. The
                         default setting is to use the current value of the
                         ``/usr/src/linux`` symlink at the filesystem root to determine
                         which kernel to build a ramdisk for.
 --compression=<method>  Compression method to use. Default is ``xz``. Also supported: ``zstd``.
 --temp_root=<path>      Where to create temporary files. Defaults to ``/var/tmp``.
---enable=<plugins>      A comma-delimited list of plugins to enable. The ``core`` plugin is
+--plugins=<plugins>     A comma-delimited list of plugins to enable. The ``core`` plugin is
                         always enabled. Type ``ramdisk list plugins`` to see a list of available
                         plugins.
 --kmod_config=<cfg>     ``ramdisk`` supports different sets of kernel module configurations, which
                         define what kernel modules get copied to the initramfs, and which ones
                         get auto-loaded by the initramfs at boot. Default value: ``full``. This
                         is currently the only option unless overridden by ``--kpop`` (see below.)
 --kpop=<mods>           A comma-delimited list of kernel module names that you are sure, if loaded,
@@ -168,14 +168,40 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.6
+--------------------
+
+Released on April 14, 2024.
+
+This is a maintenance and minor features release.
+
+* Various minor bug fixes.
+
+* Change ``--enable`` to ``--plugins`` since it's more
+  self-explanatory.
+
+* Continue to flesh out the plugin system. I added support for
+  plugins to have an activation script which will get executed
+  on startup. This is a work in progress and I still need to
+  add support for listing needed modules for a plugin which
+  will get loaded automatically.
+
+* Fix a bug in argument parsing where the code was not scanning
+  for invalid options which could result in odd parsing behavior.
+
+* Start adding support for udev. This is not yet completed but
+  the plugin system for this has been incorporated into the
+  linuxrc.
+
+
 funtoo-ramdisk 1.1.5
 --------------------
 
 Released on September 15, 2023.
 
 This is a packaging fix for the manpage.
```

### Comparing `funtoo-ramdisk-1.1.5/README.rst` & `funtoo_ramdisk-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/bin/ramdisk` & `funtoo_ramdisk-1.1.6/bin/ramdisk`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/doc/manpage.rst` & `funtoo_ramdisk-1.1.6/doc/manpage.rst.in`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.5
+:Version: ##VERSION##
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -113,15 +113,15 @@
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
                         ``ramdisk list kernels`` to display available options. The
                         default setting is to use the current value of the
                         ``/usr/src/linux`` symlink at the filesystem root to determine
                         which kernel to build a ramdisk for.
 --compression=<method>  Compression method to use. Default is ``xz``. Also supported: ``zstd``.
 --temp_root=<path>      Where to create temporary files. Defaults to ``/var/tmp``.
---enable=<plugins>      A comma-delimited list of plugins to enable. The ``core`` plugin is
+--plugins=<plugins>     A comma-delimited list of plugins to enable. The ``core`` plugin is
                         always enabled. Type ``ramdisk list plugins`` to see a list of available
                         plugins.
 --kmod_config=<cfg>     ``ramdisk`` supports different sets of kernel module configurations, which
                         define what kernel modules get copied to the initramfs, and which ones
                         get auto-loaded by the initramfs at boot. Default value: ``full``. This
                         is currently the only option unless overridden by ``--kpop`` (see below.)
 --kpop=<mods>           A comma-delimited list of kernel module names that you are sure, if loaded,
```

### Comparing `funtoo-ramdisk-1.1.5/doc/manpage.rst.in` & `funtoo_ramdisk-1.1.6/doc/manpage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: ##VERSION##
+:Version: 1.1.6
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -113,15 +113,15 @@
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
                         ``ramdisk list kernels`` to display available options. The
                         default setting is to use the current value of the
                         ``/usr/src/linux`` symlink at the filesystem root to determine
                         which kernel to build a ramdisk for.
 --compression=<method>  Compression method to use. Default is ``xz``. Also supported: ``zstd``.
 --temp_root=<path>      Where to create temporary files. Defaults to ``/var/tmp``.
---enable=<plugins>      A comma-delimited list of plugins to enable. The ``core`` plugin is
+--plugins=<plugins>     A comma-delimited list of plugins to enable. The ``core`` plugin is
                         always enabled. Type ``ramdisk list plugins`` to see a list of available
                         plugins.
 --kmod_config=<cfg>     ``ramdisk`` supports different sets of kernel module configurations, which
                         define what kernel modules get copied to the initramfs, and which ones
                         get auto-loaded by the initramfs at boot. Default value: ``full``. This
                         is currently the only option unless overridden by ``--kpop`` (see below.)
 --kpop=<mods>           A comma-delimited list of kernel module names that you are sure, if loaded,
```

### Comparing `funtoo-ramdisk-1.1.5/doc/ramdisk.8` & `funtoo_ramdisk-1.1.6/doc/ramdisk.8`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "RAMDISK" 8 "" "1.1.5" "Funtoo Linux"
+.TH "RAMDISK" "8" "" "1.1.6" "Funtoo Linux"
 .SH NAME
 ramdisk \- create a bootable initial ramdisk
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 \fBramdisk\fP [build] [\fIOPTION...\fP] \fBinitramfs_outfile\fP
 .sp
@@ -46,15 +46,15 @@
 initial RAM disk filesystem (initramfs) for booting your Linux system.
 .sp
 The internal initramfs logic is based on the logic found in Gentoo Linux\(aqs
 genkernel tool, but has been rewritten to be simpler and more efficient.
 .sp
 You can use this tool to create an initramfs to boot to a Funtoo Linux root
 ext4 or XFS filesystem, which is what we support in our official installation
-documentation at \fI\%https://www.funtoo.org/Install\fP\&.
+documentation at  <https://www.funtoo.org/Install> \&.
 .SH CAPABILITIES
 .INDENT 0.0
 .IP \(bu 2
 genkernel\-style initramfs without the cruft. In comparison to genkernel\(aqs
 initramfs, the shell code is about 10x simpler and a lot cleaner and has
 been modernized. About 100 lines of shell script, with another 215 lines
 of functions in a support file.
@@ -141,15 +141,15 @@
 .TP
 .BI \-\-compression\fB= <method>
 Compression method to use. Default is \fBxz\fP\&. Also supported: \fBzstd\fP\&.
 .TP
 .BI \-\-temp_root\fB= <path>
 Where to create temporary files. Defaults to \fB/var/tmp\fP\&.
 .TP
-.BI \-\-enable\fB= <plugins>
+.BI \-\-plugins\fB= <plugins>
 A comma\-delimited list of plugins to enable. The \fBcore\fP plugin is
 always enabled. Type \fBramdisk list plugins\fP to see a list of available
 plugins.
 .TP
 .BI \-\-kmod_config\fB= <cfg>
 \fBramdisk\fP supports different sets of kernel module configurations, which
 define what kernel modules get copied to the initramfs, and which ones
@@ -166,20 +166,18 @@
 .UNINDENT
 .SH USAGE
 .sp
 In its simplest form, the command can be used as follows, as a regular user:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ ramdisk /var/tmp/my\-new\-initramfs
 $ sudo cp /var/tmp/my\-new\-initramfs /boot
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 By default, \fBramdisk\fP will use your \fB/usr/src/linux\fP symlink to determine which
 kernel to use to build a ramdisk for. It will parse \fB/usr/src/linux/Makefile\fP,
 extract kernel version information, and then find the appropriate directory in
 \fB/lib/modules/<kernel_name>\fP for copying modules. You can type:
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/args.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 		Given input arguments sourced from ``self.unparsed_args``, scan these arguments for any optional arguments
 		specified in ``self.defined_options``, which is a dictionary of key/value pairs of
 		options. Keys are literal "--foobar" values, and values in the dict can be used to set default values.
 
 		Results are stored in ``self.opt_args`` with the found optional values set to ``True``. Any not-specified
 		argument will have a ``False`` default value.
 
-		This function returns sets ``self.unparsed_args`` to the remaining unparsed arguments.
+		This function sets ``self.unparsed_args`` to the remaining unparsed arguments.
 		"""
 		pos = 0
 		still_unparsed = []
 		# parse main arguments -- optional and leftover actions:
 		while pos < len(self.unparsed_args):
 			arg = self.unparsed_args[pos]
 			if arg in options.keys():
@@ -151,14 +151,19 @@
 				self.action = "version"
 			elif self.default_action:
 				self.action = self.default_action
 			else:
 				raise ArgParseError(f"No action specified. Specify one of: {' '.join(sorted(self.defined_actions))}")
 		self.unparsed_args = still_unparsed
 
+	def check_for_unrecognized_options(self):
+		for arg in self.unparsed_args:
+			if arg.startswith("--"):
+				raise ArgParseError(f"Unrecognized option: {arg}")
+
 	def parse_positionals(self):
 		if self.action in self.final_positionals:
 			fin_pos = self.final_positionals[self.action]
 			if len(self.unparsed_args) < len(fin_pos):
 				missing = len(fin_pos) - len(self.unparsed_args)
 				out = "Expecting additional argument"
 				if missing == 1:
@@ -200,13 +205,14 @@
 			self.parse_settings(self.global_settings)
 		if self.defined_actions:
 			self.parse_action()
 		if self.action in self.action_options:
 			self.parse_options(self.action_options[self.action])
 		if self.action in self.action_settings:
 			self.parse_settings(self.action_settings[self.action])
+		self.check_for_unrecognized_options()
 		self.parse_positionals()
 		if self.action == "help":
 			self.do_help()
 		elif self.action == "version":
 			self.do_version()
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/config_files.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/config_files.py`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/const.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	}
 
 	action_settings = {
 		"build": {
 			"--kernel": None,
 			"--compression": "xz",
 			"--temp_root": "/var/tmp",
-			"--enable": "",
+			"--plugins": "",
 			"--kmod_config": "full",
 			"--kpop": None,
 		}
 	}
 
 	final_positionals = {
 		"build": ["destination"],
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/initramfs.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/initramfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 		self.compression = self.args.values.compression
 		self.module_scanner = None
 		self.size_initial = None
 		self.size_final = None
 		self.size_compressed = None
 		# When creating initramfs, enable correct plugins:
 		self.enabled_plugins = {"core"}
-		if self.args.values.enable:
-			enabled_plugins = self.args.values.enable.split(",")
+		if self.args.values.plugins:
+			enabled_plugins = self.args.values.plugins.split(",")
 			self.enabled_plugins |= set(enabled_plugins)
 		self.kernel_version = None
 		self.current_version = None
 
 	def iter_plugins(self):
 		for plugin in self.plugins.keys():
 			if plugin in self.enabled_plugins:
@@ -101,17 +101,22 @@
 
 	def setup_linuxrc_and_etc(self):
 		dest = os.path.join(self.initramfs_root, "init")
 		shutil.copy(os.path.join(self.support_root, "linuxrc"), dest)
 		os.symlink("init", os.path.join(self.initramfs_root, "linuxrc"))
 		os.symlink("../init", os.path.join(self.initramfs_root, "sbin/init"))
 		for file in os.listdir(os.path.join(self.support_root, "etc")):
-			shutil.copy(os.path.join(self.support_root, "etc", file), os.path.join(self.initramfs_root, "etc"))
+			src = os.path.join(self.support_root, "etc", file)
+			if os.path.isfile(src):
+				shutil.copy(src, os.path.join(self.initramfs_root, "etc"))
 		for x in ["init", "etc/initrd.scripts", "etc/initrd.defaults"]:
-			os.chmod(os.path.join(self.initramfs_root, x), 0O755)
+			os.chmod(os.path.join(self.initramfs_root, x), 0o755)
+		os.makedirs(os.path.join(self.initramfs_root, "etc/plugins/scan_mode"), exist_ok=True)
+		for file in os.listdir(os.path.join(self.support_root, "etc/plugins/scan_mode")):
+			shutil.copy(os.path.join(self.support_root, "etc/plugins/scan_mode", file), os.path.join(self.initramfs_root, "etc/plugins/scan_mode"))
 
 	def setup_busybox(self):
 		self.copy_binary("/bin/busybox")
 		self.copy_binary("/sbin/modprobe")
 		# Make sure these applets exist even before we tell busybox to create all the applets on initramfs:
 		for applet in [
 			"ash",
@@ -167,14 +172,22 @@
 		self.log.info("Starting modules processing...")
 		os.makedirs(f"{self.initramfs_root}/lib/modules", exist_ok=True)
 		self.module_scanner.populate_initramfs(initial_ramdisk=self)
 
 	def copy_binary(self, binary, out_path=None):
 		copy_binary(binary, dest_root=self.initramfs_root, out_path=out_path)
 
+	def install_activation_script(self, name, contents):
+		plugins_dir = os.path.join(self.initramfs_root, "etc/plugins")
+		os.makedirs(plugins_dir, exist_ok=True)
+		script_fn = os.path.join(plugins_dir, f"{name}.sh")
+		with open(script_fn, "w") as script_file:
+			script_file.write(contents)
+		os.chmod(script_fn, 0o775)
+
 	def display_enabled_plugins(self):
 		if self.plugins:
 			out_list = []
 			for plugin in sorted(self.plugins.keys()):
 				if plugin in self.enabled_plugins:
 					out_list.append(f"[orange1]{plugin}[default]")
 				else:
@@ -223,15 +236,15 @@
 			link = os.path.join(self.args.values.fs_root, "usr/src/linux")
 			if not os.path.islink(link):
 				self.log.error(f"Default linux symlink at {link} not found -- please specify a kernel. Type 'ramdisk list kernels' for a list.")
 			else:
 				self.kernel_version = get_kernel_version_from_symlink(link)
 		else:
 			if self.args.values.kernel not in self.valid_kernel_versions:
-				self.log.error(f"Specified kernel version '{self.args.kernel}' not found. Type 'ramdisk list kernels' to see list of all kernels.")
+				self.log.error(f"Specified kernel version '{self.args.values.kernel}' not found. Type 'ramdisk list kernels' to see list of all kernels.")
 			else:
 				self.kernel_version = self.args.values.kernel
 		if not self.kernel_version:
 			raise ValueError("Kernel not found")
 		self.current_version = get_current_kernel_version()
 		if self.kernel_version == self.current_version:
 			self.log.info(f"Building initramfs for: [orange1]{self.kernel_version}[default] (currently-active kernel)")
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/kernel.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/kernel.py`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/log.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/log.py`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/modules.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,16 @@
 
 		# Copy over modules.order file, but strip out lines for modules that don't exist on the initramfs. This is actually
 		# pretty easy to do, and is an easy way to get a total copied modules count:
 
 		mod_order = os.path.join(src_modroot, "modules.order")
 		if os.path.exists(mod_order):
 			with open(mod_order, "r") as mod_f:
+				if not os.path.exists(out_path):
+					os.makedirs(out_path, exist_ok=True)
 				with open(os.path.join(out_path, "modules.order"), "w") as mod_f_out:
 					for line in mod_f.readlines():
 						if line.strip() in all_subpaths:
 							mod_f_out.write(line)
 
 		self.log.info(f"[turquoise2]{mod_count}[default] kernel modules copied to initramfs.")
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/plugin_base.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/plugin_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,21 +15,31 @@
 	@property
 	def binaries(self):
 		yield
 
 	def __init__(self, ramdisk):
 		self.ramdisk = ramdisk
 
+	@property
+	def activation_script(self):
+		return None
+
 	def run(self):
 		for binary in self.binaries:
 			try:
 				if isinstance(binary, tuple):
 					final_name = binary[1]
 					binary = binary[0]
 				else:
 					final_name = binary
-				self.ramdisk.log.info(f"Copying [turquoise2]{binary}[default] to initramfs...")
+				if binary == final_name:
+					self.ramdisk.log.info(f"Copying [turquoise2]{binary}[default] to initramfs...")
+				else:
+					self.ramdisk.log.info(f"Copying [turquoise2]{binary}[default] to initramfs as [turquoise2]{final_name}[default]...")
 				self.ramdisk.copy_binary(binary, out_path=final_name)
 			except BinaryNotFoundError as bne:
 				self.ramdisk.log.error(f"Required binary [turquoise2]{bne.binary}[default] for plugin [orange1]{self.key}[default] does not exist. Please emerge {bne.dep} to fix this.")
 				return False
+		script = self.activation_script
+		if script is not None:
+			self.ramdisk.install_activation_script(self.key, script)
 		return True
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/etc/initrd.scripts` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/etc/initrd.scripts`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/bin/ash
 
-. /etc/initrd.defaults
-
 parse_cmdline() {
 	for x in $(cat /proc/cmdline)
 	do
 		case "${x}" in
 			real_root=*)
 				REAL_ROOT=${x#*=}
 			;;
@@ -27,44 +25,62 @@
 			quick)
 				# enhanced module loading:
 				QUICK='yes'
 			;;
 			slow)
 				QUICK=''
 			;;
+	    ramdisk.activate=*)
+	      PLUGINS="${x#*=}"
+	      PLUGINS="${PLUGINS/,/ }"
+	    ;;
+	    ramdisk.scan_mode=*)
+	      scan_mode="${x#*=}"
+	      if [ "$scan_mode" != "" ]; then
+	        SCAN_MODE=$scan_mode
+	      fi
+	      ;;
 			magic=*)
 				# specify magic list of modules to try, comma separated:
 				MAGIC="${x#*=}"
-				MAGIC="${x/,/ }"
+				MAGIC="${MAGIC/,/ }"
 			;;
 			real_rootflags=*)
 				REAL_ROOTFLAGS=${x#*=}
 			;;
 			rootfstype=*)
 				ROOTFSTYPE=${x#*=}
 			;;
 		esac
 	done
 }
 
+execute_plugins() {
+  local source_file
+  for plugin in $PLUGINS; do
+    source_file="/etc/plugins/${plugin}.sh"
+    if [ ! -e "${source_file}" ]; then
+      bad_msg "Specified ramdisk.activate plugin $plugin does not exist at $source_file -- cannot execute!"
+      sleep 10
+    else
+      good_msg "Executing plugin at ${source_file}"
+    . ${source_file}
+    [ $? -ne 0 ] && sleep 10
+    fi
+  done
+}
+
 backup() {
 	echo -ne "\033[0G\033[0K"
 }
 
 debug_msg() {
 	[ "$DEBUG" = "yes" ] && echo "<7>funtoo-ramdisk: $*" > /dev/kmsg
 }
 
-udev_setup() {
-	good_msg 'Activating mdev'
-	touch /dev/mdev.seq
-	[ -f /proc/sys/kernel/hotplug ] && echo /sbin/mdev > /proc/sys/kernel/hotplug
-	mdev -s || bad_msg "mdev device scan failed"
-}
-
 do_modprobe() {
 	for x in ${*}; do
 		echo -ne "${BOLD}   ::${NORMAL} Loading ${x}..."
 		debug_msg do_modprobe "loading ${x}..."
 		if /sbin/modprobe -q -s "${x}" > /dev/null 2>&1; then
 			backup
 		else
@@ -208,8 +224,7 @@
 }
 
 warn_msg() {
 	msg_string=$1
 	msg_string="${msg_string:-...}"
 	[ "$2" != 1 ] && echo -e "${WARN}**${NORMAL}${BOLD} ${msg_string} ${NORMAL}"
 }
-
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/initramfs.cpio` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/initramfs.cpio`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/linuxrc` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/linuxrc`

 * *Files 10% similar despite different names*

```diff
@@ -9,67 +9,55 @@
 [ "$$" != '1' ] && bad_msg "This script must run with a PID of 1; exiting." && exit 1
 
 mount -t proc -o noexec,nosuid,nodev proc /proc >/dev/null 2>&1
 mount -o remount,rw / >/dev/null 2>&1
 
 # Set up symlinks
 /bin/busybox --install -s
-
 mkdir -p /newroot
-
 parse_cmdline
 
+. /etc/plugins/scan_mode/${SCAN_MODE}.sh
+
 if [ "$DEBUG" = "yes" ]; then
 	echo '6' > /proc/sys/kernel/printk
 else
 	echo '0' > /proc/sys/kernel/printk
 fi
 
 if [ -z "${REAL_ROOT}" ] && [  "${FAKE_ROOT}" != "/dev/ram0" ]
 then
 	REAL_ROOT="${FAKE_ROOT}"
 fi
 
 mount_devfs
-
 mount_sysfs
-
 udev_setup
 
 # if the root filesystem type was specified, load this FS module first:
 if [ ! -b "${REAL_ROOT}" ] && [ "${ROOTFSTYPE}" != "auto" ]; then
 	good_msg "Loading ${ROOTFSTYPE} filesystem..."
 	do_modprobe "$ROOTFSTYPE"
 else
 	modules_scan filesystems
 fi
 
+execute_plugins
+
 # If "magic" list of modules was specified, use this and see if this gets us the
 # root block device:
 if [ "$MAGIC" = "1" ]; then
 	good_msg "Loading magic modules..."
 	do_modprobe $MAGIC
+  if determine_root && mount_real_root && sanity_check_root; then
+	  good_msg "Use of magic modules allowed us to find the root block device early..."
+  fi
 fi
 
-
-# This is here to try the "MAGIC" modules and see if they did the trick.
-# If so, we can skip the modules scan, below:
-if [ "$MAGIC" = "1" ] && determine_root && mount_real_root && sanity_check_root; then
-	good_msg "Use of magic modules allowed us to find the root block device early..."
-fi
-
-if [ "${MOUNTED_ROOT_FS}" != '1' ] && [ "${DETECT}" != '0' ]
-then
-	good_msg "Starting modules scanning..."
-	while read -r section; do
-		modules_scan "${section}"
-		# The "quick" boot option: try to short-circuit module loading if we appear successful:
-		[ -n "$QUICK" ] && determine_root && mount_real_root && sanity_check_root && break
-	done < /etc/modules.autoload
-fi
+[ "${MOUNTED_ROOT_FS}" != "1" ] && exhaustive_modules_scan
 
 [ "$DEBUG_SHELL" = "yes" ] && run_shell good 'Debug shell requested, starting prior to mounting root fs'
 
 while [ "${MOUNTED_ROOT_FS}" != "1" ]; do
 	determine_root && mount_real_root && sanity_check_root && break
 	# If we fail, prompt user for root block device.
 	run_shell bad "I was unable to find ${REAL_ROOT}."
@@ -84,11 +72,9 @@
 		then
 			umount $fs || run_shell bad "ERROR: Failed to move and unmount the ramdisk $fs!"
 		fi
 	fi
 done
 
 sanity_check_root postmount || run_shell bad "post-mount sanity check failed."
-
 cd / && exec /sbin/switch_root -c "/dev/console" /newroot "${REAL_INIT:-/sbin/init}" "${INIT_OPTS}"
-
 run_shell bad "Something prevented us from switching into root filesystem."
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/modules.autoload` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.autoload`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/support/module_configs/full/modules.copy` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/support/module_configs/full/modules.copy`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk/utilities.py` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk/utilities.py`

 * *Files identical despite different names*

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/PKG-INFO` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.5
+Version: 1.1.6
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.5
+:Version: 1.1.6
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -127,15 +127,15 @@
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
                         ``ramdisk list kernels`` to display available options. The
                         default setting is to use the current value of the
                         ``/usr/src/linux`` symlink at the filesystem root to determine
                         which kernel to build a ramdisk for.
 --compression=<method>  Compression method to use. Default is ``xz``. Also supported: ``zstd``.
 --temp_root=<path>      Where to create temporary files. Defaults to ``/var/tmp``.
---enable=<plugins>      A comma-delimited list of plugins to enable. The ``core`` plugin is
+--plugins=<plugins>     A comma-delimited list of plugins to enable. The ``core`` plugin is
                         always enabled. Type ``ramdisk list plugins`` to see a list of available
                         plugins.
 --kmod_config=<cfg>     ``ramdisk`` supports different sets of kernel module configurations, which
                         define what kernel modules get copied to the initramfs, and which ones
                         get auto-loaded by the initramfs at boot. Default value: ``full``. This
                         is currently the only option unless overridden by ``--kpop`` (see below.)
 --kpop=<mods>           A comma-delimited list of kernel module names that you are sure, if loaded,
@@ -168,14 +168,40 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.6
+--------------------
+
+Released on April 14, 2024.
+
+This is a maintenance and minor features release.
+
+* Various minor bug fixes.
+
+* Change ``--enable`` to ``--plugins`` since it's more
+  self-explanatory.
+
+* Continue to flesh out the plugin system. I added support for
+  plugins to have an activation script which will get executed
+  on startup. This is a work in progress and I still need to
+  add support for listing needed modules for a plugin which
+  will get loaded automatically.
+
+* Fix a bug in argument parsing where the code was not scanning
+  for invalid options which could result in odd parsing behavior.
+
+* Start adding support for udev. This is not yet completed but
+  the plugin system for this has been incorporated into the
+  linuxrc.
+
+
 funtoo-ramdisk 1.1.5
 --------------------
 
 Released on September 15, 2023.
 
 This is a packaging fix for the manpage.
```

### Comparing `funtoo-ramdisk-1.1.5/funtoo_ramdisk.egg-info/SOURCES.txt` & `funtoo_ramdisk-1.1.6/funtoo_ramdisk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,11 +31,15 @@
 funtoo_ramdisk/plugins/core.py
 funtoo_ramdisk/plugins/lvm.py
 funtoo_ramdisk/support/__init__.py
 funtoo_ramdisk/support/initramfs.cpio
 funtoo_ramdisk/support/linuxrc
 funtoo_ramdisk/support/etc/initrd.defaults
 funtoo_ramdisk/support/etc/initrd.scripts
+funtoo_ramdisk/support/etc/plugins/__init__.py
+funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
+funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
+funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
 funtoo_ramdisk/support/module_configs/__init__.py
 funtoo_ramdisk/support/module_configs/full/__init__.py
 funtoo_ramdisk/support/module_configs/full/modules.autoload
 funtoo_ramdisk/support/module_configs/full/modules.copy
```

### Comparing `funtoo-ramdisk-1.1.5/make.sh` & `funtoo_ramdisk-1.1.6/make.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	cat > funtoo_ramdisk/version.py << EOF
 __version__ = "$VERSION"
 EOF
 	for x in setup.py doc/manpage.rst; do
 		sed -e "s/##VERSION##/$VERSION/g" \
 		${x}.in > ${x}
 	done
-	rst2man.py doc/manpage.rst > doc/ramdisk.8
+	rst2man doc/manpage.rst > doc/ramdisk.8
 }
 
 commit() {
 	git commit -a -m "$PKGNAME $VERSION release."
 	git tag -f "$VERSION"
 	git push
 	git push --tags -f
```

### Comparing `funtoo-ramdisk-1.1.5/setup.py` & `funtoo_ramdisk-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open("ChangeLog.rst", "r") as fh:
 	long_description += fh.read()
 
 print(long_description)
 
 setuptools.setup(
 	name="funtoo-ramdisk",
-	version="1.1.5",
+	version="1.1.6",
 	author="Daniel Robbins, Funtoo Solutions Inc.",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for creating initial ramdisks.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse",
 	scripts=["bin/ramdisk"],
```

### Comparing `funtoo-ramdisk-1.1.5/setup.py.in` & `funtoo_ramdisk-1.1.6/setup.py.in`

 * *Files identical despite different names*

