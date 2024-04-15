# Comparing `tmp/ARS_Test_Runner-0.1.7.tar.gz` & `tmp/ARS_Test_Runner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARS_Test_Runner-0.1.7.tar", last modified: Tue Apr  2 14:39:17 2024, max compression
+gzip compressed data, was "ARS_Test_Runner-0.1.8.tar", last modified: Mon Apr 15 17:42:22 2024, max compression
```

## Comparing `ARS_Test_Runner-0.1.7.tar` & `ARS_Test_Runner-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.380583 ARS_Test_Runner-0.1.7/
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.374280 ARS_Test_Runner-0.1.7/ARS_Test_Runner/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/__init__.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/cli.py
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22705 2024-04-02 14:39:05.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/semantic_test.py
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.379033 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/affects_creative.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/treats.json
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/treats_creative.json
-drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-02 14:39:17.379877 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-02 14:39:17.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/SOURCES.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/dependency_links.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/entry_points.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/requires.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-02 14:39:16.000000 ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/top_level.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.7/LICENSE.txt
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-02 14:39:17.380354 ARS_Test_Runner-0.1.7/PKG-INFO
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.7/README.md
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-02 14:39:17.381156 ARS_Test_Runner-0.1.7/setup.cfg
--rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-02 14:39:05.000000 ARS_Test_Runner-0.1.7/setup.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 17:42:22.154117 ARS_Test_Runner-0.1.8/
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 17:42:22.147570 ARS_Test_Runner-0.1.8/ARS_Test_Runner/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/__init__.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2491 2024-03-22 17:57:09.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/cli.py
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)    22714 2024-04-15 17:39:47.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/semantic_test.py
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 17:42:22.152666 ARS_Test_Runner-0.1.8/ARS_Test_Runner/templates/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1395 2024-03-05 18:23:27.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/templates/affects_creative.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      465 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/templates/treats.json
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      505 2024-03-05 18:16:02.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner/templates/treats_creative.json
+drwxr-xr-x   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        0 2024-04-15 17:42:22.153349 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      493 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/SOURCES.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)        1 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/dependency_links.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       61 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/entry_points.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       66 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/requires.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)       16 2024-04-15 17:42:21.000000 ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/top_level.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1074 2023-09-29 16:32:08.000000 ARS_Test_Runner-0.1.8/LICENSE.txt
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     3381 2024-04-15 17:42:22.153901 ARS_Test_Runner-0.1.8/PKG-INFO
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     2711 2024-03-22 18:00:24.000000 ARS_Test_Runner-0.1.8/README.md
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)      219 2024-04-15 17:42:22.154696 ARS_Test_Runner-0.1.8/setup.cfg
+-rw-r--r--   0 abdollahis2 (2089954540) NIH\Domain Users (1360859114)     1569 2024-04-15 17:41:09.000000 ARS_Test_Runner-0.1.8/setup.py
```

### Comparing `ARS_Test_Runner-0.1.7/ARS_Test_Runner/cli.py` & `ARS_Test_Runner-0.1.8/ARS_Test_Runner/cli.py`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.7/ARS_Test_Runner/semantic_test.py` & `ARS_Test_Runner-0.1.8/ARS_Test_Runner/semantic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             else:
                 if input_category == 'biolink:Gene':
                     nodes['ON']['ids'].append(input_curie)
                     del nodes['SN']['ids']
                     edges['t_edge']['qualifier_constraints'][0]['qualifier_set'][0]['qualifier_value'] = biolink_object_aspect_qualifier
                     edges['t_edge']['qualifier_constraints'][0]['qualifier_set'][1]['qualifier_value'] = biolink_object_direction_qualifier
 
-                elif input_category == 'biolink:Chemical':
+                elif input_category == 'biolink:ChemicalEntity':
                     nodes['SN']['ids'].append(input_curie)
                     del nodes['ON']['ids']
                     edges['t_edge']['qualifier_constraints'][0]['qualifier_set'][0]['qualifier_value'] = biolink_object_aspect_qualifier
                     edges['t_edge']['qualifier_constraints'][0]['qualifier_set'][1]['qualifier_value'] = biolink_object_direction_qualifier
                 else:
                     query = {"error": f"unsupported input category provided: {input_category}"}
     else:
@@ -117,16 +117,16 @@
         creative = True
     logging.debug("Generating query message for %s in creative %s mode" % (input_curie, creative))
     message = generate_message(predicate, creative, input_curie,biolink_object_aspect_qualifier, biolink_object_direction_qualifier, input_category)
     logging.debug("query= " + json.dumps(message, indent=4, sort_keys=True))
 
     if 'error' in message.keys():
         report_card={}
-        report_card['pk']={}
-        report_card['results']=message
+        report_card['pks']={}
+        report_card['results']=[message]
     else:
         children, parent_pk = await get_children(message, ARS_URL, output_curie)
         if children[0][0] == 'ars-default-agent' and 'error' in children[0][1].keys():
             report_card={}
             report_card['pks']={}
             report_card['results']=[]
             for child in children:
```

### Comparing `ARS_Test_Runner-0.1.7/ARS_Test_Runner/templates/affects_creative.json` & `ARS_Test_Runner-0.1.8/ARS_Test_Runner/templates/affects_creative.json`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.7/ARS_Test_Runner.egg-info/PKG-INFO` & `ARS_Test_Runner-0.1.8/ARS_Test_Runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS-Test-Runner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.7/LICENSE.txt` & `ARS_Test_Runner-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.7/PKG-INFO` & `ARS_Test_Runner-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARS_Test_Runner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for ARS pass/fail test
 Home-page: https://github.com/NCATSTranslator/ARS_Test_Runner
 Author: Shervin Abdollahi, Mark Williams
 Author-email: shervin.abdollahi@Nih.gov, mark.williams5@nih.gov
 License: Public Domain
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ARS_Test_Runner-0.1.7/README.md` & `ARS_Test_Runner-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ARS_Test_Runner-0.1.7/setup.py` & `ARS_Test_Runner-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from semantic_release import setup_hook
     setup_hook(sys.argv)
 except ImportError:
     pass
 
-__version__='0.1.7'
+__version__='0.1.8'
 setup(
     name="ARS_Test_Runner",
     version= __version__,
     description="Python package for ARS pass/fail test",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Shervin Abdollahi, Mark Williams",
```

