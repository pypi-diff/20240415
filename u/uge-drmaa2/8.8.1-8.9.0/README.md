# Comparing `tmp/uge-drmaa2-8.8.1.tar.gz` & `tmp/uge-drmaa2-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uge-drmaa2-8.8.1.tar", last modified: Mon Sep 25 08:12:02 2023, max compression
+gzip compressed data, was "dist/uge-drmaa2-8.9.0.tar", last modified: Sun Apr 14 10:20:49 2024, max compression
```

## Comparing `uge-drmaa2-8.8.1.tar` & `uge-drmaa2-8.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/drmaa2/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5786 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/reservation.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4343 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/exception_mapper.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15156 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_object_descriptors.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4856 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/notification.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1633 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_slot_info_list_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3695 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/reservation_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4595 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/reservation_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2817 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/log_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22185 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/job_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5392 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/machine_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2857 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/sudo.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1607 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_job_list_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6222 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_exceptions.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4714 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/version.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5360 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/job_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     8676 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/job_array.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1741 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/singleton.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9766 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_object.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1622 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/byte_string.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    26134 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/library_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3549 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/queue_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9581 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_ctypes.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7394 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/job_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3660 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/slot_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14749 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/job.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2298 2023-09-19 04:36:53.000000 uge-drmaa2-8.8.1/drmaa2/__init__.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3742 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_constants.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12375 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/reservation_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9119 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/monitoring_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1630 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/drmaa2/drmaa2_version_descriptor.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/PKG-INFO
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/test/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1293 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_machine_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3267 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_job_array.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1770 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_reservation.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5120 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_job.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1858 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_failed.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1646 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_library_manager.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4657 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_reservation_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    10970 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_job_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6688 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_job_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3988 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_reservation_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6813 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_job_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3109 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_monitoring_session.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1288 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_notification.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6023 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_reservation_template.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1268 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_queue_info.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2261 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_sudo.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1817 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_version.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2221 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/test/test_drmaa2_init.py
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2415 2023-09-18 15:40:41.000000 uge-drmaa2-8.8.1/README.rst
-drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/uge_drmaa2.egg-info/
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/uge_drmaa2.egg-info/dependency_links.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1369 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/uge_drmaa2.egg-info/SOURCES.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/uge_drmaa2.egg-info/PKG-INFO
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        7 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/uge_drmaa2.egg-info/top_level.txt
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      240 2023-09-25 08:12:02.000000 uge-drmaa2-8.8.1/setup.cfg
--rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2156 2023-09-18 15:40:42.000000 uge-drmaa2-8.8.1/setup.py
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/drmaa2/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5824 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/reservation.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4343 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/exception_mapper.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    15156 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_object_descriptors.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4856 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/notification.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1633 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_slot_info_list_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3695 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/reservation_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4595 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/reservation_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2817 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/log_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    22251 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/job_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5388 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/machine_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2857 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/sudo.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1607 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_job_list_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6222 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_exceptions.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4711 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/version.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5360 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/job_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     8676 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/job_array.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1741 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/singleton.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9927 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_object.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1562 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/byte_string.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    26134 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/library_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3545 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/queue_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9559 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_ctypes.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     7378 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/job_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3656 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/slot_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    14745 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/job.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2290 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/__init__.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3738 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_constants.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    12361 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/reservation_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     9278 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/monitoring_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1630 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/drmaa2/drmaa2_version_descriptor.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/PKG-INFO
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/test/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1289 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_machine_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3251 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_job_array.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1766 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_reservation.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5082 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_job.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1853 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_failed.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1640 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_library_manager.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     4641 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_reservation_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)    10908 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_job_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6663 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_job_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3971 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_reservation_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     6779 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_job_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3100 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_monitoring_session.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1288 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_notification.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     5993 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_reservation_template.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1264 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_queue_info.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2243 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_sudo.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1809 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_version.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2211 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/test/test_drmaa2_init.py
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2415 2024-04-10 04:30:36.000000 uge-drmaa2-8.9.0/README.rst
+drwxr-xr-x   0 sgetest   (9901) sgegroup  (9901)        0 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/uge_drmaa2.egg-info/
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        1 2024-04-14 10:20:48.000000 uge-drmaa2-8.9.0/uge_drmaa2.egg-info/dependency_links.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     1369 2024-04-14 10:20:48.000000 uge-drmaa2-8.9.0/uge_drmaa2.egg-info/SOURCES.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     3607 2024-04-14 10:20:48.000000 uge-drmaa2-8.9.0/uge_drmaa2.egg-info/PKG-INFO
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)        7 2024-04-14 10:20:48.000000 uge-drmaa2-8.9.0/uge_drmaa2.egg-info/top_level.txt
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)      240 2024-04-14 10:20:49.000000 uge-drmaa2-8.9.0/setup.cfg
+-rw-r--r--   0 sgetest   (9901) sgegroup  (9901)     2156 2024-04-10 04:30:37.000000 uge-drmaa2-8.9.0/setup.py
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/reservation.py` & `uge-drmaa2-8.9.0/drmaa2/reservation.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,21 @@
         return ReservationInfo(ctypes_reservation_info)
 
     def __del__(self):
         pass
 
     @classmethod
     def to_py_reservation_list(cls, ctypes_list):
-        py_reservation_list = list()
+        py_reservation_list = []
         if ctypes_list:
-            count = cls.drmaa2_lib.drmaa2_list_size(ctypes_list)
+            drmaa2_lib = cls.get_drmaa2_library()
+            count = drmaa2_lib.drmaa2_list_size(ctypes_list)
             cls.logger.debug('Converting ctypes reservation list of size {}'.format(count))
             for i in range(count):
-                void_ptr = cls.drmaa2_lib.drmaa2_list_get(ctypes_list, i)
+                void_ptr = drmaa2_lib.drmaa2_list_get(ctypes_list, i)
                 if void_ptr:
                     r = cast(void_ptr, POINTER(drmaa2_r))
                     r = Reservation(r)
                     py_reservation_list.append(r)
                 else:
                     ExceptionMapper.check_last_error_code()
                     py_reservation_list.append(None)
@@ -137,9 +138,9 @@
 
     @classmethod
     def to_ctypes_reservation_list(cls, py_reservation_list):
         cls.logger.debug('Converting py reservation list of size {}'.format(len(py_reservation_list)))
         ctypes_reservation_list = cls.drmaa2_lib.drmaa2_list_create(int(ListType.RESERVATIONLIST),
                                                                     drmaa2_list_entryfree())
         for r in py_reservation_list:
-            ExceptionMapper.check_status_code(cls.drmaa2_lib.drmaa2_list_add(ctypes_reservation_list, j._struct))
+            ExceptionMapper.check_status_code(cls.drmaa2_lib.drmaa2_list_add(ctypes_reservation_list, r._struct))
         return ctypes_reservation_list
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/exception_mapper.py` & `uge-drmaa2-8.9.0/drmaa2/exception_mapper.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_object_descriptors.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_object_descriptors.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/notification.py` & `uge-drmaa2-8.9.0/drmaa2/notification.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_slot_info_list_descriptor.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_slot_info_list_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/reservation_info.py` & `uge-drmaa2-8.9.0/drmaa2/reservation_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/reservation_template.py` & `uge-drmaa2-8.9.0/drmaa2/reservation_template.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/log_manager.py` & `uge-drmaa2-8.9.0/drmaa2/log_manager.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/job_session.py` & `uge-drmaa2-8.9.0/drmaa2/job_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python 
+#!/usr/bin/env python
 # ___INFO__MARK_BEGIN__
 #######################################################################################
 # Copyright 2008-2022 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
@@ -213,15 +213,15 @@
         :type auth: Sudo or dict
 
         >>> JobSession.destroy_by_name('js-01')
         """
         cls.logger.debug('Destroying job session {}'.format(name))
         if auth:
             auth = Sudo.create_from_dict(auth)
-            self.logger.debug('Using sudo object: {}'.format(auth))
+            cls.logger.debug('Using sudo object: {}'.format(auth))
             cls.exception_mapper.check_status_code(
                 cls.get_drmaa2_library().drmaa2_destroy_jsession_as(auth._struct, ByteString(name).encode()))
         else:
             cls.exception_mapper.check_status_code(
                 cls.get_drmaa2_library().drmaa2_destroy_jsession(ByteString(name).encode()))
 
     def __del__(self):
@@ -493,15 +493,19 @@
         >>> j_list = j_session.get_all_jobs(j_info)
         """
         self.logger.debug('Requesting list of jobs using filter: {}'.format(filter))
         drmaa2_lib = self.get_drmaa2_library()
         job_info = filter
         if type(filter) == PY_DICT_TYPE:
             job_info = JobInfo(filter)
-        ctypes_filter = job_info._struct
+
+        ctypes_filter = None
+        if job_info is not None:
+            ctypes_filter = job_info._struct
+
         ctypes_job_list = drmaa2_lib.drmaa2_jsession_get_jobs(self._struct, ctypes_filter)
         if not ctypes_job_list:
             self.exception_mapper.check_last_error_code()
 
         py_job_list = []
         if ctypes_job_list:
             py_job_list = Job.to_py_job_list(ctypes_job_list)
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/machine_info.py` & `uge-drmaa2-8.9.0/drmaa2/machine_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             cls.implementation_specific_keys = cls.to_py_string_list(
                 cls.get_drmaa2_library().drmaa2_machineinfo_impl_spec())
         return cls.implementation_specific_keys
 
     @classmethod
     def to_py_machine_info_list(cls, ctypes_list):
         drmaa2_lib = cls.get_drmaa2_library()
-        py_machine_info_list = list()
+        py_machine_info_list = []
         if ctypes_list:
             count = drmaa2_lib.drmaa2_list_size(ctypes_list)
             cls.logger.debug('Converting ctypes machine info list of size {}'.format(count))
             for i in range(count):
                 void_ptr = drmaa2_lib.drmaa2_list_get(ctypes_list, i)
                 if void_ptr:
                     mi = cast(void_ptr, POINTER(drmaa2_machineinfo))
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/sudo.py` & `uge-drmaa2-8.9.0/drmaa2/sudo.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_job_list_descriptor.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_job_list_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_exceptions.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_exceptions.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/version.py` & `uge-drmaa2-8.9.0/drmaa2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         Retrieve dict of implementation-specific attrs.
 
         :returns: {str:str} dict of implementation-specific attrs.
 
         >>> print(Version.get_implementation_specific_attrs())
         ['uge_version_json':'xyz']
         """
-        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drmaa_version();
+        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drmaa_version()
         if cls.implementation_specific_attrs is None:
             cls.implementation_specific_attrs = cls.to_py_dict(
                 cls.get_drmaa2_library().uge_vi_impl_spec_get(ctypes_version))
         return cls.implementation_specific_attrs
 
     @classmethod
     def get_implementation_specific_keys(cls):
@@ -107,15 +107,15 @@
 
         >>> v = Version.get_drms_version()
         >>> print(v.major)
         8
         >>> print(v.minor)
         6.0
         """
