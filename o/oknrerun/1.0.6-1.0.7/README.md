# Comparing `tmp/oknrerun-1.0.6.tar.gz` & `tmp/oknrerun-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oknrerun-1.0.6.tar", last modified: Tue Jan 30 23:52:13 2024, max compression
+gzip compressed data, was "oknrerun-1.0.7.tar", last modified: Mon Apr 15 00:54:10 2024, max compression
```

## Comparing `oknrerun-1.0.6.tar` & `oknrerun-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 23:52:13.115653 oknrerun-1.0.6/
--rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 oknrerun-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       22 2023-12-15 00:27:56.000000 oknrerun-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3956 2024-01-30 23:52:13.114656 oknrerun-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3156 2024-01-24 03:18:41.000000 oknrerun-1.0.6/README.md
--rw-rw-rw-   0        0        0     1118 2024-01-30 23:51:20.000000 oknrerun-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-30 23:52:13.115653 oknrerun-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-30 23:52:13.030316 oknrerun-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-01-30 23:52:13.086730 oknrerun-1.0.6/src/oknrerun/
--rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknrerun-1.0.6/src/oknrerun/__init__.py
--rw-rw-rw-   0        0        0     6263 2023-05-17 08:39:07.000000 oknrerun-1.0.6/src/oknrerun/gazefilters.json
--rw-rw-rw-   0        0        0      341 2023-12-05 23:15:22.000000 oknrerun-1.0.6/src/oknrerun/okn_detection_rule.json
--rw-rw-rw-   0        0        0    13419 2023-11-08 00:58:16.000000 oknrerun-1.0.6/src/oknrerun/okndetector.gaze.config
--rw-rw-rw-   0        0        0    44675 2024-01-30 23:48:38.000000 oknrerun-1.0.6/src/oknrerun/oknrerun.py
--rw-rw-rw-   0        0        0     5913 2023-11-27 07:18:06.000000 oknrerun-1.0.6/src/oknrerun/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0      260 2023-12-03 22:22:17.000000 oknrerun-1.0.6/src/oknrerun/opm_detector_config.json
--rw-rw-rw-   0        0        0       33 2023-12-16 22:17:29.000000 oknrerun-1.0.6/src/oknrerun/ui.py
-drwxrwxrwx   0        0        0        0 2024-01-30 23:52:13.113658 oknrerun-1.0.6/src/oknrerun.egg-info/
--rw-rw-rw-   0        0        0     3956 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      112 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-01-30 23:52:13.000000 oknrerun-1.0.6/src/oknrerun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.979021 oknrerun-1.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 22:17:50.000000 oknrerun-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       22 2024-04-14 22:17:50.000000 oknrerun-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4623 2024-04-15 00:54:10.976490 oknrerun-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2024-04-14 22:17:50.000000 oknrerun-1.0.7/README.md
+-rw-rw-rw-   0        0        0     1118 2024-04-15 00:50:57.000000 oknrerun-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:54:10.979021 oknrerun-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.926352 oknrerun-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.949354 oknrerun-1.0.7/src/oknrerun/
+-rw-rw-rw-   0        0        0        0 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/__init__.py
+-rw-rw-rw-   0        0        0     6263 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/gazefilters.json
+-rw-rw-rw-   0        0        0      341 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/okn_detection_rule.json
+-rw-rw-rw-   0        0        0    13419 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/okndetector.gaze.config
+-rw-rw-rw-   0        0        0    44772 2024-04-15 00:49:51.000000 oknrerun-1.0.7/src/oknrerun/oknrerun.py
+-rw-rw-rw-   0        0        0     5913 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0      260 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/opm_detector_config.json
+-rw-rw-rw-   0        0        0       33 2024-04-14 22:17:50.000000 oknrerun-1.0.7/src/oknrerun/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:54:10.975493 oknrerun-1.0.7/src/oknrerun.egg-info/
+-rw-rw-rw-   0        0        0     4623 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 00:54:10.000000 oknrerun-1.0.7/src/oknrerun.egg-info/top_level.txt
```

### Comparing `oknrerun-1.0.6/LICENSE` & `oknrerun-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.6/PKG-INFO` & `oknrerun-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknrerun
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python program to rerun eye health diagnostic group's recording data
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/oknrerun
 Project-URL: Bug Tracker, https://github.com/jtur044/oknrerun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -55,25 +55,37 @@
 pip install -U oknrerun
 ```
 
 ## Usage
 We can rerun a recording folder with or without pupil detector.
 ### Without pupil detector
 ```
-oknrerun -d (directory to recording folder to be rerun) -okndl (directory to okndetector)
+oknrerun -d (directory to recording folder to be rerun)
 ```
 ### With pupil detector
 ```
-oknrerun -d (directory to recording folder to be rerun) -okndl (directory to okndetector) -pd (type or indicator)
+oknrerun -d (directory to recording folder to be rerun) -pd (type or indicator)
 ```
 #### type or indicator
 Type = type of pupil detector such as **opm** and **plm**.  
 Note: Currently there is only **opm** type.  
 Indicator = **on**, **y**, **1** or **true**.  
 
+### Configuration usage priority
+oknrerun will use config files inside the rerun recording folder if there is no optional flags/arguments input.  
+If it could not find valid config files inside the rerun recording folder then it will use built-in configs.  
+
+#### Valid config file name
+1. For updater config, its name must contain **gazefilter**.
+2. For okndetector config, its name must contain **okndetector**.
+3. For plot info config, its name must contain **plot**.
+4. For rule info config, its name must contain **oknserver_config** or **rule**.  
+
+If you do not want to use configs inside rerun recording foler or defaults/built-in configs, then you use **optional flags/arguments** such as **-uc** and **-okndc**.
+
 ### Optional flags/arguments
 1.  **-uc** (directory to updater config(gazefilters.json))
 2.  **-okndc** (directory to okn detector config(okndetector.gaze.config))
 3.  **-pi** (directory to plot info(oknserver_graph_plot_config.json))
 4.  **-ri** (directory to rule info(the config file which include rules))
 5.  **-bl** (buffer length of tiny fill buffer to be used with pupil detector). Default is 7.  
 6.  **-opmdc** (directory to opm detector config(opm_detector_config.json))
```

