# Comparing `tmp/MethodicConfigurator-0.1.9.tar.gz` & `tmp/methodicconfigurator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MethodicConfigurator-0.1.9.tar", last modified: Tue Apr  9 14:33:37 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.2.0.tar", last modified: Sun Apr 14 23:46:41 2024, max compression
```

## Comparing `MethodicConfigurator-0.1.9.tar` & `methodicconfigurator-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.173461 MethodicConfigurator-0.1.9/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27842 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/annotate_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17164 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    42536 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    60612 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/frontend_tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/tempcal_IMU.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.173461 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:33:34.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:46:41.733977 methodicconfigurator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:46:41.729977 methodicconfigurator-0.2.0/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27867 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6337 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20449 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26357 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/backend_mavftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8062 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/frontend_tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15843 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18931 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/tempcal_IMU.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:46:41.729977 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 23:46:41.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:46:38.000000 methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-14 23:46:41.733977 methodicconfigurator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:46:41.733977 methodicconfigurator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-14 23:46:16.000000 methodicconfigurator-0.2.0/setup.py
```

### Comparing `MethodicConfigurator-0.1.9/LICENSE.md` & `methodicconfigurator-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/annotate_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, Par):
             return self.value == other.value and self.comment == other.comment
         return False
 
     @staticmethod
-    def load_param_file_into_dict(param_file: str) -> Dict[str, 'Par']:
+    def load_param_file_into_dict(param_file: str) -> Dict[str, 'Par']:  # pylint: disable=R0912
         """
         Loads an ArduPilot parameter file into a dictionary with name, value pairs.
 
         Parameters:
         parm_file (str): The name of the parameter file to load.
 
         Returns:
@@ -509,16 +509,16 @@
         raise SystemExit("Invalid parameter name")
     if param_len > PARAM_NAME_MAX_LEN:
         logging.critical("Too long parameter name on line %d in file %s", line_nr, filename)
         raise SystemExit("Too long parameter name")
     return param_name
 
 
-def update_parameter_documentation(doc: Dict[str, Any], target: str = '.', sort_type: str = 'none',
-                                   param_default_dict: Optional[Dict] = None) -> None:  # pylint: disable=R0912, R0914, R0915
+def update_parameter_documentation(doc: Dict[str, Any], target: str = '.',  # pylint: disable=R0912, R0914, R0915
+                                   sort_type: str = 'none', param_default_dict: Optional[Dict] = None) -> None:
     """
     Updates the parameter documentation in the target file or in all *.param,*.parm files of the target directory.
 
     This function iterates over all the ArduPilot parameter files in the target directory or file.
     For each file, it DELETES all comments that start at the beginning of a line, optionally sorts the
     parameter names and checks if the parameter name is in the dictionary of parameter documentation.
     If it is, it prefixes the line with comment derived from the dictionary element.
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python3
 
 '''
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
-AP_FLAKE8_CLEAN
-
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 import argparse
 from logging import basicConfig as logging_basicConfig
@@ -18,16 +16,21 @@
 from logging import warning as logging_warning
 from logging import error as logging_error
 from os import getcwd as os_getcwd
 from sys import exit as sys_exit
 
 from backend_filesystem import LocalFilesystem
 from backend_flightcontroller import FlightController
-from frontend_tkinter import show_no_param_files_error
-from frontend_tkinter import show_no_connection_error
+
+from frontend_tkinter_connection_selection import ConnectionSelectionWindow
+
+from frontend_tkinter_directory_selection import VehicleDirectorySelectionWindow
+
+from component_editor import JsonEditorApp
+
 from frontend_tkinter import gui
 
 from version import VERSION
 
 
 def argument_parser():
     """
@@ -47,78 +50,86 @@
                                      'When "Write Selected to FC" is clicked, it writes the selected parameters to the '
                                      'flight controller. '
                                      'When "Skip" is pressed, it skips to the next intermediate parameter file. '
                                      'The process gets repeated for each intermediate parameter file.')
     parser.add_argument('--device',
                         type=str,
                         default="",
-                        help='MAVLink connection string to the flight controller. Defaults to autodetection')
+                        help='MAVLink connection string to the flight controller. Defaults to autodetection'
+                        )  # pylint: disable=R0801
+    parser.add_argument('-r', '--reboot-time',
+                        type=int,
+                        default=7,
+                        help='Flight controller reboot time. '
+                        'Default is %(default)s')  # pylint: disable=R0801
+    parser.add_argument('-t', '--vehicle-type',
+                        choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
+                                 'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL'],
+                        default='ArduCopter',
+                        help='The type of the vehicle. Defaults to ArduCopter')  # pylint: disable=R0801
     parser.add_argument('--vehicle-dir',
                         type=str,
                         default=os_getcwd(),
                         help='Directory containing vehicle-specific intermediate parameter files. '
-                        'Defaults to the current working directory')
+                        'Defaults to the current working directory')  # pylint: disable=R0801
     parser.add_argument('--n',
                         type=int,
                         default=0,
                         help='Start directly on the nth intermediate parameter file (skips previous files). '
-                        'Default is %(default)s')
+                        'Default is %(default)s')  # pylint: disable=R0801
     parser.add_argument('--loglevel',
                         type=str,
                         default='INFO',
                         choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
-                        help='Logging level (default is INFO).')
-    parser.add_argument('-r', '--reboot-time',
-                        type=int,
-                        default=7,
-                        help='Flight controller reboot time. '
-                        'Default is %(default)s')
-    parser.add_argument('-t', '--vehicle-type',
-                        choices=['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
-                                 'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL'],
-                        default='ArduCopter',
-                        help='The type of the vehicle. Defaults to ArduCopter',
-                        )
+                        help='Logging level (default is INFO).')  # pylint: disable=R0801
     parser.add_argument('-v', '--version',
                         action='version',
                         version=f'%(prog)s {VERSION}',
-                        help='Display version information and exit.',
-                        )
-    return parser.parse_args()
+                        help='Display version information and exit.')  # pylint: disable=R0801
+    return parser.parse_args()   # pylint: disable=R0801
 
 
 if __name__ == "__main__":
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
     # Connect to the flight controller and read the parameters
     flight_controller = FlightController(args.reboot_time)
 
     error_str = flight_controller.connect(args.device)
     if error_str:
         logging_error(error_str)
-        show_no_connection_error(error_str)
+        conn_sel_window = ConnectionSelectionWindow(flight_controller, error_str)
+        conn_sel_window.root.mainloop()
 
     local_filesystem = LocalFilesystem(args.vehicle_dir, args.vehicle_type)
 
     # Get the list of intermediate parameter files files that will be processed sequentially
     files = list(local_filesystem.file_parameters.keys())
 
+    if not files:
+        logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
+        vehicle_dir_window = VehicleDirectorySelectionWindow(local_filesystem)
+        vehicle_dir_window.root.mainloop()
+
+   # Get the list of intermediate parameter files files that will be processed sequentially
+    files = list(local_filesystem.file_parameters.keys())
+
     start_file = None  # pylint: disable=invalid-name
     if files:
         # Determine the starting file based on the --n command line argument
         start_file_index = min(args.n, len(files) - 1) # Ensure the index is within the range of available files
         if start_file_index != args.n:
             logging_warning("Starting file index %s is out of range. Starting with file %s instead.",
                             args.n, files[start_file_index])
         start_file = files[start_file_index]
-    else:
-        logging_error("No intermediate parameter files found in %s.", args.vehicle_dir)
-        show_no_param_files_error(args.vehicle_dir)
+
+    app = JsonEditorApp(VERSION, local_filesystem)
+    app.root.mainloop()
 
     # Call the GUI function with the starting intermediate parameter file
     gui(start_file, flight_controller, local_filesystem, VERSION)
 
     # Close the connection to the flight controller
-    flight_controller.close_connection()
+    flight_controller.disconnect()
     sys_exit(0)
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/backend_filesystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 #!/usr/bin/env python3
 
 '''
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
-AP_FLAKE8_CLEAN
-
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 from os import path as os_path
+from os import getcwd as os_getcwd
 from os import listdir as os_listdir
