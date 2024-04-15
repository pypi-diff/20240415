# Comparing `tmp/daliuge-engine-4.0.0.tar.gz` & `tmp/daliuge-engine-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-engine-4.0.0.tar", last modified: Mon Mar 25 14:47:44 2024, max compression
+gzip compressed data, was "daliuge-engine-4.0.1.tar", last modified: Mon Apr 15 07:01:42 2024, max compression
```

## Comparing `daliuge-engine-4.0.0.tar` & `daliuge-engine-4.0.1.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      642 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      136 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2957 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/build_engine.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.956527 daliuge-engine-4.0.0/daliuge_engine.egg-info/
--rw-r--r--   0 awicenec  (1000) awicenec  (1000)      642 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6485 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       56 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      312 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/daliuge_engine.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.956527 daliuge-engine-4.0.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.960527 daliuge-engine-4.0.0/dlg/apps/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1318 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/apps/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20109 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/app_base.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7478 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/archiving.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18223 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/bash_shell_app.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2457 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/branch.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3697 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/constructs.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5091 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/crc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/apps/dlg_app.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/apps/dlg_app2.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34187 2024-03-25 11:49:50.000000 daliuge-engine-4.0.0/dlg/apps/dockerapp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18539 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/dynlib.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8377 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/mpi.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5178 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/apps/plasmaflight.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30051 2024-03-25 11:51:05.000000 daliuge-engine-4.0.0/dlg/apps/pyfunc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7428 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/scp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    42005 2024-03-25 11:51:05.000000 daliuge-engine-4.0.0/dlg/apps/simple.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2259 2024-03-22 06:59:31.000000 daliuge-engine-4.0.0/dlg/apps/simple_functions.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/apps/socket_listener.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13666 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/dlg/dask_emulation.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.960527 daliuge-engine-4.0.0/dlg/data/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1155 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/data/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.960527 daliuge-engine-4.0.0/dlg/data/drops/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2002 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/data/drops/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2615 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/data/drops/container.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15206 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/dlg/data/drops/data_base.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4244 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/directorycontainer.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4261 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/environmentvar_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9676 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/file.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1604 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/data/drops/json_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9551 2024-03-25 11:51:05.000000 daliuge-engine-4.0.0/dlg/data/drops/memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6210 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/ngas.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5760 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/data/drops/parset_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5549 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/plasma.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6188 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/rdbms.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13805 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/data/drops/s3_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27652 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/data/io.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4162 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/ddap_protocol.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.964527 daliuge-engine-4.0.0/dlg/deploy/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/deploy/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6349 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/deploy/common.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.964527 daliuge-engine-4.0.0/dlg/deploy/configs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4724 2024-01-29 04:41:54.000000 daliuge-engine-4.0.0/dlg/deploy/configs/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22231 2024-01-29 04:41:54.000000 daliuge-engine-4.0.0/dlg/deploy/create_dlg_job.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1162 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/deploy/deployment_constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8130 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/deploy/deployment_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19786 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/deploy/dlg_monitor.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10559 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/deploy/dlg_proxy.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14426 2023-05-18 15:50:38.000000 daliuge-engine-4.0.0/dlg/deploy/helm_client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6345 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/deploy/remotes.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7004 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/deploy/slurm_client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23807 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/deploy/start_dlg_cluster.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4743 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/deploy/start_helm_cluster.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.964527 daliuge-engine-4.0.0/dlg/deploy/utils/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20541 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/dlg/deploy/utils/monitor_replayer.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    47954 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3128 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/drop_loaders.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14834 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/droputils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4699 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/dlg/event.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15287 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/graph_loader.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      479 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/group.template
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.964527 daliuge-engine-4.0.0/dlg/lifecycle/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/lifecycle/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22536 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/lifecycle/dlm.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.964527 daliuge-engine-4.0.0/dlg/lifecycle/hsm/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/lifecycle/hsm/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1745 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/lifecycle/hsm/manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9905 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/lifecycle/hsm/store.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8491 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/lifecycle/registry.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.968527 daliuge-engine-4.0.0/dlg/manager/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1112 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1294 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/client.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16847 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/dlg/manager/cmdline.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22244 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/dlg/manager/composite_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4760 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/drop_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    24082 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/manager/node_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15303 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/manager/proc_daemon.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5087 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/replay.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26271 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/dlg/manager/rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25242 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/dlg/manager/session.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3063 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/shared_memory_manager.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.968527 daliuge-engine-4.0.0/dlg/manager/web/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2024-03-25 02:13:15.000000 daliuge-engine-4.0.0/dlg/manager/web/LICENSE
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5590 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/manager/web/dim.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4107 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/manager/web/dm.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16527 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/manager/web/session.html
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.940527 daliuge-engine-4.0.0/dlg/manager/web/static/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.968527 daliuge-engine-4.0.0/dlg/manager/web/static/css/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155845 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/css/bootstrap.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2145 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/css/dm.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      929 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/manager/web/static/css/progressBar.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8527 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/manager/web/static/css/session.css
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.972527 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20127 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   116671 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45404 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23424 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18028 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.972527 daliuge-engine-4.0.0/dlg/manager/web/static/icons/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3660 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/icons/engine.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/icons/liu.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/icons/liuFavIcon.svg
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.972527 daliuge-engine-4.0.0/dlg/manager/web/static/js/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15778 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/bootbox.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78743 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/bootstrap.bundle.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.980527 daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/d3.v5.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/dagre-d3.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/dagre-d3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26332 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/dm.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89501 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/manager/web/static/js/jquery-3.6.0.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2392 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/meta.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9811 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/named_port_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5526 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/ngaslite.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2920 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/nm_dim_assigner.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      979 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/passwd.template
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2326 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/prepareUser.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1938 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/process.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4565 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/remote.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1758 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/dlg/restserver.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11106 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/dlg/rpc.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/dlg/runtime/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3346 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/dlg/runtime/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2062 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/dlg/runtime/tool_commands.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      190 2024-03-25 14:47:43.000000 daliuge-engine-4.0.0/dlg/runtime/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6577 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/shared_memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2824 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/dlg/testutils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/docker/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      711 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3223 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile.casa
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      770 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile.dev
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1871 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile.devall
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      832 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile.ray
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      611 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/docker/Dockerfile_incontext
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.940527 daliuge-engine-4.0.0/etc/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/etc/init-scripts/
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1948 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/etc/init-scripts/dlg-dim
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1952 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/etc/init-scripts/dlg-nm
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      994 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/etc/init-scripts/dlg.options
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/fabfile/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/fabfile/APPspecific.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/headers/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/headers/dlg_app.h
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/headers/dlg_app2.h
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.984527 daliuge-engine-4.0.0/pip/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      405 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/pip/requirements.txt
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     4161 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/run_engine.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6148 2024-03-25 14:36:41.000000 daliuge-engine-4.0.0/setup.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/show_DIMlogs.sh
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      183 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/show_NMlogs.sh
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      379 2023-06-29 09:21:30.000000 daliuge-engine-4.0.0/stop_engine.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.988527 daliuge-engine-4.0.0/test/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2024-03-18 12:49:15.000000 daliuge-engine-4.0.0/test/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.988527 daliuge-engine-4.0.0/test/apps/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/apps/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.988527 daliuge-engine-4.0.0/test/apps/data/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   186588 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/apps/data/test_ms.tar.gz
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5909 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/apps/dynlib_example.c
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9088 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/apps/dynlib_example2.c
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1883 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/apps/setp_up.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9651 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/test/apps/test_bash.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3233 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/test/apps/test_crc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8359 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/apps/test_docker.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10276 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/test/apps/test_dynlib.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11864 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/test/apps/test_dynlib2.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17340 2024-03-25 11:51:05.000000 daliuge-engine-4.0.0/test/apps/test_pyfunc.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13107 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/apps/test_simple.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3429 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/test/apps/test_socket.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.988527 daliuge-engine-4.0.0/test/deploy/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/deploy/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4870 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/deploy/test_common.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5175 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/deploy/test_helm_deploy.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/deploy/test_slurm_utils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.992527 daliuge-engine-4.0.0/test/graphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12649 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/graphs/ArrayLoopPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1383 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/HelloWorld_simplePG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   100639 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/graphs/HelloWorld_universePG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/graphs/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35457 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/graphs/appTestPG_namedPorts.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2185 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/application_args.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18978 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/test/graphs/compilePG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2948 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/complex.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4985 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/graphs/ddTest.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8328 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/funcTestPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9203 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/funcTestPG_namedPorts.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11025 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/graphs/pyfunc_glob_testPG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8748 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/graphs/test_graphExecution.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.992527 daliuge-engine-4.0.0/test/integrate/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.992527 daliuge-engine-4.0.0/test/integrate/chiles/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/chiles/__init__.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6166 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/integrate/chiles/chilesdo.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     4411 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/test/integrate/chiles/chilesdoapp.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6091 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/integrate/chiles/chilesdospec.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6327 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/integrate/chiles/chilesdospec_docker.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2732 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/example_split.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      434 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/example_split.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10795 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/freq_split.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.992527 daliuge-engine-4.0.0/test/integrate/msconverter/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      543 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/msconverter/makefile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13468 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/msconverter/ms_checker.cc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      439 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/integrate/msconverter/ms_converter.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/test/lifecycle/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/lifecycle/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6514 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/lifecycle/test_dlm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3552 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/test/lifecycle/test_registry.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/test/manager/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/manager/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13556 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/manager/test_daemon.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16470 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/manager/test_dim.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23335 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/test/manager/test_dm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14649 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/manager/test_mm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9781 2024-02-15 06:56:33.000000 daliuge-engine-4.0.0/test/manager/test_rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5229 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/manager/test_scalability.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3951 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/manager/test_smm.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2400 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/manager/testutils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3820 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/memoryUsage.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/test/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/reproducibility/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5363 2024-03-25 12:52:04.000000 daliuge-engine-4.0.0/test/reproducibility/testSingle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4858 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/reproducibility/test_drophash.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9811 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/test/reproducibility/test_lg_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39765 2023-05-18 15:50:38.000000 daliuge-engine-4.0.0/test/reproducibility/test_pg_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9278 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/test/reproducibility/test_toposort.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-03-25 14:47:43.996527 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15776 2024-03-25 12:38:01.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/computationSandwich.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22856 2024-03-25 12:39:08.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataFan.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23460 2024-03-25 12:39:58.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataFunnel.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17082 2024-03-25 12:40:29.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataSandwich.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20507 2024-03-25 12:51:00.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testCycle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      655 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testEmpty.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20216 2024-03-25 12:50:09.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testNotDAG.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5363 2024-03-25 12:47:40.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testSingle.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15856 2024-03-25 12:51:33.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoEnd.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19926 2024-03-25 12:48:58.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoLines.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15857 2024-03-25 12:48:24.000000 daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoStart.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4096 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/test/test_JsonDrop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2882 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/test_ParameterSetDROP.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3677 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/test/test_S3Drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8959 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/test_dask_emulation.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48587 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/test_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10519 2024-03-18 15:04:41.000000 daliuge-engine-4.0.0/test/test_droputils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10122 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/test_environmentvars.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1268 2023-05-09 13:46:34.000000 daliuge-engine-4.0.0/test/test_event.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8980 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/test_graph_loader.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1164 2024-03-18 14:56:39.000000 daliuge-engine-4.0.0/test/test_input_fired_app_drop.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1589 2023-05-09 13:02:30.000000 daliuge-engine-4.0.0/test/test_io.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10509 2023-06-29 08:45:39.000000 daliuge-engine-4.0.0/test/test_session.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4642 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/test_shared_memory.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1672 2022-11-30 13:05:02.000000 daliuge-engine-4.0.0/test/test_tool.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7933 2023-05-18 15:50:38.000000 daliuge-engine-4.0.0/test/test_utils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.320600 daliuge-engine-4.0.1/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      642 2024-04-15 07:01:42.320600 daliuge-engine-4.0.1/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      136 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/README.md
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2990 2024-04-12 15:05:26.000000 daliuge-engine-4.0.1/build_engine.sh
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.284600 daliuge-engine-4.0.1/daliuge_engine.egg-info/
+-rw-r--r--   0 awicenec  (1000) awicenec  (1000)      642 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6485 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       56 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      312 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2024-04-15 07:01:42.000000 daliuge-engine-4.0.1/daliuge_engine.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.288600 daliuge-engine-4.0.1/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.292600 daliuge-engine-4.0.1/dlg/apps/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1318 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/apps/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20109 2024-04-10 04:55:36.000000 daliuge-engine-4.0.1/dlg/apps/app_base.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7478 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/archiving.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18495 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/dlg/apps/bash_shell_app.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2457 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/branch.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3697 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/constructs.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5091 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/crc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/apps/dlg_app.h
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/apps/dlg_app2.h
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34187 2024-03-25 11:49:50.000000 daliuge-engine-4.0.1/dlg/apps/dockerapp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18539 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/dynlib.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8377 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/mpi.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5178 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/apps/plasmaflight.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    29773 2024-04-12 16:16:10.000000 daliuge-engine-4.0.1/dlg/apps/pyfunc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7428 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/scp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    42014 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/dlg/apps/simple.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2259 2024-03-22 06:59:31.000000 daliuge-engine-4.0.1/dlg/apps/simple_functions.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/apps/socket_listener.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13666 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/dlg/dask_emulation.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.292600 daliuge-engine-4.0.1/dlg/data/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1155 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/data/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.292600 daliuge-engine-4.0.1/dlg/data/drops/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2002 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/data/drops/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2615 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/data/drops/container.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15147 2024-04-12 15:12:00.000000 daliuge-engine-4.0.1/dlg/data/drops/data_base.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4244 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/directorycontainer.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4261 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/environmentvar_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9676 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/file.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1604 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/data/drops/json_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9551 2024-03-25 11:51:05.000000 daliuge-engine-4.0.1/dlg/data/drops/memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6210 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/ngas.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5760 2024-04-04 16:47:06.000000 daliuge-engine-4.0.1/dlg/data/drops/parset_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5549 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/plasma.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6188 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/dlg/data/drops/rdbms.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13799 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/dlg/data/drops/s3_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27652 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/data/io.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4162 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/ddap_protocol.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/deploy/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/deploy/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6349 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/deploy/common.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/deploy/configs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4724 2024-01-29 04:41:54.000000 daliuge-engine-4.0.1/dlg/deploy/configs/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22231 2024-01-29 04:41:54.000000 daliuge-engine-4.0.1/dlg/deploy/create_dlg_job.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1162 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/deploy/deployment_constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8130 2024-04-09 05:09:22.000000 daliuge-engine-4.0.1/dlg/deploy/deployment_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19786 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/deploy/dlg_monitor.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10559 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/deploy/dlg_proxy.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14426 2023-05-18 15:50:38.000000 daliuge-engine-4.0.1/dlg/deploy/helm_client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6345 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/deploy/remotes.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7004 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/deploy/slurm_client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23807 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/deploy/start_dlg_cluster.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4743 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/deploy/start_helm_cluster.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/deploy/utils/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20541 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/dlg/deploy/utils/monitor_replayer.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    47954 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3128 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/drop_loaders.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14786 2024-04-12 15:12:00.000000 daliuge-engine-4.0.1/dlg/droputils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4699 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/dlg/event.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15287 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/graph_loader.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      507 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/dlg/group.template
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/lifecycle/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/lifecycle/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22536 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/lifecycle/dlm.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/lifecycle/hsm/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/lifecycle/hsm/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1745 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/lifecycle/hsm/manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9905 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/lifecycle/hsm/store.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8491 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/lifecycle/registry.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/manager/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1112 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1294 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/client.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16847 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/dlg/manager/cmdline.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22746 2024-04-15 05:51:59.000000 daliuge-engine-4.0.1/dlg/manager/composite_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4760 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/drop_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    24082 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/manager/node_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15303 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/manager/proc_daemon.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5087 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/replay.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26138 2024-04-12 16:16:34.000000 daliuge-engine-4.0.1/dlg/manager/rest.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25242 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/dlg/manager/session.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3063 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/shared_memory_manager.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.296600 daliuge-engine-4.0.1/dlg/manager/web/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2024-04-12 15:17:52.000000 daliuge-engine-4.0.1/dlg/manager/web/LICENSE
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6373 2024-04-15 05:51:59.000000 daliuge-engine-4.0.1/dlg/manager/web/dim.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4107 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/manager/web/dm.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16527 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/manager/web/session.html
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.280600 daliuge-engine-4.0.1/dlg/manager/web/static/
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.300600 daliuge-engine-4.0.1/dlg/manager/web/static/css/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155845 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/css/bootstrap.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2145 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/css/dm.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      929 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/manager/web/static/css/progressBar.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8527 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/manager/web/static/css/session.css
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.300600 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20127 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   116671 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45404 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23424 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18028 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.300600 daliuge-engine-4.0.1/dlg/manager/web/static/icons/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3660 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/icons/engine.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/icons/liu.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/icons/liuFavIcon.svg
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.300600 daliuge-engine-4.0.1/dlg/manager/web/static/js/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15778 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/bootbox.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78743 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/d3.v5.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/dagre-d3.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/dagre-d3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26332 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/dm.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89501 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/manager/web/static/js/jquery-3.6.0.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2392 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/meta.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11588 2024-04-12 16:17:01.000000 daliuge-engine-4.0.1/dlg/named_port_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5526 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/ngaslite.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2920 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/nm_dim_assigner.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1056 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/dlg/passwd.template
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2326 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/prepareUser.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1938 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/process.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4565 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/remote.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1758 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/dlg/restserver.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11106 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/dlg/rpc.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/dlg/runtime/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3346 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/dlg/runtime/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2062 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/dlg/runtime/tool_commands.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      190 2024-04-15 07:01:41.000000 daliuge-engine-4.0.1/dlg/runtime/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6577 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/shared_memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2824 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/dlg/testutils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/docker/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      711 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/docker/Dockerfile
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3223 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/docker/Dockerfile.casa
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      857 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/docker/Dockerfile.dev
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1871 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/docker/Dockerfile.devall
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      832 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/docker/Dockerfile.ray
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      611 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/docker/Dockerfile_incontext
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.280600 daliuge-engine-4.0.1/etc/
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/etc/init-scripts/
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1948 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/etc/init-scripts/dlg-dim
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1952 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/etc/init-scripts/dlg-nm
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      994 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/etc/init-scripts/dlg.options
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/fabfile/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/fabfile/APPspecific.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/headers/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5420 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/headers/dlg_app.h
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1825 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/headers/dlg_app2.h
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.304600 daliuge-engine-4.0.1/pip/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      405 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/pip/requirements.txt
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     4678 2024-04-12 16:16:40.000000 daliuge-engine-4.0.1/run_engine.sh
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2024-04-15 07:01:42.320600 daliuge-engine-4.0.1/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6148 2024-04-15 06:59:37.000000 daliuge-engine-4.0.1/setup.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/show_DIMlogs.sh
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      183 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/show_NMlogs.sh
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      379 2023-06-29 09:21:30.000000 daliuge-engine-4.0.1/stop_engine.sh
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.308600 daliuge-engine-4.0.1/test/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2024-03-18 12:49:15.000000 daliuge-engine-4.0.1/test/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.308600 daliuge-engine-4.0.1/test/apps/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/apps/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.308600 daliuge-engine-4.0.1/test/apps/data/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   186588 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/apps/data/test_ms.tar.gz
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5909 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/apps/dynlib_example.c
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9088 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/apps/dynlib_example2.c
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1883 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/apps/setp_up.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9651 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/test/apps/test_bash.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3233 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/test/apps/test_crc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8359 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/apps/test_docker.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10276 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/test/apps/test_dynlib.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11864 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/test/apps/test_dynlib2.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17356 2024-04-12 16:12:35.000000 daliuge-engine-4.0.1/test/apps/test_pyfunc.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13107 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/apps/test_simple.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3429 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/test/apps/test_socket.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.312600 daliuge-engine-4.0.1/test/deploy/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/deploy/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4870 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/deploy/test_common.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5175 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/deploy/test_helm_deploy.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1499 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/deploy/test_slurm_utils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.312600 daliuge-engine-4.0.1/test/graphs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12649 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/graphs/ArrayLoopPG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1383 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/HelloWorld_simplePG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   100639 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/graphs/HelloWorld_universePG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/graphs/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35457 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/graphs/appTestPG_namedPorts.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2185 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/application_args.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18978 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/test/graphs/compilePG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2948 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/complex.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4985 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/graphs/ddTest.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8328 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/funcTestPG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9203 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/funcTestPG_namedPorts.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11025 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/graphs/pyfunc_glob_testPG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8748 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/graphs/test_graphExecution.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.312600 daliuge-engine-4.0.1/test/integrate/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.312600 daliuge-engine-4.0.1/test/integrate/chiles/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/chiles/__init__.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6166 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/integrate/chiles/chilesdo.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     4411 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/test/integrate/chiles/chilesdoapp.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6091 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/integrate/chiles/chilesdospec.py
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     6327 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/integrate/chiles/chilesdospec_docker.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2732 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/example_split.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      434 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/example_split.sh
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10795 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/freq_split.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.316600 daliuge-engine-4.0.1/test/integrate/msconverter/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      543 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/msconverter/makefile
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13468 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/msconverter/ms_checker.cc
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      439 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/integrate/msconverter/ms_converter.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.316600 daliuge-engine-4.0.1/test/lifecycle/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/lifecycle/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6514 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/lifecycle/test_dlm.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3552 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/test/lifecycle/test_registry.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.316600 daliuge-engine-4.0.1/test/manager/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/manager/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    13556 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/manager/test_daemon.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16470 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/manager/test_dim.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23335 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/test/manager/test_dm.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14649 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/manager/test_mm.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9781 2024-02-15 06:56:33.000000 daliuge-engine-4.0.1/test/manager/test_rest.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5229 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/manager/test_scalability.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3951 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/manager/test_smm.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2400 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/manager/testutils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3820 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/memoryUsage.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.316600 daliuge-engine-4.0.1/test/reproducibility/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/reproducibility/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5363 2024-03-25 12:52:04.000000 daliuge-engine-4.0.1/test/reproducibility/testSingle.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4858 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/reproducibility/test_drophash.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9811 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/test/reproducibility/test_lg_blockdag.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39765 2023-05-18 15:50:38.000000 daliuge-engine-4.0.1/test/reproducibility/test_pg_blockdag.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9278 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/test/reproducibility/test_toposort.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:42.320600 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15776 2024-03-25 12:38:01.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/computationSandwich.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    22856 2024-03-25 12:39:08.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataFan.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    23460 2024-03-25 12:39:58.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataFunnel.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17082 2024-03-25 12:40:29.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataSandwich.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20507 2024-03-25 12:51:00.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testCycle.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      655 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testEmpty.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20216 2024-03-25 12:50:09.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testNotDAG.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5363 2024-03-25 12:47:40.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testSingle.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15856 2024-03-25 12:51:33.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoEnd.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    19926 2024-03-25 12:48:58.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoLines.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15857 2024-03-25 12:48:24.000000 daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoStart.graph
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4096 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/test/test_JsonDrop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2882 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/test_ParameterSetDROP.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3677 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/test/test_S3Drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8959 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/test_dask_emulation.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48587 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/test_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10519 2024-03-18 15:04:41.000000 daliuge-engine-4.0.1/test/test_droputils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10122 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/test_environmentvars.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1268 2023-05-09 13:46:34.000000 daliuge-engine-4.0.1/test/test_event.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8980 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/test_graph_loader.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1164 2024-03-18 14:56:39.000000 daliuge-engine-4.0.1/test/test_input_fired_app_drop.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1589 2023-05-09 13:02:30.000000 daliuge-engine-4.0.1/test/test_io.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10509 2023-06-29 08:45:39.000000 daliuge-engine-4.0.1/test/test_session.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4642 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/test_shared_memory.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1672 2022-11-30 13:05:02.000000 daliuge-engine-4.0.1/test/test_tool.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7933 2023-05-18 15:50:38.000000 daliuge-engine-4.0.1/test/test_utils.py
```

### Comparing `daliuge-engine-4.0.0/PKG-INFO` & `daliuge-engine-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daliuge-engine
-Version: 4.0.0
+Version: 4.0.1
 Summary: Data Activated 流 (flow) Graph Engine - Execution Engine
 Home-page: https://github.com/ICRAR/daliuge
 Author: ICRAR DIA Group
 Author-email: dfms_prototype@googlegroups.com
 License: LGPLv2+
 Provides-Extra: spead
 Provides-Extra: drive-casa
