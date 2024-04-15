# Comparing `tmp/FM13_transform-0.0.3.tar.gz` & `tmp/fm13_transform-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM13_transform-0.0.3.tar", last modified: Fri Apr  5 18:27:41 2024, max compression
+gzip compressed data, was "fm13_transform-0.0.4.tar", last modified: Mon Apr 15 19:43:10 2024, max compression
```

## Comparing `FM13_transform-0.0.3.tar` & `fm13_transform-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:27:41.503158 FM13_transform-0.0.3/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-04-05 17:41:39.000000 FM13_transform-0.0.3/MANIFEST.in
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 18:27:41.502158 FM13_transform-0.0.3/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:52:09.000000 FM13_transform-0.0.3/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      729 2024-04-05 18:27:30.000000 FM13_transform-0.0.3/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-04-05 17:42:44.000000 FM13_transform-0.0.3/requirements.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 18:27:41.503158 FM13_transform-0.0.3/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:27:41.499158 FM13_transform-0.0.3/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:27:41.500158 FM13_transform-0.0.3/src/FM13_transform/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:27.000000 FM13_transform-0.0.3/src/FM13_transform/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    84266 2024-04-05 18:27:18.000000 FM13_transform-0.0.3/src/FM13_transform/data2bufr.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:27:41.502158 FM13_transform-0.0.3/src/FM13_transform/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:59.000000 FM13_transform-0.0.3/src/FM13_transform/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    14244 2024-04-05 17:37:39.000000 FM13_transform-0.0.3/src/FM13_transform/resources/synop-mappings-308009.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-05 18:27:41.502158 FM13_transform-0.0.3/src/FM13_transform.egg-info/
--rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      565 2024-04-05 18:27:41.000000 FM13_transform-0.0.3/src/FM13_transform.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      422 2024-04-05 18:27:41.000000 FM13_transform-0.0.3/src/FM13_transform.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-04-05 18:27:41.000000 FM13_transform-0.0.3/src/FM13_transform.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-05 18:27:41.000000 FM13_transform-0.0.3/src/FM13_transform.egg-info/requires.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-04-05 18:27:41.000000 FM13_transform-0.0.3/src/FM13_transform.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-15 19:43:10.306928 fm13_transform-0.0.4/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       43 2024-04-05 17:41:39.000000 fm13_transform-0.0.4/MANIFEST.in
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      622 2024-04-15 19:43:10.305928 fm13_transform-0.0.4/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:52:09.000000 fm13_transform-0.0.4/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      805 2024-04-15 19:42:35.000000 fm13_transform-0.0.4/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       37 2024-04-05 17:42:44.000000 fm13_transform-0.0.4/requirements.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-15 19:43:10.306928 fm13_transform-0.0.4/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-15 19:43:10.302928 fm13_transform-0.0.4/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-15 19:43:10.303928 fm13_transform-0.0.4/src/FM13_transform/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:27.000000 fm13_transform-0.0.4/src/FM13_transform/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    85110 2024-04-15 19:41:44.000000 fm13_transform-0.0.4/src/FM13_transform/data2bufr.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-15 19:43:10.305928 fm13_transform-0.0.4/src/FM13_transform/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-03-29 16:53:59.000000 fm13_transform-0.0.4/src/FM13_transform/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    13902 2024-04-15 19:29:58.000000 fm13_transform-0.0.4/src/FM13_transform/resources/synop-mappings-308009.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2024-04-15 19:43:10.305928 fm13_transform-0.0.4/src/FM13_transform.egg-info/
+-rw-r--r--   0 alexander.thompson  (1013) alexander.thompson  (1013)      622 2024-04-15 19:43:10.000000 fm13_transform-0.0.4/src/FM13_transform.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      422 2024-04-15 19:43:10.000000 fm13_transform-0.0.4/src/FM13_transform.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2024-04-15 19:43:10.000000 fm13_transform-0.0.4/src/FM13_transform.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2024-04-15 19:43:10.000000 fm13_transform-0.0.4/src/FM13_transform.egg-info/requires.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       15 2024-04-15 19:43:10.000000 fm13_transform-0.0.4/src/FM13_transform.egg-info/top_level.txt
```

### Comparing `FM13_transform-0.0.3/PKG-INFO` & `fm13_transform-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FM13_transform
-Version: 0.0.3
-Summary: Package for converting FM13 SYNOP to BUFR4
-Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>
+Version: 0.0.4
+Summary: Package for converting FM13 SYNOP to BUFR4 and GeoJSON
+Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>, Alex Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP SHIP,FM-13,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: csv2bufr
```

### Comparing `FM13_transform-0.0.3/src/FM13_transform/data2bufr.py` & `fm13_transform-0.0.4/src/FM13_transform/data2bufr.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,24 +152,24 @@
          'precipitation_s3', 'ps3_time_period', 'precipitation_24h',
          'highest_gust_1', 'highest_gust_2']
 
 # Build the dictionary template
 synop_template = dict.fromkeys(_keys)
 
 THISDIR = os.path.dirname(os.path.realpath(__file__))
