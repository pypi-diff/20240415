# Comparing `tmp/alas-ce0-client-5.0.78.tar.gz` & `tmp/alas-ce0-client-5.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alas-ce0-client-5.0.78.tar", last modified: Thu Mar 14 12:19:41 2024, max compression
+gzip compressed data, was "alas-ce0-client-5.0.80.tar", last modified: Mon Apr 15 14:53:05 2024, max compression
```

## Comparing `alas-ce0-client-5.0.78.tar` & `alas-ce0-client-5.0.80.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.151336 alas-ce0-client-5.0.78/
--rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/LICENSE.txt
--rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/MANIFEST.in
--rw-r--r--   0 lzambra    (501) staff       (20)      955 2024-03-14 12:19:41.151047 alas-ce0-client-5.0.78/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/README.rst
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.115693 alas-ce0-client-5.0.78/alas_ce0/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/__init__.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.117614 alas-ce0-client-5.0.78/alas_ce0/clients/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)     6223 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/api_client.py
--rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/clients/core.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.118642 alas-ce0-client-5.0.78/alas_ce0/common/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/common/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/common/client_base.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.124001 alas-ce0-client-5.0.78/alas_ce0/delivery/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/b2c.py
--rw-r--r--   0 lzambra    (501) staff       (20)    51736 2024-03-10 18:52:47.000000 alas-ce0-client-5.0.78/alas_ce0/delivery/delivery_order.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.129163 alas-ce0-client-5.0.78/alas_ce0/integration/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/device_magic.py
--rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/shipper.py
--rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/integration/whatsapp.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.143556 alas-ce0-client-5.0.78/alas_ce0/management/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/barcode.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1511 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/bulk.py
--rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/configuration.py
--rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/contact.py
--rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/cross_docking.py
--rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/delivery_entity.py
--rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/distribution_zone.py
--rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/employee.py
--rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/feature.py
--rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-5.0.78/alas_ce0/management/geographic_coverage.py
--rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/geographic_coverage_active.py
--rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/maintenance.py
--rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/notification.py
--rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/package_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/packaging.py
--rw-r--r--   0 lzambra    (501) staff       (20)      732 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/pallet.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2024-02-12 13:10:27.000000 alas-ce0-client-5.0.78/alas_ce0/management/position.py
--rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/product_template.py
--rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/resource.py
--rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/role.py
--rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/roles_group.py
--rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/service_level.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/shelf.py
--rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/task.py
--rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/user.py
--rw-r--r--   0 lzambra    (501) staff       (20)      591 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.78/alas_ce0/management/user_app.py
--rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/management/vehicle.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.145181 alas-ce0-client-5.0.78/alas_ce0/reporting/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/regional_partner_report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/report.py
--rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/reporting/report_manager.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.145940 alas-ce0-client-5.0.78/alas_ce0/scheduling/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/scheduling/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/scheduling/route.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.146869 alas-ce0-client-5.0.78/alas_ce0/task/
--rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/task/__init__.py
--rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.78/alas_ce0/task/data_job.py
-drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-03-14 12:19:41.150188 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/
--rw-r--r--   0 lzambra    (501) staff       (20)      955 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/PKG-INFO
--rw-r--r--   0 lzambra    (501) staff       (20)     1852 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/SOURCES.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        1 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/dependency_links.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       48 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/requires.txt
--rw-r--r--   0 lzambra    (501) staff       (20)        9 2024-03-14 12:19:41.000000 alas-ce0-client-5.0.78/alas_ce0_client.egg-info/top_level.txt
--rw-r--r--   0 lzambra    (501) staff       (20)       67 2024-03-14 12:19:41.151950 alas-ce0-client-5.0.78/setup.cfg
--rw-r--r--   0 lzambra    (501) staff       (20)     3807 2024-03-14 12:11:49.000000 alas-ce0-client-5.0.78/setup.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.999564 alas-ce0-client-5.0.80/
+-rw-r--r--   0 lzambra    (501) staff       (20)       23 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/LICENSE.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)      238 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/MANIFEST.in
+-rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-04-15 14:53:04.999284 alas-ce0-client-5.0.80/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)      260 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/README.rst
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.965331 alas-ce0-client-5.0.80/alas_ce0/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/__init__.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.966369 alas-ce0-client-5.0.80/alas_ce0/clients/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/clients/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     6256 2024-04-13 01:17:08.000000 alas-ce0-client-5.0.80/alas_ce0/clients/api_client.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      748 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/clients/core.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.967005 alas-ce0-client-5.0.80/alas_ce0/common/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/common/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    12200 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/common/client_base.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.968133 alas-ce0-client-5.0.80/alas_ce0/delivery/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/delivery/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      307 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/delivery/b2c.py
+-rw-r--r--   0 lzambra    (501) staff       (20)    51663 2024-04-15 14:38:13.000000 alas-ce0-client-5.0.80/alas_ce0/delivery/delivery_order.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.969861 alas-ce0-client-5.0.80/alas_ce0/integration/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/integration/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      596 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/integration/device_magic.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      274 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/integration/shipper.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      283 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/integration/whatsapp.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.984740 alas-ce0-client-5.0.80/alas_ce0/management/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      609 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/barcode.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1511 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.80/alas_ce0/management/bulk.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      531 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/configuration.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      152 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/contact.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      362 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/cross_docking.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     1066 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/delivery_entity.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      349 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/distribution_zone.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      917 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/employee.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      153 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/feature.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      492 2022-08-17 20:26:11.000000 alas-ce0-client-5.0.80/alas_ce0/management/geographic_coverage.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      462 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/geographic_coverage_active.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      337 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/maintenance.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      757 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/notification.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      298 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/package_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      352 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/packaging.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      732 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.80/alas_ce0/management/pallet.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2024-02-12 13:10:27.000000 alas-ce0-client-5.0.80/alas_ce0/management/position.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      169 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/product_template.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      155 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/resource.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      147 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/role.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      160 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/roles_group.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      336 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/service_level.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/shelf.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      400 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/task.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      584 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/user.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      591 2024-02-12 13:05:56.000000 alas-ce0-client-5.0.80/alas_ce0/management/user_app.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      316 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/management/vehicle.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.987792 alas-ce0-client-5.0.80/alas_ce0/reporting/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/reporting/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      323 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/reporting/regional_partner_report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      495 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/reporting/report.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      311 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/reporting/report_manager.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.989375 alas-ce0-client-5.0.80/alas_ce0/scheduling/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/scheduling/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)     2412 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/scheduling/route.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.991499 alas-ce0-client-5.0.80/alas_ce0/task/
+-rw-r--r--   0 lzambra    (501) staff       (20)        0 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/task/__init__.py
+-rw-r--r--   0 lzambra    (501) staff       (20)      289 2022-07-06 21:05:07.000000 alas-ce0-client-5.0.80/alas_ce0/task/data_job.py
+drwxr-xr-x   0 lzambra    (501) staff       (20)        0 2024-04-15 14:53:04.997997 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/
+-rw-r--r--   0 lzambra    (501) staff       (20)      976 2024-04-15 14:53:04.000000 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/PKG-INFO
+-rw-r--r--   0 lzambra    (501) staff       (20)     1852 2024-04-15 14:53:04.000000 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/SOURCES.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        1 2024-04-15 14:53:04.000000 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/dependency_links.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       55 2024-04-15 14:53:04.000000 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/requires.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)        9 2024-04-15 14:53:04.000000 alas-ce0-client-5.0.80/alas_ce0_client.egg-info/top_level.txt
+-rw-r--r--   0 lzambra    (501) staff       (20)       67 2024-04-15 14:53:05.000388 alas-ce0-client-5.0.80/setup.cfg
+-rw-r--r--   0 lzambra    (501) staff       (20)     3825 2024-04-15 14:52:52.000000 alas-ce0-client-5.0.80/setup.py
```

### Comparing `alas-ce0-client-5.0.78/PKG-INFO` & `alas-ce0-client-5.0.80/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 5.0.78
+Version: 5.0.80
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Keywords: alas-ce0 api client development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 2.7
 License-File: LICENSE.txt
