# Comparing `tmp/furthrmind-0.1b1.tar.gz` & `tmp/furthrmind-0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furthrmind-0.1b1.tar", max compression
+gzip compressed data, was "furthrmind-0.1b2.tar", max compression
```

## Comparing `furthrmind-0.1b1.tar` & `furthrmind-0.1b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b1/LICENSE
--rwxr-xr-x   0        0        0     2899 2024-04-15 16:22:20.748563 furthrmind-0.1b1/README.md
--rwxr-xr-x   0        0        0     1876 2024-04-15 16:12:36.272916 furthrmind-0.1b1/furthrmind/__init__.py
--rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b1/furthrmind/collection/__init__.py
--rwxr-xr-x   0        0        0    19254 2024-04-15 16:12:36.344833 furthrmind-0.1b1/furthrmind/collection/baseclass.py
--rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b1/furthrmind/collection/category.py
--rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b1/furthrmind/collection/column.py
--rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b1/furthrmind/collection/comboboxentry.py
--rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b1/furthrmind/collection/datatable.py
--rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b1/furthrmind/collection/experiment.py
--rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b1/furthrmind/collection/field.py
--rwxr-xr-x   0        0        0    10119 2024-04-15 16:12:36.242521 furthrmind-0.1b1/furthrmind/collection/fielddata.py
--rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b1/furthrmind/collection/file.py
--rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b1/furthrmind/collection/group.py
--rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b1/furthrmind/collection/import_collection.py
--rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b1/furthrmind/collection/project.py
--rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b1/furthrmind/collection/researchitem.py
--rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b1/furthrmind/collection/sample.py
--rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b1/furthrmind/collection/unit.py
--rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b1/furthrmind/file_loader.py
--rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b1/furthrmind/utils.py
--rwxr-xr-x   0        0        0      723 2024-04-15 16:23:01.277524 furthrmind-0.1b1/pyproject.toml
--rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 furthrmind-0.1b1/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b2/LICENSE
+-rwxr-xr-x   0        0        0     2869 2024-04-15 16:25:04.221154 furthrmind-0.1b2/README.md
+-rwxr-xr-x   0        0        0     1876 2024-04-15 16:12:36.272916 furthrmind-0.1b2/furthrmind/__init__.py
+-rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b2/furthrmind/collection/__init__.py
+-rwxr-xr-x   0        0        0    19254 2024-04-15 16:12:36.344833 furthrmind-0.1b2/furthrmind/collection/baseclass.py
+-rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b2/furthrmind/collection/category.py
+-rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b2/furthrmind/collection/column.py
+-rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b2/furthrmind/collection/comboboxentry.py
+-rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b2/furthrmind/collection/datatable.py
+-rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b2/furthrmind/collection/experiment.py
+-rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b2/furthrmind/collection/field.py
+-rwxr-xr-x   0        0        0    10119 2024-04-15 16:12:36.242521 furthrmind-0.1b2/furthrmind/collection/fielddata.py
+-rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b2/furthrmind/collection/file.py
+-rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b2/furthrmind/collection/group.py
+-rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b2/furthrmind/collection/import_collection.py
+-rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b2/furthrmind/collection/project.py
+-rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b2/furthrmind/collection/researchitem.py
+-rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b2/furthrmind/collection/sample.py
+-rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b2/furthrmind/collection/unit.py
+-rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b2/furthrmind/file_loader.py
+-rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b2/furthrmind/utils.py
+-rwxr-xr-x   0        0        0      723 2024-04-15 16:28:01.241448 furthrmind-0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 furthrmind-0.1b2/PKG-INFO
```

### Comparing `furthrmind-0.1b1/LICENSE` & `furthrmind-0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/README.md` & `furthrmind-0.1b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 ## Basic usage
 
 Create an instance of the furthrmind class and pass the url to your server, your api key. 
 Optionally you can pass the project name or id of the project you would like to work with.
 
 ```
-from furthrmind_sdk.furthrmind import FURTHRmind
+from furthrmind import FURTHRmind
 fm = FURTHRmind(host, api_key, project_name="my project")
 ```
 
 In order to retrieve data, you have to import the corresponding collection class and call the
 get or get_all method. The method will return an instance / a list with instances of the 
 Experiment class. The instance of the experiment class will contain all data that belong to
 your experiment. Additionally, the experiment object has some convenient method for:
 add_field, add_many_fields, remove_field, update_field_value, update_field_unit, add_file, 
 remove_file, add_datatable
 
 ```
-furthrmind_sdk.collection import Experiment
+collection import Experiment
 exp_list = Experiment.get_all()
 ```
 
 To create a new experiment, you need to call the create() or create_many() method. Please 
 consider the correct input arguments for each collection class. For experiments, the create
 method expects to pass the new exp name and the name or id of the group that it should belong to. 
 If you want to add an experiment to a subgroup, you need to pass the id of this group. The
