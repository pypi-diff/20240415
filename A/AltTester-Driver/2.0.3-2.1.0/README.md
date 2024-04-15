# Comparing `tmp/AltTester-Driver-2.0.3.tar.gz` & `tmp/alttester_driver-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AltTester-Driver-2.0.3.tar", last modified: Tue Jan  9 12:40:45 2024, max compression
+gzip compressed data, was "alttester_driver-2.1.0.tar", last modified: Mon Apr 15 10:33:03 2024, max compression
```

## Comparing `AltTester-Driver-2.0.3.tar` & `alttester_driver-2.1.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.449878 AltTester-Driver-2.0.3/
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.372859 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/
--rw-rw-rw-   0        0        0     3511 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4513 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-09 12:40:45.000000 AltTester-Driver-2.0.3/AltTester_Driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       57 2023-07-28 14:01:00.000000 AltTester-Driver-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3511 2024-01-09 12:40:45.449878 AltTester-Driver-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-01-08 12:23:58.000000 AltTester-Driver-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.383171 AltTester-Driver-2.0.3/alttester/
--rw-rw-rw-   0        0        0     1065 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/__init__.py
--rw-rw-rw-   0        0        0      736 2024-01-09 11:15:26.000000 AltTester-Driver-2.0.3/alttester/__version__.py
--rw-rw-rw-   0        0        0    11405 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/_websocket.py
--rw-rw-rw-   0        0        0    37973 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/altdriver.py
--rw-rw-rw-   0        0        0    12484 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/altobject.py
--rw-rw-rw-   0        0        0     1013 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/by.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.389441 AltTester-Driver-2.0.3/alttester/commands/
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.392952 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/
--rw-rw-rw-   0        0        0     1011 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/__init__.py
--rw-rw-rw-   0        0        0     2608 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/add_notification_listener.py
--rw-rw-rw-   0        0        0     1874 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/remove_notification_listener.py
--rw-rw-rw-   0        0        0     1022 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/reset_input.py
--rw-rw-rw-   0        0        0     1967 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/set_server_logging.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.398942 AltTester-Driver-2.0.3/alttester/commands/FindObjects/
--rw-rw-rw-   0        0        0     1347 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/__init__.py
--rw-rw-rw-   0        0        0     2104 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object.py
--rw-rw-rw-   0        0        0     1285 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object_at_coordinates.py
--rw-rw-rw-   0        0        0     2125 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object_which_contains.py
--rw-rw-rw-   0        0        0     2105 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_objects.py
--rw-rw-rw-   0        0        0     2126 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_objects_which_contains.py
--rw-rw-rw-   0        0        0     2145 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_component_property.py
--rw-rw-rw-   0        0        0     2571 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_object.py
--rw-rw-rw-   0        0        0     2676 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
--rw-rw-rw-   0        0        0     2732 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_object_which_contains.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.408532 AltTester-Driver-2.0.3/alttester/commands/InputActions/
--rw-rw-rw-   0        0        0     1477 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/__init__.py
--rw-rw-rw-   0        0        0     1263 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/begin_touch.py
--rw-rw-rw-   0        0        0     1665 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/click_coordinates.py
--rw-rw-rw-   0        0        0     1258 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/end_touch.py
--rw-rw-rw-   0        0        0     2008 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/keys_down.py
--rw-rw-rw-   0        0        0     1937 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/keys_up.py
--rw-rw-rw-   0        0        0     1583 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/move_mouse.py
--rw-rw-rw-   0        0        0     1388 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/move_touch.py
--rw-rw-rw-   0        0        0     1564 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/multi_point_swipe.py
--rw-rw-rw-   0        0        0     2307 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/press_keys.py
--rw-rw-rw-   0        0        0     1674 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/scroll_mouse.py
--rw-rw-rw-   0        0        0     1625 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/swipe.py
--rw-rw-rw-   0        0        0     1661 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/tap_coordinates.py
--rw-rw-rw-   0        0        0     1581 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/InputActions/tilt.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.411532 AltTester-Driver-2.0.3/alttester/commands/Notifications/
--rw-rw-rw-   0        0        0     1171 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/__init__.py
--rw-rw-rw-   0        0        0     1613 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/base_notification_callbacks.py
--rw-rw-rw-   0        0        0      922 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/load_scene_mode.py
--rw-rw-rw-   0        0        0      891 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/load_scene_notification_result.py
--rw-rw-rw-   0        0        0      902 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/log_notification_result.py
--rw-rw-rw-   0        0        0      863 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/Notifications/notification_type.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.419722 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/
--rw-rw-rw-   0        0        0     1477 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/__init__.py
--rw-rw-rw-   0        0        0     2658 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/call_method.py
--rw-rw-rw-   0        0        0     1548 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/click_element.py
--rw-rw-rw-   0        0        0     1247 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/get_all_components.py
--rw-rw-rw-   0        0        0     1652 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/get_component_property.py
--rw-rw-rw-   0        0        0     1213 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/get_text.py
--rw-rw-rw-   0        0        0     1246 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_down.py
--rw-rw-rw-   0        0        0     1247 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_enter.py
--rw-rw-rw-   0        0        0     1227 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_exit.py
--rw-rw-rw-   0        0        0     1227 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_up.py
--rw-rw-rw-   0        0        0     1658 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/set_component_property.py
--rw-rw-rw-   0        0        0     1363 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/set_text.py
--rw-rw-rw-   0        0        0     1544 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/tap_element.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.425286 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/
--rw-rw-rw-   0        0        0     1606 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/__init__.py
--rw-rw-rw-   0        0        0      967 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/delete_player_pref.py
--rw-rw-rw-   0        0        0     1217 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/delete_player_pref_key.py
--rw-rw-rw-   0        0        0      971 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_all_loaded_scenes.py
--rw-rw-rw-   0        0        0     1002 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_current_scene.py
--rw-rw-rw-   0        0        0     1717 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_player_pref_key.py
--rw-rw-rw-   0        0        0     1108 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_time_scale.py
--rw-rw-rw-   0        0        0     1455 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/load_scene.py
--rw-rw-rw-   0        0        0     2094 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/set_player_pref_key.py
--rw-rw-rw-   0        0        0     1457 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/set_time_scale.py
--rw-rw-rw-   0        0        0     1381 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/unload_scene.py
--rw-rw-rw-   0        0        0     1759 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
--rw-rw-rw-   0        0        0     1283 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/__init__.py
--rw-rw-rw-   0        0        0     8206 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/base_command.py
--rw-rw-rw-   0        0        0     1224 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/get_png_screenshot.py
--rw-rw-rw-   0        0        0      967 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/get_server_version.py
--rw-rw-rw-   0        0        0     1621 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/get_static_property.py
--rw-rw-rw-   0        0        0     1601 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/commands/set_static_property.py
--rw-rw-rw-   0        0        0     4582 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/exceptions.py
--rw-rw-rw-   0        0        0     8555 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/keycode.py
--rw-rw-rw-   0        0        0     1075 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/logging.py
--rw-rw-rw-   0        0        0      992 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/playerpref.py
--rw-rw-rw-   0        0        0     1726 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/alttester/reverse_port_forwarding.py
--rw-rw-rw-   0        0        0      181 2023-12-20 16:37:47.000000 AltTester-Driver-2.0.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       53 2023-10-24 11:47:21.000000 AltTester-Driver-2.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-09 12:40:45.449878 AltTester-Driver-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3446 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.365338 AltTester-Driver-2.0.3/tests/
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.433272 AltTester-Driver-2.0.3/tests/integration/
--rw-rw-rw-   0        0        0      715 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/__init__.py
--rw-rw-rw-   0        0        0     4164 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/conftest.py
--rw-rw-rw-   0        0        0     5246 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_driver.py
--rw-rw-rw-   0        0        0     4422 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_notifications.py
--rw-rw-rw-   0        0        0     1557 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_reverse_port_forwarding.py
--rw-rw-rw-   0        0        0    37024 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene01.py
--rw-rw-rw-   0        0        0     5395 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene02.py
--rw-rw-rw-   0        0        0     6737 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene03.py
--rw-rw-rw-   0        0        0     5369 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene05.py
--rw-rw-rw-   0        0        0     4643 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene07.py
--rw-rw-rw-   0        0        0     2410 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene09.py
--rw-rw-rw-   0        0        0     4416 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/test_scene10.py
--rw-rw-rw-   0        0        0     1143 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/integration/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-09 12:40:45.448878 AltTester-Driver-2.0.3/tests/unit/
--rw-rw-rw-   0        0        0      715 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     2442 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/unit/test_altobject.py
--rw-rw-rw-   0        0        0     2293 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/unit/test_commands.py
--rw-rw-rw-   0        0        0     6297 2024-01-09 11:13:58.000000 AltTester-Driver-2.0.3/tests/unit/test_websocket.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.206964 alttester_driver-2.1.0/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.204364 alttester_driver-2.1.0/AltTester_Driver.egg-info/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4559 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/not-zip-safe
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/requires.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2024-04-15 10:33:02.000000 alttester_driver-2.1.0/AltTester_Driver.egg-info/top_level.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/MANIFEST.in
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3560 2024-04-15 10:33:03.205752 alttester_driver-2.1.0/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1601 2024-03-31 06:05:52.000000 alttester_driver-2.1.0/README.md
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.972165 alttester_driver-2.1.0/alttester/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1040 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      718 2024-03-25 09:42:14.000000 alttester_driver-2.1.0/alttester/__version__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    12267 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/alttester/_websocket.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    37704 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/alttester/altdriver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    12119 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      977 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/by.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.980078 alttester_driver-2.1.0/alttester/commands/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.013066 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      990 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2538 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/add_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1824 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/remove_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      992 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/reset_input.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1908 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/AltTesterCommands/set_server_logging.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.044821 alttester_driver-2.1.0/alttester/commands/FindObjects/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2042 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1247 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_at_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2063 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_object_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2043 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2064 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/find_objects_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2461 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2496 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2598 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2654 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_which_contains.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.059878 alttester_driver-2.1.0/alttester/commands/InputActions/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1447 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1225 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/begin_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1614 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/click_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1219 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/end_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1951 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/keys_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1882 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/keys_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1534 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/move_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1347 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/move_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1515 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/multi_point_swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2239 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/press_keys.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1623 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/scroll_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/tap_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1532 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/InputActions/tilt.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.105713 alttester_driver-2.1.0/alttester/commands/Notifications/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1149 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1579 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/base_notification_callbacks.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      894 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_mode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      869 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/log_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      838 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/Notifications/notification_type.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.117539 alttester_driver-2.1.0/alttester/commands/ObjectCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1448 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2587 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/call_method.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1499 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/click_element.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_all_components.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1605 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1175 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1209 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_enter.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_exit.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1189 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1610 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1321 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1495 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/ObjectCommands/tap_element.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.134176 alttester_driver-2.1.0/alttester/commands/UnityCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1578 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1179 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      944 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      974 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_current_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1075 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/get_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1409 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/load_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2037 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/set_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1410 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/set_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/unload_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1710 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1256 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7982 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/alttester/commands/base_command.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1187 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_png_screenshot.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      940 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_server_version.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1574 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/get_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1554 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/commands/set_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5039 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/alttester/exceptions.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     8202 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/keycode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1033 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/logging.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      960 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/playerpref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1680 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/alttester/reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      300 2024-04-15 07:14:09.000000 alttester_driver-2.1.0/requirements-dev.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/requirements.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2024-04-15 10:33:03.207659 alttester_driver-2.1.0/setup.cfg
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3351 2024-01-09 14:51:06.000000 alttester_driver-2.1.0/setup.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:02.947278 alttester_driver-2.1.0/tests/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.198107 alttester_driver-2.1.0/tests/integration/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7353 2024-04-15 07:14:09.000000 alttester_driver-2.1.0/tests/integration/conftest.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5110 2024-04-01 07:09:49.000000 alttester_driver-2.1.0/tests/integration/test_driver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4366 2024-01-09 14:51:06.000000 alttester_driver-2.1.0/tests/integration/test_notifications.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1512 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/test_reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    21323 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene01_part1.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    18718 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene01_part2.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5202 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene02.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6527 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene03.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5191 2024-04-10 07:45:53.000000 alttester_driver-2.1.0/tests/integration/test_scene05.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4478 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene07.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2306 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene09.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4259 2024-03-25 08:05:11.000000 alttester_driver-2.1.0/tests/integration/test_scene10.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1114 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/integration/utils.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:03.202908 alttester_driver-2.1.0/tests/unit/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      699 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2368 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2229 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_commands.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     6103 2023-11-07 12:46:27.000000 alttester_driver-2.1.0/tests/unit/test_websocket.py
```

### Comparing `AltTester-Driver-2.0.3/AltTester_Driver.egg-info/PKG-INFO` & `alttester_driver-2.1.0/AltTester_Driver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-Metadata-Version: 2.1
-Name: AltTester-Driver
-Version: 2.0.3
-Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://alttester.com/docs/sdk/latest/
-Author: Altom Consulting
-Author-email: contact@alttester.com
-License: GNU GPLv3
-Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://alttester.com/docs/sdk/latest
-Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
-Keywords: unity testing tests
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: C#
-Classifier: Programming Language :: Java
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.4.0
-Description-Content-Type: text/markdown
-
-# AltTester Python Bindings
-
-This package contains an library for adding Python language binding to the AltTester framework.
-
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
-
-You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
-
-Read the documentation on https://alttester.com/docs/sdk/latest/
-
-## Get Started
-
-Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
-
-## Development
-
--   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
--   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
-
-### Running Tests
-
-Run the following command to install the dev dependencies:
-
-```
-$ pip install -r requirements-dev.txt
-```
-
-#### Unit Tests
-
-```
-$ pytest tests/unit/
-```
-
-#### Integration Tests
-
-```
-$ pytest tests/integration/
-```
-
-## Contributing
-
-Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
-
-## Support
-
-Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
-
-Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
-
-## License
-
-Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
+Metadata-Version: 2.1
+Name: AltTester-Driver
+Version: 2.1.0
+Summary: Python bindings for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
+Home-page: https://alttester.com/docs/sdk/latest/
+Author: Altom Consulting
+Author-email: contact@alttester.com
+License: GNU GPLv3
+Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
+Project-URL: Documentation, https://alttester.com/docs/sdk/latest
+Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
+Keywords: unity testing tests
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: C#
+Classifier: Programming Language :: Java
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: Software Development :: Testing :: Unit
+Requires-Python: >=3.4.0
+Description-Content-Type: text/markdown
+Requires-Dist: loguru
+Requires-Dist: deprecated
+Requires-Dist: websocket-client
+Requires-Dist: pure-python-adb
+
+# AltTester® Python Bindings
+
+This package contains an library for adding Python language binding to the AltTester® framework.
+
+AltTester® Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python, Java or Robot Framework.
+
+You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
+
+Read the documentation on https://alttester.com/docs/sdk/latest/
+
+## Get Started
+
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
+
+## Development
+
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+
+### Running Tests
+
+Run the following command to install the dev dependencies:
+
+```
+$ pip install -r requirements-dev.txt
+```
+
+#### Unit Tests
+
+```
+$ pytest tests/unit/
+```
+
+#### Integration Tests
+
+```
+$ pytest tests/integration/
+```
+
+## Contributing
+
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
+
+## Support
+
+Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
+
+Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
+
+## License
+
+Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/AltTester_Driver.egg-info/SOURCES.txt` & `alttester_driver-2.1.0/AltTester_Driver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 alttester/commands/UnityCommands/unload_scene.py
 alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_driver.py
 tests/integration/test_notifications.py
 tests/integration/test_reverse_port_forwarding.py
-tests/integration/test_scene01.py
+tests/integration/test_scene01_part1.py
+tests/integration/test_scene01_part2.py
 tests/integration/test_scene02.py
 tests/integration/test_scene03.py
 tests/integration/test_scene05.py
 tests/integration/test_scene07.py
 tests/integration/test_scene09.py
 tests/integration/test_scene10.py
 tests/integration/utils.py
