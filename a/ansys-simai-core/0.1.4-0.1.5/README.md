# Comparing `tmp/ansys_simai_core-0.1.4.tar.gz` & `tmp/ansys_simai_core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_simai_core-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_simai_core-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_simai_core-0.1.4.tar` & `ansys_simai_core-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1089 2024-02-29 09:25:41.074142 ansys_simai_core-0.1.4/LICENSE
--rw-r--r--   0        0        0     5009 2024-02-29 09:25:41.074142 ansys_simai_core-0.1.4/README.rst
--rw-r--r--   0        0        0     4796 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1532 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/__init__.py
--rw-r--r--   0        0        0     1146 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/__init__.py
--rw-r--r--   0        0        0     2202 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/client.py
--rw-r--r--   0        0        0     2397 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/design_of_experiments.py
--rw-r--r--   0        0        0     5852 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/geometry.py
--rw-r--r--   0        0        0    10158 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/mixin.py
--rw-r--r--   0        0        0     1975 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/optimization.py
--rw-r--r--   0        0        0     4901 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/post_processing.py
--rw-r--r--   0        0        0     2650 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/prediction.py
--rw-r--r--   0        0        0     2707 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/project.py
--rw-r--r--   0        0        0     6030 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/sse.py
--rw-r--r--   0        0        0     2722 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/training_data.py
--rw-r--r--   0        0        0     2456 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/training_data_part.py
--rw-r--r--   0        0        0     3818 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/api/workspace.py
--rw-r--r--   0        0        0    12992 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/client.py
--rw-r--r--   0        0        0     1146 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/__init__.py
--rw-r--r--   0        0        0    12193 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/base.py
--rw-r--r--   0        0        0     3158 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/design_of_experiments.py
--rw-r--r--   0        0        0     2638 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/downloads.py
--rw-r--r--   0        0        0    22009 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/geometries.py
--rw-r--r--   0        0        0    11257 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/geometry_utils.py
--rw-r--r--   0        0        0     4766 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/lists.py
--rw-r--r--   0        0        0    10794 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/optimizations.py
--rw-r--r--   0        0        0    30612 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/post_processings.py
--rw-r--r--   0        0        0     9794 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/predictions.py
--rw-r--r--   0        0        0     4743 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/projects.py
--rw-r--r--   0        0        0     7571 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/selection_post_processings.py
--rw-r--r--   0        0        0     9701 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/selections.py
--rw-r--r--   0        0        0    11163 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/training_data.py
--rw-r--r--   0        0        0     2137 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/training_data_parts.py
--rw-r--r--   0        0        0     9460 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/types.py
--rw-r--r--   0        0        0     6541 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/data/workspaces.py
--rw-r--r--   0        0        0     4108 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/errors.py
--rw-r--r--   0        0        0        0 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/py.typed
--rw-r--r--   0        0        0     1146 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/__init__.py
--rw-r--r--   0        0        0     9373 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/auth.py
--rw-r--r--   0        0        0     4522 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/config_file.py
--rw-r--r--   0        0        0     4325 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/configuration.py
--rw-r--r--   0        0        0     2761 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/files.py
--rw-r--r--   0        0        0     5041 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/grouping.py
--rw-r--r--   0        0        0     1627 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/misc.py
--rw-r--r--   0        0        0     4132 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/numerical.py
--rw-r--r--   0        0        0     3903 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/requests.py
--rw-r--r--   0        0        0     3084 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/sse_client.py
--rw-r--r--   0        0        0     1643 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/typing.py
--rw-r--r--   0        0        0     2118 2024-02-29 09:25:41.078142 ansys_simai_core-0.1.4/src/ansys/simai/core/utils/validation.py
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5009 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/README.rst
+-rw-r--r--   0        0        0     4796 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1532 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/client.py
+-rw-r--r--   0        0        0     2397 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/design_of_experiments.py
+-rw-r--r--   0        0        0     5852 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/geometry.py
+-rw-r--r--   0        0        0    10158 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/mixin.py
+-rw-r--r--   0        0        0     1975 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/optimization.py
+-rw-r--r--   0        0        0     4901 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/post_processing.py
+-rw-r--r--   0        0        0     2650 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/prediction.py
+-rw-r--r--   0        0        0     3749 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/project.py
+-rw-r--r--   0        0        0     6030 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/sse.py
+-rw-r--r--   0        0        0     2903 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data.py
+-rw-r--r--   0        0        0     2456 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data_part.py
+-rw-r--r--   0        0        0     3818 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/api/workspace.py
+-rw-r--r--   0        0        0    13489 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/client.py
+-rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/__init__.py
+-rw-r--r--   0        0        0    12193 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/base.py
+-rw-r--r--   0        0        0     3158 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/design_of_experiments.py
+-rw-r--r--   0        0        0     2638 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/downloads.py
+-rw-r--r--   0        0        0    22009 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometries.py
+-rw-r--r--   0        0        0    11257 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometry_utils.py
+-rw-r--r--   0        0        0     4766 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/lists.py
+-rw-r--r--   0        0        0     4318 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/models.py
+-rw-r--r--   0        0        0    10813 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/optimizations.py
+-rw-r--r--   0        0        0    30612 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/post_processings.py
+-rw-r--r--   0        0        0     9794 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/predictions.py
+-rw-r--r--   0        0        0     6826 2024-04-15 16:25:29.006181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/projects.py
+-rw-r--r--   0        0        0     7571 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/selection_post_processings.py
+-rw-r--r--   0        0        0     9701 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/selections.py
+-rw-r--r--   0        0        0    11040 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data.py
+-rw-r--r--   0        0        0     2137 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data_parts.py
+-rw-r--r--   0        0        0     9460 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/types.py
+-rw-r--r--   0        0        0     6541 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/data/workspaces.py
+-rw-r--r--   0        0        0     4108 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/py.typed
+-rw-r--r--   0        0        0     1146 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/__init__.py
+-rw-r--r--   0        0        0     9373 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/auth.py
+-rw-r--r--   0        0        0     4522 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/config_file.py
+-rw-r--r--   0        0        0     5970 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/configuration.py
+-rw-r--r--   0        0        0     2761 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/files.py
+-rw-r--r--   0        0        0     5041 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/grouping.py
+-rw-r--r--   0        0        0     1627 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/misc.py
+-rw-r--r--   0        0        0     4132 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/numerical.py
+-rw-r--r--   0        0        0     3903 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/requests.py
+-rw-r--r--   0        0        0     3084 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/sse_client.py
+-rw-r--r--   0        0        0     1643 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/typing.py
+-rw-r--r--   0        0        0     2118 2024-04-15 16:25:29.010181 ansys_simai_core-0.1.5/src/ansys/simai/core/utils/validation.py
+-rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ansys_simai_core-0.1.5/PKG-INFO
```

### Comparing `ansys_simai_core-0.1.4/LICENSE` & `ansys_simai_core-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/README.rst` & `ansys_simai_core-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/pyproject.toml` & `ansys_simai_core-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Using PDM with flit backend
 [build-system]
 requires = ["flit_core>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-simai-core"
-version = "0.1.4"
+version = "0.1.5"
 description = "A python wrapper for Ansys SimAI"
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/__init__.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/__init__.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/client.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/design_of_experiments.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/design_of_experiments.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/geometry.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/geometry.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/mixin.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/mixin.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/optimization.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/optimization.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/post_processing.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/post_processing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/prediction.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/prediction.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/project.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,7 +62,32 @@
             f"projects/{project_id}/sample",
             json={"training_data": training_data_id},
             return_json=False,
         )
 
     def delete_project(self, project_id: str):
         self._delete(f"projects/{project_id}", return_json=False)
