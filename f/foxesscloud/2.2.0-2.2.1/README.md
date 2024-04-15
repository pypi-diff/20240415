# Comparing `tmp/foxesscloud-2.2.0.tar.gz` & `tmp/foxesscloud-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-an7s2f9q\foxesscloud-2.2.0.tar", last modified: Tue Apr  9 15:32:39 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-rjjzde6s\foxesscloud-2.2.1.tar", last modified: Mon Apr 15 11:21:29 2024, max compression
```

## Comparing `foxesscloud-2.2.0.tar` & `foxesscloud-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.0/LICENCE
--rw-rw-rw-   0        0        0    39156 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    38601 2024-04-09 15:25:31.000000 foxesscloud-2.2.0/README.md
--rw-rw-rw-   0        0        0      635 2024-04-09 15:23:57.000000 foxesscloud-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud/
--rw-rw-rw-   0        0        0   175090 2024-04-09 15:25:23.000000 foxesscloud-2.2.0/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   169383 2024-04-09 15:28:42.000000 foxesscloud-2.2.0/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39156 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 15:32:39.000000 foxesscloud-2.2.0/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.1/LICENCE
+-rw-rw-rw-   0        0        0    39391 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    38836 2024-04-15 11:18:57.000000 foxesscloud-2.2.1/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-15 11:08:55.000000 foxesscloud-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud/
+-rw-rw-rw-   0        0        0   175247 2024-04-15 11:11:43.000000 foxesscloud-2.2.1/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   169540 2024-04-15 11:11:43.000000 foxesscloud-2.2.1/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39391 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.0/LICENCE` & `foxesscloud-2.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.0/PKG-INFO` & `foxesscloud-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.0
+Version: 2.2.1
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -390,16 +390,16 @@
 
 ```
 f.battery_info(count, plot, log)
 f.battery_monitor(interval, run, log, save, count)
 ```
 
 battery_info() prints information on the battery and cells:
-+ count: optional over-ride. The default is based on rounding the battery voltage divided by 53
-+ plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
++ count: optional over-ride. The default is based on factorising the number of cells reported by 16 or 18 to work out the number of batteries.
++ plot: 1 plot the cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
 + log: see below. Default is 0
 
 battery_monitor() runs battery_info() in log mode on a schedule to provide information on the battery status over a period of time:
 + interval: the time in minutes between log entries. The default is 30 minutes
 + run: the number of log entries to create. The default is 48 i.e. every 30 minues for 24 hours in total
 + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The default is 1
 + save: name of a CSV file to write log data to
