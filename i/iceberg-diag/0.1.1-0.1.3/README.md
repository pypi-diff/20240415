# Comparing `tmp/iceberg_diag-0.1.1.tar.gz` & `tmp/iceberg_diag-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg_diag-0.1.1.tar", max compression
+gzip compressed data, was "iceberg_diag-0.1.3.tar", max compression
```

## Comparing `iceberg_diag-0.1.1.tar` & `iceberg_diag-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2024-01-29 10:14:36.487779 iceberg_diag-0.1.1/LICENSE
--rw-r--r--   0        0        0     2426 2024-02-04 08:36:24.256047 iceberg_diag-0.1.1/README.md
--rw-r--r--   0        0        0       84 2024-02-02 14:42:34.387856 iceberg_diag-0.1.1/icebergdiag/__init__.py
--rw-r--r--   0        0        0     8048 2024-02-04 08:39:29.459751 iceberg_diag-0.1.1/icebergdiag/cli.py
--rw-r--r--   0        0        0        0 2024-01-29 10:14:36.488312 iceberg_diag-0.1.1/icebergdiag/diagnostics/__init__.py
--rw-r--r--   0        0        0     6079 2024-02-04 08:35:57.327054 iceberg_diag-0.1.1/icebergdiag/diagnostics/manager.py
--rw-r--r--   0        0        0     1223 2024-02-01 16:31:24.840365 iceberg_diag-0.1.1/icebergdiag/diagnostics/requester.py
--rw-r--r--   0        0        0     3785 2024-02-02 09:54:31.118015 iceberg_diag-0.1.1/icebergdiag/diagnostics/response.py
--rw-r--r--   0        0        0     3305 2024-02-04 08:35:15.374603 iceberg_diag-0.1.1/icebergdiag/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-29 10:14:36.488934 iceberg_diag-0.1.1/icebergdiag/metrics/__init__.py
--rw-r--r--   0        0        0      659 2024-02-02 09:54:31.118752 iceberg_diag-0.1.1/icebergdiag/metrics/table.py
--rw-r--r--   0        0        0     6196 2024-02-02 09:54:31.119249 iceberg_diag-0.1.1/icebergdiag/metrics/table_metric.py
--rw-r--r--   0        0        0     8647 2024-02-02 11:12:31.424532 iceberg_diag-0.1.1/icebergdiag/metrics/table_metrics.py
--rw-r--r--   0        0        0     1602 2024-01-29 10:14:36.489494 iceberg_diag-0.1.1/icebergdiag/metrics/table_metrics_displayer.py
--rw-r--r--   0        0        0     1972 2024-02-04 07:46:56.307451 iceberg_diag-0.1.1/icebergdiag/utils.py
--rw-r--r--   0        0        0      710 2024-02-04 08:21:56.046117 iceberg_diag-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3277 1970-01-01 00:00:00.000000 iceberg_diag-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-29 10:14:36.487779 iceberg_diag-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2468 2024-04-15 12:29:04.592228 iceberg_diag-0.1.3/README.md
+-rw-r--r--   0        0        0       84 2024-02-02 14:42:34.387856 iceberg_diag-0.1.3/icebergdiag/__init__.py
+-rw-r--r--   0        0        0     8520 2024-04-15 13:32:57.762385 iceberg_diag-0.1.3/icebergdiag/cli.py
+-rw-r--r--   0        0        0        0 2024-01-29 10:14:36.488312 iceberg_diag-0.1.3/icebergdiag/diagnostics/__init__.py
+-rw-r--r--   0        0        0     7901 2024-04-15 14:39:25.549076 iceberg_diag-0.1.3/icebergdiag/diagnostics/manager.py
+-rw-r--r--   0        0        0     1831 2024-04-15 12:29:04.593438 iceberg_diag-0.1.3/icebergdiag/diagnostics/requester.py
+-rw-r--r--   0        0        0     3785 2024-02-02 09:54:31.118015 iceberg_diag-0.1.3/icebergdiag/diagnostics/response.py
+-rw-r--r--   0        0        0     3568 2024-04-15 12:29:04.593778 iceberg_diag-0.1.3/icebergdiag/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-29 10:14:36.488934 iceberg_diag-0.1.3/icebergdiag/metrics/__init__.py
+-rw-r--r--   0        0        0      659 2024-02-02 09:54:31.118752 iceberg_diag-0.1.3/icebergdiag/metrics/table.py
+-rw-r--r--   0        0        0     6196 2024-02-02 09:54:31.119249 iceberg_diag-0.1.3/icebergdiag/metrics/table_metric.py
+-rw-r--r--   0        0        0     8647 2024-02-02 11:12:31.424532 iceberg_diag-0.1.3/icebergdiag/metrics/table_metrics.py
+-rw-r--r--   0        0        0     1602 2024-01-29 10:14:36.489494 iceberg_diag-0.1.3/icebergdiag/metrics/table_metrics_displayer.py
+-rw-r--r--   0        0        0     1972 2024-04-14 15:15:22.316705 iceberg_diag-0.1.3/icebergdiag/utils.py
+-rw-r--r--   0        0        0      710 2024-04-15 14:46:23.010938 iceberg_diag-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 iceberg_diag-0.1.3/PKG-INFO
```

### Comparing `iceberg_diag-0.1.1/LICENSE` & `iceberg_diag-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/README.md` & `iceberg_diag-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 - `-h`, `--help`: Display the help message and exit.
 - `--profile PROFILE`: Set the AWS credentials profile for the session, defaults to the environment's current settings.
 - `--region REGION`: Set the AWS region for operations, defaults to the specified profile's default region.
 - `--database DATABASE`: Set the database name, will list all available iceberg tables if no `--table-name` provided.
 - `--table-name TABLE_NAME`: Enter the table name or a glob pattern (e.g., `'*'`, `'tbl_*'`).
 - `--remote`: Enable remote diagnostics by sending data to the Upsolver API for processing.   
 Provides more detailed analytics and includes information about file size reducations.
