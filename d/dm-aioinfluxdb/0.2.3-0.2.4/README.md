# Comparing `tmp/dm-aioinfluxdb-0.2.3.tar.gz` & `tmp/dm_aioinfluxdb-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-aioinfluxdb-0.2.3.tar", last modified: Thu Feb  8 16:19:15 2024, max compression
+gzip compressed data, was "dm_aioinfluxdb-0.2.4.tar", last modified: Mon Apr 15 06:43:19 2024, max compression
```

## Comparing `dm-aioinfluxdb-0.2.3.tar` & `dm_aioinfluxdb-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:19:15.006199 dm-aioinfluxdb-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-08 16:19:15.006199 dm-aioinfluxdb-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-08 16:18:56.000000 dm-aioinfluxdb-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:19:15.002199 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-08 16:18:56.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-02-08 16:18:56.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb/aioinfluxdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:19:15.006199 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 16:19:15.006199 dm-aioinfluxdb-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-08 16:19:14.000000 dm-aioinfluxdb-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:43:19.146981 dm_aioinfluxdb-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-15 06:43:19.146981 dm_aioinfluxdb-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-15 06:43:10.000000 dm_aioinfluxdb-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:43:19.146981 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 06:43:10.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-15 06:43:10.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb/aioinfluxdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:43:19.146981 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-15 06:43:19.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 06:43:19.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:43:19.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 06:43:19.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 06:43:19.000000 dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:43:19.146981 dm_aioinfluxdb-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-15 06:43:18.000000 dm_aioinfluxdb-0.2.4/setup.py
```

### Comparing `dm-aioinfluxdb-0.2.3/PKG-INFO` & `dm_aioinfluxdb-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aioinfluxdb
-Version: 0.2.3
+Version: 0.2.4
 Summary: This is my custom aioinfluxdb client
 Home-page: https://pypi.org/project/dm-aioinfluxdb
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aioinfluxdb
 Keywords: dm aioinfluxdb
 Classifier: Programming Language :: Python :: 3.8
@@ -35,18 +35,23 @@
 
 async def main():
     # create client
     influxdb_client = DMAioInfluxDBClient("localhost", 8086, "org", "token")
 
     # create influxdb points
     point1 = influxdb_client.create_point("example-measurement", {"value": 1.5}, {"tag1": "tag1-value"})
+    # or
     point2 = DMAioInfluxDBClient.create_point("example-measurement", {"value": 0}, {"tag2": "tag2-value"})
 
     # write one or more points
     await influxdb_client.write("example-bucket", point1)
+    # write line protocol record
+    record = "example-measurement,tag1=tag1-value, value=1.5 1713162515"
+    await influxdb_client.write("example-bucket", record)
+
     # type: bool
     status = await influxdb_client.write("example-bucket", [point1, point2])
 
     # return error message in case of error
     # type: (bool, str)
     status, err_msg = await influxdb_client.write("example-bucket", point1, return_errors=True)
```

### Comparing `dm-aioinfluxdb-0.2.3/README.md` & `dm_aioinfluxdb-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 
 async def main():
     # create client
     influxdb_client = DMAioInfluxDBClient("localhost", 8086, "org", "token")
 
     # create influxdb points
     point1 = influxdb_client.create_point("example-measurement", {"value": 1.5}, {"tag1": "tag1-value"})
+    # or
     point2 = DMAioInfluxDBClient.create_point("example-measurement", {"value": 0}, {"tag2": "tag2-value"})
 
     # write one or more points
     await influxdb_client.write("example-bucket", point1)
+    # write line protocol record
+    record = "example-measurement,tag1=tag1-value, value=1.5 1713162515"
+    await influxdb_client.write("example-bucket", record)
+
     # type: bool
     status = await influxdb_client.write("example-bucket", [point1, point2])
 
     # return error message in case of error
     # type: (bool, str)
     status, err_msg = await influxdb_client.write("example-bucket", point1, return_errors=True)
```

### Comparing `dm-aioinfluxdb-0.2.3/dm_aioinfluxdb/aioinfluxdb_client.py` & `dm_aioinfluxdb-0.2.4/dm_aioinfluxdb/aioinfluxdb_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,21 +68,30 @@
         if return_errors:
             return result, error_message
         return result
 
     async def write(
         self,
         bucket: str,
-        record: Point | list[Point],
+        record: Point | list[Point] | str,
         return_errors: bool = None,
         err_logging: bool = None
     ) -> bool | (bool, str):
         points = record if isinstance(record, list) else [record]
-        to_line_points = map(lambda p: p.to_line_protocol(), points)
-        points = list(filter(lambda p: p, to_line_points))
+        prepared_points = []
+        for p in points:
+            if isinstance(p, Point):
+                line_p = p.to_line_protocol()
+                if line_p:
+                    prepared_points.append(line_p)
+            elif isinstance(p, str):
+                prepared_points.append(p)
+            else:
+                return False, "Expected record: Point | list[Point] | str"
+
         if not points:
             return False
 
         async def write_callback(client: InfluxDBClientAsync) -> bool:
             await client.write_api().write(bucket=bucket, record=points)
             return True
```

### Comparing `dm-aioinfluxdb-0.2.3/dm_aioinfluxdb.egg-info/PKG-INFO` & `dm_aioinfluxdb-0.2.4/dm_aioinfluxdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aioinfluxdb
-Version: 0.2.3
+Version: 0.2.4
 Summary: This is my custom aioinfluxdb client
 Home-page: https://pypi.org/project/dm-aioinfluxdb
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aioinfluxdb
 Keywords: dm aioinfluxdb
 Classifier: Programming Language :: Python :: 3.8
@@ -35,18 +35,23 @@
 
 async def main():
     # create client
     influxdb_client = DMAioInfluxDBClient("localhost", 8086, "org", "token")
 
     # create influxdb points
     point1 = influxdb_client.create_point("example-measurement", {"value": 1.5}, {"tag1": "tag1-value"})
+    # or
     point2 = DMAioInfluxDBClient.create_point("example-measurement", {"value": 0}, {"tag2": "tag2-value"})
 
     # write one or more points
     await influxdb_client.write("example-bucket", point1)
+    # write line protocol record
+    record = "example-measurement,tag1=tag1-value, value=1.5 1713162515"
+    await influxdb_client.write("example-bucket", record)
+
     # type: bool
     status = await influxdb_client.write("example-bucket", [point1, point2])
 
     # return error message in case of error
     # type: (bool, str)
     status, err_msg = await influxdb_client.write("example-bucket", point1, return_errors=True)
```

### Comparing `dm-aioinfluxdb-0.2.3/setup.py` & `dm_aioinfluxdb-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aioinfluxdb',
-    version='v0.2.3',
+    version='v0.2.4',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aioinfluxdb client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aioinfluxdb',
     packages=find_packages(),
```