-        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drms_version();
+        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drms_version()
         py_version = Version(ctypes_version)
         cls.get_drmaa2_library().drmaa2_version_free(ctypes_version)
         return py_version
 
     @classmethod
     def get_drmaa_version(cls):
         """
@@ -125,11 +125,11 @@
 
         >>> v = Version.get_drmaa_version()
         >>> print(v.major)
         2
         >>> print(v.minor)
         0
         """
-        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drmaa_version();
+        ctypes_version = cls.get_drmaa2_library().drmaa2_get_drmaa_version()
         py_version = Version(ctypes_version)
         cls.get_drmaa2_library().drmaa2_version_free(ctypes_version)
         return py_version
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/job_info.py` & `uge-drmaa2-8.9.0/drmaa2/job_info.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/job_array.py` & `uge-drmaa2-8.9.0/drmaa2/job_array.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/singleton.py` & `uge-drmaa2-8.9.0/drmaa2/singleton.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_object.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         :returns: Dictionary representing object's structure.
 
         >>> v = Version.get_drms_version()
         >>> print(v.to_dict())
         {'implementation_specific': {}, 'major': '8', 'minor': '6.0'}
         """
-        d = dict()
+        d = {}
         if not self._struct:
             for (k, v) in self._dict.items():
                 if v is not None:
                     d[k] = v
                     if type(v) == PY_STRING_TYPE:
                         pass
                     elif type(v) == PY_BYTES_TYPE:
@@ -203,15 +203,15 @@
 
     def __repr__(self):
         """ Object representation. """
         return '%s(%s)' % (self.__class__.__name__, self.__str__())
 
     @classmethod
     def to_py_dict(cls, ctypes_dict):
-        py_dict = dict()
+        py_dict = {}
         if ctypes_dict:
             drmaa2_lib = cls.get_drmaa2_library()
             ctypes_list = drmaa2_lib.drmaa2_dict_list(ctypes_dict)
             list_size = drmaa2_lib.drmaa2_list_size(ctypes_list)
             if list_size < 0:
                 ExceptionMapper.check_last_error_code()
             for i in range(list_size):
@@ -223,15 +223,15 @@
                 py_dict[key] = value
             drmaa2_lib.drmaa2_list_free(pointer(c_void_p(ctypes_list)))
             drmaa2_lib.drmaa2_dict_free(pointer(c_void_p(ctypes_dict)))
         return py_dict
 
     @classmethod
     def to_py_string_list(cls, ctypes_list):
-        py_list = list()
+        py_list = []
         if ctypes_list:
             drmaa2_lib = cls.get_drmaa2_library()
             list_size = drmaa2_lib.drmaa2_list_size(ctypes_list)
             if list_size < 0:
                 ExceptionMapper.check_last_error_code()
             for i in range(list_size):
                 void_ptr = drmaa2_lib.drmaa2_list_get(ctypes_list, i)
@@ -256,14 +256,20 @@
         value_list = [ByteString(v).encode() for v in py_list]
         for i in range(len(value_list)):
             v = value_list[i]
             ExceptionMapper.check_status_code(drmaa2_lib.drmaa2_list_add(ctypes_list, v))
         return ctypes_list
 
     @classmethod
+    def to_ctypes_string_list_or_none(cls, py_list):
+        if py_list is None:
+            return None
+        return cls.to_ctypes_string_list(py_list)
+
+    @classmethod
     def get_implementation_specific_keys(cls):
         return cls.implementation_specific_keys
 
 
 #######################################################################
 # Test.
 if __name__ == '__main__':
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/byte_string.py` & `uge-drmaa2-8.9.0/drmaa2/byte_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,19 @@
 
     def __str__(self):
         return str(self.s)
 
     def encode(self):
         if self.s is None or self.python_version == '2':
             return self.s
-        else:
-            try:
-                return self.s.encode()
-            except AttributeError:
-                return self.s
+        try:
+            return self.s.encode()
+        except AttributeError:
+            return self.s
 
     def decode(self):
         if self.s is None or self.python_version == '2':
             return self.s
-        else:
-            try:
-                return self.s.decode()
-            except AttributeError:
-                return self.s
+        try:
+            return self.s.decode()
+        except AttributeError:
+            return self.s
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/library_manager.py` & `uge-drmaa2-8.9.0/drmaa2/library_manager.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/drmaa2/queue_info.py` & `uge-drmaa2-8.9.0/drmaa2/queue_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             cls.implementation_specific_keys = cls.to_py_string_list(
                 cls.get_drmaa2_library().drmaa2_queueinfo_impl_spec())
         return cls.implementation_specific_keys
 
     @classmethod
     def to_py_queue_info_list(cls, ctypes_list):
         drmaa2_lib = cls.get_drmaa2_library()
-        py_queue_info_list = list()
+        py_queue_info_list = []
         if ctypes_list:
             count = drmaa2_lib.drmaa2_list_size(ctypes_list)
             cls.logger.debug('Converting ctypes queue info list of size {}'.format(count))
             for i in range(count):
                 void_ptr = drmaa2_lib.drmaa2_list_get(ctypes_list, i)
                 if void_ptr:
                     qi = cast(void_ptr, POINTER(drmaa2_queueinfo))
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_ctypes.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_ctypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,15 @@
     #            values[key] = val
     #        super().__init__(**values)
 
     def __eq__(self, other):
         if isinstance(other, str):
             if self.python_version == '2':
                 return self.value == other
-            else:
-                return self.value == other.encode()
+            return self.value == other.encode()
         else:
             return self.value == other.value
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def encode(self):
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/job_template.py` & `uge-drmaa2-8.9.0/drmaa2/job_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,18 +131,18 @@
         setattr(self._struct.contents, 'jobCategory', drmaa2_string())
         setattr(self._struct.contents, 'jobName', drmaa2_string())
         setattr(self._struct.contents, 'inputPath', drmaa2_string())
         setattr(self._struct.contents, 'outputPath', drmaa2_string())
         setattr(self._struct.contents, 'errorPath', drmaa2_string())
         setattr(self._struct.contents, 'reservationId', drmaa2_string())
         setattr(self._struct.contents, 'queueName', drmaa2_string())
-        setattr(self._struct.contents, 'job_environment', dict())
-        setattr(self._struct.contents, 'stage_in_files', dict())
-        setattr(self._struct.contents, 'stage_out_files', dict())
-        setattr(self._struct.contents, 'resource_limits', dict())
+        setattr(self._struct.contents, 'job_environment', {})
+        setattr(self._struct.contents, 'stage_in_files', {})
+        setattr(self._struct.contents, 'stage_out_files', {})
+        setattr(self._struct.contents, 'resource_limits', {})
         setattr(self._struct.contents, 'accountingId', drmaa2_string())
         self.get_drmaa2_library().drmaa2_jtemplate_free(pointer(self._struct))
 
     @classmethod
     def get_implementation_specific_keys(cls):
         """
         Retrieve list of implementation-specific keys.
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/slot_info.py` & `uge-drmaa2-8.9.0/drmaa2/slot_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if cls.implementation_specific_keys is None:
             # cls.implementation_specific_keys = cls.to_py_string_list(cls.get_drmaa2_library().drmaa2_slotinfo_impl_spec())
             cls.implementation_specific_keys = []
         return cls.implementation_specific_keys
 
     @classmethod
     def to_py_job_list(cls, ctypes_list):
-        py_job_list = list()
+        py_job_list = []
         if ctypes_list:
             count = cls.drmaa2_lib.drmaa2_list_size(ctypes_list)
             cls.logger.debug('Converting ctypes job list of size {}'.format(count))
             for i in range(count):
                 void_ptr = cls.drmaa2_lib.drmaa2_list_get(ctypes_list, i)
                 if void_ptr:
                     si = cast(void_ptr, POINTER(drmaa2_slotinfo))
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/job.py` & `uge-drmaa2-8.9.0/drmaa2/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
     def __del__(self):
         pass
 
     @classmethod
     def to_py_job_list(cls, ctypes_list):
         drmaa2_lib = cls.get_drmaa2_library()