+from os import makedirs as os_makedirs
+from os import sep as os_sep
+
+from shutil import copy2 as shutil_copy2
+from shutil import copytree as shutil_copytree
+
 from re import compile as re_compile
+from re import match as re_match
+from re import escape as re_escape
+
 # from sys import exit as sys_exit
 # from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
+
 from json import load as json_load
+from json import dump as json_dump
+from json import JSONDecodeError
+
 from typing import Dict
 from typing import List
 from typing import Tuple
+
 from zipfile import ZipFile
+
 from annotate_params import BASE_URL, PARAM_DEFINITION_XML_FILE, Par
 from annotate_params import get_xml_data
 from annotate_params import create_doc_dict
 from annotate_params import format_columns
 from annotate_params import split_into_lines
 from annotate_params import update_parameter_documentation
 
@@ -50,15 +64,15 @@
 
     Returns:
     - bool: True if the difference is within the tolerance, False otherwise.
     """
     return abs(x - y) <= atol + (rtol * abs(y))
 
 
-class LocalFilesystem:
+class LocalFilesystem:  # pylint: disable=too-many-instance-attributes, too-many-public-methods
     """
     A class to manage local filesystem operations for the ArduPilot methodic configurator.
 
     This class provides methods for initializing and re-initializing the filesystem context,
     reading parameters from files, and handling file documentation. It is designed to simplify
     the interaction with the local filesystem for managing ArduPilot configuration files.
 