+
+    def launch_build(
+        self,
+        project_id: str,
+        config: Dict[str, Any],
+        dismiss_data_with_fields_discrepancies: bool = False,
+        dismiss_data_with_volume_overflow: bool = False,
+    ):
+        """Launches a build for a project and according to a given configuration.
+
+        Args:
+            project_id: the ID of the project
+            config: the build configuration
+            dismiss_data_with_fields_discrepancies: set to True for omitting data with missing properties
+            dismiss_data_with_volume_overflow: set to True for omitting data outside the Domain of Analysis
+
+        """
+        params = {
+            "dismiss_data_with_fields_discrepancies": dismiss_data_with_fields_discrepancies,
+            "dismiss_data_with_volume_overflow": dismiss_data_with_volume_overflow,
+        }
+        return self._post(f"projects/{project_id}/model", json=config, params=params)
+
+    def is_project_trainable(self, project_id: str):
+        return self._get(f"projects/{project_id}/trainable")
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/sse.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/sse.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/training_data.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,7 +58,10 @@
         return self._delete(
             f"training_data/{training_data_id}/project/{project_id}/association",
             return_json=False,
         )
 
     def compute_training_data(self, training_data_id: str) -> None:
         self._post(f"training_data/{training_data_id}/compute")
+
+    def get_training_data_subset(self, project_id: str, training_data_id: str) -> Dict[str, Any]:
+        return self._get(f"projects/{project_id}/data/{training_data_id}/subset")
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/training_data_part.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/training_data_part.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/api/workspace.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/api/workspace.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/client.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,26 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 from typing import List, Optional
 
