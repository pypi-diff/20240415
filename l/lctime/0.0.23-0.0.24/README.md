# Comparing `tmp/lctime-0.0.23.tar.gz` & `tmp/lctime-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctime-0.0.23.tar", last modified: Thu Apr  4 21:15:50 2024, max compression
+gzip compressed data, was "lctime-0.0.24.tar", last modified: Mon Apr 15 19:48:49 2024, max compression
```

## Comparing `lctime-0.0.23.tar` & `lctime-0.0.24.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.275904 lctime-0.0.23/
--rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-04 21:15:50.275904 lctime-0.0.23/PKG-INFO
--rw-r-----   0 user      (1000) user      (1000)     4983 2024-04-04 21:13:38.000000 lctime-0.0.23/README.md
--rw-r--r--   0 user      (1000) user      (1000)     1855 2024-04-04 21:14:50.000000 lctime-0.0.23/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-04 21:15:50.275904 lctime-0.0.23/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.255904 lctime-0.0.23/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.255904 lctime-0.0.23/src/lctime/
--rw-r--r--   0 user      (1000) user      (1000)      983 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     4077 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/cell_types.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.263904 lctime-0.0.23/src/lctime/characterization/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    11792 2024-04-03 14:36:44.000000 lctime-0.0.23/src/lctime/characterization/input_capacitance.py
--rw-r--r--   0 user      (1000) user      (1000)    64459 2024-02-22 10:39:09.000000 lctime-0.0.23/src/lctime/characterization/main_lctime.py
--rw-r-----   0 user      (1000) user      (1000)     7311 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/main_sp2bool.py
--rw-r-----   0 user      (1000) user      (1000)     4926 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/ngspice_simulation.py
--rw-r--r--   0 user      (1000) user      (1000)    24914 2024-04-03 14:36:44.000000 lctime-0.0.23/src/lctime/characterization/ngspice_subprocess.py
--rw-r-----   0 user      (1000) user      (1000)    14444 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/piece_wise_linear.py
--rw-r-----   0 user      (1000) user      (1000)     4810 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/test_ngspice_shared.py
--rw-r-----   0 user      (1000) user      (1000)     5414 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/test_ngspice_subprocess.py
--rw-r--r--   0 user      (1000) user      (1000)    15265 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/timing_combinatorial.py
--rw-r--r--   0 user      (1000) user      (1000)    61091 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/timing_sequential.py
--rw-r--r--   0 user      (1000) user      (1000)    16441 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.267904 lctime-0.0.23/src/lctime/lccommon/
--rw-r-----   0 user      (1000) user      (1000)      128 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     1955 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/data_types.py
--rw-r--r--   0 user      (1000) user      (1000)    10475 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/net_util.py
--rw-r-----   0 user      (1000) user      (1000)     5094 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/spice_parser.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.267904 lctime-0.0.23/src/lctime/liberty/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     4870 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/merge.py
--rw-r-----   0 user      (1000) user      (1000)     5853 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/util.py
--rw-r-----   0 user      (1000) user      (1000)     3919 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/visualize.py
--rw-r--r--   0 user      (1000) user      (1000)      472 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/licence.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.271904 lctime-0.0.23/src/lctime/logic/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     6513 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/cmos_sim.py
--rw-r-----   0 user      (1000) user      (1000)    10591 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/cmos_synth.py
--rw-r-----   0 user      (1000) user      (1000)    49051 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/functional_abstraction.py
--rw-r-----   0 user      (1000) user      (1000)     2365 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/graph_enumeration.py
--rw-r-----   0 user      (1000) user      (1000)    21778 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/seq_recognition.py
--rw-r-----   0 user      (1000) user      (1000)     1845 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/smt_4value_logic_scratch.py
--rw-r-----   0 user      (1000) user      (1000)     1690 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/types.py
--rw-r-----   0 user      (1000) user      (1000)     2657 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.271904 lctime-0.0.23/src/lctime/transistor_sizing/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/transistor_sizing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     9277 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/transistor_sizing/width_opt.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.275904 lctime-0.0.23/src/lctime.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1505 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      216 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      128 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.027940 lctime-0.0.24/
+-rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-15 19:48:49.027940 lctime-0.0.24/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     4983 2024-04-04 21:13:38.000000 lctime-0.0.24/README.md
+-rw-r--r--   0 user      (1000) user      (1000)     1855 2024-04-15 19:47:59.000000 lctime-0.0.24/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-15 19:48:49.027940 lctime-0.0.24/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.015940 lctime-0.0.24/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.015940 lctime-0.0.24/src/lctime/
+-rw-r--r--   0 user      (1000) user      (1000)      983 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     4044 2024-04-15 06:15:13.000000 lctime-0.0.24/src/lctime/cell_types.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.019940 lctime-0.0.24/src/lctime/characterization/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/characterization/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    18489 2024-04-09 15:09:28.000000 lctime-0.0.24/src/lctime/characterization/flipflop.py
+-rw-r--r--   0 user      (1000) user      (1000)    11924 2024-04-08 14:05:48.000000 lctime-0.0.24/src/lctime/characterization/input_capacitance.py
+-rw-r--r--   0 user      (1000) user      (1000)      664 2024-04-08 14:20:37.000000 lctime-0.0.24/src/lctime/characterization/leakage_power.py
+-rw-r--r--   0 user      (1000) user      (1000)    52246 2024-04-15 06:35:09.000000 lctime-0.0.24/src/lctime/characterization/main_lctime.py
+-rw-r-----   0 user      (1000) user      (1000)     7278 2024-04-15 06:14:54.000000 lctime-0.0.24/src/lctime/characterization/main_sp2bool.py
+-rw-r-----   0 user      (1000) user      (1000)     4926 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/characterization/ngspice_simulation.py
+-rw-r--r--   0 user      (1000) user      (1000)    24914 2024-04-03 14:36:44.000000 lctime-0.0.24/src/lctime/characterization/ngspice_subprocess.py
+-rw-r-----   0 user      (1000) user      (1000)    14444 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/characterization/piece_wise_linear.py
+-rw-r-----   0 user      (1000) user      (1000)     4843 2024-04-08 14:11:01.000000 lctime-0.0.24/src/lctime/characterization/test_ngspice_shared.py
+-rw-r-----   0 user      (1000) user      (1000)     5497 2024-04-08 14:10:21.000000 lctime-0.0.24/src/lctime/characterization/test_ngspice_subprocess.py
+-rw-r--r--   0 user      (1000) user      (1000)    15763 2024-04-08 14:12:52.000000 lctime-0.0.24/src/lctime/characterization/timing_combinatorial.py
+-rw-r--r--   0 user      (1000) user      (1000)    61091 2024-04-09 08:45:09.000000 lctime-0.0.24/src/lctime/characterization/timing_sequential.py
+-rw-r--r--   0 user      (1000) user      (1000)    16558 2024-04-07 21:18:13.000000 lctime-0.0.24/src/lctime/characterization/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.023940 lctime-0.0.24/src/lctime/lccommon/
+-rw-r-----   0 user      (1000) user      (1000)      128 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/lccommon/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     1955 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/lccommon/data_types.py
+-rw-r--r--   0 user      (1000) user      (1000)    10444 2024-04-15 06:16:06.000000 lctime-0.0.24/src/lctime/lccommon/net_util.py
+-rw-r-----   0 user      (1000) user      (1000)     5094 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/lccommon/spice_parser.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.023940 lctime-0.0.24/src/lctime/liberty/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/liberty/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     4870 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/liberty/merge.py
+-rw-r-----   0 user      (1000) user      (1000)     5853 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/liberty/util.py
+-rw-r-----   0 user      (1000) user      (1000)     3920 2024-04-15 06:30:14.000000 lctime-0.0.24/src/lctime/liberty/visualize.py
+-rw-r--r--   0 user      (1000) user      (1000)      436 2024-04-15 06:14:28.000000 lctime-0.0.24/src/lctime/licence.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.023940 lctime-0.0.24/src/lctime/logic/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     6515 2024-04-15 06:29:07.000000 lctime-0.0.24/src/lctime/logic/cmos_sim.py
+-rw-r-----   0 user      (1000) user      (1000)    10591 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/cmos_synth.py
+-rw-r-----   0 user      (1000) user      (1000)    49234 2024-04-15 06:26:52.000000 lctime-0.0.24/src/lctime/logic/functional_abstraction.py
+-rw-r-----   0 user      (1000) user      (1000)     2365 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/graph_enumeration.py
+-rw-r-----   0 user      (1000) user      (1000)    25679 2024-04-09 14:50:20.000000 lctime-0.0.24/src/lctime/logic/seq_recognition.py
+-rw-r-----   0 user      (1000) user      (1000)     1845 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/smt_4value_logic_scratch.py
+-rw-r-----   0 user      (1000) user      (1000)     1690 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/types.py
+-rw-r-----   0 user      (1000) user      (1000)     2657 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/logic/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.023940 lctime-0.0.24/src/lctime/transistor_sizing/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/transistor_sizing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     9277 2024-01-25 11:27:22.000000 lctime-0.0.24/src/lctime/transistor_sizing/width_opt.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-15 19:48:49.027940 lctime-0.0.24/src/lctime.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1590 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      216 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      128 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2024-04-15 19:48:49.000000 lctime-0.0.24/src/lctime.egg-info/top_level.txt
```

### Comparing `lctime-0.0.23/PKG-INFO` & `lctime-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctime
-Version: 0.0.23
+Version: 0.0.24
 Summary: CMOS standard-cell characterization kit.
 Author-email: "T. Kramer" <code@tkramer.ch>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://codeberg.org/librecell/lctime
 Project-URL: Repository, https://codeberg.org/librecell/lctime
 Project-URL: Issue Tracker, https://codeberg.org/librecell/lctime/issues
 Keywords: cmos,cell,characterization,vlsi,asic
```

### Comparing `lctime-0.0.23/README.md` & `lctime-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/pyproject.toml` & `lctime-0.0.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Thomas Kramer
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 [project]
 name = "lctime"
-version = "0.0.23"
+version = "0.0.24"
 description='CMOS standard-cell characterization kit.'
 readme = {file = "README.md", content-type="text/markdown"}
 license = {text = "AGPL-3.0-or-later"}
 
 requires-python = ">=3.7"
 
 keywords= ["cmos", "cell", "characterization", "vlsi", "asic"]
```

### Comparing `lctime-0.0.23/src/lctime/__init__.py` & `lctime-0.0.24/src/lctime/__init__.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/cell_types.py` & `lctime-0.0.24/src/lctime/cell_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Copyright (c) 2021 Thomas Kramer.
-# SPDX-FileCopyrightText: 2022 Thomas Kramer <code@tkramer.ch>
-#
+# SPDX-FileCopyrightText: 2021-2022 Thomas Kramer <code@tkramer.ch>
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 from typing import Dict, List, Set
 import sympy
 from sympy.logic import boolalg
 from .logic.types import CombinationalOutput
```

### Comparing `lctime-0.0.23/src/lctime/characterization/input_capacitance.py` & `lctime-0.0.24/src/lctime/characterization/input_capacitance.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,38 +12,40 @@
 from itertools import product
 
 from .util import *
 from .piece_wise_linear import *
 from .ngspice_subprocess import run_simulation
 from ..lccommon.net_util import get_subcircuit_ports
 import logging
+from typing import Dict
 
 from scipy import interpolate
 
 logger = logging.getLogger(__name__)
 
 
 def characterize_input_capacitances(
         input_pins: List[str],
         active_pin: str,
         output_pins: List[str],
         cell_conf: CellConfig
-):
+) -> Dict[str, float]:
     """
     Estimate the input capacitance of the `active_pin`.
     The estimation is done by simulating a constant current flowing into an input and measuring the
     time it takes for the input to go from high to low or low to high. This time multiplied by the current
     yields the transported charge which together with the voltage difference tells the capacitance.
     The measurement is done for all combinations of static inputs (all other inputs that are not measured).
 
     :param input_pins: List of all input pin names.
     :param active_pin: Name of the pin to be measured.
     :param output_pins: List of cell output pins.
     :param config: Parameters for the characterization.
 
+    :returns: Dictionary containing input capacitances for rise, fall and average case.
     """
 
     assert isinstance(cell_conf, CellConfig)
     assert isinstance(cell_conf.global_conf, CharacterizationConfig)
     cfg = cell_conf.global_conf
 
     inputs_inverted = cell_conf.complementary_pins.values()
```

### Comparing `lctime-0.0.23/src/lctime/characterization/main_lctime.py` & `lctime-0.0.24/src/lctime/characterization/main_lctime.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Copyright (c) 2019-2020 Thomas Kramer.
-# SPDX-FileCopyrightText: 2022 Thomas Kramer <code@tkramer.ch>
+# SPDX-FileCopyrightText: 2019-2024 Thomas Kramer <code@tkramer.ch>
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 """
 Main program file for the `lctime` standard-cell characterization tool.
 """
 
