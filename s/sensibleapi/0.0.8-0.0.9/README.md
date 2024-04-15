# Comparing `tmp/sensibleapi-0.0.8.tar.gz` & `tmp/sensibleapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensibleapi-0.0.8.tar", last modified: Fri Dec  8 13:33:56 2023, max compression
+gzip compressed data, was "sensibleapi-0.0.9.tar", last modified: Fri Dec  8 17:43:50 2023, max compression
```

## Comparing `sensibleapi-0.0.8.tar` & `sensibleapi-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 13:33:56.840364 sensibleapi-0.0.8/
--rw-r--r--   0 horape     (501) staff       (20)     1074 2023-11-23 16:12:06.000000 sensibleapi-0.0.8/LICENSE
--rw-r--r--   0 horape     (501) staff       (20)    12331 2023-12-08 13:33:56.840131 sensibleapi-0.0.8/PKG-INFO
--rw-r--r--   0 horape     (501) staff       (20)    11904 2023-12-08 13:28:17.000000 sensibleapi-0.0.8/README.md
-drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 13:33:56.839107 sensibleapi-0.0.8/sensibleapi/
--rw-r--r--   0 horape     (501) staff       (20)       37 2023-12-06 18:37:28.000000 sensibleapi-0.0.8/sensibleapi/__init__.py
--rw-r--r--   0 horape     (501) staff       (20)     5481 2023-12-08 13:28:19.000000 sensibleapi-0.0.8/sensibleapi/sensibleapi.py
-drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 13:33:56.839924 sensibleapi-0.0.8/sensibleapi.egg-info/
--rw-r--r--   0 horape     (501) staff       (20)    12331 2023-12-08 13:33:56.000000 sensibleapi-0.0.8/sensibleapi.egg-info/PKG-INFO
--rw-r--r--   0 horape     (501) staff       (20)      251 2023-12-08 13:33:56.000000 sensibleapi-0.0.8/sensibleapi.egg-info/SOURCES.txt
--rw-r--r--   0 horape     (501) staff       (20)        1 2023-12-08 13:33:56.000000 sensibleapi-0.0.8/sensibleapi.egg-info/dependency_links.txt
--rw-r--r--   0 horape     (501) staff       (20)        9 2023-12-08 13:33:56.000000 sensibleapi-0.0.8/sensibleapi.egg-info/requires.txt
--rw-r--r--   0 horape     (501) staff       (20)       12 2023-12-08 13:33:56.000000 sensibleapi-0.0.8/sensibleapi.egg-info/top_level.txt
--rw-r--r--   0 horape     (501) staff       (20)       38 2023-12-08 13:33:56.840406 sensibleapi-0.0.8/setup.cfg
--rw-r--r--   0 horape     (501) staff       (20)      677 2023-12-08 13:30:07.000000 sensibleapi-0.0.8/setup.py
+drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 17:43:50.175550 sensibleapi-0.0.9/
+-rw-r--r--   0 horape     (501) staff       (20)     1074 2023-11-23 16:12:06.000000 sensibleapi-0.0.9/LICENSE
+-rw-r--r--   0 horape     (501) staff       (20)    12439 2023-12-08 17:43:50.175321 sensibleapi-0.0.9/PKG-INFO
+-rw-r--r--   0 horape     (501) staff       (20)    12012 2023-12-08 17:42:56.000000 sensibleapi-0.0.9/README.md
+drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 17:43:50.174466 sensibleapi-0.0.9/sensibleapi/
+-rw-r--r--   0 horape     (501) staff       (20)       37 2023-12-06 18:37:28.000000 sensibleapi-0.0.9/sensibleapi/__init__.py
+-rw-r--r--   0 horape     (501) staff       (20)     5481 2023-12-08 13:28:19.000000 sensibleapi-0.0.9/sensibleapi/sensibleapi.py
+drwxr-xr-x   0 horape     (501) staff       (20)        0 2023-12-08 17:43:50.175164 sensibleapi-0.0.9/sensibleapi.egg-info/
+-rw-r--r--   0 horape     (501) staff       (20)    12439 2023-12-08 17:43:50.000000 sensibleapi-0.0.9/sensibleapi.egg-info/PKG-INFO
+-rw-r--r--   0 horape     (501) staff       (20)      251 2023-12-08 17:43:50.000000 sensibleapi-0.0.9/sensibleapi.egg-info/SOURCES.txt
+-rw-r--r--   0 horape     (501) staff       (20)        1 2023-12-08 17:43:50.000000 sensibleapi-0.0.9/sensibleapi.egg-info/dependency_links.txt
+-rw-r--r--   0 horape     (501) staff       (20)        9 2023-12-08 17:43:50.000000 sensibleapi-0.0.9/sensibleapi.egg-info/requires.txt
+-rw-r--r--   0 horape     (501) staff       (20)       12 2023-12-08 17:43:50.000000 sensibleapi-0.0.9/sensibleapi.egg-info/top_level.txt
+-rw-r--r--   0 horape     (501) staff       (20)       38 2023-12-08 17:43:50.175585 sensibleapi-0.0.9/setup.cfg
+-rw-r--r--   0 horape     (501) staff       (20)      677 2023-12-08 17:43:18.000000 sensibleapi-0.0.9/setup.py
```

### Comparing `sensibleapi-0.0.8/LICENSE` & `sensibleapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sensibleapi-0.0.8/PKG-INFO` & `sensibleapi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensibleapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for Sensible, the developer-first platform for extracting structured data from documents so that you can build document-automation features into your SaaS products
 Home-page: https://github.com/sensible-hq/sensible-api-py
 Author: Sensible Technologies, Inc
 Author-email: hello@sensible.so
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -58,15 +58,15 @@
 
 ```python
 sensible = SensibleSDK("YOUR_API_KEY")
 ```
 
 **Note:** Ensure you secure your API key in production, for example as a GitHub secret.
 
