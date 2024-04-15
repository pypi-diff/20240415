# Comparing `tmp/tyba_client-0.3.7.tar.gz` & `tmp/tyba_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyba_client-0.3.7.tar", max compression
+gzip compressed data, was "tyba_client-0.4.0.tar", max compression
```

## Comparing `tyba_client-0.3.7.tar` & `tyba_client-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-01-03 22:30:17.132261 tyba_client-0.3.7/LICENSE
--rw-r--r--   0        0        0     1385 2024-01-11 22:22:09.981795 tyba_client-0.3.7/README.md
--rw-r--r--   0        0        0      772 2024-03-21 20:10:08.619040 tyba_client-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-12 18:20:06.257802 tyba_client-0.3.7/tyba_client/__init__.py
--rw-r--r--   0        0        0     5761 2024-01-12 18:20:06.258290 tyba_client-0.3.7/tyba_client/client.py
--rw-r--r--   0        0        0     4428 2024-03-21 20:06:18.764085 tyba_client-0.3.7/tyba_client/forecast.py
--rw-r--r--   0        0        0     7015 2024-01-12 18:20:06.259458 tyba_client-0.3.7/tyba_client/io.py
--rw-r--r--   0        0        0    17498 2024-01-12 18:20:06.260227 tyba_client-0.3.7/tyba_client/models.py
--rw-r--r--   0        0        0      876 2024-01-12 18:20:06.260712 tyba_client-0.3.7/tyba_client/utils.py
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 tyba_client-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-15 06:02:12.062137 tyba_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1385 2024-04-15 06:02:12.062206 tyba_client-0.4.0/README.md
+-rw-r--r--   0        0        0      766 2024-04-15 09:30:52.462357 tyba_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-15 09:31:44.081853 tyba_client-0.4.0/tyba_client/__init__.py
+-rw-r--r--   0        0        0     5761 2024-04-15 06:02:12.069944 tyba_client-0.4.0/tyba_client/client.py
+-rw-r--r--   0        0        0     4428 2024-04-15 06:02:12.070041 tyba_client-0.4.0/tyba_client/forecast.py
+-rw-r--r--   0        0        0     5783 2024-04-15 06:14:17.827925 tyba_client-0.4.0/tyba_client/io.py
+-rw-r--r--   0        0        0    17525 2024-04-15 06:14:17.834494 tyba_client-0.4.0/tyba_client/models.py
+-rw-r--r--   0        0        0     3379 2024-04-15 06:46:15.574478 tyba_client-0.4.0/tyba_client/solar_resource.py
+-rw-r--r--   0        0        0      876 2024-04-15 06:02:12.070316 tyba_client-0.4.0/tyba_client/utils.py
+-rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 tyba_client-0.4.0/PKG-INFO
```

### Comparing `tyba_client-0.3.7/LICENSE` & `tyba_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tyba_client-0.3.7/README.md` & `tyba_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tyba_client-0.3.7/pyproject.toml` & `tyba_client-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "tyba-client"
-version = "0.3.7"
+version = "0.4.0"
 description = "A Python API client for the Tyba Public API"
 authors = ["Tyler Nisonoff <tyler@tybaenergy.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25.1"
-dataclasses-json = "^0.5.4"
+dataclasses-json = "^0.6.4"
 marshmallow = "^3.12.1"
 pandas = "^1.3.2"
-tyba-financial-model = "^0.1.0"
-structlog = "^23.1.0"
-generation-models = "^0.4.1"
+tyba-financial-model = "^0"
+structlog = "^24.1.0"
+generation-models = "^0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^5.2"
+pytest = "^8.1.1"
 ipython = "^7.29.0"
 ipdb = "^0.13.9"
 sphinx = "^7.0.1"
 autodoc-pydantic = "^1.8.0"
 boto3 = "^1.28.22"
 nbsphinx = "^0.9.3"
 sphinx-rtd-theme = "^2.0.0"
```

### Comparing `tyba_client-0.3.7/tyba_client/client.py` & `tyba_client-0.4.0/tyba_client/client.py`

 * *Files identical despite different names*

### Comparing `tyba_client-0.3.7/tyba_client/forecast.py` & `tyba_client-0.4.0/tyba_client/forecast.py`

 * *Files identical despite different names*

### Comparing `tyba_client-0.3.7/tyba_client/io.py` & `tyba_client-0.4.0/tyba_client/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from __future__ import annotations
 from generation_models import (
     PVModuleMermoudLejeune,
     ONDInverter,
     ONDEfficiencyCurve,
     ONDTemperatureDerateCurve,
-    SolarResource,
-    SolarResourceTimeSeries,
 )
-import pandas as pd
-import typing as t
 
 
 def read_pvsyst_file(path: str) -> dict:
     try:
         with open(path, "r", encoding="utf-8-sig") as f:
             blob = {}
             trace = [blob]
@@ -156,52 +152,7 @@
         power_curves=power_curves,
         dc_turn_on=float(converter["PSeuil"]),
         pnt=float(data["Night_Loss"]),
         aux_loss=aux_loss,
         aux_loss_threshold=aux_loss_threshold,
         includes_xfmr=includes_xfmr,
     )