-        py_job_list = list()
+        py_job_list = []
         if ctypes_list:
             count = drmaa2_lib.drmaa2_list_size(ctypes_list)
             cls.logger.debug('Converting ctypes job list of size {}'.format(count))
             for i in range(count):
                 void_ptr = drmaa2_lib.drmaa2_list_get(ctypes_list, i)
                 if void_ptr:
                     j = cast(void_ptr, POINTER(drmaa2_j))
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/__init__.py` & `uge-drmaa2-8.9.0/drmaa2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
-from .drmaa2_constants import (Bool, Capability, Cpu, Event, JobState, 
+from .drmaa2_constants import (Bool, Capability, Cpu, Event, JobState,
     ListType, Os, ResourceLimit, StatusCode, Time)
 from .drmaa2_exceptions import (Drmaa2Exception, DeniedByDrms,
-    DrmCommunicationError, TryLaterError, SessionManagementError, 
-    TimeoutError, InternalError, InvalidArgument, 
-    InvalidSession, InvalidState, ResourceNotAvailable, 
+    DrmCommunicationError, TryLaterError, SessionManagementError,
+    TimeoutError, InternalError, InvalidArgument,
+    InvalidSession, InvalidState, ResourceNotAvailable,
     UnsupportedAttribute, UnsupportedOperation,
     ImplementationSpecificError, AuthorizationError)
 from .library_manager import LibraryManager
 from .log_manager import LogManager
 from .job_session import JobSession
 from .job_info import JobInfo
 from .job_array import JobArray
@@ -40,14 +40,14 @@
 from .monitoring_session import MonitoringSession
 from .machine_info import MachineInfo
 from .queue_info import QueueInfo
 from .notification import Notification
 
 get_drms_name = LibraryManager.get_drms_name
 get_drmaa_name = LibraryManager.get_drmaa_name
-drmaa_supports = LibraryManager.drmaa_supports 
+drmaa_supports = LibraryManager.drmaa_supports
 get_drms_version = Version.get_drms_version
 get_drmaa_version = Version.get_drmaa_version
-get_job_session_names = JobSession.list_session_names 
-get_reservation_session_names = ReservationSession.list_session_names 
- 
-__version__ = '8.8.1'
+get_job_session_names = JobSession.list_session_names
+get_reservation_session_names = ReservationSession.list_session_names
+
+__version__ = '8.9.0'
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_constants.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 UNSET_BOOL = 0
 UNSET_ENUM = -1
 UNSET_NUM = -1
 UNSET_PRIORITY = -99999
 UNSET_TIME = -3
 
 POSIX_EPOCH = datetime.utcfromtimestamp(0)
-PY_DICT_TYPE = type(dict())
+PY_DICT_TYPE = type({})
 PY_STRING_TYPE = type('string')
 PY_BYTES_TYPE = type(b'string')
 
 
 class Bool(IntEnum):
     """ DRMAA2 Bool enum. """
     FALSE = 0
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/reservation_session.py` & `uge-drmaa2-8.9.0/drmaa2/reservation_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python 
+#!/usr/bin/env python
 # ___INFO__MARK_BEGIN__
 #######################################################################################
 # Copyright 2008-2022 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
@@ -78,26 +78,26 @@
         name = name or session_dict.get('name')
         if not name:
             name = uuid4().hex
             check_for_existing_session = False
         contact = contact or session_dict.get('contact') or drmaa2_string()
         create_new_session = True
         if check_for_existing_session:
-             existing_session_names = self.list_session_names()
-             session_names_to_check = [name]
-             if contact:
-                 session_names_to_check.append('%s@%s' % (contact,name))
-             else:
-                 session_names_to_check.append('%s@%s' % (getpass.getuser(),name))
-             for n in session_names_to_check:
-                 if n in existing_session_names:
-                     name = n
-                     self.logger.debug('Discovered existing job session with name {}'.format(n))
-                     create_new_session = False
-                     break
+            existing_session_names = self.list_session_names()
+            session_names_to_check = [name]
+            if contact:
+                session_names_to_check.append('%s@%s' % (contact,name))
+            else:
+                session_names_to_check.append('%s@%s' % (getpass.getuser(),name))
+            for n in session_names_to_check:
+                if n in existing_session_names:
+                    name = n
+                    self.logger.debug('Discovered existing job session with name {}'.format(n))
+                    create_new_session = False
+                    break
 
         self._name_bs = ByteString()
         self._auth = auth
         if create_new_session:
             self._struct = self.__create(name, contact, auth)
         else:
             self._struct = self.__open(name)
@@ -289,8 +289,7 @@
         ctypes_reservation_list = drmaa2_lib.drmaa2_rsession_get_reservations(self._struct)
         if not ctypes_reservation_list:
             self.exception_mapper.check_last_error_code()
         py_reservation_list = Reservation.to_py_reservation_list(ctypes_reservation_list)
         self.logger.debug('Retrieved {} reservations'.format(len(py_reservation_list)))
         drmaa2_lib.drmaa2_list_free(pointer(c_void_p(ctypes_reservation_list)))
         return py_reservation_list
-
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/monitoring_session.py` & `uge-drmaa2-8.9.0/drmaa2/monitoring_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python 
+#!/usr/bin/env python
 # ___INFO__MARK_BEGIN__
 #######################################################################################
 # Copyright 2008-2022 Altair Engineering Inc.
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.
 #
 # You may obtain a copy of the License at
@@ -125,15 +125,15 @@
 
         >>> mi_list = m_session.get_all_machines(['univa.example.com'])
         >>> print(mi_list)
          [MachineInfo({'available': 'TRUE', 'cores_per_socket': 1, 'implementation_specific': {}, 'load': 0.07999999821186066, 'machine_arch': 'X64', 'machine_os': 'OTHER_OS', 'machine_os_version': Version({'implementation_specific': {}}), 'name': 'univ.example.com', 'phys_memory': 4047372, 'sockets': 1, 'threads_per_core': 1, 'virt_memory': 8110599})]
         """
         self.logger.debug('Requesting list of machines using filter: {}'.format(filter))
         drmaa2_lib = self.get_drmaa2_library()
-        ctypes_filter = self.to_ctypes_string_list(filter)
+        ctypes_filter = self.to_ctypes_string_list_or_none(filter)
         ctypes_machine_info_list = drmaa2_lib.drmaa2_msession_get_all_machines(self._struct, ctypes_filter)
         if not ctypes_machine_info_list:
             self.exception_mapper.check_last_error_code()
 
         py_machine_info_list = []
         if ctypes_machine_info_list:
             py_machine_info_list = MachineInfo.to_py_machine_info_list(ctypes_machine_info_list)
@@ -152,15 +152,15 @@
 
         >>> qi_list = m_session.get_all_queues(['all.q'])
         >>> print(qi_list)
         [QueueInfo({'implementation_specific': {}, 'name': 'all.q'})]
         """
         self.logger.debug('Requesting list of queues using filter: {}'.format(filter))
         drmaa2_lib = self.get_drmaa2_library()
-        ctypes_filter = self.to_ctypes_string_list(filter)
+        ctypes_filter = self.to_ctypes_string_list_or_none(filter)
         ctypes_queue_info_list = drmaa2_lib.drmaa2_msession_get_all_queues(self._struct, ctypes_filter)
         if not ctypes_queue_info_list:
             self.exception_mapper.check_last_error_code()
 
         py_queue_info_list = []
         if ctypes_queue_info_list:
             py_queue_info_list = QueueInfo.to_py_queue_info_list(ctypes_queue_info_list)
@@ -183,15 +183,19 @@
         [Reservation({'id': '49'})]
         """
         self.logger.debug('Requesting list of reservations using filter: {}'.format(filter))
         drmaa2_lib = self.get_drmaa2_library()
         reservation_info = filter
         if type(filter) == PY_DICT_TYPE:
             reservation_info = ReservationInfo(filter)
-        ctypes_filter = reservation_info._struct
+
+        ctypes_filter = None
+        if reservation_info is not None:
+            ctypes_filter = reservation_info._struct
+
         ctypes_reservation_list = drmaa2_lib.drmaa2_msession_get_all_reservations(self._struct, ctypes_filter)
         if not ctypes_reservation_list:
             self.exception_mapper.check_last_error_code()
 
         py_reservation_list = []
         if ctypes_reservation_list:
             py_reservation_list = Reservation.to_py_reservation_list(ctypes_reservation_list)
@@ -211,15 +215,19 @@
         >>> j_list = m_session.get_all_jobs(j_info)
         """
         self.logger.debug('Requesting list of jobs using filter: {}'.format(filter))
         drmaa2_lib = self.get_drmaa2_library()
         job_info = filter
         if type(filter) == PY_DICT_TYPE:
             job_info = JobInfo(filter)
-        ctypes_filter = job_info._struct
+
+        ctypes_filter = None
+        if job_info is not None:
+            ctypes_filter = job_info._struct
+
         ctypes_job_list = drmaa2_lib.drmaa2_msession_get_all_jobs(self._struct, ctypes_filter)
         if not ctypes_job_list:
             self.exception_mapper.check_last_error_code()
 
         py_job_list = []
         if ctypes_job_list:
             py_job_list = Job.to_py_job_list(ctypes_job_list)
```

### Comparing `uge-drmaa2-8.8.1/drmaa2/drmaa2_version_descriptor.py` & `uge-drmaa2-8.9.0/drmaa2/drmaa2_version_descriptor.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/PKG-INFO` & `uge-drmaa2-8.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-drmaa2
-Version: 8.8.1
+Version: 8.9.0
 Summary: UGE DRMAA2 Python API
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2008-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-drmaa2-8.8.1/test/test_machine_info.py` & `uge-drmaa2-8.9.0/test/test_machine_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     host_list = os.popen('qconf -sel').read().split()
     print('\nGot hosts: %s' % host_list)
     h = host_list[0]
     print('\nUsing first host: %s' % h)
     ms = MonitoringSession('ms-01')
     mi_list = ms.get_all_machines([h])
     print(mi_list)
-    assert (len(mi_list) == 1)
+    assert len(mi_list) == 1
     mi = mi_list[0]
-    assert (mi.name == h)
+    assert mi.name == h
     print('\nGot machine info: %s' % (mi.to_dict()))
```

### Comparing `uge-drmaa2-8.8.1/test/test_job_array.py` & `uge-drmaa2-8.9.0/test/test_job_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,63 +31,63 @@
     ja.terminate()
     j_list = ja.job_list
     failed_jobs = []
     for j in j_list:
         s, ss = j.get_state()
         if s == JobState.FAILED:
             failed_jobs.append(j)
-    assert (len(failed_jobs) > 0)
+    assert len(failed_jobs) > 0
     print('\nTerminate job array: %s' % (ja))
 
 
 def test_suspend_and_resume():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 3, 2)
     j_list = ja.job_list
     js.wait_any_started(j_list)
     ja.suspend()
     suspended_jobs = []
     for j in j_list:
-        s, ss = j.get_state()
+        s, _ = j.get_state()
         if s == JobState.SUSPENDED:
             suspended_jobs.append(j)
-    assert (len(suspended_jobs) > 0)
+    assert len(suspended_jobs) > 0
     print('\nSuspend job array: %s' % (ja))
     ja.resume()
     for j in suspended_jobs:
-        s, ss = j.get_state()
-        assert (s != JobState.SUSPENDED)
+        s, _ = j.get_state()
+        assert s != JobState.SUSPENDED
     print('Resume job array: %s' % (ja))
 
 
 def test_hold_and_release():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 3, 2)
     ja.hold()
     held_jobs = []
     j_list = ja.job_list
     for j in j_list:
-        s, ss = j.get_state()
+        s, _ = j.get_state()
         if s.name.endswith('HELD'):
             held_jobs.append(j)
-    assert (len(held_jobs) > 0)
+    assert len(held_jobs) > 0
     print('\nHold job array: %s' % (ja))
     ja.release()
     for j in held_jobs:
-        s, ss = j.get_state()
-        assert (not s.name.endswith('HELD'))
+        s, _ = j.get_state()
+        assert not s.name.endswith('HELD')
     print('Release job array: %s' % (ja))
 
 
 def test_get_template():
     session_name = generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 3, 2)
     jt = ja.get_template()
-    assert (jt.job_name == job_name)
+    assert jt.job_name == job_name
     print('\nGet template: %s' % (jt))
```

### Comparing `uge-drmaa2-8.8.1/test/test_reservation.py` & `uge-drmaa2-8.9.0/test/test_reservation.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def test_get_info():
     rs = ReservationSession('rs-01')
     r_name = 'res-%s' % int(random.uniform(0, 1000))
     r = rs.request_reservation({'reservation_name': r_name, 'duration': 100})
     ri = r.get_info()