@@ -21,18 +20,19 @@
 
 from ..logic.util import is_unate_in_xi
 from ..liberty import util as liberty_util
 from ..logic import functional_abstraction
 from ..logic import seq_recognition
 from ..logic.types import CombinationalOutput
 
-from .util import *
 from .timing_combinatorial import characterize_comb_cell
 from .timing_sequential import *
 from .input_capacitance import characterize_input_capacitances
+from . import flipflop
+from . import util
 
 from copy import deepcopy
 
 from ..lccommon import net_util
 from ..lccommon.net_util import load_transistor_netlist, is_ground_net, is_supply_net
 import networkx as nx
 from sympy.logic import satisfiable
@@ -173,628 +173,786 @@
     """
     Command-line tool for cell characterization.
     Currently only combinatorial cells are supported excluding tri-state cells.
     :return:
     """
 
     print(licence_notice_string_single_line())
-    print()
 
-    logger = logging.getLogger(__name__)
-    logger.info("lctime main function")
+    lctime = LcTime()
+    lctime.run()
 
-    parser = argparse.ArgumentParser(
-        description='Characterize the timing of a combinatorial cell based on a SPICE netlist. '
-                    'The resulting liberty file will contain the data of the input liberty file '
-                    'plus the updated characteristics of the selected cell.',
-        epilog='Example: lctime --liberty specification.lib --cell INVX1 AND2X1 --spice netlists.sp -I '
-               'transistor_model.m --output mylib.lib')
-
-    parser.add_argument('-l', '--liberty', required=True, metavar='LIBERTY', type=str,
-                        help='Liberty file. This must contain all necessary specifications '
-                             'needed to characterize the cell.')
-
-    parser.add_argument('--cell', required=True, metavar='CELL_NAME', type=str,
-                        action='append',
-                        nargs='+',
-                        help='Names of cells to be characterized.')
-
-    parser.add_argument('--spice', required=True, metavar='SPICE', type=str,
-                        action='append',
-                        nargs='+',
-                        help='SPICE netlist containing a subcircuit with the same name as the cell.')
-
-    parser.add_argument('-I', '--include', required=False, action='append', metavar='SPICE_INCLUDE', type=str,
-                        help='SPICE files to include such as transistor models.')
-
-    parser.add_argument('-L', '--library', required=False, action='append', metavar='SPICE_LIB', type=str,
-                        help='SPICE .LIB statements defining each a path to the library and a library name.'
-                             'Example: --library "/path/to/lib libraryName".')
-
-    parser.add_argument('--calc-mode', metavar='CALC_MODE', type=str, choices=['worst', 'typical', 'best'],
-                        default='typical',
-                        help='Calculation mode for computing the default timing arc'
-                             ' based on the conditional timing arcs. "worst", "typical" (average) or "best".')
-
-    parser.add_argument('-o', '--output', required=True, metavar='LIBERTY_OUT', type=str, help='Output liberty file.')
-
-    parser.add_argument('--workingdir', required=False, metavar='WORKDIR', type=str,
-                        help="Directory for ngspice simulation scripts and raw results.")
-
-    parser.add_argument('--output-loads', required=True, metavar='CAPACITANCES', type=str,
-                        help="List of output load capacitances for the cells. In pico Farads."
-                             " List must be quoted, elements must be separated by a comma."
-                             " Example: '0.05, 0.1, 0.2'")
-
-    parser.add_argument('--slew-times', required=True, metavar='SLEWTIMES', type=str,
-                        help="List of slew times of the input signals in nano seconds."
-                             " List must be quoted, elements must be separated by a comma."
-                             " Example: '0.05, 0.1, 0.2'")
-
-    parser.add_argument('--related-pin-transition', required=False, metavar='SLEWTIMES', type=str,
-                        help="List of slew times of the clock signal in nano seconds. "
-                             "This is used for sequential cells only. "
-                             "List must be quoted, elements must be separated by a comma. "
-                             "Example: '0.05, 0.1, 0.2'")
-
-    parser.add_argument('--analyze-cell-function', action='store_true',
-                        help='Derive the logical function of the cell from the SPICE netlist (experimental).')
-
-    parser.add_argument('--diff', required=False,
-                        nargs="+",
-                        metavar='DIFFERENTIAL_PATTERN',
-                        type=str,
-                        help='Specify differential inputs as "NonInverting,Inverting" tuples.'
-                             'The placeholder "%%" can be used like "%%_P,%%_N" or "%%,%%_Diff", ...')
-
-    parser.add_argument('--time-step', default=10e-12,
-                        metavar='TIME_STEP',
-                        type=float,
-                        help='Specify the simulation time-step in seconds. Default is 10e-12.')
-
-    parser.add_argument('--debug', action='store_true',
-                        help='Enable debug mode (more verbose logging).')
-
-    parser.add_argument('--debug-plots', action='store_true',
-                        help='Create debug plots of simulation waveforms.')
 
-    # Parse arguments
-    args = parser.parse_args()
+class LcTime:
 
-    DEBUG = args.debug
-    log_level = logging.DEBUG if DEBUG else logging.INFO
+    def __init__(self):
+        args = None
+        workdir: str = None
+        library: Group = None
+        new_library: Group = None # Library under construction.
+        conf: CharacterizationConfig = None
+
+    def run(self):
+        logger = logging.getLogger(__name__)
+        logger.info("lctime main function")
+
+        self.f00_parse_args()
+        self.f01_init_logging()
+        self.f02_init_workdir()
+        self.f03_init_netlists()
+        self.f04_check_cell_names()
+        self.f05_load_liberty_template()
+        self.f06_check_delay_model()
+        self.f07_init_new_library()
+        self.f08_load_operating_conditions()
+        self.f09_init_include_statements()
+        self.f10_init_characterization_config()
+        self.f11_init_table_indices()
+        self.f12_characterize_library()
+        self.write_liberty()
+
+    def f00_parse_args(self):
+        parser = argparse.ArgumentParser(
+            description='Characterize the timing of a combinatorial cell based on a SPICE netlist. '
+                        'The resulting liberty file will contain the data of the input liberty file '
+                        'plus the updated characteristics of the selected cell.',
+            epilog='Example: lctime --liberty specification.lib --cell INVX1 AND2X1 --spice netlists.sp -I '
+                   'transistor_model.m --output mylib.lib')
+
+        parser.add_argument('-l', '--liberty', required=True, metavar='LIBERTY', type=str,
+                            help='Liberty file. This must contain all necessary specifications '
+                                 'needed to characterize the cell.')
+
+        parser.add_argument('--cell', required=True, metavar='CELL_NAME', type=str,
+                            action='append',
+                            nargs='+',
+                            help='Names of cells to be characterized.')
+
+        parser.add_argument('--spice', required=True, metavar='SPICE', type=str,
+                            action='append',
+                            nargs='+',
+                            help='SPICE netlist containing a subcircuit with the same name as the cell.')
+
+        parser.add_argument('-I', '--include', required=False, action='append', metavar='SPICE_INCLUDE', type=str,
+                            help='SPICE files to include such as transistor models.')
+
+        parser.add_argument('-L', '--library', required=False, action='append', metavar='SPICE_LIB', type=str,
+                            help='SPICE .LIB statements defining each a path to the library and a library name.'
+                                 'Example: --library "/path/to/lib libraryName".')
+
+        parser.add_argument('--calc-mode', metavar='CALC_MODE', type=str, choices=['worst', 'typical', 'best'],
+                            default='typical',
+                            help='Calculation mode for computing the default timing arc'
+                                 ' based on the conditional timing arcs. "worst", "typical" (average) or "best".')
+
+        parser.add_argument('-o', '--output', required=True, metavar='LIBERTY_OUT', type=str, help='Output liberty file.')
+
+        parser.add_argument('--workingdir', required=False, metavar='WORKDIR', type=str,
+                            help="Directory for ngspice simulation scripts and raw results.")
+
+        parser.add_argument('--output-loads', required=True, metavar='CAPACITANCES', type=str,
+                            help="List of output load capacitances for the cells. In pico Farads."
+                                 " List must be quoted, elements must be separated by a comma."
+                                 " Example: '0.05, 0.1, 0.2'")
+
+        parser.add_argument('--slew-times', required=True, metavar='SLEWTIMES', type=str,
+                            help="List of slew times of the input signals in nano seconds."
+                                 " List must be quoted, elements must be separated by a comma."
+                                 " Example: '0.05, 0.1, 0.2'")
+
+        parser.add_argument('--related-pin-transition', required=False, metavar='SLEWTIMES', type=str,
+                            help="List of slew times of the clock signal in nano seconds. "
+                                 "This is used for sequential cells only. "
+                                 "List must be quoted, elements must be separated by a comma. "
+                                 "Example: '0.05, 0.1, 0.2'")
+
+        parser.add_argument('--analyze-cell-function', action='store_true',
+                            help='Derive the logical function of the cell from the SPICE netlist (experimental).')
+
+        parser.add_argument('--diff', required=False,
+                            nargs="+",
+                            metavar='DIFFERENTIAL_PATTERN',
+                            type=str,
+                            help='Specify differential inputs as "NonInverting,Inverting" tuples.'
+                                 'The placeholder "%%" can be used like "%%_P,%%_N" or "%%,%%_Diff", ...')
+
+        parser.add_argument('--time-step', default=10e-12,
+                            metavar='TIME_STEP',
+                            type=float,
+                            help='Specify the simulation time-step in seconds. Default is 10e-12.')
+
+        parser.add_argument('--debug', action='store_true',
+                            help='Enable debug mode (more verbose logging).')
 
-    if DEBUG:
-        log_format = '%(module)16s %(levelname)8s: %(message)s'
-    else:
-        # Also output name of function in DEBUG mode.
-        log_format = '%(module)16s %(funcName)16s %(levelname)8s: %(message)s'
+        parser.add_argument('--debug-plots', action='store_true',
+                            help='Create debug plots of simulation waveforms.')
 
-    logging.basicConfig(format=log_format, level=log_level)
+        parser.add_argument('-j', '--jobs', type=int, default=1, metavar="NUM_JOBS", help="number of threads for cell-level parallelism")
 
-    workingdir = args.workingdir
-    if workingdir is None:
-        workingdir = tempfile.mkdtemp(prefix="lctime-")
-
-    # Get list of cell names to be characterized.
-    cell_names = [n for names in args.cell for n in names]  # Flatten the nested list.
-
-    # Get list of user-provided netlist files.
-    netlist_files = [n for names in args.spice for n in names]  # Flatten the nested list.
-
-    # Generate a lookup-table which tells for each cell name which netlist file to use.
-    netlist_file_table: Dict[str, str] = dict()
-    for netlist_file in netlist_files:
-        logger.info("Load SPICE netlist: {}".format(netlist_file))
-        parser = SpiceParser(path=netlist_file)
-        for sub in parser.subcircuits:
-            if sub.name in netlist_file_table:
-                # Abort if a sub circuit is defined in multiple netlists.
-                abort(
-                    f"Sub-circuit '{sub.name}' is defined in multiple netlists: {netlist_file_table[sub.name]}, {netlist_file}")
-            netlist_file_table[sub.name] = netlist_file
-
-    # Test if all cell names can be found in the netlist files.
-    cell_names_not_found = set(cell_names) - netlist_file_table.keys()
-    if cell_names_not_found:
-        abort(f"Cell names not found in netlists: {', '.join(cell_names_not_found)}")
-
-    # Load liberty file.
-    lib_file = args.liberty
-    logger.info("Reading liberty: {}".format(lib_file))
-    with open(lib_file) as f:
-        data = f.read()
-    library = liberty_parser.parse_liberty(data)
-
-    # Check if the delay model is supported.
-    delay_model = library['delay_model']
-    supported_delay_models = ['table_lookup']
-    if delay_model not in supported_delay_models:
-        msg = "Delay model not supported: '{}'. Must be one of {}.".format(delay_model,
-                                                                           ", ".join(supported_delay_models))
-        logger.error(msg)
-        assert False, msg
-
-    # Make independent copies of the library.
-    new_library = deepcopy(library)
-    # Strip all cell groups.
-    new_library.groups = [g for g in new_library.groups if g.group_name != 'cell']
-    # Strip away all LUT template table groups.
-    table_types = ['lu_table_template', 'power_lut_template']
-    new_library.groups = [g for g in new_library.groups if g.group_name not in table_types]
-
-    # Load operation voltage and temperature.
-    # TODO: load voltage/temperature from operating_conditions group
-    supply_voltage = library['nom_voltage']
-    temperature = library['nom_temperature']
-    logger.info('Supply voltage = {:f} V'.format(supply_voltage))
-    logger.info('Temperature = {:f} V'.format(temperature))
-
-    # Get timing corner from liberty file.
-    # Find definitions of operating conditions and sort them by name.
-    operating_conditions_list = library.get_groups('operating_conditions')
-    # Put into a dict by name.
-    operating_conditions: Dict[str, Group] = {str(g.args[0]): g for g in operating_conditions_list}
+        # Parse arguments
+        self.args = parser.parse_args()
+        
 