-
-
-psm_column_map = {
-    "Year": "year",
-    "Month": "month",
-    "Day": "day",
-    "Hour": "hour",
-    "Minute": "minute",
-    "GHI": "gh",
-    "DNI": "dn",
-    "DHI": "df",
-    "POA": "poa",
-    "Temperature": "tdry",
-    # twet
-    "Dew Point": "tdew",
-    "Relative Humidity": "rhum",
-    "Pressure": "pres",
-    # Snow
-    "Surface Albedo": "alb",
-    # aod
-    "Wind Speed": "wspd",
-    "Wind Direction": "wdir",
-}
-
-
-def solar_resource_from_psm_csv(
-    filename: str,
-    typical: bool = True,
-    monthly_albedo: t.Optional[t.List[float]] = None,
-) -> SolarResource:
-    """_"""
-    with open(filename) as f:
-        _meta = [f.readline().split(",") for _ in range(2)]
-        _data = pd.read_csv(f)
-    meta = {k: v for k, v in zip(*_meta)}
-    data = _data.rename(columns=psm_column_map)
-    return SolarResource(
-        latitude=float(meta["Latitude"]),
-        longitude=float(meta["Longitude"]),
-        elevation=float(meta["Elevation"]),
-        time_zone_offset=float(meta["Time Zone"]),
-        data=SolarResourceTimeSeries(**data.to_dict(orient="list")),
-        monthly_albedo=monthly_albedo,
-        typical=typical,
-    )
```

### Comparing `tyba_client-0.3.7/tyba_client/models.py` & `tyba_client-0.4.0/tyba_client/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 from enum import Enum
 from dataclasses_json import config, dataclass_json
 import pandas as pd
 import typing as t
-from .io import read_pvsyst_file, psm_column_map
+from .io import read_pvsyst_file
+from .solar_resource import psm_column_map
 
 from tyba_client.utils import string_enum
 
 
 class ValidationError(ValueError):
     pass
```

### Comparing `tyba_client-0.3.7/tyba_client/utils.py` & `tyba_client-0.4.0/tyba_client/utils.py`

 * *Files identical despite different names*

### Comparing `tyba_client-0.3.7/PKG-INFO` & `tyba_client-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: tyba-client
-Version: 0.3.7
+Version: 0.4.0
 Summary: A Python API client for the Tyba Public API
 License: MIT
 Author: Tyler Nisonoff
 Author-email: tyler@tybaenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dataclasses-json (>=0.5.4,<0.6.0)
-Requires-Dist: generation-models (>=0.4.1,<0.5.0)
+Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
+Requires-Dist: generation-models (>=0,<1)
 Requires-Dist: marshmallow (>=3.12.1,<4.0.0)
 Requires-Dist: pandas (>=1.3.2,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
-Requires-Dist: tyba-financial-model (>=0.1.0,<0.2.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Requires-Dist: tyba-financial-model (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Tyba API Client
 
 ## Examples
 For examples see [https://github.com/Tyba-Energy/tyba-client-notebooks](https://github.com/Tyba-Energy/tyba-client-notebooks).
 The script examples in tyba-python-client/examples will be deprecated eventually.
```

