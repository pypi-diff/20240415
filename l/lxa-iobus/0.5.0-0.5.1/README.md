# Comparing `tmp/lxa-iobus-0.5.0.tar.gz` & `tmp/lxa_iobus-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxa-iobus-0.5.0.tar", last modified: Fri Apr  5 13:46:09 2024, max compression
+gzip compressed data, was "lxa_iobus-0.5.1.tar", last modified: Mon Apr 15 07:14:32 2024, max compression
```

## Comparing `lxa-iobus-0.5.0.tar` & `lxa_iobus-0.5.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)    10764 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/LICENSE.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      130 2021-07-15 15:09:52.000000 lxa-iobus-0.5.0/MANIFEST.in
--rw-r--r--   0 chris     (1000) chris     (1000)    20717 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     8088 2024-04-05 07:58:15.000000 lxa-iobus-0.5.0/README.rst
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.477770 lxa-iobus-0.5.0/lxa_iobus/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    12010 2024-03-20 10:20:32.000000 lxa-iobus-0.5.0/lxa_iobus/canopen.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.477770 lxa-iobus-0.5.0/lxa_iobus/cli/
--rw-r--r--   0 chris     (1000) chris     (1000)      230 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/cli/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)      928 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/cli/lpc11xxcanisp_invoke.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2436 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/cli/lpc11xxcanisp_program.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14440 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/cli/optick.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4463 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/cli/server.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.477770 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    14770 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/can_isp.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/
--rw-r--r--   0 chris     (1000) chris     (1000)       52 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)    25396 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/ethmux-S01.bin
--rwxr-xr-x   0 chris     (1000) chris     (1000)    25792 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/lxatac_can_io-t01.bin
--rwxr-xr-x   0 chris     (1000) chris     (1000)    24532 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/optick-t01.bin
--rwxrwxr-x   0 chris     (1000) chris     (1000)    24468 2020-10-06 13:05:09.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/ptxtac-S03_CAN_GPIO.bin
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/loader/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/loader/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)      264 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/loader/reset.bin
--rwxrwxr-x   0 chris     (1000) chris     (1000)      260 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/loader/soft_reset.bin
--rw-r--r--   0 chris     (1000) chris     (1000)    20337 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/network.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/node/
--rw-r--r--   0 chris     (1000) chris     (1000)        0 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3217 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/base_node.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9405 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/bus_node.py
--rw-r--r--   0 chris     (1000) chris     (1000)    32915 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/object_directory.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3453 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/products.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3812 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/node/remote_node.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/server/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    24924 2024-04-05 06:53:21.000000 lxa-iobus-0.5.0/lxa_iobus/server/server.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/server/static/
--rw-r--r--   0 chris     (1000) chris     (1000)     8188 2024-03-20 10:20:32.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/index.html
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/
--rw-rw-r--   0 chris     (1000) chris     (1000)   287630 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.js
--rw-rw-r--   0 chris     (1000) chris     (1000)    89476 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   137986 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.min.map
--rw-rw-r--   0 chris     (1000) chris     (1000)    16797 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/pure-min.css
--rw-rw-r--   0 chris     (1000) chris     (1000)   510646 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   226441 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.min.js
--rw-rw-r--   0 chris     (1000) chris     (1000)   864248 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.min.js.map
--rw-rw-r--   0 chris     (1000) chris     (1000)     4296 2020-10-06 12:57:40.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/lib/rpc.js
--rw-r--r--   0 chris     (1000) chris     (1000)     3800 2024-03-20 10:20:32.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/main.js
--rw-r--r--   0 chris     (1000) chris     (1000)     1813 2024-03-20 10:20:32.000000 lxa-iobus-0.5.0/lxa_iobus/server/static/style.css
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/lxa_iobus.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)    20717 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1595 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      246 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       55 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       10 2024-04-05 13:46:09.000000 lxa-iobus-0.5.0/lxa_iobus.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      997 2024-04-05 13:37:51.000000 lxa-iobus-0.5.0/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-05 13:46:09.481770 lxa-iobus-0.5.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.667817 lxa_iobus-0.5.1/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10764 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/LICENSE.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      130 2021-07-15 15:09:52.000000 lxa_iobus-0.5.1/MANIFEST.in
+-rw-r--r--   0 chris     (1000) chris     (1000)    20717 2024-04-15 07:14:32.663817 lxa_iobus-0.5.1/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     8088 2024-04-05 07:58:15.000000 lxa_iobus-0.5.1/README.rst
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.655817 lxa_iobus-0.5.1/lxa_iobus/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    12010 2024-03-20 10:20:32.000000 lxa_iobus-0.5.1/lxa_iobus/canopen.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/cli/
+-rw-r--r--   0 chris     (1000) chris     (1000)      230 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/cli/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      928 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/cli/lpc11xxcanisp_invoke.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2436 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/cli/lpc11xxcanisp_program.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14440 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/cli/optick.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4463 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/cli/server.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    14770 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/can_isp.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/
+-rw-r--r--   0 chris     (1000) chris     (1000)       52 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)    25396 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/ethmux-S01.bin
+-rwxr-xr-x   0 chris     (1000) chris     (1000)    25792 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/lxatac_can_io-t01.bin
+-rwxr-xr-x   0 chris     (1000) chris     (1000)    24532 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/optick-t01.bin
+-rwxrwxr-x   0 chris     (1000) chris     (1000)    24468 2020-10-06 13:05:09.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/ptxtac-S03_CAN_GPIO.bin
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/loader/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/loader/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      264 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/loader/reset.bin
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      260 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/loader/soft_reset.bin
+-rw-r--r--   0 chris     (1000) chris     (1000)    20337 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/network.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/node/
+-rw-r--r--   0 chris     (1000) chris     (1000)        0 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3217 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/base_node.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9405 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/bus_node.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    32915 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/object_directory.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3453 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/products.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3812 2024-04-05 06:53:21.000000 lxa_iobus-0.5.1/lxa_iobus/node/remote_node.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/server/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    24929 2024-04-15 06:17:57.000000 lxa_iobus-0.5.1/lxa_iobus/server/server.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.659817 lxa_iobus-0.5.1/lxa_iobus/server/static/
+-rw-r--r--   0 chris     (1000) chris     (1000)     8188 2024-03-20 10:20:32.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/index.html
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.663817 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/
+-rw-rw-r--   0 chris     (1000) chris     (1000)   287630 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)    89476 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   137986 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.min.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)    16797 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/pure-min.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)   510646 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   226441 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.min.js
+-rw-rw-r--   0 chris     (1000) chris     (1000)   864248 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.min.js.map
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4296 2020-10-06 12:57:40.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/lib/rpc.js
+-rw-r--r--   0 chris     (1000) chris     (1000)     3800 2024-03-20 10:20:32.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/main.js
+-rw-r--r--   0 chris     (1000) chris     (1000)     1813 2024-03-20 10:20:32.000000 lxa_iobus-0.5.1/lxa_iobus/server/static/style.css
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-15 07:14:32.663817 lxa_iobus-0.5.1/lxa_iobus.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)    20717 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1595 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      246 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       55 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       10 2024-04-15 07:14:32.000000 lxa_iobus-0.5.1/lxa_iobus.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      997 2024-04-15 06:18:48.000000 lxa_iobus-0.5.1/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-15 07:14:32.667817 lxa_iobus-0.5.1/setup.cfg
```

### Comparing `lxa-iobus-0.5.0/LICENSE.txt` & `lxa_iobus-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/PKG-INFO` & `lxa_iobus-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxa-iobus
-Version: 0.5.0
+Version: 0.5.1
 Summary: Linux Automation IOBus Server
 Author-email: Linux Automation GmbH <info@linux-automation.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `lxa-iobus-0.5.0/README.rst` & `lxa_iobus-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/canopen.py` & `lxa_iobus-0.5.1/lxa_iobus/canopen.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/cli/lpc11xxcanisp_invoke.py` & `lxa_iobus-0.5.1/lxa_iobus/cli/lpc11xxcanisp_invoke.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/cli/lpc11xxcanisp_program.py` & `lxa_iobus-0.5.1/lxa_iobus/cli/lpc11xxcanisp_program.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/cli/optick.py` & `lxa_iobus-0.5.1/lxa_iobus/cli/optick.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/cli/server.py` & `lxa_iobus-0.5.1/lxa_iobus/cli/server.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/can_isp.py` & `lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/can_isp.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/ethmux-S01.bin` & `lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/ethmux-S01.bin`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/lxatac_can_io-t01.bin` & `lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/lxatac_can_io-t01.bin`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/optick-t01.bin` & `lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/optick-t01.bin`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/lpc11xxcanisp/firmware/ptxtac-S03_CAN_GPIO.bin` & `lxa_iobus-0.5.1/lxa_iobus/lpc11xxcanisp/firmware/ptxtac-S03_CAN_GPIO.bin`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/network.py` & `lxa_iobus-0.5.1/lxa_iobus/network.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/node/base_node.py` & `lxa_iobus-0.5.1/lxa_iobus/node/base_node.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/node/bus_node.py` & `lxa_iobus-0.5.1/lxa_iobus/node/bus_node.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/node/object_directory.py` & `lxa_iobus-0.5.1/lxa_iobus/node/object_directory.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/node/products.py` & `lxa_iobus-0.5.1/lxa_iobus/node/products.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/node/remote_node.py` & `lxa_iobus-0.5.1/lxa_iobus/node/remote_node.py`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/server.py` & `lxa_iobus-0.5.1/lxa_iobus/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
             value = post["value"]
 
             node = self.network.get_node_by_name(node_name)
 
             if value == "toggle":
                 await node.od.outputs.toggle(pin_name)
 
