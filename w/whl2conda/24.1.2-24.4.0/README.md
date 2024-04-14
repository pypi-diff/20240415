# Comparing `tmp/whl2conda-24.1.2.tar.gz` & `tmp/whl2conda-24.4.0.tar.gz`

## Comparing `whl2conda-24.1.2.tar` & `whl2conda-24.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/VERSION
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/__about__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/py.typed
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/api/__init__.py
--rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/api/converter.py
--rw-r--r--   0        0        0    34643 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/api/stdrename.json
--rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/api/stdrename.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/__init__.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/build.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/common.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/config.py
--rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/convert.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/diff.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/cli/main.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/external/__init__.py
--rw-r--r--   0        0        0    26218 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/external/version.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/impl/__init__.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/impl/download.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/impl/prompt.py
--rw-r--r--   0        0        0     9907 2020-02-02 00:00:00.000000 whl2conda-24.1.2/src/whl2conda/impl/pyproject.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 whl2conda-24.1.2/.gitignore
--rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 whl2conda-24.1.2/LICENSE.md
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 whl2conda-24.1.2/README.md
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 whl2conda-24.1.2/pyproject.toml
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 whl2conda-24.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/VERSION
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__about__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/py.typed
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/__init__.py
+-rw-r--r--   0        0        0    33693 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/converter.py
+-rw-r--r--   0        0        0    34867 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/stdrename.json
+-rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/stdrename.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/build.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/common.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/config.py
+-rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/convert.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/diff.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/install.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/main.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/external/__init__.py
+-rw-r--r--   0        0        0    26218 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/external/version.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/__init__.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/download.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/prompt.py
+-rw-r--r--   0        0        0     9907 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/pyproject.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/wheel.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 whl2conda-24.4.0/.gitignore
+-rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 whl2conda-24.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 whl2conda-24.4.0/README.md
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 whl2conda-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 whl2conda-24.4.0/PKG-INFO
```

### Comparing `whl2conda-24.1.2/src/whl2conda/__about__.py` & `whl2conda-24.4.0/src/whl2conda/__about__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/__init__.py` & `whl2conda-24.4.0/src/whl2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/__main__.py` & `whl2conda-24.4.0/src/whl2conda/__main__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/api/__init__.py` & `whl2conda-24.4.0/src/whl2conda/api/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/api/converter.py` & `whl2conda-24.4.0/src/whl2conda/api/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 import time
 from dataclasses import dataclass
 from hashlib import sha256
 from pathlib import Path
 from typing import Any, NamedTuple, Optional, Sequence
 
 # third party
-from wheel.wheelfile import WheelFile
 from conda_package_handling.api import create as create_conda_pkg
 
 # this project
 from ..__about__ import __version__
 from ..impl.prompt import bool_input
 from ..impl.pyproject import CondaPackageFormat
+from ..impl.wheel import unpack_wheel
 from .stdrename import load_std_renames
 
 __all__ = [
     "CondaPackageFormat",
     "DependencyRename",
     "Wheel2CondaConverter",
     "Wheel2CondaError",
@@ -292,15 +292,14 @@
     }
 
     package_name: str = ""
     logger: logging.Logger
     wheel_path: Path
     out_dir: Path
     dry_run: bool = False
-    wheel: Optional[WheelFile]
     out_format: CondaPackageFormat = CondaPackageFormat.V2
     overwrite: bool = False
     keep_pip_dependencies: bool = False
     dependency_rename: list[DependencyRename]
     extra_dependencies: list[str]
     python_version: str = ""
     interactive: bool = False
@@ -881,21 +880,16 @@
             else:
                 self._warn("Cannot convert bad version spec: '%s'", spec)
 
         return ",".join(filter(bool, version_specs))
 
     def _extract_wheel(self, temp_dir: Path) -> Path:
         self.logger.info("Reading %s", self.wheel_path)
-        wheel = WheelFile(self.wheel_path)
         wheel_dir = temp_dir / "wheel-files"
-        wheel.extractall(wheel_dir)
-        if self.logger.getEffectiveLevel() <= logging.DEBUG:
-            for wheel_file in wheel_dir.glob("**/*"):
-                if wheel_file.is_file():
-                    self._debug("Extracted %s", wheel_file.relative_to(wheel_dir))
+        unpack_wheel(self.wheel_path, wheel_dir, logger=self.logger)
         return wheel_dir
 
     def _warn(self, msg, *args):
         self.logger.warning(msg, *args)
 
     def _info(self, msg, *args):
         self.logger.info(msg, *args)
