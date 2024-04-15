# Comparing `tmp/meshtastic-2.3.4.post1.tar.gz` & `tmp/meshtastic-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.3.4.post1.tar", last modified: Mon Apr  8 17:50:04 2024, max compression
+gzip compressed data, was "meshtastic-2.3.5.tar", last modified: Mon Apr 15 06:47:19 2024, max compression
```

## Comparing `meshtastic-2.3.4.post1.tar` & `meshtastic-2.3.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.478169 meshtastic-2.3.4.post1/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53538 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/apponly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/atak_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/atak_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/localonly_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    41793 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/module_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/portnums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20907 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:50:04.478169 meshtastic-2.3.4.post1/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 17:50:04.000000 meshtastic-2.3.4.post1/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:50:04.482169 meshtastic-2.3.4.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 17:50:00.000000 meshtastic-2.3.4.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 06:47:12.000000 meshtastic-2.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 06:47:12.000000 meshtastic-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-15 06:47:19.329728 meshtastic-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-15 06:47:12.000000 meshtastic-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53865 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25228 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/apponly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/atak_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/atak_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/cannedmessages_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/clientonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65909 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/connection_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/deviceonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/localonly_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    42944 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86471 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48852 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/module_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/mqtt_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/nanopb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/nanopb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    31340 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/paxcount_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/paxcount_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/portnums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/remote_hardware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/rtttl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/storeforward_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6140 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/telemetry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/xmodem_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-15 06:47:12.000000 meshtastic-2.3.5/meshtastic/xmodem_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:47:19.329728 meshtastic-2.3.5/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 06:47:19.000000 meshtastic-2.3.5/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:47:19.329728 meshtastic-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-15 06:47:12.000000 meshtastic-2.3.5/setup.py
```

### Comparing `meshtastic-2.3.4.post1/LICENSE.txt` & `meshtastic-2.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/PKG-INFO` & `meshtastic-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.4.post1
+Version: 2.3.5
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.4.post1/README.md` & `meshtastic-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/__init__.py` & `meshtastic-2.3.5/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/__main__.py` & `meshtastic-2.3.5/meshtastic/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,19 @@
             interface.getNode(args.dest, False).commitSettingsTransaction()
 
         if args.factory_reset:
             closeNow = True
             waitForAckNak = True
             interface.getNode(args.dest, False).factoryReset()
 
+        if args.remove_node:
+            closeNow = True
+            waitForAckNak = True
+            interface.getNode(args.dest, False).removeNode(args.remove_node)
+
         if args.reset_nodedb:
             closeNow = True
             waitForAckNak = True
             interface.getNode(args.dest, False).resetNodeDb()
 
         if args.sendtext:
             closeNow = True
@@ -1329,16 +1334,20 @@
     group.add_argument(
         "--factory-reset",
         help="Tell the destination node to install the default config",
         action="store_true",
     )
 
     group.add_argument(
+        "--remove-node",
+        help="Tell the destination node to remove a specific node from its DB, by node number or ID"
+    )
+    group.add_argument(
         "--reset-nodedb",
-        help="Tell the destination node clear its list of nodes",
+        help="Tell the destination node to clear its list of nodes",
         action="store_true",
     )
 
     group.add_argument(
         "--reply", help="Reply to received messages", action="store_true"
     )
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/admin_pb2.py` & `meshtastic-2.3.5/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/admin_pb2.pyi` & `meshtastic-2.3.5/meshtastic/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/apponly_pb2.py` & `meshtastic-2.3.5/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/apponly_pb2.pyi` & `meshtastic-2.3.5/meshtastic/apponly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/atak_pb2.py` & `meshtastic-2.3.5/meshtastic/atak_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/atak_pb2.pyi` & `meshtastic-2.3.5/meshtastic/atak_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/ble_interface.py` & `meshtastic-2.3.5/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.3.5/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/cannedmessages_pb2.pyi` & `meshtastic-2.3.5/meshtastic/cannedmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/channel_pb2.py` & `meshtastic-2.3.5/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/channel_pb2.pyi` & `meshtastic-2.3.5/meshtastic/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.py` & `meshtastic-2.3.5/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/clientonly_pb2.pyi` & `meshtastic-2.3.5/meshtastic/clientonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/config_pb2.py` & `meshtastic-2.3.5/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/config_pb2.pyi` & `meshtastic-2.3.5/meshtastic/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.py` & `meshtastic-2.3.5/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/connection_status_pb2.pyi` & `meshtastic-2.3.5/meshtastic/connection_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.py` & `meshtastic-2.3.5/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/deviceonly_pb2.pyi` & `meshtastic-2.3.5/meshtastic/deviceonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/globals.py` & `meshtastic-2.3.5/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/localonly_pb2.py` & `meshtastic-2.3.5/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/localonly_pb2.pyi` & `meshtastic-2.3.5/meshtastic/localonly_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/mesh_interface.py` & `meshtastic-2.3.5/meshtastic/mesh_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import logging
 import random
 import sys
 import threading
 import time
 from datetime import datetime
 
