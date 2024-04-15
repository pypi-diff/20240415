# Comparing `tmp/pyorchestra-0.5.3.tar.gz` & `tmp/pyorchestra-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.5.3.tar", max compression
+gzip compressed data, was "pyorchestra-0.5.4.tar", max compression
```

## Comparing `pyorchestra-0.5.3.tar` & `pyorchestra-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2024-04-08 14:17:17.642952 pyorchestra-0.5.3/LICENSE
--rwxr-xr-x   0        0        0    25622 2024-04-08 14:17:17.642952 pyorchestra-0.5.3/README.md
--rwxr-xr-x   0        0        0       62 2024-04-08 14:17:17.642952 pyorchestra-0.5.3/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      655 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1294 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/main.py
--rwxr-xr-x   0        0        0    10221 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      531 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/backend.py
--rwxr-xr-x   0        0        0    19628 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/formatting.py
--rwxr-xr-x   0        0        0      168 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/job.py
--rwxr-xr-x   0        0        0     1575 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/models.py
--rwxr-xr-x   0        0        0    10720 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-08 14:17:17.646952 pyorchestra-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-15 14:33:34.358906 pyorchestra-0.5.4/LICENSE
+-rwxr-xr-x   0        0        0    25711 2024-04-15 14:33:34.358906 pyorchestra-0.5.4/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      655 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1294 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/main.py
+-rwxr-xr-x   0        0        0    10283 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      531 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/backend.py
+-rwxr-xr-x   0        0        0    19740 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/core.py
+-rwxr-xr-x   0        0        0      873 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/formatting.py
+-rwxr-xr-x   0        0        0      168 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/job.py
+-rwxr-xr-x   0        0        0     1575 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/models.py
+-rwxr-xr-x   0        0        0    10720 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    26585 1970-01-01 00:00:00.000000 pyorchestra-0.5.4/PKG-INFO
```

### Comparing `pyorchestra-0.5.3/LICENSE` & `pyorchestra-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/README.md` & `pyorchestra-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -251,44 +251,45 @@
                     tzinfo=<DstTzInfo 'Europe/Berlin' LMT+1:16:00             
                     STD>))                                                      
            ...
            INFO     Orchestra starting                                core.py:82
 ╭────────┬──────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
 │State   │ Shedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
 ├────────┼──────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
-│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin │ 0:36:09  │ 0/1      │ gpu     │
-│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin │ 0:28:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
+│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
-│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin │ 0:38:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin │ 14:23:09 │ 0/1      │ gpu     │
+│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
 │Running │ CYCLIC   │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
-│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin │ 2:46:09  │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin │ 18:38:09 │ 0/inf    │ gpu     │
-│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin │ 4:23:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin │ 2 days   │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin │ 0:26:09  │ 0/inf    │ gpu     │
-│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin │ 0:00:24  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin │ 28 days  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin │ 2 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin │ 3 days   │ 0/1      │ gpu     │
+│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
+│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
+│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin │ 0:38:23  │ 0/inf    │ gpu     │
+│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
 │Running │ WEEKLY   │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
 ╰────────┴──────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
 ╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 ### Pausing and resuming jobs