@@ -68,22 +82,22 @@
         file_documentation_filename (str): The name of the file containing documentation for the configuration files.
         file_documentation (dict): A dictionary containing the file documentation.
         file_parameters (dict): A dictionary of parameters read from intermediate parameter files.
         param_default_dict (dict): A dictionary of default parameter values.
         doc_dict (dict): A dictionary containing documentation for each parameter.
     """
     def __init__(self, vehicle_dir: str, vehicle_type: str):
-        self.vehicle_dir = vehicle_dir
-        self.vehicle_type = vehicle_type
-        self.re_init(vehicle_dir, vehicle_type)
+        self.file_documentation_filename = "file_documentation.json"
+        self.vehicle_components_json_filename = "vehicle_components.json"
+        if vehicle_dir is not None:
+            self.re_init(vehicle_dir, vehicle_type)
 
     def re_init(self, vehicle_dir: str, vehicle_type: str):
         self.vehicle_dir = vehicle_dir
         self.vehicle_type = vehicle_type
-        self.file_documentation_filename = "file_documentation.json"
         self.file_documentation = {}
         self.param_default_dict = {}
         self.doc_dict = {}
 
         # Read intermediate parameters from files
         self.file_parameters = self.read_params_from_files()
         if not self.file_parameters:
@@ -112,19 +126,17 @@
         self.extend_and_reformat_parameter_documentation_metadata()
 
     def extend_and_reformat_parameter_documentation_metadata(self):
         for param_name, param_info in self.doc_dict.items():
             if 'fields' in param_info:
                 if 'Units' in param_info['fields']:
                     param_info['unit'] = param_info['fields']['Units'].split('(')[0].strip()
-                if 'Units' in param_info['fields']:
                     param_info['unit_tooltip'] = param_info['fields']['Units'].split('(')[1].strip(')')
                 if 'Range' in param_info['fields']:
                     param_info['min'] = float(param_info['fields']['Range'].split(' ')[0].strip())
-                if 'Range' in param_info['fields']:
                     param_info['max'] = float(param_info['fields']['Range'].split(' ')[1].strip())
                 if 'Calibration' in param_info['fields']:
                     param_info['Calibration'] = self.str_to_bool(param_info['fields']['Calibration'].strip())
                 if 'ReadOnly' in param_info['fields']:
                     param_info['ReadOnly'] = self.str_to_bool(param_info['fields']['ReadOnly'].strip())
                 if 'RebootRequired' in param_info['fields']:
                     param_info['RebootRequired'] = self.str_to_bool(param_info['fields']['RebootRequired'].strip())
@@ -350,7 +362,80 @@
         script_dir = os_path.dirname(os_path.abspath(__file__))
         return os_path.join(script_dir, 'ArduPilot_icon.png')
 
     @staticmethod
     def application_logo_filepath():
         script_dir = os_path.dirname(os_path.abspath(__file__))
         return os_path.join(script_dir, 'ArduPilot_logo.png')
+
+    def vehicle_image_filepath(self):
+        return os_path.join(self.vehicle_dir, 'vehicle.jpg')
+
+    def vehicle_image_exists(self):
+        return os_path.exists(self.vehicle_image_filepath())
+
+    def load_vehicle_components_json_data(self):
+        data = {}
+        try:
+            filepath = os_path.join(self.vehicle_dir, self.vehicle_components_json_filename)
+            with open(filepath, 'r', encoding='utf-8') as file:
+                data = json_load(file)
+        except FileNotFoundError:
+            logging_warning("File '%s' not found in %s.", self.vehicle_components_json_filename, self.vehicle_dir)
+        except JSONDecodeError:
+            logging_error("Error decoding JSON data from file '%s'.", filepath)
+        return data
+
+    def save_vehicle_components_json_data(self, data):
+        filepath = os_path.join(self.vehicle_dir, self.vehicle_components_json_filename)
+        with open(filepath, 'w', encoding='utf-8') as file:
+            json_dump(data, file, indent=4)
+
+    def new_vehicle_dir(self, base_dir: str, new_dir: str):
+        return os_path.join(base_dir, new_dir)
+
+    def create_new_vehicle_dir(self, new_vehicle_dir: str):
+        # Check if the new vehicle directory already exists
+        if os_path.exists(new_vehicle_dir):
+            return "Directory already exists, choose a different one"
+
+        try:
+            # Create the new vehicle directory
+            os_makedirs(new_vehicle_dir, exist_ok=True)
+        except OSError as e:
+            logging_error("Error creating new vehicle directory: %s", e)
+            return str(e)
+        return ""
+
+    def copy_template_files_to_new_vehicle_dir(self, template_dir: str, new_vehicle_dir: str):
+        # Copy the template files to the new vehicle directory
+        for item in os_listdir(template_dir):
+            s = os_path.join(template_dir, item)
+            d = os_path.join(new_vehicle_dir, item)
+            if os_path.isdir(s):
+                shutil_copytree(s, d)
+            else:
+                shutil_copy2(s, d)
+
+    @staticmethod
+    def getcwd():
+        return os_getcwd()
+
+    @staticmethod
+    def valid_directory_name(dir_name: str):
+        """
+        Checks if a given directory name contains only alphanumeric characters, underscores, hyphens,
+        and the OS directory separator.
+
+        This function is designed to ensure that the directory name does not contain characters that are
+        invalid for directory names in many operating systems. It does not guarantee that the name
+        is valid in all contexts or operating systems, as directory name validity can vary.
+
+        Parameters:
+        - dir_name (str): The directory name to check.
+
+        Returns:
+        - bool: True if the directory name matches the allowed pattern, False otherwise.
+        """
+        # Include os.sep in the pattern
+        pattern = r'^[\w' + re_escape(os_sep) + '-]+$'
+        return re_match(pattern, dir_name) is not None
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/frontend_tkinter.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/frontend_tkinter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,45 @@
 #!/usr/bin/env python3
 
 '''
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
-AP_FLAKE8_CLEAN
-
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 import tkinter as tk
-from tkinter import filedialog
 from tkinter import messagebox
-from tkinter import simpledialog
 from tkinter import ttk
 from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 from logging import critical as logging_critical
 from PIL import Image
 from PIL import ImageTk
-from platform import system as platform_system
 from typing import List
 from typing import Tuple
 
 from webbrowser import open as webbrowser_open  # to open the blog post documentation
 
 from backend_filesystem import LocalFilesystem
 from backend_filesystem import is_within_tolerance
+
 from backend_flightcontroller import FlightController
 
+from frontend_tkinter_base import show_tooltip
+from frontend_tkinter_base import AutoResizeCombobox
+from frontend_tkinter_base import ScrollFrame
+from frontend_tkinter_base import BaseWindow
+
+from frontend_tkinter_connection_selection import ConnectionSelectionWidgets
 
-def show_error_message(title: str, message: str):
-    root = tk.Tk()
-    # Set the theme to 'alt'
-    style = ttk.Style()
-    style.theme_use('alt')
-    root.withdraw() # Hide the main window
-    messagebox.showwarning(title, message)
-    root.destroy()
-
-
-def show_no_param_files_error(dirname: str):
-    error_message = f"No intermediate parameter files found in the selected '{dirname}' vehicle directory.\n" \
-        "Please select a vehicle directory containing valid ArduPilot methodic intermediate parameter files."
-    show_error_message("No Parameter Files Found", error_message)
-
-
-def show_no_connection_error(error_string: str):
-    error_message = f"{error_string}\n\nPlease connect a flight controller, wait a few seconds,\n" \
-        "restart the software and select its connection port."
-    show_error_message("No Connection to the Flight Controller", error_message)
-
-
-def show_tooltip(widget, text):
-    def enter(_event):
-        # Calculate the position of the tooltip based on the widget's position
-        x = widget.winfo_rootx() + widget.winfo_width() // 2
-        y = widget.winfo_rooty() + widget.winfo_height()
-        tooltip.geometry(f"+{x}+{y}")
-        tooltip.deiconify()
-
-    def leave(_event):
-        tooltip.withdraw()
-
-    tooltip = tk.Toplevel(widget)
-    tooltip.wm_overrideredirect(True)
-    tooltip_label = tk.Label(tooltip, text=text, bg="#ffffe0", relief="solid", borderwidth=1, justify=tk.LEFT)
-    tooltip_label.pack()
-    tooltip.withdraw() # Initially hide the tooltip
-
-    # Bind the <Enter> and <Leave> events to show and hide the tooltip
-    widget.bind("<Enter>", enter)
-    widget.bind("<Leave>", leave)
+from frontend_tkinter_directory_selection import VehicleDirectorySelectionWidgets
 
 
 def show_about_window(root, version: str):
     # Create a new window for the custom "About" message
     about_window = tk.Toplevel(root)
     about_window.title("About")
     about_window.geometry("650x220")
@@ -112,223 +73,43 @@
     user_manual_button.pack(side=tk.LEFT, padx=10, pady=10)
     support_forum_button.pack(side=tk.LEFT, padx=10, pady=10)
     report_bug_button.pack(side=tk.LEFT, padx=10, pady=10)
     credits_button.pack(side=tk.LEFT, padx=10, pady=10)
     source_button.pack(side=tk.LEFT, padx=10, pady=10)
 
 
-# https://dev.to/geraldew/python-tkinter-an-exercise-in-wrapping-the-combobox-ndb
-class PairTupleCombobox(ttk.Combobox):
-
-    def _process_listPairTuple(self, ip_listPairTuple):
-        r_list_keys = []
-        r_list_shows = []
-        for tpl in ip_listPairTuple:
-            r_list_keys.append(tpl[0])
-            r_list_shows.append(tpl[1])
-        return r_list_keys, r_list_shows
-
-    def __init__(self, container, p_listPairTuple, selected_element, *args, **kwargs):
-        super().__init__(container, *args, **kwargs)
-        self.set_entries_tupple(p_listPairTuple, selected_element)
-
-    def set_entries_tupple(self, p_listPairTuple, selected_element):
-        self.list_keys, self.list_shows = self._process_listPairTuple(p_listPairTuple)
-        self['values'] = tuple(self.list_shows)
-        # still need to set the default value from the nominated key
-        if selected_element:
-            try:
-                default_key_index = self.list_keys.index(selected_element)
-                self.current(default_key_index)
-            except IndexError:
-                logging_critical("connection combobox selected string '%s' not in list %s", selected_element, self.list_keys)
-                exit(1)
-            except ValueError:
-                logging_critical("connection combobox selected string '%s' not in list %s", selected_element, self.list_keys)
-                exit(1)
-            gui.update_combobox_width(self)
-        else:
-            logging_warning("No connection combobox element selected")
-
-    def getSelectedKey(self):
-        try:
-            i_index = self.current()
-            return self.list_keys[i_index]
-        except IndexError:
-            return None
-
-
-class AutoResizeCombobox(ttk.Combobox):
-
-    def __init__(self, container, values, selected_element, tooltip, *args, **kwargs):
-        super().__init__(container, *args, **kwargs)
-        self.set_entries_tupple(values, selected_element, tooltip)
-
-    def set_entries_tupple(self, values, selected_element, tooltip=None):
-        self['values'] = tuple(values)
-        if selected_element:
-            if selected_element in values:
-                self.set(selected_element)
-            else:
-                logging_error("param_file combobox selected string '%s' not in list %s", selected_element, values)
-        else:
-            if values:
-                logging_warning("No param_file combobox element selected")
-        if values:
-            gui.update_combobox_width(self)
-        if tooltip:
-            show_tooltip(self, tooltip)
-
-
-class ScrollFrame(tk.Frame):
-    def __init__(self, parent):
-        super().__init__(parent) # create a frame (self)
-
-        self.canvas = tk.Canvas(self, borderwidth=0)                                 # place canvas on self
-
-        # place a frame on the canvas, this frame will hold the child widgets
-        self.viewPort = tk.Frame(self.canvas)
-
-        self.vsb = tk.Scrollbar(self, orient="vertical", command=self.canvas.yview)  # place a scrollbar on self
-        # attach scrollbar action to scroll of canvas
-        self.canvas.configure(yscrollcommand=self.vsb.set)
-
-        self.vsb.pack(side="right", fill="y")                                        # pack scrollbar to right of self
-        # pack canvas to left of self and expand to fill
-        self.canvas.pack(side="left", fill="both", expand=True)
-        self.canvas_window = self.canvas.create_window((4, 4), window=self.viewPort, # add view port frame to canvas
-                                                       anchor="nw", tags="self.viewPort")
-
-        # bind an event whenever the size of the viewPort frame changes.
-        self.viewPort.bind("<Configure>", self.onFrameConfigure)
-        # bind an event whenever the size of the canvas frame changes.
-        self.canvas.bind("<Configure>", self.onCanvasConfigure)
-
-        # bind wheel events when the cursor enters the control
-        self.viewPort.bind('<Enter>', self.onEnter)
-        # unbind wheel events when the cursor leaves the control
-        self.viewPort.bind('<Leave>', self.onLeave)
-
-        # perform an initial stretch on render, otherwise the scroll region has a tiny border until the first resize
-        self.onFrameConfigure(None)
-
-    def onFrameConfigure(self, event):
-        '''Reset the scroll region to encompass the inner frame'''
-        # whenever the size of the frame changes, alter the scroll region respectively.
-        self.canvas.configure(scrollregion=self.canvas.bbox("all"))
-        # Calculate the bounding box for the scroll region, starting from the second row
-        # bbox = self.canvas.bbox("all")
-        # if bbox:
-        #     # Adjust the bounding box to start from the second row
-        #     bbox = (bbox[0], bbox[1] + self.canvas.winfo_reqheight(), bbox[2], bbox[3])
-        #     self.canvas.configure(scrollregion=bbox)
-
-    def onCanvasConfigure(self, event):
-        '''Reset the canvas window to encompass inner frame when required'''
-        canvas_width = event.width
-        # whenever the size of the canvas changes alter the window region respectively.
-        self.canvas.itemconfig(self.canvas_window, width=canvas_width)
-
-    def onMouseWheel(self, event):                         # cross platform scroll wheel event
-        canvas_height = self.canvas.winfo_height()
-        rows_height = self.canvas.bbox("all")[3]
-
-        if rows_height > canvas_height: # only scroll if the rows overflow the frame
-            if platform_system() == 'Windows':
-                self.canvas.yview_scroll(int(-1 * (event.delta / 120)), "units")
-            elif platform_system() == 'Darwin':
-                self.canvas.yview_scroll(int(-1 * event.delta), "units")
-            else:
-                if event.num == 4:
-                    self.canvas.yview_scroll(-1, "units")
-                elif event.num == 5:
-                    self.canvas.yview_scroll(1, "units")
-
-    def onEnter(self, event):                               # bind wheel events when the cursor enters the control
-        if platform_system() == 'Linux':
-            self.canvas.bind_all("<Button-4>", self.onMouseWheel)
-            self.canvas.bind_all("<Button-5>", self.onMouseWheel)
-        else:
-            self.canvas.bind_all("<MouseWheel>", self.onMouseWheel)
 
-    def onLeave(self, event):                               # unbind wheel events when the cursor leaves the control
-        if platform_system() == 'Linux':
-            self.canvas.unbind_all("<Button-4>")
-            self.canvas.unbind_all("<Button-5>")
-        else:
-            self.canvas.unbind_all("<MouseWheel>")
-
-
-class gui:
+class gui(BaseWindow):
     def __init__(self, current_file: str, flight_controller: FlightController,
                  local_filesystem: LocalFilesystem, version: str):
+        super().__init__()
         self.current_file = current_file
         self.flight_controller = flight_controller
         self.local_filesystem = local_filesystem
 
         self.at_least_one_param_edited = False
         self.at_least_one_changed_parameter_written = False
         self.write_checkbutton_var = {}
-        self.root = tk.Tk()
         self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version)
         self.root.geometry("880x500") # Set the window width
 
-        # Set the theme to 'alt'
-        style = ttk.Style()
-        style.theme_use('alt')
-
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_connection_and_quit)
 
-        # Set the application icon for the window and all child windows
-        # https://pythonassets.com/posts/window-icon-in-tk-tkinter/
-        self.root.iconphoto(True, tk.PhotoImage(file=LocalFilesystem.application_icon_filepath()))
-
         config_frame = tk.Frame(self.root)
         config_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
 
         config_subframe = tk.Frame(config_frame)
         config_subframe.pack(side=tk.LEFT, fill="x", expand=True, anchor=tk.NW) # Pack the frame at the top of the window
 
-        # Get the background color for the 'TFrame' widget
-        self.default_background_color = '#f0f0f0' # style.lookup('TFrame', 'background')
-
-        # Configure the background color for the checkbutton
-        style.configure('TCheckbutton', background=self.default_background_color)
-        style.configure('TCombobox', background=self.default_background_color)
-
         # Create a new frame inside the config_subframe for the intermediate parameter file directory selection labels
         # and directory selection button
-        directory_selection_frame = tk.Frame(config_subframe)
-        directory_selection_frame.pack(side=tk.LEFT, fill="x", expand=False, padx=(4, 6))
-
-        # Create a description label for the directory
-        directory_selection_label = tk.Label(directory_selection_frame, text="Vehicle directory:")
-        directory_selection_label.pack(side=tk.TOP, anchor=tk.NW) # Add the label to the top of the directory_selection_frame
-
-        # Create a new subframe for the directory selection
-        directory_selection_subframe = tk.Frame(directory_selection_frame)
-        directory_selection_subframe.pack(side=tk.TOP, fill="x", expand=False, anchor=tk.NW)
-
-        # Create a read-only entry for the directory
-        vehicle_directory_name = self.local_filesystem.get_vehicle_directory_name()
-        vehicle_dir_var = tk.StringVar(value=vehicle_directory_name)
-        self.directory_entry = tk.Entry(directory_selection_subframe, textvariable=vehicle_dir_var,
-                                        width=max(4, len(vehicle_directory_name)), state='readonly')
-        self.directory_entry.pack(side=tk.LEFT, fill="x", expand=True, anchor=tk.NW, pady=(4, 0))
-        show_tooltip(self.directory_entry,
-                     "Vehicle-specific directory containing the intermediate\nparameter files to be written to the flight "
-                     "controller")
-
-        # Create a button for directory selection
-        directory_selection_button = ttk.Button(directory_selection_subframe, text="...",
-                                                command=self.on_select_vehicle_directory, width=2)
-        directory_selection_button.pack(side=tk.RIGHT, anchor=tk.NW)
-        show_tooltip(directory_selection_button, "Select the vehicle-specific directory containing the\nintermediate "
-                     "parameter files to be written to the flight controller")
+        directory_selection_frame = VehicleDirectorySelectionWidgets(self, config_subframe, self.local_filesystem,
+                                                                     destroy_parent_on_open=False)
+        directory_selection_frame.container_frame.pack(side=tk.LEFT, fill="x", expand=False, padx=(4, 6))
 
         # Create a new frame inside the config_subframe for the intermediate parameter file selection label and combobox
         file_selection_frame = tk.Frame(config_subframe)
         file_selection_frame.pack(side=tk.LEFT, fill="x", expand=False, padx=(6, 6))
 
         # Create a label for the combobox
         file_selection_label = tk.Label(file_selection_frame, text="Current intermediate parameter file:")
@@ -343,30 +124,17 @@
                                                           "advance to the next file once the current file is written to the "
                                                           "fight controller",
                                                           state='readonly', width=45)
         self.file_selection_combobox.bind("<<ComboboxSelected>>", self.on_param_file_combobox_change)
         self.file_selection_combobox.pack(side=tk.TOP, anchor=tk.NW, pady=(4, 0))
 
         # Create a new frame inside the config_subframe for the flight controller connection selection label and combobox
-        conn_selection_frame = tk.Frame(config_subframe)
-        conn_selection_frame.pack(side=tk.RIGHT, fill="x", expand=False, padx=(6, 4))
-
-        # Create a description label for the flight controller connection selection
-        conn_selection_label = tk.Label(conn_selection_frame, text="flight controller connection:")
-        conn_selection_label.pack(side=tk.TOP, anchor=tk.NW) # Add the label to the top of the conn_selection_frame
-
-        # Create a read-only combobox for flight controller connection selection
-        self.conn_selection_combobox = PairTupleCombobox(conn_selection_frame, self.flight_controller.get_connection_tuples(),
-                                                         self.flight_controller.comport.device if
-                                                         hasattr(self.flight_controller.comport, "device") else None,
-                                                         state='readonly')
-        self.conn_selection_combobox.bind("<<ComboboxSelected>>", self.on_select_connection_combobox_change)
-        self.conn_selection_combobox.pack(side=tk.TOP, anchor=tk.NW, pady=(4, 0))
-        show_tooltip(self.conn_selection_combobox, "Select the flight controller connection\nYou can add a custom connection "
-                     "to the existing ones")
+        csw = ConnectionSelectionWidgets(self, config_subframe, self.flight_controller,
+                                         destroy_parent_on_connect=False, read_params_on_connect=True)
+        csw.container_frame.pack(side=tk.RIGHT, fill="x", expand=False, padx=(6, 4))
 
         # Load the ArduPilot logo and scale it down to image_height pixels in height
         image_height = 40
         image = Image.open(LocalFilesystem.application_logo_filepath())
         width, height = image.size
         aspect_ratio = width / height
         new_width = int(image_height * aspect_ratio)
@@ -449,94 +217,27 @@
         skip_button.pack(side=tk.RIGHT, padx=(8, 8)) # Add right padding to the skip button
         show_tooltip(skip_button, "Skip to the next intermediate parameter file without writing any changes to the flight "
                      "controller\nIf changes have been made to the current file it will ask if you want to save them")
 
         self.root.after(50, self.read_flight_controller_parameters(reread=False)) # 50 milliseconds
         self.root.mainloop()
 
-    @staticmethod
-    def update_combobox_width(combobox):
-        # Calculate the maximum width needed for the content
-        max_width = max(len(value) for value in combobox['values'])
-        # Set a minimum width for the combobox
-        min_width = 4 # Adjust this value as needed
-        # Set the width of the combobox to the maximum width, but not less than the minimum width
-        combobox.config(width=max(min_width, max_width))
-
-    def on_select_vehicle_directory(self):
-        # Open the directory selection dialog
-        selected_directory = filedialog.askdirectory(initialdir=self.local_filesystem.vehicle_dir)
-        if selected_directory:
-            self.local_filesystem.vehicle_dir = selected_directory
-            displayed_directory = self.local_filesystem.get_vehicle_directory_name()
-            # Set the width of the directory_entry to match the width of the displayed_directory text
-            self.directory_entry.config(width=max(4, len(displayed_directory)), state='normal')
-            self.directory_entry.delete(0, tk.END)
-            self.directory_entry.insert(0, displayed_directory)
-            self.directory_entry.config(state='readonly')
-            self.root.update_idletasks()
-            # Update the local_filesystem with the new directory
-            self.local_filesystem.re_init(selected_directory, self.local_filesystem.vehicle_type)
-            files = list(self.local_filesystem.file_parameters.keys())
-            if files:
-                self.file_selection_combobox.set_entries_tupple(files, files[0])
-                # Trigger the combobox change event to update the table
-                self.on_param_file_combobox_change(None, forced=True)
-            else:
-                # No files were found in the selected directory
-                show_no_param_files_error(selected_directory)
-
     def on_param_file_combobox_change(self, _event, forced: bool = False):
         if not self.file_selection_combobox['values']:
             return
         self.param_edit_widgets_event_generate_focus_out()
         selected_file = self.file_selection_combobox.get()
         if self.current_file != selected_file or forced:
             self.write_changes_to_intermediate_parameter_file()
             # Update the current_file attribute to the selected file
             self.current_file = selected_file
             self.at_least_one_changed_parameter_written = False
             self.update_documentation_labels()
             self.repopulate_parameter_table(selected_file)
 
-    def on_select_connection_combobox_change(self, _event):
-        selected_connection = self.conn_selection_combobox.getSelectedKey()
-        logging_debug(f"Connection combobox changed to: {selected_connection}")
-        if self.flight_controller.master is None or selected_connection != self.flight_controller.comport.device:
-            if selected_connection == 'Add another':
-                self.on_add_connection(None)
-                return
-            self.reconnect(selected_connection)
-
-    def on_add_connection(self, _event):
-        # Open the connection selection dialog
-        selected_connection = simpledialog.askstring("Flight Controller Connection",
-                                                     "Enter the connection string to the flight controller. "
-                                                     "Examples are:\n\nCOM4 (on windows)\n"
-                                                     "/dev/serial/by-id/usb-xxx (on linux)\n"
-                                                     "tcp:127.0.0.1:5761\n"
-                                                     "udp:udp:127.0.0.1:14551")
-        logging_debug(f"Will add new connection: {selected_connection} if not duplicated")
-        self.flight_controller.add_connection(selected_connection)
-        connection_tuples = self.flight_controller.get_connection_tuples()
-        logging_debug(f"Updated connection tuples: {connection_tuples} with selected connection: {selected_connection}")
-        self.conn_selection_combobox.set_entries_tupple(connection_tuples, selected_connection)
-        self.reconnect(selected_connection)
-
-    def reconnect(self, selected_connection: str = None):
-        if selected_connection:
-            [self.connection_progress_window,
-             self.connection_progress_bar,
-             self.connection_progress_label] = self.create_progress_window("Connecting with the FC")
-            error_message = self.flight_controller.connect(selected_connection, self.update_connection_progress_bar)
-            if error_message:
-                show_no_connection_error(error_message)
-                return
-            self.connection_progress_window.destroy()
-
     def read_flight_controller_parameters(self, reread: bool = False):
         [self.param_read_progress_window,
          self.param_read_progress_bar,
          self.param_read_progress_label] = self.create_progress_window(("Re-r" if reread else "R") + "eading FC parameters")
         # Download all parameters from the flight controller
         self.flight_controller.fc_parameters = self.flight_controller.read_params(self.update_param_download_progress_bar)
         self.param_read_progress_window.destroy()  # for the case that we are doing test and there is no real FC connected
@@ -594,15 +295,15 @@
         if not different_params and self.show_only_differences.get():
             logging_info("No different parameters found in %s. Skipping...", selected_file)
             messagebox.showinfo("ArduPilot methodic configurator",
                                 f"No different parameters found in {selected_file}. Skipping...")
             self.on_skip_click(force_focus_out_event=False)
             return
         # Clear the current table
-        for widget in self.scroll_frame.viewPort.winfo_children():
+        for widget in self.scroll_frame.view_port.winfo_children():
             widget.destroy()
         # Repopulate the table with the new parameters
         if self.show_only_differences.get():
             self.update_table(different_params, fc_parameters)
         else:
             self.update_table(self.local_filesystem.file_parameters[selected_file], fc_parameters)
         # Scroll to the top of the parameter table
@@ -614,47 +315,47 @@
         tooltips = ["Parameter name must be ^[A-Z][A-Z_0-9]* and most 16 characters long",
                     "Current value on the flight controller ",
                     "New value from the above selected intermediate parameter file",
                     "Parameter Unit",
                     "When selected, write new value to the flight controller",
                     "Reason why respective parameter changed"]
         for i, header in enumerate(headers):
-            label = tk.Label(self.scroll_frame.viewPort, text=header)
+            label = tk.Label(self.scroll_frame.view_port, text=header)
             label.grid(row=0, column=i, sticky="ew") # Use sticky="ew" to make the label stretch horizontally
             show_tooltip(label, tooltips[i])
 
         self.write_checkbutton_var = {}
         try:
             # Create the new table
             for i, (param_name, param) in enumerate(params.items()):
                 param_metadata = self.local_filesystem.doc_dict.get(param_name, None)
 
                 is_calibration = param_metadata.get('Calibration', False) if param_metadata else False
                 is_readonly = param_metadata.get('ReadOnly', False) if param_metadata else False
-                parameter_label = tk.Label(self.scroll_frame.viewPort, text=param_name + (" " * (16 - len(param_name))),
+                parameter_label = tk.Label(self.scroll_frame.view_port, text=param_name + (" " * (16 - len(param_name))),
                                            background="red" if is_readonly else "yellow" if is_calibration else
                                            self.default_background_color)
                 if param_name in fc_parameters:
                     value_str = format(fc_parameters[param_name], '.6f').rstrip('0').rstrip('.')
-                    flightcontroller_value = tk.Label(self.scroll_frame.viewPort, text=value_str)
+                    flightcontroller_value = tk.Label(self.scroll_frame.view_port, text=value_str)
                 else:
-                    flightcontroller_value = tk.Label(self.scroll_frame.viewPort, text="N/A", background="blue")
+                    flightcontroller_value = tk.Label(self.scroll_frame.view_port, text="N/A", background="blue")
 
-                new_value_entry = tk.Entry(self.scroll_frame.viewPort, width=10, justify=tk.RIGHT, background="white")
+                new_value_entry = tk.Entry(self.scroll_frame.view_port, width=10, justify=tk.RIGHT, background="white")
                 new_value_entry.insert(0, format(param.value, '.6f').rstrip('0').rstrip('.'))
                 new_value_entry.bind("<FocusOut>", lambda event, current_file=self.current_file, param_name=param_name:
                                      self.on_parameter_value_change(event, current_file, param_name))
 
-                unit_label = tk.Label(self.scroll_frame.viewPort, text=param_metadata.get('unit') if param_metadata else "")
+                unit_label = tk.Label(self.scroll_frame.view_port, text=param_metadata.get('unit') if param_metadata else "")
 
                 self.write_checkbutton_var[param_name] = tk.BooleanVar(value=True) # Default to selected
-                write_write_checkbutton = ttk.Checkbutton(self.scroll_frame.viewPort,
+                write_write_checkbutton = ttk.Checkbutton(self.scroll_frame.view_port,
                                                           variable=self.write_checkbutton_var[param_name])
 
-                change_reason_entry = tk.Entry(self.scroll_frame.viewPort, background="white")
+                change_reason_entry = tk.Entry(self.scroll_frame.view_port, background="white")
                 change_reason_entry.insert(0, "" if param.comment is None else param.comment)
                 change_reason_entry.bind("<FocusOut>", lambda event, current_file=self.current_file, param_name=param_name:
                                          self.on_parameter_change_reason_change(event, current_file, param_name))
 
                 doc_tooltip = param_metadata.get('doc_tooltip') if param_metadata else \
                     "No documentation available in apm.pdef.xml for this parameter"
                 if doc_tooltip:
@@ -674,26 +375,26 @@
                     new_value_entry,
                     unit_label,
                     write_write_checkbutton,
                     change_reason_entry,
                 ]
                 for j, widget in enumerate(row):
                     # Use sticky="ew" to make the widget stretch horizontally
-                    widget.grid(row=i+1, column=j, sticky="w" if j == 0 else "ew" if j == 5 else "e")
+                    widget.grid(row=i+1, column=j, sticky="w" if j == 0 else "ew" if j == 5 else "e", padx=(0, 5) if j == 5 else 0)
         except KeyError as e:
             logging_critical("Parameter %s not found in the %s file: %s", param_name, self.current_file, e, exc_info=True)
             exit(1)
 
         # Configure the table_frame to stretch columns
-        self.scroll_frame.viewPort.columnconfigure(0, weight=0, minsize=120) # Parameter name
-        self.scroll_frame.viewPort.columnconfigure(1, weight=0) # Current Value
-        self.scroll_frame.viewPort.columnconfigure(2, weight=0) # New Value
-        self.scroll_frame.viewPort.columnconfigure(3, weight=0) # Units
-        self.scroll_frame.viewPort.columnconfigure(4, weight=0) # write to FC
-        self.scroll_frame.viewPort.columnconfigure(5, weight=1) # Change reason
+        self.scroll_frame.view_port.columnconfigure(0, weight=0, minsize=120) # Parameter name
+        self.scroll_frame.view_port.columnconfigure(1, weight=0) # Current Value
+        self.scroll_frame.view_port.columnconfigure(2, weight=0) # New Value
+        self.scroll_frame.view_port.columnconfigure(3, weight=0) # Units
+        self.scroll_frame.view_port.columnconfigure(4, weight=0) # write to FC
+        self.scroll_frame.view_port.columnconfigure(5, weight=1) # Change reason
 
     def on_parameter_value_change(self, event, current_file, param_name):
         # Get the new value from the Entry widget
         new_value = event.widget.get()
         try:
             old_value = self.local_filesystem.file_parameters[current_file][param_name].value
         except KeyError as e:
@@ -757,71 +458,14 @@
             if checkbutton_state.get():
                 selected_params[param_name] = self.local_filesystem.file_parameters[self.current_file][param_name]
         return selected_params
 
     def on_show_only_changed_checkbox_change(self):
         self.repopulate_parameter_table(self.current_file)
 
-    def create_progress_window(self, title: str):
-        # Create a new window for the param_read progress bar
-        progress_window = tk.Toplevel(self.root)
-        progress_window.title(title)
-        progress_window.geometry("300x80")
-
-        # Center the param_read progress window on the main window
-        self.center_window(progress_window, self.root)
-
-        # Create a param_read progress bar
-        progress_bar = ttk.Progressbar(progress_window, length=100, mode='determinate')
-        progress_bar.pack(side=tk.TOP, fill=tk.X, expand=False, padx=(5, 5), pady=(10, 10))
-
-        # Create a param_read label to display the progress message
-        progress_label = tk.Label(progress_window, text="")
-        progress_label.pack(side=tk.TOP, fill=tk.X, expand=False, pady=(10, 10))
-
-        return progress_window, progress_bar, progress_label
-
-    def center_window(self, window, parent):
-        """
-        Center a window on its parent window.
-
-        Args:
-            window (tk.Toplevel): The window to center.
-            parent (tk.Tk): The parent window.
-        """
-        window.update_idletasks()
-        parent_width = parent.winfo_width()
-        parent_height = parent.winfo_height()
-        window_width = window.winfo_width()
-        window_height = window.winfo_height()
-        x = parent.winfo_x() + (parent_width // 2) - (window_width // 2)
-        y = parent.winfo_y() + (parent_height // 2) - (window_height // 2)
-        window.geometry(f"+{x}+{y}")
-
-    def update_connection_progress_bar(self, current_value: int, max_value: int):
-        """
-        Update the FC connection progress bar and the progress message with the current progress.
-
-        Args:
-            current_value (int): The current progress value.
-            max_value (int): The maximum progress value.
-        """
-        self.connection_progress_window.lift()
-
-        self.connection_progress_bar['value'] = current_value
-        self.connection_progress_bar['maximum'] = max_value
-        self.connection_progress_bar.update()
-
-        # Update the reset progress message
-        self.connection_progress_label.config(text=f"waiting for {current_value} of {max_value} seconds")
-
-        # Close the reset progress window when the process is complete
-        if current_value == max_value:
-            self.connection_progress_window.destroy()
-
     def update_reset_progress_bar(self, current_value: int, max_value: int):
         """
         Update the FC reset progress bar and the progress message with the current progress.
 
         Args:
             current_value (int): The current progress value.
             max_value (int): The maximum progress value.