+from typing import Any, Callable, Dict, List, Optional, Union
+
 import google.protobuf.json_format
 import timeago # type: ignore[import-untyped]
 from pubsub import pub # type: ignore[import-untyped]
 from tabulate import tabulate
 
 import meshtastic.node
 from meshtastic import (
@@ -50,43 +52,43 @@
 
     class MeshInterfaceError(Exception):
         """An exception class for general mesh interface errors"""
         def __init__(self, message):
             self.message = message
             super().__init__(self.message)
 
-    def __init__(self, debugOut=None, noProto=False):
+    def __init__(self, debugOut=None, noProto: bool=False) -> None:
         """Constructor
 
         Keyword Arguments:
             noProto -- If True, don't try to run our protocol on the
                        link - just be a dumb serial client.
         """
         self.debugOut = debugOut
-        self.nodes = None  # FIXME
-        self.isConnected = threading.Event()
-        self.noProto = noProto
-        self.localNode = meshtastic.node.Node(self, -1)  # We fixup nodenum later
-        self.myInfo = None  # We don't have device info yet
-        self.metadata = None  # We don't have device metadata yet
-        self.responseHandlers = {}  # A map from request ID to the handler
+        self.nodes: Optional[Dict[str,Dict]] = None  # FIXME
+        self.isConnected: threading.Event = threading.Event()
+        self.noProto: bool = noProto
+        self.localNode: meshtastic.node.Node = meshtastic.node.Node(self, -1)  # We fixup nodenum later
+        self.myInfo: Optional[mesh_pb2.MyNodeInfo] = None  # We don't have device info yet
+        self.metadata: Optional[mesh_pb2.DeviceMetadata] = None  # We don't have device metadata yet
+        self.responseHandlers: Dict[int,ResponseHandler] = {}  # A map from request ID to the handler
         self.failure = (
             None  # If we've encountered a fatal exception it will be kept here
         )
-        self._timeout = Timeout()
-        self._acknowledgment = Acknowledgment()
-        self.heartbeatTimer = None
+        self._timeout: Timeout = Timeout()
+        self._acknowledgment: Acknowledgment = Acknowledgment()
+        self.heartbeatTimer: Optional[threading.Timer] = None
         random.seed()  # FIXME, we should not clobber the random seedval here, instead tell user they must call it
-        self.currentPacketId = random.randint(0, 0xFFFFFFFF)
-        self.nodesByNum = None
-        self.configId = None
-        self.gotResponse = False  # used in gpio read
-        self.mask = None  # used in gpio read and gpio watch
-        self.queueStatus = None
-        self.queue = collections.OrderedDict()
+        self.currentPacketId: int = random.randint(0, 0xFFFFFFFF)
+        self.nodesByNum: Optional[Dict[int, Dict]] = None
+        self.configId: Optional[int] = None
+        self.gotResponse: bool = False  # used in gpio read
+        self.mask: Optional[int] = None  # used in gpio read and gpio watch
+        self.queueStatus: Optional[mesh_pb2.QueueStatus] = None
+        self.queue: collections.OrderedDict = collections.OrderedDict()
 
     def close(self):
         """Shutdown this interface"""
         if self.heartbeatTimer:
             self.heartbeatTimer.cancel()
 
         self._sendDisconnect()
@@ -99,15 +101,15 @@
             logging.error(
                 f"An exception of type {exc_type} with value {exc_value} has occurred"
             )
         if traceback is not None:
             logging.error(f"Traceback: {traceback}")
         self.close()
 
-    def showInfo(self, file=sys.stdout):  # pylint: disable=W0613
+    def showInfo(self, file=sys.stdout) -> str:  # pylint: disable=W0613
         """Show human readable summary about this object"""
         owner = f"Owner: {self.getLongName()} ({self.getShortName()})"
         myinfo = ""
         if self.myInfo:
             myinfo = f"\nMy info: {message_to_json(self.myInfo)}"
         metadata = ""
         if self.metadata:
@@ -131,36 +133,36 @@
                 # use id as dictionary key for correct json format in list of nodes
                 nodeid = n2["user"]["id"]
                 nodes[nodeid] = n2
         infos = owner + myinfo + metadata + mesh + json.dumps(nodes)
         print(infos)
         return infos
 
-    def showNodes(self, includeSelf=True, file=sys.stdout):  # pylint: disable=W0613
+    def showNodes(self, includeSelf: bool=True, file=sys.stdout) -> str:  # pylint: disable=W0613
         """Show table summary of nodes in mesh"""
 
-        def formatFloat(value, precision=2, unit=""):
+        def formatFloat(value, precision=2, unit="") -> Optional[str]:
             """Format a float value with precision."""
             return f"{value:.{precision}f}{unit}" if value else None
 
-        def getLH(ts):
+        def getLH(ts) -> Optional[str]:
             """Format last heard"""
             return (
                 datetime.fromtimestamp(ts).strftime("%Y-%m-%d %H:%M:%S") if ts else None
             )
 
-        def getTimeAgo(ts):
+        def getTimeAgo(ts) -> Optional[str]:
             """Format how long ago have we heard from this node (aka timeago)."""
             return (
                 timeago.format(datetime.fromtimestamp(ts), datetime.now())
                 if ts
                 else None
             )
 
-        rows = []
+        rows: List[Dict[str, Any]] = []
         if self.nodesByNum:
             logging.debug(f"self.nodes:{self.nodes}")
             for node in self.nodesByNum.values():
                 if not includeSelf and node["num"] == self.localNode.nodeNum:
                     continue
 
                 row = {"N": 0, "User": f"UNK: {node['num']}", "ID": f"!{node['num']:08x}"}
@@ -204,14 +206,15 @@
                             ),
                         }
                     )
 
                 row.update(
                     {
                         "SNR": formatFloat(node.get("snr"), 2, " dB"),
+                        "Hops Away": node.get("hopsAway", "unknown"),
                         "Channel": node.get("channel"),
                         "LastHeard": getLH(node.get("lastHeard")),
                         "Since": getTimeAgo(node.get("lastHeard")),
                     }
                 )
 
                 rows.append(row)