-    assert (ri.reservation_name == r_name)
+    assert ri.reservation_name == r_name
     r.terminate()
     print('\nGet info: %s' % (ri))
 
 
 def test_terminate():
     rs = ReservationSession('rs-01')
     r_name = 'res-%s' % int(random.uniform(0, 1000))
@@ -42,9 +42,9 @@
 
 def test_get_template():
     rs = ReservationSession('rs-01')
     r_name = 'res-%s' % int(random.uniform(0, 1000))
     d = {'reservation_name': r_name, 'duration': 100}
     r = rs.request_reservation(d)
     rt = r.get_template()
-    assert (rt.reservation_name == r_name)
+    assert rt.reservation_name == r_name
     print('\nGet template: %s' % (rt))
```

### Comparing `uge-drmaa2-8.8.1/test/test_job.py` & `uge-drmaa2-8.9.0/test/test_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,121 +14,121 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
-from .utils import generate_random_string
-from drmaa2 import JobSession
 from drmaa2 import JobState
+from drmaa2 import JobSession
+from .utils import generate_random_string
 
 
 def test_get_info():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j.wait_started()
     ji = j.get_info()
-    assert (ji.job_name == job_name)
+    assert ji.job_name == job_name
     print('\nGet info: %s' % (ji))
 
 
 def test_get_state():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
-    (j_state, j_sub_state) = j.get_state()
-    assert (isinstance(j_state, JobState))
+    (j_state, _) = j.get_state()
+    assert isinstance(j_state, JobState)
     print('\nGet state %s for job %s' % (j_state, j))
 
 
 def test_terminate():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     ji = j.get_info()
-    assert (ji.terminating_signal is None)
+    assert ji.terminating_signal is None
     j.wait_started()
     j.terminate()
     j.wait_terminated()
     ji = j.get_info()
-    assert (ji.terminating_signal is not None)
+    assert ji.terminating_signal is not None
     print('\nTerminate job: %s' % (ji))
 
 
 def test_suspend_and_resume():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j.wait_started()
     ji = j.get_info()
-    assert (ji.job_state != JobState.SUSPENDED.name)
+    assert ji.job_state != JobState.SUSPENDED.name
     j.suspend()
     ji = j.get_info()
-    assert (ji.job_state == JobState.SUSPENDED.name)
+    assert ji.job_state == JobState.SUSPENDED.name
     print('\nSuspend job: %s' % (ji))
     j.resume()
     ji = j.get_info()
-    assert (ji.job_state != JobState.SUSPENDED.name)
+    assert ji.job_state != JobState.SUSPENDED.name
     print('Resume job: %s' % (ji))
 
 
 def test_hold_and_release():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     ji = j.get_info()
-    assert (not ji.job_state.endswith('HELD'))
+    assert not ji.job_state.endswith('HELD')
     j.hold()
     ji = j.get_info()
-    assert (ji.job_state.endswith('HELD'))
+    assert ji.job_state.endswith('HELD')
     print('\nHold job: %s' % (ji))
     j.release()
     ji = j.get_info()
-    assert (not ji.job_state.endswith('HELD'))
+    assert not ji.job_state.endswith('HELD')
     print('Release job: %s' % (ji))
 
 
 def test_wait_started():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j.wait_started()
-    s, ss = j.get_state()
-    assert (s == JobState.RUNNING)
+    s, _ = j.get_state()
+    assert s == JobState.RUNNING
     print('\nWait started for job: %s' % (j))
 
 
 def test_wait_terminated():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j.wait_terminated()
-    s, ss = j.get_state()
-    assert (s == JobState.DONE)
+    s, _ = j.get_state()
+    assert s == JobState.DONE
     print('\nWait terminated for job: %s' % (j))
 
 
 def test_get_template():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     job_name = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': job_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     jt = j.get_template()
-    assert (jt.job_name == job_name)
+    assert jt.job_name == job_name
     print('\nGet template: %s' % (jt))
```

### Comparing `uge-drmaa2-8.8.1/test/test_failed.py` & `uge-drmaa2-8.9.0/test/test_failed.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
-from .utils import generate_random_string
-from drmaa2 import JobSession
 from drmaa2 import JobState
+from drmaa2 import JobSession
+from .utils import generate_random_string
 
 
 def test_get_info():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     jn = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': jn, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     ji = j.get_info()
-    assert (ji.job_name == jn)
+    assert ji.job_name == jn
     print('\nGet info: %s' % (ji))
 
 
 def test_wait_terminated():
     session_name = 'drmaa2python-%s' % generate_random_string()
     js = JobSession(session_name)
     jn = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': jn, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j.wait_terminated()
-    s, ss = j.get_state()
-    assert (s == JobState.DONE)
+    s, _ = j.get_state()
+    assert s == JobState.DONE
     print('\nWait terminated for job: %s' % (j))
     ji = j.get_info()
     print('\nGet info: %s' % (ji))
```

### Comparing `uge-drmaa2-8.8.1/test/test_library_manager.py` & `uge-drmaa2-8.9.0/test/test_library_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 from drmaa2 import LibraryManager
 from drmaa2 import Capability
 
 
 def test_get_drms_name():
     lm = LibraryManager.get_instance()
     n = lm.get_drms_name()
-    assert (n != '')
+    assert n != ''
     print('\nGot DRMS name: %s' % (n))
 
 
 def test_get_drmaa_name():
     lm = LibraryManager.get_instance()
     n = lm.get_drmaa_name()
-    assert (n != '')
+    assert n != ''
     print('\nGot DRMAA name: %s' % (n))
 
 
 def test_drmaa_supports():
     lm = LibraryManager.get_instance()
     print('\nVerifying support for %s capabilities' % (len(Capability)))
     supported = []
     for c in Capability:
         s = lm.drmaa_supports(c)
         if s:
             supported.append(s)
         print('Support for %s: %s' % (c, s))
-    assert (len(supported) > 0)
+    assert len(supported) > 0
     print('DRMAA2 supports %s out of %s capabilities' % (len(supported), len(Capability)))
```

### Comparing `uge-drmaa2-8.8.1/test/test_reservation_info.py` & `uge-drmaa2-8.9.0/test/test_reservation_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,49 +15,49 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import datetime
-from .utils import generate_random_string
-from .utils import generate_random_int
-from drmaa2 import ReservationSession
 from drmaa2 import ReservationInfo
+from drmaa2 import ReservationSession
 from drmaa2.drmaa2_constants import POSIX_EPOCH
+from .utils import generate_random_string
+from .utils import generate_random_int
 
 
 def test_reservation_info_from_reservation():
     rs = ReservationSession('rs-01')
     reservation_name = 'r.%s' % generate_random_string()
     r = rs.request_reservation({'reservation_name': reservation_name, 'duration': 100})
     ri = r.get_info()
-    assert (ri.reservation_name == reservation_name)
+    assert ri.reservation_name == reservation_name
     print('\nReservation info from reservation: %s' % (ri))
 
 
 def test_get_implementation_specific_keys():
     keys = ReservationInfo.get_implementation_specific_keys()
-    assert (len(keys) > 0)
+    assert len(keys) > 0
     print('\nReservation info implementation specific keys: %s' % (keys))
 
 
 def test_reservation_id_attr():
     ri = ReservationInfo()
     reservation_id = generate_random_string()
     ri.reservation_id = reservation_id
-    assert (ri.reservation_id == reservation_id)
+    assert ri.reservation_id == reservation_id
     print('\nReservation info with reservation_id: %s' % (reservation_id))
 
 
 def test_reservation_name_attr():
     ri = ReservationInfo()
     reservation_name = generate_random_string()
     ri.reservation_name = reservation_name
-    assert (ri.reservation_name == reservation_name)
+    assert ri.reservation_name == reservation_name
     print('\nReservation info with reservation_name: %s' % (reservation_name))
 
 
 def test_reserved_start_time_attr():
     reserved_start_time = datetime.datetime.now()
     ri = ReservationInfo()
     ri.reserved_start_time = reserved_start_time
@@ -74,44 +74,44 @@
         (reserved_end_time - POSIX_EPOCH).total_seconds()))
     print('\nReservation info object with reserved_end_time: %s' % (reserved_end_time))
 
 
 def test_users_acl_attr():
     users_acl = []
     n_users_acl = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_users_acl):
+    for _ in range(0, n_users_acl):
         users_acl.append(generate_random_string())
     ri = ReservationInfo()
     ri.users_acl = users_acl
-    assert (ri.users_acl == users_acl)
+    assert ri.users_acl == users_acl
     print('\nreservation info object with %s users_acl: %s' % (len(users_acl), users_acl))
 
 
 def test_reserved_slots_attr():
     ri = ReservationInfo()
     reserved_slots = generate_random_int(lower_bound=1, upper_bound=1024)
     ri.reserved_slots = reserved_slots
-    assert (ri.reserved_slots == reserved_slots)
+    assert ri.reserved_slots == reserved_slots
     print('\nReservation info with reserved_slots: %s' % (reserved_slots))
 
 
 def test_reserved_machines_attr():
     reserved_machines = []
     n_reserved_machines = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_reserved_machines):
+    for _ in range(0, n_reserved_machines):
         reserved_machines.append(generate_random_string())
     ri = ReservationInfo()
     ri.reserved_machines = reserved_machines
-    assert (ri.reserved_machines == reserved_machines)
+    assert ri.reserved_machines == reserved_machines
     print('\nreservation info object with %s reserved_machines: %s' % (len(reserved_machines), reserved_machines))
 
 
 def test_implementation_specific_attr():
     implementation_specific = {}
     keys = ReservationInfo.get_implementation_specific_keys()
     for k in keys:
         v = generate_random_string()
         implementation_specific[k] = v
     ri = ReservationInfo()
     ri.implementation_specific = implementation_specific
-    assert (ri.implementation_specific == implementation_specific)
+    assert ri.implementation_specific == implementation_specific
     print('\nReservation info object with implementation_specific: %s' % (implementation_specific))
```

### Comparing `uge-drmaa2-8.8.1/test/test_job_template.py` & `uge-drmaa2-8.9.0/test/test_job_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,296 +15,296 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import datetime
-from .utils import generate_random_string
-from .utils import generate_random_int
-from drmaa2 import JobTemplate
 from drmaa2 import Bool
 from drmaa2 import Os
 from drmaa2 import Cpu
+from drmaa2 import JobTemplate
 from drmaa2 import Drmaa2Exception
 from drmaa2.drmaa2_constants import POSIX_EPOCH