-# MAPPINGS_307080 = f"{THISDIR}{os.sep}resources{os.sep}synop-mappings-307080.json"  # noqa
-# MAPPINGS_307096 = f"{THISDIR}{os.sep}resources{os.sep}synop-mappings-307096.json"  # noqa
+MAPPINGS_307080 = f"{THISDIR}{os.sep}resources{os.sep}synop-mappings-307080.json"  # noqa
+MAPPINGS_307096 = f"{THISDIR}{os.sep}resources{os.sep}synop-mappings-307096.json"  # noqa
 MAPPINGS_308009 = f"{THISDIR}{os.sep}resources{os.sep}synop-mappings-308009.json"  # noqa
 
 
 # Load template mappings files, this will be updated for each message.
-# with open(MAPPINGS_307080) as fh:
-#     _mapping_307080 = json.load(fh)
-# with open(MAPPINGS_307096) as fh:
-#     _mapping_307096 = json.load(fh)
+with open(MAPPINGS_307080) as fh:
+    _mapping_307080 = json.load(fh)
+with open(MAPPINGS_307096) as fh:
+    _mapping_307096 = json.load(fh)
 with open(MAPPINGS_308009) as fh:
     _mapping_308009 = json.load(fh)
 
 def parse_synop(message: str, year: int, month: int) -> dict:
     """
     This function parses a SYNOP message, storing and returning the
     data as a Python dictionary.
@@ -186,14 +186,15 @@
     # Get the full output decoded message from the pymetdecoder package
     try:
         decoded = synop.SYNOP().decode(message)
     except Exception as e:
         LOGGER.error("Unable to decode the SYNOP message.")
         raise e
 
+    '''pprint(decoded)'''
     # Get the template dictionary to be filled
     output = deepcopy(synop_template)
 
     # SECTIONS 0 AND 1
 
     # The following do not need to be converted
     output['report_type'] = message[0:4]
@@ -255,109 +256,141 @@
             output['wet_bulb_temperature'] = \
                 round(decoded['wet_bulb_temperature']['value'] + 273.15, 2)
         except Exception:
             output['wet_bulb_temperature'] = None
     else:
         output['wet_bulb_temperature'] = None
 
-    if decoded.get('ice_accretion').get('thickness') is not None:
-        try:
-            output['iceDepositThickness'] = \
-                round(decoded['ice_accretion']['thickness']['value']/100, 2)
-        except Exception:
+
+    try: 
+        if decoded.get('ice_accretion').get('thickness') is not None:
+            try:
+                output['iceDepositThickness'] = \
+                    round(decoded['ice_accretion']['thickness']['value']/100, 2)
+            except Exception:
+                output['iceDepositThickness'] = None
+        else:
             output['iceDepositThickness'] = None
-    else:
+    except Exception:
         output['iceDepositThickness'] = None
 
-    if decoded.get('ice_accretion').get('rate') is not None:
-        try:
-            output['rateOfIceAccretionEstimated'] = \
-                decoded['ice_accretion']['rate']['_code']
-        except Exception:
+    try:
+        if decoded.get('ice_accretion').get('rate') is not None:
+            try:
+                output['rateOfIceAccretionEstimated'] = \
+                    decoded['ice_accretion']['rate']['_code']
+            except Exception:
+                output['rateOfIceAccretionEstimated'] = None
+        else:
             output['rateOfIceAccretionEstimated'] = None
-    else:
+    except Exception:
         output['rateOfIceAccretionEstimated'] = None
 
-    if decoded.get('ice_accretion').get('source') is not None:
-        try:
-            output['causeOfIceAccretion'] = \
-                decoded['ice_accretion']['source']['_code']
-        except Exception:
+    try:
+        if decoded.get('ice_accretion').get('source') is not None:
+            try:
+                output['causeOfIceAccretion'] = \
+                    decoded['ice_accretion']['source']['_code']
+            except Exception:
+                output['causeOfIceAccretion'] = None
+        else:
             output['causeOfIceAccretion'] = None
-    else:
+    except Exception:
         output['causeOfIceAccretion'] = None
 
-    if decoded.get('sea_land_ice').get('concentration') is not None:
-        try:
-            output['seaIceConcentration'] = \
-                decoded['sea_land_ice']['concentration']['value']
-        except Exception:
+    try: 
+        if decoded.get('sea_land_ice').get('concentration') is not None:
+            try:
+                output['seaIceConcentration'] = \
+                    decoded['sea_land_ice']['concentration']['value']
+            except Exception:
+                output['seaIceConcentration'] = None
+        else:
             output['seaIceConcentration'] = None
-    else:
+    except Exception:
         output['seaIceConcentration'] = None
 
-    if decoded.get('sea_land_ice').get('land_origin') is not None:
-        try:
-            output['amountAndTypeOfIce'] = \
-                decoded['sea_land_ice']['land_origin']['value']
-        except Exception:
+    try:
+        if decoded.get('sea_land_ice').get('land_origin') is not None:
+            try:
+                output['amountAndTypeOfIce'] = \
+                    decoded['sea_land_ice']['land_origin']['value']
+            except Exception:
+                output['amountAndTypeOfIce'] = None
+        else:
             output['amountAndTypeOfIce'] = None
-    else:
+    except Exception:
         output['amountAndTypeOfIce'] = None
 
-    if decoded.get('sea_land_ice').get('condition_trend') is not None:
-        try:
-            output['iceSituation'] = \
-                decoded['sea_land_ice']['condition_trend']['value']
-        except Exception:
+    try:
+        if decoded.get('sea_land_ice').get('condition_trend') is not None:
+            try:
+                output['iceSituation'] = \
+                    decoded['sea_land_ice']['condition_trend']['value']
+            except Exception:
+                output['iceSituation'] = None
+        else:
             output['iceSituation'] = None
-    else:
+    except Exception:
         output['iceSituation'] = None
 
-    if decoded.get('sea_land_ice').get('development') is not None:
-        try:
-            output['iceDevelopment'] = \
-                decoded['sea_land_ice']['development']['value']
-        except Exception:
+
+    try:
+        if decoded.get('sea_land_ice').get('development') is not None:
+            try:
+                output['iceDevelopment'] = \
+                    decoded['sea_land_ice']['development']['value']
+            except Exception:
+                output['iceDevelopment'] = None
+        else:
             output['iceDevelopment'] = None
-    else:
+    except Exception:
         output['iceDevelopment'] = None
 
-    if decoded.get('sea_land_ice').get('direction') is not None:
-        try:
-            output['iceEdgeBearing'] = \
-                decoded['sea_land_ice']['direction']['_code']
-        except Exception:
+    try:
+        if decoded.get('sea_land_ice').get('direction') is not None:
+            try:
+                output['iceEdgeBearing'] = \
+                    decoded['sea_land_ice']['direction']['_code']
+            except Exception:
+                output['iceEdgeBearing'] = None
+        else:
             output['iceEdgeBearing'] = None
-    else:
+    except Exception:
         output['iceEdgeBearing'] = None
 
-    if decoded.get('sea_surface_temperature').get('measurement_type') is not None:
-        try:
-            measurement_type = decoded.get('sea_surface_temperature').get('measurement_type').get('_code')
-            if measurement_type in [0,1]:
-                output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 0
-            elif measurement_type in [2,3]:
-                output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 1
-            elif measurement_type in [4,5]:
-                output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 2
-            else:
-                output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 14
-        except Exception:
+    try:
+        if decoded.get('sea_surface_temperature').get('measurement_type') is not None:
+            try:
+                measurement_type = decoded.get('sea_surface_temperature').get('measurement_type').get('_code')
+                if measurement_type in [0,1]:
+                    output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 0
+                elif measurement_type in [2,3]:
+                    output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 1
+                elif measurement_type in [4,5]:
+                    output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 2
+                else:
+                    output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 14
+            except Exception:
+                output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 15
+        else:
             output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 15
-    else:
+    except Exception:
         output['methodOfWaterTemperatureAndOrOrSalinityMeasurement'] = 15
 
-    if decoded.get('sea_surface_temperature').get('value') is not None:
-        try:
-            output['oceanographicWaterTemperature'] = \
-                round(decoded['sea_surface_temperature']['value'] + 273.15, 2)
-        except Exception:
+    try:
+        if decoded.get('sea_surface_temperature').get('value') is not None:
+            try:
+                output['oceanographicWaterTemperature'] = \
+                    round(decoded['sea_surface_temperature']['value'] + 273.15, 2)
+            except Exception:
+                output['oceanographicWaterTemperature'] = None
+        else:
             output['oceanographicWaterTemperature'] = None
-    else:
+    except Exception:
         output['oceanographicWaterTemperature'] = None
 
     if decoded.get('wind_waves') is not None:
         try:
             for windWave in decoded.get('wind_waves'):
                 if windWave['instrumental'] == True:
                     output['periodOfWaves'] = \
@@ -482,15 +515,15 @@
     else:
         output['template'] = 307080
 
     '''here just choose the template as 308009'''
     output['template'] = 308009
 
     if decoded.get('callsign') is not None:
-        pprint(decoded)
+        '''pprint(decoded)'''
         try:
             tsi = decoded['callsign']['value']
             output['station_id'] = tsi
             output['block_no'] = tsi[0:2]
             output['station_no'] = tsi[2:5]
         except Exception:
             tsi = None
@@ -1571,15 +1604,15 @@
     #                                     f" {tsi} in station list file"))
     #             tsi_mapping[tsi] = wsi
     #         except Exception as e:
     #             LOGGER.error(e)
     #             error_msgs.append(str(e))
 
     #     fh.close()
-        # metadata = metadata_dict[wsi]
+    #     # metadata = metadata_dict[wsi]
     # else:
     #     LOGGER.error("Invalid metadata")
     #     raise ValueError("Invalid metadata")
 
     # ===========================================
     # Split the data by the end of message signal
     # ===========================================
@@ -1690,93 +1723,94 @@
                 continue
 
             # Now determine and load the appropriate mappings
             # file depending on the value of the wind indicator.
             # This will be updated for each message.
             '''msg is the synop parser output.'''
             bufr_template = msg['template']
-            # if bufr_template == 307096:
-            #     # Get mapping template, this needs to be
-            #     # reloaded everytime as each SYNOP can have a
-            #     # different number of replications
-            #     mapping = deepcopy(_mapping_307096)
-            # else:
-            #     # Get mapping template, this needs to be
-            #     # reloaded everytime as each SYNOP can have a
-            #     # different number of replications
-            #     mapping = deepcopy(_mapping_307080)
+            if bufr_template == 307096:
+                # Get mapping template, this needs to be
+                # reloaded everytime as each SYNOP can have a
+                # different number of replications
+                mapping = deepcopy(_mapping_307096)
+            else:
+                # Get mapping template, this needs to be
+                # reloaded everytime as each SYNOP can have a
+                # different number of replications
+                mapping = deepcopy(_mapping_307080)
             mapping = deepcopy(_mapping_308009)
             # set WSI
-            # try:
-            #     wsi = tsi_mapping[tsi]
-            # except Exception:
-            #     conversion_success[tsi] = False
-            #     LOGGER.warning(f"Station {tsi} not found in station file")
-            #     warning_msgs.append(f"Station {tsi} not found in station file")
-            #     result = {
-            #         "_meta": {
-            #             "id": None,
-            #             "geometry": None,
-            #             "properties": {
-            #                 "md5": None,
-            #                 "wigos_station_identifier": None,
-            #                 "datetime": None,
-            #                 "originating_centre": None,
-            #                 "data_category": None
-            #             },
-            #             "result": {
-            #                 "code": FAILED,
-            #                 "message": "Error encoding, BUFR set to None",
-            #                 "warnings": warning_msgs,
-            #                 "errors": error_msgs
-            #             },
-            #             "template": None,
-            #             "csv": None
-            #         }
-            #     }
-            #     yield result
-            #     # Reset warning and error messages array for next iteration
-            #     warning_msgs = []
-            #     error_msgs = []
-            #     continue
+            try:
+                '''wsi = tsi_mapping[tsi]'''
+                wsi = '0-20000-0-ZSUY'
+            except Exception:
+                conversion_success[tsi] = False
+                LOGGER.warning(f"Station {tsi} not found in station file")
+                warning_msgs.append(f"Station {tsi} not found in station file")
+                result = {
+                    "_meta": {
+                        "id": None,
+                        "geometry": None,
+                        "properties": {
+                            "md5": None,
+                            "wigos_station_identifier": None,
+                            "datetime": None,
+                            "originating_centre": None,
+                            "data_category": None
+                        },
+                        "result": {
+                            "code": FAILED,
+                            "message": "Error encoding, BUFR set to None",
+                            "warnings": warning_msgs,
+                            "errors": error_msgs
+                        },
+                        "template": None,
+                        "csv": None
+                    }
+                }
+                yield result
+                # Reset warning and error messages array for next iteration
+                warning_msgs = []
+                error_msgs = []
+                continue
 
             # parse WSI to get sections
             try:
-                # wsi_series, wsi_issuer, wsi_issue_number, wsi_local = wsi.split("-")   # noqa
+                wsi_series, wsi_issuer, wsi_issue_number, wsi_local = wsi.split("-")   # noqa
 
-                # # get other required metadata
-                # latitude = metadata_dict[wsi]["latitude"]
-                # longitude = metadata_dict[wsi]["longitude"]
-                # station_height = metadata_dict[wsi]["elevation"]
-                # barometer_height = metadata_dict[wsi]["barometer_height"]
+                # get other required metadata
+                latitude = msg["latitude"]
+                longitude = msg["longitude"]
+                station_height = 0
+                barometer_height = 0
 
                 # add these values to the data dictionary
                 '''msg is the synop parser output'''
-                # msg['_wsi_series'] = wsi_series
-                # msg['_wsi_issuer'] = wsi_issuer
-                # msg['_wsi_issue_number'] = wsi_issue_number
-                # msg['_wsi_local'] = wsi_local
-                # msg['_latitude'] = latitude
-                # msg['_longitude'] = longitude
-                # msg['_station_height'] = station_height
-                # msg['_barometer_height'] = barometer_height
+                msg['_wsi_series'] = wsi_series
+                msg['_wsi_issuer'] = wsi_issuer
+                msg['_wsi_issue_number'] = wsi_issue_number
+                msg['_wsi_local'] = wsi_local
+                msg['_latitude'] = latitude
+                msg['_longitude'] = longitude
+                msg['_station_height'] = station_height
+                msg['_barometer_height'] = barometer_height
                 conversion_success[tsi] = True
             except Exception:
                 conversion_success[tsi] = False
 
-                # if wsi == "":
-                #     LOGGER.warning(f"Missing WSI for station {tsi}")
-                #     warning_msgs.append(f"Missing WSI for station {tsi}")
-                # else:
-                #     # If station has not been found in the station
-                #     # list, don't repeat warning unnecessarily
-                #     if not (f"Station {tsi} not found in station file"
-                #             in warning_msgs):
-                #         LOGGER.warning(f"Invalid metadata for station {tsi} found in station file, unable to parse")  # noqa
-                #         warning_msgs.append(f"Invalid metadata for station {tsi} found in station file, unable to parse")  # noqa
+                if wsi == "":
+                    LOGGER.warning(f"Missing WSI for station {tsi}")
+                    warning_msgs.append(f"Missing WSI for station {tsi}")
+                else:
+                    # If station has not been found in the station
+                    # list, don't repeat warning unnecessarily
+                    if not (f"Station {tsi} not found in station file"
+                            in warning_msgs):
+                        LOGGER.warning(f"Invalid metadata for station {tsi} found in station file, unable to parse")  # noqa
+                        warning_msgs.append(f"Invalid metadata for station {tsi} found in station file, unable to parse")  # noqa
 
             if conversion_success[tsi]:
                 try:
                     for idx in range(num_s3_clouds):
                         # Build the dictionary of mappings for section 3
                         # group 8NsChshs
 
@@ -1812,16 +1846,14 @@
                         # Specifically, by B/C1.5.2.1, clouds with bases
                         # below but tops above station level have vertical
                         # significance code 10.
                         # Clouds with bases and tops below station level
                         # have vertical significance code 11.
                         cloud_top_height = msg[f'cloud_height_s4_{idx+1}']
 
-                        station_height = 0
-
                         if cloud_top_height > int(station_height):
                             vs_s4 = 10
                         else:
                             vs_s4 = 11
 
                         # NOTE: Some of the ecCodes keys are used in
                         # the above, so we must add 'num_s3_clouds'
@@ -1855,15 +1887,15 @@
                         f"Missing station height for station {tsi}")
                     conversion_success[tsi] = False
 
             if conversion_success[tsi]:
                 # At this point we have a dictionary for the data, a
                 # dictionary of the mappings and the metadata
                 # The last step is to convert to BUFR.
-                unexpanded_descriptors = [301150, bufr_template]
+                unexpanded_descriptors = [bufr_template]
                 short_delayed_replications = []
                 # update replications
                 delayed_replications = [max(1, num_s3_clouds),
                                         max(1, num_s4_clouds)]
                 extended_delayed_replications = []
                 table_version = 37
                 try:
@@ -1933,29 +1965,29 @@
                         "code": FAILED,
                         "message": "Error encoding, BUFR set to None",
                         "warnings": warning_msgs,
                         "errors": error_msgs
                     }
                     conversion_success[tsi] = False
 
-                rmk = f"SHIP_{tsi}_{isodate}"
+                rmk = f"SHIP_{wsi}_{isodate}"
 
                 # now additional metadata elements
                 result["_meta"] = {
                     "id": rmk,
                     "geometry": {
                         "type": "Point",
                         "coordinates": [
                             message.get_element('#1#longitude'),
                             message.get_element('#1#latitude')
                         ]
                     },
                     "properties": {
                         "md5": message.md5(),
-                        "wigos_station_identifier": f"0-20009-0-{message.get_element('#1#shipOrMobileLandStationIdentifier')}",
+                        "wigos_station_identifier": wsi,
                         "datetime": message.get_datetime(),
                         "originating_centre":
                         message.get_element("bufrHeaderCentre"),
                         "data_category": message.get_element("dataCategory")
                     },
                     "result": status,
                     "template": bufr_template,
@@ -2003,46 +2035,39 @@
         conversion_count = sum(tsi for tsi in conversion_success.values())
 
         # Log number of messages converted
         LOGGER.info((f"{conversion_count} / {len(messages)}"
                     " reports converted successfully"))
         
 
-def my_multiple_reports_308009():
+def my_multiple_reports_308009_backup():
         return "BBXX \
             ZSUY 26123 99172 30042 07415 32931 10103 21090 39765 42250 57020 60071 72006 82110 91155 \
             22275 00170 10212 20718 31603 40503 50402 61111 81165 ICE 21251 \
             333 10178 21073 34101 45010 54000 55055 00010 20003 30002 50001 60004 \
             60035 70500 83145 81533 91008 91111 \
             444 18031 22053="
-        
+
+def my_multiple_reports_308009():
+        return "BBXX \
+             WTDL 08154 99293 70948 43/// /3406 10235 20227 40140 5//// 7//// 8//// 222// 04216 2//// 3//// 4//// 5//// 6//// 8//// ICE /////="        
+
+def my_multiple_reports_308009_sample2():
         '''return "BBXX \
             ZSUY 26123 99172 30042 07415 32931 10103 21090 39765 42250 57020 60071 72006 82110 91155 \
-            22275 00170 10212 31603 40503 50402 61111 81165 ICE 21251 \
+            22275 00170 10212 20718 31603 40503 50402 61111 81165 ICE 21251 \
             333 10178 21073 34101 45010 54000 55055 00010 20003 30002 50001 60004 \
             60035 70500 83145 81533 91008 91111 \
-            444 18031 22053= \
+            444 18031 22053="'''
+
+        return "BBXX \
             ZSUY 26123 99172 30042 41398 81414 10210 20132 40205 5//// 70222\
             881// 22275 00170 20301 316// 40503 5//// 80165=\
-            AMOUK60 12091 99524 10048 46/// ///// 10079 20061 40018="'''
+            AMOUK60 12091 99524 10048 46/// ///// 10079 20061 40018="        
+
     
 
 def my_metadata_string():
     md = "station_name,wigos_station_identifier,traditional_station_identifier,facility_type,latitude,longitude,elevation,barometer_height,territory_name,wmo_region\n" + \
             "OCNA SUGATAG,0-20000-0-ZSUY,ZSUY,Land (fixed),47.77706163,23.94046026,503,504.43,Romania,6\n" + \
             "IASI,0-20000-0-AMOUK60,AMOUK60,Land (fixed),47.16333333,27.62722222,74.29,75.69,Romania,6"  # noqa
     return md
-
-# multiple_reports = my_multiple_reports_308009()
-# metadata_string = my_metadata_string()
-
-# result = transform(
-#     multiple_reports, metadata_string, 2022, 3
-# )
-# msgs = {}
-# for item in result:
-#     pprint(item)
-#     print()
-#     '''msgs[item['_meta']['id']] = item
-#     pprint(msgs)'''
-
-
```

### Comparing `FM13_transform-0.0.3/src/FM13_transform/resources/synop-mappings-308009.json` & `fm13_transform-0.0.4/src/FM13_transform/resources/synop-mappings-308009.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965556298276886%*

 * *Differences: {"'data'": '{delete: [3, 2, 1, 0]}', "'header'": "{16: {'value': 'array:308009'}}"}*

```diff
@@ -1,26 +1,10 @@
 {
     "data": [
         {
-            "eccodes_key": "#1#wigosIdentifierSeries",
-            "value": "data:_wsi_series"
-        },
-        {
-            "eccodes_key": "#1#wigosIssuerOfIdentifier",
-            "value": "data:_wsi_issuer"
-        },
-        {
-            "eccodes_key": "#1#wigosIssueNumber",
-            "value": "data:_wsi_issue_number"
-        },
-        {
-            "eccodes_key": "#1#wigosLocalIdentifierCharacter",
-            "value": "data:_wsi_local"
-        },
-        {
             "_comment": "callsign",
             "eccodes_key": "#1#shipOrMobileLandStationIdentifier",
             "value": "data:callsign"
         },
         {
             "_comment": "unknown",
             "eccodes_key": "#1#directionOfMotionOfMovingObservingPlatform",
@@ -607,15 +591,15 @@
         },
         {
             "eccodes_key": "typicalMinute",
             "value": "data:minute"
         },
         {
             "eccodes_key": "unexpandedDescriptors",
-            "value": "array:301150, 308009"
+            "value": "array:308009"
         }
     ],
     "inputDelayedDescriptorReplicationFactor": [
         1,
         1
     ],
     "inputExtendedDelayedDescriptorReplicationFactor": [],
```

### Comparing `FM13_transform-0.0.3/src/FM13_transform.egg-info/PKG-INFO` & `fm13_transform-0.0.4/src/FM13_transform.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FM13_transform
-Version: 0.0.3
-Summary: Package for converting FM13 SYNOP to BUFR4
-Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>
+Version: 0.0.4
+Summary: Package for converting FM13 SYNOP to BUFR4 and GeoJSON
+Author-email: Zhan Zhang <zhan.j.zhang@noaa.gov>, Alex Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,SYNOP SHIP,FM-13,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: csv2bufr
```

