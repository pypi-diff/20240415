# Comparing `tmp/clickable-ut-8.0.1.tar.gz` & `tmp/clickable-ut-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickable-ut-8.0.1.tar", last modified: Wed Nov  8 20:40:45 2023, max compression
+gzip compressed data, was "clickable-ut-8.1.0.tar", last modified: Mon Apr 15 17:15:16 2024, max compression
```

## Comparing `clickable-ut-8.0.1.tar` & `clickable-ut-8.1.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.739050 clickable-ut-8.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35121 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3874 2023-11-08 20:40:45.739050 clickable-ut-8.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2486 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.716051 clickable-ut-8.0.1/clickable/
--rw-rw-rw-   0 root         (0) root         (0)     3000 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.718051 clickable-ut-8.0.1/clickable/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/cmake.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/custom.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/go.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/make.py
--rw-rw-rw-   0 root         (0) root         (0)     1577 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/pure.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/qbs.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/qmake.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/builders/rust.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/command_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.723051 clickable-ut-8.0.1/clickable/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15298 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/build.py
--rw-rw-rw-   0 root         (0) root         (0)     2747 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2770 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/clean.py
--rw-rw-rw-   0 root         (0) root         (0)     2909 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/clean_images.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/create.py
--rw-rw-rw-   0 root         (0) root         (0)    15590 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/desktop.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/devices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.725051 clickable-ut-8.0.1/clickable/commands/docker/
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/debug_gdb_support.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/debug_valgrind_support.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/docker_config.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/docker_support.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/go_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/multimedia_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.726051 clickable-ut-8.0.1/clickable/commands/docker/nvidia/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/nvidia/legacy_nvidia_support.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/nvidia_support.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/rust_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/theme_support.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/docker/webapp_support.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/gdb.py
--rw-rw-rw-   0 root         (0) root         (0)    14090 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/gdbserver.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/ide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.726051 clickable-ut-8.0.1/clickable/commands/idedelegates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/idedelegate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.727051 clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/
--rw-rw-rw-   0 root         (0) root         (0)    18552 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in
--rw-rw-rw-   0 root         (0) root         (0)    31576 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/Readme.md
--rw-rw-rw-   0 root         (0) root         (0)     8225 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/install.py
--rw-rw-rw-   0 root         (0) root         (0)     2704 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/log.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/logs.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/no_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     4585 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/publish.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/review.py
--rw-rw-rw-   0 root         (0) root         (0)     1859 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/run.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/screenshots.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/script.py
--rw-rw-rw-   0 root         (0) root         (0)     3465 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/test.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/update_images.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/commands/writable_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.730051 clickable-ut-8.0.1/clickable/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/base.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/build.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/clickable.schema
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/command.py
--rw-rw-rw-   0 root         (0) root         (0)     4673 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4125 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/device.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/global_config.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/ide.py
--rw-rw-rw-   0 root         (0) root         (0)     8738 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/libconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    36713 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6169 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/config/project.schema
--rw-rw-rw-   0 root         (0) root         (0)    20913 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/container.py
--rw-rw-rw-   0 root         (0) root         (0)     8748 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/device.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.730051 clickable-ut-8.0.1/clickable/system/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/access.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.731051 clickable-ut-8.0.1/clickable/system/queries/
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/queries/legacy_docker_version.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/queries/nvidia_drivers_in_use.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/query.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/require.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.731051 clickable-ut-8.0.1/clickable/system/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/requirements/nvidia_container_toolkit.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/requirements/nvidia_docker.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/system/requirements/nvidia_modprobe.py
--rw-rw-rw-   0 root         (0) root         (0)    10277 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/clickable/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.733051 clickable-ut-8.0.1/clickable_ut.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3874 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3880 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-08 20:40:45.000000 clickable-ut-8.0.1/clickable_ut.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.734051 clickable-ut-8.0.1/debian/
--rw-rw-rw-   0 root         (0) root         (0)    40038 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/control
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/copyright
--rwxrwxrwx   0 root         (0) root         (0)      728 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/rules
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.734051 clickable-ut-8.0.1/debian/source/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/debian/source/format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.737051 clickable-ut-8.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.738051 clickable-ut-8.0.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.738051 clickable-ut-8.0.1/docs/_static/images/
--rw-rw-rw-   0 root         (0) root         (0)     2647 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/_static/images/logo.png
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/_static/version.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-08 20:40:45.738051 clickable-ut-8.0.1/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/_templates/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/_templates/layout.html
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/app-templates.rst
--rwxrwxrwx   0 root         (0) root         (0)       45 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/autobuild.sh
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/builders.rst
--rw-rw-rw-   0 root         (0) root         (0)    24588 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     7065 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/commands.rst
--rw-rw-rw-   0 root         (0) root         (0)     5310 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3559 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/config.rst
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/continuous-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/debugging.rst
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/env-vars.rst
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2216 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/migration-guides.rst
--rw-rw-rw-   0 root         (0) root         (0)     3412 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/migration.rst
--rw-rw-rw-   0 root         (0) root         (0)     8684 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/migration7.rst
--rw-rw-rw-   0 root         (0) root         (0)    17091 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/project-config.rst
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     5608 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-11-08 20:40:45.739050 clickable-ut-8.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2082 2023-11-08 20:40:44.000000 clickable-ut-8.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.633488 clickable-ut-8.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35121 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      390 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-15 17:15:16.633488 clickable-ut-8.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.607488 clickable-ut-8.1.0/clickable/
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.609488 clickable-ut-8.1.0/clickable/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/cmake.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/custom.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/go.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/make.py
+-rw-rw-rw-   0 root         (0) root         (0)     1577 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/pure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/qbs.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/qmake.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/builders/rust.py
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/command_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.615488 clickable-ut-8.1.0/clickable/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15298 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/build.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2770 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     6316 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/clean_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     5349 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/create.py
+-rw-rw-rw-   0 root         (0) root         (0)    15729 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/devices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.617488 clickable-ut-8.1.0/clickable/commands/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/debug_gdb_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/debug_valgrind_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/docker_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/docker_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/go_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/multimedia_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.618488 clickable-ut-8.1.0/clickable/commands/docker/nvidia/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/nvidia_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/rust_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/theme_support.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/docker/webapp_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/gdb.py
+-rw-rw-rw-   0 root         (0) root         (0)    14090 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/gdbserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/ide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.618488 clickable-ut-8.1.0/clickable/commands/idedelegates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/idedelegate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.619488 clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/
+-rw-rw-rw-   0 root         (0) root         (0)    18552 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in
+-rw-rw-rw-   0 root         (0) root         (0)    31576 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/Readme.md
+-rw-rw-rw-   0 root         (0) root         (0)     8225 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/install.py
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/no_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/review.py
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/run.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/screenshots.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/script.py
+-rw-rw-rw-   0 root         (0) root         (0)     3465 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/update_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/commands/writable_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.622488 clickable-ut-8.1.0/clickable/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/build.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/clickable.schema
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4125 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/global_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/ide.py
+-rw-rw-rw-   0 root         (0) root         (0)     8738 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/libconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    36713 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6169 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/config/project.schema
+-rw-rw-rw-   0 root         (0) root         (0)    21603 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     8748 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.623488 clickable-ut-8.1.0/clickable/system/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/access.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.623488 clickable-ut-8.1.0/clickable/system/queries/
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/queries/legacy_docker_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/queries/nvidia_drivers_in_use.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/require.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.624488 clickable-ut-8.1.0/clickable/system/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/requirements/nvidia_container_toolkit.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/requirements/nvidia_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/system/requirements/nvidia_modprobe.py
+-rw-rw-rw-   0 root         (0) root         (0)    10479 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/clickable/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.632488 clickable-ut-8.1.0/clickable_ut.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3880 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-15 17:15:16.000000 clickable-ut-8.1.0/clickable_ut.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.627488 clickable-ut-8.1.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)    40399 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/copyright
+-rwxrwxrwx   0 root         (0) root         (0)      728 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/rules
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.627488 clickable-ut-8.1.0/debian/source/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/debian/source/format
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.631488 clickable-ut-8.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.631488 clickable-ut-8.1.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.632488 clickable-ut-8.1.0/docs/_static/images/
+-rw-rw-rw-   0 root         (0) root         (0)     2647 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/_static/images/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/_static/version.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 17:15:16.632488 clickable-ut-8.1.0/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/_templates/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/_templates/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/app-templates.rst
+-rwxrwxrwx   0 root         (0) root         (0)       45 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/autobuild.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/builders.rst
+-rw-rw-rw-   0 root         (0) root         (0)    24855 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7065 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/commands.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/continuous-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/env-vars.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2873 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/migration-guides.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8684 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/migration7.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17091 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/project-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5608 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-15 17:15:16.633488 clickable-ut-8.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2082 2024-04-15 17:15:15.000000 clickable-ut-8.1.0/setup.py
```

### Comparing `clickable-ut-8.0.1/LICENSE` & `clickable-ut-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/PKG-INFO` & `clickable-ut-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickable-ut
-Version: 8.0.1
+Version: 8.1.0
 Summary: Compile, build, and deploy Ubuntu Touch click packages all from the command line.
 Home-page: https://clickable-ut.dev/
 Author: Brian Douglass
 License: GPL3
 Project-URL: Documentation, https://clickable-ut.dev/en/latest/
 Project-URL: Source, https://gitlab.com/clickable/clickable
 Project-URL: Bug Tracker, https://gitlab.com/clickable/clickable/-/issues