-    logger.info("Operating conditions: {}".format(set(operating_conditions.keys())))
+    def f01_init_logging(self):
+        DEBUG = self.args.debug
+        log_level = logging.DEBUG if DEBUG else logging.INFO
+
+        if DEBUG:
+            # Also output name of function in DEBUG mode.
+            log_format = '%(module)16s %(funcName)16s %(levelname)8s: %(message)s'
+        else:
+            log_format = '%(levelname)8s: %(message)s'
 
-    """
-    TODO: Use the information from the operating conditions.
-    Example:
-    operating_conditions (MPSS) {
-        calc_mode : worst ;
-        process : 1.5 ;
-        process_label : "ss" ;
-        temperature : 70 ;
-        voltage : 4.75 ;
-        tree_type : worse_case_tree ;
-    }
-    """
+        logging.basicConfig(format=log_format, level=log_level)
+    
+    def f02_init_workdir(self):
+        self.workingdir = self.args.workingdir
+        if self.workingdir is None:
+            self.workingdir = tempfile.mkdtemp(prefix="lctime-")
 
-    def _transistors2multigraph(transistors) -> nx.MultiGraph:
-        """ Create a graph representing the transistor network.
-            Each edge corresponds to a transistor, each node to a net.
-        """
-        G = nx.MultiGraph()
-        for t in transistors:
-            G.add_edge(t.source_net, t.drain_net, (t.gate_net, t.channel_type))
-        assert nx.is_connected(G)
-        return G
-
-    # Get timing corner from liberty file.
-    # TODO: let user overwrite it.
-    calc_modes = {
-        'typical': CalcMode.TYPICAL,
-        'worst': CalcMode.WORST,
-        'best': CalcMode.BEST,
-    }
-
-    # TODO: Make use of this.
-    default_operating_conditions = library['default_operating_conditions']
-    logger.info("Default operating conditions: {}".format(default_operating_conditions))
-
-    assert args.calc_mode in calc_modes, "Unknown calculation mode: {}".format(args.calc_mode)
-
-    calc_mode = calc_modes[args.calc_mode]
-    logger.info("calc_mode: {}".format(calc_mode.name))
-
-    # Read trip points from liberty file.
-    trip_points = read_trip_points_from_liberty(library)
-
-    logger.debug(trip_points)
-
-    spice_includes = args.include if args.include else []
-    if len(spice_includes) == 0:
-        logger.warning("No transistor model supplied. Use --include or -I.")
-
-    # Sanitize include paths.
-    input_argument_error = False
-    for path in spice_includes:
-        if not os.path.isfile(path):
-            logger.error(f"Include file does not exist: {path}")
-            input_argument_error = True
-
-    spice_libraries_raw: List[str] = args.library if args.library else []
-    # Split library statements into path and library name.
-    spice_libraries: List[Tuple[str, str]] = [tuple(s.strip() for s in l.split(" ", maxsplit=2))
-                                              for l in spice_libraries_raw
-                                              ]
-    # Sanitize the library arguments.
-    for lib, raw in zip(spice_libraries, spice_libraries_raw):
-        if len(lib) != 2 or not lib[0] or not lib[1]:
-            abort(f'Library statements must be of the format "/path/to/library libraryName". Found: "{raw}".')
-
-        path, name = lib
-        if not os.path.isfile(path):
-            logger.error(f"Library file does not exist: {path}")
-            input_argument_error = True
-
-    # Exit if some input arguments were obviously invalid.
-    if input_argument_error:
-        abort("Exit because of invalid arguments.")
-
-    # .LIB statements
-    library_statements = [f".LIB {path} {name}" for path, name in spice_libraries]
-
-    # .INCLUDE statements
-    include_statements = [f".include {i}" for i in spice_includes]
-
-    setup_statements = library_statements + include_statements
-
-    # Setup array of output capacitances and input slews.
-    output_capacitances = np.array([float(s.strip()) for s in args.output_loads.split(",")]) * 1e-12  # pF
-    input_transition_times = np.array([float(s.strip()) for s in args.slew_times.split(",")]) * 1e-9  # ns
-
-    # Transition times of the clock pin.
-    if args.related_pin_transition:
-        related_pin_transition = np.array(
-            [float(s.strip()) for s in args.related_pin_transition.split(",")]) * 1e-9  # ns
-    else:
-        related_pin_transition = None
+    def f03_init_netlists(self):
+        
+        # Get list of cell names to be characterized.
+        self.cell_names = [n for names in self.args.cell for n in names]  # Flatten the nested list.
+
+        # Get list of user-provided netlist files.
+        netlist_files = [n for names in self.args.spice for n in names]  # Flatten the nested list.
 
-    logger.info(f"Output capacitances [pF]: {output_capacitances / 1e-12}")
-    logger.info(f"Input slew times [ns]: {input_transition_times / 1e-9}")
-    if related_pin_transition is not None:
-        logger.info(f"Related pin transition times [ns]: {related_pin_transition / 1e-9}")
-
-    # TODO: Make time resolution parametrizable.
-    time_resolution_seconds = float(args.time_step)
-    logger.info(f"Time resolution = {time_resolution_seconds}s")
-    if time_resolution_seconds <= 0:
-        abort('Time step must be larger than zero.')
-
-    if time_resolution_seconds > 1e-9:
-        logger.warning(f"Timestep is larger than 1ns: {time_resolution_seconds}s")
-
-    # Setup configuration struct.
-    conf = CharacterizationConfig()
-    conf.supply_voltage = supply_voltage
-    conf.trip_points = trip_points
-    conf.timing_corner = calc_mode
-    conf.setup_statements = setup_statements
-    conf.time_step = time_resolution_seconds
-    conf.temperature = temperature
-    conf.workingdir = workingdir
-    conf.debug = args.debug
-    conf.debug_plots = args.debug_plots
+        # Generate a lookup-table which tells for each cell name which netlist file to use.
+        self.netlist_file_table: Dict[str, str] = dict()
+        for netlist_file in netlist_files:
+            logger.info("Load SPICE netlist: {}".format(netlist_file))
+            parser = SpiceParser(path=netlist_file)
+            for sub in parser.subcircuits:
+                if sub.name in self.netlist_file_table:
+                    # Abort if a sub circuit is defined in multiple netlists.
+                    abort(
+                        f"Sub-circuit '{sub.name}' is defined in multiple netlists: {self.netlist_file_table[sub.name]}, {netlist_file}")
+                self.netlist_file_table[sub.name] = netlist_file
+
+    def f04_check_cell_names(self):
+        # Test if all cell names can be found in the netlist files.
+        cell_names_not_found = set(self.cell_names) - self.netlist_file_table.keys()
+        if cell_names_not_found:
+            abort(f"Cell names not found in netlists: {', '.join(cell_names_not_found)}")
+
+    def f05_load_liberty_template(self):
+        # Load liberty file.
+        lib_file = self.args.liberty
+        logger.info("Reading liberty: {}".format(lib_file))
+        with open(lib_file) as f:
+            data = f.read()
+        self.library = liberty_parser.parse_liberty(data)
+
+    def f06_check_delay_model(self):
+        # Check if the delay model is supported.
+        delay_model = self.library['delay_model']
+        supported_delay_models = ['table_lookup']
+        if delay_model not in supported_delay_models:
+            msg = "Delay model not supported: '{}'. Must be one of {}.".format(delay_model,
+                                                                               ", ".join(supported_delay_models))
+            logger.debug(msg)
+            abort(msg)
 
-    conf.get_units_from_liberty(library)
+    def f07_init_new_library(self):
+        # Make independent copies of the library.
+        self.new_library = deepcopy(self.library)
+        # Strip all cell groups.
+        self.new_library.groups = [g for g in self.new_library.groups if g.group_name != 'cell']
+        # Strip away all LUT template table groups.
+        table_types = ['lu_table_template', 'power_lut_template']
+        self.new_library.groups = [g for g in self.new_library.groups if g.group_name not in table_types]
 
-    logger.info(f"Capacitance unit: {conf.capacitance_unit} F")
-    logger.info(f"Time unit: {conf.time_unit} s")
+    def f10_init_characterization_config(self):
+        
+        # Setup configuration struct.
+        conf = CharacterizationConfig()
+        
+        # Load operation voltage and temperature.
+        # TODO: load voltage/temperature from operating_conditions group
+        conf.supply_voltage = self.library['nom_voltage']
+        logger.info('Supply voltage = {:f} V'.format(conf.supply_voltage))
+        conf.temperature = self.library['nom_temperature']
+        logger.info('Temperature = {:f} V'.format(conf.temperature))
+
+        # Read trip points from liberty file.
+        conf.trip_points = util.read_trip_points_from_liberty(self.library)
+        logger.debug(conf.trip_points)
+        
+        # Get timing corner from liberty file.
+        # TODO: let user overwrite it.
+        calc_modes = {
+            'typical': CalcMode.TYPICAL,
+            'worst': CalcMode.WORST,
+            'best': CalcMode.BEST,
+        }
+        assert self.args.calc_mode in calc_modes, "Unknown calculation mode: {}".format(self.args.calc_mode)
+        conf.timing_corner = calc_modes[self.args.calc_mode]
+        logger.info("timing corner: {}".format(conf.timing_corner.name))
+        
+        conf.setup_statements = self.setup_statements
+        
+        # Simulation time step
+        time_resolution_seconds = float(self.args.time_step)
+        logger.info(f"Time resolution = {time_resolution_seconds}s")
+        if time_resolution_seconds <= 0:
+            abort('Time step must be larger than zero.')
+
+        if time_resolution_seconds > 1e-9:
+            logger.warning(f"Timestep is larger than 1ns: {time_resolution_seconds}s")
+        conf.time_step = time_resolution_seconds
+        
+        conf.workingdir = self.workingdir
+        conf.debug = self.args.debug
+        conf.debug_plots = self.args.debug_plots
+        conf.get_units_from_liberty(self.library)
+
+        logger.info(f"Capacitance unit: {conf.capacitance_unit} F")
+        logger.info(f"Time unit: {conf.time_unit} s")
+        self.conf = conf
+        
+    def f08_load_operating_conditions(self):
+        # TODO: not used at the moment
+        # Get timing corner from liberty file.
+        # Find definitions of operating conditions and sort them by name.
+        operating_conditions_list = self.library.get_groups('operating_conditions')
+        # Put into a dict by name.
+        operating_conditions: Dict[str, Group] = {str(g.args[0]): g for g in operating_conditions_list}
 