@@ -220,15 +223,15 @@
         for i, row in enumerate(rows):
             row["N"] = i + 1
 
         table = tabulate(rows, headers="keys", missingval="N/A", tablefmt="fancy_grid")
         print(table)
         return table
 
-    def getNode(self, nodeId, requestChannels=True):
+    def getNode(self, nodeId: str, requestChannels: bool=True) -> meshtastic.node.Node:
         """Return a node object which contains device settings and channel info"""
         if nodeId in (LOCAL_ADDR, BROADCAST_ADDR):
             return self.localNode
         else:
             n = meshtastic.node.Node(self, nodeId)
             # Only request device settings and channel info when necessary
             if requestChannels:
@@ -237,19 +240,19 @@
                 if not n.waitForConfig():
                     our_exit("Error: Timed out waiting for channels")
             return n
 
     def sendText(
         self,
         text: str,
-        destinationId=BROADCAST_ADDR,
-        wantAck=False,
-        wantResponse=False,
-        onResponse=None,
-        channelIndex=0,
+        destinationId: Union[int, str]=BROADCAST_ADDR,
+        wantAck: bool=False,
+        wantResponse: bool=False,
+        onResponse: Optional[Callable[[mesh_pb2.MeshPacket], Any]]=None,
+        channelIndex: int=0,
     ):
         """Send a utf8 string to some other node, if the node has a display it
            will also be shown on the device.
 
         Arguments:
             text {string} -- The text to send
 
@@ -276,20 +279,20 @@
             onResponse=onResponse,
             channelIndex=channelIndex,
         )
 
     def sendData(
         self,
         data,
-        destinationId=BROADCAST_ADDR,
-        portNum=portnums_pb2.PortNum.PRIVATE_APP,
-        wantAck=False,
-        wantResponse=False,
-        onResponse=None,
-        channelIndex=0,
+        destinationId: Union[int, str]=BROADCAST_ADDR,
+        portNum: portnums_pb2.PortNum.ValueType=portnums_pb2.PortNum.PRIVATE_APP,
+        wantAck: bool=False,
+        wantResponse: bool=False,
+        onResponse: Optional[Callable[[mesh_pb2.MeshPacket], Any]]=None,
+        channelIndex: int=0,
     ):
         """Send a data packet to some other node
 
         Keyword Arguments:
             data -- the data to send, either as an array of bytes or
                     as a protobuf (which will be automatically
                     serialized to bytes)