```

### Comparing `clickable-ut-8.0.1/README.md` & `clickable-ut-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/__init__.py` & `clickable-ut-8.1.0/clickable/__init__.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/base.py` & `clickable-ut-8.1.0/clickable/builders/base.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/cmake.py` & `clickable-ut-8.1.0/clickable/builders/cmake.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/make.py` & `clickable-ut-8.1.0/clickable/builders/make.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/pure.py` & `clickable-ut-8.1.0/clickable/builders/pure.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/qbs.py` & `clickable-ut-8.1.0/clickable/builders/qbs.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/qmake.py` & `clickable-ut-8.1.0/clickable/builders/qmake.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/builders/rust.py` & `clickable-ut-8.1.0/clickable/builders/rust.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/cli.py` & `clickable-ut-8.1.0/clickable/cli.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/command_utils.py` & `clickable-ut-8.1.0/clickable/command_utils.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/base.py` & `clickable-ut-8.1.0/clickable/commands/base.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/build.py` & `clickable-ut-8.1.0/clickable/commands/build.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/chain.py` & `clickable-ut-8.1.0/clickable/commands/chain.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/ci.py` & `clickable-ut-8.1.0/clickable/commands/ci.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/clean.py` & `clickable-ut-8.1.0/clickable/commands/clean.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/clean_images.py` & `clickable-ut-8.1.0/clickable/commands/clean_images.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/create.py` & `clickable-ut-8.1.0/clickable/commands/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from datetime import datetime
 
 from clickable.config.constants import Constants
 from clickable.exceptions import ClickableException