+from .utils import generate_random_string
+from .utils import generate_random_int
 
 
 def test_remote_command_attr():
     remote_command = generate_random_string()
     jt = JobTemplate()
     jt.remote_command = remote_command
-    assert (jt.remote_command == remote_command)
+    assert jt.remote_command == remote_command
     print('\nJob template object with remote_command: %s' % (remote_command))
 
 
 def test_args_attr():
     args = []
     n_args = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_args):
+    for _ in range(0, n_args):
         args.append(generate_random_string())
     jt = JobTemplate()
     jt.args = args
-    assert (jt.args == args)
+    assert jt.args == args
     print('\nJob template object with %s args: %s' % (len(args), args))
 
 
 def test_submit_as_hold_attr():
     submit_as_hold = generate_random_int(lower_bound=0, upper_bound=1)
     jt = JobTemplate()
     jt.submit_as_hold = submit_as_hold
-    assert (jt.submit_as_hold == Bool(submit_as_hold).name)
+    assert jt.submit_as_hold == Bool(submit_as_hold).name
     print('\nJob template object with submit_as_hold: %s' % (submit_as_hold))
 
 
 def test_rerunnable_attr():
     rerunnable = generate_random_int(lower_bound=0, upper_bound=1)
     jt = JobTemplate()
     jt.rerunnable = rerunnable
-    assert (jt.rerunnable == Bool(rerunnable).name)
+    assert jt.rerunnable == Bool(rerunnable).name
     print('\nJob template object with rerunnable: %s' % (rerunnable))
 
 
 def test_job_environment_attr():
     job_environment = {}
     n_args = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_args):
+    for _ in range(0, n_args):
         name = generate_random_string().upper()
         value = generate_random_string()
         job_environment[name] = value
     jt = JobTemplate()
     jt.job_environment = job_environment
-    assert (jt.job_environment == job_environment)
+    assert jt.job_environment == job_environment
     print('\nJob template object with job_environment: %s' % (job_environment))
 
 
 def test_working_directory_attr():
     working_directory = generate_random_string()
     jt = JobTemplate()
     jt.working_directory = working_directory
-    assert (jt.working_directory == working_directory)
+    assert jt.working_directory == working_directory
     print('\nJob template object with working_directory: %s' % (working_directory))
 
 
 def test_job_category_attr():
     job_category = generate_random_string()
     jt = JobTemplate()
     jt.job_category = job_category
-    assert (jt.job_category == job_category)
+    assert jt.job_category == job_category
     print('\nJob template object with job_category: %s' % (job_category))
 
 
 def test_email_attr():
     email = []
     n_email = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_email):
+    for _ in range(0, n_email):
         email.append(generate_random_string())
     jt = JobTemplate()
     jt.email = email
-    assert (jt.email == email)
+    assert jt.email == email
     print('\nJob template object with %s emails: %s' % (len(email), email))
 
 
 def test_email_on_started_attr():
     email_on_started = generate_random_int(lower_bound=0, upper_bound=1)
     jt = JobTemplate()
     jt.email_on_started = email_on_started
-    assert (jt.email_on_started == Bool(email_on_started).name)
+    assert jt.email_on_started == Bool(email_on_started).name
     print('\nJob template object with email_on_started: %s' % (email_on_started))
 
 
 def test_email_on_terminated_attr():
     email_on_terminated = generate_random_int(lower_bound=0, upper_bound=1)
     jt = JobTemplate()
     jt.email_on_terminated = email_on_terminated
-    assert (jt.email_on_terminated == Bool(email_on_terminated).name)
+    assert jt.email_on_terminated == Bool(email_on_terminated).name
     print('\nJob template object with email_on_terminated: %s' % (email_on_terminated))
 
 
 def test_job_name_attr():
     job_name = generate_random_string()
     jt = JobTemplate()
     jt.job_name = job_name
-    assert (jt.job_name == job_name)
+    assert jt.job_name == job_name
     print('\nJob template object with job_name: %s' % (job_name))
 
 
 def test_input_path_attr():
     input_path = generate_random_string()
     jt = JobTemplate()
     jt.input_path = input_path
-    assert (jt.input_path == input_path)
+    assert jt.input_path == input_path
     print('\nJob template object with input_path: %s' % (input_path))
 
 
 def test_output_path_attr():
     output_path = generate_random_string()
     jt = JobTemplate()
     jt.output_path = output_path
-    assert (jt.output_path == output_path)
+    assert jt.output_path == output_path
     print('\nJob template object with output_path: %s' % (output_path))
 
 
 def test_error_path_attr():
     error_path = generate_random_string()
     jt = JobTemplate()
     jt.error_path = error_path
-    assert (jt.error_path == error_path)
+    assert jt.error_path == error_path
     print('\nJob template object with error_path: %s' % (error_path))
 
 
 def test_join_files_attr():
     join_files = generate_random_int(lower_bound=0, upper_bound=1)
     jt = JobTemplate()
     jt.join_files = join_files
-    assert (jt.join_files == Bool(join_files).name)
+    assert jt.join_files == Bool(join_files).name
     print('\nJob template object with join_files: %s' % (join_files))
 
 
 def test_reservation_id_attr():
     reservation_id = generate_random_string()
     jt = JobTemplate()
     jt.reservation_id = reservation_id
-    assert (jt.reservation_id == reservation_id)
+    assert jt.reservation_id == reservation_id
     print('\nJob template object with reservation_id: %s' % (reservation_id))
 
 
 def test_queue_name_attr():
     queue_name = generate_random_string()
     jt = JobTemplate()
     jt.queue_name = queue_name
-    assert (jt.queue_name == queue_name)
+    assert jt.queue_name == queue_name
     print('\nJob template object with queue_name: %s' % (queue_name))
 
 
 def test_min_slots_attr():
     min_slots = generate_random_int(lower_bound=0, upper_bound=100)
     jt = JobTemplate()
     jt.min_slots = min_slots
-    assert (jt.min_slots == min_slots)
+    assert jt.min_slots == min_slots
     print('\nJob template object with min_slots: %s' % (min_slots))
 
 
 def test_max_slots_attr():
     max_slots = generate_random_int(lower_bound=0, upper_bound=100)
     jt = JobTemplate()
     jt.max_slots = max_slots
-    assert (jt.max_slots == max_slots)
+    assert jt.max_slots == max_slots
     print('\nJob template object with max_slots: %s' % (max_slots))
 
 
 def test_priority_attr():
     priority = generate_random_int(lower_bound=0, upper_bound=1000)
     jt = JobTemplate()
     jt.priority = priority
-    assert (jt.priority == priority)
+    assert jt.priority == priority
     print('\nJob template object with priority: %s' % (priority))
 
 
 def test_candidate_machines_attr():
     candidate_machines = []
     n_candidate_machines = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_candidate_machines):
+    for _ in range(0, n_candidate_machines):
         candidate_machines.append(generate_random_string())
     jt = JobTemplate()
     jt.candidate_machines = candidate_machines
-    assert (jt.candidate_machines == candidate_machines)
+    assert jt.candidate_machines == candidate_machines
     print('\nJob template object with %s candidate_machines: %s' % (len(candidate_machines), candidate_machines))
 
 
 def test_min_phys_memory_attr():
     min_phys_memory = generate_random_int(lower_bound=0, upper_bound=1000)
     jt = JobTemplate()
     jt.min_phys_memory = min_phys_memory
-    assert (jt.min_phys_memory == min_phys_memory)
+    assert jt.min_phys_memory == min_phys_memory
     print('\nJob template object with min_phys_memory: %s' % (min_phys_memory))
 
 
 def test_machine_os_attr():
     machine_os = generate_random_int(lower_bound=0, upper_bound=11)
     jt = JobTemplate()
     jt.machine_os = machine_os
-    assert (jt.machine_os == Os(machine_os).name)
+    assert jt.machine_os == Os(machine_os).name
     print('\nJob template object with machine_os: %s' % (machine_os))
 
 
 def test_machine_arch_attr():
     machine_arch = generate_random_int(lower_bound=0, upper_bound=16)
     jt = JobTemplate()
     jt.machine_arch = machine_arch
-    assert (jt.machine_arch == Cpu(machine_arch).name)
+    assert jt.machine_arch == Cpu(machine_arch).name
     print('\nJob template object with machine_arch: %s' % (machine_arch))
 
 
 def test_start_time_attr():
     start_time = datetime.datetime.now()
     jt = JobTemplate()
     jt.start_time = start_time
-    assert (int((jt.start_time - POSIX_EPOCH).total_seconds()) == int((start_time - POSIX_EPOCH).total_seconds()))
+    assert int((jt.start_time - POSIX_EPOCH).total_seconds()) == int((start_time - POSIX_EPOCH).total_seconds())
     print('\nJob template object with start_time: %s' % (start_time))
 
 
 def test_deadline_time_attr():
     deadline_time = datetime.datetime.now() + datetime.timedelta(hours=1)
     jt = JobTemplate()
     jt.deadline_time = deadline_time
-    assert (int((jt.deadline_time - POSIX_EPOCH).total_seconds()) == int((deadline_time - POSIX_EPOCH).total_seconds()))
+    assert int((jt.deadline_time - POSIX_EPOCH).total_seconds()) == int((deadline_time - POSIX_EPOCH).total_seconds())
     print('\nJob template object with deadline_time: %s' % (deadline_time))
 
 
 def test_stage_in_files_attr():
     stage_in_files = {}
     n_args = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_args):
+    for _ in range(0, n_args):
         name = generate_random_string().upper()
         value = generate_random_string()
         stage_in_files[name] = value
     jt = JobTemplate()
     jt.stage_in_files = stage_in_files
-    assert (jt.stage_in_files == stage_in_files)
+    assert jt.stage_in_files == stage_in_files
     print('\nJob template object with stage_in_files: %s' % (stage_in_files))
 
 
 def test_stage_out_files_attr():
     stage_out_files = {}
     n_args = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_args):
+    for _ in range(0, n_args):
         name = generate_random_string().upper()
         value = generate_random_string()
         stage_out_files[name] = value
     jt = JobTemplate()
     jt.stage_out_files = stage_out_files
-    assert (jt.stage_out_files == stage_out_files)
+    assert jt.stage_out_files == stage_out_files
     print('\nJob template object with stage_out_files: %s' % (stage_out_files))
 
 
 def test_resource_limits_attr():
     resource_limits = {}
     n_args = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_args):
+    for _ in range(0, n_args):
         name = generate_random_string().upper()
         value = generate_random_string()
         resource_limits[name] = value
     jt = JobTemplate()
     jt.resource_limits = resource_limits
