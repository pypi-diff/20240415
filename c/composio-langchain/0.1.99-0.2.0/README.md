# Comparing `tmp/composio_langchain-0.1.99.tar.gz` & `tmp/composio_langchain-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.99.tar", last modified: Fri Apr 12 15:24:23 2024, max compression
+gzip compressed data, was "composio_langchain-0.2.0.tar", last modified: Mon Apr 15 09:07:46 2024, max compression
```

## Comparing `composio_langchain-0.1.99.tar` & `composio_langchain-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:23.738706 composio_langchain-0.1.99/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.99/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 15:24:23.738463 composio_langchain-0.1.99/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.99/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:23.737305 composio_langchain-0.1.99/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 09:34:14.000000 composio_langchain-0.1.99/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5518 2024-04-12 01:13:56.000000 composio_langchain-0.1.99/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.99/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:23.738207 composio_langchain-0.1.99/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 15:24:23.000000 composio_langchain-0.1.99/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-12 15:24:23.000000 composio_langchain-0.1.99/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:24:23.000000 composio_langchain-0.1.99/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      149 2024-04-12 15:24:23.000000 composio_langchain-0.1.99/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-12 15:24:23.000000 composio_langchain-0.1.99/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      455 2024-04-12 15:24:05.000000 composio_langchain-0.1.99/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:24:23.738750 composio_langchain-0.1.99/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-12 15:24:05.000000 composio_langchain-0.1.99/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:46.148240 composio_langchain-0.2.0/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_langchain-0.2.0/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-15 09:07:46.148039 composio_langchain-0.2.0/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-15 07:39:40.000000 composio_langchain-0.2.0/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:46.146940 composio_langchain-0.2.0/composio_langchain/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      101 2024-04-15 07:39:40.000000 composio_langchain-0.2.0/composio_langchain/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5265 2024-04-15 09:05:53.000000 composio_langchain-0.2.0/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-15 07:39:40.000000 composio_langchain-0.2.0/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:46.147824 composio_langchain-0.2.0/composio_langchain.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3332 2024-04-15 09:07:46.000000 composio_langchain-0.2.0/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-15 09:07:46.000000 composio_langchain-0.2.0/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-15 09:07:46.000000 composio_langchain-0.2.0/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      148 2024-04-15 09:07:46.000000 composio_langchain-0.2.0/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-15 09:07:46.000000 composio_langchain-0.2.0/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      454 2024-04-15 09:07:06.000000 composio_langchain-0.2.0/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-15 09:07:46.148284 composio_langchain-0.2.0/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-15 09:07:06.000000 composio_langchain-0.2.0/setup.py
```

### Comparing `composio_langchain-0.1.99/PKG-INFO` & `composio_langchain-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.99
+Version: 0.2.0
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.99
+Requires-Dist: composio_core===0.2.0
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.99/README.md` & `composio_langchain-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.99/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.2.0/composio_langchain/composio_tool_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,15 @@
 
         if param_type in schema_type_python_type_dict:
             signature_param_type = schema_type_python_type_dict[param_type]
         else:
             signature_param_type = pydantic_model_from_param_schema(param_schema)
 
         param_default = param_schema.get('default', fallback_values[param_type])
-        param_annotation = Annotated[signature_param_type, param_schema.get('description', 
-                                                                            param_schema.get('desc',
-                                                                                             param_title))]
+        param_annotation = signature_param_type
         param = Parameter(
             name=param_name,
             kind=Parameter.POSITIONAL_OR_KEYWORD,
             annotation=param_annotation,
             default=Parameter.empty if param_name in required_params else param_default 
         )
         is_required = param_name in required_params
```

### Comparing `composio_langchain-0.1.99/composio_langchain/pydantic_utils.py` & `composio_langchain-0.2.0/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.99/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.2.0/composio_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.99
+Version: 0.2.0
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.99
+Requires-Dist: composio_core===0.2.0
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.99/setup.py` & `composio_langchain-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.99",
+    version="0.2.0",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

