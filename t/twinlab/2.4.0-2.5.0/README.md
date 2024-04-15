# Comparing `tmp/twinlab-2.4.0.tar.gz` & `tmp/twinlab-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-2.4.0.tar", max compression
+gzip compressed data, was "twinlab-2.5.0.tar", max compression
```

## Comparing `twinlab-2.4.0.tar` & `twinlab-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1031 2024-03-11 09:16:22.945659 twinlab-2.4.0/LICENSE
--rw-r--r--   0        0        0      555 2024-03-18 13:45:32.588743 twinlab-2.4.0/README.md
--rw-r--r--   0        0        0     1914 2024-03-19 19:30:35.778324 twinlab-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1527 2024-03-19 09:17:12.471040 twinlab-2.4.0/twinlab/__init__.py
--rw-r--r--   0        0        0      171 2024-03-12 11:24:16.616707 twinlab-2.4.0/twinlab/_version.py
--rw-r--r--   0        0        0    13517 2024-03-19 09:17:12.471262 twinlab-2.4.0/twinlab/api.py
--rw-r--r--   0        0        0    39402 2024-03-19 19:30:35.780935 twinlab-2.4.0/twinlab/client.py
--rw-r--r--   0        0        0     8288 2024-03-19 10:51:55.777038 twinlab-2.4.0/twinlab/core.py
--rw-r--r--   0        0        0     7702 2024-03-19 09:17:12.472209 twinlab-2.4.0/twinlab/dataset.py
--rw-r--r--   0        0        0      834 2024-03-18 14:20:15.931606 twinlab-2.4.0/twinlab/distributions.py
--rw-r--r--   0        0        0    50592 2024-03-19 19:30:35.781416 twinlab-2.4.0/twinlab/emulator.py
--rw-r--r--   0        0        0     2896 2024-03-19 09:17:12.472833 twinlab-2.4.0/twinlab/helper.py
--rw-r--r--   0        0        0    18328 2024-03-19 19:30:35.781564 twinlab-2.4.0/twinlab/params.py
--rw-r--r--   0        0        0     1862 2024-03-18 14:20:15.932897 twinlab-2.4.0/twinlab/plotting.py
--rw-r--r--   0        0        0      562 2024-03-18 14:20:15.933130 twinlab-2.4.0/twinlab/prior.py
--rw-r--r--   0        0        0     1084 2024-03-18 14:20:15.933190 twinlab-2.4.0/twinlab/sampling.py
--rw-r--r--   0        0        0     1637 2024-03-12 11:24:16.626252 twinlab-2.4.0/twinlab/settings.py
--rw-r--r--   0        0        0     5104 2024-03-19 09:17:12.473149 twinlab-2.4.0/twinlab/utils.py
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 twinlab-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1031 2024-03-11 09:16:22.945659 twinlab-2.5.0/LICENSE
+-rw-r--r--   0        0        0      555 2024-03-18 13:45:32.588743 twinlab-2.5.0/README.md
+-rw-r--r--   0        0        0     1802 2024-04-15 09:02:01.144244 twinlab-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1486 2024-04-11 10:18:35.345552 twinlab-2.5.0/twinlab/__init__.py
+-rw-r--r--   0        0        0      171 2024-03-12 11:24:16.616707 twinlab-2.5.0/twinlab/_version.py
+-rw-r--r--   0        0        0    13517 2024-03-20 17:24:42.877209 twinlab-2.5.0/twinlab/api.py
+-rw-r--r--   0        0        0    44109 2024-04-11 10:18:35.345728 twinlab-2.5.0/twinlab/client.py
+-rw-r--r--   0        0        0    10034 2024-04-11 10:18:35.345916 twinlab-2.5.0/twinlab/core.py
+-rw-r--r--   0        0        0     8676 2024-04-11 10:18:35.346087 twinlab-2.5.0/twinlab/dataset.py
+-rw-r--r--   0        0        0      829 2024-04-11 10:18:35.346314 twinlab-2.5.0/twinlab/distributions.py
+-rw-r--r--   0        0        0    61723 2024-04-15 08:15:42.021188 twinlab-2.5.0/twinlab/emulator.py
+-rw-r--r--   0        0        0     4876 2024-04-11 10:18:35.346907 twinlab-2.5.0/twinlab/helper.py
+-rw-r--r--   0        0        0    29491 2024-04-11 10:18:35.347178 twinlab-2.5.0/twinlab/params.py
+-rw-r--r--   0        0        0     1862 2024-04-09 17:31:34.286104 twinlab-2.5.0/twinlab/plotting.py
+-rw-r--r--   0        0        0      668 2024-04-11 10:18:35.347422 twinlab-2.5.0/twinlab/prior.py
+-rw-r--r--   0        0        0     1926 2024-04-11 10:18:35.347716 twinlab-2.5.0/twinlab/sampling.py
+-rw-r--r--   0        0        0     1637 2024-03-12 11:24:16.626252 twinlab-2.5.0/twinlab/settings.py
+-rw-r--r--   0        0        0     5233 2024-04-11 10:18:35.347832 twinlab-2.5.0/twinlab/utils.py
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 twinlab-2.5.0/PKG-INFO
```

### Comparing `twinlab-2.4.0/LICENSE` & `twinlab-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-2.4.0/README.md` & `twinlab-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-2.4.0/pyproject.toml` & `twinlab-2.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "2.4.0"
+version = "2.5.0"
 description = "Python interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab"
 authors = ["digiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
@@ -19,36 +19,38 @@
     "Micol Greta Giannelli <micol@digilab.co.uk>",
     "Jasper Cantwell <jasper@digilab.co.uk>",
 ]
 keywords = ["machine-learning", "AI", "cloud", "twinLab", "digiLab"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<3.13"
 matplotlib = ">=3.7"
-numpy = "^1.24.0"
-pandas = "^1.5.3,<2.0.0"
+numpy = [
+    { version = "^1.24", python = ">=3.8,<3.9" },
+    { version = "^1.26", python = ">=3.9,<3.13" },
+]
+pandas = [
+    { version = "^1.5.3", python = ">=3.8,<3.9" },
+    { version = "^2.0", python = ">=3.9,<3.13" },
+]
 python-dotenv = "^1.0.0"
 requests = "^2.28.2"
 typeguard = "^4.0.0"
 pytest = "^7.4.3"
 setuptools = "^69.0.2"
+deprecated = "^1.2.14"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 IPython = "^8.11"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-regtest = "^1.5.1"
 pytest-regressions = "^2.5.0"
-mkdocs = "^1.4.2"             # NOTE: This is used for the documentation
-Markdown = "^3.3.7"           # NOTE: This is used for the documentation
-mkdocstrings = "*"            # NOTE: This is used for the documentation
-mkdocstrings-python = "*"     # NOTE: This is used for the documentation
-mkdocs-material = "^9.5.6"
 
 # NOTE: This allows for better collection of the pytests
 # NOTE: Allows tests that have the same name but in different folders
 [tool.pytest.ini_options]
 addopts = "--import-mode=importlib"
 
 [build-system]
```

### Comparing `twinlab-2.4.0/twinlab/__init__.py` & `twinlab-2.5.0/twinlab/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,74 @@
 # Version
 from ._version import __version__
 
+# Campaign functions
+# NOTE: Deprecated (v1)
+# Dataset functions
+# NOTE: Deprecated (v1)
 # General functions
 # NOTE: Deprecated (v1)
 from .client import (
-    set_api_key,
-    set_server_url,
+    active_learn_campaign,
+    delete_campaign,
+    delete_dataset,
     get_api_key,
+    get_calibration_curve_campaign,
     get_server_url,
     get_user_information,
     get_versions,
-    list_datasets,
     list_campaigns,
-)
-
-# Dataset functions
-# NOTE: Deprecated (v1)
-from .client import (
-    upload_dataset,
-    query_dataset,
-    view_dataset,
-    delete_dataset,
-)
-
-# Campaign functions
-# NOTE: Deprecated (v1)
-from .client import (
-    train_campaign,
-    query_campaign,
-    view_campaign,
+    list_datasets,
+    optimise_campaign,
     predict_campaign,
+    query_campaign,
+    query_dataset,
     sample_campaign,
-    active_learn_campaign,
-    solve_inverse_campaign,
-    optimise_campaign,
     score_campaign,
-    get_calibration_curve_campaign,
-    delete_campaign,
-)
-
-# Prior class
-from .prior import (
-    Prior,
-)
-
-# Distribution class
-from .distributions import (
-    Distribution,
-)
-
-# Sampling methods
-from .sampling import (
-    Sampling,
+    set_api_key,
+    set_server_url,
+    solve_inverse_campaign,
+    train_campaign,
+    upload_dataset,
+    view_campaign,
+    view_dataset,
 )
 
 # General functions
 from .core import (
-    versions,
-    user_information,
-    set_api_key,
     get_api_key,
-    set_server_url,
     get_server_url,
     list_datasets,
     list_emulators,
     list_example_datasets,
     load_example_dataset,
+    set_api_key,
+    set_server_url,
+    user_information,
+    versions,
 )
-
 from .dataset import Dataset
 
+# Distribution class
+from .distributions import Distribution
 from .emulator import Emulator
-
+from .helper import get_sample, join_samples, load_dataset, load_params
 from .params import (
+    AcqFuncParams,
+    BenchmarkParams,
+    CalibrateParams,
+    DesignParams,
     EstimatorParams,
     ModelSelectionParams,
-    TrainParams,
-    ScoreParams,
-    BenchmarkParams,
+    OptimiserParams,
     PredictParams,
-    SampleParams,
     RecommendParams,
-    CalibrateParams,
-    DesignParams,
+    SampleParams,
+    ScoreParams,
+    TrainParams,
 )
 
-from .helper import load_dataset, load_params, get_sample, join_samples
+# Prior class
+from .prior import Prior
+
+# Sampling methods
+from .sampling import Sampling
```

### Comparing `twinlab-2.4.0/twinlab/api.py` & `twinlab-2.5.0/twinlab/api.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.4.0/twinlab/client.py` & `twinlab-2.5.0/twinlab/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import json
 import os
 import time
 from pprint import pprint
 from typing import Optional, Tuple, Union
 
 # Third-party imports
+from deprecated import deprecated
 import pandas as pd
 from typeguard import typechecked
 
 # Project imports
 from . import api, settings, utils
 
+DEPRECATION_VERSION = "2.5.0"
 PING_TIME_TRAIN_DEFAULT = 5.0  # Seconds
 PING_TIME_PREDICT_DEFAULT = 5.0  # Seconds
 
 ### Utility functions ###
 
 # TODO: Move to utils.py?
 
@@ -80,15 +82,14 @@
         method,
         data_csv=data_csv,
         data_std_csv=data_std_csv,
         processor=processor,
         verbose=debug,
         **kwargs,
     )
-
     if "dataframe" in response.keys():
         output_csv = _get_value_from_body("dataframe", response)
         return io.StringIO(output_csv)
     else:
         output_result = _get_value_from_body("result", response)
         return output_result
 