@@ -336,21 +339,21 @@
         if onResponse is not None:
             self._addResponseHandler(meshPacket.id, onResponse)
         p = self._sendPacket(meshPacket, destinationId, wantAck=wantAck)
         return p
 
     def sendPosition(
         self,
-        latitude=0.0,
-        longitude=0.0,
-        altitude=0,
-        timeSec=0,
-        destinationId=BROADCAST_ADDR,
-        wantAck=False,
-        wantResponse=False,
+        latitude: float=0.0,
+        longitude: float=0.0,
+        altitude: int=0,
+        timeSec: int=0,
+        destinationId: Union[int, str]=BROADCAST_ADDR,
+        wantAck: bool=False,
+        wantResponse: bool=False,
     ):
         """
         Send a position packet to some other node (normally a broadcast)
 
         Also, the device software will notice this packet and use it to automatically
         set its notion of the local position.
 
@@ -369,38 +372,38 @@
             logging.debug(f"p.longitude_i:{p.longitude_i}")
 
         if altitude != 0:
             p.altitude = int(altitude)
             logging.debug(f"p.altitude:{p.altitude}")
 
         if timeSec == 0:
-            timeSec = time.time()  # returns unix timestamp in seconds
-        p.time = int(timeSec)
+            timeSec = int(time.time())  # returns unix timestamp in seconds
+        p.time = timeSec
         logging.debug(f"p.time:{p.time}")
 
         return self.sendData(
             p,
             destinationId,
             portNum=portnums_pb2.PortNum.POSITION_APP,
             wantAck=wantAck,
             wantResponse=wantResponse,
         )
 
-    def sendTraceRoute(self, dest, hopLimit):
+    def sendTraceRoute(self, dest: Union[int, str], hopLimit: int):
         """Send the trace route"""
         r = mesh_pb2.RouteDiscovery()
         self.sendData(
             r,
             destinationId=dest,
             portNum=portnums_pb2.PortNum.TRACEROUTE_APP,
             wantResponse=True,
             onResponse=self.onResponseTraceRoute,
         )
         # extend timeout based on number of nodes, limit by configured hopLimit
-        waitFactor = min(len(self.nodes) - 1, hopLimit)
+        waitFactor = min(len(self.nodes) - 1 if self.nodes else 0, hopLimit)
         self.waitForTraceRoute(waitFactor)
 
     def onResponseTraceRoute(self, p):
         """on response for trace route"""
         routeDiscovery = mesh_pb2.RouteDiscovery()
         routeDiscovery.ParseFromString(p["decoded"]["payload"])
         asDict = google.protobuf.json_format.MessageToDict(routeDiscovery)
@@ -475,32 +478,32 @@
             if telemetry.device_metrics.air_util_tx is not None:
                 print(f"Transmit air utilization: {telemetry.device_metrics.air_util_tx:.2f}%")
 
         elif p["decoded"]["portnum"] == 'ROUTING_APP':
             if p["decoded"]["routing"]["errorReason"] == 'NO_RESPONSE':
                 our_exit("No response from node. At least firmware 2.1.22 is required on the destination node.")
 
-    def _addResponseHandler(self, requestId, callback):
+    def _addResponseHandler(self, requestId: int, callback: Callable):
         self.responseHandlers[requestId] = ResponseHandler(callback)
 
-    def _sendPacket(self, meshPacket, destinationId=BROADCAST_ADDR, wantAck=False):
+    def _sendPacket(self, meshPacket: mesh_pb2.MeshPacket, destinationId: Union[int,str]=BROADCAST_ADDR, wantAck: bool=False):
         """Send a MeshPacket to the specified node (or if unspecified, broadcast).
         You probably don't want this - use sendData instead.
 
         Returns the sent packet. The id field will be populated in this packet and
         can be used to track future message acks/naks.
         """
 
         # We allow users to talk to the local node before we've completed the full connection flow...
         if self.myInfo is not None and destinationId != self.myInfo.my_node_num:
             self._waitConnected()
 
         toRadio = mesh_pb2.ToRadio()
 
-        nodeNum = 0
+        nodeNum: int = 0
         if destinationId is None:
             our_exit("Warning: destinationId must not be None")
         elif isinstance(destinationId, int):
             nodeNum = destinationId
         elif destinationId == BROADCAST_ADDR:
             nodeNum = BROADCAST_NUM
         elif destinationId == LOCAL_ADDR:
@@ -510,17 +513,18 @@
                 our_exit("Warning: No myInfo found.")
         # A simple hex style nodeid - we can parse this without needing the DB
         elif destinationId.startswith("!"):
             nodeNum = int(destinationId[1:], 16)
         else:
             if self.nodes:
                 node = self.nodes.get(destinationId)
-                if not node:
+                if node is None:
                     our_exit(f"Warning: NodeId {destinationId} not found in DB")
-                nodeNum = node["num"]
+                else:
+                    nodeNum = node["num"]
             else:
                 logging.warning("Warning: There were no self.nodes.")
 
         meshPacket.to = nodeNum
         meshPacket.want_ack = wantAck
         loraConfig = getattr(self.localNode.localConfig, "lora")
         hopLimit = getattr(loraConfig, "hop_limit")
@@ -564,17 +568,17 @@
 
     def waitForTelemetry(self):
         """Wait for telemetry"""
         success = self._timeout.waitForTelemetry(self._acknowledgment)
         if not success:
             raise MeshInterface.MeshInterfaceError("Timed out waiting for telemetry")
 
-    def getMyNodeInfo(self):
+    def getMyNodeInfo(self) -> Optional[Dict]:
         """Get info about my node."""
-        if self.myInfo is None:
+        if self.myInfo is None or self.nodesByNum is None:
             return None
         logging.debug(f"self.nodesByNum:{self.nodesByNum}")
         return self.nodesByNum.get(self.myInfo.my_node_num)
 
     def getMyUser(self):
         """Get user"""
         nodeInfo = self.getMyNodeInfo()
@@ -603,15 +607,15 @@
             if not self.isConnected.wait(timeout):  # timeout after x seconds
                 raise MeshInterface.MeshInterfaceError("Timed out waiting for connection completion")
 
         # If we failed while connecting, raise the connection to the client
         if self.failure:
             raise self.failure
 
-    def _generatePacketId(self):
+    def _generatePacketId(self) -> int:
         """Get a new unique packet ID"""
         if self.currentPacketId is None:
             raise MeshInterface.MeshInterfaceError("Not connected yet, can not generate packet")
         else:
             self.currentPacketId = (self.currentPacketId + 1) & 0xFFFFFFFF
             return self.currentPacketId
 
@@ -665,26 +669,26 @@
 
     def _sendDisconnect(self):
         """Tell device we are done using it"""
         m = mesh_pb2.ToRadio()
         m.disconnect = True
         self._sendToRadio(m)
 
-    def _queueHasFreeSpace(self):
+    def _queueHasFreeSpace(self) -> bool:
         # We never got queueStatus, maybe the firmware is old
         if self.queueStatus is None:
             return True
         return self.queueStatus.free > 0
 
-    def _queueClaim(self):
+    def _queueClaim(self) -> None:
         if self.queueStatus is None:
             return
         self.queueStatus.free -= 1
 
-    def _sendToRadio(self, toRadio):
+    def _sendToRadio(self, toRadio: mesh_pb2.ToRadio) -> None:
         """Send a ToRadio protobuf to the device"""
         if self.noProto:
             logging.warning(
                 f"Not sending packet because protocol use is disabled by noProto"
             )
         else:
             # logging.debug(f"Sending toRadio: {stripnl(toRadio)}")
@@ -725,26 +729,26 @@
                 ):  # Packet got acked under us
                     logging.debug(f"packet {packetId:08x} got acked under us")
                     continue
                 if packet:
                     self.queue[packetId] = packet
             # logging.warn("queue + resentQueue: " + " ".join(f'{k:08x}' for k in self.queue))
 
-    def _sendToRadioImpl(self, toRadio):
+    def _sendToRadioImpl(self, toRadio: mesh_pb2.ToRadio) -> None:
         """Send a ToRadio protobuf to the device"""
         logging.error(f"Subclass must provide toradio: {toRadio}")
 
-    def _handleConfigComplete(self):
+    def _handleConfigComplete(self) -> None:
         """
         Done with initial config messages, now send regular MeshPackets
         to ask for settings and channels
         """
         self.localNode.requestChannels()
 
-    def _handleQueueStatusFromRadio(self, queueStatus):
+    def _handleQueueStatusFromRadio(self, queueStatus) -> None:
         self.queueStatus = queueStatus
         logging.debug(
             f"TX QUEUE free {queueStatus.free} of {queueStatus.maxlen}, res = {queueStatus.res}, id = {queueStatus.mesh_packet_id:08x} "
         )
 
         if queueStatus.res:
             return
@@ -887,15 +891,15 @@
                 self.localNode.moduleConfig.paxcounter.CopyFrom(
                     fromRadio.moduleConfig.paxcounter
                 )
 
         else:
             logging.debug("Unexpected FromRadio payload")
 
-    def _fixupPosition(self, position):
+    def _fixupPosition(self, position: Dict) -> Dict:
         """Convert integer lat/lon into floats
 
         Arguments:
             position {Position dictionary} -- object to fix up
         Returns the position with the updated keys
         """
         if "latitudeI" in position:
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/mesh_pb2.py` & `meshtastic-2.3.5/meshtastic/mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/mesh_pb2.pyi` & `meshtastic-2.3.5/meshtastic/mesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/module_config_pb2.py` & `meshtastic-2.3.5/meshtastic/module_config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/module_config_pb2.pyi` & `meshtastic-2.3.5/meshtastic/module_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.py` & `meshtastic-2.3.5/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/mqtt_pb2.pyi` & `meshtastic-2.3.5/meshtastic/mqtt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.py` & `meshtastic-2.3.5/meshtastic/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/nanopb_pb2.pyi` & `meshtastic-2.3.5/meshtastic/nanopb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/node.py` & `meshtastic-2.3.5/meshtastic/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Node class
 """
 
 import base64
 import logging
 import time
 