-    # Characterize all cells in the list.
-    def characterize_cell(cell_name: str) -> Group:
+        logger.info("Operating conditions: {}".format(set(operating_conditions.keys())))
+
+        """
+        TODO: Use the information from the operating conditions.
+        Example:
+        operating_conditions (MPSS) {
+            calc_mode : worst ;
+            process : 1.5 ;
+            process_label : "ss" ;
+            temperature : 70 ;
+            voltage : 4.75 ;
+            tree_type : worse_case_tree ;
+        }
+        """
+
+        # TODO: Make use of this.
+        default_operating_conditions = self.library['default_operating_conditions']
+        logger.info("Default operating conditions: {}".format(default_operating_conditions))
+        
+    def f09_init_include_statements(self):
+        # Create .include statements for ngspice
+        
+        spice_includes = self.args.include if self.args.include else []
+        if len(spice_includes) == 0:
+            logger.warning("No transistor model supplied. Use --include or -I.")
+
+        # Sanitize include paths.
+        input_argument_error = False
+        for path in spice_includes:
+            if not os.path.isfile(path):
+                logger.error(f"Include file does not exist: {path}")
+                input_argument_error = True
+
+        spice_libraries_raw: List[str] = self.args.library if self.args.library else []
+        # Split library statements into path and library name.
+        spice_libraries: List[Tuple[str, str]] = [tuple(s.strip() for s in l.split(" ", maxsplit=2))
+                                                  for l in spice_libraries_raw
+                                                  ]
+        # Sanitize the library arguments.
+        for lib, raw in zip(spice_libraries, spice_libraries_raw):
+            if len(lib) != 2 or not lib[0] or not lib[1]:
+                abort(f'Library statements must be of the format "/path/to/library libraryName". Found: "{raw}".')
+
+            path, name = lib
+            if not os.path.isfile(path):
+                logger.error(f"Library file does not exist: {path}")
+                input_argument_error = True
+
+        # Exit if some input arguments were obviously invalid.
+        if input_argument_error:
+            abort("Exit because of invalid arguments.")
+
+        # .LIB statements
+        library_statements = [f".LIB {path} {name}" for path, name in spice_libraries]
+
+        # .INCLUDE statements
+        include_statements = [f".include {i}" for i in spice_includes]
+
+        self.setup_statements = library_statements + include_statements
+        
+    def f11_init_table_indices(self):
+        """
+        Load values for input transition times and output loads.
+        """
+        
+        # Setup array of output capacitances and input slews.
+        self.output_capacitances = np.array([float(s.strip()) for s in self.args.output_loads.split(",")]) * 1e-12  # pF
+        self.input_transition_times = np.array([float(s.strip()) for s in self.args.slew_times.split(",")]) * 1e-9  # ns
+
+        # Transition times of the clock pin.
+        if self.args.related_pin_transition:
+            self.related_pin_transition = np.array(
+                [float(s.strip()) for s in self.args.related_pin_transition.split(",")]) * 1e-9  # ns
+        else:
+            self.related_pin_transition = None
+
+        logger.info(f"Output capacitances [pF]: {self.output_capacitances / 1e-12}")
+        logger.info(f"Input slew times [ns]: {self.input_transition_times / 1e-9}")
+        if self.related_pin_transition is not None:
+            logger.info(f"Related pin transition times [ns]: {self.related_pin_transition / 1e-9}")
+
+    def f12_characterize_library(self):
+        if self.args.jobs != 1:
+            # Characterize cells in parallel.
+            new_cell_groups = joblib.Parallel(n_jobs=self.args.jobs, prefer='threads') \
+                (joblib.delayed(self.characterize_cell)(cell_name) for cell_name in self.cell_names)
+        else:
+            # Characterize cells sequentially.
+            new_cell_groups = [self.characterize_cell(cell_name) for cell_name in self.cell_names]
+
+        for new_cell_group in new_cell_groups:
+            self.new_library.groups.append(new_cell_group)      
+
+
+    def write_liberty(self):
+        """
+        Dump new liberty library to disk.
+        """
+        assert self.new_library is not None
+        
+        logger.info("Write liberty: {}".format(self.args.output))
+        with open(self.args.output, 'w') as f:
+
+            # Write URL to lctime.
+
+            s = """/*
+Generated by lctime ({}).
+*/
+    
+    """
+            f.write(s.format(original_source_repository()))
+
+            f.write(str(self.new_library))
+        
+    def characterize_cell(self, cell_name: str) -> Group:
         """
         Characterize a cell and create an updated cell group.
         :param cell_name:
         :return: Return an updated cell group.
         """
 
-        # Create working directory if it does not exist yet.
-        cell_workingdir = os.path.join(conf.workingdir, cell_name)
-        if not os.path.exists(cell_workingdir):
-            os.mkdir(cell_workingdir)
+        cell_setup = CellSetup(self, cell_name)
 
-        # Get netlist and liberty group.
-        netlist_file = netlist_file_table[cell_name]
+        return cell_setup.run()
+
+class CellSetup:
+    """
+    Measurement setup for a single cell.
+    """
+
+    def __init__(self, lctime: LcTime, cell_name: str):
+        self.lctime = lctime
+        """
+        Global values.
+        """
+        self.cell_name: str = cell_name
+        self.cell_workdir: str = None
+        self.output_capacitances = None
+        self.input_transition_times = None
+        self.related_pin_transition = None
+        self.cell_group = None
+        self.cell_type_liberty = None
+        "Cell type as derived from liberty file."
+        self.cell_type = None
+
+    def init_workdir(self):
+        """
+        Create working directory if it does not exist yet.
+        """
+        self.cell_workingdir = os.path.join(self.lctime.conf.workingdir, self.cell_name)
+        if not os.path.exists(self.cell_workingdir):
+            os.mkdir(self.cell_workingdir)
+
+    def init_indices(self):
+        self.output_capacitances = self.lctime.output_capacitances
+        self.input_transition_times = self.lctime.input_transition_times
+        self.related_pin_transition = self.lctime.related_pin_transition
+
+    def recognize_cell_type(self):
         try:
-            cell_group = select_cell(library, cell_name)
+            self.cell_group = select_cell(self.lctime.library, self.cell_name)
 
             # Determine type of cell (latch, flip-flop, combinational).
-            cell_type_liberty = recognize_cell_from_liberty(cell_group)
-            cell_type = cell_type_liberty
+            self.cell_type_liberty = recognize_cell_from_liberty(self.cell_group)
+            self.cell_type = self.cell_type_liberty
         except KeyError as e:
-            logger.warning(f"No cell group defined yet in liberty file: {cell_name}")
+            logger.warning(f"No cell group defined yet in liberty file: {self.cell_name}")
 
-            if not args.analyze_cell_function:
+            if not self.lctime.args.analyze_cell_function:
                 abort("Cell is not defined in liberty. Enable cell recognition with --analyze.")
 
-            cell_type_liberty = Combinational()  # Default: Empty cell.
+            self.cell_type_liberty = Combinational()  # Default: Empty cell.
 
             # Cell group does not exist, so create it.
             logger.debug("Create empty cell group.")
-            cell_group = Group(group_name='cell', args=[cell_name])
-            library.groups.append(cell_group)
+            self.cell_group = Group(group_name='cell', args=[self.cell_name])
+            self.lctime.library.groups.append(self.cell_group)
 
             # The liberty did not define anything about this cell.
-            cell_type = None
+            self.cell_type = None
 
         # Check that the name matches.
-        assert cell_group.args == [cell_name], "Cell name does not match."  # This should not happen.
-
-        logger.info("Cell: {}".format(cell_name))
-        logger.info("Netlist: {}".format(netlist_file))
-
+        assert self.cell_group.args == [self.cell_name], "Cell name does not match."  # This should not happen.
+        
+    def init_pins(self):
         # Get information on pins from the liberty file.
-        input_pins = [str(s) for s in cell_type_liberty.inputs]
-        output_pins = [str(s) for s in cell_type_liberty.outputs.keys()]
+        self.input_pins = [str(s) for s in self.cell_type_liberty.inputs]
+        self.output_pins = [str(s) for s in self.cell_type_liberty.outputs.keys()]
+        
+        logger.info(f"Input pins as defined in liberty: {self.input_pins}")
+        logger.info(f"Output pins as defined in liberty: {sorted(self.cell_type_liberty.outputs.keys())}")
+
 
-        liberty_pins = set(input_pins) | set(output_pins)
+    def init_case_lookup_table(self):
+        """
+        Create lookup table to fix lower/upper case mismatches between Liberty and SPICE.
+        """
+        
+        # Get all IO pins defined in liberty.
+        liberty_pins = set(self.input_pins) | set(self.output_pins)
         # Convert to strings.
         liberty_pins = {str(p) for p in liberty_pins}
-
+        
         # Create a lookup table to reconstruct lower/upper case letters.
         # This is a workaround. The SPICE parser converts everything to uppercase.
-        case_lookup_table = {p.lower(): p for p in liberty_pins}
-        if len(case_lookup_table) != len(liberty_pins):
+        self.case_lookup_table = {p.lower(): p for p in liberty_pins}
+        if len(self.case_lookup_table) != len(liberty_pins):
             # It's not a one-to-one mapping!
             logger.warning(f"Mixed lower case and upper case could cause trouble.")
 
-        def fix_case(pin: str) -> str:
-            """
-            Restore lower/upper case of signals that went lost during SPICE parsing.
-            """
-            return case_lookup_table.get(pin.lower(), pin)
-
-        logger.info(f"Input pins as defined in liberty: {input_pins}")
-        logger.info(f"Output pins as defined in liberty: {sorted(cell_type_liberty.outputs.keys())}")
-
-        # Load netlist of cell
-        # TODO: Load all netlists at the beginning.
-        logger.info('Load netlist: %s', netlist_file)
-        try:
-            transistors_abstract, cell_pins = load_transistor_netlist(netlist_file, cell_name)
-        except Exception as e:
-            abort(str(e))
-
-        if len(transistors_abstract) == 0:
-            msg = "No transistors found in cell. (The netlist must be flattened, sub-circuits are not resolved)"
-            abort(msg)
-
-        cell_pins = [fix_case(p) for p in cell_pins]
-        for t in transistors_abstract:
-            t.source_net = fix_case(t.source_net)
-            t.drain_net = fix_case(t.drain_net)
-            t.gate_net = fix_case(t.gate_net)
-
-        # Get pin ordering of spice circuit.
-        spice_ports = get_subcircuit_ports(netlist_file, cell_name)
-        logger.info(f"SPICE subcircuit ports: {spice_ports}")
-        io_pins = net_util.get_io_pins(cell_pins)
-
-        # Detect power pins.
-        # TODO: don't decide based only on net name.
-        power_pins = [p for p in cell_pins if net_util.is_power_net(p)]
-        assert len(power_pins) == 2, "Expected to have 2 power pins."
-        vdd_pins = [p for p in power_pins if net_util.is_supply_net(p)]
-        gnd_pins = [p for p in power_pins if net_util.is_ground_net(p)]
-        assert len(vdd_pins) == 1, "Expected to find one VDD pin but found: {}".format(vdd_pins)
-        assert len(gnd_pins) == 1, "Expected to find one GND pin but found: {}".format(gnd_pins)
-        vdd_pin = vdd_pins[0]
-        gnd_pin = gnd_pins[0]
-
-        # Sanity check: All pins defined in liberty must appear in the SPICE netlist.
-        all_liberty_pins = set()
-        for pin in cell_group.get_groups("pin"):
-            assert isinstance(pin, liberty_parser.Group)
-            pin_name = pin.args[0]
-            all_liberty_pins.add(pin_name)
-            complementary_pin = pin.get("complementary_pin")
-            if complementary_pin is not None:
-                all_liberty_pins.add(complementary_pin)
-        all_spice_pins = set(cell_pins)
-        pins_not_in_spice = sorted(all_liberty_pins - all_spice_pins)
-
-        if pins_not_in_spice:
-            abort(f"Pins defined in liberty but not in SPICE netlist: {', '.join(pins_not_in_spice)}")
-
-        # Convert the transistor network into its multi-graph representation.
-        # This is used for a formal analysis of the network.
-        transistor_graph = _transistors2multigraph(transistors_abstract)
-
-        # Detect input nets from the transistor netlist (if enabled).
-        if args.analyze_cell_function:
-            logger.debug("Detect input nets from the circuit.")
-            detected_inputs = functional_abstraction.find_input_gates(transistor_graph)
-            # Detect nets that must be inputs (connected to gates only but do not
-            # appear in the list of pins in the SPICE circuit definition.
-            inputs_missing_in_spice = detected_inputs - all_spice_pins
-            if inputs_missing_in_spice:
-                logger.warning(f"The circuit has gate nets that must be inputs "
-                               f"but are not in the pin definition of the SPICE circuit: "
-                               f"{', '.join(sorted(inputs_missing_in_spice))}")
-            # Same check for pins declared in liberty template.
-            inputs_missing_in_liberty = detected_inputs - all_liberty_pins
-            if inputs_missing_in_liberty:
-                logger.warning(f"The circuit has gate nets that must be inputs "
-                               f"but are not declared as a pin in the liberty template: "
-                               f"{', '.join(sorted(inputs_missing_in_liberty))}")
-
-            # Add detected input pins.
-            diff = detected_inputs - set(input_pins)
-            if diff:
-                logger.info(f"Also include detected pins: {', '.join(sorted(diff))}")
-                input_pins.extend(diff)
-
-            # Find pins that are defined in the SPICE circuit but are not inputs nor power.
-            maybe_outputs = all_spice_pins - set(input_pins) - set(power_pins)
-            if maybe_outputs:
-                logger.info(f"Potential output pins: {', '.join(sorted(maybe_outputs))}")
-                output_pins.extend(maybe_outputs)
+    def fix_case(self, pin: str) -> str:
+        """
+        Restore lower/upper case of signals that went lost during SPICE parsing.
+        """
+        return self.case_lookup_table.get(pin.lower(), pin)
 
-        # Sanity check.
-        if len(input_pins) == 0:
-            msg = "Cell has no input pins."
-            logger.error(msg)
-            assert False, msg
-
-        # Sanity check.
-        if len(output_pins) == 0:
-            msg = "Cell has no output pins."
-            logger.error(msg)
-            assert False, msg
+    def init_differential_inputs(self):
 
         # Extract differential pairs from liberty.
         # Liberty allows to reference complementary pins with the 'complementary_pin' attribute.
         logger.debug("Load complementary pins from liberty.")
         differential_inputs_liberty = dict()
