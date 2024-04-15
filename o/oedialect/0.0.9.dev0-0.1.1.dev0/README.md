# Comparing `tmp/oedialect-0.0.9.dev0.tar.gz` & `tmp/oedialect-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oedialect-0.0.9.dev0.tar", last modified: Wed May  6 15:12:41 2020, max compression
+gzip compressed data, was "oedialect-0.1.1.dev0.tar", last modified: Mon Apr 15 13:57:46 2024, max compression
```

## Comparing `oedialect-0.0.9.dev0.tar` & `oedialect-0.1.1.dev0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 glauer    (1000) glauer    (1000)        0 2020-05-06 15:12:41.897964 oedialect-0.0.9.dev0/
--rw-r--r--   0 glauer    (1000) glauer    (1000)     1732 2020-05-06 15:12:41.901297 oedialect-0.0.9.dev0/PKG-INFO
--rw-r--r--   0 glauer    (1000) glauer    (1000)     1152 2020-04-01 12:22:22.000000 oedialect-0.0.9.dev0/README.md
-drwxr-xr-x   0 glauer    (1000) glauer    (1000)        0 2020-05-06 15:12:41.897964 oedialect-0.0.9.dev0/oedialect/
--rw-r--r--   0 glauer    (1000) glauer    (1000)      140 2020-04-15 17:59:25.000000 oedialect-0.0.9.dev0/oedialect/__init__.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)    40075 2020-05-04 09:33:55.000000 oedialect-0.0.9.dev0/oedialect/compiler.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)      234 2020-04-15 17:59:25.000000 oedialect-0.0.9.dev0/oedialect/dbapi.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)    17579 2020-04-22 16:33:11.000000 oedialect-0.0.9.dev0/oedialect/dialect.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)    11995 2020-04-22 16:33:11.000000 oedialect-0.0.9.dev0/oedialect/engine.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)      140 2020-04-15 17:59:25.000000 oedialect-0.0.9.dev0/oedialect/error.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)      512 2020-04-15 17:59:25.000000 oedialect-0.0.9.dev0/oedialect/requirements.py
-drwxr-xr-x   0 glauer    (1000) glauer    (1000)        0 2020-05-06 15:12:41.897964 oedialect-0.0.9.dev0/oedialect.egg-info/
--rw-r--r--   0 glauer    (1000) glauer    (1000)     1732 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/PKG-INFO
--rw-r--r--   0 glauer    (1000) glauer    (1000)      436 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/SOURCES.txt
--rw-r--r--   0 glauer    (1000) glauer    (1000)        1 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/dependency_links.txt
--rw-r--r--   0 glauer    (1000) glauer    (1000)       72 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/entry_points.txt
--rw-r--r--   0 glauer    (1000) glauer    (1000)       91 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/requires.txt
--rw-r--r--   0 glauer    (1000) glauer    (1000)     1460 2020-04-23 15:05:58.000000 oedialect-0.0.9.dev0/oedialect.egg-info/test.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)       10 2020-05-06 15:12:41.000000 oedialect-0.0.9.dev0/oedialect.egg-info/top_level.txt
--rw-r--r--   0 glauer    (1000) glauer    (1000)      348 2020-05-06 15:12:41.901297 oedialect-0.0.9.dev0/setup.cfg
--rw-r--r--   0 glauer    (1000) glauer    (1000)      903 2020-05-06 15:11:41.000000 oedialect-0.0.9.dev0/setup.py
-drwxr-xr-x   0 glauer    (1000) glauer    (1000)        0 2020-05-06 15:12:41.897964 oedialect-0.0.9.dev0/test/
--rw-r--r--   0 glauer    (1000) glauer    (1000)     1812 2020-04-01 11:23:01.000000 oedialect-0.0.9.dev0/test/test.py
--rw-r--r--   0 glauer    (1000) glauer    (1000)      496 2020-04-15 17:59:25.000000 oedialect-0.0.9.dev0/test/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:57:46.467357 oedialect-0.1.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-15 13:57:46.463358 oedialect-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:57:46.463358 oedialect-0.1.1.dev0/oedialect/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40313 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17665 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/oedialect/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:57:46.463358 oedialect-0.1.1.dev0/oedialect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:57:46.000000 oedialect-0.1.1.dev0/oedialect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 13:57:46.467357 oedialect-0.1.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:57:46.463358 oedialect-0.1.1.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-15 13:57:42.000000 oedialect-0.1.1.dev0/test/test_suite.py
```

### Comparing `oedialect-0.0.9.dev0/PKG-INFO` & `oedialect-0.1.1.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,66 @@
 Metadata-Version: 2.1
 Name: oedialect
-Version: 0.0.9.dev0
+Version: 0.1.1.dev0
 Summary: SQL-Alchemy dialect for the OpenEnergy Platform
 Home-page: https://github.com/openego/oedialect
 Author: MGlauer
 Author-email: martinglauer89@gmail.com
