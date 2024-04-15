# Comparing `tmp/RunRunner-0.1.2.tar.gz` & `tmp/RunRunner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RunRunner-0.1.2.tar", last modified: Thu Mar 28 14:21:53 2024, max compression
+gzip compressed data, was "RunRunner-0.1.3.tar", last modified: Mon Apr 15 15:36:29 2024, max compression
```

## Comparing `RunRunner-0.1.2.tar` & `RunRunner-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-03-28 14:21:53.728817 RunRunner-0.1.2/
--rw-r--r--   0 thijssnelleman   (501) staff       (20)     1684 2024-03-28 14:21:53.728710 RunRunner-0.1.2/PKG-INFO
-drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-03-28 14:21:53.727528 RunRunner-0.1.2/RunRunner.egg-info/
--rw-r--r--   0 thijssnelleman   (501) staff       (20)     1684 2024-03-28 14:21:53.000000 RunRunner-0.1.2/RunRunner.egg-info/PKG-INFO
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      329 2024-03-28 14:21:53.000000 RunRunner-0.1.2/RunRunner.egg-info/SOURCES.txt
--rw-r--r--   0 thijssnelleman   (501) staff       (20)        1 2024-03-28 14:21:53.000000 RunRunner-0.1.2/RunRunner.egg-info/dependency_links.txt
--rw-r--r--   0 thijssnelleman   (501) staff       (20)       14 2024-03-28 14:21:53.000000 RunRunner-0.1.2/RunRunner.egg-info/requires.txt
--rw-r--r--   0 thijssnelleman   (501) staff       (20)       10 2024-03-28 14:21:53.000000 RunRunner-0.1.2/RunRunner.egg-info/top_level.txt
-drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-03-28 14:21:53.728465 RunRunner-0.1.2/runrunner/
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      658 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/__init__.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)     1714 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/base.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)    14546 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/local.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      786 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/logger.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)    23756 2024-03-28 14:12:55.000000 RunRunner-0.1.2/runrunner/slurm.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)     1595 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/timing.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      907 2024-03-26 15:34:58.000000 RunRunner-0.1.2/runrunner/utils.py
--rw-r--r--   0 thijssnelleman   (501) staff       (20)       38 2024-03-28 14:21:53.728855 RunRunner-0.1.2/setup.cfg
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      704 2024-03-28 14:21:26.000000 RunRunner-0.1.2/setup.py
-drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-03-28 14:21:53.728573 RunRunner-0.1.2/test/
--rw-r--r--   0 thijssnelleman   (501) staff       (20)      831 2024-03-26 15:34:58.000000 RunRunner-0.1.2/test/test_timing.py
+drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-04-15 15:36:29.480762 RunRunner-0.1.3/
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)     1684 2024-04-15 15:36:29.480642 RunRunner-0.1.3/PKG-INFO
+drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-04-15 15:36:29.479386 RunRunner-0.1.3/RunRunner.egg-info/
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)     1684 2024-04-15 15:36:29.000000 RunRunner-0.1.3/RunRunner.egg-info/PKG-INFO
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      329 2024-04-15 15:36:29.000000 RunRunner-0.1.3/RunRunner.egg-info/SOURCES.txt
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)        1 2024-04-15 15:36:29.000000 RunRunner-0.1.3/RunRunner.egg-info/dependency_links.txt
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)       14 2024-04-15 15:36:29.000000 RunRunner-0.1.3/RunRunner.egg-info/requires.txt
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)       10 2024-04-15 15:36:29.000000 RunRunner-0.1.3/RunRunner.egg-info/top_level.txt
+drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-04-15 15:36:29.480368 RunRunner-0.1.3/runrunner/
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      658 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/__init__.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)     1714 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/base.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)    14546 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/local.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      786 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/logger.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)    24129 2024-04-15 15:32:20.000000 RunRunner-0.1.3/runrunner/slurm.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)     1595 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/timing.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      907 2024-03-26 15:34:58.000000 RunRunner-0.1.3/runrunner/utils.py
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)       38 2024-04-15 15:36:29.480802 RunRunner-0.1.3/setup.cfg
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      704 2024-04-15 15:36:07.000000 RunRunner-0.1.3/setup.py
+drwxr-xr-x   0 thijssnelleman   (501) staff       (20)        0 2024-04-15 15:36:29.480483 RunRunner-0.1.3/test/
+-rw-r--r--   0 thijssnelleman   (501) staff       (20)      831 2024-03-26 15:34:58.000000 RunRunner-0.1.3/test/test_timing.py
```

### Comparing `RunRunner-0.1.2/PKG-INFO` & `RunRunner-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunRunner
-Version: 0.1.2
+Version: 0.1.3
 Summary: RunRunner is a wrapper library for creating and managing subprocesses and their status, mainly focussed on using Slurm but (in absence) can also work with local jobs.
 Home-page: https://github.com/thijssnelleman/RunRunner
 Author: Thijs Snelleman
 Author-email: fkt_sparkle@aim.rwth-aachen.de
 Description-Content-Type: text/markdown
 
 # RunRunner - A Python handler for managing (Slurm)Jobs