+from clickable.utils import check_command
 from .base import Command
 
 COOKIECUTTER_AVAILABLE = True
 try:
     import cookiecutter.main
 except ImportError:
     COOKIECUTTER_AVAILABLE = False
@@ -148,14 +149,16 @@
         if not COOKIECUTTER_AVAILABLE:
             raise ClickableException(
                 'Cookiecutter is not available on your computer, more information '
                 'can be found here: '
                 'https://cookiecutter.readthedocs.io/en/latest/installation.html'
             )
 
+        check_command("git")
+
         config_file = os.path.join(Constants.clickable_dir, 'cookiecutter_config.yaml')
         if not os.path.isfile(config_file):
             config_file = None
 
         try:
             cookiecutter.main.cookiecutter(
                 COOKIECUTTER_URL,
```

### Comparing `clickable-ut-8.0.1/clickable/commands/desktop.py` & `clickable-ut-8.1.0/clickable/commands/desktop.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,17 @@
                 "Valgrind (--valgrind) and GDB (--gdb or --gdbserver) can not be combined."
             )
 
         if self.desktop_locale != "C" and "." not in self.desktop_locale:
             self.desktop_locale = f"{self.desktop_locale}.UTF-8"
 
     def run(self):
+        if self.container.docker_desktop:
+            raise ClickableException("Desktop Mode isn't supported when using Docker Desktop.")
+
         self.prepare_run()
         self.run_app()
 
     def prepare_run(self):
         if self.skip_build or self.custom_mode:
             self.container.setup()
         else:
```

### Comparing `clickable-ut-8.0.1/clickable/commands/devices.py` & `clickable-ut-8.1.0/clickable/commands/devices.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/debug_gdb_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/debug_gdb_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/docker_config.py` & `clickable-ut-8.1.0/clickable/commands/docker/docker_config.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/go_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/go_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/multimedia_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/multimedia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/nvidia/legacy_nvidia_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/nvidia/legacy_nvidia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py` & `clickable-ut-8.1.0/clickable/commands/docker/nvidia/nvidia_support_since_docker_version_1903.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/nvidia_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/nvidia_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/rust_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/rust_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/theme_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/theme_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/docker/webapp_support.py` & `clickable-ut-8.1.0/clickable/commands/docker/webapp_support.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/gdb.py` & `clickable-ut-8.1.0/clickable/commands/gdb.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/gdbserver.py` & `clickable-ut-8.1.0/clickable/commands/gdbserver.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/ide.py` & `clickable-ut-8.1.0/clickable/commands/ide.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in` & `clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/CMakeLists.txt.user.shared.in`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz` & `clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator/QtProject.tar.xz`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/idedelegates/qtcreator.py` & `clickable-ut-8.1.0/clickable/commands/idedelegates/qtcreator.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/install.py` & `clickable-ut-8.1.0/clickable/commands/install.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/launch.py` & `clickable-ut-8.1.0/clickable/commands/launch.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/log.py` & `clickable-ut-8.1.0/clickable/commands/log.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/logs.py` & `clickable-ut-8.1.0/clickable/commands/logs.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/publish.py` & `clickable-ut-8.1.0/clickable/commands/publish.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/review.py` & `clickable-ut-8.1.0/clickable/commands/review.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/run.py` & `clickable-ut-8.1.0/clickable/commands/run.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/script.py` & `clickable-ut-8.1.0/clickable/commands/script.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/setup.py` & `clickable-ut-8.1.0/clickable/commands/setup.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/shell.py` & `clickable-ut-8.1.0/clickable/commands/shell.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/test.py` & `clickable-ut-8.1.0/clickable/commands/test.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/update_images.py` & `clickable-ut-8.1.0/clickable/commands/update_images.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/commands/writable_image.py` & `clickable-ut-8.1.0/clickable/commands/writable_image.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/clickable.schema` & `clickable-ut-8.1.0/clickable/config/clickable.schema`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/constants.py` & `clickable-ut-8.1.0/clickable/config/constants.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/device.py` & `clickable-ut-8.1.0/clickable/config/device.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/file_helpers.py` & `clickable-ut-8.1.0/clickable/config/file_helpers.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/global_config.py` & `clickable-ut-8.1.0/clickable/config/global_config.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/libconfig.py` & `clickable-ut-8.1.0/clickable/config/libconfig.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/project.py` & `clickable-ut-8.1.0/clickable/config/project.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/config/project.schema` & `clickable-ut-8.1.0/clickable/config/project.schema`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/container.py` & `clickable-ut-8.1.0/clickable/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,23 @@
         self.docker_mode = self.config.needs_docker()
         self.minimum_version = minimum_version \
             if minimum_version \
             else __container_minimum_required__
         self.docker_image = self.config.docker_image
         self.base_docker_image = self.docker_image
 