-    assert (jt.resource_limits == resource_limits)
+    assert jt.resource_limits == resource_limits
     print('\nJob template object with resource_limits: %s' % (resource_limits))
 
 
 def test_accounting_id_attr():
     accounting_id = generate_random_string()
     jt = JobTemplate()
     jt.accounting_id = accounting_id
-    assert (jt.accounting_id == accounting_id)
+    assert jt.accounting_id == accounting_id
     print('\nJob template object with accounting_id: %s' % (accounting_id))
 
 
 def test_implementation_specific_attr():
     implementation_specific = {}
     keys = JobTemplate.get_implementation_specific_keys()
     for k in keys:
         v = generate_random_string()
         implementation_specific[k] = v
     jt = JobTemplate()
     jt.implementation_specific = implementation_specific
-    assert (jt.implementation_specific == implementation_specific)
+    assert jt.implementation_specific == implementation_specific
     print('\nJob template object with implementation_specific: %s' % (implementation_specific))
```

### Comparing `uge-drmaa2-8.8.1/test/test_job_session.py` & `uge-drmaa2-8.9.0/test/test_job_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import random
+from drmaa2 import JobInfo
+from drmaa2 import JobSession
 from .utils import generate_random_string
 from .utils import needs_uge
-from drmaa2 import JobSession
-from drmaa2 import JobInfo
 
 
 @needs_uge
 def test_list_session_names():
     session_names = JobSession.list_session_names()
     assert (type(session_names) == type([]))
     print('\nThere are %s existing sessions: %s' % (len(session_names), session_names))
 
 
 def test_new_session():
     session_name = generate_random_string()
     existing_session_names = JobSession.list_session_names()
-    js = JobSession(session_name)
+    _ = JobSession(session_name)
     session_names = JobSession.list_session_names()
-    assert (len(session_names) == len(existing_session_names) + 1)
+    assert len(session_names) == len(existing_session_names) + 1
     print('\nCreated new session: %s' % (session_name))
 
 
 def test_existing_session():
     session_name = generate_random_string()
     existing_session_names = JobSession.list_session_names()
     js = JobSession(session_name, destroy_on_exit=False)
     session_names = JobSession.list_session_names()
-    assert (len(session_names) == len(existing_session_names) + 1)
+    assert len(session_names) == len(existing_session_names) + 1
     print('\nCreated new session: %s' % (session_name))
     del js
     js = JobSession(session_name)
     session_names2 = JobSession.list_session_names()
     assert (len(session_names) == len(session_names2))
     print('Opened existing session: %s' % (session_name))
     del js
@@ -63,62 +63,62 @@
     session_names = JobSession.list_session_names()
     print('\nExisting session names: %s' % session_names)
     for name in session_names:
         print('Destroying session: %s' % name)
         JobSession.destroy_by_name(name)
     session_names = JobSession.list_session_names()
     print('Remaining session names: %s' % session_names)
-    assert (len(session_names) == 0)
+    assert len(session_names) == 0
 
 
 def test_run_job():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     j_id = j.id
-    assert (len(j_id) > 0)
+    assert len(j_id) > 0
     print('\nSubmitted job id: %s' % j_id)
 
 
 def test_run_bulk_jobs():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 5, 2)
     jl = ja.job_list
     ja_id = ja.id
-    assert (len(ja_id) > 0)
-    assert (len(jl) == 2)
+    assert len(ja_id) > 0
+    assert len(jl) == 2
     print('\nSubmitted job array id: %s' % ja_id)
 
 
 def test_wait_any_started():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 5, 2)
     jl = ja.job_list
     jl_ids = list(map(lambda j: j.id, jl))
     print('\nWaiting on start of any job with id from %s' % jl_ids)
     j = js.wait_any_started(jl)
-    assert (j.id in jl_ids)
+    assert j.id in jl_ids
     print('Job %s started' % j)
 
 
 def test_wait_any_terminated():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 5, 2)
     jl = ja.job_list
     jl_ids = list(map(lambda j: j.id, jl))
     print('\nWaiting on termination of any job with id from %s' % jl_ids)
     j = js.wait_any_terminated(jl)
-    assert (j.id in jl_ids)
+    assert j.id in jl_ids
     print('Job %s terminated' % j)
 
 
 def test_wait_all_started():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
@@ -126,15 +126,15 @@
     jl = ja.job_list
     jl_ids = list(map(lambda j: j.id, jl))
     jl_ids.sort()
     print('\nWaiting on start of all jobs: %s' % jl_ids)
     jl2 = js.wait_all_started(jl)
     jl2_ids = list(map(lambda j: j.id, jl2))
     jl2_ids.sort()
-    assert (jl_ids == jl2_ids)
+    assert jl_ids == jl2_ids
     print('Jobs started: ' % jl2_ids)
 
 
 def test_wait_all_terminated():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
@@ -142,25 +142,25 @@
     jl = ja.job_list
     jl_ids = list(map(lambda j: j.id, jl))
     jl_ids.sort()
     print('\nWaiting on termination of all jobs: %s' % jl_ids)
     jl2 = js.wait_all_terminated(jl)
     jl2_ids = list(map(lambda j: j.id, jl2))
     jl2_ids.sort()
-    assert (jl_ids == jl2_ids)
+    assert jl_ids == jl2_ids
     print('Jobs terminated: ' % jl2_ids)
 
 
 def test_get_job_array():
     session_name = generate_random_string()
     js = JobSession(session_name)
     d = {'remote_command': '/bin/sleep', 'args': ['5'], 'output_path': '/dev/null', 'join_files': True}
     ja = js.run_bulk_jobs(d, 1, 10, 5, 2)
     ja2 = js.get_job_array(ja.id)
-    assert (ja.id == ja2.id)
+    assert ja.id == ja2.id
     print('\nRetrieved job array: %s' % ja2)
 
 
 def test_get_job_categories():
     session_name = generate_random_string()
     js = JobSession(session_name)
     job_categories = js.get_job_categories()
@@ -175,8 +175,8 @@
     j = js.run_job(d)
     print('\nSubmitted job: %s' % j)
     ji = j.get_info()
     print('Retrieving jobs matching job info %s' % ji)
     ji2 = JobInfo({'job_id': ji.job_id})
     j_list = js.get_jobs(ji2)
     print('Got jobs: %s' % j_list)
-    assert (len(j_list) >= 1)
+    assert len(j_list) >= 1
```

### Comparing `uge-drmaa2-8.8.1/test/test_reservation_session.py` & `uge-drmaa2-8.9.0/test/test_reservation_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import random
+from drmaa2 import ReservationSession
 from .utils import generate_random_string
 from .utils import needs_uge
-from drmaa2 import ReservationSession
 
 
 @needs_uge
 def test_list_session_names():
     session_names = ReservationSession.list_session_names()
-    assert (type(session_names) == type([]))
+    assert type(session_names) == type([])
     print('\nThere are %s existing sessions: %s' % (len(session_names), session_names))
 
 
 def test_new_session():
     session_name = generate_random_string()
     existing_session_names = ReservationSession.list_session_names()
-    rs = ReservationSession(session_name)
+    _ = ReservationSession(session_name)
     session_names = ReservationSession.list_session_names()
-    assert (len(session_names) == len(existing_session_names) + 1)
+    assert len(session_names) == len(existing_session_names) + 1
     print('\nCreated new session: %s' % (session_name))
 
 
 def test_existing_session():
     session_name = generate_random_string()
     existing_session_names = ReservationSession.list_session_names()
     rs = ReservationSession(session_name, destroy_on_exit=False)
     session_names = ReservationSession.list_session_names()
-    assert (len(session_names) == len(existing_session_names) + 1)
+    assert len(session_names) == len(existing_session_names) + 1
     print('\nCreated new session: %s' % (session_name))
     del rs
     rs = ReservationSession(session_name)
     session_names2 = ReservationSession.list_session_names()
     assert (len(session_names) == len(session_names2))
     print('Opened existing session: %s' % (session_name))
     del rs
@@ -62,45 +62,45 @@
     session_names = ReservationSession.list_session_names()
     print('\nExisting session names: %s' % session_names)
     for name in session_names:
         print('Destroying session: %s' % name)
         ReservationSession.destroy_by_name(name)
     session_names = ReservationSession.list_session_names()
     print('Remaining session names: %s' % session_names)
-    assert (len(session_names) == 0)
+    assert len(session_names) == 0
 
 
 def test_request_reservation():
     rs = ReservationSession('rs-01')
     r_name = 'reservation-%s' % int(random.uniform(0, 1000))
     r = rs.request_reservation({'reservation_name': r_name, 'duration': 100})
     print('\nRequested reservation: %s' % r)
     ri = r.get_info()
-    assert (ri.reservation_name == r_name)
+    assert ri.reservation_name == r_name
     print('Got reservation info: %s' % ri)
 
 
 def test_get_reservations():
     rs = ReservationSession('rs-01')
     r_name = 'reservation-%s' % int(random.uniform(0, 1000))
     r = rs.request_reservation({'reservation_name': r_name, 'duration': 100})
     print('\nRequested reservation: %s' % r)
     r_list = rs.get_reservations()
     print('Got reservations: %s' % r_list)
-    assert (len(r_list) >= 1)
+    assert len(r_list) >= 1
     r_found = False
     for r2 in r_list:
         if r2.id == r.id:
             r_found = True
             break
-    assert (r_found)
+    assert r_found
     r.terminate()
 
 
 def test_get_reservation():
     rs = ReservationSession('rs-01')
     r_name = 'reservation-%s' % int(random.uniform(0, 1000))
     r = rs.request_reservation({'reservation_name': r_name, 'duration': 100})
     print(r)
     r2 = rs.get_reservation(r.id)
-    assert (r2.id == r.id)
+    assert r2.id == r.id
     print('Got reservation: %s' % r)
```

### Comparing `uge-drmaa2-8.8.1/test/test_job_info.py` & `uge-drmaa2-8.9.0/test/test_job_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,151 +16,151 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import datetime
 import socket
-from .utils import generate_random_string
-from .utils import generate_random_int
-from drmaa2 import JobSession
 from drmaa2 import JobInfo
 from drmaa2 import JobState
+from drmaa2 import JobSession
 from drmaa2.drmaa2_constants import POSIX_EPOCH
+from .utils import generate_random_int
+from .utils import generate_random_string
 
 
 def test_job_info_from_job():
     session_name = generate_random_string()
     js = JobSession(session_name)
     jn = 'drmaa2python-%s' % generate_random_string()
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': jn, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
     ji = j.get_info()
