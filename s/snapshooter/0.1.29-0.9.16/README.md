# Comparing `tmp/snapshooter-0.1.29.tar.gz` & `tmp/snapshooter-0.9.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-0.1.29.tar", last modified: Wed Apr 10 20:50:46 2024, max compression
+gzip compressed data, was "snapshooter-0.9.16.tar", last modified: Mon Apr 15 19:52:16 2024, max compression
```

## Comparing `snapshooter-0.1.29.tar` & `snapshooter-0.9.16.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:50:46.697024 snapshooter-0.1.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 20:50:29.000000 snapshooter-0.1.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-10 20:50:46.697024 snapshooter-0.1.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-10 20:50:29.000000 snapshooter-0.1.29/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:50:46.697024 snapshooter-0.1.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 20:50:29.000000 snapshooter-0.1.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:50:46.693024 snapshooter-0.1.29/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 20:50:29.000000 snapshooter-0.1.29/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-10 20:50:29.000000 snapshooter-0.1.29/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-10 20:50:29.000000 snapshooter-0.1.29/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 20:50:29.000000 snapshooter-0.1.29/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27005 2024-04-10 20:50:29.000000 snapshooter-0.1.29/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:50:46.697024 snapshooter-0.1.29/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 20:50:46.000000 snapshooter-0.1.29/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:50:46.697024 snapshooter-0.1.29/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:50:29.000000 snapshooter-0.1.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 20:50:29.000000 snapshooter-0.1.29/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-10 20:50:29.000000 snapshooter-0.1.29/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 20:50:29.000000 snapshooter-0.1.29/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:52:16.863891 snapshooter-0.9.16/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 19:52:00.000000 snapshooter-0.9.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-15 19:52:16.863891 snapshooter-0.9.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-15 19:52:00.000000 snapshooter-0.9.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:52:16.863891 snapshooter-0.9.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 19:52:00.000000 snapshooter-0.9.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:52:16.863891 snapshooter-0.9.16/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 19:52:08.000000 snapshooter-0.9.16/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 19:52:00.000000 snapshooter-0.9.16/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 19:52:00.000000 snapshooter-0.9.16/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 19:52:00.000000 snapshooter-0.9.16/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 19:52:00.000000 snapshooter-0.9.16/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33097 2024-04-15 19:52:00.000000 snapshooter-0.9.16/snapshooter/snapshooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:52:16.863891 snapshooter-0.9.16/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:52:16.000000 snapshooter-0.9.16/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:52:16.863891 snapshooter-0.9.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:52:00.000000 snapshooter-0.9.16/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:52:00.000000 snapshooter-0.9.16/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 19:52:00.000000 snapshooter-0.9.16/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 19:52:00.000000 snapshooter-0.9.16/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-0.1.29/LICENSE` & `snapshooter-0.9.16/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-0.1.29/PKG-INFO` & `snapshooter-0.9.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.1.29
+Version: 0.9.16
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-0.1.29/README.md` & `snapshooter-0.9.16/README.md`

 * *Files identical despite different names*

### Comparing `snapshooter-0.1.29/setup.py` & `snapshooter-0.9.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+version = os.getenv("VERSION")
+
 setuptools.setup(
     name="snapshooter",
-    version="0.1.29",
+    version=version,
     author="jeromerg",
     author_email="jeromerg@gmx.net",
     description="Provides a set of utilities for comparing and backing up data on different filesystems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeromerg/snapshooter",
     packages=setuptools.find_packages(),
@@ -19,15 +22,15 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'fsspec',
         'pandas',
         'tabulate',
         'typer[all]',
-
+        'tzlocal',
     ],
     entry_points={
         'console_scripts': [
             'snapshooter=snapshooter.cli:main_cli',
         ],
     },
     python_requires='>=3.10',
```

### Comparing `snapshooter-0.1.29/snapshooter/cli.py` & `snapshooter-0.9.16/snapshooter/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from typing_extensions import Annotated
 
 from snapshooter import Heap, Snapshooter, convert_snapshot_to_df, compare_snapshots as compare_snapshots_
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger(__name__)
 
+# get root logger
+root_logger = logging.getLogger()
+# shift logging for azure.core.pipeline.policies.http_logging_policy (if root logger is set to INFO, then set this to WARNING and so one)
+logging.getLogger("azure.core.pipeline.policies.http_logging_policy").setLevel(root_logger.getEffectiveLevel() + 10)
 
 main_cli = typer.Typer()
 
 
 @dataclass
 class SharedConfig:
     root_dir             : str
