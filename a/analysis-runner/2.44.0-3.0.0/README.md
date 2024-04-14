# Comparing `tmp/analysis-runner-2.44.0.tar.gz` & `tmp/analysis-runner-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-runner-2.44.0.tar", last modified: Tue Mar  5 20:59:48 2024, max compression
+gzip compressed data, was "analysis-runner-3.0.0.tar", last modified: Sun Apr 14 23:15:22 2024, max compression
```

## Comparing `analysis-runner-2.44.0.tar` & `analysis-runner-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:59:48.351670 analysis-runner-2.44.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-03-05 20:59:48.351670 analysis-runner-2.44.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:59:48.347670 analysis-runner-2.44.0/analysis_runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2125 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cli_analysisrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cli_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25771 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/analysis_runner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:59:48.351670 analysis-runner-2.44.0/analysis_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-05 20:59:48.000000 analysis-runner-2.44.0/analysis_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 20:59:48.351670 analysis-runner-2.44.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:59:48.351670 analysis-runner-2.44.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-03-05 20:59:47.000000 analysis-runner-2.44.0/test/test_analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:15:22.561691 analysis-runner-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-14 23:15:22.557691 analysis-runner-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:15:22.557691 analysis-runner-3.0.0/analysis_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2146 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/cli_analysisrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/cli_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/analysis_runner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:15:22.557691 analysis-runner-3.0.0/analysis_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 23:15:22.000000 analysis-runner-3.0.0/analysis_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:15:22.561691 analysis-runner-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:15:22.557691 analysis-runner-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-14 23:15:21.000000 analysis-runner-3.0.0/test/test_analysis_runner.py
```

### Comparing `analysis-runner-2.44.0/LICENSE` & `analysis-runner-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.44.0/PKG-INFO` & `analysis-runner-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.44.0
+Version: 3.0.0
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.44.0/README.md` & `analysis-runner-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.44.0/analysis_runner/cli.py` & `analysis-runner-3.0.0/analysis_runner/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 
 """
 CLI for interfacing with deployed analysis runner.
 See README.md for more information.
 """
-from typing import Dict, Tuple, Callable
-
-import sys
 import argparse
+import sys
+from typing import Callable, Sequence
 
 from analysis_runner._version import __version__
 from analysis_runner.cli_analysisrunner import (
     add_analysis_runner_args,
     run_analysis_runner_from_args,
 )
-from analysis_runner.cli_cromwell import add_cromwell_args, run_cromwell_from_args
 from analysis_runner.cli_config import add_config_args, run_config_from_args
+from analysis_runner.cli_cromwell import add_cromwell_args, run_cromwell_from_args
 
 
-def main_from_args(args=None):
+def main_from_args(args: Sequence[str] | None = None):
     """
     Parse args using argparse
     (if args is None, argparse automatically uses `sys.argv`)
     """
     parser = argparse.ArgumentParser()
     # https://docs.python.org/dev/library/argparse.html#action
 
@@ -30,15 +29,15 @@
         '-v',
         '--version',
         action='version',
         version=f'analysis-runner v{__version__}',
     )
 
     default_mode = 'analysis-runner'
-    modes: Dict[str, Tuple[Callable[[], argparse.ArgumentParser], Callable]] = {
+    modes: dict[str, tuple[Callable[[], argparse.ArgumentParser], Callable]] = {
         'analysis-runner': (add_analysis_runner_args, run_analysis_runner_from_args),
         'cromwell': (add_cromwell_args, run_cromwell_from_args),
         'config': (add_config_args, run_config_from_args),
     }
 
     args = args or sys.argv[1:]
 
@@ -57,15 +56,15 @@
 optional positional arguments:
   [{{{cs_modekeys},version,help}}]
     DEFAULT = analysis-runner
 
 optional arguments:
   -h, --help       show this help message and exit
   -v, --version    display the version and exit
-"""
+""",
         )
         return
     if mode in ('-v', '--version', 'version'):
         print(f'analysis-runner v{__version__}')
         return
 
     if mode not in modes:
```

### Comparing `analysis-runner-2.44.0/analysis_runner/cli_analysisrunner.py` & `analysis-runner-3.0.0/analysis_runner/cli_analysisrunner.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 
 import argparse
 import os
 from shutil import which
 from typing import List, Optional
 
 import requests
+
+from analysis_runner.util import (
+    _perform_version_check,
+    add_general_args,
+    confirm_choice,
+    get_server_endpoint,
+    logger,
+)
 from cpg_utils.cloud import get_google_identity_token
 from cpg_utils.config import read_configs