-    assert (ji.job_name == jn)
+    assert ji.job_name == jn
     print('\nJob info from job: %s' % (ji))
 
 
 def test_get_implementation_specific_keys():
     keys = JobInfo.get_implementation_specific_keys()
-    assert (len(keys) > 0)
+    assert len(keys) > 0
     print('\nJob info implementation specific keys: %s' % (keys))
 
 
 def test_job_id_attr():
     ji = JobInfo()
     job_id = generate_random_string()
     ji.job_id = job_id
-    assert (ji.job_id == job_id)
+    assert ji.job_id == job_id
     print('\nJob info with job_id: %s' % (job_id))
 
 
 def test_job_name_attr():
     ji = JobInfo()
     job_name = generate_random_string()
     ji.job_name = job_name
-    assert (ji.job_name == job_name)
+    assert ji.job_name == job_name
     print('\nJob info with job_name: %s' % (job_name))
 
 
 def test_exit_status_attr():
     ji = JobInfo()
     exit_status = generate_random_int(lower_bound=0, upper_bound=255)
     ji.exit_status = exit_status
-    assert (ji.exit_status == exit_status)
+    assert ji.exit_status == exit_status
     print('\nJob info with exit_status: %s' % (exit_status))
 
 
 def test_terminating_signal_attr():
     ji = JobInfo()
     terminating_signal = generate_random_string()
     ji.terminating_signal = terminating_signal
-    assert (ji.terminating_signal == terminating_signal)
+    assert ji.terminating_signal == terminating_signal
     print('\nJob info with terminating_signal: %s' % (terminating_signal))
 
 
 def test_annotation_attr():
     ji = JobInfo()
     annotation = generate_random_string()
     ji.annotation = annotation
-    assert (ji.annotation == annotation)
+    assert ji.annotation == annotation
     print('\nJob info with annotation: %s' % (annotation))
 
 
 def test_job_state_attr():
     ji = JobInfo()
     job_state = JobState(generate_random_int(lower_bound=0, upper_bound=9))
     ji.job_state = job_state
-    assert (ji.job_state == job_state.name)
+    assert ji.job_state == job_state.name
     print('\nJob info with job_state: %s' % (job_state))
 
 
 def test_job_sub_state_attr():
     ji = JobInfo()
     job_sub_state = generate_random_string()
     ji.job_sub_state = job_sub_state
-    assert (ji.job_sub_state == job_sub_state)
+    assert ji.job_sub_state == job_sub_state
     print('\nJob info with job_sub_state: %s' % (job_sub_state))
 
 
 def test_allocated_machines_attr():
     allocated_machines = []
     n_allocated_machines = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_allocated_machines):
+    for _ in range(0, n_allocated_machines):
         allocated_machines.append(generate_random_string())
     ji = JobInfo()
     ji.allocated_machines = allocated_machines
-    assert (ji.allocated_machines == allocated_machines)
+    assert ji.allocated_machines == allocated_machines
     print('\nJob info object with %s allocated_machines: %s' % (len(allocated_machines), allocated_machines))
 
 
 def test_submission_machine_attr():
     ji = JobInfo()
     submission_machine = socket.gethostname()
     ji.submission_machine = submission_machine
-    assert (ji.submission_machine == submission_machine)
+    assert ji.submission_machine == submission_machine
     print('\nJob info with submission_machine: %s' % (submission_machine))
 
 
 def test_job_owner_attr():
     ji = JobInfo()
     job_owner = generate_random_string()
     ji.job_owner = job_owner
-    assert (ji.job_owner == job_owner)
+    assert ji.job_owner == job_owner
     print('\nJob info with job_owner: %s' % (job_owner))
 
 
 def test_slots_attr():
     ji = JobInfo()
     slots = generate_random_int(lower_bound=0, upper_bound=1024)
     ji.slots = slots
-    assert (ji.slots == slots)
+    assert ji.slots == slots
     print('\nJob info with slots: %s' % (slots))
 
 
 def test_queue_name_attr():
     ji = JobInfo()
     queue_name = generate_random_string()
     ji.queue_name = queue_name
-    assert (ji.queue_name == queue_name)
+    assert ji.queue_name == queue_name
     print('\nJob info with queue_name: %s' % (queue_name))
 
 
 def test_wallclock_time_attr():
     ji = JobInfo()
     wallclock_time = datetime.datetime.fromtimestamp(generate_random_int(lower_bound=0, upper_bound=12386400))
     ji.wallclock_time = wallclock_time
-    assert (ji.wallclock_time == wallclock_time)
+    assert ji.wallclock_time == wallclock_time
     print('\nJob info with wallclock_time: %s' % (wallclock_time))
 
 
 def test_cpu_time_attr():
     ji = JobInfo()
     cpu_time = generate_random_int(lower_bound=0, upper_bound=86400)
     ji.cpu_time = cpu_time
-    assert (ji.cpu_time == cpu_time)
+    assert ji.cpu_time == cpu_time
     print('\nJob info with cpu_time: %s' % (cpu_time))
 
 
 def test_submission_time_attr():
     submission_time = datetime.datetime.now()
     ji = JobInfo()
     ji.submission_time = submission_time
@@ -189,9 +189,9 @@
     implementation_specific = {}
     keys = JobInfo.get_implementation_specific_keys()
     for k in keys:
         v = generate_random_string()
         implementation_specific[k] = v
     ji = JobInfo()
     ji.implementation_specific = implementation_specific
-    assert (ji.implementation_specific == implementation_specific)
+    assert ji.implementation_specific == implementation_specific
     print('\nJob info object with implementation_specific: %s' % (implementation_specific))
```

### Comparing `uge-drmaa2-8.8.1/test/test_monitoring_session.py` & `uge-drmaa2-8.9.0/test/test_monitoring_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,27 @@
     print('\nGot queue list: %s' % q_name_list)
     ms = MonitoringSession('ms-01')
     qi_list = ms.get_all_queues(q_name_list)
     assert (len(qi_list) == len(q_name_list))
     for qi in qi_list:
         q_name = qi.name
         print('Checking queue: %s' % (qi.to_dict()))
-        assert (q_name in q_name_list)
+        assert q_name in q_name_list
 
 
 def test_get_all_machines():
     h_name_list = os.popen('qconf -sel').read().split()
     print('\nGot host list: %s' % h_name_list)
     ms = MonitoringSession('ms-01')
     mi_list = ms.get_all_machines(h_name_list)
     assert (len(mi_list) == len(h_name_list))
     for mi in mi_list:
         h_name = mi.name
         print('Checking machine: %s' % (mi.to_dict()))
-        assert (h_name in h_name_list)
+        assert h_name in h_name_list
 
 
 def test_get_all_jobs():
     js = JobSession('js-01')
     j_name = 'drmaa2python-%s' % int(random.uniform(0, 1000))
     d = {'remote_command': '/bin/sleep', 'args': ['10'], 'job_name': j_name, 'output_path': '/dev/null', 'join_files': True}
     j = js.run_job(d)
@@ -62,26 +62,26 @@
     j.wait_started()
     ms = MonitoringSession('ms-01')
     print('Opened monitoring session: %s' % ms.name)
     ji2 = JobInfo({'job_id': ji.job_id})
     print('Retrieving jobs matching job info %s' % ji2)
     j_list = ms.get_all_jobs(ji2)
     print('Got all jobs: %s' % j_list)
-    assert (len(j_list) >= 1)
+    assert len(j_list) >= 1
 
 
 def test_get_all_reservatios():
     rs = ReservationSession('rs-01')
     r_name = 'drmaa2python-%s' % int(random.uniform(0, 1000))
     d = {'reservation_name': r_name, 'duration': 100}
     r = rs.request_reservation(d)
     print('\nCreated reservation: %s' % r)
     ri = r.get_info()
-    # At the moment one cannot have both reservation and monitoring 
+    # At the moment one cannot have both reservation and monitoring
     # sessions opened at the same time
     rs.close()
 
     ms = MonitoringSession('ms-01')
     print('Retrieving reservations matching reservation info %s' % ri)
     r_list = ms.get_all_reservations(ri)
     print('Got all reservations: %s' % r_list)
-    assert (len(r_list) == 1)
+    assert len(r_list) == 1
```

### Comparing `uge-drmaa2-8.8.1/test/test_notification.py` & `uge-drmaa2-8.9.0/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/test/test_reservation_template.py` & `uge-drmaa2-8.9.0/test/test_reservation_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,144 +15,144 @@
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
 import datetime
-from .utils import generate_random_string
-from .utils import generate_random_int
-from drmaa2 import ReservationSession
-from drmaa2 import ReservationTemplate
 from drmaa2 import Os
 from drmaa2 import Cpu
+from drmaa2 import ReservationSession
+from drmaa2 import ReservationTemplate
 from drmaa2.drmaa2_constants import POSIX_EPOCH
+from .utils import generate_random_string
+from .utils import generate_random_int
 
 
 def test_reservation_template_from_reservation():
     rs = ReservationSession('rs-01')
     reservation_name = 'r.%s' % generate_random_string()
     r = rs.request_reservation({'reservation_name': reservation_name, 'duration': 100})
     rt = r.get_template()
-    assert (rt.reservation_name == reservation_name)
+    assert rt.reservation_name == reservation_name
     print('\nReservation template from reservation: %s' % (rt))
 
 
 def test_get_implementation_specific_keys():
     keys = ReservationTemplate.get_implementation_specific_keys()
-    assert (len(keys) > 0)
+    assert len(keys) > 0
     print('\nReservation template implementation specific keys: %s' % (keys))
 
 
 def test_reservation_name_attr():
     rt = ReservationTemplate()
     reservation_name = generate_random_string()
     rt.reservation_name = reservation_name
-    assert (rt.reservation_name == reservation_name)
+    assert rt.reservation_name == reservation_name
     print('\nReservation template with reservation_name: %s' % (reservation_name))
 
 
 def test_start_time_attr():
     start_time = datetime.datetime.now()
     rt = ReservationTemplate()
     rt.start_time = start_time
-    assert (int((rt.start_time - POSIX_EPOCH).total_seconds()) == int((start_time - POSIX_EPOCH).total_seconds()))
+    assert int((rt.start_time - POSIX_EPOCH).total_seconds()) == int((start_time - POSIX_EPOCH).total_seconds())
     print('\nReservation template object with start_time: %s' % (start_time))
 
 
 def test_end_time_attr():
     end_time = datetime.datetime.now() + datetime.timedelta(hours=24)
     rt = ReservationTemplate()
     rt.end_time = end_time
