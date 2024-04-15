# Comparing `tmp/stadb-0.0.3.tar.gz` & `tmp/stadb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadb-0.0.3.tar", last modified: Thu Apr  4 14:36:30 2024, max compression
+gzip compressed data, was "stadb-0.0.4.tar", last modified: Mon Apr 15 10:50:50 2024, max compression
```

## Comparing `stadb-0.0.3.tar` & `stadb-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.3/LICENSE
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 14:36:30.600966 stadb-0.0.3/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-04 10:42:11.000000 stadb-0.0.3/README.md
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-04 14:36:22.000000 stadb-0.0.3/pyproject.toml
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-04 14:36:30.600966 stadb-0.0.3/setup.cfg
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/stadb/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.3/src/stadb/__init__.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.3/src/stadb/logger.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.3/src/stadb/postgresql.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    52882 2024-04-04 14:12:35.000000 stadb-0.0.3/src/stadb/sensorthings.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.3/src/stadb/timescaledb.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.3/src/stadb/utils.py
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 14:36:30.600966 stadb-0.0.3/src/stadb.egg-info/
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/SOURCES.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/dependency_links.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/requires.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-04 14:36:30.000000 stadb-0.0.3/src/stadb.egg-info/top_level.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.3/src/test.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.953537 stadb-0.0.4/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.4/LICENSE
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-15 10:50:50.953537 stadb-0.0.4/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-15 10:48:07.000000 stadb-0.0.4/README.md
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-15 10:48:07.000000 stadb-0.0.4/pyproject.toml
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-15 10:50:50.953537 stadb-0.0.4/setup.cfg
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.949537 stadb-0.0.4/src/
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.949537 stadb-0.0.4/src/stadb/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.4/src/stadb/__init__.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.4/src/stadb/logger.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.4/src/stadb/postgresql.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    42150 2024-04-15 10:50:18.000000 stadb-0.0.4/src/stadb/sensorthings.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.4/src/stadb/timescaledb.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.4/src/stadb/utils.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.953537 stadb-0.0.4/src/stadb.egg-info/
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/SOURCES.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/dependency_links.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/requires.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/top_level.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.4/src/test.py
```

### Comparing `stadb-0.0.3/LICENSE` & `stadb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stadb-0.0.3/PKG-INFO` & `stadb-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.3
+Version: 0.0.4
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.2
+* **version**: 0.0.4
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.3/README.md` & `stadb-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.2
+* **version**: 0.0.4
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.3/pyproject.toml` & `stadb-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 
 [project]
 
 name = "stadb"  # REQUIRED, is the only field that cannot be marked as dynamic.
