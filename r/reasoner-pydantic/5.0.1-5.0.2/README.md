# Comparing `tmp/reasoner-pydantic-5.0.1.tar.gz` & `tmp/reasoner-pydantic-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-5.0.1.tar", last modified: Fri Apr 12 19:37:00 2024, max compression
+gzip compressed data, was "reasoner-pydantic-5.0.2.tar", last modified: Mon Apr 15 16:09:00 2024, max compression
```

## Comparing `reasoner-pydantic-5.0.1.tar` & `reasoner-pydantic-5.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.353155 reasoner-pydantic-5.0.1/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.353155 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.658257 reasoner-pydantic-5.0.2/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 16:09:00.000000 reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:09:00.662257 reasoner-pydantic-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 16:08:57.000000 reasoner-pydantic-5.0.2/setup.py
```

### Comparing `reasoner-pydantic-5.0.1/PKG-INFO` & `reasoner-pydantic-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.1
+Version: 5.0.2
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.1/README.md` & `reasoner-pydantic-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/__init__.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/base_model.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/message.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/metakg.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/qgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     categories: Optional[HashableSequence[BiolinkEntity]] = Field(
         None,
         title="categories",
         nullable=True,
     )
     _nonzero_categories = validator("categories", allow_reuse=True)(nonzero_validator)
 
-    set_interpretation: Optional[SetInterpretationEnum] = Field(None, nullable=True)
+    set_interpretation: Optional[SetInterpretationEnum] = Field("BATCH", nullable=True)
     constraints: Optional[HashableSequence[AttributeConstraint]] = Field(
         default=HashableSequence[AttributeConstraint](__root__=[]),
         title="attribute constraints",
     )
 
     class Config:
         title = "query-graph node"
```

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/results.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/shared.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/utils.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic/workflow.py` & `reasoner-pydantic-5.0.2/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.1
+Version: 5.0.2
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-5.0.2/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.1/setup.py` & `reasoner-pydantic-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="5.0.1",
+    version="5.0.2",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