-
-from analysis_runner.constants import get_server_endpoint
-from analysis_runner.git import (
+from cpg_utils.git import (
     check_if_commit_is_on_remote,
     get_git_branch_name,
     get_git_commit_ref_of_current_repository,
     get_git_default_remote,
     get_relative_path_from_git_root,
     get_repo_name_from_remote,
 )
-from analysis_runner.util import (
-    _perform_version_check,
-    add_general_args,
-    confirm_choice,
-    logger,
-)
 
 
-def add_analysis_runner_args(parser=None) -> argparse.ArgumentParser:
+def add_analysis_runner_args(
+    parser: Optional[argparse.ArgumentParser] = None,
+) -> argparse.ArgumentParser:
     """
     Add CLI arguments for standard analysis-runner
     """
     if not parser:
         parser = argparse.ArgumentParser('analysis-runner subparser')
 
     add_general_args(parser)
@@ -95,20 +97,20 @@
     )
 
     parser.add_argument('script', nargs=argparse.REMAINDER, default=[])
 
     return parser
 
 
-def run_analysis_runner_from_args(args):
+def run_analysis_runner_from_args(args: argparse.ArgumentParser):
     """Run analysis runner from argparse.parse_arguments"""
     return run_analysis_runner(**vars(args))
 
 
-def run_analysis_runner(  # pylint: disable=too-many-arguments
+def run_analysis_runner(  # noqa: C901
     dataset: str,
     output_dir: str,
     script: List[str],
     description: str,
     access_level: str,
     commit: Optional[str] = None,
     repository: Optional[str] = None,
@@ -117,34 +119,33 @@
     cpu: Optional[str] = None,
     memory: Optional[str] = None,
     storage: Optional[str] = None,
     preemptible: Optional[str] = None,
     branch: Optional[str] = None,
     config: Optional[List[str]] = None,
     env: Optional[List[str]] = None,
-    use_test_server=False,
-    server_url=None,
+    use_test_server: bool = False,
+    server_url: Optional[str] = None,
 ):
     """
     Main function that drives the CLI.
     """
 
     if repository is not None and commit is None:
         raise ValueError(
             "You must supply the '--commit <SHA>' parameter "
-            "when specifying the '--repository'"
+            "when specifying the '--repository'",
         )
 
     _perform_version_check()
 
-    if access_level == 'full':
-        if not confirm_choice(
-            'Full access increases the risk of accidental data loss. Continue?',
-        ):
-            raise SystemExit()
+    if access_level == 'full' and not confirm_choice(
+        'Full access increases the risk of accidental data loss. Continue?',
+    ):
+        raise SystemExit
 
     _repository = repository
     _commit_ref = commit
     _branch = branch or get_git_branch_name()
     _script = list(script)
     _cwd = cwd
 
@@ -170,55 +171,55 @@
             _script[0] = './' + _script[0]
     elif not (which(_script[0]) or which(executable_path)):
         # the first el of _script is not executable
         # (at least on this computer)
         if not confirm_choice(
             f"The program '{executable_path}' was not executable \n"
             f'(or a script could not be found) on this computer. \n'
-            f'Please confirm to continue.'
+            f'Please confirm to continue.',
         ):
-            raise SystemExit()
+            raise SystemExit
 
     if repository is None:
         _repository = get_repo_name_from_remote(get_git_default_remote())
         if _commit_ref is None:
             _commit_ref = get_git_commit_ref_of_current_repository()
 
         if _cwd is None:
             _cwd = get_relative_path_from_git_root()
 
-        if not check_if_commit_is_on_remote(_commit_ref):
-            if not confirm_choice(
-                f'The commit "{_commit_ref}" was not found on GitHub '
-                '(Did you forget to push your latest commit?) \n'
-                'Please confirm if you want to proceed anyway.'
-            ):
-                raise SystemExit()
+        if not check_if_commit_is_on_remote(_commit_ref) and not confirm_choice(
+            f'The commit "{_commit_ref}" was not found on GitHub '
+            '(Did you forget to push your latest commit?) \n'
+            'Please confirm if you want to proceed anyway.',
+        ):
+            raise SystemExit
 
     if _cwd == '.':
         _cwd = None
 
     _env = None
     if env:
         _env = {}
         for env_var_pair in env:
             try:
                 pair = env_var_pair.split('=', maxsplit=1)
                 _env[pair[0]] = pair[1]
             except IndexError as e:
                 raise IndexError(
-                    env_var_pair + ' does not conform to key=value format.'
+                    env_var_pair + ' does not conform to key=value format.',
                 ) from e
 
     _config = None
     if config:
         _config = dict(read_configs(config))
 
     server_endpoint = get_server_endpoint(
-        server_url=server_url, is_test=use_test_server
+        server_url=server_url,
+        is_test=use_test_server,
     )
     _token = get_google_identity_token(server_endpoint)
 
     logger.info(f'Submitting {_repository}@{_commit_ref} for dataset "{dataset}"')
 
     response = requests.post(
         server_endpoint,
@@ -244,20 +245,20 @@
         timeout=60,
     )
     try:
         response.raise_for_status()
         logger.info(f'Request submitted successfully: {response.text}')
     except requests.HTTPError as e:
         logger.critical(
-            f'Request failed with status {response.status_code}: {str(e)}\n'
+            f'Request failed with status {response.status_code}: {e!s}\n'
             f'Full response: {response.text}',
         )
 
 
-def _perform_shebang_check(script):
+def _perform_shebang_check(script: str) -> None:
     """
     Returns None if script has shebang, otherwise raises Exception
     """
     with open(script, encoding='utf-8') as f:
         potential_shebang = f.readline()
         if potential_shebang.startswith('#!'):
             return
```

### Comparing `analysis-runner-2.44.0/analysis_runner/cli_config.py` & `analysis-runner-3.0.0/analysis_runner/cli_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 CLI options for standard analysis-runner
 """
 
-import os
 import argparse
+import os
 import sys
-from typing import List
 
 import requests
 import toml
-from cpg_utils.config import read_configs
+
+from analysis_runner.util import _perform_version_check, get_server_endpoint, logger
 from cpg_utils.cloud import get_google_identity_token
-from analysis_runner.constants import get_server_endpoint
-from analysis_runner.util import _perform_version_check, logger
+from cpg_utils.config import read_configs
 
 
-def add_config_args(parser=None) -> argparse.ArgumentParser:
+def add_config_args(
+    parser: argparse.ArgumentParser | None = None,
+) -> argparse.ArgumentParser:
     """
     Add CLI arguments for standard analysis-runner
     """
     if not parser:
         parser = argparse.ArgumentParser('config subparser')
 
     parser.add_argument(
@@ -69,39 +70,41 @@
         required=False,
         help='Output path to write the generated config to (in YAML)',
     )
 
     return parser
 
 
-def run_config_from_args(args):
+def run_config_from_args(args: argparse.ArgumentParser):
     """Run analysis runner from argparse.parse_arguments"""
     return run_config(**vars(args))
 
 
-def run_config(  # pylint: disable=too-many-arguments
-    dataset,
-    output_dir,
-    access_level,
-    image=None,
-    config: List[str] = None,
-    config_output=None,
-    use_test_server=False,
+def run_config(
+    dataset: str,
+    output_dir: str,
+    access_level: str,
+    image: str | None = None,
+    config: list[str] | None = None,
+    config_output: str | None = None,
+    use_test_server: bool = False,
+    server_url: str | None = None,
 ):
     """
     Main function that drives the CLI.
     """
     _perform_version_check()
 
     _config = None
     if config:
         _config = dict(read_configs(config))
 
     server_endpoint = os.path.join(
-        get_server_endpoint(is_test=use_test_server), 'config'
+        get_server_endpoint(is_test=use_test_server, server_url=server_url),
+        'config',
     )
     _token = get_google_identity_token(server_endpoint)
 
     response = requests.post(
         server_endpoint,
         json={
             'dataset': dataset,
@@ -115,20 +118,20 @@
     )
     try:
         response.raise_for_status()
         if config_output:
             if not config_output.endswith('.toml'):
                 logger.warning(
                     'The config is written as a .toml file, but the extension on the '
-                    'file you have provided is not .toml'
+                    'file you have provided is not .toml',
                 )
             with open(config_output, 'w+', encoding='utf-8') as f:
                 toml.dump(response.json(), f)
                 logger.info(f'Wrote config to {config_output}')
         else:
             toml.dump(response.json(), sys.stdout)
 
     except requests.HTTPError as e:
         logger.critical(
-            f'Request failed with status {response.status_code}: {str(e)}\n'
+            f'Request failed with status {response.status_code}: {e!s}\n'
             f'Full response: {response.text}',
         )
```

### Comparing `analysis-runner-2.44.0/analysis_runner/cli_cromwell.py` & `analysis-runner-3.0.0/analysis_runner/cli_cromwell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,111 @@
 """
 Cromwell CLI
 """
 
-# pylint: disable=too-many-arguments,too-many-return-statements,broad-except
 import argparse
 import json
 import os.path
-from typing import Dict, List, Optional
+from typing import Any
 
 import requests
-from cpg_utils.cloud import get_google_identity_token
 
-from analysis_runner.constants import get_server_endpoint
-from analysis_runner.cromwell_model import WorkflowMetadataModel
-from analysis_runner.git import (
+from analysis_runner.util import (
+    _perform_version_check,
+    add_general_args,
+    confirm_choice,
+    get_server_endpoint,
+    logger,
+)
+from cpg_utils.cloud import get_google_identity_token
+from cpg_utils.cromwell_model import WorkflowMetadataModel
+from cpg_utils.git import (
     check_if_commit_is_on_remote,
     get_git_branch_name,
     get_git_commit_ref_of_current_repository,
     get_git_default_remote,
     get_relative_path_from_git_root,
     get_repo_name_from_remote,
 )
-from analysis_runner.util import (
-    _perform_version_check,
-    add_general_args,
-    confirm_choice,
-    logger,
-)
 
 
 def cromwell_modes() -> dict:
     """This is a function instead of a constant so we don't see ordering definition errors."""
     return {
         'submit': (_add_cromwell_submit_args_to, _run_cromwell),
         'status': (_add_cromwell_status_args, _check_cromwell_status),
         'visualise': (
             _add_cromwell_metadata_visualier_args,
             _visualise_cromwell_metadata_from_file,
         ),
     }
 
 
-def add_cromwell_args(parser=None) -> argparse.ArgumentParser:
+def add_cromwell_args(
+    parser: argparse.ArgumentParser | None = None,
+) -> argparse.ArgumentParser:
     """Create / add arguments for cromwell argparser"""
     if not parser:
         parser = argparse.ArgumentParser('cromwell analysis-runner')
 
     subparsers = parser.add_subparsers(dest='cromwell_mode')
 
     for mode, (add_args, _) in cromwell_modes().items():
         add_args(subparsers.add_parser(mode))
 
     return parser
 
 
-def run_cromwell_from_args(args):
+def run_cromwell_from_args(args: argparse.ArgumentParser):
     """Run cromwell CLI mode from argparse.args"""
     _cromwell_modes = cromwell_modes()
 
     kwargs = vars(args)
     cromwell_mode = kwargs.pop('cromwell_mode')
     if cromwell_mode not in _cromwell_modes:
         raise NotImplementedError(cromwell_mode)
 
     return _cromwell_modes[cromwell_mode][1](**kwargs)
 
 
-def _add_generic_cromwell_visualiser_args(parser: argparse.ArgumentParser):
+def _add_generic_cromwell_visualiser_args(
+    parser: argparse.ArgumentParser,
+) -> argparse.ArgumentParser:
     parser.add_argument('-l', '--expand-completed', default=False, action='store_true')
     parser.add_argument('--monochrome', default=False, action='store_true')
 
+    return parser
+
 
-def _add_cromwell_status_args(parser: argparse.ArgumentParser):
+def _add_cromwell_status_args(
+    parser: argparse.ArgumentParser,
+) -> argparse.ArgumentParser:
     """Add cli args for checking status of Cromwell workflow"""
     parser.add_argument('workflow_id')
     parser.add_argument('--json-output', help='Output metadata to this path')
 
     _add_generic_cromwell_visualiser_args(parser)
 
     return parser
 
 
-def _add_cromwell_metadata_visualier_args(parser: argparse.ArgumentParser):
+def _add_cromwell_metadata_visualier_args(
+    parser: argparse.ArgumentParser,
+) -> argparse.ArgumentParser:
     """
     Add arguments for visualising cromwell workflow from metadata file
     """
     parser.add_argument('metadata_file')
     _add_generic_cromwell_visualiser_args(parser)
     return parser
 
 
-def _add_cromwell_submit_args_to(parser):
+def _add_cromwell_submit_args_to(
+    parser: argparse.ArgumentParser,
+) -> argparse.ArgumentParser:
     """
     Add cli args for submitting WDL workflow to cromwell,
     via the analysis runner
     """
 
     add_general_args(parser)
 
@@ -110,15 +121,15 @@
         '-p',
         '--imports',
         required=False,
         action='append',
         help=(
             'A directory which is used to search for workflow imports. You can specify this argument multiple times.'
             'Note: the directories are zipped from the cwd with `zip -r {directory1} {directory2}`.'
-            'Please raise an issue to change this behaviour',
+            'Please raise an issue to change this behaviour'
         ),
     )
     parser.add_argument(
         '--workflow-input-prefix',
         type=str,
         required=False,
         help='Prefix to apply to all inputs AFTER the workflow argument, usually the workflow name',
@@ -145,68 +156,66 @@
         nargs=argparse.REMAINDER,
         help='--{key} {value} that get automatically parsed into an inputs json',
     )
 
     return parser
 
 