+- `-v, --verbose`: Enable verbose logging
 
 ### Usage
 1. Displaying help information:
     ```bash
      iceberg-diag --help
     ```
```

### Comparing `iceberg_diag-0.1.1/icebergdiag/cli.py` & `iceberg_diag-0.1.3/icebergdiag/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import logging
+import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import partial
 from typing import List, Callable, Any, Tuple
 
 from rich import box
 from rich.console import Console
 from rich.logging import RichHandler
@@ -14,30 +15,42 @@
 from icebergdiag.diagnostics.requester import DiagnosticsRequester
 from icebergdiag.diagnostics.response import DiagnosticsResponse
 from icebergdiag.exceptions import TableMetricsCalculationError, IcebergDiagnosticsError, RequestHandlingError
 from icebergdiag.metrics.table import Table
 from icebergdiag.metrics.table_metrics import TableMetrics
 from icebergdiag.metrics.table_metrics_displayer import TableMetricsDisplayer, RunMode
 
-logging.basicConfig(
-    level="ERROR",
-    format="%(message)s",
-    handlers=[RichHandler(rich_tracebacks=False, show_path=False)]
-)
+
+def configure_logging(verbose=False):
+    logging.basicConfig(
+        level="ERROR",
+        format="%(message)s",
+        handlers=[RichHandler(rich_tracebacks=True, show_path=False)]
+    )
+    if verbose:
+        logging.getLogger().setLevel(logging.INFO)
+        os.environ['S3FS_LOGGING_LEVEL'] = 'DEBUG'
+        debug_loggers = ['icebergdiag', 'pyiceberg']
+        for logger_name in debug_loggers:
+            logging.getLogger(logger_name).setLevel(logging.DEBUG)
+
+
+logger = logging.getLogger(__name__)
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog='iceberg-diag',
         description='Iceberg Diagnostics Tool')
     parser.add_argument('--profile', type=str, help='AWS profile name')
     parser.add_argument('--region', type=str, help='AWS region')
     parser.add_argument('--database', type=str, help='Database name')
     parser.add_argument('--table-name', type=str, help="Table name or glob pattern (e.g., '*', 'tbl_*')")
     parser.add_argument('--remote', action='store_true', help='Use remote diagnostics')
+    parser.add_argument('-v', '--verbose', action='store_true', help='Enable debug logs')
     return parser.parse_args()
 
 
 def stderr_print(stderr_message: str) -> None:
     Console(stderr=True).print(stderr_message, style="yellow")
 
 
@@ -159,16 +172,16 @@
         displayer.display_metrics(table_result.metrics, RunMode.REMOTE)
         failed_tables.extend(table_result.extract_errors())
 
     process_tables(diagnostics_manager, database, table_pattern, metric_function, result_handler)
 
 
 def cli_runner() -> None:
-    logger = logging.getLogger(__name__)
     args = parse_arguments()
+    configure_logging(args.verbose)
     try:
         diagnostics_manager = run_with_progress(IcebergDiagnosticsManager, "Initializing...",
                                                 profile=args.profile, region=args.region)
 
         if args.database is None:
             list_databases(diagnostics_manager)
         elif args.table_name is None:
```

### Comparing `iceberg_diag-0.1.1/icebergdiag/diagnostics/manager.py` & `iceberg_diag-0.1.3/icebergdiag/diagnostics/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,101 @@
 import fnmatch
+import logging
+import traceback
 from itertools import chain
 from typing import List, Iterable, Dict, Any, Optional, Tuple
 
 import boto3
 import botocore.exceptions as boto3_exceptions
 from botocore.client import BaseClient
 from botocore.config import Config
 from pyiceberg.catalog import load_glue, Catalog
 from pyiceberg.catalog.glue import GlueCatalog
-from pyiceberg.io import PY_IO_IMPL, FSSPEC_FILE_IO
 from pyiceberg.manifest import DataFile
 from pyiceberg.table import Table as IcebergTable, _open_manifest
 from pyiceberg.utils.concurrent import ExecutorFactory
 
 from icebergdiag.exceptions import ProfileNotFoundError, EndpointConnectionError, \
     IcebergDiagnosticsError, DatabaseNotFound, TableMetricsCalculationError, SSOAuthenticationError, \
     SessionInitializationError
 from icebergdiag.metrics.table import Table
 from icebergdiag.metrics.table_metrics import TableMetrics, MetricsCalculator
 
-CATALOG_CONFIG = {PY_IO_IMPL: FSSPEC_FILE_IO}
+logger = logging.getLogger(__name__)
 
 
 class IcebergDiagnosticsManager:
     def __init__(self, profile: str, region: Optional[str] = None):
+        logger.debug(f"Initializing with profile={profile}, region={region if region else 'default'}")
         self.profile = profile
         self.region = region
         self._initialize_catalog()
 
     def _initialize_catalog(self):
+        logger.debug("Starting catalog initialization")
         try:
             self._validate()
+            self.session = boto3.Session(profile_name=self.profile, region_name=self.region)
+            credentials = self.session.get_credentials().get_frozen_credentials()
             self.catalog = load_glue(name="glue",
-                                     conf={"profile_name": self.profile, "region_name": self.region, **CATALOG_CONFIG})
+                                     conf={"profile_name": self.profile,
+                                           "region_name": self.session.region_name,
+                                           "aws_access_key_id": credentials.access_key,
+                                           "aws_secret_access_key": credentials.secret_key,
+                                           "aws_session_token": credentials.token,
+                                           "s3.access-key-id": credentials.access_key,
+                                           "s3.secret-access-key": credentials.secret_key,
+                                           "s3.session-token": credentials.token,
+                                           "s3.region": self.session.region_name,
+                                           })
             self.glue_client = IcebergDiagnosticsManager._get_glue_client(self.catalog)
-            self.session = boto3.Session(profile_name=self.profile, region_name=self.region)
+            logger.debug("Glue Catalog initialized successfully")
         except boto3_exceptions.ProfileNotFound:
             raise ProfileNotFoundError(self.profile)
         except boto3_exceptions.EndpointConnectionError:
             raise EndpointConnectionError(self.region)
         except boto3_exceptions.SSOError as e:
             raise SSOAuthenticationError(self.profile, e) from e
         except boto3_exceptions.BotoCoreError as e:
             raise SessionInitializationError(self.profile, e)
         except Exception as e:
             raise IcebergDiagnosticsError(f"An unexpected error occurred: {e}")
 
     def _validate(self):
+        logger.debug("Validating session")
         try:
             session = boto3.Session(profile_name=self.profile, region_name=self.region)
             temp_config = Config(retries={'max_attempts': 1})
             temp_glue_client = session.client('glue', config=temp_config)
             temp_glue_client.get_databases(MaxResults=1)
+            logger.debug("Session validated successfully")
         except Exception as e:
             raise e
 
     def list_databases(self) -> List[str]:
         databases = self.catalog.list_namespaces()
         return sorted([db[0] for db in databases])
 
     def list_tables(self, database: str) -> List[str]:
         try:
             return self._fetch_and_filter_tables(database)
         except self.glue_client.exceptions.EntityNotFoundException as e:
             raise DatabaseNotFound(database) from e
 
     def get_matching_tables(self, database: str, search_pattern: str) -> List[str]:
+        logger.debug(f"Searching for tables in database '{database}' with pattern '{search_pattern}'")
         all_tables = self.list_tables(database)
         return fnmatch.filter(all_tables, search_pattern)
 
     def calculate_metrics(self, table: Table) -> TableMetrics:
+        logger.debug(f"Calculating metrics for table: '{table}'", )
         try:
             return TableDiagnostics(self.catalog, table).get_metrics()
         except Exception as e:
+            logger.debug(f"Failed to Calculate metrics: {''.join(traceback.format_exception(e))}")
             raise TableMetricsCalculationError(table, e)
 
     def _fetch_and_filter_tables(self, database: str) -> List[str]:
         next_token = None
         iceberg_tables = []
         while True:
             params = {'DatabaseName': database}
@@ -125,36 +144,43 @@
         self.catalog = catalog
 
     def get_metrics(self) -> TableMetrics:
         metrics = MetricsCalculator.compute_metrics(*self._get_manifest_files())
         return TableMetrics(self.table, metrics)
 
     def _load_table(self) -> IcebergTable:
+        logger.debug(f"Loading table {self.table.full_table_name()}")
         return self.catalog.load_table(self.table.full_table_name())
 
     def _get_manifest_files(self) -> Tuple[Iterable[DataFile], int]:
+        logger.debug(f"Getting manifest files for table '{self.table}'")
         """Returns a list of all data files in manifest entries.
 
         Returns:
             Iterable of DataFile objects.
         """
+
         def no_filter(_):
             return True
 
         table = self._load_table()
+        logger.debug(f"Scanning table: {self.table.full_table_name()}")
         scan = table.scan()
+        logger.debug(f"Loading snapshot for table {self.table.full_table_name()}")
         snapshot = scan.snapshot()
         if not snapshot:
             return iter([]), 0
 
         io = table.io
+        logger.debug(f"Opening manifests files for table {self.table.full_table_name()}")
         manifests = snapshot.manifests(io)
         executor = ExecutorFactory.get_or_create()
         all_data_files = []
         for manifest_entry in chain(
                 *executor.map(
                     lambda manifest: _open_manifest(io, manifest, no_filter, no_filter),
                     manifests
                 )):
             all_data_files.append(manifest_entry.data_file)
 
+        logger.debug(f"All data loaded successfully for table {self.table.full_table_name()}")
         return all_data_files, len(manifests)
```

### Comparing `iceberg_diag-0.1.1/icebergdiag/diagnostics/requester.py` & `iceberg_diag-0.1.3/icebergdiag/diagnostics/requester.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,46 @@
+import logging
 from typing import Dict, Any, List
 
 import requests
 
 from icebergdiag.diagnostics.response import DiagnosticsResponse, parse_response
-from icebergdiag.exceptions import RequestHandlingError
+from icebergdiag.exceptions import RequestHandlingError, ParsingResponseError
 from icebergdiag.metrics.table import Table
 
+logger = logging.getLogger(__name__)
+
 
 class DiagnosticsRequester:
     METRICS_URL = "https://iceberg-auditor.upsolver.com/v2/wizards/optimizer/cli-analyze"
 
     def __init__(self, url: str = METRICS_URL):
         self.url = url
 
     def request_metrics(self, session_info: Dict[str, Any],
                         tables: List[Table]) -> DiagnosticsResponse:
         requested_tables = [table.full_table_name() for table in tables]
+        logger.debug(f"Preparing to send metrics request for tables: {', '.join(requested_tables)}")
         result = self._post({**session_info, "tables": requested_tables})
-        parsed_result = self._parse_response(result)
+        parsed_result = self._parse_response(result, requested_tables)
+
+        logger.debug(f"Received and parsed metrics for tables successfully.")
         return parsed_result
 
     def _post(self, data: Dict[str, Any]) -> Dict[str, Any]:
         try:
             response = requests.post(self.url, json=data)
             response.raise_for_status()
+            logger.debug("HTTP POST request successful, parsing response.")
             return response.json()
         except requests.RequestException as e:
             raise RequestHandlingError(data["tables"], e)
 
     @staticmethod
