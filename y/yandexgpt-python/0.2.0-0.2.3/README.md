# Comparing `tmp/yandexgpt-python-0.2.0.tar.gz` & `tmp/yandexgpt-python-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandexgpt-python-0.2.0.tar", last modified: Fri Apr 12 17:51:11 2024, max compression
+gzip compressed data, was "yandexgpt-python-0.2.3.tar", last modified: Mon Apr 15 07:25:34 2024, max compression
```

## Comparing `yandexgpt-python-0.2.0.tar` & `yandexgpt-python-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-12 17:51:11.165915 yandexgpt-python-0.2.0/
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     1067 2024-04-11 13:49:09.000000 yandexgpt-python-0.2.0/LICENSE
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     4822 2024-04-12 17:51:11.165915 yandexgpt-python-0.2.0/PKG-INFO
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     4225 2024-04-12 17:22:53.000000 yandexgpt-python-0.2.0/README.md
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       38 2024-04-12 17:51:11.165915 yandexgpt-python-0.2.0/setup.cfg
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)      745 2024-04-12 17:30:28.000000 yandexgpt-python-0.2.0/setup.py
-drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-12 17:51:11.159249 yandexgpt-python-0.2.0/yandex_gpt/
--rw-rw-r--   0 gregory1m  (1000) gregory1m  (1000)      473 2024-04-12 13:11:25.000000 yandexgpt-python-0.2.0/yandex_gpt/__init__.py
--rw-rw-r--   0 gregory1m  (1000) gregory1m  (1000)    15603 2024-04-12 17:25:58.000000 yandexgpt-python-0.2.0/yandex_gpt/config_manager.py
--rw-rw-r--   0 gregory1m  (1000) gregory1m  (1000)     6489 2024-04-12 06:45:19.000000 yandexgpt-python-0.2.0/yandex_gpt/yandex_gpt.py
-drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-12 17:51:11.162582 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     4822 2024-04-12 17:51:11.000000 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/PKG-INFO
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)      302 2024-04-12 17:51:11.000000 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/SOURCES.txt
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)        1 2024-04-12 17:51:11.000000 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/dependency_links.txt
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       66 2024-04-12 17:51:11.000000 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/requires.txt
--rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       11 2024-04-12 17:51:11.000000 yandexgpt-python-0.2.0/yandexgpt_python.egg-info/top_level.txt
+drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-15 07:25:34.650514 yandexgpt-python-0.2.3/
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     1067 2024-04-11 13:49:09.000000 yandexgpt-python-0.2.3/LICENSE
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     5068 2024-04-15 07:25:34.650514 yandexgpt-python-0.2.3/PKG-INFO
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     4479 2024-04-15 07:11:09.000000 yandexgpt-python-0.2.3/README.md
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       38 2024-04-15 07:25:34.650514 yandexgpt-python-0.2.3/setup.cfg
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)      737 2024-04-15 07:17:49.000000 yandexgpt-python-0.2.3/setup.py
+drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-15 07:25:34.650514 yandexgpt-python-0.2.3/yandex_gpt/
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)      532 2024-04-13 05:22:12.000000 yandexgpt-python-0.2.3/yandex_gpt/__init__.py
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)    18151 2024-04-13 14:07:29.000000 yandexgpt-python-0.2.3/yandex_gpt/config_manager.py
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     6258 2024-04-13 18:47:16.000000 yandexgpt-python-0.2.3/yandex_gpt/thread.py
+-rw-rw-r--   0 gregory1m  (1000) gregory1m  (1000)    13535 2024-04-13 21:44:15.000000 yandexgpt-python-0.2.3/yandex_gpt/yandex_gpt.py
+drwxr-xr-x   0 gregory1m  (1000) gregory1m  (1000)        0 2024-04-15 07:25:34.650514 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)     5068 2024-04-15 07:25:34.000000 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/PKG-INFO
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)      323 2024-04-15 07:25:34.000000 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/SOURCES.txt
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)        1 2024-04-15 07:25:34.000000 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/dependency_links.txt
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       66 2024-04-15 07:25:34.000000 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/requires.txt
+-rw-r--r--   0 gregory1m  (1000) gregory1m  (1000)       11 2024-04-15 07:25:34.000000 yandexgpt-python-0.2.3/yandexgpt_python.egg-info/top_level.txt
```

### Comparing `yandexgpt-python-0.2.0/LICENSE` & `yandexgpt-python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yandexgpt-python-0.2.0/PKG-INFO` & `yandexgpt-python-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-Metadata-Version: 2.1
-Name: yandexgpt-python
-Version: 0.2.0
-Summary: A Python SDK for interacting with the YandexGPT API.
-Home-page: https://github.com/allseeteam/yandexgpt-python
-Author: Gregory Matsnev
-Author-email: grigorij1m@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.9.3
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: PyJWT==2.8.0
-Requires-Dist: requests==2.31.0
-
 # YandexGPT Python SDK
 
 ## Introduction
 The YandexGPT Python SDK provides an easy-to-use interface for interacting with the Yandex GPT API. It includes asynchronous methods for sending requests to the Yandex GPT API, handling authentication, and processing responses. This SDK is designed to simplify the integration of Yandex GPT functionalities into Python applications.
 
 ## Table of Contents
 - [Introduction](#Introduction)
 - [Features](#Features)
+- [Documentation](#Documentation)
 - [Installation using pip](#Installation-using-pip)
 - [Local installation using pip](#Local-installation-using-pip)
 - [Usage](#Usage)
 - [Configuration](#Configuration)
 - [Examples](#Examples)
 - [Troubleshooting](#Troubleshooting)
 - [Contributors](#Contributors)
@@ -37,14 +20,18 @@
 - Asynchronous API calls to Yandex GPT.
 - Easy configuration of API credentials and model parameters.
 - Supports multiple GPT models.
 - Includes utility for managing API request headers and payload.
 
 The SDK depends on several Python libraries for its operation. These dependencies are specified in the [requirements.txt](requirements.txt) file.
 
+
+## Documentation
+For more detailed information, including installation guides, usage examples, and API references, please visit the [YandexGPT Python SDK Documentation](https://yandexgpt-python.readthedocs.io/en/latest/).
+
 ## Installation using pip
 To install the YandexGPT Python SDK as a package using pip, run the following command:
 ```shell
 pip install yandexgpt-python
 ```
 
 ## Local installation using pip
@@ -112,11 +99,11 @@
 ```
 
 
 ## Troubleshooting
 For any issues related to the configuration or usage of the SDK, ensure that the catalog ID, API key, and model type are correctly set and that the environment variables (if used) are properly configured.
 
 ## Contributors
-This project is developed and maintained by Gregory Matsnev. Contributions are welcome.
+This project is developed and maintained by ALL SEE LLC. Contributions are welcome.
 
 ## License
 This project is licensed under the MIT License. For more information, see the LICENSE file in the project's GitHub repository.
```

### Comparing `yandexgpt-python-0.2.0/README.md` & `yandexgpt-python-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+Metadata-Version: 2.1
+Name: yandexgpt-python
+Version: 0.2.3
+Summary: A Python SDK for interacting with the YandexGPT API.
+Home-page: https://github.com/allseeteam/yandexgpt-python
+Author: ALL SEE LLC
+Author-email: info@allsee.team
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.9.3
+Requires-Dist: cryptography==42.0.5
+Requires-Dist: PyJWT==2.8.0
+Requires-Dist: requests==2.31.0
+
 # YandexGPT Python SDK
 
 ## Introduction
 The YandexGPT Python SDK provides an easy-to-use interface for interacting with the Yandex GPT API. It includes asynchronous methods for sending requests to the Yandex GPT API, handling authentication, and processing responses. This SDK is designed to simplify the integration of Yandex GPT functionalities into Python applications.
 
 ## Table of Contents
 - [Introduction](#Introduction)
 - [Features](#Features)
+- [Documentation](#Documentation)
 - [Installation using pip](#Installation-using-pip)
 - [Local installation using pip](#Local-installation-using-pip)
 - [Usage](#Usage)
 - [Configuration](#Configuration)
 - [Examples](#Examples)
 - [Troubleshooting](#Troubleshooting)
 - [Contributors](#Contributors)
@@ -19,14 +38,18 @@
 - Asynchronous API calls to Yandex GPT.
 - Easy configuration of API credentials and model parameters.
 - Supports multiple GPT models.
 - Includes utility for managing API request headers and payload.
 
 The SDK depends on several Python libraries for its operation. These dependencies are specified in the [requirements.txt](requirements.txt) file.
 
+
+## Documentation
+For more detailed information, including installation guides, usage examples, and API references, please visit the [YandexGPT Python SDK Documentation](https://yandexgpt-python.readthedocs.io/en/latest/).
+
 ## Installation using pip
 To install the YandexGPT Python SDK as a package using pip, run the following command:
 ```shell
 pip install yandexgpt-python
 ```
 
 ## Local installation using pip
@@ -94,11 +117,11 @@
 ```
 
 
 ## Troubleshooting
 For any issues related to the configuration or usage of the SDK, ensure that the catalog ID, API key, and model type are correctly set and that the environment variables (if used) are properly configured.
 
 ## Contributors
-This project is developed and maintained by Gregory Matsnev. Contributions are welcome.
+This project is developed and maintained by ALL SEE LLC. Contributions are welcome.
 
 ## License
 This project is licensed under the MIT License. For more information, see the LICENSE file in the project's GitHub repository.
```

### Comparing `yandexgpt-python-0.2.0/yandex_gpt/config_manager.py` & `yandexgpt-python-0.2.3/yandex_gpt/config_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,74 +15,117 @@
         "yandexgpt",
         "yandexgpt-lite",
         "summarization"
     ]
 
 
 class YandexGPTConfigManagerBase:
+    """
+    Base class for YaGPT configuration management. It handles configurations related to model type, catalog ID, IAM
+    token, and API key for authorization when making requests to the completion endpoint.
+
+    Attributes
+    ----------
+    model_type : Optional[str]
+        The model type to use. Supported values include 'yandexgpt', 'yandexgpt-lite', 'summarization'.
+    catalog_id : Optional[str]
+        The Catalog ID on YandexCloud to be used.
+    iam_token : Optional[str]
+        The IAM token for authorization. Either `iam_token` or `api_key` is used for authorization. If both are
+        provided, `iam_token` will be preferred. More details on getting an IAM token can be found here:
+        https://yandex.cloud/ru/docs/iam/operations/iam-token/create-for-sa
+    api_key : Optional[str]
+        The API key for authorization. More details on getting an API key can be found here:
+        https://yandex.cloud/ru/docs/iam/operations/api-key/create
+    """
     def __init__(
             self,
             model_type: Optional[str] = None,
             catalog_id: Optional[str] = None,
             iam_token: Optional[str] = None,
             api_key: Optional[str] = None,
     ) -> None:
         """
-        Base class for YaGPT configuration. It contains model type, catalog ID, IAM token or API key, which are used for
-        authorization when making requests to the completion endpoint.
+        Initializes a new instance of the YandexGPTConfigManagerBase class.
 
-        :param model_type: model type to use. Supported values: 'yandexgpt', 'yandexgpt-lite', 'summarization'.
-        :param catalog_id: Catalog ID on YandexCloud to use.
-        :param iam_token: IAM token to use (you provide either iam_token or api_key, if you provide both, iam_token will
-        be used in the future) (how to get IAM token:
-        https://yandex.cloud/ru/docs/iam/operations/iam-token/create-for-sa).
-        :param api_key: API key to use (how to get API key:
-        https://yandex.cloud/ru/docs/iam/operations/api-key/create).
+        Parameters
+        ----------
+        model_type : Optional[str], optional
+            Model type to use.
+        catalog_id : Optional[str], optional
+            Catalog ID on YandexCloud to use.
+        iam_token : Optional[str], optional
+            IAM token for authorization.
+        api_key : Optional[str], optional
+            API key for authorization.
         """
         self.model_type: Optional[str] = model_type
         self.catalog_id: Optional[str] = catalog_id
         self.iam_token: Optional[str] = iam_token
         self.api_key: Optional[str] = api_key
 
     @property
     def completion_request_authorization_field(self) -> str:
         """
-        A dynamic property that returns authorization field for the completion request header.
-        Either iam_token or api_key must be set, otherwise ValueError will be raised.
-        :return: authorization field for the completion request header in the form of a string: "Bearer {iam_token}" or
-        "Api-Key {api_key}".
+        Returns the authorization field for the completion request header based on the IAM token or API key.
+
+        Raises
+        ------
+        ValueError
+            If neither IAM token nor API key is set.
+
+        Returns
+        -------
+        str
+            The authorization field for the completion request header in the form of "Bearer {iam_token}" or
+            "Api-Key {api_key}".
         """
         # Checking if either iam_token or api_key is set and returning the authorization field string
         if self.iam_token:
             return f"Bearer {self.iam_token}"
         elif self.api_key:
             return f"Api-Key {self.api_key}"
         else:
             raise ValueError("IAM token or API key is not set")
 
     @property
     def completion_request_catalog_id_field(self) -> str:
         """
-        A dynamic property that returns catalog id field for the completion request header. If catalog_id is not set,
-        ValueError will be raised.
-        :return: catalog id field for the completion request header in the form of a string: "{catalog_id}".
+        Returns the catalog ID field for the completion request header.
+
+        Raises
+        ------
+        ValueError
+            If catalog_id is not set.
+
+        Returns
+        -------
+        str
+            The catalog ID field for the completion request header.
         """
         # Checking if catalog_id is set and returning the catalog id field string
         if self.catalog_id:
             return self.catalog_id
         else:
             raise ValueError("Catalog ID is not set")
 
     @property
     def completion_request_model_type_uri_field(self) -> str:
         """
-        A dynamic property that returns model type field for the completion request payload. If model_type or catalog_id
-        is not set, ValueError will be raised. If model_type not in available_models, ValueError will be raised.
-        :return: model type field for the completion request header in the form of a string:
-        "gpt://{self.config_manager.catalog_id}/{self.config_manager.model_type}/latest".
+        Returns the model type URI field for the completion request payload.
+
+        Raises
+        ------
+        ValueError
+            If model_type or catalog_id is not set or if model_type is not in the available models.
+
+        Returns
+        -------
+        str
+            The model type URI field for the completion request header in the URI format.
         """
         global available_models
 
         # Checking if model_type is in available_models
         if self.model_type not in available_models:
             raise ValueError(f"Model type {self.model_type} is not supported. Supported values: {available_models}")
 
@@ -90,29 +133,47 @@
         if self.model_type and self.catalog_id:
             return f"gpt://{self.catalog_id}/{self.model_type}/latest"
         else:
             raise ValueError("Model type or catalog ID is not set")
 
 
 class YandexGPTConfigManagerForAPIKey(YandexGPTConfigManagerBase):
+    """
+    Class for configuring the YandexGPT model using an API key. It supports setting model type, catalog ID, and API key
+    directly or through environment variables. The class allows for configuration flexibility by providing the option to
+    use environmental variables for model type (`YANDEX_GPT_MODEL_TYPE`), catalog ID (`YANDEX_GPT_CATALOG_ID`), and API
+    key (`YANDEX_GPT_API_KEY`), which can override the constructor values if set.
+
+    Attributes
+    ----------
+    model_type : Optional[str]
+        The model type to use. Supported values include 'yandexgpt', 'yandexgpt-lite', 'summarization'.
+    catalog_id : Optional[str]
+        The Catalog ID on YandexCloud to be used.
+    api_key : Optional[str]
+        The API key for authorization. More details on obtaining an API key can be found here:
+        https://yandex.cloud/ru/docs/iam/operations/api-key/create
+    """
     def __init__(
             self,
             model_type: Optional[str] = None,
             catalog_id: Optional[str] = None,
             api_key: Optional[str] = None,
     ) -> None:
         """
-        Class for YaGPT configuration using API key. It contains model type, catalog ID and API key, which are used for
-        authorization when making requests to the completion endpoint. You can set parameters using the constructor or
-        set them in the environment variables: YANDEX_GPT_MODEL_TYPE, YANDEX_GPT_CATALOG_ID and YANDEX_GPT_API_KEY.
-
-        :param model_type: model type to use. Supported values: 'yandexgpt', 'yandexgpt-lite', 'summarization'.
-        :param catalog_id: Catalog ID on YandexCloud to use.
-        :param api_key: API key to use (how to get API key:
-        https://yandex.cloud/ru/docs/iam/operations/api-key/create).
+        Initializes a new instance of the YandexGPTConfigManagerForAPIKey class.
+
+        Parameters
+        ----------
+        model_type : Optional[str], optional
+            Model type to use.
+        catalog_id : Optional[str], optional
+            Catalog ID on YandexCloud to use.
+        api_key : Optional[str], optional
+            API key for authorization.
         """
         # Setting model type, catalog ID and API key from the constructor
         super().__init__(
             model_type=model_type,
             catalog_id=catalog_id,
             api_key=api_key
         )
@@ -121,23 +182,23 @@
         self._set_config_from_env_vars()
 
         # Checking if model type, catalog ID and API key are set
         self._check_config()
 
     def _set_config_from_env_vars(self) -> None:
         """
-        Sets config from environment variables. If environment variables are not set, default values will be used.
+        Sets configuration parameters from environment variables if they are not provided in the constructor.
         """
         self.model_type = os.environ.get("YANDEX_GPT_MODEL_TYPE", self.model_type)
         self.catalog_id = os.environ.get("YANDEX_GPT_CATALOG_ID", self.catalog_id)
         self.api_key = os.environ.get("YANDEX_GPT_API_KEY", self.api_key)
 
     def _check_config(self) -> None:
         """
-        Checks if model type, catalog ID and API key are set. If not, ValueError will be raised.
+        Ensures that the necessary configuration parameters are set, raising a ValueError if any are missing.
         """
         if not self.model_type:
             raise ValueError(
                 "Model type is not set. You can ether provide it in the constructor or set in YANDEX_GPT_MODEL_TYPE "
                 "environment variable"
             )
         elif not self.catalog_id:
@@ -149,35 +210,52 @@
             raise ValueError(
                 "API key is not set. You can ether provide it in the constructor or set in YANDEX_GPT_API_KEY "
                 "environment variable"
             )
 
 
 class YandexGPTConfigManagerForIAMToken(YandexGPTConfigManagerBase):
+    """
+    Class for configuring the YandexGPT model using an IAM token. It handles configurations involving model type,
+    catalog ID, and IAM token, with options for direct input or initialization via environment variables. The class
+    provides several pathways for initializing these configurations:
+
+    1. Directly through constructor parameters.
+    2. Through environment variables `YANDEX_GPT_MODEL_TYPE`, `YANDEX_GPT_CATALOG_ID`, and `YANDEX_GPT_IAM_TOKEN`.
+    3. Automatically generating the IAM token using the environment variables `YANDEX_GPT_IAM_URL`,
+       `YANDEX_GPT_SERVICE_ACCOUNT_ID`, `YANDEX_GPT_SERVICE_ACCOUNT_KEY_ID`, `YANDEX_GPT_CATALOG_ID`, and
+       `YANDEX_GPT_PRIVATE_KEY`.
+
+    Attributes
+    ----------
+    model_type : Optional[str]
+        The model type to use. Supported values include 'yandexgpt', 'yandexgpt-lite', 'summarization'.
+    catalog_id : Optional[str]
+        The Catalog ID on YandexCloud to be used.
+    iam_token : Optional[str]
+        The IAM token for authorization. Details on obtaining an IAM token can be found here:
+        https://yandex.cloud/ru/docs/iam/operations/iam-token/create-for-sa
+    """
     def __init__(
             self,
             model_type: Optional[str] = None,
             catalog_id: Optional[str] = None,
             iam_token: Optional[str] = None,
     ) -> None:
         """
-        Class for YaGPT configuration using IAM token. It contains model type, catalog ID and IAM token, which are used
-        for authorization when making requests to the completion endpoint.
+        Initializes a new instance of the YandexGPTConfigManagerForIAMToken class.
 
-        For initialization, you can ether:
-        1) Provide model type, IAM token, and catalog ID directly as constructor parameters;
-        2) Use YANDEX_GPT_MODEL_TYPE, YANDEX_GPT_CATALOG_ID and YANDEX_GPT_IAM_TOKEN environment variables for direct
-        initialization;
-        3) Use YANDEX_GPT_IAM_URL, YANDEX_GPT_SERVICE_ACCOUNT_ID, YANDEX_GPT_SERVICE_ACCOUNT_KEY_ID,
-        YANDEX_GPT_CATALOG_ID and YANDEX_GPT_PRIVATE_KEY environment variables for generating IAM token;
-
-        :param model_type: model type to use. Supported values: 'yandexgpt', 'yandexgpt-lite', 'summarization'.
-        :param catalog_id: Catalog ID on YandexCloud to use.
-        :param iam_token: IAM token to use (how to get IAM token:
-        https://yandex.cloud/ru/docs/iam/operations/iam-token/create-for-sa).
+        Parameters
+        ----------
+        model_type : Optional[str], optional
+            Model type to use.
+        catalog_id : Optional[str], optional
+            Catalog ID on YandexCloud to use.
+        iam_token : Optional[str], optional
+            IAM token for authorization.
         """
         # Setting model type, catalog ID and IAM token from the constructor
         super().__init__(
             model_type=model_type,
             catalog_id=catalog_id,
             iam_token=iam_token
         )
@@ -197,28 +275,28 @@
             return
         else:
             # Trying to initialize from environment variables
             self._set_config_from_env_vars()
 
     def _set_config_from_env_vars(self) -> None:
         """
-        Sets config from environment variables. If environment variables are not set, default values will be used. If
-        IAM token is not set in environment variables, trying to generate it using environment variables.
+        Sets config from environment variables or tries to generate the IAM token using additional environment variables
+        if not directly provided.
         """
         self.model_type = os.environ.get("YANDEX_GPT_MODEL_TYPE", self.model_type)
         self.catalog_id = os.environ.get("YANDEX_GPT_CATALOG_ID", self.catalog_id)
         self.iam_token = os.environ.get("YANDEX_GPT_IAM_TOKEN", self.iam_token)
 
         if not self.iam_token:
             # If IAM token is not set, trying to initialize from config and private key
             self._set_iam_from_env_config_and_private_key()
 
     def _set_iam_from_env_config_and_private_key(self) -> None:
         """
-        Generates and sets IAM token from environment variables.
+        Generates and sets IAM token from environment variables if not provided.
         """
         # Getting environment variables
         iam_url: str = os.getenv("YANDEX_GPT_IAM_URL", "https://iam.api.cloud.yandex.net/iam/v1/tokens")
         service_account_id: Optional[str] = os.getenv("YANDEX_GPT_SERVICE_ACCOUNT_ID", None)
         service_account_key_id: Optional[str] = os.getenv("YANDEX_GPT_SERVICE_ACCOUNT_KEY_ID", None)
         catalog_id: Optional[str] = os.getenv("YANDEX_GPT_CATALOG_ID", None)
         private_key: Optional[str] = os.getenv("YANDEX_GPT_PRIVATE_KEY", None)
@@ -242,20 +320,31 @@
     def _generate_jwt_token(
             service_account_id: str,
             private_key: str,
             key_id: str,
             url: str = "https://iam.api.cloud.yandex.net/iam/v1/tokens",
     ) -> str:
         """
-        Generates JWT token from service account id, private key, and key id.
-        :param service_account_id: service account id
-        :param private_key: private key
-        :param key_id: key id
-        :param url: url for swapping JWT token to IAM request
-        :return: encoded JWT token
+        Generates and swaps a JWT token to an IAM token.
+
+        Parameters
+        ----------
+        service_account_id : str
+            Service account ID
+        private_key : str
+            Private key
+        key_id : str
+            Service account key ID
+        url : str
+            IAM URL for token request
+
+        Returns
+        -------
+        str
+            The IAM token
         """
         # Generating JWT token
         now: int = int(time.time())
         payload: Dict[str, Any] = {
             "aud": url,
             "iss": service_account_id,
             "iat": now,
@@ -270,18 +359,32 @@
         return encoded_token
 
     @staticmethod
     def _swap_jwt_to_iam(
             jwt_token: str, url: str = "https://iam.api.cloud.yandex.net/iam/v1/tokens"
     ) -> str:
         """
-        Swaps JWT token to IAM token.
-        :param jwt_token: encoded JWT token
-        :param url: url for swapping JWT token to IAM request
-        :return: IAM token
+        Swaps a JWT token for an IAM token by making a POST request to the Yandex IAM service.
+
+        Parameters
+        ----------
+        jwt_token : str
+            The JWT token to be swapped.
+        url : str, optional
+            The URL to send the JWT token to, by default set to Yandex IAM token service endpoint.
+
+        Returns
+        -------
+        str
+            The IAM token received in response.
+
+        Raises
+        ------
+        Exception
+            If the request fails or does not return a successful response.
         """
         headers: Dict[str, str] = {"Content-Type": "application/json"}
         data: Dict[str, str] = {"jwt": jwt_token}
         # Swapping JWT token to IAM
         response: requests.Response = requests.post(
             url,
             headers=headers,
@@ -292,15 +395,15 @@
             return response.json()["iamToken"]
         else:
             # If failed to get IAM token raise an exception
             raise Exception(f"Failed to get IAM token. Status code: {response.status_code}\n{response.text}")
 
     def _check_config(self) -> None:
         """
-        Checks if model type, catalog ID and API key are set. If not, ValueError will be raised.
+        Ensures that the necessary configuration parameters are set, raising a ValueError if any are missing.
         """
         if not self.model_type:
             raise ValueError(
                 "Model type is not set. You can ether provide it in the constructor or set in YANDEX_GPT_MODEL_TYPE "
                 "environment variable"
             )
         elif not self.catalog_id:
@@ -315,21 +418,29 @@
                 "YANDEX_GPT_SERVICE_ACCOUNT_KEY_ID, YANDEX_GPT_CATALOG_ID and YANDEX_GPT_PRIVATE_KEY environment "
                 "variables"
             )
 
 
 class YandexGPTConfigManagerForIAMTokenWithBase64Key(YandexGPTConfigManagerForIAMToken):
     """
-    This class is modified version of YandexGPTConfigManagerForIAMToken for handling base64-encoded private key set in
-    YANDEX_GPT_PRIVATE_KEY_BASE64 environment variable. It may be useful when dealing with docker because there is no
-    special characters like '\n' which can break key parsing to docker container environment.
+    A specialized configuration manager for YandexGPT that handles base64-encoded private keys. This is particularly
+    useful in environments like Docker where special characters (e.g., newline) in environment variables can cause
+    issues. The private key is expected to be set in the YANDEX_GPT_PRIVATE_KEY_BASE64 environment variable.
+
+    Inherits attributes from YandexGPTConfigManagerForIAMToken.
     """
     def _set_iam_from_env_config_and_private_key(self) -> None:
         """
-        Generates and sets IAM token from environment variables.
+        Overrides the base method to generate and set the IAM token using a base64-encoded private key from
+        environment variables.
+
+        Raises
+        ------
+        ValueError
+            If any required environment variables are missing.
         """
         # Getting environment variables
         iam_url: str = os.getenv("YANDEX_GPT_IAM_URL", "https://iam.api.cloud.yandex.net/iam/v1/tokens")
         service_account_id: Optional[str] = os.getenv("YANDEX_GPT_SERVICE_ACCOUNT_ID", None)
         service_account_key_id: Optional[str] = os.getenv("YANDEX_GPT_SERVICE_ACCOUNT_KEY_ID", None)
         catalog_id: Optional[str] = os.getenv("YANDEX_GPT_CATALOG_ID", None)
         private_key_base64: Optional[str] = os.getenv("YANDEX_GPT_PRIVATE_KEY_BASE64", None)
```

### Comparing `yandexgpt-python-0.2.0/yandexgpt_python.egg-info/PKG-INFO` & `yandexgpt-python-0.2.3/yandexgpt_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: yandexgpt-python
-Version: 0.2.0
+Version: 0.2.3
 Summary: A Python SDK for interacting with the YandexGPT API.
 Home-page: https://github.com/allseeteam/yandexgpt-python
-Author: Gregory Matsnev
-Author-email: grigorij1m@gmail.com
+Author: ALL SEE LLC
+Author-email: info@allsee.team
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.9.3
@@ -20,14 +20,15 @@
 
 ## Introduction
 The YandexGPT Python SDK provides an easy-to-use interface for interacting with the Yandex GPT API. It includes asynchronous methods for sending requests to the Yandex GPT API, handling authentication, and processing responses. This SDK is designed to simplify the integration of Yandex GPT functionalities into Python applications.
 
 ## Table of Contents
 - [Introduction](#Introduction)
 - [Features](#Features)
+- [Documentation](#Documentation)
 - [Installation using pip](#Installation-using-pip)
 - [Local installation using pip](#Local-installation-using-pip)
 - [Usage](#Usage)
 - [Configuration](#Configuration)
 - [Examples](#Examples)
 - [Troubleshooting](#Troubleshooting)
 - [Contributors](#Contributors)
@@ -37,14 +38,18 @@
 - Asynchronous API calls to Yandex GPT.
 - Easy configuration of API credentials and model parameters.
 - Supports multiple GPT models.
 - Includes utility for managing API request headers and payload.
 
 The SDK depends on several Python libraries for its operation. These dependencies are specified in the [requirements.txt](requirements.txt) file.
 
+
+## Documentation
+For more detailed information, including installation guides, usage examples, and API references, please visit the [YandexGPT Python SDK Documentation](https://yandexgpt-python.readthedocs.io/en/latest/).
+
 ## Installation using pip
 To install the YandexGPT Python SDK as a package using pip, run the following command:
 ```shell
 pip install yandexgpt-python
 ```
 
 ## Local installation using pip
@@ -112,11 +117,11 @@
 ```
 
 
 ## Troubleshooting
 For any issues related to the configuration or usage of the SDK, ensure that the catalog ID, API key, and model type are correctly set and that the environment variables (if used) are properly configured.
 
 ## Contributors
-This project is developed and maintained by Gregory Matsnev. Contributions are welcome.
+This project is developed and maintained by ALL SEE LLC. Contributions are welcome.
 
 ## License
 This project is licensed under the MIT License. For more information, see the LICENSE file in the project's GitHub repository.
```