-            elif value:
+            elif int(value):
                 await node.od.outputs.set_high(pin_name)
 
             else:
                 await node.od.outputs.set_low(pin_name)
 
             logger.info(
                 "set_pin: set pin %s on node %s to %s",
```

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/index.html` & `lxa_iobus-0.5.1/lxa_iobus/server/static/index.html`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.min.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/jquery-3.5.1.min.map` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/jquery-3.5.1.min.map`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/pure-min.css` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/pure-min.css`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.min.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.min.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/ractive.min.js.map` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/ractive.min.js.map`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/lib/rpc.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/lib/rpc.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/main.js` & `lxa_iobus-0.5.1/lxa_iobus/server/static/main.js`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus/server/static/style.css` & `lxa_iobus-0.5.1/lxa_iobus/server/static/style.css`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/lxa_iobus.egg-info/PKG-INFO` & `lxa_iobus-0.5.1/lxa_iobus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxa-iobus
-Version: 0.5.0
+Version: 0.5.1
 Summary: Linux Automation IOBus Server
 Author-email: Linux Automation GmbH <info@linux-automation.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `lxa-iobus-0.5.0/lxa_iobus.egg-info/SOURCES.txt` & `lxa_iobus-0.5.1/lxa_iobus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lxa-iobus-0.5.0/pyproject.toml` & `lxa_iobus-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lxa-iobus"
 description = "Linux Automation IOBus Server"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name = "Linux Automation GmbH", email = "info@linux-automation.com" },
 ]
 readme = "README.rst"
 license = { file = "LICENSE.txt" }
 dependencies = [
   "aiohttp~=3.8",
```