-    def _parse_response(data: Dict[str, Any]) -> DiagnosticsResponse:
-        return parse_response(data)
+    def _parse_response(data: Dict[str, Any], tables: List[str]) -> DiagnosticsResponse:
+        logger.debug("Parsing response data")
+        try:
+            response = parse_response(data)
+            logger.debug(f"Response parsed successfully")
+            return response
+        except Exception as e:
+            raise ParsingResponseError(data, tables, e)
```

### Comparing `iceberg_diag-0.1.1/icebergdiag/diagnostics/response.py` & `iceberg_diag-0.1.3/icebergdiag/diagnostics/response.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/icebergdiag/exceptions.py` & `iceberg_diag-0.1.3/icebergdiag/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Dict, Any
 
 import requests
 
 from icebergdiag.metrics.table import Table
 
 
 class IcebergDiagnosticsError(Exception):
@@ -42,14 +42,15 @@
     def __init__(self, region: Optional[str]):
         region_message = f"region '{region}'" if region is not None else "default region"
         super().__init__(f"Could not connect to AWS in the {region_message}.")
 
 
 class SessionInitializationError(IcebergDiagnosticsError):
     """Exception raised when an AWS session fails to initialize."""
+
     def __init__(self, profile: Optional[str], original_error: Exception):
         profile_part = f"with profile '{profile}'" if profile else "with default profile"
         message = f"Failed to initialize AWS session {profile_part}: {original_error}"
         super().__init__(message)
 
 
 class UnexpectedError(IcebergDiagnosticsError):
@@ -80,7 +81,12 @@
 
     def __init__(self, table_names: List[str], error: requests.RequestException):
         if isinstance(error, requests.HTTPError):
             message = str(error).split(" for url:")[0]
         else:
             message = f'An error occurred during the request for tables {table_names}: {error.__class__.__name__}'
         super().__init__(message)
+
+
+class ParsingResponseError(IcebergDiagnosticsError):
+    def __init__(self, data: Dict[str, Any], table_names: List[str], error: Exception):
+        super().__init__(f"Failed to parse diagnostics response {data} for tables: {table_names}: {error}")
```

### Comparing `iceberg_diag-0.1.1/icebergdiag/metrics/table.py` & `iceberg_diag-0.1.3/icebergdiag/metrics/table.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/icebergdiag/metrics/table_metric.py` & `iceberg_diag-0.1.3/icebergdiag/metrics/table_metric.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/icebergdiag/metrics/table_metrics.py` & `iceberg_diag-0.1.3/icebergdiag/metrics/table_metrics.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/icebergdiag/metrics/table_metrics_displayer.py` & `iceberg_diag-0.1.3/icebergdiag/metrics/table_metrics_displayer.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/icebergdiag/utils.py` & `iceberg_diag-0.1.3/icebergdiag/utils.py`

 * *Files identical despite different names*

### Comparing `iceberg_diag-0.1.1/pyproject.toml` & `iceberg_diag-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iceberg-diag"
-version = "0.1.1"
+version = "0.1.3"
 description = "Upsolver Iceberg Auditor CLI"
 authors = ["Upsolver <developers@upsolver.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Upsolver/iceberg-diag"
```

### Comparing `iceberg_diag-0.1.1/PKG-INFO` & `iceberg_diag-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-diag
-Version: 0.1.1
+Version: 0.1.3
 Summary: Upsolver Iceberg Auditor CLI
 Home-page: https://github.com/Upsolver/iceberg-diag
 License: MIT
 Author: Upsolver
 Author-email: developers@upsolver.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -70,14 +70,15 @@
 - `-h`, `--help`: Display the help message and exit.
 - `--profile PROFILE`: Set the AWS credentials profile for the session, defaults to the environment's current settings.
 - `--region REGION`: Set the AWS region for operations, defaults to the specified profile's default region.
 - `--database DATABASE`: Set the database name, will list all available iceberg tables if no `--table-name` provided.
 - `--table-name TABLE_NAME`: Enter the table name or a glob pattern (e.g., `'*'`, `'tbl_*'`).
 - `--remote`: Enable remote diagnostics by sending data to the Upsolver API for processing.   
 Provides more detailed analytics and includes information about file size reducations.
+- `-v, --verbose`: Enable verbose logging
 
 ### Usage
 1. Displaying help information:
     ```bash
      iceberg-diag --help
     ```
```