-    assert (int((rt.end_time - POSIX_EPOCH).total_seconds()) == int((end_time - POSIX_EPOCH).total_seconds()))
+    assert int((rt.end_time - POSIX_EPOCH).total_seconds()) == int((end_time - POSIX_EPOCH).total_seconds())
     print('\nReservation template object with end_time: %s' % (end_time))
 
 
 def test_duration_attr():
     rt = ReservationTemplate()
     duration = generate_random_int(lower_bound=1, upper_bound=86400)
     rt.duration = duration
-    assert (rt.duration == duration)
+    assert rt.duration == duration
     print('\nReservation template with duration: %s' % (duration))
 
 
 def test_min_slots_attr():
     rt = ReservationTemplate()
     min_slots = generate_random_int(lower_bound=1, upper_bound=1024)
     rt.min_slots = min_slots
-    assert (rt.min_slots == min_slots)
+    assert rt.min_slots == min_slots
     print('\nReservation template with min_slots: %s' % (min_slots))
 
 
 def test_max_slots_attr():
     rt = ReservationTemplate()
     max_slots = generate_random_int(lower_bound=1, upper_bound=1024)
     rt.max_slots = max_slots
-    assert (rt.max_slots == max_slots)
+    assert rt.max_slots == max_slots
     print('\nReservation template with max_slots: %s' % (max_slots))
 
 
 def test_job_category_attr():
     rt = ReservationTemplate()
     job_category = generate_random_string()
     rt.job_category = job_category
-    assert (rt.job_category == job_category)
+    assert rt.job_category == job_category
     print('\nReservation template with job_category: %s' % (job_category))
 
 
 def test_users_acl_attr():
     users_acl = []
     n_users_acl = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_users_acl):
+    for _ in range(0, n_users_acl):
         users_acl.append(generate_random_string())
     rt = ReservationTemplate()
     rt.users_acl = users_acl
-    assert (rt.users_acl == users_acl)
+    assert rt.users_acl == users_acl
     print('\nreservation template object with %s users_acl: %s' % (len(users_acl), users_acl))
 
 
 def test_candidate_machines_attr():
     candidate_machines = []
     n_candidate_machines = generate_random_int(lower_bound=1, upper_bound=5)
-    for i in range(0, n_candidate_machines):
+    for _ in range(0, n_candidate_machines):
         candidate_machines.append(generate_random_string())
     rt = ReservationTemplate()
     rt.candidate_machines = candidate_machines
-    assert (rt.candidate_machines == candidate_machines)
+    assert rt.candidate_machines == candidate_machines
     print(
         '\nreservation template object with %s candidate_machines: %s' % (len(candidate_machines), candidate_machines))
 
 
 def test_min_phys_memory_attr():
     rt = ReservationTemplate()
     min_phys_memory = generate_random_int(lower_bound=1, upper_bound=86400)
     rt.min_phys_memory = min_phys_memory
-    assert (rt.min_phys_memory == min_phys_memory)
+    assert rt.min_phys_memory == min_phys_memory
     print('\nReservation template with min_phys_memory: %s' % (min_phys_memory))
 
 
 def test_machine_os_attr():
     rt = ReservationTemplate()
     machine_os = generate_random_int(lower_bound=0, upper_bound=11)
     rt.machine_os = machine_os
-    assert (rt.machine_os == Os(machine_os).name)
+    assert rt.machine_os == Os(machine_os).name
     print('\nReservation template with machine_os: %s' % (machine_os))
 
 
 def test_machine_arch_attr():
     machine_arch = generate_random_int(lower_bound=0, upper_bound=16)
     rt = ReservationTemplate()
     rt.machine_arch = machine_arch
-    assert (rt.machine_arch == Cpu(machine_arch).name)
+    assert rt.machine_arch == Cpu(machine_arch).name
     print('\nReservation template object with machine_arch: %s' % (machine_arch))
 
 
 def test_implementation_specific_attr():
     implementation_specific = {}
     keys = ReservationTemplate.get_implementation_specific_keys()
     for k in keys:
         v = generate_random_string()
         implementation_specific[k] = v
     rt = ReservationTemplate()
     rt.implementation_specific = implementation_specific
-    assert (rt.implementation_specific == implementation_specific)
+    assert rt.implementation_specific == implementation_specific
     print('\nReservation template object with implementation_specific: %s' % (implementation_specific))
```

### Comparing `uge-drmaa2-8.8.1/test/test_queue_info.py` & `uge-drmaa2-8.9.0/test/test_queue_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
 
 def test_queue_info():
     q_name_list = os.popen('qconf -sql').read().split()
     print('\nGot queue list: %s' % q_name_list)
     ms = MonitoringSession('ms-01')
     qi_list = ms.get_all_queues(q_name_list)
-    assert (len(qi_list) > 0)
+    assert len(qi_list) > 0
     for qi in qi_list:
         q_name = qi.name
         print('\nChecking queue: %s' % (qi.to_dict()))
-        assert (q_name in q_name_list)
+        assert q_name in q_name_list
```

### Comparing `uge-drmaa2-8.8.1/test/test_sudo.py` & `uge-drmaa2-8.9.0/test/test_sudo.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #######################################################################################
 # ___INFO__MARK_END__
 
-from .utils import generate_random_string
-from .utils import generate_random_int
 from drmaa2 import Sudo
 from drmaa2 import Drmaa2Exception
+from .utils import generate_random_string
+from .utils import generate_random_int
 
 
 def test_username_attr():
     username = generate_random_string()
     s = Sudo()
     s.username = username
-    assert (s.username == username)
+    assert s.username == username
     s2 = Sudo(username=username)
-    assert (s2.username == username)
+    assert s2.username == username
     s3 = Sudo(sudo_dict={'username': username})
-    assert (s3.username == username)
+    assert s3.username == username
     print('\nSudo object with username: %s' % (username))
 
 
 def test_groupname_attr():
     groupname = generate_random_string()
     s = Sudo()
     s.groupname = groupname
-    assert (s.groupname == groupname)
+    assert s.groupname == groupname
     s2 = Sudo(groupname=groupname)
-    assert (s2.groupname == groupname)
+    assert s2.groupname == groupname
     s3 = Sudo(sudo_dict={'groupname': groupname})
-    assert (s3.groupname == groupname)
+    assert s3.groupname == groupname
     print('\nSudo object with groupname: %s' % (groupname))
 
 
 def test_uid_attr():
     uid = generate_random_int()
     s = Sudo()
     s.uid = uid
@@ -60,13 +60,13 @@
     print('\nSudo object with uid: %s' % (uid))
 
 
 def test_gid_attr():
     gid = generate_random_int()
     s = Sudo()
     s.gid = gid
-    assert (s.gid == gid)
+    assert s.gid == gid
     s2 = Sudo(gid=gid)
-    assert (s2.gid == gid)
+    assert s2.gid == gid
     s3 = Sudo(sudo_dict={'gid': gid})
-    assert (s3.gid == gid)
+    assert s3.gid == gid
     print('\nSudo object with gid: %s' % (gid))
```

### Comparing `uge-drmaa2-8.8.1/test/test_version.py` & `uge-drmaa2-8.9.0/test/test_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     assert (v.major != '' and v.minor != '')
     print('\nGot DRMAA version: %s' % (v))
 
 
 def test_to_dict():
     v = Version.get_drmaa_version()
     d = v.to_dict()
-    assert (v.major == d['major'])
-    assert (v.minor == d['minor'])
+    assert v.major == d['major']
+    assert v.minor == d['minor']
     print('\nVersion object conversion to dictionary: %s' % (d))
 
 
 def test_get_implementation_specific_keys():
     keys = Version.get_implementation_specific_keys()
-    assert (keys is not None)
+    assert keys is not None
     print('\nVersion object has %s impl specific keys %s.' % (len(keys), keys))
 
 
 def test_get_implementation_specific_attrs():
     attrs = Version.get_implementation_specific_attrs()
-    assert (attrs is not None)
+    assert attrs is not None
     print('\nVersion object has %s impl specific attrs %s.' % (len(attrs), attrs))
```

### Comparing `uge-drmaa2-8.8.1/test/test_drmaa2_init.py` & `uge-drmaa2-8.9.0/test/test_drmaa2_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,39 +31,39 @@
     v = drmaa2.get_drmaa_version()
     assert (v.major != '' and v.minor != '')
     print('\nGot DRMAA version: %s' % (v))
 
 
 def test_get_drms_name():
     n = drmaa2.get_drms_name()
-    assert (n != '')
+    assert n != ''
     print('\nGot DRMS name: %s' % (n))
 
 
 def test_get_drmaa_name():
     n = drmaa2.get_drmaa_name()
-    assert (n != '')
+    assert n != ''
     print('\nGot DRMAA name: %s' % (n))
 
 
 def test_drmaa_supports():
     print('\nVerifying support for %s capabilities' % (len(drmaa2.Capability)))
     supported = []
     for c in drmaa2.Capability:
         s = drmaa2.drmaa_supports(c)
         if s:
             supported.append(s)
         print('Support for %s: %s' % (c, s))
-    assert (len(supported) > 0)
+    assert len(supported) > 0
     print('DRMAA2 supports %s out of %s capabilities' % (len(supported), len(drmaa2.Capability)))
 
 
 def test_get_job_session_names():
     sessions = drmaa2.get_job_session_names()
-    assert (type(sessions) == type([]))
+    assert type(sessions) == type([])
     print('\nGot %s job sessions: %s' % (len(sessions), sessions))
 
 
 def test_get_reservation_session_names():
     sessions = drmaa2.get_reservation_session_names()
-    assert (type(sessions) == type([]))
+    assert type(sessions) == type([])
     print('\nGot %s reservation sessions: %s' % (len(sessions), sessions))
```

### Comparing `uge-drmaa2-8.8.1/README.rst` & `uge-drmaa2-8.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/uge_drmaa2.egg-info/SOURCES.txt` & `uge-drmaa2-8.9.0/uge_drmaa2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uge-drmaa2-8.8.1/uge_drmaa2.egg-info/PKG-INFO` & `uge-drmaa2-8.9.0/uge_drmaa2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: uge-drmaa2
-Version: 8.8.1
+Version: 8.9.0
 Summary: UGE DRMAA2 Python API
 Home-page: https://www.altair.com
 Author: Altair Engineering Inc.
 Author-email: support@altair.com
 License: Apache 2.0
 Description: (c) Copyright 2008-2022 Altair Engineering Inc.
             Licensed under the Apache License, Version 2.0 (the "License"); you may not
```

### Comparing `uge-drmaa2-8.8.1/setup.py` & `uge-drmaa2-8.9.0/setup.py`

 * *Files identical despite different names*

