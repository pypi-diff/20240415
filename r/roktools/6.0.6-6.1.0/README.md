# Comparing `tmp/roktools-6.0.6.tar.gz` & `tmp/roktools-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.0.6.tar", max compression
+gzip compressed data, was "roktools-6.1.0.tar", max compression
```

## Comparing `roktools-6.0.6.tar` & `roktools-6.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-14 17:01:04.977159 roktools-6.0.6/LICENSE
--rw-r--r--   0        0        0     1665 2024-04-14 17:01:04.977159 roktools-6.0.6/README.md
--rw-r--r--   0        0        0     1162 2024-04-14 17:01:04.977159 roktools-6.0.6/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/decorator.py
--rw-r--r--   0        0        0      927 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/file.py
--rw-r--r--   0        0        0    33628 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-04-14 17:01:05.057158 roktools-6.0.6/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1878 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9505 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-04-14 17:01:05.057158 roktools-6.0.6/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1746 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5905 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-04-14 17:01:05.057158 roktools-6.0.6/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    29654 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/rinex.py
--rwxr-xr-x   0        0        0     1083 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/tensorial.py
--rw-r--r--   0        0        0    11178 2024-04-14 17:01:04.977159 roktools-6.0.6/roktools/time.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-15 13:58:20.577908 roktools-6.1.0/LICENSE
+-rw-r--r--   0        0        0     1665 2024-04-15 13:58:20.577908 roktools-6.1.0/README.md
+-rw-r--r--   0        0        0     1162 2024-04-15 13:58:20.581908 roktools-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/decorator.py
+-rw-r--r--   0        0        0      933 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/file.py
+-rw-r--r--   0        0        0    33628 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:58:20.629907 roktools-6.1.0/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1884 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9505 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:58:20.633907 roktools-6.1.0/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1745 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5905 2024-04-15 13:58:20.581908 roktools-6.1.0/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:58:20.633907 roktools-6.1.0/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-04-15 13:58:20.585908 roktools-6.1.0/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    31190 2024-04-15 13:58:20.585908 roktools-6.1.0/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1084 2024-04-15 13:58:20.585908 roktools-6.1.0/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-04-15 13:58:20.585908 roktools-6.1.0/roktools/tensorial.py
+-rw-r--r--   0        0        0    11178 2024-04-15 13:58:20.585908 roktools-6.1.0/roktools/time.py
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 roktools-6.1.0/PKG-INFO
```

### Comparing `roktools-6.0.6/LICENSE` & `roktools-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/README.md` & `roktools-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/pyproject.toml` & `roktools-6.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.0.6"
+version = "6.1.0"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.0.6/roktools/cl.py` & `roktools-6.1.0/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/file.py` & `roktools-6.1.0/roktools/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from functools import wraps
 from typing import IO
 
+
 def process_filename_or_file_handler(mode):
     def decorator(func):
         @wraps(func)
         def wrapper(input, *args, **kwargs):
             if isinstance(input, str):
                 with open(input, mode) as fh:
                     return func(fh, *args, **kwargs)
             else:
                 return func(input, *args, **kwargs)
         return wrapper
     return decorator
 
+
 def grep_lines(filename: str, pattern_string: str):
     """
     Generator function used to grep lines from a file. Can be used in methods
     such as numpy.genfromtxt, ...
 
     >>> generator = grep_lines(filename, "pattern")
     >>> data = numpy.loadtxt(generator)
     """
 
     with open(filename, 'r') as fh:
         for line in fh:
             if pattern_string in line:
                 yield line
 
-def skip_lines(fh:IO, n_lines:int):
+
+def skip_lines(fh: IO, n_lines: int):
 
     for _ in range(n_lines):
-        fh.readline()
+        fh.readline()
```

### Comparing `roktools-6.0.6/roktools/geodetic.py` & `roktools-6.1.0/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/gnss/edit.py` & `roktools-6.1.0/roktools/gnss/edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 
 ARC_ID_FIELD = 'arc_id'
 
+
 def compute_phase_arc_id(data: pd.DataFrame) -> pd.DataFrame:
     """
     Computes the phase arc ID, that can be used later to perform operations
     on a per-arc basis (compute arc bias, ...)
     """
 
     data[ARC_ID_FIELD] = data.groupby('signal')['slip'].transform('cumsum')
@@ -31,33 +32,35 @@
 
     data['slip'] = np.any([data['slip'], marked_epochs], axis=0)
 
     data = compute_phase_arc_id(data)
 
     return data
 
-def detrend(data:pd.DataFrame, observable: str, n_samples:int) -> pd.DataFrame:
+
+def detrend(data: pd.DataFrame, observable: str, n_samples: int) -> pd.DataFrame:
     """
     Detrend a given observable by using a rolling window of a certain number of
     samples
     """
 
     trend_column = f'{observable}_trend'
     detrended_column = f'{observable}_detrended'
 
     trend = data.groupby(['signal', ARC_ID_FIELD])[observable].transform(lambda x: x.rolling(n_samples).mean())
     data[trend_column] = trend
     data[detrended_column] = data[observable] - data[trend_column]
 
     return data
 
