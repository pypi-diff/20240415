# Comparing `tmp/zfs_replicate-3.2.8.tar.gz` & `tmp/zfs_replicate-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfs_replicate-3.2.8.tar", max compression
+gzip compressed data, was "zfs_replicate-3.2.9.tar", max compression
```

## Comparing `zfs_replicate-3.2.8.tar` & `zfs_replicate-3.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1290 2024-02-18 11:15:14.087806 zfs_replicate-3.2.8/LICENSE
--rw-r--r--   0        0        0     3619 2024-02-18 11:15:14.087806 zfs_replicate-3.2.8/README.md
--rw-r--r--   0        0        0     1613 2024-02-18 11:15:14.087806 zfs_replicate-3.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/__init__.pyi
--rw-r--r--   0        0        0       33 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/__init__.py
--rw-r--r--   0        0        0       35 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/cli/__init__.py
--rw-r--r--   0        0        0      912 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/cli/click.py
--rw-r--r--   0        0        0     4164 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/cli/main.py
--rw-r--r--   0        0        0      203 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/compress/__init__.py
--rw-r--r--   0        0        0      484 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/compress/command.py
--rw-r--r--   0        0        0      170 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/compress/type.py
--rw-r--r--   0        0        0      327 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/error.py
--rw-r--r--   0        0        0      711 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/filesystem/__init__.py
--rw-r--r--   0        0        0     1546 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/filesystem/create.py
--rw-r--r--   0        0        0      660 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/filesystem/destroy.py
--rw-r--r--   0        0        0     1524 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/filesystem/list.py
--rw-r--r--   0        0        0      412 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/filesystem/type.py
--rw-r--r--   0        0        0      952 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/list.py
--rw-r--r--   0        0        0      273 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/optional.py
--rw-r--r--   0        0        0      330 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/snapshot/__init__.py
--rw-r--r--   0        0        0      692 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/snapshot/destroy.py
--rw-r--r--   0        0        0     2369 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/snapshot/list.py
--rw-r--r--   0        0        0     2094 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/snapshot/send.py
--rw-r--r--   0        0        0      799 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/snapshot/type.py
--rw-r--r--   0        0        0      183 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/ssh/__init__.py
--rw-r--r--   0        0        0      158 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/ssh/cipher.py
--rw-r--r--   0        0        0      815 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/ssh/command.py
--rw-r--r--   0        0        0      598 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/subprocess.py
--rw-r--r--   0        0        0      256 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/task/__init__.py
--rw-r--r--   0        0        0     2160 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/task/execute.py
--rw-r--r--   0        0        0     3220 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/task/generate.py
--rw-r--r--   0        0        0     2560 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/task/report.py
--rw-r--r--   0        0        0      413 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs/replicate/task/type.py
--rw-r--r--   0        0        0       17 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/__init__.py
--rw-r--r--   0        0        0       27 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/__init__.py
--rw-r--r--   0        0        0     1369 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/cli_test/main_test.py
--rw-r--r--   0        0        0       35 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/compress_test/__init__.py
--rw-r--r--   0        0        0      410 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/compress_test/command_test.py
--rw-r--r--   0        0        0     2195 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/list_test.py
--rw-r--r--   0        0        0      653 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/optional_test.py
--rw-r--r--   0        0        0       36 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/__init__.py
--rw-r--r--   0        0        0     1257 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/list_test.py
--rw-r--r--   0        0        0      737 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/strategies.py
--rw-r--r--   0        0        0      441 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/type_test.py
--rw-r--r--   0        0        0     1971 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/task_test/generate_test.py
--rw-r--r--   0        0        0      579 2024-02-18 11:15:14.091806 zfs_replicate-3.2.8/zfs_test/replicate_test/task_test/report_test.py
--rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 zfs_replicate-3.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1290 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/LICENSE
+-rw-r--r--   0        0        0     3619 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/README.md
+-rw-r--r--   0        0        0     1613 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/__init__.pyi
+-rw-r--r--   0        0        0       33 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/__init__.py
+-rw-r--r--   0        0        0       35 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/cli/__init__.py
+-rw-r--r--   0        0        0      912 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/cli/click.py
+-rw-r--r--   0        0        0     4164 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/cli/main.py
+-rw-r--r--   0        0        0      203 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/compress/__init__.py
+-rw-r--r--   0        0        0      484 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/compress/command.py
+-rw-r--r--   0        0        0      170 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/compress/type.py
+-rw-r--r--   0        0        0      327 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/error.py
+-rw-r--r--   0        0        0      711 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/filesystem/__init__.py
+-rw-r--r--   0        0        0     1546 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/filesystem/create.py
+-rw-r--r--   0        0        0      660 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/filesystem/destroy.py
+-rw-r--r--   0        0        0     1524 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/filesystem/list.py
+-rw-r--r--   0        0        0      412 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/filesystem/type.py
+-rw-r--r--   0        0        0      952 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/list.py
+-rw-r--r--   0        0        0      273 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/optional.py
+-rw-r--r--   0        0        0      330 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/snapshot/__init__.py
+-rw-r--r--   0        0        0      692 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/snapshot/destroy.py
+-rw-r--r--   0        0        0     2369 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/snapshot/list.py
+-rw-r--r--   0        0        0     2094 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/snapshot/send.py
+-rw-r--r--   0        0        0      799 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/snapshot/type.py
+-rw-r--r--   0        0        0      183 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/ssh/__init__.py
+-rw-r--r--   0        0        0      158 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/ssh/cipher.py
+-rw-r--r--   0        0        0      815 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/ssh/command.py
+-rw-r--r--   0        0        0      598 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/subprocess.py
+-rw-r--r--   0        0        0      256 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/task/__init__.py
+-rw-r--r--   0        0        0     2160 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/task/execute.py
+-rw-r--r--   0        0        0     3220 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/task/generate.py
+-rw-r--r--   0        0        0     2560 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/task/report.py
+-rw-r--r--   0        0        0      413 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs/replicate/task/type.py
+-rw-r--r--   0        0        0       17 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs_test/__init__.py
+-rw-r--r--   0        0        0       27 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs_test/replicate_test/__init__.py
+-rw-r--r--   0        0        0     1369 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs_test/replicate_test/cli_test/main_test.py
+-rw-r--r--   0        0        0       35 2024-02-24 14:48:01.576382 zfs_replicate-3.2.9/zfs_test/replicate_test/compress_test/__init__.py
+-rw-r--r--   0        0        0      410 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/compress_test/command_test.py
+-rw-r--r--   0        0        0     2195 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/list_test.py
+-rw-r--r--   0        0        0      653 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/optional_test.py
+-rw-r--r--   0        0        0       36 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/__init__.py
+-rw-r--r--   0        0        0     1257 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/list_test.py
+-rw-r--r--   0        0        0      737 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/strategies.py
+-rw-r--r--   0        0        0      441 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/type_test.py
+-rw-r--r--   0        0        0     1971 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/task_test/generate_test.py
+-rw-r--r--   0        0        0      579 2024-02-24 14:48:01.580382 zfs_replicate-3.2.9/zfs_test/replicate_test/task_test/report_test.py
+-rw-r--r--   0        0        0     4903 1970-01-01 00:00:00.000000 zfs_replicate-3.2.9/PKG-INFO
```

### Comparing `zfs_replicate-3.2.8/LICENSE` & `zfs_replicate-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/README.md` & `zfs_replicate-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/pyproject.toml` & `zfs_replicate-3.2.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 description = "ZFS Snapshot Replicator"
 keywords = ["zfs", "replication", "backup", "remote"]
 license = "BSD-2-Clause"
 name = "zfs-replicate"
 packages = [{include = "zfs"}, {include = "zfs_test", format = "sdist"}]
 readme = "README.md"
 repository = "https://github.com/alunduil/zfs-replicate"