+from pydantic import ValidationError
 from semver.version import Version
 
 from ansys.simai.core import __version__
 from ansys.simai.core.api.client import ApiClient
 from ansys.simai.core.data.design_of_experiments import DesignOfExperimentsCollection
 from ansys.simai.core.data.geometries import GeometryDirectory
-from ansys.simai.core.data.optimizations import OptimizationDirectory, OptimizationTrialRunDirectory
+from ansys.simai.core.data.models import ModelDirectory
+from ansys.simai.core.data.optimizations import (
+    OptimizationDirectory,
+    OptimizationTrialRunDirectory,
+)
 from ansys.simai.core.data.post_processings import PostProcessingDirectory
 from ansys.simai.core.data.predictions import PredictionDirectory
 from ansys.simai.core.data.projects import Project, ProjectDirectory
 from ansys.simai.core.data.training_data import TrainingDataDirectory
 from ansys.simai.core.data.training_data_parts import TrainingDataPartDirectory
 from ansys.simai.core.data.types import Path
 from ansys.simai.core.data.workspaces import Workspace, WorkspaceDirectory
@@ -64,24 +69,28 @@
             simai = SimAIClient(
                 organization="company_name", https_proxy="http://company_proxy:3128"
             )
     """
 
     @steal_kwargs_type(ClientConfig)
     def __init__(self, **kwargs):
-        config = ClientConfig(**kwargs)
+        try:
+            config = ClientConfig(**kwargs)
+        except ValidationError as pydandic_exc:
+            raise InvalidConfigurationError(pydandic_exc) from None
 
         api_client_class = getattr(config, "_api_client_class_override", ApiClient)
         self._api = api_client_class(simai_client=self, config=config)
         self._doe_collection = DesignOfExperimentsCollection(client=self)
         self._geometry_directory = GeometryDirectory(client=self)
         self._optimization_directory = OptimizationDirectory(client=self)
         self._optimization_trial_run_directory = OptimizationTrialRunDirectory(client=self)
         self._post_processing_directory = PostProcessingDirectory(client=self)
         self._project_directory = ProjectDirectory(client=self)
+        self._model_directory = ModelDirectory(client=self)
         self._workspace_directory = WorkspaceDirectory(client=self)
         self._prediction_directory = PredictionDirectory(client=self)
         self._training_data_directory = TrainingDataDirectory(client=self)
         self._training_data_part_directory = TrainingDataPartDirectory(client=self)
         self._current_workspace = None
         self._current_project = None
         if config.workspace is not None:
@@ -240,14 +249,21 @@
     @property
     def workspaces(self):
         """Representation of all workspaces on the server.
         For more information, see :ref:`workspaces`.
         """
         return self._workspace_directory
 
+    @property
+    def models(self):
+        """Representation of all workspaces on the server.
+        For more information, see :ref:`workspaces`.
+        """
+        return self._model_directory
+
     @classmethod
     def from_config(
         cls,
         profile: str = "default",
         path: Optional[Path] = None,
         **kwargs,
     ) -> "SimAIClient":
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/__init__.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/base.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/base.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/design_of_experiments.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/design_of_experiments.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/downloads.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/geometries.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometries.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/geometry_utils.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/lists.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/lists.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/optimizations.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/optimizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,28 +24,32 @@
 from typing import Callable, Dict, List, Optional, Tuple
 
 from tqdm import tqdm
 from wakepy import keep
 
 from ansys.simai.core.data.base import ComputableDataModel, Directory
 from ansys.simai.core.data.geometries import Geometry
-from ansys.simai.core.data.types import Identifiable, NamedFile, get_id_from_identifiable
+from ansys.simai.core.data.types import (
+    Identifiable,
+    NamedFile,
+    get_id_from_identifiable,
+)
 from ansys.simai.core.data.workspaces import Workspace
 from ansys.simai.core.errors import InvalidArguments
 
 logger = logging.getLogger(__name__)
 
 
 class Optimization(ComputableDataModel):
     """Provides the local representation of an optimization definition object."""
 
     def _try_geometry(
         self, geometry: Identifiable[Geometry], geometry_parameters: Dict
     ) -> "OptimizationTrialRun":
-        return self._client._optimization_trial_run_directory.try_geometry(
+        return self._client._optimization_trial_run_directory._try_geometry(
             self.id, geometry, geometry_parameters
         )
 
 
 class OptimizationTrialRun(ComputableDataModel):
     """Provides the local representation of an optimization trial run object.
 