+Requires-Dist: enum34
 Requires-Dist: httplib2
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 Alas Ce0 Client API
```

### Comparing `alas-ce0-client-5.0.78/alas_ce0/clients/api_client.py` & `alas-ce0-client-5.0.80/alas_ce0/clients/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import contextlib
-import httplib
+import http.client as httplib
 import json
-import urlparse
+import urllib.parse as urlparse
 import ssl
 from requests_toolbelt.utils import dump
 
 from requests.auth import HTTPBasicAuth
 
 
 class ApiHttpClientException(Exception):
@@ -55,15 +55,15 @@
     def _get_client(self):
         url_parsed = urlparse.urlparse(self.base_url)
 
         if self.http_debug:
             old_send = httplib.HTTPConnection.send
 
             def new_send(self, data):
-                print data
+                print (data)
                 return old_send(self, data)
 
             httplib.HTTPConnection.send = new_send
 
         if url_parsed.scheme == 'http':
             yield httplib.HTTPConnection(
                 url_parsed.hostname,
```

### Comparing `alas-ce0-client-5.0.78/alas_ce0/clients/core.py` & `alas-ce0-client-5.0.80/alas_ce0/clients/core.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/common/client_base.py` & `alas-ce0-client-5.0.80/alas_ce0/common/client_base.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/delivery/delivery_order.py` & `alas-ce0-client-5.0.80/alas_ce0/delivery/delivery_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,263 +666,236 @@
         return event_info['schedule_rejected_3_comments']
     return None
 
 def get_status_info_wom(delivery_order):
     events_info, status, last_event_timestamp = None, None, None
 
     if delivery_order['status'] == DeliveryOrderStatusType.PhysicallyReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Despacho recepcionado'
 
     elif delivery_order['status'] == DeliveryOrderStatusType.B2BReceptionRejected.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Orden Cancelada por Logística'
 
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.B2CTraveling.value,
                                       DeliveryOrderStatusType.DeliveryCourierReceived.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Despacho en ruta'
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.NotDelivered.value, DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotExchanged.value, DeliveryOrderStatusType.NotExchangable.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = "Intento {}".format( str(delivery_order['delivery_attemps']) )
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.Delivered.value, DeliveryOrderStatusType.Exchanged.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Entregado'
 
     #elif delivery_order['status'] == DeliveryOrderStatusType.NotDeliverable.value:
-    #    events_info = filter(
-    #        lambda x: x['status'] == delivery_order['status'],
-    #        delivery_order['events_info']
-    #    )
+    #    events_info = list(filter(
+    #        lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+    #    ))
     #    status = 'Orden Cancelada'
 
     elif delivery_order['status'] == DeliveryOrderStatusType.B2CReceptionRejected.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Cliente desiste'
 
     elif delivery_order['status'] == DeliveryOrderStatusType.ALASRejected.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'No Entregado'
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.Steal.value, DeliveryOrderStatusType.Missing.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Mermada'
 
     else:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
 
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
     if events_info:
         last_event_timestamp = events_info[len(events_info) - 1]['timestamp'].split('.')[0]
 
     return status, last_event_timestamp
 
 def get_status_info(delivery_order, r_reason = False):
     events_info, status, description, last_event_timestamp = None, None, None, None
 
     if delivery_order['status'] == DeliveryOrderStatusType.Planning.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.VirtuallyReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Planificación'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.PhysicallyReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Recepción Física'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.B2BReceptionRejected.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Rechazada B2B'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DistributionCenterReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.SERTravelling.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Viajando SER'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.SERReceived.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryConfirmed.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Entrega Agendada'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryNotConfirmed.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Entrega Agendada'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.DeliveryScheduled.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.B2CTraveling.value, DeliveryOrderStatusType.DeliveryCourierReceived.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'En Ruta'
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.NotDelivered.value, DeliveryOrderStatusType.NotExchanged.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
 
     elif delivery_order['status'] == DeliveryOrderStatusType.Delivered.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Entregado'
         description = 'Entrega realizada'
 
     elif delivery_order['status'] == DeliveryOrderStatusType.Exchanged.value:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status = 'Intercambiada'
         description = 'Intercambio realizada'
 
     elif delivery_order['status'] in DELIVERY_ORDER_REJECTED_STATUSES:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description = get_rejected_reason(events_info[len(events_info) - 1]['info'])
         if description is None:
             description = "Entrega Rechazada"
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotExchangable.value]:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] if delivery_order['status'] in description_dic else status
     else:
-        events_info = filter(
-            lambda x: x['status'] == delivery_order['status'],
-            delivery_order['events_info']
-        )
+        events_info = list(filter(
+            lambda x: x['status'] == delivery_order['status'], delivery_order['events_info']
+        ))
 
         status_dic = get_delivery_order_status_dic()
         status = status_dic[delivery_order['status']]
 
         description_dic = get_delivery_order_status_description_dic()
         description = description_dic[delivery_order['status']] \
             if delivery_order['status'] in description_dic \
@@ -942,16 +915,24 @@
             reason = reason_dic[reason]
 
         return status, description, last_event_timestamp, reason
 
     return status, description, last_event_timestamp
 
 def get_macro_status(delivery_order):
-    in_route_amount = len(filter(lambda x: x == 17, delivery_order['statuses']))
-    in_quarantine_amount = len(filter(lambda x: x == 52, delivery_order['statuses']))
+    in_route_amount = len(
+        list(filter(
+            lambda x: x == 17, delivery_order['statuses']
+        ))
+    )
+    in_quarantine_amount = len(
+        list(filter(
+            lambda x: x == 52, delivery_order['statuses']
+        ))
+    )
     status = get_delivery_order_status_dic()
 
     if delivery_order['status'] in [
         DeliveryOrderStatusType.DeliveryRejected.value,
         DeliveryOrderStatusType.B2CRejected.value,
         DeliveryOrderStatusType.B2CReceptionRejected.value]:
         return 'Rechazado Cliente'
