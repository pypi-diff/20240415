# Comparing `tmp/perun-0.6.1.tar.gz` & `tmp/perun-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun-0.6.1.tar", max compression
+gzip compressed data, was "perun-0.6.2.tar", max compression
```

## Comparing `perun-0.6.1.tar` & `perun-0.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1527 2024-03-19 15:07:48.984675 perun-0.6.1/LICENSE
--rw-r--r--   0        0        0     8502 2024-03-19 15:07:48.984675 perun-0.6.1/README.md
--rw-r--r--   0        0        0      255 2024-03-19 15:07:48.984675 perun-0.6.1/perun/__init__.py
--rw-r--r--   0        0        0       93 2024-03-19 15:07:48.984675 perun-0.6.1/perun/__main__.py
--rw-r--r--   0        0        0       18 2024-03-19 15:07:48.984675 perun-0.6.1/perun/api/__init__.py
--rw-r--r--   0        0        0     8687 2024-03-19 15:07:48.984675 perun-0.6.1/perun/api/cli.py
--rw-r--r--   0        0        0     2494 2024-03-19 15:07:48.984675 perun-0.6.1/perun/api/decorator.py
--rw-r--r--   0        0        0       22 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/__init__.py
--rw-r--r--   0        0        0     1319 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/backend.py
--rw-r--r--   0        0        0     5303 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/nvml.py
--rw-r--r--   0        0        0     7867 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/powercap_rapl.py
--rw-r--r--   0        0        0     4639 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/psutil.py
--rw-r--r--   0        0        0     3697 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/rocmsmi.py
--rw-r--r--   0        0        0     1743 2024-03-19 15:07:48.984675 perun-0.6.1/perun/backend/util.py
--rw-r--r--   0        0        0     7095 2024-03-19 15:07:48.984675 perun-0.6.1/perun/comm.py
--rw-r--r--   0        0        0     2482 2024-03-19 15:07:48.984675 perun-0.6.1/perun/configuration.py
--rw-r--r--   0        0        0     3097 2024-03-19 15:07:48.984675 perun-0.6.1/perun/coordination.py
--rw-r--r--   0        0        0    13405 2024-03-19 15:07:48.988674 perun-0.6.1/perun/core.py
--rw-r--r--   0        0        0       26 2024-03-19 15:07:48.988674 perun-0.6.1/perun/data_model/__init__.py
--rw-r--r--   0        0        0    13357 2024-03-19 15:07:48.988674 perun-0.6.1/perun/data_model/data.py
--rw-r--r--   0        0        0     2937 2024-03-19 15:07:48.988674 perun-0.6.1/perun/data_model/measurement_type.py
--rw-r--r--   0        0        0      989 2024-03-19 15:07:48.988674 perun-0.6.1/perun/data_model/sensor.py
--rw-r--r--   0        0        0       18 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/__init__.py
--rw-r--r--   0        0        0     5876 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/bench.py
--rw-r--r--   0        0        0     8878 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/hdf5.py
--rw-r--r--   0        0        0     5463 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/io.py
--rw-r--r--   0        0        0     1177 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/json.py
--rw-r--r--   0        0        0     2197 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/pandas.py
--rw-r--r--   0        0        0      631 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/pickle.py
--rw-r--r--   0        0        0     4360 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/text_report.py
--rw-r--r--   0        0        0     2311 2024-03-19 15:07:48.988674 perun-0.6.1/perun/io/util.py
--rw-r--r--   0        0        0      944 2024-03-19 15:07:48.988674 perun-0.6.1/perun/logging.py
--rw-r--r--   0        0        0       36 2024-03-19 15:07:48.988674 perun-0.6.1/perun/monitoring/__init__.py
--rw-r--r--   0        0        0     4232 2024-03-19 15:07:48.988674 perun-0.6.1/perun/monitoring/application.py
--rw-r--r--   0        0        0    13888 2024-03-19 15:07:48.988674 perun-0.6.1/perun/monitoring/monitor.py
--rw-r--r--   0        0        0     6386 2024-03-19 15:07:48.988674 perun-0.6.1/perun/monitoring/subprocess.py
--rw-r--r--   0        0        0    24915 2024-03-19 15:07:48.988674 perun-0.6.1/perun/processing.py
--rw-r--r--   0        0        0     5406 2024-03-19 15:07:48.988674 perun-0.6.1/perun/util.py
--rw-r--r--   0        0        0     2139 2024-03-19 15:07:48.988674 perun-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     9598 1970-01-01 00:00:00.000000 perun-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1527 2024-04-15 13:33:04.003538 perun-0.6.2/LICENSE
+-rw-r--r--   0        0        0     8502 2024-04-15 13:33:04.003538 perun-0.6.2/README.md
+-rw-r--r--   0        0        0      255 2024-04-15 13:33:04.003538 perun-0.6.2/perun/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-15 13:33:04.003538 perun-0.6.2/perun/__main__.py
+-rw-r--r--   0        0        0       18 2024-04-15 13:33:04.003538 perun-0.6.2/perun/api/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-15 13:33:04.003538 perun-0.6.2/perun/api/cli.py
+-rw-r--r--   0        0        0     2494 2024-04-15 13:33:04.003538 perun-0.6.2/perun/api/decorator.py
+-rw-r--r--   0        0        0       22 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/__init__.py
+-rw-r--r--   0        0        0     1319 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/backend.py
+-rw-r--r--   0        0        0     5303 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/nvml.py
+-rw-r--r--   0        0        0     7867 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/powercap_rapl.py
+-rw-r--r--   0        0        0     4639 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/psutil.py
+-rw-r--r--   0        0        0     3697 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/rocmsmi.py
+-rw-r--r--   0        0        0     1743 2024-04-15 13:33:04.003538 perun-0.6.2/perun/backend/util.py
+-rw-r--r--   0        0        0     7095 2024-04-15 13:33:04.003538 perun-0.6.2/perun/comm.py
+-rw-r--r--   0        0        0     2482 2024-04-15 13:33:04.003538 perun-0.6.2/perun/configuration.py
+-rw-r--r--   0        0        0     3097 2024-04-15 13:33:04.003538 perun-0.6.2/perun/coordination.py
+-rw-r--r--   0        0        0    13405 2024-04-15 13:33:04.003538 perun-0.6.2/perun/core.py
+-rw-r--r--   0        0        0       26 2024-04-15 13:33:04.003538 perun-0.6.2/perun/data_model/__init__.py
+-rw-r--r--   0        0        0    13657 2024-04-15 13:33:04.003538 perun-0.6.2/perun/data_model/data.py
+-rw-r--r--   0        0        0     2937 2024-04-15 13:33:04.003538 perun-0.6.2/perun/data_model/measurement_type.py
+-rw-r--r--   0        0        0      989 2024-04-15 13:33:04.003538 perun-0.6.2/perun/data_model/sensor.py
+-rw-r--r--   0        0        0       18 2024-04-15 13:33:04.003538 perun-0.6.2/perun/io/__init__.py
+-rw-r--r--   0        0        0     5876 2024-04-15 13:33:04.003538 perun-0.6.2/perun/io/bench.py
+-rw-r--r--   0        0        0     8752 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/hdf5.py
+-rw-r--r--   0        0        0     5463 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/io.py
+-rw-r--r--   0        0        0     1177 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/json.py
+-rw-r--r--   0        0        0     2197 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/pandas.py
+-rw-r--r--   0        0        0      631 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/pickle.py
+-rw-r--r--   0        0        0     4360 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/text_report.py
+-rw-r--r--   0        0        0     2311 2024-04-15 13:33:04.007538 perun-0.6.2/perun/io/util.py
+-rw-r--r--   0        0        0      944 2024-04-15 13:33:04.007538 perun-0.6.2/perun/logging.py
+-rw-r--r--   0        0        0       36 2024-04-15 13:33:04.007538 perun-0.6.2/perun/monitoring/__init__.py
+-rw-r--r--   0        0        0     4282 2024-04-15 13:33:04.007538 perun-0.6.2/perun/monitoring/application.py
+-rw-r--r--   0        0        0    13888 2024-04-15 13:33:04.007538 perun-0.6.2/perun/monitoring/monitor.py
+-rw-r--r--   0        0        0     6386 2024-04-15 13:33:04.007538 perun-0.6.2/perun/monitoring/subprocess.py
+-rw-r--r--   0        0        0    24922 2024-04-15 13:33:04.007538 perun-0.6.2/perun/processing.py
+-rw-r--r--   0        0        0     5406 2024-04-15 13:33:04.007538 perun-0.6.2/perun/util.py
+-rw-r--r--   0        0        0     2139 2024-04-15 13:33:04.007538 perun-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9598 1970-01-01 00:00:00.000000 perun-0.6.2/PKG-INFO
```

### Comparing `perun-0.6.1/LICENSE` & `perun-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/README.md` & `perun-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/api/cli.py` & `perun-0.6.2/perun/api/cli.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/api/decorator.py` & `perun-0.6.2/perun/api/decorator.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/backend.py` & `perun-0.6.2/perun/backend/backend.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/nvml.py` & `perun-0.6.2/perun/backend/nvml.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/powercap_rapl.py` & `perun-0.6.2/perun/backend/powercap_rapl.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/psutil.py` & `perun-0.6.2/perun/backend/psutil.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/rocmsmi.py` & `perun-0.6.2/perun/backend/rocmsmi.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/backend/util.py` & `perun-0.6.2/perun/backend/util.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/comm.py` & `perun-0.6.2/perun/comm.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/configuration.py` & `perun-0.6.2/perun/configuration.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/coordination.py` & `perun-0.6.2/perun/coordination.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/core.py` & `perun-0.6.2/perun/core.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/data_model/data.py` & `perun-0.6.2/perun/data_model/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,24 +220,37 @@
             Region to mark the event from.
         """
         if region_name not in self._regions:
             self._regions[region_name] = []
 
         self._regions[region_name].append(time.time_ns())
 
+    def isEmpty(self) -> bool:
+        """Check if there are any regions marked.
+
+        Returns
+        -------
+        bool
+            True if there are no regions marked.
+        """
+        return len(self._regions.keys()) == 0
+
+    def __str__(self) -> str:
+        """Return string representation of LocalRegions object."""
+        return str(self._regions)
+
 
 @dataclasses.dataclass
 class Region:
     """Stores region data from all MPI ranks.
 
     For each marked region (decorated function), an numpy array with timestamps indicating function starts and ends.
     """
 
     id: str = ""
-    world_size: int = 0
     raw_data: Dict[int, np.ndarray] = dataclasses.field(default_factory=dict)
     runs_per_rank: Optional[Stats] = None
     runtime: Optional[Stats] = None
     power: Optional[Stats] = None
     cpu_util: Optional[Stats] = None
     gpu_util: Optional[Stats] = None
     processed: bool = False
@@ -246,17 +259,16 @@
         """Convert regions to a python dictionary.
 
         Returns
         -------
         Dict[str, Dict[int, np.ndarray]]
             Dictionary with region data.
         """
-        result = {
+        result: Dict[str, Any] = {
             "id": self.id,
-            "world_size": self.world_size,
             "raw_data": self.raw_data,
         }
 
         result["runs_per_rank"] = (
             asdict(self.runs_per_rank) if self.runs_per_rank else None
         )
         result["runtime"] = asdict(self.runtime) if self.runtime else None
@@ -278,15 +290,14 @@
         Returns
         -------
         Regions
             Regions object.
         """
         regionObj = Region()
         regionObj.id = regionDictionary["id"]