@@ -196,15 +200,15 @@
                     geometry = self._client.geometries.upload(
                         generated_geometry,
                         metadata=geometry_parameters,
                         workspace_id=workspace_id,
                     )
                     logger.debug("Running trial.")
                     progress_bar.set_description("Running trial.")
-                    trial_run = optimization.try_geometry(geometry, geometry_parameters)
+                    trial_run = optimization._try_geometry(geometry, geometry_parameters)
                     trial_run.wait()
                     iteration_result = {
                         "parameters": geometry_parameters,
                         "objective": trial_run.fields["outcome_values"],
                     }
                     progress_bar.set_postfix(**iteration_result)
                     if trial_run.fields.get("is_feasible", True):
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/post_processings.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/post_processings.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/predictions.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/predictions.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/projects.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/projects.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,63 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, NamedTuple, Optional
 
 from ansys.simai.core.data.base import DataModel, Directory
+from ansys.simai.core.data.models import ModelConfiguration
 from ansys.simai.core.data.types import Identifiable, get_id_from_identifiable
 from ansys.simai.core.errors import InvalidArguments
 
 if TYPE_CHECKING:
     from ansys.simai.core.data.training_data import TrainingData
 
 
+class IsTrainableInfo(NamedTuple):
+    """Properties for project's trainability.
+
+    The objects of this class can be used as booleans
+    in condition statements as in the example:
+
+    Example:
+        Verify the project is trainable
+
+        .. code-block:: python
+
+            pt = my_project.is_trainable()
+
+            if pt:
+                print(pt)
+
+        It prints:
+
+        .. code-block:: shell
+
+            <is_trainable: False, reason(s): Not enough data to train a model: we need at least 3 data points to train a model.>
+
+    Attributes:
+        is_trainable (bool):    True if the project is trainable, False if it is not.
+        reason (str):           If not_trainable is False, the reason why the project is not trainable. None otherwise.
+
+    """
+
+    is_trainable: bool
+    reason: str = None
+
+    def __bool__(self) -> bool:
+        return self.is_trainable
+
+    def __repr__(self) -> str:
+        return f"<is_trainable: {self.is_trainable}, reason(s): {self.reason}>"
+
+
 class Project(DataModel):
     """Provides the local representation of a  project object."""
 
     def __repr__(self) -> str:
         return f"<Project: {self.id}, {self.name}>"
 
     @property