@@ -27,32 +31,44 @@
     heap_storage_options : str
     snap_dir             : str
     snap_storage_options : str
 
 
 @main_cli.callback(no_args_is_help=True)
 def shared_to_all_commands(
-    ctx                  : typer.Context,
-    file_root            : Annotated[str, typer.Option(envvar="FILE_ROOT"            , help="The directory under consideration, to backup or to restore to. Provided as fsspec path/uri")],
-    heap_root            : Annotated[str, typer.Option(envvar="HEAP_ROOT"            , help="The directory containing the heap files. Provided as fsspec path/uri")],
-    snap_root            : Annotated[str, typer.Option(envvar="SNAP_ROOT"            , help="The directory containing the snapshot files. Provided as fsspec path/uri")],
-    file_storage_options : Annotated[str, typer.Option(envvar="FILE_STORAGE_OPTIONS" , help="Additional storage options to pass to fsspec dir file system. expected JSON string")] = None,
-    heap_storage_options : Annotated[str, typer.Option(envvar="HEAP_STORAGE_OPTIONS" , help="Additional storage options to pass to fsspec heap_dir file system. expected JSON string")] = None,
-    snap_storage_options : Annotated[str, typer.Option(envvar="SNAP_STORAGE_OPTIONS" , help="Additional storage options to pass to fsspec snap_dir file system. expected JSON string")] = None,
+    ctx                     : typer.Context,
+    file_root               : Annotated[str, typer.Option(envvar="FILE_ROOT"               , help="The directory under consideration, to backup or to restore to. Provided as fsspec path/uri")],
+    heap_root               : Annotated[str, typer.Option(envvar="HEAP_ROOT"               , help="The directory containing the heap files. Provided as fsspec path/uri")],
+    snap_root               : Annotated[str, typer.Option(envvar="SNAP_ROOT"               , help="The directory containing the snapshot files. Provided as fsspec path/uri")],
+    file_storage_options    : Annotated[str, typer.Option(envvar="FILE_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec dir file system. expected JSON string")] = None,
+    heap_storage_options    : Annotated[str, typer.Option(envvar="HEAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec heap_dir file system. expected JSON string")] = None,
+    snap_storage_options    : Annotated[str, typer.Option(envvar="SNAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec snap_dir file system. expected JSON string")] = None,
+    parallel_copy_to_heap   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_HEAP"   , help="Number of parallel threads to use for copying files to heap")] = 20,
+    parallel_copy_to_file   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_FILE"   , help="Number of parallel threads to use for copying files to file")] = 20,
+    parallel_delete_in_file : Annotated[int, typer.Option(envvar="PARALLEL_DELETE_IN_FILE" , help="Number of parallel threads to use for deleting files in file")] = 20,
 ):
     file_storage_options_dict = json.loads(file_storage_options or "{}")
     heap_storage_options_dict = json.loads(heap_storage_options or "{}")
     snap_storage_options_dict = json.loads(snap_storage_options or "{}")
 
     file_fs, file_root = fsspec.url_to_fs(file_root, **file_storage_options_dict)
     heap_fs, heap_root = fsspec.url_to_fs(heap_root, **heap_storage_options_dict)
     snap_fs, snap_root = fsspec.url_to_fs(snap_root, **snap_storage_options_dict)
 
-    heap = Heap(heap_fs=heap_fs, heap_root=f"{heap_root}/heap")
-    snapshooter = Snapshooter(file_fs=file_fs, file_root=file_root, snap_fs=snap_fs, snap_root=snap_root, heap=heap)
+    heap = Heap(heap_fs=heap_fs, heap_root=heap_root)
+    snapshooter = Snapshooter(
+        file_fs                 = file_fs, 
+        file_root               = file_root, 
+        snap_fs                 = snap_fs, 
+        snap_root               = snap_root, 
+        heap                    = heap,
+        parallel_copy_to_heap   = parallel_copy_to_heap,
+        parallel_copy_to_file   = parallel_copy_to_file,
+        parallel_delete_in_file = parallel_delete_in_file,
+    )
 
     ctx.obj = snapshooter
     ctx.ensure_object(Snapshooter)
 
 
 @main_cli.command()
 def make_snapshot(
@@ -65,25 +81,27 @@
         save_snapshot=save_snapshot,
         download_missing_files=download_missing_files
     )
 
 
 @main_cli.command()
 def restore_snapshot(
-    ctx           : typer.Context,
-    path          : Annotated[str, typer.Argument(help="The path to the snapshot file to restore. If not set, then it will look for the latest snapshot available, that fulfills the --latest timestamp if provided")] = None,
-    latest        : Annotated[str, typer.Argument(help="If set, then look for the latest snapshot before or at this timestamp. Expected format is 'YYYY-MM-DD' or 'YYYY-MM-DDTHH:MM:SS[offset]'.")] = None,
-    save_snapshot : Annotated[bool, typer.Option(help="Whether to save the current state into a 'backup' snapshot or not. Default is True.")] = True,
+    ctx                  : typer.Context,
+    path                 : Annotated[str, typer.Argument(help="The path to the snapshot file to restore. If not set, then it will look for the latest snapshot available, that fulfills the --latest timestamp if provided")] = None,
+    latest               : Annotated[str, typer.Argument(help="If set, then look for the latest snapshot before or at this timestamp. Expected format is 'YYYY-MM-DD' or 'YYYY-MM-DDTHH:MM:SS[offset]'.")] = None,
+    save_snapshot_before : Annotated[bool, typer.Option(help="Whether to save the current state into a 'backup' snapshot or not. Default is True.")] = True,
+    save_snapshot_after  : Annotated[bool, typer.Option(help="Whether to save the restored state into a 'backup' snapshot or not. Default is True.")] = False,
 ):
     snapshooter: Snapshooter = ctx.obj
     latest_timestamp = datetime.fromisoformat(latest) if latest is not None else None
     snapshooter.restore_snapshot(
         snapshot_to_restore=path,
         latest_timestamp=latest_timestamp,
-        save_snapshot=save_snapshot,
+        save_snapshot_before=save_snapshot_before,
+        save_snapshot_after=save_snapshot_after,
     )
 
 
 @main_cli.command()
 def list_snapshots(
     ctx: typer.Context,
 ):
```

### Comparing `snapshooter-0.1.29/snapshooter/jsonl_utils.py` & `snapshooter-0.9.16/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-0.1.29/snapshooter/snapshooter.py` & `snapshooter-0.9.16/snapshooter/snapshooter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+from abc import abstractmethod
 import datetime
 import gzip
 import hashlib
 import json
 import logging
 import os
 import queue
 import re
 import threading
 import time
 import traceback
 import uuid
 from contextlib import contextmanager
 from io import BufferedReader