-        regionObj.world_size = regionDictionary["world_size"]
         regionObj.raw_data = regionDictionary["raw_data"]
         regionObj.processed = regionDictionary["processed"]
         if regionObj.processed:
             regionObj.runs_per_rank = Stats.fromDict(regionDictionary["runs_per_rank"])
             regionObj.runtime = Stats.fromDict(regionDictionary["runtime"])
             regionObj.power = Stats.fromDict(regionDictionary["power"])
             regionObj.cpu_util = Stats.fromDict(regionDictionary["cpu_util"])
@@ -349,28 +360,28 @@
         ----------
         localRegions : List[LocalRegions]
             Gathered local regions from all MPI ranks
         start_time : int
             'Official' start time of the run.
         """
         self.regions = {}
-        world_size = len(localRegions)
+        log.debug(f"Local regions: {localRegions}")
         for rank, l_region in enumerate(localRegions):
-            for region_name, data in l_region._regions.items():
-                if region_name not in self.regions:
-                    r = Region()
-                    r.id = region_name
-                    r.world_size = world_size
-                    self.regions[region_name] = r
-
-                t_s = np.array(data)
-                t_s -= start_time
-                t_s = t_s.astype("float32")
-                t_s *= 1e-9
-                self.regions[region_name].raw_data[rank] = t_s
+            if not l_region.isEmpty():
+                for region_name, data in l_region._regions.items():
+                    if region_name not in self.regions:
+                        r = Region()
+                        r.id = region_name
+                        self.regions[region_name] = r
+
+                    t_s = np.array(data)
+                    t_s -= start_time
+                    t_s = t_s.astype("float32")
+                    t_s *= 1e-9
+                    self.regions[region_name].raw_data[rank] = t_s
 
     def toDict(self, include_raw_data: bool = True) -> Dict:
         """Transform object to dictionary."""
         resultsDict = {
             "id": self.id,
             "type": self.type.value,
             "metadata": self.metadata,
```

### Comparing `perun-0.6.1/perun/data_model/measurement_type.py` & `perun-0.6.2/perun/data_model/measurement_type.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/data_model/sensor.py` & `perun-0.6.2/perun/data_model/sensor.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/bench.py` & `perun-0.6.2/perun/io/bench.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/hdf5.py` & `perun-0.6.2/perun/io/hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,14 @@
     _addMetric(region_group, region.cpu_util)  # type: ignore
     _addMetric(region_group, region.gpu_util)  # type: ignore
     _addMetric(region_group, region.power)  # type: ignore
     _addMetric(region_group, region.runs_per_rank)  # type: ignore
     _addMetric(region_group, region.runtime)  # type: ignore
     region_group.attrs["id"] = region.id
     region_group.attrs["processed"] = region.processed
-    region_group.attrs["world_size"] = region.world_size
     raw_data_group = region_group.create_group("raw_data")
     for rank, data in region.raw_data.items():
         raw_data_group.create_dataset(str(rank), data=data)
 
 
 def _readRegions(group: h5py.Group) -> Dict[str, Region]:
     regionsDict: Dict[str, Region] = {}
@@ -250,15 +249,14 @@
     return regionsDict
 
 
 def _readRegion(group: h5py.Group) -> Region:
     regionObj = Region()
     regionObj.id = group.attrs["id"]  # type: ignore
     regionObj.processed = group.attrs["processed"]  # type: ignore
-    regionObj.world_size = group.attrs["world_size"]  # type: ignore
 
     regionObj.cpu_util = _readMetric(group["CPU_UTIL"])  # type: ignore
     regionObj.gpu_util = _readMetric(group["GPU_UTIL"])  # type: ignore
     regionObj.power = _readMetric(group["POWER"])  # type: ignore
     regionObj.runtime = _readMetric(group["RUNTIME"])  # type: ignore
     regionObj.runs_per_rank = _readMetric(group["N_RUNS"])  # type: ignore
```

### Comparing `perun-0.6.1/perun/io/io.py` & `perun-0.6.2/perun/io/io.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/json.py` & `perun-0.6.2/perun/io/json.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/pandas.py` & `perun-0.6.2/perun/io/pandas.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/pickle.py` & `perun-0.6.2/perun/io/pickle.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/text_report.py` & `perun-0.6.2/perun/io/text_report.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/io/util.py` & `perun-0.6.2/perun/io/util.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/logging.py` & `perun-0.6.2/perun/logging.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/monitoring/application.py` & `perun-0.6.2/perun/monitoring/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Application module."""
 
 import gc
