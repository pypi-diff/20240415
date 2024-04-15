# Comparing `tmp/data2rdf-2.0.0rc0.tar.gz` & `tmp/data2rdf-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc0.tar", last modified: Thu Apr 11 13:39:24 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc1.tar", last modified: Mon Apr 15 21:15:36 2024, max compression
```

## Comparing `data2rdf-2.0.0rc0.tar` & `data2rdf-2.0.0rc1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6212 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/abox_template_generation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7614 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/chowlk/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/chowlk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2610 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/chowlk/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5092 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/csv_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8035 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/excel_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16621 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/pipeline_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/qudt/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9129 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/rdf_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/input/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_csv2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_excel2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.068108 data2rdf-2.0.0rc1/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1823 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5376 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/data2rdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 21:15:36.000000 data2rdf-2.0.0rc1/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.072108 data2rdf-2.0.0rc1/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2655 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/csv_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:36.076108 data2rdf-2.0.0rc1/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-15 21:15:31.000000 data2rdf-2.0.0rc1/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc0/LICENSE` & `data2rdf-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc0/PKG-INFO` & `data2rdf-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -18,18 +18,17 @@
 Requires-Dist: chowlk-unofficial-fork==0.0.2
 Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
-Requires-Dist: python-magic==0.4.27
 Requires-Dist: rdflib<7,>=6
 Requires-Dist: requests
-Requires-Dist: tables==3.8.0
+Requires-Dist: tables<4,>=3
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: html5lib==1.1; extra == "docs"
 Requires-Dist: ipython==8.12.3; extra == "docs"
 Requires-Dist: jinja2==3.1.3; extra == "docs"
```

### Comparing `data2rdf-2.0.0rc0/README.md` & `data2rdf-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc0/data2rdf/abox_template_generation.py` & `data2rdf-2.0.0rc1/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 import os
 from pathlib import Path
 
 from rdflib import Graph, Literal, URIRef
 from rdflib.namespace import OWL, RDF, RDFS, SKOS
 