```

### Comparing `daliuge-engine-4.0.0/build_engine.sh` & `daliuge-engine-4.0.1/build_engine.sh`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         C_TAG="master"
         echo "Building daliuge-engine slim version ${VCS_TAG} using daliuge-common:${VCS_TAG}"
         docker build --build-arg USER=${USER} --build-arg VCS_TAG=${VCS_TAG} --no-cache -t icrar/daliuge-engine.big:${VCS_TAG} -f docker/Dockerfile .
         echo "Build finished! Slimming the image now"
         echo ">>>>> docker-slim output <<<<<<<<<"
         docker run -it --rm -v /var/run/docker.sock:/var/run/docker.sock dslim/docker-slim build --include-shell \
             --include-path /etc --include-path /usr/local/lib --include-path /usr/local/bin --include-path /usr/lib/python3.8 \
-            --include-path /usr/lib/python3 --include-path /dlg --include-path /daliuge --publish-exposed-ports=true \
+            --include-path /usr/lib/python3 --include-path /usr/bin/hostname --include-path /dlg --include-path /daliuge --publish-exposed-ports=true \
             --http-probe=true --tag=icrar/daliuge-engine:${VCS_TAG}\
             icrar/daliuge-engine.big:${VCS_TAG} \
 	    ;;
     *)
         echo "Usage: build_engine.sh <dep|dev|devall|slim>"
         exit 0;;
 esac
```

### Comparing `daliuge-engine-4.0.0/daliuge_engine.egg-info/PKG-INFO` & `daliuge-engine-4.0.1/daliuge_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daliuge-engine
-Version: 4.0.0
+Version: 4.0.1
 Summary: Data Activated 流 (flow) Graph Engine - Execution Engine
 Home-page: https://github.com/ICRAR/daliuge
 Author: ICRAR DIA Group
 Author-email: dfms_prototype@googlegroups.com
 License: LGPLv2+
 Provides-Extra: spead
 Provides-Extra: drive-casa
```

### Comparing `daliuge-engine-4.0.0/daliuge_engine.egg-info/SOURCES.txt` & `daliuge-engine-4.0.1/daliuge_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/__init__.py` & `daliuge-engine-4.0.1/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/__init__.py` & `daliuge-engine-4.0.1/dlg/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/app_base.py` & `daliuge-engine-4.0.1/dlg/apps/app_base.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/archiving.py` & `daliuge-engine-4.0.1/dlg/apps/archiving.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/bash_shell_app.py` & `daliuge-engine-4.0.1/dlg/apps/bash_shell_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,24 +37,29 @@
 import tempfile
 import threading
 import time
 import types
 import json
 
 from .. import droputils, utils