### Comparing `oknrerun-1.0.6/pyproject.toml` & `oknrerun-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "oknrerun"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python program to rerun eye health diagnostic group's recording data"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "numpy", "commentjson", "scipy", "matplotlib", "ehdg_tools>=4.0.8", "ehdg_pupil_detector", "okntool", "opencv-python"]
 classifiers = [
```

### Comparing `oknrerun-1.0.6/src/oknrerun/gazefilters.json` & `oknrerun-1.0.7/src/oknrerun/gazefilters.json`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.6/src/oknrerun/okndetector.gaze.config` & `oknrerun-1.0.7/src/oknrerun/okndetector.gaze.config`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.6/src/oknrerun/oknrerun.py` & `oknrerun-1.0.7/src/oknrerun/oknrerun.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,16 @@
 
 
 # This function is copy all the data inside from the input directory excluding the folder from ignore folder array.
 # It ignores to copy the files inside, but it creates the directory for it.
 # Because we do not want to copy unnecessary files.
 def copy_folder_with_ignore_folder(copy_dir, paste_dir, ignore_folder_array):
     file_folder_list = os.listdir(copy_dir)
+    if not os.path.isdir(paste_dir):
+        os.mkdir(paste_dir)
     for file_folder in file_folder_list:
         first_letter = str(file_folder).lower()[0]
         if first_letter == ".":
             pass
         else:
             copy_path = os.path.join(copy_dir, file_folder)
             paste_path = os.path.join(paste_dir, file_folder)
@@ -463,15 +465,15 @@
         return
     output_csv_dir = os.path.join(trial_folder_dir, f"{trial_name}.csv")
     redetect(detector, buffer, trial_video_dir, output_csv_dir, event_id_input, direction_input)
 
     return output_csv_dir
 
 
-# This function is to find the file name in the config folder
+# This function is to find the file name with the given search strings in the config folder
 def get_config_name(config_folder_input, search_string, search_string_two=None):
     file_list = os.listdir(config_folder_input)
     if search_string_two:
         for file_name in file_list:
             if str(search_string) in str(file_name) or str(search_string_two) in str(file_name):
                 file_path = os.path.join(config_folder_input, file_name)
                 if os.path.isfile(file_path):
```

### Comparing `oknrerun-1.0.6/src/oknrerun/oknserver_graph_plot_config.json` & `oknrerun-1.0.7/src/oknrerun/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `oknrerun-1.0.6/src/oknrerun.egg-info/PKG-INFO` & `oknrerun-1.0.7/src/oknrerun.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknrerun
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python program to rerun eye health diagnostic group's recording data
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/oknrerun
 Project-URL: Bug Tracker, https://github.com/jtur044/oknrerun/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -55,25 +55,37 @@
 pip install -U oknrerun
 ```
 
 ## Usage
 We can rerun a recording folder with or without pupil detector.
 ### Without pupil detector
 ```
-oknrerun -d (directory to recording folder to be rerun) -okndl (directory to okndetector)
+oknrerun -d (directory to recording folder to be rerun)
 ```
 ### With pupil detector
 ```
-oknrerun -d (directory to recording folder to be rerun) -okndl (directory to okndetector) -pd (type or indicator)
+oknrerun -d (directory to recording folder to be rerun) -pd (type or indicator)
 ```
 #### type or indicator
 Type = type of pupil detector such as **opm** and **plm**.  
 Note: Currently there is only **opm** type.  
 Indicator = **on**, **y**, **1** or **true**.  
 
+### Configuration usage priority
+oknrerun will use config files inside the rerun recording folder if there is no optional flags/arguments input.  
+If it could not find valid config files inside the rerun recording folder then it will use built-in configs.  
+
+#### Valid config file name
+1. For updater config, its name must contain **gazefilter**.
+2. For okndetector config, its name must contain **okndetector**.
+3. For plot info config, its name must contain **plot**.
+4. For rule info config, its name must contain **oknserver_config** or **rule**.  
+
+If you do not want to use configs inside rerun recording foler or defaults/built-in configs, then you use **optional flags/arguments** such as **-uc** and **-okndc**.
+
 ### Optional flags/arguments
 1.  **-uc** (directory to updater config(gazefilters.json))
 2.  **-okndc** (directory to okn detector config(okndetector.gaze.config))
 3.  **-pi** (directory to plot info(oknserver_graph_plot_config.json))
 4.  **-ri** (directory to rule info(the config file which include rules))
 5.  **-bl** (buffer length of tiny fill buffer to be used with pupil detector). Default is 7.  
 6.  **-opmdc** (directory to opm detector config(opm_detector_config.json))
```

### Comparing `oknrerun-1.0.6/src/oknrerun.egg-info/SOURCES.txt` & `oknrerun-1.0.7/src/oknrerun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