+from typing import Union
+
 from meshtastic import admin_pb2, apponly_pb2, channel_pb2, localonly_pb2, portnums_pb2
 from meshtastic.util import (
     Timeout,
     camel_to_snake,
     fromPSK,
     our_exit,
     pskToString,
@@ -599,14 +601,31 @@
         # If sending to a remote node, wait for ACK/NAK
         if self == self.iface.localNode:
             onResponse = None
         else:
             onResponse = self.onAckNak
         return self._sendAdmin(p, onResponse=onResponse)
 
+    def removeNode(self, nodeId: Union[int, str]):
+        """Tell the node to remove a specific node by ID"""
+        if isinstance(nodeId, str):
+            if nodeId.startswith("!"):
+                nodeId = int(nodeId[1:], 16)
+            else:
+                nodeId = int(nodeId)
+
+        p = admin_pb2.AdminMessage()
+        p.remove_by_nodenum = nodeId
+
+        if self == self.iface.localNode:
+            onResponse = None
+        else:
+            onResponse = self.onAckNak
+        return self._sendAdmin(p, onResponse=onResponse)
+
     def resetNodeDb(self):
         """Tell the node to reset its list of nodes."""
         p = admin_pb2.AdminMessage()
         p.nodedb_reset = True
         logging.info(f"Telling node to reset the NodeDB")
 
         # If sending to a remote node, wait for ACK/NAK
@@ -736,17 +755,17 @@
             p, wantResponse=True, onResponse=self.onResponseRequestChannel
         )
 
     # pylint: disable=R1710
     def _sendAdmin(
         self,
         p: admin_pb2.AdminMessage,
-        wantResponse=True,
+        wantResponse: bool=True,
         onResponse=None,
-        adminIndex=0,
+        adminIndex: int=0,
     ):
         """Send an admin message to the specified node (or the local node if destNodeNum is zero)"""
 
         if self.noProto:
             logging.warning(
                 f"Not sending packet because protocol use is disabled by noProto"
             )
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.py` & `meshtastic-2.3.5/meshtastic/paxcount_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/paxcount_pb2.pyi` & `meshtastic-2.3.5/meshtastic/paxcount_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/portnums_pb2.py` & `meshtastic-2.3.5/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/portnums_pb2.pyi` & `meshtastic-2.3.5/meshtastic/portnums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/remote_hardware.py` & `meshtastic-2.3.5/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.3.5/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/remote_hardware_pb2.pyi` & `meshtastic-2.3.5/meshtastic/remote_hardware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.py` & `meshtastic-2.3.5/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/rtttl_pb2.pyi` & `meshtastic-2.3.5/meshtastic/rtttl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/serial_interface.py` & `meshtastic-2.3.5/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.py` & `meshtastic-2.3.5/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/storeforward_pb2.pyi` & `meshtastic-2.3.5/meshtastic/storeforward_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/stream_interface.py` & `meshtastic-2.3.5/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/supported_device.py` & `meshtastic-2.3.5/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/tcp_interface.py` & `meshtastic-2.3.5/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.py` & `meshtastic-2.3.5/meshtastic/telemetry_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\x12\nmeshtastic\"i\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\"\x9b\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\x89\x02\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12\x33\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x19.meshtastic.DeviceMetricsH\x00\x12=\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x1e.meshtastic.EnvironmentMetricsH\x00\x12<\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x1d.meshtastic.AirQualityMetricsH\x00\x12\x31\n\rpower_metrics\x18\x05 \x01(\x0b\x32\x18.meshtastic.PowerMetricsH\x00\x42\t\n\x07variant*\xe0\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ameshtastic/telemetry.proto\x12\nmeshtastic\"\x81\x01\n\rDeviceMetrics\x12\x15\n\rbattery_level\x18\x01 \x01(\r\x12\x0f\n\x07voltage\x18\x02 \x01(\x02\x12\x1b\n\x13\x63hannel_utilization\x18\x03 \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x04 \x01(\x02\x12\x16\n\x0euptime_seconds\x18\x05 \x01(\r\"\xa8\x01\n\x12\x45nvironmentMetrics\x12\x13\n\x0btemperature\x18\x01 \x01(\x02\x12\x19\n\x11relative_humidity\x18\x02 \x01(\x02\x12\x1b\n\x13\x62\x61rometric_pressure\x18\x03 \x01(\x02\x12\x16\n\x0egas_resistance\x18\x04 \x01(\x02\x12\x0f\n\x07voltage\x18\x05 \x01(\x02\x12\x0f\n\x07\x63urrent\x18\x06 \x01(\x02\x12\x0b\n\x03iaq\x18\x07 \x01(\r\"\x8c\x01\n\x0cPowerMetrics\x12\x13\n\x0b\x63h1_voltage\x18\x01 \x01(\x02\x12\x13\n\x0b\x63h1_current\x18\x02 \x01(\x02\x12\x13\n\x0b\x63h2_voltage\x18\x03 \x01(\x02\x12\x13\n\x0b\x63h2_current\x18\x04 \x01(\x02\x12\x13\n\x0b\x63h3_voltage\x18\x05 \x01(\x02\x12\x13\n\x0b\x63h3_current\x18\x06 \x01(\x02\"\xbf\x02\n\x11\x41irQualityMetrics\x12\x15\n\rpm10_standard\x18\x01 \x01(\r\x12\x15\n\rpm25_standard\x18\x02 \x01(\r\x12\x16\n\x0epm100_standard\x18\x03 \x01(\r\x12\x1a\n\x12pm10_environmental\x18\x04 \x01(\r\x12\x1a\n\x12pm25_environmental\x18\x05 \x01(\r\x12\x1b\n\x13pm100_environmental\x18\x06 \x01(\r\x12\x16\n\x0eparticles_03um\x18\x07 \x01(\r\x12\x16\n\x0eparticles_05um\x18\x08 \x01(\r\x12\x16\n\x0eparticles_10um\x18\t \x01(\r\x12\x16\n\x0eparticles_25um\x18\n \x01(\r\x12\x16\n\x0eparticles_50um\x18\x0b \x01(\r\x12\x17\n\x0fparticles_100um\x18\x0c \x01(\r\"\x89\x02\n\tTelemetry\x12\x0c\n\x04time\x18\x01 \x01(\x07\x12\x33\n\x0e\x64\x65vice_metrics\x18\x02 \x01(\x0b\x32\x19.meshtastic.DeviceMetricsH\x00\x12=\n\x13\x65nvironment_metrics\x18\x03 \x01(\x0b\x32\x1e.meshtastic.EnvironmentMetricsH\x00\x12<\n\x13\x61ir_quality_metrics\x18\x04 \x01(\x0b\x32\x1d.meshtastic.AirQualityMetricsH\x00\x12\x31\n\rpower_metrics\x18\x05 \x01(\x0b\x32\x18.meshtastic.PowerMetricsH\x00\x42\t\n\x07variant*\xe0\x01\n\x13TelemetrySensorType\x12\x10\n\x0cSENSOR_UNSET\x10\x00\x12\n\n\x06\x42ME280\x10\x01\x12\n\n\x06\x42ME680\x10\x02\x12\x0b\n\x07MCP9808\x10\x03\x12\n\n\x06INA260\x10\x04\x12\n\n\x06INA219\x10\x05\x12\n\n\x06\x42MP280\x10\x06\x12\t\n\x05SHTC3\x10\x07\x12\t\n\x05LPS22\x10\x08\x12\x0b\n\x07QMC6310\x10\t\x12\x0b\n\x07QMI8658\x10\n\x12\x0c\n\x08QMC5883L\x10\x0b\x12\t\n\x05SHT31\x10\x0c\x12\x0c\n\x08PMSA003I\x10\r\x12\x0b\n\x07INA3221\x10\x0e\x12\n\n\x06\x42MP085\x10\x0f\x42\x64\n\x13\x63om.geeksville.meshB\x0fTelemetryProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'meshtastic.telemetry_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\017TelemetryProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _TELEMETRYSENSORTYPE._serialized_start=1041
-  _TELEMETRYSENSORTYPE._serialized_end=1265
-  _DEVICEMETRICS._serialized_start=42
-  _DEVICEMETRICS._serialized_end=147
-  _ENVIRONMENTMETRICS._serialized_start=150
-  _ENVIRONMENTMETRICS._serialized_end=305
-  _POWERMETRICS._serialized_start=308
-  _POWERMETRICS._serialized_end=448
-  _AIRQUALITYMETRICS._serialized_start=451
-  _AIRQUALITYMETRICS._serialized_end=770
-  _TELEMETRY._serialized_start=773
-  _TELEMETRY._serialized_end=1038
+  _TELEMETRYSENSORTYPE._serialized_start=1079
+  _TELEMETRYSENSORTYPE._serialized_end=1303
+  _DEVICEMETRICS._serialized_start=43
+  _DEVICEMETRICS._serialized_end=172
+  _ENVIRONMENTMETRICS._serialized_start=175
+  _ENVIRONMENTMETRICS._serialized_end=343
+  _POWERMETRICS._serialized_start=346
+  _POWERMETRICS._serialized_end=486
+  _AIRQUALITYMETRICS._serialized_start=489
+  _AIRQUALITYMETRICS._serialized_end=808
+  _TELEMETRY._serialized_start=811
+  _TELEMETRY._serialized_end=1076
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/telemetry_pb2.pyi` & `meshtastic-2.3.5/meshtastic/telemetry_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BATTERY_LEVEL_FIELD_NUMBER: builtins.int
     VOLTAGE_FIELD_NUMBER: builtins.int
     CHANNEL_UTILIZATION_FIELD_NUMBER: builtins.int
     AIR_UTIL_TX_FIELD_NUMBER: builtins.int
