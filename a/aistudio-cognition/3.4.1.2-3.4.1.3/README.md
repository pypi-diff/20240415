# Comparing `tmp/aistudio_cognition-3.4.1.2.tar.gz` & `tmp/aistudio_cognition-3.4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aistudio_cognition-3.4.1.2.tar", max compression
+gzip compressed data, was "aistudio_cognition-3.4.1.3.tar", max compression
```

## Comparing `aistudio_cognition-3.4.1.2.tar` & `aistudio_cognition-3.4.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16056 2024-03-15 10:12:55.618156 aistudio_cognition-3.4.1.2/aistudio_cognition/cognibot/models.py
--rw-r--r--   0        0        0       46 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/models/__init__.py
--rw-r--r--   0        0        0      141 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/models/response_status.py
--rw-r--r--   0        0        0       82 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/__init__.py
--rw-r--r--   0        0        0     7059 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/luis.py
--rw-r--r--   0        0        0       47 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/models/__init__.py
--rw-r--r--   0        0        0      467 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/models/luis_settings.py
--rw-r--r--   0        0        0     2830 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/prediction.py
--rw-r--r--   0        0        0     5207 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/rule.py
--rw-r--r--   0        0        0      674 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/models.py
--rw-r--r--   0        0        0      357 2024-03-15 09:47:02.750076 aistudio_cognition-3.4.1.2/pyproject.toml
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 aistudio_cognition-3.4.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16094 2024-04-15 05:33:15.163792 aistudio_cognition-3.4.1.3/aistudio_cognition/cognibot/models.py
+-rw-r--r--   0        0        0       46 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/models/__init__.py
+-rw-r--r--   0        0        0      141 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/models/response_status.py
+-rw-r--r--   0        0        0       82 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/__init__.py
+-rw-r--r--   0        0        0     7059 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/luis.py
+-rw-r--r--   0        0        0       47 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/models/__init__.py
+-rw-r--r--   0        0        0      467 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/models/luis_settings.py
+-rw-r--r--   0        0        0     2830 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/prediction.py
+-rw-r--r--   0        0        0     5207 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/rule.py
+-rw-r--r--   0        0        0      674 2024-03-15 08:14:34.225844 aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/models.py
+-rw-r--r--   0        0        0      357 2024-04-15 05:33:15.163792 aistudio_cognition-3.4.1.3/pyproject.toml
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 aistudio_cognition-3.4.1.3/PKG-INFO
```

### Comparing `aistudio_cognition-3.4.1.2/aistudio_cognition/cognibot/models.py` & `aistudio_cognition-3.4.1.3/aistudio_cognition/cognibot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     TIME = "time"
 
 
 class CardType(Enum):
     HERO = "Hero"
     ADAPTIVE = "Adaptive"
     ADAPTIVE_LIST = "Adaptive List"
+    WHATSAPP_FLOWS = "WhatsApp Flows"
 
 
 class ActionType(Enum):
     PYTHON = "python"
     AE_WORKFLOW = "ae_workflow"
```

### Comparing `aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/luis.py` & `aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/luis.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/prediction.py` & `aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/prediction.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/luis/rule.py` & `aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/luis/rule.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.4.1.2/aistudio_cognition/nlu/models.py` & `aistudio_cognition-3.4.1.3/aistudio_cognition/nlu/models.py`

 * *Files identical despite different names*

### Comparing `aistudio_cognition-3.4.1.2/PKG-INFO` & `aistudio_cognition-3.4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistudio-cognition
-Version: 3.4.1.2
+Version: 3.4.1.3
 Summary: NLU and KM prediction utility for AIStudio
 Author: Ankita Nair
 Author-email: ankita.nair@automationedge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

