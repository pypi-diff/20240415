# Comparing `tmp/pynfe_xml2dict-0.0.2.tar.gz` & `tmp/pynfe_xml2dict-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynfe_xml2dict-0.0.2.tar", max compression
+gzip compressed data, was "pynfe_xml2dict-0.0.3.tar", max compression
```

## Comparing `pynfe_xml2dict-0.0.2.tar` & `pynfe_xml2dict-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       92 2024-04-15 14:30:20.395539 pynfe_xml2dict-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/cte/__init__.py
--rw-r--r--   0        0        0       25 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/cte/index.py
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfce/__init__.py
--rw-r--r--   0        0        0      160 2024-04-15 19:05:03.581897 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-15 18:32:14.713733 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_dest__.py
--rw-r--r--   0        0        0     2704 2024-04-15 14:48:41.674789 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_det__.py
--rw-r--r--   0        0        0     1569 2024-04-15 14:48:16.866926 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_emit__.py
--rw-r--r--   0        0        0     1453 2024-04-15 14:48:22.890893 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_ide__.py
--rw-r--r--   0        0        0     2108 2024-04-15 19:05:36.297523 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/ler_nfe.py
--rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfse/__init__.py
--rw-r--r--   0        0        0       26 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfse/index.py
--rw-r--r--   0        0        0      178 2024-04-15 14:42:39.400938 pynfe_xml2dict-0.0.2/pynfe_xml2dict/utils/__init__.py
--rw-r--r--   0        0        0     4087 2024-04-15 14:41:41.869318 pynfe_xml2dict-0.0.2/pynfe_xml2dict/utils/functions.py
--rw-r--r--   0        0        0      491 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.2/pynfe_xml2dict/utils/read_xml.py
--rw-r--r--   0        0        0      461 2024-04-15 19:58:03.523152 pynfe_xml2dict-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 pynfe_xml2dict-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2024-04-15 14:30:20.395539 pynfe_xml2dict-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 21:28:14.047643 pynfe_xml2dict-0.0.3/pynfe_xml2dict/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/cte/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/cte/index.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfce/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-15 21:31:42.855707 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-15 18:32:14.713733 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_dest__.py
+-rw-r--r--   0        0        0     2704 2024-04-15 14:48:41.674789 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_det__.py
+-rw-r--r--   0        0        0     1569 2024-04-15 14:48:16.866926 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_emit__.py
+-rw-r--r--   0        0        0     1468 2024-04-15 21:30:43.580809 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_ide__.py
+-rw-r--r--   0        0        0     2126 2024-04-15 21:31:25.180035 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/ler_nfe.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfse/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfse/index.py
+-rw-r--r--   0        0        0      178 2024-04-15 14:42:39.400938 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/__init__.py
+-rw-r--r--   0        0        0     4087 2024-04-15 14:41:41.869318 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/functions.py
+-rw-r--r--   0        0        0      491 2024-04-15 14:00:19.622087 pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/read_xml.py
+-rw-r--r--   0        0        0      461 2024-04-15 21:32:18.827617 pynfe_xml2dict-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 pynfe_xml2dict-0.0.3/PKG-INFO
```

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_dest__.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_dest__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_det__.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_det__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_emit__.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_emit__.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/__tag_ide__.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/__tag_ide__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 dirNameSrc = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..')
 sys.path.append(dirNameSrc)
 
-from utils.functions import returnDataInDictOrArray, treatsFieldAsNumber
+from pynfe_xml2dict.utils.functions import returnDataInDictOrArray, treatsFieldAsNumber
 from typing import Dict
 
 
 class TagIde():
     def __init__(self, dataTagIde: dict):
         self.__dataTagIde = dataTagIde
         self.__objIde: Dict[str, str] = {}
```

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/nfe/ler_nfe.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/nfe/ler_nfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union, Dict
 
-from utils.functions import returnDataInDictOrArray
-from utils.read_xml import readXml
-from nfe.__tag_ide__ import TagIde
-from nfe.__tag_emit__ import TagEmit
-from nfe.__tag_dest__ import TagDest
-from nfe.__tag_det__ import TagDet
+from pynfe_xml2dict.utils.functions import returnDataInDictOrArray
+from pynfe_xml2dict.utils.read_xml import readXml
+from .__tag_ide__ import TagIde
+from .__tag_emit__ import TagEmit
+from .__tag_dest__ import TagDest
+from .__tag_det__ import TagDet
 
 
 class LerNfe():
     def __init__(self, pathXml: str):
         self.__dataXml = readXml(pathXml)
         self.__objNf: Dict['str', dict] = {}
```

### Comparing `pynfe_xml2dict-0.0.2/pynfe_xml2dict/utils/functions.py` & `pynfe_xml2dict-0.0.3/pynfe_xml2dict/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pynfe_xml2dict-0.0.2/PKG-INFO` & `pynfe_xml2dict-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynfe_xml2dict
-Version: 0.0.2
+Version: 0.0.3
 Summary: Leitura de XML referente a notas fiscais NF-e, NFC-e e CT-e para dicionário
 License: MIT
 Keywords: python,nfe,xml
 Author: ElderVivot
 Author-email: eldervivot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