+
 ```python
 import asyncio
 import datetime
 
 import pytz
 from scheduler import trigger
 
@@ -313,33 +314,33 @@
 async def main():
     await orchestra.create_schedule()
 
     # schedule a regular python function, this won't be tracked in the database and Orchestra does not support resuming such jobs in case of a shutdown
     orchestra.scheduler.cyclic(timing=datetime.timedelta(seconds=10), alias="Hello World every 10s", handle=hello)
 
     # schedule a Celery task function, Orchestra fully supports scheduling Celery tasks programmatically as well as through a schedule definition
-    orchestra.schedule_celery_task(schedule=orchestra.scheduler.cyclic,
-                                   timing=datetime.timedelta(seconds=1),
-                                   task=simple_task,
-                                   job_name="Simple task every 1s",
-                                   tags={"latency", "gpu"})
-
-    orchestra.schedule_celery_task(schedule=orchestra.scheduler.weekly,
-                                   timing=trigger.Monday(datetime.time(hour=16, minute=30, tzinfo=pytz.timezone("Europe/Berlin"))),
-                                   task=simple_task,
-                                   job_name="Simple task every Monday at 16:30 UTC",
-                                   tags={"cpu"})
+    job1 = orchestra.schedule_celery_task(schedule=orchestra.scheduler.cyclic,
+                                          timing=datetime.timedelta(seconds=1),
+                                          task=simple_task,
+                                          job_name="Simple task every 1s",
+                                          tags={"latency", "gpu"})
+
+    job2 = orchestra.schedule_celery_task(schedule=orchestra.scheduler.weekly,
+                                          timing=trigger.Monday(datetime.time(hour=16, minute=30, tzinfo=pytz.timezone("Europe/Berlin"))),
+                                          task=simple_task,
+                                          job_name="Simple task every Monday at 16:30 UTC",
+                                          tags={"cpu"})
 
-    # you may pause a task by name or by matching tags
+    # you may pause a task by name, references or by matching tags
     orchestra.pause_job("Simple task every Monday at 16:30 UTC")
 
-    orchestra.pause_jobs_with_tags({"latency"}, any_tag=True)
+    orchestra.pause_jobs({job1, job2})
 
     # resume job by name or by matching tags
-    orchestra.resume_jobs_with_tags({"latency"}, any_tag=True)
+    orchestra.resume_jobs(orchestra.get_jobs(tags={"latency"}))
 
     await orchestra.run()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `pyorchestra-0.5.3/orchestra/api/dto/job.py` & `pyorchestra-0.5.4/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/dto/run.py` & `pyorchestra-0.5.4/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/dto/schedule_definition.py` & `pyorchestra-0.5.4/orchestra/api/dto/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/dto/task.py` & `pyorchestra-0.5.4/orchestra/api/dto/task.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/main.py` & `pyorchestra-0.5.4/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/routers/jobs.py` & `pyorchestra-0.5.4/orchestra/api/routers/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
              {
                  "name": schedule_definition.name,
                  "task": schedule_definition.task,
                  "enabled": True,
                  "schedule": {
                      "timing": schedule_definition.timing,
                      "timezone": schedule_definition.timezone or "utc"
-                 }
+                 },
+                 "tags": set(schedule_definition.tags or [])
              }
          ]}]
     instance.add_schedules(module_definition, attempt_resume=schedule_definition.resume or False)
 
 
 @router.get("/jobs", tags=["jobs"])
 async def get_jobs(tags: Annotated[list[str] | None, Query(description="Optional list of tags to filter scheduled jobs")] = None,
```

### Comparing `pyorchestra-0.5.3/orchestra/api/routers/tags.py` & `pyorchestra-0.5.4/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/api/routers/tasks.py` & `pyorchestra-0.5.4/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/backend.py` & `pyorchestra-0.5.4/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/core.py` & `pyorchestra-0.5.4/orchestra/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,26 +143,26 @@
             self, job_name: str, module_name: str, task_name: str, additional_options: dict) -> Callable:
         module = importlib.import_module(module_name)
         task: celery.Task = getattr(module, task_name)
 
         return self.wrap_celery_task(job_name, task, additional_options)
 
     def schedule_celery_task(self, job_name: str, task: Callable, schedule: Callable[..., Job], timing: datetime.datetime | datetime.timedelta | datetime.time | Weekday,
-                             tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None):
+                             tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None) -> StatefulJob | None:
         module_name, _, task_name = task.name.rpartition(".")  # type:ignore
-        self.schedule_job(job_name=job_name, module_name=module_name, task_name=task_name, schedule=schedule, timing=timing, tags=tags, attempt_resume=attempt_resume,
-                          additional_options=additional_options)
+        return self.schedule_job(job_name=job_name, module_name=module_name, task_name=task_name, schedule=schedule, timing=timing, tags=tags, attempt_resume=attempt_resume,
+                                 additional_options=additional_options)
 
     async def create_schedule(self, module_definitions: list[dict] = None, loop=None) -> None:
         self.scheduler = self.scheduler or Scheduler(tzinfo=pytz.utc, loop=self.get_event_loop(loop))
         if module_definitions is not None:
             self.add_schedules(module_definitions)
 
     def schedule_job(self, job_name: str, module_name: str, task_name: str, schedule: Callable[..., Job], timing: datetime.datetime | datetime.timedelta | datetime.time | Weekday,
-                     tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None, schedule_definition: Any = None):
+                     tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None, schedule_definition: Any = None) -> StatefulJob | None:
         session = self.backend.ResultSession()
         with session_cleanup(session):
             resume_parameters: dict = {}
             if attempt_resume:
                 logs = (
                     select(Run)
                     .where(Run.job == job_name)
@@ -211,14 +211,16 @@
                 logger.warning(
                     f"Job {job_name} was scheduled to run {timing}, resuming using {last_running_time_local}, tz={last_run.timezone} as reference time."
                     f" Next run at {next_run_local}, tz={last_run.timezone}"
                 )
             else:
                 logger.info(f"Job {job_name} was scheduled to run {timing}")
 
+            return StatefulJob(job, is_paused=False)
+
     def add_schedules(self, module_definitions: list[dict], attempt_resume: bool = True):
         for index, block in enumerate(module_definitions or []):
             block_name: str = block.get("name", f"{index + 1}. schedule block")
             block_module: str | None = block.get("module")
 
             if block_module is None:
                 error_message: str = f"Module is undefined for {block_name}. Definition:\n\n{pretty_print_block(block)}"
```

### Comparing `pyorchestra-0.5.3/orchestra/formatting.py` & `pyorchestra-0.5.4/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/models.py` & `pyorchestra-0.5.4/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/orchestra/scheduling.py` & `pyorchestra-0.5.4/orchestra/scheduling.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.3/pyproject.toml` & `pyorchestra-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.5.3"
+version = "0.5.4"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.5.3/PKG-INFO` & `pyorchestra-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.5.3
+Version: 0.5.4
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -274,44 +274,45 @@
                     tzinfo=<DstTzInfo 'Europe/Berlin' LMT+1:16:00             
                     STD>))                                                      
            ...
            INFO     Orchestra starting                                core.py:82
 ╭────────┬──────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
 │State   │ Shedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
 ├────────┼──────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