@@ -974,21 +955,21 @@
 
     elif delivery_order['status'] in [DeliveryOrderStatusType.NotDeliverable.value, DeliveryOrderStatusType.NotWithdrawn.value, DeliveryOrderStatusType.NotExchangable.value]:
         return 'Rechazado 3 Intentos'
 
     return status[delivery_order['status']]
 
 def get_b2c_delivery_events(delivery_order):
-    return filter(
+    return list(filter(
         lambda x: (x['status'] == 15 and 'b2c_delivery_actual' in x['info']) or
                     x['status'] == 18 or
                     x['status'] == 19 or
                     x['status'] in DELIVERY_ORDER_REJECTED_STATUSES,
         delivery_order['events_info']
-    )
+    ))
     
 def get_not_delivered_reason(event_info):
     reasons = ['No hay quien reciba', 'Dirección Incompleta', 'Problema Documentación', 'Código Erróneo', 'Paso Automatico', 'Siniestro', 'Merma']
 
     if 'not_delivered_3_reason' in event_info and event_info['not_delivered_3_reason']:
         return reasons[event_info['not_delivered_3_reason'] - 1]
     if 'not_delivered_2_reason' in event_info and event_info['not_delivered_2_reason']:
```

### Comparing `alas-ce0-client-5.0.78/alas_ce0/integration/device_magic.py` & `alas-ce0-client-5.0.80/alas_ce0/integration/device_magic.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/barcode.py` & `alas-ce0-client-5.0.80/alas_ce0/management/barcode.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/bulk.py` & `alas-ce0-client-5.0.80/alas_ce0/management/bulk.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/configuration.py` & `alas-ce0-client-5.0.80/alas_ce0/management/configuration.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/delivery_entity.py` & `alas-ce0-client-5.0.80/alas_ce0/management/delivery_entity.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/employee.py` & `alas-ce0-client-5.0.80/alas_ce0/management/employee.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/notification.py` & `alas-ce0-client-5.0.80/alas_ce0/management/notification.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/pallet.py` & `alas-ce0-client-5.0.80/alas_ce0/management/pallet.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/user.py` & `alas-ce0-client-5.0.80/alas_ce0/management/user.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/management/user_app.py` & `alas-ce0-client-5.0.80/alas_ce0/management/user_app.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0/scheduling/route.py` & `alas-ce0-client-5.0.80/alas_ce0/scheduling/route.py`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/alas_ce0_client.egg-info/PKG-INFO` & `alas-ce0-client-5.0.80/alas_ce0_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: alas-ce0-client
-Version: 5.0.78
+Version: 5.0.80
 Summary: API client for Alas.Ce0 project
 Home-page: https://github.com/pypa/alas-ce0-client
 Author: Leonardo Zambra
 Author-email: lzambra@alasxpress.com
 License: MIT
 Keywords: alas-ce0 api client development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 2.7
 License-File: LICENSE.txt
+Requires-Dist: enum34
 Requires-Dist: httplib2
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 Alas Ce0 Client API
```

### Comparing `alas-ce0-client-5.0.78/alas_ce0_client.egg-info/SOURCES.txt` & `alas-ce0-client-5.0.80/alas_ce0_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alas-ce0-client-5.0.78/setup.py` & `alas-ce0-client-5.0.80/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-API_CLIENT_VERSION = '5.0.78'
+API_CLIENT_VERSION = '5.0.80'
 
 setup(
     name='alas-ce0-client',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
@@ -53,16 +53,16 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 3 or both.
-        'Programming Language :: Python :: 3.10',
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 2.7',
     ],
 
     # What does your project relate to?
     keywords='alas-ce0 api client development',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
@@ -72,15 +72,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['httplib2'],\
+    install_requires=['enum34', 'httplib2'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': ['check-manifest'],
```