+    UPTIME_SECONDS_FIELD_NUMBER: builtins.int
     battery_level: builtins.int
     """
     0-100 (>100 means powered)
     """
     voltage: builtins.float
     """
     Voltage measured
@@ -182,23 +183,28 @@
     """
     Utilization for the current channel, including well formed TX, RX and malformed RX (aka noise).
     """
     air_util_tx: builtins.float
     """
     Percent of airtime for transmission used within the last hour.
     """
+    uptime_seconds: builtins.int
+    """
+    How long the device has been running since the last reboot (in seconds)
+    """
     def __init__(
         self,
         *,
         battery_level: builtins.int = ...,
         voltage: builtins.float = ...,
         channel_utilization: builtins.float = ...,
         air_util_tx: builtins.float = ...,
+        uptime_seconds: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["air_util_tx", b"air_util_tx", "battery_level", b"battery_level", "channel_utilization", b"channel_utilization", "voltage", b"voltage"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["air_util_tx", b"air_util_tx", "battery_level", b"battery_level", "channel_utilization", b"channel_utilization", "uptime_seconds", b"uptime_seconds", "voltage", b"voltage"]) -> None: ...
 
 global___DeviceMetrics = DeviceMetrics
 
 @typing_extensions.final
 class EnvironmentMetrics(google.protobuf.message.Message):
     """
     Weather station or other environmental metrics
