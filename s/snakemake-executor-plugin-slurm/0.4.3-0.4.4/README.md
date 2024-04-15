# Comparing `tmp/snakemake_executor_plugin_slurm-0.4.3.tar.gz` & `tmp/snakemake_executor_plugin_slurm-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.3.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm-0.4.4.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm-0.4.3.tar` & `snakemake_executor_plugin_slurm-0.4.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/LICENSE
--rw-r--r--   0        0        0      319 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/README.md
--rw-r--r--   0        0        0     1152 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    20487 2024-04-12 08:17:08.233040 snakemake_executor_plugin_slurm-0.4.3/snakemake_executor_plugin_slurm/__init__.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/LICENSE
+-rw-r--r--   0        0        0      319 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/README.md
+-rw-r--r--   0        0        0     1151 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    20100 2024-04-15 09:17:24.183849 snakemake_executor_plugin_slurm-0.4.4/snakemake_executor_plugin_slurm/__init__.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.4.4/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm-0.4.3/LICENSE` & `snakemake_executor_plugin_slurm-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm-0.4.3/pyproject.toml` & `snakemake_executor_plugin_slurm-0.4.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm"
-version = "0.4.3"
+version = "0.4.4"
 description = "A Snakemake executor plugin for submitting jobs to a SLURM cluster."
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
@@ -12,16 +12,16 @@
 repository = "https://github.com/snakemake/snakemake-executor-plugin-slurm"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/executor/slurm.html"
 keywords = ["snakemake", "plugin", "executor", "cluster", "slurm"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 snakemake-interface-common = "^1.13.0"
-snakemake-interface-executor-plugins = "^9.0.0"
-snakemake-executor-plugin-slurm-jobstep = "^0.1.10"
+snakemake-interface-executor-plugins = "^9.1.1"
+snakemake-executor-plugin-slurm-jobstep = "^0.2.0"
 throttler = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 flake8 = "^6.1.0"
 coverage = "^7.3.1"
 pytest = "^7.4.2"
```

### Comparing `snakemake_executor_plugin_slurm-0.4.3/snakemake_executor_plugin_slurm/__init__.py` & `snakemake_executor_plugin_slurm-0.4.4/snakemake_executor_plugin_slurm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from snakemake_interface_executor_plugins.executors.base import SubmittedJobInfo
 from snakemake_interface_executor_plugins.executors.remote import RemoteExecutor
 from snakemake_interface_executor_plugins.settings import CommonSettings
 from snakemake_interface_executor_plugins.jobs import (
     JobExecutorInterface,
 )
 from snakemake_interface_common.exceptions import WorkflowError
+from snakemake_executor_plugin_slurm_jobstep import get_cpus_per_task
 
 
 # Required:
 # Specify common settings shared by various executors.
 common_settings = CommonSettings(
     # define whether your executor plugin executes locally
     # or remotely. In virtually all cases, it will be remote execution
@@ -122,26 +123,15 @@
         if job.resources.get("mpi", False):
             if job.resources.get("nodes", False):
                 call += f" --nodes={job.resources.get('nodes', 1)}"
 
         # fixes #40 - set ntasks regarlless of mpi, because
         # SLURM v22.05 will require it for all jobs
         call += f" --ntasks={job.resources.get('tasks', 1)}"
-
-        cpus_per_task = job.threads
-        if job.resources.get("cpus_per_task"):
-            if not isinstance(cpus_per_task, int):
-                raise WorkflowError(
-                    f"cpus_per_task must be an integer, but is {cpus_per_task}"
-                )
-            cpus_per_task = job.resources.cpus_per_task
-        # ensure that at least 1 cpu is requested
-        # because 0 is not allowed by slurm
-        cpus_per_task = max(1, cpus_per_task)
-        call += f" --cpus-per-task={cpus_per_task}"
+        call += f" --cpus-per-task={get_cpus_per_task(job)}"
 
         if job.resources.get("slurm_extra"):
             call += f" {job.resources.slurm_extra}"
 
         exec_job = self.format_job_exec(job)
 
         # ensure that workdir is set correctly
```

### Comparing `snakemake_executor_plugin_slurm-0.4.3/PKG-INFO` & `snakemake_executor_plugin_slurm-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Snakemake executor plugin for submitting jobs to a SLURM cluster.
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: snakemake-executor-plugin-slurm-jobstep (>=0.1.10,<0.2.0)
+Requires-Dist: snakemake-executor-plugin-slurm-jobstep (>=0.2.0,<0.3.0)
 Requires-Dist: snakemake-interface-common (>=1.13.0,<2.0.0)
-Requires-Dist: snakemake-interface-executor-plugins (>=9.0.0,<10.0.0)
+Requires-Dist: snakemake-interface-executor-plugins (>=9.1.1,<10.0.0)
 Requires-Dist: throttler (>=1.2.2,<2.0.0)
 Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/executor/slurm.html
 Project-URL: Repository, https://github.com/snakemake/snakemake-executor-plugin-slurm
 Description-Content-Type: text/markdown
 
 # Snakemake executor plugin: slurm
```