-from dlg.named_port_utils import replace_named_ports
+from dlg.named_port_utils import (
+    DropParser,
+    get_port_reader_function,
+    replace_named_ports,
+)
 from ..ddap_protocol import AppDROPStates, DROPStates
 from ..apps.app_base import BarrierAppDROP, AppDROP
 from ..exceptions import InvalidDropException
 from ..meta import (
     dlg_string_param,
     dlg_component,
     dlg_batch_input,
     dlg_batch_output,
     dlg_streaming_input,
+    dlg_enum_param,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 def message_stdouts(prefix, stdout, stderr, enc="utf8"):
@@ -159,14 +164,15 @@
     Common class for BashShell apps. It simply requires a command to be
     specified.
     """
 
     # TODO: use the shlex module for most of the construction of the
     # command line to get a proper and safe shell syntax
     command = dlg_string_param("Bash command", None)
+    input_parser: DropParser = dlg_enum_param(DropParser, "input_parser", DropParser.PICKLE)  # type: ignore
 
     def initialize(self, **kwargs):
         super(BashShellBase, self).initialize(**kwargs)
 
         self.proc = None
         self._inputRedirect = self._popArg(kwargs, "input_redirection", "")
         self._outputRedirect = self._popArg(kwargs, "output_redirection", "")
@@ -210,22 +216,24 @@
             uid: o for uid, o in outputs.items() if not droputils.has_path(o)
         }
         # deal with named ports
         inport_names = self.parameters["inputs"] if "inputs" in self.parameters else []
         outport_names = (
             self.parameters["outputs"] if "outputs" in self.parameters else []
         )
+        reader = get_port_reader_function(self.input_parser)
         keyargs, pargs = replace_named_ports(
             inputs.items(),
             outputs.items(),
             inport_names,
             outport_names,
             self.appArgs,
             argumentPrefix=self._argumentPrefix,
             separator=self._paramValueSeparator,
+            parser=reader,
         )
         argumentString = (
             f"{' '.join(map(str,pargs + keyargs))}"  # add kwargs to end of pargs
         )
         # complete command including all additional parameters and optional redirects
         if len(argumentString.strip()) > 0:
             # the _cmdLineArgs would very likely make the command line invalid
```

### Comparing `daliuge-engine-4.0.0/dlg/apps/branch.py` & `daliuge-engine-4.0.1/dlg/apps/branch.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/constructs.py` & `daliuge-engine-4.0.1/dlg/apps/constructs.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/crc.py` & `daliuge-engine-4.0.1/dlg/apps/crc.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/dlg_app.h` & `daliuge-engine-4.0.1/dlg/apps/dlg_app.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/dlg_app2.h` & `daliuge-engine-4.0.1/dlg/apps/dlg_app2.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/dockerapp.py` & `daliuge-engine-4.0.1/dlg/apps/dockerapp.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/dynlib.py` & `daliuge-engine-4.0.1/dlg/apps/dynlib.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/mpi.py` & `daliuge-engine-4.0.1/dlg/apps/mpi.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/plasmaflight.py` & `daliuge-engine-4.0.1/dlg/apps/plasmaflight.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/pyfunc.py` & `daliuge-engine-4.0.1/dlg/apps/pyfunc.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,17 +33,22 @@
 import pickle
 
 from typing import Callable
 import dill
 from io import StringIO
 from contextlib import redirect_stdout
 
-from dlg import droputils, drop_loaders
+from dlg import drop_loaders
 from dlg.utils import serialize_data, deserialize_data
-from dlg.named_port_utils import check_ports_dict, identify_named_ports
+from dlg.named_port_utils import (
+    DropParser,
+    check_ports_dict,
+    get_port_reader_function,
+    identify_named_ports,
+)
 from dlg.apps.app_base import BarrierAppDROP
 from dlg.exceptions import InvalidDropException
 from dlg.meta import (
     dlg_string_param,
     dlg_enum_param,
     dlg_dict_param,
     dlg_component,
@@ -132,24 +137,14 @@
             return mod
 
 
 def import_using_code(code):
     return dill.loads(code)
 
 
-class DropParser(Enum):
-    RAW = "raw"
-    PICKLE = "pickle"
-    EVAL = "eval"
-    NPY = "npy"
-    # JSON = "json"
-    PATH = "path"  # input only
-    DATAURL = "dataurl"  # input only
-
-
 ##
 # @brief PythonMemberFunction
 # @details A placeholder APP to aid construction of new class member function applications.
 # This is mainly useful (and used) when starting a new workflow from scratch.
 # @par EAGLE_START
 # @param category PythonMemberFunction
 # @param tag daliuge
@@ -350,14 +345,159 @@
                     bool
                     or self._applicationArgs[kw]["value"]
                     or self._applicationArgs[kw]["precious"],
                 ):
                     # only transfer if there is a value or precious is True
                     self._applicationArgs.pop(kw)
 
+    def _init_appArgs(self, pargsDict, keyargsDict, inputs, outputs, posargs) -> list:
+        """
+        Identify and fill application arguments.
+
+        Deals with positional and keyword arguments.
+
+        Returns:
+        --------
+        list, [funcargs, pargs]
+        """
+        pargs = []
+        funcargs = {}
+        if "applicationArgs" in self.parameters:
+            appArgs = self.parameters["applicationArgs"]  # we'll pop the default ones
+            _dum = [appArgs.pop(k) for k in self.func_def_keywords if k in appArgs]
+            logger.debug(
+                "Default keyword arguments removed: %s",
+                [i for i in _dum],
+            )
+            # update the positional args
+            pargsDict.update(
+                {k: self.parameters[k] for k in pargsDict if k in self.parameters}
+            )
+            # if defined in both we use AppArgs values
+            for arg in appArgs:
+                # check value type and interpret
+                if appArgs[arg]["type"] in ["Json", "Complex"]:
+                    try:
+                        value = ast.literal_eval(appArgs[arg]["value"])
+                        logger.debug(
+                            f"Evaluated %s to %s",
+                            appArgs[arg]["value"],
+                            type(value),
+                        )
+                        appArgs[arg]["value"] = value
+                    except ValueError:
+                        logger.error("Unable to evaluate %s", appArgs[arg]["value"])
+                else:
+                    value = appArgs[arg]["value"]
+                if arg in pargsDict:
+                    pargsDict.update({arg: value})
+
+            _ = [appArgs.pop(k) for k in pargsDict if k in appArgs]
+            logger.debug("Updated posargs dictionary: %s", pargsDict)
+
+            keyargsDict.update(
+                {k: appArgs[k]["value"] for k in keyargsDict if k in appArgs}
+            )
+            logger.debug("Updated keyargs dictionary: %s", keyargsDict)
+
+            # 2. put all remaining arguments into *args and **kwargs
+            # TODO: This should only be done if the function signature allows it
+            vparg = []
+            vkarg = {}
+            logger.debug(f"Remaining AppArguments {appArgs}")
+            for arg in appArgs:
+                if appArgs[arg]["type"] in ["Json", "Complex"]:
+                    value = ast.literal_eval(appArgs[arg]["value"])
+                else:
+                    value = appArgs[arg]["value"]
+                if appArgs[arg]["positional"]:
+                    vparg.append(value)
+                else:
+                    vkarg.update({arg: value})
+
+            # TODO: check where this is defined in signature
+            self.arguments = inspect.getfullargspec(self.f)
+            if self.arguments.varargs:
+                logger.debug("Adding remaining *args to pargs %s", vparg)
+                pargs.extend(vparg)
+            if self.arguments.varkw:
+                logger.debug("Adding remaining **kwargs to funcargs: %s", vkarg)
+                funcargs.update(vkarg)
+
+        logger.debug(f"Updating funcargs with values from pargsDict {pargsDict}")
+        funcargs.update(pargsDict)
+
+        # Mixin the values from named ports
+        portargs = self._ports2args(inputs, outputs, posargs, pargsDict, keyargsDict)
+
+        logger.debug(f"Updating funcargs with values from named ports {portargs}")
+        funcargs.update(portargs)
+
+        return [funcargs, pargs]
+
+    def _ports2args(self, inputs, outputs, posargs, pargsDict, keyargsDict) -> dict:
+        """
+        Replace arguments with values from ports.
+
+        Returns:
+        --------
+        portargs dictionary
+        """
+        portargs = {}
+        # 3. replace default argument values with named input ports
+        # TODO: investigate performing inputs and outputs in a single call
+        if "inputs" in self.parameters and check_ports_dict(self.parameters["inputs"]):
+            check_len = min(
+                len(inputs),
+                self.fn_nargs + self.fn_nkw,
+            )
+            inputs_dict = collections.OrderedDict()
+            for inport in self.parameters["inputs"]:
+                key = list(inport.keys())[0]
+                inputs_dict[key] = {"name": inport[key], "path": inputs[key]}
+            portargs.update(
+                identify_named_ports(
+                    inputs_dict,
+                    posargs,
+                    pargsDict,
+                    keyargsDict,
+                    check_len=check_len,
+                    mode="inputs",
+                )
+            )
+        else:
+            # Just as a fallback using the index, but this is risky!
+            for i in range(min(len(inputs), self.fn_nargs)):
+                portargs.update({self.argnames[i]: list(inputs.values())[i]})
+
+        # 4. replace default argument values with named output ports
+        if "outputs" in self.parameters and check_ports_dict(
+            self.parameters["outputs"]
+        ):
+            check_len = min(len(outputs), self.fn_nargs + self.fn_nkw)
+            outputs_dict = collections.OrderedDict()
+            for outport in self.parameters["outputs"]:
+                key = list(outport.keys())[0]
+                outputs_dict[key] = {
+                    "name": outport[key],
+                    "path": outputs[key],
+                }
+
+            portargs.update(
+                identify_named_ports(
+                    outputs_dict,
+                    posargs,
+                    pargsDict,
+                    keyargsDict,
+                    check_len=check_len,
+                    mode="outputs",
+                )
+            )
+        return portargs
+
     def initialize_with_func_code(self):
         """
         This function takes over if code is passed in through an argument.
         """
         if not isinstance(self.func_code, bytes):
             self.func_code = base64.b64decode(self.func_code.encode("utf8"))
         self.f = import_using_code(self.func_code)
@@ -449,37 +589,15 @@
 
         Input ports will NOT be used by index (anymore), but by using the name of the port.
         Since each input port requires an associated data drop, this provides a unique
         mapping. This also allows to pass values to any function argument through a port.
 
         """
         funcargs = {}
-        # Inputs are un-pickled and treated as the arguments of the function
-        # Their order must be preserved, so we use an OrderedDict
-        if self.input_parser is DropParser.PICKLE:
-            # all_contents = lambda x: pickle.loads(droputils.allDropContents(x))
-            all_contents = drop_loaders.load_pickle
-        elif self.input_parser is DropParser.EVAL:
-
-            def optionalEval(x):
-                # Null and Empty Drops will return an empty byte string
-                # which should propogate back to None
-                content: str = droputils.allDropContents(x).decode("utf-8")
-                return ast.literal_eval(content) if len(content) > 0 else None
-
-            all_contents = optionalEval
-        elif self.input_parser is DropParser.NPY:
-            all_contents = drop_loaders.load_npy
-        elif self.input_parser is DropParser.PATH:
-            all_contents = lambda x: x.path
-        elif self.input_parser is DropParser.DATAURL:
-            all_contents = lambda x: x.dataurl
-        else:
-            raise ValueError(self.input_parser.__repr__())
-
+        all_contents = get_port_reader_function(self.input_parser)
         inputs = collections.OrderedDict()
         for uid, drop in self._inputs.items():
             inputs[uid] = all_contents(drop)
 
         outputs = collections.OrderedDict()
         for uid, drop in self._outputs.items():
             if self.output_parser is DropParser.PATH:
@@ -491,143 +609,26 @@
         # that match one of the keyword argument names
         # if defaults dict has not been specified at all we'll go ahead anyway
 
         # 1. Fill arguments with rest of inputs
         logger.debug(f"available inputs: {inputs}")
 
         posargs = list(self.posonly.keys()) + list(self.poskw.keys())
-        kwargs = {}
-        pargs = []
         # fill the pargsDict with positional and poskw arguments and defaults
         pargsDict = {k: v.default for k, v in self.posonly.items()}
         pargsDict.update({k: v.default for k, v in self.poskw.items()})
         logger.debug("Initial pos_kwargs dictionary: %s", pargsDict)
         # fill the keyargsDict with kwonly arguments and defaults
         keyargsDict = {k: v.default for k, v in self.kwonly.items()}
         logger.debug("Initial kwonly dictionary: %s", self.kwonly)
 
-        # replace default argument values with provided values
-        if "applicationArgs" in self.parameters:
-            appArgs = self.parameters[
-                "applicationArgs"
-            ]  # we'll pop the identified ones
-            _dum = [appArgs.pop(k) for k in self.func_def_keywords if k in appArgs]
-            logger.debug(
-                "Default keyword arguments removed: %s",
-                [i for i in _dum],
-            )
-            # update the positional args
-            pargsDict.update(
-                {k: self.parameters[k] for k in pargsDict if k in self.parameters}
-            )
-            # if defined in both we use AppArgs values
-            for k in appArgs:
-                # check value type and interpret
-                if appArgs[k]["type"] in ["Json", "Complex"]:
-                    try:
-                        value = ast.literal_eval(appArgs[k]["value"])
-                        logger.debug(
-                            f"Evaluated %s to %s",
-                            appArgs[k]["value"],
-                            type(value),
-                        )
-                        appArgs[k]["value"] = value
-                    except ValueError:
-                        logger.error("Unable to evaluate %s", appArgs[k]["value"])
-                else:
-                    value = appArgs[k]["value"]
-                if k in pargsDict:
-                    pargsDict.update({k: value})
-
-            _ = [appArgs.pop(k) for k in pargsDict if k in appArgs]
-            logger.debug("Updated posargs dictionary: %s", pargsDict)
-
-            keyargsDict.update(
-                {k: appArgs[k]["value"] for k in keyargsDict if k in appArgs}
-            )
-            logger.debug("Updated keyargs dictionary: %s", keyargsDict)
-
-            # 2. put all remaining arguments into *args and **kwargs
-            # TODO: This should only be done if the function signature allows it
-            vparg = []
-            vkarg = {}
-            logger.debug(f"Remaining AppArguments {appArgs}")
-            for arg in appArgs:
-                if appArgs[arg]["type"] in ["Json", "Complex"]:
-                    value = ast.literal_eval(appArgs[arg]["value"])
-                else:
-                    value = appArgs[arg]["value"]
-                if appArgs[arg]["positional"]:
-                    vparg.append(value)
-                else:
-                    vkarg.update({arg: value})
-
-            # TODO: check where this is defined in signature
-            self.arguments = inspect.getfullargspec(self.f)
-            if self.arguments.varargs:
-                logger.debug("Adding remaining *args to pargs %s", vparg)
-                pargs.extend(vparg)
-            if self.arguments.varkw:
-                logger.debug("Adding remaining **kwargs to funcargs: %s", vkarg)
-                funcargs.update(vkarg)
-
-        # 3. replace default argument values with named input ports
-        # TODO: investigate performing inputs and outputs in a single call
-        if "inputs" in self.parameters and check_ports_dict(self.parameters["inputs"]):
-            check_len = min(
-                len(inputs),
-                self.fn_nargs + self.fn_nkw,
-            )
-            inputs_dict = collections.OrderedDict()
-            for inport in self.parameters["inputs"]:
-                key = list(inport.keys())[0]
-                inputs_dict[key] = {"name": inport[key], "path": inputs[key]}
-            kwargs.update(
-                identify_named_ports(
-                    inputs_dict,
-                    posargs,
-                    pargsDict,
-                    keyargsDict,
-                    check_len=check_len,
-                    mode="inputs",
-                )
-            )
-        else:
-            # Just as a fallback using the index, but this is risky!
-            for i in range(min(len(inputs), self.fn_nargs)):
-                kwargs.update({self.argnames[i]: list(inputs.values())[i]})
-
-        # 4. replace default argument values with named output ports
-        if "outputs" in self.parameters and check_ports_dict(
-            self.parameters["outputs"]
-        ):
-            check_len = min(len(outputs), self.fn_nargs + self.fn_nkw)
-            outputs_dict = collections.OrderedDict()
-            for outport in self.parameters["outputs"]:
-                key = list(outport.keys())[0]
-                outputs_dict[key] = {
-                    "name": outport[key],
-                    "path": outputs[key],
-                }
-
-            kwargs.update(
-                identify_named_ports(
-                    outputs_dict,
-                    posargs,
-                    pargsDict,
-                    keyargsDict,
-                    check_len=check_len,
-                    mode="outputs",
-                )
-            )
-        logger.debug(f"Updating funcargs with values from pargsDict {pargsDict}")
-        funcargs.update(pargsDict)
-
-        logger.debug(f"Updating funcargs with values from named ports {kwargs}")
-        funcargs.update(kwargs)
+        # deal with arguments of any sort
+        funcargs, pargs = self._init_appArgs(
+            pargsDict, keyargsDict, inputs, outputs, posargs
+        )
 
         self._recompute_data["args"] = funcargs.copy()
 
         # 5. remove self argument if this is the initializer.
         if (
             self.func_name is not None
             and self.func_name.split(".")[-1] in ["__init__", "__class__"]
@@ -670,14 +671,16 @@
                 if self.output_parser is DropParser.PICKLE:
                     logger.debug(f"Writing pickeled result {type(r)} to {o}")
                     o.write(pickle.dumps(r))
                 elif self.output_parser is DropParser.EVAL:
                     o.write(repr(r).encode("utf-8"))
                 elif self.output_parser is DropParser.NPY:
                     drop_loaders.save_npy(o, r)
+                elif self.output_parser is DropParser.RAW:
+                    o.write(r)
                 else:
                     ValueError(self.output_parser.__repr__())
 
     def generate_recompute_data(self):
         for name, val in self._recompute_data.items():
             try:
                 json.dumps(val)
```

### Comparing `daliuge-engine-4.0.0/dlg/apps/scp.py` & `daliuge-engine-4.0.1/dlg/apps/scp.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/simple.py` & `daliuge-engine-4.0.1/dlg/apps/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 #
 """Applications used as examples, for testing, or in simple situations"""
 import _pickle
 from numbers import Number
 import pickle
 import random
 from typing import List, Optional
-import urllib.error
-import urllib.request
+import requests
 import logging
 import time
 import numpy as np
 
 from dlg import droputils, drop_loaders
 from dlg.apps.app_base import BarrierAppDROP
 from dlg.data.drops.container import ContainerDROP
@@ -643,26 +642,25 @@
         [dlg_streaming_input("binary/*")],
     )
 
     url = dlg_string_param("url", "")
 
     def run(self):
         try:
-            u = urllib.request.urlopen(self.url)
-        except urllib.error.URLError as e:
+            logger.info("Accessing URL %s", self.url)
+            u = requests.get(self.url)
+        except requests.exceptions.RequestException as e:
             raise e.reason
 
-        content = u.read()
-
         outs = self.outputs
         if len(outs) < 1:
             raise Exception("At least one output should have been added to %r" % self)
         for o in outs:
-            o.len = len(content)
-            o.write(content)  # send content to all outputs
+            o.len = len(u.content)
+            o.write(u.content)  # send content to all outputs
 
 
 ##
 # @brief GenericScatterApp
 # @details An APP that splits about any object that can be converted to a numpy array
 # into as many parts as the app has outputs, provided that the initially converted numpy
 # array has enough elements. The return will be a numpy array of arrays, where the first
```

### Comparing `daliuge-engine-4.0.0/dlg/apps/simple_functions.py` & `daliuge-engine-4.0.1/dlg/apps/simple_functions.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/apps/socket_listener.py` & `daliuge-engine-4.0.1/dlg/apps/socket_listener.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/dask_emulation.py` & `daliuge-engine-4.0.1/dlg/dask_emulation.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/__init__.py` & `daliuge-engine-4.0.1/dlg/data/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/__init__.py` & `daliuge-engine-4.0.1/dlg/data/drops/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/container.py` & `daliuge-engine-4.0.1/dlg/data/drops/container.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/data_base.py` & `daliuge-engine-4.0.1/dlg/data/drops/data_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,23 +164,21 @@
         self._checkStateAndDescriptor(descriptor)
         io = self._rios[descriptor]
         return io.read(count, **kwargs)
 
     def _checkStateAndDescriptor(self, descriptor):
         if self.status != DROPStates.COMPLETED:
             raise Exception(
-                "%r is in state %s (!=COMPLETED), cannot be read"
-                % (self, self.status)
+                "%r is in state %s (!=COMPLETED), cannot be read" % (self, self.status)
             )
         if descriptor is None:
             raise ValueError("Illegal empty descriptor given")
         if descriptor not in self._rios:
             raise Exception(
-                "Illegal descriptor %d given, remember to open() first"
-                % (descriptor)
+                "Illegal descriptor %d given, remember to open() first" % (descriptor)
             )
 
     def isBeingRead(self):
         """
         Returns `True` if the DROP is currently being read; `False`
         otherwise
         """
@@ -196,18 +194,16 @@
         The underlying storage mechanism is responsible for implementing the
         final writing logic via the `self.writeMeta()` method.
         """
 
         if self.status not in [DROPStates.INITIALIZED, DROPStates.WRITING]:
             raise Exception("No more writing expected")
 
-        if not isinstance(data, (bytes, memoryview)):
-            raise Exception(
-                "Data type not of binary type: %s", type(data).__name__
-            )
+        if not isinstance(data, (bytes, memoryview, str)):
+            raise Exception("Data type not of binary type: ", type(data).__name__)
 
         # We lazily initialize our writing IO instance because the data of this
         # DROP might not be written through this DROP
         if not self._wio:
             self._wio = self.getIO()
             try:
                 self._wio.open(OpenMode.OPEN_WRITE)
```

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/directorycontainer.py` & `daliuge-engine-4.0.1/dlg/data/drops/directorycontainer.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/environmentvar_drop.py` & `daliuge-engine-4.0.1/dlg/data/drops/environmentvar_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/file.py` & `daliuge-engine-4.0.1/dlg/data/drops/file.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/json_drop.py` & `daliuge-engine-4.0.1/dlg/data/drops/json_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/memory.py` & `daliuge-engine-4.0.1/dlg/data/drops/memory.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/ngas.py` & `daliuge-engine-4.0.1/dlg/data/drops/ngas.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/parset_drop.py` & `daliuge-engine-4.0.1/dlg/data/drops/parset_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/plasma.py` & `daliuge-engine-4.0.1/dlg/data/drops/plasma.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/rdbms.py` & `daliuge-engine-4.0.1/dlg/data/drops/rdbms.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/data/drops/s3_drop.py` & `daliuge-engine-4.0.1/dlg/data/drops/s3_drop.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     dlg_batch_input,
     dlg_batch_output,
     dlg_streaming_input,
     dlg_string_param,
     dlg_list_param,
 )
 
-from dlg.named_port_utils import identify_named_ports, check_ports_dict
+# from dlg.named_port_utils import identify_named_ports, check_ports_dict
 
 
 ##
 # @brief S3
 # @details An object available in a bucket on a S3 (Simple Storage Service) object storage platform
 # @par EAGLE_START
 # @param category S3
@@ -124,18 +124,18 @@
 
     def getIO(self) -> DataIO:
         """
         Return
         :return:
         """
         logger.debug("S3DROP producers: %s", self._producers)
-        if check_ports_dict(self._producers):
-            self.mapped_inputs = identify_named_ports(
-                self._producers, {}, self.keyargs, mode="inputs"
-            )
+        # if check_ports_dict(self._producers):
+        #     self.mapped_inputs = identify_named_ports(
+        #         self._producers, {}, self.keyargs, mode="inputs"
+        #     )
         logger.debug("Parameters found: {}", self.parameters)
         return S3IO(
             self.aws_access_key_id,
             self.aws_secret_access_key,
             self.profile_name,
             self.Bucket,
             self.Key,
@@ -305,16 +305,15 @@
             ):  # write, if there is still something in the buffer
                 self._writeBuffer2S3(self._buffer)
             # complete multipart upload and cleanup
             res = self._s3.list_parts(
                 Bucket=self._bucket, Key=self._key, UploadId=self._uploadId
             )
             parts = [
-                {"ETag": p["ETag"], "PartNumber": p["PartNumber"]}
-                for p in res["Parts"]
+                {"ETag": p["ETag"], "PartNumber": p["PartNumber"]} for p in res["Parts"]
             ]
             # TODO: Check checksum!
             res = self._s3.complete_multipart_upload(
                 Bucket=self._bucket,
                 Key=self._key,
                 UploadId=self._uploadId,
                 MultipartUpload={"Parts": parts},
```

### Comparing `daliuge-engine-4.0.0/dlg/data/io.py` & `daliuge-engine-4.0.1/dlg/data/io.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/ddap_protocol.py` & `daliuge-engine-4.0.1/dlg/ddap_protocol.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/__init__.py` & `daliuge-engine-4.0.1/dlg/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/common.py` & `daliuge-engine-4.0.1/dlg/deploy/common.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/configs/__init__.py` & `daliuge-engine-4.0.1/dlg/deploy/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/create_dlg_job.py` & `daliuge-engine-4.0.1/dlg/deploy/create_dlg_job.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/deployment_constants.py` & `daliuge-engine-4.0.1/dlg/deploy/deployment_constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/deployment_utils.py` & `daliuge-engine-4.0.1/dlg/deploy/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/dlg_monitor.py` & `daliuge-engine-4.0.1/dlg/deploy/dlg_monitor.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/dlg_proxy.py` & `daliuge-engine-4.0.1/dlg/deploy/dlg_proxy.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/helm_client.py` & `daliuge-engine-4.0.1/dlg/deploy/helm_client.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/remotes.py` & `daliuge-engine-4.0.1/dlg/deploy/remotes.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/slurm_client.py` & `daliuge-engine-4.0.1/dlg/deploy/slurm_client.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/start_dlg_cluster.py` & `daliuge-engine-4.0.1/dlg/deploy/start_dlg_cluster.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/start_helm_cluster.py` & `daliuge-engine-4.0.1/dlg/deploy/start_helm_cluster.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/deploy/utils/monitor_replayer.py` & `daliuge-engine-4.0.1/dlg/deploy/utils/monitor_replayer.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/drop.py` & `daliuge-engine-4.0.1/dlg/drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/drop_loaders.py` & `daliuge-engine-4.0.1/dlg/drop_loaders.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/droputils.py` & `daliuge-engine-4.0.1/dlg/droputils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 #
 """
 Utility methods and classes to be used when interacting with DROPs
 """
 
-import base64
 import collections
 import io
 import time
 import logging
-import pickle
 import re
 import threading
 import traceback
 
 from dlg.ddap_protocol import DROPStates
 from dlg.data.io import IOForURL, OpenMode
 from dlg import common
@@ -135,29 +133,25 @@
         if not data:
             break
         buf.write(data)
     drop.close(desc)
     return buf.getvalue()
 
 
-def copyDropContents(
-    source: "DataDROP", target: "DataDROP", bufsize: int = 65536
-):
+def copyDropContents(source: "DataDROP", target: "DataDROP", bufsize: int = 65536):
     """
     Manually copies data from one DROP into another, in bufsize steps
     """
     logger.debug("Copying from %s to %s", repr(source), repr(target))
     sdesc = source.open()
     buf = source.read(sdesc, bufsize)
     logger.debug("Read %d bytes from %s", len(buf), repr(source))
     st = time.time()
     ssize = source.size if source.size is not None else -1
-    logger.debug(
-        "Source size: %s; Source checksum: %s", ssize, source.checksum
-    )
+    logger.debug("Source size: %s; Source checksum: %s", ssize, source.checksum)
     tot_w = 0
     ofl = True
     # target._expectedSize = ssize
     while buf:
         tot_w += target.write(buf)
         dur = int(time.time() - st)
         if dur > 5 and dur % 5 == 0 and ofl:
```

### Comparing `daliuge-engine-4.0.0/dlg/event.py` & `daliuge-engine-4.0.1/dlg/event.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/graph_loader.py` & `daliuge-engine-4.0.1/dlg/graph_loader.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/__init__.py` & `daliuge-engine-4.0.1/dlg/lifecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/dlm.py` & `daliuge-engine-4.0.1/dlg/lifecycle/dlm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/hsm/__init__.py` & `daliuge-engine-4.0.1/dlg/lifecycle/hsm/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/hsm/manager.py` & `daliuge-engine-4.0.1/dlg/lifecycle/hsm/manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/hsm/store.py` & `daliuge-engine-4.0.1/dlg/lifecycle/hsm/store.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/lifecycle/registry.py` & `daliuge-engine-4.0.1/dlg/lifecycle/registry.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/__init__.py` & `daliuge-engine-4.0.1/dlg/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/client.py` & `daliuge-engine-4.0.1/dlg/manager/client.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/cmdline.py` & `daliuge-engine-4.0.1/dlg/manager/cmdline.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/composite_manager.py` & `daliuge-engine-4.0.1/dlg/manager/composite_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,30 +194,43 @@
         self._tp.close()
         self._tp.terminate()
         self._tp.join()
 
     def _checkDM(self):
         while True:
             for host in self._dmHosts:
+                if ":" in host:
+                    host, port = host.split(":")
+                    port = int(port)
+                else:
+                    port = constants.NODE_DEFAULT_REST_PORT
                 if self._dmCheckerEvt.is_set():
                     break
-                if not self.check_dm(host, timeout=self._dmCheckTimeout):
+                if not self.check_dm(host, port, timeout=self._dmCheckTimeout):
                     logger.error(
                         "Couldn't contact manager for host %s, will try again later",
                         host,
                     )
             if self._dmCheckerEvt.wait(60):
                 break
 
     @property
     def dmHosts(self):
         return self._dmHosts[:]
 
     def addDmHost(self, host):
-        self._dmHosts.append(host)
+        if ":" not in host:
+            if self._subDmId == "node":
+                host += constants.NODE_DEFAULT_REST_PORT
+            elif self._subDmId == "island":
+                host += constants.ISLAND_DEFAULT_REST_PORT
+        if host not in self._dmHosts:
+            self._dmHosts.append(host)
+        else:
+            logger.warning("Host %s already registered.", host)
 
     def removeDmHost(self, host):
         if host in self._dmHosts:
             self._dmHosts.remove(host)
 
     @property
     def nodes(self):
@@ -252,20 +265,21 @@
         return self._sessionIds
 
     #
     # Replication of commands to underlying drop managers
     # If "collect" is given, then individual results are also kept in the given
     # structure, which is either a dictionary or a list
     #
-    def _do_in_host(
-        self, action, sessionId, exceptions, f, collect, port, iterable
-    ):
+    def _do_in_host(self, action, sessionId, exceptions, f, collect, port, iterable):
         host = iterable
         if isinstance(iterable, (list, tuple)):
             host = iterable[0]
+        if ":" in host:
+            host, port = host.split(":")
+            port = int(port)
 
         try:
             with self.dmAt(host, port) as dm:
                 res = f(dm, iterable, sessionId)
 
             if isinstance(collect, dict):
                 collect.update(res)
@@ -277,17 +291,15 @@
             logger.exception(
                 "Error while %s on host %s, session %s",
                 action,
                 host,
                 sessionId,
             )
 
-    def replicate(
-        self, sessionId, f, action, collect=None, iterable=None, port=None
-    ):
+    def replicate(self, sessionId, f, action, collect=None, iterable=None, port=None):
         """
         Replicates the given function call on each of the underlying drop managers
         """
         thrExs = {}
         iterable = iterable or self._dmHosts
         port = port or self._dmPort
         self._tp.map(
@@ -314,30 +326,26 @@
         logger.info("Creating Session %s in all hosts", sessionId)
         self.replicate(sessionId, self._createSession, "creating sessions")
         logger.info("Successfully created session %s in all hosts", sessionId)
         self._sessionIds.append(sessionId)
 
     def _cancelSession(self, dm, host, sessionId):
         dm.cancelSession(sessionId)
-        logger.debug(
-            "Successfully cancelled session %s on %s", sessionId, host
-        )
+        logger.debug("Successfully cancelled session %s on %s", sessionId, host)
 
     def cancelSession(self, sessionId):
         """
         Cancels a session in all underlying DMs.
         """
         logger.info("Cancelled session %s in all hosts", sessionId)
         self.replicate(sessionId, self._cancelSession, "cancelling sessions")
 
     def _destroySession(self, dm, host, sessionId):
         dm.destroySession(sessionId)
-        logger.debug(
-            "Successfully destroyed session %s on %s", sessionId, host
-        )
+        logger.debug("Successfully destroyed session %s on %s", sessionId, host)
 
     def destroySession(self, sessionId):
         """
         Destroy a session in all underlying DMs.
         """
         logger.info("Destroying Session %s in all hosts", sessionId)
         self.replicate(sessionId, self._destroySession, "creating sessions")
@@ -351,17 +359,15 @@
             sessionId,
             host,
         )
 
     def _addGraphSpec(self, dm, host_and_graphspec, sessionId):
         host, graphSpec = host_and_graphspec
         dm.addGraphSpec(sessionId, graphSpec)
-        logger.info(
-            "Successfully appended graph to session %s on %s", sessionId, host
-        )
+        logger.info("Successfully appended graph to session %s on %s", sessionId, host)
 
     def addGraphSpec(self, sessionId, graphSpec):
         # The first step is to break down the graph into smaller graphs that
         # belong to the same host, so we can submit that graph into the individual
         # DMs. For this we need to make sure that our graph has a the correct
         # attribute set
         logger.info(
@@ -400,17 +406,15 @@
             self._graph[uid_for_drop(dropSpec)] = dropSpec
         # At each partition the relationships between DROPs should be local at the
         # moment of submitting the graph; thus we record the inter-partition
         # relationships separately and remove them from the original graph spec
         logger.info("Graph split into %r", perPartition.keys())
         inter_partition_rels = []
         for dropSpecs in perPartition.values():
-            inter_partition_rels += graph_loader.removeUnmetRelationships(
-                dropSpecs
-            )
+            inter_partition_rels += graph_loader.removeUnmetRelationships(dropSpecs)
         sanitize_relations(inter_partition_rels, self._graph)
         logger.info(
             "Removed (and sanitized) %d inter-dm relationships",
             len(inter_partition_rels),
         )
 
         # Store the inter-partition relationships; later on they have to be
@@ -425,17 +429,15 @@
             drop_rels[rhn][lhn].append(rel)
 
         self._drop_rels[sessionId] = drop_rels
         logger.debug("Calculated NM-level drop relationships: %r", drop_rels)
 
         # Create the individual graphs on each DM now that they are correctly
         # separated.
-        logger.info(
-            "Adding individual graphSpec of session %s to each DM", sessionId
-        )
+        logger.info("Adding individual graphSpec of session %s to each DM", sessionId)
         for partition in perPartition:
             if self._graph.get("reprodata") is not None:
                 perPartition[partition].append(self._graph["reprodata"])
         self.replicate(
             sessionId,
             self._addGraphSpec,
             "appending graphSpec to individual DMs",
```

### Comparing `daliuge-engine-4.0.0/dlg/manager/constants.py` & `daliuge-engine-4.0.1/dlg/manager/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/drop_manager.py` & `daliuge-engine-4.0.1/dlg/manager/drop_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/node_manager.py` & `daliuge-engine-4.0.1/dlg/manager/node_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/proc_daemon.py` & `daliuge-engine-4.0.1/dlg/manager/proc_daemon.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/replay.py` & `daliuge-engine-4.0.1/dlg/manager/replay.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/rest.py` & `daliuge-engine-4.0.1/dlg/manager/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,36 +74,32 @@
             if isinstance(res, (bytes, bottle.HTTPResponse)):
                 return res
 
             if res is not None:
                 bottle.response.content_type = "application/json"
                 # set CORS headers
                 origin = bottle.request.headers.raw("Origin")
-                if origin is None:
-                    origin = "http://localhost:8084"
-                elif not re.match(
-                    r"http://((localhost)|(127.0.0.1)):80[0-9][0-9]", origin
+                logger.debug("CORS request comming from: %s", origin)
+                if origin is None or re.match(
+                    r"http://dlg-trans.local:80[0-9][0-9]", origin
                 ):
+                    origin = "http://dlg-trans.local:8084"
+                elif re.match(r"http://((localhost)|(127.0.0.1)):80[0-9][0-9]", origin):
                     origin = "http://localhost:8084"
                 bottle.response.headers["Access-Control-Allow-Origin"] = origin
-                bottle.response.headers[
-                    "Access-Control-Allow-Credentials"
-                ] = "true"
-                bottle.response.headers[
-                    "Access-Control-Allow-Methods"
-                ] = "GET, POST, PUT, OPTIONS"
-                bottle.response.headers[
-                    "Access-Control-Allow-Headers"
-                ] = "Origin, Accept, Content-Type, Content-Encoding, X-Requested-With, X-CSRF-Token"
-            jres = (
-                json.dumps(res) if res else json.dumps({"Status": "Success"})
-            )
-            logger.debug(
-                "Bottle sending back result: %s", jres[: min(len(jres), 80)]
-            )
+                bottle.response.headers["Access-Control-Allow-Credentials"] = "true"
+                bottle.response.headers["Access-Control-Allow-Methods"] = (
+                    "GET, POST, PUT, OPTIONS"
+                )
+                bottle.response.headers["Access-Control-Allow-Headers"] = (
+                    "Origin, Accept, Content-Type, Content-Encoding, X-Requested-With, X-CSRF-Token"
+                )
+                logger.debug("CORS headers set to allow from: %s", origin)
+            jres = json.dumps(res) if res else json.dumps({"Status": "Success"})
+            logger.debug("Bottle sending back result: %s", jres[: min(len(jres), 80)])
             return json.dumps(res)
         except Exception as e:
             logger.exception("Error while fulfilling request")
 
             status, eargs = 500, ()
             if isinstance(e, NotImplementedError):
                 status, eargs = 501, e.args
@@ -162,32 +158,22 @@
 
         # Mappings
         app = self.app
         app.get("/api/submission_method", callback=self.submit_methods)
         app.post("/api/stop", callback=self.stop_manager)
         app.post("/api/sessions", callback=self.createSession)
         app.get("/api/sessions", callback=self.getSessions)
-        app.get(
-            "/api/sessions/<sessionId>", callback=self.getSessionInformation
-        )
+        app.get("/api/sessions/<sessionId>", callback=self.getSessionInformation)
         app.delete("/api/sessions/<sessionId>", callback=self.destroySession)
         app.get("/api/sessions/<sessionId>/logs", callback=self.getLogFile)
-        app.get(
-            "/api/sessions/<sessionId>/status", callback=self.getSessionStatus
-        )
-        app.post(
-            "/api/sessions/<sessionId>/deploy", callback=self.deploySession
-        )
-        app.post(
-            "/api/sessions/<sessionId>/cancel", callback=self.cancelSession
-        )
+        app.get("/api/sessions/<sessionId>/status", callback=self.getSessionStatus)
+        app.post("/api/sessions/<sessionId>/deploy", callback=self.deploySession)
+        app.post("/api/sessions/<sessionId>/cancel", callback=self.cancelSession)
         app.get("/api/sessions/<sessionId>/graph", callback=self.getGraph)
-        app.get(
-            "/api/sessions/<sessionId>/graph/size", callback=self.getGraphSize
-        )
+        app.get("/api/sessions/<sessionId>/graph/size", callback=self.getGraphSize)
         app.get(
             "/api/sessions/<sessionId>/graph/status",
             callback=self.getGraphStatus,
         )
         app.post(
             "/api/sessions/<sessionId>/graph/append",
             callback=self.addGraphParts,
@@ -197,17 +183,15 @@
             callback=self.getSessionReproData,
         )
         app.get(
             "/api/sessions/<sessionId>/repro/status",
             callback=self.getSessionReproStatus,
         )
 
-        app.route(
-            "/api/sessions", method="OPTIONS", callback=self.acceptPreflight
-        )
+        app.route("/api/sessions", method="OPTIONS", callback=self.acceptPreflight)
         app.route(
             "/api/sessions/<sessionId>/graph/append",
             method="OPTIONS",
             callback=self.acceptPreflight2,
         )
 
         # The non-REST mappings that serve HTML-related content
@@ -222,17 +206,15 @@
         Methods through which subclasses can initialize other mappings on top of
         the default ones and perform other DataManager-specific actions.
         The default implementation does nothing.
         """
 
     @daliuge_aware
     def submit_methods(self):
-        return {
-            "methods": [DeploymentMethods.BROWSER, DeploymentMethods.SERVER]
-        }
+        return {"methods": [DeploymentMethods.BROWSER, DeploymentMethods.SERVER]}
 
     def _stop_manager(self):
         self.dm.shutdown()
         self.stop()
         logger.info(
             "Thanks for using our %s, come back again :-)",
             self.dm.__class__.__name__,
@@ -404,17 +386,15 @@
             "/api/sessions/<sessionId>/graph/link",
             callback=self.linkGraphParts,
         )
         app.post(
             "/api/sessions/<sessionId>/subscriptions",
             callback=self.add_node_subscriptions,
         )
-        app.post(
-            "/api/sessions/<sessionId>/trigger", callback=self.trigger_drops
-        )
+        app.post("/api/sessions/<sessionId>/trigger", callback=self.trigger_drops)
         # The non-REST mappings that serve HTML-related content
         app.get("/", callback=self.visualizeDM)
         app.get("/api/shutdown", callback=self.shutdown_node_manager)
 
     @daliuge_aware
     def shutdown_node_manager(self):
         logger.debug("Shutting down node manager")
@@ -613,17 +593,15 @@
     # ===========================================================================
     # non-REST methods
     # ===========================================================================
     def visualizeDIM(self):
         tpl = file_as_string("web/dim.html")
         urlparts = bottle.request.urlparts
         selectedNode = (
-            bottle.request.params["node"]
-            if "node" in bottle.request.params
-            else ""
+            bottle.request.params["node"] if "node" in bottle.request.params else ""
         )
         serverUrl = urlparts.scheme + "://" + urlparts.netloc
         return bottle.template(
             tpl,
             dmType=self.dm.__class__.__name__,
             dmPort=self.dm.dmPort,
             serverUrl=serverUrl,
@@ -694,30 +672,26 @@
         with RestClient(host=host, port=port, timeout=10) as c:
             return json.loads(c._POST("/managers/node/stop").read())
 
     @daliuge_aware
     def addNM(self, host, node):
         port = constants.ISLAND_DEFAULT_REST_PORT
         logger.debug("Adding NM %s to DIM %s", node, host)
-        with RestClient(
-            host=host, port=port, timeout=10, url_prefix="/api"
-        ) as c:
+        with RestClient(host=host, port=port, timeout=10, url_prefix="/api") as c:
             return json.loads(
                 c._POST(
                     f"/node/{node}",
                 ).read()
             )
 
     @daliuge_aware
     def removeNM(self, host, node):
         port = constants.ISLAND_DEFAULT_REST_PORT
         logger.debug("Removing NM %s from DIM %s", node, host)
-        with RestClient(
-            host=host, port=port, timeout=10, url_prefix="/api"
-        ) as c:
+        with RestClient(host=host, port=port, timeout=10, url_prefix="/api") as c:
             return json.loads(c._DELETE(f"/node/{node}").read())
 
     @daliuge_aware
     def getNMInfo(self, host):
         port = constants.DAEMON_DEFAULT_REST_PORT
         logger.debug("Sending request %s:%s/managers/node", host, port)
         with RestClient(host=host, port=port, timeout=10) as c:
```

### Comparing `daliuge-engine-4.0.0/dlg/manager/session.py` & `daliuge-engine-4.0.1/dlg/manager/session.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/shared_memory_manager.py` & `daliuge-engine-4.0.1/dlg/manager/shared_memory_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/LICENSE` & `daliuge-engine-4.0.1/dlg/manager/web/LICENSE`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/dim.html` & `daliuge-engine-4.0.1/dlg/manager/web/dim.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,153 @@
 <!doctype html>
 
 <head>
-	<meta charset="utf-8">
-	<title>{{dmType}}</title>
-	<link rel="shortcut icon" type="image/svg" href="static/icons/liuFavIcon.svg"/>
-	<script src="/static/js/d3/d3.v5.min.js"></script>
-	<script src="/static/js/dm.js"></script>
-	<script src="/static/js/jquery-3.6.0.min.js"></script>
-	<script src="/static/js/bootstrap.bundle.min.js"></script>
-	<script src="/static/js/bootbox.min.js"></script>
-	<link href="/static/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
-	<link  href="/static/css/dm.css" rel="stylesheet" type="text/css"/>
-	<link  href="/static/css/progressBar.css" rel="stylesheet" type="text/css"/>
-	<style>
-		@import "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.4.0/css/font-awesome.css";
-	</style>
+    <meta charset="utf-8">
+    <title>{{dmType}}</title>
+    <link rel="shortcut icon" type="image/svg" href="static/icons/liuFavIcon.svg" />
+    <script src="/static/js/d3/d3.v5.min.js"></script>
+    <script src="/static/js/dm.js"></script>
+    <script src="/static/js/jquery-3.6.0.min.js"></script>
+    <script src="/static/js/bootstrap.bundle.min.js"></script>
+    <script src="/static/js/bootbox.min.js"></script>
+    <link href="/static/css/bootstrap.min.css" rel="stylesheet" type="text/css" />
+    <link href="/static/css/dm.css" rel="stylesheet" type="text/css" />
+    <link href="/static/css/progressBar.css" rel="stylesheet" type="text/css" />
+    <style>
+        @import "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.4.0/css/font-awesome.css";
+    </style>
 </head>
 
 <body>
-	<!-- custom bootstrap navbar -->
-	<nav class="navbar fixed-top navbar-expand-lg navbar-dark" style="background-color: #004085;">
-		<!-- Navbar content -->
-		<a href="/" class="navbar-brand inactiveLink">
-			<object data="/static/icons/liu.svg" type="image/svg+xml" width="30" height="30" class="d-inline-block align-top" alt="LiuIcon"></object>
-			<img src="/static/icons/engine.svg" width="auto" height="30" class="d-inline-block align-top" alt="EngineIcon">
-			<span>{{dmType}}</span>
-		</a>
-		<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
-			<span class="navbar-toggler-icon"></span>
-		</button>
-		<div class="collapse navbar-collapse" id="navbarNav">
-			<ul class="nav navbar-nav navbar-center">
+    <!-- custom bootstrap navbar -->
+    <nav class="navbar fixed-top navbar-expand-lg navbar-dark" style="background-color: #004085;">
+        <!-- Navbar content -->
+        <a href="/" class="navbar-brand inactiveLink">
+            <object data="/static/icons/liu.svg" type="image/svg+xml" width="30" height="30"
+                class="d-inline-block align-top" alt="LiuIcon"></object>
+            <img src="/static/icons/engine.svg" width="auto" height="30" class="d-inline-block align-top"
+                alt="EngineIcon">
+            <span>{{dmType}}</span>
+        </a>
+        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
+            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
+            <span class="navbar-toggler-icon"></span>
+        </button>
+        <div class="collapse navbar-collapse" id="navbarNav">
+            <ul class="nav navbar-nav navbar-center">
+            </ul>
+            <ul class="nav navbar-nav  ml-auto">
             </ul>
-			<ul class="nav navbar-nav  ml-auto">
-			</ul>
-		</div>
-	</nav>
-	<div id="graphNameWrapper">
+        </div>
+    </nav>
+    <div id="graphNameWrapper">
         <li id="islandDisplay"></li>
         <li id="nodeDisplay"></li>
     </div>
-	<div id="dimContentWrapper" class="container">
-    <div id="sessions">
-        <h4>Sessions</h4>
-        <table class="table table-striped" id="sessionsTable">
-            <thead>
-            <tr>
-                <th>Session ID</th>
-                <th>State</th>
-                <th># Drops</th>
-                <th>Details</th>
-            <th></th>
-					</tr>
-            </thead>
-            <tbody>
-            </tbody>
-        </table>
-        <button class="btn btn-secondary" id="addSessionBtn" type="button"><span class="fa fa-plus"></span>
-            Add Session
-        </button>
-        <button class="btn btn-secondary" id="refreshSessionListBtn" type="button"><span
-                class="fa fa-refresh"></span> Refresh
-        </button>
-    </div>
+    <div id="dimContentWrapper" class="container">
+        <div id="sessions">
+            <h4>Sessions</h4>
+            <table class="table table-striped" id="sessionsTable">
+                <thead>
+                    <tr>
+                        <th>Session ID</th>
+                        <th>State</th>
+                        <th># Drops</th>
+                        <th>Details</th>
+                        <th></th>
+                    </tr>
+                </thead>
+                <tbody>
+                </tbody>
+            </table>
+            <button class="btn btn-secondary" id="addSessionBtn" type="button"><span class="fa fa-plus"></span>
+                Add Session
+            </button>
+            <button class="btn btn-secondary" id="refreshSessionListBtn" type="button"><span
+                    class="fa fa-refresh"></span> Refresh
+            </button>
+        </div>
+
+        <div id="nodes">
+            <h4>Nodes</h4>
+            <table class="table table-striped" id="nodesTable">
+                <thead>
+                    <tr>
+                        <th>Node</th>
+                        <th>Details</th>
+                    </tr>
+                </thead>
+                <tbody></tbody>
+            </table>
+            <button class="btn btn-secondary" id="refreshNodeListBtn" type="button"><span class="fa fa-refresh"></span>
+                Refresh
+            </button>
+        </div>
 
-    <div id="nodes">
-        <h4>Nodes</h4>
-        <table class="table table-striped" id="nodesTable">
-            <thead>
-            <tr>
-                <th>Node</th>
-                <th>Details</th>
-            </tr>
-            </thead>
-            <tbody></tbody>
-        </table>
-        <button class="btn btn-secondary" id="refreshNodeListBtn" type="button"><span
-                class="fa fa-refresh"></span> Refresh
-        </button>
     </div>
 
-</div>
+    <script type="text/javascript">
 
-	<script type="text/javascript">
+        var selectedNode = '{{selectedNode}}';
+        if (selectedNode == '') {
+            selectedNode = null;
+        }
+        var serverUrl = '{{serverUrl}}';
+        var dmPort = {{ dmPort }}
+        var nodes = {{!nodes}}
+
+        var refreshSessionListBtn = d3.select('#refreshSessionListBtn');
+        var addSessionBtn = d3.select('#addSessionBtn');
+        var sessionsTbodyEl = d3.select('#sessionsTable tbody');
+
+        var serverIP = serverUrl.split("//").pop().split(":").shift();// Show/hide parts of the UI depending on whether we're zooming in or not
+
+        // into a specific node
+        if (selectedNode) {
+            d3.select('#nodes').remove();
+            d3.select('#islandDisplay').html("<a href=" + serverUrl + ">DIM: " + serverIP + "</a>");
+            d3.select('#nodeDisplay').html("<a href=" + serverUrl + "/?node=" + selectedNode + "&dim_url=" + serverUrl + ">Node: " + selectedNode + "</a>");
+        } else {
+            d3.select('#zoom-notice').remove();
+            d3.select('#nodeDisplay').remove();
+            d3.select('#islandDisplay').html("<a href=" + serverUrl + ">DIM: " + serverIP + "</a>");
+        }
+
+        // Animated filling of DropManagers and Nodes table
+        function fillTable(selector, data, href_function, nodeHref) {
+            data.sort();
+            var rows = d3.select(selector).selectAll('tr').data(data);
+            // rows.enter().append('tr');
+            var newRow = rows.enter().append('tr');
+            var nodeName = String;
+            newRow.style('opacity', 0.0).transition().delay(0).duration(500).style('opacity', 1.0)
+            newRow.append('td').classed('id', true)
+                .append('a').attr("href", nodeHref).text(String);
+            newRow.append('td').classed('details', true)
+                .append('a').attr('href', href_function)
+                .append('span').classed('fa fa-share', true);
+        }
+        if (!selectedNode) {
+            fillTable('#nodesTable tbody', nodes, function (n) { return '?node=' + n + "&dim_url=" + serverUrl; }, function (n) { return "http://" + n + "?dim_url=" + serverUrl });
+        }
+
+        // Listeners for the two session-related buttons
+        if (!selectedNode) {
+            addSessionBtn.on('click', function () {
+                promptNewSession(serverUrl, sessionsTbodyEl, refreshSessionListBtn);
+            });
+        } else {
+            addSessionBtn.remove()
+        }
+        refreshSessionListBtn.on('click', function () {
+            loadSessions(serverUrl, sessionsTbodyEl, refreshSessionListBtn, selectedNode);
+        });
 
-    var selectedNode = '{{selectedNode}}';
-    if (selectedNode == '') {
-        selectedNode = null;
-    }
-    var serverUrl = '{{serverUrl}}';
-    var dmPort = {{dmPort}}
-    var nodes = {{!nodes}}
-    
-    var refreshSessionListBtn = d3.select('#refreshSessionListBtn');
-    var addSessionBtn = d3.select('#addSessionBtn');
-    var sessionsTbodyEl = d3.select('#sessionsTable tbody');
-
-    var serverIP = serverUrl.split("//").pop().split(":").shift();// Show/hide parts of the UI depending on whether we're zooming in or not
-
-    // into a specific node
-    if (selectedNode) {
-        d3.select('#nodes').remove();
-        d3.select('#islandDisplay').html("<a href="+serverUrl+">DIM: " + serverIP+"</a>");
-		d3.select('#nodeDisplay').html("<a href="+serverUrl+"/?node="+selectedNode+"&dim_url="+serverUrl+">Node: " + selectedNode+"</a>");
-    } else {
-        d3.select('#zoom-notice').remove();
-        d3.select('#nodeDisplay').remove();
-        d3.select('#islandDisplay').html("<a href="+serverUrl+">DIM: " + serverIP+"</a>");
-	}
-
-	// Animated filling of DropManagers and Nodes table
-	function fillTable(selector, data, href_function, nodeHref) {
-		data.sort();
-		var rows = d3.select(selector).selectAll('tr').data(data);
-		// rows.enter().append('tr');
-		var newRow = rows.enter().append('tr');
-		var nodeName = String;
-		newRow.style('opacity', 0.0).transition().delay(0).duration(500).style('opacity',1.0)
-		newRow.append('td').classed('id', true)
-			.append('a').attr("href", nodeHref).text(String);
-		newRow.append('td').classed('details', true)
-			.append('a').attr('href', href_function)
-			.append('span').classed('fa fa-share', true);
-	}
-	if( !selectedNode ) {
-		fillTable('#nodesTable tbody', nodes, function(n) { return '?node=' + n+"&dim_url="+serverUrl; }, function(n){return "http://"+n+":8000"+"?dim_url="+serverUrl});
-	}
-
-    // Listeners for the two session-related buttons
-    if (!selectedNode) {
-        addSessionBtn.on('click', function () {
-            promptNewSession(serverUrl, sessionsTbodyEl, refreshSessionListBtn);
+        //Start loading the list of sessions periodically
+        var loadSessionTimer = d3.timer(function () {
+            loadSessions(serverUrl, sessionsTbodyEl, refreshSessionListBtn, selectedNode, 5000);
+            loadSessionTimer.stop()
+            return;
         });
-    } else {
-        addSessionBtn.remove()
-    }
-    refreshSessionListBtn.on('click', function () {
-        loadSessions(serverUrl, sessionsTbodyEl, refreshSessionListBtn, selectedNode);
-    });
-
-    //Start loading the list of sessions periodically
-    var loadSessionTimer =d3.timer(function () {
-        loadSessions(serverUrl, sessionsTbodyEl, refreshSessionListBtn, selectedNode, 5000);
-        loadSessionTimer.stop()
-		return;
-    });
 
-	</script>
+    </script>
 </body>
```

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/dm.html` & `daliuge-engine-4.0.1/dlg/manager/web/dm.html`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/session.html` & `daliuge-engine-4.0.1/dlg/manager/web/session.html`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/css/bootstrap.min.css` & `daliuge-engine-4.0.1/dlg/manager/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/css/dm.css` & `daliuge-engine-4.0.1/dlg/manager/web/static/css/dm.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/css/progressBar.css` & `daliuge-engine-4.0.1/dlg/manager/web/static/css/progressBar.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/css/session.css` & `daliuge-engine-4.0.1/dlg/manager/web/static/css/session.css`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot` & `daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg` & `daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf` & `daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff` & `daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2` & `daliuge-engine-4.0.1/dlg/manager/web/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/icons/engine.svg` & `daliuge-engine-4.0.1/dlg/manager/web/static/icons/engine.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/icons/liu.svg` & `daliuge-engine-4.0.1/dlg/manager/web/static/icons/liu.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/icons/liuFavIcon.svg` & `daliuge-engine-4.0.1/dlg/manager/web/static/icons/liuFavIcon.svg`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/bootbox.min.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/bootbox.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/bootstrap.bundle.min.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/d3.v5.min.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/dagre-d3.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/dagre-d3.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/d3/dagre-d3.min.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/dm.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/dm.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/manager/web/static/js/jquery-3.6.0.min.js` & `daliuge-engine-4.0.1/dlg/manager/web/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/meta.py` & `daliuge-engine-4.0.1/dlg/meta.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/named_port_utils.py` & `daliuge-engine-4.0.1/dlg/named_port_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,34 @@
+import ast
+from enum import Enum
 import logging
 import collections
 from typing import Tuple
-import dlg.common as common
+from dlg import droputils, drop_loaders
 
 logger = logging.getLogger(__name__)
 
 
+class DropParser(Enum):
+    RAW = "raw"
+    PICKLE = "pickle"
+    EVAL = "eval"
+    NPY = "npy"
+    # JSON = "json"
+    PATH = "path"  # input only
+    DATAURL = "dataurl"  # input only
+
+
 def serialize_kwargs(keyargs, prefix="--", separator=" "):
     kwargs = []
     for name, value in iter(keyargs.items()):
         if prefix == "--" and len(name) == 1:
             kwargs += [f"-{name} {value}"]
         else:
-            kwargs += [
-                f"{prefix.strip()}{name.strip()}{separator}{str(value).strip()}"
-            ]
+            kwargs += [f"{prefix.strip()}{name.strip()}{separator}{str(value).strip()}"]
     logger.debug("kwargs after serialization: %s", kwargs)
     return kwargs
 
 
 def clean_applicationArgs(applicationArgs: dict) -> dict:
     """
     Removes arguments with None and False values, if not precious. This
@@ -74,25 +84,27 @@
 def identify_named_ports(
     port_dict: dict,
     posargs: list,
     pargsDict: dict,
     keyargs: dict,
     check_len: int = 0,
     mode: str = "inputs",
+    parser: callable = None,
 ) -> dict:
     """
     Checks port names for matches with arguments and returns mapped ports.
 
     Args:
         port_dict (dict): ports {uid:name,...}
         posargs (list): available positional arguments (will be modified)
         pargsDict (dict): mapped arguments (will be modified)
         keyargs (dict): keyword arguments
         check_len (int): number of of ports to be checked
         mode (str ["inputs"]): mode, used just for logging messages
+        parser (function): parser function for this port
 
     Returns:
         dict: port arguments
 
     Side effect:
         modifies pargsDict
     """
@@ -103,45 +115,50 @@
         port_dict,
         check_len,
     )
     logger.debug("Checking against keyargs: %s", keyargs)
     portargs = {}
     posargs = list(posargs)
     keys = list(port_dict.keys())
-    logger.debug("Checking ports: %s", keys)
+    logger.debug("Checking ports: %s against %s %s", keys, posargs, keyargs)
     for i in range(check_len):
         try:
             key = port_dict[keys[i]]["name"]
             value = port_dict[keys[i]]["path"]
         except KeyError:
             logger.debug("portDict: %s", port_dict)
             raise KeyError
         if value is None:
             value = ""  # make sure we are passing NULL drop events
         if key in posargs:
+            if parser:
+                logger.debug("Reading from port using %s", parser.__repr__())
+                value = parser(port_dict[keys[i]]["drop"])
             pargsDict.update({key: value})
-            # portargs.update({key: value})
             logger.debug("Using %s '%s' for parg %s", mode, value, key)
+            portargs.update({key: value})
             posargs.pop(posargs.index(key))
         elif key in keyargs:
+            if parser:
+                logger.debug("Reading from port using %s", parser.__repr__())
+                value = parser(port_dict[keys[i]]["drop"])
             # if not found in appArgs we don't put them into portargs either
-            portargs.update({key: value})
             # pargsDict.update({key: value})
-            logger.debug(
-                "Using %s of type %s for kwarg %s", mode, type(value), key
-            )
+            portargs.update({key: value})
+            logger.debug("Using %s of type %s for kwarg %s", mode, type(value), key)
             _ = keyargs.pop(key)  # remove from original arg list
         else:
             logger.debug(
                 "No matching argument found for %s key %s, %s, %s",
                 mode,
                 key,
                 keyargs,
                 posargs,
             )
+
     logger.debug("Returning kw mapped ports: %s", portargs)
     return portargs
 
 
 def check_ports_dict(ports: list) -> bool:
     """
     Checks whether all ports in ports list are of type dict. This is
@@ -164,59 +181,60 @@
     iitems: dict,
     oitems: dict,
     inport_names: dict,
     outport_names: dict,
     appArgs: dict,
     argumentPrefix: str = "--",
     separator: str = " ",
+    parser: callable = None,
 ) -> Tuple[str, str]:
     """
     Function attempts to identify CLI component arguments that match port names.
 
     Inputs:
         iitems: itemized input port dictionary
         oitems: itemized output port dictionary
         inport_names: dictionary of input port names (key: uid)
         outport_names: dictionary of output port names (key: uid)
         appArgs: dictionary of all arguments
         argumentPrefix: prefix for keyword arguments
         separator: character used between keyword and value
+        parser: reader function for ports
+
+
 
     Returns:
         tuple of serialized keyword arguments and positional arguments
     """
     logger.debug(
         "iitems: %s; inport_names: %s; outport_names: %s",
         iitems,
         inport_names,
         outport_names,
     )
     inputs_dict = collections.OrderedDict()
     for uid, drop in iitems:
-        inputs_dict[uid] = {"path": drop.path if hasattr(drop, "path") else ""}
+        inputs_dict[uid] = {
+            "drop": drop,
+            "path": drop.path if hasattr(drop, "path") else "",
+        }
 
     outputs_dict = collections.OrderedDict()
     for uid, drop in oitems:
-        outputs_dict[uid] = {
-            "path": drop.path if hasattr(drop, "path") else ""
-        }
+        outputs_dict[uid] = {"path": drop.path if hasattr(drop, "path") else ""}
     # logger.debug("appArgs: %s", appArgs)
     # get positional args
     posargs = [arg for arg in appArgs if appArgs[arg]["positional"]]
     # get kwargs
     keyargs = {
-        arg: appArgs[arg]["value"]
-        for arg in appArgs
-        if not appArgs[arg]["positional"]
+        arg: appArgs[arg]["value"] for arg in appArgs if not appArgs[arg]["positional"]
     }
     # we will need an ordered dict for all positional arguments
     # thus we create it here and fill it with values
-    portPosargsDict = collections.OrderedDict(
-        zip(posargs, [None] * len(posargs))
-    )
+    portPosargsDict = collections.OrderedDict(zip(posargs, [None] * len(posargs)))
     logger.debug(
         "posargs: %s; keyargs: %s, %s",
         posargs,
         keyargs,
         check_ports_dict(inport_names),
     )
     portkeyargs = {}
@@ -230,14 +248,15 @@
         ipkeyargs = identify_named_ports(
             inputs_dict,
             posargs,
             portPosargsDict,
             keyargs,
             check_len=len(iitems),
             mode="inputs",
+            parser=parser,
         )
         portkeyargs.update(ipkeyargs)
     else:
         for i in range(min(len(iitems), len(posargs))):
             portkeyargs.update({list(posargs)[i]: list(iitems)[i][1]})
 
     if check_ports_dict(outport_names):
@@ -264,24 +283,20 @@
         portPosargsDict,
         ipkeyargs,
         opkeyargs,
     )
     appArgs = clean_applicationArgs(appArgs)
     # get cleaned positional args
     posargs = {
-        arg: appArgs[arg]["value"]
-        for arg in appArgs
-        if appArgs[arg]["positional"]
+        arg: appArgs[arg]["value"] for arg in appArgs if appArgs[arg]["positional"]
     }
     logger.debug("posargs: %s", posargs)
     # get cleaned kwargs
     keyargs = {
-        arg: appArgs[arg]["value"]
-        for arg in appArgs
-        if not appArgs[arg]["positional"]
+        arg: appArgs[arg]["value"] for arg in appArgs if not appArgs[arg]["positional"]
     }
     for k, v in portkeyargs.items():
         if v not in [None, ""]:
             keyargs.update({k: v})
     for k, v in portPosargsDict.items():
         logger.debug("port posarg %s has value %s", k, v)
         # logger.debug("default posarg %s has value %s", k, posargs[k])
