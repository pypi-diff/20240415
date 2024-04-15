# Comparing `tmp/Exegol-4.3.1.tar.gz` & `tmp/exegol-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Exegol-4.3.1.tar", last modified: Fri Dec 22 16:06:58 2023, max compression
+gzip compressed data, was "exegol-4.3.2.tar", last modified: Mon Apr 15 19:22:20 2024, max compression
```

## Comparing `Exegol-4.3.1.tar` & `exegol-4.3.2.tar`

### file list

```diff
@@ -1,737 +1,750 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.365405 Exegol-4.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.365405 Exegol-4.3.1/Exegol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40167 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:58.000000 Exegol-4.3.1/Exegol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-22 16:06:25.000000 Exegol-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-12-22 16:06:58.365405 Exegol-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2023-12-22 16:06:25.000000 Exegol-4.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.353405 Exegol-4.3.1/exegol/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/config/ConstantConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/config/DataCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/config/EnvInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8374 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/config/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.357406 Exegol-4.3.1/exegol/console/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/ConsoleFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/ExegolProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/ExegolPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/LayerTextColumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/MetaGitProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)    26653 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/TUI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.357406 Exegol-4.3.1/exegol/console/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/ExegolCompleter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/ParametersManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.357406 Exegol-4.3.1/exegol/console/cli/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/actions/Command.py
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/actions/ExegolParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/actions/GenericParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/console/cli/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.357406 Exegol-4.3.1/exegol/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/exceptions/ExegolExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.357406 Exegol-4.3.1/exegol/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/manager/ExegolController.py
--rw-r--r--   0 runner    (1001) docker     (127)    31116 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/manager/ExegolManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    21487 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/manager/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.361405 Exegol-4.3.1/exegol/model/
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/CacheModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    72431 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/ContainerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/ExegolContainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/ExegolContainerTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33485 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/ExegolImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/ExegolModules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/MetaImages.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/SelectableInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.361405 Exegol-4.3.1/exegol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/ContainerLogStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/DataFileUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33051 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/DockerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/ExeLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/FsUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/GitUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/GuiUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/MetaSingleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/WebUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/argParse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.365405 Exegol-4.3.1/exegol/utils/imgsync/
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/imgsync/ImageScriptSync.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/imgsync/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5110 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/imgsync/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2188 2023-12-22 16:06:25.000000 Exegol-4.3.1/exegol/utils/imgsync/spawn.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/ad.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/light.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/osint.dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/sources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.225405 Exegol-4.3.1/exegol-docker-build/sources/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    54321 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound/customqueries.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound-ce/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-reset
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-stop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/UserConfigCommunity.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3005 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.229405 Exegol-4.3.1/exegol-docker-build/sources/assets/crackmapexec/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/crackmapexec/cme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.233405 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/
--rw-r--r--   0 runner    (1001) docker     (127)   670539 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.233405 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/bloodhound.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/burpsuite.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/ghidra.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/jd-gui.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/maltego.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/remmina.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/applications/wireshark.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.233405 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/bin/desktop-restart
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/bin/desktop-start
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/bin/desktop-stop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.237405 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/config
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/docklike-2.rc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/exegol.directory
--rw-r--r--   0 runner    (1001) docker     (127)    83326 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png
--rw-r--r--   0 runner    (1001) docker     (127)   101362 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png
--rw-r--r--   0 runner    (1001) docker     (127)    91894 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xstartup.conf
--rw-r--r--   0 runner    (1001) docker     (127)    81901 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/exegol_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.237405 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (127)   117551 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/default.png
--rw-r--r--   0 runner    (1001) docker     (127)   123335 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png
--rw-r--r--   0 runner    (1001) docker     (127)   123905 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png
--rw-r--r--   0 runner    (1001) docker     (127)   123311 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png
--rw-r--r--   0 runner    (1001) docker     (127)    78352 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png
--rw-r--r--   0 runner    (1001) docker     (127)    75451 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/space.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.237405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.237405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    11136 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/apt/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/apt/keys.list
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/apt/packages.list
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/apt/sources.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/firefox/addons.txt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/python3/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/python3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.241405 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/zsh/aliases
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/zsh/history
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/zsh/zshrc
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)  1703936 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/places.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/user-setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.cme
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.describeTicket
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.getgpppassword
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.rbcd
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.secretsdump
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/grc/grc.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/logrotate/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/logrotate/exegol_vpn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/netexec/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/netexec/nxc.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/patches/cloudmapper.patch
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/proxychains/
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/proxychains/proxychains.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.245405 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.277405 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/LDAPWordlistHarvester
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/MurMurHash
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/PassTheCert
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/Xspear
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/_init
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/arsenal
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bat
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bettercap
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/blackbird
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/blazy
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bolt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/bqm
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/brakeman
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/burpsuite
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/cewl
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/checksec
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/cloudmapper
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/cloudsploit
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/clusterd
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/corscanner
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/dnschef
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/drupwn
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/eaphammer
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/emacs-nox
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/empire
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/enyx
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/evil-winrm
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/extractbitlockerkeys
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/eyewitness
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/finalrecon
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/fuxploider
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/fzf
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/gdb
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/geopincer
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ghidra
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ghunt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/gittools
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/gopherus
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/gpp-decrypt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/grc
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/h2csmuggler
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/haiti
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/havoc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/httpmethods
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ida
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/impacket
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/infoga
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/jd-gui
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/jdwp-shellifier
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/joomscan
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/jwt_tool
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/kraken
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/libmspack
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/linkfinder
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/manspider
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/metasploit
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/mobsf
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/netexec
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/nmap
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/noPac
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/nosqlmap
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ntlm_theft
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/oneforall
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pass-station
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/patator
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pcredz
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/peepdf
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/photon
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/php
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/php_filter_chain_generator
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/phpggc
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/polenum
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/powershell
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/proxychains
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pwnedornot
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pygpoabuse
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pykek
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pyrit
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/python3
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/recondog
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/responder
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/routersploit
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/rsactftool
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/sherlock
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/smali
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/soapui
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ssrfmap
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/starkiller
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/symfony-exploits
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/teamsphisher
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/testssl
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/timing_attack
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/tls-map
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/tomcatwardeployer
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/trid
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/trilium
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/username-anarchy
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/villain
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/volatility2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/weevely
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/whatweb
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/wifite
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/wpscan
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/xmllint
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/xsel
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/xsser
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/xsstrike
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/ysoserial
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/zsteg
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/bashrc
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/exegol_shells_rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.349405 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/GPOddity
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/LDAPWordlistHarvester
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/MurMurHash
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/PassTheCert
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/XSpear
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/_init
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/abuseACL
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/aclpwn
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/adb
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/adidnsdump
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/amass
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/amber
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/androguard
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/anew
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/apksigner
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/apktool
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/arjun
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/arsenal
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ascii
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/assetfinder
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/autorecon
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/avrdude
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/aws
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/azure-cli
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bettercap
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/binwalk
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/blackbird
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bloodhound
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bloodhound-ce-py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bloodhound-import
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bolt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bqm
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/brakeman
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bruteforce-luks
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/bully
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/burpsuite
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/buster
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/byp4xx
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/censys
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/certipy
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/certsync
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cewl
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cewler
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/chainsaw
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/checksec
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/chisel
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cloudmapper
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/clusterd
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cmsmap
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/coercer
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/constellation
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/corscanner
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cowpatty
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/crunch
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ctf-party
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cupp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/curl
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dex2jar
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dirb
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dirsearch
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/divideandscan
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dnschef
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dnsenum
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dnsutils
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/dnsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/donpapi
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/droopescan
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/drupwn
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/eaphammer
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/empire
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/enum4linux-ng
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/enyx
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/evil-winrm
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/exif
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/exifprobe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/exiftool
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/exiv2
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/extractbitlockerkeys
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/eyewitness
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/faketime
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/fcrackzip
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/fdisk
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ffuf
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/fierce
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/finalrecon
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/findomain
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/firefox
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/foremost
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/freeipscanner
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/frida
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/fuxploider
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gau
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gdb
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/genusernames
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/geopincer
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/geowordlists
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gf
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ghidra
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/git-dumper
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/github-email
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gittools
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gobuster
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/goldencopy
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gomapenum
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gopherus
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gosecretsdump
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/goshs
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gowitness
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gpp-decrypt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gqrx
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/gron
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/h2csmuggler
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/h8mail
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hackrf
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/haiti
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hakrawler
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hakrevdns
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hashcat
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hashonymize
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/havoc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hcxdumptool
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hcxtools
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hexedit
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/holehe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hping3
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/httpmethods
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/httprobe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/httpx
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hydra
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ida
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ignorant
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/imagemagick
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/impacket
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/infoga
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ipinfo
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/iptables
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/jackit
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/jadx
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/jd-gui
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/jdwp-shellifier
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/joomscan
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/jwt_tool
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/keepwn
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kerbrute
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kiterunner
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kraken
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kubectl
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ldapdomaindump
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ldapsearch
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ldeep
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/legba
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/libmspack
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/libnfc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ligolo-ng
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/linkfinder
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/lsassy
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/maigret
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/maltego
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/manspider
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/masky
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/masscan
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mfcuk
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mfoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/minicom
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mitm6
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mobsf
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/msprobe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/naabu
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/name-that-hash
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nasm
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nbtscan
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/netdiscover
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/netexec
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ngrok
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nmap
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/noPac
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/notify
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ntlm_theft
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ntpdate
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nuclei
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/objection
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/objectwalker
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/oneforall
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/onesixtyone
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/osrframework
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pass-station
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/patator
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pcredz
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pdfcrack
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/peepdf
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/phoneinfoga
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/photon
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/php_filter_chain_generator
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/phpggc
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pkcrack
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/polenum
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/powershell
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pp-finder
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pre2k
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/prips
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/prowler
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/proxychains
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pwncat
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pwnedornot
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pwninit
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pygpoabuse
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pykek
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pymeta
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pypykatz
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pyrit
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pywerview
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/radare2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rdesktop
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/reaver
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/recon-ng
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/recondog
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/responder
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rlwrap
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/roastinthemiddle
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/robotstester
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rsacracker
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rsactftool
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rsync
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rtl-433
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ruler
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rusthound
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rustscan
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rustscan-ce
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/samba
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/samdump2
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/scout
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/scrcpy
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/scrtdnsdump
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/searchsploit
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/semgrep
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/shellerator
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/shuffledns
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sipvicious_svcrack
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sliver
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smali
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smartbrute
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smbclient
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smbmap
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smtp-user-enum
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/snmp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sprayhound
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sqlmap
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ssh
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sshuttle
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sslscan
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sslyze
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ssrfmap
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/steghide
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/stegolsb
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/stegosuite
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/strace
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/subfinder
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/sublist3r
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/swaks
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/symfony-exploits
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tcpdump
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/teamsphisher
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/testdisk
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/testssl
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/timing_attack
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tls-map
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tomcatwardeployer
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tor
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/toutatis
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/traceroute
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/trevorspray
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/trid
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/trilium
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tshark
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/twint
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/uberfile
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/updog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/username-anarchy
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/villain
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/volatility2
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wafw00f
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/waybackurls
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/webclientservicescanner
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/weevely
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wfuzz
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/whatportis
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/whatweb
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/whois
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wifite
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/windapsearch
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wireshark
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wpscan
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wuzz
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/xfreerdp
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/xsrfprobe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/xsser
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/xsstrike
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/yalis
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/youtube-dl
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/ysoserial
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/zipalign
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/zsteg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/tmux.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/shells/zshrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.349405 Exegol-4.3.1/exegol-docker-build/sources/assets/trilium/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/trilium/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/assets/trilium/trilium-manager.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/build_logs_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/code_compliance_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.349405 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/ad.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/base.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/light.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/osint.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/web.dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.353405 Exegol-4.3.1/exegol-docker-build/sources/install/
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/common.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)    63749 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_ad.sh
--rw-r--r--   0 runner    (1001) docker     (127)    20271 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_base.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_c2.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_cloud.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_code_analysis.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_cracking.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_crypto.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_desktop.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_forensic.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_iot.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_misc.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_mobile.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_most_used.sh
--rw-r--r--   0 runner    (1001) docker     (127)    15105 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_network.sh
--rw-r--r--   0 runner    (1001) docker     (127)    26809 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_osint.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_reverse.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_rfid.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_sdr.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_steganography.sh
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_voip.sh
--rw-r--r--   0 runner    (1001) docker     (127)    39289 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_web.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_wifi.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/sources/install/package_wordlists.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-22 16:06:37.000000 Exegol-4.3.1/exegol-docker-build/web.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 16:06:58.365405 Exegol-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2023-12-22 16:06:25.000000 Exegol-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 16:06:58.365405 Exegol-4.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-22 16:06:25.000000 Exegol-4.3.1/tests/test_exegol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/Exegol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 19:21:51.000000 exegol-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-15 19:22:20.332595 exegol-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-15 19:21:51.000000 exegol-4.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/ConstantConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/DataCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/EnvInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ConsoleFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ExegolProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ExegolPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/LayerTextColumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/MetaGitProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26707 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/TUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/ExegolCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/ParametersManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/ExegolParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/GenericParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/exceptions/ExegolExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/ExegolController.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31118 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/ExegolManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/CacheModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74813 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ContainerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolContainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolContainerTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33485 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolModules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/MetaImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/SelectableInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/ContainerLogStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/DataFileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34554 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/DockerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/ExeLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/FsUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/GitUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20020 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/GuiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/MetaSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/WebUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/argParse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/utils/imgsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/ImageScriptSync.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5110 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2188 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/spawn.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/osint.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.204594 exegol-4.3.2/exegol-docker-build/sources/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58751 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/customqueries.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-reset
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-stop
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/UserConfigCommunity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3005 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/crackmapexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/crackmapexec/cme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/
+-rw-r--r--   0 runner    (1001) docker     (127)   670539 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/bloodhound.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/burpsuite.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/ghidra.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/jd-gui.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/maltego.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/remmina.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/wireshark.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-restart
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-start
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-stop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/config
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/docklike-2.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/exegol.directory
+-rw-r--r--   0 runner    (1001) docker     (127)    83326 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101362 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91894 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xstartup.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    81901 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/exegol_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (127)   117551 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123335 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123905 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123311 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78352 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75451 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/space.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11378 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/keys.list
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/packages.list
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/sources.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/firefox/addons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/python3/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/python3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/aliases
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/history
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)  1703936 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/places.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/user-setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/grc/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.cme
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.describeTicket
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.getgpppassword
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.rbcd
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.secretsdump
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/grc.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/logrotate/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/logrotate/exegol_vpn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/netexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/netexec/nxc.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/cloudmapper.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/openssl.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/proxychains.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.228594 exegol-4.3.2/exegol-docker-build/sources/assets/shells/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.256595 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/LDAPWordlistHarvester
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/MurMurHash
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/Xspear
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/_init
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bat
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/blackbird
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/blazy
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/checksec
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudmapper
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudsploit
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/drupwn
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/emacs-nox
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/empire
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/extractbitlockerkeys
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fzf
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/geopincer
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ghunt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/grc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/havoc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ida
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/metasploit
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mobsf
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/netexec
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/noPac
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/nosqlmap
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ntlm_theft
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/patator
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/peepdf
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/photon
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/php
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pyrit
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/python3
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/responder
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/routersploit
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sccmhunter
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sccmwtf
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sherlock
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/smali
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/soapui
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/starkiller
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/teamsphisher
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/timing_attack
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/trid
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/villain
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/weevely
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/whatweb
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/wifite
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xmllint
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsel
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsser
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/zsteg
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/bashrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/exegol_shells_rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/GPOddity
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/LDAPWordlistHarvester
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/MurMurHash
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/XSpear
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/_init
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/abuseACL
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aclpwn
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/adb
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/adidnsdump
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/amass
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/amber
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/androguard
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/anew
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/apksigner
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/apktool
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/arjun
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ascii
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/assetfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/autorecon
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/avrdude
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aws
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/azure-cli
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/binwalk
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/blackbird
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-ce-py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-import
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodyAD
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bruteforce-luks
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bully
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/buster
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/byp4xx
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/censys
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/certipy
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/certsync
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cewler
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/chainsaw
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/checksec
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/chisel
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudmapper
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cmsmap
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/coercer
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/constellation
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cowpatty
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crunch
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ctf-party
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cupp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/curl
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dex2jar
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dirb
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dirsearch
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/divideandscan
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsenum
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsutils
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dploot
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/droopescan
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/drupwn
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/empire
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/enum4linux-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exif
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exifprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exiftool
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exiv2
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/extractbitlockerkeys
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/faketime
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fcrackzip
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fdisk
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ffuf
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fierce
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/findomain
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/firefox
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/foremost
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/freeipscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/frida
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gau
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/genusernames
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/geopincer
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/geowordlists
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gf
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/git-dumper
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/github-email
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gobuster
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/goldencopy
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gomapenum
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gosecretsdump
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/goshs
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gowitness
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gqrx
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gron
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/h8mail
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hackrf
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hakrawler
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hakrevdns
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashcat
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashonymize
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/havoc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hcxdumptool
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hcxtools
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hexedit
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/holehe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hping3
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httpx
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hydra
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ida
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ignorant
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/imagemagick
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ipinfo
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/iptables
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jackit
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jadx
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/keepwn
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kerbrute
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kiterunner
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kubectl
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapdomaindump
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapsearch
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldeep
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/legba
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libnfc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ligolo-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/lsassy
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/maigret
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/maltego
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/masky
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/masscan
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfcuk
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/minicom
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mitm6
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mobsf
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/msprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/naabu
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/name-that-hash
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nasm
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nbtscan
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/netdiscover
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/netexec
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ngrok
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/noPac
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/notify
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntlm_theft
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntpdate
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nuclei
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/objection
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/objectwalker
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/onesixtyone
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/osrframework
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/patator
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pdfcrack
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/peepdf
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/phoneinfoga
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/photon
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pkcrack
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pp-finder
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pre2k
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pretender
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/prips
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/prowler
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwncat
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwninit
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pymeta
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pypykatz
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pyrit
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywerview
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/radare2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rdesktop
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/reaver
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/recon-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/responder
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rlwrap
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/roastinthemiddle
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/robotstester
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsacracker
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsync
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rtl-433
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ruler
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rusthound
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rustscan
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rustscan-ce
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/samba
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/samdump2
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sccmhunter
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sccmwtf
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scout
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scrcpy
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scrtdnsdump
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/searchsploit
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/semgrep
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shellerator
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shuffledns
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sipvicious_svcrack
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sliver
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smali
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smartbrute
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smbclient
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smtp-user-enum
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/snmp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sprayhound
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sqlmap
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssh
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssh-audit
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sshuttle
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sslscan
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sslyze
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/steghide
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/stegolsb
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/stegosuite
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/strace
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/subfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sublist3r
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/swaks
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tcpdump
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/teamsphisher
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/testdisk
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/timing_attack
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tor
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/traceroute
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trevorspray
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trid
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tshark
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/twint
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/uberfile
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/updog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/villain
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wafw00f
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/waybackurls
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/webclientservicescanner
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/weevely
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wfuzz
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whatportis
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whatweb
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whois
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wifite
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/windapsearch
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wireshark
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wuzz
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xfreerdp
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsrfprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsser
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/yalis
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/youtube-dl
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zipalign
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zsteg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/tmux.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/zshrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/trilium-manager.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/build_logs_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/code_compliance_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/base.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/osint.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/web.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.320595 exegol-4.3.2/exegol-docker-build/sources/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/common.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    68328 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_ad.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_base.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_c2.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_cloud.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_code_analysis.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_cracking.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_crypto.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_desktop.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_forensic.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_iot.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_misc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_mobile.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_most_used.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_network.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    27488 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_osint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_reverse.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_rfid.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_sdr.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_steganography.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_voip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_web.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_wifi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_wordlists.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/web.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/wifi.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:20.332595 exegol-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 19:21:51.000000 exegol-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:21:51.000000 exegol-4.3.2/tests/test_exegol.py
```

### Comparing `Exegol-4.3.1/Exegol.egg-info/PKG-INFO` & `exegol-4.3.2/Exegol.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.3.1
+Version: 4.3.2
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
@@ -85,19 +85,9 @@
 
 <div align="center">
   <a href="https://www.capgemini.com/" title="Follow">
     <img width="300" src="https://upload.wikimedia.org/wikipedia/fr/thumb/b/b5/Capgemini_Logo.svg/1280px-Capgemini_Logo.svg.png">
   </a>
 </div>
 