-def _run_cromwell(
-    dataset,
-    output_dir,
-    description,
-    access_level,
+def _run_cromwell(  # noqa: C901
+    dataset: str,
+    output_dir: str,
+    description: str,
+    access_level: str,
     workflow: str,
-    inputs: List[str],
-    imports: List[str] = None,
-    workflow_input_prefix: str = None,
-    dynamic_inputs: List[str] = None,
-    commit=None,
-    repository=None,
-    cwd=None,
-    labels=None,
-    dry_run=False,
-    use_test_server=False,
-    server_url=None,
-):
+    inputs: list[str],
+    imports: list[str] | None = None,
+    workflow_input_prefix: str | None = None,
+    dynamic_inputs: list[str] | None = None,
+    commit: str | None = None,
+    repository: str | None = None,
+    cwd: str | None = None,
+    labels: str | None = None,
+    dry_run: bool | None = False,
+    use_test_server: bool | None = False,
+    server_url: str | None = None,
+) -> None:
     """
     Prepare parameters for cromwell analysis-runner job
     """
     if repository is not None and commit is None:
         raise ValueError(
             "You must supply the '--commit <SHA>' parameter "
-            "when specifying the '--repository'"
+            "when specifying the '--repository'",
         )
 
     _perform_version_check()
 
-    if access_level == 'full':
-        if not confirm_choice(
-            'Full access increases the risk of accidental data loss. Continue?',
-        ):
-            raise SystemExit()
+    if access_level == 'full' and not confirm_choice(
+        'Full access increases the risk of accidental data loss. Continue?',
+    ):
+        raise SystemExit
 
     _repository = repository
     _commit_ref = commit
     _cwd = cwd
     _branch = get_git_branch_name()
 
     if repository is None:
         _repository = get_repo_name_from_remote(get_git_default_remote())
         if _commit_ref is None:
             _commit_ref = get_git_commit_ref_of_current_repository()
 
         if _cwd is None:
             _cwd = get_relative_path_from_git_root()
 