-version = "3.2.8"
+version = "3.2.9"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 python = "^3.8.0"
 
 [tool.poetry.group.test.dependencies]
 coveralls = ">=2.1.1,<4.0.0"
```

### Comparing `zfs_replicate-3.2.8/zfs/replicate/cli/click.py` & `zfs_replicate-3.2.9/zfs/replicate/cli/click.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/cli/main.py` & `zfs_replicate-3.2.9/zfs/replicate/cli/main.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/filesystem/__init__.py` & `zfs_replicate-3.2.9/zfs/replicate/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/filesystem/create.py` & `zfs_replicate-3.2.9/zfs/replicate/filesystem/create.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/filesystem/destroy.py` & `zfs_replicate-3.2.9/zfs/replicate/filesystem/destroy.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/filesystem/list.py` & `zfs_replicate-3.2.9/zfs/replicate/filesystem/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/list.py` & `zfs_replicate-3.2.9/zfs/replicate/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/snapshot/destroy.py` & `zfs_replicate-3.2.9/zfs/replicate/snapshot/destroy.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/snapshot/list.py` & `zfs_replicate-3.2.9/zfs/replicate/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/snapshot/send.py` & `zfs_replicate-3.2.9/zfs/replicate/snapshot/send.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/snapshot/type.py` & `zfs_replicate-3.2.9/zfs/replicate/snapshot/type.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/ssh/command.py` & `zfs_replicate-3.2.9/zfs/replicate/ssh/command.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/subprocess.py` & `zfs_replicate-3.2.9/zfs/replicate/subprocess.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/task/execute.py` & `zfs_replicate-3.2.9/zfs/replicate/task/execute.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/task/generate.py` & `zfs_replicate-3.2.9/zfs/replicate/task/generate.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs/replicate/task/report.py` & `zfs_replicate-3.2.9/zfs/replicate/task/report.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/cli_test/main_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/cli_test/main_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/list_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/list_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/optional_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/optional_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/list_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/list_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/snapshot_test/strategies.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/snapshot_test/strategies.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/task_test/generate_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/task_test/generate_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/zfs_test/replicate_test/task_test/report_test.py` & `zfs_replicate-3.2.9/zfs_test/replicate_test/task_test/report_test.py`

 * *Files identical despite different names*

### Comparing `zfs_replicate-3.2.8/PKG-INFO` & `zfs_replicate-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfs-replicate
-Version: 3.2.8
+Version: 3.2.9
 Summary: ZFS Snapshot Replicator
 Home-page: https://github.com/alunduil/zfs-replicate
 License: BSD-2-Clause
 Keywords: zfs,replication,backup,remote
 Author: Alex Brandt
 Author-email: alunduil@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
```

