# Comparing `tmp/owega-5.5.4.tar.gz` & `tmp/owega-5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.5.4.tar", last modified: Mon Mar 25 01:36:11 2024, max compression
+gzip compressed data, was "owega-5.5.5.tar", last modified: Mon Apr 15 12:31:22 2024, max compression
```

## Comparing `owega-5.5.4.tar` & `owega-5.5.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.163715 owega-5.5.4/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-03-24 17:43:47.000000 owega-5.5.4/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15460 2024-03-25 01:36:11.163715 owega-5.5.4/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-03-24 17:43:47.000000 owega-5.5.4/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.155715 owega-5.5.4/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.160715 owega-5.5.4/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1492 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.161715 owega-5.5.4/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4378 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5850 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.161715 owega-5.5.4/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-03-24 17:43:47.000000 owega-5.5.4/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-03-24 17:43:47.000000 owega-5.5.4/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-03-24 17:43:47.000000 owega-5.5.4/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10546 2024-03-25 01:35:17.000000 owega-5.5.4/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.162715 owega-5.5.4/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-03-24 17:43:47.000000 owega-5.5.4/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    22940 2024-03-25 01:35:47.000000 owega-5.5.4/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-03-24 17:43:47.000000 owega-5.5.4/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-03-24 17:43:47.000000 owega-5.5.4/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.162715 owega-5.5.4/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-03-24 17:43:47.000000 owega-5.5.4/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1732 2024-03-24 23:10:47.000000 owega-5.5.4/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.162715 owega-5.5.4/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-03-24 17:43:47.000000 owega-5.5.4/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10076 2024-03-24 17:43:47.000000 owega-5.5.4/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-03-24 17:43:47.000000 owega-5.5.4/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-03-24 17:43:47.000000 owega-5.5.4/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11666 2024-03-24 17:43:47.000000 owega-5.5.4/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6042 2024-03-24 17:43:47.000000 owega-5.5.4/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-03-25 01:36:11.162715 owega-5.5.4/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15460 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1637 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-03-25 01:36:11.000000 owega-5.5.4/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-03-24 17:43:47.000000 owega-5.5.4/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-03-25 01:36:11.163715 owega-5.5.4/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-03-24 17:43:47.000000 owega-5.5.4/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.499942 owega-5.5.5/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-10 21:13:16.000000 owega-5.5.5/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15547 2024-04-15 12:31:22.499942 owega-5.5.5/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-10 21:13:16.000000 owega-5.5.5/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.497942 owega-5.5.5/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.498942 owega-5.5.5/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1492 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.498942 owega-5.5.5/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4378 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5850 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.498942 owega-5.5.5/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-10 21:13:16.000000 owega-5.5.5/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-10 21:13:16.000000 owega-5.5.5/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-10 21:13:16.000000 owega-5.5.5/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     8466 2024-04-15 12:28:41.000000 owega-5.5.5/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.499942 owega-5.5.5/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-10 21:13:16.000000 owega-5.5.5/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23133 2024-04-15 12:30:18.000000 owega-5.5.5/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-10 21:13:16.000000 owega-5.5.5/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-10 21:13:16.000000 owega-5.5.5/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.499942 owega-5.5.5/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-10 21:13:16.000000 owega-5.5.5/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1732 2024-04-10 21:13:16.000000 owega-5.5.5/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.499942 owega-5.5.5/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-10 21:13:16.000000 owega-5.5.5/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10076 2024-04-10 21:13:16.000000 owega-5.5.5/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-10 21:13:16.000000 owega-5.5.5/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-10 21:13:16.000000 owega-5.5.5/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11666 2024-04-10 21:13:16.000000 owega-5.5.5/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6042 2024-04-10 21:13:16.000000 owega-5.5.5/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 12:31:22.499942 owega-5.5.5/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15547 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1637 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-15 12:31:22.000000 owega-5.5.5/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-10 21:13:16.000000 owega-5.5.5/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-15 12:31:22.499942 owega-5.5.5/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-10 21:13:16.000000 owega-5.5.5/setup.py
```

### Comparing `owega-5.5.4/PKG-INFO` & `owega-5.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.5.4
+Version: 5.5.5
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.5.4 CHANGELOG:
+OWEGA v5.5.5 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -349,8 +349,10 @@
 5.5.0: Added basic support for Mistral's API (beta feature)
 5.5.1: Removed useless available_mistral and mistral_model
         variables.
 5.5.2: Added debug info on mistral's part of ask()
        Added matching for mixtral
 5.5.3: Removed debug lines that shouldn't have been left there.
 5.5.4: Fixed a debug_print never showing.
+5.5.5: Now using openai module to ask mistral API.
+       (the code is waaaay cleaner)
 ```
```

