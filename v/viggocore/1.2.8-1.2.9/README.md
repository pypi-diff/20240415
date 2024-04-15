# Comparing `tmp/viggocore-1.2.8.tar.gz` & `tmp/viggocore-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggocore-1.2.8.tar", last modified: Wed Jan 24 20:33:29 2024, max compression
+gzip compressed data, was "viggocore-1.2.9.tar", last modified: Fri Jan 26 13:46:51 2024, max compression
```

## Comparing `viggocore-1.2.8.tar` & `viggocore-1.2.9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-24 20:33:01.000000 viggocore-1.2.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 20:33:01.000000 viggocore-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-24 20:33:29.013645 viggocore-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-24 20:33:01.000000 viggocore-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 20:33:29.013645 viggocore-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-24 20:33:01.000000 viggocore-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.001645 viggocore-1.2.8/viggocore/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/bootstrap/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/default/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/default/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/default/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/default/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/bootstrap/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/operation_after_post.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/common/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/apihandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/subsystem/transaction_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/application/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/application/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/application/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/application/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/application/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/capability/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/capability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/capability/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/capability/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/domain/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/files/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.005645 viggocore-1.2.8/viggocore/subsystem/domain/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/sql/disk_space_totals_by_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/domain_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/domain_sequence/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/file/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/file_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/file_sync/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/grant/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/grant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/grant/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/image/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/image/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/notification/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/notification/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/policy/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/project_cost/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/project_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/project_cost/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/project_cost/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/registration/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/registration/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/registration/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/role/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/role/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/role/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/role/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/role/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/route/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/route/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/route/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.009645 viggocore-1.2.8/viggocore/subsystem/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/tag/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/tag/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/tag/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/tag/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/viggocore/subsystem/timeline_event/
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/timeline_event/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1696 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/timeline_event/controller.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/timeline_event/manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2798 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/timeline_event/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/viggocore/subsystem/token/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/token/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/token/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/token/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/token/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/viggocore/subsystem/user/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/subsystem/user/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/viggocore/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.013645 viggocore-1.2.8/viggocore/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_grants_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-24 20:33:01.000000 viggocore-1.2.8/viggocore/tests/functional/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:33:29.001645 viggocore-1.2.8/viggocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-24 20:33:28.000000 viggocore-1.2.8/viggocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-24 20:33:28.000000 viggocore-1.2.8/viggocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:33:28.000000 viggocore-1.2.8/viggocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-24 20:33:28.000000 viggocore-1.2.8/viggocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-24 20:33:28.000000 viggocore-1.2.8/viggocore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-26 13:46:15.000000 viggocore-1.2.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-26 13:46:15.000000 viggocore-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-26 13:46:51.174111 viggocore-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-26 13:46:15.000000 viggocore-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 13:46:51.174111 viggocore-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-01-26 13:46:15.000000 viggocore-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/bootstrap/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/default/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/bootstrap/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/operation_after_post.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/common/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/apihandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/subsystem/transaction_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/application/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.162111 viggocore-1.2.9/viggocore/subsystem/capability/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/capability/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/files/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/sql/disk_space_totals_by_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/domain_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/domain_sequence/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/file_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/file_sync/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.166111 viggocore-1.2.9/viggocore/subsystem/grant/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/grant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/grant/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/image/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/notification/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/policy/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/project_cost/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/project_cost/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/registration/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/role/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/role/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/route/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/route/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/tag/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/timeline_event/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1696 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/controller.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2798 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/timeline_event/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.170112 viggocore-1.2.9/viggocore/subsystem/token/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/token/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/subsystem/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/subsystem/user/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.174111 viggocore-1.2.9/viggocore/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_grants_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-26 13:46:15.000000 viggocore-1.2.9/viggocore/tests/functional/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:46:51.158111 viggocore-1.2.9/viggocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-26 13:46:51.000000 viggocore-1.2.9/viggocore.egg-info/top_level.txt
```

### Comparing `viggocore-1.2.8/LICENSE` & `viggocore-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/README.md` & `viggocore-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/setup.py` & `viggocore-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/__init__.py` & `viggocore-1.2.9/viggocore/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/__init__.py` & `viggocore-1.2.9/viggocore/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/default/__init__.py` & `viggocore-1.2.9/viggocore/bootstrap/default/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/default/application.py` & `viggocore-1.2.9/viggocore/bootstrap/default/application.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/default/domain.py` & `viggocore-1.2.9/viggocore/bootstrap/default/domain.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/default/policies.py` & `viggocore-1.2.9/viggocore/bootstrap/default/policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/default/user.py` & `viggocore-1.2.9/viggocore/bootstrap/default/user.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/roles.py` & `viggocore-1.2.9/viggocore/bootstrap/roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/bootstrap/routes.py` & `viggocore-1.2.9/viggocore/bootstrap/routes.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/celery.py` & `viggocore-1.2.9/viggocore/celery.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/controller.py` & `viggocore-1.2.9/viggocore/common/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/exception.py` & `viggocore-1.2.9/viggocore/common/exception.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/input.py` & `viggocore-1.2.9/viggocore/common/input.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/manager.py` & `viggocore-1.2.9/viggocore/common/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/operation_after_post.py` & `viggocore-1.2.9/viggocore/common/operation_after_post.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/__init__.py` & `viggocore-1.2.9/viggocore/common/subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/apihandler.py` & `viggocore-1.2.9/viggocore/common/subsystem/apihandler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/controller.py` & `viggocore-1.2.9/viggocore/common/subsystem/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/driver.py` & `viggocore-1.2.9/viggocore/common/subsystem/driver.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/entity.py` & `viggocore-1.2.9/viggocore/common/subsystem/entity.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/manager.py` & `viggocore-1.2.9/viggocore/common/subsystem/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/operation.py` & `viggocore-1.2.9/viggocore/common/subsystem/operation.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/pagination.py` & `viggocore-1.2.9/viggocore/common/subsystem/pagination.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/subsystem/router.py` & `viggocore-1.2.9/viggocore/common/subsystem/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/common/utils.py` & `viggocore-1.2.9/viggocore/common/utils.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/queue.py` & `viggocore-1.2.9/viggocore/queue.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/request.py` & `viggocore-1.2.9/viggocore/request.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/resources.py` & `viggocore-1.2.9/viggocore/resources.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/scheduler.py` & `viggocore-1.2.9/viggocore/scheduler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/application/controller.py` & `viggocore-1.2.9/viggocore/subsystem/application/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/application/manager.py` & `viggocore-1.2.9/viggocore/subsystem/application/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/application/resource.py` & `viggocore-1.2.9/viggocore/subsystem/application/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/application/router.py` & `viggocore-1.2.9/viggocore/subsystem/application/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/capability/manager.py` & `viggocore-1.2.9/viggocore/subsystem/capability/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/capability/resource.py` & `viggocore-1.2.9/viggocore/subsystem/capability/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/controller.py` & `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/manager.py` & `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/resource.py` & `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/constant_for_calculation/router.py` & `viggocore-1.2.9/viggocore/subsystem/constant_for_calculation/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/controller.py` & `viggocore-1.2.9/viggocore/subsystem/domain/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/files/utils.py` & `viggocore-1.2.9/viggocore/subsystem/domain/files/utils.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/manager.py` & `viggocore-1.2.9/viggocore/subsystem/domain/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/resource.py` & `viggocore-1.2.9/viggocore/subsystem/domain/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/router.py` & `viggocore-1.2.9/viggocore/subsystem/domain/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain/tasks.py` & `viggocore-1.2.9/viggocore/subsystem/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/controller.py` & `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/manager.py` & `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/resource.py` & `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_and_table_sequence/router.py` & `viggocore-1.2.9/viggocore/subsystem/domain_and_table_sequence/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_sequence/controller.py` & `viggocore-1.2.9/viggocore/subsystem/domain_sequence/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_sequence/manager.py` & `viggocore-1.2.9/viggocore/subsystem/domain_sequence/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_sequence/resource.py` & `viggocore-1.2.9/viggocore/subsystem/domain_sequence/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/domain_sequence/router.py` & `viggocore-1.2.9/viggocore/subsystem/domain_sequence/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/file/controller.py` & `viggocore-1.2.9/viggocore/subsystem/file/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/file/manager.py` & `viggocore-1.2.9/viggocore/subsystem/file/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/file/resource.py` & `viggocore-1.2.9/viggocore/subsystem/file/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/file_sync/resource.py` & `viggocore-1.2.9/viggocore/subsystem/file_sync/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/grant/resource.py` & `viggocore-1.2.9/viggocore/subsystem/grant/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/image/controller.py` & `viggocore-1.2.9/viggocore/subsystem/image/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/image/handler.py` & `viggocore-1.2.9/viggocore/subsystem/image/handler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/image/manager.py` & `viggocore-1.2.9/viggocore/subsystem/image/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/image/resource.py` & `viggocore-1.2.9/viggocore/subsystem/image/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/image/router.py` & `viggocore-1.2.9/viggocore/subsystem/image/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/notification/resource.py` & `viggocore-1.2.9/viggocore/subsystem/notification/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/policy/resource.py` & `viggocore-1.2.9/viggocore/subsystem/policy/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/project_cost/resource.py` & `viggocore-1.2.9/viggocore/subsystem/project_cost/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/registration/controller.py` & `viggocore-1.2.9/viggocore/subsystem/registration/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/registration/router.py` & `viggocore-1.2.9/viggocore/subsystem/registration/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/role/controller.py` & `viggocore-1.2.9/viggocore/subsystem/role/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/role/manager.py` & `viggocore-1.2.9/viggocore/subsystem/role/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/role/resource.py` & `viggocore-1.2.9/viggocore/subsystem/role/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/route/manager.py` & `viggocore-1.2.9/viggocore/subsystem/route/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/route/resource.py` & `viggocore-1.2.9/viggocore/subsystem/route/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/tag/controller.py` & `viggocore-1.2.9/viggocore/subsystem/tag/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/tag/manager.py` & `viggocore-1.2.9/viggocore/subsystem/tag/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/tag/resource.py` & `viggocore-1.2.9/viggocore/subsystem/tag/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/tag/router.py` & `viggocore-1.2.9/viggocore/subsystem/tag/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/timeline_event/controller.py` & `viggocore-1.2.9/viggocore/subsystem/timeline_event/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/timeline_event/manager.py` & `viggocore-1.2.9/viggocore/subsystem/timeline_event/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/timeline_event/resource.py` & `viggocore-1.2.9/viggocore/subsystem/timeline_event/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/token/controller.py` & `viggocore-1.2.9/viggocore/subsystem/token/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/token/manager.py` & `viggocore-1.2.9/viggocore/subsystem/token/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/token/resource.py` & `viggocore-1.2.9/viggocore/subsystem/token/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/token/router.py` & `viggocore-1.2.9/viggocore/subsystem/token/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/user/controller.py` & `viggocore-1.2.9/viggocore/subsystem/user/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/user/email.py` & `viggocore-1.2.9/viggocore/subsystem/user/email.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/user/manager.py` & `viggocore-1.2.9/viggocore/subsystem/user/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/user/resource.py` & `viggocore-1.2.9/viggocore/subsystem/user/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/subsystem/user/router.py` & `viggocore-1.2.9/viggocore/subsystem/user/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/system.py` & `viggocore-1.2.9/viggocore/system.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/fixtures.py` & `viggocore-1.2.9/viggocore/tests/functional/fixtures.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_base.py` & `viggocore-1.2.9/viggocore/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_domains.py` & `viggocore-1.2.9/viggocore/tests/functional/test_domains.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_grants.py` & `viggocore-1.2.9/viggocore/tests/functional/test_grants.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_grants_policies.py` & `viggocore-1.2.9/viggocore/tests/functional/test_grants_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_policies.py` & `viggocore-1.2.9/viggocore/tests/functional/test_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_roles.py` & `viggocore-1.2.9/viggocore/tests/functional/test_roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore/tests/functional/test_users.py` & `viggocore-1.2.9/viggocore/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore.egg-info/SOURCES.txt` & `viggocore-1.2.9/viggocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `viggocore-1.2.8/viggocore.egg-info/requires.txt` & `viggocore-1.2.9/viggocore.egg-info/requires.txt`

 * *Files identical despite different names*