@@ -208,14 +214,15 @@
 
     TEMPERATURE_FIELD_NUMBER: builtins.int
     RELATIVE_HUMIDITY_FIELD_NUMBER: builtins.int
     BAROMETRIC_PRESSURE_FIELD_NUMBER: builtins.int
     GAS_RESISTANCE_FIELD_NUMBER: builtins.int
     VOLTAGE_FIELD_NUMBER: builtins.int
     CURRENT_FIELD_NUMBER: builtins.int
+    IAQ_FIELD_NUMBER: builtins.int
     temperature: builtins.float
     """
     Temperature measured
     """
     relative_humidity: builtins.float
     """
     Relative humidity percent measured
@@ -232,25 +239,31 @@
     """
     Voltage measured (To be depreciated in favor of PowerMetrics in Meshtastic 3.x)
     """
     current: builtins.float
     """
     Current measured (To be depreciated in favor of PowerMetrics in Meshtastic 3.x)
     """
+    iaq: builtins.int
+    """
+    relative scale IAQ value as measured by Bosch BME680 . value 0-500.
+    Belongs to Air Quality but is not particle but VOC measurement. Other VOC values can also be put in here.
+    """
     def __init__(
         self,
         *,
         temperature: builtins.float = ...,
         relative_humidity: builtins.float = ...,
         barometric_pressure: builtins.float = ...,
         gas_resistance: builtins.float = ...,
         voltage: builtins.float = ...,
         current: builtins.float = ...,
+        iaq: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["barometric_pressure", b"barometric_pressure", "current", b"current", "gas_resistance", b"gas_resistance", "relative_humidity", b"relative_humidity", "temperature", b"temperature", "voltage", b"voltage"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["barometric_pressure", b"barometric_pressure", "current", b"current", "gas_resistance", b"gas_resistance", "iaq", b"iaq", "relative_humidity", b"relative_humidity", "temperature", b"temperature", "voltage", b"voltage"]) -> None: ...
 
 global___EnvironmentMetrics = EnvironmentMetrics
 
 @typing_extensions.final
 class PowerMetrics(google.protobuf.message.Message):
     """
     Power Metrics (voltage / current / etc)
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/test.py` & `meshtastic-2.3.5/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/tunnel.py` & `meshtastic-2.3.5/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/util.py` & `meshtastic-2.3.5/meshtastic/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import re
 import subprocess
 import sys
 import threading
 import time
 import traceback
 from queue import Queue