+
 def remove_mean(data: pd.DataFrame, observable: str) -> pd.DataFrame:
 
     bias_field = f'{observable}_bias'
     aligned_field = f'{observable}_aligned'
 
     # For each arch id, compute the median
-    data[bias_field] = data.groupby(['signal',ARC_ID_FIELD])[observable].transform('mean')
+    data[bias_field] = data.groupby(['signal', ARC_ID_FIELD])[observable].transform('mean')
 
     data[aligned_field] = data[observable] - data[bias_field]
 
     return data
```

### Comparing `roktools-6.0.6/roktools/gnss/observables.py` & `roktools-6.1.0/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/gnss/residuals.py` & `roktools-6.1.0/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/gnss/types.py` & `roktools-6.1.0/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/logger.py` & `roktools-6.1.0/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/orbit/kepler.py` & `roktools-6.1.0/roktools/orbit/kepler.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,7 @@
     >>> mean_motion_rev_per_day = 15.5918272
     >>> mean_motion_rad_per_s = mean_motion_rev_per_day * math.tau / 86400.0
     >>> compute_semi_major_axis(mean_motion_rad_per_s)
     6768158.4970976645
     """
 
     return math.pow(EARTH_GRAVITATION_PARAM_MU/math.pow(mean_motion_rad_per_s, 2.0), 1.0 / 3.0)
-
```

### Comparing `roktools-6.0.6/roktools/orbit/tle.py` & `roktools-6.1.0/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/parsers/rtklib/stats.py` & `roktools-6.1.0/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/rinex.py` & `roktools-6.1.0/roktools/rinex.py`

 * *Files 3% similar despite different names*

```diff
@@ -597,14 +597,33 @@
             return self.epoch < other.epoch
 
         elif self.satellite.constellation != other.satellite.constellation:
             return self.satellite.constellation < other.satellite.constellation
 
         return self.satellite.prn < other.satellite.prn
 
+    def to_rinex2(self) -> str:
+
+        out = ""
+
+        id = self.satellite.prn
+        if id > 99:
+            raise ValueError('Cannot write a Rinex 2 nav block for satellite with id > 99')
+
+        epoch_line = f'{id:2d}'
+        clock_str = self.lines[1][23:]
+        out = out + f'{epoch_line} {self.epoch.strftime("%y %m %d %H %M %S.0")}{clock_str}\n'
+        for brdc_line in self.lines[2:]:
+            out = out + f'{brdc_line[1:]}\n'
+        # print extra lines
+        out = out + '    0.000000000000e+00 0.000000000000e+00 0.000000000000e+00 0.000000000000e+00\n'
+        out = out + f'{self.lines[4][1:23]} 0.000000000000e+00\n'
+
+        return out
+
 
 class Nav(object):
     """
     Class that holds Rinex Navigation data
     """
 
     RINEX4_EPH_BLOCK_LINES_LEO = 6
@@ -622,14 +641,15 @@
         f'{ConstellationId.BEIDOU.value} D1': 8,
         f'{ConstellationId.BEIDOU.value} D2': 8,
         f'{ConstellationId.BEIDOU.value} CNV1': 10,
         f'{ConstellationId.BEIDOU.value} CNV2': 10,
         f'{ConstellationId.BEIDOU.value} CNV3': 9,
         f'{ConstellationId.SBAS.value} SBAS': 4,
         f'{ConstellationId.IRNSS.value} LNAV': 8,
+        f'{ConstellationId.LEO.value}': RINEX4_EPH_BLOCK_LINES_LEO,
         f'{ConstellationId.SPIRE.value}': RINEX4_EPH_BLOCK_LINES_LEO,
         f'{ConstellationId.STARLINK.value}': RINEX4_EPH_BLOCK_LINES_LEO,
         f'{ConstellationId.ONEWEB.value}': RINEX4_EPH_BLOCK_LINES_LEO,
     }
 
     def __init__(self, file: Union[str, IO]):
         self.blocks = Nav._load(file)
@@ -803,36 +823,36 @@
         delta_n_dot = orbit.delta_n_dot_rad_per_s
         lines.append(Nav._write_orbit_line(idot, delta_n_dot, weektow.week, void))
 
         return RawNavBlock(satellite, orbit.toe, lines)
 
     @staticmethod
     @process_filename_or_file_handler('w')
-    def write_from_tle(output, tle_list: List[TLE]) -> None:
+    def write_from_tle(output, tle_list: List[TLE], rinex2=False) -> None:
 
         output.write(Nav.create_header(pgm='rinex_from_file'))
 
         for tle in tle_list:
 
             # Find the clock if available
             sat_clock = Clock(0, 0, 0)
             try:
                 satellite = tle.get_satellite()
                 orbit = tle.to_kepler()
                 nav_block = Nav.create_navblock(satellite, orbit, sat_clock)
 
-                output.write(str(nav_block))
+                output.write(nav_block.to_rinex2() if rinex2 else str(nav_block))
                 output.write('\n')
             except ValueError as e:
                 logger.warning(e)
                 continue
 
     @staticmethod
     @process_filename_or_file_handler('w')
-    def write_from_dataframe(output, df: pd.DataFrame) -> None:
+    def write_from_dataframe(output, df: pd.DataFrame, rinex2=False) -> None:
 
         output.write(Nav.create_header(pgm='rinex_from_file'))
 
         df = df.sort_values(by=['epoch', 'sat'], ascending=[True, True])
 
         for _, row in df.iterrows():
 
@@ -843,31 +863,46 @@
                 sat_clock = Clock(0, 0, 0)
                 orbit = Kepler(
                     row.epoch, row.a_m, row.eccentricity,
                     math.radians(row.inclination_deg), math.radians(row.raan_deg),
                     math.radians(row.arg_perigee_deg), math.radians(row.true_anomaly_deg))
                 nav_block = Nav.create_navblock(satellite, orbit, sat_clock)
 
-                output.write(str(nav_block))
+                output.write(nav_block.to_rinex2() if rinex2 else str(nav_block))
                 output.write('\n')
             except Exception as e:
                 logger.warning(e)
                 continue
 
+    def write(self, output_filename, rinex2=False) -> None:
+
+        with open(output_filename, 'w') as fh:
+
+            fh.write(Nav.create_header(pgm='rinex_from_file'))
+
+            for block in self.blocks:
+                try:
+                    fh.write(block.to_rinex2() if rinex2 else str(block))
+                    fh.write('\n')
+                except Exception as e:
+                    logger.warning(e)
+                    continue
+
     @staticmethod
     def _get_block_n_lines(line: str) -> int:
         """
         Give the number of lines of a navigation block for a given constellation
         """
 
         key = line[6]
         constellation = ConstellationId(key)
 
         if constellation is not ConstellationId.ONEWEB and \
            constellation is not ConstellationId.SPIRE and \
+           constellation is not ConstellationId.LEO and \
            constellation is not ConstellationId.STARLINK:
             key = key + " " + line[10:]
 
         return Nav.RINEX4_EPH_BLOCK_LINES[key]
 
     @staticmethod
     def _write_orbit_line(a: float, b: float, c: float, d: float) -> str:
@@ -886,15 +921,15 @@
 
     gmst_rad = gmst_h * math.tau / 24.0
     gmst_rad = gmst_rad % math.tau
 
     return gmst_rad
 
 
-def merge_nav(files:List[Union[str,IO]]) -> str:
+def merge_nav(files: List[Union[str, IO]]) -> str:
     """
     Merge RINEX navigation files
 
     :param files: list of RINEX Nav files to merge
 
     :return: the merged RINEX NAV file as a string
     """
@@ -936,17 +971,19 @@
 
     input_options.add_argument('--celestrak_file', metavar='<filename>', type=str,
                                help='File from Celestrak with the TLE elements to convert to RINEX. Based on https://arxiv.org/abs/2401.17767')
 
     input_options.add_argument('--csv', metavar='<filename>', type=str,
                                help='CSV file with the description of ')
 
+    parser.add_argument('--rinex2', action='store_true', help='Output the format in Rinex 2 GPS format. Will skip satellites with PRN larger than 99')
+
     # Parse the command-line arguments
     args = parser.parse_args()
 
     if args.celestrak_file:
         tle_list = read_celestrak(args.celestrak_file)
-        Nav.write_from_tle(sys.stdout, tle_list)
+        Nav.write_from_tle(sys.stdout, tle_list, rinex2=args.rinex2)
 
     elif args.csv:
         df = pd.read_csv(args.csv, parse_dates=['epoch'])
-        Nav.write_from_dataframe(sys.stdout, df)
+        Nav.write_from_dataframe(sys.stdout, df, rinex2=args.rinex2)
```

### Comparing `roktools-6.0.6/roktools/stats.py` & `roktools-6.1.0/roktools/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     pdf = np.array(pdf) * binwidth
     cdf = np.cumsum(pdf)
 
     for i in range(args.n_bins):
         print(f"{edges[i]} {pdf[i]} {cdf[i]}")
 
 
-def rms(values:Iterable) -> float:
+def rms(values: Iterable) -> float:
     """
     Compute the Root Mean Square of an array of values
 
     >>> array = [1, 2, 3, 4, 5]
     >>> rms(array)
     3.3166247903554
     """
```

### Comparing `roktools-6.0.6/roktools/tensorial.py` & `roktools-6.1.0/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/roktools/time.py` & `roktools-6.1.0/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.6/PKG-INFO` & `roktools-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.0.6
+Version: 6.1.0
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