+        self.docker_desktop = False
+
         if self.docker_mode:
             self.docker_executable = get_docker_command()
+            if self.docker_executable == 'docker':
+                format_args = "{{.OperatingSystem}}"
+                command = f'{self.docker_executable} info --format {format_args}'
+                self.docker_desktop = 'Docker Desktop' in run_subprocess_check_output(command)
+
             self.clickable_dir = f'.clickable/{self.config.build_arch}'
             if name:
                 self.clickable_dir = f'{self.clickable_dir}/{name}'
 
             self.docker_name_file = f'{self.clickable_dir}/image.json'
             self.docker_file = f'{self.clickable_dir}/Dockerfile'
 
@@ -92,23 +99,31 @@
         if env('CLICKABLE_SKIP_DOCKER_CHECKS'):
             return True
 
         check_command('systemctl')
 
         try:
             run_subprocess_check_output(
-                shlex.split('systemctl is-active --quiet snap.docker.dockerd.service'),
+                'systemctl is-active --quiet snap.docker.dockerd.service',
+                stderr=subprocess.STDOUT)
+            return True
+        except subprocess.CalledProcessError:
+            pass
+
+        try:
+            run_subprocess_check_output(
+                'systemctl is-active --quiet docker',
                 stderr=subprocess.STDOUT)
             return True
         except subprocess.CalledProcessError:
             pass
 
         try:
             run_subprocess_check_output(
-                shlex.split('systemctl is-active --quiet docker'),
+                'systemctl --user is-active --quiet docker-desktop',
                 stderr=subprocess.STDOUT)
             return True
         except subprocess.CalledProcessError:
             pass
 
         return False
 
@@ -207,14 +222,17 @@
 
         if self.user_in_docker_group_pending():
             raise ClickableException('Please log out or restart to complete')
 
     def is_docker_configured(self):
         check_command('docker')
 
+        if self.docker_desktop:
+            return True
+
         return self.docker_group_exists() and self.proccess_in_docker_group()
 
     def pull_files(self, files, dst_parent):
         os.makedirs(dst_parent, exist_ok=True)
 
         if self.config.container_mode:
             for f in files:
@@ -277,19 +295,20 @@
     def render_mounts(self, mounts):
         return " ".join([
             f"-v {host}:{container}:Z"
             for container, host in mounts.items()
         ])
 
     def render_id_mapping_string(self, mapid=os.getuid()):
-        if self.docker_executable != 'podman':
-            return ''
-        uidmap = self.render_single_id_mapping_string('--uidmap', mapid)
-        gidmap = self.render_single_id_mapping_string('--gidmap', mapid)
-        return f'{uidmap} {gidmap}'
+        if self.docker_executable == 'podman':
+            uidmap = self.render_single_id_mapping_string('--uidmap', mapid)
+            gidmap = self.render_single_id_mapping_string('--gidmap', mapid)
+            return f'{uidmap} {gidmap}'
+
+        return ''
 
     def render_single_id_mapping_string(self, flag, mapid):
         # e.g. "--uidmap 1000:0:1 --uidmap 0:1:1000"
         return f'{flag} {mapid}:0:1 {flag} 0:1:{mapid}'
 
     def run_command(self,
                     command,
@@ -320,16 +339,18 @@
                 ]
                 joined_go_paths = ':'.join(docker_gopaths)
                 go_config = f'-e GOPATH={joined_go_paths}'
 
             env_vars = self.config.prepare_docker_env_vars()
 
             user = ""