-│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin │ 0:36:09  │ 0/1      │ gpu     │
-│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin │ 0:28:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
+│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
-│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin │ 0:38:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin │ 14:23:09 │ 0/1      │ gpu     │
+│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
 │Running │ CYCLIC   │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
-│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin │ 2:46:09  │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin │ 18:38:09 │ 0/inf    │ gpu     │
-│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin │ 4:23:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin │ 2 days   │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin │ 0:26:09  │ 0/inf    │ gpu     │
-│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin │ 0:00:24  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin │ 28 days  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin │ 2 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin │ 3 days   │ 0/1      │ gpu     │
+│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
+│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
+│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
+│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
 │Running │ ONCE     │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin │ 0:38:23  │ 0/inf    │ gpu     │
+│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
 │Running │ CYCLIC   │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
 │Running │ WEEKLY   │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
 ╰────────┴──────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
 ╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 ### Pausing and resuming jobs
+
 ```python
 import asyncio
 import datetime
 
 import pytz
 from scheduler import trigger
 
@@ -336,33 +337,33 @@
 async def main():
     await orchestra.create_schedule()
 
     # schedule a regular python function, this won't be tracked in the database and Orchestra does not support resuming such jobs in case of a shutdown
     orchestra.scheduler.cyclic(timing=datetime.timedelta(seconds=10), alias="Hello World every 10s", handle=hello)
 
     # schedule a Celery task function, Orchestra fully supports scheduling Celery tasks programmatically as well as through a schedule definition
-    orchestra.schedule_celery_task(schedule=orchestra.scheduler.cyclic,
-                                   timing=datetime.timedelta(seconds=1),
-                                   task=simple_task,
-                                   job_name="Simple task every 1s",
-                                   tags={"latency", "gpu"})
-
-    orchestra.schedule_celery_task(schedule=orchestra.scheduler.weekly,
-                                   timing=trigger.Monday(datetime.time(hour=16, minute=30, tzinfo=pytz.timezone("Europe/Berlin"))),
-                                   task=simple_task,
-                                   job_name="Simple task every Monday at 16:30 UTC",
-                                   tags={"cpu"})
+    job1 = orchestra.schedule_celery_task(schedule=orchestra.scheduler.cyclic,
+                                          timing=datetime.timedelta(seconds=1),
+                                          task=simple_task,
+                                          job_name="Simple task every 1s",
+                                          tags={"latency", "gpu"})
+
+    job2 = orchestra.schedule_celery_task(schedule=orchestra.scheduler.weekly,
+                                          timing=trigger.Monday(datetime.time(hour=16, minute=30, tzinfo=pytz.timezone("Europe/Berlin"))),
+                                          task=simple_task,
+                                          job_name="Simple task every Monday at 16:30 UTC",
+                                          tags={"cpu"})
 
-    # you may pause a task by name or by matching tags
+    # you may pause a task by name, references or by matching tags
     orchestra.pause_job("Simple task every Monday at 16:30 UTC")
 
-    orchestra.pause_jobs_with_tags({"latency"}, any_tag=True)
+    orchestra.pause_jobs({job1, job2})
 
     # resume job by name or by matching tags
-    orchestra.resume_jobs_with_tags({"latency"}, any_tag=True)
+    orchestra.resume_jobs(orchestra.get_jobs(tags={"latency"}))
 
     await orchestra.run()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

