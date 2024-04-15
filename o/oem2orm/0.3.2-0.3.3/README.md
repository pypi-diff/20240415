# Comparing `tmp/oem2orm-0.3.2.tar.gz` & `tmp/oem2orm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oem2orm-0.3.2.tar", last modified: Tue Nov 29 16:05:38 2022, max compression
+gzip compressed data, was "oem2orm-0.3.3.tar", last modified: Mon Apr 15 14:58:24 2024, max compression
```

## Comparing `oem2orm-0.3.2.tar` & `oem2orm-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 16:05:38.918293 oem2orm-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-29 16:05:27.000000 oem2orm-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2022-11-29 16:05:38.918293 oem2orm-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3145 2022-11-29 16:05:27.000000 oem2orm-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 16:05:38.918293 oem2orm-0.3.2/oem2orm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 16:05:27.000000 oem2orm-0.3.2/oem2orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2022-11-29 16:05:27.000000 oem2orm-0.3.2/oem2orm/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6607 2022-11-29 16:05:27.000000 oem2orm-0.3.2/oem2orm/oep_compliance.py
--rw-r--r--   0 runner    (1001) docker     (122)    13794 2022-11-29 16:05:27.000000 oem2orm-0.3.2/oem2orm/oep_oedialect_oem2orm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-11-29 16:05:27.000000 oem2orm-0.3.2/oem2orm/postgresql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 16:05:38.918293 oem2orm-0.3.2/oem2orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      337 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-29 16:05:38.000000 oem2orm-0.3.2/oem2orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 16:05:38.918293 oem2orm-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2022-11-29 16:05:27.000000 oem2orm-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 14:58:20.000000 oem2orm-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-15 14:58:24.193353 oem2orm-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-15 14:58:20.000000 oem2orm-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/oem2orm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/oep_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/oep_oedialect_oem2orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/postgresql_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/oem2orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:58:24.193353 oem2orm-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-15 14:58:20.000000 oem2orm-0.3.3/setup.py
```

### Comparing `oem2orm-0.3.2/LICENSE` & `oem2orm-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oem2orm-0.3.2/PKG-INFO` & `oem2orm-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: oem2orm
-Version: 0.3.2
+Version: 0.3.3
 Summary: SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format
 Home-page: https://github.com/OpenEnergyPlatform/oem2orm
 Author: henhuy, jh-RLI
 Author-email: Hendrik.Huyskens@rl-institut.de
 Project-URL: Bug Reports, https://github.com/OpenEnergyPlatform/oem2orm/issues
 Project-URL: Source, https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sqlalchemy==1.3.14
+Requires-Dist: oedialect==1.1
+Requires-Dist: requests
+Requires-Dist: jmespath
+Requires-Dist: omi
+Requires-Dist: click
 
 # OEM to ORM
 
 Create database tables (and schema) from oemetadata json file(s)
 
 ## Installation:
 
@@ -32,15 +38,15 @@
 pipx install oem2orm
 `
 see [Pipx-Documentation](https://pypa.github.io/pipx/) for further information.
 
 
 ## Usage:
 
-This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergy-platform.org/).
+This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
 To use this tool with the OEP API you need to be signed up to the OEP since
 you need to provide an API-Token. 
 
 If you want to upload OEM that was officially reviewed you must clone the
 OEP data-preprocessing repository on [GitHub](https://github.com/OpenEnergyPlatform/data-preprocessing).
 The data-review folder contains all of the successfully reviewed OEM files.
```

### Comparing `oem2orm-0.3.2/README.md` & `oem2orm-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pipx install oem2orm
 `
 see [Pipx-Documentation](https://pypa.github.io/pipx/) for further information.
 
 
 ## Usage:
 
-This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergy-platform.org/).
+This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
 To use this tool with the OEP API you need to be signed up to the OEP since
 you need to provide an API-Token. 
 
 If you want to upload OEM that was officially reviewed you must clone the
 OEP data-preprocessing repository on [GitHub](https://github.com/OpenEnergyPlatform/data-preprocessing).
 The data-review folder contains all of the successfully reviewed OEM files.
```

### Comparing `oem2orm-0.3.2/oem2orm/main.py` & `oem2orm-0.3.3/oem2orm/main.py`

 * *Files identical despite different names*

### Comparing `oem2orm-0.3.2/oem2orm/oep_compliance.py` & `oem2orm-0.3.3/oem2orm/oep_compliance.py`

 * *Files identical despite different names*

### Comparing `oem2orm-0.3.2/oem2orm/oep_oedialect_oem2orm.py` & `oem2orm-0.3.3/oem2orm/oep_oedialect_oem2orm.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import re
 import requests
 
 import oedialect
 
 from oem2orm.postgresql_types import TYPES
 from oem2orm.oep_compliance import run_metadata_checks