-        if not check_if_commit_is_on_remote(_commit_ref):
-            if not confirm_choice(
-                f'The commit "{_commit_ref}" was not found on the remote (Github). \n'
-                'Please confirm if you want to proceed anyway.'
-            ):
-                raise SystemExit()
+        if not check_if_commit_is_on_remote(_commit_ref) and not confirm_choice(
+            f'The commit "{_commit_ref}" was not found on the remote (Github). \n'
+            'Please confirm if you want to proceed anyway.',
+        ):
+            raise SystemExit
 
     if _cwd == '.':
         _cwd = None
 
     _inputs_dict = None
     if dynamic_inputs:
         _inputs_dict = parse_additional_args(dynamic_inputs)
@@ -232,15 +241,16 @@
         'input_json_paths': inputs or [],
         'dependencies': imports or [],
         'labels': _labels,
         'branch': _branch,
     }
 
     server_endpoint = get_server_endpoint(
-        server_url=server_url, is_test=use_test_server
+        server_url=server_url,
+        is_test=use_test_server,
     )
     endpoint = os.path.join(server_endpoint, '/cromwell')
 
     if dry_run:
         logger.warning('Dry-run, printing curl and exiting')
         curl = f"""\
 curl --location --request POST \\
@@ -252,47 +262,47 @@
         print(curl)
         return
 
     response = requests.post(
         endpoint,
         json=body,
         headers={
-            'Authorization': f'Bearer {get_google_identity_token(server_endpoint)}'
+            'Authorization': f'Bearer {get_google_identity_token(server_endpoint)}',
         },
         timeout=60,
     )
     try:
         response.raise_for_status()
         logger.info(f'Request submitted successfully: {response.text}')
     except requests.HTTPError as e:
         logger.critical(
-            f'Request failed with status {response.status_code}: {str(e)}\n'
+            f'Request failed with status {response.status_code}: {e!s}\n'
             f'Full response: {response.text}',
         )
 
 
 def _check_cromwell_status(
-    workflow_id,
-    json_output: Optional[str],
+    workflow_id: str,
+    json_output: str | None,
     server_url: str | None = None,
     is_test: bool = False,
-    **kwargs,
-):
+    **kwargs: Any,
+) -> None:
     """Check cromwell status with workflow_id"""
 
     server_endpoint = get_server_endpoint(server_url, is_test)
     url = os.path.join(
         server_endpoint,
         f'cromwell/{workflow_id}/metadata',
     )
 
     response = requests.get(
         url,
         headers={
-            'Authorization': f'Bearer {get_google_identity_token(server_endpoint)}'
+            'Authorization': f'Bearer {get_google_identity_token(server_endpoint)}',
         },
         timeout=60,
     )
     response.raise_for_status()
     d = response.json()
 
     if json_output:
@@ -300,30 +310,35 @@
         with open(json_output, 'w+', encoding='utf-8') as f:
             json.dump(d, f)
 
     model = WorkflowMetadataModel.parse(d)
     print(model.display(**kwargs))
 
 
-def _visualise_cromwell_metadata_from_file(metadata_file: str, **kwargs):
+def _visualise_cromwell_metadata_from_file(
+    metadata_file: str,
+    **kwargs: Any,
+) -> None:
     """Visualise cromwell metadata progress from a json file"""
     with open(metadata_file, encoding='utf-8') as f:
         model = WorkflowMetadataModel.parse(json.load(f))
 
     visualise_cromwell_metadata(model, **kwargs)
 
 
 def visualise_cromwell_metadata(
-    model: WorkflowMetadataModel, expand_completed, monochrome
+    model: WorkflowMetadataModel,
+    expand_completed: bool,
+    monochrome: bool,
 ):
     """Print the visualisation of cromwell metadata model"""
     print(model.display(expand_completed=expand_completed, monochrome=monochrome))
 
 
-def try_parse_value(value: Optional[str]):
+def try_parse_value(value: str | None):
     """Try parse value from command line string"""
     if value is None or value == 'None' or value == 'null':
         return value
 
     if isinstance(value, list):
         return list(map(try_parse_value, value))
 
@@ -350,15 +365,15 @@
 
 
 def parse_keyword(keyword: str):
     """Parse CLI keyword"""
     return keyword[2:].replace('-', '_')
 
 
-def parse_additional_args(args: List[str]) -> Dict[str, any]:
+def parse_additional_args(args: list[str]) -> dict[str, Any]:  # noqa: C901
     """
     Parse a list of strings to an inputs json
 
     The theory is to look for any args that start with '--',
     strip those two leading dashes, replace '-' with '_'.
     1. If the keyword is followed by another keyword, then make
           the first param a boolean (with True)