@@ -294,11 +309,38 @@
     keyargs = (
         serialize_kwargs(keyargs, prefix=argumentPrefix, separator=separator)
         if len(keyargs) > 0
         else [""]
     )
     pargs = list(posargs.values())
     pargs = [""] if len(pargs) == 0 or None in pargs else pargs
-    logger.debug(
-        "After port replacement: pargs: %s; keyargs: %s", pargs, keyargs
-    )
+    logger.debug("After port replacement: pargs: %s; keyargs: %s", pargs, keyargs)
     return keyargs, pargs
+
+
+def get_port_reader_function(input_parser: DropParser):
+    """
+    Return the function used to read input from a named port
+    """
+    # Inputs are un-pickled and treated as the arguments of the function
+    # Their order must be preserved, so we use an OrderedDict
+    if input_parser is DropParser.PICKLE:
+        # all_contents = lambda x: pickle.loads(droputils.allDropContents(x))
+        reader = drop_loaders.load_pickle
+    elif input_parser is DropParser.EVAL:
+
+        def optionalEval(x):
+            # Null and Empty Drops will return an empty byte string
+            # which should propogate back to None
+            content: str = droputils.allDropContents(x).decode("utf-8")
+            return ast.literal_eval(content) if len(content) > 0 else None
+
+        reader = optionalEval
+    elif input_parser is DropParser.NPY:
+        reader = drop_loaders.load_npy
+    elif input_parser is DropParser.PATH:
+        reader = lambda x: x.path
+    elif input_parser is DropParser.DATAURL:
+        reader = lambda x: x.dataurl
+    else:
+        raise ValueError(input_parser.__repr__())
+    return reader
```

### Comparing `daliuge-engine-4.0.0/dlg/ngaslite.py` & `daliuge-engine-4.0.1/dlg/ngaslite.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/nm_dim_assigner.py` & `daliuge-engine-4.0.1/dlg/nm_dim_assigner.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/passwd.template` & `daliuge-engine-4.0.1/dlg/passwd.template`

 * *Files 2% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
 list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
 irc:x:39:39:ircd:/var/run/ircd:/usr/sbin/nologin
 gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
 nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
 _apt:x:100:65534::/nonexistent:/usr/sbin/nologin
 messagebus:x:101:102::/nonexistent:/usr/sbin/nologin
+avahi:x:102:103:Avahi mDNS daemon,,,:/var/run/avahi-daemon:/usr/sbin/nologin
```