@@ -858,15 +502,15 @@
 
         # Close the param read progress window when the process is complete
         if current_value == max_value:
             self.param_read_progress_window.destroy()
 
     def param_edit_widgets_event_generate_focus_out(self):
         # Trigger the <FocusOut> event for all entry widgets to ensure all changes are processed
-        for widget in self.scroll_frame.viewPort.winfo_children():
+        for widget in self.scroll_frame.view_port.winfo_children():
             if isinstance(widget, tk.Entry):
                 widget.event_generate("<FocusOut>", when="now")
 
     def write_params_that_require_reset(self, selected_params: dict):
         """
         Write the selected parameters to the flight controller that require a reset.
 
@@ -959,14 +603,15 @@
             self.read_flight_controller_parameters(True)
             logging_info("Re-read all parameters from the flight controller")
 
             # Validate that the read parameters are the same as the ones in the current_file
             param_write_error = []
             for param_name, param in selected_params.items():
                 if param_name in self.flight_controller.fc_parameters and \
+                   param is not None and \
                    not is_within_tolerance(self.flight_controller.fc_parameters[param_name], float(param.value)):
                     logging_error("Parameter %s write to the flight controller failed. Expected: %f, Actual: %f",
                                   param_name, param.value, self.flight_controller.fc_parameters[param_name])
                     param_write_error.append(param_name)
                 if param_name not in self.flight_controller.fc_parameters:
                     logging_error("Parameter %s write to the flight controller failed. Expected: %f, Actual: N/A",
                                   param_name, param.value)
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/param_ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 '''
 decode ftp parameter protocol data
 '''
 
+# pylint: skip-file
+
 import struct
 import sys
 
 
 class ParamData(object):
     def __init__(self):
         # params as (name, value, ptype)
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 This script updates the PID adjustment parameters to be factor of the corresponding autotuned or optimized parameters.
 
 Usage:
     ./param_pid_adjustment_update.py -d /path/to/directory optimized_parameter_file.param
 
 This file is part of Ardupilot methodic configurator. https://github.com/ArduPilot/MethodicConfigurator
 
-AP_FLAKE8_CLEAN
-
 (C) 2024 Amilcar do Carmo Lucas, IAV GmbH
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 import os
 import argparse
@@ -76,14 +74,21 @@
             raise argparse.ArgumentTypeError(f'must be within [{min_value}, {max_value}]')
         return f
     # Return function handle to checking function
     return range_checker
 
 
 class Par:
+    """
+    A class representing a parameter with a value and an optional comment.
+
+    Attributes:
+        value (float): The value of the parameter.
+        comment (str): An optional comment describing the parameter.
+    """
     def __init__(self, value: float, comment: str = None):
         self.value = value
         self.comment = comment
 
     @staticmethod
     def load_param_file_into_dict(param_file: str) -> Dict[str, 'Par']:
         parameter_dict = {}
@@ -101,30 +106,32 @@
                 if "," in line:
                     parameter, value = line.split(",", 1)
                 elif " " in line:
                     parameter, value = line.split(" ", 1)
                 elif "\t" in line:
                     parameter, value = line.split("\t", 1)
                 else:
-                    raise SystemExit("Missing parameter-value separator: %s in %s line %u" % (line, param_file, n))
+                    raise SystemExit(f"Missing parameter-value separator: {line} in {param_file} line {n}")
                 if len(parameter) > PARAM_NAME_MAX_LEN:
-                    raise SystemExit("Too long parameter name: %s in %s line %u" % (parameter, param_file, n))
+                    raise SystemExit(f"Too long parameter name: {parameter} in {param_file} line {n}")
                 if not re.match(PARAM_NAME_REGEX, parameter):
-                    raise SystemExit("Invalid characters in parameter name %s in %s line %u" % (parameter, param_file, n))
+                    raise SystemExit(f"Invalid characters in parameter name {parameter} in {param_file} line {n}")
                 try:
                     fvalue = float(value)
                 except ValueError as exc:
-                    raise SystemExit("Invalid parameter value %s in %s line %u" % (value, param_file, n)) from exc
+                    raise SystemExit(f"Invalid parameter value {value} in {param_file} line {n}") from exc
                 if parameter in parameter_dict:
-                    raise SystemExit("Duplicated parameter %s in %s line %u" % (parameter, param_file, n))
+                    raise SystemExit(f"Duplicated parameter {parameter} in {param_file} line {n}")
                 parameter_dict[parameter] = Par(fvalue, comment)
         return parameter_dict, content
 
     @staticmethod
-    def export_to_param(param_dict: Dict[str, 'Par'], filename_out: str, content_header: List[str] = []) -> None:
+    def export_to_param(param_dict: Dict[str, 'Par'], filename_out: str, content_header: List[str] = None) -> None:
+        if content_header is None:
+            content_header = []
         with open(filename_out, "w", encoding="utf-8") as output_file:
             if content_header:
                 output_file.write('\n'.join(content_header) + '\n')
             for key, par in param_dict.items():
                 line = f"{key},{format(par.value, '.6f').rstrip('0').rstrip('.')}"
                 if par.comment:
                     line += f"  # {par.comment}"
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator/tempcal_IMU.py` & `methodicconfigurator-0.2.0/MethodicConfigurator/tempcal_IMU.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 '''
 Create temperature calibration parameters for IMUs based on log data.
 '''
 
+# pylint: skip-file
+
 import sys
 import math
 import re
 from pymavlink import mavutil
 import numpy as np
 import matplotlib.pyplot as pyplot
 # from scipy import signal
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.1.9
+Version: 0.2.0
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,23 +21,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
 Requires-Dist: requests
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mock; extra == "dev"
 
 # ArduPilot Methodic Configurator
+# Everyone should be able to configure ArduPilot for their vehicles
 
 | Lint | Build | Test | Deploy |
 | ---- | ----- | ---- | ------ |
-| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
-| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
-| | | | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
+| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | [![Python unit-tests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml) | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
+| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | [![Pytest unittests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml) | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
+| | | [![coverage](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml) | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
 
 Amilcar Lucas's ArduPilot Methodic Configurator is a Python tool that implements a [clear and proven configuration sequence of ArduPilot of drones](https://discuss.ardupilot.org/t/how-to-methodically-tune-almost-any-multicopter-using-arducopter-4-4-x/110842/1).
 It provides a graphical user interface (GUI) for managing and visualizing ArduPilot parameters, parameter files and documentation.
 
 ![Application Screenshot](https://github.com/ArduPilot/MethodicConfigurator/raw/master/images/App_screenshot1.png)
 
 ## Usage
@@ -82,9 +87,9 @@
 
 ## Code of conduct
 
 To use and develop this software you must obey the [ArduPilot Methodic Configurator Code of Conduct](https://github.com/ArduPilot/MethodicConfigurator/blob/master/CODE_OF_CONDUCT.md).
 
 ## License
 
-This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
+This project is licensed under the [GNU General Public License v3.0](https://github.com/ArduPilot/MethodicConfigurator/blob/master/LICENSE.md).
 It builds upon other [opensource software packages](https://github.com/ArduPilot/MethodicConfigurator/blob/master/credits/CREDITS.md)
```

### Comparing `MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/SOURCES.txt` & `methodicconfigurator-0.2.0/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 README.md
 setup.py
 MethodicConfigurator/__init__.py
 MethodicConfigurator/annotate_params.py
 MethodicConfigurator/ardupilot_methodic_configurator.py
 MethodicConfigurator/backend_filesystem.py
 MethodicConfigurator/backend_flightcontroller.py
+MethodicConfigurator/backend_mavftp.py
 MethodicConfigurator/component_editor.py
 MethodicConfigurator/extract_param_defaults.py
 MethodicConfigurator/frontend_tkinter.py
+MethodicConfigurator/frontend_tkinter_base.py
+MethodicConfigurator/frontend_tkinter_connection_selection.py
+MethodicConfigurator/frontend_tkinter_directory_selection.py
 MethodicConfigurator/param_ftp.py
 MethodicConfigurator/param_pid_adjustment_update.py
 MethodicConfigurator/tempcal_IMU.py
 MethodicConfigurator/version.py
 MethodicConfigurator.egg-info/PKG-INFO
 MethodicConfigurator.egg-info/SOURCES.txt
 MethodicConfigurator.egg-info/dependency_links.txt
```

### Comparing `MethodicConfigurator-0.1.9/PKG-INFO` & `methodicconfigurator-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.1.9
+Version: 0.2.0
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,23 +21,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pymavlink
 Requires-Dist: pyserial
 Requires-Dist: pillow
 Requires-Dist: requests
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mock; extra == "dev"
 
 # ArduPilot Methodic Configurator
+# Everyone should be able to configure ArduPilot for their vehicles
 
 | Lint | Build | Test | Deploy |
 | ---- | ----- | ---- | ------ |
-| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
-| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
-| | | | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
+| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | [![Python unit-tests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml) | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
+| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | [![Pytest unittests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml) | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
+| | | [![coverage](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml) | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
 
 Amilcar Lucas's ArduPilot Methodic Configurator is a Python tool that implements a [clear and proven configuration sequence of ArduPilot of drones](https://discuss.ardupilot.org/t/how-to-methodically-tune-almost-any-multicopter-using-arducopter-4-4-x/110842/1).
 It provides a graphical user interface (GUI) for managing and visualizing ArduPilot parameters, parameter files and documentation.
 
 ![Application Screenshot](https://github.com/ArduPilot/MethodicConfigurator/raw/master/images/App_screenshot1.png)
 
 ## Usage
@@ -82,9 +87,9 @@
 
 ## Code of conduct
 
 To use and develop this software you must obey the [ArduPilot Methodic Configurator Code of Conduct](https://github.com/ArduPilot/MethodicConfigurator/blob/master/CODE_OF_CONDUCT.md).
 
 ## License
 
-This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
+This project is licensed under the [GNU General Public License v3.0](https://github.com/ArduPilot/MethodicConfigurator/blob/master/LICENSE.md).
 It builds upon other [opensource software packages](https://github.com/ArduPilot/MethodicConfigurator/blob/master/credits/CREDITS.md)
```

### Comparing `MethodicConfigurator-0.1.9/README.md` & `methodicconfigurator-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ArduPilot Methodic Configurator
+# Everyone should be able to configure ArduPilot for their vehicles
 
 | Lint | Build | Test | Deploy |
 | ---- | ----- | ---- | ------ |
-| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
-| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
-| | | | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
+| [![Pylint](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pylint.yml) | | [![Python unit-tests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unit-tests.yml) | [![pages-build-deployment](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/pages/pages-build-deployment) |
+| [![test Python cleanliness](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-cleanliness.yml) | | [![Pytest unittests](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/unittests.yml) | [![Upload MethodicConfigurator Package](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/python-publish.yml) |
+| | | [![coverage](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/coverage.yml) | [![Windows Build](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml/badge.svg)](https://github.com/ArduPilot/MethodicConfigurator/actions/workflows/windows_build.yml) |
 
 Amilcar Lucas's ArduPilot Methodic Configurator is a Python tool that implements a [clear and proven configuration sequence of ArduPilot of drones](https://discuss.ardupilot.org/t/how-to-methodically-tune-almost-any-multicopter-using-arducopter-4-4-x/110842/1).
 It provides a graphical user interface (GUI) for managing and visualizing ArduPilot parameters, parameter files and documentation.
 
 ![Application Screenshot](images/App_screenshot1.png)
 
 ## Usage
@@ -53,9 +54,9 @@
 
 ## Code of conduct
 
 To use and develop this software you must obey the [ArduPilot Methodic Configurator Code of Conduct](CODE_OF_CONDUCT.md).
 
 ## License
 
-This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
+This project is licensed under the [GNU General Public License v3.0](LICENSE.md).
 It builds upon other [opensource software packages](credits/CREDITS.md)
```

### Comparing `MethodicConfigurator-0.1.9/setup.py` & `methodicconfigurator-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,19 @@
 # as that breaks the pip install. It seems that pip is not smart enough to
 # use the system versions of these dependencies, so it tries to download and install
 # large numbers of modules like tkinter etc which may be already installed
 requirements = ['pymavlink>=2.4.14',
                 'pyserial>=3.0']
 
 dev_requirements = [
-    'flake8',
+    'ruff',
+    'pytest',
+    'pytest-cov',
+    'coverage',
+    'mock',
     # Add any other development requirements here
 ]
 
 prj_url = "https://github.com/ArduPilot/MethodicConfigurator"
 
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as f:
```