-## Quickstart
+## Quickstart<a id="quickstart"></a>
 
 To extract data from a sample document at a URL:
 
 1. Install the Sensible SDK using the steps in the previous section.
 2. Paste the following code into an empty `index.py` file:
 
 ```python
@@ -112,15 +112,15 @@
 
 #### Optional: Understand extraction
 
 Navigate to the example in the [SenseML editor](https://app.sensible.so/editor/?d=sensible_instruct_basics&c=contract&g=contract) to see how the extraction you just ran works in the Sensible app. You can add more fields to the left pane to extract more data:
 
 ![Click to enlarge](https://raw.githubusercontent.com/sensible-hq/sensible-docs/main/readme-sync/assets/v0/images/final/sdk_node_1.png)
 
-## Usage: Extract document data
+## Usage: Extract document data<a id="usage-extract-document-data"></a>
 
 You can use this SDK to extract data from a document, as specified by the extraction configurations and document types defined in your Sensible account.
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document data extraction:
 
@@ -166,15 +166,15 @@
 ### Extraction results
 
 Get extraction results by using a webhook or calling the Wait For method.
 
 For the schema for the results of an extraction request,  see [Extract data from a document](https://docs.sensible.so/reference/extract-data-from-a-document) and expand the 200 responses in the middle pane and the right pane to see the model and an example, respectively.
 
 
-## Usage: Classify documents by type
+## Usage: Classify documents by type<a id="usage-classify-documents-by-type"></a>
 
 You can use this SDK to classify a document by type, as specified by the document types defined in your Sensible account. For more information, see [Classifying documents by type](https://docs.sensible.so/docs/classify).
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document classification:
```

### Comparing `sensibleapi-0.0.8/README.md` & `sensibleapi-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ```python
 sensible = SensibleSDK("YOUR_API_KEY")
 ```
 
 **Note:** Ensure you secure your API key in production, for example as a GitHub secret.
 
-## Quickstart
+## Quickstart<a id="quickstart"></a>
 
 To extract data from a sample document at a URL:
 
 1. Install the Sensible SDK using the steps in the previous section.
 2. Paste the following code into an empty `index.py` file:
 
 ```python
