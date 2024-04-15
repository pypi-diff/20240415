# Comparing `tmp/autocron-0.9.2.tar.gz` & `tmp/autocron-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocron-0.9.2.tar", last modified: Sun Jan 14 20:19:53 2024, max compression
+gzip compressed data, was "autocron-0.9.5.tar", last modified: Mon Apr 15 13:40:02 2024, max compression
```

## Comparing `autocron-0.9.2.tar` & `autocron-0.9.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-01-14 20:19:53.107790 autocron-0.9.2/
--rw-r--r--   0 klaus      (501) staff       (20)     1085 2023-03-24 06:45:35.000000 autocron-0.9.2/LICENSE.txt
--rw-r--r--   0 klaus      (501) staff       (20)       90 2024-01-11 18:14:55.000000 autocron-0.9.2/MANIFEST.in
--rw-r--r--   0 klaus      (501) staff       (20)     3393 2024-01-14 20:19:53.107735 autocron-0.9.2/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)     2193 2024-01-13 16:36:00.000000 autocron-0.9.2/README.md
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-01-14 20:19:53.105677 autocron-0.9.2/autocron/
--rw-r--r--   0 klaus      (501) staff       (20)     1233 2024-01-14 20:16:21.000000 autocron-0.9.2/autocron/__init__.py
--rw-r--r--   0 klaus      (501) staff       (20)     9577 2024-01-13 16:11:55.000000 autocron-0.9.2/autocron/admin.py
--rw-r--r--   0 klaus      (501) staff       (20)     5341 2024-01-11 17:12:43.000000 autocron-0.9.2/autocron/decorators.py
--rw-r--r--   0 klaus      (501) staff       (20)     7022 2024-01-13 12:22:40.000000 autocron-0.9.2/autocron/engine.py
--rw-r--r--   0 klaus      (501) staff       (20)    11262 2024-01-14 19:53:36.000000 autocron-0.9.2/autocron/schedule.py
--rw-r--r--   0 klaus      (501) staff       (20)    29311 2024-01-13 16:11:55.000000 autocron-0.9.2/autocron/sql_interface.py
--rw-r--r--   0 klaus      (501) staff       (20)     5040 2024-01-14 19:53:36.000000 autocron-0.9.2/autocron/worker.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-01-14 20:19:53.107512 autocron-0.9.2/autocron.egg-info/
--rw-r--r--   0 klaus      (501) staff       (20)     3393 2024-01-14 20:19:53.000000 autocron-0.9.2/autocron.egg-info/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)      449 2024-01-14 20:19:53.000000 autocron-0.9.2/autocron.egg-info/SOURCES.txt
--rw-r--r--   0 klaus      (501) staff       (20)        1 2024-01-14 20:19:53.000000 autocron-0.9.2/autocron.egg-info/dependency_links.txt
--rw-r--r--   0 klaus      (501) staff       (20)       49 2024-01-14 20:19:53.000000 autocron-0.9.2/autocron.egg-info/entry_points.txt
--rw-r--r--   0 klaus      (501) staff       (20)        9 2024-01-14 20:19:53.000000 autocron-0.9.2/autocron.egg-info/top_level.txt
--rw-r--r--   0 klaus      (501) staff       (20)       81 2023-04-22 13:30:54.000000 autocron-0.9.2/pyproject.toml
--rw-r--r--   0 klaus      (501) staff       (20)     1286 2024-01-14 20:19:53.108048 autocron-0.9.2/setup.cfg
--rw-r--r--   0 klaus      (501) staff       (20)      135 2023-03-23 08:40:38.000000 autocron-0.9.2/setup.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-01-14 20:19:53.106849 autocron-0.9.2/tests/
--rw-r--r--   0 klaus      (501) staff       (20)     6161 2024-01-07 11:56:05.000000 autocron-0.9.2/tests/test_engine.py
--rw-r--r--   0 klaus      (501) staff       (20)    10640 2024-01-14 19:53:36.000000 autocron-0.9.2/tests/test_schedule.py
--rw-r--r--   0 klaus      (501) staff       (20)    29219 2024-01-09 17:12:11.000000 autocron-0.9.2/tests/test_sql_interface.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 13:40:02.153453 autocron-0.9.5/
+-rw-r--r--   0 klaus      (501) staff       (20)     1085 2024-04-03 12:57:14.000000 autocron-0.9.5/LICENSE.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       61 2024-04-03 13:00:18.000000 autocron-0.9.5/MANIFEST.in
+-rw-r--r--   0 klaus      (501) staff       (20)     3392 2024-04-15 13:40:02.153362 autocron-0.9.5/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)     2193 2024-01-13 16:36:00.000000 autocron-0.9.5/README.md
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 13:40:02.150464 autocron-0.9.5/autocron/
+-rw-r--r--   0 klaus      (501) staff       (20)     1284 2024-04-15 13:28:18.000000 autocron-0.9.5/autocron/__init__.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6929 2024-04-03 09:47:15.000000 autocron-0.9.5/autocron/admin.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6916 2024-04-15 13:28:09.000000 autocron-0.9.5/autocron/decorators.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7594 2024-04-09 10:05:02.000000 autocron-0.9.5/autocron/engine.py
+-rw-r--r--   0 klaus      (501) staff       (20)    10767 2024-02-14 08:16:16.000000 autocron-0.9.5/autocron/schedule.py
+-rw-r--r--   0 klaus      (501) staff       (20)    33910 2024-04-15 13:28:09.000000 autocron-0.9.5/autocron/sqlite_interface.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6101 2024-04-03 09:33:49.000000 autocron-0.9.5/autocron/worker.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 13:40:02.153124 autocron-0.9.5/autocron.egg-info/
+-rw-r--r--   0 klaus      (501) staff       (20)     3392 2024-04-15 13:40:02.000000 autocron-0.9.5/autocron.egg-info/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)      501 2024-04-15 13:40:02.000000 autocron-0.9.5/autocron.egg-info/SOURCES.txt
+-rw-r--r--   0 klaus      (501) staff       (20)        1 2024-04-15 13:40:02.000000 autocron-0.9.5/autocron.egg-info/dependency_links.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       49 2024-04-15 13:40:02.000000 autocron-0.9.5/autocron.egg-info/entry_points.txt
+-rw-r--r--   0 klaus      (501) staff       (20)        9 2024-04-15 13:40:02.000000 autocron-0.9.5/autocron.egg-info/top_level.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       81 2023-04-22 13:30:54.000000 autocron-0.9.5/pyproject.toml
+-rw-r--r--   0 klaus      (501) staff       (20)     1269 2024-04-15 13:40:02.153733 autocron-0.9.5/setup.cfg
+-rw-r--r--   0 klaus      (501) staff       (20)      135 2023-03-23 08:40:38.000000 autocron-0.9.5/setup.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 13:40:02.152815 autocron-0.9.5/tests/
+-rw-r--r--   0 klaus      (501) staff       (20)     3349 2024-04-15 13:28:09.000000 autocron-0.9.5/tests/test_decorators.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2412 2024-04-03 09:07:51.000000 autocron-0.9.5/tests/test_engine.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7652 2024-02-14 08:16:16.000000 autocron-0.9.5/tests/test_schedule.py
+-rw-r--r--   0 klaus      (501) staff       (20)    13980 2024-04-08 14:37:26.000000 autocron-0.9.5/tests/test_sqlite_interface.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1918 2024-04-08 14:37:26.000000 autocron-0.9.5/tests/test_worker.py
```

### Comparing `autocron-0.9.2/LICENSE.txt` & `autocron-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autocron-0.9.2/PKG-INFO` & `autocron-0.9.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: autocron
-Version: 0.9.2
+Version: 0.9.5
 Summary: Asynchronous background tasks for Python web-frameworks with no dependencies
 Home-page: https://github.com/kbr/autocron
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
 Project-URL: Homepage, https://github.com/kbr/autocron
 Project-URL: Code, https://github.com/kbr/autocron
 Project-URL: Issue tracker, https://github.com/kbr/autocron/issues