-from data2rdf.chowlk.utils import add_emmo_name_to_diagrams
-
 
 def run_chowlk(inputfile, outputfile):
     from chowlk.transformations import transform_ontology
     from chowlk.utils import read_drawio_xml
 
     logging.info(
         f"Launching chowlk for transforming the ontology: {inputfile}"
@@ -145,33 +143,25 @@
 
         # filename = pathlib.Path(self.xml_path).name
 
         # self.mod_xml_path = os.path.join(out_path, filename.replace(".xml",".mod.xml"))
         # self.ttl_path = os.path.join(out_path, filename.replace('.xml','.ttl'))
         # self.ttl_path_ns = os.path.join(out_path, filename.replace('.xml','.ns.ttl'))
 
-    def xml_conversion(self):
-        add_emmo_name_to_diagrams(self.xml_path, self.mod_xml_path)
-
     def run_chowlk(self):
         run_chowlk(self.mod_xml_path, self.ttl_path)
 
     def add_individual_labels(self):
         add_individual_labels(self.ttl_path, self.ttl_path)
 
     def change_namespace(self, ttl_path_ns, unique_uri="http://test.org#"):
         convert_abox_namespace(self.ttl_path, ttl_path_ns)
 
     def run_pipeline(self):
         try:
-            self.xml_conversion()
-        except Exception as e:
-            logging.error(e, exc_info=True)
-
-        try:
             self.run_chowlk()
         except Exception as e:
             logging.error(e, exc_info=True)
 
         try:
             self.add_individual_labels()
         except Exception as e:
```

### Comparing `data2rdf-2.0.0rc0/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc1/data2rdf/qudt/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,16 @@
-import json
+"""Data2RDF utils"""
 import tempfile
 import warnings
 from functools import lru_cache
-from typing import List, Optional, Union
+from typing import List, Optional
 
 import requests
-from pydantic import AnyUrl
 from rdflib import Graph
 
-from data2rdf.config import config
-
-
-def make_qudt_quantity(
-    oclass: str,
-    value: Union[float, int],
-    unit: Optional[str] = None,
-    iri: AnyUrl = config.base_iri,
-    separator: str = config.separator,
-    suffix: Optional[str] = None,
-) -> Graph:
-    graph = Graph()
-    if not suffix:
-        suffix = oclass.split(separator)[-1]
-    if not iri.endswith(separator):
-        prefix = iri + separator
-    else:
-        prefix = iri
-    model = {
-        "@context": {
-            "fileid": prefix,
-            "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
-            "xsd": "http://www.w3.org/2001/XMLSchema#",
-            "qudt": "http://qudt.org/schema/qudt/",
-        },
-        "@id": f"{prefix}:{suffix}",
-        "@type": oclass,
-        "qudt:value": {
-            "@type": "xsd:float",
-            "@value": value,
-        }
-        ** _check_qudt_mapping(unit),
-    }
-    graph.parse(data=json.dumps(model), format="json-ld")
-    return graph
-
 
 def _qudt_sparql(symbol: str) -> str:
     return f"""PREFIX qudt: <http://qudt.org/schema/qudt/>
     SELECT DISTINCT ?unit
         WHERE {{
             ?unit a qudt:Unit .
             {{
@@ -57,45 +20,44 @@
             {{
                 ?unit qudt:ucumCode "{symbol}"^^qudt:UCUMcs .
             }}
         }}"""
 
 
 @lru_cache
-def _get_qudt_ontology() -> requests.Response:
-    url = config.qudt_units
-    response = requests.get(url)
+def _get_qudt_ontology(qudt_iri: str) -> requests.Response:
+    response = requests.get(qudt_iri)
     if response.status_code != 200:
         raise RuntimeError(
-            f"Could not download QUDT ontology. Please check URI: {url}"
+            f"Could not download QUDT ontology. Please check URI: {qudt_iri}"
         )
     response.encoding = "utf-8"
     return response
 
 
 def _to_tempfile(content) -> str:
     with tempfile.NamedTemporaryFile(
         mode="w", suffix=".ttl", delete=False, encoding="utf-8"
     ) as tmp:
         tmp.write(content)
     return tmp.name
 
 
 @lru_cache
-def _get_qudt_graph() -> Graph:
-    response = _get_qudt_ontology()
+def _get_qudt_graph(qudt_iri: str) -> Graph:
+    response = _get_qudt_ontology(qudt_iri)
     file = _to_tempfile(response.text)
 
     graph = Graph()
     graph.parse(file, encoding="utf-8")
     return graph
 
 
-def _get_query_match(symbol: str) -> List[str]:
-    graph = _get_qudt_graph()
+def _get_query_match(symbol: str, qudt_iri: str) -> List[str]:
+    graph = _get_qudt_graph(qudt_iri)
     query = _qudt_sparql(symbol)
     return [str(row["unit"]) for row in graph.query(query)]
 
 
 def _check_qudt_mapping(symbol: Optional[str]) -> Optional[str]:
     if symbol:
         match = _get_query_match(symbol)
```

### Comparing `data2rdf-2.0.0rc0/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc1/data2rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -18,18 +18,17 @@
 Requires-Dist: chowlk-unofficial-fork==0.0.2
 Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
-Requires-Dist: python-magic==0.4.27
 Requires-Dist: rdflib<7,>=6
 Requires-Dist: requests
-Requires-Dist: tables==3.8.0
+Requires-Dist: tables<4,>=3
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: html5lib==1.1; extra == "docs"
 Requires-Dist: ipython==8.12.3; extra == "docs"
 Requires-Dist: jinja2==3.1.3; extra == "docs"
```

### Comparing `data2rdf-2.0.0rc0/data2rdf.egg-info/SOURCES.txt` & `data2rdf-2.0.0rc1/data2rdf.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 data2rdf/__init__.py
-data2rdf/abox_template_generation.py
-data2rdf/annotation_pipeline.py
 data2rdf/config.py
-data2rdf/csv_parser.py
-data2rdf/excel_parser.py
-data2rdf/mapper.py
-data2rdf/parser.py
-data2rdf/pipeline_logging.py
-data2rdf/rdf_generation.py
+data2rdf/utils.py
 data2rdf.egg-info/PKG-INFO
 data2rdf.egg-info/SOURCES.txt
 data2rdf.egg-info/dependency_links.txt
 data2rdf.egg-info/entry_points.txt
 data2rdf.egg-info/requires.txt
 data2rdf.egg-info/top_level.txt
-data2rdf/chowlk/__init__.py
-data2rdf/chowlk/utils.py
+data2rdf/models/__init__.py
+data2rdf/models/mapping.py
+data2rdf/parsers/__init__.py
+data2rdf/parsers/base.py
+data2rdf/parsers/csv.py
+data2rdf/parsers/excel.py
+data2rdf/parsers/utils.py
+data2rdf/pipelines/__init__.py
+data2rdf/pipelines/abox_scaffolding_pipeline.py
+data2rdf/pipelines/annotation_pipeline.py
 data2rdf/qudt/__init__.py
 data2rdf/qudt/utils.py
 tests/__init__.py
+tests/test_models.py
 tests/test_utils.py
 tests/csv_pipeline_test/__init__.py
-tests/csv_pipeline_test/test_abox_pipeline.py
-tests/csv_pipeline_test/test_csv2rdf.py
-tests/csv_pipeline_test/test_utils.py
+tests/csv_pipeline_test/test_parser.py
+tests/csv_pipeline_test/test_pipeline.py
 tests/csv_pipeline_test/input/__init__.py
 tests/xls_pipeline_test/__init__.py
-tests/xls_pipeline_test/test_abox_pipeline.py
-tests/xls_pipeline_test/test_excel2rdf.py
-tests/xls_pipeline_test/test_utils.py
+tests/xls_pipeline_test/test_parser.py
+tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc0/setup.cfg` & `data2rdf-2.0.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc0
+version = v2.0.0rc1
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
@@ -23,18 +23,17 @@
 	chowlk-unofficial-fork==0.0.2
 	lru-cache<1
 	openpyxl>=3,<4
 	pandas>=2,<3
 	pydantic>=2,<3
 	pydantic-settings
 	python-dotenv
-	python-magic==0.4.27
 	rdflib>=6,<7
 	requests
-	tables==3.8.0
+	tables>=3,<4
 python_requires = >=3.8
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	abox_conv = data2rdf.cli.abox_conversion:terminal
```