```

### Comparing `whl2conda-24.1.2/src/whl2conda/api/stdrename.json` & `whl2conda-24.4.0/src/whl2conda/api/stdrename.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992196209587514%*

 * *Differences: {"'$date'": "'Sun, 28 Jan 2024 17:38:56 GMT'",*

 * * "'$etag'": "'f5d7c0bdb46b34790aa49f1ee2b4b393ec7af5bc331e9551d81a08278f30537d'",*

 * * "'conda-subprocess'": "'conda_subprocess'",*

 * * "'lightgbm-ray'": "'lightgbm_ray'",*

 * * "'s1-frame-enumerator'": "'s1_frame_enumerator'",*

 * * "'simple-template'": "'simple_template'",*

 * * "'tile-mate'": "'tile_mate'",*

 * * "'xgboost-ray'": "'xgboost_ray'"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "$date": "Mon, 15 Jan 2024 23:42:57 GMT",
-    "$etag": "f925d70019e5918474b0c1796a45888d954c367c2f6c34687274fa83a17456f8",
+    "$date": "Sun, 28 Jan 2024 17:38:56 GMT",
+    "$etag": "f5d7c0bdb46b34790aa49f1ee2b4b393ec7af5bc331e9551d81a08278f30537d",
     "$max-age": "300",
     "$source": "https://raw.githubusercontent.com/regro/cf-graph-countyfair/master/mappings/pypi/name_mapping.json",
     "0164e082b29777fbc56c2373b68da93d23a29a040787e7f1c65e1562f133": "django-jsoneditor",
     "33162c0a7b28a4d8c83da07bc2b12cee58c120b4a9e8bba31c41c8d35a16": "vcversioner",
     "9e118aa3f6684187e7ba3727864cfd8e8209ad2d4c59b668f1d41e76f241": "pyelastix",
     "acrv-datasets": "acrv_datasets",
     "aiida-wannier90-workflows": "aiida-wannier90_workflows",
@@ -177,14 +177,15 @@
     "compas-occ": "compas_occ",
     "compas-rrc": "compas_rrc",
     "compas-skeleton": "compas_skeleton",
     "compas-slicer": "compas_slicer",
     "compas-tna": "compas_tna",
     "compas-view2": "compas_view2",
     "compress-json": "compress_json",
+    "conda-subprocess": "conda_subprocess",
     "connection-pool": "connection_pool",
     "constructive-geometries": "constructive_geometries",
     "contact-map": "contact_map",
     "contrib-colormaps": "contrib_colormaps",
     "cookiecutter-project-upgrader": "cookiecutter_project_upgrader",
     "coreapi": "python-coreapi",
     "coreschema": "python-coreschema",
@@ -461,14 +462,15 @@
     "lazy-loader": "lazy_loader",
     "lazy-table": "lazy_table",
     "lcov-cobertura": "lcov_cobertura",
     "leveldb": "python-leveldb",
     "libaio": "python-libaio",
     "libarchive-c": "python-libarchive-c",
     "libsvm": "libsvm-python",
+    "lightgbm-ray": "lightgbm_ray",
     "liknorm": "liknorm-py",
     "linear-operator": "linear_operator",
     "lit": "lit-nlp",
     "log-symbols": "log_symbols",
     "logging-exceptions": "logging_exceptions",
     "logging-tree": "logging_tree",
     "lpython-emulation": "lpython_emulation",
@@ -738,14 +740,15 @@
     "retry-decorator": "retry_decorator",
     "reverse-geocoder": "reverse_geocoder",
     "ribs": "pyribs-base",
     "robot-descriptions": "robot_descriptions",
     "ruamel-yaml": "ruamel_yaml",
     "ruamel-yaml-jinja2": "ruamel.yaml.jinja2",
     "s-gd2": "s_gd2",
+    "s1-frame-enumerator": "s1_frame_enumerator",
     "sagemaker": "sagemaker-python-sdk",
     "sagemaker-containers": "sagemaker_containers",
     "sagemaker-mxnet-training": "sagemaker_mxnet_container",
     "sagemaker-pyspark": "sagemaker_pyspark",
     "sas-kernel": "sas_kernel",
     "scanning-drift-corr": "scanning_drift_corr",
     "scikits-odes": "scikits.odes",
@@ -758,14 +761,15 @@
     "semantic-version": "semantic_version",
     "setuptools-dso": "setuptools_dso",
     "setuptools-markdown": "setuptools_markdown",
     "setuptools-scm-git-archive": "setuptools_scm_git_archive",
     "simple-benchmark": "simple_benchmark",
     "simple-h5py": "simple_h5py",
     "simple-slurm": "simple_slurm",
+    "simple-template": "simple_template",
     "smartystreets-python-sdk": "smartystreets_python_sdk",
     "solar-system-ephemerides": "solar_system_ephemerides",
     "solvation-analysis": "solvation_analysis",
     "sound-field-analysis": "sound_field_analysis",
     "sounddevice": "python-sounddevice",
     "soundfile": "pysoundfile",
     "sourmash": "sourmash-minimal",
@@ -809,14 +813,15 @@
     "termstyle": "python-termstyle",
     "testflows-asserts": "testflows.asserts",
     "tethys-dask-scheduler": "tethys_dask_scheduler",
     "tethys-dataset-services": "tethys_dataset_services",
     "text-models": "text_models",
     "thrift-sasl": "thrift_sasl",
     "tidy-headers": "tidy_headers",
+    "tile-mate": "tile_mate",
     "tiledb": "tiledb-py",
     "toolbox-utils": "toolbox_utils",
     "torch": "pytorch",
     "torch-cluster": "pytorch_cluster",
     "torch-geometric": "pytorch_geometric",
     "torch-scatter": "pytorch_scatter",
     "torch-sparse": "pytorch_sparse",
@@ -865,14 +870,15 @@
     "wq-io": "wq.io",
     "wwt-api-client": "wwt_api_client",
     "wwt-data-formats": "wwt_data_formats",
     "wwt-jupyterlab-extension": "wwt_jupyterlab_extension",
     "wwt-kernel-data-relay": "wwt_kernel_data_relay",
     "xarray-leaflet": "xarray_leaflet",
     "xarray-mongodb": "xarray_mongodb",
+    "xgboost-ray": "xgboost_ray",
     "xxhash": "python-xxhash",
     "yggdrasil-framework": "yggdrasil",
     "yoda-tools": "yodatools",
     "zc-buildout": "zc.buildout",
     "zc-lockfile": "zc.lockfile",
     "zc-recipe-egg": "zc.recipe.egg",
     "zenodo-backpack": "zenodo_backpack",
```

### Comparing `whl2conda-24.1.2/src/whl2conda/api/stdrename.py` & `whl2conda-24.4.0/src/whl2conda/api/stdrename.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/__init__.py` & `whl2conda-24.4.0/src/whl2conda/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/build.py` & `whl2conda-24.4.0/src/whl2conda/cli/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             pkg = self._build_package(wheel)
             if not self.args.no_test:
                 self._test_package(pkg)
             self._install_package(pkg)
         finally:
             self._cleanup()
         end = time.time()
-        print(f"Elapsed time: {end-start:f} seconds")
+        print(f"Elapsed time: {end - start:f} seconds")
 
     def _render_recipe(self):
         conda_bld = get_conda_bld_path()
         with tempfile.TemporaryDirectory(prefix="whl2conda-build-") as tmpdir:
             tmp_recipe_file = Path(tmpdir) / "meta.yaml"
             cmd = [
                 "conda",
```

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/common.py` & `whl2conda-24.4.0/src/whl2conda/cli/common.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/config.py` & `whl2conda-24.4.0/src/whl2conda/cli/config.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/convert.py` & `whl2conda-24.4.0/src/whl2conda/cli/convert.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/diff.py` & `whl2conda-24.4.0/src/whl2conda/cli/diff.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/install.py` & `whl2conda-24.4.0/src/whl2conda/cli/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,25 +282,34 @@
 
             if parsed.dry_run:
                 # dry run of a package file install fails in conda
                 print("Running ", install_pkg_cmd)
             else:
                 subprocess.check_call(install_pkg_cmd)
 
-        # Workaround for https://github.com/conda/conda/issues/13479
-        # If a package is installed directly from file, then set solver to classic
-        set_solver_cmd = (
-            ["conda", "run"]
-            + env_opts
-            + ["conda", "config", "--env", "--set", "solver", "classic"]
-        )
+        check_libmamba_cmd = "conda list -n base conda-libmamba-solver --json".split()
         if parsed.dry_run:
-            print("Running ", set_solver_cmd)
+            print("running ", check_libmamba_cmd)
         else:
-            subprocess.check_call(set_solver_cmd)
+            jsonstr = subprocess.check_output(check_libmamba_cmd, encoding="utf-8")
+            jobj = json.loads(jsonstr)
+            version_str = jobj and jobj[0].get("version")
+            version = tuple(int(s) for s in version_str.split("."))
+            if version < (24, 1, 0):
+                # Workaround for https://github.com/conda/conda/issues/13479
+                # If a package is installed directly from file, then set solver to classic
+                set_solver_cmd = (
+                    ["conda", "run"]
+                    + env_opts
+                    + ["conda", "config", "--env", "--set", "solver", "classic"]
+                )
+                if parsed.dry_run:
+                    print("Running ", set_solver_cmd)
+                else:
+                    subprocess.check_call(set_solver_cmd)
 
 
 conda_depend_re = re.compile(r"\s*(?P<name>[\w\d.-]+)\s*(?P<version>.*)")
 
 
 def _prune_dependencies(
     dependencies: list[str], file_specs: list[InstallFileInfo]
```

### Comparing `whl2conda-24.1.2/src/whl2conda/cli/main.py` & `whl2conda-24.4.0/src/whl2conda/cli/main.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/external/__init__.py` & `whl2conda-24.4.0/src/whl2conda/external/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/external/version.py` & `whl2conda-24.4.0/src/whl2conda/external/version.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/impl/__init__.py` & `whl2conda-24.4.0/src/whl2conda/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/impl/download.py` & `whl2conda-24.4.0/src/whl2conda/impl/download.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/impl/prompt.py` & `whl2conda-24.4.0/src/whl2conda/impl/prompt.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/src/whl2conda/impl/pyproject.py` & `whl2conda-24.4.0/src/whl2conda/impl/pyproject.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/LICENSE.md` & `whl2conda-24.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/README.md` & `whl2conda-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `whl2conda-24.1.2/pyproject.toml` & `whl2conda-24.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -72,60 +72,14 @@
 [[tool.mypy.overrides]]
 module = [
     "conda_package_handling.*",
     "wheel.*"
 ]
 ignore_missing_imports = true
 
-[tool.pylint.main]
-ignore-paths=['^src/whl2conda/external/.*$']
-
-[tool.pylint.build_main]
-jobs = 0  # enable parallel checks
-py-version = "3.8" # min python version
-source-roots = ["src"]
-
-[tool.pylint.design]
-max-args = 5
-max-attributes = 20
-max-bool-expr = 5
-max-branches = 12
-max-locals = 15
-max-parents = 7
-max-public-methods = 20
-max-returns = 6
-max-statements = 50
-min-public-methods = 1
-
-[tool.pylint.similarities]
-min-similarity-lines = 6
-
-[tool.pylint.variables]
-allowed-redefined-builtins = ["help", "license"]
-
-[tool.pylint."messages control"]
-disable = [
-    "bad-inline-option",
-    "deprecated-pragma",
-    "file-ignored",
-    "fixme",
-    "invalid-name",
-    "line-too-long",
-    "locally-disabled",
-    "raw-checker-failed",
-    "suppressed-message",
-    "too-many-arguments",
-    "trailing-newlines",
-    "unspecified-encoding",
-    "use-dict-literal",
-    "use-symbolic-message-instead",
-    "useless-suppression",
-    "wrong-import-order"
-]
-
 [tool.ruff]
 line-length = 88
 exclude = [
     "src/whl2conda/external"
 ]
 
 [tool.ruff.format]
```

### Comparing `whl2conda-24.1.2/PKG-INFO` & `whl2conda-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: whl2conda
-Version: 24.1.2
+Version: 24.4.0
 Summary: Build conda packages directly from pure python wheels
 Project-URL: homepage, https://github.com/analog-cbarber/whl2conda
 Project-URL: repository, https://github.com/analog-cbarber/whl2conda
 Project-URL: documentation, https://zuzukin.github.io/whl2conda/
 Author-email: Christopher Barber <christopher.barber@analog.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
```