@@ -104,220 +105,237 @@
 
 
 ### ###
 
 ### General functions ###
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def set_api_key(api_key: str) -> None:
     """
-    # Set API key
 
     Set the user API key for the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        api_key (str): API key for the `twinLab` cloud.
 
-    - `api_key`: `str`, API key for the `twinLab` cloud.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
+            tl.set_api_key("12345")
 
-    ```python
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+            The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    tl.set_api_key("12345")
-    ```
     """
     os.environ["TWINLAB_API_KEY"] = api_key
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def set_server_url(url: str) -> None:
     """
-    # Set server URL
+
+    Set server URL
 
     Set the server URL for the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        url (str): URL for the `twinLab` cloud.
 
-    - `url`: `str`, URL for the `twinLab` cloud.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
 
-    ```python
-    import twinlab as tl
+            tl.set_url("https://twinlab.digilab.co.uk")
 
-    tl.set_url("https://twinlab.digilab.co.uk")
-    ```
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
     """
     os.environ["TWINLAB_URL"] = url
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def get_server_url() -> str:
     """
-    # Get the server URL
+
+    Get the server URL
 
     Get the server URL for the `twinLab` cloud.
 
-    ## Returns:
+    Returns:
+        str: containing the server URL
 
-    - `str` containing the server URL.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
+            tl.get_server_url()
 
-    ```python
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    tl.get_server_url()
-    ```
     """
     return os.getenv("TWINLAB_URL")
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def get_api_key() -> str:
     """
-    # Get the user API key
 
     Get the user API key for the `twinLab` cloud.
 
-    ## Returns:
+    Returns:
+        str: containing the server API key
 
-    - `str` containing the server API key.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
+            tl.get_api_key()
 
-    ```python
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    tl.get_api_key()
-    ```
     """
     return os.getenv("TWINLAB_API_KEY")
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def get_user_information(
     verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> dict:
     """
-        # Get user information
 
-        Get information about the user.
+    Get information about the user.
 
-        ## Arguments:
+    Args:
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
 
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-        - `debug`: `bool`, `Optional`. Determining level of information logged on the server
-    .
-        ## Returns:
+    Returns:
+        dict: containing user information
 
-        - `dict` containing user information.
+    Examples:
+        .. code-block:: python
 
-        ## Example:
+            user_info = tl.get_user_information()
+            print(user_info)
 
-        ```python
-        import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-        user_info = tl.get_user_information()
-        print(user_info)
-        ```
     """
     _, response = api.get_user(verbose=debug)
     user_info = response
     if verbose:
         print("User information:")
         pprint(user_info, compact=True, sort_dicts=False)
     return user_info
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def get_versions(
     verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> dict:
     """
-    # Get versions
 
-    Get information about the twinLab version being used
 
-    ## Arguments:
+    Get information about the twinLab version being used
 
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
+    Args:
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
 
-    ## Returns:
+    Returns:
+        dict: Dictionary containing version information
 
-    - `dict` containing version information.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
+            version_info = tl.get_versions()
+            print(version_info)
 
-    ```python
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    version_info = tl.get_versions()
-    print(version_info)
-    ```
     """
     _, response = api.get_versions(verbose=debug)
     version_info = response
     if verbose:
         print("Version information:")
         pprint(version_info, compact=True, sort_dicts=False)
     return version_info
 
 
 ### ###
 
 ### Dataset functions ###
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def upload_dataset(
     filepath_or_df: Union[str, pd.DataFrame],
     dataset_id: str,
     use_upload_url: Optional[bool] = True,
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
 ) -> None:
     """
-    # Upload dataset
+
 
     Upload a dataset to the `twinLab` cloud so that it can be queried and used for training.
 
-    ## Arguments:
+    Args:
+        filepath_or_df (Union[`str`.`pandas.DataFrame`]): Location of csv dataset on local machine or `pandas.DataFrame`.
+        dataset_id (str): Name for the dataset when saved to the twinLab cloud.
+        use_upload_url (bool, optional): `Optional`. Determining whether to upload via a pre-signed url or directly to the server.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Examples:
+        Upload a local file:
+
+        .. code-block:: python
+
+            data_filepath = "path/to/dataset.csv"
+            tl.upload_dataset(data_filepath, "my_dataset")
+
+        Upload a `pandas.DataFrame`:
+
+        .. code-block:: python
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `filepath_or_df`: Union[`str`,`pandas.DataFrame`]. Location of csv dataset on local machine or `pandas.DataFrame`.
-    - `dataset_id`: `str`. Name for the dataset when saved to the twinLab cloud.
-    **Warning:** If the `dataset_id` already exists for the current cloud account, it will be overwritten by the
-    newly uploaded dataset.
-    - `use_upload_url`: `bool`, `Optional`. Determining whether to upload via a pre-signed url or directly to the server.
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    **NOTE:** Local data must be a CSV file, working data should be a `pandas.DataFrame`.
-
-    ## Examples:
-
-    Upload a local file:
-    ```python
-    import twinlab as tl
-
-    data_filepath = "path/to/dataset.csv"
-    tl.upload_dataset(data_filepath, "my_dataset")
-    ```
-
-    Upload a `pandas.DataFrame`:
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    ```
     """
 
     # Upload the file (either via link or directly)
     if use_upload_url:
         _, response = api.generate_upload_url(dataset_id, verbose=debug)
         upload_url = _get_value_from_body("url", response)
         if type(filepath_or_df) is str:
@@ -341,279 +359,241 @@
         _, response = api.upload_dataset(dataset_id, csv_string, verbose=debug)
 
     if verbose:
         message = _get_message(response)
         print(message)
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def list_datasets(
     verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> list:
     """
-    # List datasets
 
     List datasets that have been uploaded to the `twinLab` cloud.
 
-    ## Arguments:
-
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
+    Args:
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
 
-    ## Returns:
+    Returns:
+        list: List of datasets uploaded to the `twinLab` cloud.
 
-    - `list` of `str` dataset IDs.
+    Examples:
+        .. code-block:: python
 
-    ## Example:
+            datasets = tl.list_datasets()
+            print(datasets)
 
-    ```python
-    import pandas as pd
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    datasets = tl.list_datasets()
-    print(datasets)
-    ```
     """
     _, response = api.list_datasets(verbose=debug)
     datasets = _get_value_from_body("datasets", response)
     if verbose:
         print("Datasets:")
         pprint(datasets, compact=True, sort_dicts=False)
     return datasets
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def view_dataset(
     dataset_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> pd.DataFrame:
     """
-    # View dataset
 
-    View a dataset that exists on the twinLab cloud.
-
-    ## Arguments:
-
-    - `dataset_id`: `str`. Name for the dataset when saved to the twinLab cloud.
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    ## Returns:
-
-    - `pandas.DataFrame` of the dataset.
+    View dataset
 
+    View a dataset that exists on the twinLab cloud.
 
-    ## Example:
+    Args:
+        dataset_id (str): Name for the dataset when saved to the twinLab cloud.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        pandas.DataFrame: Dataframe of the dataset
+
+    Examples:
+        .. code-block:: python
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            df = tl.view_dataset("my_dataset")
+            print(df)
 
-    ```python
-    import pandas as pd
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    df = tl.view_dataset("my_dataset")
-    print(df)
-    ```
     """
     _, response = api.view_dataset(dataset_id, verbose=debug)
     csv_string = _get_value_from_body("dataset", response)
     csv_string = io.StringIO(csv_string)
     df = pd.read_csv(csv_string, sep=",")
     if verbose:
         print("Dataset:")
         print(df)
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def query_dataset(
     dataset_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> pd.DataFrame:
     """
-    # Query dataset
-
-    Query a dataset that exists on the `twinLab` cloud by printing summary statistics.
-
-    ## Arguments:
 
-    - `dataset_id`: `str`. Name of dataset on S3. This should be the same as the uploaded file name.
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
+    Query dataset
 
-    ## Returns:
-
-    - `pandas.DataFrame` containing summary statistics for the dataset.
+    Query a dataset that exists on the `twinLab` cloud by printing summary statistics.
 
-    ## Example:
+    Args:
+        dataset_id (str): Name of dataset on S3. This should be the same as the uploaded file name.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        pandas.DataFrame: Dataframe containing summary statistics for the dataset
+
+    Examples:
+        .. code-block:: python
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            df = tl.query_dataset("my_dataset")
+            print(df)
 
-    ```python
-    import pandas as pd
-    import twinlab as tl
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    df = tl.query_dataset("my_dataset")
-    print(df)
-    ```
     """
     _, response = api.summarise_dataset(dataset_id, verbose=debug)
     csv_string = _get_value_from_body("dataset_summary", response)
     csv_string = io.StringIO(csv_string)
     df = pd.read_csv(csv_string, index_col=0, sep=",")
     if verbose:
         print("Dataset summary:")
         print(df)
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def delete_dataset(
     dataset_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> None:
     """
-    # Delete dataset
+
+    Delete dataset
 
     Delete a dataset from the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        dataset_id (str): Name of dataset to delete from the Cloud.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Examples:
+        .. code-block:: python
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            tl.delete_dataset("my_dataset")
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `dataset_id`: `str`. Name of dataset to delete from the Cloud.
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    tl.delete_dataset("my_dataset")
-    ```
     """
     _, response = api.delete_dataset(dataset_id, verbose=debug)
     if verbose:
         message = _get_message(response)
         print(message)
 
 
 ###  ###
 
 ### Campaign functions ###
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def train_campaign(
     filepath_or_params: Union[str, dict],
     campaign_id: str,
     ping_time: Optional[float] = PING_TIME_TRAIN_DEFAULT,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
 ) -> None:
     """
-    # Train campaign
 
     Train a campaign in the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        filepath_or_params (str): `dict`. Union. Filepath to local json or parameters dictionary for training.
+        campaign_id (str): Name for the final trained campaign.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+        dataset_id (str): Dataset ID of the dataset as stored in the Cloud.
+        inputs (list): A list of strings referring to the columns in the
+        outputs (list): A list of strings referring to the columns in the
+        estimator (str, optional): `Optional`. The type of estimator used in the pipeline. This can be either
+        estimator_kwargs (dict, optional): `Optional`. Keywords passed to the underlying estimator.
+        decompose_input (bool, optional): `Optional`. Specifies whether the input parameters
+        input_explained_variance (float, optional): `Optional`. Specifies how much of the
+        decompose_output (bool, optional): `Optional`. Specifies whether the output parameters
+        output_explained_variance (float, optional): `Optional`. Specifies how much of the
+        train_test_ratio (float, optional): `Optional`. Specifies the ratio of training samples in
+        model_selection (bool, optional): `Optional`. Whether to run model selection.
+        model_selection_kwargs (dict, optional): `Optional`. Keywords passed to the model
+        seed (int, optional): `Optional`. Specifies the seed for the random number generator.
+
+    Examples:
+
+        Train using a local `.json` parameters file:
+
+        .. code-block:: python
+
+            import twinlab as tl
+
+            tl.train_campaign("path/to/params.json", "my_campaign")
+
+        Train via a `python` dictionary:
+
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `filepath_or_params`: `str`, `dict`, Union. Filepath to local json or parameters dictionary for training.
-    - `campaign_id`: `str`. Name for the final trained campaign.
-    **Warning:** If the `campaign_id` already exists for the current Cloud account, it will be overwritten by the
-    newly trained campaign.
-    - `ping_time`: `float`, `Optional`. Time in seconds between pings to the server to check if the job is complete.
-    - `processor`: `str`, `Optional`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    The parameters retrieved from the first argument are divided into 2 different sets of parameters; one for
-    setting up the campaign, and the other for training the campaign.
-
-    Parameters to setup the campaign (used during initialization of a Campaign class object):
-    - `dataset_id`: `str`. Dataset ID of the dataset as stored in the Cloud.
-    - `inputs`: `list`. A list of strings referring to the columns in the
-                `pandas.DataFrame` that will be used as input parameters.
-    - `outputs`: `list`. A list of strings referring to the columns in the
-                `pandas.DataFrame` that will be used as output parameters.
-    - `estimator`: `str`, `Optional`. The type of estimator used in the pipeline. This can be either
-                "gaussian_process_regression" or "gradient_boosting_regression".
-    - `estimator_kwargs`: `dict`, `Optional`. Keywords passed to the underlying estimator.
-                The estimator_kwargs dictionary for "gaussian_process_regression" allows the
-                following keywords:
-                `detrend`: `bool`, `Optional`. Specifies whther to linearly detrend the output
-                        data before estimator fitting. Defaults to False.
-                `device`: `str`, `Optional`. Specifies whether to fit the estimator using
-                        "cpu" or "gpu". Default is `"cpu"`.
-    - `decompose_input`: `bool`, `Optional`. Specifies whether the input parameters
-                should be decomposed.
-    - `input_explained_variance`: `float`, `Optional`. Specifies how much of the
-                variance should be explained after the truncation of the SVD
-                (Singular Value Decomposition) for functional input.
-    - `decompose_output`: `bool`, `Optional`. Specifies whether the output parameters
-                should be decomposed.
-    - `output_explained_variance`: `float`, `Optional`. Specifies how much of the
-                variance should be explained after the truncation of the SVD
-                (Singular Value Decomposition) for functional output.
-
-    Parameters to train the campaign (used when the fit() function is called using a Campaign class object for training):
-    - `train_test_ratio`: `float`, `Optional`. Specifies the ratio of training samples in
-            the dataset.
-    - `model_selection`: `bool`, `Optional`. Whether to run model selection.
-    - `model_selection_kwargs`: `dict`, `Optional`. Keywords passed to the model
-            selection process.
-            The model_selection_kwargs dictionary for "gaussian_process_regression" allows the
-            following keywords:
-            `seed`: `int`, `Optional`. Specifies the seed for the random number genrator for every
-                trial of the model selection process.
-            `evaluation_metric`: `str`, `Optional`. Specifies the evaluation metric used to score
-                different configuration during the model selection process. This can be "BIC" or "MSLL". The
-                default is `"MSLL"`.
-            `val_ratio`: `float`, `Optional`. Specifies the percentage of random validation data
-                allocated to to compute the "BIC" metric. The default is `0.2`.
-            `base_kernels`: `Set[str]`, `Optional`. Specifies the list of kernels to use for
-                Compositional Kernel Search. This can be "all", "restricted" or a `Set[str]` object.
-                Set of available kernels are ["LIN", "M12", "M32", "M52", "PER", "RBF", "RQF"].
-                The default is `"restricted"`; using ["LIN", "M32", "M52", "PER", "RBF"].
-            `depth`: `int`, `Optional`. Specifies the number of base kernels to be combined in
-                the Compositional Kernel Search. A `depth=3` means the resulting kernel may be
-                composed from three base kernels, e.g. "(LIN+PER)*RBF" or "(M12*RBF)+RQF".
-                Default is `1`.
-            `beam`: `int`, `Optional`. Specifies the beam width of the Compositional Kernel Search
-                algorithm. For example, `beam=1` is an exhaustive search (algorithmically 'greedy'); `beam=None` performs breadth-first search, and
-                `beam>1` perfroms the beam search with the specified beam value. Default is `None`.
-            `resources_per_trial`: `dict`, `Optional`. The amount of CPU and GPU resources allocated
-                to each trial of model selection. Default is `{"cpu": 1, "gpu": 0}`.
-    - `seed`: `int`, `Optional`. Specifies the seed for the random number generator.
-
-    ## Example:
-
-    Train using a local `.json` parameters file:
-
-    ```python
-    import twinlab as tl
-
-    tl.train_campaign("path/to/params.json", "my_campaign")
-    ```
-
-    Train via a `python` dictionary:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    ```
     """
     if type(filepath_or_params) is dict:
         params = filepath_or_params
     elif type(filepath_or_params) is str:
         filepath = filepath_or_params
         params = json.load(open(filepath))
     else:
@@ -632,211 +612,227 @@
     complete = False
     while not complete:
         status = _status_campaign(campaign_id, verbose=False, debug=debug)
         complete = _get_value_from_body("job_complete", status)
         time.sleep(ping_time)
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def list_campaigns(
     verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> list:
     """
-    # List campaigns
+
+    List campaigns
 
     List campaigns that have been completed to the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
 
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
+    Returns:
+        list
 
-    ## Returns:
+    Examples:
+        .. code-block:: python
 
-    - A `list` of `str` campaign IDs.
+            import twinlab as tl
 
-    ## Example:
+            campaigns = tl.list_campaigns()
+            print(campaigns)
 
-    ```python
-    import twinlab as tl
 
-    campaigns = tl.list_campaigns()
-    print(campaigns)
-    ```
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
+
     """
     _, response = api.list_models(verbose=debug)
     campaigns = _get_value_from_body("models", response)
     if verbose:
         print("Trained models:")
         pprint(campaigns, compact=True, sort_dicts=False)
     return campaigns
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def view_campaign(
     campaign_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> dict:
     """
-    # View campaign
+
+    View campaign
 
     View a campaign that exists on the twinLab cloud.
 
-    ## Arguments:
+    Args:
+        campaign_id (str): Name for the model when saved to the twinLab cloud.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        dict: containing the campaign training parameters
+
+    Examples:
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            params = tl.view_campaign("my_campaign")
+            print(params)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `campaign_id`: `str`. Name for the model when saved to the twinLab cloud.
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    ## Returns:
-
-    - `dict` containing the campaign training parameters.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    params = tl.view_campaign("my_campaign")
-    print(params)
-    ```
     """
     _, response = api.view_model(campaign_id, verbose=debug)
     model_parameters = response
     if verbose:
         print("Campaign summary:")
         pprint(model_parameters, compact=True, sort_dicts=False)
     return model_parameters
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def query_campaign(
     campaign_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> dict:
     """
-    # Query campaign
+
+    Query campaign
 
     Get summary statistics for a pre-trained campaign in the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        campaign_id (str): Name of trained campaign to query
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        dict: containing summary statistics for the pre-trained campaign
+
+    Examples:
+        .. code-block:: python
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            info = tl.query_campaign("my_campaign")
+            print(info)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `campaign_id`: `str`. Name of trained campaign to query
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    ## Returns:
-
-    - `dict` containing summary statistics for the pre-trained campaign.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    info = tl.query_campaign("my_campaign")
-    print(info)
-    ```
     """
     _, response = api.summarise_model(campaign_id, verbose=debug)
     summary = response
     if verbose:
         print("Model summary:")
         pprint(summary, compact=True, sort_dicts=False)
     return summary
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def predict_campaign(
     filepath_or_df: Union[str, pd.DataFrame],
     campaign_id: str,
     sync: Optional[bool] = False,
     ping_time: Optional[float] = PING_TIME_PREDICT_DEFAULT,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
-    # Predict campaign
+
+    Predict campaign
 
     Make predictions from a pre-trained model that exists on the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        filepath_or_df (str): Location of .csv file dataset on local machine
+        campaign_id (str): Name of pre-trained campaign to use for predictions.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+        campaign_id (str`.):
+
+    Returns:
+        tuple: containing
+        df_mean:
+        df_std:
+
+    Examples:
+
+        Using a local file:
+
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            filepath = "path/to/data.csv" # Local
+            campaign_id = 'my_campaign" # Pre-trained
+            df_mean, df_std = tl.predict_campaign(filepath, campaign_id)
+            print(df_mean)
+            print(df_std)
+
+        Using a `pandas.DataFrame`:
+
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+            tl.predict_campaign(df, "my_campaign")
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `filepath_or_df`: `str`. Location of .csv file dataset on local machine
-        or `pandas.DataFrame` for evaluation
-    - `campaign_id`: `str`. Name of pre-trained campaign to use for predictions.
-    - `processor`: `str`, `Optional`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    - `campaign_id`: `str`.
-
-    **NOTE:** Evaluation data must be a .csv file, or a `pandas.DataFrame` that is interpretable as a .csv.
-
-    ## Returns:
-
-     - `tuple` containing:
-        - `df_mean`: `pandas.DataFrame` containing mean predictions.
-        - `df_std`: `pandas.DataFrame` containing standard deviation predictions.
-
-    ## Example:
-
-    Using a local file:
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    filepath = "path/to/data.csv" # Local
-    campaign_id = 'my_campaign" # Pre-trained
-    df_mean, df_std = tl.predict_campaign(filepath, campaign_id)
-    print(df_mean)
-    print(df_std)
-    ```
-
-    Using a `pandas.DataFrame`:
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-    tl.predict_campaign(df, "my_campaign")
-    ```
     """
 
     if sync:
         csv = _use_campaign(
             campaign_id,
             method="predict",
             filepath_or_df=filepath_or_df,
@@ -872,84 +868,87 @@
         print(df_mean)
         print("Standard deviation predictions:")
         print(df_std)
 
     return df_mean, df_std
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def sample_campaign(
     filepath_or_df: Union[str, pd.DataFrame],
     campaign_id: str,
     num_samples: int,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
-    # Sample campaign
+
+    Sample campaign
 
     Draw samples from a pre-trained campaign that exists on the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        filepath_or_df (str): Location of .csv dataset on local machine for evaluation
+        campaign_id (str): Name of pre-trained campaign to use for predictions.
+        num_samples (int): Number of samples to draw for each row of the evaluation data.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        pandas.DataFrame: with the sampled values
+
+    Examples:
+        Using a local file:
+
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            filepath = "path/to/data.csv" # Local
+            n = 10
+            df_mean, df_std = tl.sample_campaign(filepath, "my_campaign", n)
+            print(df_mean)
+            print(df_std)
+
+        Using a `pandas.DataFrame`:
+
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+            n = 10
+            tl.sample_campaign(df, "my_campaign", n)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `filepath_or_df`: `str`. Location of .csv dataset on local machine for evaluation
-        or `pandas.DataFrame`.
-    - `campaign_id`: `str`. Name of pre-trained campaign to use for predictions.
-    - `num_samples`: `int`. Number of samples to draw for each row of the evaluation data.
-    - `processor`: `str`, `Optional`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    **NOTE:** Evaluation data must be a .csv file, or a `pandas.DataFrame` that is interpretable as a .csv.
-
-    ## Returns:
-
-    - `pandas.DataFrame` with the sampled values.
-
-    ## Example:
-
-    Using a local file:
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    filepath = "path/to/data.csv" # Local
-    n = 10
-    df_mean, df_std = tl.sample_campaign(filepath, "my_campaign", n)
-    print(df_mean)
-    print(df_std)
-    ```
-
-    Using a `pandas.DataFrame`:
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-    n = 10
-    tl.sample_campaign(df, "my_campaign", n)
-    ```
     """
 
     csv = _use_campaign(
         campaign_id,
         method="sample",
         filepath_or_df=filepath_or_df,
         num_samples=num_samples,
@@ -961,58 +960,64 @@
     df = pd.read_csv(csv, header=[0, 1], sep=",")
     if verbose:
         print("Samples:")
         print(df)
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def active_learn_campaign(
     campaign_id: str,
     num_points: int,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
-    # Active learn campaign
+
+    Active learn campaign
 
     Draw new candidate data points via active learning from a pre-trained campaign
+
     that exists on the `twinLab` cloud.
 
-    ## Arguments:
-    - `campaign_id`: `str`. Name of pre-trained campaign to use for predictions.
-    - `num_points`: `int`. Number of samples to draw for each row of the evaluation data.
-    - `processor`: `str`, `Optional`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-
-    ## Returns:
-
-    - `pandas.DataFrame` containing the recommended sample locations
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    n = 10
-    df = tl.active_learn_campaign("my_campaign", n)
-    print(df)
-    ```
+    Args:
+        campaign_id (str): Name of pre-trained campaign to use for predictions.
+        num_points (int): Number of samples to draw for each row of the evaluation data.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+
+    Returns:
+        pandas.DataFrame: containing the recommended sample locations
+
+    Examples:
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            n = 10
+            df = tl.active_learn_campaign("my_campaign", n)
+            print(df)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
+
     """
 
     csv = _use_campaign(
         campaign_id,
         method="get_candidate_points",
         acq_func="qNIPV",
         num_points=num_points,
@@ -1024,65 +1029,66 @@
     df = pd.read_csv(csv, sep=",")
     if verbose:
         print("Candidate points:")
         print(df)
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def optimise_campaign(
     campaign_id: str,
     num_points: int,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
-    # Optimise campaign
+
+    Optimise campaign
 
     Draw new candidate data points by optimizing for "qEI" (Monte Carlo Expected Improvement)
+
     acquisition function from a pre-trained campaign that exists on the `twinLab` cloud.
 
-    ## Arguments:
-    - `campaign_id`: `str`. Name of pre-trained campaign to use for predictions.
-    - `num_points`: `int`. Number of samples to draw for each row of the evaluation data.
-    - `processor`: `str`, `Optional`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`, `Optional`. Determining level of information returned to the user.
-    - `debug`: `bool`, `Optional`. Determining level of information logged on the server.
-    - `acq_kwargs`: `dict`, `Optional`. Specifies the keyword arguments to modify the behavior of
-        the acquisition function. This dictionary currently allows only one keyword argument.
-        - `weights`: `list[float]`. Specifies the weightage for different objectives to be
-            optimised in a mulit-objective optimisation scenario. By default all weights are equal.
-            For example, for a problem with two outputs, if the weights are as follows `[1, 0.5]`, this indicates
-            that we focus on maximising the first output dimension twice as much as
-            the second output dimension.
-
-    ## Returns:
-
-    - `pandas.DataFrame` containing the recommended sample locations.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [0.0, 0.25, 0.75, 1.0], 'y': [-1.60856306, -0.27526546, -0.34670215, -1.65062947]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    n = 1
-    df = tl.optimise_campaign("my_campaign", n)
-    print(df)
-    ```
+    Args:
+        campaign_id (str): Name of pre-trained campaign to use for predictions.
+        num_points (int): Number of samples to draw for each row of the evaluation data.
+        verbose (bool, optional): `Optional`. Determining level of information returned to the user.
+        acq_kwargs (dict, optional): `Optional`. Specifies the keyword arguments to modify the behavior of
+        weights (list[float]): Specifies the weightage for different objectives to be
+
+    Returns:
+        pandas.DataFrame: containing the recommended sample locations
+
+    Examples:
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [0.0, 0.25, 0.75, 1.0], 'y': [-1.60856306, -0.27526546, -0.34670215, -1.65062947]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            n = 1
+            df = tl.optimise_campaign("my_campaign", n)
+            print(df)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
+
     """
 
     csv = _use_campaign(
         campaign_id,
         method="get_candidate_points",
         acq_func="qEI",
         num_points=num_points,
@@ -1094,61 +1100,65 @@
     df = pd.read_csv(csv, sep=",")
     if verbose:
         print("Candidate points:")
         print(df)
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def solve_inverse_campaign(
     campaign_id: str,
     filepath_or_df: Union[str, pd.DataFrame],
     filepath_or_df_std: Union[str, pd.DataFrame],
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = False,
     debug: Optional[bool] = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
-    # Inverse modelling on campaign
+
+    Inverse modelling on campaign
 
     Given a set of observations, inverse modelling finds the model that would best suit the data.
 
-    ## Arguments:
+    Args:
+        campaign_id (str): Name of pre-trained campaign to use for predictions.
+        data_csv (pandas.DataFrame): A `pandas.DataFrame` of observations.
+        data_std_csv`  (pandas.DataFrame): A `pandas.DataFrame` of errors on the observations.
+        verbose (bool): Determining level of information returned to the user.
+
+    Returns:
+        pandas.DataFrame: containing the recommended model statistics
+
+    Examples:
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            data_csv = pd.DataFrame({'y': [1]})
+            data_std_csv = pd.DataFrame({'y': [0.498]})
+            df = tl.solve_inverse_campaign("my_campaign", data_csv, data_std_csv)
+            print(df)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `campaign_id`: `str`. Name of pre-trained campaign to use for predictions.
-    - `data_csv`: `pandas.DataFrame`. A `pandas.DataFrame` of observations.
-    - `data_std_csv` : `pandas.DataFrame`. A `pandas.DataFrame` of errors on the observations.
-    - `processor`: `str`. Processor to use for sampling ("cpu"; "gpu").
-    - `verbose`: `bool`. Determining level of information returned to the user.
-    - `debug`: `bool`. Determining level of information logged on the server.
-
-    ## Returns:
-
-    - `pandas.DataFrame` containing the recommended model statistics.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    data_csv = pd.DataFrame({'y': [1]})
-    data_std_csv = pd.DataFrame({'y': [0.498]})
-    df = tl.solve_inverse_campaign("my_campaign", data_csv, data_std_csv)
-    print(df)
-    ```
     """
 
     csv = _use_campaign(
         campaign_id,
         method="solve_inverse",
         filepath_or_df=filepath_or_df,
         filepath_or_df_std=filepath_or_df_std,
@@ -1169,45 +1179,51 @@
     if verbose:
         print("Inverse model statistics:")
         print(df)
 
     return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def score_campaign(
     campaign_id: str,
     combined_score: Optional[bool] = False,
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = True,
     debug: Optional[bool] = False,
 ) -> Optional[Union[float, pd.DataFrame]]:
     """
-    # Quantify the performance of your trained model with a model score.
 
-    ## Arguments:
-    - `combined_score`: `bool`. Determining whether to average scores across dimensions. If False, will return a `numpy` array even if only one dimension.
+    Quantify the performance of your trained model with a model score.
 
-    ### Returns:
+    Args:
+        combined_score (bool): Determining whether to average scores across dimensions. If False. will return a `numpy` array even if only one dimension.
 
-    Either:
-    - `pandas.DataFrame`. Containing the scores for each output dimension.
-    - `float. Containing the average score across all output dimensions.
-    - `None` if no test data is available.
+    Returns:
+        None:
+        float:
+        pandas.DataFrame: containing the trained model score
 
-    ### Example:
+    Examples:
+        .. code-block:: python
 
-    ```python
-    import pandas as pd
-    import twinlab as tl
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+            tl.predict_campaign(df, "my_campaign")
+            tl.score_campaign(df, combined_score=True)
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-    tl.predict_campaign(df, "my_campaign")
-    tl.score_campaign(df, combined_score=True)
-    ```
     """
 
     score = _use_campaign(
         campaign_id,
         method="score",
         combined_score=combined_score,
         processor=processor,
@@ -1218,58 +1234,64 @@
         score = pd.read_csv(score, sep=",")
     if verbose:
         print("Campaign Score:")
         print(score)
     return score
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def get_calibration_curve_campaign(
     campaign_id: str,
     type: Optional[str] = "quantile",
     processor: Optional[str] = "cpu",
     verbose: Optional[bool] = True,
     debug: Optional[bool] = False,
 ) -> Optional[pd.DataFrame]:
     """
-    # Quantify the performance of your trained model with a calibration curve.
 
-    ## Arguments:
+    Quantify the performance of your trained model with a calibration curve.
+
+    Args:
+        type (str): Determine whether to use "quantiile" or "interval" for the model calibration error.
 
-    - `type`: `str`. Determine whether to use "quantiile" or "interval" for the model calibration error.
+    Returns:
+        None:
+        pd.DataFrame: containing the data for the calibration curve
 
-    ## Returns:
+    Examples:
+        .. code-block:: python
 
-    - Either:
-    - `pandas.DataFrame` containing the data for the calibration curve in each output dimension.
-    - `None` if no test data is available.
+            import pandas as pd
+            import twinlab as tl
 
-    ## Example:
+            df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
+            tl.train_campaign(df, "my_campaign")
+            tl.get_calibration_curve(df, type="quantile")
 
-    ```pyt
-    import pandas as pd
-    import twinlab as tl
+            # Plot the calibration curve
 
-    df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-    tl.train_campaign(df, "my_campaign")
-    tl.get_calibration_curve(df, type="quantile")
+            fraction_observed = tl.get_calibration_curve(type="quantile")
+            fraction_expected = np.linspace(0,1,fraction_observed.shape[0])
 
-    # Plot the calibration curve
-    fraction_observed = tl.get_calibration_curve(type="quantile")
-    fraction_expected = np.linspace(0,1,fraction_observed.shape[0])
+            fig, ax = plt.subplots(figsize=(5, 5))
 
-    fig, ax = plt.subplots(figsize=(5, 5))
-    ax.set_title("Calibration curve")
-    ax.set_xlabel("Expected coverage")
-    ax.set_ylabel("Observed coverage")
+            ax.set_title("Calibration curve")
+            ax.set_xlabel("Expected coverage")
+            ax.set_ylabel("Observed coverage")
+            plt.plot(np.linspace(0, 1, 100), fraction_observed)
+            plt.plot(np.linspace(0, 1, 100), np.linspace(0, 1, 100), "--")
+            plt.show()
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    plt.plot(np.linspace(0, 1, 100), fraction_observed)
-    plt.plot(np.linspace(0, 1, 100), np.linspace(0, 1, 100), "--")
-    plt.show()
-    ```
     """
 
     csv = _use_campaign(
         campaign_id,
         method="get_calibration_curve",
         type=type,
         processor=processor,
@@ -1280,45 +1302,51 @@
         df = pd.read_csv(csv, sep=",")
         if verbose:
             print("Calibration curve information:")
             pprint(df)
         return df
 
 
+@deprecated(
+    version=DEPRECATION_VERSION,
+    reason=f"The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.",
+)
 @typechecked
 def delete_campaign(
     campaign_id: str, verbose: Optional[bool] = False, debug: Optional[bool] = False
 ) -> None:
     """
-    # Delete campaign
+
+    Delete campaign
 
     Delete campaign from the `twinLab` cloud.
 
-    ## Arguments:
+    Args:
+        campaign_id (str:):
+        verbose (bool, optional): Optional. determining level of information returned to the user.
+
+    Examples:
+        .. code-block:: python
+
+            import pandas as pd
+            import twinlab as tl
+
+            df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
+            tl.upload_dataset(df, "my_dataset")
+            params = {
+                "dataset_id": "my_dataset",
+                "inputs": ["X"],
+                "outputs": ["y"],
+            }
+            tl.train_campaign(params, "my_campaign")
+            tl.delete_campaign("my_campaign")
+
+    .. deprecated:: 2.5.0
+        The twinLab Python client version v1 will be deprecated imminently. Please upgrade to the latest version of the twinLab Python client. Avaible at https://pypi.org/project/twinlab/.
 
-    - `campaign_id`: `str`; name of trained campaign to delete from the cloud.
-    - `verbose`: `bool`, Optional, determining level of information returned to the user.
-    - `debug`: `bool`, Optional, determining level of information logged on the server.
-
-    ## Example:
-
-    ```python
-    import pandas as pd
-    import twinlab as tl
-
-    df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-    tl.upload_dataset(df, "my_dataset")
-    params = {
-        "dataset_id": "my_dataset",
-        "inputs": ["X"],
-        "outputs": ["y"],
-    }
-    tl.train_campaign(params, "my_campaign")
-    tl.delete_campaign("my_campaign")
-    ```
     """
     _, response = api.delete_model(campaign_id, verbose=debug)
     if verbose:
         message = _get_message(response)
         print(message)
```

### Comparing `twinlab-2.4.0/twinlab/distributions.py` & `twinlab-2.5.0/twinlab/distributions.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 @typechecked
 class DistributionMethods(Enum):
     UNIFORM = "uniform"
 
 
 @typechecked
 class Uniform:
-    """
-    Represents a one-dimensional uniform distribution between a minimum and maximum value.
+    """A one-dimensional continous uniform distribution between a minimum and maximum value.
 
     Args:
         min (float): The minimum value of the distribution.
         max (float): The maximum value of the distribution.
+
     """
 
     def __init__(self, min: float, max: float):
         self.min = min
         self.max = max
 
     def to_json(self):
```

### Comparing `twinlab-2.4.0/twinlab/emulator.py` & `twinlab-2.5.0/twinlab/emulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -169,82 +169,66 @@
         raise ValueError(f"Method {method} not recognised")
 
 
 ### ###
 
 
 class Emulator:
-    """
-    # Emulator
-
-    A class representing a trainable twinLab emulator.
-
-    ## Attributes:
-
-    - `id`: `str`. This is the name of the emulator in the twinLab cloud.
-
-    ## Methods:
-
-    - `train()`. Performs the training of an emulator on the `twinLab` cloud.
-    - `view()`. Returns the training parameters of a trained emulator on the `twinLab` cloud.
-    - `summarise()`. Returns a statistical summary of a trained emulator on the `twinlab` cloud.
-    - `score()`. Returns a calibration curve for a trained emulator on the `twinlab` cloud.
-    - `benchmark()`. Returns a calibration curve for a trained emulator on the `twinlab` cloud.
-    - `predict()`. Returns the emulator prediction on the specified input data.
-    - `sample()`. Returns samples generated from the posterior distribution of the estimator.
-    - `recommend()`. Returns candidate data points from a trained emulator on the `twinLab` cloud.
-    - `calibrate()`. Returns a model that best suits the specified input data.
-    - `delete()`. Deletes an emulator on the `twinlab` cloud.
+    """A trainable twinLab emulator.
 
+    An emulator is trainable model that learns the trends in a dataset.
+    It is a machine-learning model in that it requires a dataset of inputs ``X`` and outputs ``y`` on which to be trained.
+    In this way, it learns to mimic, or emulate, the dataset and can be used to make predictions on new data.
+    Emulators are also often called models, surrogates, or digital twins.
+
+    Attributes:
+        id (str): The name for the emulator in the twinLab cloud.
+            If an emulator that does not currently exist is specified, then a new emulator will be instantiated.
+            Otherwise the corresponding emulator will be loaded from the cloud.
+            Be sure to double check which emulators have been created using .. autofunction:: `~list_emulator`.
     """
 
     @typechecked
     def __init__(self, id: str):
         self.id = id
 
-    # @typechecked # TODO: Does not work with List[Prior]??
+    # @typechecked # TODO: Typecheck does not seem to work with List[Prior]??
     def design(
         self,
         priors: List[Prior],
         num_points: int,
         params: DesignParams = DesignParams(),
         verbose: bool = False,
     ) -> pd.DataFrame:
-        """
-        # Design
-
-        Get an initial design space for your emulator
-
-        ## Arguments:
-
-        - `priors`: `List[Prior]`. A list of `Prior` objects that define the prior distributions for each input.
-        - `num_points`: `int`. Number of points to sample in each dimension.
-        - `params`: `DesignParams`, `Optional`. An `DesignParams` object that contains all of the optional initial design parameters.
+        """Generate an initial design space for an emulator.
 
-        ## Returns:
-
-        - `pandas.DataFrame` containing the initial design space.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        emulator = tl.Emulator("emulator_id")
-
-        my_priors = [
-            tl.Prior("x1", tl.distribution.Uniform(0, 12)),
-            tl.Prior("x2", tl.distribution.Uniform(0, 0.5)),
-            tl.Prior("x3 ", tl.distribution.Uniform(0, 10)),
-        ]
+        The method is used to generate an initial design for evaluating a set of experiments, emulator, or simulation.
+        This is useful if data has not yet been collected and a user wants to generate an initial design space to train an emulator.
+        Optimal space-filling methods can be used to generate an initial design space that are significantly better than either random or grid sampling.
+        If data has already been acquired then an initial emulator can be trained using ``Emulator.train()`` and new sampling locations can be recommended using ``Emulator.recommend()``.
+
+        Args:
+            priors (list[Prior]): A list of ``Prior`` objects that define the prior distributions for each input.
+                These are independent one-dimensional probability distributions for each parameter.
+            num_points (int): The number of points to sample in designing the initial space.
+            params (twinlab.DesignParams, optional): A parameter configuration that contains all of the optional initial-design parameters.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("emulator_id")
+
+                my_priors = [
+                    tl.Prior("x1", tl.distribution.Uniform(0, 12)),
+                    tl.Prior("x2", tl.distribution.Uniform(0, 0.5)),
+                    tl.Prior("x3 ", tl.distribution.Uniform(0, 10)),
+                ]
 
-        initial_design = emulator.design(my_priors, 10)
+                initial_design = emulator.design(my_priors, 10)
 
-        ```
         """
         # Convert priors to json so they can be passed through the API
         priors = [prior.to_json() for prior in priors]
 
         # Call the API function
         _, response = api.get_initial_design(
             priors,
@@ -273,39 +257,54 @@
         dataset: Dataset,
         inputs: List[str],
         outputs: List[str],
         params: TrainParams = TrainParams(),
         wait: bool = True,
         verbose: bool = False,
     ) -> Optional[str]:
-        """
-        # Train
+        """Train an emulator on the twinLab cloud.
 
-        Train an emulator on the `twinLab` cloud.
+        This is the primary functionality of twinLab, where an emulator is trained on a dataset.
+        The emulator learns trends in the dataset and then is able to make predictions on new data.
+        These new data can be far away from the training data, and the emulator will interpolate between the training data points.
+        The emulator can also be used to extrapolate beyond the training data, but this is less reliable.
+        The emulator can be trained on a dataset with multiple inputs and outputs,
+        and can be used to make predictions on new data with multiple inputs and outputs.
+        The powerful algorithms in twinLab allow for the emulator to not only make predictions,
+        but to also quantify the uncertainty in these predictions.
+        This is extremely advantageous, because it allows for the reliability of the predictions to be quantified.
+
+        Args:
+            dataset (Dataset): The training and test data for the emulator.
+                The ratio of train to test data can be set in ``TrainParams``.
+            inputs (list[str]): A list of the input column names in the training dataset.
+                These correspond to the independent variables in the dataset, which are often the parameters of a model.
+                These are usually known as ``X`` (note that capital) values.
+            outputs (list[str]): A list of the output column names in the training dataset.
+                These correspond to the dependent variables in the dataset, which are often the results of a model.
+                These are usually known as ``y`` values.
+            params (TrainParams, optional): A training parameter configuration that contains all optional training parameters.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+                Setting ``wait=False`` is useful for longer training jobs.
+            verbose (bool, optional): Display information about the operation while running.
+
+        Returns:
+            If ``wait=True`` the function will run until the emulator is trained on the cloud.
+            If ``wait=False`` the function will return the process ID and exit.
+            This is useful for longer training jobs.
+            The training status can then be checked later using ``Emulator.status()``.
+
+        Example:
+            .. code-block:: python
+
+                df = pd.DataFrame({"X": [1, 2, 3, 4], "y": [1, 4, 9, 16]})
+                dataset = tl.Dataset("my_dataset")
+                dataset.upload(df)
+                emulator.train(dataset, ["X"], ["y"])
 
-        ## Arguments:
-
-        - `dataset`: `Dataset`. twinLab dataset object which contains the training data for the emulator.
-        - `inputs`: `list[str]`. List of input names in the training dataset.
-        - `outputs`; `list[str]`. List of output names in the training dataset.
-        - `params`: `TrainParams`, `optional`. A `TrainParams` object that contains all necessary training parameters.
-        - `wait`: `bool`, `optional`. If `True`, wait for the job to complete, otherwise return the process ID and exit.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator.train(dataset, ['X'], ['y'])
-        ```
         """
 
         # Making a dictionary from TrainParams class
         if PROCESSOR == "gpu":
             print(
                 "Emulator is being trained on GPU. Inference operations must also be performed on GPU"
             )
@@ -331,169 +330,197 @@
             return self.process_id
         _wait_for_training_completion(self.id, self.process_id, verbose=verbose)
         if verbose:
             print(
                 f"Training of emulator {self.id} with process ID {self.process_id} is complete!"
             )
 
+    # TODO: This seems to be completely broken!! There is no self.process_id!!
     @typechecked
-    def status(self, verbose: bool = False) -> Tuple[int, dict]:
-        asynch_status, response = api.train_response_model(
-            self.id, self.process_id, verbose=DEBUG
-        )
-        if verbose:
-            message = utils.get_message(response)
-            print(message)
-        return asynch_status, response
+    def status(self, process_id: str, verbose: bool = False) -> dict:
+        """Check the status of a training process on the twinLab cloud.
 
-    @typechecked
-    def view(self, verbose: bool = False) -> dict:
-        """
-        # View
+        Args:
+            process_id (str): The process ID of the training process to check the status of.
+            verbose (bool, optional): Display information about the operation while running.
 
-        View an emulator that exists on the `twinLab` cloud.
+        Returns:
+            Tuple[int, dict]: A tuple containing the status code and the response body.
 
-        ## Arguments:
+        Example:
+            .. code-block:: python
 
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user. Default is False.
+                emulator = tl.Emulator("beb7f97f")
+                emulator.status()
 
-        ## Returns:
+            .. code-block:: console
 
-        - `dict` containing the emulator training parameters.
+                {
+                    'process_status': 'Your job has finished and is on its way back to you.',
+                    'process_id': 'beb7f97f',
+                }
 
-        ## Example:
+        """
+        _, response = api.train_response_model(self.id, process_id, verbose=DEBUG)
+        message = _get_response_message(response)
+        if verbose:
+            print(message)
+        return response
 
-        ```python
-        import pandas as pd
-        import twinlab as tl
+    @typechecked
+    def view(self, verbose: bool = False) -> dict:
+        """View an emulator that exists on the twinLab cloud.
+
+        This returns the parameter configuration of the emulator that is stored on the twinLab cloud.
+        This allows a user to check the parameters that were used to train an emulator.
+
+        Args:
+            verbose (bool, optional): Display information about the operation while running.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.view()
+
+            .. code-block:: console
+
+                {'dataset_id': 'quickstart',
+                 'decompose_inputs': False,
+                 'decompose_outputs': False,
+                 'estimator': 'gaussian_process_regression',
+                 'estimator_kwargs': {'detrend': False, 'estimator_type': 'single_task_gp'},
+                 'inputs': ['x'],
+                 'modal_handle': 'fc-6L9EsWZhOkc8xyHguPphh6',
+                 'model_id': 'quickstart',
+                 'model_selection': False,
+                 'model_selection_kwargs': {'base_kernels': 'restricted',
+                                            'depth': 1,
+                                            'evaluation_metric': 'MSLL',
+                                            'val_ratio': 0.2},
+                 'outputs': ['y'],
+                 'train_test_ratio': 0.8}
 
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        emulator_params = emulator.view()
-        print(emulator_params)
-        ```
         """
 
         _, response = api.view_model(self.id, verbose=DEBUG)
         parameters = (
             response  # Note that the whole body of the response is the parameters
         )
         if verbose:
             print("Emulator parameters summary:")
             pprint(parameters, compact=True, sort_dicts=False)
         return parameters
 
     @typechecked
     def view_train_data(self, verbose: bool = False) -> pd.DataFrame:
-        """
-        # View Train Data
-
-        View training data with which the emulator was trained in the `twinLab` cloud.
-
-        ## Arguments:
+        """View training data with which the emulator was trained in the twinLab cloud.
 
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False.
+        Args:
+            verbose (bool, optional): Display information about the operation while running.
 
-        ## Returns:
+        Returns:
+            pandas.DataFrame: Dataframe containing the training data on which the emulator was trained
 
-        - `Pandas.DataFrame` containing the training data on which the emulator was trained.
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.view_train_data()
+
+            .. code-block:: console
+
+                          x         y
+                0  0.696469 -0.817374
+                1  0.286139  0.887656
+                2  0.226851  0.921553
+                3  0.551315 -0.326334
+                4  0.719469 -0.832518
+                5  0.423106  0.400669
+                6  0.980764 -0.164966
+                7  0.684830 -0.960764
 
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        training_dataset = emulator.view_train_data()
-        print(training_dataset)
-        ```
         """
         _, response = api.view_data_model(self.id, dataset_type="train", verbose=DEBUG)
         train_csv_string = utils.get_value_from_body("training_data", response)
         train_csv_string = io.StringIO(train_csv_string)
         df_train = pd.read_csv(train_csv_string, sep=",", index_col=0)
         if verbose:
             print("Training data")
             pprint(df_train)
         return df_train
 
     @typechecked
     def view_test_data(self, verbose: bool = False) -> pd.DataFrame:
-        """
-        # View Test Data
+        """View test data on which the emulator was tested in the twinLab cloud.
 
-        View test data on which the emulator was tested in the `twinLab` cloud.
+        Args:
+            verbose (bool, optional): Display information about the operation while running.
 
-        ## Arguments:
+        Returns:
+            pandas.DataFrame: Dataframe containing the training data on which the emulator was tested
 
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False.
+        Example:
 
-        ## Returns:
+            .. code-block:: python
 
-        - `Pandas.DataFrame` containing the test data on which the emulator was tested.
+                emulator = tl.Emulator("quickstart")
+                emulator.view_test_data()
 
-        ## Example:
+            .. code-block:: console
 
-        ```python
-        import pandas as pd
-        import twinlab as tl
+                          x         y
+                0  0.480932  0.340115
+                1  0.392118  0.845795
 
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        test_dataset = emulator.view_test_data()
-        print(test_dataset)
-        ```
         """
         _, response = api.view_data_model(self.id, dataset_type="test", verbose=DEBUG)
         test_csv_string = utils.get_value_from_body("test_data", response)
         test_csv_string = io.StringIO(test_csv_string)
         df_test = pd.read_csv(test_csv_string, sep=",", index_col=0)
         if verbose:
             print("Test data")
             pprint(df_test)
         return df_test
 
     def list_processes(self, verbose: bool = False) -> Dict[str, Dict]:
-        """
-        # List Processes
-
-        List all processes associated with the emulator on the `twinLab` cloud.
+        """List all of the processes associated with a given emulator on the twinLab cloud.
 
-        ## Arguments:
+        Args:
+            verbose (bool, optional): Determining level of information returned to the user. Default is False.
 
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False. If True, user will see the run time, start time, and status of an emulator.
+        Returns:
+            dict: Dictionary containing all processes associated with the emulator
 
-        ## Returns:
-
-        - `None`
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
+        Example:
+
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.list_processes()
+
+            .. code-block:: console
+
+                [
+                    {
+                        'method': 'sample',
+                        'process_id': '23346a9c',
+                        'run_time': '0:00:05',
+                        'start_time': '2024-04-09 17:10:12',
+                        'status': 'success'
+                    },
+                    {
+                        'method': 'sample',
+                        'process_id': '676623b0',
+                        'run_time': '0:00:04',
+                        'start_time': '2024-04-09 18:45:48',
+                        'status': 'success'
+                    },
+                ]
 
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        emulator.list_processes()
-        ```
         """
         _, response = api.list_processes_model(model_id=self.id, verbose=DEBUG)
         processes = utils.get_value_from_body("processes", response)
 
         # Create dictionary of cuddly response
         status_dict = {
             "success": "Successful processes:",
@@ -520,45 +547,44 @@
                     pprint(procs)
         return processes
 
     @typechecked
     def get_process(
         self, process_id: str, verbose: bool = False
     ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]:
-        """
-        # Get Process
-
-        Get details of a particular process associated with the emulator on the `twinLab` cloud.
-
-        ## Arguments:
-
-        - `process_id`: `str`. The process ID of the process to get details of.
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False.
-
-        ## Returns:
+        """Get the results from a process associated with the emulator on the twinLab cloud.
 
-        - `None`
+        This allows a user to retrieve any results from processes (jobs) they have run previously.
+        The list of available process IDs can be obtained from the ``list_processes()`` method.
 
-        ## Example:
+        Args:
+            process_id (str): The ID of the process from which to get the results.
+            verbose (bool, optional): Display information about the operation while running.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.get_process("23346a9c")
+
+            .. code-block:: console
+
+                            y
+                            0         1         2         3
+                0   -0.730114  0.474193  0.046743  1.327620
+                1   -0.656061  0.505923  0.074198  1.289113
+                2   -0.579500  0.538610  0.100665  1.247405
+                3   -0.502726  0.574996  0.128068  1.205057
+                4   -0.428691  0.614687  0.157740  1.165903
 
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        emulator.recommend(2, 'qEI')
-        emulator.get_process('some_process_id')
-        ```
         """
         _, response = api.list_processes_model(model_id=self.id, verbose=DEBUG)
-        method = response["processes"][process_id]["method"]
+        for i in range(len(response["processes"])):
+            if response["processes"][i]["process_id"] == process_id:
+                method = response["processes"][i]["method"]
         _, response = api.use_response_model(
             model_id=self.id,
             method=method,
             process_id=process_id,
             verbose=DEBUG,
         )
         csv = utils.get_value_from_body("dataframe", response)
@@ -568,42 +594,38 @@
             return df_mean, df_std
         else:
             df = _process_csv(csv, method, verbose=verbose)
             return df
 
     @typechecked
     def summarise(self, verbose: bool = False) -> dict:
-        """
-        # Summarise
+        """Get a summary of a trained emulator on the twinLab cloud.
 
-        Get summary statistics for a pre-trained emulator in the `twinLab` cloud.
+        This summary returns transformer diagnostics, with details about the input/output decomposition.
+        It also returns the estimator diagnostics, detailing properties of the trained emulator.
+        This information can help inform a user about the makeup of an emulator -- for example, what kind of kernel was used.
 
-        ## Arguments:
+        Args:
+            verbose (bool, optional): Display information about the operation while running.
 
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user. Default is False.
+        Example:
+            .. code-block:: python
 
-        ## Returns:
+                emulator = tl.Emulator("quickstart")
+                emulator.summarise()
 
-        - `dict` containing summary statistics for the pre-trained emulator.
+            .. code-block:: console
 
-        ## Example:
+                {
+                    'estimator_diagnostics': ...,
+                    'transformer_diagnostics': ...,
+                }
 
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        info = emulator.summarise()
-        print(info)
-        ```
         """
+        # TODO: Improve the docstring once the summary has been improved
         _, response = api.summarise_model(self.id, verbose=DEBUG)
         summary = utils.get_value_from_body("model_summary", response)
         del summary["data_diagnostics"]
         if verbose:
             print("Trained emulator summary:")
             pprint(summary, compact=True, sort_dicts=False)
         return summary
@@ -630,61 +652,76 @@
             method,
             data_csv=data_csv,
             data_std_csv=data_std_csv,
             **kwargs,
             processor=PROCESSOR,
             verbose=DEBUG,
         )
+
+        # Check if an acq func value exists in the response
+        # If it does then also return it with the dataframe
+        if "acq_func_value" in response.keys():
+            acq_func_value = utils.get_value_from_body("acq_func_value", response)
+            return io.StringIO(output_csv), acq_func_value
         if "dataframe" in response.keys():
             output_csv = utils.get_value_from_body("dataframe", response)
             return io.StringIO(output_csv)
         else:
             output = utils.get_value_from_body("result", response)
             return output
 
     @typechecked
     def score(
         self,
         params: ScoreParams = ScoreParams(),
         verbose: bool = False,
     ) -> Optional[Union[pd.DataFrame, float]]:
-        """
-        # Score
+        """Score the performance of a trained emulator.
+
+        Returns a score for a trained emulator that quantifies its performance on the test dataset.
+        Note that a test dataset must have been defined in order for this to produce a result.
+        This means that ``train_test_ratio`` in TrainParams must be less than ``1`` when training the emulator.
+        If there is no test dataset then this will return ``None``.
+        The score can be calculated using two metrics: the mean-squared error (MSE) or mean-standarised log loss (MSLL).
+        See the ``ScoreParams`` class for a full list and description of available metrics.
+
+        Args:
+            params (ScoreParams, optional): A parameters object that contains optional scoring parameters.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            Either a ``pandas.DataFrame`` containing the emulator per output dimension (if ``combined_score = False``),
+            or a ``float`` containing the combined score of the emulator averaged acorss output dimensions (if ``combined_score = True``),
+            or ``None`` if there was no test data defined during training.
+
+        Examples:
+
+            Request the mean-standarised log loss (MSLL) averaged (combined) across all emulator output dimensions:
+
+            .. code-block:: python
+
+                emulator = tl.Emulator("my_emulator")
+                params = tl.ScoreParams(metric="MSLL", combined_score=True)
+                emulator.score(params=params)
+
+            .. code-block:: console
 
-        Quantify the performance of your trained emulator with an emulator score.
-        Note that a test dataset must have been defined in order for this to produce a meaningful result.
-        This means that `train_test_ratio` must be less than 1 when training your emulator.
-
-        ## Arguments:
-
-        - `params`: `ScoreParams`, `optional`. A `ScoreParams` object that contains all necessary scoring parameters.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ### Returns:
-
-        Either:
-        - `pandas.DataFrame` containing the emulator per output dimension.
-        - `float` containing the combined score of the emulator.
-        - `None` if there is no test data.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        dataset = tl.Dataset("my_dataset")
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        params = tl.TrainParams(train_test_ratio=0.75)
-        emulator.train(dataset, ['X'], ['y'], params)
-        score = emulator.score()
-        print(score)
-        ```
+                -4.07
+
+            Request the mean-squared error (MSE) for each output individually:
+
+            .. code-block:: python
+
+                emulator = tl.Emulator("my_emulator")
+                params = tl.ScoreParams(metric="MSE", combined_score=False)
+                emulator.score(params=params)
+
+            .. code-block:: console
+
+                pd.DataFrame({'y1': [1.8], 'y2': [0.9]})
         """
 
         score = self._use_method(
             method="score",
             **params.unpack_parameters(),
             verbose=verbose,
         )
@@ -693,126 +730,135 @@
         if score is not None:
             if not params.combined_score:  # DataFrame
                 score = pd.read_csv(score, sep=",")
             if verbose:
                 print("Emulator Score:")
                 print(score)  # Could be pd.DataFrame or float
             return score
+        else:
+            print(
+                "No test data was available for this emulator, so it cannot be scored."
+            )
 
     @typechecked
     def benchmark(
         self,
         params: BenchmarkParams = BenchmarkParams(),
         verbose: bool = False,
     ) -> Optional[pd.DataFrame]:
-        """
-        # Benchmark
-
-        Quantify the performance of your trained emulator with a calibration curve.
-        Note that a test dataset must have been defined in order for this to produce a meaningful result.
-        This means that `train_test_ratio` must be less than 1 when training your emulator.
-
-        ## Arguments:
-
-        - `params`: `BenchmarkParams`, `optional`. A `BenchmarkParams` object that contains all parameters for benchmarking the emulators.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ## Returns:
-
-        Either:
-        - `pandas.DataFrame` containing the data for the calibration curve in each dimension.
-        - `None` if there is no test data.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
+        """Benchmark the performance of a trained emulator with a calibration curve.
 
-        emulator = tl.Emulator("emulator_id")
-        params = tl.TrainParams(train_test_ratio=0.75)
-        emulator.train(dataset, ['X'], ['y'], params)
+        A test dataset must have been defined in order for this to produce a meaningful result.
+        This means that ``train_test_ratio`` must be less than 1 when training the emulator.
+        The calibration curve can be plotted to show how well the training data fits to the emulator,
+        and is calculated differently depending on the `params` chosen.
+        The returned dataframe contains 100 rows for each output column of the emulator.
+        These can be plotted to ascertain the performance of the emulator.
+
+        Args:
+            params (BenchmarkParams, optional): A parameter-configuration object that contains optional parameters for benchmarking an emulator.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            pandas.DataFrame, None: Either a ``pandas.DataFrame`` containing the calibration curve for an emulator, or ``None`` if there is no test data.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.benchmark()
+
+            .. code-block:: console
+
+                      y
+                0   0.0
+                1   0.0
+                2   0.0
+                3   0.0
+                4   0.0
+                ..  ...
+                95  1.0
+                96  1.0
+                97  1.0
+                98  1.0
+                99  1.0
 
-        # Plot the calibration curve
-        fraction_observed = emulator.benchmark()
-        fraction_expected = np.linspace(0,1,fraction_observed.shape[0])
-
-        fig, ax = plt.subplots(figsize=(5, 5))
-        ax.set_title("Calibration curve")
-        ax.set_xlabel("Expected coverage")
-        ax.set_ylabel("Observed coverage")
-
-        plt.plot(np.linspace(0, 1, 100), fraction_observed)
-        plt.plot(np.linspace(0, 1, 100), np.linspace(0, 1, 100), "--")
-        plt.show()
-        ```
         """
+        # TODO: This needs to be understood and documented better
 
         csv = self._use_method(
             method="get_calibration_curve",
             **params.unpack_parameters(),
             verbose=verbose,
         )
 
         # Only return the DataFrame if there is test data
         if csv is not None:
             df = pd.read_csv(csv, sep=",")
             if verbose:
                 print("Calibration curve:")
                 pprint(df)
             return df
+        else:
+            print(
+                "No test data was available for this emulator, so it cannot be benchmarked."
+            )
 
     @typechecked
     def predict(
         self,
         df: pd.DataFrame,
         params: PredictParams = PredictParams(),
         wait: bool = True,
         verbose: bool = False,
-    ) -> Union[str, Tuple[pd.DataFrame, pd.DataFrame]]:
-        """
-        # Predict
-
-        Make predictions from a pre-trained emulator that exists on the `twinLab` cloud.
-
-        ## Arguments:
-
-        - `df`: `pandas.DataFrame`. A `pandas.DataFrame` containing the values to make predictions on.
-        - `params`: `PredictParams`. A `PredictParams` object that contains parameters to make predictions.
-        - `wait`: `bool`, `optional`, determining whether to wait for the job to complete, only used if `sync` is `False`
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
+    ) -> Union[Tuple[pd.DataFrame, pd.DataFrame], str]:
+        """Make predictions using a trained emulator that exists on the twinLab cloud.
 
-        **NOTE:** Evaluation data must be a .csv file, or a `pandas.DataFrame` that is interpretable as a .csv file.
+        This method makes predictions from a trained emulator on new data.
+        This method is the workhorse of the twinLab suite, allowing users to make predictions based on their training data.
+        The emulator can make predictions on data that are far away from the training data, and can interpolate reliably between the training data points.
+        The emulator returns both a predicted mean and standard deviation for each output dimension.
+        This allows a user to not only make predictions, but also to quantify the uncertainty on those predictions.
+        For a Gaussian Process, the standard deviation is a measure of the uncertainty in the prediction,
+        while the mean is the prediction itself.
+        The emulator is 95% confident that the true value lies within two standard deviations of the mean.
+
+        Args:
+            df (pandas.DataFrame): The ``X`` values for which to make predictions.
+            params (PredictParams): A parameter-configuration that contains optional parameters for making predictions.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            Tuple[pandas.DataFrame, pandas.DataFrame], str: By default a tuple containing the mean and standard deviation of the emulator prediction.
+            Instead, if ``wait=False``, the process ID is returned.
+            The results can then be retrieved later using ``Emulator.get_process(<process_id>)``.
+            Process IDs associated with an emulator can be found using ``Emulator.list_processes()``.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                df = pd.DataFrame({'x': [0.1, 0.2, 0.3, 0.4]})
+                df_mean, df_std = emulator.predict(df)
+
+            .. code-block:: console
+
+                          y
+                0  0.845942
+                1  0.922921
+                2  0.846308
+                3  0.570473
+
+                          y
+                0  0.404200
+                1  0.180853
+                2  0.146619
+                3  0.147886
 
-        ## Returns:
-
-        - `tuple` containing:
-            - `df_mean`: `pandas.DataFrame` containing mean predictions.
-            - `df_std`: `pandas.DataFrame` containing standard deviation predictions.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        df_test = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-        df_mean, df_std = emulator.predict(df_test)
-        print(df_mean)
-        print(df_std)
-        ```
         """
         API_METHOD = "predict"
         if SYNC:
             csv = self._use_method(
                 method=API_METHOD,
                 df=df,
                 **params.unpack_parameters(),
@@ -844,55 +890,57 @@
     def sample(
         self,
         df: pd.DataFrame,
         num_samples: int,
         params: SampleParams = SampleParams(),
         wait: bool = True,
         verbose: bool = False,
-    ) -> Union[str, pd.DataFrame]:
-        """
-        # Sample
-
-        Draw samples from a pre-trained emulator that exists on the `twinLab` cloud.
-
-        ## Arguments:
-
-        - `df` : `pandas.DataFrame`. A `pandas.DataFrame` containing the values to sample from.
-        - `num_samples`: `int`. Number of samples to draw for each row of the evaluation data.
-        - `params`: `SampleParams`, `optional`. A `SampleParams` object with sampling parameters.
-        - `wait`: `bool`, `optional`. If true, wait for the job to complete, otherwise return the process ID and exit.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        **NOTE:** Evaluation data must be a .csv file, or a `pandas.DataFrame` that is interpretable as a .csv file.
+    ) -> Union[pd.DataFrame, str]:
+        """Draw samples from a trained emulator that exists on the twinLab cloud.
 
-        ## Returns:
+        A secondary functionality of the emulator is to draw sample predictions from the trained emulator.
+        Rather than quantifying the uncertainty in the predictions, this method draws samples from the emulator.
+        The collection of samples can be used to explore the distribution of the emulator predictions.
+        Each sample is a possible prediction of the emulator, and therefore a prediction of a possible new observation from the data-generation process.
+        The covariance in the emulator predictions can therefore be explored, which is particularly useful for functional Gaussian Processes.
+
+        If the output of the multi-indexed DataFrame needs to be manipulated then we provide the convenience functions:
+
+            - ``tl.get_sample``: Isolate an individual sample into a new ``pandas.DataFrame``
+            - ``tl.join_samples``: Join together multiple sets of samples into a single ``pandas.DataFrame``
+
+        Args:
+            df (pandas.DataFrame): The ``X`` values for which to draw samples.
+            num_samples (int): Number of samples to draw for each row of the evaluation data.
+            params (SampleParams, optional): A `SampleParams` object with sampling parameters.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            pandas.DataFrame, str: By default a multi-indexed DataFrame containing the ``y`` samples drawn from the emulator.
+            Instead, if ``wait=False`` the process ID is returned.
+            The results can then be retrieved later using ``Emulator.get_process(<process_id>)``.
+            Process IDs associated with an emulator can be found using ``Emulator.list_processes()``.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                df = pd.DataFrame({'x': [0.1, 0.2, 0.3, 0.4]})
+                emulator.sample(df, 3)
+
+            .. code-block:: console
+
+                          y
+                          0         1         2
+                0  0.490081  1.336099  0.608441
+                1  0.829179  1.038671  0.807405
+                2  0.805102  0.773975  0.984713
+                3  0.605568  0.416630  0.713652
 
-        - `pandas.DataFrame` with the sampled values.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-
-        df = pd.DataFrame({'X': [1.5, 2.5, 3.5]})
-        n = 10
-        df_samples = emulator.sample(df, n)
-        print(df_samples)
-
-        df_single_sample = tl.get_sample(df_samples, 0) # Accessing Sample 1
-        print(df_single_sample)
-        ```
         """
         API_METHOD = "sample"
         if SYNC:
             csv = self._use_method(
                 method=API_METHOD,
                 df=df,
                 num_samples=num_samples,
@@ -926,60 +974,109 @@
     def recommend(
         self,
         num_points: int,
         acq_func: str,
         params: RecommendParams = RecommendParams(),
         wait: bool = True,
         verbose: bool = False,
-    ) -> Union[str, pd.DataFrame]:
-        """
-        # Recommend
+    ) -> Union[Tuple[pd.DataFrame, float], str]:
+        """Draw new recommended data points from a trained emulator that exists on the twinLab cloud.
+
+        The recommend functionality of an emulator is used to suggest new data points to sample.
+        These new data points can be chosen depending on a variety of different user objectives.
+        Currently, the user can choose between ``"optimise"`` and ``"explore"`` acquisition functions.
+        Choosing ``"optimise"`` will obtain suggested ``"X"`` values the evaluation of which (acquiring the corresponding ``"y"``) will maximise the knowledge of the emulator about the location of the maximum.
+        A classic use case for this would be a user trying to maximise the output of a model.
+        For example, the maximum strenth of a pipe given a set of design parameters.
+        Choosing ``"explore"`` will instead suggest ``"X"`` that reduce the overall uncertainty of the emulator across the entire input space.
+        A classic use case for this would be a user trying to reduce overally uncertainty.
+        For example, a user trying to reduce the uncertainty in the strength of a pipe across all design parameters.
+        The number of requested data points can be specified by the user, and if this is greater than one then then recommendations are all suggested at once, and are designed to be the optmial set, as a group, to achieve the user outcome.
+        twinLab optimises which specific acquisition function within the chosen category will be used, prioritising numerical stability based on the number of points requested.
+
+        The value of the acquisition function is also returned to the user.
+        While this is of limited value in isolation, the trend of the acquisition function value over multiple iterations of ``Recommend`` can be used to understand the performance of the emulator.
+        The ``Emualtor.learn`` method can be used to improve the performance of an emulator iteratively.
+
+        Args:
+            num_points (int): The number of samples to draw for each row of the evaluation data.
+            acq_func (str): Specifies the acquisition function to be used when recommending new points.
+                The acquisition function can be either ``"explore"`` or ``"optimise"``.
+            params (RecommendParams, optional): A parameter configuration that contains all of the optional recommendation parameters.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            Tuple[pandas.DataFrame, float], str: By default, a tuple is returned containing the recommended samples and the acquisition function value.
+            Instead, if ``wait=False``, the process ID is returned.
+            The results can then be retrieved later using ``Emulator.get_process(<process_id>)``.
+            Process IDs associated with an emulator can be found using ``Emulator.list_processes()``.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.recommend(5, "explore")
+
+            .. code-block:: console
+
+                          x
+                0  0.852853
+                1  0.914091
+                2  0.804012
+                3  0.353463
+                4  0.595268
+
+                -0.00553509
+
+        Example:
+
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                emulator.recommend(3, "optimisation")
+
+            .. code-block:: console
+
+                          x
+                0  0.273920
+                1  0.306423
+                2  0.226851
 
-        Draw new candidate data points via active learning from a pre-trained emulator
-        that exists on the `twinLab` cloud.
+                0.046944751
 
-        ## Arguments:
-        - `num_points`: `int`. Number of samples to draw for each row of the evaluation data.
-        - `acq_func`: `str`. Specifies the acquisition function to be used when recommending new points; this can be chose from a list of possible fucntions:
-        `"ExpectedImprovement"`, `"qExpectedImprovement"`, `"LogExpectedImprovement"`, `"qLogExpectedImprovement"`, `"PosteriorStandardDeviation"`, `"qNegIntegratedPosteriorVariance"`.
-        - `params`: `RecommendParams`, `optional`. A `RecommendParams` object that contains all recommendation parameters.
-        - `wait`: `bool`, `optional`. If true, wait for the job to complete, otherwise return the process ID and exit.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ## Returns:
-
-        - `pandas.DataFrame` containing the recommended sample locations.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        n = 10
-        df = emulator.recommend(n, 'qEI')
-        print(df)
-        ```
         """
         API_METHOD = "get_candidate_points"
+
+        # Convert acq_func names to correct method depending on number of points requested
+        if acq_func == "optimise":
+            if num_points == 1:
+                acq_func = "EI"
+            else:
+                acq_func = "qEI"
+        if acq_func == "explore":
+            acq_func = "qNIPV"
+
         if SYNC:
-            csv = self._use_method(
-                model_id=self.id,
+            csv, acq_func_value = self._use_method(
                 method=API_METHOD,
                 num_points=num_points,
                 acq_func=ACQ_FUNC_DICT[acq_func],
                 **params.unpack_parameters(),
                 verbose=verbose,
             )
+
+            df = _process_csv(csv, API_METHOD, verbose=verbose)
+
+            if verbose:
+                print("Recommended samples:")
+                print(df)
+
+            return df, acq_func_value
+
         else:
             _, response = api.use_request_model(
                 model_id=self.id,
                 method=API_METHOD,
                 num_points=num_points,
                 acq_func=ACQ_FUNC_DICT[acq_func],
                 **params.unpack_parameters(),
@@ -991,60 +1088,73 @@
                 print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
             if not wait:
                 return process_id
             _, response = _wait_for_job_completion(
                 self.id, API_METHOD, process_id, verbose=verbose
             )
             csv = utils.get_value_from_body("dataframe", response)
+            acq_func_value = float(
+                utils.get_value_from_body("acq_func_value", response)
+            )
             csv = io.StringIO(csv)
-        df = _process_csv(csv, API_METHOD, verbose=verbose)
-        return df
+
+            df = _process_csv(csv, API_METHOD, verbose=verbose)
+
+            if verbose:
+                print("Recommended samples:")
+                print(df)
+                print("Acquisition function value:")
+                print(acq_func_value)
+
+            return df, acq_func_value
 
     @typechecked
     def calibrate(
         self,
         df_obs: pd.DataFrame,
         df_std: pd.DataFrame,
         params: CalibrateParams = CalibrateParams(),
         wait: bool = True,
         verbose: bool = False,
-    ) -> Union[str, pd.DataFrame]:
-        """
-        # Calibrate
+    ) -> Union[pd.DataFrame, str]:
+        """Solve an inverse problem using a trained emulator on the twinLab cloud.
+
+        A classic trained emulator can ingest ``X`` values and use these to predict corresponding ``y`` values.
+        However, the emulator can also be used to solve an inverse problem, where the user has an observation of ``y`` and wants to find the corresponding ``X``.
+        Problems of this type are common in engineering and science, where the user has an observation of a system and wants to find the parameters that generated that observation.
+        This operation can be numerically intensive, and the emulator can be used to solve this problem quickly and efficiently.
+
+        Args:
+            df_obs (pandas.DataFrame): A dataframe containing the single observation.
+            df_std (pandas.DataFrame): A dataframe containing the error on the single observation.
+            params (CalibrateParams, optional): A parameter configuration that contains all optional calibration parameters.
+            wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            pandas.DataFrame, str: By default, the solution to the inverse problem is either presented as a summary,
+            or as the full set of points sampled from the posterior distribution.
+            See the documentation for ``CalibrateParams`` for more information on the different options.
+            Instead, if ``wait=False``, the process ID is returned.
+            The results can then be retrieved later using ``Emulator.get_process(<process_id>)``.
+            Process IDs associated with an emulator can be found using ``Emulator.list_processes()``.
+
+        Example:
+            .. code-block:: python
+
+                emulator = tl.Emulator("quickstart")
+                df_obs = pd.DataFrame({'y': [0.1]})
+                df_std = pd.DataFrame({'y': [0.01]})
+                emulator.calibrate(df_obs, df_std)
 
-        Given a set of observations, inverse modelling finds the model that would best suit the data.
+            .. code-block:: console
 
-        ## Arguments:
+                    mean     sd  hdi_3%  hdi_97%  mcse_mean  mcse_sd  ess_bulk  ess_tail  r_hat
+                x  0.496  0.013   0.471    0.521        0.0      0.0    2025.0    2538.0    1.0
 
-        - `df_obs` : `pandas.DataFrame`. A `pandas.DataFrame` containing the observations.
-        - `df_std` : `pandas.DataFrame`. A `pandas.DataFrame` containing the error on the observations.
-        - `params`: `CalibrateParams`, `optional`. A `CalibrateParams` object that contains all calibration parameters.
-        - `wait`: `bool`, `optional`. If true, wait for the job to complete, otherwise return the process ID and exit.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ## Returns:
-
-        - `pandas.DataFrame` containing the recommended model statistics.
-
-        ## Example:
-
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-        data_csv = pd.DataFrame({'y': [1]})
-        data_std_csv = pd.DataFrame({'y': [0.498]})
-        df = emulator.calibrate(data_csv, data_std_csv)
-        print(df)
-        ```
         """
         API_METHOD = "solve_inverse"
         if SYNC:
             csv = self._use_method(
                 method=API_METHOD,
                 df=df_obs,
                 df_std=df_std,
@@ -1085,80 +1195,50 @@
         num_points_per_loop: int,
         acq_func: str,
         simulation: Callable,  # A function that ingests X and returns y
         train_params: TrainParams = TrainParams(),
         recommend_params: RecommendParams = RecommendParams(),
         verbose: bool = False,
     ) -> None:
-        """
-        # Learn
-
-        Perform learning to train an emulator on the `twinLab` cloud in a loop to demonstrate active learning and optimisation routines.
+        """Perform active learning to improve an emulator on the twinLab cloud.
 
-        ## Arguments:
-        - `dataset`: `Dataset`. twinLab dataset object which contains the training data for the emulator.
-        - `inputs`: `list[str]`. List of input names in the training dataset.
-        - `outputs`; `list[str]`. List of output names in the training dataset.
-        - `num_loops`: `int`. Number of loops to run the learning process.
-        - `num_points_per_loop`: `int`. Number of points to sample in each loop.
-        - `acq_func`: `str`. Specifies the acquisition function to be used when recommending new points; this can be chose from a list of possible fucntions:
-            `"ExpectedImprovement"`, `"qExpectedImprovement"`, `"LogExpectedImprovement"`, `"qLogExpectedImprovement"`, `"PosteriorStandardDeviation"`, `"qNegIntegratedPosteriorVariance"`.
-        - `simulation`: `Callable`. A function that takes in a set of inputs and generates the outputs(a simulator for the data generating process).
-        - `train_params`: `TrainParams`, `optional`. A `TrainParams` object that contains all necessary training parameters.
-        - `recommend_params`: `RecommendParams`, `optional`. A `RecommendParams` object that contains all recommendation parameters.
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
-
-        ## Example:
-
-            ```python
-            import pandas as pd
-            import numpy as np
-
-            import twinlab as tl
-
-            grid = np.linspace(0, 1)
-
-            # Defining the simulation function
-            def model(x):
-                return (x[0] * grid - 2) ** 2 * np.sin(x[1] * grid - 4)
-
-            def generate_output(x):
-                y = np.zeros((x.shape[0], grid.size))
-                for i, x_i in enumerate(x):
-                    y[i, :] = model(x_i)
-                return y
-
-            emulator_id = "my_emulator"
-            dataset_id = "my_dataset"
-            input_columns = ["x1", "x2"]
-            output_columns = ["y_{}".format(i) for i in range(grid.size)]
-
-            # Create emulator
-            emulator = tl.Emulator(id=emulator_id)
-            training_dataset = tl.Dataset(dataset_id)
-            training_dataset.upload(df)
-
-            params = tl.TrainParams(
-                train_test_ratio=0.75,
-                estimator="gaussian_process_regression",
-                output_explained_variance=0.99999,
-            )
+        Active learning is a method that can identify and utilise the most informative data points to add to an emulator in order to reduce the number of measurements to be taken or simulations that are required.
+        Using active learning can result in a more accurate model, trained with less data.
+        The primary difference between this method and ``Emulator.recommend`` is that in this method the emulator is trained on the new data points that are suggested in an active loop.
+        This way, new data can be used to update an emulator until the desired level of accuracy is achieved.
+        This can be done using either the ``"optmise"`` or ``"explore"`` acquisition functions.
+        The emulator can therefore be updated with the objective of either finding the point of maximum output or reducing the overall uncertainty in the emulator.
+
+        Args:
+            dataset (Dataset): twinLab dataset object which contains the initial training data for the emulator.
+            inputs (list[str]): List of input column names in the training dataset.
+            outputs (list[str]): List of output column names in the training dataset.
+            num_loops (int): Number of loops to run the learning process.
+            num_points_per_loop (int): Number of points to sample in each loop.
+            acq_func (str): Specifies the acquisition function to be used when recommending new points: either ``"explore"`` or ``"optimise"``.
+            simulation (Callable): A function that takes in a set of inputs and generates the outputs (for example, a simulator for the data generating process).
+            train_params (TrainParams, optional): A parameter configuration that contains optional training parameters.
+            recommend_params (RecommendParams, optional): A parameter configuration that contains optional recommendation parameters.
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Examples:
+            .. code-block:: python
+
+                emulator = tl.Emulator(id=emulator_id)
+                dataset = tl.Dataset(dataset_id)
+                emulator.learn(
+                    dataset=dataset,
+                    inputs=["X"],
+                    outputs=["y"],
+                    num_loops=3,
+                    num_points_per_loop=5,
+                    acq_func="explore",
+                    simulation=my_simulator,
+                )
 
-            # Call the learn function
-            emulator.learn(
-                dataset=training_dataset,
-                inputs=input_columns,
-                outputs=output_columns,
-                num_loops=1,
-                num_points_per_loop=1,
-                acq_func="EI",
-                simulation=generate_output,
-                train_params=params,
-            )
-            ```
         """
 
         # Loop over iterations of learning
         for i in range(num_loops):
 
             # Train model
             self.train(
@@ -1169,15 +1249,15 @@
                 verbose=verbose,
             )
 
             # Get recommendations on all but final iteration
             if i < num_loops - 1:
 
                 # Compute optimal sample location(s)
-                candidate_points = self.recommend(
+                candidate_points, _ = self.recommend(
                     num_points=num_points_per_loop,
                     acq_func=acq_func,
                     params=recommend_params,
                     verbose=verbose,
                 )
                 print(f"Iteration: {i}")
                 print("Suggested candidate point(s):")
@@ -1192,37 +1272,27 @@
                 # Download current training data, append new data, and reupload
                 df_train = self.view_train_data()
                 df_train = pd.concat([df_train, candidate_points], ignore_index=True)
                 dataset.upload(df_train)
 
     @typechecked
     def delete(self, verbose: bool = False) -> None:
-        """
-        # Delete
+        """Delete emulator from the twinLab cloud.
 
-        Delete emulator from the `twinLab` cloud.
+        It can be useful to delete an emulator to keep a cloud account tidy, or if an emulator is no longer necessary.
 
-        ## Arguments:
+        Args:
+            verbose (bool, optional): Display detailed information about the operation while running.
 
-        - `verbose`: `bool`, `optional`. Determining level of information returned to the user.
+        Examples:
+            .. code-block:: python
 
-        ## Example:
+                emulator = tl.Emulator("quickstart")
+                emulator.delete()
 
-        ```python
-        import pandas as pd
-        import twinlab as tl
-
-        df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-        dataset = tl.Dataset("my_dataset")
-        dataset.upload(df)
-        emulator = tl.Emulator("emulator_id")
-        emulator.train(dataset, ['X'], ['y'])
-
-        emulator.delete()
-        ```
         """
         _, response = api.delete_model(self.id, verbose=DEBUG)
         if verbose:
             message = utils.get_message(response)
             print(message)
 
     @typechecked
@@ -1233,46 +1303,43 @@
         x_fixed: Dict[str, float] = {},
         params: PredictParams = PredictParams(),
         x_lim: Optional[Tuple[float, float]] = None,
         n_points: int = 100,
         label: str = "Emulator",
         color: str = digilab_colors["light_blue"],
         verbose: bool = False,
-    ) -> plt:
-        """
-        # Plot
+    ) -> plt.plot:
+        """Plot the predictions from an emulator across a single dimension with one and two standard deviation bands.
 
-        Plot the predictions from an emulator across a single dimension with one and two standard deviation bands.
         This will make a call to the emulator to predict across the specified dimension.
         Note that a multi-dimensional emulator will be sliced across the other dimensions.
         The matplotlib.pyplot object is returned, and can be further modified by the user.
 
-        ## Arguments:
-        - `x_axis`: `str`. The name of the x-axis variable.
-        - `y_axis`: `str`. The name of the y-axis variable.
-        - `x_fixed`: `dict`, `Optional`. A dictionary of fixed values for the other X variables. Note that all X variables of your emulator must either be specified as x_axis or appear as x_fixed keys. To pass through "None", either leave x_fixed out or pass through an empty dictionary.
-        - `params`: `PredictParams`, `Optional`. A `PredictParams` object that contains all necessary prediction parameters.
-        - `x_lim`: `Tuple[float, float]`, `Optional`. The limits of the x-axis. If not provided, the limits will be taken directly from the emulator.
-        - `n_points`: `int`, `Optional`. The number of points to predict across the x-axis. Default is 100.
-        - `label`: `str`. The label for the line in the plot, defaults to "Emulator prediction".
-        - `color`: `str`. The color of the plot, defaults to digiLab blue. Can be any valid matplotlib color (https://matplotlib.org/stable/gallery/color/named_colors.html)
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False.
-
-        ## Returns:
-        - `matplotlib.pyplot` object
-
-        ## Example:
-
-        ```python
-        import twinlab as tl
-
-        emulator = tl.Emulator("emulator_id") # A pre-trained emulator
-        plt = emulator.plot("Time", "Temperature", x_fixed={"Latitude": 0, "Longitude": 30})
-        plt.show()
-        ```
+        Args:
+            x_axis (str): The name of the x-axis variable.
+            y_axis (str): The name of the y-axis variable.
+            x_fixed (dict, optional): A dictionary of fixed values for the other X variables.
+                Note that all X variables of an emulator must either be specified as x_axis or appear as x_fixed keys.
+                To pass through "None". either leave x_fixed out or pass through an empty dictionary.
+            params: (PredictParams, optional). A parameter configuration that contains optional prediction parameters.
+            x_lim (tuple[float, float], optional]: The limits of the x-axis.
+                If not provided. the limits will be taken directly from the emulator.
+            n_points (int, optional): The number of points to sample in the x-axis.
+            label (str, optional): The label for the line in the plot. defaults to "Emulator prediction".
+            color (str, optional): The color of the plot. Defaults to digiLab blue.
+                Can be any valid matplotlib color (https://matplotlib.org/stable/gallery/color/named_colors.html).
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Examples:
+            .. code-block:: python
+
+                emulator = tl.Emulator("emulator_id")
+                plt = emulator.plot("Time", "Temperature", x_fixed={"Latitude": 0, "Longitude": 30})
+                plt.show()
+
         """
 
         # Get information about inputs/outputs from the emulator
         _, response = api.summarise_model(self.id, verbose=DEBUG)
         inputs = set(response["model_summary"]["data_diagnostics"]["inputs"].keys())
         outputs = set(response["model_summary"]["data_diagnostics"]["outputs"].keys())
 
@@ -1319,48 +1386,50 @@
         x_fixed: Dict[str, float] = {},
         params: PredictParams = PredictParams(),
         x1_lim: Optional[Tuple[float, float]] = None,
         x2_lim: Optional[Tuple[float, float]] = None,
         n_points: int = 25,
         cmap=digilab_cmap,
         verbose: bool = False,
-    ) -> plt:
-        """
-        # Heatmap
+    ) -> plt.plot:
+        """Plot a heatmap of the predictions from an emulator across two dimensions.
 
-        Plot a heatmap of the predictions from an emulator across two dimensions.
-        The uncertainty of the emulator is not plotted here.
         This will make a call to the emulator to predict across the specified dimensions.
         Note that a higher-than-two-dimensional emulator will be sliced across the other dimensions.
         The matplotlib.pyplot object is returned, and can be further modified by the user.
+        The uncertainty of the emulator is not plotted here.
+
+        Args:
+            x1_axis (str): The name of the x1-axis variable (horizonal axis).
+            x2_axis (str): The name of the x2-axis variable (vertical axis).
+            y_axis (str): The name of the plotted variable (heatmap).
+            x_fixed (dict, optional): A dictionary of fixed values for the other ``X`` variables.
+                Note that all ``X`` variables of an emulator must either be specified as ``x1_axis``, ``x2_axis`` or appear as keys in ``x_fixed``.
+                Passing an empty dictionary (the default) will fix none of the variables.
+            params: (PredictParams, optional). A parameter configuration that contains optional prediction parameters.
+            x1_lim (tuple[float, float], optional): The limits of the x1-axis.
+                If not provided. the limits will be taken directly from the emulator.
+            x2_lim (tuple[float, float], optional): The limits of the x2-axis.
+                If not provided. the limits will be taken directly from the emulator.
+            n_points (int, optional): The number of points to sample in each dimension.
+                The default is 25, which will create a 25x25 grid.
+            cmap (str, optional): The color of the plot. Defaults to a digiLab palette.
+                Can be any valid matplotlib color (https://matplotlib.org/stable/users/explain/colors/colormaps.html).
+            verbose (bool, optional): Display detailed information about the operation while running.
+
+        Returns:
+            matplotlib.pyplot: Matplotlib plot object
+
+        Examples:
+            .. code-block:: python
+
+                emulator = tl.Emulator("emulator_id") # A trained emulator
+                plt = emulator.heatmap("Latitude", "Longitude", "Rainfall", x_fixed={"Month": 6})
+                plt.show()
 
-        ## Arguments:
-        - `x1_axis`: `str`. The name of the x1-axis variable (horizonal axis).
-        - `x2_axis`: `str`. The name of the x2-axis variable (vertical axis).
-        - `y_axis`: `str`. The name of the plotted variable (heatmap).
-        - `x_fixed`: `dict`, `Optional`. A dictionary of fixed values for the other X variables. Note that all X variables of your emulator must either be specified as x1_axis, x2_axis, or appear as x_fixed keys. To pass through "None", either leave x_fixed out or pass through an empty dictionary.
-        - `params`: `PredictParams`, `Optional`. A `PredictParams` object that contains all necessary prediction parameters.
-        - `x1_lim`: `Tuple[float, float]`, `Optional`. The limits of the x1-axis. If not provided, the limits will be taken directly from the emulator.
-        - `x2_lim`: `Tuple[float, float]`, `Optional`. The limits of the x2-axis. If not provided, the limits will be taken directly from the emulator.
-        - `n_points`: `int`, `Optional`. The number of points to predict across each axis. Default is 25.
-        - `cmap`: `str`. The color of the plot, defaults to digiLab palette. Can be any valid matplotlib color (https://matplotlib.org/stable/users/explain/colors/colormaps.html).
-        - `verbose`: `bool`, `Optional`. Determining level of information returned to the user. Default is False.
-
-        ## Returns:
-        - `matplotlib.pyplot` object
-
-        ## Example:
-
-        ```python
-        import twinlab as tl
-
-        emulator = tl.Emulator("emulator_id") # A pre-trained emulator
-        plt = emulator.heatmap("Latitude", "Longitude", "Rainfall", x_fixed={"Month": 6})
-        plt.show()
-        ```
         """
 
         # Get information about inputs/outputs from the emulator
         _, response = api.summarise_model(self.id, verbose=DEBUG)
         inputs = set(response["model_summary"]["data_diagnostics"]["inputs"].keys())
         outputs = set(response["model_summary"]["data_diagnostics"]["outputs"].keys())
```

### Comparing `twinlab-2.4.0/twinlab/plotting.py` & `twinlab-2.5.0/twinlab/plotting.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.4.0/twinlab/settings.py` & `twinlab-2.5.0/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.4.0/twinlab/utils.py` & `twinlab-2.5.0/twinlab/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,49 +21,50 @@
         message = response
     return message
 
 
 @typechecked
 def get_value_from_body(key: str, body: dict):
     """
-    # API error messaging
 
     Relay responses from api.py directly.
+
     This improves error messaging.
+
     """
     if key in body.keys():
         return body[f"{key}"]
     else:
         print(body)
         raise KeyError(f"{key} not in API response body")
 
 
 @typechecked
 def coerce_params_dict(params: dict) -> dict:
     """
-    # Parameter dictionary relabeling
 
     Relabel parameters to be consistent with twinLab library.
+
     """
     if "train_test_split" in params.keys() or "test_train_split" in params.keys():
         raise TypeError("train_test_split is deprecated. Use train_test_ratio instead.")
     for param in settings.PARAMS_COERCION:
         if param in params:
             params[settings.PARAMS_COERCION[param]] = params.pop(param)
     if "train_test_ratio" not in params.keys():
         params["train_test_ratio"] = 1.0
     return params
 
 
 @typechecked
 def check_dataset(string: str) -> None:
     """
-    # Check datasets
 
     Check that a sensible dataframe can be created from a .csv file string.
+
     """
 
     # check for duplicate columns # TODO this assumes label is row 0
     header = pd.read_csv(io.StringIO(string), header=None, nrows=1).iloc[0].to_list()
     if len(set(header)) != len(header):
         raise TypeError("Dataset must contain no duplicate column names.")
 
@@ -93,24 +94,23 @@
 def upload_dataframe_to_presigned_url(
     df: pd.DataFrame,
     url: str,
     verbose: bool = False,
     check: bool = False,
 ) -> None:
     """
-    # Upload DataFrame to URL
 
     Upload a `pandas.DataFrame` to the specified pre-signed URL.
 
-    ## Arguments:
+    Args:
+        df (pandas.DataFrame): The `pandas.DataFrame` to upload
+        url (str): The pre-signed URL generated for uploading the file.
+        verbose (bool): defaults to `False`.
+        check (bool): defaults to `False`. Check the dataset before uploading.
 
-    - df: `pandas.DataFrame`. The `pandas.DataFrame` to upload
-    - url: `str`. The pre-signed URL generated for uploading the file.
-    - verbose: `bool`, defaults to `False`.
-    - check: `bool`, defaults to `False`. Check the dataset before uploading.
     """
     if check:
         csv_string = df.to_csv(index=False)
         check_dataset(csv_string)
     headers = {"Content-Type": "application/octet-stream"}
     buffer = io.BytesIO()
     df.to_csv(buffer, index=False)
@@ -129,24 +129,23 @@
 def upload_file_to_presigned_url(
     file_path: str,
     url: str,
     verbose: bool = False,
     check: bool = False,
 ) -> None:
     """
-    # Upload files to URL
 
     Upload a file to the specified pre-signed URL.
 
-    ## Arguments:
+    Args:
+        file_path (str): The path to the local file a user wants to upload.
+        presigned_url (str): The pre-signed URL generated for uploading the file.
+        verbose (bool): defaults to `False`.
+        check (bool): defaults to `False`. Check the dataset before uploading.
 
-    - file_path: `str`. The path to the local file you want to upload.
-    - presigned_url: `str`. The pre-signed URL generated for uploading the file.
-    - verbose: `bool`, defaults to `False`.
-    - check: `bool`, defaults to `False`. Check the dataset before uploading.
     """
     if check:
         with open(file_path, "rb") as file:
             csv_string = file.read().decode("utf-8")
             check_dataset(csv_string)
     with open(file_path, "rb") as file:
         headers = {"Content-Type": "application/octet-stream"}
@@ -161,7 +160,19 @@
 
 
 @typechecked
 def get_csv_string(df: pd.DataFrame) -> str:
     buffer = io.StringIO()
     df.to_csv(buffer, index=False)
     return buffer.getvalue()
+
+
+@typechecked
+def remove_none_values(d: dict) -> dict:
+    """
+    Function to remove None values from a nested dictionary.
+    """
+    return {
+        k: remove_none_values(v) if isinstance(v, dict) else v
+        for k, v in d.items()
+        if v is not None
+    }
```

### Comparing `twinlab-2.4.0/PKG-INFO` & `twinlab-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python interface for twinLab machine-learning in the cloud.
 Home-page: https://www.digilab.co.uk
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: digiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
 Maintainer-email: alexander@digilab.co.uk
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: matplotlib (>=3.7)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (>=1.24,<2.0) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: numpy (>=1.26,<2.0) ; python_version >= "3.9" and python_version < "3.13"
+Requires-Dist: pandas (>=1.5.3,<2.0.0) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: pandas (>=2.0,<3.0) ; python_version >= "3.9" and python_version < "3.13"
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: setuptools (>=69.0.2,<70.0.0)
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://digilab-ai.github.io/twinLab
 Project-URL: Repository, https://github.com/digiLab-ai/twinLab-client
```