```

### Comparing `furthrmind-0.1b1/furthrmind/__init__.py` & `furthrmind-0.1b2/furthrmind/__init__.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/baseclass.py` & `furthrmind-0.1b2/furthrmind/collection/baseclass.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/category.py` & `furthrmind-0.1b2/furthrmind/collection/category.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/column.py` & `furthrmind-0.1b2/furthrmind/collection/column.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/comboboxentry.py` & `furthrmind-0.1b2/furthrmind/collection/comboboxentry.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/datatable.py` & `furthrmind-0.1b2/furthrmind/collection/datatable.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/experiment.py` & `furthrmind-0.1b2/furthrmind/collection/experiment.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/field.py` & `furthrmind-0.1b2/furthrmind/collection/field.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/fielddata.py` & `furthrmind-0.1b2/furthrmind/collection/fielddata.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/file.py` & `furthrmind-0.1b2/furthrmind/collection/file.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/group.py` & `furthrmind-0.1b2/furthrmind/collection/group.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/project.py` & `furthrmind-0.1b2/furthrmind/collection/project.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/researchitem.py` & `furthrmind-0.1b2/furthrmind/collection/researchitem.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/sample.py` & `furthrmind-0.1b2/furthrmind/collection/sample.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/collection/unit.py` & `furthrmind-0.1b2/furthrmind/collection/unit.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/file_loader.py` & `furthrmind-0.1b2/furthrmind/file_loader.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/furthrmind/utils.py` & `furthrmind-0.1b2/furthrmind/utils.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b1/pyproject.toml` & `furthrmind-0.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furthrmind"
-version = "0.1b1"
+version = "0.1b2"
 description = "Official python wrapper for the FURTHRmind rest api."
 authors = ["Daniel Menne"]
 license = "GNU GENERAL PUBLIC LICENSE Version 3"
 readme = "README.md"
 repository = "https://github.com/FURTHRresearch/furthrmind-sdk"
 
 [tool.poetry.dependencies]
```

### Comparing `furthrmind-0.1b1/PKG-INFO` & `furthrmind-0.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furthrmind
-Version: 0.1b1
+Version: 0.1b2
 Summary: Official python wrapper for the FURTHRmind rest api.
 Home-page: https://github.com/FURTHRresearch/furthrmind-sdk
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Author: Daniel Menne
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -31,27 +31,27 @@
 
 ## Basic usage
 
 Create an instance of the furthrmind class and pass the url to your server, your api key. 
 Optionally you can pass the project name or id of the project you would like to work with.
 
 ```
-from furthrmind_sdk.furthrmind import FURTHRmind
+from furthrmind import FURTHRmind
 fm = FURTHRmind(host, api_key, project_name="my project")
 ```
 
 In order to retrieve data, you have to import the corresponding collection class and call the
 get or get_all method. The method will return an instance / a list with instances of the 
 Experiment class. The instance of the experiment class will contain all data that belong to
 your experiment. Additionally, the experiment object has some convenient method for:
 add_field, add_many_fields, remove_field, update_field_value, update_field_unit, add_file, 
 remove_file, add_datatable
 
 ```
-furthrmind_sdk.collection import Experiment
+collection import Experiment
 exp_list = Experiment.get_all()
 ```
 
 To create a new experiment, you need to call the create() or create_many() method. Please 
 consider the correct input arguments for each collection class. For experiments, the create
 method expects to pass the new exp name and the name or id of the group that it should belong to. 
 If you want to add an experiment to a subgroup, you need to pass the id of this group. The
```