-from typing import List, Dict, Set, Callable
+from typing import Any, Generator, List, Dict, Set, Callable
 
 import fsspec
 import pandas as pd
 from fsspec import AbstractFileSystem
 import concurrent.futures
-from .fsspec_utils import get_md5_getter, jsonify_file_info, natural_sort_key
+from .fsspec_utils import get_md5_getter, jsonify_file_info, natural_sort_key, patch_AbstractFileSystem_str_function
 from .jsonl_utils import dumps_jsonl, loads_jsonl
 
 log = logging.getLogger(__name__)
 
+
+patch_AbstractFileSystem_str_function()
+
+
 # noinspection RegExpRedundantEscape
-FMT_PLACEHOLDER_REGEX = re.compile(r"\{[^\}]*?\}")
-DEFAULT_SRC_FS        = fsspec.filesystem("file")
-DEFAULT_SNAP_ROOT     = os.path.normpath(os.path.abspath("./data/backup/snapshots"))
-DEFAULT_SNAP_FS       = fsspec.filesystem("file")
-SNAP_TIMESTAMP_FMT    = "%Y-%m-%d_%H-%M-%S_%fZ"
-SNAP_PATH_FMT         = f"{{timestamp:%Y}}/{{timestamp:%m}}/{{timestamp:{SNAP_TIMESTAMP_FMT}}}.jsonl.gz"
-DEFAULT_HEAP_ROOT     = os.path.normpath(os.path.abspath("./data/backup/heap"))
-DEFAULT_HEAP_FS       = fsspec.filesystem("file")
-HEAP_FMT_FN           = lambda md5: f"{md5[:2]}/{md5[2:4]}/{md5[4:6]}/{md5}.gz"
-BLOCK_SIZE            = 8 * 1024 * 1024  # 8MB
+FMT_PLACEHOLDER_REGEX  = re.compile(r"\{[^\}]*?\}")
+DEFAULT_SRC_FS         = fsspec.filesystem("file")
+DEFAULT_SNAP_ROOT      = os.path.normpath(os.path.abspath("./data/backup/snapshots"))
+DEFAULT_SNAP_FS        = fsspec.filesystem("file")
+SNAP_TIMESTAMP_UTC_FMT = "%Y-%m-%d_%H-%M-%S_%fZ"
+SNAP_PATH_FMT          = f"{{timestamp_utc:%Y}}/{{timestamp_utc:%m}}/{{timestamp_utc:{SNAP_TIMESTAMP_UTC_FMT}}}.jsonl.gz"
+DEFAULT_HEAP_ROOT      = os.path.normpath(os.path.abspath("./data/backup/heap"))
+DEFAULT_HEAP_FS        = fsspec.filesystem("file")
+HEAP_FMT_FN            = lambda md5: f"{md5[:2]}/{md5[2:4]}/{md5[4:6]}/{md5}.gz"
+BLOCK_SIZE             = 8 * 1024 * 1024  # 8MB
 
 
 def _coerce_fs(fs: AbstractFileSystem | str) -> AbstractFileSystem:
     if isinstance(fs, str):
         return fsspec.filesystem(fs)
     elif isinstance(fs, AbstractFileSystem):
         return fs