-version = "0.0.3"  # REQUIRED, although can be dynamic
+version = "0.0.4"  # REQUIRED, although can be dynamic
 description = "SensorThings API database connector for advanced functionalities"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["sta", "setuptools", "development", "sensorthings"]
 
 authors = [
```

### Comparing `stadb-0.0.3/src/stadb/logger.py` & `stadb-0.0.4/src/stadb/logger.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.3/src/stadb/postgresql.py` & `stadb-0.0.4/src/stadb/postgresql.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.3/src/stadb/sensorthings.py` & `stadb-0.0.4/src/stadb/sensorthings.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,63 +4,28 @@
 author: Enoc Martínez
 institution: Universitat Politècnica de Catalunya (UPC)
 email: enoc.martinez@upc.edu
 license: MIT
 created: 4/10/23
 """
 
-
 from .postgresql import PgDatabaseConnector
 from .logger import LoggerSuperclass
 from .utils import reverse_dictionary, dataframe_to_dict, run_subprocess, merge_dataframes_by_columns
 import json
 import pandas as pd
 import numpy as np
 from .timescaledb import TimescaleDB
 import rich
 from rich.progress import Progress
 import time
 import os
 import gc
 
 
-def varname_from_datastream(ds_name):
-    """
-    Extracts a variable name from a datastream name. The datastream name must follow the following pattern:
-        <station>:<sensor>:<VARNAME>:<data_type>
-    :param ds_name:
-    :raises: SyntaxError if the patter doesn't match
-    :return: variable name
-    """
-    splitted = ds_name.split(":")
-    if len(splitted) != 4:
-        raise SyntaxError(f"Datastream name {ds_name} doesn't have the expected format!")
-    varname = splitted[2]
-    return varname
-
-
-def varname_from_datastream_dataframe(df, datastream_name):
-    """
-    Renames a dataframe from raw_data table (value, qc_flag) to variable names, e.g. if variable name TEMP, then
-    value->TEMP qc_flag->TEMP_qc
-    """
-    varname = varname_from_datastream(datastream_name)
-    varname_qc = varname + "_qc"
-    varname_std = varname + "_std"
-    df = df.rename(columns={"value": varname, "qc_flag": varname_qc, "stdev": varname_std})
-    return df, varname
-
-
-def varname_from_datastream(datastream_name):
-    """
-    Takes a raw data name (e.g. OBSEA:SBE37:PSAL:raw_data) to variable name (PSAL)
-    """
-    return datastream_name.split(":")[2]
-
-
 def rsync_files(host: str, folder, files: list):
     """
     Uses rsync to copy some files to a remote folder
     """
     assert type(host) is str, "invalid type"
     assert type(folder) is str, "invalid type"
     assert type(files) is list, "invalid type"
@@ -96,44 +61,33 @@
         if timescaledb:
             self.timescale = TimescaleDB(self, logger)
         else:
             self.timescale = None
 
         # This dicts provide a quick way to get the relations between elements in the database without doing a query
         # they are initialized with __initialize_dicts()
-        self.datastream_id_varname = {}      # key: datastream_id, value: variable name
         self.datastream_id_sensor_name = {}  # key: datastream_id, value: sensor name
-        self.sensor_id_name = {}             # key: sensor id, value: name
-        self.thing_id_name = {}             # key: sensor id, value: name
-        self.datastream_name_id = {}         # key: datastream name, value: datastream id
-        self.obs_prop_name_id = {}           # key: observed property name, value: observed property id
+        self.sensor_id_name = {}  # key: sensor id, value: name
+        self.thing_id_name = {}  # key: sensor id, value: name
+        self.datastream_name_id = {}  # key: datastream name, value: datastream id
+        self.obs_prop_name_id = {}  # key: observed property name, value: observed property id
 
         # dictionaries where sensors key is name and value is ID
         self.__initialize_dicts()
 
         # dictionaries where key is ID and value is name
         self.sensor_name_id = reverse_dictionary(self.sensor_id_name)
         self.datastream_id_name = reverse_dictionary(self.datastream_name_id)
         self.thing_name_id = reverse_dictionary(self.thing_id_name)
         self.obs_prop_id_name = reverse_dictionary(self.obs_prop_name_id)
         self.datastream_properties = self.get_datastream_properties()
 
         self.__last_observation_index = -1
         self.get_last_observation_id()
 
-    def sensor_var_from_datastream(self, datastream_id):
-        """
-        Returns the sensor name and variable name from a datastream_id
-        :param datastream_id: datastream ID
-        :returns: a tuple of sensor_name, varname
-        """
-        sensor_name = self.datastream_id_sensor_name[datastream_id]
-        varname = self.datastream_id_varname[datastream_id]
-        return sensor_name, varname
-
     def __initialize_dicts(self):
         """
         Initialize the dicts used for quickly access to relations without querying the database
         """
         self.info("Initializing internal structures...")
         # DATASTREAM -> SENSOR relation
         query = """
@@ -143,17 +97,14 @@
             where "DATASTREAMS"."SENSOR_ID" = "SENSORS"."ID" order by datastream_id asc;"""
         df = self.dataframe_from_query(query)
 
         # key: datastream_id ; value: sensor name
         self.datastream_id_sensor_name = dataframe_to_dict(df, "datastream_id", "sensor_name")
         datastream_name_dict = dataframe_to_dict(df, "datastream_id", "datastream_name")
 
-        # convert datastream name into variable name "OBSEA:SBE16:TEMP:raw_data -> TEMP
-        self.datastream_id_varname = {key: name.split(":")[2] for key, name in datastream_name_dict.items()}
-
         # SENSOR ID -> SENSOR NAME
         self.sensor_id_name = self.get_sensors()  # key: sensor_id, value: sensor_name
         self.thing_id_name = self.get_things()  # key: sensor_id, value: sensor_name
 
         # DATASTREAM_NAME -> DATASTREAM_ID
         df = self.dataframe_from_query(f'select "ID", "NAME" from "DATASTREAMS";')
         self.datastream_name_id = dataframe_to_dict(df, "NAME", "ID")
@@ -171,80 +122,14 @@
         :return: dataframe with datastreams ID, NAME and PROPERTIES
         """
         query = (f'select "ID" as id , "NAME" as name, "THING_ID" as thing_id, "OBS_PROPERTY_ID" AS obs_prop_id,'
                  f' "PROPERTIES" as properties from "DATASTREAMS" where "SENSOR_ID" = {sensor_id};')
         df = self.dataframe_from_query(query)
         return df
 
-    def get_sensor_qc_metadata(self, name: str):
-        """
-        Returns an object with all the necessary information to apply QC to all variables from the sensor
-        :return:
-        """
-        sensor_id = self.sensor_id_name[name]
-        data = {
-            "name": name,
-            "id": int(sensor_id),  # from numpy.int64 to regular int
-            "variables": {}
-        }
-        query = 'select "ID" as id , "NAME" as name, "PROPERTIES" as properties ' \
-                f'from "DATASTREAMS" where "SENSOR_ID" = {sensor_id};'
-        df = self.dataframe_from_query(query)
-        for _, row in df.iterrows():
-            ds_name = row["name"]
-            properties = row["properties"]
-            if "rawSensorData" not in properties.keys() or not properties["rawSensorData"]:
-                # if rawSensorData = False of if there is no rawSensorData flag, just ignore this datastream
-                self.debug(f"Ignoring datastream {ds_name}")
-                continue
-            self.info(f"Loading configuration for datastream {ds_name}")
-            varname = varname_from_datastream(ds_name)
-
-            qc_config = {}
-            try:
-                qc_config = properties["QualityControl"]["configuration"]
-            except KeyError as e:
-                self.warning(f"Quality Control for variable {varname} not found!")
-                self.warning(f"KeyError: {e}")
-
-            data["variables"][varname] = {
-                "variable_name": varname,
-                "datastream_name": ds_name,
-                "datastream_id": int(self.datastream_name_id[ds_name]),
-                "quality_control": qc_config
-            }
-        return data
-
-    def get_qc_config(self, raw_sensor_data_flag="rawSensorData") -> dict:
-        """
-        Gets the QC config for all sensors from the database and stores it in a dictionary
-        :return: dict with the configuration
-        """
-        sensors = {}
-
-        for sensor, sensor_id in self.sensor_id_name.items():
-            sensors[sensor] = {"datastreams": {}, "id": sensor_id, "name": sensor}
-
-            # Select Datastreams belonging to a sensor and expand rawData flag and quality control config
-            q = f'select "ID" as id, "NAME" as name, ("PROPERTIES"->>\'QualityControl\') as qc_config, ' \
-                f'("PROPERTIES"->>\'{raw_sensor_data_flag}\')::BOOLEAN as is_raw_data ' \
-                f' from "DATASTREAMS" where "SENSOR_ID" = {sensor_id};'
-
-            df = self.dataframe_from_query(q, debug=False)
-
-            for index, row in df.iterrows():
-                if not row["is_raw_data"]:
-                    self.warning(f"[yellow] ignoring datastream {row['name']}")
-                    continue
-
-                sensors[sensor]["datastreams"][row["id"]] = {
-                    "name": row["name"],
-                    "qc_config": json.loads(row["qc_config"])
-                }
-
     def get_sensors(self):
         """
         Returns a dictionary with sensor's names and their id, e.g. {"SBE37": 3, "AWAC": 5}
         :return: dictionary
         """
         df = self.dataframe_from_query('select "ID", "NAME" from "SENSORS";')
         return dataframe_to_dict(df, "NAME", "ID")
@@ -319,51 +204,14 @@
             elif thing_id in thing_foi.keys() and thing_foi[thing_id]:  # could be null...
                 datastream_features[datastream_id] = thing_foi[thing_id]
                 continue
             else:
                 self.warning(f"Could not get FOI for datastream {datastream_id}! this may crash the code later")
         return datastream_features
 
-    def get_last_datastream_timestamp(self, datastream_id):
-        """
-        Returns a timestamp (pd.Timestamp) with the last data point from a certain datastream. If there's no data
-        return None or pd.Timestamp
-        """
-
-        properties = self.datastream_properties[datastream_id]
-        if properties["rawSensorData"]:
-            query = f"select timestamp from {self.raw_data_table} where datastream_id = {datastream_id} order by" \
-                    f" timestamp desc limit 1;"
-            row = self.dataframe_from_query(query)
-
-        else:
-            query = f'select "PHENOMENON_TIME_START" as timestamp from "OBSERVATIONS" where "DATASTREAM_ID" = {datastream_id} ' \
-                    f'order by "PHENOMENON_TIME_START" desc limit 1;'
-            row = self.dataframe_from_query(query)
-
-        if row.empty:
-            return None
-
-        return row["timestamp"][0]
-
-    def get_last_datastream_data(self, datastream_id, hours):
-        """
-        Gets the last N hours of data from a datastream
-        :param datastream_id: ID of the datastream
-        :param hours: get last X hours
-        :return: dataframe with the data
-        """
-        query = f"select timestamp, value, qc_flag from raw_data where datastream_id = {datastream_id} " \
-                f"and timestamp > now() - INTERVAL '{hours} hours' order by timestamp asc;"
-        df = self.dataframe_from_query(query)
-        df["timestamp"] = pd.to_datetime(df["timestamp"], utc=True)
-        df.set_index("timestamp", inplace=True)
-        df.sort_index(inplace=True)
-        return df
-
     def get_data(self, identifier, time_start: str, time_end: str):
         """
         Access the 0BSERVATIONS data table and exports all data between time_start and time_end
         :param identifier: datasream name (str) or datastream id (int)
         :param time_start: start time
         :param time_end: end time  (not included)
         """
@@ -385,106 +233,14 @@
         df = self.dataframe_from_query(query)
         df["timestamp"] = pd.to_datetime(df["timestamp"], utc=True)
         if not df.empty and np.isnan(df["stdev"].max()):
             self.debug(f"Dropping stdev for {self.datastream_id_name[identifier]}")
             del df["stdev"]
         return df.set_index("timestamp")
 
-    def dataframe_from_datastream(self, datastream_id: int, time_start: pd.Timestamp, time_end: pd.Timestamp):
-        """
-        Takes the ID of a datastream and exports its data to a dataframe.
-        """
-        df = self.dataframe_from_query(f'select "PROPERTIES" from "DATASTREAMS" where "ID"={datastream_id};')
-        if df.empty:
-            raise ValueError(f"Datastream with ID={datastream_id} not found in database!")
-        properties = df.values[0][0]  # only one value with the properties in JSON format
-        # if the datastream has rawSensorData=True in properties, export from raw_data
-        if self.timescale and properties["rawSensorData"]:
-            df = self.timescale.get_raw_data(datastream_id, time_start, time_end)
-        else:  # otherwise export from observations
-            df = self.get_data(datastream_id, time_start, time_end)
-        df, _ = varname_from_datastream_dataframe(df, self.datastream_id_name[datastream_id])
-        return df
-
-    def get_dataset(self, sensor:str, station_name:str, options: dict, time_start: pd.Timestamp, time_end:pd.Timestamp,
-                    variables: list=[])-> pd.DataFrame:
-        """
-        Gets all data from a sensor deployed at a certain station from time_start to time_end. If variables is specified
-        only a subset of variables will be returned.
-
-        options is a dict with "rawData" key (true/false) and if False, averagePeriod MUST be specified like:
-            {"rawData": false, "averagePeriod": "30min"}
-                OR
-            {"rawData": true}
-
-        :param sensor: sensor name
-        :param station: station name
-        :param time_start:
-        :param time_end:
-        :param options: dict with rawData and optionally averagePeriod.
-        :param variables: list of variable names
-        :return:
-        """
-        # Make sure options are correct
-        assert("rawData" in options.keys())
-        if not options["rawData"]:
-            assert("averagePeriod" in options.keys())
-
-        raw_data = options["rawData"]
-
-        if variables:
-            rich.print(f"Keeping only variables: {variables}")
-
-        sensor_id = self.sensor_id_name[sensor]
-        station_id = self.thing_id_name[station_name]
-        # Get all datastreams for a sensor
-        datastreams = self.get_sensor_datastreams(sensor_id)
-        # Keep only datastreams at a specific station
-        datastreams = datastreams[datastreams["thing_id"] == station_id]
-
-        # Drop datastreams with variables that are not in the list
-        if variables:
-            variable_ids = [self.obs_prop_name_id[v] for v in variables]
-            rich.print(f"variables {variable_ids}")
-            # keep only variables in list
-            all_variable_ids = np.unique(datastreams["obs_prop_id"].values)
-            remove_this = [var_id for var_id in all_variable_ids if var_id not in variable_ids]
-            for remove_id in remove_this:
-                datastreams = datastreams[datastreams["obs_prop_id"] != remove_id]  # keep others
-
-        # Keep only datastreams that match data type
-        remove_idxs = []
-        for idx, row in datastreams.iterrows():
-            if raw_data:
-                if not row["properties"]["rawSensorData"]:
-                    remove_idxs.append(idx)
-            else: # Keep only those variables that are not raw_data and whose period matches the data_type
-                if row["properties"]["rawSensorData"]:  # Do not keep raw data
-                    remove_idxs.append(idx)
-                elif row["properties"]["averagePeriod"] != options["averagePeriod"]:  # do not keep data with different period
-                    remove_idxs.append(idx)
-
-        datastreams = datastreams.drop(remove_idxs)
-
-        # Query data for every datastream
-        data = []
-        for idx, row in datastreams.iterrows():
-            datastream_id = row["id"]
-            obs_prop_id = row["obs_prop_id"]
-          #  df = self.get_data(datastream_id, time_start, time_end)
-            df = self.dataframe_from_datastream(datastream_id, time_start, time_end)
-
-            varname = self.obs_prop_id_name[obs_prop_id]
-            rename = {"value": varname, "qc_flag": varname + "_QC"}
-            if "stdev" in df.columns:
-                rename["stdev"] = varname  + "_SD"
-            df = df.rename(columns=rename)
-            data.append(df)
-        return merge_dataframes_by_columns(data)
-
     def check_if_table_exists(self, view_name):
         """
         Checks if a view already exists
         :param view_name: database view to check if exists
         :return: True if exists, False if it doesn't
         """
         # Select all from information_schema
@@ -742,15 +498,16 @@
             foi_id = self.post_via_api(df, url, df.iloc[0], datastreams, avg_period=avg_period, parameters={})
             df = df.iloc[1:-1]
 
         rich.print("Splitting input dataframe into smaller ones")
         rows = int(max_rows / len(datastreams))
         dataframes = slice_dataframes(df, max_rows=rows)
 
-        files = self.dataframes_to_observations_csv(dataframes, datastreams, tmp_folder, foi_id, avg_period=avg_period, profile=profile)
+        files = self.dataframes_to_observations_csv(dataframes, datastreams, tmp_folder, foi_id, avg_period=avg_period,
+                                                    profile=profile)
         rich.print(f"Generating all files took {time.time() - init:0.02f} seconds")
 
         if self.host != "localhost" and self.host != "127.0.0.1":
             t = time.time()
             rich.print("rsync files to remote server...", end="")
             rsync_files(self.host, tmp_folder, files)
             rich.print(f"[green]done![/green] took {time.time() - t:.02f} s")
@@ -775,15 +532,16 @@
             for file in files:
                 os.remove(file)
                 progress.advance(task1, advance=1)
 
         if self.host != "localhost" and self.host != "127.0.0.1":
             rm_remote_files(self.host, files)
 
-    def dataframes_to_observations_csv(self, dataframes: list, column_mapper: dict, folder: str, feature_id: int, avg_period:str = "", profile=False):
+    def dataframes_to_observations_csv(self, dataframes: list, column_mapper: dict, folder: str, feature_id: int,
+                                       avg_period: str = "", profile=False):
         """
         Write dataframes into local csv files ready for sql copy following the syntax in table OBSERVATIONS
         """
         files = []
         i = 0
         with Progress() as progress:
             task = progress.add_task("converting dataframes to OBSERVATIONS csv", total=len(dataframes))
@@ -826,43 +584,42 @@
                 file = os.path.join(folder, f"timeseries_copy_{i:04d}.csv")
                 i += 1
                 rich.print(f"format timeseries CSV {i:04d} of {len(dataframes)}")
                 self.format_detections_csv(dataframe, file)
                 files.append(file)
         return files
 
-    def dataframes_to_files_csv(self, dataframes:list, folder):
+    def dataframes_to_files_csv(self, dataframes: list, folder):
         i = 0
         files = []
         with Progress() as progress:
             task = progress.add_task("converting data to 'files' csv", total=len(dataframes))
             for dataframe in dataframes:
                 progress.advance(task, 1)
                 file = os.path.join(folder, f"files_copy_{i:04d}.csv")
                 i += 1
                 rich.print(f"format timeseries CSV {i:04d} of {len(dataframes)}")
                 self.format_files_csv(dataframe, file)
                 files.append(file)
         return files
 
-    def dataframes_to_inference_csv(self, dataframes:list, folder):
+    def dataframes_to_inference_csv(self, dataframes: list, folder):
         i = 0
         files = []
         with Progress() as progress:
             task = progress.add_task("converting data to 'inference' csv", total=len(dataframes))
             for dataframe in dataframes:
                 progress.advance(task, 1)
                 file = os.path.join(folder, f"files_copy_{i:04d}.csv")
                 i += 1
                 rich.print(f"format timeseries CSV {i:04d} of {len(dataframes)}")
                 self.format_inference_csv(dataframe, file)
                 files.append(file)
         return files
 
-
     def dataframes_to_profile_csv(self, dataframes: list, column_mapper: dict, folder: str):
         """
         Write dataframes into local csv files ready for sql copy following the syntax in table OBSERVATIONS
         """
         i = 0
         files = []
         with Progress() as progress:
@@ -1111,15 +868,15 @@
         df["ID"] = np.arange(0, len(df.index.values), dtype=int) + self.__last_observation_index + 1
         self.__last_observation_index = df["ID"].values[-1]
 
         # Keep only columns as in the Database
 
         df = df[["PHENOMENON_TIME_START", "PHENOMENON_TIME_END", "RESULT_TIME", "RESULT_TYPE", "RESULT_NUMBER",
                  "RESULT_BOOLEAN", "RESULT_JSON", "RESULT_STRING", "RESULT_QUALITY", "VALID_TIME_START",
-                 "VALID_TIME_END", "PARAMETERS", "DATASTREAM_ID",  "FEATURE_ID", "ID"]]
+                 "VALID_TIME_END", "PARAMETERS", "DATASTREAM_ID", "FEATURE_ID", "ID"]]
         df.to_csv(filename, index=False)
 
     def format_inference_csv(self, df_in, filename):
         """
         Takes a dataframe and arranges it accordingly to the OBSERVATIONS table from a SensorThings API, preparing the
         data to be inserted by a COPY statement
         :param df_in: input dataframe
@@ -1170,15 +927,15 @@
         df["ID"] = np.arange(0, len(df.index.values), dtype=int) + self.__last_observation_index + 1
         self.__last_observation_index = df["ID"].values[-1]
 
         # Keep only columns as in the Database
 
         df = df[["PHENOMENON_TIME_START", "PHENOMENON_TIME_END", "RESULT_TIME", "RESULT_TYPE", "RESULT_NUMBER",
                  "RESULT_BOOLEAN", "RESULT_JSON", "RESULT_STRING", "RESULT_QUALITY", "VALID_TIME_START",
-                 "VALID_TIME_END", "PARAMETERS", "DATASTREAM_ID",  "FEATURE_ID", "ID"]]
+                 "VALID_TIME_END", "PARAMETERS", "DATASTREAM_ID", "FEATURE_ID", "ID"]]
         df.to_csv(filename, index=False)
 
     def sql_copy_csv(self, filename, table="OBSERVATIONS", delimiter=","):
         """
         Execute a COPY query to copy from a local CSV file to a database
         :return:
         """
```

### Comparing `stadb-0.0.3/src/stadb/timescaledb.py` & `stadb-0.0.4/src/stadb/timescaledb.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.3/src/stadb/utils.py` & `stadb-0.0.4/src/stadb/utils.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.3/src/stadb.egg-info/PKG-INFO` & `stadb-0.0.4/src/stadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.3
+Version: 0.0.4
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.2
+* **version**: 0.0.4
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