-            if not root_user:
-                user = f"-u {os.getuid()}"
+            if self.docker_desktop:
+                user = '--user 0:0'
+            elif not root_user:
+                user = f"--user {os.getuid()}"
 
             id_mappings = self.render_id_mapping_string()
 
             mounts = self.render_mounts(
                 self.get_docker_mounts(transparent=[cwd, self.config.root_dir]))
 
             command_cwd = self.config.build_dir if use_build_dir else cwd
```

### Comparing `clickable-ut-8.0.1/clickable/device.py` & `clickable-ut-8.1.0/clickable/device.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/logger.py` & `clickable-ut-8.1.0/clickable/logger.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/system/queries/legacy_docker_version.py` & `clickable-ut-8.1.0/clickable/system/queries/legacy_docker_version.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/system/queries/nvidia_drivers_in_use.py` & `clickable-ut-8.1.0/clickable/system/queries/nvidia_drivers_in_use.py`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/clickable/utils.py` & `clickable-ut-8.1.0/clickable/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,21 +322,27 @@
 
 
 def make_absolute(path, change_keys=False):
     if not path:
         return path
 
     if isinstance(path, list):
-        return [make_absolute(p) for p in path]
+        return [make_absolute(p,
+                              change_keys=change_keys) for p in path]
 
     if isinstance(path, dict):
         if change_keys:
-            return {make_absolute(key): path[key] for key in path}
+            return {make_absolute(key,
+                                  change_keys=change_keys): path[key] for key in path}
 
-        return {key: make_absolute(path[key]) for key in path}
+        return {key: make_absolute(
+            path[key], change_keys=change_keys) for key in path}
+
+    if path.startswith('$'):
+        return path
 
     return os.path.abspath(path)
 
 
 def make_env_var_conform(name):
     return re.sub(r"[^A-Z0-9_]", "_", name.upper())
```

### Comparing `clickable-ut-8.0.1/clickable/version.py` & `clickable-ut-8.1.0/clickable/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 REQUESTS_AVAILABLE = True
 try:
     import requests
 except ImportError:
     REQUESTS_AVAILABLE = False
 
-__version__ = '8.0.1'
+__version__ = '8.1.0'
 
 __container_minimum_required__ = 11
 
 DATE_FORMAT = '%Y-%m-%dT%H:%M:%S'
 
 
 def show_version():
```

### Comparing `clickable-ut-8.0.1/clickable_ut.egg-info/PKG-INFO` & `clickable-ut-8.1.0/clickable_ut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickable-ut
-Version: 8.0.1
+Version: 8.1.0
 Summary: Compile, build, and deploy Ubuntu Touch click packages all from the command line.
 Home-page: https://clickable-ut.dev/
 Author: Brian Douglass
 License: GPL3
 Project-URL: Documentation, https://clickable-ut.dev/en/latest/
 Project-URL: Source, https://gitlab.com/clickable/clickable
 Project-URL: Bug Tracker, https://gitlab.com/clickable/clickable/-/issues
```

### Comparing `clickable-ut-8.0.1/clickable_ut.egg-info/SOURCES.txt` & `clickable-ut-8.1.0/clickable_ut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/debian/changelog` & `clickable-ut-8.1.0/debian/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+clickable (8.1.0) unstable; urgency=medium
+
+  * Added support for rootless Docker Desktop
+  * Released Clickable snap package
+  * Fixed bug with paths starting with a placeholder
+  * Fixed no-lock command for focal
+  * Reverted unintended CMake downgrade in Clickable containers
+
+ -- Clickable <bhdouglass+clickable@gmail.com>  Sun, 14 Apr 2024 09:08:19 -0500
+
 clickable (8.0.1) unstable; urgency=medium
 
   * Changed default framework to 20.04.1
   * Improved error message when the manifest is missing
   * Added workaround for ADB access on Xenial devices (added --xenial-adb to enforce and speed it up)
   * Fixed using gdbserver on Focal
   * Fixed shell and setup commands warning about missing project