@@ -109,15 +114,15 @@
 
         :param heap_fs: The file system of the heap files.
         :param heap_root: The root directory of the heap files.
         """
         self.heap_fs   = _coerce_fs(heap_fs)
         self.heap_root = _coerce_root_dir(heap_fs, heap_root)
         # Get all heap files
-        log.info(f"List out heap files in {self.heap_fs} / {self.heap_root}")
+        log.info(f"List out heap files in {self.heap_root}")
         lister = ParallelLister(
             fs=self.heap_fs,
             root=self.heap_root,
             parallel_listers=10,
         )
         heap_file_paths = [fi["name"] for fi in lister.list_files()]
         # basename WITHOUT EXTENSION corresponds to the md5
@@ -162,65 +167,80 @@
                 self.heap_fs.rm(temp_file_path)
                 log.debug(f"Removed temp file '{temp_file_path}'")
             except Exception as e:
                 log.exception(f"Error removing temp file '{temp_file_path}'")
             raise
 
     @contextmanager
-    def open(self, md5: str) -> BufferedReader:
+    def open(self, md5: str) -> Generator[BufferedReader, Any, Any]:
         heap_file_path_relative = HEAP_FMT_FN(md5)
         heap_file_path = f"{self.heap_root}/{heap_file_path_relative}"
         with self.heap_fs.open(heap_file_path, "rb") as heap_file, gzip.GzipFile(fileobj=heap_file, mode='rb') as heap_file:
             yield heap_file
 
 
 class Snapshooter:
     def __init__(
         self,
         file_fs   : AbstractFileSystem,
         file_root : str,
         snap_fs   : AbstractFileSystem,
         snap_root : str,
         heap      : Heap,
-        parallel_downloaders: int = 10
+        parallel_copy_to_heap   : int = 10,
+        parallel_copy_to_file   : int = 10,
+        parallel_delete_in_file : int = 10,
     ) -> None:
         """ Create a new Snapshooter instance.
 
         :param file_fs: The file system of the source files.
         :param file_root: The root directory of the source files.
         :param snap_fs: The file system of the snapshot files.
         :param snap_root: The root directory of the snapshot files.
         :param heap: The heap instance, that stores the files by their checksum.
         """
         self.file_fs   : AbstractFileSystem = _coerce_fs(file_fs)
         self.file_root : str                = _coerce_root_dir(file_fs, file_root)
         self.snap_fs   : AbstractFileSystem = _coerce_fs(snap_fs)
         self.snap_root : str                = _coerce_root_dir(snap_fs, snap_root)
         self.heap      : Heap               = heap
-        self.parallel_downloaders : int     = parallel_downloaders
+        self.parallel_copy_to_heap   : int  = parallel_copy_to_heap
+        self.parallel_copy_to_file   : int  = parallel_copy_to_file
+        self.parallel_delete_in_file : int  = parallel_delete_in_file
+        
 
     def convert_snapshot_timestamp_to_path(self, timestamp: datetime.datetime) -> str:
         """ Convert the given timestamp to a snapshot file path.
 
         :param timestamp: The timestamp of the snapshot.
         :return: The path of the snapshot file.
         """
-        snap_file_path = SNAP_PATH_FMT.format(timestamp=timestamp)
+        # if timestamp is naiv, then assume local time
+        if timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone()
+        
+        # convert to utc
+        timestamp_utc = timestamp.astimezone(datetime.timezone.utc)
+        
+        # create snapshot file path
+        snap_file_path = SNAP_PATH_FMT.format(timestamp_utc=timestamp_utc)
         snap_file_path = f"{self.snap_root}/{snap_file_path}"
+
         return snap_file_path
 
     def convert_snapshot_path_to_timestamp(self, snap_file_path: str) -> datetime.datetime:
         """ Extract from the given snapshot file path the timestamp of the snapshot.
 
         :param snap_file_path: The path of the snapshot file.
         :return: The timestamp of the snapshot.
         """
         snap_file_name     = os.path.basename(snap_file_path)
         snap_timestamp_str = snap_file_name.split(".")[0]
-        snap_timestamp     = datetime.datetime.strptime(snap_timestamp_str, SNAP_TIMESTAMP_FMT)
+        snap_timestamp     = datetime.datetime.strptime(snap_timestamp_str, SNAP_TIMESTAMP_UTC_FMT)
+        snap_timestamp     = snap_timestamp.replace(tzinfo=datetime.timezone.utc)
         return snap_timestamp
 
     def get_snapshot_paths(self) -> list[str]:
         """ Get all snapshot paths from the snapshot file system.
 
         :return: The paths of all snapshots sorted by path name (descending).
         """
@@ -236,31 +256,36 @@
 
         :param latest_timestamp: If given, search for the latest snapshot which was created before or at the given timestamp. Default: None
         :return: The path of the latest snapshot or None, if no snapshot was found.
         """
         log.info("Search latest snapshot")
         snapshot_paths = self.get_snapshot_paths()
         if len(snapshot_paths) == 0:
-            log.info(f"No snapshot found in {self.snap_fs} / {self.snap_root}")
+            log.info(f"No snapshot found in {self.snap_root}")
             return None
 
         snapshot_path_by_filename = { f.split("/")[-1]: f for f in snapshot_paths }
         snapshot_filenames_in_reverse_order = sorted(snapshot_path_by_filename.keys(), key=natural_sort_key, reverse=True)
 
         # slice the list of snapshots to the one before the given timestamp    
         snapshot_path = None
         if latest_timestamp is not None:
-            limit_snapshot_relative_path = SNAP_PATH_FMT.format(timestamp=latest_timestamp)
+            # if timestamp is naiv, then assume local time
+            if latest_timestamp.tzinfo is None or latest_timestamp.tzinfo.utcoffset(latest_timestamp) is None:
+                latest_timestamp = latest_timestamp.astimezone()
+            # convert to utc
+            latest_timestamp_utc = latest_timestamp.astimezone(datetime.timezone.utc)
+            limit_snapshot_relative_path = SNAP_PATH_FMT.format(timestamp_utc=latest_timestamp_utc)
             limit_snapshot_filename = limit_snapshot_relative_path.split("/")[-1]
             for filename in snapshot_filenames_in_reverse_order:
                 if filename <= limit_snapshot_filename:
                     snapshot_path = snapshot_path_by_filename[filename]
                     break
             if snapshot_path is None:
-                log.info(f"No snapshot found in {self.snap_fs} / {self.snap_root} with timestamp before (or equal) '{latest_timestamp}'")
+                log.info(f"No snapshot found in {self.snap_root} with timestamp before (or equal) '{latest_timestamp}'")
                 return None
         else:
             snapshot_path = snapshot_path_by_filename[snapshot_filenames_in_reverse_order[0]]
         
         log.info(f"Found snapshot '{snapshot_path}'")
         return snapshot_path
 
@@ -276,15 +301,15 @@
                 log.info(f"Try read latest snapshot before '{latest_timestamp}'")
             snapshot_path = self.try_get_snapshot_path(latest_timestamp)
             if snapshot_path is None:
                 return None
         else:
             log.info(f"Try read snapshot from provided path '{snapshot_path}'")
 
-        log.info(f"Read snapshot from {snapshot_path} ({self.snap_fs})")
+        log.info(f"Read snapshot from {snapshot_path}")
 
         with self.snap_fs.open(snapshot_path, "rb") as f, gzip.GzipFile(fileobj=f) as g:
             text = g.read().decode("utf-8")
             latest_snapshot = loads_jsonl(text)  # type: List[Dict]
 
         log.info(f"Read snapshot contains {len(latest_snapshot)} files")
         return latest_snapshot