+from oem2orm.settings import OEP_URL, OEP_API_URL
 
 # prepare connection string to connect via oep API
 CONNECTION_STRING = "{engine}://{user}:{token}@{host}"
 #
 DB = namedtuple("Database", ["engine", "metadata"])
 
 
@@ -34,30 +35,30 @@
     pass
 
 
 class MetadataError(Exception):
     pass
 
 
-def setup_logger():
+def setup_logger(logger_level: str = "Yes"):
     """
     Easy logging setup depending on user input. Provides a logger for INFO level logging.
     :return: logging.INFO or none
     """
-    logger_level = input("Display logging information[Yes] or [No]:")
+
     if re.fullmatch("[Yy]es", logger_level):
-        print("logging activated")
+        print("Logging activated")
         return logging.basicConfig(
             format="%(levelname)s:%(message)s", level=logging.INFO
         )
     elif re.fullmatch("[Nn]o", logger_level):
         pass
 
 
-def setup_db_connection(engine="postgresql+oedialect", host="openenergy-platform.org"):
+def setup_db_connection(engine="postgresql+oedialect", host=OEP_URL):
     """
     Create SQLAlchemy connection to Database API with Username and Token.
     Default is the OEP RESTful-API.
 
     :param engine: Database engine, default is postgresql
     :param host: API provider
     :return: DB(sa.engine, sa.metadata) namedtuple
@@ -77,17 +78,16 @@
     engine = sa.create_engine(conn_str)
     metadata = sa.MetaData(bind=engine)
     return DB(engine, metadata)
 
 
 def setupApiAction(schema, table, token=None):
     API_ACTION = namedtuple("API_Action", ["dest_url", "headers"])
-    OEP_URL = "https://openenergy-platform.org"
 
-    url = OEP_URL + "/api/v0/schema/{schema}/tables/{table}/meta/".format(
+    url = OEP_API_URL + "schema/{schema}/tables/{table}/meta/".format(
         schema=schema, table=table
     )
 
     token = token if token else setUserToken()
     headers = {
         "Authorization": "Token %s" % token,
         "Accept": "application/json",
@@ -103,25 +103,27 @@
     The tables can be a list of ORM.
 
     :param db: API
     :param tables: SQLAlchemy ORM objects (automatically retrieved from OEM json strings)
     :return: none
     """
     for table in tables:
+        logging.info(f"Working on table: {table}")
         if not db.engine.dialect.has_schema(db.engine, table.schema):
-            error_msg = f'The provided database schema: "{table.schema}" does not exist. Please use an existing schema'
+            error_msg = f'The provided database schema: "{table.schema}" does not exist. Please use an existing ' \
+                        f'schema from the `name` column from: {OEP_URL}/dataedit/schemas'
             logging.info(error_msg)
             raise DatabaseError(error_msg)
         else:
             if not db.engine.dialect.has_table(db.engine, table.name, table.schema):
                 try:
                     table.create(checkfirst=True)
                     logging.info(f"Created table {table.name}")
                 except oedialect.engine.ConnectionException as ce:
-                    error_msg = f'Error when uploading table "{table.name}".'
+                    error_msg = f'Error when uploading table "{table.name}". Reason: {ce}.'
                     logging.error(error_msg)
                     raise DatabaseError(error_msg) from ce
                 except sa.exc.ProgrammingError as pe:
                     error_msg = f'Table "{table.name}" already exists.'
                     logging.error(error_msg)
                     raise DatabaseError(error_msg) from pe
 
@@ -199,15 +201,15 @@
         }
         # Create columns:
         columns = []
         for field in jmespath.search("schema.fields[*]", table):
             # Get column type:
             try:
                 column_type = TYPES[field["type"]]