@@ -102,15 +102,15 @@
 
 #### Optional: Understand extraction
 
 Navigate to the example in the [SenseML editor](https://app.sensible.so/editor/?d=sensible_instruct_basics&c=contract&g=contract) to see how the extraction you just ran works in the Sensible app. You can add more fields to the left pane to extract more data:
 
 ![Click to enlarge](https://raw.githubusercontent.com/sensible-hq/sensible-docs/main/readme-sync/assets/v0/images/final/sdk_node_1.png)
 
-## Usage: Extract document data
+## Usage: Extract document data<a id="usage-extract-document-data"></a>
 
 You can use this SDK to extract data from a document, as specified by the extraction configurations and document types defined in your Sensible account.
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document data extraction:
 
@@ -156,15 +156,15 @@
 ### Extraction results
 
 Get extraction results by using a webhook or calling the Wait For method.
 
 For the schema for the results of an extraction request,  see [Extract data from a document](https://docs.sensible.so/reference/extract-data-from-a-document) and expand the 200 responses in the middle pane and the right pane to see the model and an example, respectively.
 
 
-## Usage: Classify documents by type
+## Usage: Classify documents by type<a id="usage-classify-documents-by-type"></a>
 
 You can use this SDK to classify a document by type, as specified by the document types defined in your Sensible account. For more information, see [Classifying documents by type](https://docs.sensible.so/docs/classify).
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document classification:
```

### Comparing `sensibleapi-0.0.8/sensibleapi/sensibleapi.py` & `sensibleapi-0.0.9/sensibleapi/sensibleapi.py`

 * *Files identical despite different names*

### Comparing `sensibleapi-0.0.8/sensibleapi.egg-info/PKG-INFO` & `sensibleapi-0.0.9/sensibleapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensibleapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for Sensible, the developer-first platform for extracting structured data from documents so that you can build document-automation features into your SaaS products
 Home-page: https://github.com/sensible-hq/sensible-api-py
 Author: Sensible Technologies, Inc
 Author-email: hello@sensible.so
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -58,15 +58,15 @@
 
 ```python
 sensible = SensibleSDK("YOUR_API_KEY")
 ```
 
 **Note:** Ensure you secure your API key in production, for example as a GitHub secret.
 
-## Quickstart
+## Quickstart<a id="quickstart"></a>
 
 To extract data from a sample document at a URL:
 
 1. Install the Sensible SDK using the steps in the previous section.
 2. Paste the following code into an empty `index.py` file:
 
 ```python
@@ -112,15 +112,15 @@
 
 #### Optional: Understand extraction
 
 Navigate to the example in the [SenseML editor](https://app.sensible.so/editor/?d=sensible_instruct_basics&c=contract&g=contract) to see how the extraction you just ran works in the Sensible app. You can add more fields to the left pane to extract more data:
 
 ![Click to enlarge](https://raw.githubusercontent.com/sensible-hq/sensible-docs/main/readme-sync/assets/v0/images/final/sdk_node_1.png)
 
-## Usage: Extract document data
+## Usage: Extract document data<a id="usage-extract-document-data"></a>
 
 You can use this SDK to extract data from a document, as specified by the extraction configurations and document types defined in your Sensible account.
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document data extraction:
 
@@ -166,15 +166,15 @@
 ### Extraction results
 
 Get extraction results by using a webhook or calling the Wait For method.
 
 For the schema for the results of an extraction request,  see [Extract data from a document](https://docs.sensible.so/reference/extract-data-from-a-document) and expand the 200 responses in the middle pane and the right pane to see the model and an example, respectively.
 
 
-## Usage: Classify documents by type
+## Usage: Classify documents by type<a id="usage-classify-documents-by-type"></a>
 
 You can use this SDK to classify a document by type, as specified by the document types defined in your Sensible account. For more information, see [Classifying documents by type](https://docs.sensible.so/docs/classify).
 
 ### Overview
 
 See the following steps for an overview of the SDK's workflow for document classification:
```

### Comparing `sensibleapi-0.0.8/setup.py` & `sensibleapi-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='sensibleapi',
-    version='0.0.8',
+    version='0.0.9',
     author='Sensible Technologies, Inc',
     author_email='hello@sensible.so',
     description='Python SDK for Sensible, the developer-first platform for extracting structured data from documents so that you can build document-automation features into your SaaS products',
     packages=find_packages(),
     install_requires=['requests'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