-License: UNKNOWN
-Description: ﻿<a href="http://oep.iks.cs.ovgu.de/"><img align="right" width="200" height="200" src="https://avatars2.githubusercontent.com/u/37101913?s=400&u=9b593cfdb6048a05ea6e72d333169a65e7c922be&v=4" alt="OpenEnergyPlatform"></a>
-        
-        # An [SQLAlchemy][0] [Dialect][1] for the [OEP][2]
-        
-        SQLAlchemy internally uses so called "dialects" to provide a consistent
-        interface to different database drivers. The `oedialect` supplies your
-        SQLAlchemy installation with a dialect using the REST-API of the [Open
-        Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
-        SQLAlchemy to down- and upload data to an OEP instance.
-        
-        [0]: https://www.sqlalchemy.org/
-        [1]: https://docs.sqlalchemy.org/en/13/dialects/
-        [2]: https://github.com/OpenEnergyPlatform/oeplatform
-        
-        ## License / Copyright
-        
-        This repository is licensed under [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)
-        
-        ## Installation
-        
-        `pip install oedialect`
-        
-        On MS-Windows make sure to install a version of `shapely` first.
-        `conda install shapely -c conda-forge`
-        
-        ## Example
-        
-        You can find a basic example [here](doc/example/oedialect_basic_example.ipynb).
-        
 Keywords: postgres,open,energy,database,sql,rest
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sqlalchemy>=1.3.16
+Requires-Dist: requests>=2.13
+Requires-Dist: psycopg2-binary
+Requires-Dist: geoalchemy2<0.7.0
+Requires-Dist: shapely
+Requires-Dist: python-dateutil
+Provides-Extra: tests
+Requires-Dist: black; extra == "tests"
+Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest==5.3; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Requires-Dist: sqlahelper; extra == "tests"
+Requires-Dist: geojson; extra == "tests"
+
+﻿<a href="http://oep.iks.cs.ovgu.de/"><img align="right" width="200" height="200" src="https://avatars2.githubusercontent.com/u/37101913?s=400&u=9b593cfdb6048a05ea6e72d333169a65e7c922be&v=4" alt="OpenEnergyPlatform"></a>
+
+# An [SQLAlchemy][0] [Dialect][1] for the [OEP][2]
+
+SQLAlchemy internally uses so called "dialects" to provide a consistent
+interface to different database drivers. The `oedialect` supplies your
+SQLAlchemy installation with a dialect using the REST-API of the [Open
+Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
+SQLAlchemy to down- and upload data to an OEP instance.
+
+[0]: https://www.sqlalchemy.org/
+[1]: https://docs.sqlalchemy.org/en/13/dialects/
+[2]: https://github.com/OpenEnergyPlatform/oeplatform
+
+## License / Copyright
+
+This repository is licensed under [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+
+## Installation
+
+`pip install oedialect`
+
+On MS-Windows make sure to install a version of `shapely` first.
+`conda install shapely -c conda-forge`
+
+## Tutorials
+
+You can find tutorials and examples [here](https://github.com/OpenEnergyPlatform/examples/tree/master/api).
+
+
+## Testing
+
+To run the tests locally, first install the `tox` test environment
+`pip install tox`
+
+You need to setup a local instance of the [Open Energy Platform](https://github.com/OpenEnergyPlatform/oeplatform)
+
+Set your connection token that you got from your local OEP instance
+`LOCAL_OEP_TOKEN=<your_token>`
+
+Finally, run
+`tox`
```

#### html2text {}

```diff
@@ -1,18 +1,28 @@
-Metadata-Version: 2.1 Name: oedialect Version: 0.0.9.dev0 Summary: SQL-Alchemy
+Metadata-Version: 2.1 Name: oedialect Version: 0.1.1.dev0 Summary: SQL-Alchemy
 dialect for the OpenEnergy Platform Home-page: https://github.com/openego/
-oedialect Author: MGlauer Author-email: martinglauer89@gmail.com License:
-UNKNOWN Description: ï»¿_[_O_p_e_n_E_n_e_r_g_y_P_l_a_t_f_o_r_m_] # An [SQLAlchemy][0] [Dialect][1]
-for the [OEP][2] SQLAlchemy internally uses so called "dialects" to provide a
+oedialect Author: MGlauer Author-email: martinglauer89@gmail.com Keywords:
+postgres,open,energy,database,sql,rest Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: sqlalchemy>=1.3.16 Requires-Dist:
+requests>=2.13 Requires-Dist: psycopg2-binary Requires-Dist: geoalchemy2<0.7.0
+Requires-Dist: shapely Requires-Dist: python-dateutil Provides-Extra: tests
+Requires-Dist: black; extra == "tests" Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest==5.3; extra == "tests" Requires-Dist: pandas; extra ==
+"tests" Requires-Dist: sqlahelper; extra == "tests" Requires-Dist: geojson;
+extra == "tests" ï»¿_[_O_p_e_n_E_n_e_r_g_y_P_l_a_t_f_o_r_m_] # An [SQLAlchemy][0] [Dialect][1] for
+the [OEP][2] SQLAlchemy internally uses so called "dialects" to provide a
 consistent interface to different database drivers. The `oedialect` supplies
 your SQLAlchemy installation with a dialect using the REST-API of the [Open
 Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
 SQLAlchemy to down- and upload data to an OEP instance. [0]: https://
 www.sqlalchemy.org/ [1]: https://docs.sqlalchemy.org/en/13/dialects/ [2]:
 https://github.com/OpenEnergyPlatform/oeplatform ## License / Copyright This
 repository is licensed under [GNU Affero General Public License v3.0 (AGPL-
 3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html) ## Installation `pip
 install oedialect` On MS-Windows make sure to install a version of `shapely`
-first. `conda install shapely -c conda-forge` ## Example You can find a basic
-example [here](doc/example/oedialect_basic_example.ipynb). Keywords:
-postgres,open,energy,database,sql,rest Platform: UNKNOWN Description-Content-
-Type: text/markdown
+first. `conda install shapely -c conda-forge` ## Tutorials You can find
+tutorials and examples [here](https://github.com/OpenEnergyPlatform/examples/
+tree/master/api). ## Testing To run the tests locally, first install the `tox`
+test environment `pip install tox` You need to setup a local instance of the
+[Open Energy Platform](https://github.com/OpenEnergyPlatform/oeplatform) Set
+your connection token that you got from your local OEP instance
+`LOCAL_OEP_TOKEN=` Finally, run `tox`
```

### Comparing `oedialect-0.0.9.dev0/README.md` & `oedialect-0.1.1.dev0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -19,10 +19,24 @@
 ## Installation
 
 `pip install oedialect`
 
 On MS-Windows make sure to install a version of `shapely` first.
 `conda install shapely -c conda-forge`
 
-## Example
+## Tutorials
 
-You can find a basic example [here](doc/example/oedialect_basic_example.ipynb).
+You can find tutorials and examples [here](https://github.com/OpenEnergyPlatform/examples/tree/master/api).
+
+
+## Testing
+
+To run the tests locally, first install the `tox` test environment
+`pip install tox`
+
+You need to setup a local instance of the [Open Energy Platform](https://github.com/OpenEnergyPlatform/oeplatform)
+
+Set your connection token that you got from your local OEP instance
+`LOCAL_OEP_TOKEN=<your_token>`
+
+Finally, run
+`tox`
```

#### html2text {}

```diff
@@ -5,9 +5,13 @@
 Platform (OEP)][2]. In short, the `oedialect` allows you to use SQLAlchemy to
 down- and upload data to an OEP instance. [0]: https://www.sqlalchemy.org/ [1]:
 https://docs.sqlalchemy.org/en/13/dialects/ [2]: https://github.com/
 OpenEnergyPlatform/oeplatform ## License / Copyright This repository is
 licensed under [GNU Affero General Public License v3.0 (AGPL-3.0)](https://
 www.gnu.org/licenses/agpl-3.0.en.html) ## Installation `pip install oedialect`
 On MS-Windows make sure to install a version of `shapely` first. `conda install
-shapely -c conda-forge` ## Example You can find a basic example [here](doc/
-example/oedialect_basic_example.ipynb).
+shapely -c conda-forge` ## Tutorials You can find tutorials and examples [here]
+(https://github.com/OpenEnergyPlatform/examples/tree/master/api). ## Testing To
+run the tests locally, first install the `tox` test environment `pip install
+tox` You need to setup a local instance of the [Open Energy Platform](https://
+github.com/OpenEnergyPlatform/oeplatform) Set your connection token that you
+got from your local OEP instance `LOCAL_OEP_TOKEN=` Finally, run `tox`
```

### Comparing `oedialect-0.0.9.dev0/oedialect/compiler.py` & `oedialect-0.1.1.dev0/oedialect/compiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,95 @@
-from sqlalchemy.dialects.postgresql.base import PGExecutionContext, \
-    PGDDLCompiler
-from sqlalchemy.sql import crud, selectable, util, elements, compiler, \
-    functions, operators, expression
+from sqlalchemy.dialects.postgresql.base import (
+    PGExecutionContext,
+    PGDDLCompiler,
+    PGTypeCompiler,
+)
+from sqlalchemy.sql import (
+    crud,
+    selectable,
+    util,
+    elements,
+    compiler,
+    functions,
+    operators,
+    expression,
+)
 from sqlalchemy import exc
 from sqlalchemy.sql.annotation import Annotated
-from sqlalchemy.sql.compiler import RESERVED_WORDS, LEGAL_CHARACTERS, \
-    ILLEGAL_INITIAL_CHARACTERS, BIND_PARAMS, \
-    BIND_PARAMS_ESC, OPERATORS, BIND_TEMPLATES, FUNCTIONS, EXTRACT_MAP, \
-    COMPOUND_KEYWORDS
+from sqlalchemy.sql.compiler import (
+    RESERVED_WORDS,
+    LEGAL_CHARACTERS,
+    ILLEGAL_INITIAL_CHARACTERS,
+    BIND_PARAMS,
+    BIND_PARAMS_ESC,
+    OPERATORS,
+    BIND_TEMPLATES,
+    FUNCTIONS,
+    EXTRACT_MAP,
+    COMPOUND_KEYWORDS,
+)
 from sqlalchemy.dialects import postgresql
+from geoalchemy2.elements import WKBElement
+from sqlalchemy.ext.compiler import compiles
+import json
 
 from oedialect import error
 
-DEFAULT_SCHEMA = 'sandbox'
+DEFAULT_SCHEMA = "sandbox"
 
-class OEDDLCompiler(PGDDLCompiler):
 
+class OEDDLCompiler(PGDDLCompiler):
     def __str__(self):
-        return ''
+        return ""
 
     def visit_create_table(self, create):
-        jsn = {'request_type': 'put', 'command': 'schema/{schema}/tables/{table}/'.format(
-            schema=create.element.schema if create.element.schema else DEFAULT_SCHEMA,
-            table=create.element.name
-        )}
+        jsn = {
+            "request_type": "put",
+            "command": "schema/{schema}/tables/{table}/".format(
+                schema=create.element.schema
+                if create.element.schema
+                else DEFAULT_SCHEMA,
+                table=create.element.name,
+            ),
+        }
 
         # if only one primary key, specify it along with the column
         first_pk = False
         cols = []
         for create_column in create.columns:
             column = create_column.element
             cd = {
-                'name': column.name,
-                'is_nullable': column.nullable,
-                'data_type': self.type_compiler.process(column.type),
-                'primary_key': column.primary_key,
-                'autoincrement': column.autoincrement,
+                "name": column.name,
+                "is_nullable": column.nullable,
+                "data_type": self.type_compiler.process(column.type),
+                "primary_key": column.primary_key,
+                "autoincrement": column.autoincrement,
             }
-            #cd['character_maximum_length'] = column.type.elsize
-            cd['foreign_key'] = []
+            # cd['character_maximum_length'] = column.type.elsize
+            cd["foreign_key"] = []
             for fk in column.foreign_keys:
-                cd['foreign_key'].append({
-                    'schema': fk.column.table.schema,
-                    'table': fk.column.table.name,
-                    'column': fk.column.name,
-                })
+                cd["foreign_key"].append(
+                    {
+                        "schema": fk.column.table.schema,
+                        "table": fk.column.table.name,
+                        "column": fk.column.name,
+                    }
+                )
 
             cols.append(cd)
 
-        jsn['constraints'] = self.create_table_constraints(
-                create.element, _include_foreign_key_constraints=  # noqa
-                create.include_foreign_key_constraints)
+        jsn["constraints"] = self.create_table_constraints(
+            create.element,
+            _include_foreign_key_constraints=create.include_foreign_key_constraints,  # noqa
+        )
 
-        jsn['columns'] = cols
+        if create.element.comment:
+            jsn["metadata"] = json.loads(create.element.comment)
+
+        jsn["columns"] = cols
 
         return jsn
 
     def create_table_constraints(self, table, _include_foreign_key_constraints=None):
 
         # On some DB order is significant: visit PK first, then the
         # other constraints (engine.ReflectionTest.testbasic failed on FB2)
@@ -66,1023 +99,1105 @@
 
         all_fkcs = table.foreign_key_constraints
         if _include_foreign_key_constraints is not None:
             omit_fkcs = all_fkcs.difference(_include_foreign_key_constraints)
         else:
             omit_fkcs = set()
 
-        constraints.extend([c for c in table._sorted_constraints
-                            if c is not table.primary_key and
-                            c not in omit_fkcs])
+        constraints.extend(
+            [
+                c
+                for c in table._sorted_constraints
+                if c is not table.primary_key and c not in omit_fkcs
+            ]
+        )
 
         return [
-            p for p in
-            (self.process(constraint)
+            p
+            for p in (
+                self.process(constraint)
                 for constraint in constraints
-                if (
-                    constraint._create_rule is None or
-                    constraint._create_rule(self))
+                if (constraint._create_rule is None or constraint._create_rule(self))
                 and (
-                    not self.dialect.supports_alter or
-                    not getattr(constraint, 'use_alter', False)
-            )) if p is not None
+                    not self.dialect.supports_alter
+                    or not getattr(constraint, "use_alter", False)
+                )
+            )
+            if p is not None
         ]
 
     def visit_create_sequence(self, create):
 
-        jsn = {'request_type': 'put',
-               'command': 'schema/{schema}/sequences/{seq}/'.format(
-                   schema=create.element.schema if create.element.schema else DEFAULT_SCHEMA,
-                   seq=create.element.name),
-               'requires_connection': True
-               }
-        if hasattr(create.element, 'increment') \
-                and create.element.increment is not None:
-            jsn['increment'] = create.element.increment
-        if hasattr(create.element, 'start') \
-                and create.element.start is not None:
-            jsn['start'] = create.element.start
-        if hasattr(create.element, 'minvalue') \
-                and create.element.minvalue is not None:
-            jsn['minvalue'] = create.element.minvalue
-        if hasattr(create.element, 'maxvalue') \
-                and create.element.maxvalue is not None:
-            jsn['maxvalue'] = create.element.maxvalue
-        if hasattr(create.element, 'nomaxvalue') \
-                and create.element.nominvalue is not None:
-            jsn['nominvalue'] = create.element.nominvalue
-        if hasattr(create.element, 'nomaxvalue') \
-                and create.element.nomaxvalue is not None:
-            jsn['nomaxvalue'] = create.element.nomaxvalue
-        if hasattr(create.element, 'cache') \
-                and create.element.cache is not None:
-            jsn['cache'] = create.element.cache
-        if hasattr(create.element, 'order') \
-                and create.element.order is True:
-            jsn['order'] = create.element.order
-        if hasattr(create.element, 'cycle') \
-                and create.element.cycle is not None:
-            jsn['cycle'] = create.element.cycle
-        if hasattr(create.element, 'optional') \
-                and create.element.optional is not None:
-            jsn['optional'] = create.element.optional
+        jsn = {
+            "request_type": "put",
+            "command": "schema/{schema}/sequences/{seq}/".format(
+                schema=create.element.schema
+                if create.element.schema
+                else DEFAULT_SCHEMA,
+                seq=create.element.name,
+            ),
+            "requires_connection": True,
+        }
+        if (
+            hasattr(create.element, "increment")
+            and create.element.increment is not None
+        ):
+            jsn["increment"] = create.element.increment
+        if hasattr(create.element, "start") and create.element.start is not None:
+            jsn["start"] = create.element.start
+        if hasattr(create.element, "minvalue") and create.element.minvalue is not None:
+            jsn["minvalue"] = create.element.minvalue
+        if hasattr(create.element, "maxvalue") and create.element.maxvalue is not None:
+            jsn["maxvalue"] = create.element.maxvalue
+        if (
+            hasattr(create.element, "nomaxvalue")
+            and create.element.nominvalue is not None
+        ):
+            jsn["nominvalue"] = create.element.nominvalue
+        if (
+            hasattr(create.element, "nomaxvalue")
+            and create.element.nomaxvalue is not None
+        ):
+            jsn["nomaxvalue"] = create.element.nomaxvalue
+        if hasattr(create.element, "cache") and create.element.cache is not None:
+            jsn["cache"] = create.element.cache
+        if hasattr(create.element, "order") and create.element.order is True:
+            jsn["order"] = create.element.order
+        if hasattr(create.element, "cycle") and create.element.cycle is not None:
+            jsn["cycle"] = create.element.cycle
+        if hasattr(create.element, "optional") and create.element.optional is not None:
+            jsn["optional"] = create.element.optional
 
         return jsn
 
     def visit_drop_sequence(self, drop):
-        return {'request_type': 'delete',
-               'command': 'schema/{schema}/sequences/{seq}/'.format(
-                   schema=drop.element.schema if drop.element.schema else DEFAULT_SCHEMA,
-                   seq=drop.element.name),
-               }
-
+        return {
+            "request_type": "delete",
+            "command": "schema/{schema}/sequences/{seq}/".format(
+                schema=drop.element.schema if drop.element.schema else DEFAULT_SCHEMA,
+                seq=drop.element.name,
+            ),
+        }
 
     def visit_create_column(self, create, first_pk=False):
         column = create.element
 
         if column.system:
             return None
 
-        jsn = self.get_column_specification(
-            column,
-            first_pk=first_pk
-        )
-        const = [self.process(constraint)
-                 for constraint in column.constraints]
+        jsn = self.get_column_specification(column, first_pk=first_pk)
+        const = [self.process(constraint) for constraint in column.constraints]
         if const:
             jsn["constraints"] = const
 
         return jsn
 
     def get_column_specification(self, column, **kwargs):
         jsn = {}
-        jsn['name'] = self.preparer.format_column(column)
-        jsn['type'] = self.dialect.type_compiler.process(column.type,
-                                                         type_expression=column)
+        jsn["name"] = self.preparer.format_column(column)
+        jsn["type"] = self.dialect.type_compiler.process(
+            column.type, type_expression=column
+        )
 
         default = self.get_column_default_string(column)
         if default is not None:
-            jsn['default'] = default
+            jsn["default"] = default
 
         if not column.nullable:
-            jsn['nullable'] = 'False'
+            jsn["nullable"] = "False"
 
         return jsn
 
     def visit_drop_table(self, drop):
-        jsn = {'request_type': 'delete',
-               'command': 'schema/{schema}/tables/{table}/'.format(
-                   schema=drop.element.schema if drop.element.schema
-                                              else DEFAULT_SCHEMA,
-                   table=drop.element.name)
+        jsn = {
+            "request_type": "delete",
+            "command": "schema/{schema}/tables/{table}/".format(
+                schema=drop.element.schema if drop.element.schema else DEFAULT_SCHEMA,
+                table=drop.element.name,
+            ),
         }
         return jsn
 
     def visit_create_index(self, create):
         pass
 
     def visit_primary_key_constraint(self, constraint):
         if len(constraint) == 0:
             return []
-        jsn = {'constraint_type': 'primary_key'}
+        jsn = {"constraint_type": "primary_key"}
         if constraint.name is not None:
-            jsn['name'] = self.preparer.format_constraint(constraint)
+            jsn["name"] = self.preparer.format_constraint(constraint)
 
-        jsn['columns'] = [c.name for c in (constraint.columns_autoinc_first
-                                   if constraint._implicit_generated
-                                   else constraint.columns)]
+        jsn["columns"] = [
+            c.name
+            for c in (
+                constraint.columns_autoinc_first
+                if constraint._implicit_generated
+                else constraint.columns
+            )
+        ]
 
         return jsn
 
     def visit_foreign_key_constraint(self, constraint):
         preparer = self.preparer
 
-        jsn = {'constraint_type': 'foreign_key'}
+        jsn = {"constraint_type": "foreign_key"}
         if constraint.name is not None:
-            jsn['name'] = self.preparer.format_constraint(constraint)
+            jsn["name"] = self.preparer.format_constraint(constraint)
 
         remote_table = list(constraint.elements)[0].column.table
 
-        jsn['columns'] = [f.parent.name
-                      for f in constraint.elements]
+        jsn["columns"] = [f.parent.name for f in constraint.elements]
 
-        jsn['target_table'] = self.define_constraint_remote_table(
-                constraint, remote_table, preparer)
+        jsn["target_table"] = self.define_constraint_remote_table(
+            constraint, remote_table, preparer
+        )
 
-        jsn['target_columns'] = [f.column.name
-                                 for f in constraint.elements]
+        jsn["target_columns"] = [f.column.name for f in constraint.elements]
 
-        jsn['match'] = self.define_constraint_match(constraint)
-        jsn['cascades'] = self.define_constraint_cascades(constraint)
-        jsn['deferrable'] = self.define_constraint_deferrability(constraint)
+        jsn["match"] = self.define_constraint_match(constraint)
+        jsn["cascades"] = self.define_constraint_cascades(constraint)
+        jsn["deferrable"] = self.define_constraint_deferrability(constraint)
         return jsn
 
     def visit_unique_constraint(self, constraint):
-        jsn = {'type': 'unique'}
+        jsn = {"type": "unique"}
         if constraint.name is not None:
-            jsn['name'] = self.preparer.format_constraint(constraint)
+            jsn["name"] = self.preparer.format_constraint(constraint)
 
-        jsn['columns'] = [c.name for c in constraint]
-        jsn['deferrable'] = self.define_constraint_deferrability(constraint)
+        jsn["columns"] = [c.name for c in constraint]
+        jsn["deferrable"] = self.define_constraint_deferrability(constraint)
         return jsn
 
     def visit_column_check_constraint(self, constraint):
         raise NotImplementedError
 
 
-
 class OECompiler(postgresql.psycopg2.PGCompiler):
     def __str__(self):
-        return ''
+        return ""
 
     def visit_clauselist(self, clauselist, **kw):
         sep = clauselist.operator
         clauses = [
-            s for s in
-            (
-                c._compiler_dispatch(self, **kw)
-                for c in clauselist.clauses)
-            if s]
+            s
+            for s in (c._compiler_dispatch(self, **kw) for c in clauselist.clauses)
+            if s
+        ]
 
-        if clauselist.operator == operators.and_ or clauselist.operator == operators.or_:
+        if (
+            clauselist.operator == operators.and_
+            or clauselist.operator == operators.or_
+        ):
             sep = OPERATORS[clauselist.operator]
-            clauses = {"type": "operator",
-                "operator": sep,
-                "operands": clauses}
+            clauses = {"type": "operator", "operator": sep, "operands": clauses}
 
         return clauses
 
     def visit_unary(self, unary, **kw):
         if unary.operator:
             if unary.modifier:
                 raise exc.CompileError(
                     "Unary expression does not support operator "
-                    "and modifier simultaneously")
-            disp = self._get_operator_dispatch(
-                unary.operator, "unary", "operator")
+                    "and modifier simultaneously"
+                )
+            disp = self._get_operator_dispatch(unary.operator, "unary", "operator")
             if disp:
                 return disp(unary, unary.operator, **kw)
             else:
                 return self._generate_generic_unary_operator(
-                    unary, OPERATORS[unary.operator], **kw)
+                    unary, OPERATORS[unary.operator], **kw
+                )
         elif unary.modifier:
-            disp = self._get_operator_dispatch(
-                unary.modifier, "unary", "modifier")
+            disp = self._get_operator_dispatch(unary.modifier, "unary", "modifier")
             if disp:
                 return disp(unary, unary.modifier, **kw)
             else:
                 return self._generate_generic_unary_modifier(
-                    unary, OPERATORS[unary.modifier], **kw)
+                    unary, OPERATORS[unary.modifier], **kw
+                )
         else:
-            raise exc.CompileError(
-                "Unary expression has no operator or modifier")
+            raise exc.CompileError("Unary expression has no operator or modifier")
+
+    def visit_case(self, clause, **kwargs):
+        d = dict(type="case")
+        if clause.value is not None:
+            d["expression"] = clause.value._compiler_dispatch(self, **kwargs)
+        d["cases"] = [
+            dict(
+                when=cond._compiler_dispatch(self, **kwargs),
+                then=result._compiler_dispatch(self, **kwargs),
+            )
+            for cond, result in clause.whens
+        ]
+
+        if clause.else_ is not None:
+            d["else"] = clause.else_._compiler_dispatch(self, **kwargs)
+
+        return d
 
     def visit_grouping(self, grouping, asfrom=False, **kwargs):
-        """"
+        """ "
         TODO:
         """
         return {
-            'type': 'grouping',
-            'grouping': grouping.element._compiler_dispatch(self, **kwargs)
+            "type": "grouping",
+            "grouping": grouping.element._compiler_dispatch(self, **kwargs),
         }
 
     def visit_join(self, join, asfrom=False, **kwargs):
-        d = {'type': 'join'}
+        d = {"type": "join"}
         if join.full:
-            d['join_type'] = "FULL OUTER JOIN"
+            d["join_type"] = "FULL OUTER JOIN"
         elif join.isouter:
-            d['join_type'] = "LEFT OUTER JOIN"
+            d["join_type"] = "LEFT OUTER JOIN"
         else:
-            d['join_type'] = "JOIN "
+            d["join_type"] = "JOIN "
 
-        d['left'] = join.left._compiler_dispatch(self, asfrom=True, **kwargs)
-        d['right'] = join.right._compiler_dispatch(self, asfrom=True, **kwargs)
-        d['on'] = join.onclause._compiler_dispatch(self, **kwargs)
+        d["left"] = join.left._compiler_dispatch(self, asfrom=True, **kwargs)
+        d["right"] = join.right._compiler_dispatch(self, asfrom=True, **kwargs)
+        d["on"] = join.onclause._compiler_dispatch(self, **kwargs)
         return d
 
     def bindparam_string(self, name, positional_names=None, expanding=False, **kw):
         if self.positional:
             if positional_names is not None:
                 positional_names.append(name)
             else:
                 self.positiontup.append(name)
         if expanding:
             raise NotImplementedError
             self.contains_expanding_parameters = True
             return "([EXPANDING_%s])" % name
         return lambda d: d[name]
 
+    def render_literal_value(self, value, type_):
+        return value
 
     def visit_insert(self, insert_stmt, **kw):
         self.stack.append(
-            {'correlate_froms': set(),
-             'asfrom_froms': set(),
-             'selectable': insert_stmt})
+            {"correlate_froms": set(), "asfrom_froms": set(), "selectable": insert_stmt}
+        )
 
         self.isinsert = True
         crud_params = crud._get_crud_params(self, insert_stmt, **kw)
 
-        if not crud_params and \
-                not self.dialect.supports_default_values and \
-                not self.dialect.supports_empty_insert:
-            raise exc.CompileError("The '%s' dialect with current database "
-                                   "version settings does not support empty "
-                                   "inserts." %
-                                   self.dialect.name)
+        if (
+            not crud_params
+            and not self.dialect.supports_default_values
+            and not self.dialect.supports_empty_insert
+        ):
+            raise exc.CompileError(
+                "The '%s' dialect with current database "
+                "version settings does not support empty "
+                "inserts." % self.dialect.name
+            )
 
         if insert_stmt._has_multi_parameters:
             if not self.dialect.supports_multivalues_insert:
                 raise exc.CompileError(
                     "The '%s' dialect with current database "
                     "version settings does not support "
-                    "in-place multirow inserts." %
-                    self.dialect.name)
+                    "in-place multirow inserts." % self.dialect.name
+                )
             crud_params_single = crud_params[0]
         else:
             crud_params_single = crud_params
 
         preparer = self.preparer
         supports_default_values = self.dialect.supports_default_values
 
         jsn = {"command": "advanced/insert"}
 
         if insert_stmt._prefixes:
-            text += self._generate_prefixes(insert_stmt,
-                                            insert_stmt._prefixes, **kw)
+            text += self._generate_prefixes(insert_stmt, insert_stmt._prefixes, **kw)
 
         # table_text = preparer.format_table(insert_stmt.table)
         table_text = insert_stmt.table._compiler_dispatch(
-            self, asfrom=True, iscrud=True)
+            self, asfrom=True, iscrud=True
+        )
 
         if insert_stmt._hints:
-            dialect_hints = dict([
-                                     (table, hint_text)
-                                     for (table, dialect), hint_text in
-                                     insert_stmt._hints.items()
-                                     if dialect in ('*', self.dialect.name)
-                                     ])
+            dialect_hints = dict(
+                [
+                    (table, hint_text)
+                    for (table, dialect), hint_text in insert_stmt._hints.items()
+                    if dialect in ("*", self.dialect.name)
+                ]
+            )
             if insert_stmt.table in dialect_hints:
                 table_text = self.format_from_hint_text(
                     table_text,
                     insert_stmt.table,
                     dialect_hints[insert_stmt.table],
-                    True
+                    True,
                 )
 
-        jsn['table'] = table_text['table']
+        jsn["table"] = table_text["table"]
 
-        jsn['schema'] = table_text.get('schema', DEFAULT_SCHEMA)
+        jsn["schema"] = table_text.get("schema", DEFAULT_SCHEMA)
 
         if crud_params_single or not supports_default_values:
-            jsn["fields"] = [preparer.format_column(c[0])
-                             for c in crud_params_single]
+            jsn["fields"] = [preparer.format_column(c[0]) for c in crud_params_single]
         if self.returning or insert_stmt._returning:
             self.returning = self.returning or insert_stmt._returning
-            returning_clause = self.returning_clause(
-                insert_stmt, self.returning)
+            returning_clause = self.returning_clause(insert_stmt, self.returning)
 
             if self.returning_precedes_values:
                 jsn["returning_insert"] = returning_clause
 
         if insert_stmt.select is not None:
-            jsn['values'] = self.process(self._insert_from_select, **kw)
-            jsn['method'] = 'select'
+            jsn["values"] = self.process(self._insert_from_select, **kw)
+            jsn["method"] = "select"
         elif not crud_params and supports_default_values:
-            jsn['values'] = " DEFAULT VALUES"
+            jsn["values"] = " DEFAULT VALUES"
         elif insert_stmt._has_multi_parameters:
-            jsn['values'] = [[c[1] for c in crud_param_set]
-                             for crud_param_set in crud_params]
+            jsn["values"] = [
+                [c[1] for c in crud_param_set] for crud_param_set in crud_params
+            ]
         else:
-            jsn['values'] = [[c[1] for c in crud_params]]
+            jsn["values"] = [[c[1] for c in crud_params]]
 
         if self.returning and not self.returning_precedes_values:
             jsn["returning"] = returning_clause
 
         return jsn
 
     def visit_getitem_binary(self, binary, operator, **kw):
         return {
-            'type': 'operator',
-            'operator':'getitem',
-            'operands': [
+            "type": "operator",
+            "operator": "getitem",
+            "operands": [
                 self.process(binary.left, **kw),
-                self.process(binary.right, **kw)
-            ]
+                self.process(binary.right, **kw),
+            ],
         }
 
     def visit_like_op_binary(self, binary, operator, **kw):
         return {
             "type": "operator",
             "operator": "like",
             "operands": [
                 self.process(binary.left, **kw),
                 self.process(binary.right, **kw),
             ],
         }
 
     def visit_slice(self, element, **kw):
         return {
-            'type':  'slice',
-            'start': self.process(element.start, **kw),
-            'stop':  self.process(element.stop, **kw),
+            "type": "slice",
+            "start": self.process(element.start, **kw),
+            "stop": self.process(element.stop, **kw),
         }
 
-    def visit_alias(self, alias, asfrom=False, ashint=False,
-                    iscrud=False,
-                    fromhints=None, **kwargs):
+    def visit_alias(
+        self, alias, asfrom=False, ashint=False, iscrud=False, fromhints=None, **kwargs
+    ):
 
         if asfrom or ashint:
             if isinstance(alias.name, elements._truncated_label):
                 alias_name = self._truncated_identifier("alias", alias.name)
             else:
                 alias_name = alias.name
 
         if ashint:
             return self.preparer.format_alias(alias, alias_name)
         elif asfrom:
-            ret = alias.original._compiler_dispatch(self,
-                                                    asfrom=True, **kwargs)
-            ret['alias'] = self.preparer.format_alias(alias, alias_name)
+            ret = alias.original._compiler_dispatch(self, asfrom=True, **kwargs)
+            ret["alias"] = self.preparer.format_alias(alias, alias_name)
 
             if fromhints and alias in fromhints:
-                ret = self.format_from_hint_text(ret, alias,
-                                                 fromhints[alias], iscrud)
+                ret = self.format_from_hint_text(ret, alias, fromhints[alias], iscrud)
 
             return ret
         else:
             return alias.original._compiler_dispatch(self, **kwargs)
 
     def visit_delete(self, delete_stmt, **kw):
-        self.stack.append({'correlate_froms': set([delete_stmt.table]),
-                           "asfrom_froms": set([delete_stmt.table]),
-                           "selectable": delete_stmt})
+        self.stack.append(
+            {
+                "correlate_froms": set([delete_stmt.table]),
+                "asfrom_froms": set([delete_stmt.table]),
+                "selectable": delete_stmt,
+            }
+        )
         self.isdelete = True
 
-        jsn = {'command': "advanced/delete"}
+        jsn = {"command": "advanced/delete"}
 
         if delete_stmt._prefixes:
-            text += self._generate_prefixes(delete_stmt,
-                                            delete_stmt._prefixes, **kw)
+            text += self._generate_prefixes(delete_stmt, delete_stmt._prefixes, **kw)
 
         table_text = delete_stmt.table._compiler_dispatch(
-            self, asfrom=True, iscrud=True)
+            self, asfrom=True, iscrud=True
+        )
 
         if delete_stmt._hints:
-            dialect_hints = dict([
-                                     (table, hint_text)
-                                     for (table, dialect), hint_text in
-                                     delete_stmt._hints.items()
-                                     if dialect in ('*', self.dialect.name)
-                                     ])
+            dialect_hints = dict(
+                [
+                    (table, hint_text)
+                    for (table, dialect), hint_text in delete_stmt._hints.items()
+                    if dialect in ("*", self.dialect.name)
+                ]
+            )
             if delete_stmt.table in dialect_hints:
                 table_text = self.format_from_hint_text(
                     table_text,
                     delete_stmt.table,
                     dialect_hints[delete_stmt.table],
-                    True
+                    True,
                 )
 
         else:
             dialect_hints = None
 
-        jsn['table'] = table_text['table']
+        jsn["table"] = table_text["table"]
 
-        jsn['schema'] = table_text.get('schema', DEFAULT_SCHEMA)
+        jsn["schema"] = table_text.get("schema", DEFAULT_SCHEMA)
 
         if delete_stmt._returning:
             self.returning = delete_stmt._returning
             if self.returning_precedes_values:
-                jsn['returning_delete'] = " " + self.returning_clause(
-                    delete_stmt, delete_stmt._returning)
+                jsn["returning_delete"] = " " + self.returning_clause(
+                    delete_stmt, delete_stmt._returning
+                )
 
         if delete_stmt._whereclause is not None:
             t = delete_stmt._whereclause._compiler_dispatch(self)
             if t:
-                jsn['where'] = t
+                jsn["where"] = t
 
         if self.returning and not self.returning_precedes_values:
-            jsn['returning'] = self.returning_clause(
-                delete_stmt, delete_stmt._returning)
+            jsn["returning"] = self.returning_clause(
+                delete_stmt, delete_stmt._returning
+            )
 
         self.stack.pop(-1)
 
         return jsn
 
-    def visit_table(self, table, asfrom=False, iscrud=False, ashint=False,
-                    fromhints=None, **kwargs):
+    def visit_table(
+        self, table, asfrom=False, iscrud=False, ashint=False, fromhints=None, **kwargs
+    ):
         if asfrom or ashint:
             # this is a from_item and a table
-            jsn = {'type': 'table'}
+            jsn = {"type": "table"}
             if getattr(table, "schema", None):
-                jsn['schema'] = table.schema
+                jsn["schema"] = table.schema
             else:
-                jsn['schema'] = DEFAULT_SCHEMA
+                jsn["schema"] = DEFAULT_SCHEMA
 
-            jsn['table'] = table.name
+            jsn["table"] = table.name
 
             # if fromhints and table in fromhints:
             #    ret = self.format_from_hint_text(ret, table,
             #                                     fromhints[table], iscrud)
 
             return jsn
         else:
             raise NotImplementedError("visit_table (%s)" % table.name)
             # return {}
 
-    def visit_select(self, select, asfrom=False, parens=True,
-                     fromhints=None,
-                     compound_index=0,
-                     nested_join_translation=False,
-                     select_wraps_for=None,
-                     **kwargs):
-        jsn = {'command': 'advanced/search', 'type': 'select'}
-        needs_nested_translation = \
-            select.use_labels and \
-            not nested_join_translation and \
-            not self.stack and \
-            not self.dialect.supports_right_nested_joins
+    def visit_select(
+        self,
+        select,
+        asfrom=False,
+        parens=True,
+        fromhints=None,
+        compound_index=0,
+        nested_join_translation=False,
+        select_wraps_for=None,
+        **kwargs
+    ):
+        jsn = {"command": "advanced/search", "type": "select"}
+        needs_nested_translation = (
+            select.use_labels
+            and not nested_join_translation
+            and not self.stack
+            and not self.dialect.supports_right_nested_joins
+        )
 
         if needs_nested_translation:
-            transformed_select = self._transform_select_for_nested_joins(
-                select)
+            transformed_select = self._transform_select_for_nested_joins(select)
             text = self.visit_select(
-                transformed_select, asfrom=asfrom, parens=parens,
+                transformed_select,
+                asfrom=asfrom,
+                parens=parens,
                 fromhints=fromhints,
                 compound_index=compound_index,
-                nested_join_translation=True, **kwargs
+                nested_join_translation=True,
+                **kwargs
             )
 
         toplevel = not self.stack
         entry = self._default_stack_entry if toplevel else self.stack[-1]
 
-        populate_result_map = toplevel or \
-                              (
-                                  compound_index == 0 and entry.get(
-                                      'need_result_map_for_compound', False)
-                              ) or entry.get('need_result_map_for_nested',
-                                             False)
+        populate_result_map = (
+            toplevel
+            or (
+                compound_index == 0 and entry.get("need_result_map_for_compound", False)
+            )
+            or entry.get("need_result_map_for_nested", False)
+        )
 
         # this was first proposed as part of #3372; however, it is not
         # reached in current tests and could possibly be an assertion
         # instead.
-        if not populate_result_map and 'add_to_result_map' in kwargs:
-            del kwargs['add_to_result_map']
+        if not populate_result_map and "add_to_result_map" in kwargs:
+            del kwargs["add_to_result_map"]
 
         if needs_nested_translation:
             if populate_result_map:
-                self._transform_result_map_for_nested_joins(
-                    select, transformed_select)
+                self._transform_result_map_for_nested_joins(select, transformed_select)
             return jsn
 
         froms = self._setup_select_stack(select, entry, asfrom)
 
         column_clause_args = kwargs.copy()
-        column_clause_args.update({
-            'within_label_clause': False,
-            'within_columns_clause': False
-        })
+        column_clause_args.update(
+            {"within_label_clause": False, "within_columns_clause": False}
+        )
 
         if select._hints:
             hint_text, byfrom = self._setup_select_hints(select)
             if hint_text:
                 text += hint_text + " "
         else:
             byfrom = None
 
-
         """
         if select._prefixes:
             text += self._generate_prefixes(
                 select, select._prefixes, **kwargs)
         """
         if select._distinct:
-            jsn['distinct'] = True
+            jsn["distinct"] = True
 
         # the actual list of columns to print in the SELECT column list.
         inner_columns = [
-            c for c in [
+            c
+            for c in [
                 self._label_select_column(
                     select,
                     column,
-                    populate_result_map, asfrom,
+                    populate_result_map,
+                    asfrom,
                     column_clause_args,
-                    name=name)
+                    name=name,
+                )
                 for name, column in select._columns_plus_names
-                ]
-            if c is not None
             ]
+            if c is not None
+        ]
 
         if populate_result_map and select_wraps_for is not None:
             # if this select is a compiler-generated wrapper,
             # rewrite the targeted columns in the result map
             wrapped_inner_columns = set(select_wraps_for.inner_columns)
             translate = dict(
-                (outer, inner.pop()) for outer, inner in [
-                    (
-                        outer,
-                        outer.proxy_set.intersection(wrapped_inner_columns))
+                (outer, inner.pop())
+                for outer, inner in [
+                    (outer, outer.proxy_set.intersection(wrapped_inner_columns))
                     for outer in select.inner_columns
-                    ] if inner
+                ]
+                if inner
             )
             self._result_columns = [
                 (key, name, tuple(translate.get(o, o) for o in obj), type_)
                 for key, name, obj, type_ in self._result_columns
-                ]
+            ]
 
         jsn = self._compose_select_body(
-            jsn, select, inner_columns, froms, byfrom, kwargs)
+            jsn, select, inner_columns, froms, byfrom, kwargs
+        )
 
         if select._statement_hints:
             per_dialect = [
-                ht for (dialect_name, ht)
-                in select._statement_hints
-                if dialect_name in ('*', self.dialect.name)
-                ]
+                ht
+                for (dialect_name, ht) in select._statement_hints
+                if dialect_name in ("*", self.dialect.name)
+            ]
             if per_dialect:
                 text += " " + self.get_statement_hint_text(per_dialect)
 
         if self.ctes and self._is_toplevel_select(select):
             text = self._render_cte_clause() + text
 
         if select._suffixes:
-            text += " " + self._generate_prefixes(
-                select, select._suffixes, **kwargs)
+            text += " " + self._generate_prefixes(select, select._suffixes, **kwargs)
 
         self.stack.pop(-1)
 
         if asfrom and parens:
             return jsn  # "(" + text + ")"
         else:
             return jsn
 
     def visit_update(self, update_stmt, asfrom=False, **kw):
         toplevel = not self.stack
 
         self.stack.append(
-            {'correlate_froms': set([update_stmt.table]),
-             "asfrom_froms": set([update_stmt.table]),
-             "selectable": update_stmt})
+            {
+                "correlate_froms": set([update_stmt.table]),
+                "asfrom_froms": set([update_stmt.table]),
+                "selectable": update_stmt,
+            }
+        )
 
         extra_froms = update_stmt._extra_froms
 
-        d = {'command': 'advanced/update'}
+        d = {"command": "advanced/update"}
 
-        d['table'] = update_stmt.table.name
+        d["table"] = update_stmt.table.name
         if update_stmt.table.schema:
-            d['schema'] = update_stmt.table.schema.name
+            d["schema"] = update_stmt.table.schema.name
 
+        crud_params = crud._setup_crud_params(self, update_stmt, crud.ISUPDATE, **kw)
 
-        crud_params = crud._setup_crud_params(
-            self, update_stmt, crud.ISUPDATE, **kw)
+        include_table = extra_froms and self.render_table_with_column_in_update_from
 
-        include_table = extra_froms and \
-            self.render_table_with_column_in_update_from
-
-        d['fields'] = [c[0]._compiler_dispatch(self, include_table=include_table) for c in crud_params]
-        d['values'] = [c[1] for c in crud_params]
+        d["fields"] = [
+            c[0]._compiler_dispatch(self, include_table=include_table)
+            for c in crud_params
+        ]
+        d["values"] = [c[1] for c in crud_params]
 
         if update_stmt._whereclause is not None:
             t = self.process(update_stmt._whereclause, **kw)
             if t:
-                d['where'] = t
+                d["where"] = t
 
         limit = self.update_limit_clause(update_stmt)
         if limit:
-            d['limit'] = limit
+            d["limit"] = limit
 
         return d
 
-    def visit_compound_select(self, cs, asfrom=False,
-                              parens=True, compound_index=0, **kwargs):
+    def visit_compound_select(
+        self, cs, asfrom=False, parens=True, compound_index=0, **kwargs
+    ):
         toplevel = not self.stack
 
         entry = self._default_stack_entry if toplevel else self.stack[-1]
-        need_result_map = toplevel or \
-            (compound_index == 0
-                and entry.get('need_result_map_for_compound', False))
+        need_result_map = toplevel or (
+            compound_index == 0 and entry.get("need_result_map_for_compound", False)
+        )
 
         self.stack.append(
             {
-                'correlate_froms': entry['correlate_froms'],
-                'asfrom_froms': entry['asfrom_froms'],
-                'selectable': cs,
-                'need_result_map_for_compound': need_result_map
-            })
+                "correlate_froms": entry["correlate_froms"],
+                "asfrom_froms": entry["asfrom_froms"],
+                "selectable": cs,
+                "need_result_map_for_compound": need_result_map,
+            }
+        )
 
         keyword = self.compound_keywords.get(cs.keyword)
 
-        jsn = {'keyword' : keyword,
-               'type': 'select',
-               'selects':
-                    [c._compiler_dispatch(self,
-                                          asfrom=asfrom, parens=False,
-                                          compound_index=i, **kwargs)
-                     for i, c in enumerate(cs.selects)]
-                }
+        jsn = {
+            "keyword": keyword,
+            "type": "select",
+            "selects": [
+                c._compiler_dispatch(
+                    self, asfrom=asfrom, parens=False, compound_index=i, **kwargs
+                )
+                for i, c in enumerate(cs.selects)
+            ],
+        }
 
-        group_by = cs._group_by_clause._compiler_dispatch(
-            self, asfrom=asfrom, **kwargs)
+        group_by = cs._group_by_clause._compiler_dispatch(self, asfrom=asfrom, **kwargs)
         if group_by:
-            jsn['group_by'] = group_by
+            jsn["group_by"] = group_by
 
         order_by = self.order_by_clause(cs, **kwargs)
 
         if order_by:
-            jsn['order_by'] = order_by
+            jsn["order_by"] = order_by
 
-        boundaries = (cs._limit_clause is not None
-                 or cs._offset_clause is not None) and \
-            self.limit_clause(cs, **kwargs) or ""
+        boundaries = (
+            (cs._limit_clause is not None or cs._offset_clause is not None)
+            and self.limit_clause(cs, **kwargs)
+            or ""
+        )
 
         if boundaries:
             jsn.update(boundaries)
 
-        #if self.ctes and toplevel:
+        # if self.ctes and toplevel:
         #    text = self._render_cte_clause() + text
 
         self.stack.pop(-1)
-        #if asfrom and parens:
+        # if asfrom and parens:
         #    return "(" + text + ")"
-        #else:
+        # else:
 
         if toplevel:
-            jsn['command'] = 'advanced/search'
+            jsn["command"] = "advanced/search"
 
         return jsn
 
     def visit_cast(self, cast, **kwargs):
         return {
-            'type': 'cast',
-            'source': cast.clause._compiler_dispatch(self, **kwargs),
-            'as': cast.typeclause._compiler_dispatch(self, **kwargs)}
+            "type": "cast",
+            "source": cast.clause._compiler_dispatch(self, **kwargs),
+            "as": cast.typeclause._compiler_dispatch(self, **kwargs),
+        }
 
     def visit_over(self, over, **kwargs):
         return {
-            'type': 'over',
-            'function': over.func._compiler_dispatch(self, **kwargs),
-            'clauses': [
-                {'type': word,
-                 'clause': clause._compiler_dispatch(self, **kwargs)}
+            "type": "over",
+            "function": over.func._compiler_dispatch(self, **kwargs),
+            "clauses": [
+                {"type": word, "clause": clause._compiler_dispatch(self, **kwargs)}
                 for word, clause in (
-                    ('PARTITION', over.partition_by),
-                    ('ORDER', over.order_by)
+                    ("PARTITION", over.partition_by),
+                    ("ORDER", over.order_by),
                 )
                 if clause is not None and len(clause)
-                ]}
+            ],
+        }
 
     def visit_funcfilter(self, funcfilter, **kwargs):
         return {
-            'type': 'funcfilter',
-            'function': funcfilter.func._compiler_dispatch(self, **kwargs),
-            'where': funcfilter.criterion._compiler_dispatch(self, **kwargs)
+            "type": "funcfilter",
+            "function": funcfilter.func._compiler_dispatch(self, **kwargs),
+            "where": funcfilter.criterion._compiler_dispatch(self, **kwargs),
         }
 
     def visit_extract(self, extract, **kwargs):
         field = self.extract_map.get(extract.field, extract.field)
         return {
-            'type': 'extract',
-            'field': field,
-            'expression': extract.expr._compiler_dispatch(self, **kwargs)}
-
-    def visit_label(self, label,
-                    add_to_result_map=None,
-                    within_label_clause=False,
-                    within_columns_clause=False,
-                    render_label_as_label=None,
-                    **kw):
+            "type": "extract",
+            "field": field,
+            "expression": extract.expr._compiler_dispatch(self, **kwargs),
+        }
+
+    def visit_label(
+        self,
+        label,
+        add_to_result_map=None,
+        within_label_clause=False,
+        within_columns_clause=False,
+        render_label_as_label=None,
+        **kw
+    ):
         # only render labels within the columns clause
         # or ORDER BY clause of a select.  dialect-specific compilers
         # can modify this behavior.
-        render_label_with_as = (within_columns_clause and not
-        within_label_clause)
+        render_label_with_as = within_columns_clause and not within_label_clause
         render_label_only = render_label_as_label is label
 
-        d = {'type': 'label'}
+        d = {"type": "label"}
 
         if isinstance(label.name, elements._truncated_label):
             labelname = self._truncated_identifier("colident", label.name)
         else:
             labelname = label.name
-        d['label'] = labelname
+        d["label"] = labelname
 
         if render_label_with_as:
             if add_to_result_map is not None:
                 add_to_result_map(
                     labelname,
                     label.name,
-                    (label, labelname,) + label._alt_names,
-                    label.type
+                    (label, labelname) + label._alt_names,
+                    label.type,
                 )
 
             d = {
-                'type': 'label',
-                'element': label.element._compiler_dispatch(
-                    self, within_columns_clause=True,
-                    within_label_clause=True, **kw),
-                'label': self.preparer.format_label(label, labelname)}
+                "type": "label",
+                "element": label.element._compiler_dispatch(
+                    self, within_columns_clause=True, within_label_clause=True, **kw
+                ),
+                "label": self.preparer.format_label(label, labelname),
+            }
 
-        d['element'] = label.element._compiler_dispatch(
-            self, within_columns_clause=False, **kw)
+        d["element"] = label.element._compiler_dispatch(
+            self, within_columns_clause=False, **kw
+        )
 
         return d
 
     def visit_function(self, func, add_to_result_map=None, **kwargs):
         if add_to_result_map is not None:
-            add_to_result_map(
-                func.name, func.name, (), func.type
-            )
+            add_to_result_map(func.name, func.name, (), func.type)
 
         disp = getattr(self, "visit_%s_func" % func.name.lower(), None)
         if disp:
             return disp(func, **kwargs)
         else:
             name = FUNCTIONS.get(func.__class__, func.name)
-            return {'type': 'function',
-                    'function': ".".join(list(func.packagenames) + [name]),
-                    'operands': self.function_argspec(func, **kwargs)}
+            return {
+                "type": "function",
+                "function": ".".join(list(func.packagenames) + [name]),
+                "operands": self.function_argspec(func, **kwargs),
+            }
 
-    def visit_column(self, column, add_to_result_map=None,
-                     include_table=True, **kwargs):
+    def visit_column(
+        self, column, add_to_result_map=None, include_table=True, **kwargs
+    ):
         name = orig_name = column.name
         if name is None:
-            raise exc.CompileError("Cannot compile Column object until "
-                                   "its 'name' is assigned.")
+            raise exc.CompileError(
+                "Cannot compile Column object until " "its 'name' is assigned."
+            )
 
         is_literal = column.is_literal
         if not is_literal and isinstance(name, elements._truncated_label):
             name = self._truncated_identifier("colident", name)
 
         if add_to_result_map is not None:
-            add_to_result_map(
-                name,
-                orig_name,
-                (column, name, column.key),
-                column.type
-            )
+            add_to_result_map(name, orig_name, (column, name, column.key), column.type)
 
         if is_literal:
             name = self.escape_literal_column(name)
         # else:
         #    name = self.preparer.quote(name)
-        jsn = {'type': 'column', 'column': name, 'is_literal': is_literal}
+        jsn = {"type": "column", "column": name, "is_literal": is_literal}
         table = column.table
         if table is None or not include_table or not table.named_with_column:
             return jsn
         else:
             tablename = table.name
             if isinstance(tablename, elements._truncated_label):
-                jsn['alias'] = self._truncated_identifier("alias", tablename)
+                jsn["alias"] = self._truncated_identifier("alias", tablename)
             else:
-                jsn['table'] = tablename
+                jsn["table"] = tablename
                 if table.schema:
-                    jsn['schema'] = table.schema
+                    jsn["schema"] = table.schema
                 else:
-                    jsn['schema'] = DEFAULT_SCHEMA
+                    jsn["schema"] = DEFAULT_SCHEMA
 
             return jsn
 
     def visit_null(self, expr, **kw):
         return None
 
     def _generate_generic_binary(self, binary, opstring, **kw):
-        return {'type': 'operator',
-                'operands': [binary.left._compiler_dispatch(self, **kw),
-                             binary.right._compiler_dispatch(self, **kw)],
-                'operator': opstring}
+        return {
+            "type": "operator",
+            "operands": [
+                binary.left._compiler_dispatch(self, **kw),
+                binary.right._compiler_dispatch(self, **kw),
+            ],
+            "operator": opstring,
+        }
 
     def _generate_generic_unary_operator(self, unary, opstring, **kw):
-        return {'type': 'operator',
-                'operator': opstring,
-                'operands': [unary.element._compiler_dispatch(self, **kw)]}
+        return {
+            "type": "operator",
+            "operator": opstring,
+            "operands": [unary.element._compiler_dispatch(self, **kw)],
+        }
 
     def _generate_generic_unary_modifier(self, unary, opstring, **kw):
-        return {'type': 'modifier',
-                'operator': opstring,
-                'operands': [unary.element._compiler_dispatch(self, **kw)]}
-
-    def _label_select_column(self, select, column,
-                             populate_result_map,
-                             asfrom, column_clause_args,
-                             name=None,
-                             within_columns_clause=True):
+        return {
+            "type": "modifier",
+            "operator": opstring,
+            "operands": [unary.element._compiler_dispatch(self, **kw)],
+        }
+
+    def _label_select_column(
+        self,
+        select,
+        column,
+        populate_result_map,
+        asfrom,
+        column_clause_args,
+        name=None,
+        within_columns_clause=True,
+    ):
         """produce labeled columns present in a select()."""
 
-        if column.type._has_column_expression and \
-                populate_result_map:
+        if column.type._has_column_expression and populate_result_map:
             col_expr = column.type.column_expression(column)
-            add_to_result_map = lambda keyname, name, objects, type_: \
-                self._add_to_result_map(
-                    keyname, name,
-                    (column,) + objects, type_)
+            add_to_result_map = (
+                lambda keyname, name, objects, type_: self._add_to_result_map(
+                    keyname, name, (column,) + objects, type_
+                )
+            )
         else:
             col_expr = column
             if populate_result_map:
                 add_to_result_map = self._add_to_result_map
             else:
                 add_to_result_map = None
 
         if not within_columns_clause:
             result_expr = col_expr
         elif isinstance(column, elements.Label):
             if col_expr is not column:
                 result_expr = compiler._CompileLabel(
-                    col_expr,
-                    column.name,
-                    alt_names=(column.element,)
+                    col_expr, column.name, alt_names=(column.element,)
                 )
             else:
                 result_expr = col_expr
 
         elif select is not None and name:
             result_expr = compiler._CompileLabel(
-                col_expr,
-                name,
-                alt_names=(column._key_label,)
+                col_expr, name, alt_names=(column._key_label,)
             )
 
-        elif \
-                                                asfrom and \
-                                                isinstance(column,
-                                                           elements.ColumnClause) and \
-                                        not column.is_literal and \
-                                        column.table is not None and \
-                        not isinstance(column.table, selectable.Select):
-            result_expr = compiler._CompileLabel(col_expr,
-                                                 elements._as_truncated(
-                                                     column.name),
-                                                 alt_names=(column.key,))
         elif (
-                        not isinstance(column, elements.TextClause) and
-                        (
-                                    not isinstance(column,
-                                                   elements.UnaryExpression) or
-                                    column.wraps_column_expression
-                        ) and
-                    (
-                                not hasattr(column, 'name') or
-                                isinstance(column, functions.Function)
-                    )
+            asfrom
+            and isinstance(column, elements.ColumnClause)
+            and not column.is_literal
+            and column.table is not None
+            and not isinstance(column.table, selectable.Select)
+        ):
+            result_expr = compiler._CompileLabel(
+                col_expr, elements._as_truncated(column.name), alt_names=(column.key,)
+            )
+        elif (
+            not isinstance(column, elements.TextClause)
+            and (
+                not isinstance(column, elements.UnaryExpression)
+                or column.wraps_column_expression
+            )
+            and (not hasattr(column, "name") or isinstance(column, functions.Function))
         ):
             result_expr = compiler._CompileLabel(col_expr, column.anon_label)
         elif col_expr is not column:
             # TODO: are we sure "column" has a .name and .key here ?
             # assert isinstance(column, elements.ColumnClause)
-            result_expr = compiler._CompileLabel(col_expr,
-                                                 elements._as_truncated(
-                                                     column.name),
-                                                 alt_names=(column.key,))
+            result_expr = compiler._CompileLabel(
+                col_expr, elements._as_truncated(column.name), alt_names=(column.key,)
+            )
         else:
             result_expr = col_expr
 
         column_clause_args.update(
             within_columns_clause=within_columns_clause,
-            add_to_result_map=add_to_result_map
-        )
-        return result_expr._compiler_dispatch(
-            self,
-            **column_clause_args
+            add_to_result_map=add_to_result_map,
         )
+        return result_expr._compiler_dispatch(self, **column_clause_args)
 
-    def _compose_select_body(
-            self, jsn, select, inner_columns, froms, byfrom, kwargs):
+    def _compose_select_body(self, jsn, select, inner_columns, froms, byfrom, kwargs):
 
-        jsn['fields'] = inner_columns
+        jsn["fields"] = inner_columns
 
         if froms:
             if select._hints:
-                jsn['from'] = [f._compiler_dispatch(self, asfrom=True,
-                                                    fromhints=byfrom, **kwargs)
-                               for f in froms]
+                jsn["from"] = [
+                    f._compiler_dispatch(self, asfrom=True, fromhints=byfrom, **kwargs)
+                    for f in froms
+                ]
             else:
-                jsn['from'] = [f._compiler_dispatch(self, asfrom=True, **kwargs)
-                               for f in froms]
-        else:
-            jsn['from'] = self.default_from()
+                jsn["from"] = [
+                    f._compiler_dispatch(self, asfrom=True, **kwargs) for f in froms
+                ]
 
         if select._whereclause is not None:
             t = select._whereclause._compiler_dispatch(self, **kwargs)
             if t:
-                jsn['where'] = t
+                jsn["where"] = t
 
         if select._group_by_clause.clauses:
-            group_by = select._group_by_clause._compiler_dispatch(
-                self, **kwargs)
+            group_by = select._group_by_clause._compiler_dispatch(self, **kwargs)
             if group_by:
-                jsn['group_by'] = group_by
+                jsn["group_by"] = group_by
 
         if select._having is not None:
             t = select._having._compiler_dispatch(self, **kwargs)
             if t:
-                jsn['having'] = t
+                jsn["having"] = t
 
         if select._order_by_clause.clauses:
-            jsn['order_by'] = self.order_by_clause(select, **kwargs)
+            jsn["order_by"] = self.order_by_clause(select, **kwargs)
 
-        if (select._limit_clause is not None or
-                    select._offset_clause is not None):
+        if select._limit_clause is not None or select._offset_clause is not None:
             jsn.update(self.limit_clause(select, **kwargs))
 
         if select._for_update_arg is not None:
-            jsn['for_update'] = self.for_update_clause(select, **kwargs)
+            jsn["for_update"] = self.for_update_clause(select, **kwargs)
 
         return jsn
 
     def _generate_prefixes(self, stmt, prefixes, **kw):
         clause = " ".join(
             prefix._compiler_dispatch(self, **kw)
             for prefix, dialect_name in prefixes
-            if dialect_name is None or
-            dialect_name == self.dialect.name
+            if dialect_name is None or dialect_name == self.dialect.name
         )
         if clause:
             clause += " "
         return clause
 
     def _setup_select_stack(self, select, entry, asfrom):
-        correlate_froms = entry['correlate_froms']
-        asfrom_froms = entry['asfrom_froms']
+        correlate_froms = entry["correlate_froms"]
+        asfrom_froms = entry["asfrom_froms"]
 
         if asfrom:
             froms = select._get_display_froms(
-                explicit_correlate_froms=correlate_froms.difference(
-                    asfrom_froms),
-                implicit_correlate_froms=())
+                explicit_correlate_froms=correlate_froms.difference(asfrom_froms),
+                implicit_correlate_froms=(),
+            )
         else:
             froms = select._get_display_froms(
                 explicit_correlate_froms=correlate_froms,
-                implicit_correlate_froms=asfrom_froms)
+                implicit_correlate_froms=asfrom_froms,
+            )
 
         new_correlate_froms = set(selectable._from_objects(*froms))
         all_correlate_froms = new_correlate_froms.union(correlate_froms)
 
         new_entry = {
-            'asfrom_froms': new_correlate_froms,
-            'correlate_froms': all_correlate_froms,
-            'selectable': select,
+            "asfrom_froms": new_correlate_froms,
+            "correlate_froms": all_correlate_froms,
+            "selectable": select,
         }
         self.stack.append(new_entry)
         return froms
 
     def limit_clause(self, select, **kw):
         d = {}
         if select._limit_clause is not None:
-            d['limit'] = self.process(select._limit_clause, **kw)
+            d["limit"] = self.process(select._limit_clause, **kw)
         if select._offset_clause is not None:
-            d['offset'] = self.process(select._offset_clause, **kw)
+            d["offset"] = self.process(select._offset_clause, **kw)
         return d
 
     def returning_clause(self, stmt, returning_cols):
         columns = [
             self._label_select_column(None, c, True, False, {})
             for c in expression._select_iterables(returning_cols)
-            ]
+        ]
         return columns
 
     def order_by_clause(self, select, **kw):
         order_by = select._order_by_clause._compiler_dispatch(self, **kw)
         if order_by:
             return order_by
         else:
             return {}
 
     def for_update_clause(self, select, **kw):
-        return {'for_update': True}
+        return {"for_update": True}
+
+    def visit_wkb_element(self, element):
+        return element.compile()
+
+    def visit_isfalse_unary_operator(self, element, operator, **kw):
+        return {
+            "type": "operator",
+            "operator": "not",
+            "operands": [self.process(element.element, **kw)],
+        }
+
+
+class OETypeCompiler(PGTypeCompiler):
+    def visit_FLOAT(self, type_, **kw):
+        if type_.asdecimal:
+            d = {"type": "datatype", "datatype": "FLOAT", "kwargs": {"asdecimal": True}}
+            if not type_.precision:
+                d["precision"] = type_.precision
+            return d
+        if not type_.precision:
+            return "FLOAT"
+        else:
+            return "FLOAT(%(precision)s)" % {"precision": type_.precision}
+
+
+@compiles(WKBElement)
+def compiles_WKBElement(element, compiler):
+    compiler.visit_wkb_element(element)
```

### Comparing `oedialect-0.0.9.dev0/oedialect/dialect.py` & `oedialect-0.1.1.dev0/oedialect/dialect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,95 @@
 from sqlalchemy.dialects import postgresql
 from sqlalchemy import util
 from sqlalchemy.engine import reflection
 from sqlalchemy.dialects.postgresql.base import PGExecutionContext
 
 import shapely
 import geoalchemy2
+import json
 import logging
 import warnings
 
 from oedialect import dbapi, compiler as oecomp
-from oedialect.compiler import OEDDLCompiler, OECompiler
+from oedialect.compiler import OEDDLCompiler, OECompiler, OETypeCompiler
 
-logger = logging.getLogger('sqlalchemy.dialects.postgresql')
+logger = logging.getLogger("sqlalchemy.dialects.postgresql")
 
 
 class OEExecutionContext(PGExecutionContext):
-
     def fire_sequence(self, sequence, type_):
 
-        seq = {'type': 'sequence', 'sequence': sequence.name}
+        seq = {"type": "sequence", "sequence": sequence.name}
         if sequence.schema is not None:
-            seq['schema'] = sequence.schema
+            seq["schema"] = sequence.schema
 
         query = {
-            'command': 'advanced/search',
-            'type': 'select',
-            'fields': [
-                {'type': 'function',
-                 'function': 'nextval',
-                 'operands': [seq]}
-            ]
+            "command": "advanced/search",
+            "type": "select",
+            "fields": [{"type": "function", "function": "nextval", "operands": [seq]}],
         }
 
         return self._execute_scalar(query, type_)
 
     @classmethod
-    def _init_compiled(cls, dialect, connection, dbapi_connection,
-                       compiled, parameters):
+    def _init_compiled(
+        cls, dialect, connection, dbapi_connection, compiled, parameters
+    ):
         """Initialize execution context for a Compiled construct."""
 
         self = cls.__new__(cls)
         self.root_connection = connection
         self._dbapi_connection = dbapi_connection
         self.dialect = connection.dialect
 
         self.compiled = compiled
 
         # this should be caught in the engine before
         # we get here
         assert compiled.can_execute
 
         self.execution_options = compiled.execution_options.union(
-            connection._execution_options)
+            connection._execution_options
+        )
 
         self.result_column_struct = (
-            compiled._result_columns, compiled._ordered_columns,
-            compiled._textual_ordered_columns)
+            compiled._result_columns,
+            compiled._ordered_columns,
+            compiled._textual_ordered_columns,
+        )
 
         self.unicode_statement = util.text_type(compiled)
         if not dialect.supports_unicode_statements:
-            self.statement = self.unicode_statement.encode(
-                self.dialect.encoding)
+            self.statement = self.unicode_statement.encode(self.dialect.encoding)
         else:
             self.statement = self.unicode_statement
 
         self.isinsert = compiled.isinsert
         self.isupdate = compiled.isupdate
         self.isdelete = compiled.isdelete
         self.is_text = compiled.isplaintext
 
         if not parameters:
             self.compiled_parameters = [compiled.construct_params()]
         else:
-            self.compiled_parameters = \
-                [compiled.construct_params(m, _group_number=grp) for
-                 grp, m in enumerate(parameters)]
+            self.compiled_parameters = [
+                compiled.construct_params(m, _group_number=grp)
+                for grp, m in enumerate(parameters)
+            ]
 
             self.executemany = len(parameters) > 1
 
         self.cursor = self.create_cursor()
 
         if self.isinsert or self.isupdate or self.isdelete:
             self.is_crud = True
             self._is_explicit_returning = bool(compiled.statement._returning)
             self._is_implicit_returning = bool(
-                compiled.returning and not compiled.statement._returning)
+                compiled.returning and not compiled.statement._returning
+            )
 
         if self.compiled.insert_prefetch or self.compiled.update_prefetch:
             if self.executemany:
                 self._process_executemany_defaults()
             else:
                 self._process_executesingle_defaults()
 
@@ -113,36 +114,35 @@
 
                 if encode:
                     param = dict(
                         (
                             dialect._encoder(key)[0],
                             processors[key](compiled_params[key])
                             if key in processors
-                            else compiled_params[key]
+                            else compiled_params[key],
                         )
                         for key in compiled_params
                     )
                 else:
                     param = dict(
                         (
                             key,
                             processors[key](compiled_params[key])
                             if key in processors
-                            else compiled_params[key]
+                            else compiled_params[key],
                         )
                         for key in compiled_params
                     )
 
                 parameters.append(param)
         self.parameters = dialect.execute_sequence_format(parameters)
 
         self.statement = compiled
         return self
 
-
     @classmethod
     def _init_ddl(cls, dialect, connection, dbapi_connection, compiled_ddl):
         self = cls.__new__(cls)
         self.root_connection = connection
         self._dbapi_connection = dbapi_connection
         self.dialect = connection.dialect
 
@@ -167,75 +167,66 @@
             self.parameters = [dialect.execute_sequence_format()]
         else:
             self.parameters = [{}]
 
         self.statement = compiled_ddl.string
         return self
 
-
     def get_insert_default(self, column):
-        if column.primary_key and \
-                column is column.table._autoincrement_column:
+        if column.primary_key and column is column.table._autoincrement_column:
             if column.server_default and column.server_default.has_argument:
 
                 exc = {
-                    'command': 'advanced/search',
-                    'type': 'select',
-                    'fields': [column.server_default.arg]
+                    "command": "advanced/search",
+                    "type": "select",
+                    "fields": [column.server_default.arg],
                 }
 
                 # pre-execute passive defaults on primary key columns
-                return self._execute_scalar(exc
-                                            ,
-                                            column.type)
-
-            elif (column.default is None or
-                  (column.default.is_sequence and
-                   column.default.optional)):
+                return self._execute_scalar(exc, column.type)
+
+            elif column.default is None or (
+                column.default.is_sequence and column.default.optional
+            ):
 
                 # execute the sequence associated with a SERIAL primary
                 # key column. for non-primary-key SERIAL, the ID just
                 # generates server side.
 
                 try:
                     seq_name = column._postgresql_seq_name
                 except AttributeError:
                     tab = column.table.name
                     col = column.name
-                    tab = tab[0:29 + max(0, (29 - len(col)))]
-                    col = col[0:29 + max(0, (29 - len(tab)))]
+                    tab = tab[0 : 29 + max(0, (29 - len(col)))]
+                    col = col[0 : 29 + max(0, (29 - len(tab)))]
                     name = "%s_%s_seq" % (tab, col)
                     column._postgresql_seq_name = seq_name = name
 
                 if column.table is not None:
-                    effective_schema = self.connection.schema_for_object(
-                        column.table)
+                    effective_schema = self.connection.schema_for_object(column.table)
                 else:
                     effective_schema = None
 
-                seq = {'type':'sequence', 'sequence': seq_name}
+                seq = {"type": "sequence", "sequence": seq_name}
                 if effective_schema is not None:
-                    seq['schema'] = effective_schema
+                    seq["schema"] = effective_schema
 
                 exc = {
-                    'command': 'advanced/search',
-                    'type': 'select',
-                    'fields': [
-                        {'type': 'function',
-                         'function': 'nextval',
-                         'operands': [seq]}
-                    ]
+                    "command": "advanced/search",
+                    "type": "select",
+                    "fields": [
+                        {"type": "function", "function": "nextval", "operands": [seq]}
+                    ],
                 }
 
-
                 return self._execute_scalar(exc, column.type)
 
         return super(PGExecutionContext, self).get_insert_default(column)
 
-
     @property
     def rowcount(self):
         return self.cursor.rowcount
 
     def create_server_side_cursor(self):
         return self._dbapi_connection.cursor()
 
@@ -243,41 +234,38 @@
 class OEDialect(postgresql.psycopg2.PGDialect_psycopg2):
     ddl_compiler = OEDDLCompiler
     statement_compiler = OECompiler
     execution_ctx_cls = OEExecutionContext
     _supports_create_index_concurrently = False
     _supports_drop_index_concurrently = False
     supports_comments = False
-
+    type_compiler = OETypeCompiler
 
     def __init__(self, *args, **kwargs):
         self._engine = None
-        self.default_schema_name = 'model_draft'
-        if kwargs.get('json_serializer') is not None:
-            warnings.warn('Use of the keyword \'json_serializer\' is not '
-                          'supported')
-        kwargs['json_serializer'] = lambda x: x
-
-        if kwargs.get('json_deserializer') is not None:
-            warnings.warn('Use of the keyword \'json_serializer\' is not '
-                          'supported')
+        self.default_schema_name = "model_draft"
+        if kwargs.get("json_serializer") is not None:
+            warnings.warn("Use of the keyword 'json_serializer' is not " "supported")
+        kwargs["json_serializer"] = lambda x: x
+
+        if kwargs.get("json_deserializer") is not None:
+            warnings.warn("Use of the keyword 'json_serializer' is not " "supported")
 
-        kwargs['json_deserializer'] = lambda x: x
+        kwargs["json_deserializer"] = lambda x: x
         super(OEDialect, self).__init__(*args, **kwargs)
         self.dbapi = dbapi
 
-
     """def do_execute(self, cursor, statement, parameters, context=None):
         cursor.execute(context, parameters)"""
 
     def initialize(self, connection):
         pass
 
     def _check_unicode_description(self, connection):
-        return isinstance('x', sa_util.text_type)
+        return isinstance("x", sa_util.text_type)
 
     def _check_unicode_returns(self, connection, additional_tests=None):
         return True
 
     def _get_server_version_info(self, connection):
         return (9, 3)
 
@@ -291,200 +279,221 @@
             return res
 
     def _get_default_schema_name(self, connection):
         # TODO: return connection.scalar("select current_schema()")
         return None
 
     def has_schema(self, connection, schema):
-        return self.execute_with_cursor(connection,{'command': 'advanced/has_schema',
-                              'schema': schema})
+        return self.execute_with_cursor(
+            connection, {"command": "advanced/has_schema", "schema": schema}
+        )
 
     def has_table(self, connection, table_name, schema=None):
-        query = {'table': table_name}
+        query = {"table": table_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         else:
-            query['schema'] = oecomp.DEFAULT_SCHEMA
+            query["schema"] = oecomp.DEFAULT_SCHEMA
 
-        query['command'] = 'advanced/has_table'
+        query["command"] = "advanced/has_table"
         return self.execute_with_cursor(connection, query)
 
     def has_sequence(self, connection, sequence_name, schema=None):
-        query = {'sequence_name': sequence_name}
+        query = {"sequence_name": sequence_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
 
-        query['command'] = 'advanced/has_sequence'
+        query["command"] = "advanced/has_sequence"
         return self.execute_with_cursor(connection, query)
 
     def has_type(self, connection, type_name, schema=None):
-        query = {'type_name': type_name}
+        query = {"type_name": type_name}
         if schema:
-            query['schema'] = schema
-        query['command'] = 'advanced/has_type'
+            query["schema"] = schema
+        query["command"] = "advanced/has_type"
         return self.execute_with_cursor(connection, query)
 
     @reflection.cache
     def get_table_oid(self, connection, table_name, schema=None, **kw):
         raise NotImplementedError
 
     @reflection.cache
     def get_schema_names(self, connection, **kw):
         query = dict(kw)
-        query['command'] = 'advanced/get_schema_names'
+        query["command"] = "advanced/get_schema_names"
         return self.execute_with_cursor(connection, query)
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         query = {}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         query.update(kw)
-        query['command'] = 'advanced/get_table_names'
+        query["command"] = "advanced/get_table_names"
         return self.execute_with_cursor(connection, query)
 
+    def get_table_comment(self, connection, table_name, schema=None, **kw):
+        query = dict(
+            request_type="get",
+            command="schema/{schema}/tables/{table}/meta/".format(
+                schema=schema if schema else "sandbox", table=table_name
+            ),
+        )
+        result = self.execute_with_cursor(connection, query)
+        result = dict(text=json.dumps(result) if result else None)
+        return result
+
     @reflection.cache
     def get_view_names(self, connection, schema=None, **kw):
         query = {}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         query.update(kw)
-        query['command'] = 'advanced/get_view_names'
+        query["command"] = "advanced/get_view_names"
         return self.execute_with_cursor(connection, query)
 
     @reflection.cache
     def get_view_definition(self, connection, view_name, schema=None, **kw):
-        query = {'view_name': view_name}
+        query = {"view_name": view_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         query.update(kw)
-        query['command'] = 'advanced/get_view_definition'
+        query["command"] = "advanced/get_view_definition"
         with connection.connect() as conn:
             return conn.connection.cursor().execute(query)
 
     @reflection.cache
     def get_columns_raw(self, engine, table_name, schema=None, **kw):
-        query = {'table': table_name}
+        query = {"table": table_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
 
         # Json does not permit compound dictionary keys.
         # Fortunately, we need just the cached table name.
-        query['info_cache'] = {'+'.join(k[1]): v for k, v in kw['info_cache'].items() if k[0] == 'get_columns_raw'}
-        query['command'] = 'advanced/get_columns'
+        query["info_cache"] = {
+            "+".join(k[1]): v
+            for k, v in kw["info_cache"].items()
+            if k[0] == "get_columns_raw"
+        }
+        query["command"] = "advanced/get_columns"
         with engine.connect() as conn:
-            response = conn.connection.post('advanced/get_columns', query)
+            response = conn.connection.post("advanced/get_columns", query)
 
-            content = response['content']
+            content = response["content"]
         return content
 
     def get_columns(self, engine, table_name, schema=None, **kw):
 
-            content = self.get_columns_raw(engine, table_name, schema, **kw)
-            rows = content['columns']
-            domains = content['domains']
-            enums = content['enums']
-
-            columns = []
-            for name, format_type, default, notnull, attnum, table_oid in rows:
-                column_info = self._get_column_info(
-                    name, format_type, default, notnull, domains, enums, schema,
-                    None)
-                columns.append(column_info)
-            return columns
+        content = self.get_columns_raw(engine, table_name, schema, **kw)
+        rows = content["columns"]
+        domains = content["domains"]
+        enums = content["enums"]
+
+        columns = []
+        for name, format_type, default, notnull, attnum, table_oid in rows:
+            column_info = self._get_column_info(
+                name, format_type, default, notnull, domains, enums, schema, None, None
+            )  # Usage of 'generated' argument skipped
+            columns.append(column_info)
+        return columns
 
     @reflection.cache
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
-        query = {'table': str(table_name)}
+        query = {"table": str(table_name)}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         with connection.connect() as conn:
-            val = conn.connection.post('advanced/get_pk_constraint', query)
-            return val['content']
+            val = conn.connection.post("advanced/get_pk_constraint", query)
+            return val["content"]
 
     @reflection.cache
-    def get_foreign_keys(self, connection, table_name, schema=None,
-                         postgresql_ignore_search_path=False, **kw):
-        query = {'table': table_name}
+    def get_foreign_keys(
+        self,
+        connection,
+        table_name,
+        schema=None,
+        postgresql_ignore_search_path=False,
+        **kw
+    ):
+        query = {"table": table_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         if postgresql_ignore_search_path:
-            query['postgresql_ignore_search_path'] = \
-                postgresql_ignore_search_path
+            query["postgresql_ignore_search_path"] = postgresql_ignore_search_path
         query.update(kw)
-        if 'info_cache' in query:
-            del query['info_cache']
-        query['command'] = 'advanced/get_foreign_keys'
+        if "info_cache" in query:
+            del query["info_cache"]
+        query["command"] = "advanced/get_foreign_keys"
         return self.execute_with_cursor(connection, query)
 
     @reflection.cache
     def get_indexes(self, connection, table_name, schema, **kw):
-        query = {'table': table_name, 'schema': schema}
+        query = {"table": table_name, "schema": schema}
         query.update(kw)
-        query['command'] = 'advanced/get_indexes'
+        query["command"] = "advanced/get_indexes"
         return self.execute_with_cursor(connection, query)
 
     @reflection.cache
-    def get_unique_constraints(self, connection, table_name,
-                               schema=None, **kw):
-        query = {'table': table_name}
+    def get_unique_constraints(self, connection, table_name, schema=None, **kw):
+        query = {"table": table_name}
         if schema:
-            query['schema'] = schema
+            query["schema"] = schema
         query.update(kw)
-        if 'info_cache' in query:
-            del query['info_cache']
+        if "info_cache" in query:
+            del query["info_cache"]
         with connection.connect() as conn:
-            val = conn.connection.post('advanced/get_unique_constraints', query)
-            return val['content']
+            val = conn.connection.post("advanced/get_unique_constraints", query)
+            return val["content"]
 
     def get_isolation_level(self, connection):
-        query= {'command': 'advanced/get_isolation_level'}
+        query = {"command": "advanced/get_isolation_level"}
         cursor = connection.cursor()
         cursor.execute(query)
         cursor.close()
         val = cursor.fetchone()[0]
         return val.upper()
 
-
     def set_isolation_level(self, connection, level):
-        query = {'command': 'advanced/set_isolation_level',
-                 'level': level}
+        query = {"command": "advanced/set_isolation_level", "level": level}
         return self.execute_with_cursor(connection, query)
 
-
     def do_prepare_twophase(self, connection, xid):
-        result = connection.connection.cursor().execute('advanced/do_prepare_twophase', {'xid': xid})
-
-
-    def do_rollback_twophase(self, connection, xid,
-                             is_prepared=True, recover=False):
-        result = connection.connection.post('advanced/do_rollback_twophase', {'xid': xid,
-                                               'is_prepared':is_prepared,
-                                               'recover': recover})
-
-    def do_commit_twophase(self, connection, xid,
-                           is_prepared=True, recover=False):
-        result = connection.connection.post('advanced/do_commit_twophase', {'xid': xid,
-                                             'is_prepared': is_prepared,
-                                             'recover': recover})
+        result = connection.connection.cursor().execute(
+            "advanced/do_prepare_twophase", {"xid": xid}
+        )
+
+    def do_rollback_twophase(self, connection, xid, is_prepared=True, recover=False):
+        result = connection.connection.post(
+            "advanced/do_rollback_twophase",
+            {"xid": xid, "is_prepared": is_prepared, "recover": recover},
+        )
+
+    def do_commit_twophase(self, connection, xid, is_prepared=True, recover=False):
+        result = connection.connection.post(
+            "advanced/do_commit_twophase",
+            {"xid": xid, "is_prepared": is_prepared, "recover": recover},
+        )
 
     def do_recover_twophase(self, connection):
-        result = connection.connection.post('advanced/do_recover_twophase', {})
+        result = connection.connection.post("advanced/do_recover_twophase", {})
         return [row[0] for row in result]
 
     def on_connect(self):
         return None
 
+
 # hic sunt dracones
 
 # We need to inject some functionality into WKBElements in order to handle the
 # static format for geometries returned by the API.
 # I'm sorry!
 
 orig_init_WKBElement = geoalchemy2.WKBElement.__init__
 
+
 def init_WKBElement(self, data, *args, **kwargs):
     if isinstance(data, str):
         data = shapely.wkb.dumps(shapely.wkb.loads(data, hex=True))
     orig_init_WKBElement(self, data, *args, **kwargs)
 
+
 geoalchemy2.WKBElement.__init__ = init_WKBElement
```

### Comparing `oedialect-0.0.9.dev0/oedialect/engine.py` & `oedialect-0.1.1.dev0/oedialect/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,67 +2,78 @@
 
 import os
 import requests
 import sqlalchemy
 from dateutil.parser import parse as parse_date
 from shapely import wkb
 from psycopg2.extensions import PYINTERVAL
-
+from decimal import Decimal
+import datetime
 from oedialect import error
+from sqlalchemy.dialects.postgresql.base import _DECIMAL_TYPES
+
+from oedialect.settings import OEP_URL, LOCAL_OEP_URL
 
 
 def date_handler(obj):
     """
     Implements a handler to serialize dates in JSON-strings
     :param obj: An object
     :return: The str method is called (which is the default serializer for JSON) unless the object has an attribute  *isoformat*
     """
-    if hasattr(obj, 'isoformat'):
-        return obj.isoformat()
+    if isinstance(obj, datetime.time):
+        return {"type": "value", "datatype": "time", "value": obj.isoformat()}
+    elif isinstance(obj, datetime.datetime):
+        return {"type": "value", "datatype": "datetime", "value": obj.isoformat()}
+    elif isinstance(obj, datetime.date):
+        return {"type": "value", "datatype": "date", "value": obj.isoformat()}
+    elif isinstance(obj, Decimal):
+        return {"type": "value", "datatype": "Decimal", "value": str(obj)}
     else:
         return str(obj)
 
-class OEConnection():
-    """
 
-    """
+class OEConnection:
+    """"""
 
     """
         Connection methods
     """
 
-    def __init__(self, host='localhost', port=80, user='', database='', password=''):
+    def __init__(self, host=LOCAL_OEP_URL, port=80, user="", database="", password=""):
         self.__host = host
         self.__port = port
         self.__user = user
         self.__token = password
-        response = self.post('advanced/connection/open', {})['content']
-        self._id = response['connection_id']
+        response = self.post("advanced/connection/open", {})["content"]
+        self._id = response["connection_id"]
         self.__transactions = set()
         self._cursors = set()
         self.__closed = False
 
     """
         TODO: Look at PGDialect in sqlalchemy.dialects.postgresql.base
     """
 
     def close(self, *args, **kwargs):
-        #for cursor in self._cursors:
+        # for cursor in self._cursors:
         #    cursor.close()
-        response = self.post('advanced/connection/close', {},
-                             requires_connection_id=True)
-
+        response = self.post(
+            "advanced/connection/close", {}, requires_connection_id=True
+        )
 
     def commit(self, *args, **kwargs):
-        response = self.post('advanced/connection/commit', {},
-                             requires_connection_id=True)
+        response = self.post(
+            "advanced/connection/commit", {}, requires_connection_id=True
+        )
 
     def rollback(self, *args, **kwargs):
-        response = self.post('advanced/connection/rollback', {},
-                             requires_connection_id=True)
+        response = self.post(
+            "advanced/connection/rollback", {}, requires_connection_id=True
+        )
 
     def cursor(self, *args, **kwargs):
         cursor = OECursor(self)
         self._cursors.add(cursor)
         return cursor
 
     """
@@ -130,247 +141,295 @@
 
     def fileno(self, *args, **kwargs):
         raise NotImplementedError
 
     def isexecuting(self, *args, **kwargs):
         raise NotImplementedError
 
-
     def post_expect_stream(self, suffix, query, cursor_id=None):
         sender = requests.post
 
         header = dict(urlheaders)
         if self.__token:
-            header['Authorization'] = 'Token %s' % self.__token
+            header["Authorization"] = "Token %s" % self.__token
 
         data = {}
         if cursor_id:
-            data['connection_id'] = self._id
-            data['cursor_id'] = cursor_id
+            data["connection_id"] = self._id
+            data["cursor_id"] = cursor_id
 
         host = self.__host
-        if self.__host in ['oep.iks.cs.ovgu.de', 'oep2.iks.cs.ovgu.de',
-                           'oep.iws.cs.ovgu.de', 'oep2.iws.cs.ovgu.de',
-                           'openenergyplatform.org']:
-            host = 'openenergy-platform.org'
+        if self.__host in [
+            "oep.iks.cs.ovgu.de",
+            "oep2.iks.cs.ovgu.de",
+            "oep.iws.cs.ovgu.de",
+            "oep2.iws.cs.ovgu.de",
+            "openenergyplatform.org",
+            "openenergy-platform.org",
+        ]:
+            host = OEP_URL
 
         port = self.__port if self.__port != 80 else 443
 
-        protocol = os.environ.get('OEDIALECT_PROTOCOL', 'https')
-        assert protocol in ['http', 'https']
+        protocol = os.environ.get("OEDIALECT_PROTOCOL", "https")
+        assert protocol in ["http", "https"]
 
-        verify = os.environ.get('OEDIALECT_VERIFY_CERTIFICATE', 'TRUE') == 'TRUE'
+        verify = os.environ.get("OEDIALECT_VERIFY_CERTIFICATE", "TRUE") == "TRUE"
 
         response = sender(
-            '{protocol}://{host}:{port}/api/v0/{suffix}'.format(
-                protocol=protocol,
-                host=host,
-                port=port,
-                suffix=suffix),
+            "{protocol}://{host}:{port}/api/v0/{suffix}".format(
+                protocol=protocol, host=host, port=port, suffix=suffix
+            ),
             json=json.loads(json.dumps(data)),
-            headers=header, stream=True, verify=verify)
+            headers=header,
+            stream=True,
+            verify=verify,
+        )
 
         process_returntype(response)
 
         try:
             i = 0
             for line in response.iter_lines():
-                yield json.loads(line.decode('utf8').replace("'", '\\"'))
+                yield json.loads(line.decode("utf8").replace("'", '\\"'))
         except Exception as e:
             raise
 
-
-
     def post(self, suffix, query, cursor_id=None, requires_connection_id=False):
         sender = requests.post
-        if isinstance(query, dict) and 'request_type' in query:
-            if query['request_type'] == 'put':
+        if isinstance(query, dict) and "request_type" in query:
+            if query["request_type"] == "put":
                 sender = requests.put
-            if query['request_type'] == 'delete':
+            if query["request_type"] == "delete":
                 sender = requests.delete
+            if query["request_type"] == "get":
+                sender = requests.get
 
-        if 'info_cache' in query:
-            del query['info_cache']
+        if "info_cache" in query:
+            del query["info_cache"]
 
-        data = {'query': query}
+        data = {"query": query}
 
         if requires_connection_id or cursor_id:
-            data['connection_id'] = self._id
+            data["connection_id"] = self._id
 
         if cursor_id:
-            data['cursor_id'] = cursor_id
+            data["cursor_id"] = cursor_id
 
         header = dict(urlheaders)
         if self.__token:
-            header['Authorization'] = 'Token %s'%self.__token
+            header["Authorization"] = "Token %s" % self.__token
 
         host = self.__host
-        if self.__host in ['oep.iks.cs.ovgu.de', 'oep2.iks.cs.ovgu.de',
-                           'oep.iws.cs.ovgu.de', 'oep2.iws.cs.ovgu.de',
-                           'openenergyplatform.org']:
-            host = 'openenergy-platform.org'
-
+        if self.__host in [
+            "oep.iks.cs.ovgu.de",
+            "oep2.iks.cs.ovgu.de",
+            "oep.iws.cs.ovgu.de",
+            "oep2.iws.cs.ovgu.de",
+            "openenergyplatform.org",
+            "openenergy-platform.org",
+        ]:
+            host = OEP_URL
 
         port = self.__port if self.__port != 80 else 443
 
-        protocol = os.environ.get('OEDIALECT_PROTOCOL', 'https')
-        assert protocol in ['http', 'https']
-        verify = os.environ.get('OEDIALECT_VERIFY_CERTIFICATE', 'TRUE') == 'TRUE'
+        protocol = os.environ.get("OEDIALECT_PROTOCOL", "https")
+        assert protocol in ["http", "https"]
+        verify = os.environ.get("OEDIALECT_VERIFY_CERTIFICATE", "TRUE") == "TRUE"
         ans = sender(
-            '{protocol}://{host}:{port}/api/v0/{suffix}'.format(
-                protocol=protocol,
-                host=host,
-                port=port,
-                suffix=suffix),
+            "{protocol}://{host}:{port}/api/v0/{suffix}".format(
+                protocol=protocol, host=host, port=port, suffix=suffix
+            ),
             json=json.loads(json.dumps(data, default=date_handler)),
-            headers=header, verify=verify)
+            headers=header,
+            verify=verify,
+        )
 
         try:
             json_response = ans.json()
         except:
-            raise ConnectionException('Answer contains no JSON: ' + repr(ans))
+            raise ConnectionException("Answer contains no JSON: " + repr(ans))
 
         process_returntype(ans, json_response)
 
+        if isinstance(query, dict) and "request_type" in query:
+            if query["request_type"] == "get":
+                json_response = dict(content=json_response)
+
         return json_response
 
+
 def process_returntype(response, content=None):
     if content is None:
         content = {}
     if 400 <= response.status_code < 500:
         message = content.get("reason", "")
-        raise ConnectionException('HTTP %d (%s): %s'%(response.status_code,response.reason, message))
+        raise ConnectionException(
+            "HTTP %d (%s): %s" % (response.status_code, response.reason, message)
+        )
     elif 500 <= response.status_code < 600:
-        raise ConnectionException('Server side error: ' + content.get('reason', 'No reason returned'))
+        raise ConnectionException(
+            "Server side error: " + content.get("reason", "No reason returned")
+        )
+
 
 class OECursor:
     description = None
     rowcount = -1
 
     def __init__(self, connection):
         self.__connection = connection
         try:
-            response = self.__connection.post('advanced/cursor/open', {}, requires_connection_id=True)
-            if 'content' not in response:
-                raise error.CursorError('Could not open cursor: ' + str(response['reason']) if 'reason' in response else 'No reason returned')
-            response = response['content']
+            response = self.__connection.post(
+                "advanced/cursor/open", {}, requires_connection_id=True
+            )
+            if "content" not in response:
+                raise error.CursorError(
+                    "Could not open cursor: " + str(response["reason"])
+                    if "reason" in response
+                    else "No reason returned"
+                )
+            response = response["content"]
         except:
             raise
-        self.__id = response['cursor_id']
-
+        self.__id = response["cursor_id"]
 
     def __replace_params(self, jsn, params):
-        if type(jsn) == dict:
+        if jsn is None:
+            return dict(type="value", value=None)
+        elif type(jsn) == dict:
             for k in jsn:
                 jsn[k] = self.__replace_params(jsn[k], params)
             return jsn
         elif type(jsn) == list:
             return list(map(lambda x: self.__replace_params(x, params), jsn))
-        elif type(jsn) in [str, sqlalchemy.sql.elements.quoted_name,
-                           sqlalchemy.sql.elements._truncated_label]:
-            return (jsn % params).strip("'<>").replace('\'', '\"')
+        elif type(jsn) in [
+            str,
+            sqlalchemy.sql.elements.quoted_name,
+            sqlalchemy.sql.elements._truncated_label,
+        ]:
+            return (jsn % params).strip("'<>").replace("'", '"')
         elif isinstance(jsn, int):
             return jsn
         elif callable(jsn):
             return jsn(params)
         else:
             raise Exception("Unknown jsn type (%s) in %s" % (type(jsn), jsn))
 
     __cell_processors = {
         17: lambda cell: wkb.dumps(wkb.loads(cell, hex=True)),
         1114: lambda cell: parse_date(cell),
         1082: lambda cell: parse_date(cell).date(),
-        1186: lambda cell: PYINTERVAL(cell, None)
+        1083: lambda cell: parse_date(cell).time(),
+        1186: lambda cell: PYINTERVAL(cell, None),
     }
 
-    def process_result(self,row):
+    def process_result(self, row):
         for i, x in enumerate(self.description):
             # Translate WKB-hex to binary representation
             if row[i]:
                 if x[1] in self.__cell_processors:
                     row[i] = self.__cell_processors[x[1]](row[i])
+                elif x[1] in _DECIMAL_TYPES:
+                    if isinstance(row[i], list):
+                        row[i] = [Decimal(x) for x in row[i]]
+                    else:
+                        row[i] = Decimal(row[i])
+
         return row
 
     def fetchone(self):
-        response = self.__connection.post('advanced/cursor/fetch_one', {}, cursor_id=self.__id)[
-            'content']
+        response = self.__connection.post(
+            "advanced/cursor/fetch_one", {}, cursor_id=self.__id
+        )["content"]
         if response:
             response = self.process_result(response)
         return response
 
     def fetchall(self):
-        result = self.__connection.post_expect_stream('advanced/cursor/fetch_all', {}, cursor_id=self.__id)
+        result = self.__connection.post_expect_stream(
+            "advanced/cursor/fetch_all", {}, cursor_id=self.__id
+        )
         if result:
             for row in result:
                 yield self.process_result(row)
 
     def fetchmany(self, size):
-        result = self.__connection.post_expect_stream('advanced/cursor/fetch_many', {'size': size}, cursor_id=self.__id)
+        result = self.__connection.post_expect_stream(
+            "advanced/cursor/fetch_many", {"size": size}, cursor_id=self.__id
+        )
 
         if result:
             for row in result:
                 yield self.process_result(row)
 
-
     def execute(self, query_obj, params=None):
         if query_obj is None:
             return
         if not isinstance(query_obj, dict):
             if isinstance(query_obj, str):
-                raise Exception('Plain string commands are not supported.'
-                                'Please use SQLAlchemy datastructures')
+                raise Exception(
+                    "Plain string commands are not supported."
+                    "Please use SQLAlchemy datastructures"
+                )
             query = query_obj.string
         else:
             query = query_obj
         query = dict(query)
-        requires_connection_id = query.get('requires_connection', False)
+        requires_connection_id = query.get("requires_connection", False)
 
-        query['connection_id'] = self.__connection._id
-        query['cursor_id'] = self.__id
+        query["connection_id"] = self.__connection._id
+        query["cursor_id"] = self.__id
         if params:
-            if isinstance(params, tuple) and 'values' in query:
-                query['values'] = [self.__replace_params(query['values'][0], p) for p in params]
+            if isinstance(params, tuple) and "values" in query:
+                query["values"] = [
+                    self.__replace_params(query["values"][0], p) for p in params
+                ]
             else:
                 query = self.__replace_params(query, params)
         # query = context.compiled.string
-        command = query.pop('command')
-        return self.__execute_by_post(command, query,
-                                  requires_connection_id=requires_connection_id)
+        command = query.pop("command")
+        return self.__execute_by_post(
+            command, query, requires_connection_id=requires_connection_id
+        )
 
     def executemany(self, query, params=None):
         if params is None:
             return self.execute(query)
         else:
             if query.isinsert and not (query.isdelete or query.isupdate):
                 return self.execute(query, params)
             else:
                 return [self.execute(query, p) for p in params]
 
     def close(self):
-        self.__connection.post('advanced/cursor/close', {}, cursor_id=self.__id)
+        self.__connection.post("advanced/cursor/close", {}, cursor_id=self.__id)
 
     def __execute_by_post(self, command, query, requires_connection_id=False):
 
-        response = self.__connection.post(command, query, cursor_id=self.__id,
-                                requires_connection_id=requires_connection_id)
+        response = self.__connection.post(
+            command,
+            query,
+            cursor_id=self.__id,
+            requires_connection_id=requires_connection_id,
+        )
 
-        if 'content' in response:
-            result = response['content']
+        if "content" in response:
+            result = response["content"]
             if result:
                 if isinstance(result, dict):
-                    if 'description' in result:
-                        self.description = result['description']
-                    if 'rowcount' in result:
-                        self.rowcount = result['rowcount']
+                    if "description" in result:
+                        self.description = result["description"]
+                    if "rowcount" in result:
+                        self.rowcount = result["rowcount"]
+                    return result
                 else:
                     return result
             else:
                 return result
 
 
-
-urlheaders = {
-}
+urlheaders = {}
 
 
 class ConnectionException(Exception):
     pass
```

### Comparing `oedialect-0.0.9.dev0/oedialect.egg-info/PKG-INFO` & `oedialect-0.1.1.dev0/oedialect.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,66 @@
 Metadata-Version: 2.1
 Name: oedialect
-Version: 0.0.9.dev0
+Version: 0.1.1.dev0
 Summary: SQL-Alchemy dialect for the OpenEnergy Platform
 Home-page: https://github.com/openego/oedialect
 Author: MGlauer
 Author-email: martinglauer89@gmail.com
-License: UNKNOWN
-Description: ﻿<a href="http://oep.iks.cs.ovgu.de/"><img align="right" width="200" height="200" src="https://avatars2.githubusercontent.com/u/37101913?s=400&u=9b593cfdb6048a05ea6e72d333169a65e7c922be&v=4" alt="OpenEnergyPlatform"></a>
-        
-        # An [SQLAlchemy][0] [Dialect][1] for the [OEP][2]
-        
-        SQLAlchemy internally uses so called "dialects" to provide a consistent
-        interface to different database drivers. The `oedialect` supplies your
-        SQLAlchemy installation with a dialect using the REST-API of the [Open
-        Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
-        SQLAlchemy to down- and upload data to an OEP instance.
-        
-        [0]: https://www.sqlalchemy.org/
-        [1]: https://docs.sqlalchemy.org/en/13/dialects/
-        [2]: https://github.com/OpenEnergyPlatform/oeplatform
-        
-        ## License / Copyright
-        
-        This repository is licensed under [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)
-        
-        ## Installation
-        
-        `pip install oedialect`
-        
-        On MS-Windows make sure to install a version of `shapely` first.
-        `conda install shapely -c conda-forge`
-        
-        ## Example
-        
-        You can find a basic example [here](doc/example/oedialect_basic_example.ipynb).
-        
 Keywords: postgres,open,energy,database,sql,rest
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sqlalchemy>=1.3.16
+Requires-Dist: requests>=2.13
+Requires-Dist: psycopg2-binary
+Requires-Dist: geoalchemy2<0.7.0
+Requires-Dist: shapely
+Requires-Dist: python-dateutil
+Provides-Extra: tests
+Requires-Dist: black; extra == "tests"
+Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest==5.3; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Requires-Dist: sqlahelper; extra == "tests"
+Requires-Dist: geojson; extra == "tests"
+
+﻿<a href="http://oep.iks.cs.ovgu.de/"><img align="right" width="200" height="200" src="https://avatars2.githubusercontent.com/u/37101913?s=400&u=9b593cfdb6048a05ea6e72d333169a65e7c922be&v=4" alt="OpenEnergyPlatform"></a>
+
+# An [SQLAlchemy][0] [Dialect][1] for the [OEP][2]
+
+SQLAlchemy internally uses so called "dialects" to provide a consistent
+interface to different database drivers. The `oedialect` supplies your
+SQLAlchemy installation with a dialect using the REST-API of the [Open
+Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
+SQLAlchemy to down- and upload data to an OEP instance.
+
+[0]: https://www.sqlalchemy.org/
+[1]: https://docs.sqlalchemy.org/en/13/dialects/
+[2]: https://github.com/OpenEnergyPlatform/oeplatform
+
+## License / Copyright
+
+This repository is licensed under [GNU Affero General Public License v3.0 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+
+## Installation
+
+`pip install oedialect`
+
+On MS-Windows make sure to install a version of `shapely` first.
+`conda install shapely -c conda-forge`
+
+## Tutorials
+
+You can find tutorials and examples [here](https://github.com/OpenEnergyPlatform/examples/tree/master/api).
+
+
+## Testing
+
+To run the tests locally, first install the `tox` test environment
+`pip install tox`
+
+You need to setup a local instance of the [Open Energy Platform](https://github.com/OpenEnergyPlatform/oeplatform)
+
+Set your connection token that you got from your local OEP instance
+`LOCAL_OEP_TOKEN=<your_token>`
+
+Finally, run
+`tox`
```

#### html2text {}

```diff
@@ -1,18 +1,28 @@
-Metadata-Version: 2.1 Name: oedialect Version: 0.0.9.dev0 Summary: SQL-Alchemy
+Metadata-Version: 2.1 Name: oedialect Version: 0.1.1.dev0 Summary: SQL-Alchemy
 dialect for the OpenEnergy Platform Home-page: https://github.com/openego/
-oedialect Author: MGlauer Author-email: martinglauer89@gmail.com License:
-UNKNOWN Description: ï»¿_[_O_p_e_n_E_n_e_r_g_y_P_l_a_t_f_o_r_m_] # An [SQLAlchemy][0] [Dialect][1]
-for the [OEP][2] SQLAlchemy internally uses so called "dialects" to provide a
+oedialect Author: MGlauer Author-email: martinglauer89@gmail.com Keywords:
+postgres,open,energy,database,sql,rest Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: sqlalchemy>=1.3.16 Requires-Dist:
+requests>=2.13 Requires-Dist: psycopg2-binary Requires-Dist: geoalchemy2<0.7.0
+Requires-Dist: shapely Requires-Dist: python-dateutil Provides-Extra: tests
+Requires-Dist: black; extra == "tests" Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest==5.3; extra == "tests" Requires-Dist: pandas; extra ==
+"tests" Requires-Dist: sqlahelper; extra == "tests" Requires-Dist: geojson;
+extra == "tests" ï»¿_[_O_p_e_n_E_n_e_r_g_y_P_l_a_t_f_o_r_m_] # An [SQLAlchemy][0] [Dialect][1] for
+the [OEP][2] SQLAlchemy internally uses so called "dialects" to provide a
 consistent interface to different database drivers. The `oedialect` supplies
 your SQLAlchemy installation with a dialect using the REST-API of the [Open
 Energy Platform (OEP)][2]. In short, the `oedialect` allows you to use
 SQLAlchemy to down- and upload data to an OEP instance. [0]: https://
 www.sqlalchemy.org/ [1]: https://docs.sqlalchemy.org/en/13/dialects/ [2]:
 https://github.com/OpenEnergyPlatform/oeplatform ## License / Copyright This
 repository is licensed under [GNU Affero General Public License v3.0 (AGPL-
 3.0)](https://www.gnu.org/licenses/agpl-3.0.en.html) ## Installation `pip
 install oedialect` On MS-Windows make sure to install a version of `shapely`
-first. `conda install shapely -c conda-forge` ## Example You can find a basic
-example [here](doc/example/oedialect_basic_example.ipynb). Keywords:
-postgres,open,energy,database,sql,rest Platform: UNKNOWN Description-Content-
-Type: text/markdown
+first. `conda install shapely -c conda-forge` ## Tutorials You can find
+tutorials and examples [here](https://github.com/OpenEnergyPlatform/examples/
+tree/master/api). ## Testing To run the tests locally, first install the `tox`
+test environment `pip install tox` You need to setup a local instance of the
+[Open Energy Platform](https://github.com/OpenEnergyPlatform/oeplatform) Set
+your connection token that you got from your local OEP instance
+`LOCAL_OEP_TOKEN=` Finally, run `tox`
```

### Comparing `oedialect-0.0.9.dev0/test/test.py` & `oedialect-0.1.1.dev0/test/test.py`

 * *Files identical despite different names*

