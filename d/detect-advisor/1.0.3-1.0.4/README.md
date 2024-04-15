# Comparing `tmp/detect_advisor-1.0.3.tar.gz` & `tmp/detect_advisor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detect_advisor-1.0.3.tar", last modified: Sat Apr  6 17:28:23 2024, max compression
+gzip compressed data, was "detect_advisor-1.0.4.tar", last modified: Mon Apr 15 11:25:57 2024, max compression
```

## Comparing `detect_advisor-1.0.3.tar` & `detect_advisor-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:23.723386 detect_advisor-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-06 17:28:23.723386 detect_advisor-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:23.723386 detect_advisor-1.0.3/detect_advisor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/global_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    14507 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/detect_advisor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:28:23.723386 detect_advisor-1.0.3/detect_advisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-06 17:28:23.000000 detect_advisor-1.0.3/detect_advisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-06 17:28:23.000000 detect_advisor-1.0.3/detect_advisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:28:23.000000 detect_advisor-1.0.3/detect_advisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 17:28:23.000000 detect_advisor-1.0.3/detect_advisor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 17:28:23.000000 detect_advisor-1.0.3/detect_advisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-06 17:28:19.000000 detect_advisor-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:28:23.723386 detect_advisor-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/detect_advisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/global_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/detect_advisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/setup.cfg
```

### Comparing `detect_advisor-1.0.3/LICENSE` & `detect_advisor-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/PKG-INFO` & `detect_advisor-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detect_advisor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Detect Advisor - prescan project folders to determine how to scan with Detect
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/detect_advisor
 Project-URL: Issues, https://github.com/matthewb66/detect_advisor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `detect_advisor-1.0.3/README.md` & `detect_advisor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/detect_advisor/config.py` & `detect_advisor-1.0.4/detect_advisor/config.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/detect_advisor/global_values.py` & `detect_advisor-1.0.4/detect_advisor/global_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # Constants
-advisor_version = "1.0.3"
+advisor_version = "1.0.4"
 detect_version = "9.X.0"
 
 ext_list = {
     'src': ['.4th', '.actionscript', '.ada', '.adb', '.ads', '.aidl', '.as', '.as8', '.asm', '.asp', '.aspx', '.aug',
             '.awk', '.bas', '.bash', '.bat', '.bf', '.bfpp', '.bi', '.bms', '.bmx', '.boo', '.c', '.c#', '.c++',
             '.cbl', '.cc', '.cfc', '.cfm', '.cgi', '.chai', '.clj', '.cljc', '.cljs', '.cls', '.cmd', '.com', '.cpp',
             '.cpy', '.cs', '.cu', '.cuh', '.cxx', '.d', '.dpk', '.dylan', '.e', '.ec', '.eh', '.el', '.erl', '.es',
```

### Comparing `detect_advisor-1.0.3/detect_advisor/main.py` & `detect_advisor-1.0.4/detect_advisor/main.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/detect_advisor/messages.py` & `detect_advisor-1.0.4/detect_advisor/messages.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/detect_advisor/output.py` & `detect_advisor-1.0.4/detect_advisor/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     summary += "--------------------  --------------   --------------   -------------   -------------   -------------\n"
 
     summary += global_values.rep + "\n"
 
     print(summary)
     if reportfile is not None:
-        with open(reportfile, "wa") as repfile:
+        with open(reportfile, "a") as repfile:
             repfile.write(summary)
 
 
 def output_full_rep(reportfile):
 
     rep = "\n\n" + global_values.full_rep + "\n\n"
 
@@ -142,15 +142,15 @@
     }
     for ftype in desc.keys():
         rep += desc[ftype] + '\n' + "\n".join(global_values.file_list[ftype]) + '\n\n'
 
     print(rep)
 
     if reportfile is not None:
-        with open(reportfile, "wa") as repfile:
+        with open(reportfile, "a") as repfile:
             repfile.write(rep)
 
 
 def output_recs(critical_only, reportfile):
     # global global_values.messages
 
     text = global_values.messages
@@ -179,15 +179,15 @@
 
     if critical_only and not global_values.recs_msgs_dict['crit']:
         text += ("- No Critical Recommendations\n")
 
     print(text)
 
     if reportfile is not None:
-        with open(reportfile, "wa") as repfile:
+        with open(reportfile, "a") as repfile:
             repfile.write(text)
 
 
 def output_cli(critical_only, reportfile):
     output = "+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++\n\nDETECT CLI:\n\n"
     if global_values.recs_msgs_dict['crit']:
         output += "Note that scan will probably fail - see CRITICAL recommendations above\n\n"
@@ -225,15 +225,15 @@
         if global_values.cli_msgs_dict['rep'] != '':
             output += "\nREPORTING OPTIONS:\n" + global_values.cli_msgs_dict['rep'] + "\n"
 
     print(output)
 
     if reportfile is not None:
         output = re.sub(r"^", "    ", output, flags=re.MULTILINE)
-        with open(reportfile, "wa") as repfile:
+        with open(reportfile, "a") as repfile:
             repfile.write(output)
 
 
 def output_config(projdir):
     config_file = os.path.join(projdir, "application-project.yml")
     if not os.path.exists(config_file):
         config = "#\n# EXAMPLE PROJECT CONFIG FILE\n" + \
```

### Comparing `detect_advisor-1.0.3/detect_advisor/process.py` & `detect_advisor-1.0.4/detect_advisor/process.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.3/detect_advisor.egg-info/PKG-INFO` & `detect_advisor-1.0.4/detect_advisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detect_advisor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Detect Advisor - prescan project folders to determine how to scan with Detect
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/detect_advisor
 Project-URL: Issues, https://github.com/matthewb66/detect_advisor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `detect_advisor-1.0.3/pyproject.toml` & `detect_advisor-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "detect_advisor"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Matthew Brady", email="mbrad@synopsys.com" },
 ]
 description = "Detect Advisor - prescan project folders to determine how to scan with Detect"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