```

### Comparing `RunRunner-0.1.2/RunRunner.egg-info/PKG-INFO` & `RunRunner-0.1.3/RunRunner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RunRunner
-Version: 0.1.2
+Version: 0.1.3
 Summary: RunRunner is a wrapper library for creating and managing subprocesses and their status, mainly focussed on using Slurm but (in absence) can also work with local jobs.
 Home-page: https://github.com/thijssnelleman/RunRunner
 Author: Thijs Snelleman
 Author-email: fkt_sparkle@aim.rwth-aachen.de
 Description-Content-Type: text/markdown
 
 # RunRunner - A Python handler for managing (Slurm)Jobs
```

### Comparing `RunRunner-0.1.2/runrunner/__init__.py` & `RunRunner-0.1.3/runrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/runrunner/base.py` & `RunRunner-0.1.3/runrunner/base.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/runrunner/local.py` & `RunRunner-0.1.3/runrunner/local.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/runrunner/logger.py` & `RunRunner-0.1.3/runrunner/logger.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/runrunner/slurm.py` & `RunRunner-0.1.3/runrunner/slurm.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,19 @@
 
     cmd: str
     working_dir: Path = Field(default_factory=Path)
     output_file: Path = None
     stdout_file: Path = None
     stderr_file: Path = None
     slurm_job_id: str = None
-    _slurm_job_details_dict: dict = {}
+    _slurm_job_details: dict = pydantic.PrivateAttr()
+
+    def __init__(self,**data: list) -> None:
+        super().__init__(**data)
+        self._slurm_job_details = {}
 
     @property
     def start_time(self) -> datetime | None:
         '''Return the start time of the job. If not started yet return None.'''
         datetime_string = self.job_log.get(_START_TIME_)
         if datetime_string is None:
             return None
@@ -212,37 +216,37 @@
             return None
         else:
             return parse_datetime(datetime_string)
 
     @property
     def slurm_job_details(self) -> dict[str, str]:
         '''Retrieve the latest job details from Slurm.'''
-        if 'JobState' in self._slurm_job_details_dict:
+        if 'JobState' in self._slurm_job_details:
             # We can only re-request information on waiting jobs
             current_state = Status.from_slurm_string(
-                self._slurm_job_details_dict['JobState'])
+                self._slurm_job_details['JobState'])
             if current_state not in [Status.RUNNING, Status.WAITING]:
-                return self._slurm_job_details_dict
+                return self._slurm_job_details
 
         scontrol = simple_run(f'scontrol show job {self.slurm_job_id}')
 
         if scontrol.returncode != os.EX_OK:
             # Scontrol was not (any longer) able to provide information about the job:
             # Therefore, we must deduct what we can
             if self.stderr_file.exists() and os.stat(self.stderr_file).st_size > 0:
-                self._slurm_job_details_dict['JobState'] = 'FAILED'
+                self._slurm_job_details['JobState'] = 'FAILED'
             elif self.stdout_file.exists() and os.stat(self.stdout_file).st_size > 0:
-                self._slurm_job_details_dict['JobState'] = 'COMPLETED'
-            return self._slurm_job_details_dict
+                self._slurm_job_details['JobState'] = 'COMPLETED'
+            return self._slurm_job_details
 
         data = re.findall(_regex_slurm_scontrol_show_job, scontrol.stdout)
         for entry in data:
             key, value = entry.split('=', 1)
-            self._slurm_job_details_dict[key] = value
-        return self._slurm_job_details_dict
+            self._slurm_job_details[key] = value
+        return self._slurm_job_details
 
     @property
     def status(self) -> Status:
         '''Return the Status of the job.'''
         job_details = self.slurm_job_details
         if 'JobState' not in job_details:
             return Status.NOTSET
@@ -393,16 +397,16 @@
                 # Find the highest number
                 names = [f.stem for f in self.base_dir.glob(f'{base_name}*.sh')]
                 match = _regex_slurmrun_name_.findall('\n'.join(names))
                 value = max([int(m[1]) for m in match]) if match else 0
 
                 new_name = f'{base_name}-{value+1:0{number_of_digits}}'
 
-                Log.warn('Script file with the same name detected.')
-                Log.warn(f'Using a new unique name: {self.name} -> {new_name}')
+                Log.warn('Script file with the same name detected. '
+                         f'Using a new unique name: {self.name} -> {new_name}')
                 self.name = new_name
             # Save json (not perfect, but somewhat reserve the name)
             self.to_file()
 
     def add_job(self, cmd: str, working_dir: Path = None, output: Path = None) -> None:
         '''Add a job to the list of jobs. The name is created automatically.'''
         self.jobs.append(SlurmJob(
@@ -453,19 +457,26 @@
 
     @property
     def json_filepath(self) -> Path:
         '''Path to the json file containing the description of the run.'''
         return self.filepath('.json')
 
     @classmethod
-    def from_file(cls, file: Path) -> SlurmRun:
-        '''Load a SlurmRun from a json file.'''
+    def from_file(cls, file: Path, load_dependencies: bool = False) -> SlurmRun:
+        '''Load a SlurmRun from a json file.
+
+        Args:
+            file: Path to the JSON file to load the object from
+            load_dependencies: If True, the dependecies in the file will also be loaded.
+        '''
         with open(file, 'r') as f:
             data = json.load(f)
         data['loaded_from_file'] = True
+        if not load_dependencies:
+            data["dependencies"] = []
         return cls.parse_obj(data)
 
     def to_file(self, verbose=True) -> Path:
         '''Save the run description to a json file. Return a path to the file.'''
         if verbose:
             Log.info(f'Saving run description to file {self.json_filepath}')
         with open(self.json_filepath, 'w') as f:
```

### Comparing `RunRunner-0.1.2/runrunner/timing.py` & `RunRunner-0.1.3/runrunner/timing.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/runrunner/utils.py` & `RunRunner-0.1.3/runrunner/utils.py`

 * *Files identical despite different names*

### Comparing `RunRunner-0.1.2/setup.py` & `RunRunner-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Setup for RunRunner.'''
 from setuptools import setup, find_packages
 import os
 
 setup(
     name='RunRunner',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/thijssnelleman/RunRunner',
     author='Thijs Snelleman',
     author_email='fkt_sparkle@aim.rwth-aachen.de',
     description='RunRunner is a wrapper library for creating and managing subprocesses and their status, mainly focussed on using Slurm but (in absence) can also work with local jobs.',
     long_description=open("README.MD", 'r').read() if os.path.exists("README.MD") else '',
     long_description_content_type="text/markdown",
     packages=find_packages(include=['runrunner']),
```

### Comparing `RunRunner-0.1.2/test/test_timing.py` & `RunRunner-0.1.3/test/test_timing.py`

 * *Files identical despite different names*