-        for pin in cell_group.get_groups("pin"):
+        for pin in self.cell_group.get_groups("pin"):
             assert isinstance(pin, liberty_parser.Group)
             pin_name = pin.args[0]
             complementary_pin = pin.get("complementary_pin")
             if complementary_pin is not None:
                 differential_inputs_liberty[pin_name] = complementary_pin
 
         # Match differential inputs.
-        if args.diff is not None:
+        if self.lctime.args.diff is not None:
             logger.debug("Match complementary pins from user-defined pattern.")
-            differential_inputs_from_pattern = find_differential_inputs_by_pattern(args.diff, input_pins)
+            differential_inputs_from_pattern = find_differential_inputs_by_pattern(self.lctime.args.diff, self.input_pins)
         else:
             differential_inputs_from_pattern = dict()
 
         # Merge the differential pairs provided from the user with the pairs detected from the liberty file.
         differential_inputs_liberty.update(differential_inputs_from_pattern)
-        differential_inputs = differential_inputs_liberty
+        self.differential_inputs = differential_inputs_liberty
 
         # Sanity checks on complementary pins.
         # Complementary pin should not be defined as pin group in liberty file.
-        for pin in cell_group.get_groups("pin"):
+        for pin in self.cell_group.get_groups("pin"):
             assert isinstance(pin, liberty_parser.Group)
             pin_name = pin.args[0]
-            if pin_name in differential_inputs.values():
+            if pin_name in self.differential_inputs.values():
                 logger.warning(
                     f"Complementary pin is modelled in the liberty file but will not be characterized: {pin_name}")
 
-        for noninv, inv in differential_inputs.items():
+        for noninv, inv in self.differential_inputs.items():
             logger.info(f"Differential input (+,-): {noninv}, {inv}")
 
         # Find all input pins that are not inverted inputs of a differential pair.
-        inverted_pins = differential_inputs.values()
-        input_pins_non_inverted = [p for p in input_pins if p not in inverted_pins]
+        inverted_pins = self.differential_inputs.values()
+
+        self.input_pins_non_inverted = [p for p in self.input_pins if p not in inverted_pins]
         "All input pins that are not inverted inputs of a differential pair"
 
-        if args.analyze_cell_function:
-            # Derive boolean functions for the outputs from the netlist.
+
+    def create_cell_config(self) -> CellConfig:
+        # Setup cell specific configuration.
+        cell_conf = CellConfig()
+        cell_conf.cell_name = self.cell_name
+        cell_conf.global_conf = self.lctime.conf
+        cell_conf.complementary_pins = self.differential_inputs
+        cell_conf.ground_net = self.gnd_pin()
+        cell_conf.supply_net = self.vdd_pin()
+        cell_conf.workingdir = self.cell_workingdir
+        cell_conf.spice_netlist_file = self.lctime.netlist_file_table[self.cell_name]
+        
+        # Get pin ordering of spice circuit.
+        cell_conf.spice_ports = get_subcircuit_ports(self.netlist_file_path(), self.cell_name)
+        logger.debug(f"SPICE subcircuit ports: {cell_conf.spice_ports}")
+
+        return cell_conf
+        
+    def netlist_file_path(self) -> str:
+        """
+        Get path to SPICE netlist.
+        """
+        return self.lctime.netlist_file_table[self.cell_name]
+
+    def vdd_pin(self):
+        # TODO: don't decide based only on net name.
+        power_pins = self.power_pins()
+        assert len(power_pins) == 2, "Expected to have 2 power pins."
+        vdd_pins = [p for p in power_pins if net_util.is_supply_net(p)]
+        assert len(vdd_pins) == 1, "Expected to find one VDD pin but found: {}".format(vdd_pins)
+        return vdd_pins[0]
+    
+    def gnd_pin(self):
+        # TODO: don't decide based only on net name.
+        power_pins = self.power_pins()
+        assert len(power_pins) == 2, "Expected to have 2 power pins."
+        gnd_pins = [p for p in power_pins if net_util.is_ground_net(p)]
+        assert len(gnd_pins) == 1, "Expected to find one GND pin but found: {}".format(gnd_pins)
+        return gnd_pins[0]
+        
+        
+    def power_pins(self) -> List[str]:
+        # TODO: don't decide based only on net name.
+        return [p for p in self.cell_pins if net_util.is_power_net(p)]
+        
+
+    def get_liberty_pins(self) -> Set:
+        """
+        Get set of pin names defined in liberty template.
+        """
+        liberty_pins = set()
+        for pin in self.cell_group.get_groups("pin"):
+            assert isinstance(pin, liberty_parser.Group)
+            pin_name = pin.args[0]
+            liberty_pins.add(pin_name)
+            complementary_pin = pin.get("complementary_pin")
+            if complementary_pin is not None:
+                liberty_pins.add(complementary_pin)
+        return liberty_pins
+        
+    def check_pins(self):
+        """
+        Sanity check: All pins defined in liberty must appear in the SPICE netlist.
+        """
+        all_spice_pins = set(self.cell_pins)
+        pins_not_in_spice = sorted(self.get_liberty_pins() - all_spice_pins)
+
+        if pins_not_in_spice:
+            abort(f"Pins defined in liberty but not in SPICE netlist: {', '.join(pins_not_in_spice)}")
+
+    def io_pins(self):
+        """
+        Get data pins, i.e. all pins which are not power pins.
+        """
+        return net_util.get_io_pins(self.cell_pins)
+
+    def load_netlist(self):
+        """ Load netlist of cell
+        Populate the self.transistor_graph variable.
+        """
+        # TODO: Load all netlists at the beginning of lctime to detect errors early.
+        # Get netlist and liberty group.
+        logger.info('Load netlist: %s', self.netlist_file_path())
+        try:
+            transistors_abstract, cell_pins = load_transistor_netlist(self.netlist_file_path(), self.cell_name)
+        except Exception as e:
+            abort(str(e))
+
+        if len(transistors_abstract) == 0:
+            msg = "No transistors found in cell. (The netlist must be flattened, sub-circuits are not resolved)"
+            abort(msg)
+
+        self.cell_pins = [self.fix_case(p) for p in cell_pins]
+        for t in transistors_abstract:
+            t.source_net = self.fix_case(t.source_net)
+            t.drain_net = self.fix_case(t.drain_net)
+            t.gate_net = self.fix_case(t.gate_net)
+
+        # Convert the transistor network into its multi-graph representation.
+        # This is used for a formal analysis of the network.
+        self.transistor_graph = _transistors2multigraph(transistors_abstract)
+        
+
+    def recognize_input_pins(self):
+        """
+        Dectect input pins / gates by analyzing the transistor network.
+        """
+        
+        logger.debug("Detect input nets from the circuit.")
+        detected_inputs = functional_abstraction.find_input_gates(self.transistor_graph)
+        # Detect nets that must be inputs (connected to gates only but do not
+        # appear in the list of pins in the SPICE circuit definition.
+        all_spice_pins = set(self.cell_pins)
+        inputs_missing_in_spice = detected_inputs - all_spice_pins
+        if inputs_missing_in_spice:
+            logger.warning(f"The circuit has gate nets that must be inputs "
+                           f"but are not in the pin definition of the SPICE circuit: "
+                           f"{', '.join(sorted(inputs_missing_in_spice))}")
+        # Same check for pins declared in liberty template.
+        inputs_missing_in_liberty = detected_inputs - self.get_liberty_pins()
+        if inputs_missing_in_liberty:
+            logger.warning(f"The circuit has gate nets that must be inputs "
+                           f"but are not declared as a pin in the liberty template: "
+                           f"{', '.join(sorted(inputs_missing_in_liberty))}")
+
+        # Add detected input pins.
+        diff = detected_inputs - set(self.input_pins)
+        if diff:
+            logger.info(f"Also include detected pins: {', '.join(sorted(diff))}")
+            self.input_pins.extend(diff)
+
+        # Find pins that are defined in the SPICE circuit but are not inputs nor power.
+        maybe_outputs = all_spice_pins - set(self.input_pins) - set(self.power_pins())
+        if maybe_outputs:
+            logger.info(f"Potential output pins: {', '.join(sorted(maybe_outputs))}")
+            self.output_pins.extend(maybe_outputs)
+
+    def recognize_cell_function(self):
+            """
+            Derive boolean functions for the outputs from the netlist.
+            """
             logger.info("Derive boolean functions for the outputs based on the netlist.")
 