@@ -292,19 +317,19 @@
     def read_snapshot(
         self,
         snapshot_path: str | None = None,
         latest_timestamp: datetime.datetime | None = None,
     ) -> List[dict]:
         latest_snapshot = self.try_read_snapshot(snapshot_path=snapshot_path, latest_timestamp=latest_timestamp)
         if latest_snapshot is None:
-            raise Exception(f"No snapshot found in {self.snap_fs} / {self.snap_root}")
+            raise Exception(f"No snapshot found in '{self.snap_root}'")
         return latest_snapshot
 
     def _make_snapshot_without_md5(self) -> List[dict]:
-        log.info(f"List out src files in {self.file_fs} / {self.file_root} (may last long)")
+        log.info(f"List out src files in '{self.file_root}' (may last long)")
         lister = ParallelLister(
             fs=self.file_fs,
             root=self.file_root,
             parallel_listers=10,
         )
         src_file_infos = lister.list_files()
         log.info(f"Found {len(src_file_infos)} src files")
@@ -343,15 +368,15 @@
                 src_file_info["md5"] = md5
 
     def make_snapshot(
         self,
         save_snapshot: bool = True,
         download_missing_files: bool = True
     ) -> tuple[List[dict], datetime.datetime]:
-        timestamp = datetime.datetime.utcnow()
+        timestamp = datetime.datetime.now(datetime.timezone.utc)
         log.info(f"Making Snapshot with timestamp = '{timestamp}'")
 
         log.info(f"Retrieving prior snapshot to optimize download...")
         latest_snapshot = self.try_read_snapshot(latest_timestamp=timestamp)
         if latest_snapshot is None:
             latest_snapshot = []
         log.info(f"Prior snapshot retrieved")
@@ -372,23 +397,23 @@
         else:
             file_names_missings = set()
 
         all_file_names_to_download = file_names_without_md5 | file_names_missings
         if len(all_file_names_to_download) > 0:
             log.info(f"Downloading {len(all_file_names_to_download)} files to heap")
 