-Keywords: background task,web-framework,django,flask,pyramid,bottle,tornado,starlette
+Keywords: tasks,background,python
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # autocron
 
 ![](https://img.shields.io/pypi/pyversions/autocron.svg)
```

### Comparing `autocron-0.9.2/README.md` & `autocron-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `autocron-0.9.2/autocron/engine.py` & `autocron-0.9.5/autocron/engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 To use the Engine create an instance and call ``.start(filename)`` on
 this instance with the database filename to use as argument. The
 function ``start(filename)`` in the ``__init__.py`` module of autocron
 handles this.
 """
 
+import os
 import pathlib
 import signal
 import subprocess
 import sys
 import threading
 import time
-from types import SimpleNamespace
 
-from .sql_interface import SQLiteInterface
+from .sqlite_interface import SQLiteInterface
 
 
 WORKER_MODULE_NAME = "worker.py"
-WORKER_START_DELAY = 0.2
+WORKER_START_DELAY = 0.02
 
 
 def start_subprocess(database_file):
     """
     Starts the worker process in a detached subprocess. The
     `database_file` is a string with an absolute or relative path to the
     database in use.
@@ -32,68 +32,56 @@
     cmd = [sys.executable, worker_file]
     if database_file:
         cmd.append(database_file)
     cwd = pathlib.Path.cwd()
     return subprocess.Popen(cmd, cwd=cwd)
 
 
-def run_worker_monitor(exit_event, database_file):
-    """
-    Starts the worker processes and monitors that the workers are up and
-    running. Restart workers if necessary. This function must run in a
-    separate thread. The 'exit_event' is a threading.Event() instance
-    and the `database_file` is a string with an absolute or relative
-    path to the database in use. If the monitor receives an exit_event
-    the running workers are terminated and the function will return,
-    terminating its own thread as well.
-    """
-    processes = []
-    interface = SQLiteInterface()
-    interface.db_name = database_file
-    max_workers = interface.get_max_workers()
-    for _ in range(max_workers):
-        process = start_subprocess(database_file)
-        processes.append(SimpleNamespace(pid=process.pid, process=process))
-        # don't start multiple workers too fast one after the other
-        # because they may run into a sqlite write-lock. This will not cause
-        # a wrong behaviour on starting, monitoring and stopping the workers
-        # but can lead to a wrong statistic in the autocron admin/setting.
-        time.sleep(WORKER_START_DELAY)
-    while True:
-        for entry in processes:
-            if entry.process.poll() is not None:
-                # trouble: process is not running any more.
-                # deregister the terminated process from the setting
-                # and start a new process.
-                interface.decrement_running_workers(entry.pid)
-                new_process = start_subprocess(database_file)
-                entry.pid = new_process.pid
-                entry.process = new_process
-                # in case more than one process needs a restart:
-                time.sleep(WORKER_START_DELAY)
-        idle_time = interface.get_monitor_idle_time()
-        if exit_event.wait(timeout=idle_time):
-            break
-    for entry in processes:
-        entry.process.terminate()
-
-
 class Engine:
     """
     The Engine is the entry-point for autocron. Starting the engine will
     start the monitor thread. The monitor-thread in turn starts and
     supervise the workers. (The interface argument is used for testing.)
     """
     def __init__(self, interface=None):
         # the ìnterface argument is for testing. In production this
         # argument is not provided for initialization.
         self.interface = interface if interface else SQLiteInterface()
         self.exit_event = None
         self.monitor_thread = None
         self.orig_signal_handlers = {}
+        self.processes = []
+
+    def worker_monitor(self):
+        """
+        Starts the worker processes and monitors that the workers are up
+        and running. Restart workers if necessary. This function must
+        run in a separate thread. The 'exit_event' is a
+        threading.Event() instance and the `database_file` is a string
+        with an absolute or relative path to the database in use. If the
+        monitor receives an exit_event the function will return,
+        terminating its own thread.
+        """
+        database_file = self.interface.db_name
+        timeout = self.interface.monitor_idle_time
+
+        for _ in range(self.interface.max_workers):
+            self.processes.append(start_subprocess(database_file))
+            time.sleep(WORKER_START_DELAY)
+
+        while True:
+            for process in self.processes:
+                if process.poll() is not None:
+                    self.interface.decrement_running_workers(process.pid)
+                    self.processes.remove(process)
+                    self.processes.append(start_subprocess(database_file))
+                    # in case more workers need a restart:
+                    time.sleep(WORKER_START_DELAY)
+            if self.exit_event.wait(timeout=timeout):
+                break
 
     def set_signal_handlers(self):
         """
         Set self._terminate() as handler for a couple of
         termination-signals and store the orinal handlers for this
         signals.
         """
@@ -103,76 +91,106 @@
             signal.SIGABRT,
             signal.SIGHUP,  # availablity: Unix
         ]
         for signalnum in signalnums:
             self.orig_signal_handlers[signalnum] = signal.getsignal(signalnum)
             signal.signal(signalnum, self._terminate)
 
-    def start(self, database_file):
+    def start(self, database_file, workers=None):
         """
         Starts the autocron worker in case autocron is active and no
         other application process has already started the workers. The
-        *database_file* argument is a string with the name of the
+        ``database_file`` argument is a string with the name of the
         database to use (like "the_application.db") or a Path instance.
         If the name represents a relative path, the database is stored
         in the ``~/.autocron`` directory. This directory will get
         created if not already existing. If the name represents an
         absolute path, then this path will be used as is. In this case
         all directories of the path must exist.
 
-        The function returns a boolean: True if workers have been
-        started and False otherwise. A return value of False does not
-        mean, that no workers are running – another application process
-        may have be first.
+        The ``workers`` argument takes the number of workers (as
+        integer) and stores this value in the database. If the value is
+        ``None`` (default) the number of workers is taken from the
+        database.
+
+        The function returns a boolean: ``True`` if workers have been
+        started and ``False`` otherwise. A return value of ``False``
+        does not mean that no workers are running – another application
+        process may have been first on aquiring the rights to start and
+        monitor the worker processes.
         """
+        result = False
         self.interface.init_database(database_file)
-        if (
-            self.interface.autocron_lock_is_set
-            or self.interface.monitor_lock_flag_is_set
-        ):
-            # in both cases start is not allowed
-            return False
-        self.interface.set_monitor_lock_flag(True)
-        # this is a safety check for not starting more than
-        # one monitor thread:
-        if not self.monitor_thread:
+
+        # don't start the engine if autocron is not active:
+        if self.interface.autocron_lock:
+            return result
+
+        # autocron is active:
+        # check whether start() has been called from a worker process
+        # (this can happen depending on the framework architecture)
+        pid = os.getpid()
+        if self.interface.is_worker_pid(pid):
+            # in this case the engine should not start
+            return result
+
+        # check whether the process monitors the workers,
+        # but dont't start the monitor twice:
+        if self.interface.acquire_monitor_lock() and not self.monitor_thread:
+
+            # adapt number of workers if given
+            if workers is not None:
+                # override the already loaded value
+                self.interface.max_workers = workers
+                # and update the settings
+                settings = self.interface.get_settings()
+                settings.max_workers = workers
+                self.interface.update_settings(settings)
+
             self.set_signal_handlers()
             self.exit_event = threading.Event()
-            self.monitor_thread = threading.Thread(
-                target=run_worker_monitor,
-                args=(self.exit_event, database_file)
-            )
+            self.monitor_thread = threading.Thread(target=self.worker_monitor)
             self.monitor_thread.start()
-        return True
+            result = True
+
+        # start the registrator thread to populate the database:
+        self.interface.registrator.start()
+        return result
 
     def stop(self):
         """
-        Shut down the monitor-thread which in turn will stop all running
-        workers. Also release the monitor_lock flag.
+        Terminate the workers and tear-down the database. This method is
+        called when the application itself terminates. It is not
+        necessary to call this method directly.
         """
         if self.monitor_thread:
             # check for self.exit_event for a test-scenario.
             # in production if self.monitor_thread is not None
             # self.exit_event is also not None
             if self.exit_event:
+                # terminate the monitor thread
                 self.exit_event.set()
             self.monitor_thread = None
-            settings = self.interface.get_settings()
-            settings.monitor_lock = False
-            # in case of a crash the workers will terminate but
-            # may not reliable reset their states. So do it here:
-            settings.running_workers = 0
-            settings.worker_pids = ""
-            self.interface.set_settings(settings)
-            self.interface.delete_cronjobs()
+
+        # terminate the workers (if any) here in the main process:
+        # don't do this in the monitor thread, because the monitor thread
+        # may be unable to send the terminate signal to all workers before
+        # the main process terminates.
+        for process in self.processes:
+            process.terminate()
+
+        # stop registration and clean up the database
+        self.interface.registrator.stop()
+        self.interface.tear_down_database()
 
     def _terminate(self, signalnum, stackframe=None):
         """
         Terminate autocron by calling the engine.stop() method.
         Afterward reraise the signal again for the original
         signal-handler.
         """
-        # stackframe may be given to the signal-handler, but is unused
+        # a stackframe may be given to the signal-handler
+        # which is not used here.
         # pylint: disable=unused-argument
         self.stop()
         signal.signal(signalnum, self.orig_signal_handlers[signalnum])
         signal.raise_signal(signalnum)  # requires Python >= 3.8
```

### Comparing `autocron-0.9.2/autocron/sql_interface.py` & `autocron-0.9.5/autocron/sqlite_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,69 @@
 """
-sql_interface.py
+The sqlite interface.
 
-SQLite interface for storing tasks.
-
-The autocron database consists of three tables:
-task: stores all tasks that should get executed later
-result: stores all results from task returning a result
-settings: configuration settings for a project
+Data models, sql-definition and access routines.
 """
 
+# some structures are larger than pylint likes:
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-instance-attributes
+
+
 import datetime
+import functools
 import pathlib
 import pickle
+import queue
 import sqlite3
-import types
+import threading
+import time
 
 
 DEFAULT_STORAGE = ".autocron"
+REGISTER_BACKGROUND_TASK_TIMEOUT = 2.0
 
+SQLITE_OPERATIONAL_ERROR_RETRIES = 100
+SQLITE_OPERATIONAL_ERROR_DELAY = 0.01
+SQLITE_DELAY_INCREMENT_STEPS = 20
+SQLITE_DELAY_INCREMENT_FACTOR = 1.5
+
+SQLITE_EXCLUSIVE_ACCESS = "BEGIN EXCLUSIVE"
+
+SETTINGS_DEFAULT_WORKERS = 1
+SETTINGS_DEFAULT_RUNNING_WORKERS = 0
+SETTINGS_DEFAULT_MONITOR_LOCK = False
+SETTINGS_DEFAULT_AUTOCRON_LOCK = False
+SETTINGS_DEFAULT_MONITOR_IDLE_TIME = 5  # seconds
+SETTINGS_DEFAULT_WORKER_IDLE_TIME = 0  # 0 seconds means auto idle time
+SETTINGS_DEFAULT_WORKER_PIDS = ""
+SETTINGS_DEFAULT_RESULT_TTL = 1800  # Storage time (time to live) in seconds
+
+SETTINGS_DEFAULT_DATA = {
+    "max_workers": SETTINGS_DEFAULT_WORKERS,
+    "running_workers": SETTINGS_DEFAULT_RUNNING_WORKERS,
+    "monitor_lock": SETTINGS_DEFAULT_MONITOR_LOCK,
+    "autocron_lock": SETTINGS_DEFAULT_AUTOCRON_LOCK,
+    "monitor_idle_time": SETTINGS_DEFAULT_MONITOR_IDLE_TIME,
+    "worker_idle_time": SETTINGS_DEFAULT_WORKER_IDLE_TIME,
+    "worker_pids": SETTINGS_DEFAULT_WORKER_PIDS,
+    "result_ttl": SETTINGS_DEFAULT_RESULT_TTL
+}
 
-# -- table: task - structure and commands ------------------------------------
-DB_TABLE_NAME_TASK = "task"
-CMD_CREATE_TASK_TABLE = f"""
-CREATE TABLE IF NOT EXISTS {DB_TABLE_NAME_TASK}
-(
-    uuid TEXT,
-    schedule datetime,
-    status INTEGER,
-    crontab TEXT,
-    function_module TEXT,
-    function_name TEXT,
-    function_arguments BLOB
-)
-"""
-CMD_STORE_TASK = f"""
-INSERT INTO {DB_TABLE_NAME_TASK} VALUES
-(
-    :uuid,
-    :schedule,
-    :status,
-    :crontab,
-    :function_module,
-    :function_name,
-    :function_arguments
-)
-"""
-TASK_COLUMN_SEQUENCE =\
-    "rowid,uuid,schedule,status,crontab,"\
-    "function_module,function_name,function_arguments"
-CMD_GET_TASKS_BY_NAME =f"""
-    SELECT {TASK_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_TASK}
-    WHERE function_module == ? AND function_name == ?"""
-CMD_GET_TASKS_ON_DUE = f"""
-    SELECT {TASK_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_TASK}
-    WHERE schedule <= ?"""
-CMD_GET_TASKS_ON_DUE_WITH_STATUS = CMD_GET_TASKS_ON_DUE + " AND status == ?"
-CMD_GET_TASKS = f"""
-    SELECT {TASK_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_TASK}"""
-CMD_UPDATE_TASK_STATUS = f"""
-    UPDATE {DB_TABLE_NAME_TASK} SET status = ? WHERE rowid == ?"""
-CMD_GET_CRONTASKS = f"""
-    SELECT  {TASK_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_TASK}
-    WHERE crontab <> ''"""
-CMD_UPDATE_CRONTASK_SCHEDULE = f"""
-    UPDATE {DB_TABLE_NAME_TASK} SET schedule = ?, status = ? WHERE rowid == ?"""
-CMD_DELETE_TASK = f"DELETE FROM {DB_TABLE_NAME_TASK} WHERE rowid == ?"
-CMD_DELETE_CRON_TASKS = f"DELETE FROM {DB_TABLE_NAME_TASK} WHERE crontab <> ''"
-CMD_COUNT_TABLE_ROWS = "SELECT COUNT(*) FROM {table_name}"
+BOOLEAN_SETTINGS = ["monitor_lock", "autocron_lock"]
 
 # Status codes used for task-status the result-entries:
 TASK_STATUS_WAITING = 1
 TASK_STATUS_PROCESSING = 2
 TASK_STATUS_READY = 3
 TASK_STATUS_ERROR = 4
 TASK_STATUS_UNAVAILABLE = 5
 
 
-# -- table: result - structure and commands ----------------------------------
-DB_TABLE_NAME_RESULT = "result"
-CMD_CREATE_RESULT_TABLE = f"""
-CREATE TABLE IF NOT EXISTS {DB_TABLE_NAME_RESULT}
-(
-    uuid TEXT PRIMARY KEY,
-    status INTEGER,
-    function_module TEXT,
-    function_name TEXT,
-    function_arguments BLOB,
-    function_result BLOB,
-    error_message TEXT,
-    ttl datetime
-)
-"""
-
-# Storage time (time to live) for results in seconds
-RESULT_TTL = 1800
-
-CMD_STORE_RESULT = f"""
-INSERT INTO {DB_TABLE_NAME_RESULT} VALUES
-(
-    :uuid,
-    :status,
-    :function_module,
-    :function_name,
-    :function_arguments,
-    :function_result,
-    :error_message,
-    :ttl
-)
-"""
-RESULT_COLUMN_SEQUENCE =\
-    "rowid,uuid,status,function_module,function_name,"\
-    "function_arguments,function_result,error_message, ttl"
-CMD_GET_RESULTS = f"""
-    SELECT {RESULT_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_RESULT}"""
-CMD_GET_RESULT_BY_UUID = f"""
-    SELECT {RESULT_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_RESULT}
-    WHERE uuid == ?"""
-CMD_UPDATE_RESULT = f"""
-    UPDATE {DB_TABLE_NAME_RESULT} SET
-        status = ?,
-        function_result = ?,
-        error_message = ?,
-        ttl = ?
-    WHERE uuid == ?"""
-# CMD_DELETE_RESULT = f"""\
-#     DELETE FROM {DB_TABLE_NAME_RESULT} WHERE uuid == ?"""
-CMD_DELETE_OUTDATED_RESULTS = f"""
-    DELETE FROM {DB_TABLE_NAME_RESULT}
-    WHERE status == {TASK_STATUS_READY} AND ttl <= ?"""
-
-
-# -- table: settings - structure and commands --------------------------------
-DB_TABLE_NAME_SETTINGS = "settings"
-CMD_CREATE_SETTINGS_TABLE = f"""
-CREATE TABLE IF NOT EXISTS {DB_TABLE_NAME_SETTINGS}
-(
-    max_workers INTEGER,
-    running_workers INTEGER,
-    monitor_lock INTEGER,
-    autocron_lock INTEGER,
-    monitor_idle_time REAL,
-    worker_idle_time REAL,
-    worker_pids TEXT,
-    result_ttl INTEGER
-)
-"""
-
-DEFAULT_MAX_WORKERS = 1
-DEFAULT_RUNNING_WORKERS = 0
-DEFAULT_MONITOR_LOCK = 0
-DEFAULT_AUTOCRON_LOCK = 0
-DEFAULT_MONITOR_IDLE_TIME = 5.0  # seconds
-DEFAULT_WORKER_IDLE_TIME = 2.0  # seconds
-DEFAULT_WORKER_PIDS = ""
-
-CMD_SETTINGS_STORE_VALUES = f"""
-INSERT INTO {DB_TABLE_NAME_SETTINGS} VALUES
-(
-    :max_workers,
-    :running_workers,
-    :monitor_lock,
-    :autocron_lock,
-    :monitor_idle_time,
-    :worker_idle_time,
-    :worker_pids,
-    :result_ttl
-)
-"""
-SETTINGS_COLUMN_SEQUENCE =\
-    "rowid,max_workers,running_workers,"\
-    "monitor_lock,autocron_lock,"\
-    "monitor_idle_time,worker_idle_time,"\
-    "worker_pids,result_ttl"
-BOOLEAN_SETTINGS = ["monitor_lock", "autocron_lock"]
-CMD_SETTINGS_GET_SETTINGS = f"""
-    SELECT {SETTINGS_COLUMN_SEQUENCE} FROM {DB_TABLE_NAME_SETTINGS}"""
-CMD_SETTINGS_UPDATE = f"""
-    UPDATE {DB_TABLE_NAME_SETTINGS} SET
-        max_workers = ?,
-        running_workers = ?,
-        monitor_lock = ?,
-        autocron_lock = ?,
-        monitor_idle_time = ?,
-        worker_idle_time = ?,
-        worker_pids = ?,
-        result_ttl = ?
-    WHERE rowid == ?"""
-
-
 # sqlite3 default adapters and converters deprecated as of Python 3.12:
-
 def datetime_adapter(value):
     """
     Gets a python datetime-instance and returns an ISO 8601 formated
     string for sqlite3 storage.
     """
     return value.isoformat()
 
@@ -206,696 +76,943 @@
     return datetime.datetime.fromisoformat(value.decode())
 
 
 sqlite3.register_adapter(datetime.datetime, datetime_adapter)
 sqlite3.register_converter("datetime", datetime_converter)
 
 
-# pylint does not like instances with dynamic attributes:
-# pylint: disable=attribute-defined-outside-init
-class HybridNamespace(types.SimpleNamespace):
+# sqlite3: decorator for SQLiteInterface-methods accessing the database
+def db_access(function):
     """
-    A namespace-object with additional dictionary-like attribute access.
+    Access decorator. Repeats the decorated function several times in
+    case the database is locked because of write- or exclusive-access.
     """
-    def __init__(self, data=None):
-        """
-        Set initial values.
-        If data is given, it must be a dictionary.
-        """
-        if data is not None:
-            self.__dict__.update(data)
 
-    def __getitem__(self, name):
-        return self.__dict__[name]
+    @functools.wraps(function)
+    def wrapper(*args, **kwargs):
+        """
+        Repeat the wrapped function call in case of an OperationalError.
+        If this fails for SQLITE_MAX_RETRY_LIMIT times, the original
+        error is raised.
+        """
+        message = ""
+        delay = SQLITE_OPERATIONAL_ERROR_DELAY
+        for retry_num in range(SQLITE_OPERATIONAL_ERROR_RETRIES):
+            try:
+                return function(*args, **kwargs)
+            except sqlite3.OperationalError as err:
+                message = str(err)
+                time.sleep(delay)
+            if not retry_num % SQLITE_DELAY_INCREMENT_STEPS:
+                delay *= SQLITE_DELAY_INCREMENT_FACTOR
+        raise sqlite3.OperationalError(message)
+    return wrapper
 
-    def __setitem__(self, name, value):
-        self.__dict__[name] = value
 
-    def __len__(self):
-        return len(self.__dict__)
+class Model:
+    """
+    Base model for the table classes for common sql-creation and access
+    methods.
+    """
 
-    def __repr__(self):
-        return "\n".join(f"{k}:{v}" for k, v in self.__dict__.items())
+    # class attributes to redefine in subclasses:
+    table_name = ""
+    columns = {}
+
+    def __init__(self, connection=None):
+        self.connection = connection
+        self.rowid = None
+
+    def store(self):
+        """
+        Store a new row. data is a dictionary with all column data.
+        After storage the instance-attribute `rowid` will be set.
+        """
+        columns = ",".join(f":{name}" for name in self.columns)
+        sql = f"""INSERT INTO {self.table_name} VALUES ({columns})
+                  RETURNING rowid"""
+        cursor = self.connection.run(sql, self.__dict__)
+        result = cursor.fetchone()
+        # result is a tuple representing the RETURNING values
+        # from the sql command. In this case it is a tuple with
+        # a single entry holding the new created rowid:
+        self.rowid = result[0]
+        return self.rowid
+
+    def update(self):
+        """Make the current set of attributes persistent.
+        """
+        columns = ",".join(f"{name} = :{name}" for name in self.columns)
+        sql = f"""UPDATE {self.table_name} SET {columns}
+                  WHERE rowid == :rowid"""
+        self.connection.run(sql, self.__dict__)
 
-    def __str__(self):
-        # same as __repr__ but without the rowid
-        lines = repr(self).split("\n")
-        lines = [line for line in lines if not line.startswith("rowid")]
-        return "\n".join(lines)
+    def delete(self):
+        """Delete this instance by the rowid.
+        """
+        sql = f"DELETE FROM {self.table_name} WHERE rowid == {self.rowid}"
+        self.connection.run(sql)
 
+    @classmethod
+    def _get_sql_select(cls):
+        """Helper function for the select-classmethods.
+        """
+        columns = list(cls.columns.keys())
+        columns.append("rowid")
+        columns = ",".join(columns)
+        return f"SELECT {columns} FROM {cls.table_name}"
 
-class TaskResult(HybridNamespace):
-    """
-    Helper class to make task-results more handy.
-    """
+    @classmethod
+    def select(cls, connection, rowid=None, sql=None, data=None):
+        """
+        Returns an instance depending on the arguments or None if no
+        entry matches. If just `rowid` is given makes a lookup by the
+        `rowid`. Otherwise `sql` and `data` must be given to make
+        specific selection.
+        """
+        if rowid is not None:
+            # simple select by rowid
+            sql = cls._get_sql_select()
+            sql = f"{sql} WHERE rowid == :rowid"
+            data = {"rowid": rowid}
+        cursor = connection.run(sql, data)
+        cursor.row_factory = getattr(cls, "row_factory", None)
+        data = cursor.fetchone()
+        instance = None
+        if data:
+            instance = cls(connection)
+            instance.__dict__.update(data)
+        return instance
 
-    def _refresh(self):
+    @classmethod
+    def select_all(cls, connection):
         """
-        If the status is TASK_STATUS_WAITING try to update the
-        task_result dictionary with data retrieved from the database.
-        This will return a new task_result instance. If the new instance
-        is still in waiting status, do nothing. Otherwise update
-        self.__dict__ with the retrieved data.
-        The `interface` argument is for testing.
+        Select all entries from a table and returns a list of
+        model-instances. If there is no entry in the table an empty list
+        is returned.
+        """
+        sql = cls._get_sql_select()
+        cursor = connection.run(sql)
+        cursor.row_factory = getattr(cls, "row_factory", None)
+        data_set = cursor.fetchall()
+        instances = []
+        for data in data_set:
+            instance = cls(connection)
+            instance.__dict__.update(data)
+            instances.append(instance)
+        return instances
+
+    @classmethod
+    def create_table(cls, connection):
+        """Create the database table for the model if not already existing.
         """
-        if self.status == TASK_STATUS_WAITING:
-            try:
-                result = self.interface.get_result_by_uuid(self.uuid)
-            except AttributeError:
-                pass
-            else:
-                if result is not None:
-                    self.__dict__.update(result.__dict__)
+        columns = ",".join(
+            f"{field} {type}" for field, type in cls.columns.items()
+        )
+        connection.run(
+            f"CREATE TABLE IF NOT EXISTS {cls.table_name}({columns})"
+        )
 
-    @property
-    def result(self):
+    @classmethod
+    def count_rows(cls, connection):
+        """Return the number of rows in the table.
         """
-        Shortcut to access the result. If the result is not available
-        because the task still waits to get executed an AttributeError
-        with the message "result not available" is raised.
-        """
-        if self.status == TASK_STATUS_READY:
-            return self.function_result
-        raise AttributeError("result not available.")
+        cursor = connection.run(f"SELECT COUNT(*) FROM {cls.table_name}")
+        return cursor.fetchone()[0]
 
-    @property
-    def is_waiting(self):
-        """indicates task still waiting to get processed."""
-        self._refresh()
-        return self.status == TASK_STATUS_WAITING
 
-    @property
-    def is_ready(self):
-        """indicates task has been processed."""
-        self._refresh()
-        return self.status == TASK_STATUS_READY
+class Task(Model):
+    """Model to store functions for later execution.
+    """
 
-    @property
-    def has_error(self):
-        """indicates error_message is set."""
-        self._refresh()
-        return self.status == TASK_STATUS_ERROR
+    table_name = "task"
+    columns = {
+        "uuid": "TEXT",
+        "schedule": "datetime",
+        "status": "INTEGER",
+        "crontab": "TEXT",
+        "function_module": "TEXT",
+        "function_name": "TEXT",
+        "function_arguments": "BLOB"
+    }
+
+    def __init__(
+        self,
+        connection=None,
+        func=None,
+        args=(),
+        kwargs=None,
+        uuid="",
+        crontab="",
+        schedule=None,
+        status=TASK_STATUS_WAITING
+    ):
+        super().__init__(connection=connection)
+        self.func = func
+        self.args = args
+        self.kwargs = kwargs
+        self.uuid = uuid
+        self.crontab = crontab
+        self.schedule = schedule
+        self.status = status
+        self.function_module = None
+        self.function_name = None
+        self.function_arguments = None
+
+    def store(self):
+        """
+        Store a new task in the database. Returns the rowid of the new dataset.
+        """
+        if self.schedule is None:
+            self.schedule = datetime.datetime.now()
+        if self.func:
+            self.function_module = self.func.__module__
+            self.function_name = self.func.__name__
+        else:
+            self.function_module = ""
+            self.function_name = ""
+        self.function_arguments = pickle.dumps((self.args, self.kwargs))
+        super().store()
+
+    def update(self):
+        """Make the current state of attributes persistent.
+        """
+        # function arguments may have changed:
+        self.function_arguments = pickle.dumps((self.args, self.kwargs))
+        super().update()
 
     @classmethod
-    def from_data_tuple(cls, row_data):
-        """
-        Returns a new TaskResult-Instance initialized with a tuple
-        representing the data from result-table row.
+    def _get_next_task_sql_and_data(cls):
+        """Helper method for next_task and next_cron_task.
         """
-        column_names = RESULT_COLUMN_SEQUENCE.split(",")
-        data = dict(zip(column_names, row_data))
-        instance = cls(data)
-        instance.function_result = pickle.loads(instance.function_result)
-        instance.function_arguments = pickle.loads(instance.function_arguments)
-        return instance
+        sql = cls._get_sql_select()
+        sql = f"""{sql} WHERE schedule <= :schedule
+                  AND status == {TASK_STATUS_WAITING}"""
+        data = {"schedule": datetime.datetime.now()}
+        return sql, data
 
     @classmethod
-    def from_function_call(cls, func, *args, **kwargs):
+    def get_by_function_name(cls, function, connection):
         """
-        Renturns a new TaskResult-Instance with the result from the
-        given function executed with the given arguments. This exists
-        for type consistency to return a TaskResult from delay-decorated
-        functions even if autotask is inactive.
+        Return a task instance identified by the given function or None
+        if no task is found.
         """
+        sql = cls._get_sql_select()
+        sql = f"""{sql} WHERE function_module == :function_module
+                        AND function_name == :function_name"""
         data = {
-            "function_result": func(*args, **kwargs),
-            "function_arguments": (args, kwargs),
-            "status": TASK_STATUS_READY
+            "function_module": function.__module__,
+            "function_name": function.__name__
         }
-        return cls(data)
+        return cls.select(connection=connection, sql=sql, data=data)
 
     @classmethod
-    def from_registration(cls, uuid, interface):
+    def next_task(cls, connection):
+        """Returns a task instance which is on due.
         """
-        Returns a TaskResult-Instance with the state
-        TASK_STATUS_WAITING, the result None and a set uuid. This
-        instance can be used to call the ``update()`` method for a
-        delayed result.
+        sql, data = cls._get_next_task_sql_and_data()
+        return cls.select(connection, sql=sql, data=data)
+
+    @classmethod
+    def next_cron_task(cls, connection):
+        """Returns a crontask instance which is on due.
         """
-        data = {
-            "function_result": None,
-            "status": TASK_STATUS_WAITING,
-            "uuid": uuid,
-            "interface": interface
-        }
-        return cls(data)
+        sql, data = cls._get_next_task_sql_and_data()
+        sql = f"{sql} AND crontab <> ''"
+        return cls.select(connection, sql=sql, data=data)
 
     @classmethod
-    def from_none(cls):
+    def delete_crontasks(cls, connection):
+        """Delete all task which are cron-tasks.
         """
-        Returns a new empty TaskResult-Instance if there is no waiting
-        function to call and no result to expect. The available
-        attributes are 'status' with the value TASK_STATUS_UNAVAILABLE and
-        the 'result' has the value None. All other attributes are
-        undefined and accessing them will raise an AttributeError.
+        sql = f"DELETE FROM {cls.table_name} WHERE crontab <> ''"
+        connection.run(sql)
+
+    @classmethod
+    def change_status(cls, connection, prev_status, new_status):
+        """Change the status of a task from a given one to a new one.
         """
-        data = {
-            "status": TASK_STATUS_UNAVAILABLE,
-            "function_result": None
-        }
-        return cls(data)
+        sql = f"""UPDATE {cls.table_name} SET status = :new_status
+                  WHERE status == :prev_status"""
+        data = {"prev_status": prev_status, "new_status": new_status}
+        connection.run(sql, data)
+
+    @staticmethod
+    def row_factory(cursor, row):
+        """
+        SQLite factory class to convert a row from a task-table to a
+        dictionary.
+        """
+        function_arguments_column_name = "function_arguments"
+        data = {}
+        column_names = [entry[0] for entry in cursor.description]
+        for name, value in zip(column_names, row):
+            if name == function_arguments_column_name:
+                args, kwargs = pickle.loads(value)
+                data["args"] = args
+                data["kwargs"] = kwargs
+            else:
+                data[name] = value
+        return data
 
 
-# pylint: disable=too-many-public-methods
-class SQLiteInterface:
-    """
-    SQLite interface for application specific operations.
-    This class is a Singleton.
+class Result(Model):
+    """The model to store function result of delayed executed tasks.
     """
 
-    _instance = None
-
-    def __new__(cls):
-        if cls._instance is None:
-            cls._instance = super().__new__(cls)
-        return cls._instance
+    table_name = "result"
+    columns = {
+        "uuid": "TEXT PRIMARY KEY",
+        "status": "INTEGER",
+        "function_module": "TEXT",
+        "function_name": "TEXT",
+        "function_arguments": "BLOB",
+        "function_result": "BLOB",
+        "error_message": "TEXT",
+        "ttl": "datetime"
+    }
 
-    def __init__(self):
-        self._preregistered_tasks = []
-        self._result_ttl = datetime.timedelta(seconds=RESULT_TTL)
-        self._accept_registrations = True
-        self._db_name = None
-        self.autocron_lock_is_set = None
+    def __init__(
+        self,
+        connection=None,
+        func=None,
+        args=(),
+        kwargs=None,
+        function_result=None,
+        error_message="",
+        uuid="",
+        status=TASK_STATUS_WAITING,
+        ttl=None,
+        function_name = "",
+        function_module = "",
+        function_arguments = None,
+        rowid = None
+    ):
+        super().__init__(connection=connection)
+        self.rowid = rowid
+        self.func = func
+        self.args = args
+        self.kwargs = kwargs
+        self.uuid = uuid
+        self.status = status
+        self.function_name = function_name
+        self.function_module = function_module
+        self.function_arguments = function_arguments
+        self.function_result = function_result
+        self.error_message = error_message
+        self.ttl = ttl if ttl else datetime.datetime.now()
 
     @property
-    def db_name(self):
-        """Return hidden _db_name (because of the setter)"""
-        return self._db_name
-
-    @db_name.setter
-    def db_name(self, db_name):
+    def has_error(self):
         """
-        Expand the given database filename to the storage-location path
-        if the filename is not an absolute path. In the latter case the
-        absolute path will get used (and must exist). If db_name is None
-        set None directly.
+        Returns True if the error message is not empty. The return value
+        is invalid as long as ``is_ready()`` does not return True.
         """
-        if db_name is None:
-            self._db_name = None
-        else:
-            self._set_storage_location(db_name)
+        return bool(self.error_message)
 
     @property
-    def accept_registrations(self):
+    def result(self):
         """
-        Return a boolean whether callables are allowed to get registered
-        in the database.
+        Shortcut for the attribute ``function_result``. The return value is invalid as
+        long as ``is_ready()`` does not return True.
         """
-        return self._accept_registrations and not self.autocron_lock_is_set
+        return self.function_result
 
-    @accept_registrations.setter
-    def accept_registrations(self, value):
-        """
-        Setter for the hidden _accept_registrations flag (because of the
-        getter)
+    def is_ready(self):
         """
-        self._accept_registrations = value
+        Returns ``True`` if the task has been processed, otherwise ``False``. If
+        the task has been processed the result may be available or an
+        error-message may be set.
+
+        Note for async frameworks: this is a *blocking call*.
+        """
+        processed_states = (TASK_STATUS_READY, TASK_STATUS_ERROR)
+        if self.status not in processed_states:
+            # connect to database for a refresh of the data
+            interface = SQLiteInterface()
+            result = interface.get_result_by_uuid(uuid=self.uuid)
+            if result is not None:
+                self.__dict__.update(result.__dict__)
+            return self.status in processed_states
+        return True
+
+    def store(self):
+        """Stores the result as a new entry in the result-table.
+        """
+        if self.func:
+            self.function_module = self.func.__module__
+            self.function_name = self.func.__name__
+        else:
+            self.function_module = ""
+            self.function_name = ""
+        self.function_arguments = pickle.dumps((self.args, self.kwargs))
+        self.function_result = pickle.dumps(self.function_result)
+        super().store()
 
-    @property
-    def is_initialized(self):
-        """Flag whether the database is available."""
-        return self._db_name is not None
-
-    def _init_database(self):
-        """
-        Creates a new database in case that an older one is not existing
-        and in case of missing settings set the settings-default values.
-        """
-        self._create_tables()
-        self._initialize_settings_table()
-        settings = self.get_settings()
-        self.autocron_lock_is_set = settings.autocron_lock
-        self._result_ttl = datetime.timedelta(seconds=settings.result_ttl)
-
-    def _create_tables(self):
-        """
-        Create all used tables in case of a new db and missing tables.
-        """
-        self._execute(CMD_CREATE_TASK_TABLE)
-        self._execute(CMD_CREATE_RESULT_TABLE)
-        self._execute(CMD_CREATE_SETTINGS_TABLE)
-
-    def _initialize_settings_table(self):
-        """
-        Check for an existing settings row in the settings-table.
-        If there is no row create an entry with the default values.
-        """
-        rows = self._count_table_rows(DB_TABLE_NAME_SETTINGS)
-        if not rows:
-            data = {
-                "max_workers": DEFAULT_MAX_WORKERS,
-                "running_workers": DEFAULT_RUNNING_WORKERS,
-                "monitor_lock": DEFAULT_MONITOR_LOCK,
-                "autocron_lock": DEFAULT_AUTOCRON_LOCK,
-                "monitor_idle_time": DEFAULT_MONITOR_IDLE_TIME,
-                "worker_idle_time": DEFAULT_WORKER_IDLE_TIME,
-                "worker_pids": DEFAULT_WORKER_PIDS,
-                "result_ttl": RESULT_TTL
-            }
-            self._execute(CMD_SETTINGS_STORE_VALUES, data)
-
-    def _count_table_rows(self, table_name):
-        """
-        Helper function to count the number of entries in the given
-        table. Returns a numeric value. In case of an unknown table_name
-        a sqlite3.OperationalError will get raised.
-        """
-        cmd = CMD_COUNT_TABLE_ROWS.format(table_name=table_name)
-        cursor = self._execute(cmd)
-        number_of_rows = cursor.fetchone()[0]
-        return number_of_rows
-
-    def _execute(self, cmd, parameters=(), many=False):
-        """
-        Run a command with parameters. Parameters can be a sequence of
-        values to get used in an ordered way or a dictionary with
-        key-value pairs, where the key are the value-names used in the
-        db (i.e. the column names).
-        If 'many' is true then con.executemany() gets called and
-        parameters is interpreted differently as as sequence of ordered
-        tuples or dictionaries as placehoöders for the provided cmd.
-        """
-        if self._db_name is None:
-            raise IOError("No autocron database defined.")
-        con = sqlite3.connect(
-            self._db_name,
-            detect_types=sqlite3.PARSE_DECLTYPES
+    @classmethod
+    def from_registration(cls, func, args, kwargs, uuid="",
+                          status=TASK_STATUS_WAITING,
+                          function_result=None, error_message=""):
+        """
+        Return a new instance with the given arguments as attributes.
+        """
+        return cls(
+            func=func, args=args, kwargs=kwargs, uuid=uuid,
+            function_result=function_result,status=status,
+            error_message=error_message
         )
-        with con:
-            if many:
-                return con.executemany(cmd, parameters)
-            return con.execute(cmd, parameters)
-
-    def _set_storage_location(self, db_name):
-        """
-        Set the database file location. If the path is absolute use the
-        path as is. The directory part of the path must exist. If the
-        path is relative the database file gets stored in the
-        '~.autocron/' directory. If no home directory is found on the
-        running platform the current working directory is used as a
-        fallback. However in such cases it would be safer to provide an
-        absolute path to the database location.
-        """
-        path = pathlib.Path(db_name)
-        if not path.is_absolute():
-            try:
-                path = pathlib.Path.home() / DEFAULT_STORAGE / path.name
-            except RuntimeError:
-                # no home directory found
-                path = pathlib.Path.cwd() / db_name
-        self._db_name = path
 
-    def _preregister_task(self, data):
+    @classmethod
+    def from_uuid(cls, connection, uuid):
         """
-        Take the data, which is a dictionary,and convert it to another
-        dict without the key 'self'. Pickle the dict and append it to
-        _preregistered tasks.
+        Returns a Result instance from the database with the given uuid.
+        If there is no entry return None.
         """
-        data = {k: v for k, v in data.items() if k != "self"}
-        self._preregistered_tasks.append(data)
+        sql = cls._get_sql_select()
+        sql = f"{sql} WHERE uuid == :uuid"
+        data = {"uuid": uuid}
+        return cls.select(connection, sql=sql, data=data)
 
-    def _register_preregistered_tasks(self):
-        """
-        Run the stored registrations on the now up and
-        running database.
+    @classmethod
+    def delete_outdated(cls, connection, schedule):
         """
-        for data in self._preregistered_tasks:
-            self.register_callable(**data)
-
-    def init_database(self, db_name):
+        Delete all result entries where the ttl is <= schedule.
+        (ttl is a datetime object and works as a timestamp for storage.)
         """
-        Public callable for delayed initialization. Set the database
-        (which is a string or Path) and runs the correponding
-        initialization.
-        """
-        if not self.is_initialized:
-            self._set_storage_location(db_name)
-            self._init_database()
-            # ignore the result, but set new state:
-            self.get_tasks_on_due(
-                status=TASK_STATUS_PROCESSING,
-                new_status=TASK_STATUS_WAITING
-            )
-            self._register_preregistered_tasks()
-
-
-    # -- task-methods ---
+        sql = f"""DELETE FROM {cls.table_name}
+                  WHERE status <> {TASK_STATUS_WAITING}
+                  AND ttl <= :ttl"""
+        connection.run(sql, {"ttl": schedule})
 
     @staticmethod
-    def _fetch_all_callable_entries(cursor):
+    def row_factory(cursor, row):
         """
-        Internal function to iterate over a selection of entries and unpack
-        the columns to a dictionary with the following key-value pairs:
-
-            {
-                "rowid": integer,
-                "uuid": string,
-                "schedule": datetime,
-                "status": integer,
-                "crontab": string,
-                "function_module": string,
-                "function_name": string,
-                "args": tuple(of original datatypes),
-                "kwargs": dict(of original datatypes),
-            }
-
-        Returns a list of HybridNamespace instances or an empty list if
-        a selection does not match any row.
-        """
-        def process(row):
-            """
-            Gets a `row` and returns a dictionary with Python datatypes.
-            `row` is an ordered tuple of columns as defined in `CREATE
-            TABLE`. The blob column with the pickled arguments is the
-            last column.
-            """
-            args, kwargs = pickle.loads(row[-1])
-            data = {
-                key: row[i] for i, key in enumerate(
-                    TASK_COLUMN_SEQUENCE.strip().split(",")[:-1]
-                )
-            }
-            data["args"] = args
-            data["kwargs"] = kwargs
-            return HybridNamespace(data)
+        SQLite factory class to convert a row from the result-table to a
+        dictionary.
+        """
+        data = {}
+        column_names = [entry[0] for entry in cursor.description]
+        for name, value in zip(column_names, row):
+            if name in ("function_arguments", "function_result"):
+                data[name] = pickle.loads(value)
+            else:
+                data[name] = value
+        return data
 
-        return [process(row) for row in cursor.fetchall()]
 
-    # pylint: disable=too-many-arguments
-    def register_callable(
-        self,
-        func,
-        uuid="",
-        schedule=None,
-        status=TASK_STATUS_WAITING,
-        crontab="",
-        args=None,
-        kwargs=None,
-        unique=False,
-    ):
-        """
-        Store a callable in the task-table of the database. If the
-        argument `unique` is given, don't register a callable twice. In
-        this case an already registered callable with the same
-        signature (module.name) gets overwritten. This can be useful for
-        cron-tasks to not register them multiple times.
-        """
-        if self.is_initialized:
-            if unique:
-                tasks = self.get_tasks_by_signature(func)
-                for task in tasks:
-                    self.delete_callable(task)
-            if not schedule:
-                schedule = datetime.datetime.now()
-            if args is None:
-                args = ()
-            if kwargs is None:
-                kwargs = {}
-            arguments = pickle.dumps((args, kwargs))
-            data = {
-                "uuid": uuid,
-                "schedule": schedule,
-                "status": status,
-                "crontab": crontab,
-                "function_module": func.__module__,
-                "function_name": func.__name__,
-                "function_arguments": arguments,
-            }
-            self._execute(CMD_STORE_TASK, data)
-            if uuid:
-                self.register_result(func, uuid, args=args, kwargs=kwargs)
-        else:
-            self._preregister_task(locals())
+class Settings(Model):
+    """
+    Model with a single entry in the database storing the settings.
+    """
 
-    def get_tasks(self):
-        """
-        Generic method to return all tasks as a list of HybridNamespace
-        instances.
-        """
-        cursor = self._execute(CMD_GET_TASKS)
-        return self._fetch_all_callable_entries(cursor)
+    table_name = "settings"
+    columns = {
+        "max_workers": "INTEGER",
+        "running_workers": "INTEGER",
+        "monitor_lock": "INTEGER",
+        "autocron_lock": "INTEGER",
+        "monitor_idle_time": "INTEGER",
+        "worker_idle_time": "INTEGER",
+        "worker_pids": "TEXT",
+        "result_ttl": "INTEGER"
+    }
+
+    def __init__(self, connection=None, data=None):
+        """
+        Initializes settings with the values from data. data must be a
+        dictionary with key value pairs according the `columns` class
+        attribute. If data is not given the
+        SETTINGS_DEFAULT_DATA-dictionary is used to populate the
+        settings data.
+        """
+        super().__init__(connection)
+        data = data if data else SETTINGS_DEFAULT_DATA
+        self.__dict__.update(data)
 
-    def get_tasks_on_due(self, schedule=None, status=None, new_status=None):
+    def __repr__(self):
+        """Self representation used by the admin-tool.
         """
-        Returns tasks on due as a list of HybridNamespace instances. If
-        'status' is given the status is also used for the selection. If
-        'new_status' is given the selection gets updated with the new
-        status.
-        """
-        if not schedule:
-            schedule = datetime.datetime.now()
-        if status:
-            cursor = self._execute(
-                CMD_GET_TASKS_ON_DUE_WITH_STATUS,
-                [schedule, status]
-            )
-        else:
-            cursor = self._execute(CMD_GET_TASKS_ON_DUE, [schedule])
-        tasks = self._fetch_all_callable_entries(cursor)
-        if new_status and tasks:
-            values = [(new_status, task.rowid) for task in tasks]
-            self._execute(CMD_UPDATE_TASK_STATUS, values, many=True)
-            # also update the status in the previous fetched tasks:
-            for task in tasks:
-                task.status = new_status
-        return tasks
+        width = len(max(self.columns, key=len))
+        attributes = []
+        for key in self.columns:
+            value = self.__dict__[key]
+            attributes.append(f"{key:<{width}}: {value}")
+        return "\n".join(attributes)
 
-    def get_tasks_by_signature(self, func):
+    @classmethod
+    def read(cls, connection):
         """
-        Return all tasks matching the function-signature as a list of
-        HybridNamespace instances.
+        Returns a settings instance with data read from the database. If
+        there is no settings entry in the table returns None.
         """
-        parameters = func.__module__, func.__name__
-        cursor = self._execute(CMD_GET_TASKS_BY_NAME, parameters)
-        return self._fetch_all_callable_entries(cursor)
+        entries = cls.select_all(connection)
+        if not entries:
+            return None
+        return entries[0]
 
-    def delete_callable(self, entry):
+    @staticmethod
+    def row_factory(cursor, row):
         """
-        Delete the entry in the callable-table. Entry should be a
-        dictionary as returned from `get_tasks_on_due()`. The row to delete
-        gets identified by the `rowid`.
+        SQLite factory function to convert a row from a settings-table
+        to a dictionary.
         """
-        self._execute(CMD_DELETE_TASK, [entry["rowid"]])
+        column_names = [entry[0] for entry in cursor.description]
+        data = {name: bool(value) if name in BOOLEAN_SETTINGS else value
+                for name, value in zip(column_names, row)}
+        return data
 
-    def get_crontasks(self):
-        """
-        Return all crontasks as a list of HybridNamespace instances.
+
+class TaskRegistrator:
+    """
+    Handles the task registration in a separate thread so that
+    registration is a non-blocking operation.
+    """
+
+    def __init__(self, interface):
+        self.interface = interface
+        self.task_queue = queue.Queue()
+        self.exit_event = threading.Event()
+        self.registration_thread = None
+
+    def register(self, func, args=(), kwargs=None,
+                       crontab="", uuid="", schedule=None):
+        """
+        Register a task for later processing. Arguments are the same as
+        for `SQLiteInterface.register_task()` which is called from a
+        seperate thread.
         """
-        cursor = self._execute(CMD_GET_CRONTASKS)
-        return self._fetch_all_callable_entries(cursor)
+        if kwargs is None:
+            kwargs = {}
+        self.task_queue.put({
+            "func": func,
+            "schedule": schedule,
+            "crontab": crontab,
+            "uuid": uuid,
+            "args": args,
+            "kwargs": kwargs,
+        })
 
-    def delete_cronjobs(self):
+    def _process_queue(self):
         """
-        Delete all cronjobs from the task-table.
+        Register task in a separate thread taking the tasks from a
+        task_queue.
         """
-        self._execute(CMD_DELETE_CRON_TASKS)
+        while True:
+            try:
+                data = self.task_queue.get(
+                    timeout=REGISTER_BACKGROUND_TASK_TIMEOUT
+                )
+            except queue.Empty:
+                # check for exit_event on empty queue so the queue items
+                # can get handled before terminating the thread
+                if self.exit_event.is_set():
+                    break
+            else:
+                self.interface.register_task(**data)
 
-    def update_crontask_schedule(self, rowid, schedule):
+    def start(self):
         """
-        Update the `schedule` of the table entry with the given `rowid`.
-        As this should be a crontask the status is set to WAITING.
+        Start processing the queue in a seperate thread.
         """
-        parameters = schedule, TASK_STATUS_WAITING, rowid
-        self._execute(CMD_UPDATE_CRONTASK_SCHEDULE, parameters)
+        # don't start multiple threads
+        if self.registration_thread is None:
+            self.registration_thread = threading.Thread(
+                target=self._process_queue
+            )
+            self.registration_thread.start()
 
-    def count_tasks(self):
+    def stop(self):
         """
-        Returns the number of rows in the task-table, therefore
-        providing the number of tasks stored in the database.
+        Terminates the running registration thread.
         """
-        return self._count_table_rows(DB_TABLE_NAME_TASK)
+        if self.registration_thread:
+            self.exit_event.set()
+            self.registration_thread = None
 
 
-    # -- result-methods ---
+class SQLiteConnection:
+    """
+    SQLite connection. `run()` can get called as often as required. The
+    database keeps connected. Leaving the context will commit and close
+    the database connection. In case of an exception during the context
+    instead of a commit the connection will do a rollback.
+    """
 
-    @property
-    def result_ttl(self):
-        """
-        Returns the new ttl as a datetime instance with an offset of now.
-        """
-        return datetime.datetime.now() + self._result_ttl
+    def __init__(self, db_name, row_factory=None, exclusive=False):
+        self.row_factory = row_factory
+        self.db_name = db_name
+        self.connection = None
+        self.exclusive = exclusive
+
+    def __enter__(self):
+        self.connection = sqlite3.connect(
+            database=self.db_name,
+            detect_types=sqlite3.PARSE_DECLTYPES
+        )
+        if self.row_factory:
+            self.connection.row_factory = self.row_factory
+        if self.exclusive:
+            self.connection.execute(SQLITE_EXCLUSIVE_ACCESS)
+        return self
+
+    def __exit__(self, *args):
+        if any(args):
+            # there was an exception:
+            self.connection.rollback()
+        else:
+            self.connection.commit()
+        self.connection.close()
 
-    def register_result(
-            self,
-            func,
-            uuid,
-            args=(),
-            status=TASK_STATUS_WAITING,
-            kwargs=None,
-        ):
-        """
-        Register an entry in the result table of the database. The entry
-        stores the uuid and the status `False` as zero `0` because the
-        task is pending and no result available jet.
+    def run(self, command, parameters=(), many=None):
         """
-        if not kwargs:
-            kwargs = {}
-        arguments = pickle.dumps((args, kwargs))
-        data = {
-            "uuid": uuid,
-            "status": status,
-            "function_module": func.__module__,
-            "function_name": func.__name__,
-            "function_arguments": arguments,
-            "function_result": pickle.dumps(None),
-            "error_message": "",
-            "ttl": self.result_ttl,
-        }
-        self._execute(CMD_STORE_RESULT, data)
+        Runs an sql command with the given parameters. If the command
+        supports qmark style, the parameters must be a tuple with the
+        parameters in the proper order. If many is True, the parameters
+        must be a sequence of tuples.
+        If the command supports named style, parameters should be a
+        dictionary. If many is True, parameters should be a sequence of
+        dicts.
+        Returns the result of the given command.
+        """
+        if parameters and many is None:
+            # try to find out whether it is many or not:
+            if isinstance(parameters, (tuple, list)):
+                # could be qmark parameters or a sequence of tuples or dicts
+                # take the first element of the sequence, if this is another
+                # sequence or dict then these are parameters for an
+                # executemany() command, else just execute()
+                many = isinstance(parameters[0], (tuple, list, dict))
+        if many:
+            return self.connection.executemany(command, parameters)
+        return self.connection.execute(command, parameters)
 
-    def get_results(self):
-        """
-        Generic method to return all results as a list of TaskResult
-        instances.
-        """
-        cursor = self._execute(CMD_GET_RESULTS)
-        rows = cursor.fetchall()
-        return [TaskResult.from_data_tuple(row) for row in rows]
 
-    def get_result_by_uuid(self, uuid):
+Connection = SQLiteConnection
+
+
+class SQLiteInterface:
+    """
+    SQLite interface for application specific operations.
+    This class is a Singleton.
+    """
+
+    _instance = None
+
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+        return cls._instance
+
+    def __init__(self):
+        # run __init__ just once
+        if self.__dict__:
+            return
+        self._db_name = None
+        self._result_ttl = None
+        # accept_registrations will get set to False
+        # by the worker processes to not register callables by the workers
+        self.accept_registrations = True
+        # these attributes are set later by reading the settings:
+        self.autocron_lock = None
+        self.monitor_lock = None
+        self.monitor_idle_time = None
+        self.max_workers = None
+        self.worker_idle_time = None
+        # the registrator for non blocking registration:
+        self.registrator = TaskRegistrator(self)
+
+    @property
+    def db_name(self):
+        """Return hidden _db_name (because of the setter)"""
+        return self._db_name
+
+    @db_name.setter
+    def db_name(self, db_name):
         """
-        Return a dataset (as TaskResult) or None.
+        Expand the given database filename to the storage-location path
+        if the filename is not an absolute path. In the latter case the
+        absolute path will get used (and must exist). If db_name is None
+        set None directly.
         """
-        cursor = self._execute(CMD_GET_RESULT_BY_UUID, (uuid,))
-        row = cursor.fetchone()  # tuple of data or None
-        if row:
-            result = TaskResult.from_data_tuple(row)
+        if db_name is None:
+            self._db_name = None
         else:
-            result = None
-        return result
+            path = pathlib.Path(db_name)
+            if not path.is_absolute():
+                try:
+                    path = pathlib.Path.home() / DEFAULT_STORAGE / path.name
+                except RuntimeError:
+                    # no home directory found
+                    path = pathlib.Path.cwd() / db_name
+            self._db_name = path
 
-    def update_result(self, uuid, result=None, error_message=""):
+    @property
+    def result_ttl(self):
         """
-        Updates the result-entry with the given `uuid` to status 1|2 and
-        stores the `result` or `error_message`.
+        Returns the new ttl as a datetime instance with an offset of now.
         """
-        status = TASK_STATUS_ERROR if error_message else TASK_STATUS_READY
-        function_result = pickle.dumps(result)
-        ttl = self.result_ttl
-        parameters = status, function_result, error_message, ttl, uuid
-        self._execute(CMD_UPDATE_RESULT, parameters)
+        return datetime.datetime.now() + self._result_ttl
 
-    def count_results(self):
+    @result_ttl.setter
+    def result_ttl(self, value=SETTINGS_DEFAULT_RESULT_TTL):
         """
-        Returns the number of rows in the task-table, therefore
-        providing the number of tasks stored in the database.
+        Set the ttl as timedelta in seconds. This is the lifetime from
+        an offset to the future.
         """
-        return self._count_table_rows(DB_TABLE_NAME_RESULT)
+        self._result_ttl = datetime.timedelta(seconds=value)
 
-    def delete_outdated_results(self):
+    @db_access
+    def init_database(self, db_name):
         """
-        Deletes results with status TASK_STATUS_READY that have exceeded
-        the time to live (ttl).
+        Set the database name and set up initial data.
         """
-        now = datetime.datetime.now()
-        self._execute(CMD_DELETE_OUTDATED_RESULTS, (now,))
+        if not self.db_name:
+            self.db_name = db_name
+            with Connection(self.db_name, exclusive=True) as conn:
+                Task.create_table(conn)
+                Result.create_table(conn)
+                Settings.create_table(conn)
+
+                # try to read the settings. If this fails create the first
+                # (and only) settings dataset with the default values:
+                settings = Settings.read(conn)
+                if settings is None:
+                    settings = Settings(conn)  # this set the defaults
+                    settings.store()  # store defaults in the database
+
+                # set attributes from settings that don't change during runtime:
+                self.autocron_lock = settings.autocron_lock
+                self.monitor_lock = settings.monitor_lock
+                self.monitor_idle_time = settings.monitor_idle_time
+                self.max_workers = settings.max_workers
+                self.worker_idle_time = settings.worker_idle_time
+                self.result_ttl = settings.result_ttl
+
+    @db_access
+    def register_task(self, func, schedule=None, crontab="", uuid="",
+                      args=(), kwargs=None):
+        """
+        Store a callable in the task-table of the database. If the
+        callable is a delayed task with a potential result create also a
+        corresponding entry in the result table. If the callable is a
+        crontask, check whether the task is already registered and don't
+        register the callable again.
+        """
+        if self.accept_registrations:
+            if not schedule:
+                schedule = datetime.datetime.now()
+            if kwargs is None:
+                kwargs = {}
+            with Connection(self.db_name, exclusive=True) as conn:
+                if crontab and Task.get_by_function_name(func, conn):
+                    # don't register a crontab twice:
+                    return
+                task = Task(
+                    connection=conn,
+                    func=func,
+                    schedule=schedule,
+                    crontab=crontab,
+                    uuid=uuid,
+                    args=args,
+                    kwargs=kwargs
+                )
+                task.store()
 
-    # -- setting-methods ---
+                # if a uuid is given it is a delayed function that
+                # may return a result:
+                if uuid:
+                    result = Result(
+                        connection=conn,
+                        func=func,
+                        args=args,
+                        kwargs=kwargs,
+                        uuid=uuid,
+                        ttl=self.result_ttl
+                    )
+                    result.store()
+
+    @db_access
+    def get_next_task(self):
+        """
+        Returns the next task on due with crontasks first or None if
+        there is not task on due. If a task is returned the status is
+        set to TASK_STATUS_PROCESSING first.
+        """
+        with Connection(self.db_name, exclusive=True) as conn:
+            task = Task.next_cron_task(conn) or Task.next_task(conn)
+            if task:
+                task.status = TASK_STATUS_PROCESSING
+                task.update()
+        return task
+
+    @db_access
+    def update_task_schedule(self, task, schedule):
+        """Updates the schedule of the given task.
+        """
+        with Connection(self.db_name) as conn:
+            task.connection = conn
+            task.schedule = schedule
+            task.status = TASK_STATUS_WAITING
+            task.update()
 
-    def get_settings(self):
+    @db_access
+    def count_tasks(self):
+        """Return the number of entries in the task-table.
         """
-        Returns a HybridNamespace instance with the settings as attributes:
-        - max_workers
-        - running_workers
-        - monitor_lock
-        - autocron_lock
-        - monitor_idle_time
-        - worker_idle_time
-        - worker_pids
-        - result_ttl
-        - rowid (not a setting but included)
-        """
-        cursor = self._execute(CMD_SETTINGS_GET_SETTINGS)
-        row = cursor.fetchone()  # there is only one row
-        col_names = SETTINGS_COLUMN_SEQUENCE.split(",")
-        data = dict(zip(col_names, row))
-        for key in BOOLEAN_SETTINGS:
-            data[key] = bool(data[key])
-        return HybridNamespace(data)
-
-    def set_settings(self, settings):
-        """
-        Takes a HybridNamespace instance as settings
-        argument (like the one returned from get_settings) and updates
-        the setting values in the database.
-        """
-        data = (
-            settings.max_workers,
-            settings.running_workers,
-            int(settings.monitor_lock),
-            int(settings.autocron_lock),
-            settings.monitor_idle_time,
-            settings.worker_idle_time,
-            settings.worker_pids,
-            settings.result_ttl,
-            settings.rowid
-        )
-        self._execute(CMD_SETTINGS_UPDATE, data)
+        with Connection(self.db_name) as conn:
+            return Task.count_rows(conn)
 
-    def get_monitor_idle_time(self):
+    @db_access
+    def get_tasks(self):
+        """Return a list of all tasks.
         """
-        Convenience function to get the monitor_idle_time from the settings.
+        with Connection(self.db_name) as conn:
+            return Task.select_all(conn)
+
+    @db_access
+    def delete_task(self, task):
+        """Delete the task which may not have a valid connection-attribute.
         """
-        return self.get_settings().monitor_idle_time
+        # solution: inject a valid connection
+        with Connection(self.db_name) as conn:
+            task.connection = conn
+            task.delete()
 
-    def get_worker_idle_time(self):
+    @db_access
+    def get_result_by_uuid(self, uuid):
         """
-        Convenience function to get the worker_idle_time from the settings.
+        Return a Result instance from the database identified by the uuid.
         """
-        return self.get_settings().worker_idle_time
+        with Connection(self.db_name) as conn:
+            return Result.from_uuid(connection=conn, uuid=uuid)
 
-    def get_max_workers(self):
-        """
-        Convenience function to get the max_workers from the settings.
+    @db_access
+    def count_results(self):
+        """Return the number of entries in the task-table.
         """
-        return self.get_settings().max_workers
+        with Connection(self.db_name) as conn:
+            return Result.count_rows(conn)
 
-    @property
-    def monitor_lock_flag_is_set(self):
+    @db_access
+    def update_result(
+        self,
+        uuid,
+        result=None,
+        error_message="",
+        ttl=None
+    ):
         """
-        Returns the status of the monitor-lock flag..
+        Updates the result with the uuid with the values of the
+        arguments result and error_message.
         """
-        return self.get_settings().monitor_lock
+        function_result = pickle.dumps(result)
+        ttl = ttl if ttl else self.result_ttl
+        status = TASK_STATUS_ERROR if error_message else TASK_STATUS_READY
+        with Connection(self.db_name) as conn:
+            result = Result.from_uuid(conn, uuid=uuid)
+            result.function_result = function_result
+            result.function_arguments = pickle.dumps(result.function_arguments)
+            result.error_message = error_message
+            result.status = status
+            result.ttl = ttl
+            result.update()
 
-    def set_monitor_lock_flag(self, value):
-        """
-        Set monitor_lock flag to the given state.
+    @db_access
+    def delete_outdated_results(self):
+        """Delete all resuts with a ttl <= now.
         """
-        settings = self.get_settings()
-        settings.monitor_lock = value
-        self.set_settings(settings)
+        with Connection(self.db_name) as conn:
+            Result.delete_outdated(conn, datetime.datetime.now())
 
+    @db_access
     def increment_running_workers(self, pid):
         """
-        Increment the running_worker-setting by 1.
+        Add the pid to the worker pid-list and increase the running
+        worker num by 1.
         """
-        settings = self.get_settings()
-        if settings.worker_pids:
-            pids = settings.worker_pids.split(",")
-        else:
-            pids = []
-        pids.append(str(pid))
-        settings.worker_pids = ",".join(pids)
-        settings.running_workers += 1
-        self.set_settings(settings)
+        with Connection(self.db_name) as conn:
+            settings = Settings.read(connection=conn)
+            settings.worker_pids = f"{settings.worker_pids},{pid}".lstrip(",")
+            settings.running_workers += 1
+            settings.update()
 
+    @db_access
     def decrement_running_workers(self, pid):
         """
-        Decrement the running_worker-setting by 1.
-        But don't allow a value below zero.
+        Delete the pid from the worker_pids list and decrement the
+        running_workers counter.
         """
-        settings = self.get_settings()
-        if settings.worker_pids:
+        with Connection(self.db_name) as conn:
+            settings = Settings.read(connection=conn)
             pids = settings.worker_pids.split(",")
-        else:
-            pids = []
-        try:
-            pids.remove(str(pid))
-        except ValueError:
-            # can happen when decrement gets called before increment
-            # otherwise it is a weird error that should not happen
-            pass
-        else:
-            if settings.running_workers > 0:
-                settings.running_workers -= 1
-            settings.worker_pids = ",".join(pids)
-            self.set_settings(settings)
+            try:
+                pids.remove(str(pid))
+            except ValueError:
+                # pid not in list: ignore
+                pass
+            else:
+                settings.worker_pids = ",".join(pids)
+                settings.running_workers = len(pids)
+                settings.update()
+
+    @db_access
+    def is_worker_pid(self, pid):
+        """Check whether the provided pid is one of the worker pids.
+        """
+        with Connection(self.db_name) as conn:
+            settings = Settings.read(connection=conn)
+        pids = (int(p) for p in settings.worker_pids.split(",") if p)
+        return pid in pids
+
+    @db_access
+    def acquire_monitor_lock(self):
+        """
+        Tries to acquire the monitor-lock flag: if the flag is set to
+        False, then set it to True. Otherwise keep the flag as is.
+        Return True if the flag has been set to True, otherwise return
+        False.
+        """
+        with Connection(self.db_name, exclusive=True) as conn:
+            settings = Settings.read(connection=conn)
+            if not settings.monitor_lock:
+                settings.monitor_lock = True
+                settings.update()
+                return True
+            return False
+
+    @db_access
+    def get_settings(self):
+        """Returns the settings dataset.
+        """
+        with Connection(self.db_name) as conn:
+            return Settings.read(connection=conn)
+
+    @db_access
+    def update_settings(self, settings):
+        """Updates the settings dataset.
+        """
+        with Connection(self.db_name) as conn:
+            settings.connection = conn
+            settings.update()
+
+    @db_access
+    def tear_down_database(self):
+        """
+        Reset all settings here so that the workers don't have to access
+        the database again on shutdown.
+        """
+        # gets called from the engine in case the interface
+        # is the worker_master
+        with Connection(self.db_name, exclusive=True) as conn:
+            settings = Settings.read(conn)
+            settings.monitor_lock = False
+            settings.running_workers = 0
+            settings.worker_pids = ""
+            settings.update()
+            Task.delete_crontasks(conn)
+            # reset the status of unfinished tasks from the
+            # last run to handle them again:
+            Task.change_status(
+                conn,
+                prev_status=TASK_STATUS_PROCESSING,
+                new_status=TASK_STATUS_WAITING
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autocron-0.9.2/autocron/worker.py` & `autocron-0.9.5/autocron/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 worker.py
 
-worker class for handling cron and delegated tasks.
+worker class for handling cron- and delayed-tasks.
 """
 
 import importlib
 import os
 import signal
 import sys
 import time
 
-from autocron.schedule import (
-    CronScheduler,
-    get_periodic_schedule,
-)
-from autocron import sql_interface
+from autocron.schedule import CronScheduler
+from autocron import sqlite_interface
 
 
-WORKER_IDLE_TIME = 4.0  # seconds
+# base idle time (in seconds) for auto-calculation
+DEFAULT_WORKER_IDLE_TIME = 1
 
 
 class Worker:
     """
     Runs in a separate process for task-handling.
     Gets supervised and monitored from the engine.
     """
@@ -29,64 +27,88 @@
         self.active = True
         self.result = None
         self.error_message = None
         signal.signal(signal.SIGINT, self.terminate)
         signal.signal(signal.SIGTERM, self.terminate)
         # Get a SQLiteInterface instance 'as is' without the
         # initialization step to clean up tasks.
-        # Providing the databasename will set the dtatabase
-        # to initialized-state. So no new tasks are registered
-        # from a worker.
-        # (keep in mind that every worker runs in a separate process.)
-        self.interface = sql_interface.SQLiteInterface()
-        self.interface.db_name=database_filename
+        # Providing the databasename will set the database
+        # to an initialized-state.
+        self.interface = sqlite_interface.SQLiteInterface()
+        self.interface.init_database(database_filename)
+        # prevent the interface to register functions from the worker-process:
         self.interface.accept_registrations = False
+        self.worker_idle_time = self._get_worker_idle_time()
+
+    def _get_worker_idle_time(self):
+        """
+        If worker_idle_time is in auto-mode (value in database settings
+        is 0), then calculate the idle time based on the number of
+        active workers. A higher idle time is necessary on higher
+        numbers of workers to keep the sqlite database accessible and
+        reactive.
+        auto_idle time keeps 1 second for up to 8 workers. Then it adds
+        0.025 seconds per additional worker.
+        """
+        idle_time = self.interface.worker_idle_time
+        if not idle_time:
+            workers = self.interface.max_workers
+            default = DEFAULT_WORKER_IDLE_TIME
+            idle_time = max(default, default + 0.025 * (workers - 8))
+        return idle_time
 
     def terminate(self, *args):  # pylint: disable=unused-argument
         """
         Signal handler to stop the process, terminates the loop in
-        `run()`.
+        `run()`. As a signal handler terminate must accept optional
+        positional arguments.
         """
         self.active = False
 
     def run(self):
         """
         Main event loop for the worker. Takes callables and processes
         them as long as callables are available. Otherwise keep idle.
         """
         pid = os.getpid()
         self.interface.increment_running_workers(pid)
         while self.active:
-            if not self.handle_tasks():
+            if not self.handle_task():
                 # nothing to do, check for results to delete:
                 self.interface.delete_outdated_results()
-                time.sleep(self.interface.get_worker_idle_time())
-        self.interface.decrement_running_workers(pid)
+                # don't sleep too long in case of longer idle-times
+                # wake up at least every second to check for self.active
+                # to terminate as soon as possible:
+                idle_time = self.worker_idle_time
+                while idle_time > 0:
+                    time.sleep(min(1, idle_time))
+                    if not self.active:
+                        break
+                    idle_time -= 1
 
-    def handle_tasks(self):
+    def handle_task(self):
         """
-        Checks for tasks and process them. If there are no tasks to
+        Checks for a task on due and process the task. If there are no tasks to
         handle the method return `False` indicating that the main loop
-        can switch to idle state. If  tasks have been handled, the
+        can switch to idle state. If a task have been handled, the
         method return `True` to indicate that meanwhile more tasks may be
         waiting.
         """
-        tasks = self.interface.get_tasks_on_due(
-            status=sql_interface.TASK_STATUS_WAITING,
-            new_status=sql_interface.TASK_STATUS_PROCESSING
-        )
-        if tasks:
-            for task in tasks:
-                if self.active is False:
-                    # terminate as soon as possible
-                    return True
-                self.error_message = None
-                self.result = None
-                self.process_task(task)
-                self.postprocess_task(task)
+        task = self.interface.get_next_task()
+        if task:
+            if self.active is False:
+                # don't process the task and terminate as soon as possible.
+                # crontasks will register on next start again and unhandled
+                # task will remain in the database and marked as waiting
+                # on next start to get handled again.
+                return True
+            self.error_message = None
+            self.result = None
+            self.process_task(task)
+            self.postprocess_task(task)
             return True
         return False
 
     def process_task(self, task):
         """
         Handle the given task. The task is a dictionary as returned from
         SQLInterface._fetch_all_callable_entries(cursor):
@@ -121,25 +143,20 @@
                 uuid=task.uuid,
                 result=self.result,
                 error_message=self.error_message
             )
         if task.crontab:
             # if the task has a crontab calculate new schedule
             # and update the task-entry
-            schedule = get_periodic_schedule(task)
-            if schedule is None:
-                scheduler = CronScheduler(crontab=task.crontab)
-                schedule = scheduler.get_next_schedule()
-            self.interface.update_crontask_schedule(
-                rowid=task.rowid,
-                schedule=schedule
-            )
+            scheduler = CronScheduler(crontab=task.crontab)
+            schedule = scheduler.get_next_schedule()
+            self.interface.update_task_schedule(task, schedule)
         else:
             # not a cronjob: delete the task from the db
-            self.interface.delete_callable(task)
+            self.interface.delete_task(task)
 
 
 def start_worker():
     """subprocess entry-point"""
     # insert cwd of hosting application to pythonpath
     sys.path.insert(0, os.getcwd())
     # engine provides the database name as first argument:
```

### Comparing `autocron-0.9.2/autocron.egg-info/PKG-INFO` & `autocron-0.9.5/autocron.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: autocron
-Version: 0.9.2
+Version: 0.9.5
 Summary: Asynchronous background tasks for Python web-frameworks with no dependencies
 Home-page: https://github.com/kbr/autocron
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
 Project-URL: Homepage, https://github.com/kbr/autocron
 Project-URL: Code, https://github.com/kbr/autocron
 Project-URL: Issue tracker, https://github.com/kbr/autocron/issues
-Keywords: background task,web-framework,django,flask,pyramid,bottle,tornado,starlette
+Keywords: tasks,background,python
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # autocron
 
 ![](https://img.shields.io/pypi/pyversions/autocron.svg)
```

### Comparing `autocron-0.9.2/setup.cfg` & `autocron-0.9.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
 author = Klaus Bremer
 author_email = bremer@bremer-media.com
 platform = any
-keywords = background task, web-framework, django, flask, pyramid, bottle, tornado, starlette
+keywords = tasks, background, python
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: 3.13
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 
 [options]
 packages = autocron
 
 [options.entry_points]
```