-            cell_type = analyze_boolean_functions(
-                cell_type,
-                cell_group,
-                transistor_graph,
-                io_pins,
-                differential_inputs,
-                vdd_pin,
-                gnd_pin,
+            self.cell_type = analyze_boolean_functions(
+                self.cell_type,
+                self.cell_group,
+                self.transistor_graph,
+                self.io_pins(),
+                self.differential_inputs,
+                self.vdd_pin(),
+                self.gnd_pin(),
             )
 
-            merge_cell_types(cell_type_liberty, cell_type)
+            merge_cell_types(self.cell_type_liberty, self.cell_type)
+
+    def run(self) -> Group:
+        """
+        Characterize the cell and create a populated 'cell' group data structure.
+        """
+        
+        logger.info("Cell: {}".format(self.cell_name))
+
+        self.init_workdir()
+        self.init_indices()
+        self.recognize_cell_type()
+        self.init_pins()
+        self.init_case_lookup_table()
+        self.load_netlist()
+        self.check_pins()
+        
+
+        # Detect input nets from the transistor netlist (if enabled).
+        if self.lctime.args.analyze_cell_function:
+            self.recognize_input_pins()
+            
+        # Sanity check.
+        if len(self.input_pins) == 0:
+            # TODO: could be valid for tie cells.
+            abort("Cell has no input pins.")
+
+        # Sanity check.
+        if len(self.output_pins) == 0:
+            abort("Cell has no output pins.")
+
+        self.init_differential_inputs()
+
+        if self.lctime.args.analyze_cell_function:
+            self.recognize_cell_function()
         else:
             # Skip functional abstraction and take the functions provided in the liberty file.
             # output_functions_symbolic = output_functions_user
             pass  # TODO
 
-        logger.info("Run characterization.")
 
-        # Setup cell specific configuration.
-        cell_conf = CellConfig()
-        cell_conf.cell_name = cell_name
-        cell_conf.global_conf = conf
-        cell_conf.complementary_pins = differential_inputs
-        cell_conf.ground_net = gnd_pin
-        cell_conf.supply_net = vdd_pin
-        cell_conf.workingdir = cell_workingdir
-        cell_conf.spice_netlist_file = netlist_file_table[cell_name]
-        cell_conf.spice_ports = spice_ports
+        logger.info(f"Run characterization for {self.cell_name}")
 
+        cell_conf = self.create_cell_config()
+        
         # Add groups for the cell to be characterized.
-        new_cell_group = deepcopy(select_cell(library, cell_name))
+        new_cell_group = deepcopy(select_cell(self.lctime.library, self.cell_name))
 
         # Populate the cell group with missing pin groups.
         create_missing_pin_groups(
             new_cell_group,
-            cell_type,
+            self.cell_type,
             cell_conf,
-            output_pins,
-            input_pins_non_inverted
+            self.output_pins,
+            self.input_pins_non_inverted
         )
 
         # Measure input pin capacitances.
         measure_input_capacitances(
-            conf,
+            self.lctime.conf,
             cell_conf,
-            input_pins,
-            input_pins_non_inverted,
-            output_pins,
+            self.input_pins,
+            self.input_pins_non_inverted,
+            self.output_pins,
             new_cell_group
         )
 
-        if isinstance(cell_type, Combinational):
+        if isinstance(self.cell_type, Combinational):
             characterize_combinational_output(
-                new_library,
+                self.lctime.new_library,
                 new_cell_group,
-                conf,
-                cell_type,
+                self.lctime.conf,
+                self.cell_type,
                 cell_conf,
-                input_pins,
-                input_pins_non_inverted,
-                output_capacitances,
-                input_transition_times
+                self.input_pins,
+                self.input_pins_non_inverted,
+                self.output_capacitances,
+                self.input_transition_times
             )
-        elif isinstance(cell_type, SingleEdgeDFF):
-            characterize_flip_flop_output(
-                new_library,
+        elif isinstance(self.cell_type, SingleEdgeDFF):
+            flipflop.characterize_flip_flop_output(
+                self.lctime.new_library,
                 new_cell_group,
-                conf,
-                cell_type,
+                self.lctime.conf,
+                self.cell_type,
                 cell_conf,
-                related_pin_transition,
-                input_transition_times,
-                output_capacitances=output_capacitances
+                self.related_pin_transition,
+                self.input_transition_times,
+                output_capacitances=self.output_capacitances
             )
-        elif isinstance(cell_type, Latch):
+        elif isinstance(self.cell_type, Latch):
             logger.info("Characterize latch.")
             logger.error("Characterization of latches is not yet supported.")
 
             """
             Characterization of latches is very similar to the one of flip-flops. Delays, hold and setup times
             are measured relative to the de-activating edge of the clock signal instead of the active clock edge.
             """
 
-            assert False, "Characterization of latches is not yet supported."
+            abort("Characterization of latches is not yet supported.")
         else:
-            assert False, f"Unsupported cell type: {type(cell_type)}"
+            assert False, f"Unsupported cell type: {type(self.cell_type)}"
 
         assert isinstance(new_cell_group, Group)
         return new_cell_group
 
-    # Characterize cells in parallel.
-    # new_cell_groups = joblib.Parallel(n_jobs=-1, prefer='threads') \
-    #     (joblib.delayed(characterize_cell)(cell_name) for cell_name in cell_names)
-
-    # Characterize cells sequentially.
-    new_cell_groups = [characterize_cell(cell_name) for cell_name in cell_names]
-
-    for new_cell_group in new_cell_groups:
-        new_library.groups.append(new_cell_group)
-
-    with open(args.output, 'w') as f:
-        logger.info("Write liberty: {}".format(args.output))
-
-        # Write URL to lctime.
-
-        s = """/*
-Generated by lctime ({}).
-*/
-
-"""
-        f.write(s.format(original_source_repository()))
-
-        f.write(str(new_library))
-
 
 def analyze_boolean_functions(
-        cell_type: CellType,
+        cell_type: Optional[CellType],
         cell_group: Group,
         transistor_graph: nx.MultiGraph,
         io_pins: Set,
         differential_inputs: Dict[str, str],
         vdd_pin: str,
         gnd_pin: str,
 ) -> CellType:
+    assert isinstance(cell_group, Group)
+    assert cell_group.group_name == 'cell', "not a cell group"
+    assert cell_type is None or isinstance(cell_type, CellType)
+
     abstracted_circuit = functional_abstraction.analyze_circuit_graph(
         graph=transistor_graph,
         pins_of_interest=io_pins,
         constant_input_pins={
             vdd_pin: True,
             gnd_pin: False},
         differential_inputs=differential_inputs,
@@ -1036,23 +1194,23 @@
 
             # Get the table indices.
             # TODO: get correct index/variable mapping from liberty file.
             index_1 = result['total_output_net_capacitance'] / conf.capacitance_unit
             index_2 = result['input_net_transition'] / conf.time_unit
 
             # Create template tables.
-            template_table = liberty_util.create_delay_template_table(new_library, len(index_1), len(index_2))
-            table_template_name = template_table.args[0]
+            delay_template_table = liberty_util.create_delay_template_table(new_library, len(index_1), len(index_2))
+            delay_table_template_name = delay_template_table.args[0]
 
             # Create liberty timing tables.
             timing_tables = []
             for table_name in ['cell_rise', 'cell_fall', 'rise_transition', 'fall_transition']:
                 table = Group(
                     table_name,
-                    args=[table_template_name],
+                    args=[delay_table_template_name],
                 )
 
                 table.set_array('index_1', index_1)
                 table.set_array('index_2', index_2)
                 table.set_array('values', result[table_name] / conf.time_unit)
 
                 timing_tables.append(table)
@@ -1068,420 +1226,48 @@
                 attributes=timing_attributes,
                 groups=timing_tables
             )
 
             # Attach timing group to output pin group.
             output_pin_group.groups.append(timing_group)
 
-
-def characterize_flip_flop_output(
-        new_library: Group,
-        new_cell_group: Group,
-        conf: CharacterizationConfig,
-        cell_type: SingleEdgeDFF,
-        cell_conf: CellConfig,
-        related_pin_transition: np.ndarray,
-        input_transition_times: np.ndarray,
-        output_capacitances: np.ndarray,
-):
-    assert isinstance(cell_type, SingleEdgeDFF)
-
-    logger.info("Characterize single-edge triggered flip-flop.")
-
-    if related_pin_transition is None:
-        abort("Need to specify 'related-pin-transition' for the clock pin.")
-
-    # Create or update the 'ff' group.
-    ff_group = new_cell_group.get_groups('ff')
-    if not ff_group:
-        ff_group = Group('ff')
-        new_cell_group.groups.append(ff_group)
-
-    # Store content of 'ff' group.
-    ff_group.args = [str(cell_type.internal_state), str(cell_type.internal_state) + "_INV"]
-    ff_group.set_boolean_function('clocked_on', cell_type.clocked_on)
-    ff_group.set_boolean_function('next_state', cell_type.next_state)
-    if cell_type.async_preset:
-        ff_group.set_boolean_function('preset', cell_type.async_preset)
-    if cell_type.async_clear:
-        ff_group.set_boolean_function('clear', cell_type.async_clear)
-
-    # Find clock pin.
-    clock_signals = list(cell_type.clocked_on.atoms(sympy.Symbol))
-    if len(clock_signals) != 1:
-        logger.error(f"Expect exactly one clock signal. Got {clock_signals}")
-    clock_signal = clock_signals[0]
-    # Find clock polarity:
-    clock_edge_polarity = cell_type.clocked_on.subs({clock_signal: True})
-    clock_pin = str(clock_signal.name)
-
-    assert isinstance(clock_pin, str)
-
-    logger.info(f"Clock signal: {clock_pin}")
-    logger.info(f"Clock polarity: {'rising' if clock_edge_polarity else 'falling'}")
-
-    # Find preset/clear signals.
-    # Make sure preset/clear are disabled.
-    preset_condition = cell_type.async_preset
-    clear_condition = cell_type.async_clear
-    # Find a variable assignment such that neither preset nor clear is active.
-    no_preset_no_clear = list(satisfiable(~preset_condition & ~clear_condition, all_models=True))
-    for model in no_preset_no_clear:
-        logger.info(f"FF in normal operation mode when: {model}")
-    preset_clear_input = no_preset_no_clear[0]
-    if len(no_preset_no_clear) > 1:
-        logger.warning(f"Multiple possibilities found for disabling preset and clear. "
-                       f"Take the first one ({preset_clear_input}).")
-
-    # Find all data pins that are relevant for the internal state of the flip-flop.
-    data_in_pins = sorted(cell_type.next_state.atoms(sympy.Symbol))
-    logger.debug(f"Input pins relevant for internal state: {data_in_pins}")
-
-    assert isinstance(cell_type.internal_state,
-                      sympy.Symbol), "Internal flip-flop-state variable is not defined."
-
-    # Find all output pins that depend on the internal state.
-    data_out_pins: List[sympy.Symbol] = [name for name, output in cell_type.outputs.items()
-                                         if cell_type.internal_state in output.function.atoms()
-                                         ]
-    logger.debug(f"Output pins that depend on the internal state: {data_out_pins}")
-
-    
-    # Remember a clock pulse width which for sure samples a stable data signal.
-    clock_pulse_width_guess = 0
-
-    # TODO use this function to simplify the below code.
-    ## Find data input pins which can control the output pin.
-    #control_and_observe_pins = find_flipflop_state_control_and_observe_pins(cell_type, preset_clear_input)
-    #assert len(control_and_observe_pins) > 0, "No input pin found which can control the flip-flop state."
-    
-    
-    # Characterize setup/hold for each data pin.
-    for i, data_in_pin in enumerate(data_in_pins):
-        logger.info(f"Measure constraints of pin {data_in_pin} ({i}/{len(data_in_pins)}).")
-
-        # Find all assignments of the other data pins such that the data pin controls
-        # the internal state.
-        # Find values of the other pins such that:
-        #  next_state(data_in_pin=0, other_pins) != next_state(data_in_pin=1, other_pins)
-        next_state_0 = cell_type.next_state.subs({data_in_pin: False})
-        next_state_1 = cell_type.next_state.subs({data_in_pin: True})
-        models = list(satisfiable(next_state_0 ^ next_state_1, all_models=True))
-
-        for other_pin_values in models:
-            # Express the assignment of the other pins as a boolean formula.
-            # This will also be used as a 'when' statement in the liberty file.
-            when_other_inputs = sympy.And(*(pin if value else ~pin for pin, value in other_pin_values.items()))
-            logger.info(f"Measure constraints of pin {data_in_pin} when {when_other_inputs}.")
-
-            # Set static voltages of other input pins.
-            other_pin_values.update(preset_clear_input)
-            static_input_voltages = dict()
-            for pin, value in other_pin_values.items():
-                if not isinstance(pin, sympy.Symbol):
-                    continue
-                value = value == True
-                voltage = cell_conf.global_conf.supply_voltage if value else 0.0
-                pin = str(pin)
-                logger.debug(f"{pin} = {voltage} V")
-                static_input_voltages[pin] = voltage
-
-            # Find an output pin such that the internal state is observable.
-            observer_outputs = []  # Output pins that can observe the internal memory state.
-            for output_pin, output in cell_type.outputs.items():
-                function = output.function
-                # Substitute with constant input pins.
-                function = function.subs(other_pin_values)
-
-                # Compute the output for all values of the internal state and make sure it is different.
-                function0 = function.subs({cell_type.internal_state: False})
-                function1 = function.subs({cell_type.internal_state: True})
-                is_observable = not satisfiable(~(function0 ^ function1))  # Test if function0 != function1
-
-                logger.debug(f"Internal state {cell_type.internal_state} observable from output {output_pin} "
-                             f"when {other_pin_values}: {is_observable}")
-
-                if is_observable:
-                    observer_outputs.append(output_pin)
-
-            logger.debug(f"Internal state is observable from: {observer_outputs}")
-
-            if not observer_outputs:
-                # When the internal state is not observable we cannot measure constraints.
-                # Skip this combination.
-                logger.warning(
-                    f"Internal memory state {cell_type.internal_state} is not observable from any output "
-                    f"when {other_pin_values}. Skipping input combination.")
-                continue
-
-            # Take just one of the observer output pins.
-            data_out_pin = observer_outputs[0]
-            logger.debug(f"Output pin: {data_out_pin}")
-
-            # == Start characterization ==
-
-            # Convert from sympy.Symbol to string.
-            data_in_pin = str(data_in_pin)
-            data_out_pin = str(data_out_pin)
-
-            def find_min_clock_pulse_width(clock_pulse_polarity: bool, rising_data_edge: bool):
-                min_clock_pulse_width, delay = find_minimum_clock_pulse_width(
-                    cell_config=cell_conf,
-                    ff_clock_edge_polarity=clock_edge_polarity,
-                    clock_input=clock_pin,
-                    data_in=data_in_pin,
-                    data_out=data_out_pin,
-                    setup_time=2e-9,  # Choose a reasonably large setup time.
-                    clock_pulse_polarity=clock_pulse_polarity,
-                    rising_data_edge=rising_data_edge,
-                    clock_rise_time=10e-12,  # TODO: Something fails when 0.
-                    clock_fall_time=10e-12,  # TODO: How to choose this?
-                    output_load_capacitances={data_out_pin: 0},
-                    clock_pulse_width_guess=100e-12,
-                    max_delay_estimation=1e-7,
-                    static_input_voltages=static_input_voltages,
-                )
-                logger.debug(f'min_clock_pulse_width = {min_clock_pulse_width}, delay = {delay}')
-                return min_clock_pulse_width, delay
-
-            # Find the minimal clock pulse for negative and positive pulses.
-            # For each pulse type inspect rising and falling data edges.
-            logger.info(f"Find minimal clock pulse width ({clock_pin}).")
-            min_pulse_width_low, _delay = max(find_min_clock_pulse_width(False, False),
-                                              find_min_clock_pulse_width(False, True))
-            logger.info(f"min_pulse_width_low = {min_pulse_width_low} s")
-            min_pulse_width_high, _delay = max(find_min_clock_pulse_width(True, False),
-                                               find_min_clock_pulse_width(True, True))
-            logger.info(f"min_pulse_width_high = {min_pulse_width_high} s")
+            # Create template tables.
+            power_template_table = liberty_util.create_power_template_table(new_library, len(index_1), len(index_2))
+            power_table_template_name = power_template_table.args[0]
             
-            # Find the shortest clock pulse width which samles a stable data signal for all cases.
-            clock_pulse_width_guess = max(clock_pulse_width_guess, min_pulse_width_low, min_pulse_width_high)
-
-            # Write information on clock pin to liberty.
-            # TODO: minimum pulse width is potentially computed for many different input combinations. Take min/max of them! (Now just the last one will be stored)
-            clock_pin_group = new_cell_group.get_group('pin', clock_pin)
-            clock_pin_group['clock'] = 'true'
-            clock_pin_group['min_pulse_width_high'] = min_pulse_width_high / conf.time_unit
-            clock_pin_group['min_pulse_width_low'] = min_pulse_width_low / conf.time_unit
-
-            # Find setup and hold times.
-            result = characterize_flip_flop_setup_hold(
-                cell_conf=cell_conf,
-                data_in_pin=data_in_pin,
-                data_out_pin=data_out_pin,
-                clock_pin=clock_pin,
-                clock_edge_polarity=clock_edge_polarity,
-
-                constrained_pin_transition=input_transition_times,
-                related_pin_transition=related_pin_transition,
-
-                output_load_capacitance=0,  # TODO: Is it accurate to assume zero output load?
-
-                static_input_voltages=static_input_voltages
-            )
-
-            # Get the table indices.
-            # TODO: get correct index/variable mapping from liberty file.
-            index_1 = result['related_pin_transition'] / conf.time_unit
-            index_2 = result['constrained_pin_transition'] / conf.time_unit
-            # TODO: remember all necessary templates and create template tables.
-
-            input_pin_group = new_cell_group.get_group('pin', data_in_pin)
-
-            clock_edge = 'rising' if clock_edge_polarity else 'falling'
-
-            # Add setup/hold information to the liberty pin group.
-            for constraint_type in ['hold', 'setup']:
-                template_table = liberty_util.create_constraint_template_table(
-                    new_library, constraint_type, len(index_1), len(index_2)
-                )
-                table_template_name = template_table.args[0]
-
-                rise_constraint = Group('rise_constraint', args=[table_template_name])
-                rise_constraint.set_array('index_1', index_1)
-                rise_constraint.set_array('index_2', index_2)
-                rise_constraint.set_array(
-                    'values',
-                    result[f'{constraint_type}_rise_constraint'] / conf.time_unit
-                )
-
-                fall_constraint = Group('fall_constraint', args=[table_template_name])
-                fall_constraint.set_array('index_1', index_1)
-                fall_constraint.set_array('index_2', index_2)
-                fall_constraint.set_array(
-                    'values',
-                    result[f'{constraint_type}_fall_constraint'] / conf.time_unit
-                )
-
-                timing_group = Group(
-                    'timing',
-                    attributes=[
-                        Attribute('timing_type', f'{constraint_type}_{clock_edge}'),
-                        Attribute('related_pin', EscapedString(clock_pin))
-                    ],
-                    groups=[rise_constraint, fall_constraint]
+            # Create liberty power tables.
+            power_tables = []
+            for table_name in ['rise_power', 'fall_power']:
+                table = Group(
+                    table_name,
+                    args=[power_table_template_name],
                 )
 
-                if len(when_other_inputs.atoms(sympy.Symbol)) > 0:
-                    timing_group.set_boolean_function('when', when_other_inputs)
-
-                input_pin_group.groups.append(timing_group)
-
-    
-    # Measure clock-to-output delays.
-    for data_out_pin in data_out_pins:
-        
-        logger.info(f"Measure clock-to-output delay for output '{data_out_pin}'")
-        
-        output_function = cell_type.outputs[data_out_pin].function
-        logger.info(f"Output function: {output_function}")
-        
-        # Convert output pin to string
-        data_out_pin_name = str(data_out_pin)
-    
-        output_pin_group = new_cell_group.get_group('pin', data_out_pin_name)
-        output_pin_group.set_boolean_function('function', output_function)
-        related_pin = clock_pin
-        
-        # Find data input pins which can control the output pin.
-        possible_input_pins = find_flipflop_state_control_and_observe_pins(cell_type, preset_clear_input)
-
-        assert len(possible_input_pins) > 0, "No input pin found which can control the flip-flop state."
-            
-        # Select an input pin and a combination of other input values such that the input pin controls output of the flip-flop.
-        data_in_pin, static_input_values, observer_outputs = possible_input_pins[0]
-
-        assert data_out_pin in observer_outputs, f"Flip-flop state is not observable from {data_out_pin} when {static_input_values}."
-
-        # Translate logic values to voltages.
-        static_input_voltages = {
-            pin: value * cell_conf.global_conf.supply_voltage 
-            for pin, value in static_input_values.items()
-        }
-
-        logger.info(f"Use input pin {data_in_pin} with other pin values {static_input_voltages}")
-     
-        for clock_transition_time in related_pin_transition:
-            for output_capacitance in output_capacitances:
-        
-                output_load_capacitances = {data_out_pin_name: output_capacitance} 
-                
-                for data_edge_polarity in [False, True]:
-                    
-                    # Choose setup and hold time to be used for the delay measurement.
-                    settings = {
-                        CalcMode.BEST: (1e-9, 1e-9), # Use large setup and hold times. This leads to shorter propagation time.
-                        CalcMode.WORST: (1e-9, 1e-9), # Use short setup and hold times. This leads to longer propagation times.
-                        CalcMode.TYPICAL: (1e-9, 1e-9),
-                    }
-                    
-                    (setup_time, hold_time) = settings[conf.timing_corner]
-                    
-                    clock_cycle_hint = clock_pulse_width_guess * 2 # Choose a big-enough clock pulse such that data is sampled for sure.
-        
-                    data_transition_time = 1e-13 # TODO
-                    
-                    delay, slew_time = measure_clock_to_output_delay(
-                        cell_conf,
-                        data_in_pin,
-                        data_out_pin_name,
-                        clock_pin,
-                        clock_edge_polarity,
-                        data_edge_polarity,
-                        output_load_capacitances,
-                        clock_transition_time,
-                        data_transition_time,
-                        setup_time,
-                        hold_time,
-                        clock_cycle_hint,
-                        static_input_voltages
-                    )
-                    print(f"delay = {delay}")
-        
-        #timing_group = Group(
-        #    'timing',
-        #    attributes={
-        #        'timing_type': [f'rising_edge'],
-        #        'related_pin': [EscapedString(related_pin)]
-        #    },
-        #    groups=[cell_rise, cell_fall]
-        #)
-
-def find_flipflop_state_control_and_observe_pins(
-    cell_type: SingleEdgeDFF,
-    other_inputs: Dict[sympy.Symbol, sympy.Symbol]
-) -> List[Tuple[str, Dict[str, bool]]]:
-    """
-    Find data input pins which control the state of the flip-flop.
-
-
-    Returns a list of pins which can control the flip-flop state together with 
-    1) an assignment of other input values (clear, preset, ...) such that the input pin becomes controlling
-    2) a list of output pins which allow to observe the internal state with the given other input values
-    """
+                table.set_array('index_1', index_1)
+                table.set_array('index_2', index_2)
+                table.set_array('values', result[table_name] / conf.energy_unit)
 
-    assert isinstance(cell_type, SingleEdgeDFF), "cell_type must be a SingleEdgeDFF"
-    
-    # Find all data pins that are relevant for the internal state of the flip-flop.
-    data_in_pins = sorted(cell_type.next_state.atoms(sympy.Symbol))
-    logger.debug(f"Input pins relevant for internal state: {data_in_pins}")
-
-    # Find data input pins which can control the output pin.
-    controlling_input_pins = []
-    for data_in_pin in data_in_pins:
-    
-        # Find all assignments of the other data pins such that the data pin controls
-        # the internal state.
-        # Find values of the other pins such that:
-        #  next_state(data_in_pin=0, other_pins) != next_state(data_in_pin=1, other_pins)
-        next_state_0 = cell_type.next_state.subs({data_in_pin: False})
-        next_state_1 = cell_type.next_state.subs({data_in_pin: True})
-        models = list(satisfiable(next_state_0 ^ next_state_1, all_models=True))
-
-        for other_pin_values in models:
-            # Express the assignment of the other pins as a boolean formula.
-            # This will also be used as a 'when' statement in the liberty file.
-            when_other_inputs = sympy.And(*(pin if value else ~pin for pin, value in other_pin_values.items()))
-            logger.info(f"Measure clock-to-output delay with data input {data_in_pin} when {when_other_inputs}.")
+                power_tables.append(table)
 
-            # Set static voltages of other input pins.
-            other_pin_values.update(other_inputs)
+            power_attributes = [
+                Attribute('related_pin', EscapedString(related_pin)),
+            ]
             
-            logger.debug(f"Pin {data_in_pin} controls the flip-flop state when: {other_pin_values}")
+            internal_power_group = Group(
+                'internal_power',
+                attributes=power_attributes,
+                groups=power_tables
+            )
             
-
-            static_input_voltages = dict()
-            for pin, value in other_pin_values.items():
-                if not isinstance(pin, sympy.Symbol):
-                    continue
-                value = value == True
-                pin = str(pin)
-                logger.debug(f"{pin} = {value} V")
-                static_input_voltages[pin] = value
-                
-            # Find an output pin such that the internal state is observable.
-            observer_outputs = []  # Output pins that can observe the internal memory state.
-            for output_pin, output in cell_type.outputs.items():
-                function = output.function
-                # Substitute with constant input pins.
-                function = function.subs(other_pin_values)
-
-                # Compute the output for all values of the internal state and make sure it is different.
-                function0 = function.subs({cell_type.internal_state: False})
-                function1 = function.subs({cell_type.internal_state: True})
-                is_observable = not satisfiable(~(function0 ^ function1))  # Test if function0 != function1
-
-                logger.debug(f"Internal state {cell_type.internal_state} observable from output {output_pin} "
-                             f"when {other_pin_values}: {is_observable}")
-
-                if is_observable:
-                    observer_outputs.append(output_pin)
-
-            logger.debug(f"Internal state is observable from: {observer_outputs}")
-
-            # Remember the pin which controls the internal state and the the required
-            # voltages at the other pins.
-            controlling_input_pins.append((str(data_in_pin), static_input_voltages, observer_outputs))
-
-    return controlling_input_pins
-
+            # Attach group to output pin group.
+            output_pin_group.groups.append(internal_power_group)
+    
+def _transistors2multigraph(transistors) -> nx.MultiGraph:
+    """ Create a graph representing the transistor network.
+        Each edge corresponds to a transistor, each node to a net.
+    """
+    G = nx.MultiGraph()
+    for t in transistors:
+        G.add_edge(t.source_net, t.drain_net, (t.gate_net, t.channel_type))
+    assert nx.is_connected(G)
+    return G
```

### Comparing `lctime-0.0.23/src/lctime/characterization/main_sp2bool.py` & `lctime-0.0.24/src/lctime/characterization/main_sp2bool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Copyright (c) 2019 Thomas Kramer.
-# SPDX-FileCopyrightText: 2022 Thomas Kramer <code@tkramer.ch>
-#
+# SPDX-FileCopyrightText: 2019-2024 Thomas Kramer <code@tkramer.ch>
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 from ..logic import functional_abstraction
 from ..logic import seq_recognition
 from . import util
 
 import argparse
```

### Comparing `lctime-0.0.23/src/lctime/characterization/ngspice_simulation.py` & `lctime-0.0.24/src/lctime/characterization/ngspice_simulation.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/characterization/ngspice_subprocess.py` & `lctime-0.0.24/src/lctime/characterization/ngspice_subprocess.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/characterization/piece_wise_linear.py` & `lctime-0.0.24/src/lctime/characterization/piece_wise_linear.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/characterization/test_ngspice_shared.py` & `lctime-0.0.24/src/lctime/characterization/test_ngspice_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 #
 #     print(np.array(analysis['a']))
 #     plt.plot(analysis.time, analysis['input'], 'x-')
 #     plt.plot(analysis.time, np.array(analysis['a']), 'x-')
 #     plt.show()
 
 
-def test3():
+def _test3():
 
     netlist = r""".title Input capacitance measurement for pin "A"
 .include /home/kramert/unison/local/blackbird/git/librecell-examples/librecell_invx1_example/gpdk45nm.m
 .include /home/kramert/unison/local/blackbird/git/librecell-examples/librecell_invx1_example/INVX1.pex.netlist
 Xcircuit_unter_test A GND VDD Y INVX1
 Vpower_vdd VDD GND 1.1V
 Isrc_A GND A 10000nA
@@ -143,8 +143,8 @@
     if plot_name == 'const':
         raise Exception("Simulation failed.")
     plot = ngs.plot(None, plot_name)
     analysis = plot.to_analysis()
 
     plt.plot(analysis.time, analysis['y'], 'x-')
     plt.plot(analysis.time, np.array(analysis['a']), 'x-')
-    plt.show()
+    # Disable for automatic tests: plt.show()
```

### Comparing `lctime-0.0.23/src/lctime/characterization/test_ngspice_subprocess.py` & `lctime-0.0.24/src/lctime/characterization/test_ngspice_subprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import os
 import asyncio
 import logging
 import threading, queue
 import time
 from typing import List
 
+from .ngspice_subprocess import NgSpiceInteractive
+
 
 def test_simple_simulation():
     """Run a simple transient simulation in a ngspice subprocess and retreive the results from a file."""
 
     sim_file = tempfile.mktemp()
     sim_output_file = tempfile.mktemp()
 
@@ -60,15 +62,15 @@
     y_time = data[:, 2]
     y = data[:, 3]
 
     assert all(a_time == y_time)
 
     plt.plot(a_time, a, 'x-')
     plt.plot(y_time, y, 'x-')
-    plt.show()
+    # Disable for automatic tests: plt.show()
 
     os.remove(sim_output_file)
     os.remove(sim_file)
 
 
 def test_interactive_subprocess():
     import subprocess
```

### Comparing `lctime-0.0.23/src/lctime/characterization/timing_combinatorial.py` & `lctime-0.0.24/src/lctime/characterization/timing_combinatorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,29 +211,31 @@
                 time, voltages, currents = simulate_cell(
                     cell_name=cell_conf.cell_name,
                     cell_ports=ports,
                     input_voltages=input_voltages,
                     initial_voltages=initial_node_voltages,
                     breakpoint_statements=breakpoint_statements,
                     output_voltages=[related_pin, output_pin],
-                    output_currents=[cell_conf.supply_net],
+                    output_currents=[cell_conf.supply_net, related_pin],
                     simulation_file=sim_file,
                     simulation_output_file=sim_output_file,
                     max_simulation_time=time_max,
                     simulation_title=simulation_title,
                     temperature=cfg.temperature,
                     output_load_capacitances={output_pin: output_cap},
                     time_step=cfg.time_step,
                     setup_statements=setup_statements,
                     ground_net=cell_conf.ground_net,
                     debug=cfg.debug,
                 )
 
                 # Retrieve data.
-                supply_current = currents[cell_conf.supply_net]
+                supply_current = - currents[cell_conf.supply_net]
+                gate_current = - currents[related_pin]
+                
                 input_voltage = voltages[related_pin]
                 output_voltage = voltages[output_pin]
 
                 if cfg.debug_plots:
                     logger.debug("Create plot of waveforms: {}".format(sim_plot_file))
                     import matplotlib
                     matplotlib.use('Agg')
@@ -245,17 +247,24 @@
                     plt.plot(time, supply_current, label='supply current')
                     plt.legend()
                     plt.savefig(sim_plot_file)
                     plt.close()
 
                 # TODO: What unit does rise_power/fall_power have in liberty files???
                 # Is it really power or energy?
-                switching_power = np.mean(supply_current * vdd)
-                switching_energy = switching_power * (time[-1] - time[0])
-
+                dt = time[-1] - time[0]
+                assert dt > 0.
+                gate_energy = np.mean(gate_current * input_voltage) * dt
+                supply_energy = np.mean(supply_current * vdd) * dt
+                logger.debug(f"switching energy (supply): {supply_energy}")
+                logger.debug(f"switching energy (gate): {gate_energy}")
+
+                switching_energy = gate_energy + supply_energy
+                assert switching_energy >= 0., "switching power consumption through power supply is negative"
+                
                 v_thresh = 0.5 * vdd
 
                 # Get input signal before switching and after.
                 input_a = input_voltage[0] > v_thresh
                 input_b = input_voltage[-1] > v_thresh
                 assert input_a != input_b
```

### Comparing `lctime-0.0.23/src/lctime/characterization/timing_sequential.py` & `lctime-0.0.24/src/lctime/characterization/timing_sequential.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/characterization/util.py` & `lctime-0.0.24/src/lctime/characterization/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,18 @@
         """
         Time unit used in the liberty file.
         """
         self.capacitance_unit: float = 1e-12 # [F]
         """
         Capacitance unit used in the liberty file.
         """
+        self.energy_unit: float = 1e-12 # [pJ]
+        """
+        Energy unit used in the liberty file.
+        """
 
     def get_units_from_liberty(self, library: Group):
         """
         Read units from liberty data.
         """
         # Units
         # TODO: choose correct unit from liberty file
```

### Comparing `lctime-0.0.23/src/lctime/lccommon/data_types.py` & `lctime-0.0.24/src/lctime/lccommon/data_types.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/lccommon/net_util.py` & `lctime-0.0.24/src/lctime/lccommon/net_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Copyright (c) 2019 Thomas Kramer.
-# SPDX-FileCopyrightText: 2022 Thomas Kramer <code@tkramer.ch>
+# SPDX-FileCopyrightText: 2019-2023 Thomas Kramer <code@tkramer.ch>
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 from ..lccommon.data_types import *
 import networkx as nx
 from typing import Tuple, List, Set, Iterable, Dict
 import klayout.db as db
```

### Comparing `lctime-0.0.23/src/lctime/lccommon/spice_parser.py` & `lctime-0.0.24/src/lctime/lccommon/spice_parser.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/liberty/merge.py` & `lctime-0.0.24/src/lctime/liberty/merge.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/liberty/util.py` & `lctime-0.0.24/src/lctime/liberty/util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/liberty/visualize.py` & `lctime-0.0.24/src/lctime/liberty/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     y_label = template['variable_1']
 
     z_label = "[{}]".format(time_unit)
 
     plot3d(x_axis, y_axis, z_data, x_label=x_label, y_label=y_label, z_label=z_label)
 
 
-def test_plot_nldm():
+def _test_plot_nldm():
     import os.path
     lib_file = os.path.join(os.path.dirname(__file__), '../../test_data/freepdk45/gscl45nm.lib')
 
     data = open(lib_file).read()
 
     library = parse_liberty(data)
```

### Comparing `lctime-0.0.23/src/lctime/logic/cmos_sim.py` & `lctime-0.0.24/src/lctime/logic/cmos_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from itertools import product
 from typing import Any, Dict, List, Iterable, Tuple
 from enum import Enum
 
 import sympy
 from sympy.logic import SOPform
 
-from lccommon.data_types import ChannelType
+from ..lccommon.data_types import ChannelType
 
 
 class Signal(Enum):
     LOW = 0
     HIGH = 1
     X = 2
     Z = 3
```

### Comparing `lctime-0.0.23/src/lctime/logic/cmos_synth.py` & `lctime-0.0.24/src/lctime/logic/cmos_synth.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/logic/functional_abstraction.py` & `lctime-0.0.24/src/lctime/logic/functional_abstraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,22 @@
         elif value_formula:
             minterms.append(inputs)
 
     f = boolalg.SOPform(variables=all_vars, minterms=minterms, dontcares=dont_cares)
 
     return f
 
+def test_simplify_with_assumption():
+
+    a, b, c = sympy.symbols("a b c")
+    f = a & b & c
+    assumption = a & b
+
+    s = simplify_with_assumption(assumption, f)
+    assert s == c
 
 def bool_equals(f1: boolalg.Boolean, f2: boolalg.Boolean) -> bool:
     """
     Check equality of two boolean formulas.
     :param f1:
     :param f2:
     :return:
```

### Comparing `lctime-0.0.23/src/lctime/logic/graph_enumeration.py` & `lctime-0.0.24/src/lctime/logic/graph_enumeration.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/logic/seq_recognition.py` & `lctime-0.0.24/src/lctime/logic/seq_recognition.py`

 * *Files 11% similar despite different names*

```diff
@@ -508,7 +508,87 @@
     extractors = [LatchExtractor(), DFFExtractor()]
 
     for ex in extractors:
         result = ex.extract(c)
         if result is not None:
             return result
     return None
+
+def find_flipflop_state_control_and_observe_pins(
+    cell_type: SingleEdgeDFF,
+    other_inputs: Dict[sympy.Symbol, sympy.Symbol]
+) -> List[Tuple[str, Dict[str, bool]]]:
+    """
+    Find data input pins which control the state of the flip-flop.
+
+
+    Returns a list of pins which can control the flip-flop state together with 
+    1) an assignment of other input values (clear, preset, ...) such that the input pin becomes controlling
+    2) a list of output pins which allow to observe the internal state with the given other input values
+    """
+
+    assert isinstance(cell_type, SingleEdgeDFF), "cell_type must be a SingleEdgeDFF"
+    
+    # Find all data pins that are relevant for the internal state of the flip-flop.
+    data_in_pins = sorted(cell_type.next_state.atoms(sympy.Symbol))
+    logger.debug(f"Input pins relevant for internal state: {data_in_pins}")
+
+    # Find data input pins which can control the output pin.
+    controlling_input_pins = []
+    for data_in_pin in data_in_pins:
+    
+        # Find all assignments of the other data pins such that the data pin controls
+        # the internal state.
+        # Find values of the other pins such that:
+        #  next_state(data_in_pin=0, other_pins) != next_state(data_in_pin=1, other_pins)
+        next_state_0 = cell_type.next_state.subs({data_in_pin: False})
+        next_state_1 = cell_type.next_state.subs({data_in_pin: True})
+        models = list(satisfiable(next_state_0 ^ next_state_1, all_models=True))
+
+        for other_pin_values in models:
+            # Express the assignment of the other pins as a boolean formula.
+            # This will also be used as a 'when' statement in the liberty file.
+            when_other_inputs = sympy.And(*(pin if value else ~pin for pin, value in other_pin_values.items()))
+            logger.info(f"Measure clock-to-output delay with data input {data_in_pin} when {when_other_inputs}.")
+
+            # Set static voltages of other input pins.
+            other_pin_values.update(other_inputs)
+            
+            logger.debug(f"Pin {data_in_pin} controls the flip-flop state when: {other_pin_values}")
+            
+
+            static_input_voltages = dict()
+            for pin, value in other_pin_values.items():
+                if not isinstance(pin, sympy.Symbol):
+                    continue
+                value = value == True
+                pin = str(pin)
+                logger.debug(f"{pin} = {value} V")
+                static_input_voltages[pin] = value
+                
+            # Find an output pin such that the internal state is observable.
+            observer_outputs = []  # Output pins that can observe the internal memory state.
+            for output_pin, output in cell_type.outputs.items():
+                function = output.function
+                # Substitute with constant input pins.
+                function = function.subs(other_pin_values)
+
+                # Compute the output for all values of the internal state and make sure it is different.
+                function0 = function.subs({cell_type.internal_state: False})
+                function1 = function.subs({cell_type.internal_state: True})
+                is_observable = not satisfiable(~(function0 ^ function1))  # Test if function0 != function1
+
+                logger.debug(f"Internal state {cell_type.internal_state} observable from output {output_pin} "
+                             f"when {other_pin_values}: {is_observable}")
+
+                if is_observable:
+                    observer_outputs.append(output_pin)
+
+            logger.debug(f"Internal state is observable from: {observer_outputs}")
+
+            # Remember the pin which controls the internal state and the the required
+            # voltages at the other pins.
+            controlling_input_pins.append((str(data_in_pin), static_input_voltages, observer_outputs))
+
+    return controlling_input_pins
+
+
```

### Comparing `lctime-0.0.23/src/lctime/logic/smt_4value_logic_scratch.py` & `lctime-0.0.24/src/lctime/logic/smt_4value_logic_scratch.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/logic/types.py` & `lctime-0.0.24/src/lctime/logic/types.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/logic/util.py` & `lctime-0.0.24/src/lctime/logic/util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime/transistor_sizing/width_opt.py` & `lctime-0.0.24/src/lctime/transistor_sizing/width_opt.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.23/src/lctime.egg-info/PKG-INFO` & `lctime-0.0.24/src/lctime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctime
-Version: 0.0.23
+Version: 0.0.24
 Summary: CMOS standard-cell characterization kit.
 Author-email: "T. Kramer" <code@tkramer.ch>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://codeberg.org/librecell/lctime
 Project-URL: Repository, https://codeberg.org/librecell/lctime
 Project-URL: Issue Tracker, https://codeberg.org/librecell/lctime/issues
 Keywords: cmos,cell,characterization,vlsi,asic
```

### Comparing `lctime-0.0.23/src/lctime.egg-info/SOURCES.txt` & `lctime-0.0.24/src/lctime.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 src/lctime.egg-info/PKG-INFO
 src/lctime.egg-info/SOURCES.txt
 src/lctime.egg-info/dependency_links.txt
 src/lctime.egg-info/entry_points.txt
 src/lctime.egg-info/requires.txt
 src/lctime.egg-info/top_level.txt
 src/lctime/characterization/__init__.py
+src/lctime/characterization/flipflop.py
 src/lctime/characterization/input_capacitance.py
+src/lctime/characterization/leakage_power.py
 src/lctime/characterization/main_lctime.py
 src/lctime/characterization/main_sp2bool.py
 src/lctime/characterization/ngspice_simulation.py
 src/lctime/characterization/ngspice_subprocess.py
 src/lctime/characterization/piece_wise_linear.py
 src/lctime/characterization/test_ngspice_shared.py
 src/lctime/characterization/test_ngspice_subprocess.py
```