@@ -69,18 +108,40 @@
 
     @sample.setter
     def sample(self, new_sample: Identifiable["TrainingData"]):
         td_id = get_id_from_identifiable(new_sample)
         self._client._api.set_project_sample(self.id, td_id)
         self.reload()
 
+    @property
+    def last_model_configuration(self) -> ModelConfiguration:
+        """The last :class:`configuration <ansys.simai.core.data.models.ModelConfiguration>` that was used for training a model in this project."""
+        return ModelConfiguration(project_id=self.id, **self.fields.get("last_model_configuration"))
+
     def delete(self) -> None:
         """Delete the project."""
         self._client._api.delete_project(self.id)
 
+    def is_trainable(self) -> bool:
+        """Check if the project meets the prerequisites to be trained."""
+        tt = self._client._api.is_project_trainable(self.id)
+        return IsTrainableInfo(**tt)
+
+    def get_variables(self) -> dict[str, list[str]] | None:
+        """Get the available variables for the model's input/output."""
+        if not self.sample:
+            return None
+
+        sample_metadata = self.sample.fields.get("extracted_metadata")
+        data = {}
+        for key, vals in sample_metadata.items():
+            local_fields = vals.get("fields", [])
+            data[key] = [local_field.get("name") for local_field in local_fields]
+        return data
+
 
 class ProjectDirectory(Directory[Project]):
     """Provides a collection of methods related to projects.
 
     This class is accessed through ``client.projects``.
 
     Example:
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/selection_post_processings.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/selection_post_processings.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/selections.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/selections.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/training_data.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from ansys.simai.core.data.base import ComputableDataModel, Directory
 from ansys.simai.core.data.types import (
     Identifiable,
     MonitorCallback,
     NamedFile,
     Path,
     get_id_from_identifiable,
-    get_object_from_identifiable,
     unpack_named_file,
 )
 from ansys.simai.core.errors import InvalidArguments
 
 if TYPE_CHECKING:
     from ansys.simai.core.data.projects import Project
     from ansys.simai.core.data.training_data_parts import TrainingDataPart
@@ -82,20 +81,16 @@
         Args:
             project: ID or :class:`model <.projects.Project>` of the project to check
                 the :class:`~.projects.Project` object for, or its ID.
 
         Returns:
             Name of the subset that the training data belongs to in the given project.
         """
-        project_model = get_object_from_identifiable(
-            project, self._client.projects, default=self._client.current_project
-        )
-        for subset_name, list_ids in project_model.subsets:
-            if self.id in list_ids:
-                return subset_name
+        project_id = get_id_from_identifiable(project, default=self._client._current_project)
+        return self._client._api.get_training_data_subset(project_id, self.id).get("subset")
 
     @property
     def extracted_metadata(self) -> Optional[Dict]:
         """Metadata extracted from the training data."""
         return self.fields["extracted_metadata"]
 
     def compute(self) -> None:
```

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/training_data_parts.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/training_data_parts.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/types.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/types.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/data/workspaces.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/data/workspaces.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/errors.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/__init__.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/auth.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/config_file.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/config_file.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/files.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/grouping.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/grouping.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/misc.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/numerical.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/numerical.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/requests.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/requests.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/sse_client.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/typing.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/src/ansys/simai/core/utils/validation.py` & `ansys_simai_core-0.1.5/src/ansys/simai/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `ansys_simai_core-0.1.4/PKG-INFO` & `ansys_simai_core-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-simai-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python wrapper for Ansys SimAI
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