```

### Comparing `clickable-ut-8.0.1/debian/control` & `clickable-ut-8.1.0/debian/control`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/debian/copyright` & `clickable-ut-8.1.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/debian/rules` & `clickable-ut-8.1.0/debian/rules`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/Makefile` & `clickable-ut-8.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/_static/images/logo.png` & `clickable-ut-8.1.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/app-templates.rst` & `clickable-ut-8.1.0/docs/app-templates.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/builders.rst` & `clickable-ut-8.1.0/docs/builders.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/changelog.rst` & `clickable-ut-8.1.0/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. _changelog:
 
 Changelog
 =========
 
+Changes in v8.1.0
+-----------------
+
+- Added support for rootless Docker Desktop
+- Released Clickable snap package
+- Fixed bug with paths starting with a placeholder
+- Fixed ``no-lock`` command for focal
+- Reverted unintended CMake downgrade in Clickable containers
+
 Changes in v8.0.1
 -----------------
 
 - Changed default framework to 20.04.1
 - Improved error message when the manifest is missing
 - Added workaround for ADB access on Xenial devices (added ``--xenial-adb`` to enforce and speed it up)
 - Fixed using gdbserver on Focal
```

### Comparing `clickable-ut-8.0.1/docs/commands.rst` & `clickable-ut-8.1.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/conf.py` & `clickable-ut-8.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 author = 'Clickable Team'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '8.0.1'
+version = '8.1.0'
 # The full version, including alpha/beta/rc tags.
-release = '8.0.1'
+release = '8.1.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
```

### Comparing `clickable-ut-8.0.1/docs/config.rst` & `clickable-ut-8.1.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/continuous-integration.rst` & `clickable-ut-8.1.0/docs/continuous-integration.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/debugging.rst` & `clickable-ut-8.1.0/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/env-vars.rst` & `clickable-ut-8.1.0/docs/env-vars.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/getting-started.rst` & `clickable-ut-8.1.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/index.rst` & `clickable-ut-8.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/install.rst` & `clickable-ut-8.1.0/docs/install.rst`

 * *Files 20% similar despite different names*

```diff
@@ -43,14 +43,36 @@
    source ./.venv/bin/activate
    # Install clickable
    pip install clickable-ut --upgrade
    # Create clickable app
    clickable create --dir ./
 
 
+Install as Snap
+---------------
+* Make sure you have `snapd installed <https://snapcraft.io/docs/installing-snapd>`__.
+* Run:
+
+.. code-block:: bash
+   :linenos:
+
+   # Install clickable and docker
+   sudo snap install clickable
+   sudo snap install docker
+   # Add connections
+   sudo snap connect clickable:raw-usb
+   sudo snap connect clickable:docker docker
+   sudo snap connect clickable:home
+   sudo snap connect clickable:removable-media
+   sudo snap connect clickable:network
+   sudo snap connect clickable:network-bind
+   sudo snap connect clickable:ssh-keys
+   sudo snap connect clickable:ssh-public-keys
+   sudo snap connect clickable:adb-support
+
 Install Via PPA (Ubuntu)
 ------------------------
 
 * Add the `PPA <https://launchpad.net/~bhdouglass/+archive/ubuntu/clickable>`__ to your system: ``sudo add-apt-repository ppa:bhdouglass/clickable``
 * Update your package list: ``sudo apt-get update``
 * Install clickable: ``sudo apt-get install clickable``
```

### Comparing `clickable-ut-8.0.1/docs/migration.rst` & `clickable-ut-8.1.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/migration7.rst` & `clickable-ut-8.1.0/docs/migration7.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/project-config.rst` & `clickable-ut-8.1.0/docs/project-config.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/docs/usage.rst` & `clickable-ut-8.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `clickable-ut-8.0.1/setup.py` & `clickable-ut-8.1.0/setup.py`

 * *Files identical despite different names*