+import logging
+import logging.handlers
 import os
 import subprocess
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Callable, Dict, Union
 
-from perun import log
+log = logging.getLogger("perun")
 
 
 class Application:
     """
     Represents an application to be executed.
 
     Parameters
```

### Comparing `perun-0.6.1/perun/monitoring/monitor.py` & `perun-0.6.2/perun/monitoring/monitor.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/monitoring/subprocess.py` & `perun-0.6.2/perun/monitoring/subprocess.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/perun/processing.py` & `perun-0.6.2/perun/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -448,20 +448,20 @@
     Parameters
     ----------
     regions : List[Region]
         List of regions that use the same data node.
     dataNode : DataNode
         Data node with sensor data.
     """
-    world_size = regions[0].world_size
+    log.debug(f"Processing regions with sensor data: {len(regions)}")
     power = [
-        [
-            [0.0 for _ in range(region.raw_data[rank].shape[0] // 2)]
-            for rank in range(world_size)
-        ]
+        {
+            rank: [0.0 for _ in range(region.raw_data[rank].shape[0] // 2)]
+            for rank in region.raw_data.keys()
+        }
         for region in regions
     ]
     cpu_util = copy.deepcopy(power)
 
     gpu_util = copy.deepcopy(power)
     gpu_count = copy.deepcopy(power)
 
@@ -506,15 +506,15 @@
                                             _, values = getInterpolatedValues(
                                                 raw_data.timesteps.astype("float32"),
                                                 raw_data.values,
                                                 events[i * 2],
                                                 events[i * 2 + 1],
                                             )
                                             cpu_util[region_idx][rank][i] += np.mean(
-                                                values
+                                                values, dtype="float32"
                                             )
                                         elif (
                                             measuring_unit == Unit.BYTE
                                             and deviceNode.deviceType == DeviceType.GPU
                                         ):
                                             has_gpu = True
                                             _, values = getInterpolatedValues(
@@ -527,19 +527,19 @@
                                                 np.mean(values)
                                                 * 100
                                                 / raw_data.v_md.max
                                             ).astype("float32")
                                             gpu_count[region_idx][rank][i] += 1
 
     for region_idx, region in enumerate(regions):
-        r_power = np.array(list(chain(*power[region_idx])))
-        r_cpu_util = np.array(list(chain(*cpu_util[region_idx])))
+        r_power = np.array(list(chain(*power[region_idx].values())))
+        r_cpu_util = np.array(list(chain(*cpu_util[region_idx].values())))
 
-        r_gpu_util = np.array(list(chain(*gpu_util[region_idx])))
-        r_gpu_count = np.array(list(chain(*gpu_count[region_idx])))
+        r_gpu_util = np.array(list(chain(*gpu_util[region_idx].values())))
+        r_gpu_count = np.array(list(chain(*gpu_count[region_idx].values())))
 
         if has_gpu:
             r_gpu_util /= r_gpu_count
 
         region.cpu_util = Stats(
             MetricType.CPU_UTIL,
             MetricMetaData(
@@ -597,22 +597,19 @@
     ----------
     region : Region
         Region object
     """
     runs_per_rank = []
     runtime = []
 
-    for rank in range(region.world_size):
-        if rank in region.raw_data:
-            events = region.raw_data[rank]
-            runs_per_rank.append(events.shape[0] / 2)
-            for i in range(1, events.shape[0], 2):
-                runtime.append(events[i] - events[i - 1])
-        else:
-            runs_per_rank.append(0)
+    for rank in region.raw_data.keys():
+        events = region.raw_data[rank]
+        runs_per_rank.append(events.shape[0] / 2)
+        for i in range(1, events.shape[0], 2):
+            runtime.append(events[i] - events[i - 1])
 
     runs_array = np.array(runs_per_rank)
     runtime_array = np.array(runtime)
 
     region.runs_per_rank = Stats(
         MetricType.N_RUNS,
         MetricMetaData(
@@ -666,9 +663,9 @@
 
     Returns
     -------
     np.ndarray
         ROI values
     """
     new_t = np.concatenate([[start], t[np.all([t >= start, t <= end], axis=0)], [end]])
-    new_x = np.interp(new_t, t, x)
+    new_x = np.interp(new_t, t, x)  # type: ignore
     return new_t, new_x
```

### Comparing `perun-0.6.1/perun/util.py` & `perun-0.6.2/perun/util.py`

 * *Files identical despite different names*

### Comparing `perun-0.6.1/pyproject.toml` & `perun-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perun"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Gutiérrez Hermosillo Muriedas, Juan Pedro <juanpedroghm@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Helmholtz-AI-Energy/perun"
 
 [tool.poetry.scripts]
```

### Comparing `perun-0.6.1/PKG-INFO` & `perun-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Home-page: https://github.com/Helmholtz-AI-Energy/perun
 License: BSD-3-Clause
 Author: Gutiérrez Hermosillo Muriedas, Juan Pedro
 Author-email: juanpedroghm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