### Comparing `daliuge-engine-4.0.0/dlg/prepareUser.py` & `daliuge-engine-4.0.1/dlg/prepareUser.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/process.py` & `daliuge-engine-4.0.1/dlg/process.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/remote.py` & `daliuge-engine-4.0.1/dlg/remote.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/restserver.py` & `daliuge-engine-4.0.1/dlg/restserver.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/rpc.py` & `daliuge-engine-4.0.1/dlg/rpc.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/runtime/__init__.py` & `daliuge-engine-4.0.1/dlg/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/runtime/tool_commands.py` & `daliuge-engine-4.0.1/dlg/runtime/tool_commands.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/shared_memory.py` & `daliuge-engine-4.0.1/dlg/shared_memory.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/dlg/testutils.py` & `daliuge-engine-4.0.1/dlg/testutils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile` & `daliuge-engine-4.0.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile.casa` & `daliuge-engine-4.0.1/docker/Dockerfile.casa`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile.dev` & `daliuge-engine-4.0.1/docker/Dockerfile.dev`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ARG VCS_TAG
 ARG USER
 # We need the base image we build with the other Dockerfile
 FROM icrar/daliuge-common:${VCS_TAG:-latest}
 
 # RUN sudo apt-get update && sudo DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata \
 #     gcc g++ gdb casacore-dev clang-tidy-10 clang-tidy libboost1.71-all-dev libgsl-dev