### Comparing `owega-5.5.4/README.md` & `owega-5.5.5/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.5.5/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_commands.py` & `owega-5.5.5/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_context.py` & `owega-5.5.5/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.5.5/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_dinput.py` & `owega-5.5.5/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_edit.py` & `owega-5.5.5/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_estimation.py` & `owega-5.5.5/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_finput.py` & `owega-5.5.5/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_frequency.py` & `owega-5.5.5/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_image.py` & `owega-5.5.5/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_load.py` & `owega-5.5.5/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_model.py` & `owega-5.5.5/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_presence.py` & `owega-5.5.5/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_quit.py` & `owega-5.5.5/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_save.py` & `owega-5.5.5/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_system.py` & `owega-5.5.5/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_temperature.py` & `owega-5.5.5/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_tokens.py` & `owega-5.5.5/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_top_p.py` & `owega-5.5.5/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handle_tts.py` & `owega-5.5.5/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OweHandlers/handlers.py` & `owega-5.5.5/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaFun/__init__.py` & `owega-5.5.5/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaFun/functions.py` & `owega-5.5.5/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.5.5/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaFun/utility.py` & `owega-5.5.5/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.5.5/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/OwegaSession/promptsession.py` & `owega-5.5.5/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/ask.py` & `owega-5.5.5/owega/ask.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,131 +64,83 @@
     is_mistral = False
     if ("mistral" in model) or ("mixtral" in model):
         is_mistral = True
 
     headers = {}
     data_payload = {}
 
+    client = openai.OpenAI()
+
     if is_mistral:
         if baseConf.get("debug", False):
             debug_print(f"Using Mistral API for model: {model}", True)
-        headers["Authorization"] = f"Bearer {baseConf.get('mistral_api', '')}"
-        if temp_api_key:
-            headers["Authorization"] = f"Bearer {temp_api_key}"
-        url = "https://api.mistral.ai/v1/chat/completions"
-
-        msgs = [msg for msg in messages.get_messages()]
-        for i, msg in enumerate(msgs):
-            if baseConf.get("debug", False):
-                debug_print(f'{msgs[i]}', True)
-            if i > 0:
-                if msg['role'] == 'system':
-                    msgs[i]['role'] = 'assistant'
-                    msgs[i]['content'] = f"[System note: {msg['content']}]"
-                elif msg['role'] == 'function':
-                    name = msg['name']
-                    cont = json.loads(msg['content'])
-                    if name == 'get_page':
-                        content_value = cont['page']
-                        if cont['status'] != 'OK':
-                            content_value = '[UNABLE TO FETCH PAGE]'
-                        msgs[i] = {
-                            'role': 'assistant',
-                            'content': content_value,
-                        }
-                    elif name == 'execute':
-                        content_value = ''
-                        content_value += '[COMMAND STDOUT]:\n'
-                        content_value += cont['command_stdout']
-                        content_value += '\n\n'
-                        content_value += '[COMMAND STDERR]:\n'
-                        content_value += cont['command_stderr']
-                        content_value += '\n\n'
-                        content_value += f"[RETURNED {cont['return_code']}]"
-                        msgs[i] = {
-                            'role': 'assistant',
-                            'content': content_value,
-                        }
-                    else:
-                        msgs[i] = {
-                            'role': 'assistant',
-                            'content': 'done!',
-                        }
-        if msgs[-1]['role'] != 'user':
-            msgs.append({
-                'role': 'user',
-                'content': '[Continue talking according to the given context]',
-            })
-
-        data_payload = {
-            "model": model,
-            "messages": msgs,
-            "temperature": temperature,
-            "max_tokens": max_tokens,
-            "top_p": top_p,
-        }
-
-        mistral_table = {}
-
-        try:
-            mistral_table["response"] = requests.post(
-                url, json=data_payload, headers=headers)
-            mistral_table["result_json"] = mistral_table["response"].json()
-            mistral_table["content"] = \
-                mistral_table["result_json"]['choices'][0]['message']['content']
-            messages.add_answer(mistral_table["content"])
-        except Exception as e:
-            print(f"Error making request to Mistral: {str(e)}")
-            head = headers.copy()
-            auth = 'Bearer '
-            for c in head["Authorization"].replace('Bearer ', ''):
-                auth += '*'
-            head["Authorization"] = auth
-            print(f"headers: {head}")
-            print(f"mistral_table: {mistral_table}")
+        client.base_url = 'https://api.mistral.ai/v1'
+        client.api_key = baseConf.get('mistral_api', '')
+    if False:
+        pass
     else:
         if isinstance(function_call, bool):
             if function_call:
                 function_call = "auto"
             else:
                 function_call = "none"
         response = False
         while (not response):
             try:
                 if (temp_api_key):
-                    openai.api_key = temp_api_key
+                    client.api_key = temp_api_key
                 if (temp_organization):
-                    openai.organization = temp_organization
+                    client.organization = temp_organization
                 if "vision" in model:
-                    response = openai.chat.completions.create(
+                    response = client.chat.completions.create(
                         model=model,
                         temperature=temperature,
                         max_tokens=max_tokens,
                         top_p=top_p,
                         frequency_penalty=frequency_penalty,
                         presence_penalty=presence_penalty,
                         messages=messages.get_messages_vision(),
                     )
                 else:
-                    response = openai.chat.completions.create(
-                        model=model,
-                        temperature=temperature,
-                        max_tokens=max_tokens,
-                        top_p=top_p,
-                        frequency_penalty=frequency_penalty,
-                        presence_penalty=presence_penalty,
-                        messages=messages.get_messages(),
-                        tools=functionlist_to_toollist(
-                            existingFunctions.getEnabled()),
-                        tool_choice=function_call,
-                    )
-                if (temp_api_key):
-                    openai.api_key = old_api_key
-                if (temp_organization):
-                    openai.organization = old_organization
+                    if is_mistral:
+                        try:
+                            response = client.chat.completions.create(
+                                model=model,
+                                temperature=temperature,
+                                max_tokens=max_tokens,
+                                top_p=top_p,
+                                messages=messages.get_messages(),
+                                tools=functionlist_to_toollist(
+                                    existingFunctions.getEnabled()),
+                                tool_choice=function_call,
+                            )
+                        except Exception as e:
+                            if 'function calling is not enabled for this model' in str(e).lower():
+                                response = client.chat.completions.create(
+                                    model=model,
+                                    temperature=temperature,
+                                    max_tokens=max_tokens,
+                                    top_p=top_p,
+                                    messages=messages.get_messages(),
+                                )
+                            else:
+                                openai.BadRequestError
+                    else:
+                        response = client.chat.completions.create(
+                            model=model,
+                            temperature=temperature,
+                            max_tokens=max_tokens,
+                            top_p=top_p,
+                            frequency_penalty=frequency_penalty,
+                            presence_penalty=presence_penalty,
+                            messages=messages.get_messages(),
+                            tools=functionlist_to_toollist(
+                                existingFunctions.getEnabled()),
+                            tool_choice=function_call,
+                        )
             except openai.BadRequestError as e:
                 try:
                     messages.shorten()
                 except Exception:
                     print("[Owega] Critical error... Aborting request...")
                     print("[Owega] " +
                           "Please, send the following to @darkgeem on discord")
@@ -215,33 +167,29 @@
                     function_response = \
                         existingFunctions.getFunction(function_name)(**kwargs)
                     messages.add_function(function_name, function_response)
                 response2 = False
                 while not (response2):
                     try:
                         if (temp_api_key):
-                            openai.api_key = temp_api_key
+                            client.api_key = temp_api_key
                         if (temp_organization):
-                            openai.organization = temp_organization
-                        response2 = openai.chat.completions.create(
+                            client.organization = temp_organization
+                        response2 = client.chat.completions.create(
                             model=model,
                             temperature=temperature,
                             max_tokens=max_tokens,
                             top_p=top_p,
                             frequency_penalty=frequency_penalty,
                             presence_penalty=presence_penalty,
                             messages=messages.get_messages(),
                             tools=functionlist_to_toollist(
                                 existingFunctions.getEnabled()),
                             tool_choice=function_call,
                         )
-                        if (temp_api_key):
-                            openai.api_key = old_api_key
-                        if (temp_organization):
-                            openai.organization = old_organization
                     except openai.error.InvalidRequestError:
                         messages.shorten()
                     except openai.error.ServiceUnavailableError:
                         print("[Owega] Service unavailable...", end="")
                         time.sleep(1)
                         print(" Retrying now...")
                     message = response2.choices[0].message
```

### Comparing `owega-5.5.4/owega/changelog/changelog.py` & `owega-5.5.5/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,19 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 5, 5)
+            .addLine("Now using openai module to ask mistral API.")
+            .addLine("(the code is waaaay cleaner)")
+        )
+        self.logs.append(
             ChangelogEntry(5, 5, 4)
             .addLine("Fixed a debug_print never showing.")
         )
         self.logs.append(
             ChangelogEntry(5, 5, 3)
             .addLine("Removed debug lines that shouldn't have been left there.")
         )
```

### Comparing `owega-5.5.4/owega/changelog/changelogEntry.py` & `owega-5.5.5/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/changelog/version.py` & `owega-5.5.5/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/config/baseConf.py` & `owega-5.5.5/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/conversation/conversation.py` & `owega-5.5.5/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/license.py` & `owega-5.5.5/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/owega.py` & `owega-5.5.5/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega/utils.py` & `owega-5.5.5/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/owega.egg-info/PKG-INFO` & `owega-5.5.5/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.5.4
+Version: 5.5.5
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.5.4 CHANGELOG:
+OWEGA v5.5.5 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -349,8 +349,10 @@
 5.5.0: Added basic support for Mistral's API (beta feature)
 5.5.1: Removed useless available_mistral and mistral_model
         variables.
 5.5.2: Added debug info on mistral's part of ask()
        Added matching for mixtral
 5.5.3: Removed debug lines that shouldn't have been left there.
 5.5.4: Fixed a debug_print never showing.
+5.5.5: Now using openai module to ask mistral API.
+       (the code is waaaay cleaner)
 ```
```

### Comparing `owega-5.5.4/owega.egg-info/SOURCES.txt` & `owega-5.5.5/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.5.4/setup.py` & `owega-5.5.5/setup.py`

 * *Files identical despite different names*