-Dramelac and I work at *Capgemini* and we thank them for allocating some time for us to develop and maintain Exegol! Visit Capgemini website at https://www.capgemini.com/.
-
-___
-
-<div align="center">
-  <a href="https://www.hackthebox.com/" title="Follow">
-    <img width="300" src="https://exegol.readthedocs.io/en/latest/_images/hackthebox.png">
-  </a>
-</div>
-
-We also thank *HackTheBox* for continuously supporting the community and for helping us financially to acquire the necessary hardware for supporting multiple architectures (AMD64, ARM64). Show some love at https://www.hackthebox.com/ !
+Dramelac and I work at [Capgemini](https://www.capgemini.com/) and we thank them for believing in the project since day 1, and for allowing us to have this personal initiative keep going.
```

### Comparing `Exegol-4.3.1/Exegol.egg-info/SOURCES.txt` & `exegol-4.3.2/Exegol.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 exegol/__init__.py
 exegol/__main__.py
 exegol-docker-build/Dockerfile
 exegol-docker-build/ad.dockerfile
 exegol-docker-build/light.dockerfile
 exegol-docker-build/osint.dockerfile
 exegol-docker-build/web.dockerfile
+exegol-docker-build/wifi.dockerfile
 exegol-docker-build/sources/build_logs_report.py
 exegol-docker-build/sources/code_compliance_check.py
 exegol-docker-build/sources/assets/bloodhound/config.json
 exegol-docker-build/sources/assets/bloodhound/customqueries.json
 exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce
 exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-reset
 exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-stop
+exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json
 exegol-docker-build/sources/assets/burpsuite/UserConfigCommunity.json
 exegol-docker-build/sources/assets/burpsuite/conf.json
 exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh
 exegol-docker-build/sources/assets/crackmapexec/cme.conf
 exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz
 exegol-docker-build/sources/assets/desktop/exegol_logo.png
 exegol-docker-build/sources/assets/desktop/applications/bloodhound.desktop
@@ -84,16 +86,18 @@
 exegol-docker-build/sources/assets/grc/conf.ntlmrelayx
 exegol-docker-build/sources/assets/grc/conf.rbcd
 exegol-docker-build/sources/assets/grc/conf.secretsdump
 exegol-docker-build/sources/assets/grc/grc.conf
 exegol-docker-build/sources/assets/logrotate/exegol_vpn
 exegol-docker-build/sources/assets/netexec/nxc.conf
 exegol-docker-build/sources/assets/patches/cloudmapper.patch
+exegol-docker-build/sources/assets/patches/openssl.patch
 exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch
 exegol-docker-build/sources/assets/proxychains/proxychains.conf
+exegol-docker-build/sources/assets/python/requirements.txt
 exegol-docker-build/sources/assets/shells/bashrc
 exegol-docker-build/sources/assets/shells/exegol_shells_rc
 exegol-docker-build/sources/assets/shells/tmux.conf
 exegol-docker-build/sources/assets/shells/zshrc
 exegol-docker-build/sources/assets/shells/aliases.d/LDAPWordlistHarvester
 exegol-docker-build/sources/assets/shells/aliases.d/MurMurHash
 exegol-docker-build/sources/assets/shells/aliases.d/PassTheCert
@@ -211,14 +215,16 @@
 exegol-docker-build/sources/assets/shells/aliases.d/python3
 exegol-docker-build/sources/assets/shells/aliases.d/pywhisker
 exegol-docker-build/sources/assets/shells/aliases.d/pywsus
 exegol-docker-build/sources/assets/shells/aliases.d/recondog
 exegol-docker-build/sources/assets/shells/aliases.d/responder
 exegol-docker-build/sources/assets/shells/aliases.d/routersploit
 exegol-docker-build/sources/assets/shells/aliases.d/rsactftool
+exegol-docker-build/sources/assets/shells/aliases.d/sccmhunter
+exegol-docker-build/sources/assets/shells/aliases.d/sccmwtf
 exegol-docker-build/sources/assets/shells/aliases.d/shadowcoerce
 exegol-docker-build/sources/assets/shells/aliases.d/sherlock
 exegol-docker-build/sources/assets/shells/aliases.d/simplyemail
 exegol-docker-build/sources/assets/shells/aliases.d/smali
 exegol-docker-build/sources/assets/shells/aliases.d/smuggler
 exegol-docker-build/sources/assets/shells/aliases.d/soapui
 exegol-docker-build/sources/assets/shells/aliases.d/spiderfoot
@@ -280,14 +286,15 @@
 exegol-docker-build/sources/assets/shells/history.d/binwalk
 exegol-docker-build/sources/assets/shells/history.d/blackbird
 exegol-docker-build/sources/assets/shells/history.d/bloodhound
 exegol-docker-build/sources/assets/shells/history.d/bloodhound-ce-py
 exegol-docker-build/sources/assets/shells/history.d/bloodhound-import
 exegol-docker-build/sources/assets/shells/history.d/bloodhound-py
 exegol-docker-build/sources/assets/shells/history.d/bloodhound-quickwin
+exegol-docker-build/sources/assets/shells/history.d/bloodyAD
 exegol-docker-build/sources/assets/shells/history.d/bolt
 exegol-docker-build/sources/assets/shells/history.d/bqm
 exegol-docker-build/sources/assets/shells/history.d/brakeman
 exegol-docker-build/sources/assets/shells/history.d/bruteforce-luks
 exegol-docker-build/sources/assets/shells/history.d/bully
 exegol-docker-build/sources/assets/shells/history.d/burpsuite
 exegol-docker-build/sources/assets/shells/history.d/buster
@@ -324,14 +331,15 @@
 exegol-docker-build/sources/assets/shells/history.d/dirsearch
 exegol-docker-build/sources/assets/shells/history.d/divideandscan
 exegol-docker-build/sources/assets/shells/history.d/dnschef
 exegol-docker-build/sources/assets/shells/history.d/dnsenum
 exegol-docker-build/sources/assets/shells/history.d/dnsutils
 exegol-docker-build/sources/assets/shells/history.d/dnsx
 exegol-docker-build/sources/assets/shells/history.d/donpapi
+exegol-docker-build/sources/assets/shells/history.d/dploot
 exegol-docker-build/sources/assets/shells/history.d/droopescan
 exegol-docker-build/sources/assets/shells/history.d/drupwn
 exegol-docker-build/sources/assets/shells/history.d/eaphammer
 exegol-docker-build/sources/assets/shells/history.d/empire
 exegol-docker-build/sources/assets/shells/history.d/enum4linux-ng
 exegol-docker-build/sources/assets/shells/history.d/enyx
 exegol-docker-build/sources/assets/shells/history.d/evil-winrm
@@ -477,14 +485,15 @@
 exegol-docker-build/sources/assets/shells/history.d/phpggc
 exegol-docker-build/sources/assets/shells/history.d/pkcrack
 exegol-docker-build/sources/assets/shells/history.d/pkinittools
 exegol-docker-build/sources/assets/shells/history.d/polenum
 exegol-docker-build/sources/assets/shells/history.d/powershell
 exegol-docker-build/sources/assets/shells/history.d/pp-finder
 exegol-docker-build/sources/assets/shells/history.d/pre2k
+exegol-docker-build/sources/assets/shells/history.d/pretender
 exegol-docker-build/sources/assets/shells/history.d/prips
 exegol-docker-build/sources/assets/shells/history.d/privexchange
 exegol-docker-build/sources/assets/shells/history.d/prowler
 exegol-docker-build/sources/assets/shells/history.d/proxmark3
 exegol-docker-build/sources/assets/shells/history.d/proxychains
 exegol-docker-build/sources/assets/shells/history.d/pth-tools
 exegol-docker-build/sources/assets/shells/history.d/pwncat
@@ -516,14 +525,16 @@
 exegol-docker-build/sources/assets/shells/history.d/rtl-433
 exegol-docker-build/sources/assets/shells/history.d/ruler
 exegol-docker-build/sources/assets/shells/history.d/rusthound
 exegol-docker-build/sources/assets/shells/history.d/rustscan
 exegol-docker-build/sources/assets/shells/history.d/rustscan-ce
 exegol-docker-build/sources/assets/shells/history.d/samba
 exegol-docker-build/sources/assets/shells/history.d/samdump2
+exegol-docker-build/sources/assets/shells/history.d/sccmhunter
+exegol-docker-build/sources/assets/shells/history.d/sccmwtf
 exegol-docker-build/sources/assets/shells/history.d/scout
 exegol-docker-build/sources/assets/shells/history.d/scrcpy
 exegol-docker-build/sources/assets/shells/history.d/scrtdnsdump
 exegol-docker-build/sources/assets/shells/history.d/searchsploit
 exegol-docker-build/sources/assets/shells/history.d/semgrep
 exegol-docker-build/sources/assets/shells/history.d/shadowcoerce
 exegol-docker-build/sources/assets/shells/history.d/shellerator
@@ -538,14 +549,15 @@
 exegol-docker-build/sources/assets/shells/history.d/smtp-user-enum
 exegol-docker-build/sources/assets/shells/history.d/smuggler
 exegol-docker-build/sources/assets/shells/history.d/snmp
 exegol-docker-build/sources/assets/shells/history.d/spiderfoot
 exegol-docker-build/sources/assets/shells/history.d/sprayhound
 exegol-docker-build/sources/assets/shells/history.d/sqlmap
 exegol-docker-build/sources/assets/shells/history.d/ssh
+exegol-docker-build/sources/assets/shells/history.d/ssh-audit
 exegol-docker-build/sources/assets/shells/history.d/sshuttle
 exegol-docker-build/sources/assets/shells/history.d/sslscan
 exegol-docker-build/sources/assets/shells/history.d/sslyze
 exegol-docker-build/sources/assets/shells/history.d/ssrfmap
 exegol-docker-build/sources/assets/shells/history.d/steghide
 exegol-docker-build/sources/assets/shells/history.d/stegolsb
 exegol-docker-build/sources/assets/shells/history.d/stegosuite
```

### Comparing `Exegol-4.3.1/LICENSE` & `exegol-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/PKG-INFO` & `exegol-4.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.3.1
+Version: 4.3.2
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
@@ -85,19 +85,9 @@
 
 <div align="center">
   <a href="https://www.capgemini.com/" title="Follow">
     <img width="300" src="https://upload.wikimedia.org/wikipedia/fr/thumb/b/b5/Capgemini_Logo.svg/1280px-Capgemini_Logo.svg.png">
   </a>
 </div>
 
-Dramelac and I work at *Capgemini* and we thank them for allocating some time for us to develop and maintain Exegol! Visit Capgemini website at https://www.capgemini.com/.
-
-___
-
-<div align="center">
-  <a href="https://www.hackthebox.com/" title="Follow">
-    <img width="300" src="https://exegol.readthedocs.io/en/latest/_images/hackthebox.png">
-  </a>
-</div>
-
-We also thank *HackTheBox* for continuously supporting the community and for helping us financially to acquire the necessary hardware for supporting multiple architectures (AMD64, ARM64). Show some love at https://www.hackthebox.com/ !
+Dramelac and I work at [Capgemini](https://www.capgemini.com/) and we thank them for believing in the project since day 1, and for allowing us to have this personal initiative keep going.
```

### Comparing `Exegol-4.3.1/README.md` & `exegol-4.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,19 +53,9 @@
 
 <div align="center">
   <a href="https://www.capgemini.com/" title="Follow">
     <img width="300" src="https://upload.wikimedia.org/wikipedia/fr/thumb/b/b5/Capgemini_Logo.svg/1280px-Capgemini_Logo.svg.png">
   </a>
 </div>
 
-Dramelac and I work at *Capgemini* and we thank them for allocating some time for us to develop and maintain Exegol! Visit Capgemini website at https://www.capgemini.com/.
-
-___
-
-<div align="center">
-  <a href="https://www.hackthebox.com/" title="Follow">
-    <img width="300" src="https://exegol.readthedocs.io/en/latest/_images/hackthebox.png">
-  </a>
-</div>
-
-We also thank *HackTheBox* for continuously supporting the community and for helping us financially to acquire the necessary hardware for supporting multiple architectures (AMD64, ARM64). Show some love at https://www.hackthebox.com/ !
+Dramelac and I work at [Capgemini](https://www.capgemini.com/) and we thank them for believing in the project since day 1, and for allowing us to have this personal initiative keep going.
```

### Comparing `Exegol-4.3.1/exegol/config/ConstantConfig.py` & `exegol-4.3.2/exegol/config/ConstantConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 from pathlib import Path
 
 
 class ConstantConfig:
     """Constant parameters information"""
     # Exegol Version
-    version: str = "4.3.1"
+    version: str = "4.3.2"
 
     # Exegol documentation link
     documentation: str = "https://exegol.rtfd.io/"
     discord: str = "https://discord.gg/cXThyp7D6P"
     # OS Dir full root path of exegol project
     src_root_path_obj: Path = Path(__file__).parent.parent.parent.resolve()
     # Path of the Dockerfile
```

### Comparing `Exegol-4.3.1/exegol/config/DataCache.py` & `exegol-4.3.2/exegol/config/DataCache.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/config/EnvInfo.py` & `exegol-4.3.2/exegol/config/EnvInfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+import os
 import platform
 from enum import Enum
+from pathlib import Path
 from typing import Optional, Any, List
 
 from exegol.config.ConstantConfig import ConstantConfig
 from exegol.utils.ExeLog import logger
 
 
 class EnvInfo:
@@ -13,14 +15,19 @@
 
     class HostOs(Enum):
         """Dictionary class for static OS Name"""
         WINDOWS = "Windows"
         LINUX = "Linux"
         MAC = "Mac"
 
+    class DisplayServer(Enum):
+        """Dictionary class for static Display Server"""
+        WAYLAND = "Wayland"
+        X11 = "X11"
+
     class DockerEngine(Enum):
         """Dictionary class for static Docker engine name"""
         WLS2 = "WSL2"
         HYPERV = "Hyper-V"
         DOCKER_DESKTOP = "Docker desktop"
         ORBSTACK = "Orbstack"
         LINUX = "Kernel"
@@ -104,14 +111,28 @@
         """Return Host OS
         Can be 'Windows', 'Mac' or 'Linux'"""
         # initData must be called from DockerUtils on client initialisation
         assert cls.__docker_host_os is not None
         return cls.__docker_host_os
 
     @classmethod
+    def getDisplayServer(cls) -> DisplayServer:
+        """Returns the display server
+        Can be 'X11' or 'Wayland'"""
+        session_type = os.getenv("XDG_SESSION_TYPE", "x11")
+        if session_type == "wayland":
+            return cls.DisplayServer.WAYLAND
+        elif session_type == "x11":
+            return cls.DisplayServer.X11
+        else:
+            # Should return an error
+            logger.warning(f"Unknown session type {session_type}. Using X11 as fallback.")
+            return cls.DisplayServer.X11
+
+    @classmethod
     def getWindowsRelease(cls) -> str:
         # Cache check
         if cls.__windows_release is None:
             if cls.is_windows_shell:
                 # From a Windows shell, python supply an approximate (close enough) version of windows
                 cls.__windows_release = platform.win32_ver()[1]
             else:
@@ -125,14 +146,19 @@
 
     @classmethod
     def isMacHost(cls) -> bool:
         """Return true if macOS is detected on the host"""
         return cls.getHostOs() == cls.HostOs.MAC
 
     @classmethod
+    def isWaylandAvailable(cls) -> bool:
+        """Return true if wayland is detected on the host"""
+        return cls.getDisplayServer() == cls.DisplayServer.WAYLAND or bool(os.getenv("WAYLAND_DISPLAY"))
+
+    @classmethod
     def isDockerDesktop(cls) -> bool:
         """Return true if docker desktop is used on the host"""
         return cls.__is_docker_desktop
 
     @classmethod
     def isOrbstack(cls) -> bool:
         """Return true if docker desktop is used on the host"""
```

### Comparing `Exegol-4.3.1/exegol/config/UserConfig.py` & `exegol-4.3.2/exegol/config/UserConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         shell_logging_data = config_data.get("shell_logging", {})
         self.shell_logging_method = self._load_config_str(shell_logging_data, 'logging_method', self.shell_logging_method, choices=self.shell_logging_method_options)
         self.shell_logging_compress = self._load_config_bool(shell_logging_data, 'enable_log_compression', self.shell_logging_compress)
 
         # Desktop section
         desktop_data = config_data.get("desktop", {})
         self.desktop_default_enable = self._load_config_bool(desktop_data, 'enabled_by_default', self.desktop_default_enable)
-        self.desktop_default_proto = self._load_config_str(desktop_data, 'default_proto', self.desktop_default_proto, choices=self.desktop_available_proto)
+        self.desktop_default_proto = self._load_config_str(desktop_data, 'default_protocol', self.desktop_default_proto, choices=self.desktop_available_proto)
         self.desktop_default_localhost = self._load_config_bool(desktop_data, 'localhost_by_default', self.desktop_default_localhost)
 
     def get_configs(self) -> List[str]:
         """User configs getter each options"""
         configs = [
             f"User config file: [magenta]{self._file_path}[/magenta]",
             f"Private workspace: [magenta]{self.private_volume_path}[/magenta]",
```

### Comparing `Exegol-4.3.1/exegol/console/ConsoleFormat.py` & `exegol-4.3.2/exegol/console/ConsoleFormat.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/ExegolProgress.py` & `exegol-4.3.2/exegol/console/ExegolProgress.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/LayerTextColumn.py` & `exegol-4.3.2/exegol/console/LayerTextColumn.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/MetaGitProgress.py` & `exegol-4.3.2/exegol/console/MetaGitProgress.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/TUI.py` & `exegol-4.3.2/exegol/console/TUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,18 +447,18 @@
             container_info_header += f" [{color}]({container.image.getArch()})[/{color}]"
         recap.add_column(container_info_header)
         # Main features
         if comment:
             recap.add_row("[bold blue]Comment[/bold blue]", comment)
         if passwd:
             recap.add_row(f"[bold blue]Credentials[/bold blue]", f"[deep_sky_blue3]{container.config.getUsername()}[/deep_sky_blue3] : [deep_sky_blue3]{passwd}[/deep_sky_blue3]")
-        recap.add_row("[bold blue]Desktop[/bold blue]", container.config.getDesktopConfig())
+        recap.add_row("[bold blue]Remote Desktop[/bold blue]", container.config.getDesktopConfig())
         if creation_date:
             recap.add_row("[bold blue]Creation date[/bold blue]", creation_date)
-        recap.add_row("[bold blue]X11[/bold blue]", boolFormatter(container.config.isGUIEnable()))
+        recap.add_row("[bold blue]Console GUI[/bold blue]", boolFormatter(container.config.isGUIEnable()) + container.config.getTextGuiSockets())
         recap.add_row("[bold blue]Network[/bold blue]", container.config.getTextNetworkMode())
         recap.add_row("[bold blue]Timezone[/bold blue]", boolFormatter(container.config.isTimezoneShared()))
         recap.add_row("[bold blue]Exegol resources[/bold blue]", boolFormatter(container.config.isExegolResourcesEnable()) +
                       f"{'[bright_black](/opt/resources)[/bright_black]' if container.config.isExegolResourcesEnable() else ''}")
         recap.add_row("[bold blue]My resources[/bold blue]", boolFormatter(container.config.isMyResourcesEnable()) +
                       f"{'[bright_black]({})[/bright_black]'.format(container.config.getMyResourcesPath()) if container.config.isMyResourcesEnable() else ''}")
         recap.add_row("[bold blue]Shell logging[/bold blue]", boolFormatter(container.config.isShellLoggingEnable()) +
```

### Comparing `Exegol-4.3.1/exegol/console/cli/ExegolCompleter.py` & `exegol-4.3.2/exegol/console/cli/ExegolCompleter.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/cli/ParametersManager.py` & `exegol-4.3.2/exegol/console/cli/ParametersManager.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/cli/actions/Command.py` & `exegol-4.3.2/exegol/console/cli/actions/Command.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/cli/actions/ExegolParameters.py` & `exegol-4.3.2/exegol/console/cli/actions/ExegolParameters.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/console/cli/actions/GenericParameters.py` & `exegol-4.3.2/exegol/console/cli/actions/GenericParameters.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/manager/ExegolController.py` & `exegol-4.3.2/exegol/manager/ExegolController.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/manager/ExegolManager.py` & `exegol-4.3.2/exegol/manager/ExegolManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,17 +230,17 @@
                 UpdateManager.updateWrapper()
         else:
             logger.empty_line(log_level=logging.DEBUG)
 
     @classmethod
     def print_sponsors(cls):
         """Show exegol sponsors"""
-        logger.success(
-            """We thank [link=https://www.capgemini.com/fr-fr/carrieres/offres-emploi/][blue]Capgemini[/blue][/link] for supporting the project [bright_black](helping with dev)[/bright_black] :pray:""")
-        logger.success("""We thank [link=https://www.hackthebox.com/][green]HackTheBox[/green][/link] for sponsoring the [bright_black]multi-arch[/bright_black] support :green_heart:""")
+        #logger.success("""We thank [link=https://www.capgemini.com/fr-fr/carrieres/offres-emploi/][blue]Capgemini[/blue][/link] for supporting the project [bright_black](helping with dev)[/bright_black] :pray:""")
+        #logger.success("""We thank [link=https://www.hackthebox.com/][green]HackTheBox[/green][/link] for sponsoring the [bright_black]multi-arch[/bright_black] support :green_heart:""")
+        pass
 
     @classmethod
     def __loadOrInstallImage(cls,
                              override_image: Optional[str] = None,
                              multiple: bool = False,
                              must_exist: bool = False) -> Union[Optional[ExegolImage], List[ExegolImage]]:
         """Select / Load (and install) an ExegolImage
```

### Comparing `Exegol-4.3.1/exegol/manager/UpdateManager.py` & `exegol-4.3.2/exegol/manager/UpdateManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,29 +246,36 @@
             logger.warning(f'Unable to parse Exegol version : {version} / {ConstantConfig.version}')
         return isUpToDate
 
     @classmethod
     def __get_current_version(cls):
         """Get the current version of the exegol wrapper. Handle dev version and release stable version depending on the current version."""
         current_version = ConstantConfig.version
-        if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
+        if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE) and ConstantConfig.git_source_installation:
             module = ExegolModules().getWrapperGit(fast_load=True)
             if module.isAvailable:
                 current_version = str(module.get_current_commit())[:8]
         return current_version
 
     @staticmethod
     def display_current_version():
         """Get the current version of the exegol wrapper. Handle dev version and release stable version depending on the current version."""
-        commit_version = ""
-        if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
+        version_details = ""
+        if ConstantConfig.git_source_installation:
             module = ExegolModules().getWrapperGit(fast_load=True)
             if module.isAvailable:
-                commit_version = f" [bright_black]\\[{str(module.get_current_commit())[:8]}][/bright_black]"
-        return f"[blue]v{ConstantConfig.version}[/blue]{commit_version}"
+                current_branch = module.getCurrentBranch()
+                commit_version = ""
+                if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
+                    commit_version = "-" + str(module.get_current_commit())[:8]
+                if current_branch is None:
+                    current_branch = "HEAD"
+                if current_branch != "master" or commit_version != "":
+                    version_details = f" [bright_black]\\[{current_branch}{commit_version}][/bright_black]"
+        return f"[blue]v{ConstantConfig.version}[/blue]{version_details}"
 
     @classmethod
     def __tagUpdateAvailable(cls, latest_version, current_version=None):
         """Update the 'update available' cache data."""
         DataCache().get_wrapper_data().last_version = latest_version
         DataCache().get_wrapper_data().current_version = cls.__get_current_version() if current_version is None else current_version
 
@@ -343,14 +350,16 @@
                 build_path = custom_build_path
             else:
                 logger.critical(f"The directory {custom_build_path.absolute()} doesn't contain any Dockerfile profile.")
         logger.debug(f"Using {build_path} as path for dockerfiles")
 
         # Choose dockerfile
         profiles = cls.listBuildProfiles(profiles_path=build_path)
+        if len(profiles) == 0:
+            logger.critical(f"No build profile found in {build_path}. Check your exegol installation, it seems to be broken...")
         build_profile: Optional[str] = ParametersManager().build_profile
         build_dockerfile: Optional[str] = None
         if build_profile is not None:
             build_dockerfile = profiles.get(build_profile)
             if build_dockerfile is None:
                 logger.error(f"Build profile {build_profile} not found.")
         if build_dockerfile is None:
```

### Comparing `Exegol-4.3.1/exegol/model/CacheModels.py` & `exegol-4.3.2/exegol/model/CacheModels.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/model/ContainerConfig.py` & `exegol-4.3.2/exegol/model/ContainerConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                         ExegolMetadata.comment.value: ["setComment", "getComment"],
                         ExegolMetadata.password.value: ["setPasswd", "getPasswd"]}
 
     def __init__(self, container: Optional[Container] = None):
         """Container config default value"""
         self.hostname = ""
         self.__enable_gui: bool = False
+        self.__gui_engine: List[str] = []
         self.__share_timezone: bool = False
         self.__my_resources: bool = False
         self.__my_resources_path: str = "/opt/my-resources"
         self.__exegol_resources: bool = False
         self.__network_host: bool = True
         self.__privileged: bool = False
         self.__wrapper_start_enabled: bool = False
@@ -126,18 +127,21 @@
         container_config = container.attrs.get("Config", {})
         self.tty = container_config.get("Tty", True)
         self.__parseEnvs(container_config.get("Env", []))
         self.__parseLabels(container_config.get("Labels", {}))
         self.interactive = container_config.get("OpenStdin", True)
         self.legacy_entrypoint = container_config.get("Entrypoint") is None
         self.__enable_gui = False
-        for env in self.__envs:
-            if "DISPLAY" in env:
-                self.__enable_gui = True
-                break
+        envs_key = self.__envs.keys()
+        if "DISPLAY" in envs_key:
+            self.__enable_gui = True
+            self.__gui_engine.append("X11")
+        if "WAYLAND_DISPLAY" in envs_key:
+            self.__enable_gui = True
+            self.__gui_engine.append("Wayland")
 
         # Host Config section
         host_config = container.attrs.get("HostConfig", {})
         self.__privileged = host_config.get("Privileged", False)
         caps = host_config.get("CapAdd", [])
         if caps is not None:
             self.__capabilities = caps
@@ -356,47 +360,75 @@
         if self.__vpn_path:
             command_options.append(f"--vpn {self.__vpn_path}")
 
         return command_options
 
     def enableGUI(self):
         """Procedure to enable GUI feature"""
-        if not GuiUtils.isGuiAvailable():
-            logger.error("X11 feature (i.e. GUI apps) is [red]not available[/red] on your environment. [orange3]Skipping[/orange3].")
+        x11_available = GuiUtils.isX11GuiAvailable()
+        wayland_available = GuiUtils.isWaylandGuiAvailable()
+        if not x11_available and not wayland_available:
+            logger.error("Console GUI feature (i.e. GUI apps) is [red]not available[/red] on your environment. [orange3]Skipping[/orange3].")
             return
         if not self.__enable_gui:
             logger.verbose("Config: Enabling display sharing")
-            try:
-                host_path = GuiUtils.getX11SocketPath()
-                if host_path is not None:
-                    self.addVolume(host_path, GuiUtils.default_x11_path, must_exist=True)
-            except CancelOperation as e:
-                logger.warning(f"Graphical interface sharing could not be enabled: {e}")
-                return
+            if x11_available:
+                try:
+                    host_path: Optional[Union[Path, str]] = GuiUtils.getX11SocketPath()
+                    if host_path is not None:
+                        assert type(host_path) is str
+                        self.addVolume(host_path, GuiUtils.default_x11_path, must_exist=True)
+                    # X11 can be used accros network without volume on Mac
+                    self.addEnv("DISPLAY", GuiUtils.getDisplayEnv())
+                    self.__gui_engine.append("X11")
+                except CancelOperation as e:
+                    logger.warning(f"Graphical X11 interface sharing could not be enabled: {e}")
+            else:
+                logger.warning("X11 cannot be shared, only wayland, some graphical applications might not work...")
+            if wayland_available:
+                try:
+                    host_path = GuiUtils.getWaylandSocketPath()
+                    if host_path is not None:
+                        self.addVolume(host_path.as_posix(), f"/tmp/{host_path.name}", must_exist=True)
+                        self.addEnv("XDG_SESSION_TYPE", "wayland")
+                        self.addEnv("XDG_RUNTIME_DIR", "/tmp")
+                        self.addEnv("WAYLAND_DISPLAY", GuiUtils.getWaylandEnv())
+                        self.__gui_engine.append("Wayland")
+                except CancelOperation as e:
+                    logger.warning(f"Graphical Wayland interface sharing could not be enabled: {e}")
             # TODO support pulseaudio
-            self.addEnv("DISPLAY", GuiUtils.getDisplayEnv())
             for k, v in self.__static_gui_envs.items():
                 self.addEnv(k, v)
             self.__enable_gui = True
 
     def __disableGUI(self):
         """Procedure to disable X11 (GUI) feature (Only for interactive config)"""
         if self.__enable_gui:
             self.__enable_gui = False
             logger.verbose("Config: Disabling display sharing")
             self.removeVolume(container_path="/tmp/.X11-unix")
             self.removeEnv("DISPLAY")
+            self.removeEnv("XDG_SESSION_TYPE")
+            self.removeEnv("XDG_RUNTIME_DIR")
+            self.removeEnv("WAYLAND_DISPLAY")
             for k in self.__static_gui_envs.keys():
                 self.removeEnv(k)
+            self.__gui_engine.clear()
 
     def enableSharedTimezone(self):
         """Procedure to enable shared timezone feature"""
         if EnvInfo.is_windows_shell:
             logger.warning("Timezone sharing is not supported from a Windows shell. Skipping.")
             return
+        elif EnvInfo.isMacHost():
+            # On Orbstack /etc cannot be shared + we should test how Orbstack handle symlink
+            # With docker desktop, symlink are resolved as full path on container creation. When tzdata is updated on the host, the container can no longer be started because the files of the previous package version are missing.
+            # TODO Test if env var can be used as replacement
+            logger.warning("Timezone sharing on Mac isn't supported for instability issues. Skipping.")
+            return
         if not self.__share_timezone:
             logger.verbose("Config: Enabling host timezones")
             # Try to share /etc/timezone (deprecated old timezone file)
             try:
                 self.addVolume("/etc/timezone", "/etc/timezone", read_only=True, must_exist=True)
                 logger.verbose("Volume was successfully added for [magenta]/etc/timezone[/magenta]")
                 timezone_loaded = True
@@ -555,15 +587,15 @@
                         logger.critical(f"The network {self.__desktop_host}:{self.__desktop_port} is not available !")
                     else:
                         logger.critical(f"The supplied network configuration {self.__desktop_host}:{self.__desktop_port} is not available ! ([{e.errno}] {e})")
 
     def __disableDesktop(self):
         """Procedure to disable exegol desktop feature"""
         if self.isDesktopEnabled():
-            logger.verbose("Config: Disabling shell logging")
+            logger.verbose("Config: Disabling exegol desktop")
             assert self.__desktop_proto is not None
             if not self.__network_host:
                 self.__removePort(self.__default_desktop_port[self.__desktop_proto])
             self.__desktop_proto = None
             self.__desktop_host = None
             self.__desktop_port = None
             self.removeLabel(self.ExegolFeatures.desktop.value)
@@ -970,21 +1002,20 @@
                     # Find a match
                     for resource in EnvInfo.getDockerDesktopResources():
                         if path_match.startswith(resource):
                             match = True
                             break
                     if not match:
                         logger.critical(f"Bind volume from {host_path} is not possible, Docker Desktop configuration is incorrect. "
-                                        f"A parent directory must be shared in "
-                                        f"[magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta].")
+                                        f"You need to modify the config to share a parent directory in [magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta].")
             # Choose to update fs directory perms if available and depending on user choice
             # if force_sticky_group is set, user choice is bypassed, fs will be updated.
             execute_update_fs = force_sticky_group or (enable_sticky_group and (UserConfig().auto_update_workspace_fs ^ ParametersManager().update_fs_perms))
             try:
-                if not (path.is_file() or path.is_dir()):
+                if not path.exists():
                     if must_exist:
                         raise CancelOperation(f"{host_path} does not exist on your host.")
                     else:
                         # If the directory is created by exegol, bypass user preference and enable shared perms (if available)
                         execute_update_fs = force_sticky_group or enable_sticky_group
                         path.mkdir(parents=True, exist_ok=True)
             except PermissionError:
@@ -1076,17 +1107,18 @@
         return self.__envs
 
     def getShellEnvs(self) -> List[str]:
         """Overriding envs when opening a shell"""
         result = []
         # Select default shell to use
         result.append(f"{self.ExegolEnv.user_shell.value}={ParametersManager().shell}")
-        # Share X11 (GUI Display) config
+        # Update X11 DISPLAY socket if needed
         if self.__enable_gui:
             current_display = GuiUtils.getDisplayEnv()
+
             # If the default DISPLAY environment in the container is not the same as the DISPLAY of the user's session,
             # the environment variable will be updated in the exegol shell.
             if current_display and self.__envs.get('DISPLAY', '') != current_display:
                 # This case can happen when the container is created from a local desktop
                 # but exegol can be launched from remote access via ssh with X11 forwarding
                 # (Be careful, an .Xauthority file may be needed).
                 result.append(f"DISPLAY={current_display}")
@@ -1279,17 +1311,17 @@
     def getTextFeatures(self, verbose: bool = False) -> str:
         """Text formatter for features configurations (Privileged, X11, Network, Timezone, Shares)
         Print config only if they are different from their default config (or print everything in verbose mode)"""
         result = ""
         if verbose or self.__privileged:
             result += f"{getColor(not self.__privileged)[0]}Privileged: {'On :fire:' if self.__privileged else '[green]Off :heavy_check_mark:[/green]'}{getColor(not self.__privileged)[1]}{os.linesep}"
         if verbose or self.isDesktopEnabled():
-            result += f"{getColor(self.isDesktopEnabled())[0]}Desktop: {self.getDesktopConfig()}{getColor(self.isDesktopEnabled())[1]}{os.linesep}"
+            result += f"{getColor(self.isDesktopEnabled())[0]}Remote Desktop: {self.getDesktopConfig()}{getColor(self.isDesktopEnabled())[1]}{os.linesep}"
         if verbose or not self.__enable_gui:
-            result += f"{getColor(self.__enable_gui)[0]}X11: {boolFormatter(self.__enable_gui)}{getColor(self.__enable_gui)[1]}{os.linesep}"
+            result += f"{getColor(self.__enable_gui)[0]}Console GUI: {boolFormatter(self.__enable_gui)}{getColor(self.__enable_gui)[1]}{os.linesep}"
         if verbose or not self.__network_host:
             result += f"[green]Network mode: [/green]{self.getTextNetworkMode()}{os.linesep}"
         if self.__vpn_path is not None:
             result += f"[green]VPN: [/green]{self.getVpnName()}{os.linesep}"
         if verbose or not self.__share_timezone:
             result += f"{getColor(self.__share_timezone)[0]}Share timezone: {boolFormatter(self.__share_timezone)}{getColor(self.__share_timezone)[1]}{os.linesep}"
         if verbose or not self.__exegol_resources:
@@ -1313,14 +1345,20 @@
         """Get Desktop feature status / config"""
         if not self.isDesktopEnabled():
             return boolFormatter(False)
         config = (f"{self.__desktop_proto}://"
                   f"{'localhost' if self.__desktop_host == '127.0.0.1' else self.__desktop_host}:{self.__desktop_port}")
         return f"[link={config}][deep_sky_blue3]{config}[/deep_sky_blue3][/link]"
 
+    def getTextGuiSockets(self):
+        if self.__enable_gui:
+            return f"[bright_black]({' + '.join(self.__gui_engine)})[/bright_black]"
+        else:
+            return ""
+
     def getTextNetworkMode(self) -> str:
         """Network mode, text getter"""
         network_mode = "host" if self.__network_host else "bridge"
         if self.__vpn_path:
             network_mode += " with VPN"
         return network_mode
 
@@ -1332,15 +1370,15 @@
         return datetime.strptime(self.__creation_date, "%Y-%m-%dT%H:%M:%SZ").strftime("%d/%m/%Y %H:%M")
 
     def getTextMounts(self, verbose: bool = False) -> str:
         """Text formatter for Mounts configurations. The verbose mode does not exclude technical volumes."""
         result = ''
         hidden_mounts = ['/tmp/.X11-unix', '/opt/resources', '/etc/localtime',
                          '/etc/timezone', '/my-resources', '/opt/my-resources',
-                         '/.exegol/entrypoint.sh', '/.exegol/spawn.sh']
+                         '/.exegol/entrypoint.sh', '/.exegol/spawn.sh', '/tmp/wayland-0', '/tmp/wayland-1']
         for mount in self.__mounts:
             # Not showing technical mounts
             if not verbose and mount.get('Target') in hidden_mounts:
                 continue
             read_only_text = f"[bright_black](RO)[/bright_black] " if verbose else ''
             read_write_text = f"[orange3](RW)[/orange3] " if verbose else ''
             result += f"{read_only_text if mount.get('ReadOnly') else read_write_text}{mount.get('Source')} :right_arrow: {mount.get('Target')}{os.linesep}"
@@ -1361,15 +1399,15 @@
         return result
 
     def getTextEnvs(self, verbose: bool = False) -> str:
         """Text formatter for Envs configuration. The verbose mode does not exclude technical variables."""
         result = ''
         for k, v in self.__envs.items():
             # Blacklist technical variables, only shown in verbose
-            if not verbose and k in list(self.__static_gui_envs.keys()) + [v.value for v in self.ExegolEnv] + ["DISPLAY", "PATH"]:
+            if not verbose and k in list(self.__static_gui_envs.keys()) + [v.value for v in self.ExegolEnv] + ["DISPLAY", "WAYLAND_DISPLAY", "XDG_SESSION_TYPE", "XDG_RUNTIME_DIR", "PATH"]:
                 continue
             result += f"{k}={v}{os.linesep}"
         return result
 
     def getTextPorts(self) -> str:
         """Text formatter for Ports configuration.
         Dict Port key = container port/protocol
```

### Comparing `Exegol-4.3.1/exegol/model/ExegolContainer.py` & `exegol-4.3.2/exegol/model/ExegolContainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,19 @@
     def __start_container(self):
         """
         This method start the container and display startup status update to the user.
         :return:
         """
         with console.status(f"Waiting to start {self.name}", spinner_style="blue") as progress:
             start_date = datetime.utcnow()
-            self.__container.start()
+            try:
+                self.__container.start()
+            except APIError as e:
+                logger.debug(e)
+                logger.critical(f"Docker raise a critical error when starting the container [green]{self.name}[/green], error message is: {e.explanation}")
             if not self.config.legacy_entrypoint:  # TODO improve startup compatibility check
                 try:
                     # Try to find log / startup messages. Will time out after 2 seconds if the image don't support status update through container logs.
                     for line in ContainerLogStream(self.__container, start_date=start_date, timeout=2):
                         # Once the last log "READY" is received, the startup sequence is over and the execution can continue
                         if line == "READY":
                             break
@@ -319,16 +323,20 @@
         If X11 (GUI) is enabled, allow X11 access on host ACL (if not already allowed) for linux and mac.
         On Windows host, WSLg X11 don't have xhost ACL.
         :return:
         """
         if self.config.isGUIEnable() and not self.__xhost_applied and not EnvInfo.isWindowsHost():
             self.__xhost_applied = True  # Can be applied only once per execution
             if shutil.which("xhost") is None:
-                logger.error("The [green]xhost[/green] command is not available on your [bold]host[/bold]. "
-                             "Exegol was unable to allow your container to access your graphical environment (or you don't have one).")
+                if EnvInfo.is_linux_shell:
+                    debug_msg = "Try to install the package [green]xorg-xhost[/green] or maybe you don't have X11 on your host?"
+                else:
+                    debug_msg = "or you don't have one"
+                logger.error(f"The [green]xhost[/green] command is not available on your [bold]host[/bold]. "
+                             f"Exegol was unable to allow your container to access your graphical environment ({debug_msg}).")
                 return
 
             if EnvInfo.isMacHost():
                 logger.debug(f"Adding xhost ACL to localhost")
                 # add xquartz inet ACL
                 with console.status(f"Starting XQuartz...", spinner_style="blue"):
                     os.system(f"xhost + localhost > /dev/null")
```

### Comparing `Exegol-4.3.1/exegol/model/ExegolContainerTemplate.py` & `exegol-4.3.2/exegol/model/ExegolContainerTemplate.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/model/ExegolImage.py` & `exegol-4.3.2/exegol/model/ExegolImage.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/model/ExegolModules.py` & `exegol-4.3.2/exegol/model/ExegolModules.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/model/MetaImages.py` & `exegol-4.3.2/exegol/model/MetaImages.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/ContainerLogStream.py` & `exegol-4.3.2/exegol/utils/ContainerLogStream.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/DataFileUtils.py` & `exegol-4.3.2/exegol/utils/DataFileUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/DockerUtils.py` & `exegol-4.3.2/exegol/utils/DockerUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from datetime import datetime
+from time import sleep
 from typing import List, Optional, Union, cast
 
 import docker
 from docker import DockerClient
 from docker.errors import APIError, DockerException, NotFound, ImageNotFound
 from docker.models.images import Image
 from docker.models.volumes import Volume
@@ -134,15 +135,15 @@
             docker_args["auto_remove"] = temporary
         try:
             container = docker_create_function(**docker_args)
         except APIError as err:
             message = err.explanation.decode('utf-8').replace('[', '\\[') if type(err.explanation) is bytes else err.explanation
             if message is not None:
                 message = message.replace('[', '\\[')
-                logger.error(message)
+                logger.error(f"Docker error received: {message}")
             logger.debug(err)
             model.rollback()
             try:
                 container = cls.__client.containers.list(all=True, filters={"name": model.container_name})
                 if container is not None and len(container) > 0:
                     for c in container:
                         if c.name == model.container_name:  # Search for exact match
@@ -525,41 +526,70 @@
 
     @classmethod
     def removeImage(cls, image: ExegolImage, upgrade_mode: bool = False) -> bool:
         """Remove an ExegolImage from disk"""
         tag = image.removeCheck()
         if tag is None:  # Skip removal if image is not installed locally.
             return False
-        try:
-            with console.status(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...", spinner_style="blue"):
+        with console.status(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...", spinner_style="blue"):
+            try:
                 if not image.isVersionSpecific() and image.getInstalledVersionName() != image.getName() and not upgrade_mode:
                     # Docker can't remove multiple images at the same tag, version specific tag must be remove first
                     logger.debug(f"Removing image {image.getFullVersionName()}")
-                    cls.__client.images.remove(image.getFullVersionName(), force=False, noprune=False)
+                    if not cls.__remove_image(image.getFullVersionName()):
+                        logger.critical(f"An error occurred while removing this image : {image.getFullVersionName()}")
                 logger.debug(f"Removing image {image.getLocalId()} ({image.getFullVersionName() if upgrade_mode else image.getFullName()})")
-                cls.__client.images.remove(image.getLocalId(), force=False, noprune=False)
-            logger.verbose(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...")
-            logger.success(f"{'Previous d' if upgrade_mode else 'D'}ocker image successfully removed.")
-            return True
-        except APIError as err:
-            # Handle docker API error code
-            logger.verbose(err.explanation)
-            if err.status_code == 409:
-                if upgrade_mode:
-                    logger.error(f"The '{image.getName()}' image cannot be deleted yet, "
-                                 "all containers using this old image must be deleted first.")
+                if cls.__remove_image(image.getLocalId()):
+                    logger.verbose(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...")
+                    logger.success(f"{'Previous d' if upgrade_mode else 'D'}ocker image successfully removed.")
+                    return True
+            except APIError as err:
+                # Handle docker API error code
+                logger.verbose(err.explanation)
+                if err.status_code == 409:
+                    if upgrade_mode:
+                        logger.error(f"The '{image.getName()}' image cannot be deleted yet, "
+                                     "all containers using this old image must be deleted first.")
+                    else:
+                        logger.error(f"The '{image.getName()}' image cannot be deleted because "
+                                     f"it is currently used by a container. Aborting.")
+                elif err.status_code == 404:
+                    logger.error(f"This image doesn't exist locally {image.getLocalId()} ({image.getFullName()}). Aborting.")
                 else:
-                    logger.error(f"The '{image.getName()}' image cannot be deleted because "
-                                 f"it is currently used by a container. Aborting.")
-            elif err.status_code == 404:
-                logger.error(f"This image doesn't exist locally {image.getLocalId()} ({image.getFullName()}). Aborting.")
-            else:
-                logger.critical(f"An error occurred while removing this image : {err}")
+                    logger.critical(f"An error occurred while removing this image : {err}")
+        return False
+
+    @classmethod
+    def __remove_image(cls, image_name: str) -> bool:
+        """
+        Handle docker image removal with timeout support
+        :param image_name: Name of the docker image to remove
+        :return: True is removal successful and False otherwise
+        """
+        try:
+            cls.__client.images.remove(image_name, force=False, noprune=False)
+            return True
         except ReadTimeout:
-            logger.error(f"The deletion of the image has timeout, the deletion may be incomplete.")
+            logger.warning("The deletion of the image has timeout. Docker is still processing the removal, please wait.")
+            max_retry = 5
+            wait_time = 5
+            for i in range(5):
+                try:
+                    _ = cls.__client.images.get(image_name)
+                    # DockerSDK image getter is an exact matching, no need to add more check
+                except APIError as err:
+                    if err.status_code == 404:
+                        return True
+                    else:
+                        logger.debug(f"Unexpected error after timeout: {err}")
+                except ReadTimeout:
+                    wait_time = wait_time + wait_time*i
+                    logger.info(f"Docker timeout again ({i+1}/{max_retry}). Next retry in {wait_time} seconds...")
+                    sleep(wait_time)  # Wait x seconds before retry
+            logger.error(f"The deletion of the image '{image_name}' has timeout, the deletion may be incomplete.")
         return False
 
     @classmethod
     def buildImage(cls, tag: str, build_profile: Optional[str] = None, build_dockerfile: Optional[str] = None, dockerfile_path: str = ConstantConfig.build_context_path):
         """Build a docker image from source"""
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to build a docker image in offline mode. The build process need access to internet ...")
```

### Comparing `Exegol-4.3.1/exegol/utils/ExeLog.py` & `exegol-4.3.2/exegol/utils/ExeLog.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/FsUtils.py` & `exegol-4.3.2/exegol/utils/FsUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/GitUtils.py` & `exegol-4.3.2/exegol/utils/GitUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/GuiUtils.py` & `exegol-4.3.2/exegol/utils/GuiUtils.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,28 +17,41 @@
     """This utility class allows determining if the current system supports the GUI
     from the information of the system (through X11 sharing)."""
 
     __distro_name = ""
     default_x11_path = "/tmp/.X11-unix"
 
     @classmethod
-    def isGuiAvailable(cls) -> bool:
+    def isX11GuiAvailable(cls) -> bool:
         """
         Check if the host OS can support GUI application with X11 sharing
         :return: bool
         """
         # GUI (X11 sharing) was not supported on Windows before WSLg
         if EnvInfo.isWindowsHost():
             return cls.__windowsGuiChecks()
         elif EnvInfo.isMacHost():
             return cls.__macGuiChecks()
         # Linux default is True
         return True
 
     @classmethod
+    def isWaylandGuiAvailable(cls) -> bool:
+        """
+        Check if the host OS can support GUI application with WAYLAND sharing
+        :return: bool
+        """
+        if EnvInfo.isWindowsHost():
+            return False  # TODO To Be defined (WSLg works fine for now)
+        # elif EnvInfo.isMacHost():
+        #    return False
+        # Linux or Mac, rely on var env settings
+        return EnvInfo.isWaylandAvailable()
+
+    @classmethod
     def getX11SocketPath(cls) -> Optional[str]:
         """
         Get the host path of the X11 socket
         :return:
         """
         if cls.__distro_name:
             # Distro name can only be set if the current host OS is Windows
@@ -55,17 +68,29 @@
         elif EnvInfo.isMacHost():
             # Docker desktop don't support UNIX socket through volume, we are using XQuartz over the network until then
             return None
         # Other distributions (Linux / Mac) have the default socket path
         return cls.default_x11_path
 
     @classmethod
+    def getWaylandSocketPath(cls) -> Optional[Path]:
+        """
+        Get the host path of the Wayland socket
+        :return:
+        """
+        wayland_dir = os.getenv("XDG_RUNTIME_DIR")
+        wayland_socket = os.getenv("WAYLAND_DISPLAY")
+        if wayland_dir is None or wayland_socket is None:
+            return None
+        return Path(wayland_dir, wayland_socket)
+
+    @classmethod
     def getDisplayEnv(cls) -> str:
         """
-        Get the current DISPLAY env to access X11 socket
+        Get the current DISPLAY environment to access X11 socket
         :return:
         """
         if EnvInfo.isMacHost():
             # xquartz Mac mode
             return "host.docker.internal:0"
 
         # Add ENV check is case of user don't have it, which will mess up GUI (X11 sharing) if fallback does not work
@@ -73,14 +98,22 @@
         if not EnvInfo.is_windows_shell:
             if os.getenv("DISPLAY") is None:
                 logger.warning("The DISPLAY environment variable is not set on your host. This can prevent GUI apps to start through X11 sharing")
 
         # DISPLAY var is fetch from the current user environment. If it doesn't exist, using ':0'.
         return os.getenv('DISPLAY', ":0")
 
+    @classmethod
+    def getWaylandEnv(cls) -> str:
+        """
+        Get the current WAYLAND_DISPLAY environment to access wayland socket
+        :return:
+        """
+        return os.getenv('WAYLAND_DISPLAY', 'wayland-0')
+
     # # # # # # Mac specific methods # # # # # #
 
     @classmethod
     def __macGuiChecks(cls) -> bool:
         """
         Procedure to check if the Mac host supports GUI (X11 sharing) with docker through XQuartz
         :return: bool
```

### Comparing `Exegol-4.3.1/exegol/utils/MetaSingleton.py` & `exegol-4.3.2/exegol/utils/MetaSingleton.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/WebUtils.py` & `exegol-4.3.2/exegol/utils/WebUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 import time
+import os
 from typing import Any, Optional, Dict
 
 import requests
 from requests import Response
 
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import CancelOperation
@@ -120,15 +121,22 @@
         Url: web page to quest
         Service_name: service display name for logging purpose
         Retry_count: number of retry allowed."""
         # In case of API timeout, allow retrying 1 more time
         for i in range(retry_count):
             try:
                 try:
-                    response = requests.request(method=method, url=url, timeout=(5, 10), verify=ParametersManager().verify, headers=headers, data=data)
+                    proxies = {}
+                    http_proxy = os.environ.get('HTTP_PROXY') or os.environ.get('http_proxy')
+                    if http_proxy:
+                        proxies['http'] = http_proxy
+                    https_proxy = os.environ.get('HTTPS_PROXY') or os.environ.get('https_proxy')
+                    if https_proxy:
+                        proxies['https'] = https_proxy
+                    response = requests.request(method=method, url=url, timeout=(10, 20), verify=ParametersManager().verify, headers=headers, data=data, proxies=proxies if len(proxies) > 0 else None)
                     return response
                 except requests.exceptions.HTTPError as e:
                     if e.response is not None:
                         logger.error(f"Response error: {e.response.content.decode('utf-8')}")
                     else:
                         logger.error(f"Response error: {e}")
                 except requests.exceptions.ConnectionError as err:
```

### Comparing `Exegol-4.3.1/exegol/utils/argParse.py` & `exegol-4.3.2/exegol/utils/argParse.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/imgsync/ImageScriptSync.py` & `exegol-4.3.2/exegol/utils/imgsync/ImageScriptSync.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/imgsync/entrypoint.sh` & `exegol-4.3.2/exegol/utils/imgsync/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol/utils/imgsync/spawn.sh` & `exegol-4.3.2/exegol/utils/imgsync/spawn.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/Dockerfile` & `exegol-4.3.2/exegol-docker-build/Dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/ad.dockerfile` & `exegol-4.3.2/exegol-docker-build/ad.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/light.dockerfile` & `exegol-4.3.2/exegol-docker-build/light.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/osint.dockerfile` & `exegol-4.3.2/exegol-docker-build/osint.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound/config.json` & `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/config.json`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound/customqueries.json` & `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/customqueries.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9543822816084138%*

 * *Differences: {"'queries'": "{8: {'queryList': {0: {'query': 'MATCH (o {owned: TRUE}) RETURN o'}}}, 9: "*

 * *              "{'queryList': {0: {'query': 'MATCH p=(u:User {owned: TRUE})-[:MemberOf]->(g:Group) "*

 * *              "RETURN p'}}}, 10: {'queryList': {0: {'query': 'MATCH p=(u:User {owned: "*

 * *              "TRUE})-[:MemberOf*1..]->(g:Group) RETURN p'}}}, 11: {'queryList': {0: {'query': "*

 * *              "'MATCH p=shortestPath((n {owned: "*

 * *              'TRUE})-[:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceC […]*

```diff
@@ -82,89 +82,89 @@
         },
         {
             "category": "Owned Objects",
             "name": "Owned objects",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (m) WHERE m.owned=TRUE RETURN m"
+                    "query": "MATCH (o {owned: TRUE}) RETURN o"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Direct groups of owned users",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
                     "props": {},
-                    "query": "MATCH (u:User {owned:true}), (g:Group), p=(u)-[:MemberOf]->(g) RETURN p"
+                    "query": "MATCH p=(u:User {owned: TRUE})-[:MemberOf]->(g:Group) RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Unrolled groups of owned users",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (m:User) WHERE m.owned=TRUE WITH m MATCH p=(m)-[:MemberOf*1..]->(n:Group) RETURN p"
+                    "query": "MATCH p=(u:User {owned: TRUE})-[:MemberOf*1..]->(g:Group) RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Shortest paths from owned objects to High Value Targets (5 hops)",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=shortestPath((n {owned:true})-[:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|CanRDP|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory|CanPSRemote*1..5]->(m {highvalue:true})) WHERE NOT n=m RETURN p"
+                    "query": "MATCH p=shortestPath((n {owned: TRUE})-[:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|CanRDP|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory|CanPSRemote*1..5]->(m {highvalue: TRUE})) WHERE NOT n=m RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Most exploitable paths from owned objects to High Value Targets (5 hops)",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((n {owned:true})-[:MemberOf|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory*1..5]->(m {highvalue:true})) WHERE NOT n=m RETURN p"
+                    "query": "MATCH p=allShortestPaths((n {owned: TRUE})-[:MemberOf|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory*1..5]->(m {highvalue:true})) WHERE NOT n=m RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Next steps (5 hops) from owned objects",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=shortestPath((c {owned: true})-[*1..5]->(s)) WHERE NOT c = s RETURN p"
+                    "query": "MATCH p=shortestPath((c {owned: TRUE})-[*1..5]->(s)) WHERE NOT c = s RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Next steps (3 hops) from owned objects",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=shortestPath((c {owned: true})-[*1..3]->(s)) WHERE NOT c = s RETURN p"
+                    "query": "MATCH p=shortestPath((c {owned: TRUE})-[*1..3]->(s)) WHERE NOT c = s RETURN p"
                 }
             ]
         },
         {
             "category": "Owned Objects",
             "name": "Owned users with permissions against GPOs",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(u:User {owned:true})-[r:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink*1..]->(g:GPO) RETURN p"
+                    "query": "MATCH p=(u:User {owned: TRUE})-[r:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink*1..]->(g:GPO) RETURN p"
                 }
             ]
         },
         {
             "category": "Domains/Forests",
             "name": "Connections between different domains/forests",
             "queryList": [
@@ -176,15 +176,15 @@
         },
         {
             "category": "Domains/Forests",
             "name": "Connections (ACEs only) between different domains/forests",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p = (a)-[r]->(b) WHERE NOT a.domain = b.domain AND r.isacl = True RETURN p"
+                    "query": "MATCH p = (a)-[r]->(b) WHERE NOT a.domain = b.domain AND r.isacl = TRUE RETURN p"
                 }
             ]
         },
         {
             "category": "Domains/Forests",
             "name": "Can a user from domain A do anything to any computer in domain B (Warning: VERY Heavy)",
             "queryList": [
@@ -197,127 +197,127 @@
                     "final": false,
                     "query": "MATCH (n:Domain) RETURN $result + '=>' + n.name ORDER BY n.name DESC",
                     "title": "Select destination domain..."
                 },
                 {
                     "allowCollapse": false,
                     "final": true,
-                    "query": "WITH split($result, \"=>\") as selectedDomains WITH selectedDomains[0] as sourceDomain, selectedDomains[1] as destDomain MATCH (n:User {domain: sourceDomain}) MATCH (m:Computer {domain: destDomain}) MATCH p=allShortestPaths((n)-[r:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|CanRDP|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin*1..]->(m)) WHERE NOT n = m RETURN p",
+                    "query": "WITH split($result, \"=>\") AS selectedDomains WITH selectedDomains[0] AS sourceDomain, selectedDomains[1] AS destDomain MATCH (n:User {domain: sourceDomain}) MATCH (m:Computer {domain: destDomain}) MATCH p=allShortestPaths((n)-[r:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|CanRDP|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin*1..]->(m)) WHERE NOT n = m RETURN p",
                     "startNode": "{}"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "Kerberoastable users with a path to DA",
+            "name": "Kerberoastable enabled users",
             "queryList": [
                 {
+                    "allowCollapse": false,
                     "final": true,
-                    "query": "MATCH (u:User {hasspn:true}) MATCH (g:Group) WHERE g.objectid ENDS WITH '-512' MATCH p = shortestPath( (u)-[*1..]->(g) ) RETURN p"
+                    "query": "MATCH (u:User {enabled: TRUE, hasspn: TRUE}) RETURN u"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "Kerberoastable users with a path to High Value",
+            "name": "AS-REProastable enabled users",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User {hasspn:true}),(n {highvalue:true}),p = shortestPath( (u)-[*1..]->(n) ) RETURN p"
+                    "query": "MATCH (u:User {enabled: TRUE, dontreqpreauth: TRUE}) RETURN u"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": " Kerberoastable users and where they are AdminTo",
+            "name": "Kerberoastable users with a path to DA",
             "queryList": [
                 {
                     "final": true,
-                    "query": "OPTIONAL MATCH (u:User) WHERE u.hasspn=true OPTIONAL MATCH (u)-[r:AdminTo]->(c:Computer) RETURN u"
+                    "query": "MATCH p = shortestPath( (u:User {enabled: TRUE, hasspn: TRUE})-[*1..]->(g:Group) ) WHERE g.objectid ENDS WITH '-512' RETURN p"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "Kerberoastable users who are members of high value groups",
+            "name": "Kerberoastable enabled users with a path to High Value",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User)-[r:MemberOf*1..]->(g:Group) WHERE g.highvalue=true AND u.hasspn=true RETURN u"
+                    "query": "MATCH p = shortestPath( (u:User {enabled: TRUE, hasspn: TRUE})-[*1..]->(n {highvalue: TRUE}) ) RETURN p"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "Kerberoastable users with passwords last set > 5 years ago",
+            "name": "Kerberoastable enabled users and where they are AdminTo",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User) WHERE n.hasspn=true AND WHERE u.pwdlastset < (datetime().epochseconds - (1825 * 86400)) and NOT u.pwdlastset IN [-1.0, 0.0] RETURN u"
+                    "query": "MATCH p = shortestPath((u:User {enabled: TRUE, hasspn:TRUE})-[:AdminTo]->(c:Computer {enabled: TRUE})) RETURN p"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "Kerberoastable Users",
+            "name": "Kerberoastable enabled users who are members of high value groups",
             "queryList": [
                 {
-                    "allowCollapse": false,
                     "final": true,
-                    "query": "MATCH (n:User)WHERE n.hasspn=true RETURN n"
+                    "query": "MATCH p = shortestPath((u:User {enabled: TRUE, hasspn: TRUE})-[:MemberOf*1..]->(g:Group {highvalue: TRUE})) RETURN p"
                 }
             ]
         },
         {
             "category": "Roasting",
-            "name": "AS-REProastable Users",
+            "name": "Kerberoastable enabled users with passwords last set > 5 years ago",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User {dontreqpreauth: true}) RETURN u"
+                    "query": "MATCH (u:User {enabled: TRUE, hasspn: TRUE}) WHERE u.pwdlastset < (datetime().epochseconds - (1825 * 86400)) AND NOT u.pwdlastset IN [-1.0, 0.0] RETURN u"
                 }
             ]
         },
         {
             "category": "Kerberos Delegations",
-            "name": "Unconstrained Delegations",
+            "name": "Unconstrained Delegations for enabled computers",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (c {unconstraineddelegation:true}) RETURN c"
+                    "query": "MATCH (c {enabled: TRUE, unconstraineddelegation: TRUE}) RETURN c"
                 }
             ]
         },
         {
             "category": "Kerberos Delegations",
             "name": "Constrained Delegations (with Protocol Transition)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (c) WHERE NOT c.allowedtodelegate IS NULL AND c.trustedtoauth=true RETURN c"
+                    "query": "MATCH (c) WHERE NOT c.allowedtodelegate IS NULL AND c.trustedtoauth=TRUE RETURN c"
                 }
             ]
         },
         {
             "category": "Kerberos Delegations",
             "name": "Constrained Delegations (without Protocol Transition)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (c) WHERE NOT c.allowedtodelegate IS NULL AND c.trustedtoauth=false RETURN c"
+                    "query": "MATCH (c) WHERE NOT c.allowedtodelegate IS NULL AND c.trustedtoauth=FALSE RETURN c"
                 }
             ]
         },
         {
             "category": "Kerberos Delegations",
             "name": "Resource-Based Constrained Delegations",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(u)-[:AllowedToAct]->(c) RETURN p"
+                    "query": "MATCH p=(u:User {enabled: TRUE})-[:AllowedToAct]->(c:Computer {enabled: TRUE}) RETURN p"
                 }
             ]
         },
         {
             "category": "Kerberos Delegations",
             "name": "Unconstrained Delegation systems (without domain controllers)",
             "queryList": [
@@ -339,15 +339,15 @@
         },
         {
             "category": "Kerberos Delegations",
             "name": "Shortest paths from owned principals to unconstrained delegation systems",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n {owned:true}) MATCH p=shortestPath((n)-[:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory|CanPSRemote*1..]->(m:Computer {unconstraineddelegation: true})) WHERE NOT n=m RETURN p"
+                    "query": "MATCH p=shortestPath((o {owned: TRUE})-[:MemberOf|HasSession|AdminTo|AllExtendedRights|AddMember|ForceChangePassword|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ExecuteDCOM|AllowedToDelegate|ReadLAPSPassword|Contains|GpLink|AddAllowedToAct|AllowedToAct|SQLAdmin|ReadGMSAPassword|HasSIDHistory|CanPSRemote*1..]->(m:Computer {unconstraineddelegation: TRUE})) WHERE NOT o=m RETURN p"
                 }
             ]
         },
         {
             "category": "Weak ACLs",
             "name": "Between users (1 hop, max 200)",
             "queryList": [
@@ -470,75 +470,85 @@
         {
             "category": "Admins",
             "name": "Logged in Admins",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=(a:Computer {enabled: TRUE})-[r:HasSession]->(b:User {enabled: TRUE}) WITH a,b,r MATCH p=shortestPath((b)-[:AdminTo|MemberOf*1..]->(a)) RETURN p"
+                    "query": "MATCH p=(c:Computer {enabled: TRUE})-[:HasSession]->(u:User {enabled: TRUE}) WITH c,u MATCH p=shortestPath((u)-[:AdminTo|MemberOf*1..]->(c)) RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
             "name": "Users with local admin rights",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(m:User {enabled: TRUE})-[r:AdminTo]->(n:Computer {enabled: TRUE}) RETURN p"
+                    "query": "MATCH p=(m:User {enabled: TRUE})-[:AdminTo]->(n:Computer {enabled: TRUE}) RETURN p"
+                }
+            ]
+        },
+        {
+            "category": "Admins",
+            "name": "Administrators and Domain/Entreprise Admins with sessions",
+            "queryList": [
+                {
+                    "final": true,
+                    "query": "MATCH (u:User {enabled: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-(512|519|(?i)S-1-5-32-544)$' WITH COLLECT(u.objectid) AS domainAdmins MATCH p = (c2:Computer {enabled: TRUE})-[:HasSession]->(u2:User {enabled: TRUE}) WHERE u2.objectid IN domainAdmins RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
-            "name": "Domain admins sessions",
+            "name": "Administrators and Domain/Entreprise Admins with sessions not on domain controllers",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:User {enabled: TRUE})-[:MemberOf]->(g:Group) WHERE g.objectid ENDS WITH '-512' MATCH p = (c:Computer {enabled: TRUE})-[:HasSession]->(n) RETURN p"
+                    "query": "MATCH (u:User {enabled: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-(512|519|(?i)S-1-5-32-544)$' WITH COLLECT(u.objectid) AS domainAdmins MATCH (c:Computer {enabled: TRUE})-[:MemberOf*1..]->(g2:Group) WHERE g2.objectid =~ '.*-(516|(?i)S-1-5-9)$' WITH COLLECT(c.objectid) AS domainControllers, domainAdmins MATCH p = (c2:Computer {enabled: TRUE})-[:HasSession]->(u2:User {enabled: TRUE}) WHERE u2.objectid IN domainAdmins AND NOT c2.objectid IN domainControllers RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
-            "name": "Privileged users sessions",
+            "name": "High Value users sessions",
             "queryList": [
                 {
                     "final": true,
                     "query": "MATCH (n:User {enabled: TRUE})-[:MemberOf*1..]->(g:Group {highvalue: TRUE}) MATCH p = (c:Computer {enabled: TRUE})-[:HasSession]->(n) RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
             "name": "Users with adminCount, not sensitive for delegation, not members of Protected Users",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u)-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ \"(?i)S-1-5-.*-525\" WITH COLLECT (u.name) as protectedUsers MATCH p=(u2:User)-[:MemberOf*1..3]->(g2:Group) WHERE u2.admincount=true AND u2.sensitive=false AND NOT u2.name IN protectedUsers RETURN p"
+                    "query": "MATCH (u:User {enabled:TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '(?i)S-1-5-.*-525$' WITH COLLECT (u.objectid) AS protectedUsers MATCH p=(u2:User {enabled:TRUE, admincount:TRUE, sensitive:FALSE})-[:MemberOf*1..3]->(g2:Group) WHERE NOT u2.objectid IN protectedUsers RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
             "name": "Enabled Domain/Enterprise Administrators, not sensitive for delegation and not members of Protected Users",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User {enabled: TRUE, admincount: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-525$' WITH COLLECT(u.objectid) as protectedUsers MATCH p=(u2:User {enabled: TRUE, admincount: TRUE, sensitive: FALSE})-[:MemberOf*1..]->(g2:Group) WHERE NOT u2.objectid IN protectedUsers AND g2.objectid =~ '.*-(512|519|(?i)S-1-5-32-544)$' RETURN p"
+                    "query": "MATCH (u:User {enabled: TRUE, admincount: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-525$' WITH COLLECT(u.objectid) AS protectedUsers MATCH p=(u2:User {enabled: TRUE, admincount: TRUE, sensitive: FALSE})-[:MemberOf*1..]->(g2:Group) WHERE NOT u2.objectid IN protectedUsers AND g2.objectid =~ '.*-(512|519|(?i)S-1-5-32-544)$' RETURN p"
                 }
             ]
         },
         {
             "category": "Admins",
             "name": "Enabled users, members of high value groups, not sensitive for delegation and not members of Protected Users (Heavy)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User {enabled: TRUE, admincount: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-525$' WITH COLLECT (u.objectid) as protectedUsers MATCH p=(u2:User {enabled: TRUE, sensitive: FALSE})-[:MemberOf*1..]->(g2:Group {highvalue: TRUE}) WHERE NOT u2.objectid IN protectedUsers RETURN p"
+                    "query": "MATCH (u:User {enabled: TRUE, admincount: TRUE})-[:MemberOf*1..]->(g:Group) WHERE g.objectid =~ '.*-525$' WITH COLLECT (u.objectid) AS protectedUsers MATCH p=(u2:User {enabled: TRUE, sensitive: FALSE})-[:MemberOf*1..]->(g2:Group {highvalue: TRUE}) WHERE NOT u2.objectid IN protectedUsers RETURN p"
                 }
             ]
         },
         {
             "category": "Groups",
             "name": "Groups that contain the word 'admin'",
             "queryList": [
@@ -550,108 +560,108 @@
         },
         {
             "category": "Groups",
             "name": "Groups that can change user passwords",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(m:Group)-[r:ForceChangePassword]->(n:User) RETURN DISTINCT m[.]name,  COUNT(m[.]name) ORDER BY COUNT(m[.]name) DESC"
+                    "query": "MATCH p=(m:Group)-[:ForceChangePassword]->(n:User) RETURN DISTINCT m[.]name,  COUNT(m[.]name) ORDER BY COUNT(m[.]name) DESC"
                 }
             ]
         },
         {
             "category": "Groups",
             "name": "Groups of High Value Targets",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(n:User)-[r:MemberOf*1..]->(m:Group {highvalue:true}) RETURN p"
+                    "query": "MATCH p=(n:User)-[:MemberOf*1..]->(m:Group {highvalue:true}) RETURN p"
                 }
             ]
         },
         {
             "category": "Groups",
             "name": "Non Admin Groups with High Value Privileges",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=(g:Group)-[r:Owns|:WriteDacl|:GenericAll|:WriteOwner|:ExecuteDCOM|:GenericWrite|:AllowedToDelegate|:ForceChangePassword]->(n:Computer) WHERE NOT g.name CONTAINS 'ADMIN' RETURN p"
+                    "query": "MATCH p=(g:Group)-[:Owns|:WriteDacl|:GenericAll|:WriteOwner|:ExecuteDCOM|:GenericWrite|:AllowedToDelegate|:ForceChangePassword]->(n:Computer) WHERE NOT g.name CONTAINS 'ADMIN' RETURN p"
                 }
             ]
         },
         {
             "category": "Groups",
             "name": "Groups with Computer and User Objects",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "endNode": "{}",
                     "final": true,
-                    "query": "MATCH (c:Computer)-[r:MemberOf*1..]->(groupsWithComps:Group) WITH groupsWithComps MATCH (u:User)-[r:MemberOf*1..]->(groupsWithComps) RETURN DISTINCT(groupsWithComps) as groupsWithCompsAndUsers"
+                    "query": "MATCH (c:Computer)-[:MemberOf*1..]->(groupsWithComps:Group) WITH groupsWithComps MATCH (u:User)-[r:MemberOf*1..]->(groupsWithComps) RETURN DISTINCT(groupsWithComps) AS groupsWithCompsAndUsers"
                 }
             ]
         },
         {
             "category": "Groups",
-            "name": "Groups that can reset passwords (Warning: Heavy)",
+            "name": "Groups that can reset passwords of enabled users (Warning: Heavy)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(m:Group)-[r:ForceChangePassword]->(n:User) RETURN p"
+                    "query": "MATCH p=(g:Group)-[:ForceChangePassword]->(u:User {enabled: TRUE}) RETURN p"
                 }
             ]
         },
         {
             "category": "Groups",
-            "name": "Groups that have local admin rights (Warning: Heavy)",
+            "name": "Groups that have local admin rights on enabled computers (Warning: Heavy)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(m:Group)-[r:AdminTo]->(n:Computer) RETURN p"
+                    "query": "MATCH p=(g:Group)-[:AdminTo]->(c:Computer {enabled: TRUE}) RETURN p"
                 }
             ]
         },
         {
             "category": "Users",
             "name": "Users never logged on and account still active",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:User) WHERE n.lastlogontimestamp=-1.0 AND n.enabled=TRUE RETURN n "
+                    "query": "MATCH (u:User {enabled: TRUE, lastlogontimestamp:-1.0}) RETURN u"
                 }
             ]
         },
         {
             "category": "Users",
-            "name": "Users logged in the last 90 days",
+            "name": "Users logged in the last 90 days and account still active",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User) WHERE u.lastlogon < (datetime().epochseconds - (90 * 86400)) and NOT u.lastlogon IN [-1.0, 0.0] RETURN u"
+                    "query": "MATCH (u:User {enabled: TRUE}) WHERE u.lastlogon < (datetime().epochseconds - (90 * 86400)) and NOT u.lastlogon IN [-1.0, 0.0] RETURN u"
                 }
             ]
         },
         {
             "category": "Users",
-            "name": "Users with passwords last set in the last 90 days",
+            "name": "Users with passwords last set in the last 90 days and account still active",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (u:User) WHERE u.pwdlastset < (datetime().epochseconds - (90 * 86400)) and NOT u.pwdlastset IN [-1.0, 0.0] RETURN u"
+                    "query": "MATCH (u:User {enabled: TRUE}) WHERE u.pwdlastset < (datetime().epochseconds - (90 * 86400)) and NOT u.pwdlastset IN [-1.0, 0.0] RETURN u"
                 }
             ]
         },
         {
             "category": "Users",
-            "name": "Find if unprivileged users have rights to add members into groups",
+            "name": "Find if unprivileged users have rights to add members into groups (3 hops)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:User {admincount:False}) MATCH p=allShortestPaths((n)-[r:AddMember*1..]->(m:Group)) RETURN p"
+                    "query": "MATCH p=(u:User {enabled: TRUE, admincount: FALSE})-[:AddMember*1..3]->(m:Group) RETURN p"
                 }
             ]
         },
         {
             "category": "Users",
             "name": "Find all users a part of the VPN group",
             "queryList": [
@@ -699,19 +709,29 @@
                     "final": true,
                     "query": "MATCH p=(o {highvalue: FALSE})-[:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink]->(g:GPO) SET o.highvalue=TRUE RETURN p"
                 }
             ]
         },
         {
             "category": "GPOs",
-            "name": "Find if any domain user has interesting permissions against a GPO (Warning: Heavy)",
+            "name": "Find if any enabled unprivileged domain user has interesting permissions against a GPO (3 hops, limit 200)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(u:User)-[r:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink*1..]->(g:GPO) RETURN p"
+                    "query": "MATCH p=(u:User {enabled: TRUE, admincount: FALSE})-[:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink*1..3]->(g:GPO) RETURN p LIMIT 200"
+                }
+            ]
+        },
+        {
+            "category": "GPOs",
+            "name": "Find if any enabled unprivileged domain user has interesting permissions against a GPO (5 hops, limit 200, Warning: Heavy)",
+            "queryList": [
+                {
+                    "final": true,
+                    "query": "MATCH p=(u:User {enabled: TRUE, admincount: FALSE})-[:AllExtendedRights|GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|GpLink*1..5]->(g:GPO) RETURN p LIMIT 200"
                 }
             ]
         },
         {
             "category": "Outdated OS",
             "name": "Find all computers running with Windows XP",
             "queryList": [
@@ -774,113 +794,135 @@
         {
             "category": "Top Ten",
             "name": "Top Ten Users with Most Sessions",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)<-[r:HasSession]-(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH n, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)-[r:HasSession]->(n) RETURN p"
+                    "query": "MATCH (n:User),(m:Computer), (n)<-[r:HasSession]-(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH n, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)-[r:HasSession]->(n) RETURN p"
                 }
             ]
         },
         {
             "category": "Top Ten",
             "name": "Top Ten Computers with Most Sessions",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)<-[r:HasSession]-(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)-[r:HasSession]->(n) RETURN p"
+                    "query": "MATCH (n:User),(m:Computer), (n)<-[r:HasSession]-(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)-[r:HasSession]->(n) RETURN p"
                 }
             ]
         },
         {
             "category": "Top Ten",
             "name": "Top Ten Users with Most Local Admin Rights",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH n, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN p"
+                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH n, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN p"
                 }
             ]
         },
         {
             "category": "Top Ten",
             "name": "Top Ten Computers with Most Admins and their admins",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN p"
+                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN p"
                 }
             ]
         },
         {
             "category": "Top Ten",
             "name": "Top Ten Computers with Most Admins",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN m"
+                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) RETURN m"
                 }
             ]
         },
         {
             "category": "Top Ten",
             "name": "(Warning: edits the DB) Mark Top Ten Computers with Most Admins as HVT",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) as rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) SET m.highvalue = true RETURN m"
+                    "query": "MATCH (n:User),(m:Computer), (n)-[r:AdminTo]->(m) WHERE NOT n.name STARTS WITH 'ANONYMOUS LOGON' AND NOT n.name='' WITH m, count(r) AS rel_count order by rel_count desc LIMIT 10 MATCH p=(m)<-[r:AdminTo]-(n) SET m.highvalue = true RETURN m"
                 }
             ]
         },
         {
             "category": "Top Ten",
-            "name": "Top 20 nodes with most first degree object controls",
+            "name": "Top 20 nodes, 5 nested max, not DA, not HVT, most group deleg rights",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=(u)-[r1]->(n) WHERE r1.isacl = true WITH u, count(r1) AS count_ctrl ORDER BY count_ctrl DESC LIMIT 20 RETURN u"
+                    "query": "MATCH (daGroup:Group)<-[:MemberOf*1..]-(domainAdmin) WHERE daGroup.objectid ENDS WITH '-512' WITH COLLECT(domainAdmin) AS domainAdmins MATCH (admGroup:Group)<-[:MemberOf*1..]-(domainAdm) WHERE admGroup.objectid ENDS WITH '-544' WITH domainAdmins, COLLECT(domainAdm) AS domainAdms MATCH p=(u)-[r1:MemberOf*1..5]->(g:Group)-[r2]->(n) WHERE r2.isacl=true AND NOT u IN domainAdmins AND NOT u IN domainAdms AND NOT u.highvalue=true WITH u, COUNT(r2) AS count_ctrl ORDER BY count_ctrl DESC LIMIT 20 RETURN u"
                 }
             ]
         },
         {
             "category": "Top Ten",
-            "name": "Top Ten nodes with most group delegated object controls",
+            "name": "Top 10 computers, 5 nested max, not DC, most group deleg rights",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=(u)-[r1:MemberOf*1..]->(g:Group)-[r2]->(n) WHERE r2.isacl=true WITH u, count(r2) AS count_ctrl ORDER BY count_ctrl DESC LIMIT 20 RETURN u"
+                    "query": "MATCH (dcGroup:Group)<-[:MemberOf*1..]-(domainControllers) WHERE dcGroup.objectid ENDS WITH '-516' WITH COLLECT(domainControllers) AS domainControllers MATCH p=(u:Computer)-[r1:MemberOf*1..5]->(g:Group)-[r2]->(n) WHERE r2.isacl=true AND NOT u IN domainControllers WITH u, count(r2) AS count_ctrl ORDER BY count_ctrl DESC LIMIT 10 RETURN u"
                 }
             ]
         },
         {
             "category": "RDP",
-            "name": "Find machines Domain Users can RDP into",
+            "name": "Find enabled machines Domain Users can RDP to",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=(g:Group)-[:CanRDP]->(c:Computer) where g.objectid ENDS WITH '-513' RETURN p"
+                    "query": "MATCH p=((g:Group)-[:CanRDP]->(c:Computer {enabled: TRUE})) WHERE g.objectid ENDS WITH '-513' RETURN p AS path UNION MATCH p2=((g2:Group)-[:MemberOf*1..]->(g3:Group)-[:CanRDP]->(c2:Computer {enabled: TRUE})) WHERE g2.objectid ENDS WITH '-513' RETURN p2 AS path"
                 }
             ]
         },
         {
             "category": "RDP",
-            "name": "Find Servers Domain Users can RDP To",
+            "name": "Find enabled servers Domain Users can RDP to",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH p=(g:Group)-[:CanRDP]->(c:Computer) where g.name STARTS WITH 'DOMAIN USERS' AND c.operatingsystem CONTAINS 'Server' RETURN p"
+                    "query": "MATCH p=((g:Group)-[:CanRDP]->(c:Computer {enabled: TRUE})) WHERE g.objectid ENDS WITH '-513' AND c.operatingsystem =~ '(?i).*Server.*' RETURN p AS path UNION MATCH p2=((g2:Group)-[:MemberOf*1..]->(g3:Group)-[:CanRDP]->(c2:Computer {enabled: TRUE})) WHERE g2.objectid ENDS WITH '-513' AND c2.operatingsystem =~ '(?i).*Server.*' RETURN p2 AS path"
+                }
+            ]
+        },
+        {
+            "category": "RDP",
+            "name": "Find enabled machines Authenticated Users can RDP to",
+            "queryList": [
+                {
+                    "allowCollapse": true,
+                    "final": true,
+                    "query": "MATCH p=((g:Group)-[:CanRDP]->(c:Computer {enabled: TRUE})) WHERE g.objectid =~ '(?i).*S-1-5-11$' RETURN p AS path UNION MATCH p2=((g2:Group)-[:MemberOf*1..]->(g3:Group)-[:CanRDP]->(c2:Computer {enabled: TRUE})) WHERE g2.objectid =~ '(?i).*S-1-5-11$' RETURN p2 AS path"
+                }
+            ]
+        },
+        {
+            "category": "RDP",
+            "name": "Find enabled servers Authenticated Users can RDP to",
+            "queryList": [
+                {
+                    "allowCollapse": true,
+                    "final": true,
+                    "query": "MATCH p=((g:Group)-[:CanRDP]->(c:Computer {enabled: TRUE})) WHERE g.objectid =~ '(?i).*S-1-5-11$' AND c.operatingsystem =~ '(?i).*Server.*' RETURN p AS path UNION MATCH p2=((g2:Group)-[:MemberOf*1..]->(g3:Group)-[:CanRDP]->(c2:Computer {enabled: TRUE})) WHERE g2.objectid =~ '(?i).*S-1-5-11$' AND c2.operatingsystem =~ '(?i).*Server.*' RETURN p2 AS path"
                 }
             ]
         },
         {
             "category": "RDP",
             "name": "Find what groups can RDP",
             "queryList": [
@@ -972,35 +1014,35 @@
         },
         {
             "category": "Certificates",
             "name": "Find all Certificate Templates",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template'}) RETURN n"
                 }
             ]
         },
         {
             "category": "Certificates",
             "name": "Find enabled Certificate Templates",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and n.Enabled = true RETURN n"
+                    "query": "MATCH (n:GPO {Enabled: TRUE, type: 'Certificate Template'}) RETURN n"
                 }
             ]
         },
         {
             "category": "Certificates",
             "name": "Find Certificate Authorities",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Enrollment Service' RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Enrollment Service'}) RETURN n"
                 }
             ]
         },
         {
             "category": "Certificates",
             "name": "Find objects with the ManageCa or ManageCertificates right on Certificate Authorities",
             "queryList": [
@@ -1012,31 +1054,31 @@
         },
         {
             "category": "Certificates",
             "name": "Show Enrollment Rights for Certificate Template",
             "queryList": [
                 {
                     "final": false,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' RETURN n.name",
+                    "query": "MATCH (n:GPO {type: 'Certificate Template'}) RETURN n.name",
                     "title": "Select a Certificate Template..."
                 },
                 {
                     "allowCollapse": false,
                     "final": true,
-                    "query": "MATCH p=(g)-[:Enroll|AutoEnroll]->(n:GPO {name:$result}) WHERE n.type = 'Certificate Template' RETURN p"
+                    "query": "MATCH p=(g)-[:Enroll|AutoEnroll]->(n:GPO {type: 'Certificate Template', name:$result}) RETURN p"
                 }
             ]
         },
         {
             "category": "Certificates",
             "name": "Show Rights for Certificate Authority",
             "queryList": [
                 {
                     "final": false,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Enrollment Service' RETURN n.name",
+                    "query": "MATCH (n:GPO {type: 'Enrollment Service'}) RETURN n.name",
                     "title": "Select a Certificate Authority..."
                 },
                 {
                     "allowCollapse": false,
                     "final": true,
                     "query": "MATCH p=(g)-[:ManageCa|ManageCertificates|Auditor|Operator|Read|Enroll]->(n:GPO {name:$result}) RETURN p"
                 }
@@ -1044,254 +1086,254 @@
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Misconfigured Certificate Templates (ESC1)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and n.`Enrollee Supplies Subject` = true and n.`Client Authentication` = true and n.`Enabled` = true  RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template', `Enrollee Supplies Subject`: TRUE, `Client Authentication`: TRUE, `Enabled`: TRUE}) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Misconfigured Certificate Templates from Owned Principals (ESC1)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Certificate Template' and n.`Enrollee Supplies Subject` = true and n.`Client Authentication` = true and n.`Enabled` = true RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[*1..]->(n:GPO {type: 'Certificate Template', `Enrollee Supplies Subject`: TRUE, `Client Authentication`: TRUE, `Enabled`: TRUE})) WHERE g<>n RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Misconfigured Certificate Templates (ESC2)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and n.`Enabled` = true and (n.`Extended Key Usage` = [] or 'Any Purpose' IN n.`Extended Key Usage`)  RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template', `Enabled`: TRUE}) WHERE (n.`Extended Key Usage` = [] OR 'Any Purpose' IN n.`Extended Key Usage`) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Misconfigured Certificate Templates from Owned Principals (ESC2)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Certificate Template' and n.`Enabled` = true and (n.`Extended Key Usage` = [] or 'Any Purpose' IN n.`Extended Key Usage`) RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[*1..]->(n:GPO {type: 'Certificate Template', `Enabled`: TRUE})) WHERE g<>n AND (n.`Extended Key Usage` = [] OR 'Any Purpose' IN n.`Extended Key Usage`) RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Enrollment Agent Templates (ESC3)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and n.`Enabled` = true and (n.`Extended Key Usage` = [] or 'Any Purpose' IN n.`Extended Key Usage` or 'Certificate Request Agent' IN n.`Extended Key Usage`)  RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template', `Enabled`: TRUE}) WHERE (n.`Extended Key Usage` = [] OR 'Any Purpose' IN n.`Extended Key Usage` OR 'Certificate Request Agent' IN n.`Extended Key Usage`) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Enrollment Agent Templates from Owned Principals (ESC3)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Certificate Template' and n.`Enabled` = true and (n.`Extended Key Usage` = [] or 'Any Purpose' IN n.`Extended Key Usage` or 'Certificate Request Agent' IN n.`Extended Key Usage`) RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[*1..]->(n:GPO {type: 'Certificate Template', `Enabled`: TRUE})) WHERE g<>n AND (n.`Extended Key Usage` = [] OR 'Any Purpose' IN n.`Extended Key Usage` OR 'Certificate Request Agent' IN n.`Extended Key Usage`) RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Vulnerable Certificate Template Access Control (ESC4)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=shortestPath((g)-[:GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Certificate Template' and n.`Enabled` = true RETURN p"
+                    "query": "MATCH p=shortestPath((g)-[:GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner*1..]->(n:GPO {type: 'Certificate Template', `Enabled`: TRUE})) WHERE g<>n RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Vulnerable Certificate Template Access Control from Owned Principals (ESC4)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[r*1..]->(n:GPO)) WHERE g<>n and n.type = 'Certificate Template' and n.Enabled = true and NONE(x in relationships(p) WHERE type(x) = 'Enroll' or type(x) = 'AutoEnroll') RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[*1..]->(n:GPO {type: 'Certificate Template', `Enabled`: TRUE})) WHERE g<>n AND NONE(x IN relationships(p) WHERE type(x) = 'Enroll' OR type(x) = 'AutoEnroll') RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Certificate Authorities with User Specified SAN (ESC6)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Enrollment Service' and n.`User Specified SAN` = 'Enabled' RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Enrollment Service', `User Specified SAN`:'Enabled'}) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Vulnerable Certificate Authority Access Control (ESC7)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=shortestPath((g)-[r:GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ManageCa|ManageCertificates*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Enrollment Service' RETURN p"
+                    "query": "MATCH p=shortestPath((g)-[:GenericAll|GenericWrite|Owns|WriteDacl|WriteOwner|ManageCa|ManageCertificates*1..]->(n:GPO {type: 'Enrollment Service'})) WHERE g<>n RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Vulnerable Certificate Authority Access Control from Owned Principals (ESC7)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[*1..]->(n:GPO)) WHERE  g<>n and n.type = 'Enrollment Service' and NONE(x in relationships(p) WHERE type(x) = 'Enroll' or type(x) = 'AutoEnroll') RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[*1..]->(n:GPO {type:'Enrollment Service'})) WHERE g<>n AND NONE(x IN relationships(p) WHERE type(x) = 'Enroll' OR type(x) = 'AutoEnroll') RETURN p"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Certificate Authorities with HTTP Web Enrollment (ESC8)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Enrollment Service' and n.`Web Enrollment` = 'Enabled' RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Enrollment Service', `Web Enrollment`:'Enabled'}) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Unsecured Certificate Templates - Domain Escalation (ESC9)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and n.`Enrollee Supplies Subject` = true and n.`Client Authentication` = true and n.`Enabled` = true  RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template', `Enrollee Supplies Subject`: TRUE, `Client Authentication`: TRUE, `Enabled`: TRUE}) RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Find Unsecured Certificate Templates - PKI (ESC9)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH (n:GPO) WHERE n.type = 'Certificate Template' and 'NoSecurityExtension' in n.`Enrollment Flag` and n.`Enabled` = true  RETURN n"
+                    "query": "MATCH (n:GPO {type: 'Certificate Template', `Enabled`: TRUE}) WHERE 'NoSecurityExtension' IN n.`Enrollment Flag` RETURN n"
                 }
             ]
         },
         {
             "category": "AD CS Domain Escalation",
             "name": "Shortest Paths to Unsecured Certificate Templates from Owned Principals (ESC9)",
             "queryList": [
                 {
                     "final": true,
-                    "query": "MATCH p=allShortestPaths((g {owned:true})-[r*1..]->(n:GPO)) WHERE n.type = 'Certificate Template' and g<>n and 'NoSecurityExtension' in n.`Enrollment Flag` and n.`Enabled` = true and NONE(rel in r WHERE type(rel) in ['EnabledBy','Read','ManageCa','ManageCertificates']) RETURN p"
+                    "query": "MATCH p=allShortestPaths((g {owned: TRUE})-[r*1..]->(n:GPO {type: 'Certificate Template', `Enabled`: TRUE})) WHERE g<>n AND 'NoSecurityExtension' IN n.`Enrollment Flag` AND NONE(rel IN r WHERE type(rel) IN ['EnabledBy','Read','ManageCa','ManageCertificates']) RETURN p"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Find users with a plaintext attribute that can RDP into something",
+            "name": "Find enabled users with a plaintext attribute that can RDP into something",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintext=True MATCH p1=(u1)-[:CanRDP*1..]->(c:Computer) RETURN u1"
+                    "query": "MATCH p=(u:User {enabled: TRUE, plaintext: TRUE})-[:CanRDP*1..]->(c:Computer) RETURN u"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Find users with a plaintext attribute that belong to high value groups",
+            "name": "Find enabled users with a plaintext attribute that belong to high value groups",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintext=True MATCH p=(u1:User)-[r:MemberOf*1..]->(m:Group {highvalue:true}) RETURN u1"
+                    "query": "MATCH p=(u:User {enabled, TRUE, plaintext: TRUE})-[:MemberOf*1..]->(g:Group {highvalue: TRUE}) RETURN p"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Find users with a plaintext attribute that are kerberoastable",
+            "name": "Find enabled users with a plaintext attribute that are kerberoastable",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintext=True AND u1.hasspn=True RETURN u1"
+                    "query": "MATCH (u:User {enabled: TRUE, plaintext: TRUE, hasspn: TRUE}) RETURN u"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with seasons in their password and are high value targets",
+            "name": "Find enabled users with seasons in their password and are high value targets",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"([Ww]inter.*|[sS]pring.*|[sS]ummer.*|[fF]all.*)\" MATCH p=(u1:User)-[r:MemberOf*1..]->(m:Group {highvalue:true}) RETURN u1"
+                    "query": "MATCH p=(u:User {enabled: TRUE, plaintext: TRUE})-[:MemberOf*1..]->(g:Group {highvalue: TRUE}) WHERE u.plaintextpassword =~ '(?i).*(?:winter|spring|summer|fall).*' RETURN u"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with seasons in their password and have local admin on at least one computer",
+            "name": "Find enabled users with seasons in their password and have local admin on at least one computer",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"([Ww]inter.*|[sS]pring.*|[sS]ummer.*|[fF]all.*)\" MATCH p=(u1:User)-[r:AdminTo]->(n:Computer) RETURN p"
+                    "query": "MATCH p=(u:User {enabled: TRUE, plaintext: TRUE})-[:AdminTo]->(n:Computer) WHERE u.plaintextpassword =~ '(?i).*(?:winter|spring|summer|fall).*' RETURN p"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with seasons in their password and a path to high value targets (limit to 25 results)",
+            "name": "Find enabled users with seasons in their password and a path to high value targets (limit to 25 results)",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"([Ww]inter.*|[sS]pring.*|[sS]ummer.*|[fF]all.*)\" MATCH p=shortestPath((u1:User)-[*1..]->(n {highvalue:true})) WHERE u1<>n RETURN u1 LIMIT 25"
+                    "query": "MATCH p=shortestPath((u:User {enabled: TRUE, plaintext: TRUE})-[*1..]->(n {highvalue: TRUE})) WHERE u.plaintextpassword =~ '(?i).*(?:winter|spring|summer|fall).*' AND u<>n RETURN u LIMIT 25"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with a variant of \"password\" in their password and are high value targets",
+            "name": "Find enabled users with a variant of \"password\" in their password and are members of high value groups",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"(.*[pP][aA@][sS$][sS$][wW][oO0][rR][dD].*)\" MATCH p=(u1:User)-[r:MemberOf*1..]->(m:Group {highvalue:true}) RETURN u1"
+                    "query": "MATCH p=(u:User {enabled: TRUE, plaintext: TRUE})-[:MemberOf*1..]->(m:Group {highvalue: TRUE}) WHERE u.plaintextpassword =~ '(?i).*(?:password).*' RETURN u"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with a variant of \"password\" in their password and have local admin on at least one computer",
+            "name": "Find enabled users with a variant of \"password\" in their password and have local admin on at least one computer",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"(.*[pP][aA@][sS$][sS$][wW][oO0][rR][dD].*)\" MATCH p=(u1:User)-[r:AdminTo]->(n:Computer) RETURN p"
+                    "query": "MATCH p=(u:User {enabled: TRUE, plaintext: TRUE})-[:AdminTo]->(c:Computer {enabled: TRUE}) WHERE u.plaintextpassword =~ '(?i).*(?:password).*' RETURN u"
                 }
             ]
         },
         {
             "category": "PlainText Password Queries",
-            "name": "Return users with a variant of \"password\" in their password and a path to high value targets (limit to 25 results)",
+            "name": "Find enabled users with a variant of \"password\" in their password and a path to high value targets (limit to 25 results)",
             "queryList": [
                 {
                     "allowCollapse": true,
                     "final": true,
-                    "query": "MATCH (u1:User) WHERE u1.plaintextpassword =~ \"(.*[pP][aA@][sS$][sS$][wW][oO0][rR][dD].*)\"  MATCH p=shortestPath((u1:User)-[*1..]->(n {highvalue:true})) WHERE  u1<>n RETURN u1 LIMIT 25"
+                    "query": "MATCH p=shortestPath((u:User {enabled: TRUE, plaintext: TRUE})-[*1..]->(o {highvalue: TRUE})) WHERE u.plaintextpassword =~ '(?i).*(?:password).*' RETURN p LIMIT 25"
                 }
             ]
         },
         {
             "category": "Indexes",
             "name": "Add indexes to the database",
             "queryList": [
@@ -1358,23 +1400,38 @@
                 {
                     "final": false,
                     "query": "CREATE INDEX UserAdminCountIdx IF NOT EXISTS FOR (u:User) on (u.admincount)",
                     "title": "Add index on the property User Admincount"
                 },
                 {
                     "final": false,
+                    "query": "CREATE INDEX UserPlaintextIdx IF NOT EXISTS FOR (u:User) on (u.plaintext)",
+                    "title": "Add index on the property User Plaintext"
+                },
+                {
+                    "final": false,
                     "query": "CREATE INDEX ComputerEnabledIdx IF NOT EXISTS FOR (c:Computer) on (c.enabled)",
                     "title": "Add index on the property Computer Enabled"
                 },
                 {
                     "final": false,
                     "query": "CREATE INDEX UserEnabledIdx IF NOT EXISTS FOR (u:User) on (u.enabled)",
                     "title": "Add index on the property User Enabled"
                 },
                 {
+                    "final": false,
+                    "query": "CREATE INDEX UserHasSPNIdx IF NOT EXISTS FOR (u:User) on (u.hasspn)",
+                    "title": "Add index on the property User HasSPN"
+                },
+                {
+                    "final": false,
+                    "query": "CREATE INDEX GPOTypeIdx IF NOT EXISTS FOR (g:GPO) on (g.type)",
+                    "title": "Add index on the property GPO Type"
+                },
+                {
                     "final": true,
                     "query": "CREATE INDEX GPOEnabledIdx IF NOT EXISTS FOR (g:GPO) on (g.enabled)",
                     "title": "Add index on the property GPO Enabled"
                 }
             ]
         }
     ]
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce` & `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/conf.json` & `exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/conf.json`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/bin/desktop-start` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-start`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/config` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/config`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/exegol_logo.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/exegol_logo.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/default.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/default.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/desktop/wallpapers/space.png` & `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/space.png`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/entrypoint.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,21 @@
     cp --preserve=mode /.exegol/skel/zsh/* "$MY_SETUP_PATH/zsh/"
   fi
 }
 
 function deploy_tmux() {
   colorecho "Deploying tmux"
   if [[ -d "$MY_SETUP_PATH/tmux" ]]; then
-    # copy tmux/tmux.conf to ~/.tmux.conf
-    [[ -f "$MY_SETUP_PATH/tmux/tmux.conf" ]] && cp "$MY_SETUP_PATH/tmux/tmux.conf" ~/.tmux.conf
+    # id define, copy tmux/tmux.conf to ~/.tmux.conf
+    if [[ -f "$MY_SETUP_PATH/tmux/tmux.conf" ]]; then
+      # This key must always be defined (if redefined later in the file, the user user will take precedence)
+      echo 'set-option -g default-shell /bin/zsh' > ~/.tmux.conf
+      # Adding custom user config
+      cat "$MY_SETUP_PATH/tmux/tmux.conf" >> ~/.tmux.conf
+    fi
   else
     mkdir "$MY_SETUP_PATH/tmux" && chmod 770 "$MY_SETUP_PATH/tmux"
   fi
 }
 
 function deploy_vim() {
   colorecho "Deploying vim"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/README.md` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/exegol/start.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/start.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/places.sqlite` & `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/places.sqlite`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/setup.py` & `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/setup.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/firefox/user-setup.py` & `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/user-setup.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.getgpppassword` & `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.getgpppassword`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx` & `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.rbcd` & `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.rbcd`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/grc/conf.secretsdump` & `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.secretsdump`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/grc/grc.conf` & `exegol-4.3.2/exegol-docker-build/sources/assets/grc/grc.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/patches/cloudmapper.patch` & `exegol-4.3.2/exegol-docker-build/sources/assets/patches/cloudmapper.patch`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch` & `exegol-4.3.2/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/proxychains/proxychains.conf` & `exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/proxychains.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/fzf` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fzf`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/metasploit` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/metasploit`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
 alias msfconsole='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfconsole'
 alias msfd='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfd'
-alias msfdb='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfdb'
+msfdb_func() {
+    sudo -u postgres sh -c "cd /opt/tools/metasploit-framework && /usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/bundle exec /opt/tools/metasploit-framework/msfdb $@"
+}
+alias msfdb='msfdb_func'
 alias msfrpc='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfrpc'
 alias msfrpcd='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfrpcd'
 alias msfupdate='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfupdate'
 alias msfvenom='/usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/ruby /opt/tools/metasploit-framework/msfvenom'
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/aliases.d/responder` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/responder`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 function MultiRelay.py { (cd /opt/tools/Responder/tools/ && /opt/tools/Responder/venv/bin/python3 /opt/tools/Responder/tools/MultiRelay.py "$@") }
 alias RunFinger.py='/opt/tools/Responder/venv/bin/python3 /opt/tools/Responder/tools/RunFinger.py'
 alias Responder.py='/opt/tools/Responder/venv/bin/python3 /opt/tools/Responder/Responder.py'
 alias responder-http-on="sed -i 's/HTTP = Off/HTTP = On/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'HTTP ='"
 alias responder-http-off="sed -i 's/HTTP = On/HTTP = Off/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'HTTP ='"
 alias responder-smb-on="sed -i 's/SMB = Off/SMB = On/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'SMB ='"
 alias responder-smb-off="sed -i 's/SMB = On/SMB = Off/g' /opt/tools/Responder/Responder.conf && cat /opt/tools/Responder/Responder.conf | grep --color=never 'SMB ='"
+alias responder="Responder.py"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/exegol_shells_rc` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/exegol_shells_rc`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/GPOddity` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/GPOddity`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/crackmapexec` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackmapexec`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+crackmapexec smb --list-modules
+crackmapexec ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" -M maq
+crackmapexec ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD"
+crackmapexec ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" --asreproast ASREProastables.txt --kdcHost "$DC_HOST"
+crackmapexec ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" --kerberoasting Kerberoastables.txt --kdcHost "$DC_HOST"
+crackmapexec smb "$TARGET" --continue-on-success --no-bruteforce -u users.txt -p passwords.txt
+crackmapexec smb "$TARGET" --continue-on-success -u users.txt -p passwords.txt
+crackmapexec smb "$TARGET" --local-auth -u "$USER" -H "$NT_HASH" -M enum_avproducts
+crackmapexec smb "$TARGET" --local-auth -u "$USER" -H "$NT_HASH" -M mimikatz
+crackmapexec smb "$TARGET" -u '' -p '' --pass-pol
+crackmapexec smb 192.168.56.0/24 --gen-relay-list smb_targets.txt
+crackmapexec smb 192.168.56.0/24 --local-auth -u '' -p ''
+crackmapexec smb 192.168.56.0/24 -u "$USER" -p "$PASSWORD" --loggedon-users
+crackmapexec smb 192.168.56.0/24 -u "$USER" -p "$PASSWORD" --sessions
+crackmapexec smb 192.168.56.0/24 -u "$USER" -p "$PASSWORD" --shares
+crackmapexec smb 192.168.56.0/24 -u '' -p '' --shares
+crackmapexec smb "$IP" -u "$USER" -p "$PASSWORD" -M noPac
+crackmapexec smb "$IP" -u "$USER" -p "$PASSWORD" -M petitpotam
+crackmapexec smb "$IP" -u '' -p '' -M zerologon
+crackmapexec smb "$IP" -u '' -p '' -M ms17-010
+crackmapexec smb "$IP" -u '' -p '' -M ioxidresolver
 cme smb --list-modules
 cme ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" -M maq
 cme ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD"
 cme ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" --asreproast ASREProastables.txt --kdcHost "$DC_HOST"
 cme ldap "$DC_HOST" -d "$DOMAIN" -u "$USER" -p "$PASSWORD" --kerberoasting Kerberoastables.txt --kdcHost "$DC_HOST"
 cme smb "$TARGET" --continue-on-success --no-bruteforce -u users.txt -p passwords.txt
 cme smb "$TARGET" --continue-on-success -u users.txt -p passwords.txt
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/hashcat` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashcat`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/impacket` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/impacket`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/kiterunner` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kiterunner`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/krbrelayx` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/krbrelayx`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nmap` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pth-tools` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pth-tools`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/pywerview` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywerview`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/rsactftool` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsactftool`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/tls-map` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-map`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/volatility3` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility3`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/history.d/wfuzz` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wfuzz`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/shells/zshrc` & `exegol-4.3.2/exegol-docker-build/sources/assets/shells/zshrc`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 export HISTFILESIZE=1000000000
 export HISTSIZE=1000000000
 export HISTTIMEFORMAT="[%F %T] "
 setopt INC_APPEND_HISTORY
 setopt EXTENDED_HISTORY
 setopt HIST_FIND_NO_DUPS
 
+# TERM to prevent tmux not working with autosuggestion
+export TERM=xterm-256color
+
 # Color correction for zsh-syntax-highlighting
 ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE='fg=#626262'
 ZSH_HIGHLIGHT_STYLES[comment]='fg=#888888'
 
 # At the end, loads user-defined zshrc post-routines if the file exists otherwise creates a default file if my-resources is enabled in the container
 if [ -f /opt/my-resources/setup/zsh/zshrc ]
 then
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/trilium/config.ini` & `exegol-4.3.2/exegol-docker-build/sources/assets/trilium/config.ini`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/assets/trilium/trilium-manager.sh` & `exegol-4.3.2/exegol-docker-build/sources/assets/trilium/trilium-manager.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/build_logs_report.py` & `exegol-4.3.2/exegol-docker-build/sources/build_logs_report.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/code_compliance_check.py` & `exegol-4.3.2/exegol-docker-build/sources/code_compliance_check.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/Dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/README.md` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/ad.dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/ad.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/base.dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/base.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/light.dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/light.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/osint.dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/osint.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/dockerfiles/web.dockerfile` & `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/web.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/common.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/common.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/bash
 # Author: The Exegol Project
 
 # Functions and commands that will be retried multiple times to counter random network issues when building
-CATCH_AND_RETRY_COMMANDS=("curl" "wget" "apt-fast" "git" "go" "apt-get" "nvm" "pipx" "pip2" "pip3")
+CATCH_AND_RETRY_COMMANDS=("curl" "wget" "apt-fast" "git" "go" "apt-get" "nvm" "pipx" "pip2" "pip3" "cargo" "gem")
 
 export RED='\033[1;31m'
 export BLUE='\033[1;34m'
 export GREEN='\033[1;32m'
 export NOCOLOR='\033[0m'
 
 ### Echo functions
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/entrypoint.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_ad.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_ad.sh`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,34 @@
     add-to-list "samdump2,https://github.com/azan121468/SAMdump2,A tool to dump Windows NT/2k/XP/Vista password hashes from SAM files"
     add-to-list "smbclient,https://github.com/samba-team/samba,SMBclient is a command-line utility that allows you to access Windows shared resources"
     add-to-list "onesixtyone,https://github.com/trailofbits/onesixtyone,onesixtyone is an SNMP scanner which utilizes a sweep technique to achieve very high performance."
     add-to-list "nbtscan,https://github.com/charlesroelli/nbtscan,NBTscan is a program for scanning IP networks for NetBIOS name information."
     add-to-list "ldapsearch,https://wiki.debian.org/LDAP/LDAPUtils,Search for and display entries (ldap)"
 }
 
+function install_pretender() {
+    # CODE-CHECK-WHITELIST=add-aliases
+    colorecho "Installing Pretender"
+    go install -v github.com/RedTeamPentesting/pretender@latest
+    asdf reshim golang
+    add-history pretender
+    add-test-command "pretender --help |& grep pretender"
+    add-to-list "pretender,https://github.com/RedTeamPentesting/pretender,an mitm tool for helping with relay attacks."
+}
+
 function install_responder() {
     colorecho "Installing Responder"
     git -C /opt/tools/ clone --depth 1 https://github.com/lgandx/Responder
     cd /opt/tools/Responder || exit
     fapt gcc-mingw-w64-x86-64
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     # following requirements needed by MultiRelay.py
-    pip3 install pycryptodome pycryptodomex six
+    pip3 install pycryptodomex six
     deactivate
     sed -i 's/ Random/ 1122334455667788/g' /opt/tools/Responder/Responder.conf
     sed -i 's/files\/AccessDenied.html/\/opt\/tools\/Responder\/files\/AccessDenied.html/g' /opt/tools/Responder/Responder.conf
     sed -i 's/files\/BindShell.exe/\/opt\/tools\/Responder\/files\/BindShell.exe/g' /opt/tools/Responder/Responder.conf
     sed -i 's/certs\/responder.crt/\/opt\/tools\/Responder\/certs\/responder.crt/g' /opt/tools/Responder/Responder.conf
     sed -i 's/certs\/responder.key/\/opt\/tools\/Responder\/certs\/responder.key/g' /opt/tools/Responder/Responder.conf
     x86_64-w64-mingw32-gcc /opt/tools/Responder/tools/MultiRelay/bin/Runas.c -o /opt/tools/Responder/tools/MultiRelay/bin/Runas.exe -municode -lwtsapi32 -luserenv
@@ -53,70 +63,71 @@
     add-test-command "MultiRelay.py --help"
     add-to-list "responder,https://github.com/lgandx/Responder,a LLMNR / NBT-NS and MDNS poisoner."
 }
 
 function install_sprayhound() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing sprayhound"
-    pipx install git+https://github.com/Hackndo/sprayhound
+    pipx install --system-site-packages git+https://github.com/Hackndo/sprayhound
     add-history sprayhound
     add-test-command "sprayhound --help"
     add-to-list "sprayhound,https://github.com/Hackndo/Sprayhound,Active Directory password audit tool."
 }
 
 function install_smartbrute() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing smartbrute"
-    pipx install git+https://github.com/ShutdownRepo/smartbrute
+    pipx install --system-site-packages git+https://github.com/ShutdownRepo/smartbrute
     add-history smartbrute
     add-test-command "smartbrute --help"
     add-to-list "smartbrute,https://github.com/ShutdownRepo/SmartBrute,The smart password spraying and bruteforcing tool for Active Directory Domain Services."
 }
 
 function install_ldapdomaindump() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing ldapdomaindump"
+    # Remove --system-site-packages because the ldapdomaindump package conflicts with the base package
     pipx install git+https://github.com/dirkjanm/ldapdomaindump
     add-history ldapdomaindump
     add-test-command "ldapdomaindump --help"
     add-to-list "ldapdomaindump,https://github.com/dirkjanm/ldapdomaindump,A tool for dumping domain data from an LDAP service"
 }
 
 function install_crackmapexec() {
     colorecho "Installing CrackMapExec"
     git -C /opt/tools/ clone --depth 1 https://github.com/Porchetta-Industries/CrackMapExec
-    pipx install /opt/tools/CrackMapExec/
+    pipx install --system-site-packages /opt/tools/CrackMapExec/
     mkdir -p ~/.cme
     [[ -f ~/.cme/cme.conf ]] && mv ~/.cme/cme.conf ~/.cme/cme.conf.bak
     cp -v /root/sources/assets/crackmapexec/cme.conf ~/.cme/cme.conf
     # below is for having the ability to check the source code when working with modules and so on
     cp -v /root/sources/assets/grc/conf.cme /usr/share/grc/conf.cme
     add-aliases crackmapexec
     add-history crackmapexec
     add-test-command "crackmapexec --help"
     add-to-list "crackmapexec,https://github.com/Porchetta-Industries/CrackMapExec,Network scanner."
 }
 
 function install_bloodhound-py() {
     colorecho "Installing and Python ingestor for BloodHound"
-    pipx install git+https://github.com/fox-it/BloodHound.py
+    pipx install --system-site-packages git+https://github.com/fox-it/BloodHound.py
     add-aliases bloodhound-py
     add-history bloodhound-py
     add-test-command "bloodhound.py --help"
     add-to-list "bloodhound.py,https://github.com/fox-it/BloodHound.py,BloodHound ingestor in Python."
 }
 
 
 function install_bloodhound-ce-py() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing and Python ingestor for BloodHound-CE"
     git -C /opt/tools/ clone https://github.com/dirkjanm/BloodHound.py BloodHound-CE.py
     cd /opt/tools/BloodHound-CE.py || exit
     git checkout bloodhound-ce
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install .
     deactivate
     ln -v -s /opt/tools/BloodHound-CE.py/venv/bin/bloodhound-python /opt/tools/bin/bloodhound-ce.py
     add-history bloodhound-ce-py
     add-test-command "bloodhound-ce.py --help"
     add-to-list "bloodhound-ce.py,https://github.com/fox-it/BloodHound.py,BloodHound-CE ingestor in Python."
@@ -197,25 +208,19 @@
     mkdir /opt/tools/BloodHound-CE/work
     ln -v -s /opt/tools/BloodHound-CE/src/artifacts/bhapi /opt/tools/BloodHound-CE/bloodhound
     cp -v /opt/tools/BloodHound-CE/src/dockerfiles/configs/bloodhound.config.json /opt/tools/BloodHound-CE/
     cp -v /root/sources/assets/bloodhound-ce/* /opt/tools/bin/
     chmod +x /opt/tools/bin/bloodhound*
 
     # Configuration
-    sed -i "s#app-db#127.0.0.1##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#graph-db#127.0.0.1##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#8080#1030##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#0.0.0.0#127.0.0.1##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#neo4j:bloodhoundcommunityedition#neo4j:exegol4thewin##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#user=bloodhound password=bloodhoundcommunityedition#user=bloodhound password=exegol4thewin##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#/etc/bloodhound/collectors#/opt/tools/BloodHound-CE/collectors##" /opt/tools/BloodHound-CE/bloodhound.config.json
-    sed -i "s#/opt/bloodhound/work#/opt/tools/BloodHound-CE/work##" /opt/tools/BloodHound-CE/bloodhound.config.json
+    cp -v /root/sources/assets/bloodhound-ce/bloodhound.config.json /opt/tools/BloodHound-CE/
 
     # the following test command probably needs to be changed. No idea how we can make sure bloodhound-ce works as intended.
     add-test-command "/opt/tools/BloodHound-CE/bloodhound -version"
+    add-test-command "service postgresql start && sleep 5 && PGPASSWORD=exegol4thewin psql -U bloodhound -d bloodhound -h localhost -c '\l' && service postgresql stop"
     add-to-list "BloodHound-CE,https://github.com/SpecterOps/BloodHound,Active Directory security tool for reconnaissance and attacking AD environments (Community Edition)"
 }
 
 function install_cypheroth() {
     colorecho "Installing cypheroth"
     git -C /opt/tools/ clone --depth 1 https://github.com/seajaysec/cypheroth
     add-aliases cypheroth
@@ -223,32 +228,32 @@
     add-test-command "cypheroth.sh --help|& grep 'Example with Defaults:'"
     add-to-list "cyperoth,https://github.com/seajaysec/cypheroth,Automated extensible toolset that runs cypher queries against Bloodhound's Neo4j backend and saves output to spreadsheets."
 }
 
 function install_mitm6_pip() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing mitm6 with pip"
-    pipx install mitm6
+    pipx install --system-site-packages mitm6
     add-history mitm6
     add-test-command "mitm6 --help"
     add-to-list "mitm6,https://github.com/fox-it/mitm6,Tool to conduct a man-in-the-middle attack against IPv6 protocols."
 }
 
 function install_aclpwn() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing aclpwn with pip"
-    pipx install git+https://github.com/aas-n/aclpwn.py
+    pipx install --system-site-packages git+https://github.com/aas-n/aclpwn.py
     add-history aclpwn
     add-test-command "aclpwn -h"
     add-to-list "aclpwn,https://github.com/aas-n/aclpwn.py,Tool for testing the security of Active Directory access controls."
 }
 
 function install_impacket() {
     colorecho "Installing Impacket scripts"
-    pipx install git+https://github.com/ThePorgs/impacket
+    pipx install --system-site-packages git+https://github.com/ThePorgs/impacket
     pipx inject impacket chardet
     cp -v /root/sources/assets/grc/conf.ntlmrelayx /usr/share/grc/conf.ntlmrelayx
     cp -v /root/sources/assets/grc/conf.secretsdump /usr/share/grc/conf.secretsdump
     cp -v /root/sources/assets/grc/conf.getgpppassword /usr/share/grc/conf.getgpppassword
     cp -v /root/sources/assets/grc/conf.rbcd /usr/share/grc/conf.rbcd
     cp -v /root/sources/assets/grc/conf.describeTicket /usr/share/grc/conf.describeTicket
     add-aliases impacket
@@ -273,25 +278,25 @@
     add-test-command "ms14-068.py |& grep '<clearPassword>'"
     add-to-list "pykek,https://github.com/preempt/pykek,PyKEK (Python Kerberos Exploitation Kit) a python library to manipulate KRB5-related data."
 }
 
 function install_lsassy() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing lsassy"
-    pipx install lsassy
+    pipx install --system-site-packages lsassy
     add-history lsassy
     add-test-command "lsassy --version"
     add-to-list "lsassy,https://github.com/Hackndo/lsassy,Windows secrets and passwords extraction tool."
 }
 
 function install_privexchange() {
     colorecho "Installing privexchange"
     git -C /opt/tools/ clone --depth 1 https://github.com/dirkjanm/PrivExchange
     cd /opt/tools/PrivExchange || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases privexchange
     add-history privexchange
     add-test-command "privexchange.py --help"
     add-to-list "privexchange,https://github.com/dirkjanm/PrivExchange,a tool to perform attacks against Microsoft Exchange server using NTLM relay techniques"
@@ -393,68 +398,68 @@
     fi
 }
 
 function install_krbrelayx() {
     colorecho "Installing krbrelayx"
     git -C /opt/tools/ clone --depth 1 https://github.com/dirkjanm/krbrelayx
     cd /opt/tools/krbrelayx || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
-    pip3 install dnspython ldap3 impacket dsinternals pycryptodome
+    pip3 install dnspython ldap3 impacket dsinternals
     deactivate
     cp -v /root/sources/assets/grc/conf.krbrelayx /usr/share/grc/conf.krbrelayx
     add-aliases krbrelayx
     add-history krbrelayx
     add-test-command "krbrelayx.py --help"
     add-test-command "addspn.py --help"
     add-test-command "addspn.py --help"
     add-test-command "printerbug.py --help"
     add-to-list "krbrelayx,https://github.com/dirkjanm/krbrelayx,a tool for performing Kerberos relay attacks"
 }
 
 function install_evilwinrm() {
     colorecho "Installing evil-winrm"
-    rvm use 3.2.2@evil-winrm --create
+    rvm use 3.1.2@evil-winrm --create
     gem install evil-winrm
     rvm use 3.2.2@default
     add-aliases evil-winrm
     add-history evil-winrm
     add-test-command "evil-winrm --help"
     add-to-list "evilwinrm,https://github.com/Hackplayers/evil-winrm,Tool to connect to a remote Windows system with WinRM."
 }
 
 function install_pypykatz() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing pypykatz"
     # without following fix, tool raises "oscrypto.errors.LibraryNotFoundError: Error detecting the version of libcrypto"
     # see https://github.com/wbond/oscrypto/issues/78 and https://github.com/wbond/oscrypto/issues/75
-    local temp_fix_limit="2024-01-20"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       git -C /opt/tools/ clone --depth 1 https://github.com/skelsec/pypykatz
       cd /opt/tools/pypykatz || exit
-      python3 -m venv ./venv/
+      python3 -m venv --system-site-packages ./venv
       source ./venv/bin/activate
       pip3 install .
       pip3 install --force oscrypto@git+https://github.com/wbond/oscrypto.git
       ln -v -s /opt/tools/pypykatz/venv/bin/pypykatz /opt/tools/bin/pypykatz
       deactivate
     fi
-    # pipx install pypykatz
+    # pipx install --system-site-packages pypykatz
     add-history pypykatz
     add-test-command "pypykatz version"
     add-test-command "pypykatz crypto nt 'exegol4thewin'"
     add-to-list "pypykatz,https://github.com/skelsec/pypykatz,a Python library for mimikatz-like functionality"
 }
 
 function install_krbjack() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
     colorecho "Installing krbjack"
-    pipx install krbjack
+    pipx install --system-site-packages krbjack
     add-test-command "krbjack --help"
     add-to-list "krbjack,https://github.com/almandin/krbjack,A Kerberos AP-REQ hijacking tool with DNS unsecure updates abuse."
 }
 
 function install_enyx() {
     colorecho "Installing enyx"
     git -C /opt/tools/ clone --depth 1 https://github.com/trickster0/Enyx
@@ -463,25 +468,25 @@
     add-test-command "enyx.py"
     add-to-list "enyx,https://github.com/trickster0/enyx,Framework for building offensive security tools."
 }
 
 function install_enum4linux-ng() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing enum4linux-ng"
-    pipx install git+https://github.com/cddmp/enum4linux-ng
+    pipx install --system-site-packages git+https://github.com/cddmp/enum4linux-ng
     add-history enum4linux-ng
     add-test-command "enum4linux-ng --help"
     add-to-list "enum4linux-ng,https://github.com/cddmp/enum4linux-ng,Tool for enumerating information from Windows and Samba systems."
 }
 
 function install_zerologon() {
     colorecho "Pulling CVE-2020-1472 exploit and scan scripts"
     mkdir /opt/tools/zerologon
     cd /opt/tools/zerologon || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     git -C /opt/tools/zerologon clone --depth 1 https://github.com/SecuraBV/CVE-2020-1472 zerologon-scan
     git -C /opt/tools/zerologon clone --depth 1 https://github.com/dirkjanm/CVE-2020-1472 zerologon-exploit
     add-aliases zerologon
     add-history zerologon
@@ -521,15 +526,15 @@
 }
 
 function install_oaburl() {
     colorecho "Downloading oaburl.py"
     mkdir /opt/tools/OABUrl
     wget -O /opt/tools/OABUrl/oaburl.py "https://gist.githubusercontent.com/snovvcrash/4e76aaf2a8750922f546eed81aa51438/raw/96ec2f68a905eed4d519d9734e62edba96fd15ff/oaburl.py"
     cd /opt/tools/OABUrl/ || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install requests
     deactivate
     add-aliases oaburl
     add-history oaburl
     add-test-command "oaburl.py --help"
     add-to-list "oaburl,https://gist.githubusercontent.com/snovvcrash/4e76aaf2a8750922f546eed81aa51438/raw/96ec2f68a905eed4d519d9734e62edba96fd15ff/oaburl.py,Find Open redirects and other vulnerabilities."
@@ -549,30 +554,30 @@
     add-to-list "lnkup,https://github.com/Plazmaz/lnkUp,This tool will allow you to generate LNK payloads. Upon rendering or being run they will exfiltrate data."
 }
 
 function install_polenum() {
     colorecho "Installing polenum"
     git -C /opt/tools/ clone --depth 1 https://github.com/Wh1t3Fox/polenum
     cd /opt/tools/polenum || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases polenum
     add-history polenum
     add-test-command "polenum.py --help"
     add-to-list "polenum,https://github.com/Wh1t3Fox/polenum,Polenum is a Python script which uses the Impacket library to extract user information through the SMB protocol."
 }
 
 function install_smbmap() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing smbmap"
     git -C /opt/tools clone --depth 1 https://github.com/ShawnDEvans/smbmap
     cd /opt/tools/smbmap || exit
-    pipx install .
+    pipx install --system-site-packages .
     add-history smbmap
     add-test-command "smbmap --help"
     add-to-list "smbmap,https://github.com/ShawnDEvans/smbmap,A tool to enumerate SMB shares and check for null sessions"
 }
 
 function install_pth-tools() {
     colorecho "Installing pth-tools"
@@ -596,25 +601,25 @@
         criticalecho-noexit "This installation function doesn't support architecture $(uname -m)" && return
     fi
 }
 
 function install_smtp-user-enum() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing smtp-user-enum"
-    pipx install smtp-user-enum
+    pipx install --system-site-packages smtp-user-enum
     add-history smtp-user-enum
     add-test-command "smtp-user-enum --help"
     add-to-list "smtp-user-enum,https://github.com/pentestmonkey/smtp-user-enum,A tool to enumerate email addresses via SMTP"
 }
 
 function install_gpp-decrypt() {
     colorecho "Installing gpp-decrypt"
     git -C /opt/tools/ clone --depth 1 https://github.com/t0thkr1s/gpp-decrypt
     cd /opt/tools/gpp-decrypt || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install pycryptodome colorama
     deactivate
     add-aliases gpp-decrypt
     add-history gpp-decrypt
     add-test-command "gpp-decrypt.py -f /opt/tools/gpp-decrypt/groups.xml"
     add-to-list "gpp-decrypt,https://github.com/t0thkr1s/gpp-decrypt,A tool to decrypt Group Policy Preferences passwords"
@@ -628,15 +633,15 @@
     add-test-command "ntlmv1-multi.py --ntlmv1 a::a:a:a:a"
     add-to-list "ntlmv1-multi,https://github.com/evilmog/ntlmv1-multi,Exploit a vulnerability in Microsoft Windows to gain system-level access."
 }
 
 function install_hashonymize() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing hashonymizer"
-    pipx install git+https://github.com/ShutdownRepo/hashonymize
+    pipx install --system-site-packages git+https://github.com/ShutdownRepo/hashonymize
     add-history hashonymize
     add-test-command "hashonymize --help"
     add-to-list "hashonymize,https://github.com/ShutdownRepo/hashonymize,This small tool is aimed at anonymizing hashes files for offline but online cracking like Google Collab for instance (see https://github.com/ShutdownRepo/google-colab-hashcat)."
 }
 
 function install_gosecretsdump() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -647,31 +652,30 @@
     add-test-command "gosecretsdump -version"
     add-to-list "gosecretsdump,https://github.com/c-sto/gosecretsdump,Implements NTLMSSP network authentication protocol in Go"
 }
 
 function install_adidnsdump() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing adidnsdump"
-    pipx install git+https://github.com/dirkjanm/adidnsdump
-    pipx inject adidnsdump pycryptodome
+    pipx install --system-site-packages git+https://github.com/dirkjanm/adidnsdump
     add-history adidnsdump
     add-test-command "adidnsdump --help"
     add-to-list "adidnsdump,https://github.com/dirkjanm/adidnsdump,Active Directory Integrated DNS dump utility"
 }
 
 function install_pygpoabuse() {
     colorecho "Installing pyGPOabuse"
     git -C /opt/tools/ clone --depth 1 https://github.com/Hackndo/pyGPOAbuse
     cd /opt/tools/pyGPOAbuse || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     # without following fix, tool raises "oscrypto.errors.LibraryNotFoundError: Error detecting the version of libcrypto"
     # see https://github.com/wbond/oscrypto/issues/78 and https://github.com/wbond/oscrypto/issues/75
-    local temp_fix_limit="2024-01-20"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       pip3 install --force oscrypto@git+https://github.com/wbond/oscrypto.git
     fi
     deactivate
     add-aliases pygpoabuse
@@ -679,102 +683,102 @@
     add-test-command "pygpoabuse.py --help"
     add-to-list "pygpoabuse,https://github.com/Hackndo/pyGPOAbuse,A tool for abusing GPO permissions to escalate privileges"
 }
 
 function install_bloodhound-import() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing bloodhound-import"
-    pipx install bloodhound-import
+    pipx install --system-site-packages bloodhound-import
     add-history bloodhound-import
     add-test-command "bloodhound-import --help"
     add-to-list "bloodhound-import,https://github.com/fox-it/BloodHound.py,Import data into BloodHound for analyzing active directory trust relationships"
 }
 
 function install_bloodhound-quickwin() {
     colorecho "Installing bloodhound-quickwin"
     git -C /opt/tools/ clone --depth 1 https://github.com/kaluche/bloodhound-quickwin
     cd /opt/tools/bloodhound-quickwin || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases bloodhound-quickwin
     add-history bloodhound-quickwin
     add-test-command "bloodhound-quickwin --help"
     add-to-list "bloodhound-quickwin,https://github.com/kaluche/bloodhound-quickwin,A tool for BloodHounding on Windows machines without .NET or Powershell installed"
 }
 
 function install_ldapsearch-ad() {
     colorecho "Installing ldapsearch-ad"
     git -C /opt/tools/ clone --depth 1 https://github.com/yaap7/ldapsearch-ad
     cd /opt/tools/ldapsearch-ad || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases ldapsearch-ad
     add-history ldapsearch-ad
     add-test-command "ldapsearch-ad.py --version"
     add-to-list "ldapsearch-ad,https://github.com/yaap7/ldapsearch-ad,LDAP search utility with AD support"
 }
 
 function install_petitpotam() {
     colorecho "Installing PetitPotam"
     git -C /opt/tools/ clone --depth 1 https://github.com/ly4k/PetitPotam
     cd /opt/tools/PetitPotam || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     mv /opt/tools/PetitPotam /opt/tools/PetitPotam_alt
     git -C /opt/tools/ clone --depth 1 https://github.com/topotam/PetitPotam
     cd /opt/tools/PetitPotam || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases petitpotam
     add-history petitpotam
     add-test-command "petitpotam.py --help"
     add-to-list "petitpotam,https://github.com/topotam/PetitPotam,Windows machine account manipulation"
 }
 
 function install_dfscoerce() {
     colorecho "Installing DfsCoerce"
     git -C /opt/tools/ clone --depth 1 https://github.com/Wh04m1001/DFSCoerce
     cd /opt/tools/DFSCoerce || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases dfscoerce
     add-history dfscoerce
     add-test-command "dfscoerce.py --help"
     add-to-list "dfscoerce,https://github.com/Wh04m1001/dfscoerce,DFS-R target coercion tool"
 }
 
 function install_coercer() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Coercer"
-    pipx install git+https://github.com/p0dalirius/Coercer
+    pipx install --system-site-packages git+https://github.com/p0dalirius/Coercer
     add-history coercer
     add-test-command "coercer --help"
     add-to-list "coercer,https://github.com/p0dalirius/coercer,DFS-R target coercion tool"
 }
 
 function install_pkinittools() {
     colorecho "Installing PKINITtools"
     git -C /opt/tools/ clone --depth 1 https://github.com/dirkjanm/PKINITtools
     cd /opt/tools/PKINITtools || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     # without following fix, tool raises "oscrypto.errors.LibraryNotFoundError: Error detecting the version of libcrypto"
     # see https://github.com/wbond/oscrypto/issues/78 and https://github.com/wbond/oscrypto/issues/75
-    local temp_fix_limit="2024-01-20"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       pip3 install --force oscrypto@git+https://github.com/wbond/oscrypto.git
     fi
     deactivate
     add-aliases pkinittools
@@ -783,29 +787,29 @@
     add-to-list "pkinittools,https://github.com/dirkjanm/PKINITtools,Pkinit support tools"
 }
 
 function install_pywhisker() {
     colorecho "Installing pyWhisker"
     git -C /opt/tools/ clone --depth 1 https://github.com/ShutdownRepo/pywhisker
     cd /opt/tools/pywhisker || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases pywhisker
     add-history pywhisker
     add-test-command "pywhisker.py --help"
     add-to-list "pywhisker,https://github.com/ShutdownRepo/pywhisker,PyWhisker is a Python equivalent of the original Whisker made by Elad Shamir and written in C#. This tool allows users to manipulate the msDS-KeyCredentialLink attribute of a target user/computer to obtain full control over that object. It's based on Impacket and on a Python equivalent of Michael Grafnetter's DSInternals called PyDSInternals made by podalirius."
 }
 
 function install_manspider() {
     colorecho "Installing Manspider"
     git -C /opt/tools clone --depth 1 https://github.com/blacklanternsecurity/MANSPIDER.git
     cd /opt/tools/MANSPIDER || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install .
     deactivate
     touch ./man_spider/lib/init.py
     sed -i "s#from .lib import#from lib import##" man_spider/manspider.py
     add-aliases manspider
     add-history manspider
@@ -813,45 +817,45 @@
     add-to-list "manspider,https://github.com/blacklanternsecurity/MANSPIDER,Manspider will crawl every share on every target system. If provided creds don't work it will fall back to 'guest' then to a null session."
 }
 
 function install_targetedKerberoast() {
     colorecho "Installing targetedKerberoast"
     git -C /opt/tools/ clone --depth 1 https://github.com/ShutdownRepo/targetedKerberoast
     cd /opt/tools/targetedKerberoast || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases targetedkerberoast
     add-history targetedkerberoast
     add-test-command "targetedKerberoast.py --help"
     add-to-list "targetedKerberoast,https://github.com/ShutdownRepo/targetedKerberoast,Kerberoasting against specific accounts"
 }
 
 function install_pcredz() {
     colorecho "Installing PCredz"
     fapt libpcap-dev
     git -C /opt/tools/ clone --depth 1 https://github.com/lgandx/PCredz
     cd /opt/tools/PCredz || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install Cython python-libpcap
     deactivate
     add-aliases pcredz
     add-history pcredz
     add-test-command "PCredz --help"
     add-to-list "pcredz,https://github.com/lgandx/PCredz,PowerShell credential dumper"
 }
 
 function install_pywsus() {
     colorecho "Installing pywsus"
     fapt libxml2-dev libxslt-dev
     git -C /opt/tools/ clone --depth 1 https://github.com/GoSecure/pywsus
     cd /opt/tools/pywsus || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     # https://github.com/GoSecure/pywsus/pull/12
     echo -e "beautifulsoup4==4.9.1\nlxml==4.9.1\nsoupsieve==2.0.1" > requirements.txt
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases pywsus
     add-history pywsus
@@ -859,111 +863,104 @@
     add-to-list "pywsus,https://github.com/GoSecure/pywsus,Python implementation of a WSUS client"
 }
 
 function install_donpapi() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing DonPAPI"
     fapt swig
-    pipx install git+https://github.com/login-securite/DonPAPI
+    pipx install --system-site-packages git+https://github.com/login-securite/DonPAPI
     add-history donpapi
     add-test-command "DonPAPI --help"
     add-to-list "donpapi,https://github.com/login-securite/DonPAPI,Dumping revelant information on compromised targets without AV detection"
 }
 
 function install_webclientservicescanner() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing webclientservicescanner"
-    pipx install git+https://github.com/Hackndo/WebclientServiceScanner
+    pipx install --system-site-packages git+https://github.com/Hackndo/WebclientServiceScanner
     add-history webclientservicescanner
     add-test-command "webclientservicescanner --help"
     add-to-list "webclientservicescanner,https://github.com/Hackndo/webclientservicescanner,Scans for web service endpoints"
 }
 
 function install_certipy() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Certipy"
-    pipx install git+https://github.com/ly4k/Certipy
+    pipx install --system-site-packages git+https://github.com/ly4k/Certipy
     add-history certipy
     add-test-command "certipy --version"
     add-to-list "certipy,https://github.com/ly4k/Certipy,Python tool to create and sign certificates"
 }
 
 function install_shadowcoerce() {
     colorecho "Installing ShadowCoerce PoC"
     git -C /opt/tools/ clone --depth 1 https://github.com/ShutdownRepo/ShadowCoerce
     cd /opt/tools/ShadowCoerce || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases shadowcoerce
     add-history shadowcoerce
     add-test-command "shadowcoerce.py --help"
     add-to-list "shadowcoerce,https://github.com/ShutdownRepo/shadowcoerce,Utility for bypassing the Windows Defender antivirus by hiding a process within a legitimate process."
 }
 
 function install_gmsadumper() {
     colorecho "Installing gMSADumper"
     git -C /opt/tools/ clone --depth 1 https://github.com/micahvandeusen/gMSADumper
     cd /opt/tools/gMSADumper || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
-    # https://github.com/micahvandeusen/gMSADumper/issues/12
-    local temp_fix_limit="2024-01-20"
-    if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
-      criticalecho "Temp fix expired. Exiting."
-    else
-      pip3 install pycryptodome
-    fi
     deactivate
     add-aliases gmsadumper
     add-history gmsadumper
     add-test-command "gMSADumper.py --help"
     add-to-list "gmsadumper,https://github.com/micahvandeusen/gMSADumper,A tool for extracting credentials and other information from a Microsoft Active Directory domain."
 }
 
 function install_pylaps() {
     colorecho "Installing pyLAPS"
     git -C /opt/tools/ clone --depth 1 https://github.com/p0dalirius/pyLAPS
     cd /opt/tools/pyLAPS || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases pylaps
     add-history pylaps
     add-test-command "pyLAPS.py --help"
     add-to-list "pylaps,https://github.com/p0dalirius/pylaps,Utility for enumerating and querying LDAP servers."
 }
 
 function install_finduncommonshares() {
     colorecho "Installing FindUncommonShares"
     git -C /opt/tools/ clone --depth 1 https://github.com/p0dalirius/FindUncommonShares
     cd /opt/tools/FindUncommonShares/ || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases finduncommonshares
     add-history finduncommonshares
     add-test-command "FindUncommonShares.py --help"
     add-to-list "finduncommonshares,https://github.com/p0dalirius/FindUncommonShares,Script that can help identify shares that are not commonly found on a Windows system."
 }
 
 function install_ldaprelayscan() {
     colorecho "Installing LdapRelayScan"
     git -C /opt/tools/ clone --depth 1 https://github.com/zyn3rgy/LdapRelayScan
     cd /opt/tools/LdapRelayScan || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     # without following fix, tool raises "oscrypto.errors.LibraryNotFoundError: Error detecting the version of libcrypto"
     # see https://github.com/wbond/oscrypto/issues/78 and https://github.com/wbond/oscrypto/issues/75
-    local temp_fix_limit="2024-01-20"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       pip3 install --force oscrypto@git+https://github.com/wbond/oscrypto.git
     fi
     deactivate
     add-aliases ldaprelayscan
@@ -973,29 +970,29 @@
 }
 
 function install_goldencopy() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing GoldenCopy"
     git -C /opt/tools/ clone --depth 1 https://github.com/Dramelac/GoldenCopy
     cd /opt/tools/GoldenCopy || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install .
     deactivate
     ln -v -s /opt/tools/GoldenCopy/venv/bin/goldencopy /opt/tools/bin/goldencopy
     add-history goldencopy
     add-test-command "goldencopy --help"
     add-to-list "goldencopy,https://github.com/Dramelac/GoldenCopy,Copy the properties and groups of a user from neo4j (bloodhound) to create an identical golden ticket"
 }
 
 function install_crackhound() {
     colorecho "Installing CrackHound"
     git -C /opt/tools/ clone --depth 1 https://github.com/trustedsec/CrackHound
     cd /opt/tools/CrackHound || exit
-    python3 -m venv ./venv/
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases crackhound
     add-history crackhound
     add-test-command "crackhound.py --help"
     add-to-list "crackhound,https://github.com/trustedsec/crackhound,A fast WPA/WPA2/WPA3 WiFi Handshake capture / password recovery and analysis tool"
@@ -1011,15 +1008,15 @@
     add-to-list "kerbrute,https://github.com/ropnop/kerbrute,A tool to perform Kerberos pre-auth bruteforcing"
 }
 
 function install_ldeep() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing ldeep"
     fapt libkrb5-dev krb5-config
-    pipx install ldeep
+    pipx install --system-site-packages ldeep
     add-history ldeep
     add-test-command "ldeep --help"
     add-to-list "ldeep,https://github.com/franc-pentest/ldeep,ldeep is a tool to discover hidden paths on Web servers."
 }
 
 function install_rusthound() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -1054,70 +1051,70 @@
     add-test-command "rusthound-ce --help"
     add-to-list "rusthound (v2),https://github.com/OPENCYBER-FR/RustHound,BloodHound-CE ingestor in Rust."
 }
 
 function install_certsync() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing certsync"
-    pipx install git+https://github.com/zblurx/certsync
+    pipx install --system-site-packages git+https://github.com/zblurx/certsync
     add-history certsync
     add-test-command "certsync --help"
     add-to-list "certsync,https://github.com/zblurx/certsync,certsync is a tool that helps you synchronize certificates between two directories."
 }
 
 function install_keepwn() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing KeePwn"
-    pipx install git+https://github.com/Orange-Cyberdefense/KeePwn
+    pipx install --system-site-packages git+https://github.com/Orange-Cyberdefense/KeePwn
     add-history keepwn
     add-test-command "KeePwn --help"
     add-to-list "KeePwn,https://github.com/Orange-Cyberdefense/KeePwn,KeePwn is a tool that extracts passwords from KeePass 1.x and 2.x databases."
 }
 
 function install_pre2k() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing pre2k"
-    pipx install git+https://github.com/garrettfoster13/pre2k
+    pipx install --system-site-packages git+https://github.com/garrettfoster13/pre2k
     add-history pre2k
     add-test-command "pre2k --help"
     add-to-list "pre2k,https://github.com/garrettfoster13/pre2k,pre2k is a tool to check if a Windows domain has any pre-2000 Windows 2000 logon names still in use."
 }
 
 function install_msprobe() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing msprobe"
-    pipx install git+https://github.com/puzzlepeaches/msprobe
+    pipx install --system-site-packages git+https://github.com/puzzlepeaches/msprobe
     add-history msprobe
     add-test-command "msprobe --help"
     add-to-list "msprobe,https://github.com/puzzlepeaches/msprobe,msprobe is a tool to identify Microsoft Windows hosts and servers that are running certain services."
 }
 
 function install_masky() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing masky"
-    pipx install git+https://github.com/Z4kSec/Masky
+    pipx install --system-site-packages git+https://github.com/Z4kSec/Masky
     add-history masky
     add-test-command "masky --help"
-    add-to-list "masky,https://github.com/Z4kSec/masky,masky is a tool to mask sensitive data / such as credit card numbers / in logs and other files."
+    add-to-list "masky,https://github.com/Z4kSec/Masky,Masky is a python library providing an alternative way to remotely dump domain users' credentials thanks to an ADCS. A command line tool has been built on top of this library in order to easily gather PFX or NT hashes and TGT on a larger scope"
 }
 
 function install_roastinthemiddle() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing roastinthemiddle"
-    pipx install git+https://github.com/Tw1sm/RITM
+    pipx install --system-site-packages git+https://github.com/Tw1sm/RITM
     add-history roastinthemiddle
     add-test-command "roastinthemiddle --help"
     add-to-list "roastinthemiddle,https://github.com/Tw1sm/RITM,RoastInTheMiddle is a tool to intercept and relay NTLM authentication requests."
 }
 
 function install_PassTheCert() {
     colorecho "Installing PassTheCert"
     git -C /opt/tools/ clone --depth 1 https://github.com/AlmondOffSec/PassTheCert
     cd /opt/tools/PassTheCert/Python/ || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install impacket
     deactivate
     add-aliases PassTheCert
     add-history PassTheCert
     add-test-command "passthecert.py --help"
     add-to-list "PassTheCert,https://github.com/AlmondOffSec/PassTheCert,PassTheCert is a tool to extract Active Directory user password hashes from a domain controller's local certificate store."
@@ -1156,102 +1153,102 @@
     add-to-list "neo4j,https://github.com/neo4j/neo4j,Database."
 }
 
 function install_noPac() {
     colorecho "Installing noPac"
     git -C /opt/tools/ clone --depth 1 https://github.com/Ridter/noPac
     cd /opt/tools/noPac || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases noPac
     add-history noPac
     add-test-command "noPac.py --help"
     add-to-list "noPac,https://github.com/Ridter/noPac,Exploiting CVE-2021-42278 and CVE-2021-42287 to impersonate DA from standard domain user."
 }
 
 function install_roadtools() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
     colorecho "Installing roadtools"
-    pipx install roadrecon
+    pipx install --system-site-packages roadrecon
     add-test-command "roadrecon --help"
     add-test-command "roadrecon-gui --help"
     add-to-list "ROADtools,https://github.com/dirkjanm/ROADtools,ROADtools is a framework to interact with Azure AD. It consists of a library (roadlib) with common components / the ROADrecon Azure AD exploration tool and the ROADtools Token eXchange (roadtx) tool."
 }
 
 function install_teamsphisher() {
     colorecho "Installing TeamsPhisher"
     git -C /opt/tools clone --depth 1 https://github.com/Octoberfest7/TeamsPhisher
     cd /opt/tools/TeamsPhisher || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install msal colorama requests
     deactivate
     add-aliases teamsphisher
     add-history teamsphisher
     add-test-command "teamsphisher.py --help"
     add-to-list "TeamsPhisher,https://github.com/Octoberfest7/TeamsPhisher,TeamsPhisher is a Python3 program that facilitates the delivery of phishing messages and attachments to Microsoft Teams users whose organizations allow external communications."
 }
 
 function install_GPOddity() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing GPOddity"
-    pipx install git+https://github.com/synacktiv/GPOddity
+    pipx install --system-site-packages git+https://github.com/synacktiv/GPOddity
     add-history GPOddity
     add-test-command "gpoddity --help"
     add-to-list "GPOddity,https://github.com/synacktiv/GPOddity,Aiming at automating GPO attack vectors through NTLM relaying (and more)"
 }
 
 function install_netexec() {
     colorecho "Installing netexec"
     git -C /opt/tools/ clone --depth 1 https://github.com/Pennyw0rth/NetExec
-    pipx install /opt/tools/NetExec/
+    pipx install --system-site-packages /opt/tools/NetExec/
     mkdir -p ~/.nxc
     [[ -f ~/.nxc/nxc.conf ]] && mv ~/.nxc/nxc.conf ~/.nxc/nxc.conf.bak
     cp -v /root/sources/assets/netexec/nxc.conf ~/.nxc/nxc.conf
     cp -v /root/sources/assets/grc/conf.cme /usr/share/grc/conf.cme
     add-aliases netexec
     add-history netexec
     add-test-command "netexec --help"
     add-to-list "netexec,https://github.com/Pennyw0rth/NetExec,Network scanner (Crackmapexec updated)."
 }
 
 function install_extractbitlockerkeys() {
     colorecho "Installing ExtractBitlockerKeys"
     git -C /opt/tools/ clone --depth 1 https://github.com/p0dalirius/ExtractBitlockerKeys
     cd /opt/tools/ExtractBitlockerKeys || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases extractbitlockerkeys
     add-history extractbitlockerkeys
     add-test-command "ExtractBitlockerKeys.py|& grep 'usage: ExtractBitlockerKeys.py'"
     add-to-list "ExtractBitlockerKeys,https://github.com/p0dalirius/ExtractBitlockerKeys,A system administration or post-exploitation script to automatically extract the bitlocker recovery keys from a domain."
 }
 
 function install_LDAPWordlistHarvester() {
     colorecho "Installing LDAPWordlistHarvester"
     git -C /opt/tools/ clone --depth 1 https://github.com/p0dalirius/LDAPWordlistHarvester
     cd /opt/tools/LDAPWordlistHarvester || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases LDAPWordlistHarvester
     add-history LDAPWordlistHarvester
     add-test-command "LDAPWordlistHarvester.py --help"
     add-to-list "LDAPWordlistHarvester,https://github.com/p0dalirius/LDAPWordlistHarvester,Generate a wordlist from the information present in LDAP in order to crack passwords of domain accounts"
 }
 
 function install_pywerview() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing pywerview"
-    pipx install git+https://github.com/the-useless-one/pywerview
+    pipx install --system-site-packages git+https://github.com/the-useless-one/pywerview
     add-history pywerview
     add-test-command "pywerview --help"
     add-to-list "pywerview,https://github.com/the-useless-one/pywerview,A (partial) Python rewriting of PowerSploit's PowerView."
 }
 
 function install_freeipscanner() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -1263,50 +1260,113 @@
     add-test-command "freeipscanner.sh --help"
     add-to-list "freeipscanner,https://github.com/scrt/freeipscanner,A simple bash script to enumerate stale ADIDNS entries"
 }
 
 function install_scrtdnsdump() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing scrtdnsdump"
-    pipx install git+https://github.com/scrt/scrtdnsdump
+    pipx install --system-site-packages git+https://github.com/scrt/scrtdnsdump
     add-history scrtdnsdump
     add-test-command "scrtdnsdump --help"
     add-to-list "scrtdnsdump,https://github.com/scrt/scrtdnsdump,Enumeration and exporting of all DNS records in the zone for recon purposes of internal networks"
 }
 
 function install_ntlm_theft() {
     colorecho "Installing ntlm_theft"
     git -C /opt/tools/ clone --depth 1 https://github.com/Greenwolf/ntlm_theft
     cd /opt/tools/ntlm_theft || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install xlsxwriter
     deactivate
     add-aliases ntlm_theft
     add-history ntlm_theft
     add-test-command "ntlm_theft.py --help"
     add-to-list "ntlm_theft,https://github.com/Greenwolf/ntlm_theft,A tool for generating multiple types of NTLMv2 hash theft files"
 }
 
 function install_abuseACL() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing abuseACL"
-    pipx install git+https://github.com/AetherBlack/abuseACL
+    pipx install --system-site-packages git+https://github.com/AetherBlack/abuseACL
     add-history abuseACL
     add-test-command "abuseACL --help"
     add-to-list "abuseACL,https://github.com/AetherBlack/abuseACL,A python script to automatically list vulnerable Windows ACEs/ACLs."
 }
 
+function install_bloodyAD() {
+    # CODE-CHECK-WHITELIST=add-aliases
+    colorecho "Installing bloodyAD"
+    pipx install --system-site-packages git+https://github.com/CravateRouge/bloodyAD
+    add-history bloodyAD
+    add-test-command "bloodyAD --help"
+    add-to-list "bloodyAD,https://github.com/CravateRouge/bloodyAD,bloodyAD is an Active Directory privilege escalation swiss army knife."
+}
+
+function install_dploot() {
+    # CODE-CHECK-WHITELIST=add-aliases
+    colorecho "Installing dploot"
+    pipx install --system-site-packages git+https://github.com/zblurx/dploot
+    add-history dploot
+    add-test-command "dploot --help"
+    add-to-list "dploot,https://github.com/zblurx/dploot,dploot is Python rewrite of SharpDPAPI written un C#."
+}
+
+# function install_PXEThief() {
+#     # CODE-CHECK-WHITELIST=
+#     colorecho "Installing PXEThief"
+#     git -C /opt/tools/ clone --depth 1 https://github.com/MWR-CyberSec/PXEThief
+#     cd /opt/tools/PXEThief || exit
+#     python3 -m venv ./venv
+#     source ./venv/bin/activate
+# TODO: pywin32 not found
+#     pip3 install -r requirements.txt
+#     deactivate
+#     add-aliases PXEThief
+#     add-history PXEThief
+#     add-test-command "PXEThief --help"
+#     add-to-list "PXEThief,https://github.com/MWR-CyberSec/PXEThief,PXEThief is a toolset designed to exploit vulnerabilities in Microsoft Endpoint Configuration Manager's OS Deployment enabling credential theft from network and task sequence accounts."
+# }
+
+function install_sccmhunter() {
+    colorecho "Installing sccmhunter"
+    git -C /opt/tools/ clone --depth 1 https://github.com/garrettfoster13/sccmhunter
+    cd /opt/tools/sccmhunter || exit
+    python3 -m venv --system-site-packages ./venv
+    source ./venv/bin/activate
+    pip3 install -r requirements.txt
+    deactivate
+    add-aliases sccmhunter
+    add-history sccmhunter
+    add-test-command "sccmhunter.py --help"
+    add-to-list "sccmhunter,https://github.com/garrettfoster13/sccmhunter,SCCMHunter is a post-ex tool built to streamline identifying, profiling, and attacking SCCM related assets in an Active Directory domain."
+}
+
+function install_sccmwtf() {
+    # CODE-CHECK-WHITELIST=add-test-command
+    colorecho "Installing sccmwtf"
+    git -C /opt/tools/ clone --depth 1 https://github.com/xpn/sccmwtf
+    cd /opt/tools/sccmwtf || exit
+    python3 -m venv --system-site-packages ./venv
+    source ./venv/bin/activate
+    pip3 install -r requirements.txt
+    deactivate
+    add-aliases sccmwtf
+    add-history sccmwtf
+    add-to-list "sccmwtf,https://github.com/xpn/sccmwtf,This code is designed for exploring SCCM in a lab."
+}
+
 # Package dedicated to internal Active Directory tools
 function package_ad() {
     set_env
     local start_time
     local end_time
     start_time=$(date +%s)
     install_ad_apt_tools
+    install_pretender
     install_responder               # LLMNR, NBT-NS and MDNS poisoner
     install_ldapdomaindump
     install_crackmapexec            # Network scanner
     install_sprayhound              # Password spraying tool
     install_smartbrute              # Password spraying tool
     install_bloodhound-py           # ingestor for legacy BloodHound
     install_bloodhound-ce-py           # ingestor for legacy BloodHound
@@ -1388,11 +1448,16 @@
     install_LDAPWordlistHarvester
     install_pywerview
     install_freeipscanner
     # install_scrtdnsdump          # This tool is a fork of adidnsdump (https://github.com/dirkjanm/adidnsdump). We are currently waiting to see if a PR will be made.
     install_bloodhound-ce          # AD (Community Edition) security tool for reconnaissance and attacking AD environments
     install_ntlm_theft
     install_abuseACL
+    install_bloodyAD               # Active Directory privilege escalation swiss army knife.
+    install_dploot                 # Python rewrite of SharpDPAPI written un C#.
+    # install_PXEThief             # TODO: pywin32 not found - PXEThief is a toolset designed to exploit vulnerabilities in Microsoft Endpoint Configuration Manager's OS Deployment, enabling credential theft from network and task sequence accounts.
+    install_sccmhunter             # SCCMHunter is a post-ex tool built to streamline identifying, profiling, and attacking SCCM related assets in an Active Directory domain.
+    install_sccmwtf                # This code is designed for exploring SCCM in a lab.
     end_time=$(date +%s)
     local elapsed_time=$((end_time - start_time))
     colorecho "Package ad completed in $elapsed_time seconds."
 }
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_base.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_base.sh`

 * *Files 3% similar despite different names*

```diff
@@ -317,22 +317,41 @@
     elif [[ $(uname -m) = 'aarch64' ]]
     then
         local arch="aarch64"
     else
         criticalecho-noexit "This installation function doesn't support architecture $(uname -m)" && return
     fi
     local jdk_url
-    jdk_url=$(curl --location --silent "https://api.github.com/repos/adoptium/temurin11-binaries/releases/latest" | grep 'browser_download_url.*jdk_'"$arch"'_linux.*tar.gz"' | grep -o 'https://[^"]*')
+    jdk_url=$(curl --location --silent "https://api.github.com/repos/adoptium/temurin11-binaries/releases" | grep 'browser_download_url.*jdk_'"$arch"'_linux.*tar.gz"' | grep -o 'https://[^"]*' | sort | tail -n1)
     curl --location -o /tmp/openjdk11-jdk.tar.gz "$jdk_url"
     tar -xzf /tmp/openjdk11-jdk.tar.gz --directory /tmp
     mkdir -p "/usr/lib/jvm"
     mv /tmp/jdk-11* /usr/lib/jvm/java-11-openjdk
     add-test-command "/usr/lib/jvm/java-11-openjdk/bin/java --version"
 }
 
+function install_java21() {
+    # CODE-CHECK-WHITELIST=add-history,add-aliases,add-to-list
+    colorecho "Installing java 11"
+    if [[ $(uname -m) = 'x86_64' ]]
+    then
+        wget -O /tmp/openjdk21-jdk.tar.gz "https://download.java.net/java/GA/jdk21.0.2/f2283984656d49d69e91c558476027ac/13/GPL/openjdk-21.0.2_linux-x64_bin.tar.gz"
+
+    elif [[ $(uname -m) = 'aarch64' ]]
+    then
+        wget -O /tmp/openjdk21-jdk.tar.gz "https://download.java.net/java/GA/jdk21.0.2/f2283984656d49d69e91c558476027ac/13/GPL/openjdk-21.0.2_linux-aarch64_bin.tar.gz"
+    else
+        criticalecho-noexit "This installation function doesn't support architecture $(uname -m)" && return
+    fi
+    tar -xzf /tmp/openjdk21-jdk.tar.gz --directory /tmp
+    mkdir -p "/usr/lib/jvm"
+    mv /tmp/jdk-21* /usr/lib/jvm/java-21-openjdk
+    add-test-command "/usr/lib/jvm/java-21-openjdk/bin/java --version"
+}
+
 function add_debian_repository_components() {
     # add non-free non-free-firmware contrib repository
     # adding at the end of the line start with Components of the repository to add
     colorecho "add non-free non-free-firmware contrib repository"
     local source_file="/etc/apt/sources.list.d/debian.sources"
     local out_file="/etc/apt/sources.list.d/debian2.sources"
 
@@ -350,14 +369,16 @@
     # Function used to clean up post-install files
     colorecho "Cleaning..."
     local listening_processes
     updatedb
     rm -rfv /tmp/*
     rm -rfv /var/lib/apt/lists/*
     rm -rfv /root/sources
+    rm -rfv /root/.cache
+    rm -rfv /root/.gradle/caches
     colorecho "Stop listening processes"
     listening_processes=$(ss -lnpt | awk -F"," 'NR>1 {split($2,a,"="); print a[2]}')
     if [[ -n $listening_processes ]]; then
         echo "Listening processes detected"
         ss -lnpt
         echo "Kill processes"
         # shellcheck disable=SC2086
@@ -406,14 +427,15 @@
     less x11-apps net-tools vim nano jq iputils-ping iproute2 tidy mlocate libtool \
     dos2unix ftp sshpass telnet nfs-common ncat netcat-traditional socat rdate putty \
     screen p7zip-full p7zip-rar unrar xz-utils xsltproc parallel tree ruby ruby-dev ruby-full bundler \
     nim perl libwww-perl openjdk-17-jdk openvpn openresolv \
     logrotate tmux tldr bat libxml2-utils virtualenv chromium libsasl2-dev \
     libldap2-dev libssl-dev isc-dhcp-client sqlite3 dnsutils samba ssh snmp faketime php \
     python3 grc emacs-nox xsel xxd libnss3-tools
+    apt-mark hold tzdata  # Prevent apt upgrade error when timezone sharing is enable
 
     filesystem
     install_locales
     cp -v /root/sources/assets/shells/exegol_shells_rc /opt/.exegol_shells_rc
     cp -v /root/sources/assets/shells/bashrc ~/.bashrc
 
     install_asdf
@@ -454,14 +476,15 @@
 
     # Rust, Cargo, rvm
     install_rust_cargo
     install_rvm                                         # Ruby Version Manager
 
     # java11 install, and java17 as default
     install_java11
+    install_java21
     ln -s -v /usr/lib/jvm/java-17-openjdk-* /usr/lib/jvm/java-17-openjdk    # To avoid determining the correct path based on the architecture
     update-alternatives --set java /usr/lib/jvm/java-17-openjdk-*/bin/java  # Set the default openjdk version to 17
 
     install_go                                          # Golang language
     install_ohmyzsh                                     # Awesome shell
     install_fzf                                         # Fuzzy finder
     add-history curl
@@ -504,9 +527,15 @@
     # NVM (install in conctext)
     zsh -c "source ~/.zshrc && nvm install node && nvm use default"
 
     # Set Global config path to vendor
     # All programs using bundle will store their deps in vendor/
     bundle config path vendor/
 
-    # Remote Graphical Desktop installation
+    # OpenSSL activate legacy support
+    cat /root/sources/assets/patches/openssl.patch >> /etc/ssl/openssl.cnf
+    add-test-command "echo -n '1337' | openssl dgst -md4"
+    add-test-command "python3 -c 'import hashlib;print(hashlib.new(\"md4\", \"1337\".encode()).digest())'"
+
+    # Global python dependencies
+    pip3 install -r /root/sources/assets/python/requirements.txt
 }
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_c2.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_c2.sh`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 source common.sh
 # sourcing package_ad.sh for the install_powershell() function
 source package_ad.sh
 
 function install_pwncat() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing pwncat"
-    pipx install pwncat-cs
+    pipx install --system-site-packages pwncat-cs
     # Because Blowfish has been deprecated, downgrade cryptography version - https://github.com/paramiko/paramiko/issues/2038
     pipx inject pwncat-cs cryptography==36.0.2
     add-history pwncat
     add-test-command "pwncat-cs --version"
     add-to-list "pwncat,https://github.com/calebstewart/pwncat,A lightweight and versatile netcat alternative that includes various additional features."
 }
 
@@ -23,31 +23,40 @@
     git -C /opt/tools clone --depth 1 https://github.com/rapid7/metasploit-framework.git
     cd /opt/tools/metasploit-framework || exit
     rvm use 3.2.2@metasploit --create
     gem install bundler
     bundle install
     # fixes 'You have already activated timeout 0.3.1, but your Gemfile requires timeout 0.4.0. Since timeout is a default gem, you can either remove your dependency on it or try updating to a newer version of bundler that supports timeout as a default gem.'
     # fixes 'You have already activated timeout 0.4.1, but your Gemfile requires timeout 0.4.0. Prepending `bundle exec` to your command may solve this.'
-    local temp_fix_limit="2024-02-25"
+    local temp_fix_limit="2024-04-25"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       gem install timeout --version 0.4.0
     fi
     rvm use 3.2.2@default
+
+    # msfdb setup
+    fapt postgresql
+    cp -r /root/.bundle /var/lib/postgresql
+    chown -R postgres:postgres /var/lib/postgresql/.bundle
+    sudo -u postgres sh -c "git config --global --add safe.directory /opt/tools/metasploit-framework && cd /opt/tools/metasploit-framework && /usr/local/rvm/gems/ruby-3.2.2@metasploit/wrappers/bundle exec /opt/tools/metasploit-framework/msfdb init"
+    cp -r /var/lib/postgresql/.msf4 /root
+
     add-aliases metasploit
     add-test-command "msfconsole --help"
+    add-test-command "msfdb --help"
     add-test-command "msfvenom --list platforms"
     add-to-list "metasploit,https://github.com/rapid7/metasploit-framework,A popular penetration testing framework that includes many exploits and payloads"
 }
 
 function install_routersploit() {
     # CODE-CHECK-WHITELIST=add-history
     colorecho "Installing RouterSploit"
-    pipx install routersploit
+    pipx install --system-site-packages routersploit
     pipx inject routersploit colorama
     add-aliases routersploit
     add-test-command "routersploit --help"
     add-to-list "routersploit,https://github.com/threat9/routersploit,Security audit tool for routers."
 }
 
 function install_sliver() {
@@ -57,15 +66,15 @@
     git -C /opt/tools/ clone https://github.com/BishopFox/sliver.git
     cd /opt/tools/sliver || exit
     asdf local golang 1.19
     # making the static version checkout a temporary thing
     # function below will serve as a reminder to update sliver's version regularly
     # when the pipeline fails because the time limit is reached: update the version and the time limit
     # or check if it's possible to make this dynamic
-    local temp_fix_limit="2024-02-25"
+    local temp_fix_limit="2024-04-25"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       git checkout tags/v1.5.41
     fi
     make
     ln -s /opt/tools/sliver/sliver-server /opt/tools/bin/sliver-server
@@ -84,15 +93,15 @@
     # Installing .NET 6.0 SDK
     wget -O /tmp/dotnet-install.sh https://dot.net/v1/dotnet-install.sh
     chmod +x /tmp/dotnet-install.sh
     /tmp/dotnet-install.sh --channel 6.0
     install_powershell
     git -C /opt/tools/ clone --recursive https://github.com/BC-SECURITY/Empire
     cd /opt/tools/Empire || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     if [[ $(uname -m) = 'x86_64' ]]
     then
       pip3 install .
     elif [[ $(uname -m) = 'aarch64' ]]
     then
       # for ARM64, pip install doesn't work because of donut-shellcode not supporting this arch (https://github.com/TheWover/donut/issues/139)
@@ -136,15 +145,15 @@
     add-to-list "Havoc,https://github.com/HavocFramework/Havoc,Command & Control Framework"
 }
 
 function install_villain() {
     colorecho "Installing Villain"
     git -C /opt/tools/ clone --depth 1 https://github.com/t3l3machus/Villain
     cd /opt/tools/Villain || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r ./requirements.txt
     deactivate
     add-aliases villain
     add-history villain
     add-test-command "Villain.py -h"
     add-to-list "Villain,https://github.com/t3l3machus/Villain,Command & Control Framework"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_cloud.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_cloud.sh`

 * *Files 4% similar despite different names*

```diff
@@ -49,24 +49,24 @@
     add-test-command "aws --version"
     add-to-list "awscli,https://aws.amazon.com/cli/,Command-line interface for Amazon Web Services."
 }
 
 function install_scout() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing ScoutSuite"
-    pipx install scoutsuite
+    pipx install --system-site-packages scoutsuite
     add-history scout
     add-test-command "scout --help"
     add-to-list "scout,https://github.com/nccgroup/ScoutSuite,Scout Suite is an open source multi-cloud security-auditing tool which enables security posture assessment of cloud environments."
 }
 
 function install_cloudsplaining() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Cloudsplaining"
-    pipx install cloudsplaining
+    pipx install --system-site-packages cloudsplaining
     add-history cloudsplaining
     add-test-command "cloudsplaining --help"
     add-to-list "cloudsplaining,https://github.com/salesforce/cloudsplaining,AWS IAM Security Assessment tool that identifies violations of least privilege and generates a risk-prioritized report."
 }
 
 function install_cloudsploit() {
     colorecho "Installing Cloudsploit"
@@ -77,27 +77,27 @@
     add-test-command "cloudsploit -h"
     add-to-list "cloudsploit,https://github.com/aquasecurity/cloudsploit,Cloud Security Posture Management"
 }
 
 function install_prowler() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Prowler"
-    pipx install prowler
+    pipx install --system-site-packages prowler
     add-history prowler
     add-test-command "prowler -h"
     add-to-list "prowler,https://github.com/prowler-cloud/prowler,Perform Cloud Security best practices assessments / audits / incident response / compliance / continuous monitoring / hardening and forensics readiness."
 }
 
 function install_cloudmapper() {
     colorecho "Installing Cloudmapper"
     git -C /opt/tools clone --depth 1 https://github.com/duo-labs/cloudmapper.git 
     cd /opt/tools/cloudmapper || exit
     cp -v /root/sources/assets/patches/cloudmapper.patch cloudmapper.patch
     git apply --verbose cloudmapper.patch
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install wheel
     pip3 install -r requirements.txt
     deactivate
     add-aliases cloudmapper
     add-history cloudmapper
     add-test-command 'cloudmapper.py --help |& grep "usage"'
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_code_analysis.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_code_analysis.sh`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     add-test-command "brakeman --help"
     add-to-list "brakeman,https://github.com/presidentbeef/brakeman,Static analysis tool for Ruby on Rails applications"
 }
 
 function install_semgrep() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing semgrep"
-    pipx install semgrep
+    pipx install --system-site-packages semgrep
     add-history semgrep
     add-test-command "semgrep --help"
     add-to-list "semgrep,https://github.com/returntocorp/semgrep/,Static analysis tool that supports multiple languages and can find a variety of vulnerabilities and coding errors."
 }
 
 function install_pp-finder() {
     # CODE-CHECK-WHITELIST=add-aliases
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_cracking.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_cracking.sh`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     add-test-command "7z2john.pl|& grep 'Usage'"
     add-to-list "john,https://github.com/openwall/john,John the Ripper password cracker."
 }
 
 function install_name-that-hash() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Name-That-Hash"
-    pipx install name-that-hash
+    pipx install --system-site-packages name-that-hash
     add-history name-that-hash
     add-test-command "nth --help"
     add-to-list "name-that-hash,https://github.com/HashPals/Name-That-Hash,Online tool for identifying hashes."
 }
 
 function install_haiti() {
     colorecho "Installing haiti"
@@ -56,15 +56,15 @@
     add-test-command "haiti --help"
     add-to-list "haiti,https://github.com/noraj/haiti,haiti is a A CLI tool (and library) to identify hash types (hash type identifier)."
 }
 
 function install_geowordlists() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing GeoWordlists"
-    pipx install git+https://github.com/p0dalirius/GeoWordlists
+    pipx install --system-site-packages git+https://github.com/p0dalirius/GeoWordlists
     add-history geowordlists
     add-test-command "geowordlists --help"
     add-to-list "geowordlists,https://github.com/p0dalirius/GeoWordlists,tool to generate wordlists of passwords containing cities at a defined distance around the client city."
 }
 
 function install_pkcrack() {
     # CODE-CHECK-WHITELIST=add-aliases
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_crypto.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_crypto.sh`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 function install_rsactftool() {
     colorecho "Installing Rsactftool"
     # This tool uses z3solver, which is very long to build (5 min)
     fapt libmpc-dev
     git -C /opt/tools clone --depth 1 https://github.com/RsaCtfTool/RsaCtfTool
     cd /opt/tools/RsaCtfTool || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases rsactftool
     add-history rsactftool
     add-test-command "RsaCtfTool.py --help"
     add-to-list "rsactftool,https://github.com/RsaCtfTool/RsaCtfTool,The rsactftool tool is used for RSA cryptographic operations and analysis."
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_desktop.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_desktop.sh`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     mv 'Prof--XFCE- 2.1' Prof_XFCE_2_1
     cp -r ./Prof_XFCE_2_1 /root/.themes/
     rm -rf /tmp/Prof*
 
     # Dock
     fapt xfce4-dev-tools libglib2.0-dev libgtk-3-dev libwnck-3-dev libxfce4ui-2-dev libxfce4panel-2.0-dev g++ build-essential
     git -C /tmp clone https://gitlab.xfce.org/panel-plugins/xfce4-docklike-plugin.git
+    git -C /tmp/xfce4-docklike-plugin checkout xfce4-docklike-plugin-0.4.2
     cd /tmp/xfce4-docklike-plugin
     sh autogen.sh --prefix=/tmp/
     make
     make install
     CUSTOM_PATH=$(find /usr/lib/ -name "xfce*"|head -n1)
     mv -v /tmp/lib/xfce4/panel/plugins/libdocklike.* "$CUSTOM_PATH/panel/plugins"
     mv -v /tmp/share/xfce4/panel/plugins/docklike.desktop /usr/share/xfce4/panel/plugins
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_forensic.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_forensic.sh`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,18 @@
     add-test-command "volatility2 --help"
     add-to-list "volatility2,https://github.com/volatilityfoundation/volatility,Volatile memory extraction utility framework"
 }
 
 function install_volatility3() {
     colorecho "Installing volatility3"
     git -C /opt/tools/ clone --depth 1 https://github.com/volatilityfoundation/volatility3
-    pipx install /opt/tools/volatility3
+    pipx install --system-site-packages /opt/tools/volatility3
     # volatility's setup.py installs requirements from requirements-minimal.txt. Some reqs from requirements.txt are missing, injecting now
-    pipx inject volatility3 yara-python capstone pycryptodome
+    # pipx doesn't support injection of a requirements file : https://github.com/pypa/pipx/issues/934
+    sed -e '/^#/d' -e '/^-r requirements-minimal.txt/d' /opt/tools/volatility3/requirements.txt | xargs pipx inject volatility3
     add-aliases volatility3
     add-history volatility3
     add-test-command "volatility3 --help"
     add-to-list "volatility3,https://github.com/volatilityfoundation/volatility3,Advanced memory forensics framework"
 }
 
 function install_trid() {
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_iot.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_iot.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_misc.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_misc.sh`

 * *Files 6% similar despite different names*

```diff
@@ -30,42 +30,42 @@
     add-test-command "goshs -v"
     add-to-list "goshs,https://github.com/patrickhener/goshs,Goshs is a replacement for Python's SimpleHTTPServer. It allows uploading and downloading via HTTP/S with either self-signed certificate or user provided certificate and you can use HTTP basic auth."
 }
 
 function install_shellerator() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing shellerator"
-    pipx install git+https://github.com/ShutdownRepo/shellerator
+    pipx install --system-site-packages git+https://github.com/ShutdownRepo/shellerator
     add-history shellerator
     add-test-command "shellerator --help"
     add-to-list "shellerator,https://github.com/ShutdownRepo/Shellerator,a simple command-line tool for generating shellcode"
 }
 
 function install_uberfile() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing uberfile"
-    pipx install git+https://github.com/ShutdownRepo/uberfile
+    pipx install --system-site-packages git+https://github.com/ShutdownRepo/uberfile
     add-history uberfile
     add-test-command "uberfile --help"
     add-to-list "uberfile,https://github.com/ShutdownRepo/Uberfile,Uberfile is a simple command-line tool aimed to help pentesters quickly generate file downloader one-liners in multiple contexts (wget / curl / powershell / certutil...). This project code is based on my other similar project for one-liner reverseshell generation Shellerator."
 }
 
 function install_arsenal() {
     colorecho "Installing arsenal"
-    pipx install git+https://github.com/Orange-Cyberdefense/arsenal
+    pipx install --system-site-packages git+https://github.com/Orange-Cyberdefense/arsenal
     add-aliases arsenal
     add-history arsenal
     add-test-command "arsenal --version"
     add-to-list "arsenal,https://github.com/Orange-Cyberdefense/arsenal,Powerful weapons for penetration testing."
 }
 
 function install_whatportis() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing whatportis"
-    pipx install whatportis
+    pipx install --system-site-packages whatportis
     # TODO : FIX : "port": port[1] if port[1] else "---",list index out of range - cli.py
     # echo y | whatportis --update
     add-history whatportis
     add-test-command "whatportis --version"
     add-to-list "whatportis,https://github.com/ncrocfer/whatportis,Command-line tool to lookup port information"
 }
 
@@ -127,15 +127,15 @@
     add-test-command "ngrok version"
     add-to-list "ngrok,https://github.com/inconshreveable/ngrok,Expose a local server behind a NAT or firewall to the internet"
 }
 
 function install_objectwalker() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing objectwalker"
-    pipx install git+https://github.com/p0dalirius/objectwalker
+    pipx install --system-site-packages git+https://github.com/p0dalirius/objectwalker
     add-history objectwalker
     add-test-command "objectwalker --help"
     add-to-list "objectwalker,https://github.com/p0dalirius/objectwalker,A python module to explore the object tree to extract paths to interesting objects in memory."
 }
 
 function install_tig() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
@@ -149,32 +149,33 @@
     add-test-command "tig --help"
     add-to-list "tig,https://github.com/jonas/tig,Tig is an ncurses-based text-mode interface for git."
 }
 
 function install_yt-dlp() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
     colorecho "Installing yt-dlp"
-    pipx install git+https://github.com/yt-dlp/yt-dlp
+    pipx install --system-site-packages git+https://github.com/yt-dlp/yt-dlp
     add-test-command "yt-dlp --help"
     add-to-list "yt-dlp,https://github.com/yt-dlp/yt-dlp,A youtube-dl fork with additional features and fixes"
 }
 
 function install_cyberchef() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
     colorecho "Installing CyberChef"
-    local last_version
-    last_version=$(git ls-remote --tags --sort='v:refname' https://github.com/gchq/CyberChef.git | tail -n 1 | cut -d '/' -f 3 | cut -d '^' -f 1)
-    if [[ -z "$last_version" ]]; then
-        criticalecho-noexit "Latest version not found" && return
+    local last_release
+    last_release=$(curl --location --silent "https://api.github.com/repos/gchq/CyberChef/releases/latest"|grep browser_download_url|awk '{print $2}'|tr -d '"')
+    echo "$last_release"
+    if [[ -z "$last_release" ]]; then
+        criticalecho-noexit "Latest release not found" && return
     fi
     mkdir /opt/tools/CyberChef
-    wget https://github.com/gchq/CyberChef/releases/download/"$last_version"/CyberChef_"$last_version".zip -O /tmp/CyberChef.zip
+    wget "$last_release" -O /tmp/CyberChef.zip
     unzip -o /tmp/CyberChef.zip -d /opt/tools/CyberChef/
     rm /tmp/CyberChef.zip
-    mv /opt/tools/CyberChef/CyberChef_"$last_version".html /opt/tools/CyberChef/CyberChef.html
+    mv /opt/tools/CyberChef/CyberChef_*.html /opt/tools/CyberChef/CyberChef.html
     add-test-command "file /opt/tools/CyberChef/CyberChef.html"
     add-to-list "CyberChef,https://github.com/gchq/CyberChef/,The Cyber Swiss Army Knife"
 }
 
 # Package dedicated to offensive miscellaneous tools
 function package_misc() {
     set_env
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_mobile.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_mobile.sh`

 * *Files 6% similar despite different names*

```diff
@@ -64,51 +64,61 @@
     add-test-command "d2j-dex2jar.sh --help"
     add-to-list "dex2jar,https://github.com/pxb1988/dex2jar,A tool to convert Android's dex files to Java's jar files"
 }
 
 function install_frida() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing frida"
-    pipx install frida-tools
+    pipx install --system-site-packages frida-tools
     add-history frida
     add-test-command "frida --version"
     add-to-list "frida,https://github.com/frida/frida,Dynamic instrumentation toolkit"
 }
 
 function install_objection() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing objection"
-    pipx install git+https://github.com/sensepost/objection
+    pipx install --system-site-packages git+https://github.com/sensepost/objection
     add-history objection
     add-test-command "objection --help"
     add-to-list "objection,https://github.com/sensepost/objection,Runtime mobile exploration"
 }
 
 function install_androguard() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing androguard"
-    pipx install androguard
-    add-history androguard
-    add-test-command "androguard --version"
-    add-to-list "androguard,https://github.com/androguard/androguard,Reverse engineering and analysis of Android applications"
+    # androguard not installing on ARM64 (https://github.com/androguard/androguard/issues/1027), skipping temporarily
+    local temp_fix_limit="2024-05-20"
+    if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
+      criticalecho "Temp fix expired. Exiting." # check if issue was resolved by androguard team
+    fi
+    if [[ $(uname -m) = 'x86_64' ]]
+    then
+        pipx install --system-site-packages androguard
+        add-history androguard
+        add-test-command "androguard --version"
+        add-to-list "androguard,https://github.com/androguard/androguard,Reverse engineering and analysis of Android applications"
+    else
+        criticalecho-noexit "This installation function doesn't support architecture $(uname -m)" && return
+    fi
 }
 
 function install_mobsf(){
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Mobile Security Framework"
     fapt wkhtmltopdf
     git -C /opt/tools clone --depth 1 https://github.com/MobSF/Mobile-Security-Framework-MobSF MobSF
     cd /opt/tools/MobSF || exit
     # pipx --preinstall git+https://github.com/MobSF/yara-python-dex.git /opt/tools/MobSF would be needed for ARM64
     #  in the mean time, switching to manual venv and an alias for mobsf
-    local temp_fix_limit="2024-02-01"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting." # check if pipx supports preinstall now
     else
-      python3 -m venv ./venv
+      python3 -m venv --system-site-packages ./venv
       ./venv/bin/python3 -m pip install git+https://github.com/MobSF/yara-python-dex.git
       ./venv/bin/python3 -m pip install .
       add-aliases mobsf # alias is only needed with venv and can be removed when switching back to pipx
     fi
     add-history mobsf
     add-test-command "/opt/tools/MobSF/venv/bin/python -c 'from mobsf.MobSF.settings import VERSION; print(VERSION)'"
     add-to-list "mobsf,https://github.com/MobSF/Mobile-Security-Framework-MobSF,Automated and all-in-one mobile application (Android/iOS/Windows) pen-testing malware analysis and security assessment framework"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_most_used.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_most_used.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_network.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_network.sh`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 source common.sh
 
 function install_network_apt_tools() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing network apt tools"
     export DEBIAN_FRONTEND=noninteractive
     fapt wireshark tshark hping3 masscan netdiscover tcpdump iptables traceroute dns2tcp freerdp2-x11 \
-    rdesktop xtightvncviewer ssh-audit hydra mariadb-client redis-tools
+    rdesktop xtightvncviewer hydra mariadb-client redis-tools
     fapt remmina remmina-plugin-rdp remmina-plugin-secret
     # remmina-plugin-spice need build ?
     # https://gitlab.com/Remmina/Remmina/-/wikis/Compilation/Compile-on-Debian-10-Buster
 
     add-history wireshark
     add-history tshark
     add-history hping3
@@ -33,15 +33,14 @@
     add-test-command "tcpdump --version"                            # Capture TCP traffic
     add-test-command "iptables --version"                           # iptables for the win
     add-test-command "traceroute --help"                            # ping ping
     add-test-command "dns2tcpc|& grep 'Usage : dns2tcpc'"           # TCP tunnel over DNS
     add-test-command "which xfreerdp"
     add-test-command "rdesktop|& grep 'Usage: rdesktop'"
     add-test-command "which xtightvncviewer"
-    add-test-command "ssh-audit --help |& grep 'verbose output'"    # SSH server audit
     add-test-command "hydra -h |& grep 'more command line options'" # Login scanner
     add-test-command "mariadb --version"                            # Mariadb client
     add-test-command "redis-cli --version"                          # Redis protocol
     add-test-command "remmina --help"                          # Redis protocol
 
     add-to-list "wireshark,https://github.com/wireshark/wireshark,Wireshark is a network protocol analyzer that lets you see what’s happening on your network at a microscopic level."
     add-to-list "tshark,https://github.com/wireshark/wireshark,TShark is a terminal version of Wireshark."
@@ -51,15 +50,14 @@
     add-to-list "tcpdump,https://github.com/the-tcpdump-group/tcpdump,a powerful command-line packet analyzer for Unix-like systems"
     add-to-list "iptables,https://linux.die.net/man/8/iptables,Userspace command line tool for configuring kernel firewall"
     add-to-list "traceroute,https://github.com/iputils/iputils,Traceroute is a command which can show you the path a packet of information takes from your computer to one you specify."
     add-to-list "dns2tcp,https://github.com/alex-sector/dns2tcp,dns2tcp is a tool for relaying TCP connections over DNS."
     add-to-list "freerdp2-x11,https://github.com/FreeRDP/FreeRDP,FreeRDP is a free implementation of the Remote Desktop Protocol (RDP) released under the Apache license."
     add-to-list "rdesktop,https://github.com/rdesktop/rdesktop,rdesktop is a client for Remote Desktop Protocol (RDP) used in a number of Microsoft products including Windows NT Terminal Server / Windows 2000 Server / Windows XP and Windows 2003 Server."
     add-to-list "xtightvncviewer,https://www.commandlinux.com/man-page/man1/xtightvncviewer.1.html,xtightvncviewer is an open source VNC client software."
-    add-to-list "ssh-audit,https://github.com/arthepsy/ssh-audit,ssh-audit is a tool to test SSH server configuration for best practices."
     add-to-list "hydra,https://github.com/vanhauser-thc/thc-hydra,Hydra is a parallelized login cracker which supports numerous protocols to attack."
     add-to-list "mariadb-client,https://github.com/MariaDB/server,MariaDB is a community-developed fork of the MySQL relational database management system. The mariadb-client package includes command-line utilities for interacting with a MariaDB server."
     add-to-list "redis-tools,https://github.com/antirez/redis-tools,redis-tools is a collection of Redis client utilities including redis-cli and redis-benchmark."
     add-to-list "remmina,https://github.com/FreeRDP/Remmina,Remote desktop client."
 }
 
 function install_proxychains() {
@@ -108,40 +106,40 @@
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing autorecon"
     git -C /opt/tools/ clone --depth 1 https://gitlab.com/kalilinux/packages/oscanner.git
     ln -sv /opt/tools/oscanner/debian/helper-script/oscanner /usr/bin/oscanner
     git -C /opt/tools clone --depth 1 https://gitlab.com/kalilinux/packages/tnscmd10g.git
     ln -sv /opt/tools/tnscmd10g/tnscmd10g /usr/bin/tnscmd10g
     fapt dnsrecon wkhtmltopdf
-    pipx install git+https://github.com/Tib3rius/AutoRecon
+    pipx install --system-site-packages git+https://github.com/Tib3rius/AutoRecon
     add-history autorecon
     # test below cannot work because test runner cannot have a valid display
     # add-test-command "autorecon --version"
     add-test-command "which autorecon"
     add-to-list "autorecon,https://github.com/Tib3rius/AutoRecon,Multi-threaded network reconnaissance tool which performs automated enumeration of services."
 }
 
 function install_dnschef() {
     colorecho "Installing DNSChef"
     git -C /opt/tools/ clone --depth 1 https://github.com/iphelix/dnschef
     cd /opt/tools/dnschef || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases dnschef
     add-history dnschef
     add-test-command "dnschef.py --help"
     add-to-list "dnschef,https://github.com/iphelix/dnschef,Tool for DNS MITM attacks"
 }
 
 function install_divideandscan() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing DivideAndScan"
-    pipx install git+https://github.com/snovvcrash/DivideAndScan
+    pipx install --system-site-packages git+https://github.com/snovvcrash/DivideAndScan
     add-history divideandscan
     add-test-command "divideandscan --help"
     add-to-list "divideandscan,https://github.com/snovvcrash/divideandscan,Advanced subdomain scanner"
 }
 
 function install_chisel() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -153,39 +151,39 @@
     add-test-command "chisel --help"
     add-to-list "chisel,https://github.com/jpillora/chisel,Go based TCP tunnel with authentication and encryption support"
 }
 
 function install_sshuttle() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing sshtuttle"
-    pipx install git+https://github.com/sshuttle/sshuttle.git
+    pipx install --system-site-packages git+https://github.com/sshuttle/sshuttle.git
     add-history sshuttle
     add-test-command "sshuttle --version"
     add-to-list "sshuttle,https://github.com/sshuttle/sshuttle,Transparent proxy server that tunnels traffic through an SSH server"
 }
 
 function install_eaphammer() {
     colorecho "Installing eaphammer"
     git -C /opt/tools clone --depth 1 https://github.com/s0lst1c3/eaphammer.git
     cd /opt/tools/eaphammer || exit
     xargs apt install -y < kali-dependencies.txt
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r pip.req
     deactivate
     add-aliases eaphammer
     add-history eaphammer
     add-test-command "eaphammer -h"
     add-to-list "eaphammer,https://github.com/s0lst1c3/eaphammer,EAPHammer is a toolkit for performing targeted evil twin attacks against WPA2-Enterprise networks."
 }
 
 function install_fierce() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing fierce"
-    pipx install git+https://github.com/mschwager/fierce
+    pipx install --system-site-packages git+https://github.com/mschwager/fierce
     add-history fierce
     add-test-command "fierce --help"
     add-to-list "fierce,https://github.com/mschwager/fierce,A DNS reconnaissance tool for locating non-contiguous IP space"
 }
 
 function install_dnsx() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -262,14 +260,23 @@
     rm -rf target/release/{deps,build,.fingerprint}
     ln -s /opt/tools/legba/target/release/legba /opt/tools/bin/legba
     add-history legba
     add-test-command "legba --help"
     add-to-list "legba,https://github.com/evilsocket/legba,a multiprotocol credentials bruteforcer / password sprayer and enumerator built with Rust"
 }
 
+function install_ssh-audit() {
+    # CODE-CHECK-WHITELIST=add-aliases
+    colorecho "Installing ssh-audit"
+    pipx install --system-site-packages git+https://github.com/jtesta/ssh-audit
+    add-history ssh-audit
+    add-test-command "ssh-audit --help"
+    add-to-list "ssh-audit,https://github.com/jtesta/ssh-audit,ssh-audit is a tool to test SSH server configuration for best practices."
+}
+
 # Package dedicated to network pentest tools
 function package_network() {
     set_env
     local start_time
     local end_time
     start_time=$(date +%s)
     install_network_apt_tools
@@ -286,11 +293,12 @@
     # install_odat                  # Oracle Database Attacking Tool, FIXME
     install_dnsx                    # Fast and multi-purpose DNS toolkit
     install_shuffledns              # Wrapper around massdns to enumerate valid subdomains
     install_tailscale               # Zero config VPN for building secure networks
     install_ligolo-ng               # Tunneling tool that uses a TUN interface
     install_rustscan
     install_legba                   # Login Scanner
+    install_ssh-audit               # SSH server audit
     end_time=$(date +%s)
     local elapsed_time=$((end_time - start_time))
     colorecho "Package network completed in $elapsed_time seconds."
 }
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_osint.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_osint.sh`

 * *Files 10% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     add-to-list "whois,https://packages.debian.org/sid/whois,See information about a specific domain name or IP address."
     add-to-list "recon-ng,https://github.com/lanmaster53/recon-ng,External recon tool."
 }
 
 function install_youtubedl() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing youtube-dl"
-    pipx install youtube-dl
+    pipx install --system-site-packages youtube-dl
     add-history youtube-dl
     add-test-command "youtube-dl --version"
     add-to-list "youtubedl,https://github.com/ytdl-org/youtube-dl,Download videos from YouTube and other sites."
 }
 
 function install_sublist3r() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Sublist3r"
-    pipx install git+https://github.com/aboul3la/Sublist3r
+    pipx install --system-site-packages git+https://github.com/aboul3la/Sublist3r
     add-history sublist3r
     add-test-command "sublist3r --help"
     add-to-list "sublist3r,https://github.com/aboul3la/Sublist3r,a Python tool designed to enumerate subdomains of websites."
 }
 
 function install_assetfinder() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -91,15 +91,15 @@
     add-test-command "findomain --version"
     add-to-list "findomain,https://github.com/findomain/findomain,The fastest and cross-platform subdomain enumerator."
 }
 
 function install_holehe() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing holehe"
-    pipx install holehe
+    pipx install --system-site-packages holehe
     add-history holehe
     add-test-command "holehe --help"
     add-to-list "holehe,https://github.com/megadose/holehe,mail osint tool finding out if it is used on websites."
 }
 
 function install_simplyemail() {
     colorecho "Installing SimplyEmail"
@@ -116,30 +116,30 @@
     add-to-list "simplyemail,https://github.com/SimplySecurity/SimplyEmail,a scriptable command line tool for sending emails"
 }
 
 function install_theharvester() {
     colorecho "Installing theHarvester"
     git -C /opt/tools/ clone --depth 1 https://github.com/laramies/theHarvester
     cd /opt/tools/theHarvester || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     # The tool needs access to the proxies.yaml file in the folder.
     ln -s /opt/tools/theHarvester /usr/local/etc/
     add-aliases theharvester
     add-history theharvester
     add-test-command "theHarvester.py --help"
     add-to-list "theharvester,https://github.com/laramies/theHarvester,Tool for gathering e-mail accounts / subdomain names / virtual host / open ports / banners / and employee names from different public sources"
 }
 
 function install_h8mail() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing h8mail"
-    pipx install h8mail
+    pipx install --system-site-packages h8mail
     add-history h8mail
     add-test-command "h8mail --help"
     add-to-list "h8mail,https://github.com/khast3x/h8mail,Email OSINT and breach hunting."
 }
 
 function install_infoga() {
     colorecho "Installing infoga"
@@ -158,30 +158,31 @@
 
 function install_buster() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing buster"
     git -C /opt/tools clone --depth 1 https://github.com/sham00n/buster
     cd /opt/tools/buster || exit
     fapt libxml2-dev libxslt-dev
-    python3.6 -m venv ./venv
+    python3.6 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
-    python3.6 -m pip install cython cchardet requests beautifulsoup4 PyYaml lxml grequests gevent twint
+    # setting static lxml version since buster doesn't support latest one
+    python3.6 -m pip install cython cchardet requests beautifulsoup4 PyYaml lxml==5.1.1 grequests gevent twint
     python3.6 setup.py install
     deactivate
     ln -s /opt/tools/buster/venv/bin/buster /opt/tools/bin
     add-history buster
     add-test-command "buster --help"
     add-to-list "buster,https://github.com/sham00n/Buster,Advanced OSINT tool"
 }
 
 function install_pwnedornot() {
     colorecho "Installing pwnedornot"
     git -C /opt/tools/ clone --depth 1 https://github.com/thewhiteh4t/pwnedOrNot
     cd /opt/tools/pwnedOrNot || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install requests html2text
     deactivate
     mkdir -p "$HOME/.config/pwnedornot"
     cp config.json "$HOME/.config/pwnedornot/config.json"
     add-aliases pwnedornot
     add-history pwnedornot
@@ -207,38 +208,38 @@
     add-test-command "phoneinfoga help"
     add-to-list "phoneinfoga,https://github.com/sundowndev/PhoneInfoga,Information gathering & OSINT framework for phone numbers."
 }
 
 function install_maigret() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing maigret"
-    pipx install git+https://github.com/soxoj/maigret.git
+    pipx install --system-site-packages git+https://github.com/soxoj/maigret.git
     add-history maigret
     add-test-command "maigret --help"
     add-to-list "maigret,https://github.com/soxoj/maigret,Collects information about a target email (or domain) from Google and Bing search results"
 }
 
 function install_linkedin2username() {
     colorecho "Installing linkedin2username"
     git -C /opt/tools/ clone --depth 1 https://github.com/initstring/linkedin2username
     cd /opt/tools/linkedin2username || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases linkedin2username
     add-history linkedin2username
     add-test-command "linkedin2username.py --help"
     add-to-list "linkedin2username,https://github.com/initstring/linkedin2username,Generate a list of LinkedIn usernames from a company name."
 }
 
 function install_toutatis() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing toutatis"
-    pipx install git+https://github.com/megadose/toutatis
+    pipx install --system-site-packages git+https://github.com/megadose/toutatis
     add-history toutatis
     add-test-command "toutatis --help"
     add-to-list "toutatis,https://github.com/megadose/Toutatis,Toutatis is a tool that allows you to extract information from instagrams accounts such as e-mails / phone numbers and more."
 }
 
 function install_waybackurls() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -250,29 +251,29 @@
     add-to-list "waybackurls,https://github.com/tomnomnom/waybackurls,Fetch all the URLs that the Wayback Machine knows about for a domain."
 }
 
 function install_carbon14() {
     colorecho "Installing Carbon14"
     git -C /opt/tools/ clone --depth 1 https://github.com/Lazza/Carbon14
     cd /opt/tools/Carbon14 || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases carbon14
     add-history carbon14
     add-test-command "carbon14.py --help"
     add-to-list "carbon14,https://github.com/Lazza/carbon14,OSINT tool for estimating when a web page was written."
 }
 
 function install_photon() {
     colorecho "Installing photon"
     git -C /opt/tools/ clone --depth 1 https://github.com/s0md3v/photon
     cd /opt/tools/photon || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases photon
     add-history photon
     add-test-command "photon.py --help"
     add-to-list "photon,https://github.com/s0md3v/Photon,a fast web crawler which extracts URLs / files / intel & endpoints from a target."
@@ -316,55 +317,55 @@
     add-to-list "maltego,https://www.paterva.com/web7/downloads.php,A tool used for open-source intelligence and forensics"
 }
 
 function install_spiderfoot() {
     colorecho "Installing Spiderfoot"
     git -C /opt/tools/ clone --depth 1 https://github.com/smicallef/spiderfoot
     cd /opt/tools/spiderfoot || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases spiderfoot
     add-history spiderfoot
     add-test-command "spiderfoot --help"
     add-test-command "spiderfoot-cli --help"
     add-to-list "spiderfoot,https://github.com/smicallef/spiderfoot,A reconnaissance tool that automatically queries over 100 public data sources"
 }
 
 function install_finalrecon() {
     colorecho "Installing FinalRecon"
     git -C /opt/tools/ clone --depth 1 https://github.com/thewhiteh4t/FinalRecon
     cd /opt/tools/FinalRecon || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases finalrecon
     add-history finalrecon
     add-test-command "finalrecon.py --help"
     add-to-list "finalrecon,https://github.com/thewhiteh4t/FinalRecon,A web reconnaissance tool that gathers information about web pages"
 }
 
 function install_osrframework() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing osrframework"
-    pipx install osrframework
+    pipx install --system-site-packages osrframework
     pipx inject osrframework 'urllib3<2'
     pipx inject osrframework 'pip==21.2'
     add-history osrframework
     add-test-command "osrframework-cli --help"
     add-to-list "osrframework,https://github.com/i3visio/osrframework,Include references to a bunch of different applications related to username checking / DNS lookups / information leaks research / deep web search / regular expressions extraction and many others."
 }
 
 function install_pwndb() {
     colorecho "Installing pwndb"
     git -C /opt/tools/ clone --depth 1 https://github.com/davidtavarez/pwndb.git
     cd /opt/tools/pwndb || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases pwndb
     add-history pwndb
     add-test-command "pwndb.py --help"
     add-to-list "pwndb,https://github.com/davidtavarez/pwndb,A command-line tool for searching the pwndb database of compromised credentials."
@@ -380,15 +381,15 @@
     add-to-list "githubemail,https://github.com/paulirish/github-email,a command-line tool to retrieve a user's email from Github."
 }
 
 function install_recondog() {
     colorecho "Installing ReconDog"
     git -C /opt/tools/ clone --depth 1 https://github.com/s0md3v/ReconDog
     cd /opt/tools/ReconDog/ || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases recondog
     add-history recondog
     add-test-command "recondog --help"
     add-to-list "recondog,https://github.com/s0md3v/ReconDog,a reconnaissance tool for performing information gathering on a target."
@@ -403,48 +404,48 @@
     add-test-command "gron --help"
     add-to-list "gron,https://github.com/tomnomnom/gron,Make JSON greppable!"
 }
 
 function install_ignorant() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing ignorant"
-    pipx install git+https://github.com/megadose/ignorant
+    pipx install --system-site-packages git+https://github.com/megadose/ignorant
     add-history ignorant
     add-test-command "ignorant --help"
     add-to-list "ignorant,https://github.com/megadose/ignorant,holehe but for phone numbers."
 }
 
 function install_trevorspray() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing trevorspray"
     git -C /opt/tools/ clone --depth 1 https://github.com/blacklanternsecurity/TREVORspray
     cd /opt/tools/TREVORspray || exit
     # https://github.com/blacklanternsecurity/TREVORspray/pull/27
     sed -i "s/1.0.5/1.0.4/" pyproject.toml
-    pipx install .
+    pipx install --system-site-packages .
     add-history trevorspray
     add-test-command "trevorspray --help"
     add-to-list "trevorspray,https://github.com/blacklanternsecurity/TREVORspray,TREVORspray is a modular password sprayer with threading SSH proxying loot modules / and more"
 }
 
 function install_gitfive() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
     # GitFive only works with Python 3.10+.
     colorecho "Installing GitFive"
-    pipx install git+https://github.com/mxrch/GitFive
+    pipx install --system-site-packages git+https://github.com/mxrch/GitFive
     add-test-command "gitfive --help"
     add-to-list "GitFive,https://github.com/mxrch/GitFive,GitFive is an OSINT tool to investigate GitHub profiles."
 }
 
 function install_geopincer() {
     colorecho "Installing GeoPincer"
     git -C /opt/tools clone --depth 1 https://github.com/tloja/GeoPincer.git
     cd /opt/tools/GeoPincer || exit
     sed -i "s#regions.txt#/opt/tools/GeoPincer/regions.txt##" GeoPincer.py
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases geopincer
     add-history geopincer
     add-test-command "geopincer.py --help"
     add-to-list "GeoPincer,https://github.com/tloja/GeoPincer,GeoPincer is a script that leverages OpenStreetMap's Overpass API in order to search for locations."
@@ -462,15 +463,15 @@
     add-to-list "Yalis,https://github.com/EatonChips/yalis,Yet Another LinkedIn Scraper"
 }
 
 function install_murmurhash() {
     colorecho "Installing MurMurHash"
     git -C /opt/tools clone --depth 1 https://github.com/QU35T-code/MurMurHash
     cd /opt/tools/MurMurHash || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases MurMurHash
     add-history MurMurHash
     add-test-command "MurMurHash.py"
     add-to-list "MurMurHash,https://github.com/QU35T-code/MurMurHash,This little tool is to calculate a MurmurHash value of a favicon to hunt phishing websites on the Shodan platform."
@@ -478,42 +479,42 @@
 
 function install_blackbird() {
     colorecho "Installing Blackbird"
     git -C /opt/tools clone --depth 1 https://github.com/p1ngul1n0/blackbird
     cd /opt/tools/blackbird || exit
     sed -i "s#data.json#/opt/tools/blackbird/data.json#" blackbird.py
     sed -i "s#useragents.txt#/opt/tools/blackbird/useragents.txt#" blackbird.py
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases blackbird
     add-history blackbird
     add-test-command "blackbird.py --help"
     add-to-list "Blackbird,https://github.com/p1ngul1n0/blackbird,An OSINT tool to search fast for accounts by username across 581 sites."
 }
 
 function install_sherlock() {
     # CODE-CHECK-WHITELIST=add-history
     colorecho "Installing Sherlock"
     git -C /opt/tools/ clone --depth 1 https://github.com/sherlock-project/sherlock
     cd /opt/tools/sherlock || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases sherlock
     add-test-command "sherlock.py --help"
     add-to-list "Sherlock,https://github.com/sherlock-project/sherlock,Hunt down social media accounts by username across social networks."
 }
 
 function install_censys() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Censys"
-    pipx install censys
+    pipx install --system-site-packages censys
     add-history censys
     add-test-command "censys --help"
     add-to-list "Censys,https://github.com/censys/censys-python,An easy-to-use and lightweight API wrapper for Censys APIs"
 }
 
 function install_gomapenum() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -529,15 +530,15 @@
 
 function install_pymeta() {
   # CODE-CHECK-WHITELIST=add-aliases
   colorecho "Installing pymeta"
   fapt exiftool
   git -C /opt/tools clone --depth 1 https://github.com/m8sec/pymeta
   cd /opt/tools/pymeta || exit
-  python3 -m venv ./venv
+  python3 -m venv --system-site-packages ./venv
   source ./venv/bin/activate
   pip3 install .
   pip3 install -r requirements.txt
   deactivate
   ln -v -s /opt/tools/pymeta/venv/bin/pymeta /opt/tools/bin/
   add-history pymeta
   add-test-command "pymeta -h"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_reverse.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_reverse.sh`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     add-to-list "angr,https://github.com/angr/angr,a platform-agnostic binary analysis framework"
 }
 
 function install_checksec-py() {
     colorecho "Installing checksec.py"
     git -C /opt/tools/ clone --depth 1 https://github.com/Wenzel/checksec.py.git
     cd /opt/tools/checksec.py || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
-    pip3 install .
-    pip3 install --upgrade lief
+    pip install .
+    pip install --upgrade lief==0.13.2
     deactivate
     add-aliases checksec
     add-history checksec
     add-test-command "checksec.py --help"
     add-to-list "checksec-py,https://github.com/Wenzel/checksec.py,Python wrapper script for checksec.sh from paX."
 }
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_rfid.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_rfid.sh`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,30 @@
     add-to-list "libnfc-crypto1-crack,https://github.com/droidnewbie2/acr122uNFC,Implementation of cryptographic attack on Mifare Classic RFID cards"
 }
 
 function install_mfdread() {
     colorecho "Installing mfdread"
     git -C /opt/tools/ clone --depth 1 https://github.com/zhovner/mfdread
     cd /opt/tools/mfdread || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install bitstring
     deactivate
     add-aliases mfdread
     add-history mfdread
     add-test-command "mfdread.py /opt/tools/mfdread/dump.mfd"
     add-to-list "mfdread,https://github.com/zhovner/mfdread,Tool for reading/writing Mifare RFID tags"
 }
 
 function install_proxmark3() {
     colorecho "Installing proxmark3 client"
     colorecho "Compiling proxmark client for generic usage with PLATFORM=PM3OTHER (read https://github.com/RfidResearchGroup/proxmark3/blob/master/doc/md/Use_of_Proxmark/4_Advanced-compilation-parameters.md#platform)"
     colorecho "It can be compiled again for RDV4.0 with 'make clean && make all && make install' from /opt/tools/proxmark3/"
     fapt --no-install-recommends git ca-certificates build-essential pkg-config libreadline-dev gcc-arm-none-eabi libnewlib-dev qtbase5-dev libbz2-dev libbluetooth-dev liblz4-dev
-     git -C /opt/tools/ clone --depth 1 https://github.com/RfidResearchGroup/proxmark3.git
+    git -C /opt/tools/ clone --depth 1 https://github.com/RfidResearchGroup/proxmark3.git
     cd /opt/tools/proxmark3 || exit
     make clean
     make all PLATFORM=PM3OTHER
     make install PLATFORM=PM3OTHER
     add-aliases proxmark3
     add-history proxmark3
     add-test-command "proxmark3 --version"
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_sdr.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_sdr.sh`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     add-test-command "nrf24-network-mapper.py --help"
     add-to-list "mousejack,https://github.com/BastilleResearch/mousejack,Exploit to take over a wireless mouse and keyboard"
 }
 
 function install_jackit() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing jackit"
-    pipx install git+https://github.com/insecurityofthings/jackit
+    pipx install --system-site-packages git+https://github.com/insecurityofthings/jackit
     add-history jackit
     add-test-command "jackit --help"
     add-to-list "jackit,https://github.com/insecurityofthings/jackit,Exploit to take over a wireless mouse and keyboard"
 }
 
 # Package dedicated to SDR
 function package_sdr() {
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_steganography.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_steganography.sh`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     add-test-command "zsteg --help"
     add-to-list "zsteg,https://github.com/zed-0xff/zsteg,Detect steganography hidden in PNG and BMP images"
 }
 
 function install_stegolsb() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing stegolsb"
-    pipx install stego-lsb
+    pipx install --system-site-packages stego-lsb
     add-history stegolsb
     add-test-command "stegolsb --version"
     add-to-list "stegolsb,https://github.com/KyTn/STEGOLSB,Steganography tool to hide data in BMP images using least significant bit algorithm"
 }
 
 # Package dedicated to steganography tools
 function package_steganography() {
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_voip.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_voip.sh`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Author: The Exegol Project
 
 source common.sh
 
 function install_sipvicious() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing SIPVicious"
-    pipx install git+https://github.com/enablesecurity/sipvicious.git
+    pipx install --system-site-packages git+https://github.com/enablesecurity/sipvicious.git
     add-history sipvicious_svcrack
     add-test-command "sipvicious_svcrack --version"
     add-to-list "sipvicious,https://github.com/enablesecurity/sipvicious,Enumeration and MITM tool for SIP devices"
 }
 
 # Package dedicated to VOIP/SIP pentest tools
 function package_voip() {
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_web.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_web.sh`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     add-to-list "swaks,https://github.com/jetmore/swaks,Swaks is a featureful flexible scriptable transaction-oriented SMTP test tool."
 }
 
 function install_weevely() {
     colorecho "Installing weevely"
     git -C /opt/tools clone --depth 1 https://github.com/epinna/weevely3
     cd /opt/tools/weevely3 || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases weevely
     add-history weevely
     add-test-command "weevely.py --help"
     add-to-list "weevely,https://github.com/epinna/weevely3,a webshell designed for post-exploitation purposes that can be extended over the network at runtime."
@@ -112,25 +112,25 @@
     add-test-command "ffuf --help"
     add-to-list "ffuf,https://github.com/ffuf/ffuf,Fast web fuzzer written in Go."
 }
 
 function install_dirsearch() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing dirsearch"
-    pipx install git+https://github.com/maurosoria/dirsearch
+    pipx install --system-site-packages git+https://github.com/maurosoria/dirsearch
     add-history dirsearch
     add-test-command "dirsearch --help"
     add-to-list "dirsearch,https://github.com/maurosoria/dirsearch,Tool for searching files and directories on a web site."
 }
 
 function install_ssrfmap() {
     colorecho "Installing SSRFmap"
     git -C /opt/tools/ clone --depth 1 https://github.com/swisskyrepo/SSRFmap
     cd /opt/tools/SSRFmap || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases ssrfmap
     add-history ssrfmap
     add-test-command "ssrfmap.py --help"
     add-to-list "ssrfmap,https://github.com/swisskyrepo/SSRFmap,a tool for testing SSRF vulnerabilities."
@@ -167,15 +167,15 @@
     add-to-list "nosqlmap,https://github.com/codingo/NoSQLMap,a Python tool for testing NoSQL databases for security vulnerabilities."
 }
 
 function install_xsstrike() {
     colorecho "Installing XSStrike"
     git -C /opt/tools/ clone --depth 1 https://github.com/s0md3v/XSStrike.git
     cd /opt/tools/XSStrike || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases xsstrike
     add-history xsstrike
     add-test-command "xsstrike.py --help"
     add-to-list "xsstrike,https://github.com/s0md3v/XSStrike,a Python tool for detecting and exploiting XSS vulnerabilities."
@@ -192,38 +192,38 @@
     add-to-list "XSpear,https://github.com/hahwul/XSpear,a powerful XSS scanning and exploitation tool."
 }
 
 function install_xsser() {
     colorecho "Installing xsser"
     git -C /opt/tools clone --depth 1 https://github.com/epsylon/xsser.git
     cd /opt/tools/xsser || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install pycurl bs4 pygeoip gobject cairocffi selenium
     deactivate
     add-aliases xsser
     add-history xsser
     add-test-command "xsser --help"
     add-to-list "xsser,https://github.com/epsylon/xsser,XSS scanner."
 }
 
 function install_xsrfprobe() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing XSRFProbe"
-    pipx install git+https://github.com/0xInfection/XSRFProbe
+    pipx install --system-site-packages git+https://github.com/0xInfection/XSRFProbe
     add-history xsrfprobe
     add-test-command "xsrfprobe --help"
     add-to-list "xsrfprobe,https://github.com/0xInfection/XSRFProbe,a tool for detecting and exploiting Cross-Site Request Forgery (CSRF) vulnerabilities"
 }
 
 function install_bolt() {
     colorecho "Installing Bolt"
     git -C /opt/tools/ clone --depth 1 https://github.com/s0md3v/Bolt.git
     cd /opt/tools/Bolt || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases bolt
     add-history bolt
     add-test-command "bolt.py --help"
     add-to-list "bolt,https://github.com/s0md3v/bolt,Bolt crawls the target website to the specified depth and stores all the HTML forms found in a database for further processing."
@@ -242,30 +242,30 @@
     add-to-list "kadimus,https://github.com/P0cL4bs/Kadimus,a tool for detecting and exploiting file upload vulnerabilities"
 }
 
 function install_fuxploider() {
     colorecho "Installing fuxploider"
     git -C /opt/tools/ clone --depth 1 https://github.com/almandin/fuxploider.git
     cd /opt/tools/fuxploider || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases fuxploider
     add-history fuxploider
     add-test-command "fuxploider.py --help"
     add-to-list "fuxploider,https://github.com/almandin/fuxploider,a Python tool for finding and exploiting file upload forms/directories."
 }
 
 function install_patator() {
     colorecho "Installing patator"
     fapt libmariadb-dev libcurl4-openssl-dev libssl-dev ldap-utils libpq-dev ike-scan unzip default-jdk libsqlite3-dev libsqlcipher-dev
     git -C /opt/tools clone --depth 1 https://github.com/lanjelot/patator.git
     cd /opt/tools/patator || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases patator
     add-history patator
     add-test-command "patator.py ftp_login --help"
     add-to-list "patator,https://github.com/lanjelot/patator,Login scanner."
@@ -290,51 +290,53 @@
     add-test-command "wpscan --help"
     add-to-list "wpscan,https://github.com/wpscanteam/wpscan,A tool to enumerate WordPress-based websites"
 }
 
 function install_droopescan() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing droopescan"
-    pipx install git+https://github.com/droope/droopescan.git
+    pipx install --system-site-packages git+https://github.com/droope/droopescan.git
     add-history droopescan
     add-test-command "droopescan --help"
     add-to-list "droopescan,https://github.com/droope/droopescan,Scan Drupal websites for vulnerabilities."
 }
 
 function install_drupwn() {
     colorecho "Installing drupwn"
     git -C /opt/tools/ clone --depth 1 https://github.com/immunIT/drupwn
     cd /opt/tools/drupwn || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r ./requirements.txt
     deactivate
     add-aliases drupwn
     add-history drupwn
     add-test-command "drupwn --help"
     add-to-list "drupwn,https://github.com/immunIT/drupwn,Drupal security scanner."
 }
 
 function install_cmsmap() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing CMSmap"
-    pipx install git+https://github.com/Dionach/CMSmap.git
-    # TODO: Config ?
+    pipx install --system-site-packages git+https://github.com/Dionach/CMSmap.git
+    sed -i 's/wordlist =  wordlist\/rockyou.txt/wordlist =  \/usr\/share\/wordlists\/rockyou.txt/' /root/.local/share/pipx/venvs/cmsmap/lib/python3*/site-packages/cmsmap/cmsmap.conf
+    sed -i 's/edbpath = \/usr\/share\/exploitdb/edbpath = \/opt\/tools\/exploitdb/' /root/.local/share/pipx/venvs/cmsmap/lib/python3*/site-packages/cmsmap/cmsmap.conf
+    sed -i 's/edbtype = apt/edbtype = git/' /root/.local/share/pipx/venvs/cmsmap/lib/python3*/site-packages/cmsmap/cmsmap.conf
     # exploit-db path is required (misc package -> searchsploit)
     # cmsmap -U PC
     add-history cmsmap
     add-test-command "cmsmap --help; cmsmap --help |& grep 'Post Exploitation'"
     add-to-list "cmsmap,https://github.com/Dionach/CMSmap,Tool for security audit of web content management systems."
 }
 
 function install_moodlescan() {
     colorecho "Installing moodlescan"
     git -C /opt/tools/ clone --depth 1 https://github.com/inc0d3/moodlescan.git
     cd /opt/tools/moodlescan || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     cd /opt/tools/moodlescan || exit
     # updating moodlescan database
     catch_and_retry ./venv/bin/python3 moodlescan.py -a
     add-aliases moodlescan
@@ -367,77 +369,77 @@
     add-to-list "tls-scanner,https://github.com/tls-attacker/tls-scanner,a simple script to check the security of a remote TLS/SSL web server"
 }
 
 function install_cloudfail() {
     colorecho "Installing CloudFail"
     git -C /opt/tools/ clone --depth 1 https://github.com/m0rtem/CloudFail
     cd /opt/tools/CloudFail || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases cloudfail
     add-history cloudfail
     add-test-command "cloudfail.py --help"
     add-to-list "cloudfail,https://github.com/m0rtem/CloudFail,a reconnaissance tool for identifying misconfigured CloudFront domains."
 }
 
 function install_eyewitness() {
     colorecho "Installing EyeWitness"
     git -C /opt/tools/ clone --depth 1 https://github.com/FortyNorthSecurity/EyeWitness
     cd /opt/tools/EyeWitness || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     ./Python/setup/setup.sh
     deactivate
     add-aliases eyewitness
     add-history eyewitness
     add-test-command "EyeWitness.py --help"
     add-to-list "eyewitness,https://github.com/FortyNorthSecurity/EyeWitness,a tool to take screenshots of websites / provide some server header info / and identify default credentials if possible."
 }
 
 function install_oneforall() {
     colorecho "Installing OneForAll"
     git -C /opt/tools/ clone --depth 1 https://github.com/shmilylty/OneForAll.git
     cd /opt/tools/OneForAll || exit
     # https://github.com/shmilylty/OneForAll/pull/340
-    local temp_fix_limit="2024-01-20"
+    local temp_fix_limit="2024-05-20"
     if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
       criticalecho "Temp fix expired. Exiting."
     else
       git config --local user.email "local"
       git config --local user.name "local"
       local prs=("340")
       local pr
       for pr in "${prs[@]}"; do git fetch origin "pull/$pr/head:pull/$pr" && git merge --strategy-option theirs --no-edit "pull/$pr"; done
     fi
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases oneforall
     add-history oneforall
     add-test-command "oneforall.py version"
     add-to-list "oneforall,https://github.com/shmilylty/OneForAll,a powerful subdomain collection tool."
 }
 
 function install_wafw00f() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing wafw00f"
-    pipx install wafw00F
+    pipx install --system-site-packages wafw00F
     add-history wafw00f
     add-test-command "wafw00f --help"
     add-to-list "wafw00f,https://github.com/EnableSecurity/wafw00f,a Python tool that helps to identify and fingerprint web application firewall (WAF) products."
 }
 
 function install_corscanner() {
     colorecho "Installing CORScanner"
     git -C /opt/tools/ clone --depth 1 https://github.com/chenjj/CORScanner.git
     cd /opt/tools/CORScanner || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases corscanner
     add-history corscanner
     add-test-command "cors_scan.py --help"
     add-to-list "corscanner,https://github.com/chenjj/CORScanner,a Python script for finding CORS misconfigurations."
@@ -464,15 +466,15 @@
     add-to-list "gowitness,https://github.com/sensepost/gowitness,A website screenshot utility written in Golang."
 }
 
 function install_linkfinder() {
     colorecho "Installing LinkFinder"
     git -C /opt/tools/ clone --depth 1 https://github.com/GerbenJavado/LinkFinder.git
     cd /opt/tools/LinkFinder || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases linkfinder
     add-history linkfinder
     add-test-command "linkfinder.py --help"
     add-to-list "linkfinder,https://github.com/GerbenJavado/LinkFinder,a Python script that finds endpoints and their parameters in JavaScript files."
@@ -488,25 +490,25 @@
     add-test-command "timing_attack --help"
     add-to-list "timing,https://github.com/ffleming/timing_attack,Tool to generate a timing profile for a given command."
 }
 
 function install_updog() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing updog"
-    pipx install updog
+    pipx install --system-site-packages updog
     add-history updog
     add-test-command "updog --help"
     add-to-list "updog,https://github.com/sc0tfree/updog,Simple replacement for Python's SimpleHTTPServer."
 }
 
 function install_jwt_tool() {
     colorecho "Installing JWT tool"
     git -C /opt/tools/ clone --depth 1 https://github.com/ticarpi/jwt_tool
     cd /opt/tools/jwt_tool || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases jwt_tool
     add-history jwt_tool
     add-test-command "jwt_tool.py --help"
     add-to-list "jwt,https://github.com/ticarpi/jwt_tool,a command-line tool for working with JSON Web Tokens (JWTs)"
@@ -521,25 +523,25 @@
     add-test-command "wuzz --help"
     add-to-list "wuzz,https://github.com/asciimoo/wuzz,a command-line tool for interacting with HTTP(S) web services"
 }
 
 function install_git-dumper() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing git-dumper"
-    pipx install git-dumper
+    pipx install --system-site-packages git-dumper
     add-history git-dumper
     add-test-command "git-dumper --help"
     add-to-list "git-dumper,https://github.com/arthaud/git-dumper,Small script to dump a Git repository from a website."
 }
 
 function install_gittools() {
     colorecho "Installing GitTools"
     git -C /opt/tools/ clone --depth 1 https://github.com/internetwache/GitTools.git
     cd /opt/tools/GitTools/Finder || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases gittools
     add-history gittools
     add-test-command "extractor.sh --help|& grep 'USAGE: extractor.sh GIT-DIR DEST-DIR'"
     add-test-command "gitdumper.sh --help|& grep 'USAGE: http://target.tld/.git/'"
@@ -585,29 +587,29 @@
     add-to-list "jdwp,https://github.com/IOActive/jdwp-shellifier,This exploitation script is meant to be used by pentesters against active JDWP service / in order to gain Remote Code Execution."
 }
 
 function install_httpmethods() {
     colorecho "Installing httpmethods"
     git -C /opt/tools/ clone --depth 1 https://github.com/ShutdownRepo/httpmethods
     cd /opt/tools/httpmethods || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases httpmethods
     add-history httpmethods
     add-test-command "httpmethods.py --help"
     add-to-list "httpmethods,https://github.com/ShutdownRepo/httpmethods,Tool for exploiting HTTP methods (e.g. PUT / DELETE / etc.)"
 }
 
 function install_h2csmuggler() {
     colorecho "Installing h2csmuggler"
     git -C /opt/tools/ clone --depth 1 https://github.com/BishopFox/h2csmuggler
     cd /opt/tools/h2csmuggler || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install h2
     deactivate
     add-aliases h2csmuggler
     add-history h2csmuggler
     add-test-command "h2csmuggler.py --help"
     add-to-list "h2csmuggler,https://github.com/BishopFox/h2csmuggler,HTTP Request Smuggling tool using H2C upgrade"
@@ -638,15 +640,15 @@
     add-to-list "feroxbuster,https://github.com/epi052/feroxbuster,Simple / fast and recursive content discovery tool"
 }
 
 function install_tomcatwardeployer() {
     colorecho "Installing tomcatWarDeployer"
     git -C /opt/tools/ clone --depth 1 https://github.com/mgeeky/tomcatWarDeployer.git
     cd /opt/tools/tomcatWarDeployer || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases tomcatwardeployer
     add-history tomcatwardeployer
     add-test-command "tomcatWarDeployer.py --help"
     add-to-list "tomcatwardeployer,https://github.com/mgeeky/tomcatwardeployer,Script to deploy war file in Tomcat."
@@ -665,15 +667,15 @@
     add-test-command "clusterd.py --help"
     add-to-list "clusterd,https://github.com/hatRiot/clusterd,A tool to distribute and remotely manage Hacking Team's RCS agents."
 }
 
 function install_arjun() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing arjun"
-    pipx install arjun
+    pipx install --system-site-packages arjun
     add-history arjun
     add-test-command "arjun --help"
     add-to-list "arjun,https://github.com/s0md3v/Arjun,HTTP parameter discovery suite."
 }
 
 function install_nuclei() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -734,15 +736,15 @@
     add-test-command "anew --help"
     add-to-list "anew,https://github.com/tomnomnom/anew,A simple tool for filtering and manipulating text data / such as log files and other outputs."
 }
 
 function install_robotstester() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing Robotstester"
-    pipx install git+https://github.com/p0dalirius/robotstester
+    pipx install --system-site-packages git+https://github.com/p0dalirius/robotstester
     add-history robotstester
     add-test-command "robotstester --help"
     add-to-list "robotstester,https://github.com/p0dalirius/robotstester,Utility for testing whether a website's robots.txt file is correctly configured."
 }
 
 function install_naabu() {
     # CODE-CHECK-WHITELIST=add-aliases
@@ -777,15 +779,15 @@
     add-to-list "burpsuite,https://portswigger.net/burp,Web application security testing tool."
 }
 
 function install_smuggler() {
     colorecho "Installing smuggler.py"
     git -C /opt/tools/ clone --depth 1 https://github.com/defparam/smuggler.git
     cd /opt/tools/smuggler || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     add-aliases smuggler
     add-history smuggler
     add-test-command "smuggler.py --help"
     add-to-list "smuggler,https://github.com/defparam/smuggler,Smuggler is a tool that helps pentesters and red teamers to smuggle data into and out of the network even when there are multiple layers of security in place."
 }
 
 function install_php_filter_chain_generator() {
@@ -797,15 +799,15 @@
     add-to-list "PHP filter chain generator,https://github.com/synacktiv/php_filter_chain_generator,A CLI to generate PHP filters chain / get your RCE without uploading a file if you control entirely the parameter passed to a require or an include in PHP!"
 }
 
 function install_kraken() {
     colorecho "Installing Kraken"
     git -C /opt/tools clone --depth 1 --recurse-submodules https://github.com/kraken-ng/Kraken.git
     cd /opt/tools/Kraken || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     source ./venv/bin/activate
     pip3 install -r requirements.txt
     deactivate
     add-aliases kraken
     add-history kraken
     add-test-command "kraken.py -h"
     add-to-list "Kraken,https://github.com/kraken-ng/Kraken,Kraken is a modular multi-language webshell focused on web post-exploitation and defense evasion. It supports three technologies (PHP / JSP and ASPX) and is core is developed in Python."
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_wifi.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_wifi.sh`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,26 @@
     add-to-list "reaver,https://github.com/t6x/reaver-wps-fork-t6x,reaver is a tool for brute-forcing WPS (Wireless Protected Setup) PINs."
     add-to-list "bully,https://github.com/aanarchyy/bully,bully is a tool for brute-forcing WPS (Wireless Protected Setup) PINs."
     add-to-list "cowpatty,https://github.com/joswr1ght/cowpatty,cowpatty is a tool for offline dictionary attacks against WPA-PSK (Pre-Shared Key) networks."
 }
 
 function install_pyrit() {
     colorecho "Installing pyrit"
-    git -C /opt/tools clone --depth 1 https://github.com/JPaulMora/Pyrit
+    # can't install with python3/python2 with latest changes.
+    # steps to remove temp fix:
+    #  1. try to install pyrit with git clone + venv + setup.py install with python2 or 3 (without the git patch)
+    #  2. if it works, remove the temp fix (and probably the patch as well)
+    local temp_fix_limit="2024-05-20"
+    if [ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]; then
+      criticalecho "Temp fix expired. Exiting."
+    else
+      # git -C /opt/tools clone --depth 1 https://github.com/JPaulMora/Pyrit
+      git -C /opt/tools/ clone https://github.com/JPaulMora/Pyrit
+      git -C /opt/tools/Pyrit checkout f0f1913c645b445dd391fb047b812b5ba511782c
+    fi
     cd /opt/tools/Pyrit || exit
     fapt libpq-dev
     virtualenv --python python2 ./venv
     source ./venv/bin/activate
     pip2 install psycopg2-binary scapy
     deactivate
     # https://github.com/JPaulMora/Pyrit/issues/591
@@ -48,15 +59,15 @@
     add-to-list "pyrit,https://github.com/JPaulMora/Pyrit,Python-based WPA/WPA2-PSK attack tool."
 }
 
 function install_wifite2() {
     colorecho "Installing wifite2"
     git -C /opt/tools/ clone --depth 1 https://github.com/derv82/wifite2.git
     cd /opt/tools/wifite2 || exit
-    python3 -m venv ./venv
+    python3 -m venv --system-site-packages ./venv
     catch_and_retry ./venv/bin/python3 setup.py install
     add-aliases wifite
     add-history wifite
     add-test-command "Wifite.py --help"
     add-to-list "wifite2,https://github.com/derv82/wifite2,Script for auditing wireless networks."
 }
```

### Comparing `Exegol-4.3.1/exegol-docker-build/sources/install/package_wordlists.sh` & `exegol-4.3.2/exegol-docker-build/sources/install/package_wordlists.sh`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,22 @@
     add-test-command "cewl --help"
     add-to-list "cewl,https://digi.ninja/projects/cewl.php,Generates custom wordlists by spidering a target's website and parsing the results"
 }
 
 function install_cewler() {
     # CODE-CHECK-WHITELIST=add-aliases
     colorecho "Installing cewler"
-    pipx install cewler
+    pipx install --system-site-packages cewler
+    # https://github.com/roys/cewler/pull/5
+    local temp_fix_limit="2024-05-04"
+    if [[ "$(date +%Y%m%d)" -gt "$(date -d $temp_fix_limit +%Y%m%d)" ]]; then
+      criticalecho "Temp fix expired. Exiting."
+    else
+        pipx inject cewler pypdf==4.0.1
+    fi
     add-history cewler
     add-test-command "cewler --output cewler.txt https://thehacker.recipes/"
     add-to-list "cewler,https://github.com/roys/cewler,CeWL alternative in Python"
 }
 
 function install_seclists() {
     # CODE-CHECK-WHITELIST=add-aliases,add-history
```

### Comparing `Exegol-4.3.1/exegol-docker-build/web.dockerfile` & `exegol-4.3.2/exegol-docker-build/web.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.3.1/setup.py` & `exegol-4.3.2/setup.py`

 * *Files identical despite different names*