+RUN service dbus start && service avahi-daemon start && avahi-set-host-name dlg-engine
 RUN useradd --create-home awicenec
 COPY / /daliuge
 RUN . /dlg/bin/activate && pip install --upgrade pip && pip install wheel && cd /daliuge && \
     pip install . 
 
 EXPOSE 9000
 EXPOSE 5555
```

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile.devall` & `daliuge-engine-4.0.1/docker/Dockerfile.devall`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile.ray` & `daliuge-engine-4.0.1/docker/Dockerfile.ray`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/docker/Dockerfile_incontext` & `daliuge-engine-4.0.1/docker/Dockerfile_incontext`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/etc/init-scripts/dlg-dim` & `daliuge-engine-4.0.1/etc/init-scripts/dlg-dim`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/etc/init-scripts/dlg-nm` & `daliuge-engine-4.0.1/etc/init-scripts/dlg-nm`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/etc/init-scripts/dlg.options` & `daliuge-engine-4.0.1/etc/init-scripts/dlg.options`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/headers/dlg_app.h` & `daliuge-engine-4.0.1/headers/dlg_app.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/headers/dlg_app2.h` & `daliuge-engine-4.0.1/headers/dlg_app2.h`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/run_engine.sh` & `daliuge-engine-4.0.1/run_engine.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env bash
 DOCKER_OPTS="\
 --shm-size=2g --ipc=shareable \
 --rm \
 $([[ $(nvidia-docker version) ]] && echo '--gpus=all' || echo '') \
 --name daliuge-engine \
+-h dlg-engine \
 -v /var/run/docker.sock:/var/run/docker.sock \
 -p 5555:5555 -p 6666:6666 \
 -p 8000:8000 -p 8001:8001 \
 -p 8002:8002 -p 9000:9000 \
 --user $(id -u):$(id -g) \
 " 
 common_prep ()