```

### Comparing `AltTester-Driver-2.0.3/PKG-INFO` & `alttester_driver-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-Metadata-Version: 2.1
-Name: AltTester-Driver
-Version: 2.0.3
-Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://alttester.com/docs/sdk/latest/
-Author: Altom Consulting
-Author-email: contact@alttester.com
-License: GNU GPLv3
-Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://alttester.com/docs/sdk/latest
-Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
-Keywords: unity testing tests
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: C#
-Classifier: Programming Language :: Java
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Testing :: Acceptance
-Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.4.0
-Description-Content-Type: text/markdown
-
-# AltTester Python Bindings
-
-This package contains an library for adding Python language binding to the AltTester framework.
-
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
-
-You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
-
-Read the documentation on https://alttester.com/docs/sdk/latest/
-
-## Get Started
-
-Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
-
-## Development
-
--   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
--   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
-
-### Running Tests
-
-Run the following command to install the dev dependencies:
-
-```
-$ pip install -r requirements-dev.txt
-```
-
-#### Unit Tests
-
-```
-$ pytest tests/unit/
-```
-
-#### Integration Tests
-
-```
-$ pytest tests/integration/
-```
-
-## Contributing
-
-Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
-
-## Support
-
-Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
-
-Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
-
-## License
-
-Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
+Metadata-Version: 2.1
+Name: AltTester-Driver
+Version: 2.1.0
+Summary: Python bindings for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
+Home-page: https://alttester.com/docs/sdk/latest/
+Author: Altom Consulting
+Author-email: contact@alttester.com
+License: GNU GPLv3
+Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
+Project-URL: Documentation, https://alttester.com/docs/sdk/latest
+Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
+Keywords: unity testing tests
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: C#
+Classifier: Programming Language :: Java
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: Software Development :: Testing :: Unit
+Requires-Python: >=3.4.0
+Description-Content-Type: text/markdown
+Requires-Dist: loguru
+Requires-Dist: deprecated
+Requires-Dist: websocket-client
+Requires-Dist: pure-python-adb
+
+# AltTester® Python Bindings
+
+This package contains an library for adding Python language binding to the AltTester® framework.
+
+AltTester® Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python, Java or Robot Framework.
+
+You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
+
+Read the documentation on https://alttester.com/docs/sdk/latest/
+
+## Get Started
+
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
+
+## Development
+
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+
+### Running Tests
+
+Run the following command to install the dev dependencies:
+
+```
+$ pip install -r requirements-dev.txt
+```
+
+#### Unit Tests
+
+```
+$ pytest tests/unit/
+```
+
+#### Integration Tests
+
+```
+$ pytest tests/integration/
+```
+
+## Contributing
+
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
+
+## Support
+
+Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
+
+Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
+
+## License
+
+Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/README.md` & `alttester_driver-2.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# AltTester Python Bindings
-
-This package contains an library for adding Python language binding to the AltTester framework.
-
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
-
-You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
-
-Read the documentation on https://alttester.com/docs/sdk/latest/
-
-## Get Started
-
-Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
-
-## Development
-
--   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
--   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
-
-### Running Tests
-
-Run the following command to install the dev dependencies:
-
-```
-$ pip install -r requirements-dev.txt
-```
-
-#### Unit Tests
-
-```
-$ pytest tests/unit/
-```
-
-#### Integration Tests
-
-```
-$ pytest tests/integration/
-```
-
-## Contributing
-
-Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
-
-## Support
-
-Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
-
-Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
-
-## License
-
-Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
+# AltTester® Python Bindings
+
+This package contains an library for adding Python language binding to the AltTester® framework.
+
+AltTester® Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python, Java or Robot Framework.
+
+You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
+
+Read the documentation on https://alttester.com/docs/sdk/latest/
+
+## Get Started
+
+Check out the [Get Started](https://alttester.com/docs/sdk/latest/pages/get-started.html) guide from the documentation.
+
+## Development
+
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+
+### Running Tests
+
+Run the following command to install the dev dependencies:
+
+```
+$ pip install -r requirements-dev.txt
+```
+
+#### Unit Tests
+
+```
+$ pytest tests/unit/
+```
+
+#### Integration Tests
+
+```
+$ pytest tests/integration/
+```
+
+## Contributing
+
+Check out the full contributing guide [contributing](https://alttester.com/docs/sdk/latest/pages/contributing.html).
+
+## Support
+
+Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
+
+Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
+
+## License
+
+Distributed under the **GNU General Public License v3.0**. See [LICENSE](https://github.com/alttester/AltTester-Unity-SDK/blob/master/LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/alttester/__init__.py` & `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.altdriver import AltDriver
-from alttester.altobject import AltObject
-from alttester.by import By
-from alttester.playerpref import PlayerPrefKeyType
-from alttester.keycode import AltKeyCode
-from alttester.logging import AltLogLevel, AltLogger
-from alttester.exceptions import *
-from alttester.reverse_port_forwarding import *
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.AltTesterCommands.set_server_logging import *
+from alttester.commands.AltTesterCommands.add_notification_listener import *
+from alttester.commands.AltTesterCommands.remove_notification_listener import *
+from alttester.commands.AltTesterCommands.reset_input import *
```

### Comparing `AltTester-Driver-2.0.3/alttester/__version__.py` & `alttester_driver-2.1.0/tests/integration/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-VERSION = "2.0.3"
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
```

### Comparing `AltTester-Driver-2.0.3/alttester/_websocket.py` & `alttester_driver-2.1.0/alttester/_websocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,338 +1,361 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import time
-import json
-from collections import defaultdict, deque
-from urllib.parse import urlencode, urlunparse
-from threading import Thread
-
-from loguru import logger
-import websocket
-
-from . import exceptions
-from .commands.Notifications.notification_type import NotificationType
-from .commands.Notifications.load_scene_notification_result import LoadSceneNotificationResult
-from .commands.Notifications.log_notification_result import LogNotificationResult
-from .commands.Notifications.load_scene_mode import LoadSceneMode
-
-
-class Store:
-    """Stores the responses from AltServer."""
-
-    def __init__(self, dict=None):
-        self._store = dict or defaultdict(deque)
-
-    def __repr__(self):
-        return "{}({!r})".format(self.__class__.__name__, self._store)
-
-    def has(self, key):
-        if not key:
-            return False
-
-        return len(self._store[key]) > 0
-
-    def push(self, key, value):
-        self._store[key].append(value)
-
-    def pop(self, key):
-        try:
-            return self._store[key].popleft()
-        except IndexError:
-            return None
-
-
-class NotificationHandler:
-    """Handles the parsing of the notification messages from AltServer."""
-
-    def __init__(self):
-        self._notification_callbacks = defaultdict(list)
-
-    def __repr__(self):
-        return "{}()".format(self.__class__.__name__)
-
-    def handle_notification(self, message):
-        result = None
-        notification_type = None
-        data = json.loads(message.get("data"))
-
-        if message.get("commandName") == "loadSceneNotification":
-            notification_type = NotificationType.LOADSCENE
-            result = LoadSceneNotificationResult(
-                data.get("sceneName"),
-                LoadSceneMode(data.get("loadSceneMode"))
-            )
-        elif message.get("commandName") == "unloadSceneNotification":
-            notification_type = NotificationType.UNLOADSCENE
-            result = data
-        elif message.get("commandName") == "logNotification":
-            notification_type = NotificationType.LOG
-            result = LogNotificationResult(
-                data.get("message"),
-                data.get("stack_trace"),
-                data.get("level")
-            )
-        elif message.get("commandName") == "applicationPausedNotification":
-            notification_type = NotificationType.APPLICATION_PAUSED
-            result = bool(data)
-
-        for callback in self._notification_callbacks[notification_type]:
-            callback(result)
-
-    def add_notification_listener(self, notification_type, callback, overwrite=False):
-        if overwrite:
-            self._notification_callbacks[notification_type] = [callback]
-
-        self._notification_callbacks[notification_type].append(callback)
-
-    def remove_notification_listener(self, notification_type):
-        self._notification_callbacks[notification_type].clear()
-
-
-class CommandHandler:
-    """Handles the parsing of command messages from AltServer."""
-
-    def __init__(self):
-        self._store = Store()
-
-        self._current_command = None
-        self._timeout_commands = []
-
-    def __repr__(self):
-        return "{}()".format(self.__class__.__name__)
-
-    def set_current_command(self, message):
-        self._current_command = (message.get("messageId"), message.get("commandName"))
-
-    def get_current_command(self):
-        return self._current_command
-
-    def timeout(self):
-        """Mark the current command as timeout."""
-
-        self._timeout_commands.append(self._current_command)
-
-    def handle_command(self, message):
-        command = (message.get("messageId"), message.get("commandName"))
-
-        # Skip messages for commands that timeout
-        if command in self._timeout_commands:
-            return
-
-        self._store.push(command, message)
-
-    def has_response(self):
-        return self._store.has(self._current_command)
-
-    def get_response(self):
-        return self._store.pop(self._current_command)
-
-
-class WebsocketConnection:
-    """Handles the websocket connection with AltServer.
-
-    Args:
-        host (:obj:`str`, optional): The host to connect to. Defaults to ``127.0.0.1``.
-        port (:obj:`int`, optional): The port to connect to. Defaults to ``13000``.
-        path (:obj:`int`, optional): The path section of the url. Defaults to ``/``.
-        params (:obj:`dict`, optional): The params/query component of the url. Default to ``None``.
-        timeout (:obj:`int` or :obj:`float`, optional): The connection timeout time.
-
-    """
-
-    def __init__(self, host="127.0.0.1", port=13000, path="/", params=None, timeout=None, command_handler=None,
-                 notification_handler=None):
-        self.host = host
-        self.port = port
-        self.path = path
-        self.params = params or {}
-
-        self.url = urlunparse(["ws", "{}:{}".format(self.host, self.port), self.path, "", urlencode(self.params), ""])
-
-        self.timeout = timeout
-        self.command_timeout = 60
-        self.delay = 0.1
-
-        self._errors = deque()
-        self._close_message = None
-
-        self._thread = None
-        self._websocket = None
-        self._is_open = False
-
-        self._command_handler = command_handler
-        self._notification_handler = notification_handler
-
-    def __repr__(self):
-        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
-            self.__class__.__name__,
-            self.host,
-            self.port,
-            self.path,
-            self.params,
-            self.timeout,
-        )
-
-    def _create_connection(self):
-        # TODO: Enable and disable the trace based on an environment variable or config option
-        # Uncomment the following line if you are debugging the websocket connection
-        # websocket.enableTrace(True)
-        self._websocket = websocket.WebSocketApp(
-            self.url,
-            on_open=self._on_open,
-            on_message=self._on_message,
-            on_error=self._on_error,
-            on_close=self._on_close
-        )
-        self._thread = Thread(target=self._websocket.run_forever, daemon=True).start()
-
-    def _check_close_message(self):
-        if self._close_message:
-            reason = self._close_message[1]
-
-            if self._close_message[0] == 4001:
-                raise exceptions.NoAppConnected(reason)
-            if self._close_message[0] == 4002:
-                raise exceptions.AppDisconnectedError(reason)
-            if self._close_message[0] == 4005:
-                raise exceptions.AppDisconnectedError(reason)
-
-            raise exceptions.ConnectionError("Connection closed by AltServer with reason: {}.".format(reason))
-
-    def _check_errors(self):
-        if self._errors:
-            error = self._errors.pop()
-            self.close()
-            raise exceptions.ConnectionError(error)
-
-    def _ensure_connection_is_open(self):
-        self._check_close_message()
-        self._check_errors()
-
-        if self._websocket is None or not self._is_open:
-            self.close()
-            raise exceptions.ConnectionError("Connection closed. An unexpected error ocurred.")
-
-    def _on_message(self, ws, message):
-        """A callback which is called when the connection receives data."""
-
-        logger.debug("Received: {}", message)
-        response = json.loads(message)
-
-        if response.get("isNotification"):
-            self._notification_handler.handle_notification(response)
-        else:
-            self._command_handler.handle_command(response)
-
-    def _on_error(self, ws, error):
-        """A callback which is called when the connection gets an error."""
-
-        logger.error("Error: {}", error)
-        self._errors.append(error)
-
-    def _on_close(self, ws, close_status_code, close_msg):
-        """A callback which is called when the connection is closed."""
-
-        logger.debug(
-            "Connection to AltServer closed with status code: {} and message: '{}'.",
-            close_status_code,
-            close_msg
-        )
-
-        self._close_message = (close_status_code, close_msg)
-
-        self._is_open = False
-        self._websocket = None
-
-    def _on_open(self, ws):
-        """A callback which is called when the connection is opened."""
-
-        logger.debug("Connection opened successfully.")
-        self._is_open = True
-
-    def set_command_timeout(self, timeout):
-        self.command_timeout = timeout
-
-    def get_command_timeout(self):
-        return self.command_timeout
-
-    def connect(self):
-        logger.info("Connecting to URL: '{}'.", self.url)
-
-        elapsed_time = 0
-        self._create_connection()
-
-        while not self._is_open and (self.timeout is None or elapsed_time < self.timeout):
-            self._close_message = None
-            self._errors = []
-
-            if self._errors or self._close_message:
-                self.close()
-                self._create_connection()
-
-            time.sleep(self.delay)
-            elapsed_time += self.delay
-
-        self._check_close_message()
-        self._check_errors()
-
-        if not self._is_open:
-            self.close()
-
-            raise exceptions.ConnectionTimeoutError(
-                "Failed to connect to AltServer host: {} port: {}.".format(self.host, self.port)
-            )
-
-    def send(self, data):
-        self._ensure_connection_is_open()
-
-        message = json.dumps(data)
-        logger.debug("Sent: {}", message)
-
-        self._command_handler.set_current_command(data)
-        self._websocket.send(message)
-
-    def recv(self):
-        self._ensure_connection_is_open()
-        elapsed_time = 0
-        delay = 0.1
-
-        while elapsed_time <= self.command_timeout:
-            if self._command_handler.has_response():
-                return self._command_handler.get_response()
-
-            elapsed_time += delay
-            time.sleep(delay)
-
-        if elapsed_time > self.command_timeout:
-            self._command_handler.timeout()
-            raise exceptions.CommandResponseTimeoutException()
-
-    def close(self):
-        logger.info("Closing connection to AltServer on host: {} port: {}", self.host, self.port)
-
-        if self._websocket:
-            self._websocket.close()
-            self._websocket = None
-
-        if self._thread:
-            self._thread.join(0)
-            self._thread = None
-
-        self._errors = []
-        self._close_message = None
-        self._is_open = False
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import time
+import json
+from collections import defaultdict, deque
+from urllib.parse import urlencode, urlunparse
+from threading import Thread
+
+from loguru import logger
+import websocket
+
+from . import exceptions
+from .commands.Notifications.notification_type import NotificationType
+from .commands.Notifications.load_scene_notification_result import LoadSceneNotificationResult
+from .commands.Notifications.log_notification_result import LogNotificationResult
+from .commands.Notifications.load_scene_mode import LoadSceneMode
+
+
+class Store:
+    """Stores the responses from AltTester® Server."""
+
+    def __init__(self, dict=None):
+        self._store = dict or defaultdict(deque)
+
+    def __repr__(self):
+        return "{}({!r})".format(self.__class__.__name__, self._store)
+
+    def has(self, key):
+        if not key:
+            return False
+
+        return len(self._store[key]) > 0
+
+    def push(self, key, value):
+        self._store[key].append(value)
+
+    def pop(self, key):
+        try:
+            return self._store[key].popleft()
+        except IndexError:
+            return None
+
+
+class NotificationHandler:
+    """Handles the parsing of the notification messages from AltTester® Server."""
+
+    def __init__(self):
+        self._notification_callbacks = defaultdict(list)
+
+    def __repr__(self):
+        return "{}()".format(self.__class__.__name__)
+
+    def handle_notification(self, message):
+        result = None
+        notification_type = None
+        data = json.loads(message.get("data"))
+
+        if message.get("commandName") == "loadSceneNotification":
+            notification_type = NotificationType.LOADSCENE
+            result = LoadSceneNotificationResult(
+                data.get("sceneName"),
+                LoadSceneMode(data.get("loadSceneMode"))
+            )
+        elif message.get("commandName") == "unloadSceneNotification":
+            notification_type = NotificationType.UNLOADSCENE
+            result = data
+        elif message.get("commandName") == "logNotification":
+            notification_type = NotificationType.LOG
+            result = LogNotificationResult(
+                data.get("message"),
+                data.get("stack_trace"),
+                data.get("level")
+            )
+        elif message.get("commandName") == "applicationPausedNotification":
+            notification_type = NotificationType.APPLICATION_PAUSED
+            result = bool(data)
+
+        for callback in self._notification_callbacks[notification_type]:
+            callback(result)
+
+    def add_notification_listener(self, notification_type, callback, overwrite=False):
+        if overwrite:
+            self._notification_callbacks[notification_type] = [callback]
+
+        self._notification_callbacks[notification_type].append(callback)
+
+    def remove_notification_listener(self, notification_type):
+        self._notification_callbacks[notification_type].clear()
+
+
+class CommandHandler:
+    """Handles the parsing of command messages from AltTester® Server."""
+
+    def __init__(self):
+        self._store = Store()
+
+        self._current_command = None
+        self._timeout_commands = []
+
+    def __repr__(self):
+        return "{}()".format(self.__class__.__name__)
+
+    def set_current_command(self, message):
+        self._current_command = (message.get(
+            "messageId"), message.get("commandName"))
+
+    def get_current_command(self):
+        return self._current_command
+
+    def timeout(self):
+        """Mark the current command as timeout."""
+
+        self._timeout_commands.append(self._current_command)
+
+    def handle_command(self, message):
+        command = (message.get("messageId"), message.get("commandName"))
+
+        # Skip messages for commands that timeout
+        if command in self._timeout_commands:
+            return
+
+        self._store.push(command, message)
+
+    def has_response(self):
+        return self._store.has(self._current_command)
+
+    def get_response(self):
+        return self._store.pop(self._current_command)
+
+
+class WebsocketConnection:
+    """Handles the websocket connection with AltTester® Server.
+
+    Args:
+        host (:obj:`str`, optional): The host to connect to. Defaults to ``127.0.0.1``.
+        port (:obj:`int`, optional): The port to connect to. Defaults to ``13000``.
+        path (:obj:`int`, optional): The path section of the url. Defaults to ``/``.
+        params (:obj:`dict`, optional): The params/query component of the url. Default to ``None``.
+        timeout (:obj:`int` or :obj:`float`, optional): The connection timeout time.
+
+    """
+
+    def __init__(self, host="127.0.0.1", port=13000, path="/", params=None, timeout=None, command_handler=None,
+                 notification_handler=None):
+        self.host = host
+        self.port = port
+        self.path = path
+        self.params = params or {}
+
+        self.url = urlunparse(["ws", "{}:{}".format(
+            self.host, self.port), self.path, "", urlencode(self.params), ""])
+
+        self.timeout = timeout
+        self.command_timeout = 60
+        self.delay = 0.1
+
+        self._errors = deque()
+        self._close_message = None
+
+        self._thread = None
+        self._websocket = None
+        self._is_open = False
+
+        self._command_handler = command_handler
+        self._notification_handler = notification_handler
+        self._driver_registered_called = False
+
+    def __repr__(self):
+        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
+            self.__class__.__name__,
+            self.host,
+            self.port,
+            self.path,
+            self.params,
+            self.timeout,
+        )
+
+    def _create_connection(self):
+        # TODO: Enable and disable the trace based on an environment variable or config option
+        # Uncomment the following line if you are debugging the websocket connection
+        # websocket.enableTrace(True)
+        self._websocket = websocket.WebSocketApp(
+            self.url,
+            on_open=self._on_open,
+            on_message=self._on_message,
+            on_error=self._on_error,
+            on_close=self._on_close
+        )
+        self._thread = Thread(
+            target=self._websocket.run_forever, daemon=True).start()
+
+    def _check_close_message(self, close_message):
+        if close_message:
+            reason = close_message[1]
+
+            if close_message[0] == 4001:
+                raise exceptions.NoAppConnected(reason)
+            if close_message[0] == 4002:
+                raise exceptions.AppDisconnectedError(reason)
+            if close_message[0] == 4005:
+                raise exceptions.MultipleDriverError(reason)
+            if close_message[0] == 4007:
+                raise exceptions.MultipleDriversTryingToConnectException(
+                    reason)
+            if close_message[0] == 4009:
+                raise exceptions.MaxNoOfConnectionsDriversExceeded(
+                    reason)
+
+            raise exceptions.ConnectionError(
+                "Connection closed by AltTester® Server with reason: {}.".format(reason))
+
+    def _check_errors(self):
+        if self._errors:
+            error = self._errors.pop()
+            self.close()
+            raise exceptions.ConnectionError(error)
+
+    def _ensure_connection_is_open(self):
+        self._check_close_message(self._close_message)
+        self._check_errors()
+
+        if self._websocket is None or not self._is_open:
+            self.close()
+            raise exceptions.ConnectionError(
+                "Connection closed. An unexpected error ocurred.")
+
+    def _on_message(self, ws, message):
+        """A callback which is called when the connection receives data."""
+
+        logger.debug("Received: {}", message)
+        response = json.loads(message)
+
+        if response.get("isNotification"):
+            if "driverRegistered" in message:
+                self._driver_registered_called = True
+            else:
+                self._notification_handler.handle_notification(response)
+        else:
+            self._command_handler.handle_command(response)
+
+    def _on_error(self, ws, error):
+        """A callback which is called when the connection gets an error."""
+
+        logger.error("Error: {}", error)
+        self._errors.append(error)
+
+    def _on_close(self, ws, close_status_code, close_msg):
+        """A callback which is called when the connection is closed."""
+
+        logger.debug(
+            "Connection to AltTester® Server closed with status code: {} and message: '{}'.",
+            close_status_code,
+            close_msg
+        )
+
+        self._close_message = (close_status_code, close_msg)
+        self._driver_registered_called = False
+        self._is_open = False
+        self._websocket = None
+        if close_status_code == 4002:
+            self.connect()
+
+    def _on_open(self, ws):
+        """A callback which is called when the connection is opened."""
+
+        logger.debug("Connection opened successfully.")
+        self._is_open = True
+
+    def set_command_timeout(self, timeout):
+        self.command_timeout = timeout
+
+    def get_command_timeout(self):
+        return self.command_timeout
+
+    def connect(self):
+        logger.info("Connecting to URL: '{}'.", self.url)
+        last_close_message = None
+        elapsed_time = 0
+        while self.timeout is None or elapsed_time < self.timeout:
+            self._create_connection()
+            wait_for_notification = 0
+            try:
+                while wait_for_notification < 5:
+                    if self._driver_registered_called:
+                        logger.debug("Connected to: '{0}'.".format(self.url))
+                        return
+                    time.sleep(self.delay)
+                    wait_for_notification += self.delay
+                    self._check_close_message(self._close_message)
+            except Exception:
+                last_close_message = self._close_message
+                self.close()
+
+            elapsed_time += wait_for_notification
+
+            if self._is_open:  # Added this to be also backward compatible but it will be slower
+                return
+
+        self._check_close_message(last_close_message)
+        self._check_errors()
+        raise exceptions.ConnectionTimeoutError(
+            "Failed to connect to AltTester® Server host: {} port: {}.".format(
+                self.host, self.port)
+        )
+
+    def send(self, data):
+        self._ensure_connection_is_open()
+
+        message = json.dumps(data)
+        logger.debug("Sent: {}", message)
+
+        self._command_handler.set_current_command(data)
+        self._websocket.send(message)
+
+    def recv(self):
+        self._ensure_connection_is_open()
+        elapsed_time = 0
+        delay = 0.1
+
+        while elapsed_time <= self.command_timeout:
+            if self._command_handler.has_response():
+                return self._command_handler.get_response()
+
+            elapsed_time += delay
+            time.sleep(delay)
+
+        if elapsed_time > self.command_timeout:
+            self._command_handler.timeout()
+            raise exceptions.CommandResponseTimeoutException()
+
+    def close(self):
+        logger.info(
+            "Closing connection to AltTester® Server on host: {} port: {}", self.host, self.port)
+
+        if self._websocket:
+            self._websocket.close()
+            self._websocket = None
+
+        if self._thread:
+            self._thread.join(0)
+            self._thread = None
+
+        self._errors = []
+        self._close_message = None
+        self._is_open = False
+        self._driver_registered_called = False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/alttester/altdriver.py` & `alttester_driver-2.1.0/alttester/altdriver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,901 +1,923 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import warnings
-import sys
-
-from loguru import logger
-
-import alttester.commands as commands
-from alttester.commands.base_command import Command
-from alttester.__version__ import VERSION
-from alttester._websocket import WebsocketConnection, CommandHandler, NotificationHandler
-from alttester.altobject import AltObject
-from alttester.by import By
-
-
-warnings.filterwarnings("default", category=DeprecationWarning, module=__name__)
-
-
-class AltDriver:
-    """The driver object will help interacting with all the application objects, their properties and methods.
-
-    When you instantiate an ``AltDriver`` object in your tests, you can use it to “drive” your application like one of
-    your users would, by interacting with all the application objects, their properties and methods.  An ``AltDriver``
-    instance will connect to the AltServer.
-
-    Args:
-        host (:obj:`str`, optional): The host to connect to.
-        port (:obj:`int`, optional): The port to connect to.
-        app_name (:obj:`str`, optional): The application name. Defaults to ``__default__``.
-        enable_logging (:obj:`bool`, optional): If set to ``True`` will turn on logging, by default logging is disabled.
-        timeout (:obj:`int`, :obj:`float`, optional): The timeout duration for establishing a connection, in seconds.
-            If set to ``None``, the connection attempt will wait indefinitely. The default value is ``60`` seconds.
-
-    """
-
-    def __init__(self, host="127.0.0.1", port=13000, app_name="__default__", enable_logging=False, timeout=60):
-        self.host = host
-        self.port = port
-        self.app_name = app_name
-        self.enable_logging = enable_logging
-        self.timeout = timeout
-
-        self._config_logging(self.enable_logging)
-
-        logger.debug(
-            "Connecting to AltTester on host: '{}', port: '{}' and app name: '{}'.",
-            self.host,
-            self.port,
-            self.app_name
-        )
-
-        self._command_handler = CommandHandler()
-        self._notification_handler = NotificationHandler()
-        self._connection = WebsocketConnection(
-            host=self.host,
-            port=self.port,
-            timeout=self.timeout,
-            path="altws",
-            params={"appName": self.app_name},
-            command_handler=self._command_handler,
-            notification_handler=self._notification_handler
-        )
-        self._connection.connect()
-        self._check_server_version()
-
-    def __repr__(self):
-        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
-            self.__class__.__name__,
-            self.host,
-            self.port,
-            self.app_name,
-            self.enable_logging,
-            self.timeout
-        )
-
-    @staticmethod
-    def _config_logging(enable_logging):
-        if enable_logging:
-            logger.configure(
-                handlers=[
-                    dict(sink=sys.stdout, diagnose=False),
-                    dict(sink="./AltTester.log", enqueue=False, serialize=True, mode="w", diagnose=False),
-                ],
-                levels=[dict(name="DEBUG")],
-                activation=[("alttester", True)],
-            )
-        else:
-            logger.disable("alttester")
-
-    @staticmethod
-    def _split_version(version):
-        parts = version.split(".")
-        return (parts[0], parts[1]) if len(parts) > 1 else ("", "")
-
-    def _check_server_version(self):
-        server_version = commands.GetServerVersion.run(self._connection)
-        logger.info("Connection established with instrumented Unity app. AltTester Version: {}", server_version)
-
-        major_server, minor_server = self._split_version(server_version)
-        major_driver, minor_driver = self._split_version(VERSION)
-
-        if major_server != major_driver or minor_server != minor_driver:
-            message = "Version mismatch. AltDriver version is {}. AltTester version is {}.".format(
-                VERSION,
-                server_version
-            )
-
-            logger.warning(message)
-
-    def _get_alt_object(self, data):
-        if data is None:
-            return None
-
-        alt_object = AltObject(self, data)
-
-        logger.debug(
-            "Element {} found at x: {} y: {} mobileY: {}",
-            alt_object.name,
-            alt_object.x,
-            alt_object.y,
-            alt_object.mobileY
-        )
-
-        return alt_object
-
-    def _get_alt_objects(self, data):
-        if data is None:
-            return None
-
-        alt_objects = []
-
-        for element in data:
-            alt_object = AltObject(self, element)
-            alt_objects.append(alt_object)
-
-            logger.debug(
-                "Element {} found at x: {} y: {} mobileY: {}",
-                alt_object.name,
-                alt_object.x,
-                alt_object.y,
-                alt_object.mobileY
-            )
-
-        return alt_objects
-
-    def stop(self):
-        """Close the connection to AltTester."""
-
-        self._connection.close()
-
-    def get_command_response_timeout(self):
-        """Gets the current command response timeout for the AltTester connection.
-
-        Return:
-            int or float: The current command response time.
-
-        """
-
-        return self._connection.set_command_timeout()
-
-    def set_command_response_timeout(self, timeout):
-        """Sets the command response timeout for the AltTester connection.
-
-        Args:
-            timeout (:obj:`int` or :obj:`float`): The new command response timeout in seconds.
-
-        """
-
-        self._connection.set_command_timeout(timeout)
-
-    def get_delay_after_command(self):
-        """Gets the current delay after a command."""
-
-        return Command.get_delay_after_command()
-
-    def set_delay_after_command(self, delay):
-        """Set the delay after a command.
-
-        Args:
-            delay (:obj:`int` or :obj:`float`): The new delay a after a command.
-        """
-
-        Command.set_delay_after_command(delay)
-
-    def set_server_logging(self, logger, log_level):
-        """Sets the level of logging on AltTester.
-
-        Args:
-            logger (:obj:`AltLogger`): The type of logger.
-            log_lever (:obj:`AltLogLevel`): The logging level.
-
-        """
-
-        commands.SetServerLogging.run(self._connection, logger, log_level)
-
-    def call_static_method(self, type_name, method_name, assembly, parameters=None, type_of_parameters=None):
-        """Invoke a static method from your application.
-
-        Args:
-            type_name (:obj:`str`): The name of the script. If the script has a namespace the format should look like
-                this: ``"namespace.typeName"``.
-            method_name (:obj:`str`): The name of the public method that we want to call. If the method is inside a
-                static property/field to be able to call that method, methodName need to be the following format
-                ``"propertyName.MethodName"``.
-            assembly (:obj:`str`): The name of the assembly containing the script.
-            parameters (:obj:`list`, :obj:`tuple`, optional): Defaults to ``None``.
-            type_of_parameters (:obj:`list`, :obj:`tuple`, optional): Defaults to ``None``.
-
-        Return:
-            str: The value returned by the method is serialized to a JSON string.
-
-        """
-
-        return commands.CallMethod.run(
-            self._connection,
-            type_name, method_name, parameters=parameters, type_of_parameters=type_of_parameters, assembly=assembly
-        )
-
-    def get_current_scene(self):
-        """Returns the name of the current scene.
-
-        Returns:
-            str: The name of the current scene.
-
-        """
-
-        return commands.GetCurrentScene.run(self._connection)
-
-    def load_scene(self, scene_name, load_single=True):
-        """Loads a scene.
-
-        Args:
-            scene_name (:obj:`str`): The name of the scene to be loaded.
-            load_single (:obj`bool`, optional): Sets the loading mode. If set to ``False`` the scene will be loaded
-                additive, together with the current loaded scenes. Defaults to ``True``.
-
-        """
-
-        commands.LoadScene.run(
-            self._connection,
-            scene_name, load_single
-        )
-
-    def wait_for_current_scene_to_be(self, scene_name, timeout=30, interval=1):
-        """Waits for the scene to be loaded for a specified amount of time.
-
-        Args:
-            scene_name (:obj:`str`): The name of the scene to wait for.
-            timeout (obj:`int`, :obj:`float`, optional): The time measured in seconds to wait for the specified scene.
-                Defaults to ``30``.
-            interval (obj:`int`, :obj:`float`, optional): How often to check that the scene was loaded in the given
-                timeout. Defaults to ``1``.
-
-        Returns:
-            str: The name of the loaded scene.
-
-        """
-
-        return commands.WaitForCurrentSceneToBe.run(
-            self._connection,
-            scene_name, timeout, interval
-        )
-
-    def unload_scene(self, scene_name):
-        """Unloads a scene.
-
-        Args:
-            scene_name (:obj:`str`): The name of the scene to be unloaded.
-
-        """
-
-        commands.UnloadScene.run(self._connection, scene_name)
-
-    def get_all_loaded_scenes(self):
-        """Returns all the scenes that have been loaded.
-
-        Returns:
-            :obj:`list` of :obj:`str`: A list containing the names of all the loaded scenes.
-
-        """
-
-        return commands.GetAllLoadedScenes.run(self._connection)
-
-    def get_time_scale(self):
-        """Returns the value of the time scale.
-
-        Returns:
-            float: The value of the time scale.
-
-        """
-
-        return commands.GetTimeScale.run(self._connection)
-
-    def set_time_scale(self, time_scale):
-        """Sets the value of the time scale.
-
-        Args:
-            time_scale (:obj:`float`, :obj:`int`): The value of the time scale.
-
-        """
-
-        commands.SetTimeScale.run(self._connection, time_scale)
-
-    def get_player_pref_key(self, key_name, key_type):
-        """Returns the value for a given key from PlayerPrefs.
-
-        Args:
-            key_name (:obj:`str`): The name of the key to be retrived.
-            key_type (:obj:`PlayerPrefKeyType`): The type of the key.
-
-        """
-
-        return commands.GetPlayerPrefKey.run(
-            self._connection,
-            key_name, key_type
-        )
-
-    def set_player_pref_key(self, key_name, value, key_type):
-        """Sets the value for a given key in PlayerPrefs.
-
-        Args:
-            key_name (:obj:`str`): The name of the key to be set.
-            value (:obj:`str`): The new value of be set.
-            key_type (:obj:`PlayerPrefKeyType`): The type of the key.
-
-        """
-
-        commands.SetPlayerPrefKey.run(
-            self._connection,
-            key_name, value, key_type
-        )
-
-    def delete_player_pref_key(self, key_name):
-        """Removes a key and its corresponding value from PlayerPrefs.
-
-        Args:
-            key_name (:obj:`str`): The name of the key to be deleted.
-
-        """
-
-        commands.DeletePlayerPrefKey.run(self._connection, key_name)
-
-    def delete_player_pref(self):
-        """Removes all keys and values from PlayerPref."""
-
-        commands.DeletePlayerPref.run(self._connection)
-
-    def find_object(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
-        """Finds the first object in the scene that respects the given criteria.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the object.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            AltObject: The object.
-
-        """
-
-        data = commands.FindObject.run(
-            self._connection,
-            by, value, camera_by, camera_value, enabled
-        )
-
-        return self._get_alt_object(data)
-
-    def find_objects(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
-        """Finds all objects in the scene that respects the given criteria.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the objects.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            list of AltObject: The list of objects.
-
-        """
-
-        data = commands.FindObjects.run(
-            self._connection,
-            by, value, camera_by, camera_value, enabled
-        )
-
-        return self._get_alt_objects(data)
-
-    def find_object_which_contains(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
-        """Finds the first object in the scene that respects the given criteria.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the object.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            AltObject: The object.
-
-        """
-
-        data = commands.FindObjectWhichContains.run(
-            self._connection,
-            by, value, camera_by, camera_value, enabled
-        )
-
-        return self._get_alt_object(data)
-
-    def find_objects_which_contain(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
-        """Finds all objects in the scene that respects the given criteria.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the objects.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            enabled (:obj:`bool`): If ``True`` will match only objects that are active in hierarchy. If ``False`` will
-                match all objects. Defaults to ``True``.
-
-        Returns:
-            list of AltObjects: The list of objects.
-
-        """
-
-        data = commands.FindObjectsWhichContain.run(
-            self._connection,
-            by, value, camera_by, camera_value, enabled
-        )
-
-        return self._get_alt_objects(data)
-
-    def wait_for_object(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5, enabled=True):
-        """Waits until it finds an object that respects the given criteria or until timeout limit is reached.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the object.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
-            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
-                object again. The interval should be smaller than the timeout.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            AltObject: The object.
-
-        """
-
-        data = commands.WaitForObject.run(
-            self._connection,
-            by, value, camera_by, camera_value, timeout, interval, enabled
-        )
-
-        return self._get_alt_object(data)
-
-    def wait_for_object_which_contains(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5,
-                                       enabled=True):
-        """Waits until it finds an object that respects the given criteria or time runs out and will throw an error.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the object.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
-            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
-                object again. The interval should be smaller than the timeout.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            AltObject: The object.
-
-        """
-
-        data = commands.WaitForObjectWhichContains.run(
-            self._connection,
-            by, value, camera_by, camera_value, timeout, interval, enabled
-        )
-
-        return self._get_alt_object(data)
-
-    def wait_for_object_to_not_be_present(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5,
-                                          enabled=True):
-        """Waits until the object in the scene that respects the given criteria is no longer in the scene or until
-        timeout limit is reached.
-
-        Args:
-            by (:obj:`By`): Sets what criteria to use in order to find the object.
-            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
-                not.
-            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
-            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
-                object again. The interval should be smaller than the timeout.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        """
-
-        commands.WaitForObjectToNotBePresent.run(
-            self._connection,
-            by, value, camera_by, camera_value, timeout, interval, enabled
-        )
-
-    def get_all_elements(self, camera_by=By.NAME, camera_value="", enabled=True):
-        """Returns information about every objects loaded in the currently loaded scenes. This also means objects that
-        are set as DontDestroyOnLoad.
-
-        Args:
-            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
-            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
-                see if they respect the criteria or not. If no camera is given it will search through all camera that
-                are in the scene until some camera sees the object or return the screen coordinate of the object
-                calculated to the last camera in the scene.
-            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
-                ``False`` will match all objects. Defaults to ``True``.
-
-        Returns:
-            list of AltObjects: The list of objects.
-
-        """
-
-        return self.find_objects(By.PATH, "//*", camera_by=camera_by, camera_value=camera_value, enabled=enabled)
-
-    def move_mouse(self, coordinates, duration=0.1, wait=True):
-        """Simulates mouse movement in your application.
-
-        Args:
-            coordinates (:obj:`dict`): The screen coordinates
-            duration (:obj:`int`, optional): The time measured in seconds to move the mouse from current position to
-                the set location. Defaults to ``0.1``
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.MoveMouse.run(self._connection, coordinates, duration, wait)
-
-    def scroll(self, speed_vertical=1, duration=0.1, wait=True, speed_horizontal=1):
-        """Simulate scroll mouse action in your application.
-
-        Args:
-            speed_vertical (:obj:`int`, :obj:`float`): Set how fast to scroll. Positive values will scroll up and
-                negative values will scroll down. Defaults to ``1``
-            duration (:obj:`int`, :obj:`float`, optional): The duration of the scroll in seconds. Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-            speed_horizontal (:obj:`int`, :obj:`float`): Set how fast to scroll right or left. Defaults to ``1``
-
-        """
-
-        commands.Scroll.run(
-            self._connection,
-            speed_vertical, duration,
-            wait, speed_horizontal
-        )
-
-    def click(self, coordinates, count=1, interval=0.1, wait=True):
-        """Click at screen coordinates.
-
-        Args:
-            coordinates (:obj:`dict`): The screen coordinates.
-            count (:obj:`int`, optional): Number of taps. Defaults to ``1``.
-            interval (:obj:`int`, :obj:`float`, optional): The interval between taps in seconds. Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set to ``True`` Wait for command to finish.
-
-        """
-
-        commands.ClickCoordinates.run(self._connection, coordinates, count, interval, wait)
-
-    def key_down(self, key_code, power=1):
-        """Simulates that a specific key was pressed without taking into consideration the duration of the press.
-
-        Args:
-            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be pressed.
-            power (:obj:`float`, optional): A value between [-1,1] used for joysticks to indicate how hard the button
-                was pressed. Defaults to ``1``.
-
-        """
-
-        self.keys_down([key_code], power=power)
-
-    def keys_down(self, key_codes, power=1):
-        """Simulates that multiple keys were pressed without taking into consideration the duration of the press.
-
-        Args:
-            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be pressed.
-            power (:obj:`float`): A value between [-1,1] used for joysticks to indicate how hard the button was
-                pressed. Defaults to ``1``.
-
-        """
-
-        commands.KeysDown.run(self._connection, key_codes, power)
-
-    def key_up(self, key_code):
-        """Simulates that a specific key was released.
-
-        Args:
-            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be released.
-
-        """
-
-        self.keys_up([key_code])
-
-    def keys_up(self, key_codes):
-        """Simulates that multiple keys were released.
-
-        Args:
-            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be released.
-
-        """
-
-        commands.KeysUp.run(self._connection, key_codes)
-
-    def press_key(self, key_code, power=1, duration=0.1, wait=True):
-        """Simulates key press action in your application.
-
-        Args:
-            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be pressed.
-            power (:obj:`int`, :obj:`float`, optional): A value between [-1,1] used for joysticks to indicate how hard
-                the button was pressed. Defaults to ``1``.
-            duration (:obj:`float`, optional): The time measured in seconds from the key press to the key release.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        self.press_keys([key_code], power=power, duration=duration, wait=wait)
-
-    def press_keys(self, key_codes, power=1, duration=0.1, wait=True):
-        """Simulates multiple keypress action in your application.
-
-        Args:
-            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be pressed.
-            power (:obj:`float`): A value between [-1,1] used for joysticks to indicate how hard the buttons were
-                pressed. Defaults to ``1``.
-            duration (:obj:`float`): The time measured in seconds from the key press to the key release.
-            wait (:obj:`bool`): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.PressKeys.run(self._connection, key_codes, power, duration, wait)
-
-    def begin_touch(self, coordinates):
-        """Simulates starting of a touch on the screen.
-
-        Args:
-            coordinates (:obj:`dict`): The screen coordinates.
-
-        Returns:
-            str: A ``finger_id`` to use with ``move_touch`` and ``end_touch``.
-
-        """
-
-        return commands.BeginTouch.run(self._connection, coordinates)
-
-    def move_touch(self, finger_id, coordinates):
-        """Simulates a touch movement on the screen. Move the touch created with ``begin_touch`` from the previous
-        position to the position given as parameters.
-
-        Args:
-            finger_id (:obj:`str`): The value returned by ``begin_touch``.
-            coordinates (:obj:`dict`): Screen coordinates where the touch will be moved.
-
-        """
-
-        commands.MoveTouch.run(self._connection, finger_id, coordinates)
-
-    def end_touch(self, finger_id):
-        """Simulates ending of a touch on the screen. This command will destroy the touch making it no longer usable to
-        other movements.
-
-        Args:
-            finger_id (:obj:`str`): The value returned by ``begin_touch``.
-
-        """
-
-        commands.EndTouch.run(self._connection, finger_id)
-
-    def swipe(self, start, end, duration=0.1, wait=True):
-        """Simulates a swipe action between two points.
-
-        Args:
-            start (:obj:`dict`): Coordinates of the screen where the swipe begins.
-            end (:obj:`dict`): Coordinates of the screen where the swipe ends.
-            duration (:obj:`int`, :obj:`float`, optional): The time measured in seconds to move the mouse from start to
-                end location. Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.Swipe.run(
-            self._connection,
-            start, end, duration, wait
-        )
-
-    def multipoint_swipe(self, positions, duration=0.1, wait=True):
-        """Simulates a multipoint swipe action.
-
-        Args:
-            positions (:obj:`List[dict]`): A list of positions on the screen where the swipe be made.
-            duration (:obj:`float`): The time measured in seconds to swipe from first position to the last position.
-                Defaults to ``0.1``.
-            wait (:obj:`bool`): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.MultipointSwipe.run(self._connection, positions, duration, wait)
-
-    def tap(self, coordinates, count=1, interval=0.1, wait=True):
-        """Tap at screen coordinates.
-
-        Args:
-            coordinates (:obj:`dict`): The screen coordinates.
-            count (:obj:`int`, optional): Number of taps. Defaults to ``1``.
-            interval (:obj:`int`, :obj:`float`, optional): The interval between taps in seconds. Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.TapCoordinates.run(self._connection, coordinates, count, interval, wait)
-
-    def tilt(self, acceleration, duration=0.1, wait=True):
-        """Simulates device rotation action in your application.
-
-        Args:
-            acceleration (:obj:`dict`): The linear acceleration of a device.
-            duration (:obj:`int`, :obj:`float`, optional): How long the rotation will take in seconds.
-                Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        commands.Tilt.run(self._connection, acceleration, duration, wait)
-
-    def get_application_screensize(self):
-        screen_width = self.call_static_method(
-            "UnityEngine.Screen", "get_width",
-            "UnityEngine.CoreModule"
-        )
-        screen_height = self.call_static_method(
-            "UnityEngine.Screen", "get_height",
-            "UnityEngine.CoreModule"
-        )
-        return (screen_width, screen_height)
-
-    def get_png_screenshot(self, path):
-        """Creates a screenshot of the current scene in png format at the given path.
-
-        Args:
-            path (:obj:`str`): The path where the image will be created.
-
-        """
-
-        commands.GetPNGScreenshot.run(self._connection, path)
-
-    def hold_button(self, coordinates, duration=0.1, wait=True):
-        """Simulates holding left click button down for a specified amount of time at given coordinates.
-
-        Args:
-            coordinates (:obj:`dict`): The coordinates where the button is held down
-            duration ((:obj:`int`, :obj:`float`, optional): The time measured in seconds to keep the button down.
-                Defaults to ``0.1``.
-            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
-
-        """
-
-        return commands.Swipe.run(
-            self._connection,
-            coordinates, coordinates, duration, wait
-        )
-
-    def get_static_property(self, component_name, property_name, assembly, max_depth=2):
-        """Returns the value of the static field or property given as parameter.
-
-        Args:
-            component_name (:obj:`str`): The name of the component containing the field or property
-                to be retrieved.
-            property_name (:obj:`str`): The name of the field or property to be retrieved.
-            assembly (:obj:`str`): The name of the assembly containing the component mentioned above.
-            max_depth (:obj:`int`, optional): The value determining how deep to go in the hierarchy of objects
-                to find the field or property.
-
-        """
-
-        return commands.GetStaticProperty.run(
-            self._connection,
-            component_name, property_name, assembly, max_depth
-        )
-
-    def set_static_property(self, component_name, property_name, assembly, updated_value):
-        """Set the value of the static field or property given as parameter.
-
-        Args:
-            component_name (:obj:`str`): The name of the component containing the field or property
-                to be retrieved.
-            property_name (:obj:`str`): The name of the field or property to be retrieved.
-            assembly (:obj:`str`): The name of the assembly containing the component mentioned above.
-            updated_value (:obj:`str`): The value of the field or property to be updated.
-        """
-
-        return commands.SetStaticProperty.run(
-            self._connection,
-            component_name, property_name, assembly, updated_value
-        )
-
-    def find_object_at_coordinates(self, coordinates):
-        """Retrieves the Unity object at given coordinates
-
-        Uses EventSystem.RaycastAll to find object. If no object is found then it uses UnityEngine.Physics.Raycast
-        and UnityEngine.Physics2D.Raycast and returns the one closer to the camera.
-
-        Args:
-            coordinates (:obj:`dict`): The screen coordinates.
-
-        Returns:
-            AltObject: The UI object hit by event system Raycast, ``None`` otherwise.
-
-        """
-
-        data = commands.FindObjectAtCoordinates.run(self._connection, coordinates)
-        return self._get_alt_object(data)
-
-    def add_notification_listener(self, notification_type, notification_callback, overwrite=True):
-        """Activates a notification that the tester will send.
-
-        Args:
-            notification_type (:obj:`int`): Flag that indicates which notification to be turned on.
-            notification_callback (:obj:`method`): callback used when a notification is received.
-            overwrite (:obj:'bool', optional): Flag to set if the new callback will overwrite the other
-                callbacks or just append.
-
-        """
-
-        commands.AddNotificationListener.run(self._connection, notification_type, notification_callback, overwrite)
-
-    def remove_notification_listener(self, notification_type):
-        """Clear list of callback for the notification type and turn off the notification in tester.
-
-        Args:
-            notification_type (:obj:`int`): Flag that indicates which notification to be turned off.
-
-        """
-
-        commands.RemoveNotificationListener.run(self._connection, notification_type)
-
-    def reset_input(self):
-        """Clear all active input actions simulated by AltTester."""
-
-        commands.ResetInput.run(self._connection)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import warnings
+import sys
+
+from loguru import logger
+
+import alttester.commands as commands
+from alttester.commands.base_command import Command
+from alttester.__version__ import VERSION
+from alttester._websocket import WebsocketConnection, CommandHandler, NotificationHandler
+from alttester.altobject import AltObject
+from alttester.by import By
+
+
+warnings.filterwarnings("default", category=DeprecationWarning, module=__name__)
+
+
+class AltDriver:
+    """The driver object will help interacting with all the application objects, their properties and methods.
+
+    When you instantiate an ``AltDriver`` object in your tests, you can use it to “drive” your application like one of
+    your users would, by interacting with all the application objects, their properties and methods.  An ``AltDriver``
+    instance will connect to the AltTester® Server.
+
+    Args:
+        host (:obj:`str`, optional): The host to connect to.
+        port (:obj:`int`, optional): The port to connect to.
+        app_name (:obj:`str`, optional): The application name. Defaults to ``__default__``.
+        enable_logging (:obj:`bool`, optional): If set to ``True`` will turn on logging, by default logging is disabled.
+        timeout (:obj:`int`, :obj:`float`, optional): The timeout duration for establishing a connection, in seconds.
+            If set to ``None``, the connection attempt will wait indefinitely. The default value is ``60`` seconds.
+
+    """
+
+    def __init__(
+        self,
+        host="127.0.0.1",
+        port=13000,
+        app_name="__default__",
+        enable_logging=False,
+        timeout=60,
+        platform="unknown",
+        platform_version="unknown",
+        device_instance_id="unknown",
+        app_id="unknown"
+    ):
+        self.host = host
+        self.port = port
+        self.app_name = app_name
+        self.enable_logging = enable_logging
+        self.timeout = timeout
+        self.platform = platform
+        self.platform_version = platform_version
+        self.device_instance_id = device_instance_id
+        self.app_id = app_id
+
+        self._config_logging(self.enable_logging)
+
+        logger.debug(
+            "Connecting to AltTester® on host: '{}', port: '{}' and app name: '{}'.",
+            self.host,
+            self.port,
+            self.app_name
+        )
+
+        self._command_handler = CommandHandler()
+        self._notification_handler = NotificationHandler()
+        self._connection = WebsocketConnection(
+            host=self.host,
+            port=self.port,
+            timeout=self.timeout,
+            path="altws",
+            params={
+                "appName": self.app_name,
+                "platform": self.platform,
+                "platformVersion": self.platform_version,
+                "deviceInstanceId": self.device_instance_id,
+                "appId": self.app_id,
+                "driverType": "SDK"
+            },
+            command_handler=self._command_handler,
+            notification_handler=self._notification_handler
+        )
+        self._connection.connect()
+        self._check_server_version()
+
+    def __repr__(self):
+        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
+            self.__class__.__name__,
+            self.host,
+            self.port,
+            self.app_name,
+            self.enable_logging,
+            self.timeout
+        )
+
+    @staticmethod
+    def _config_logging(enable_logging):
+        if enable_logging:
+            logger.configure(
+                handlers=[
+                    dict(sink=sys.stdout, diagnose=False),
+                    dict(sink="./AltTester.log", enqueue=False, serialize=True, mode="w", diagnose=False),
+                ],
+                levels=[dict(name="DEBUG")],
+                activation=[("alttester", True)],
+            )
+        else:
+            logger.disable("alttester")
+
+    @staticmethod
+    def _split_version(version):
+        parts = version.split(".")
+        return (parts[0], parts[1]) if len(parts) > 1 else ("", "")
+
+    def _check_server_version(self):
+        server_version = commands.GetServerVersion.run(self._connection)
+        logger.info("Connection established with instrumented Unity app. AltTester® Version: {}", server_version)
+
+        major_server, minor_server = self._split_version(server_version)
+        major_driver, minor_driver = self._split_version(VERSION)
+
+        if major_server != major_driver or minor_server != minor_driver:
+            message = "Version mismatch. AltDriver version is {}. AltTester® version is {}.".format(
+                VERSION,
+                server_version
+            )
+
+            logger.warning(message)
+
+    def _get_alt_object(self, data):
+        if data is None:
+            return None
+
+        alt_object = AltObject(self, data)
+
+        logger.debug(
+            "Element {} found at x: {} y: {} mobileY: {}",
+            alt_object.name,
+            alt_object.x,
+            alt_object.y,
+            alt_object.mobileY
+        )
+
+        return alt_object
+
+    def _get_alt_objects(self, data):
+        if data is None:
+            return None
+
+        alt_objects = []
+
+        for element in data:
+            alt_object = AltObject(self, element)
+            alt_objects.append(alt_object)
+
+            logger.debug(
+                "Element {} found at x: {} y: {} mobileY: {}",
+                alt_object.name,
+                alt_object.x,
+                alt_object.y,
+                alt_object.mobileY
+            )
+
+        return alt_objects
+
+    def stop(self):
+        """Close the connection to AltTester."""
+
+        self._connection.close()
+
+    def get_command_response_timeout(self):
+        """Gets the current command response timeout for the AltTester® connection.
+
+        Return:
+            int or float: The current command response time.
+
+        """
+
+        return self._connection.set_command_timeout()
+
+    def set_command_response_timeout(self, timeout):
+        """Sets the command response timeout for the AltTester® connection.
+
+        Args:
+            timeout (:obj:`int` or :obj:`float`): The new command response timeout in seconds.
+
+        """
+
+        self._connection.set_command_timeout(timeout)
+
+    def get_delay_after_command(self):
+        """Gets the current delay after a command."""
+
+        return Command.get_delay_after_command()
+
+    def set_delay_after_command(self, delay):
+        """Set the delay after a command.
+
+        Args:
+            delay (:obj:`int` or :obj:`float`): The new delay a after a command.
+        """
+
+        Command.set_delay_after_command(delay)
+
+    def set_server_logging(self, logger, log_level):
+        """Sets the level of logging on AltTester.
+
+        Args:
+            logger (:obj:`AltLogger`): The type of logger.
+            log_lever (:obj:`AltLogLevel`): The logging level.
+
+        """
+
+        commands.SetServerLogging.run(self._connection, logger, log_level)
+
+    def call_static_method(self, type_name, method_name, assembly, parameters=None, type_of_parameters=None):
+        """Invoke a static method from your application.
+
+        Args:
+            type_name (:obj:`str`): The name of the script. If the script has a namespace the format should look like
+                this: ``"namespace.typeName"``.
+            method_name (:obj:`str`): The name of the public method that we want to call. If the method is inside a
+                static property/field to be able to call that method, methodName need to be the following format
+                ``"propertyName.MethodName"``.
+            assembly (:obj:`str`): The name of the assembly containing the script.
+            parameters (:obj:`list`, :obj:`tuple`, optional): Defaults to ``None``.
+            type_of_parameters (:obj:`list`, :obj:`tuple`, optional): Defaults to ``None``.
+
+        Return:
+            str: The value returned by the method is serialized to a JSON string.
+
+        """
+
+        return commands.CallMethod.run(
+            self._connection,
+            type_name, method_name, parameters=parameters, type_of_parameters=type_of_parameters, assembly=assembly
+        )
+
+    def get_current_scene(self):
+        """Returns the name of the current scene.
+
+        Returns:
+            str: The name of the current scene.
+
+        """
+
+        return commands.GetCurrentScene.run(self._connection)
+
+    def load_scene(self, scene_name, load_single=True):
+        """Loads a scene.
+
+        Args:
+            scene_name (:obj:`str`): The name of the scene to be loaded.
+            load_single (:obj`bool`, optional): Sets the loading mode. If set to ``False`` the scene will be loaded
+                additive, together with the current loaded scenes. Defaults to ``True``.
+
+        """
+
+        commands.LoadScene.run(
+            self._connection,
+            scene_name, load_single
+        )
+
+    def wait_for_current_scene_to_be(self, scene_name, timeout=30, interval=1):
+        """Waits for the scene to be loaded for a specified amount of time.
+
+        Args:
+            scene_name (:obj:`str`): The name of the scene to wait for.
+            timeout (obj:`int`, :obj:`float`, optional): The time measured in seconds to wait for the specified scene.
+                Defaults to ``30``.
+            interval (obj:`int`, :obj:`float`, optional): How often to check that the scene was loaded in the given
+                timeout. Defaults to ``1``.
+
+        Returns:
+            str: The name of the loaded scene.
+
+        """
+
+        return commands.WaitForCurrentSceneToBe.run(
+            self._connection,
+            scene_name, timeout, interval
+        )
+
+    def unload_scene(self, scene_name):
+        """Unloads a scene.
+
+        Args:
+            scene_name (:obj:`str`): The name of the scene to be unloaded.
+
+        """
+
+        commands.UnloadScene.run(self._connection, scene_name)
+
+    def get_all_loaded_scenes(self):
+        """Returns all the scenes that have been loaded.
+
+        Returns:
+            :obj:`list` of :obj:`str`: A list containing the names of all the loaded scenes.
+
+        """
+
+        return commands.GetAllLoadedScenes.run(self._connection)
+
+    def get_time_scale(self):
+        """Returns the value of the time scale.
+
+        Returns:
+            float: The value of the time scale.
+
+        """
+
+        return commands.GetTimeScale.run(self._connection)
+
+    def set_time_scale(self, time_scale):
+        """Sets the value of the time scale.
+
+        Args:
+            time_scale (:obj:`float`, :obj:`int`): The value of the time scale.
+
+        """
+
+        commands.SetTimeScale.run(self._connection, time_scale)
+
+    def get_player_pref_key(self, key_name, key_type):
+        """Returns the value for a given key from PlayerPrefs.
+
+        Args:
+            key_name (:obj:`str`): The name of the key to be retrived.
+            key_type (:obj:`PlayerPrefKeyType`): The type of the key.
+
+        """
+
+        return commands.GetPlayerPrefKey.run(
+            self._connection,
+            key_name, key_type
+        )
+
+    def set_player_pref_key(self, key_name, value, key_type):
+        """Sets the value for a given key in PlayerPrefs.
+
+        Args:
+            key_name (:obj:`str`): The name of the key to be set.
+            value (:obj:`str`): The new value of be set.
+            key_type (:obj:`PlayerPrefKeyType`): The type of the key.
+
+        """
+
+        commands.SetPlayerPrefKey.run(
+            self._connection,
+            key_name, value, key_type
+        )
+
+    def delete_player_pref_key(self, key_name):
+        """Removes a key and its corresponding value from PlayerPrefs.
+
+        Args:
+            key_name (:obj:`str`): The name of the key to be deleted.
+
+        """
+
+        commands.DeletePlayerPrefKey.run(self._connection, key_name)
+
+    def delete_player_pref(self):
+        """Removes all keys and values from PlayerPref."""
+
+        commands.DeletePlayerPref.run(self._connection)
+
+    def find_object(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
+        """Finds the first object in the scene that respects the given criteria.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the object.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            AltObject: The object.
+
+        """
+
+        data = commands.FindObject.run(
+            self._connection,
+            by, value, camera_by, camera_value, enabled
+        )
+
+        return self._get_alt_object(data)
+
+    def find_objects(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
+        """Finds all objects in the scene that respects the given criteria.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the objects.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            list of AltObject: The list of objects.
+
+        """
+
+        data = commands.FindObjects.run(
+            self._connection,
+            by, value, camera_by, camera_value, enabled
+        )
+
+        return self._get_alt_objects(data)
+
+    def find_object_which_contains(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
+        """Finds the first object in the scene that respects the given criteria.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the object.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            AltObject: The object.
+
+        """
+
+        data = commands.FindObjectWhichContains.run(
+            self._connection,
+            by, value, camera_by, camera_value, enabled
+        )
+
+        return self._get_alt_object(data)
+
+    def find_objects_which_contain(self, by, value, camera_by=By.NAME, camera_value="", enabled=True):
+        """Finds all objects in the scene that respects the given criteria.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the objects.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            enabled (:obj:`bool`): If ``True`` will match only objects that are active in hierarchy. If ``False`` will
+                match all objects. Defaults to ``True``.
+
+        Returns:
+            list of AltObjects: The list of objects.
+
+        """
+
+        data = commands.FindObjectsWhichContain.run(
+            self._connection,
+            by, value, camera_by, camera_value, enabled
+        )
+
+        return self._get_alt_objects(data)
+
+    def wait_for_object(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5, enabled=True):
+        """Waits until it finds an object that respects the given criteria or until timeout limit is reached.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the object.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`, optional): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
+            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
+                object again. The interval should be smaller than the timeout.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            AltObject: The object.
+
+        """
+
+        data = commands.WaitForObject.run(
+            self._connection,
+            by, value, camera_by, camera_value, timeout, interval, enabled
+        )
+
+        return self._get_alt_object(data)
+
+    def wait_for_object_which_contains(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5,
+                                       enabled=True):
+        """Waits until it finds an object that respects the given criteria or time runs out and will throw an error.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the object.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
+            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
+                object again. The interval should be smaller than the timeout.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            AltObject: The object.
+
+        """
+
+        data = commands.WaitForObjectWhichContains.run(
+            self._connection,
+            by, value, camera_by, camera_value, timeout, interval, enabled
+        )
+
+        return self._get_alt_object(data)
+
+    def wait_for_object_to_not_be_present(self, by, value, camera_by=By.NAME, camera_value="", timeout=20, interval=0.5,
+                                          enabled=True):
+        """Waits until the object in the scene that respects the given criteria is no longer in the scene or until
+        timeout limit is reached.
+
+        Args:
+            by (:obj:`By`): Sets what criteria to use in order to find the object.
+            value (:obj:`str`): The value to which an object will be compared to see if they respect the criteria or
+                not.
+            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            timeout (:obj:`int`, :obj:`float`, optional): The number of seconds that it will wait for object.
+            interval (:obj:`int`, :obj:`float`, optional): The number of seconds after which it will try to find the
+                object again. The interval should be smaller than the timeout.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        """
+
+        commands.WaitForObjectToNotBePresent.run(
+            self._connection,
+            by, value, camera_by, camera_value, timeout, interval, enabled
+        )
+
+    def get_all_elements(self, camera_by=By.NAME, camera_value="", enabled=True):
+        """Returns information about every objects loaded in the currently loaded scenes. This also means objects that
+        are set as DontDestroyOnLoad.
+
+        Args:
+            camera_by (:obj:`By`): Set what criteria to use in order to find the camera.
+            camera_value (:obj:`str`, optional): The value to which all the cameras in the scene will be compared to
+                see if they respect the criteria or not. If no camera is given it will search through all camera that
+                are in the scene until some camera sees the object or return the screen coordinate of the object
+                calculated to the last camera in the scene.
+            enabled (:obj:`bool`, optional): If ``True`` will match only objects that are active in hierarchy. If
+                ``False`` will match all objects. Defaults to ``True``.
+
+        Returns:
+            list of AltObjects: The list of objects.
+
+        """
+
+        return self.find_objects(By.PATH, "//*", camera_by=camera_by, camera_value=camera_value, enabled=enabled)
+
+    def move_mouse(self, coordinates, duration=0.1, wait=True):
+        """Simulates mouse movement in your application.
+
+        Args:
+            coordinates (:obj:`dict`): The screen coordinates
+            duration (:obj:`int`, optional): The time measured in seconds to move the mouse from current position to
+                the set location. Defaults to ``0.1``
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.MoveMouse.run(self._connection, coordinates, duration, wait)
+
+    def scroll(self, speed_vertical=1, duration=0.1, wait=True, speed_horizontal=1):
+        """Simulate scroll mouse action in your application.
+
+        Args:
+            speed_vertical (:obj:`int`, :obj:`float`): Set how fast to scroll. Positive values will scroll up and
+                negative values will scroll down. Defaults to ``1``
+            duration (:obj:`int`, :obj:`float`, optional): The duration of the scroll in seconds. Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+            speed_horizontal (:obj:`int`, :obj:`float`): Set how fast to scroll right or left. Defaults to ``1``
+
+        """
+
+        commands.Scroll.run(
+            self._connection,
+            speed_vertical, duration,
+            wait, speed_horizontal
+        )
+
+    def click(self, coordinates, count=1, interval=0.1, wait=True):
+        """Click at screen coordinates.
+
+        Args:
+            coordinates (:obj:`dict`): The screen coordinates.
+            count (:obj:`int`, optional): Number of taps. Defaults to ``1``.
+            interval (:obj:`int`, :obj:`float`, optional): The interval between taps in seconds. Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set to ``True`` Wait for command to finish.
+
+        """
+
+        commands.ClickCoordinates.run(self._connection, coordinates, count, interval, wait)
+
+    def key_down(self, key_code, power=1):
+        """Simulates that a specific key was pressed without taking into consideration the duration of the press.
+
+        Args:
+            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be pressed.
+            power (:obj:`float`, optional): A value between [-1,1] used for joysticks to indicate how hard the button
+                was pressed. Defaults to ``1``.
+
+        """
+
+        self.keys_down([key_code], power=power)
+
+    def keys_down(self, key_codes, power=1):
+        """Simulates that multiple keys were pressed without taking into consideration the duration of the press.
+
+        Args:
+            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be pressed.
+            power (:obj:`float`): A value between [-1,1] used for joysticks to indicate how hard the button was
+                pressed. Defaults to ``1``.
+
+        """
+
+        commands.KeysDown.run(self._connection, key_codes, power)
+
+    def key_up(self, key_code):
+        """Simulates that a specific key was released.
+
+        Args:
+            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be released.
+
+        """
+
+        self.keys_up([key_code])
+
+    def keys_up(self, key_codes):
+        """Simulates that multiple keys were released.
+
+        Args:
+            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be released.
+
+        """
+
+        commands.KeysUp.run(self._connection, key_codes)
+
+    def press_key(self, key_code, power=1, duration=0.1, wait=True):
+        """Simulates key press action in your application.
+
+        Args:
+            key_code (:obj:`AltKeyCode`): The key code of the key simulated to be pressed.
+            power (:obj:`int`, :obj:`float`, optional): A value between [-1,1] used for joysticks to indicate how hard
+                the button was pressed. Defaults to ``1``.
+            duration (:obj:`float`, optional): The time measured in seconds from the key press to the key release.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        self.press_keys([key_code], power=power, duration=duration, wait=wait)
+
+    def press_keys(self, key_codes, power=1, duration=0.1, wait=True):
+        """Simulates multiple keypress action in your application.
+
+        Args:
+            key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be pressed.
+            power (:obj:`float`): A value between [-1,1] used for joysticks to indicate how hard the buttons were
+                pressed. Defaults to ``1``.
+            duration (:obj:`float`): The time measured in seconds from the key press to the key release.
+            wait (:obj:`bool`): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.PressKeys.run(self._connection, key_codes, power, duration, wait)
+
+    def begin_touch(self, coordinates):
+        """Simulates starting of a touch on the screen.
+
+        Args:
+            coordinates (:obj:`dict`): The screen coordinates.
+
+        Returns:
+            str: A ``finger_id`` to use with ``move_touch`` and ``end_touch``.
+
+        """
+
+        return commands.BeginTouch.run(self._connection, coordinates)
+
+    def move_touch(self, finger_id, coordinates):
+        """Simulates a touch movement on the screen. Move the touch created with ``begin_touch`` from the previous
+        position to the position given as parameters.
+
+        Args:
+            finger_id (:obj:`str`): The value returned by ``begin_touch``.
+            coordinates (:obj:`dict`): Screen coordinates where the touch will be moved.
+
+        """
+
+        commands.MoveTouch.run(self._connection, finger_id, coordinates)
+
+    def end_touch(self, finger_id):
+        """Simulates ending of a touch on the screen. This command will destroy the touch making it no longer usable to
+        other movements.
+
+        Args:
+            finger_id (:obj:`str`): The value returned by ``begin_touch``.
+
+        """
+
+        commands.EndTouch.run(self._connection, finger_id)
+
+    def swipe(self, start, end, duration=0.1, wait=True):
+        """Simulates a swipe action between two points.
+
+        Args:
+            start (:obj:`dict`): Coordinates of the screen where the swipe begins.
+            end (:obj:`dict`): Coordinates of the screen where the swipe ends.
+            duration (:obj:`int`, :obj:`float`, optional): The time measured in seconds to move the mouse from start to
+                end location. Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.Swipe.run(
+            self._connection,
+            start, end, duration, wait
+        )
+
+    def multipoint_swipe(self, positions, duration=0.1, wait=True):
+        """Simulates a multipoint swipe action.
+
+        Args:
+            positions (:obj:`List[dict]`): A list of positions on the screen where the swipe be made.
+            duration (:obj:`float`): The time measured in seconds to swipe from first position to the last position.
+                Defaults to ``0.1``.
+            wait (:obj:`bool`): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.MultipointSwipe.run(self._connection, positions, duration, wait)
+
+    def tap(self, coordinates, count=1, interval=0.1, wait=True):
+        """Tap at screen coordinates.
+
+        Args:
+            coordinates (:obj:`dict`): The screen coordinates.
+            count (:obj:`int`, optional): Number of taps. Defaults to ``1``.
+            interval (:obj:`int`, :obj:`float`, optional): The interval between taps in seconds. Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.TapCoordinates.run(self._connection, coordinates, count, interval, wait)
+
+    def tilt(self, acceleration, duration=0.1, wait=True):
+        """Simulates device rotation action in your application.
+
+        Args:
+            acceleration (:obj:`dict`): The linear acceleration of a device.
+            duration (:obj:`int`, :obj:`float`, optional): How long the rotation will take in seconds.
+                Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        commands.Tilt.run(self._connection, acceleration, duration, wait)
+
+    def get_application_screensize(self):
+        screen_width = self.call_static_method(
+            "UnityEngine.Screen", "get_width",
+            "UnityEngine.CoreModule"
+        )
+        screen_height = self.call_static_method(
+            "UnityEngine.Screen", "get_height",
+            "UnityEngine.CoreModule"
+        )
+        return (screen_width, screen_height)
+
+    def get_png_screenshot(self, path):
+        """Creates a screenshot of the current scene in png format at the given path.
+
+        Args:
+            path (:obj:`str`): The path where the image will be created.
+
+        """
+
+        commands.GetPNGScreenshot.run(self._connection, path)
+
+    def hold_button(self, coordinates, duration=0.1, wait=True):
+        """Simulates holding left click button down for a specified amount of time at given coordinates.
+
+        Args:
+            coordinates (:obj:`dict`): The coordinates where the button is held down
+            duration ((:obj:`int`, :obj:`float`, optional): The time measured in seconds to keep the button down.
+                Defaults to ``0.1``.
+            wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
+
+        """
+
+        return commands.Swipe.run(
+            self._connection,
+            coordinates, coordinates, duration, wait
+        )
+
+    def get_static_property(self, component_name, property_name, assembly, max_depth=2):
+        """Returns the value of the static field or property given as parameter.
+
+        Args:
+            component_name (:obj:`str`): The name of the component containing the field or property
+                to be retrieved.
+            property_name (:obj:`str`): The name of the field or property to be retrieved.
+            assembly (:obj:`str`): The name of the assembly containing the component mentioned above.
+            max_depth (:obj:`int`, optional): The value determining how deep to go in the hierarchy of objects
+                to find the field or property.
+
+        """
+
+        return commands.GetStaticProperty.run(
+            self._connection,
+            component_name, property_name, assembly, max_depth
+        )
+
+    def set_static_property(self, component_name, property_name, assembly, updated_value):
+        """Set the value of the static field or property given as parameter.
+
+        Args:
+            component_name (:obj:`str`): The name of the component containing the field or property
+                to be retrieved.
+            property_name (:obj:`str`): The name of the field or property to be retrieved.
+            assembly (:obj:`str`): The name of the assembly containing the component mentioned above.
+            updated_value (:obj:`str`): The value of the field or property to be updated.
+        """
+
+        return commands.SetStaticProperty.run(
+            self._connection,
+            component_name, property_name, assembly, updated_value
+        )
+
+    def find_object_at_coordinates(self, coordinates):
+        """Retrieves the Unity object at given coordinates
+
+        Uses EventSystem.RaycastAll to find object. If no object is found then it uses UnityEngine.Physics.Raycast
+        and UnityEngine.Physics2D.Raycast and returns the one closer to the camera.
+
+        Args:
+            coordinates (:obj:`dict`): The screen coordinates.
+
+        Returns:
+            AltObject: The UI object hit by event system Raycast, ``None`` otherwise.
+
+        """
+
+        data = commands.FindObjectAtCoordinates.run(self._connection, coordinates)
+        return self._get_alt_object(data)
+
+    def add_notification_listener(self, notification_type, notification_callback, overwrite=True):
+        """Activates a notification that the tester will send.
+
+        Args:
+            notification_type (:obj:`int`): Flag that indicates which notification to be turned on.
+            notification_callback (:obj:`method`): callback used when a notification is received.
+            overwrite (:obj:'bool', optional): Flag to set if the new callback will overwrite the other
+                callbacks or just append.
+
+        """
+
+        commands.AddNotificationListener.run(self._connection, notification_type, notification_callback, overwrite)
+
+    def remove_notification_listener(self, notification_type):
+        """Clear list of callback for the notification type and turn off the notification in tester.
+
+        Args:
+            notification_type (:obj:`int`): Flag that indicates which notification to be turned off.
+
+        """
+
+        commands.RemoveNotificationListener.run(self._connection, notification_type)
+
+    def reset_input(self):
+        """Clear all active input actions simulated by AltTester."""
+
+        commands.ResetInput.run(self._connection)
```

### Comparing `AltTester-Driver-2.0.3/alttester/by.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_current_scene.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from enum import Enum, unique
-
-"""The By implementation."""
-
-
-@unique
-class By(Enum):
-    """Set of supported locator strategies."""
-
-    NAME = 1
-    TAG = 2
-    LAYER = 3
-    COMPONENT = 4
-    ID = 5
-    PATH = 6
-    TEXT = 7
-
-    def __str__(self):
-        return self.name
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetCurrentScene(BaseCommand):
+
+    def __init__(self, connection):
+        super().__init__(connection, "getCurrentScene")
+
+    def execute(self):
+        data = self.send()
+        return data.get("name", "")
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/__init__.py` & `alttester_driver-2.1.0/tests/unit/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.AltTesterCommands.set_server_logging import *
-from alttester.commands.AltTesterCommands.add_notification_listener import *
-from alttester.commands.AltTesterCommands.remove_notification_listener import *
-from alttester.commands.AltTesterCommands.reset_input import *
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/add_notification_listener.py` & `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/add_notification_listener.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.Notifications.notification_type import NotificationType
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class AddNotificationListener(BaseCommand):
-
-    def __init__(self, connection, notification_type, notification_callback, overwrite):
-        super().__init__(connection, "activateNotification")
-
-        if notification_type not in NotificationType:
-            raise InvalidParameterTypeException(
-                parameter_name='notification_type',
-                expected_types=[NotificationType],
-                received_type=type(notification_type)
-            )
-        self.notification_type = notification_type
-
-        if type(notification_callback) == "method":
-            raise InvalidParameterTypeException(
-                parameter_name='notification_callback',
-                expected_types=[callable],
-                received_type=type(notification_callback)
-            )
-        self.notification_callback = notification_callback
-
-        if type(overwrite) == "bool":
-            raise InvalidParameterTypeException(
-                parameter_name='overwrite',
-                expected_types=[bool],
-                received_type=type(overwrite)
-            )
-        self.overwrite = overwrite
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "notificationType": str(int(self.notification_type)),
-        })
-
-        return parameters
-
-    def execute(self):
-        self.connection._notification_handler.add_notification_listener(
-            self.notification_type,
-            self.notification_callback,
-            self.overwrite
-        )
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.Notifications.notification_type import NotificationType
+from alttester.commands.base_command import BaseCommand
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class AddNotificationListener(BaseCommand):
+
+    def __init__(self, connection, notification_type, notification_callback, overwrite):
+        super().__init__(connection, "activateNotification")
+
+        if notification_type not in NotificationType:
+            raise InvalidParameterTypeException(
+                parameter_name='notification_type',
+                expected_types=[NotificationType],
+                received_type=type(notification_type)
+            )
+        self.notification_type = notification_type
+
+        if type(notification_callback) == "method":
+            raise InvalidParameterTypeException(
+                parameter_name='notification_callback',
+                expected_types=[callable],
+                received_type=type(notification_callback)
+            )
+        self.notification_callback = notification_callback
+
+        if type(overwrite) == "bool":
+            raise InvalidParameterTypeException(
+                parameter_name='overwrite',
+                expected_types=[bool],
+                received_type=type(overwrite)
+            )
+        self.overwrite = overwrite
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "notificationType": str(int(self.notification_type)),
+        })
+
+        return parameters
+
+    def execute(self):
+        self.connection._notification_handler.add_notification_listener(
+            self.notification_type,
+            self.notification_callback,
+            self.overwrite
+        )
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/remove_notification_listener.py` & `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/remove_notification_listener.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.Notifications.notification_type import NotificationType
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class RemoveNotificationListener(BaseCommand):
-
-    def __init__(self, connection, notification_type):
-        super().__init__(connection, "deactivateNotification")
-
-        if notification_type not in NotificationType:
-            raise InvalidParameterTypeException(
-                parameter_name='notification_type',
-                expected_types=[NotificationType],
-                received_type=type(notification_type)
-            )
-        self.notification_type = notification_type
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "notificationType": str(int(self.notification_type)),
-        })
-
-        return parameters
-
-    def execute(self):
-        self.connection._notification_handler.remove_notification_listener(self.notification_type)
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.Notifications.notification_type import NotificationType
+from alttester.commands.base_command import BaseCommand
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class RemoveNotificationListener(BaseCommand):
+
+    def __init__(self, connection, notification_type):
+        super().__init__(connection, "deactivateNotification")
+
+        if notification_type not in NotificationType:
+            raise InvalidParameterTypeException(
+                parameter_name='notification_type',
+                expected_types=[NotificationType],
+                received_type=type(notification_type)
+            )
+        self.notification_type = notification_type
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "notificationType": str(int(self.notification_type)),
+        })
+
+        return parameters
+
+    def execute(self):
+        self.connection._notification_handler.remove_notification_listener(self.notification_type)
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/reset_input.py` & `alttester_driver-2.1.0/alttester/commands/Notifications/load_scene_notification_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class ResetInput(BaseCommand):
-
-    def __init__(self, connection):
-        super().__init__(connection, "resetInput")
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+
+class LoadSceneNotificationResult():
+    def __init__(self, scene_name, loadSceneMode):
+        self.scene_name = scene_name
+        self.loadSceneMode = loadSceneMode
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/AltTesterCommands/set_server_logging.py` & `alttester_driver-2.1.0/alttester/commands/AltTesterCommands/set_server_logging.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.logging import AltLogger, AltLogLevel
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class SetServerLogging(BaseCommand):
-
-    def __init__(self, connection, logger, log_level):
-        super().__init__(connection, "setServerLogging")
-
-        if logger not in AltLogger:
-            raise InvalidParameterTypeException(
-                parameter_name='logger',
-                expected_types=[AltLogger],
-                received_type=type(logger)
-            )
-
-        if log_level not in AltLogLevel:
-            raise InvalidParameterTypeException(
-                parameter_name='log_level',
-                expected_types=[AltLogLevel],
-                received_type=type(log_level)
-            )
-
-        self.logger = logger
-        self.log_level = log_level
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "logger": str(self.logger),
-            "logLevel": str(self.log_level)
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+from alttester.logging import AltLogger, AltLogLevel
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class SetServerLogging(BaseCommand):
+
+    def __init__(self, connection, logger, log_level):
+        super().__init__(connection, "setServerLogging")
+
+        if logger not in AltLogger:
+            raise InvalidParameterTypeException(
+                parameter_name='logger',
+                expected_types=[AltLogger],
+                received_type=type(logger)
+            )
+
+        if log_level not in AltLogLevel:
+            raise InvalidParameterTypeException(
+                parameter_name='log_level',
+                expected_types=[AltLogLevel],
+                received_type=type(log_level)
+            )
+
+        self.logger = logger
+        self.log_level = log_level
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "logger": str(self.logger),
+            "logLevel": str(self.log_level)
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/__init__.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.FindObjects.find_object_which_contains import *
-from alttester.commands.FindObjects.find_object import *
-from alttester.commands.FindObjects.find_objects import *
-from alttester.commands.FindObjects.find_objects_which_contains import *
-from alttester.commands.FindObjects.wait_for_object import *
-from alttester.commands.FindObjects.wait_for_object_to_not_be_present import *
-from alttester.commands.FindObjects.wait_for_object_which_contains import *
-from alttester.commands.FindObjects.find_object_at_coordinates import *
-from alttester.commands.FindObjects.wait_for_component_property import *
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.UnityCommands.delete_player_pref import DeletePlayerPref
+from alttester.commands.UnityCommands.delete_player_pref_key import DeletePlayerPrefKey
+from alttester.commands.UnityCommands.get_current_scene import GetCurrentScene
+from alttester.commands.UnityCommands.get_player_pref_key import GetPlayerPrefKey
+from alttester.commands.UnityCommands.get_time_scale import GetTimeScale
+from alttester.commands.UnityCommands.load_scene import LoadScene
+from alttester.commands.UnityCommands.set_player_pref_key import SetPlayerPrefKey
+from alttester.commands.UnityCommands.set_time_scale import SetTimeScale
+from alttester.commands.UnityCommands.wait_for_current_scene_to_be import WaitForCurrentSceneToBe
+from alttester.commands.UnityCommands.get_all_loaded_scenes import GetAllLoadedScenes
+from alttester.commands.UnityCommands.unload_scene import UnloadScene
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/tap_coordinates.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,51 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
-from alttester.by import By
-
-
-class FindObject(BaseCommand):
-
-    def __init__(self, connection, by, value, camera_by, camera_value, enabled):
-        super().__init__(connection, "findObject")
-
-        if by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="by",
-                expected_types=[By],
-                received_type=type(by)
-            )
-
-        if camera_by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="camera_by",
-                expected_types=[By],
-                received_type=type(camera_by)
-            )
-
-        self.by = by
-        self.value = value
-        self.camera_by = camera_by
-        self.camera_value = camera_value
-        self.enabled = enabled
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "by": str(self.by),
-            "path": self.get_path(self.by, self.value),
-            "cameraBy": str(self.camera_by),
-            "cameraPath": self.get_path(self.camera_by, self.camera_value),
-            "enabled": self.enabled,
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import validate_coordinates, BaseCommand
+
+
+class TapCoordinates(BaseCommand):
+
+    def __init__(self, connection, coordinates, count, interval, wait):
+        super().__init__(connection, "tapCoordinates")
+
+        self.coordinates = validate_coordinates(coordinates)
+        self.count = count
+        self.interval = interval
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "coordinates": self.coordinates,
+            "count": self.count,
+            "interval": self.interval,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        if self.wait:
+            data = self.recv()
+            self.validate_response("Finished", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object_at_coordinates.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/move_touch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class FindObjectAtCoordinates(BaseCommand):
-
-    def __init__(self, connection, coordinates):
-        super().__init__(connection, "findObjectAtCoordinates")
-
-        self.coordinates = validate_coordinates(coordinates)
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "coordinates": self.coordinates,
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import validate_coordinates, BaseCommand
+
+
+class MoveTouch(BaseCommand):
+
+    def __init__(self, connection, finger_id, coordinates):
+        super().__init__(connection, "moveTouch")
+
+        self.coordinates = validate_coordinates(coordinates)
+        self.finger_id = finger_id
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "fingerId": self.finger_id,
+            "coordinates": self.coordinates
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_object_which_contains.py` & `alttester_driver-2.1.0/alttester/commands/FindObjects/find_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
-from alttester.by import By
-
-
-class FindObjectWhichContains(BaseCommand):
-
-    def __init__(self, connection, by, value, camera_by, camera_value, enabled):
-        super().__init__(connection, "findObject")
-
-        if by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="by",
-                expected_types=[By],
-                received_type=type(by)
-            )
-
-        if camera_by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="camera_by",
-                expected_types=[By],
-                received_type=type(camera_by)
-            )
-
-        self.by = by
-        self.value = value
-        self.camera_by = camera_by
-        self.camera_value = camera_value
-        self.enabled = enabled
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "by": str(self.by),
-            "path": self.get_path_contains(self.by, self.value),
-            "cameraBy": str(self.camera_by),
-            "cameraPath": self.get_path(self.camera_by, self.camera_value),
-            "enabled": self.enabled
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+from alttester.exceptions import InvalidParameterTypeException
+from alttester.by import By
+
+
+class FindObject(BaseCommand):
+
+    def __init__(self, connection, by, value, camera_by, camera_value, enabled):
+        super().__init__(connection, "findObject")
+
+        if by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="by",
+                expected_types=[By],
+                received_type=type(by)
+            )
+
+        if camera_by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="camera_by",
+                expected_types=[By],
+                received_type=type(camera_by)
+            )
+
+        self.by = by
+        self.value = value
+        self.camera_by = camera_by
+        self.camera_value = camera_value
+        self.enabled = enabled
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "by": str(self.by),
+            "path": self.get_path(self.by, self.value),
+            "cameraBy": str(self.camera_by),
+            "cameraPath": self.get_path(self.camera_by, self.camera_value),
+            "enabled": self.enabled,
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/find_objects_which_contains.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/get_component_property.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,47 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.exceptions import InvalidParameterTypeException
-from alttester.by import By
-
-
-class FindObjectsWhichContain(BaseCommand):
-
-    def __init__(self, connection, by, value, camera_by, camera_value, enabled):
-        super().__init__(connection, "findObjects")
-
-        if by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="by",
-                expected_types=[By],
-                received_type=type(by)
-            )
-
-        if camera_by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="camera_by",
-                expected_types=[By],
-                received_type=type(camera_by)
-            )
-
-        self.by = by
-        self.value = value
-        self.camera_by = camera_by
-        self.camera_value = camera_value
-        self.enabled = enabled
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "by": str(self.by),
-            "path": self.get_path_contains(self.by, self.value),
-            "cameraBy": str(self.camera_by),
-            "cameraPath": self.get_path(self.camera_by, self.camera_value),
-            "enabled": self.enabled
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetComponentProperty(BaseCommand):
+
+    def __init__(self, connection, component_name, property_name, assembly_name, max_depth, alt_object):
+        super().__init__(connection, "getObjectComponentProperty")
+
+        self.alt_object = alt_object
+
+        self.component_name = component_name
+        self.property_name = property_name
+        self.assembly_name = assembly_name
+        self.max_depth = max_depth
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+            "component": self.component_name,
+            "property": self.property_name,
+            "assembly": self.assembly_name,
+            "maxDepth": self.max_depth,
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_component_property.py` & `alttester_driver-2.1.0/alttester/commands/set_static_property.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import time
-from loguru import logger
-from alttester.commands.base_command import Command
-from alttester.exceptions import NotFoundException, WaitTimeOutException
-
-
-class WaitForComponentProperty(Command):
-    def __init__(self, component_name, property_name,
-                 property_value, assembly, altObject, timeout=20, interval=0.5):
-        self.component_name = component_name
-        self.property_name = property_name
-        self.property_value = property_value
-        self.assembly = assembly
-        self.timeout = timeout
-        self.interval = interval
-        self.altObject = altObject
-
-    def execute(self):
-        t = 0
-        while (t <= self.timeout):
-            try:
-                property_found = self.altObject.get_component_property(
-                    self.component_name, self.property_name, self.assembly)
-                if (property_found == self.property_value):
-                    break
-            except NotFoundException:
-                logger.debug("Waiting for property {}...", self.property_name)
-                time.sleep(self.interval)
-                t += self.interval
-
-        if t >= self.timeout:
-            raise WaitTimeOutException("Property {} not found after {} seconds"
-                                       .format(
-                                           self.property_name, self.timeout))
-
-        return property_found
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class SetStaticProperty(BaseCommand):
+
+    def __init__(self, connection, component_name, property_name, assembly_name, value):
+        super().__init__(connection, "setObjectComponentProperty")
+
+        self.alt_object = None
+
+        self.component_name = component_name
+        self.property_name = property_name
+        self.assembly_name = assembly_name
+        self.value = value
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object,
+            "component": self.component_name,
+            "property": self.property_name,
+            "assembly": self.assembly_name,
+            "value": self.value
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_object.py` & `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import time
-
-from loguru import logger
-
-from alttester.by import By
-from alttester.commands.base_command import Command
-from alttester.commands.FindObjects.find_object import FindObject
-from alttester.exceptions import NotFoundException, WaitTimeOutException, InvalidParameterTypeException
-
-
-class WaitForObject(Command):
-
-    def __init__(self, connection, by, value, camera_by, camera_value, timeout, interval, enabled):
-        self.connection = connection
-
-        if by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="by",
-                expected_types=[By],
-                received_type=type(by)
-            )
-
-        if camera_by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="camera_by",
-                expected_types=[By],
-                received_type=type(camera_by)
-            )
-
-        self.by = by
-        self.value = value
-        self.camera_by = camera_by
-        self.camera_value = camera_value
-        self.timeout = timeout
-        self.interval = interval
-        self.enabled = enabled
-
-    def execute(self):
-        t = 0
-        alt_object = None
-
-        while (t <= self.timeout):
-            try:
-                alt_object = FindObject(
-                    self.connection,
-                    self.by, self.value, self.camera_by, self.camera_value, self.enabled
-                ).execute()
-
-                break
-            except NotFoundException:
-                logger.debug("Waiting for element {}...", self.value)
-                time.sleep(self.interval)
-                t += self.interval
-
-        if t >= self.timeout:
-            raise WaitTimeOutException("Element {} not found after {} seconds".format(self.value, self.timeout))
-
-        return alt_object
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import time
+
+from loguru import logger
+
+from alttester.by import By
+from alttester.commands.base_command import Command
+from alttester.commands.FindObjects.find_object import FindObject
+from alttester.exceptions import NotFoundException, WaitTimeOutException, InvalidParameterTypeException
+
+
+class WaitForObject(Command):
+
+    def __init__(self, connection, by, value, camera_by, camera_value, timeout, interval, enabled):
+        self.connection = connection
+
+        if by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="by",
+                expected_types=[By],
+                received_type=type(by)
+            )
+
+        if camera_by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="camera_by",
+                expected_types=[By],
+                received_type=type(camera_by)
+            )
+
+        self.by = by
+        self.value = value
+        self.camera_by = camera_by
+        self.camera_value = camera_value
+        self.timeout = timeout
+        self.interval = interval
+        self.enabled = enabled
+
+    def execute(self):
+        t = 0
+        alt_object = None
+
+        while (t <= self.timeout):
+            try:
+                alt_object = FindObject(
+                    self.connection,
+                    self.by, self.value, self.camera_by, self.camera_value, self.enabled
+                ).execute()
+
+                break
+            except NotFoundException:
+                logger.debug("Waiting for element {}...", self.value)
+                time.sleep(self.interval)
+                t += self.interval
+
+        if t >= self.timeout:
+            raise WaitTimeOutException("Element {} not found after {} seconds".format(self.value, self.timeout))
+
+        return alt_object
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/FindObjects/wait_for_object_which_contains.py` & `alttester_driver-2.1.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import time
-
-from loguru import logger
-
-from alttester.by import By
-from alttester.commands.base_command import Command
-from alttester.commands.FindObjects.find_object_which_contains import FindObjectWhichContains
-from alttester.exceptions import NotFoundException, WaitTimeOutException, InvalidParameterTypeException
-
-
-class WaitForObjectWhichContains(Command):
-
-    def __init__(self, connection, by, value, camera_by, camera_value, timeout, interval, enabled):
-        self.connection = connection
-
-        if by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="by",
-                expected_types=[By],
-                received_type=type(by)
-            )
-
-        if camera_by not in By:
-            raise InvalidParameterTypeException(
-                parameter_name="camera_by",
-                expected_types=[By],
-                received_type=type(camera_by)
-            )
-
-        self.by = by
-        self.value = value
-        self.camera_by = camera_by
-        self.camera_value = camera_value
-        self.timeout = timeout
-        self.interval = interval
-        self.enabled = enabled
-
-    def execute(self):
-        t = 0
-        alt_unity_object = None
-
-        while (t <= self.timeout):
-            try:
-                alt_unity_object = FindObjectWhichContains(
-                    self.connection,
-                    self.by, self.value, self.camera_by, self.camera_value, self.enabled
-                ).execute()
-
-                break
-            except NotFoundException:
-                logger.debug("Waiting for element where name contains {}...", self.value)
-                time.sleep(self.interval)
-                t += self.interval
-
-        if t >= self.timeout:
-            raise WaitTimeOutException("Element where name contains {} not found after {} seconds".format(
-                self.value,
-                self.timeout
-            ))
-
-        return alt_unity_object
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import time
+
+from loguru import logger
+
+from alttester.by import By
+from alttester.commands.base_command import Command
+from alttester.commands.FindObjects.find_object import FindObject
+from alttester.exceptions import NotFoundException, WaitTimeOutException, InvalidParameterTypeException
+
+
+class WaitForObjectToNotBePresent(Command):
+
+    def __init__(self, connection, by, value, camera_by, camera_value, timeout, interval, enabled):
+        self.connection = connection
+
+        if by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="by",
+                expected_types=[By],
+                received_type=type(by)
+            )
+
+        if camera_by not in By:
+            raise InvalidParameterTypeException(
+                parameter_name="camera_by",
+                expected_types=[By],
+                received_type=type(camera_by)
+            )
+
+        self.by = by
+        self.value = value
+        self.camera_by = camera_by
+        self.camera_value = camera_value
+        self.timeout = timeout
+        self.interval = interval
+        self.enabled = enabled
+
+    def execute(self):
+        t = 0
+
+        while (t <= self.timeout):
+            try:
+                logger.debug("Waiting for element {} to not be present...", self.value)
+
+                FindObject(
+                    self.connection,
+                    self.by, self.value, self.camera_by, self.camera_value, self.enabled
+                ).execute()
+
+                time.sleep(self.interval)
+                t += self.interval
+            except NotFoundException as ex:
+                logger.debug(ex)
+                break
+
+        if t > self.timeout:
+            logger.debug("WaitTimeOutException")
+            raise WaitTimeOutException("Element {} still found after {} seconds".format(
+                self.value,
+                self.timeout
+            ))
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/begin_touch.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/multi_point_swipe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,49 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class BeginTouch(BaseCommand):
-
-    def __init__(self, connection, coordinates):
-        super().__init__(connection, "beginTouch")
-
-        self.coordinates = validate_coordinates(coordinates)
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "coordinates": self.coordinates
-        })
-
-        return parameters
-
-    def execute(self):
-        return int(self.send())
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class MultipointSwipe(BaseCommand):
+
+    def __init__(self, connection, positions, duration, wait):
+        super().__init__(connection, "multipointSwipe")
+
+        self.positions = positions
+        self.duration = duration
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "positions": self.positions_to_json(self.positions),
+            "duration": self.duration,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        if self.wait:
+            data = self.recv()
+            self.validate_response("Finished", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/click_coordinates.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/swipe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class ClickCoordinates(BaseCommand):
-
-    def __init__(self, connection, coordinates, count, interval, wait):
-        super().__init__(connection, "clickCoordinates")
-
-        self.coordinates = validate_coordinates(coordinates)
-        self.count = count
-        self.interval = interval
-        self.wait = wait
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "coordinates": self.coordinates,
-            "count": self.count,
-            "interval": self.interval,
-            "wait": self.wait
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import validate_coordinates, BaseCommand
+
+
+class Swipe(BaseCommand):
+
+    def __init__(self, connection, start, end, duration, wait):
+        super().__init__(connection, "swipe")
+
+        self.start = validate_coordinates(start)
+        self.end = validate_coordinates(end)
+        self.duration = duration
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "start": self.start,
+            "end": self.end,
+            "duration": self.duration,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        if self.wait:
+            data = self.recv()
+            self.validate_response("Finished", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/end_touch.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/click_coordinates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class EndTouch(BaseCommand):
-
-    def __init__(self, connection, finger_id):
-        super(EndTouch, self).__init__(connection, "endTouch")
-
-        self.finger_id = finger_id
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "fingerId": self.finger_id,
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import validate_coordinates, BaseCommand
+
+
+class ClickCoordinates(BaseCommand):
+
+    def __init__(self, connection, coordinates, count, interval, wait):
+        super().__init__(connection, "clickCoordinates")
+
+        self.coordinates = validate_coordinates(coordinates)
+        self.count = count
+        self.interval = interval
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "coordinates": self.coordinates,
+            "count": self.count,
+            "interval": self.interval,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        if self.wait:
+            data = self.recv()
+            self.validate_response("Finished", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/keys_down.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/keys_up.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.keycode import AltKeyCode
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class KeysDown(BaseCommand):
-
-    def __init__(self, connection, key_codes, power):
-        super().__init__(connection, "keysDown")
-
-        if not isinstance(key_codes, (list, tuple)):
-            raise InvalidParameterTypeException(
-                parameter_name="key_codes",
-                expected_types=(list, tuple),
-                received_type=type(key_codes)
-            )
-
-        for key_code in key_codes:
-            if key_code not in AltKeyCode and key_code not in AltKeyCode.names():
-                raise InvalidParameterTypeException(
-                    parameter_name="key_code",
-                    expected_types=[AltKeyCode],
-                    received_type=type(key_code)
-                )
-
-        self.key_codes = key_codes
-        self.power = power
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "keyCodes": [str(key_code) for key_code in self.key_codes],
-            "power": self.power
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+from alttester.keycode import AltKeyCode
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class KeysUp(BaseCommand):
+
+    def __init__(self, connection, key_codes):
+        super().__init__(connection, "keysUp")
+
+        if not isinstance(key_codes, (list, tuple)):
+            raise InvalidParameterTypeException(
+                parameter_name="key_codes",
+                expected_types=(list, tuple),
+                received_type=type(key_codes)
+            )
+
+        for key_code in key_codes:
+            if key_code not in AltKeyCode and key_code not in AltKeyCode.names():
+                raise InvalidParameterTypeException(
+                    parameter_name="key_codes",
+                    expected_types=[AltKeyCode],
+                    received_type=type(key_code)
+                )
+
+        self.key_codes = key_codes
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "keyCodes": [str(key_code) for key_code in self.key_codes],
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/keys_up.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/keys_down.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.keycode import AltKeyCode
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class KeysUp(BaseCommand):
-
-    def __init__(self, connection, key_codes):
-        super().__init__(connection, "keysUp")
-
-        if not isinstance(key_codes, (list, tuple)):
-            raise InvalidParameterTypeException(
-                parameter_name="key_codes",
-                expected_types=(list, tuple),
-                received_type=type(key_codes)
-            )
-
-        for key_code in key_codes:
-            if key_code not in AltKeyCode and key_code not in AltKeyCode.names():
-                raise InvalidParameterTypeException(
-                    parameter_name="key_codes",
-                    expected_types=[AltKeyCode],
-                    received_type=type(key_code)
-                )
-
-        self.key_codes = key_codes
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "keyCodes": [str(key_code) for key_code in self.key_codes],
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+from alttester.keycode import AltKeyCode
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class KeysDown(BaseCommand):
+
+    def __init__(self, connection, key_codes, power):
+        super().__init__(connection, "keysDown")
+
+        if not isinstance(key_codes, (list, tuple)):
+            raise InvalidParameterTypeException(
+                parameter_name="key_codes",
+                expected_types=(list, tuple),
+                received_type=type(key_codes)
+            )
+
+        for key_code in key_codes:
+            if key_code not in AltKeyCode and key_code not in AltKeyCode.names():
+                raise InvalidParameterTypeException(
+                    parameter_name="key_code",
+                    expected_types=[AltKeyCode],
+                    received_type=type(key_code)
+                )
+
+        self.key_codes = key_codes
+        self.power = power
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "keyCodes": [str(key_code) for key_code in self.key_codes],
+            "power": self.power
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/move_mouse.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/click_element.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class MoveMouse(BaseCommand):
-
-    def __init__(self, connection, coordinates, duration, wait):
-        super().__init__(connection, "moveMouse")
-
-        self.coordinates = validate_coordinates(coordinates)
-        self.duration = duration
-        self.wait = wait
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "coordinates": self.coordinates,
-            "duration": self.duration,
-            "wait": self.wait,
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class ClickElement(BaseCommand):
+
+    def __init__(self, connection, alt_object, count, interval, wait):
+        super().__init__(connection, "clickElement")
+
+        self.alt_object = alt_object
+        self.count = count
+        self.interval = interval
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+            "count": self.count,
+            "interval": self.interval,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+
+        if self.wait:
+            self.validate_response("Finished", self.recv())
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/move_touch.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/set_component_property.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,48 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class MoveTouch(BaseCommand):
-
-    def __init__(self, connection, finger_id, coordinates):
-        super().__init__(connection, "moveTouch")
-
-        self.coordinates = validate_coordinates(coordinates)
-        self.finger_id = finger_id
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "fingerId": self.finger_id,
-            "coordinates": self.coordinates
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import json
+from alttester.commands.base_command import BaseCommand
+
+
+class SetComponentProperty(BaseCommand):
+
+    def __init__(self, connection, component_name, property_name, value, assembly_name, alt_object):
+        super().__init__(connection, "setObjectComponentProperty")
+
+        self.alt_object = alt_object
+
+        self.component_name = component_name
+        self.property_name = property_name
+        self.value = json.dumps(value)
+        self.assembly_name = assembly_name
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+            "component": self.component_name,
+            "property": self.property_name,
+            "assembly": self.assembly_name,
+            "value": self.value,
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/press_keys.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/call_method.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.keycode import AltKeyCode
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class PressKeys(BaseCommand):
-
-    def __init__(self, connection, key_codes, power, duration, wait):
-        super().__init__(connection, "pressKeyboardKeys")
-
-        if not isinstance(key_codes, (list, tuple)):
-            raise InvalidParameterTypeException(
-                parameter_name="key_codes",
-                expected_types=(list, tuple),
-                received_type=type(key_codes)
-            )
-
-        for key_code in key_codes:
-            if key_code not in AltKeyCode:
-                raise InvalidParameterTypeException(
-                    parameter_name="key_codes",
-                    expected_types=[AltKeyCode],
-                    received_type=type(key_code)
-                )
-
-        self.key_codes = key_codes
-        self.power = power
-        self.duration = duration
-        self.wait = wait
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "keyCodes": [str(key_code) for key_code in self.key_codes],
-            "power": self.power,
-            "duration": self.duration,
-            "wait": self.wait,
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import json
+
+from alttester.commands.base_command import BaseCommand
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class CallMethod(BaseCommand):
+
+    def __init__(self, connection, component_name, method_name, alt_object=None, parameters=None,
+                 type_of_parameters=None, assembly=""):
+        super().__init__(connection, "callComponentMethodForObject")
+
+        parameters = parameters if parameters is not None else []
+        type_of_parameters = type_of_parameters if type_of_parameters is not None else []
+
+        if not isinstance(parameters, (list, tuple)):
+            raise InvalidParameterTypeException(
+                parameter_name="parameters",
+                expected_types=(list, tuple),
+                received_type=type(parameters)
+            )
+
+        if not isinstance(type_of_parameters, (list, tuple)):
+            raise InvalidParameterTypeException(
+                parameter_name="type_of_parameters",
+                expected_types=(list, tuple),
+                received_type=type(type_of_parameters)
+            )
+
+        self.alt_object = alt_object
+        self.component_name = component_name
+        self.method_name = method_name
+        self.parameters = [json.dumps(parameter) for parameter in parameters]
+        self.type_of_parameters = type_of_parameters
+        self.assembly = assembly
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "component": self.component_name,
+            "method": self.method_name,
+            "parameters": self.parameters,
+            "typeofparameters": self.type_of_parameters,
+            "assembly": self.assembly
+        })
+
+        if self.alt_object:
+            parameters["altObject"] = self.alt_object.to_json()
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/scroll_mouse.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/scroll_mouse.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class Scroll(BaseCommand):
-
-    def __init__(self, connection, speed_vertical, duration, wait, speed_horizontal):
-        super(Scroll, self).__init__(connection, "scroll")
-
-        self.speed_vertical = speed_vertical
-        self.speed_horizontal = speed_horizontal
-        self.duration = duration
-        self.wait = wait
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "speed": self.speed_vertical,
-            "speedHorizontal": self.speed_horizontal,
-            "duration": self.duration,
-            "wait": self.wait,
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class Scroll(BaseCommand):
+
+    def __init__(self, connection, speed_vertical, duration, wait, speed_horizontal):
+        super(Scroll, self).__init__(connection, "scroll")
+
+        self.speed_vertical = speed_vertical
+        self.speed_horizontal = speed_horizontal
+        self.duration = duration
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "speed": self.speed_vertical,
+            "speedHorizontal": self.speed_horizontal,
+            "duration": self.duration,
+            "wait": self.wait,
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        if self.wait:
+            data = self.recv()
+            self.validate_response("Finished", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/InputActions/swipe.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/tap_element.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import validate_coordinates, BaseCommand
-
-
-class Swipe(BaseCommand):
-
-    def __init__(self, connection, start, end, duration, wait):
-        super().__init__(connection, "swipe")
-
-        self.start = validate_coordinates(start)
-        self.end = validate_coordinates(end)
-        self.duration = duration
-        self.wait = wait
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "start": self.start,
-            "end": self.end,
-            "duration": self.duration,
-            "wait": self.wait
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        if self.wait:
-            data = self.recv()
-            self.validate_response("Finished", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class TapElement(BaseCommand):
+
+    def __init__(self, connection, alt_object, count, interval, wait):
+        super().__init__(connection, "tapElement")
+
+        self.alt_object = alt_object
+        self.count = count
+        self.interval = interval
+        self.wait = wait
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+            "count": self.count,
+            "interval": self.interval,
+            "wait": self.wait
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+
+        if self.wait:
+            self.validate_response("Finished", self.recv())
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/__init__.py` & `alttester_driver-2.1.0/alttester/commands/Notifications/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.Notifications.base_notification_callbacks import BaseNotificationCallbacks
-from alttester.commands.Notifications.load_scene_notification_result import LoadSceneNotificationResult
-from alttester.commands.Notifications.log_notification_result import LogNotificationResult
-from alttester.commands.Notifications.notification_type import NotificationType
-from alttester.commands.Notifications.load_scene_mode import LoadSceneMode
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.Notifications.base_notification_callbacks import BaseNotificationCallbacks
+from alttester.commands.Notifications.load_scene_notification_result import LoadSceneNotificationResult
+from alttester.commands.Notifications.log_notification_result import LogNotificationResult
+from alttester.commands.Notifications.notification_type import NotificationType
+from alttester.commands.Notifications.load_scene_mode import LoadSceneMode
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/base_notification_callbacks.py` & `alttester_driver-2.1.0/alttester/commands/Notifications/base_notification_callbacks.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from loguru import logger
-
-
-class BaseNotificationCallbacks():
-    def scene_loaded_callback(self, load_scene_notification_result):
-        logger.debug("Scene {0} was loaded {1}".format(str(load_scene_notification_result.scene_name),
-                                                       str(load_scene_notification_result.loadSceneMode)))
-
-    def scene_unloaded_callback(self, scene_name):
-        logger.debug("Scene {0} was unloaded".format(scene_name))
-
-    def log_callback(self, log_notification_result):
-        logger.debug("Log of type {0} with message {1} was received".format(str(log_notification_result.type),
-                                                                            str(log_notification_result.message)))
-
-    def application_paused_callback(self, application_paused):
-        logger.debug("Application paused: {0}".format(application_paused))
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from loguru import logger
+
+
+class BaseNotificationCallbacks():
+    def scene_loaded_callback(self, load_scene_notification_result):
+        logger.debug("Scene {0} was loaded {1}".format(str(load_scene_notification_result.scene_name),
+                                                       str(load_scene_notification_result.loadSceneMode)))
+
+    def scene_unloaded_callback(self, scene_name):
+        logger.debug("Scene {0} was unloaded".format(scene_name))
+
+    def log_callback(self, log_notification_result):
+        logger.debug("Log of type {0} with message {1} was received".format(str(log_notification_result.type),
+                                                                            str(log_notification_result.message)))
+
+    def application_paused_callback(self, application_paused):
+        logger.debug("Application paused: {0}".format(application_paused))
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/load_scene_mode.py` & `alttester_driver-2.1.0/alttester/__version__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,18 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from enum import Enum, unique
-
-
-@unique
-class LoadSceneMode(Enum):
-    Single = 0
-    Additive = 1
-
-    @classmethod
-    def values(cls):
-        return [scene_mode.value for scene_mode in cls]
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+VERSION = "2.1.0"
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/load_scene_notification_result.py` & `alttester_driver-2.1.0/alttester/commands/Notifications/notification_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-
-class LoadSceneNotificationResult():
-    def __init__(self, scene_name, loadSceneMode):
-        self.scene_name = scene_name
-        self.loadSceneMode = loadSceneMode
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from enum import IntEnum
+
+
+class NotificationType(IntEnum):
+    LOADSCENE = 0
+    UNLOADSCENE = 1
+    LOG = 2,
+    APPLICATION_PAUSED = 3
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/log_notification_result.py` & `alttester_driver-2.1.0/alttester/commands/Notifications/log_notification_result.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-
-class LogNotificationResult:
-
-    def __init__(self, message, stack_trace, type):
-        self.message = message
-        self.stack_trace = stack_trace
-        self.type = type
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+
+class LogNotificationResult:
+
+    def __init__(self, message, stack_trace, type):
+        self.message = message
+        self.stack_trace = stack_trace
+        self.type = type
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/Notifications/notification_type.py` & `alttester_driver-2.1.0/alttester/commands/get_server_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from enum import IntEnum
-
-
-class NotificationType(IntEnum):
-    LOADSCENE = 0
-    UNLOADSCENE = 1
-    LOG = 2,
-    APPLICATION_PAUSED = 3
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetServerVersion(BaseCommand):
+
+    def __init__(self, connection):
+        super().__init__(connection, "getServerVersion")
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/get_all_components.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_enter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class GetAllComponents(BaseCommand):
-
-    def __init__(self, connection, alt_object):
-        super(GetAllComponents, self).__init__(connection, "getAllComponents")
-
-        self.alt_object = alt_object
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "altObjectId": self.alt_object.id
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class PointerEnter(BaseCommand):
+
+    def __init__(self, connection, alt_object):
+        super(PointerEnter, self).__init__(connection, "pointerEnterObject")
+
+        self.alt_object = alt_object
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/get_component_property.py` & `alttester_driver-2.1.0/alttester/commands/get_static_property.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class GetComponentProperty(BaseCommand):
-
-    def __init__(self, connection, component_name, property_name, assembly_name, max_depth, alt_object):
-        super().__init__(connection, "getObjectComponentProperty")
-
-        self.alt_object = alt_object
-
-        self.component_name = component_name
-        self.property_name = property_name
-        self.assembly_name = assembly_name
-        self.max_depth = max_depth
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "altObject": self.alt_object.to_json(),
-            "component": self.component_name,
-            "property": self.property_name,
-            "assembly": self.assembly_name,
-            "maxDepth": self.max_depth,
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetStaticProperty(BaseCommand):
+
+    def __init__(self, connection, component_name, property_name, assembly_name, max_depth):
+        super().__init__(connection, "getObjectComponentProperty")
+
+        self.alt_object = None
+
+        self.component_name = component_name
+        self.property_name = property_name
+        self.assembly_name = assembly_name
+        self.max_depth = max_depth
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object,
+            "component": self.component_name,
+            "property": self.property_name,
+            "assembly": self.assembly_name,
+            "maxDepth": self.max_depth,
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_down.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class PointerDown(BaseCommand):
-
-    def __init__(self, connection, alt_object):
-        super(PointerDown, self).__init__(connection, "pointerDownFromObject")
-        self.alt_object = alt_object
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "altObject": self.alt_object.to_json(),
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetAllLoadedScenes(BaseCommand):
+
+    def __init__(self, connection):
+        super().__init__(connection, "getAllLoadedScenes")
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_enter.py` & `alttester_driver-2.1.0/tests/integration/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class PointerEnter(BaseCommand):
-
-    def __init__(self, connection, alt_object):
-        super(PointerEnter, self).__init__(connection, "pointerEnterObject")
-
-        self.alt_object = alt_object
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "altObject": self.alt_object.to_json(),
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+"""Holds helper methods and test data that need to be shared among all tests."""
+
+
+class Scenes:
+    Scene01 = "Scene 1 AltDriverTestScene"
+    Scene02 = "Scene 2 Draggable Panel"
+    Scene03 = "Scene 3 Drag And Drop"
+    Scene05 = "Scene 5 Keyboard Input"
+    Scene07A = "Scene 7 New Input System Actions"
+    Scene07B = "Scene 7 Drag And Drop NIS"
+    Scene09 = "scene 9 NIS"
+    Scene10 = "Scene 10 Sample NIS"
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/ObjectCommands/pointer_exit.py` & `alttester_driver-2.1.0/alttester/commands/ObjectCommands/pointer_up.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class PointerExit(BaseCommand):
-
-    def __init__(self, connection, alt_object):
-        super().__init__(connection, "pointerExitObject")
-
-        self.alt_object = alt_object
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "altObject": self.alt_object.to_json(),
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class PointerUp(BaseCommand):
+
+    def __init__(self, connection, alt_object):
+        super().__init__(connection, "pointerUpFromObject")
+
+        self.alt_object = alt_object
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "altObject": self.alt_object.to_json(),
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/UnityCommands/delete_player_pref.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_time_scale.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class DeletePlayerPref(BaseCommand):
-
-    def __init__(self, connection):
-        super().__init__(connection, "deletePlayerPref")
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from loguru import logger
+
+from alttester.commands.base_command import BaseCommand
+
+
+class GetTimeScale(BaseCommand):
+
+    def __init__(self, connection):
+        super().__init__(connection, "getTimeScale")
+
+    def execute(self):
+        logger.debug("Get time scale")
+        data = self.send()
+
+        logger.debug("Got time scale: {}", data)
+        return float(data)
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_all_loaded_scenes.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/delete_player_pref.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class GetAllLoadedScenes(BaseCommand):
-
-    def __init__(self, connection):
-        super().__init__(connection, "getAllLoadedScenes")
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class DeletePlayerPref(BaseCommand):
+
+    def __init__(self, connection):
+        super().__init__(connection, "deletePlayerPref")
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_player_pref_key.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/get_player_pref_key.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-from alttester.playerpref import PlayerPrefKeyType
-from alttester.exceptions import InvalidParameterTypeException
-
-
-class GetPlayerPrefKey(BaseCommand):
-
-    def __init__(self, connection, key_name, key_type):
-        super().__init__(connection, "getKeyPlayerPref")
-
-        if key_type not in PlayerPrefKeyType and key_type not in PlayerPrefKeyType.value():
-            raise InvalidParameterTypeException(
-                parameter_name="key_type",
-                expected_types=[PlayerPrefKeyType],
-                received_type=type(key_type)
-            )
-
-        self.key_name = key_name
-        self.key_type = key_type
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "keyName": self.key_name,
-            "keyType": str(self.key_type)
-        })
-
-        return parameters
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+from alttester.playerpref import PlayerPrefKeyType
+from alttester.exceptions import InvalidParameterTypeException
+
+
+class GetPlayerPrefKey(BaseCommand):
+
+    def __init__(self, connection, key_name, key_type):
+        super().__init__(connection, "getKeyPlayerPref")
+
+        if key_type not in PlayerPrefKeyType and key_type not in PlayerPrefKeyType.value():
+            raise InvalidParameterTypeException(
+                parameter_name="key_type",
+                expected_types=[PlayerPrefKeyType],
+                received_type=type(key_type)
+            )
+
+        self.key_name = key_name
+        self.key_type = key_type
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "keyName": self.key_name,
+            "keyType": str(self.key_type)
+        })
+
+        return parameters
+
+    def execute(self):
+        return self.send()
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/UnityCommands/get_time_scale.py` & `alttester_driver-2.1.0/alttester/playerpref.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from loguru import logger
-
-from alttester.commands.base_command import BaseCommand
-
-
-class GetTimeScale(BaseCommand):
-
-    def __init__(self, connection):
-        super().__init__(connection, "getTimeScale")
-
-    def execute(self):
-        logger.debug("Get time scale")
-        data = self.send()
-
-        logger.debug("Got time scale: {}", data)
-        return float(data)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from enum import Enum, unique
+
+
+@unique
+class PlayerPrefKeyType(Enum):
+    Int = 1
+    String = 2
+    Float = 3
+
+    def __str__(self):
+        return str(self.value)
+
+    @classmethod
+    def values(cls):
+        return [pref_type.value for pref_type in cls]
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/UnityCommands/load_scene.py` & `alttester_driver-2.1.0/alttester/commands/UnityCommands/load_scene.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class LoadScene(BaseCommand):
-
-    def __init__(self, connection, scene_name, load_single):
-        super().__init__(connection, "loadScene")
-
-        self.scene_name = scene_name
-        self.load_single = load_single
-
-    @property
-    def _parameters(self):
-        parameters = super()._parameters
-        parameters.update(**{
-            "sceneName": self.scene_name,
-            "loadSingle": self.load_single
-        })
-
-        return parameters
-
-    def execute(self):
-        data = self.send()
-        self.validate_response("Ok", data)
-
-        data = self.recv()
-        self.validate_response("Scene Loaded", data)
-
-        return data
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.base_command import BaseCommand
+
+
+class LoadScene(BaseCommand):
+
+    def __init__(self, connection, scene_name, load_single):
+        super().__init__(connection, "loadScene")
+
+        self.scene_name = scene_name
+        self.load_single = load_single
+
+    @property
+    def _parameters(self):
+        parameters = super()._parameters
+        parameters.update(**{
+            "sceneName": self.scene_name,
+            "loadSingle": self.load_single
+        })
+
+        return parameters
+
+    def execute(self):
+        data = self.send()
+        self.validate_response("Ok", data)
+
+        data = self.recv()
+        self.validate_response("Scene Loaded", data)
+
+        return data
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/__init__.py` & `alttester_driver-2.1.0/alttester/commands/InputActions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.AltTesterCommands import *
-from alttester.commands.FindObjects import *
-from alttester.commands.InputActions import *
-from alttester.commands.ObjectCommands import *
-from alttester.commands.UnityCommands import *
-from alttester.commands.get_png_screenshot import GetPNGScreenshot
-from alttester.commands.get_server_version import GetServerVersion
-from alttester.commands.get_static_property import GetStaticProperty
-from alttester.commands.set_static_property import SetStaticProperty
-from alttester.commands.Notifications import *
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.commands.InputActions.begin_touch import *
+from alttester.commands.InputActions.click_coordinates import *
+from alttester.commands.InputActions.end_touch import *
+from alttester.commands.InputActions.keys_down import *
+from alttester.commands.InputActions.keys_up import *
+from alttester.commands.InputActions.move_mouse import *
+from alttester.commands.InputActions.move_touch import *
+from alttester.commands.InputActions.multi_point_swipe import *
+from alttester.commands.InputActions.press_keys import *
+from alttester.commands.InputActions.scroll_mouse import *
+from alttester.commands.InputActions.swipe import *
+from alttester.commands.InputActions.tap_coordinates import *
+from alttester.commands.InputActions.tilt import *
```

### Comparing `AltTester-Driver-2.0.3/alttester/commands/get_server_version.py` & `alttester_driver-2.1.0/alttester/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from alttester.commands.base_command import BaseCommand
-
-
-class GetServerVersion(BaseCommand):
-
-    def __init__(self, connection):
-        super().__init__(connection, "getServerVersion")
-
-    def execute(self):
-        return self.send()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from alttester.altdriver import AltDriver
+from alttester.altobject import AltObject
+from alttester.by import By
+from alttester.playerpref import PlayerPrefKeyType
+from alttester.keycode import AltKeyCode
+from alttester.logging import AltLogLevel, AltLogger
+from alttester.exceptions import *
+from alttester.reverse_port_forwarding import *
```

### Comparing `AltTester-Driver-2.0.3/alttester/exceptions.py` & `alttester_driver-2.1.0/alttester/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,141 +1,157 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-"""This module contains the set of AltTester's exceptions."""
-
-
-class AltException(Exception):
-    """Base exception class for AltTester."""
-
-
-class ConnectionError(AltException):
-    """Raised when the client can not connect to the server. Used as base class for all connection exceptions."""
-
-
-class ConnectionTimeoutError(ConnectionError):
-    """Raised when the client connection timeouts."""
-
-
-class NoAppConnected(ConnectionError):
-    """Raised when the client tries to connect to a server without an app."""
-
-
-class AppDisconnectedError(ConnectionError):
-    """Raised when the app closed the connection or unexpectedly disconnected."""
-
-
-class AltTesterInvalidServerResponse(AltException):
-    """Raised when the server responds with an invalid response."""
-
-    def __init__(self, expected, received):
-        super().__init__("Expected to get response {}; got {}".format(expected, received))
-
-
-class InvalidParameterTypeException(TypeError, AltException):
-    """Raised when an function or method receives an parameter that has the inappropriate type."""
-
-    def __init__(self, parameter_name, expected_types, received_type):
-        expected_types = [expected_type.__name__ for expected_type in expected_types]
-        expected_types = ", ".join(expected_types)
-
-        super().__init__(
-            "TypeError: {} must be {}; not {}.".format(parameter_name, expected_types, received_type.__name__)
-        )
-
-
-class InvalidParameterValueException(ValueError, AltException):
-    """Raised when an function or method receives an parameter that has the right type but an inappropriate value."""
-
-
-class NotFoundException(AltException):
-    """Raised when a object, camera, component, property, method or assembly is not found."""
-
-
-class SceneNotFoundException(NotFoundException):
-    """Raised when a scene is not found."""
-
-
-class ObjectNotFoundException(NotFoundException):
-    """Raised when a object is not found."""
-
-
-class CameraNotFoundException(NotFoundException):
-    """Raised when a camera is not found."""
-
-
-class PropertyNotFoundException(NotFoundException):
-    """Raised when a property is not found."""
-
-
-class MethodNotFoundException(NotFoundException):
-    """Raised when a method is not found."""
-
-
-class MethodWithGivenParametersNotFoundException(NotFoundException):
-    """Raised when a method with the given parameters is not found."""
-
-
-class ComponentNotFoundException(NotFoundException):
-    """Raised when a component is not found."""
-
-
-class AssemblyNotFoundException(NotFoundException):
-    """Raised when an assembly is not found."""
-
-
-class CouldNotPerformOperationException(AltException):
-    """Raised when an operation could not be performed."""
-
-
-class CouldNotParseJsonStringException(AltException):
-    """Raised when AltTester could not parse an JSON command."""
-
-
-class NullReferenceException(AltException):
-    """Raised when there is an attempt to dereference a null object reference."""
-
-
-class FailedToParseArgumentsException(AltException):
-    """Raised when a method arguments could not be parsed by AltTester."""
-
-
-class WaitTimeOutException(AltException):
-    """Raised when a wait command times out."""
-
-
-class CommandResponseTimeoutException(AltException):
-    """Raised when a command does't send a response in the given time."""
-
-
-class PropertyCannotBeSetException(AltException):
-    """Raised when a property could not be found or it's value could not be updated."""
-
-
-class FormatException(AltException):
-    pass
-
-
-class InvalidPathException(AltException):
-    """Raised when a command receives an invalid path."""
-
-
-class AltTesterInputModuleException(AltException):
-    pass
-
-
-class UnknownErrorException(AltException):
-    """Raised when an unexpected error occurred."""
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+"""This module contains the set of AltTester's exceptions."""
+
+
+class AltException(Exception):
+    """Base exception class for AltTester."""
+
+
+class ConnectionError(AltException):
+    """Raised when the client can not connect to the server. Used as base class for all connection exceptions."""
+
+
+class ConnectionTimeoutError(ConnectionError):
+    """Raised when the client connection timeouts."""
+
+
+class NoAppConnected(ConnectionError):
+    """Raised when the client tries to connect to a server without an app."""
+
+
+class AppDisconnectedError(ConnectionError):
+    """Raised when the app closed the connection or unexpectedly disconnected."""
+
+
+class MultipleDriverError(ConnectionError):
+    """ Raised when the client tries to connect to a server with a driver already connected.
+      Free accounts are limited to a single driver connection at a time."""
+
+
+class MultipleDriversTryingToConnectException(ConnectionError):
+    """Raised when the client tries to connect to a server at the same time with another driver"""
+
+
+class MaxNoOfConnectionsDriversExceededException(ConnectionError):
+    """Raised when the client tries to connect to a server but the limit of drivers connected
+        is exceeded"""
+
+
+class AltTesterInvalidServerResponse(AltException):
+    """Raised when the server responds with an invalid response."""
+
+    def __init__(self, expected, received):
+        super().__init__("Expected to get response {}; got {}".format(expected, received))
+
+
+class InvalidParameterTypeException(TypeError, AltException):
+    """Raised when an function or method receives an parameter that has the inappropriate type."""
+
+    def __init__(self, parameter_name, expected_types, received_type):
+        expected_types = [
+            expected_type.__name__ for expected_type in expected_types]
+        expected_types = ", ".join(expected_types)
+
+        super().__init__(
+            "TypeError: {} must be {}; not {}.".format(
+                parameter_name, expected_types, received_type.__name__)
+        )
+
+
+class InvalidParameterValueException(ValueError, AltException):
+    """Raised when an function or method receives an parameter that has the right type but an inappropriate value."""
+
+
+class NotFoundException(AltException):
+    """Raised when a object, camera, component, property, method or assembly is not found."""
+
+
+class SceneNotFoundException(NotFoundException):
+    """Raised when a scene is not found."""
+
+
+class ObjectNotFoundException(NotFoundException):
+    """Raised when a object is not found."""
+
+
+class CameraNotFoundException(NotFoundException):
+    """Raised when a camera is not found."""
+
+
+class PropertyNotFoundException(NotFoundException):
+    """Raised when a property is not found."""
+
+
+class MethodNotFoundException(NotFoundException):
+    """Raised when a method is not found."""
+
+
+class MethodWithGivenParametersNotFoundException(NotFoundException):
+    """Raised when a method with the given parameters is not found."""
+
+
+class ComponentNotFoundException(NotFoundException):
+    """Raised when a component is not found."""
+
+
+class AssemblyNotFoundException(NotFoundException):
+    """Raised when an assembly is not found."""
+
+
+class CouldNotPerformOperationException(AltException):
+    """Raised when an operation could not be performed."""
+
+
+class CouldNotParseJsonStringException(AltException):
+    """Raised when AltTester® could not parse an JSON command."""
+
+
+class NullReferenceException(AltException):
+    """Raised when there is an attempt to dereference a null object reference."""
+
+
+class FailedToParseArgumentsException(AltException):
+    """Raised when a method arguments could not be parsed by AltTester."""
+
+
+class WaitTimeOutException(AltException):
+    """Raised when a wait command times out."""
+
+
+class CommandResponseTimeoutException(AltException):
+    """Raised when a command does't send a response in the given time."""
+
+
+class PropertyCannotBeSetException(AltException):
+    """Raised when a property could not be found or it's value could not be updated."""
+
+
+class FormatException(AltException):
+    pass
+
+
+class InvalidPathException(AltException):
+    """Raised when a command receives an invalid path."""
+
+
+class AltTesterInputModuleException(AltException):
+    pass
+
+
+class UnknownErrorException(AltException):
+    """Raised when an unexpected error occurred."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/alttester/keycode.py` & `alttester_driver-2.1.0/alttester/keycode.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from enum import Enum
-
-
-class AltKeyCode(Enum):
-    NoKey = 0
-    Backspace = 8
-    Tab = 9
-    Clear = 12
-    Return = 13
-    Pause = 19
-    Escape = 27
-    Space = 32
-    Exclaim = 33
-    DoubleQuote = 34
-    Hash = 35
-    Dollar = 36
-    Ampersand = 38
-    Quote = 39
-    LeftParen = 40
-    RightParen = 41
-    Asterisk = 42
-    Plus = 43
-    Comma = 44
-    Minus = 45
-    Period = 46
-    Slash = 47
-    Alpha0 = 48
-    Alpha1 = 49
-    Alpha2 = 50
-    Alpha3 = 51
-    Alpha4 = 52
-    Alpha5 = 53
-    Alpha6 = 54
-    Alpha7 = 55
-    Alpha8 = 56
-    Alpha9 = 57
-    Colon = 58
-    Semicolon = 59
-    Less = 60
-    Equals = 61
-    Greater = 62
-    Question = 63
-    At = 64
-    LeftBracket = 91
-    Backslash = 92
-    RightBracket = 93
-    Caret = 94
-    Underscore = 95
-    BackQuote = 96
-    A = 97
-    B = 98
-    C = 99
-    D = 100
-    E = 101
-    F = 102
-    G = 103
-    H = 104
-    I = 105
-    J = 106
-    K = 107
-    L = 108
-    M = 109
-    N = 110
-    O = 111
-    P = 112
-    Q = 113
-    R = 114
-    S = 115
-    T = 116
-    U = 117
-    V = 118
-    W = 119
-    X = 120
-    Y = 121
-    Z = 122
-    Delete = 127
-    Keypad0 = 256
-    Keypad1 = 257
-    Keypad2 = 258
-    Keypad3 = 259
-    Keypad4 = 260
-    Keypad5 = 261
-    Keypad6 = 262
-    Keypad7 = 263
-    Keypad8 = 264
-    Keypad9 = 265
-    KeypadPeriod = 266
-    KeypadDivide = 267
-    KeypadMultiply = 268
-    KeypadMinus = 269
-    KeypadPlus = 270
-    KeypadEnter = 271
-    KeypadEquals = 272
-    UpArrow = 273
-    DownArrow = 274
-    RightArrow = 275
-    LeftArrow = 276
-    Insert = 277
-    Home = 278
-    End = 279
-    PageUp = 280
-    PageDown = 281
-    F1 = 282
-    F2 = 283
-    F3 = 284
-    F4 = 285
-    F5 = 286
-    F6 = 287
-    F7 = 288
-    F8 = 289
-    F9 = 290
-    F10 = 291
-    F11 = 292
-    F12 = 293
-    F13 = 294
-    F14 = 295
-    F15 = 296
-    Numlock = 300
-    CapsLock = 301
-    ScrollLock = 302
-    RightShift = 303
-    LeftShift = 304
-    RightControl = 305
-    LeftControl = 306
-    RightAlt = 307
-    LeftAlt = 308
-    RightCommand = 309
-    RightApple = 309
-    LeftCommand = 310
-    LeftApple = 310
-    LeftWindows = 311
-    RightWindows = 312
-    AltGr = 313
-    Help = 315
-    Print = 316
-    SysReq = 317
-    Break = 318
-    Menu = 319
-    Mouse0 = 323
-    Mouse1 = 324
-    Mouse2 = 325
-    Mouse3 = 326
-    Mouse4 = 327
-    Mouse5 = 328
-    Mouse6 = 329
-    JoystickButton0 = 330
-    JoystickButton1 = 331
-    JoystickButton2 = 332
-    JoystickButton3 = 333
-    JoystickButton4 = 334
-    JoystickButton5 = 335
-    JoystickButton6 = 336
-    JoystickButton7 = 337
-    JoystickButton8 = 338
-    JoystickButton9 = 339
-    JoystickButton10 = 340
-    JoystickButton11 = 341
-    JoystickButton12 = 342
-    JoystickButton13 = 343
-    JoystickButton14 = 344
-    JoystickButton15 = 345
-    JoystickButton16 = 346
-    JoystickButton17 = 347
-    JoystickButton18 = 348
-    JoystickButton19 = 349
-    Joystick1Button0 = 350
-    Joystick1Button1 = 351
-    Joystick1Button2 = 352
-    Joystick1Button3 = 353
-    Joystick1Button4 = 354
-    Joystick1Button5 = 355
-    Joystick1Button6 = 356
-    Joystick1Button7 = 357
-    Joystick1Button8 = 358
-    Joystick1Button9 = 359
-    Joystick1Button10 = 360
-    Joystick1Button11 = 361
-    Joystick1Button12 = 362
-    Joystick1Button13 = 363
-    Joystick1Button14 = 364
-    Joystick1Button15 = 365
-    Joystick1Button16 = 366
-    Joystick1Button17 = 367
-    Joystick1Button18 = 368
-    Joystick1Button19 = 369
-    Joystick2Button0 = 370
-    Joystick2Button1 = 371
-    Joystick2Button2 = 372
-    Joystick2Button3 = 373
-    Joystick2Button4 = 374
-    Joystick2Button5 = 375
-    Joystick2Button6 = 376
-    Joystick2Button7 = 377
-    Joystick2Button8 = 378
-    Joystick2Button9 = 379
-    Joystick2Button10 = 380
-    Joystick2Button11 = 381
-    Joystick2Button12 = 382
-    Joystick2Button13 = 383
-    Joystick2Button14 = 384
-    Joystick2Button15 = 385
-    Joystick2Button16 = 386
-    Joystick2Button17 = 387
-    Joystick2Button18 = 388
-    Joystick2Button19 = 389
-    Joystick3Button0 = 390
-    Joystick3Button1 = 391
-    Joystick3Button2 = 392
-    Joystick3Button3 = 393
-    Joystick3Button4 = 394
-    Joystick3Button5 = 395
-    Joystick3Button6 = 396
-    Joystick3Button7 = 397
-    Joystick3Button8 = 398
-    Joystick3Button9 = 399
-    Joystick3Button10 = 400
-    Joystick3Button11 = 401
-    Joystick3Button12 = 402
-    Joystick3Button13 = 403
-    Joystick3Button14 = 404
-    Joystick3Button15 = 405
-    Joystick3Button16 = 406
-    Joystick3Button17 = 407
-    Joystick3Button18 = 408
-    Joystick3Button19 = 409
-    Joystick4Button0 = 410
-    Joystick4Button1 = 411
-    Joystick4Button2 = 412
-    Joystick4Button3 = 413
-    Joystick4Button4 = 414
-    Joystick4Button5 = 415
-    Joystick4Button6 = 416
-    Joystick4Button7 = 417
-    Joystick4Button8 = 418
-    Joystick4Button9 = 419
-    Joystick4Button10 = 420
-    Joystick4Button11 = 421
-    Joystick4Button12 = 422
-    Joystick4Button13 = 423
-    Joystick4Button14 = 424
-    Joystick4Button15 = 425
-    Joystick4Button16 = 426
-    Joystick4Button17 = 427
-    Joystick4Button18 = 428
-    Joystick4Button19 = 429
-    Joystick5Button0 = 430
-    Joystick5Button1 = 431
-    Joystick5Button2 = 432
-    Joystick5Button3 = 433
-    Joystick5Button4 = 434
-    Joystick5Button5 = 435
-    Joystick5Button6 = 436
-    Joystick5Button7 = 437
-    Joystick5Button8 = 438
-    Joystick5Button9 = 439
-    Joystick5Button10 = 440
-    Joystick5Button11 = 441
-    Joystick5Button12 = 442
-    Joystick5Button13 = 443
-    Joystick5Button14 = 444
-    Joystick5Button15 = 445
-    Joystick5Button16 = 446
-    Joystick5Button17 = 447
-    Joystick5Button18 = 448
-    Joystick5Button19 = 449
-    Joystick6Button0 = 450
-    Joystick6Button1 = 451
-    Joystick6Button2 = 452
-    Joystick6Button3 = 453
-    Joystick6Button4 = 454
-    Joystick6Button5 = 455
-    Joystick6Button6 = 456
-    Joystick6Button7 = 457
-    Joystick6Button8 = 458
-    Joystick6Button9 = 459
-    Joystick6Button10 = 460
-    Joystick6Button11 = 461
-    Joystick6Button12 = 462
-    Joystick6Button13 = 463
-    Joystick6Button14 = 464
-    Joystick6Button15 = 465
-    Joystick6Button16 = 466
-    Joystick6Button17 = 467
-    Joystick6Button18 = 468
-    Joystick6Button19 = 469
-    Joystick7Button0 = 470
-    Joystick7Button1 = 471
-    Joystick7Button2 = 472
-    Joystick7Button3 = 473
-    Joystick7Button4 = 474
-    Joystick7Button5 = 475
-    Joystick7Button6 = 476
-    Joystick7Button7 = 477
-    Joystick7Button8 = 478
-    Joystick7Button9 = 479
-    Joystick7Button10 = 480
-    Joystick7Button11 = 481
-    Joystick7Button12 = 482
-    Joystick7Button13 = 483
-    Joystick7Button14 = 484
-    Joystick7Button15 = 485
-    Joystick7Button16 = 486
-    Joystick7Button17 = 487
-    Joystick7Button18 = 488
-    Joystick7Button19 = 489
-    Joystick8Button0 = 490
-    Joystick8Button1 = 491
-    Joystick8Button2 = 492
-    Joystick8Button3 = 493
-    Joystick8Button4 = 494
-    Joystick8Button5 = 495
-    Joystick8Button6 = 496
-    Joystick8Button7 = 497
-    Joystick8Button8 = 498
-    Joystick8Button9 = 499
-    Joystick8Button10 = 500
-    Joystick8Button11 = 501
-    Joystick8Button12 = 502
-    Joystick8Button13 = 503
-    Joystick8Button14 = 504
-    Joystick8Button15 = 505
-    Joystick8Button16 = 506
-    Joystick8Button17 = 507
-    Joystick8Button18 = 508
-    Joystick8Button19 = 509
-
-    def __str__(self):
-        return self.name
-
-    @classmethod
-    def names(cls):
-        return [key_code.name for key_code in cls]
-
-    @classmethod
-    def values(cls):
-        return [key_code.value for key_code in cls]
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from enum import Enum
+
+
+class AltKeyCode(Enum):
+    NoKey = 0
+    Backspace = 8
+    Tab = 9
+    Clear = 12
+    Return = 13
+    Pause = 19
+    Escape = 27
+    Space = 32
+    Exclaim = 33
+    DoubleQuote = 34
+    Hash = 35
+    Dollar = 36
+    Ampersand = 38
+    Quote = 39
+    LeftParen = 40
+    RightParen = 41
+    Asterisk = 42
+    Plus = 43
+    Comma = 44
+    Minus = 45
+    Period = 46
+    Slash = 47
+    Alpha0 = 48
+    Alpha1 = 49
+    Alpha2 = 50
+    Alpha3 = 51
+    Alpha4 = 52
+    Alpha5 = 53
+    Alpha6 = 54
+    Alpha7 = 55
+    Alpha8 = 56
+    Alpha9 = 57
+    Colon = 58
+    Semicolon = 59
+    Less = 60
+    Equals = 61
+    Greater = 62
+    Question = 63
+    At = 64
+    LeftBracket = 91
+    Backslash = 92
+    RightBracket = 93
+    Caret = 94
+    Underscore = 95
+    BackQuote = 96
+    A = 97
+    B = 98
+    C = 99
+    D = 100
+    E = 101
+    F = 102
+    G = 103
+    H = 104
+    I = 105
+    J = 106
+    K = 107
+    L = 108
+    M = 109
+    N = 110
+    O = 111
+    P = 112
+    Q = 113
+    R = 114
+    S = 115
+    T = 116
+    U = 117
+    V = 118
+    W = 119
+    X = 120
+    Y = 121
+    Z = 122
+    Delete = 127
+    Keypad0 = 256
+    Keypad1 = 257
+    Keypad2 = 258
+    Keypad3 = 259
+    Keypad4 = 260
+    Keypad5 = 261
+    Keypad6 = 262
+    Keypad7 = 263
+    Keypad8 = 264
+    Keypad9 = 265
+    KeypadPeriod = 266
+    KeypadDivide = 267
+    KeypadMultiply = 268
+    KeypadMinus = 269
+    KeypadPlus = 270
+    KeypadEnter = 271
+    KeypadEquals = 272
+    UpArrow = 273
+    DownArrow = 274
+    RightArrow = 275
+    LeftArrow = 276
+    Insert = 277
+    Home = 278
+    End = 279
+    PageUp = 280
+    PageDown = 281
+    F1 = 282
+    F2 = 283
+    F3 = 284
+    F4 = 285
+    F5 = 286
+    F6 = 287
+    F7 = 288
+    F8 = 289
+    F9 = 290
+    F10 = 291
+    F11 = 292
+    F12 = 293
+    F13 = 294
+    F14 = 295
+    F15 = 296
+    Numlock = 300
+    CapsLock = 301
+    ScrollLock = 302
+    RightShift = 303
+    LeftShift = 304
+    RightControl = 305
+    LeftControl = 306
+    RightAlt = 307
+    LeftAlt = 308
+    RightCommand = 309
+    RightApple = 309
+    LeftCommand = 310
+    LeftApple = 310
+    LeftWindows = 311
+    RightWindows = 312
+    AltGr = 313
+    Help = 315
+    Print = 316
+    SysReq = 317
+    Break = 318
+    Menu = 319
+    Mouse0 = 323
+    Mouse1 = 324
+    Mouse2 = 325
+    Mouse3 = 326
+    Mouse4 = 327
+    Mouse5 = 328
+    Mouse6 = 329
+    JoystickButton0 = 330
+    JoystickButton1 = 331
+    JoystickButton2 = 332
+    JoystickButton3 = 333
+    JoystickButton4 = 334
+    JoystickButton5 = 335
+    JoystickButton6 = 336
+    JoystickButton7 = 337
+    JoystickButton8 = 338
+    JoystickButton9 = 339
+    JoystickButton10 = 340
+    JoystickButton11 = 341
+    JoystickButton12 = 342
+    JoystickButton13 = 343
+    JoystickButton14 = 344
+    JoystickButton15 = 345
+    JoystickButton16 = 346
+    JoystickButton17 = 347
+    JoystickButton18 = 348
+    JoystickButton19 = 349
+    Joystick1Button0 = 350
+    Joystick1Button1 = 351
+    Joystick1Button2 = 352
+    Joystick1Button3 = 353
+    Joystick1Button4 = 354
+    Joystick1Button5 = 355
+    Joystick1Button6 = 356
+    Joystick1Button7 = 357
+    Joystick1Button8 = 358
+    Joystick1Button9 = 359
+    Joystick1Button10 = 360
+    Joystick1Button11 = 361
+    Joystick1Button12 = 362
+    Joystick1Button13 = 363
+    Joystick1Button14 = 364
+    Joystick1Button15 = 365
+    Joystick1Button16 = 366
+    Joystick1Button17 = 367
+    Joystick1Button18 = 368
+    Joystick1Button19 = 369
+    Joystick2Button0 = 370
+    Joystick2Button1 = 371
+    Joystick2Button2 = 372
+    Joystick2Button3 = 373
+    Joystick2Button4 = 374
+    Joystick2Button5 = 375
+    Joystick2Button6 = 376
+    Joystick2Button7 = 377
+    Joystick2Button8 = 378
+    Joystick2Button9 = 379
+    Joystick2Button10 = 380
+    Joystick2Button11 = 381
+    Joystick2Button12 = 382
+    Joystick2Button13 = 383
+    Joystick2Button14 = 384
+    Joystick2Button15 = 385
+    Joystick2Button16 = 386
+    Joystick2Button17 = 387
+    Joystick2Button18 = 388
+    Joystick2Button19 = 389
+    Joystick3Button0 = 390
+    Joystick3Button1 = 391
+    Joystick3Button2 = 392
+    Joystick3Button3 = 393
+    Joystick3Button4 = 394
+    Joystick3Button5 = 395
+    Joystick3Button6 = 396
+    Joystick3Button7 = 397
+    Joystick3Button8 = 398
+    Joystick3Button9 = 399
+    Joystick3Button10 = 400
+    Joystick3Button11 = 401
+    Joystick3Button12 = 402
+    Joystick3Button13 = 403
+    Joystick3Button14 = 404
+    Joystick3Button15 = 405
+    Joystick3Button16 = 406
+    Joystick3Button17 = 407
+    Joystick3Button18 = 408
+    Joystick3Button19 = 409
+    Joystick4Button0 = 410
+    Joystick4Button1 = 411
+    Joystick4Button2 = 412
+    Joystick4Button3 = 413
+    Joystick4Button4 = 414
+    Joystick4Button5 = 415
+    Joystick4Button6 = 416
+    Joystick4Button7 = 417
+    Joystick4Button8 = 418
+    Joystick4Button9 = 419
+    Joystick4Button10 = 420
+    Joystick4Button11 = 421
+    Joystick4Button12 = 422
+    Joystick4Button13 = 423
+    Joystick4Button14 = 424
+    Joystick4Button15 = 425
+    Joystick4Button16 = 426
+    Joystick4Button17 = 427
+    Joystick4Button18 = 428
+    Joystick4Button19 = 429
+    Joystick5Button0 = 430
+    Joystick5Button1 = 431
+    Joystick5Button2 = 432
+    Joystick5Button3 = 433
+    Joystick5Button4 = 434
+    Joystick5Button5 = 435
+    Joystick5Button6 = 436
+    Joystick5Button7 = 437
+    Joystick5Button8 = 438
+    Joystick5Button9 = 439
+    Joystick5Button10 = 440
+    Joystick5Button11 = 441
+    Joystick5Button12 = 442
+    Joystick5Button13 = 443
+    Joystick5Button14 = 444
+    Joystick5Button15 = 445
+    Joystick5Button16 = 446
+    Joystick5Button17 = 447
+    Joystick5Button18 = 448
+    Joystick5Button19 = 449
+    Joystick6Button0 = 450
+    Joystick6Button1 = 451
+    Joystick6Button2 = 452
+    Joystick6Button3 = 453
+    Joystick6Button4 = 454
+    Joystick6Button5 = 455
+    Joystick6Button6 = 456
+    Joystick6Button7 = 457
+    Joystick6Button8 = 458
+    Joystick6Button9 = 459
+    Joystick6Button10 = 460
+    Joystick6Button11 = 461
+    Joystick6Button12 = 462
+    Joystick6Button13 = 463
+    Joystick6Button14 = 464
+    Joystick6Button15 = 465
+    Joystick6Button16 = 466
+    Joystick6Button17 = 467
+    Joystick6Button18 = 468
+    Joystick6Button19 = 469
+    Joystick7Button0 = 470
+    Joystick7Button1 = 471
+    Joystick7Button2 = 472
+    Joystick7Button3 = 473
+    Joystick7Button4 = 474
+    Joystick7Button5 = 475
+    Joystick7Button6 = 476
+    Joystick7Button7 = 477
+    Joystick7Button8 = 478
+    Joystick7Button9 = 479
+    Joystick7Button10 = 480
+    Joystick7Button11 = 481
+    Joystick7Button12 = 482
+    Joystick7Button13 = 483
+    Joystick7Button14 = 484
+    Joystick7Button15 = 485
+    Joystick7Button16 = 486
+    Joystick7Button17 = 487
+    Joystick7Button18 = 488
+    Joystick7Button19 = 489
+    Joystick8Button0 = 490
+    Joystick8Button1 = 491
+    Joystick8Button2 = 492
+    Joystick8Button3 = 493
+    Joystick8Button4 = 494
+    Joystick8Button5 = 495
+    Joystick8Button6 = 496
+    Joystick8Button7 = 497
+    Joystick8Button8 = 498
+    Joystick8Button9 = 499
+    Joystick8Button10 = 500
+    Joystick8Button11 = 501
+    Joystick8Button12 = 502
+    Joystick8Button13 = 503
+    Joystick8Button14 = 504
+    Joystick8Button15 = 505
+    Joystick8Button16 = 506
+    Joystick8Button17 = 507
+    Joystick8Button18 = 508
+    Joystick8Button19 = 509
+
+    def __str__(self):
+        return self.name
+
+    @classmethod
+    def names(cls):
+        return [key_code.name for key_code in cls]
+
+    @classmethod
+    def values(cls):
+        return [key_code.value for key_code in cls]
```

### Comparing `AltTester-Driver-2.0.3/alttester/logging.py` & `alttester_driver-2.1.0/alttester/logging.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from enum import Enum, unique
-
-
-@unique
-class AltLogger(Enum):
-    File = 0
-    Unity = 1
-    Console = 2
-
-    def __str__(self):
-        return self.name
-
-
-@unique
-class AltLogLevel(Enum):
-    Trace = 0
-    Debug = 1
-    Info = 2
-    Warn = 3
-    Error = 4
-    Fatal = 5
-    Off = 6
-
-    def __str__(self):
-        return self.name
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from enum import Enum, unique
+
+
+@unique
+class AltLogger(Enum):
+    File = 0
+    Unity = 1
+    Console = 2
+
+    def __str__(self):
+        return self.name
+
+
+@unique
+class AltLogLevel(Enum):
+    Trace = 0
+    Debug = 1
+    Info = 2
+    Warn = 3
+    Error = 4
+    Fatal = 5
+    Off = 6
+
+    def __str__(self):
+        return self.name
```

### Comparing `AltTester-Driver-2.0.3/alttester/reverse_port_forwarding.py` & `alttester_driver-2.1.0/alttester/reverse_port_forwarding.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import subprocess
-
-from ppadb.client import Client as AdbClient
-
-
-class AltReversePortForwarding:
-    _client = AdbClient(host="127.0.0.1", port=5037)
-
-    @classmethod
-    def _get_device(cls, device_id=""):
-        if device_id == "":
-            devices = cls._client.devices()
-            if len(devices) == 0:
-                raise Exception("No device found")
-            return devices[0]
-        else:
-            return cls._client.device(device_id)
-
-    @staticmethod
-    def reverse_port_forwarding_android(device_port=13000, local_port=13000):
-        subprocess.Popen(['adb', 'reverse', 'tcp:' + str(device_port), 'tcp:' + str(local_port)]).wait()
-
-    @staticmethod
-    def remove_reverse_port_forwarding_android(device_port=13000):
-        subprocess.Popen(['adb', 'reverse', '--remove', 'tcp:' + str(device_port)]).wait()
-
-    @staticmethod
-    def remove_all_reverse_port_forwardings_android():
-        subprocess.Popen(['adb', 'reverse', '--remove-all']).wait()
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import subprocess
+
+from ppadb.client import Client as AdbClient
+
+
+class AltReversePortForwarding:
+    _client = AdbClient(host="127.0.0.1", port=5037)
+
+    @classmethod
+    def _get_device(cls, device_id=""):
+        if device_id == "":
+            devices = cls._client.devices()
+            if len(devices) == 0:
+                raise Exception("No device found")
+            return devices[0]
+        else:
+            return cls._client.device(device_id)
+
+    @staticmethod
+    def reverse_port_forwarding_android(device_port=13000, local_port=13000):
+        subprocess.Popen(['adb', 'reverse', 'tcp:' + str(device_port), 'tcp:' + str(local_port)]).wait()
+
+    @staticmethod
+    def remove_reverse_port_forwarding_android(device_port=13000):
+        subprocess.Popen(['adb', 'reverse', '--remove', 'tcp:' + str(device_port)]).wait()
+
+    @staticmethod
+    def remove_all_reverse_port_forwardings_android():
+        subprocess.Popen(['adb', 'reverse', '--remove-all']).wait()
```

### Comparing `AltTester-Driver-2.0.3/setup.py` & `alttester_driver-2.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from setuptools import setup, find_packages
-
-
-NAME = 'AltTester-Driver'
-DESCRIPTION = "Python bindings for the AltTester framework. AltTester is an open-source UI driven test " \
-    "automation tool that helps you find objects in your game and interacts with them."
-URL = 'https://alttester.com/docs/sdk/latest/'
-EMAIL = 'contact@alttester.com'
-AUTHOR = 'Altom Consulting'
-REQUIRES_PYTHON = '>=3.4.0'
-LICENSE = 'GNU GPLv3'
-
-
-with open("alttester/__version__.py") as f:
-    for line in f.readlines():
-        if "VERSION = " in line:
-            VERSION = line.replace(
-                "VERSION = ", "").replace("\"", "").replace("\n", "")
-
-with open('requirements.txt') as f:
-    REQUIRED = f.read().splitlines()
-
-
-with open('README.md') as f:
-    README = f.read()
-
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=README,
-    long_description_content_type='text/markdown',
-    license=LICENSE,
-    url=URL,
-    project_urls={
-        "Bug Tracker": "https://github.com/alttester/AltTester-Unity-SDK/issues",
-        "Documentation": "https://alttester.com/docs/sdk/latest",
-        "Source": "https://github.com/alttester/AltTester-Unity-SDK",
-    },
-
-    author=AUTHOR,
-    author_email=EMAIL,
-
-    zip_safe=False,
-    python_requires=REQUIRES_PYTHON,
-    setup_requires=REQUIRED,
-    install_requires=REQUIRED,
-    packages=find_packages(exclude=['tests']),
-    include_package_data=True,
-
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-
-        "Intended Audience :: Developers",
-        "Intended Audience :: Other Audience",
-
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-
-        "Programming Language :: C#",
-        "Programming Language :: Java",
-        "Programming Language :: Cython",
-        "Programming Language :: Python :: Implementation",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-
-        "Operating System :: OS Independent",
-
-        "Topic :: Games/Entertainment",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Testing",
-        "Topic :: Software Development :: Testing :: Acceptance",
-        "Topic :: Software Development :: Testing :: Unit",
-    ],
-    keywords="unity testing tests",
-)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+from setuptools import setup, find_packages
+
+
+NAME = 'AltTester-Driver'
+DESCRIPTION = "Python bindings for the AltTester® framework. AltTester® is an open-source UI driven test " \
+    "automation tool that helps you find objects in your game and interacts with them."
+URL = 'https://alttester.com/docs/sdk/latest/'
+EMAIL = 'contact@alttester.com'
+AUTHOR = 'Altom Consulting'
+REQUIRES_PYTHON = '>=3.4.0'
+LICENSE = 'GNU GPLv3'
+
+
+with open("alttester/__version__.py") as f:
+    for line in f.readlines():
+        if "VERSION = " in line:
+            VERSION = line.replace(
+                "VERSION = ", "").replace("\"", "").replace("\n", "")
+
+with open('requirements.txt') as f:
+    REQUIRED = f.read().splitlines()
+
+
+with open('README.md') as f:
+    README = f.read()
+
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=README,
+    long_description_content_type='text/markdown',
+    license=LICENSE,
+    url=URL,
+    project_urls={
+        "Bug Tracker": "https://github.com/alttester/AltTester-Unity-SDK/issues",
+        "Documentation": "https://alttester.com/docs/sdk/latest",
+        "Source": "https://github.com/alttester/AltTester-Unity-SDK",
+    },
+
+    author=AUTHOR,
+    author_email=EMAIL,
+
+    zip_safe=False,
+    python_requires=REQUIRES_PYTHON,
+    setup_requires=REQUIRED,
+    install_requires=REQUIRED,
+    packages=find_packages(exclude=['tests']),
+    include_package_data=True,
+
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+
+        "Intended Audience :: Developers",
+        "Intended Audience :: Other Audience",
+
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+
+        "Programming Language :: C#",
+        "Programming Language :: Java",
+        "Programming Language :: Cython",
+        "Programming Language :: Python :: Implementation",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+
+        "Operating System :: OS Independent",
+
+        "Topic :: Games/Entertainment",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Testing",
+        "Topic :: Software Development :: Testing :: Acceptance",
+        "Topic :: Software Development :: Testing :: Unit",
+    ],
+    keywords="unity testing tests",
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_driver.py` & `alttester_driver-2.1.0/tests/integration/test_driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import os
-
-import pytest
-
-from .utils import Scenes
-from alttester import By
-from alttester.__version__ import VERSION
-from alttester.commands import GetServerVersion
-from alttester.logging import AltLogLevel, AltLogger
-import alttester.exceptions as exceptions
-
-
-class TestDriver:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-
-    def test_get_version(self):
-        server_version = GetServerVersion.run(self.altdriver._connection)
-        assert VERSION.startswith(server_version)
-
-    def test_load_and_wait_for_scene(self):
-        self.altdriver.load_scene(Scenes.Scene01)
-        self.altdriver.wait_for_current_scene_to_be(Scenes.Scene01, timeout=1)
-
-        self.altdriver.load_scene(Scenes.Scene02)
-        self.altdriver.wait_for_current_scene_to_be(Scenes.Scene02, timeout=1)
-
-        assert self.altdriver.get_current_scene() == Scenes.Scene02
-
-    def test_wait_for_current_scene_to_be_with_a_non_existing_scene(self):
-        scene_name = "Scene 0"
-
-        with pytest.raises(exceptions.WaitTimeOutException) as execinfo:
-            self.altdriver.wait_for_current_scene_to_be(scene_name, timeout=1, interval=0.5)
-
-        assert str(execinfo.value) == "Scene {} not loaded after 1 seconds".format(scene_name)
-
-    def test_set_and_get_time_scale(self):
-        self.altdriver.set_time_scale(0.1)
-
-        assert self.altdriver.get_time_scale() == 0.1
-
-        self.altdriver.set_time_scale(1)
-
-    def test_screenshot(self):
-        png_path = "testPython.png"
-        self.altdriver.get_png_screenshot(png_path)
-        assert os.path.exists(png_path)
-
-    def test_wait_for_object_which_contains_with_tag(self):
-        alt_object = self.altdriver.wait_for_object_which_contains(
-            By.NAME, "Canva",
-            By.TAG, "MainCamera"
-        )
-        assert alt_object.name == "Canvas"
-
-    def test_load_additive_scenes(self):
-        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
-
-        initial_number_of_elements = self.altdriver.get_all_elements()
-        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
-        final_number_of_elements = self.altdriver.get_all_elements()
-
-        assert len(final_number_of_elements) > len(initial_number_of_elements)
-
-        scenes = self.altdriver.get_all_loaded_scenes()
-        assert len(scenes) == 2
-
-    def test_load_scene_with_invalid_scene_name(self):
-        with pytest.raises(exceptions.SceneNotFoundException):
-            self.altdriver.load_scene("Scene 0")
-
-    def test_unload_scene(self):
-        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
-        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
-
-        assert len(self.altdriver.get_all_loaded_scenes()) == 2
-
-        self.altdriver.unload_scene(Scenes.Scene02)
-        assert len(self.altdriver.get_all_loaded_scenes()) == 1
-        assert self.altdriver.get_all_loaded_scenes()[0] == Scenes.Scene01
-
-    def test_unload_only_scene(self):
-        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
-
-        with pytest.raises(exceptions.CouldNotPerformOperationException):
-            self.altdriver.unload_scene(Scenes.Scene01)
-
-    @pytest.mark.WebGLUnsupported
-    def test_set_server_logging(self):
-        rule = self.altdriver.call_static_method(
-            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
-            "Instance.Configuration.FindRuleByName",
-            "Assembly-CSharp",
-            parameters=["AltServerFileRule"],
-        )
-
-        # Default logging level in AltTester is Debug level
-        assert len(rule["Levels"]) == 5
-
-        self.altdriver.set_server_logging(AltLogger.File, AltLogLevel.Off)
-        rule = self.altdriver.call_static_method(
-            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
-            "Instance.Configuration.FindRuleByName",
-            "Assembly-CSharp",
-            parameters=["AltServerFileRule"],
-        )
-
-        assert len(rule["Levels"]) == 0
-
-        # Reset logging level
-        self.altdriver.set_server_logging(AltLogger.File, AltLogLevel.Debug)
-
-    @pytest.mark.parametrize(
-        "path", ["//[1]", "CapsuleInfo[@tag=UI]", "//CapsuleInfo[@tag=UI/Text", "//CapsuleInfo[0/Text"]
-    )
-    def test_invalid_paths(self, path):
-        with pytest.raises(exceptions.InvalidPathException):
-            self.altdriver.find_object(By.PATH, path)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import os
+
+import pytest
+
+from .utils import Scenes
+from alttester import By
+from alttester.__version__ import VERSION
+from alttester.commands import GetServerVersion
+from alttester.logging import AltLogLevel, AltLogger
+import alttester.exceptions as exceptions
+
+
+class TestDriver:
+
+    @pytest.fixture(autouse=True)
+    def setup(self, altdriver):
+        self.altdriver = altdriver
+
+    def test_get_version(self):
+        server_version = GetServerVersion.run(self.altdriver._connection)
+        assert VERSION.startswith(server_version)
+
+    def test_load_and_wait_for_scene(self):
+        self.altdriver.load_scene(Scenes.Scene01)
+        self.altdriver.wait_for_current_scene_to_be(Scenes.Scene01, timeout=1)
+
+        self.altdriver.load_scene(Scenes.Scene02)
+        self.altdriver.wait_for_current_scene_to_be(Scenes.Scene02, timeout=1)
+
+        assert self.altdriver.get_current_scene() == Scenes.Scene02
+
+    def test_wait_for_current_scene_to_be_with_a_non_existing_scene(self):
+        scene_name = "Scene 0"
+
+        with pytest.raises(exceptions.WaitTimeOutException) as execinfo:
+            self.altdriver.wait_for_current_scene_to_be(scene_name, timeout=1, interval=0.5)
+
+        assert str(execinfo.value) == "Scene {} not loaded after 1 seconds".format(scene_name)
+
+    def test_set_and_get_time_scale(self):
+        self.altdriver.set_time_scale(0.1)
+
+        assert self.altdriver.get_time_scale() == 0.1
+
+        self.altdriver.set_time_scale(1)
+
+    def test_screenshot(self):
+        png_path = "testPython.png"
+        self.altdriver.get_png_screenshot(png_path)
+        assert os.path.exists(png_path)
+
+    def test_wait_for_object_which_contains_with_tag(self):
+        alt_object = self.altdriver.wait_for_object_which_contains(
+            By.NAME, "Canva",
+            By.TAG, "MainCamera"
+        )
+        assert alt_object.name == "Canvas"
+
+    def test_load_additive_scenes(self):
+        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
+
+        initial_number_of_elements = self.altdriver.get_all_elements()
+        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
+        final_number_of_elements = self.altdriver.get_all_elements()
+
+        assert len(final_number_of_elements) > len(initial_number_of_elements)
+
+        scenes = self.altdriver.get_all_loaded_scenes()
+        assert len(scenes) == 2
+
+    def test_load_scene_with_invalid_scene_name(self):
+        with pytest.raises(exceptions.SceneNotFoundException):
+            self.altdriver.load_scene("Scene 0")
+
+    def test_unload_scene(self):
+        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
+        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
+
+        assert len(self.altdriver.get_all_loaded_scenes()) == 2
+
+        self.altdriver.unload_scene(Scenes.Scene02)
+        assert len(self.altdriver.get_all_loaded_scenes()) == 1
+        assert self.altdriver.get_all_loaded_scenes()[0] == Scenes.Scene01
+
+    def test_unload_only_scene(self):
+        self.altdriver.load_scene(Scenes.Scene01, load_single=True)
+
+        with pytest.raises(exceptions.CouldNotPerformOperationException):
+            self.altdriver.unload_scene(Scenes.Scene01)
+
+    @pytest.mark.WebGLUnsupported
+    def test_set_server_logging(self):
+        rule = self.altdriver.call_static_method(
+            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
+            "Instance.Configuration.FindRuleByName",
+            "Assembly-CSharp",
+            parameters=["AltServerFileRule"],
+        )
+
+        # Default logging level in AltTester® is Debug level
+        assert len(rule["Levels"]) == 5
+
+        self.altdriver.set_server_logging(AltLogger.File, AltLogLevel.Off)
+        rule = self.altdriver.call_static_method(
+            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
+            "Instance.Configuration.FindRuleByName",
+            "Assembly-CSharp",
+            parameters=["AltServerFileRule"],
+        )
+
+        assert len(rule["Levels"]) == 0
+
+        # Reset logging level
+        self.altdriver.set_server_logging(AltLogger.File, AltLogLevel.Debug)
+
+    @pytest.mark.parametrize(
+        "path", ["//[1]", "CapsuleInfo[@tag=UI]", "//CapsuleInfo[@tag=UI/Text", "//CapsuleInfo[0/Text"]
+    )
+    def test_invalid_paths(self, path):
+        with pytest.raises(exceptions.InvalidPathException):
+            self.altdriver.find_object(By.PATH, path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_notifications.py` & `alttester_driver-2.1.0/tests/integration/test_notifications.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import pytest
-
-from .utils import Scenes
-from alttester import By
-from alttester.commands.Notifications.notification_type import NotificationType
-from alttester.commands.Notifications.base_notification_callbacks import BaseNotificationCallbacks
-from alttester.logging import AltLogLevel
-
-
-class MockNotificationCallbacks(BaseNotificationCallbacks):
-    last_scene_loaded = ""
-    last_scene_unloaded = ""
-    log_message = ""
-    log_type = AltLogLevel.Error
-    log_stack_trace = ""
-    application_paused = False
-
-    def scene_loaded_callback(self, load_scene_notification_result):
-        self.last_scene_loaded = load_scene_notification_result.scene_name
-
-    def scene_unloaded_callback(self, scene_name):
-        self.last_scene_unloaded = scene_name
-
-    def log_callback(self, log_notification_result):
-        self.log_message = log_notification_result.message
-        self.log_stack_trace = log_notification_result.stack_trace
-        self.log_type = log_notification_result.type
-
-    def application_paused_callback(self, application_paused):
-        self.application_paused = application_paused
-
-
-class TestNotifications:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-
-    def test_load_scene_notification(self):
-        test_notification_callbacks = MockNotificationCallbacks()
-        self.altdriver.add_notification_listener(
-            NotificationType.LOADSCENE, test_notification_callbacks.scene_loaded_callback)
-        self.altdriver.load_scene(Scenes.Scene01)
-        assert test_notification_callbacks.last_scene_loaded == Scenes.Scene01
-        self.altdriver.remove_notification_listener(NotificationType.LOADSCENE)
-
-    def test_unload_scene_notification(self):
-        test_notification_callbacks = MockNotificationCallbacks()
-        self.altdriver.add_notification_listener(
-            NotificationType.UNLOADSCENE, test_notification_callbacks.scene_unloaded_callback)
-        self.altdriver.load_scene(Scenes.Scene01)
-        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
-        self.altdriver.unload_scene(Scenes.Scene02)
-        assert test_notification_callbacks.last_scene_unloaded == Scenes.Scene02
-        self.altdriver.remove_notification_listener(NotificationType.UNLOADSCENE)
-
-    def test_log_notification(self):
-        test_notification_callbacks = MockNotificationCallbacks()
-        self.altdriver.add_notification_listener(
-            NotificationType.LOG, test_notification_callbacks.log_callback)
-        self.altdriver.load_scene(Scenes.Scene01)
-        assert "Scene Loaded" in test_notification_callbacks.log_message
-        assert test_notification_callbacks.log_type == AltLogLevel.Debug.value
-        self.altdriver.remove_notification_listener(NotificationType.LOG)
-
-    def test_application_paused_notification(self):
-        test_notification_callbacks = MockNotificationCallbacks()
-        self.altdriver.add_notification_listener(
-            NotificationType.APPLICATION_PAUSED, test_notification_callbacks.application_paused_callback)
-        self.altdriver.load_scene(Scenes.Scene01)
-        alt_object = self.altdriver.find_object(By.NAME, "AltTesterPrefab")
-        alt_object.call_component_method(
-            "AltTester.AltTesterUnitySDK.AltRunner", "OnApplicationPause", "AltTester.AltTesterUnitySDK",
-            parameters=[True],
-            type_of_parameters=["System.Boolean"]
-        )
-
-        assert test_notification_callbacks.application_paused
-        self.altdriver.remove_notification_listener(NotificationType.APPLICATION_PAUSED)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import pytest
+
+from .utils import Scenes
+from alttester import By
+from alttester.commands.Notifications.notification_type import NotificationType
+from alttester.commands.Notifications.base_notification_callbacks import BaseNotificationCallbacks
+from alttester.logging import AltLogLevel
+
+
+class MockNotificationCallbacks(BaseNotificationCallbacks):
+    last_scene_loaded = ""
+    last_scene_unloaded = ""
+    log_message = ""
+    log_type = AltLogLevel.Error
+    log_stack_trace = ""
+    application_paused = False
+
+    def scene_loaded_callback(self, load_scene_notification_result):
+        self.last_scene_loaded = load_scene_notification_result.scene_name
+
+    def scene_unloaded_callback(self, scene_name):
+        self.last_scene_unloaded = scene_name
+
+    def log_callback(self, log_notification_result):
+        self.log_message = log_notification_result.message
+        self.log_stack_trace = log_notification_result.stack_trace
+        self.log_type = log_notification_result.type
+
+    def application_paused_callback(self, application_paused):
+        self.application_paused = application_paused
+
+
+class TestNotifications:
+
+    @pytest.fixture(autouse=True)
+    def setup(self, altdriver):
+        self.altdriver = altdriver
+        self.altdriver.reset_input()
+
+    def test_load_scene_notification(self):
+        test_notification_callbacks = MockNotificationCallbacks()
+        self.altdriver.add_notification_listener(
+            NotificationType.LOADSCENE, test_notification_callbacks.scene_loaded_callback)
+        self.altdriver.load_scene(Scenes.Scene01)
+        assert test_notification_callbacks.last_scene_loaded == Scenes.Scene01
+        self.altdriver.remove_notification_listener(NotificationType.LOADSCENE)
+
+    def test_unload_scene_notification(self):
+        test_notification_callbacks = MockNotificationCallbacks()
+        self.altdriver.add_notification_listener(
+            NotificationType.UNLOADSCENE, test_notification_callbacks.scene_unloaded_callback)
+        self.altdriver.load_scene(Scenes.Scene01)
+        self.altdriver.load_scene(Scenes.Scene02, load_single=False)
+        self.altdriver.unload_scene(Scenes.Scene02)
+        assert test_notification_callbacks.last_scene_unloaded == Scenes.Scene02
+        self.altdriver.remove_notification_listener(
+            NotificationType.UNLOADSCENE)
+
+    def test_log_notification(self):
+        test_notification_callbacks = MockNotificationCallbacks()
+        self.altdriver.add_notification_listener(
+            NotificationType.LOG, test_notification_callbacks.log_callback)
+        self.altdriver.load_scene(Scenes.Scene01)
+        assert "\"commandName\":\"loadScene" in test_notification_callbacks.log_message
+        assert test_notification_callbacks.log_type == AltLogLevel.Debug.value
+        self.altdriver.remove_notification_listener(NotificationType.LOG)
+
+    def test_application_paused_notification(self):
+        test_notification_callbacks = MockNotificationCallbacks()
+        self.altdriver.add_notification_listener(
+            NotificationType.APPLICATION_PAUSED, test_notification_callbacks.application_paused_callback)
+        self.altdriver.load_scene(Scenes.Scene01)
+        alt_object = self.altdriver.find_object(By.NAME, "AltTesterPrefab")
+        alt_object.call_component_method(
+            "AltTester.AltTesterUnitySDK.AltRunner", "OnApplicationPause", "AltTester.AltTesterUnitySDK",
+            parameters=[True],
+            type_of_parameters=["System.Boolean"]
+        )
+
+        assert test_notification_callbacks.application_paused
+        self.altdriver.remove_notification_listener(
+            NotificationType.APPLICATION_PAUSED)
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_reverse_port_forwarding.py` & `alttester_driver-2.1.0/tests/integration/test_reverse_port_forwarding.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import unittest
-
-from alttester import By, AltReversePortForwarding, AltDriver
-
-
-@unittest.skip
-class TestReversePortForwarding(unittest.TestCase):
-
-    altdriver = None
-
-    @classmethod
-    def setUpClass(cls):
-        AltReversePortForwarding.reverse_port_forwarding_android()
-        cls.altdriver = AltDriver()
-
-    @classmethod
-    def tearDownClass(cls):
-        cls.altdriver.stop()
-        AltReversePortForwarding.remove_reverse_port_forwarding_android()
-
-    def test_open_close_panel(self):
-        self.altdriver.load_scene("Scene 2 Draggable Panel")
-
-        self.altdriver.find_object(By.NAME, "Close Button").tap()
-        self.altdriver.find_object(By.NAME, "Button").tap()
-
-        panel_element = self.altdriver.wait_for_object(By.NAME, "Panel")
-        self.assertTrue(panel_element.enabled)
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import unittest
+
+from alttester import By, AltReversePortForwarding, AltDriver
+
+
+@unittest.skip
+class TestReversePortForwarding(unittest.TestCase):
+
+    altdriver = None
+
+    @classmethod
+    def setUpClass(cls):
+        AltReversePortForwarding.reverse_port_forwarding_android()
+        cls.altdriver = AltDriver()
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.altdriver.stop()
+        AltReversePortForwarding.remove_reverse_port_forwarding_android()
+
+    def test_open_close_panel(self):
+        self.altdriver.load_scene("Scene 2 Draggable Panel")
+
+        self.altdriver.find_object(By.NAME, "Close Button").tap()
+        self.altdriver.find_object(By.NAME, "Button").tap()
+
+        panel_element = self.altdriver.wait_for_object(By.NAME, "Panel")
+        self.assertTrue(panel_element.enabled)
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_scene02.py` & `alttester_driver-2.1.0/tests/integration/test_scene02.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,154 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import pytest
-
-from .utils import Scenes
-from alttester import By
-
-
-class TestScene02:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-        self.altdriver.load_scene(Scenes.Scene02)
-
-    def test_get_all_elements(self):
-        elements = self.altdriver.get_all_elements(enabled=False)
-        assert elements is not None
-
-        expected_names = {
-            "EventSystem", "Canvas", "Panel Drag Area", "Panel",
-            "Header", "Text", "Drag Zone", "Resize Zone", "Close Button",
-            "Debugging", "SF Scene Elements", "Main Camera", "Background",
-            "Particle System"
-        }
-
-        input_marks = []
-        names = []
-
-        for element in elements:
-            if element.name == "InputMark(Clone)":
-                input_marks.append(element.transformId)
-                continue  # skip InputMark and direct children
-            if element.transformParentId in input_marks:
-                continue  # skip InputMark and direct children
-
-            names.append(element.name)
-
-        for name in expected_names:
-            assert name in names
-
-    def test_get_all_enabled_elements(self):
-        # time.sleep(1)
-
-        elements = self.altdriver.get_all_elements(enabled=True)
-        assert elements is not None
-
-        expected_names = {
-            "EventSystem", "Canvas", "Panel Drag Area", "Panel",
-            "Header", "Text", "Drag Zone", "Resize Zone", "Close Button",
-            "Debugging", "SF Scene Elements", "Main Camera", "Background",
-            "Particle System"
-        }
-        names = [element.name for element in elements]
-        assert len(names) == 24 or len(names) == 25
-        for name in expected_names:
-            assert name in names
-
-    def test_resize_panel(self):
-        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
-        position_init = (alt_object.x, alt_object.y)
-
-        self.altdriver.swipe(
-            alt_object.get_screen_position(),
-            (alt_object.x - 200, alt_object.y - 200),
-            duration=2
-        )
-        # time.sleep(2)
-
-        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
-        position_final = (alt_object.x, alt_object.y)
-
-        assert position_init != position_final
-
-    def test_resize_panel_with_multipoint_swipe(self):
-        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
-        position_init = (alt_object.x, alt_object.y)
-
-        positions = [
-            alt_object.get_screen_position(),
-            [alt_object.x - 200, alt_object.y - 200],
-            [alt_object.x - 300, alt_object.y - 100],
-            [alt_object.x - 50, alt_object.y - 100],
-            [alt_object.x - 100, alt_object.y - 100]
-        ]
-        self.altdriver.multipoint_swipe(positions, duration=4)
-
-        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
-        position_final = (alt_object.x, alt_object.y)
-
-        assert position_init != position_final
-
-    def test_pointer_down_from_object(self):
-        panel = self.altdriver.find_object(By.NAME, "Panel")
-        color1 = panel.get_component_property(
-            "AltExampleScriptPanel",
-            "normalColor",
-            "Assembly-CSharp"
-        )
-        panel.pointer_down()
-
-        color2 = panel.get_component_property(
-            "AltExampleScriptPanel",
-            "highlightColor",
-            "Assembly-CSharp"
-        )
-
-        assert color1 != color2
-
-    def test_pointer_up_from_object(self):
-        panel = self.altdriver.find_object(By.NAME, "Panel")
-        color1 = panel.get_component_property(
-            "AltExampleScriptPanel",
-            "normalColor",
-            "Assembly-CSharp"
-        )
-        panel.pointer_down()
-
-        panel.pointer_up()
-        color2 = panel.get_component_property(
-            "AltExampleScriptPanel",
-            "highlightColor",
-            "Assembly-CSharp"
-        )
-
-        assert color1 == color2
-
-    def test_new_touch_commands(self):
-        draggable_area = self.altdriver.find_object(By.NAME, "Drag Zone")
-        initial_position = draggable_area.get_screen_position()
-
-        finger_id = self.altdriver.begin_touch(draggable_area.get_screen_position())
-        self.altdriver.move_touch(finger_id, [draggable_area.x + 10, draggable_area.y + 10])
-        self.altdriver.end_touch(finger_id)
-
-        draggable_area = self.altdriver.find_object(By.NAME, "Drag Zone")
-        assert initial_position != draggable_area
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import pytest
+
+from .utils import Scenes
+from alttester import By
+
+
+class TestScene02:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.altdriver.reset_input()
+        self.altdriver.load_scene(Scenes.Scene02)
+
+    def test_get_all_elements(self):
+        elements = self.altdriver.get_all_elements(enabled=False)
+        assert elements is not None
+
+        expected_names = {
+            "EventSystem", "Canvas", "Panel Drag Area", "Panel",
+            "Header", "Text", "Drag Zone", "Resize Zone", "Close Button",
+            "Debugging", "SF Scene Elements", "Main Camera", "Background",
+            "Particle System"
+        }
+
+        input_marks = []
+        names = []
+
+        for element in elements:
+            if element.name == "InputMark(Clone)":
+                input_marks.append(element.transformId)
+                continue  # skip InputMark and direct children
+            if element.transformParentId in input_marks:
+                continue  # skip InputMark and direct children
+
+            names.append(element.name)
+
+        for name in expected_names:
+            assert name in names
+
+    def test_get_all_enabled_elements(self):
+        # time.sleep(1)
+
+        elements = self.altdriver.get_all_elements(enabled=True)
+        assert elements is not None
+
+        expected_names = {
+            "EventSystem", "Canvas", "Panel Drag Area", "Panel",
+            "Header", "Text", "Drag Zone", "Resize Zone", "Close Button",
+            "Debugging", "SF Scene Elements", "Main Camera", "Background",
+            "Particle System"
+        }
+        names = [element.name for element in elements]
+        assert len(names) >= 22
+        for name in expected_names:
+            assert name in names
+
+    def test_resize_panel(self):
+        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
+        position_init = (alt_object.x, alt_object.y)
+
+        self.altdriver.swipe(
+            alt_object.get_screen_position(),
+            (alt_object.x - 200, alt_object.y - 200),
+            duration=2
+        )
+        # time.sleep(2)
+
+        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
+        position_final = (alt_object.x, alt_object.y)
+
+        assert position_init != position_final
+
+    def test_resize_panel_with_multipoint_swipe(self):
+        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
+        position_init = (alt_object.x, alt_object.y)
+
+        positions = [
+            alt_object.get_screen_position(),
+            [alt_object.x - 200, alt_object.y - 200],
+            [alt_object.x - 300, alt_object.y - 100],
+            [alt_object.x - 50, alt_object.y - 100],
+            [alt_object.x - 100, alt_object.y - 100]
+        ]
+        self.altdriver.multipoint_swipe(positions, duration=4)
+
+        alt_object = self.altdriver.find_object(By.NAME, "Resize Zone")
+        position_final = (alt_object.x, alt_object.y)
+
+        assert position_init != position_final
+
+    def test_pointer_down_from_object(self):
+        panel = self.altdriver.find_object(By.NAME, "Panel")
+        color1 = panel.get_component_property(
+            "AltExampleScriptPanel",
+            "normalColor",
+            "Assembly-CSharp"
+        )
+        panel.pointer_down()
+
+        color2 = panel.get_component_property(
+            "AltExampleScriptPanel",
+            "highlightColor",
+            "Assembly-CSharp"
+        )
+
+        assert color1 != color2
+
+    def test_pointer_up_from_object(self):
+        panel = self.altdriver.find_object(By.NAME, "Panel")
+        color1 = panel.get_component_property(
+            "AltExampleScriptPanel",
+            "normalColor",
+            "Assembly-CSharp"
+        )
+        panel.pointer_down()
+
+        panel.pointer_up()
+        color2 = panel.get_component_property(
+            "AltExampleScriptPanel",
+            "highlightColor",
+            "Assembly-CSharp"
+        )
+
+        assert color1 == color2
+
+    def test_new_touch_commands(self):
+        draggable_area = self.altdriver.find_object(By.NAME, "Drag Zone")
+        initial_position = draggable_area.get_screen_position()
+
+        finger_id = self.altdriver.begin_touch(
+            draggable_area.get_screen_position())
+        self.altdriver.move_touch(
+            finger_id, [draggable_area.x + 10, draggable_area.y + 10])
+        self.altdriver.end_touch(finger_id)
+
+        draggable_area = self.altdriver.find_object(By.NAME, "Drag Zone")
+        assert initial_position != draggable_area
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_scene03.py` & `alttester_driver-2.1.0/tests/integration/test_scene03.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,164 +1,163 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-
-import pytest
-
-from .utils import Scenes
-from alttester import By
-
-
-class TestScene03:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-        self.altdriver.load_scene(Scenes.Scene03)
-
-    def wait_for_swipe_to_finish(self):
-        self.altdriver.wait_for_object_to_not_be_present(By.NAME, "icon")
-
-    def get_sprite_name(self, source_image_name, image_source_drop_zone_name):
-        image_source = self.altdriver.find_object(
-            By.NAME, source_image_name).get_component_property(
-            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
-        image_source_drop_zone = self.altdriver.find_object(
-            By.NAME, image_source_drop_zone_name).get_component_property(
-            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
-        return image_source, image_source_drop_zone
-
-    def drop_image_with_multipoint_swipe(self, object_names, duration, wait):
-        positions = []
-        for name in object_names:
-            alt_object = self.altdriver.find_object(By.NAME, name)
-            positions.append(alt_object.get_screen_position())
-
-        self.altdriver.multipoint_swipe(positions, duration, wait)
-
-    def drop_image(self, drag_location_name, drop_location_name, duration, wait):
-        drag_location = self.altdriver.find_object(By.NAME, drag_location_name)
-        drop_location = self.altdriver.find_object(By.NAME, drop_location_name)
-
-        self.altdriver.swipe(drag_location.get_screen_position(
-        ), drop_location.get_screen_position(), duration, wait)
-
-    def test_pointer_enter_and_exit(self):
-        alt_object = self.altdriver.find_object(By.NAME, "Drop Image")
-        color1 = alt_object.get_component_property(
-            "AltExampleScriptDropMe",
-            "highlightColor",
-            "Assembly-CSharp"
-        )
-        alt_object.pointer_enter()
-        color2 = alt_object.get_component_property(
-            "AltExampleScriptDropMe",
-            "highlightColor",
-            "Assembly-CSharp"
-        )
-
-        assert color1["r"] != color2["r"] or \
-            color1["g"] != color2["g"] or \
-            color1["b"] != color2["b"] or \
-            color1["a"] != color2["a"]
-
-        alt_object.pointer_exit()
-        color3 = alt_object.get_component_property(
-            "AltExampleScriptDropMe",
-            "highlightColor",
-            "Assembly-CSharp"
-        )
-
-        assert color3["r"] != color2["r"] or \
-            color3["g"] != color2["g"] or \
-            color3["b"] != color2["b"] or \
-            color3["a"] != color2["a"]
-
-        assert color3["r"] == color1["r"] and \
-            color3["g"] == color1["g"] and \
-            color3["b"] == color1["b"] and \
-            color3["a"] == color1["a"]
-
-    def test_multiple_swipes(self):
-        self.drop_image("Drag Image2", "Drop Box2", 1, False)
-        self.drop_image("Drag Image2", "Drop Box1", 1, False)
-        self.drop_image("Drag Image1", "Drop Box1", 2, False)
-        self.wait_for_swipe_to_finish()
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image1", "Drop Image")
-        assert image_source == image_source_drop_zone
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image2", "Drop")
-        assert image_source == image_source_drop_zone
-
-    def test_multiple_swipe_and_waits(self):
-        self.drop_image("Drag Image2", "Drop Box2", 1, True)
-        self.drop_image("Drag Image2", "Drop Box1", 1, True)
-        self.drop_image("Drag Image1", "Drop Box1", 1, True)
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image1", "Drop Image")
-        assert image_source == image_source_drop_zone
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image2", "Drop")
-        assert image_source == image_source_drop_zone
-
-    def test_multiple_swipe_with_multipoint_swipe(self):
-
-        self.drop_image_with_multipoint_swipe(
-            ["Drag Image1", "Drop Box1"],  1, False)
-        self.drop_image_with_multipoint_swipe(
-            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, False)
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image1", "Drop Image")
-        assert image_source == image_source_drop_zone
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image2", "Drop")
-        assert image_source == image_source_drop_zone
-
-    def test_multiple_swipe_and_waits_with_multipoint_swipe(self):
-
-        self.drop_image_with_multipoint_swipe(
-            ["Drag Image1", "Drop Box1"],  1, True)
-        self.drop_image_with_multipoint_swipe(
-            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, True)
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image1", "Drop Image")
-        assert image_source == image_source_drop_zone
-
-        image_source, image_source_drop_zone = self.get_sprite_name(
-            "Drag Image2", "Drop")
-        assert image_source == image_source_drop_zone
-
-    def test_begin_move_end_touch(self):
-        alt_object1 = self.altdriver.find_object(By.NAME, "Drag Image1")
-        alt_object2 = self.altdriver.find_object(By.NAME, "Drop Box1")
-
-        id = self.altdriver.begin_touch(alt_object1.get_screen_position())
-        self.altdriver.move_touch(id, alt_object2.get_screen_position())
-        self.altdriver.end_touch(id)
-
-        imageSource = alt_object1.get_component_property(
-            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
-        imageSourceDropZone = self.altdriver.find_object(By.NAME, "Drop Image").get_component_property(
-            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
-
-        assert imageSource == imageSourceDropZone
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+
+import pytest
+
+from .utils import Scenes
+from alttester import By
+
+
+class TestScene03:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.altdriver.reset_input()
+        self.altdriver.load_scene(Scenes.Scene03)
+
+    def wait_for_swipe_to_finish(self):
+        self.altdriver.wait_for_object_to_not_be_present(By.NAME, "icon")
+
+    def get_sprite_name(self, source_image_name, image_source_drop_zone_name):
+        image_source = self.altdriver.find_object(
+            By.NAME, source_image_name).get_component_property(
+            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
+        image_source_drop_zone = self.altdriver.find_object(
+            By.NAME, image_source_drop_zone_name).get_component_property(
+            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
+        return image_source, image_source_drop_zone
+
+    def drop_image_with_multipoint_swipe(self, object_names, duration, wait):
+        positions = []
+        for name in object_names:
+            alt_object = self.altdriver.find_object(By.NAME, name)
+            positions.append(alt_object.get_screen_position())
+
+        self.altdriver.multipoint_swipe(positions, duration, wait)
+
+    def drop_image(self, drag_location_name, drop_location_name, duration, wait):
+        drag_location = self.altdriver.find_object(By.NAME, drag_location_name)
+        drop_location = self.altdriver.find_object(By.NAME, drop_location_name)
+
+        self.altdriver.swipe(drag_location.get_screen_position(
+        ), drop_location.get_screen_position(), duration, wait)
+
+    def test_pointer_enter_and_exit(self):
+        alt_object = self.altdriver.find_object(By.NAME, "Drop Image")
+        color1 = alt_object.get_component_property(
+            "AltExampleScriptDropMe",
+            "highlightColor",
+            "Assembly-CSharp"
+        )
+        alt_object.pointer_enter()
+        color2 = alt_object.get_component_property(
+            "AltExampleScriptDropMe",
+            "highlightColor",
+            "Assembly-CSharp"
+        )
+
+        assert color1["r"] != color2["r"] or \
+            color1["g"] != color2["g"] or \
+            color1["b"] != color2["b"] or \
+            color1["a"] != color2["a"]
+
+        alt_object.pointer_exit()
+        color3 = alt_object.get_component_property(
+            "AltExampleScriptDropMe",
+            "highlightColor",
+            "Assembly-CSharp"
+        )
+
+        assert color3["r"] != color2["r"] or \
+            color3["g"] != color2["g"] or \
+            color3["b"] != color2["b"] or \
+            color3["a"] != color2["a"]
+
+        assert color3["r"] == color1["r"] and \
+            color3["g"] == color1["g"] and \
+            color3["b"] == color1["b"] and \
+            color3["a"] == color1["a"]
+
+    def test_multiple_swipes(self):
+        self.drop_image("Drag Image2", "Drop Box2", 1, False)
+        self.drop_image("Drag Image2", "Drop Box1", 1, False)
+        self.drop_image("Drag Image1", "Drop Box1", 2, False)
+        self.wait_for_swipe_to_finish()
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
+        assert image_source == image_source_drop_zone
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
+        assert image_source == image_source_drop_zone
+
+    def test_multiple_swipe_and_waits(self):
+        self.drop_image("Drag Image2", "Drop Box2", 1, True)
+        self.drop_image("Drag Image2", "Drop Box1", 1, True)
+        self.drop_image("Drag Image1", "Drop Box1", 1, True)
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
+        assert image_source == image_source_drop_zone
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
+        assert image_source == image_source_drop_zone
+
+    def test_multiple_swipe_with_multipoint_swipe(self):
+
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image1", "Drop Box1"],  1, False)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, False)
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
+        assert image_source == image_source_drop_zone
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
+        assert image_source == image_source_drop_zone
+
+    def test_multiple_swipe_and_waits_with_multipoint_swipe(self):
+
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image1", "Drop Box1"],  1, True)
+        self.drop_image_with_multipoint_swipe(
+            ["Drag Image2", "Drop Box1", "Drop Box2"],  1, True)
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image1", "Drop Image")
+        assert image_source == image_source_drop_zone
+
+        image_source, image_source_drop_zone = self.get_sprite_name(
+            "Drag Image2", "Drop")
+        assert image_source == image_source_drop_zone
+
+    def test_begin_move_end_touch(self):
+        alt_object1 = self.altdriver.find_object(By.NAME, "Drag Image1")
+        alt_object2 = self.altdriver.find_object(By.NAME, "Drop Box1")
+
+        id = self.altdriver.begin_touch(alt_object1.get_screen_position())
+        self.altdriver.move_touch(id, alt_object2.get_screen_position())
+        self.altdriver.end_touch(id)
+
+        imageSource = alt_object1.get_component_property(
+            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
+        imageSourceDropZone = self.altdriver.find_object(By.NAME, "Drop Image").get_component_property(
+            "UnityEngine.UI.Image", "sprite.name", "UnityEngine.UI")
+
+        assert imageSource == imageSourceDropZone
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_scene05.py` & `alttester_driver-2.1.0/tests/integration/test_scene05.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,132 +1,131 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import time
-
-import pytest
-
-from .utils import Scenes
-from alttester import By, AltKeyCode
-
-
-class TestScene05:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-        self.altdriver.load_scene(Scenes.Scene05)
-
-    def test_movement_cube(self):
-        cube = self.altdriver.find_object(By.NAME, "Player1")
-        initial_position = (cube.worldX, cube.worldY, cube.worldZ)
-
-        self.altdriver.scroll(speed_vertical=30, duration=0.1, wait=False)
-        self.altdriver.press_key(AltKeyCode.K, power=1, duration=0.1, wait=False)
-
-        self.altdriver.press_key(AltKeyCode.O, power=1, duration=0.1)
-        cube = self.altdriver.find_object(By.NAME, "Player1")
-        final_position = (cube.worldX, cube.worldY, cube.worldZ)
-
-        assert initial_position != final_position
-
-    def test_camera_movement(self):
-        cube = self.altdriver.find_object(By.NAME, "Player1")
-        initial_position = (cube.worldX, cube.worldY, cube.worldY)
-
-        self.altdriver.press_key(AltKeyCode.W, power=1, duration=0.1, wait=False)
-        # time.sleep(2)
-
-        cube = self.altdriver.find_object(By.NAME, "Player1")
-        final_position = (cube.worldX, cube.worldY, cube.worldY)
-
-        assert initial_position != final_position
-
-    def test_update_altObject(self):
-
-        cube = self.altdriver.find_object(By.NAME, "Player1")
-        initial_position_z = cube.worldZ
-
-        self.altdriver.press_key(AltKeyCode.W, power=1, duration=0.1, wait=False)
-        time.sleep(5)
-
-        assert initial_position_z != cube.update_object().worldZ
-
-    def test_creating_stars(self):
-        stars = self.altdriver.find_objects_which_contain(By.NAME, "Star", By.NAME, "Player2")
-        assert len(stars) == 1
-
-        self.altdriver.find_objects_which_contain(By.NAME, "Player", By.NAME, "Player2")
-        pressing_point_1 = self.altdriver.find_object(By.NAME, "PressingPoint1", By.NAME, "Player2")
-
-        self.altdriver.move_mouse(pressing_point_1.get_screen_position(), duration=0.1, wait=False)
-        time.sleep(0.1)
-
-        self.altdriver.press_key(AltKeyCode.Mouse0, power=1, duration=0.1, wait=False)
-        pressing_point_2 = self.altdriver.find_object(By.NAME, "PressingPoint2", By.NAME, "Player2")
-        self.altdriver.move_mouse(pressing_point_2.get_screen_position(), duration=0.1)
-        self.altdriver.press_key(AltKeyCode.Mouse0, power=1, duration=0.1, wait=False)
-        time.sleep(0.1)
-
-        stars = self.altdriver.find_objects_which_contain(By.NAME, "Star")
-        assert len(stars) == 3
-
-    def test_power_joystick(self):
-        button_names = ["Horizontal", "Vertical"]
-        keys_to_press = [AltKeyCode.D, AltKeyCode.W]
-
-        axis_name = self.altdriver.find_object(By.NAME, "AxisName")
-        axis_value = self.altdriver.find_object(By.NAME, "AxisValue")
-
-        for button_name, key in zip(button_names, keys_to_press):
-            self.altdriver.press_key(key, power=0.5, duration=1)
-
-            assert axis_value.get_text() == "0.5"
-            assert axis_name.get_text() == button_name
-
-    def test_scroll(self):
-        player2 = self.altdriver.find_object(By.NAME, "Player2")
-        cube_initial_position = [player2.worldX, player2.worldY, player2.worldY]
-        self.altdriver.scroll(4, duration=1, wait=False)
-        time.sleep(1)
-
-        player2 = self.altdriver.find_object(By.NAME, "Player2")
-        cube_final_position = [player2.worldX, player2.worldY, player2.worldY]
-        assert cube_initial_position != cube_final_position
-
-    def test_scroll_and_wait(self):
-        player2 = self.altdriver.find_object(By.NAME, "Player2")
-        cube_initial_position = [player2.worldX, player2.worldY, player2.worldY]
-        self.altdriver.scroll(4, duration=0.3)
-
-        player2 = self.altdriver.find_object(By.NAME, "Player2")
-        cube_final_position = [player2.worldX, player2.worldY, player2.worldY]
-        assert cube_initial_position != cube_final_position
-
-    def test_key_down_and_key_up(self):
-        self.altdriver.key_down(AltKeyCode.A)
-
-        last_key_down = self.altdriver.find_object(By.NAME, "LastKeyDownValue")
-        last_key_press = self.altdriver.find_object(By.NAME, "LastKeyPressedValue")
-
-        assert last_key_down.get_text() == "97"
-        assert last_key_press.get_text() == "97"
-
-        self.altdriver.key_up(AltKeyCode.A)
-        last_key_up = self.altdriver.find_object(By.NAME, "LastKeyUpValue")
-
-        assert last_key_up.get_text() == "97"
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import time
+
+import pytest
+
+from .utils import Scenes
+from alttester import By, AltKeyCode
+
+
+class TestScene05:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.altdriver.reset_input()
+        self.altdriver.load_scene(Scenes.Scene05)
+
+    def test_movement_cube(self):
+        cube = self.altdriver.find_object(By.NAME, "Player1")
+        initial_position = (cube.worldX, cube.worldY, cube.worldZ)
+
+        self.altdriver.scroll(speed_vertical=30, duration=0.1, wait=False)
+        self.altdriver.press_key(AltKeyCode.K, power=1, duration=0.1, wait=False)
+
+        self.altdriver.press_key(AltKeyCode.O, power=1, duration=0.1)
+        cube = self.altdriver.find_object(By.NAME, "Player1")
+        final_position = (cube.worldX, cube.worldY, cube.worldZ)
+
+        assert initial_position != final_position
+
+    def test_camera_movement(self):
+        cube = self.altdriver.find_object(By.NAME, "Player1")
+        initial_position = (cube.worldX, cube.worldY, cube.worldY)
+
+        self.altdriver.press_key(AltKeyCode.W, power=1, duration=0.1, wait=False)
+        # time.sleep(2)
+
+        cube = self.altdriver.find_object(By.NAME, "Player1")
+        final_position = (cube.worldX, cube.worldY, cube.worldY)
+
+        assert initial_position != final_position
+
+    def test_update_altObject(self):
+
+        cube = self.altdriver.find_object(By.NAME, "Player1")
+        initial_position_z = cube.worldZ
+
+        self.altdriver.press_key(AltKeyCode.W, power=1, duration=0.1, wait=False)
+        time.sleep(5)
+
+        assert initial_position_z != cube.update_object().worldZ
+
+    def test_creating_stars(self):
+        stars = self.altdriver.find_objects_which_contain(By.NAME, "Star", By.NAME, "Player2")
+        assert len(stars) == 1
+
+        self.altdriver.find_objects_which_contain(By.NAME, "Player", By.NAME, "Player2")
+        pressing_point_1 = self.altdriver.find_object(By.NAME, "PressingPoint1", By.NAME, "Player2")
+
+        self.altdriver.move_mouse(pressing_point_1.get_screen_position(), duration=0.1, wait=False)
+        time.sleep(0.1)
+
+        self.altdriver.press_key(AltKeyCode.Mouse0, power=1, duration=0.1, wait=False)
+        pressing_point_2 = self.altdriver.find_object(By.NAME, "PressingPoint2", By.NAME, "Player2")
+        self.altdriver.move_mouse(pressing_point_2.get_screen_position(), duration=0.1)
+        self.altdriver.press_key(AltKeyCode.Mouse0, power=1, duration=0.1, wait=False)
+        time.sleep(0.1)
+
+        stars = self.altdriver.find_objects_which_contain(By.NAME, "Star")
+        assert len(stars) == 3
+
+    def test_power_joystick(self):
+        button_names = ["Horizontal", "Vertical"]
+        keys_to_press = [AltKeyCode.D, AltKeyCode.W]
+
+        axis_name = self.altdriver.find_object(By.NAME, "AxisName")
+        axis_value = self.altdriver.find_object(By.NAME, "AxisValue")
+
+        for button_name, key in zip(button_names, keys_to_press):
+            self.altdriver.press_key(key, power=0.5, duration=1)
+
+            assert axis_value.get_text() == "0.5"
+            assert axis_name.get_text() == button_name
+
+    def test_scroll(self):
+        player2 = self.altdriver.find_object(By.NAME, "Player2")
+        cube_initial_position = [player2.worldX, player2.worldY, player2.worldY]
+        self.altdriver.scroll(4, duration=1, wait=False)
+        time.sleep(1)
+
+        player2 = self.altdriver.find_object(By.NAME, "Player2")
+        cube_final_position = [player2.worldX, player2.worldY, player2.worldY]
+        assert cube_initial_position != cube_final_position
+
+    def test_scroll_and_wait(self):
+        player2 = self.altdriver.find_object(By.NAME, "Player2")
+        cube_initial_position = [player2.worldX, player2.worldY, player2.worldY]
+        self.altdriver.scroll(4, duration=0.3)
+
+        player2 = self.altdriver.find_object(By.NAME, "Player2")
+        cube_final_position = [player2.worldX, player2.worldY, player2.worldY]
+        assert cube_initial_position != cube_final_position
+
+    def test_key_down_and_key_up(self):
+        self.altdriver.key_down(AltKeyCode.A)
+
+        last_key_down = self.altdriver.find_object(By.NAME, "LastKeyDownValue")
+        last_key_press = self.altdriver.find_object(By.NAME, "LastKeyPressedValue")
+
+        assert last_key_down.get_text() == "97"
+        assert last_key_press.get_text() == "97"
+
+        self.altdriver.key_up(AltKeyCode.A)
+        last_key_up = self.altdriver.find_object(By.NAME, "LastKeyUpValue")
+
+        assert last_key_up.get_text() == "97"
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_scene09.py` & `alttester_driver-2.1.0/tests/integration/test_scene09.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import pytest
-
-from .utils import Scenes
-from alttester import By
-
-
-class TestScene09:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-        self.altdriver.load_scene(Scenes.Scene09)
-
-    def test_scroll_element_NIS(self):
-        scrollbar_initial = self.altdriver.find_object(By.NAME, "Scrollbar Vertical")
-        scrollbar_initial_value = scrollbar_initial.get_component_property(
-            "UnityEngine.UI.Scrollbar", "value", "UnityEngine.UI")
-        self.altdriver.move_mouse(self.altdriver.find_object(
-            By.NAME, "Scroll View").get_screen_position(), duration=0.3, wait=True)
-        self.altdriver.scroll(-3000, duration=0.5, wait=True)
-
-        scrollbar_final = self.altdriver.find_object(By.NAME, "Scrollbar Vertical")
-        scrollbar_final_value = scrollbar_final.get_component_property(
-            "UnityEngine.UI.Scrollbar", "value", "UnityEngine.UI")
-
-        assert scrollbar_initial_value != scrollbar_final_value
-
-    def test_swipe_NIS(self):
-        scrollbar = self.altdriver.find_object(By.NAME, "Handle")
-        scrollbar_position = scrollbar.get_screen_position()
-        button = self.altdriver.find_object(By.PATH, "//Scroll View/Viewport/Content/Button (4)")
-        self.altdriver.swipe(
-            button.get_screen_position(),
-            (button.x, button.y + 20),
-            duration=0.5
-        )
-
-        scrollbar_final = self.altdriver.find_object(By.NAME, "Handle")
-        scrollbar_final_position = scrollbar_final.get_screen_position()
-        assert scrollbar_position != scrollbar_final_position
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import pytest
+
+from .utils import Scenes
+from alttester import By
+
+
+class TestScene09:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.altdriver.reset_input()
+        self.altdriver.load_scene(Scenes.Scene09)
+
+    def test_scroll_element_NIS(self):
+        scrollbar_initial = self.altdriver.find_object(By.NAME, "Scrollbar Vertical")
+        scrollbar_initial_value = scrollbar_initial.get_component_property(
+            "UnityEngine.UI.Scrollbar", "value", "UnityEngine.UI")
+        self.altdriver.move_mouse(self.altdriver.find_object(
+            By.NAME, "Scroll View").get_screen_position(), duration=0.3, wait=True)
+        self.altdriver.scroll(-3000, duration=0.5, wait=True)
+
+        scrollbar_final = self.altdriver.find_object(By.NAME, "Scrollbar Vertical")
+        scrollbar_final_value = scrollbar_final.get_component_property(
+            "UnityEngine.UI.Scrollbar", "value", "UnityEngine.UI")
+
+        assert scrollbar_initial_value != scrollbar_final_value
+
+    def test_swipe_NIS(self):
+        scrollbar = self.altdriver.find_object(By.NAME, "Handle")
+        scrollbar_position = scrollbar.get_screen_position()
+        button = self.altdriver.find_object(By.PATH, "//Scroll View/Viewport/Content/Button (4)")
+        self.altdriver.swipe(
+            button.get_screen_position(),
+            (button.x, button.y + 20),
+            duration=0.5
+        )
+
+        scrollbar_final = self.altdriver.find_object(By.NAME, "Handle")
+        scrollbar_final_position = scrollbar_final.get_screen_position()
+        assert scrollbar_position != scrollbar_final_position
```

### Comparing `AltTester-Driver-2.0.3/tests/integration/test_scene10.py` & `alttester_driver-2.1.0/tests/integration/test_scene10.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,110 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import pytest
-
-from .utils import Scenes
-from alttester import By, AltKeyCode
-
-
-class TestScene10:
-
-    @pytest.fixture(autouse=True)
-    def setup(self, altdriver):
-        self.altdriver = altdriver
-        self.altdriver.reset_input()
-        self.altdriver.load_scene(Scenes.Scene10)
-
-    def test_scroll_NIS(self):
-        player = self.altdriver.find_object(By.NAME, "Player")
-
-        assert not player.get_component_property(
-            "AltNIPDebugScript",
-            "wasScrolled",
-            "Assembly-CSharp"
-        )
-
-        self.altdriver.scroll(300, duration=1, wait=True)
-
-        assert player.get_component_property(
-            "AltNIPDebugScript",
-            "wasScrolled",
-            "Assembly-CSharp"
-        )
-
-    def test_key_down_and_key_up_NIS(self):
-        player = self.altdriver.find_object(By.NAME, "Player")
-        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        self.altdriver.key_down(AltKeyCode.A)
-        self.altdriver.key_up(AltKeyCode.A)
-        lef_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert lef_position != initial_position
-
-        self.altdriver.key_down(AltKeyCode.D)
-        self.altdriver.key_up(AltKeyCode.D)
-        right_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert right_position != lef_position
-
-        self.altdriver.key_down(AltKeyCode.W)
-        self.altdriver.key_up(AltKeyCode.W)
-        up_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert up_position != right_position
-
-        self.altdriver.key_down(AltKeyCode.S)
-        self.altdriver.key_up(AltKeyCode.S)
-        down_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert down_position != up_position
-
-    def test_press_key_NIS(self):
-        player = self.altdriver.find_object(By.NAME, "Player")
-        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        self.altdriver.press_key(AltKeyCode.A)
-        left_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert left_position != initial_position
-
-        self.altdriver.press_key(AltKeyCode.D)
-        right_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert right_position != left_position
-
-        self.altdriver.press_key(AltKeyCode.W)
-        up_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert up_position != right_position
-
-        self.altdriver.press_key(AltKeyCode.S)
-        down_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        assert down_position != up_position
-
-    def test_press_keys_NIS(self):
-        player = self.altdriver.find_object(By.NAME, "Player")
-        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-
-        keys = [AltKeyCode.W, AltKeyCode.Mouse0]
-        self.altdriver.press_keys(keys)
-
-        final_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
-        assert initial_position != final_position
-
-        self.altdriver.wait_for_object(By.NAME, "SimpleProjectile(Clone)")
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import pytest
+
+from .utils import Scenes
+from alttester import By, AltKeyCode
+
+
+class TestScene10:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.altdriver.reset_input()
+        self.altdriver.load_scene(Scenes.Scene10)
+
+    def test_scroll_NIS(self):
+        player = self.altdriver.find_object(By.NAME, "Player")
+
+        assert not player.get_component_property(
+            "AltNIPDebugScript",
+            "wasScrolled",
+            "Assembly-CSharp"
+        )
+
+        self.altdriver.scroll(300, duration=1, wait=True)
+
+        assert player.get_component_property(
+            "AltNIPDebugScript",
+            "wasScrolled",
+            "Assembly-CSharp"
+        )
+
+    def test_key_down_and_key_up_NIS(self):
+        player = self.altdriver.find_object(By.NAME, "Player")
+        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        self.altdriver.key_down(AltKeyCode.A)
+        self.altdriver.key_up(AltKeyCode.A)
+        lef_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert lef_position != initial_position
+
+        self.altdriver.key_down(AltKeyCode.D)
+        self.altdriver.key_up(AltKeyCode.D)
+        right_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert right_position != lef_position
+
+        self.altdriver.key_down(AltKeyCode.W)
+        self.altdriver.key_up(AltKeyCode.W)
+        up_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert up_position != right_position
+
+        self.altdriver.key_down(AltKeyCode.S)
+        self.altdriver.key_up(AltKeyCode.S)
+        down_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert down_position != up_position
+
+    def test_press_key_NIS(self):
+        player = self.altdriver.find_object(By.NAME, "Player")
+        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        self.altdriver.press_key(AltKeyCode.A)
+        left_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert left_position != initial_position
+
+        self.altdriver.press_key(AltKeyCode.D)
+        right_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert right_position != left_position
+
+        self.altdriver.press_key(AltKeyCode.W)
+        up_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert up_position != right_position
+
+        self.altdriver.press_key(AltKeyCode.S)
+        down_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        assert down_position != up_position
+
+    def test_press_keys_NIS(self):
+        player = self.altdriver.find_object(By.NAME, "Player")
+        initial_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+
+        keys = [AltKeyCode.W, AltKeyCode.Mouse0]
+        self.altdriver.press_keys(keys)
+
+        final_position = player.get_component_property("UnityEngine.Transform", "position", "UnityEngine.CoreModule")
+        assert initial_position != final_position
+
+        self.altdriver.wait_for_object(By.NAME, "SimpleProjectile(Clone)")
```

### Comparing `AltTester-Driver-2.0.3/tests/unit/test_websocket.py` & `alttester_driver-2.1.0/tests/unit/test_websocket.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-"""
-    Copyright(C) 2023 Altom Consulting
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import json
-import unittest.mock as mock
-
-import pytest
-
-from alttester._websocket import Store, WebsocketConnection, CommandHandler, NotificationHandler
-from alttester.exceptions import ConnectionError
-
-
-class TestStore:
-
-    @pytest.fixture(autouse=True)
-    def setup(self):
-        self.store = Store()
-
-    def test_has(self):
-        assert not self.store.has("key")
-
-        self.store.push("key", mock.sentinel.value)
-
-        assert self.store.has("key")
-
-    def test_push(self):
-        assert not self.store.has("key")
-
-        self.store.push("key", mock.sentinel.value)
-
-        assert self.store.has("key")
-        assert self.store.pop("key") == mock.sentinel.value
-        assert not self.store.has("key")
-
-    def test_pop(self):
-        assert not self.store.has("key")
-        assert self.store.pop("key") is None
-
-        self.store.push("key", mock.sentinel.first)
-        self.store.push("key", mock.sentinel.second)
-
-        assert self.store.has("key")
-        assert self.store.pop("key") == mock.sentinel.first
-        assert self.store.has("key")
-        assert self.store.pop("key") == mock.sentinel.second
-        assert not self.store.has("key")
-        assert self.store.pop("key") is None
-
-    def test_multiple_keys(self):
-        assert not self.store.has("a")
-        assert self.store.pop("a") is None
-
-        assert not self.store.has("b")
-        assert self.store.pop("b") is None
-
-        self.store.push("a", mock.sentinel.first)
-        self.store.push("b", mock.sentinel.second)
-        self.store.push("a", mock.sentinel.third)
-
-        assert self.store.has("a")
-        assert self.store.pop("a") == mock.sentinel.first
-        assert self.store.has("b")
-        assert self.store.pop("b") == mock.sentinel.second
-        assert self.store.has("a")
-        assert self.store.pop("a") == mock.sentinel.third
-
-        assert not self.store.has("a")
-        assert self.store.pop("a") is None
-        assert not self.store.has("a")
-        assert self.store.pop("a") is None
-
-
-class TestWebsocketConnection:
-
-    @pytest.fixture(autouse=True)
-    def setup(self):
-        self.host = "127.0.0.1"
-        self.port = 1300
-        self.timeout = 5
-
-        self.websocket_mock = mock.Mock()
-        self.create_connection_mock = mock.Mock(
-            return_value=self.websocket_mock
-        )
-
-        self.connection = WebsocketConnection(
-            host=self.host,
-            port=self.port,
-            timeout=self.timeout,
-            command_handler=CommandHandler(),
-            notification_handler=NotificationHandler()
-        )
-        self.connection._create_connection = self.create_connection_mock
-        self.connection._is_open = True
-
-    def test_connect(self):
-        self.connection.connect()
-        self.create_connection_mock.assert_called_once()
-
-        self.websocket_mock.close.assert_not_called()
-
-    def test_on_open(self):
-        self.connection._is_open = False
-        self.connection._on_open(self.websocket_mock)
-
-        assert self.connection._is_open
-
-    def test_on_message(self):
-        command = {
-            "messageId": "0",
-            "commandName": "TestCommand"
-        }
-
-        self.connection._command_handler.set_current_command(command)
-        assert not self.connection._command_handler.has_response()
-
-        self.connection._on_message(self.connection._websocket, json.dumps(command))
-
-        assert self.connection._command_handler.has_response()
-        assert self.connection._command_handler.get_response() == command
-
-    def test_on_error(self):
-        assert not self.connection._errors
-
-        error_message = "Error message."
-        self.connection._on_error(self.connection._websocket, error_message)
-
-        assert self.connection._errors.pop() == error_message
-
-    def test_on_close(self):
-        self.connection._is_open = True
-        self.connection._on_close(self.websocket_mock, None, None)
-
-        assert not self.connection._is_open
-        assert self.connection._websocket is None
-
-    def test_recv(self):
-        command = {
-            "messageId": "0",
-            "commandName": "TestCommand"
-        }
-        self.connection.connect()
-        self.connection._websocket = self.websocket_mock
-        self.connection._command_handler.set_current_command(command)
-        self.connection._command_handler.handle_command(command)
-
-        response = self.connection.recv()
-
-        assert response == command
-
-    def test_recv_with_closed_connection(self):
-        self.connection._is_open = False
-
-        with pytest.raises(ConnectionError):
-            self.connection.recv()
-
-    def test_send(self):
-        self.connection.connect()
-        self.connection._websocket = self.websocket_mock
-
-        command = {
-            "messageId": "0",
-            "commandName": "TestCommand"
-        }
-        self.connection.send(command)
-
-        assert self.connection._command_handler.get_current_command() == (command["messageId"], command["commandName"])
-
-    def test_send_with_close_connection(self):
-        self.connection._is_open = False
-
-        command = {
-            "messageId": "0",
-            "commandName": "TestCommand"
-        }
-
-        with pytest.raises(ConnectionError):
-            self.connection.send(command)
-
-        assert self.connection._command_handler.get_current_command() != (command["messageId"], command["commandName"])
+"""
+    Copyright(C) 2023 Altom Consulting
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import json
+import unittest.mock as mock
+
+import pytest
+
+from alttester._websocket import Store, WebsocketConnection, CommandHandler, NotificationHandler
+from alttester.exceptions import ConnectionError
+
+
+class TestStore:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.store = Store()
+
+    def test_has(self):
+        assert not self.store.has("key")
+
+        self.store.push("key", mock.sentinel.value)
+
+        assert self.store.has("key")
+
+    def test_push(self):
+        assert not self.store.has("key")
+
+        self.store.push("key", mock.sentinel.value)
+
+        assert self.store.has("key")
+        assert self.store.pop("key") == mock.sentinel.value
+        assert not self.store.has("key")
+
+    def test_pop(self):
+        assert not self.store.has("key")
+        assert self.store.pop("key") is None
+
+        self.store.push("key", mock.sentinel.first)
+        self.store.push("key", mock.sentinel.second)
+
+        assert self.store.has("key")
+        assert self.store.pop("key") == mock.sentinel.first
+        assert self.store.has("key")
+        assert self.store.pop("key") == mock.sentinel.second
+        assert not self.store.has("key")
+        assert self.store.pop("key") is None
+
+    def test_multiple_keys(self):
+        assert not self.store.has("a")
+        assert self.store.pop("a") is None
+
+        assert not self.store.has("b")
+        assert self.store.pop("b") is None
+
+        self.store.push("a", mock.sentinel.first)
+        self.store.push("b", mock.sentinel.second)
+        self.store.push("a", mock.sentinel.third)
+
+        assert self.store.has("a")
+        assert self.store.pop("a") == mock.sentinel.first
+        assert self.store.has("b")
+        assert self.store.pop("b") == mock.sentinel.second
+        assert self.store.has("a")
+        assert self.store.pop("a") == mock.sentinel.third
+
+        assert not self.store.has("a")
+        assert self.store.pop("a") is None
+        assert not self.store.has("a")
+        assert self.store.pop("a") is None
+
+
+class TestWebsocketConnection:
+
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.host = "127.0.0.1"
+        self.port = 1300
+        self.timeout = 5
+
+        self.websocket_mock = mock.Mock()
+        self.create_connection_mock = mock.Mock(
+            return_value=self.websocket_mock
+        )
+
+        self.connection = WebsocketConnection(
+            host=self.host,
+            port=self.port,
+            timeout=self.timeout,
+            command_handler=CommandHandler(),
+            notification_handler=NotificationHandler()
+        )
+        self.connection._create_connection = self.create_connection_mock
+        self.connection._is_open = True
+
+    def test_connect(self):
+        self.connection.connect()
+        self.create_connection_mock.assert_called_once()
+
+        self.websocket_mock.close.assert_not_called()
+
+    def test_on_open(self):
+        self.connection._is_open = False
+        self.connection._on_open(self.websocket_mock)
+
+        assert self.connection._is_open
+
+    def test_on_message(self):
+        command = {
+            "messageId": "0",
+            "commandName": "TestCommand"
+        }
+
+        self.connection._command_handler.set_current_command(command)
+        assert not self.connection._command_handler.has_response()
+
+        self.connection._on_message(self.connection._websocket, json.dumps(command))
+
+        assert self.connection._command_handler.has_response()
+        assert self.connection._command_handler.get_response() == command
+
+    def test_on_error(self):
+        assert not self.connection._errors
+
+        error_message = "Error message."
+        self.connection._on_error(self.connection._websocket, error_message)
+
+        assert self.connection._errors.pop() == error_message
+
+    def test_on_close(self):
+        self.connection._is_open = True
+        self.connection._on_close(self.websocket_mock, None, None)
+
+        assert not self.connection._is_open
+        assert self.connection._websocket is None
+
+    def test_recv(self):
+        command = {
+            "messageId": "0",
+            "commandName": "TestCommand"
+        }
+        self.connection.connect()
+        self.connection._websocket = self.websocket_mock
+        self.connection._command_handler.set_current_command(command)
+        self.connection._command_handler.handle_command(command)
+
+        response = self.connection.recv()
+
+        assert response == command
+
+    def test_recv_with_closed_connection(self):
+        self.connection._is_open = False
+
+        with pytest.raises(ConnectionError):
+            self.connection.recv()
+
+    def test_send(self):
+        self.connection.connect()
+        self.connection._websocket = self.websocket_mock
+
+        command = {
+            "messageId": "0",
+            "commandName": "TestCommand"
+        }
+        self.connection.send(command)
+
+        assert self.connection._command_handler.get_current_command() == (command["messageId"], command["commandName"])
+
+    def test_send_with_close_connection(self):
+        self.connection._is_open = False
+
+        command = {
+            "messageId": "0",
+            "commandName": "TestCommand"
+        }
+
+        with pytest.raises(ConnectionError):
+            self.connection.send(command)
+
+        assert self.connection._command_handler.get_current_command() != (command["messageId"], command["commandName"])
```