-            except KeyError:
+            except (KeyError, ValueError):
                 raise MetadataError(
                     "Unknown column type", field, field["type"], metadata_file
                 )
 
             if field["name"] in foreign_keys:
                 foreign_key = foreign_keys[field["name"]]
                 column = sa.Column(
@@ -264,15 +266,15 @@
     """
     api_open_schema = ["model_draft", "sandbox"]
 
     if oem_schema in api_open_schema:
         return True
     else:
         logging.info(
-            "The OEP-API does not allow to write un-reviewed data to another schema then model_draft or sandbox"
+            "The OEP-API does not allow to write un-reviewed data to another schema then 'model_draft' or 'sandbox'"
         )
         return False
 
 
 def select_oem_dir(oem_folder_name=None, filename=None):
     """
     Select the metadata directory or file that is used to generate the tables.
@@ -310,15 +312,15 @@
             raise
         tables.extend(md_tables)
 
     return order_tables_by_foreign_keys(tables)
 
 
 def load_json(filepath):
-    logging.info("reading %s" % filepath)
+    logging.info("Reading metadata: %s" % filepath)
     with open(filepath, "rb") as f:
         return json.load(f)
 
 
 def mdToDict(oem_folder_path, file_name=None):
     """
     Prepares the JSON String for the sql comment on table
@@ -369,26 +371,34 @@
 
 
 def api_updateMdOnTable(metadata, token=None):
     """ """
     schema = getTableSchemaNameFromOEM(metadata)[0]
     table = getTableSchemaNameFromOEM(metadata)[1]
 
-    logging.info("UPDATE METADATA")
+    logging.info(f"Update metadata on table: {table}")
     api_action = setupApiAction(schema, table, token)
     resp = requests.post(api_action.dest_url, json=metadata, headers=api_action.headers)
     if resp.status_code == 200:
-        logging.info("   ok.")
-        logging.info(api_action.dest_url)
+        logging.info(f"METADATA SUCCESSFULLY UPDATED: {table}")
+        logging.info(f"Link to updated metadata on OEP: {api_action.dest_url}")
     else:
-        error_msg = resp.json()
-        logging.info(error_msg)
-        logging.info("HTTP status code: ")
-        logging.info(resp.status_code)
-        raise MetadataError(f"Uploading of metadata failed. Response from OEP: {error_msg}")
+        oep_err_msg_header = re.search("<h3>(.*)</h3>", resp.text).group(1)
+        err_message = (
+            f"Uploading of metadata failed. HTTPS response from OEP: {resp.status_code}, Message: {oep_err_msg_header}, URL: {resp.url}"
+            ""
+        )
+        if not resp.text.startswith("{"):
+            raise MetadataError(
+                f"The response text doesn't seem to be a json: {resp.text[:40]}..... \n\n Please check "
+                f"that the table is already created on the OEP! \n {err_message}"
+            )
+        else:
+            # in case a json is returned and there is a json error
+            raise MetadataError(err_message, resp.json())
 
 
 def api_downloadMd(schema, table, token=None):
     """ """
     logging.info("DOWNLOAD_METADATA")
     api_action = setupApiAction(schema, table, token)
     res = requests.get(api_action.dest_url)
```

### Comparing `oem2orm-0.3.2/oem2orm/postgresql_types.py` & `oem2orm-0.3.3/oem2orm/postgresql_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         # not support with oedialect
         "double precision": psql.DOUBLE_PRECISION
         # "double precision array": sa.ARRAY("DOUBLE_PRECISION"),
 
     }
 
     def __getitem__(self, item):
+        if item is None:
+            raise ValueError("Field type is 'None'.")
         if item.split(" ")[-1] == "array":
             db_type = self.types[item[:-6]]
             return psql.ARRAY(db_type)
         else:
             return self.types[item]
```

### Comparing `oem2orm-0.3.2/oem2orm.egg-info/PKG-INFO` & `oem2orm-0.3.3/oem2orm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: oem2orm
-Version: 0.3.2
+Version: 0.3.3
 Summary: SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format
 Home-page: https://github.com/OpenEnergyPlatform/oem2orm
 Author: henhuy, jh-RLI
 Author-email: Hendrik.Huyskens@rl-institut.de
 Project-URL: Bug Reports, https://github.com/OpenEnergyPlatform/oem2orm/issues
 Project-URL: Source, https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sqlalchemy==1.3.14
+Requires-Dist: oedialect==1.1
+Requires-Dist: requests
+Requires-Dist: jmespath
+Requires-Dist: omi
+Requires-Dist: click
 
 # OEM to ORM
 
 Create database tables (and schema) from oemetadata json file(s)
 
 ## Installation:
 
@@ -32,15 +38,15 @@
 pipx install oem2orm
 `
 see [Pipx-Documentation](https://pypa.github.io/pipx/) for further information.
 
 
 ## Usage:
 
-This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergy-platform.org/).
+This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
 To use this tool with the OEP API you need to be signed up to the OEP since
 you need to provide an API-Token. 
 
 If you want to upload OEM that was officially reviewed you must clone the
 OEP data-preprocessing repository on [GitHub](https://github.com/OpenEnergyPlatform/data-preprocessing).
 The data-review folder contains all of the successfully reviewed OEM files.
```

### Comparing `oem2orm-0.3.2/setup.py` & `oem2orm-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oem2orm",
-    version="0.3.2",
+    version="0.3.3",
     author="henhuy, jh-RLI",
     author_email="Hendrik.Huyskens@rl-institut.de",
     description="SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OpenEnergyPlatform/oem2orm",
     packages=setuptools.find_packages(),
@@ -24,15 +24,15 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['sqlalchemy==1.3.14', 'oedialect', 'requests', 'jmespath', 'omi', 'click'],  # Optional
+    install_requires=['sqlalchemy==1.3.14', 'oedialect==1.1', 'requests', 'jmespath', 'omi', 'click'],  # Optional
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/OpenEnergyPlatform/oem2orm/issues',
         'Source': 'https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm',
     },
     entry_points={
         'console_scripts': ['oem2orm=oem2orm.main:cli'],
     }
```