@@ -39,61 +40,67 @@
             echo "Deployment version requires access to a directory /var/dlg_home, but that does not exist!"
             echo "Please either create and grant access to $USER or build and run the development version."
         else
             common_prep
             echo "Running Engine deployment version in background..."
             echo "docker run -td "${DOCKER_OPTS}"  icrar/daliuge-engine:${VCS_TAG}"
             docker run -td ${DOCKER_OPTS}  icrar/daliuge-engine:${VCS_TAG}
-            echo "Engine IP address: "`docker exec daliuge-engine sh -c "hostname --ip-address"`
-            exit 0
+            sleep 3
+            ENGINE_NAME=`docker exec daliuge-engine sh -c "hostname"`
+            ENGINE_IP=`docker exec daliuge-engine sh -c "hostname --ip-address"`
+            # exit 0
         fi;;
     "dev")
         export DLG_ROOT="$HOME/dlg"
         common_prep
         echo "Running Engine development version in background..."
         echo "docker run -td ${DOCKER_OPTS}  icrar/daliuge-engine:${C_TAG}"
         docker run -td ${DOCKER_OPTS}  icrar/daliuge-engine:${C_TAG}
         sleep 3
+        docker exec -u root daliuge-engine bash -c "service avahi-daemon stop > /dev/null 2>&1 && service dbus restart > /dev/null 2>&1 && service avahi-daemon start > /dev/null 2>&1"
+        ENGINE_NAME=`docker exec daliuge-engine sh -c "hostname"`
         ENGINE_IP=`docker exec daliuge-engine sh -c "hostname --ip-address"`
         curl -X POST http://${ENGINE_IP}:9000/managers/island/start