@@ -391,32 +406,34 @@
 
         * Keyword with multiple values, followed by same keyword with multiple values results in nested lists
 
     >>> parse_additional_args(['--keyword', 'val1_a', 'val1_b', '--keyword', 'val2_a', 'val2_b'])
     {'keyword': [['val1_a', 'val1_b'], ['val2_a', 'val2_b']]}
     """
 
-    keywords = {}
+    keywords: dict[str, Any] = {}
 
-    def add_keyword_value_to_keywords(keyword, value):
+    def add_keyword_value_to_keywords(keyword: str | None, value: Any) -> None:
+        if not keyword:
+            return
         if keyword in keywords:
             if value is None:
                 value = [keywords.get(keyword)]
             else:
                 value = [keywords.get(keyword), try_parse_value(new_value)]
         elif value is None:
             # flag
             value = True
         else:
             value = try_parse_value(value)
 
         keywords[keyword] = value
 
     current_keyword = None
-    new_value: any = None
+    new_value: Any = None
 
     for arg in args:
         if not arg.startswith('--'):
             if new_value is None:
                 # if it's the first value we're seeing, set it
                 new_value = arg
             elif not isinstance(new_value, list):
```

### Comparing `analysis-runner-2.44.0/analysis_runner/util.py` & `analysis-runner-3.0.0/analysis_runner/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Utility function"""
-# pylint: disable=import-outside-toplevel
 