-            downloader = ParallelDownloaderToHeap(
-                file_fs=self.file_fs,
-                file_root=self.file_root,
-                snapshot_files_by_name=snapshot_files_by_name,
-                all_file_names_to_download=all_file_names_to_download,
-                heap=self.heap,
-                parallel_downloaders=self.parallel_downloaders,
+            downloader = ParallelCopyFileToHeap(
+                file_fs                = self.file_fs,
+                file_root              = self.file_root,
+                relative_paths_to_copy = all_file_names_to_download,
+                heap                   = self.heap,
+                parallelization        = self.parallel_copy_to_heap,
+                snapshot_files_by_name = snapshot_files_by_name,
             )
-            downloader.download_files()
+            downloader.process_files()
 
         if save_snapshot:
             self._save_snapshot(snapshot, timestamp)
 
         return snapshot, timestamp
 
     def _save_snapshot(
@@ -398,79 +423,92 @@
     ) -> str:
         """Save the given snapshot to the snapshot file system.
 
         :param snapshot: The snapshot to save.
         :param snapshot_timestamp: The timestamp of the snapshot to save.
         :return: The (absolute) path of the saved snapshot.
         """
-        new_snapshot_relative_path = SNAP_PATH_FMT.format(timestamp=snapshot_timestamp)
+        new_snapshot_relative_path = SNAP_PATH_FMT.format(timestamp_utc=snapshot_timestamp)
         new_snapshot_path = f"{self.snap_root}/{new_snapshot_relative_path}"
-        log.info(f"Save snapshot to {new_snapshot_path} ({self.snap_fs})")
+        log.info(f"Save snapshot to {new_snapshot_path}")
         self.snap_fs.makedirs(os.path.dirname(new_snapshot_path), exist_ok=True)
         with self.snap_fs.open(new_snapshot_path, "wb") as f, gzip.GzipFile(fileobj=f, mode='wb') as g:
             snap_content = dumps_jsonl(snapshot)
             g.write(snap_content.encode("utf-8"))
         log.info(f"Saved snapshot")
         return new_snapshot_path
 
     def restore_snapshot(
         self,
         snapshot_to_restore: str | List[dict] | pd.DataFrame | None = None,
         latest_timestamp: datetime.datetime = None,
-        save_snapshot: bool = True
+        save_snapshot_before: bool = True,
+        save_snapshot_after: bool = False,
     ):
         log.info("Loading snapshot to restore")
         # read snapshot depending on the type of snapshot_to_restore
         if snapshot_to_restore is None:
             snap = self.read_snapshot(latest_timestamp=latest_timestamp)
-            df_snap = convert_snapshot_to_df(snap)
+            df_snapshot_to_restore = convert_snapshot_to_df(snap)
         elif isinstance(snapshot_to_restore, str):
             snap = self.read_snapshot(snapshot_path=snapshot_to_restore)
-            df_snap = convert_snapshot_to_df(snap)
+            df_snapshot_to_restore = convert_snapshot_to_df(snap)
         elif isinstance(snapshot_to_restore, list):
-            df_snap = convert_snapshot_to_df(snapshot_to_restore)
+            df_snapshot_to_restore = convert_snapshot_to_df(snapshot_to_restore)
         elif isinstance(snapshot_to_restore, pd.DataFrame):
-            df_snap = snapshot_to_restore
+            df_snapshot_to_restore = snapshot_to_restore
         else:
             raise Exception(f"restore_snapshot: Unknown type {type(snapshot_to_restore)} for snapshot_to_restore. Expected: pd.DataFrame, List[dict]")
         log.info(f"Snapshot to restore loaded")
 
         log.info("Making current snapshot to apply diff to")
-        current_snapshot, _ = self.make_snapshot(save_snapshot=save_snapshot, download_missing_files=True)
+        current_snapshot, _ = self.make_snapshot(save_snapshot=save_snapshot_before, download_missing_files=True)
         log.info(f"Current snapshot made")
         df_current_snapshot = convert_snapshot_to_df(current_snapshot)
 
-        diff = compare_snapshots(df_snap, df_current_snapshot)
+        df_diff = compare_snapshots(df_snapshot_to_restore, df_current_snapshot)
 
-        self.apply_diff(diff)
+        self.apply_diff(df_diff)
+        
+        # finally save the latest state if requested
+        # Remark: There is space for optimization, because the snapshot 
+        # could be built from the snapshot before and the diff + missing file metadata for
+        # the files that were not in the snapshot before.
+        if save_snapshot_after:
+            self.make_snapshot(save_snapshot=True, download_missing_files=True)
 
     def apply_diff(self, df_diff: pd.DataFrame):
         if not isinstance(df_diff, pd.DataFrame):
             raise Exception(f"apply_diff: Unknown type {type(df_diff)} for diff. Expected: pd.DataFrame")
 
-        relative_path_only_left = set(df_diff[df_diff["status"] == "only_left"].index)
+        relative_path_only_left  = set(df_diff[df_diff["status"] == "only_left"].index)
         relative_path_only_right = set(df_diff[df_diff["status"] == "only_right"].index)
-        relative_path_different = set(df_diff[df_diff["status"] == "different"].index)
+        relative_path_different  = set(df_diff[df_diff["status"] == "different"].index)
 
         log.info(f"Copying files: {len(relative_path_only_left)} only_left + {len(relative_path_different)} different")
-        for file_relative_path in sorted(relative_path_only_left | relative_path_different):
-            file_info_row = df_diff.loc[file_relative_path, :]
-            md5 = file_info_row["md5_left"]
-            src_file_path = f"{self.file_root}/{file_relative_path}"
-            log.debug(f"Copying file with md5 '{md5}' to '{file_relative_path}'")
-            self.file_fs.makedirs(os.path.dirname(src_file_path), exist_ok=True)
-            with self.heap.open(md5) as heap_file:
-                with self.file_fs.open(src_file_path, "wb") as src_file:
-                    src_file.write(heap_file.read())
+        relative_paths_to_copy = sorted(relative_path_only_left | relative_path_different)
+        parallel_job = ParallelCopyHeapToFile(
+            file_fs                = self.file_fs,
+            file_root              = self.file_root,
+            relative_paths_to_copy = relative_paths_to_copy,
+            heap                   = self.heap,
+            parallelization        = self.parallel_copy_to_file,            
+            df_diff                = df_diff,
+        )
+        parallel_job.process_files()
 
         log.info(f"Deleting {len(relative_path_only_right)} files")
-        for file_relative_path in sorted(relative_path_only_right):
-            src_file_path = f"{self.file_root}/{file_relative_path}"
-            log.debug(f"Deleting '{file_relative_path}'")
-            self.file_fs.rm(src_file_path)
+        parallel_job = ParallelDeleteFile(
+            file_fs                = self.file_fs,
+            file_root              = self.file_root,
+            relative_paths_to_copy = relative_path_only_right,
+            heap                   = self.heap,
+            parallelization        = self.parallel_delete_in_file,
+        )
+        parallel_job.process_files()
 
 
 class ParallelLister:
     def __init__(
         self,
         fs: AbstractFileSystem,
         root: str,
@@ -494,146 +532,243 @@
         self._is_interrupted = True
         # Wake up all threads waiting on the queue by putting None as a special value
         if not old_is_interrupted:
             for _ in range(self.parallel_listers):
                 self.dir_queue.put(None)
 
     def _list_dir(self, directory: str):
-        try:
-            all_details = list(self.fs.find(directory, detail=True, withdirs=True, maxdepth=1).values())
-            # remove this directory from the file names (to avoid endless loop...)
-            all_details = [d for d in all_details if d["name"] != directory]
-            sub_dir_infos = [d for d in all_details if d['type'] == 'directory']
+            # all_details  = self.fs.find(directory, detail=True, withdirs=True, maxdepth=0).values()
+            # all_details  = list(all_details)
+            all_details    = self.fs.ls(directory, detail=True)
+            all_details    = [d for d in all_details if d["name"] != directory]  # avoid endless loop
+            sub_dir_infos  = [d for d in all_details if d['type'] == 'directory']
             src_file_infos = [d for d in all_details if d['type'] == 'file']
             for sub_dir_info in sub_dir_infos:
                 self.dir_queue.put(sub_dir_info['name'])
             with self.lock:
                 self.result.extend(src_file_infos)
-        except Exception as e:
-            error_message = f"Error listing files in {directory}: {e}"
-            error_message += "\n" + traceback.format_exc()
-            with self.lock:
-                self.errors.append(error_message)
 
     def _process_queue(self):
-        while not self._is_interrupted:
-            self.check_interrupted()
-            directory = self.dir_queue.get()
-            self.check_interrupted()
-            self._list_dir(directory)
-            self.dir_queue.task_done()
+        try:
+            while not self._is_interrupted:
+                self.check_interrupted()
+                directory = self.dir_queue.get()
+                self.check_interrupted()
+                try:
+                    self._list_dir(directory)
+                except Exception as e:
+                    error_message = f"Error listing files in {directory}: {e}"
+                    error_message += "\n" + traceback.format_exc()
+                    with self.lock:
+                        self.errors.append(error_message)
+                self.dir_queue.task_done()
+        except InterruptedError:
+            pass  # some tools log error is thread die because of exception, but we want to ignore this excepted case
 
     def _log_progress(self):
-        while True:
-            time.sleep(10)
-            self.check_interrupted()
-            log.info(f"Progress: {len(self.result)} files listed.")
+        try:
+            while True:
+                time.sleep(10)
+                self.check_interrupted()
+                log.info(f"Progress: {len(self.result)} files listed.")
+        except InterruptedError:
+            # some tools log error is thread die because of exception, but we want to ignore this excepted case
+            log.debug("ParallelLister: Logging thread interrupted properly.")
 
     def list_files(self):
+        # remark: first connection and root check in main thread improves error handling
+        try:
+            root_exists = self.fs.exists(self.root)
+        except Exception as e:
+            raise Exception(f"Error verifying root folder '{self.root}' in {self.fs}: {e}") from e
+
+        if not root_exists:
+            raise Exception(f"Root folder '{self.root}' does not exist in {self.fs}")
+        else:
+            log.info(f"Root folder '{self.root}' exists in {self.fs}. Now listing files...")
+            
+        # even first root dir search in main threa ensures that access rights are ok
+        try:
+            self._list_dir(self.root)
+        except Exception as e:
+            raise Exception(f"Error listing files of root folder '{self.root}' in {self.fs}: {e}") from e
+            
+        # start parallelized listing
         with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallel_listers) as executor:
             for _ in range(self.parallel_listers):
                 executor.submit(self._process_queue)
 
             log_thread = threading.Thread(target=self._log_progress, daemon=True)
             log_thread.start()
 
             # Add root and wait for the directory listing tasks to complete
-            self.dir_queue.put(self.root)
             self.dir_queue.join()
 
             # for logger
             self.interrupt()
 
         # Check if there were any errors during listing
         if self.errors:
             error_summary = "\n---------------------------\n".join(self.errors)
             raise Exception(f"Errors occurred during file listing:\n{error_summary}")
 
         return self.result
 
 
-class ParallelDownloaderToHeap:
+class ParallelFileProcessor:
+    """Abstract class for parallel file processing."""
     def __init__(
         self,
-        file_fs                    : AbstractFileSystem,
-        file_root                  : str,
-        snapshot_files_by_name     : Dict[str, dict],
-        all_file_names_to_download : Set[str],
-        heap                       : Heap,
-        parallel_downloaders       : int,
+        file_fs                : AbstractFileSystem,
+        file_root              : str,
+        relative_paths_to_copy : Set[str],
+        heap                   : Heap,
+        parallelization        : int,
     ):
-        self.src_fs                     = file_fs
-        self.src_root                   = file_root
-        self.snapshot_files_by_name     = snapshot_files_by_name
-        self.all_file_names_to_download = all_file_names_to_download
-        self.heap                       = heap
-        self.parallel_downloaders       = parallel_downloaders
-        self.download_count             = 0
-        self.errors                     = []  # List to store errors
-        self.lock                       = threading.Lock()
-        self._is_interrupted             = False
+        self.file_fs                   = file_fs
+        self.file_root                 = file_root
+        self.relative_paths_to_process = relative_paths_to_copy
+        self.heap                      = heap
+        self.parallelization           = parallelization
+        self.copy_count                = 0
+        self.errors                    = []  # List to store errors
+        self.lock                      = threading.Lock()
+        self._is_interrupted           = False
 
     def check_interrupted(self):
         if self._is_interrupted:
-            raise InterruptedError("Interrupted properly")
+            raise InterruptedError(f"{self.__class__.__name__}: Interrupted properly")
 
     def interrupt(self):
         self._is_interrupted = True
 
-    def _download_file(self, src_file_relative_path):
+    def process_files(self):
+        log.info(f"{self.__class__.__name__}: Processing {len(self.relative_paths_to_process)} files with {self.parallelization} workers")
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallelization) as executor:
+            log_thread = threading.Thread(target=self._log_progress, daemon=True)
+            log_thread.start()
+
+            # Submit all download tasks to the executor
+            futures = [executor.submit(self._process_file, file_relative_path) for file_relative_path in self.relative_paths_to_process]
+
+            # Wait for all futures to complete
+            try:
+                concurrent.futures.wait(futures)
+            except KeyboardInterrupt:
+                self.interrupt()
+                log.info(f"{self.__class__.__name__}: Download interrupted by user.")
+                executor.shutdown(wait=False)
+                raise
+
+        # Ensures the logging thread also completes
+        self.interrupt()
+
+        # Check if there were any errors during downloads
+        if self.errors:
+            error_summary = "\n---------------------------\n".join(self.errors)
+            raise Exception(f"{self.__class__.__name__}: Errors occurred during files processing:\n{error_summary}")
+
+    @abstractmethod
+    def _process_file(self, file_relative_path):
+        ...
+
+    def _log_progress(self):
+        try:
+            while True:
+                time.sleep(10)
+                self.check_interrupted()
+                log.info(f"{self.__class__.__name__}: Progress ... {self.copy_count}/{len(self.relative_paths_to_process)} files processed.")
+        except InterruptedError:
+            # some tools log error is thread die because of exception, but we want to ignore this excepted case
+            log.debug(f"{self.__class__.__name__}: Logging thread interrupted properly.")
+
+
+class ParallelCopyFileToHeap(ParallelFileProcessor):
+    def __init__(
+        self,
+        file_fs                : AbstractFileSystem,
+        file_root              : str,
+        relative_paths_to_copy : Set[str],
+        heap                   : Heap,
+        parallelization        : int,
+        snapshot_files_by_name : Dict[str, dict],
+    ):
+        super().__init__(file_fs, file_root, relative_paths_to_copy, heap, parallelization)        
+        self.snapshot_files_by_name = snapshot_files_by_name
+
+    def _process_file(self, file_relative_path):
         try:
-            src_file_info = self.snapshot_files_by_name[src_file_relative_path]
-            src_file_path = f"{self.src_root}/{src_file_relative_path}"
-            log.debug(f"Downloading '{src_file_relative_path}'")
+            src_file_info = self.snapshot_files_by_name[file_relative_path]
+            src_file_path = f"{self.file_root}/{file_relative_path}"
+            log.debug(f"{self.__class__.__name__}: Downloading '{file_relative_path}'")
             self.check_interrupted()
-            with self.src_fs.open(src_file_path, "rb") as f:
+            with self.file_fs.open(src_file_path, "rb") as f:
                 src_file_md5 = self.heap.add_file_to_heap(f, self.check_interrupted)
 
             if "md5" in src_file_info:
                 if src_file_info["md5"] != src_file_md5:
-                    error_message = f"MD5 mismatch for '{src_file_relative_path}' between snapshot metadata and downloaded file"
+                    error_message = f"MD5 mismatch for '{file_relative_path}' between snapshot metadata and downloaded file"
                     log.error(error_message)
                     with self.lock:
                         self.errors.append(error_message)
             else:
                 src_file_info["md5"] = src_file_md5
 
         except Exception as e:
-            error_message = f"Error downloading {src_file_relative_path}: {e}"
+            error_message = f"Error copying {file_relative_path}: {e}"
             error_message += "\n" + traceback.format_exc()
             log.error(error_message)
             with self.lock:
                 self.errors.append(error_message)
         finally:
             with self.lock:
-                self.download_count += 1
+                self.copy_count += 1
 
-    def _log_progress(self):
-        while True:
-            time.sleep(10)
-            self.check_interrupted()
-            log.info(f"Progress: {self.download_count}/{len(self.all_file_names_to_download)} files downloaded.")
 
-    def download_files(self):
-        with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallel_downloaders) as executor:
-            log_thread = threading.Thread(target=self._log_progress, daemon=True)
-            log_thread.start()
+class ParallelCopyHeapToFile(ParallelFileProcessor):
+    def __init__(
+        self,
+        file_fs                : AbstractFileSystem,
+        file_root              : str,
+        relative_paths_to_copy : Set[str],
+        heap                   : Heap,
+        parallelization        : int,
+        df_diff                : pd.DataFrame,
+    ):
+        super().__init__(file_fs, file_root, relative_paths_to_copy, heap, parallelization)
+        self.df_diff = df_diff
 
-            # Submit all download tasks to the executor
-            futures = [executor.submit(self._download_file, src_file_relative_path) for src_file_relative_path in self.all_file_names_to_download]
+    def _process_file(self, file_relative_path):
+        try:
+            md5 = self.df_diff.at[file_relative_path, "md5_left"]
+            src_file_path = f"{self.file_root}/{file_relative_path}"
+            log.debug(f"Copying file with md5 '{md5}' to '{file_relative_path}'")
+            self.file_fs.makedirs(os.path.dirname(src_file_path), exist_ok=True)  # TODO: Optimze to avoid calling every times
+            with self.heap.open(md5) as src_file:
+                with self.file_fs.open(src_file_path, "wb") as dst_file:
+                    dst_file.write(src_file.read())
+        except Exception as e:
+            error_message = f"Error copying {file_relative_path}: {e}"
+            error_message += "\n" + traceback.format_exc()
+            log.error(error_message)
+            with self.lock:
+                self.errors.append(error_message)
+        finally:
+            with self.lock:
+                self.copy_count += 1
 
-            # Wait for all futures to complete
-            try:
-                concurrent.futures.wait(futures)
-            except KeyboardInterrupt:
-                self.interrupt()
-                log.info("Download interrupted by user.")
-                executor.shutdown(wait=False)
-                raise
 
-        # Ensures the logging thread also completes
-        self.interrupt()
+class ParallelDeleteFile(ParallelFileProcessor):
+    def __init__(
+        self,
+        file_fs                : AbstractFileSystem,
+        file_root              : str,
+        relative_paths_to_copy : Set[str],
+        heap                   : Heap,
+        parallelization        : int,
+    ):
+        super().__init__(file_fs, file_root, relative_paths_to_copy, heap, parallelization)
 
-        # Check if there were any errors during downloads
-        if self.errors:
-            error_summary = "\n---------------------------\n".join(self.errors)
-            raise Exception(f"Errors occurred during file downloads:\n{error_summary}")
+    def _process_file(self, file_relative_path):
+        src_file_path = f"{self.file_root}/{file_relative_path}"
+        log.debug(f"Deleting '{file_relative_path}'")
+        self.file_fs.rm(src_file_path)
```

### Comparing `snapshooter-0.1.29/snapshooter.egg-info/PKG-INFO` & `snapshooter-0.9.16/snapshooter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 0.1.29
+Version: 0.9.16
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-0.1.29/tests/test_fsspec_utils.py` & `snapshooter-0.9.16/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