-        echo
-        echo "Engine IP address: ${ENGINE_IP}"
-        exit 0;;
+        curl -X POST http://${ENGINE_IP}:8001/api/node/dlg-engine.local;;
+        # exit 0;;
     "casa")
         DLG_ROOT="/tmp/dlg"
         export VCS_TAG=`git rev-parse --abbrev-ref HEAD | tr '[:upper:]' '[:lower:]'`
         echo "Running Engine development version in background..."
         common_prep
         CONTAINER_NM="icrar/daliuge-engine:${VCS_TAG}-casa"
         echo "docker run -td ${DOCKER_OPTS}  ${CONTAINER_NM}"
         docker run -td ${DOCKER_OPTS}  ${CONTAINER_NM}
         sleep 3
+        ENGINE_NAME=`docker exec daliuge-engine sh -c "hostname"`
         ENGINE_IP=`docker exec daliuge-engine sh -c "hostname --ip-address"`
-        curl -X POST http://${ENGIONE_IP}:9000/managers/island/start
-        echo
-        echo "Engine IP address: ${ENGINE_IP}"
-        exit 0;;
+        curl -X POST http://${ENGIONE_IP}:9000/managers/island/start;;
+        # exit 0;;
     "slim")
         export DLG_ROOT="$HOME/dlg"
         common_prep
         echo "Running Engine development version in background..."
         echo "docker run -td ${DOCKER_OPTS}  icrar/daliuge-engine:${VCS_TAG}"
         docker run -td ${DOCKER_OPTS}  icrar/daliuge-engine:${VCS_TAG}
         sleep 3
+        ENGINE_NAME=`docker exec daliuge-engine sh -c "hostname"`
         ENGINE_IP=`docker exec daliuge-engine sh -c "hostname --ip-address"`
-        curl -X POST http://${ENGINE_IP}:9000/managers/island/start
-        echo
-        echo "Engine IP address: ${ENGINE_IP}"
-        exit 0;;
+        curl -X POST http://${ENGINE_IP}:9000/managers/island/start;;
+        # exit 0;;
     "local")
         common_prep
         echo "Starting managers locally in background.."
         dlg nm -vvd -H 0.0.0.0 --dlg-path=$DLG_ROOT --dlm-cleanup-period=10
         dlg dim -vvd -H 0.0.0.0 -N localhost
         echo
         echo "Use any of the following URLs to access the DIM:"
         python -c "from dlg.utils import get_local_ip_addr; print([f'http://{addr}:8001' for addr,name in get_local_ip_addr() if not name.startswith('docker')])"
-        echo "Log files can be found in ${DLG_ROOT}/log";;
+        echo "Log files can be found in ${DLG_ROOT}/log"
+        ENGINE_NAME="localhost"
+        ENGINE_IP=`hostname --ip-address`;;
     *)
         echo "Usage run_engine.sh <dep|dev|slim|local>"
         exit 0;;
 esac
+echo
+echo "Engine NAME/IP address: ${ENGINE_NAME}/${ENGINE_IP}"
+
```

### Comparing `daliuge-engine-4.0.0/setup.py` & `daliuge-engine-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
 MAJOR = 4
 MINOR = 0
-PATCH = 0
+PATCH = 1
 RELEASE = True
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/runtime/version.py"
 PTH_FILE = "lib64_dist.pth"
 
 
 def get_git_version():
```

### Comparing `daliuge-engine-4.0.0/test/__init__.py` & `daliuge-engine-4.0.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/__init__.py` & `daliuge-engine-4.0.1/test/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/data/test_ms.tar.gz` & `daliuge-engine-4.0.1/test/apps/data/test_ms.tar.gz`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/dynlib_example.c` & `daliuge-engine-4.0.1/test/apps/dynlib_example.c`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/dynlib_example2.c` & `daliuge-engine-4.0.1/test/apps/dynlib_example2.c`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/setp_up.py` & `daliuge-engine-4.0.1/test/apps/setp_up.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_bash.py` & `daliuge-engine-4.0.1/test/apps/test_bash.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_crc.py` & `daliuge-engine-4.0.1/test/apps/test_crc.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_docker.py` & `daliuge-engine-4.0.1/test/apps/test_docker.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_dynlib.py` & `daliuge-engine-4.0.1/test/apps/test_dynlib.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_dynlib2.py` & `daliuge-engine-4.0.1/test/apps/test_dynlib2.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_pyfunc.py` & `daliuge-engine-4.0.1/test/apps/test_pyfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import os
 import pickle
 import random
 import unittest
 import numpy
 
 from dlg import droputils, drop_loaders
+from dlg.named_port_utils import DropParser
 from dlg.apps import pyfunc
 from dlg.apps.simple_functions import string2json
 from dlg.ddap_protocol import DROPStates, DROPRel, DROPLinkType
 from dlg.data.drops.memory import InMemoryDROP
 from dlg.droputils import DROPWaiterCtx
 from dlg.exceptions import InvalidDropException
 
@@ -150,16 +151,16 @@
         output_data = [2, 2] if output_data is None else output_data
 
         a = InMemoryDROP("a", "a")
         b = _PyFuncApp(
             "b",
             "b",
             f,
-            input_parser=pyfunc.DropParser.EVAL,
-            output_parser=pyfunc.DropParser.EVAL,
+            input_parser=DropParser.EVAL,
+            output_parser=DropParser.EVAL,
         )
         c = InMemoryDROP("c", "c")
 
         b.addInput(a)
         b.addOutput(c)
 
         with DROPWaiterCtx(self, c, 5):
@@ -199,16 +200,16 @@
         output_data = numpy.ones([2, 2]) if output_data is None else output_data
 
         a = InMemoryDROP("a", "a")
         b = _PyFuncApp(
             "b",
             "b",
             f,
-            input_parser=pyfunc.DropParser.NPY,
-            output_parser=pyfunc.DropParser.NPY,
+            input_parser=DropParser.NPY,
+            output_parser=DropParser.NPY,
         )
         c = InMemoryDROP("c", "c")
 
         b.addInput(a)
         b.addOutput(c)
 
         with DROPWaiterCtx(self, c, 5):
```

### Comparing `daliuge-engine-4.0.0/test/apps/test_simple.py` & `daliuge-engine-4.0.1/test/apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/apps/test_socket.py` & `daliuge-engine-4.0.1/test/apps/test_socket.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/deploy/__init__.py` & `daliuge-engine-4.0.1/test/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/deploy/test_common.py` & `daliuge-engine-4.0.1/test/deploy/test_common.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/deploy/test_helm_deploy.py` & `daliuge-engine-4.0.1/test/deploy/test_helm_deploy.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/deploy/test_slurm_utils.py` & `daliuge-engine-4.0.1/test/deploy/test_slurm_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/ArrayLoopPG.graph` & `daliuge-engine-4.0.1/test/graphs/ArrayLoopPG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/HelloWorld_simplePG.graph` & `daliuge-engine-4.0.1/test/graphs/HelloWorld_simplePG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/HelloWorld_universePG.graph` & `daliuge-engine-4.0.1/test/graphs/HelloWorld_universePG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/__init__.py` & `daliuge-engine-4.0.1/test/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/appTestPG_namedPorts.graph` & `daliuge-engine-4.0.1/test/graphs/appTestPG_namedPorts.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/application_args.graph` & `daliuge-engine-4.0.1/test/graphs/application_args.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/compilePG.graph` & `daliuge-engine-4.0.1/test/graphs/compilePG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/complex.js` & `daliuge-engine-4.0.1/test/graphs/complex.js`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/ddTest.graph` & `daliuge-engine-4.0.1/test/graphs/ddTest.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/funcTestPG.graph` & `daliuge-engine-4.0.1/test/graphs/funcTestPG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/funcTestPG_namedPorts.graph` & `daliuge-engine-4.0.1/test/graphs/funcTestPG_namedPorts.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/pyfunc_glob_testPG.graph` & `daliuge-engine-4.0.1/test/graphs/pyfunc_glob_testPG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/graphs/test_graphExecution.py` & `daliuge-engine-4.0.1/test/graphs/test_graphExecution.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/__init__.py` & `daliuge-engine-4.0.1/test/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/chiles/__init__.py` & `daliuge-engine-4.0.1/test/integrate/chiles/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/chiles/chilesdo.py` & `daliuge-engine-4.0.1/test/integrate/chiles/chilesdo.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/chiles/chilesdoapp.py` & `daliuge-engine-4.0.1/test/integrate/chiles/chilesdoapp.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/chiles/chilesdospec.py` & `daliuge-engine-4.0.1/test/integrate/chiles/chilesdospec.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/chiles/chilesdospec_docker.py` & `daliuge-engine-4.0.1/test/integrate/chiles/chilesdospec_docker.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/example_split.py` & `daliuge-engine-4.0.1/test/integrate/example_split.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/freq_split.py` & `daliuge-engine-4.0.1/test/integrate/freq_split.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/msconverter/makefile` & `daliuge-engine-4.0.1/test/integrate/msconverter/makefile`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/integrate/msconverter/ms_checker.cc` & `daliuge-engine-4.0.1/test/integrate/msconverter/ms_checker.cc`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/lifecycle/__init__.py` & `daliuge-engine-4.0.1/test/lifecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/lifecycle/test_dlm.py` & `daliuge-engine-4.0.1/test/lifecycle/test_dlm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/lifecycle/test_registry.py` & `daliuge-engine-4.0.1/test/lifecycle/test_registry.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/__init__.py` & `daliuge-engine-4.0.1/test/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_daemon.py` & `daliuge-engine-4.0.1/test/manager/test_daemon.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_dim.py` & `daliuge-engine-4.0.1/test/manager/test_dim.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_dm.py` & `daliuge-engine-4.0.1/test/manager/test_dm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_mm.py` & `daliuge-engine-4.0.1/test/manager/test_mm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_rest.py` & `daliuge-engine-4.0.1/test/manager/test_rest.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_scalability.py` & `daliuge-engine-4.0.1/test/manager/test_scalability.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/test_smm.py` & `daliuge-engine-4.0.1/test/manager/test_smm.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/manager/testutils.py` & `daliuge-engine-4.0.1/test/manager/testutils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/memoryUsage.py` & `daliuge-engine-4.0.1/test/memoryUsage.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/testSingle.graph` & `daliuge-engine-4.0.1/test/reproducibility/testSingle.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/test_drophash.py` & `daliuge-engine-4.0.1/test/reproducibility/test_drophash.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/test_lg_blockdag.py` & `daliuge-engine-4.0.1/test/reproducibility/test_lg_blockdag.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/test_pg_blockdag.py` & `daliuge-engine-4.0.1/test/reproducibility/test_pg_blockdag.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/test_toposort.py` & `daliuge-engine-4.0.1/test/reproducibility/test_toposort.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/computationSandwich.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/computationSandwich.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataFan.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataFan.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataFunnel.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataFunnel.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/dataSandwich.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/dataSandwich.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testCycle.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testCycle.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testEmpty.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testEmpty.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testNotDAG.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testNotDAG.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testSingle.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testSingle.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoEnd.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoEnd.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoLines.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoLines.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/reproducibility/topoGraphs/testTwoStart.graph` & `daliuge-engine-4.0.1/test/reproducibility/topoGraphs/testTwoStart.graph`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_JsonDrop.py` & `daliuge-engine-4.0.1/test/test_JsonDrop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_ParameterSetDROP.py` & `daliuge-engine-4.0.1/test/test_ParameterSetDROP.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_S3Drop.py` & `daliuge-engine-4.0.1/test/test_S3Drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_dask_emulation.py` & `daliuge-engine-4.0.1/test/test_dask_emulation.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_drop.py` & `daliuge-engine-4.0.1/test/test_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_droputils.py` & `daliuge-engine-4.0.1/test/test_droputils.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_environmentvars.py` & `daliuge-engine-4.0.1/test/test_environmentvars.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_event.py` & `daliuge-engine-4.0.1/test/test_event.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_graph_loader.py` & `daliuge-engine-4.0.1/test/test_graph_loader.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_input_fired_app_drop.py` & `daliuge-engine-4.0.1/test/test_input_fired_app_drop.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_io.py` & `daliuge-engine-4.0.1/test/test_io.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_session.py` & `daliuge-engine-4.0.1/test/test_session.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_shared_memory.py` & `daliuge-engine-4.0.1/test/test_shared_memory.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_tool.py` & `daliuge-engine-4.0.1/test/test_tool.py`

 * *Files identical despite different names*

### Comparing `daliuge-engine-4.0.0/test/test_utils.py` & `daliuge-engine-4.0.1/test/test_utils.py`

 * *Files identical despite different names*