+# ruff: noqa: ERA001
+
+import argparse
 import logging
 import re
 
 import requests
 
 from analysis_runner._version import __version__
-from analysis_runner.constants import SERVER_ENDPOINT
 
 BRANCH = 'main'
+SERVER_ENDPOINT = 'https://server-a2pko7ameq-ts.a.run.app'
+SERVER_TEST_ENDPOINT = 'https://server-test-a2pko7ameq-ts.a.run.app'
+ANALYSIS_RUNNER_PROJECT_ID = 'analysis-runner'
 
 logger = logging.getLogger('analysis_runner')
 logger.addHandler(logging.StreamHandler())
 logger.setLevel(logging.INFO)
 # Also update the default severity level for modules that don't use the
 # 'analysis-runner' logger.
 logging.getLogger().setLevel(logging.INFO)
@@ -26,15 +30,15 @@
     >>> get_project_id_from_service_account_email('cromwell-test@tob-wgs.iam.gserviceaccount.com')
     'tob-wgs'
     """
     # quick and dirty
     return service_account_email.split('@')[-1].split('.')[0]
 
 
-def add_general_args(parser):
+def add_general_args(parser: argparse.ArgumentParser):
     """
     Add CLI arguments that are relevant for most
     analysis-runner submission modes (standard / cromwell)
     """
     parser.add_argument(
         '--dataset',
         required=True,
@@ -110,15 +114,15 @@
             return True
         if confirmation in ('no', 'n'):
             return False
 
         print('Unrecognised option, please try again.')
 
 
-def _perform_version_check():
+def _perform_version_check() -> None:
     current_version = __version__
 
     # with this URL, we're looking for a line with format:
     #   __version__ = '<version>'
     # match it with regex: r"__version__ = '(.+)'$"
     version_url = (
         'https://raw.githubusercontent.com/populationgenomics/'
@@ -127,31 +131,33 @@
     try:
         resp = requests.get(version_url, timeout=20)
         resp.raise_for_status()
         data = resp.text
     except requests.HTTPError as e:
         logger.debug(
             f'An error occurred when fetching version '
-            f'information about the analysis-runner: {e}'
+            f'information about the analysis-runner: {e}',
         )
         return
     for line in data.splitlines(keepends=False):
         if not line.startswith('__version__ = '):
             continue
 
-        latest_version = re.match("__version__ = '(.+)'$", line).groups()[0]
-        if current_version != latest_version:
-            message = (
-                f'Your version of analysis-runner is out of date: '
-                f'{current_version} != {latest_version} (current vs latest).\n'
-                f'Your analysis will still be submitted, but may not work as expected.'
-                f' You can update the analysis-runner by running '
-                f'"pip install analysis-runner=={latest_version}".'
-            )
-            logger.warning(message)
+        match = re.match("__version__ = '(.+)'$", line)
+        if match:
+            latest_version = match.groups()[0]
+            if current_version != latest_version:
+                message = (
+                    f'Your version of analysis-runner is out of date: '
+                    f'{current_version} != {latest_version} (current vs latest).\n'
+                    f'Your analysis will still be submitted, but may not work as expected.'
+                    f' You can update the analysis-runner by running '
+                    f'"pip install analysis-runner=={latest_version}".'
+                )
+                logger.warning(message)
         return
 
 
 class AnsiiColors:
     """
     Lookup table: https://en.wikipedia.org/wiki/ANSI_escape_code#3/4_bit
     """
@@ -161,7 +167,24 @@
     BRIGHTGREEN = '\033[92m'  # Bright green
     BRIGHTYELLOW = '\033[93m'  # Bright yellow
     BRIGHTRED = '\033[91m'  # Bright red
     RESET = '\033[0m'  # SGR (Reset / Normal)
     BOLD = '\033[1m'  # SGR (Bold or increased intensity
     ITALIC = '\033[3m'  # SGR (Italic)
     UNDERLINE = '\033[4m'  # SGR (Underline)
+
+
+def get_server_endpoint(
+    server_url: str | None = SERVER_ENDPOINT,
+    is_test: bool | None = False,
+):
+    """
+    Get the server endpoint {production / test}
+    Do it in a function so it's easy to fix if the logic changes
+    """
+    if is_test:
+        return SERVER_TEST_ENDPOINT
+
+    if not server_url:
+        return SERVER_ENDPOINT
+
+    return server_url
```

### Comparing `analysis-runner-2.44.0/analysis_runner.egg-info/PKG-INFO` & `analysis-runner-3.0.0/analysis_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.44.0
+Version: 3.0.0
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.44.0/analysis_runner.egg-info/SOURCES.txt` & `analysis-runner-3.0.0/analysis_runner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 setup.py
 analysis_runner/__init__.py
 analysis_runner/_version.py
 analysis_runner/cli.py
 analysis_runner/cli_analysisrunner.py
 analysis_runner/cli_config.py
 analysis_runner/cli_cromwell.py
-analysis_runner/constants.py
 analysis_runner/cromwell.py
-analysis_runner/cromwell_model.py
 analysis_runner/dataproc.py
-analysis_runner/git.py
 analysis_runner/util.py
 analysis_runner.egg-info/PKG-INFO
 analysis_runner.egg-info/SOURCES.txt
 analysis_runner.egg-info/dependency_links.txt
 analysis_runner.egg-info/entry_points.txt
 analysis_runner.egg-info/not-zip-safe
 analysis_runner.egg-info/requires.txt
```

### Comparing `analysis-runner-2.44.0/setup.py` & `analysis-runner-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='2.44.0',
+    version='3.0.0',
     description='Analysis runner to help make analysis results reproducible',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/{PKG}',
     license='MIT',
     packages=['analysis_runner'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'cloudpathlib[all]',
-        'cpg-utils>=4.12.1',
+        'cpg-utils>=5.0.0',
         'hail',
         'requests',
         'tabulate',
     ],
     entry_points={
-        'console_scripts': ['analysis-runner=analysis_runner.cli:main_from_args']
+        'console_scripts': ['analysis-runner=analysis_runner.cli:main_from_args'],
     },
     keywords='bioinformatics',
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
```

### Comparing `analysis-runner-2.44.0/test/test_analysis_runner.py` & `analysis-runner-3.0.0/test/test_analysis_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
+# ruff: noqa: S105
 import unittest
-
-from unittest.mock import patch, MagicMock
+from typing import Any, Optional
+from unittest.mock import MagicMock, patch
 
 from analysis_runner._version import __version__
 from analysis_runner.cli import main_from_args
 
 IMPORT_AR_IDENTITY_TOKEN_PATH = (
     'analysis_runner.cli_analysisrunner.get_google_identity_token'
 )
@@ -35,75 +35,80 @@
     @patch('builtins.print')
     def test_help_full(self, mock_print: MagicMock):
         main_from_args(['--help'])
         mock_print.assert_called()
 
 
 class MockResponse:
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self.raise_for_status = lambda: None
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
 
 def apply_mock_behaviour(
-    *, mock_post: MagicMock = None, mock_identity_token: MagicMock = None
+    *,
+    mock_post: Optional[MagicMock] = None,
+    mock_identity_token: Optional[MagicMock] = None,
 ):
     if mock_post:
         mock_post.return_value = MockResponse(text='<mocked-url>')
 
     if mock_identity_token:
         mock_identity_token.return_value = '<mocked-identity-token>'
 
 
 class TestCliAnalysisRunner(unittest.TestCase):
-    ANALYSIS_RUNNER_ARGS = [
+    ANALYSIS_RUNNER_ARGS = (
         '--dataset',
         'fewgenomes',
         '--access-level',
         'test',
         '--description',
         'mock-test',
         '--output-dir',
         'hello-world-test',
         'echo',
         'hello-world',
-    ]
+    )
 
     @patch(IMPORT_AR_IDENTITY_TOKEN_PATH)
     @patch(REQUEST_POST_PATH)
     def test_regular_cli(self, mock_post: MagicMock, mock_identity_token: MagicMock):
         apply_mock_behaviour(
-            mock_post=mock_post, mock_identity_token=mock_identity_token
+            mock_post=mock_post,
+            mock_identity_token=mock_identity_token,
         )
 
         main_from_args(self.ANALYSIS_RUNNER_ARGS)
 
         mock_post.assert_called()
         mock_identity_token.assert_called()
 
     @patch(IMPORT_AR_IDENTITY_TOKEN_PATH)
     @patch(REQUEST_POST_PATH)
     def test_cli_with_mode(self, mock_post: MagicMock, mock_identity_token: MagicMock):
         apply_mock_behaviour(
-            mock_post=mock_post, mock_identity_token=mock_identity_token
+            mock_post=mock_post,
+            mock_identity_token=mock_identity_token,
         )
         main_from_args(['analysis-runner', *self.ANALYSIS_RUNNER_ARGS])
 
         mock_post.assert_called()
         mock_identity_token.assert_called()
 
 
 class TestCliCromwell(unittest.TestCase):
     @patch(IMPORT_CR_IDENTITY_TOKEN_PATH)
     @patch(REQUEST_POST_PATH)
     def test_submit_cli(self, mock_post: MagicMock, mock_identity_token: MagicMock):
         apply_mock_behaviour(
-            mock_post=mock_post, mock_identity_token=mock_identity_token
+            mock_post=mock_post,
+            mock_identity_token=mock_identity_token,
         )
 
         args = [
             'cromwell',
             'submit',
             '--dataset',
             'fewgenomes',
@@ -117,54 +122,10 @@
         ]
 
         main_from_args(args)
 
         mock_post.assert_called()
         mock_identity_token.assert_called()
 
-    @patch(IMPORT_CR_IDENTITY_TOKEN_PATH)
-    @patch(REQUEST_GET_PATH)
-    @patch('builtins.print')
-    def test_status_cli(
-        self, mock_print: MagicMock, mock_get: MagicMock, mock_id_token
-    ):
-        apply_mock_behaviour(mock_identity_token=mock_id_token)
-        cm = {
-            'id': '<mocked-id>',
-            'start': '2021-07-09T09:47:00.000Z',
-            'end': '2021-07-09T09:48:00.000Z',
-            'calls': {
-                'wf.print': [
-                    {
-                        'name': 'print',
-                        'executionStatus': 'succeeded',
-                        'start': '2021-07-09T09:47:00.000Z',
-                        'end': '2021-07-09T09:48:00.000Z',
-                    }
-                ]
-            },
-        }
-        mock_get.return_value = MockResponse(json=lambda: cm)
-
-        args = ['cromwell', 'status', '<mocked-id>', '--monochrome']
-
-        status_str = """
------------  ------------------------
-Workflow ID  <mocked-id>
-Name
-Status       preparing
-Start        2021-07-09T09:47:00.000Z
-End          2021-07-09T09:48:00.000Z
-Duration     1m:0s
------------  ------------------------
-Jobs:
-  [#] print (1m:0s)
-"""
-
-        main_from_args(args)
-
-        mock_get.assert_called()
-        mock_print.assert_called_with(status_str)
-
 
 if __name__ == '__main__':
     unittest.main()
```