+from typing import Union
+
 from google.protobuf.json_format import MessageToJson
 
 import packaging.version as pkg_version
 import requests
 import serial # type: ignore[import-untyped]
 import serial.tools.list_ports # type: ignore[import-untyped]
 
@@ -149,56 +151,56 @@
     __setattr__ = dict.__setitem__ # type: ignore[assignment]
     __delattr__ = dict.__delitem__ # type: ignore[assignment]
 
 
 class Timeout:
     """Timeout class"""
 
-    def __init__(self, maxSecs=20):
-        self.expireTime = 0
-        self.sleepInterval = 0.1
-        self.expireTimeout = maxSecs
+    def __init__(self, maxSecs: int=20):
+        self.expireTime: Union[int, float] = 0
+        self.sleepInterval: float = 0.1
+        self.expireTimeout: int = maxSecs
 
     def reset(self):
         """Restart the waitForSet timer"""
         self.expireTime = time.time() + self.expireTimeout
 
-    def waitForSet(self, target, attrs=()):
+    def waitForSet(self, target, attrs=()) -> bool:
         """Block until the specified attributes are set. Returns True if config has been received."""
         self.reset()
         while time.time() < self.expireTime:
             if all(map(lambda a: getattr(target, a, None), attrs)):
                 return True
             time.sleep(self.sleepInterval)
         return False
 
     def waitForAckNak(
         self, acknowledgment, attrs=("receivedAck", "receivedNak", "receivedImplAck")
-    ):
+    ) -> bool:
         """Block until an ACK or NAK has been received. Returns True if ACK or NAK has been received."""
         self.reset()
         while time.time() < self.expireTime:
             if any(map(lambda a: getattr(acknowledgment, a, None), attrs)):
                 acknowledgment.reset()
                 return True
             time.sleep(self.sleepInterval)
         return False
 
-    def waitForTraceRoute(self, waitFactor, acknowledgment, attr="receivedTraceRoute"):
+    def waitForTraceRoute(self, waitFactor, acknowledgment, attr="receivedTraceRoute") -> bool:
         """Block until traceroute response is received. Returns True if traceroute response has been received."""
         self.expireTimeout *= waitFactor
         self.reset()
         while time.time() < self.expireTime:
             if getattr(acknowledgment, attr, None):
                 acknowledgment.reset()
                 return True
             time.sleep(self.sleepInterval)
         return False
 
-    def waitForTelemetry(self, acknowledgment):
+    def waitForTelemetry(self, acknowledgment) -> bool:
         """Block until telemetry response is received. Returns True if telemetry response has been received."""
         self.reset()
         while time.time() < self.expireTime:
             if getattr(acknowledgment, "receivedTelemetry", None):
                 acknowledgment.reset()
                 return True
             time.sleep(self.sleepInterval)
```

### Comparing `meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.py` & `meshtastic-2.3.5/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic/xmodem_pb2.pyi` & `meshtastic-2.3.5/meshtastic/xmodem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.3.5/meshtastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.3.4.post1
+Version: 2.3.5
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.3.4.post1/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.3.5/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.3.4.post1/setup.py` & `meshtastic-2.3.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.3.4.post1",
+    version="2.3.5",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