@@ -665,15 +665,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.20.<br>
+2.2.1.<br>
+Ensure output is generated if get_battery() fails using battery_info().
+Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.0 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.1 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -282,16 +282,17 @@
 [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
 This example shows the results reported by charge needed: ![image](https://
 github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
 20d806b1e7e8) ## Battery Info Provides detailed information on the current
 state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
 (interval, run, log, save, count) ``` battery_info() prints information on the
 battery and cells: + count: optional over-ride. The default is based on
-rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
-each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
 battery_monitor() runs battery_info() in log mode on a schedule to provide
 information on the battery status over a period of time: + interval: the time
 in minutes between log entries. The default is 30 minutes + run: the number of
 log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
 total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
 cell temps. The default is 1 + save: name of a CSV file to write log data to +
 count: optional over-ride for the number of batteries This is an example of the
@@ -456,15 +457,17 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.20.
+(verbose) # Version Info 2.2.1.
+Ensure output is generated if get_battery() fails using battery_info(). Update
+f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

### Comparing `foxesscloud-2.2.0/README.md` & `foxesscloud-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -376,16 +376,16 @@
 
 ```
 f.battery_info(count, plot, log)
 f.battery_monitor(interval, run, log, save, count)
 ```
 
 battery_info() prints information on the battery and cells:
-+ count: optional over-ride. The default is based on rounding the battery voltage divided by 53
-+ plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
++ count: optional over-ride. The default is based on factorising the number of cells reported by 16 or 18 to work out the number of batteries.
++ plot: 1 plot the cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
 + log: see below. Default is 0
 
 battery_monitor() runs battery_info() in log mode on a schedule to provide information on the battery status over a period of time:
 + interval: the time in minutes between log entries. The default is 30 minutes
 + run: the number of log entries to create. The default is 48 i.e. every 30 minues for 24 hours in total
 + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The default is 1
 + save: name of a CSV file to write log data to
@@ -651,15 +651,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.20.<br>
+2.2.1.<br>
+Ensure output is generated if get_battery() fails using battery_info().
+Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
```

#### html2text {}

```diff
@@ -275,16 +275,17 @@
 [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
 This example shows the results reported by charge needed: ![image](https://
 github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
 20d806b1e7e8) ## Battery Info Provides detailed information on the current
 state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
 (interval, run, log, save, count) ``` battery_info() prints information on the
 battery and cells: + count: optional over-ride. The default is based on
-rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
-each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
 battery_monitor() runs battery_info() in log mode on a schedule to provide
 information on the battery status over a period of time: + interval: the time
 in minutes between log entries. The default is 30 minutes + run: the number of
 log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
 total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
 cell temps. The default is 1 + save: name of a CSV file to write log data to +
 count: optional over-ride for the number of batteries This is an example of the
@@ -449,15 +450,17 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.20.
+(verbose) # Version Info 2.2.1.
+Ensure output is generated if get_battery() fails using battery_info(). Update
+f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

### Comparing `foxesscloud-2.2.0/pyproject.toml` & `foxesscloud-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.0/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.1/src/foxesscloud/foxesscloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  09 April 2024
+Updated:  15 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.2"
+version = "1.3.3"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -2906,29 +2906,35 @@
 # Battery Info / Battery Monitor
 ##################################################################################################
 
 # calculate the average of a list of values
 def avg(x):
     if len(x) == 0:
         return None
-    return sum(x) / len(x)
+    count = 0
+    total = 0.0
+    for y in x:
+        if y is not None:
+            total += y
+            count += 1
+    return total / count if count > 0 else None
 
 # calculate the % imbalance in a list of values
 def imbalance(v):
     if len(v) == 0:
         return None
     max_v = max(v)
     min_v = min(v)
     return (max_v - min_v) / (max_v + min_v) * 200
 
 cells_per_battery = [16,18,15]      # allowed number of cells per battery
 
 # deduce the number of batteries from the number of cells
 def bat_count(cell_count):
-    global cell_per_battery
+    global cells_per_battery
     n = None
     for i in cells_per_battery:
         if cell_count % i == 0:
             n = i
             break
     if n is None:
         return None
@@ -2939,14 +2945,15 @@
 
 # show information about the current state of the batteries
 def battery_info(log=0, plot=1, count=None):
     global debug_setting, battery_info_app_key
     output_spool(battery_info_app_key)
     bat = get_battery()
     if bat is None:
+        output_close()
         return None
     bat_volt = bat['volt']
     current_soc = bat['soc']
     residual = bat['residual']
     bat_current = bat['current']
     bat_power = bat['power']
     bms_temperature = bat['temperature']
@@ -2963,15 +2970,15 @@
         return None
     nv_cell = int(nv / nbat + 0.5)
     cell_temps = get_cell_temps()
     if cell_temps is None:
         output_close()
         return None
     nt = len(cell_temps)
-    nt_cell = int(nt / nbat + 0.5)
+    nt_cell = int(nt / nbat)
     bat_cell_volts = []
     bat_cell_temps = []
     bat_volts = []
     bat_temps = []
     for i in range(0, nbat):
         bat_cell_volts.append(cell_volts[i * nv_cell : (i + 1) * nv_cell])
         bat_cell_temps.append(cell_temps[i * nt_cell : (i + 1) * nt_cell])
```

### Comparing `foxesscloud-2.2.0/src/foxesscloud/openapi.py` & `foxesscloud-2.2.1/src/foxesscloud/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  09 April 2024
+Updated:  15 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.0"
+version = "2.2.1"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -2775,29 +2775,35 @@
 # Battery Info / Battery Monitor
 ##################################################################################################
 
 # calculate the average of a list of values
 def avg(x):
     if len(x) == 0:
         return None
-    return sum(x) / len(x)
+    count = 0
+    total = 0.0
+    for y in x:
+        if y is not None:
+            total += y
+            count += 1
+    return total / count if count > 0 else None
 
 # calculate the % imbalance in a list of values
 def imbalance(v):
     if len(v) == 0:
         return None
     max_v = max(v)
     min_v = min(v)
     return (max_v - min_v) / (max_v + min_v) * 200
 
 cells_per_battery = [16,18,15]      # allowed number of cells per battery
 
 # deduce the number of batteries from the number of cells
 def bat_count(cell_count):
-    global cell_per_battery
+    global cells_per_battery
     n = None
     for i in cells_per_battery:
         if cell_count % i == 0:
             n = i
             break
     if n is None:
         return None
@@ -2808,14 +2814,15 @@
 
 # show information about the current state of the batteries
 def battery_info(log=0, plot=1, count=None):
     global debug_setting, battery_info_app_key
     output_spool(battery_info_app_key)
     bat = get_battery()
     if bat is None:
+        output_close()
         return None
     bat_volt = bat['volt']
     current_soc = bat['soc']
     residual = bat['residual']
     bat_current = bat['current']
     bat_power = bat['power']
     bms_temperature = bat['temperature']
@@ -2832,15 +2839,15 @@
         return None
     nv_cell = int(nv / nbat + 0.5)
     cell_temps = get_cell_temps()
     if cell_temps is None:
         output_close()
         return None
     nt = len(cell_temps)
-    nt_cell = int(nt / nbat + 0.5)
+    nt_cell = int(nt / nbat)
     bat_cell_volts = []
     bat_cell_temps = []
     bat_volts = []
     bat_temps = []
     for i in range(0, nbat):
         bat_cell_volts.append(cell_volts[i * nv_cell : (i + 1) * nv_cell])
         bat_cell_temps.append(cell_temps[i * nt_cell : (i + 1) * nt_cell])
```

### Comparing `foxesscloud-2.2.0/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.1/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.0
+Version: 2.2.1
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -390,16 +390,16 @@
 
 ```
 f.battery_info(count, plot, log)
 f.battery_monitor(interval, run, log, save, count)
 ```
 
 battery_info() prints information on the battery and cells:
-+ count: optional over-ride. The default is based on rounding the battery voltage divided by 53
-+ plot: 1 plot the cell voltages for each battery, 0 don't plot. The default is 1
++ count: optional over-ride. The default is based on factorising the number of cells reported by 16 or 18 to work out the number of batteries.
++ plot: 1 plot the cell voltages for each battery, 2 plot the cell temperatueres, 0 don't plot. The default is 1
 + log: see below. Default is 0
 
 battery_monitor() runs battery_info() in log mode on a schedule to provide information on the battery status over a period of time:
 + interval: the time in minutes between log entries. The default is 30 minutes
 + run: the number of log entries to create. The default is 48 i.e. every 30 minues for 24 hours in total
 + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add cell temps. The default is 1
 + save: name of a CSV file to write log data to
@@ -665,15 +665,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.20.<br>
+2.2.1.<br>
+Ensure output is generated if get_battery() fails using battery_info().
+Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
 Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in relation to work mode.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.0 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.1 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -282,16 +282,17 @@
 [51.30, 52.00, 52.30, 52.40, 52.50, 52.60, 52.70, 52.80, 52.9, 53.1, 53.50] ```
 This example shows the results reported by charge needed: ![image](https://
 github.com/TonyM1958/FoxESS-Cloud/assets/63789168/8b77956b-c326-43cd-b165-
 20d806b1e7e8) ## Battery Info Provides detailed information on the current
 state of the batteries: ``` f.battery_info(count, plot, log) f.battery_monitor
 (interval, run, log, save, count) ``` battery_info() prints information on the
 battery and cells: + count: optional over-ride. The default is based on
-rounding the battery voltage divided by 53 + plot: 1 plot the cell voltages for
-each battery, 0 don't plot. The default is 1 + log: see below. Default is 0
+factorising the number of cells reported by 16 or 18 to work out the number of
+batteries. + plot: 1 plot the cell voltages for each battery, 2 plot the cell
+temperatueres, 0 don't plot. The default is 1 + log: see below. Default is 0
 battery_monitor() runs battery_info() in log mode on a schedule to provide
 information on the battery status over a period of time: + interval: the time
 in minutes between log entries. The default is 30 minutes + run: the number of
 log entries to create. The default is 48 i.e. every 30 minues for 24 hours in
 total + log: 0 = display, 1 = log battery info, 2 = add cell volts, 3 = add
 cell temps. The default is 1 + save: name of a CSV file to write log data to +
 count: optional over-ride for the number of batteries This is an example of the
@@ -456,15 +457,17 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.20.
+(verbose) # Version Info 2.2.1.
+Ensure output is generated if get_battery() fails using battery_info(). Update
+f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
```

