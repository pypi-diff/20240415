# Comparing `tmp/oip_tracking_client-0.0.2-py3-none-any.whl.zip` & `tmp/oip_tracking_client-0.0.3.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17306 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 10:23 oip_tracking_client/__init__.py
--rw-r--r--  2.0 unx     5256 b- defN 24-Jan-18 10:38 oip_tracking_client/lib.py
--rw-r--r--  2.0 unx     5458 b- defN 23-Aug-05 11:46 oip_tracking_client/rest.py
--rw-r--r--  2.0 unx    10229 b- defN 24-Jan-18 03:13 oip_tracking_client/tracking.py
--rw-r--r--  2.0 unx    21094 b- defN 23-Aug-04 10:46 oip_tracking_client/wavfile.py
--rw-r--r--  2.0 unx     5598 b- defN 24-Jan-18 10:45 oip_tracking_client-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-18 10:45 oip_tracking_client-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Jan-18 10:45 oip_tracking_client-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      775 b- defN 24-Jan-18 10:45 oip_tracking_client-0.0.2.dist-info/RECORD
-9 files, 48522 bytes uncompressed, 15958 bytes compressed:  67.1%
+Zip file size: 17352 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-14 15:48 oip_tracking_client/__init__.py
+-rw-r--r--  2.0 unx     5256 b- defN 24-Mar-08 06:51 oip_tracking_client/lib.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Mar-08 06:06 oip_tracking_client/rest.py
+-rw-r--r--  2.0 unx    10205 b- defN 24-Apr-15 06:42 oip_tracking_client/tracking.py
+-rw-r--r--  2.0 unx    21096 b- defN 24-Mar-08 06:06 oip_tracking_client/wavfile.py
+-rw-r--r--  2.0 unx     5614 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-15 06:50 oip_tracking_client-0.0.3.dev0.dist-info/RECORD
+9 files, 48537 bytes uncompressed, 15964 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: oip_tracking_client/tracking.py
 Comment: 
 
 Filename: oip_tracking_client/wavfile.py
 Comment: 
 
-Filename: oip_tracking_client-0.0.2.dist-info/METADATA
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/METADATA
 Comment: 
 
-Filename: oip_tracking_client-0.0.2.dist-info/WHEEL
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: oip_tracking_client-0.0.2.dist-info/top_level.txt
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: oip_tracking_client-0.0.2.dist-info/RECORD
+Filename: oip_tracking_client-0.0.3.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oip_tracking_client/rest.py

 * *Ordering differences only*

```diff
@@ -148,8 +148,8 @@
     """Wrap the standard `requests.response.raise_for_status()` method and return reason"""
     try:
         response.raise_for_status()
     except HTTPError as e:
         if response.text:
             raise HTTPError(f"{e}. Response text: {response.text}")
         else:
-            raise e
+            raise e
```

## oip_tracking_client/tracking.py

```diff
@@ -31,17 +31,15 @@
     run = mlflow.active_run()
     if not run:
         raise RuntimeError("NO ACTIVE RUN, PLEASE START THE RUN...")
 
     # Add mlflow/experiment_id/run_id/artifacts to artifact path
     run_id = run.info.run_id
     experiment_id = run.info.experiment_id
-    artifact_path = os.path.join(
-        "mlflow", experiment_id, run_id, "artifacts", artifact_path
-    )
+    artifact_path = os.path.join(experiment_id, run_id, "artifacts", artifact_path)
 
     # Add artifact_path to extra that will be used as request body
     extra["artifact_path"] = artifact_path
 
     # Create token and headers
     endpoint: str = f"{os.environ['OIP_API_HOST']}/mlflow/update_artifact_object"
     headers: Dict[str, str] = {
```

## oip_tracking_client/wavfile.py

```diff
@@ -357,15 +357,15 @@
 
     if format_tag == WAVE_FORMAT.EXTENSIBLE and size >= (16 + 2):
         ext_chunk_size = struct.unpack(fmt + "H", fid.read(2))[0]
         bytes_read += 2
         if ext_chunk_size >= 22:
             extensible_chunk_data = fid.read(22)
             bytes_read += 22
-            raw_guid = extensible_chunk_data[(2 + 4):(2 + 4 + 16)]
+            raw_guid = extensible_chunk_data[(2 + 4) : (2 + 4 + 16)]
             # GUID template {XXXXXXXX-0000-0010-8000-00AA00389B71} (RFC-2361)
             # MS GUID byte order: first three groups are native byte order,
             # rest is Big Endian
             if is_big_endian:
                 tail = b"\x00\x00\x00\x10\x80\x00\x00\xAA\x00\x38\x9B\x71"
             else:
                 tail = b"\x00\x00\x10\x00\x80\x00\x00\xAA\x00\x38\x9B\x71"
```

## Comparing `oip_tracking_client-0.0.2.dist-info/METADATA` & `oip_tracking_client-0.0.3.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: oip-tracking-client
-Version: 0.0.2
+Version: 0.0.3.dev0
 Summary: This is the API client of Open Innovation Platform - Tracking
 Author: Rachid Belmeskine
 Author-email: rachid.belmeskine@gmail.com
 License: PRIVATE LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: typing
-Requires-Dist: mlflow
+Requires-Dist: mlflow (==2.11.3)
 Requires-Dist: numpy
 Requires-Dist: Pillow
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 
 # Open Innovation MLOps Client API
```

## Comparing `oip_tracking_client-0.0.2.dist-info/RECORD` & `oip_tracking_client-0.0.3.dev0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oip_tracking_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oip_tracking_client/lib.py,sha256=ujU_bQ6ix7noiiXpje0ZKyhJpJKi4tM0ukYQVYlbUIw,5256
-oip_tracking_client/rest.py,sha256=rJUTM7WiCNuv3Vu6um-n5P8vlcVXwR6bzZmGk5BvH_s,5458
-oip_tracking_client/tracking.py,sha256=plCCIVTLZGatqt0Yr6KYco4g8leTxluWqXNprXwQiUc,10229
-oip_tracking_client/wavfile.py,sha256=MCG-9SU-0U5qsNMSpxiWqfIItTpy-tRnC5NxQRGRKlo,21094
-oip_tracking_client-0.0.2.dist-info/METADATA,sha256=GlWUAOb8S2-NCF_He1lGz6to5ovBVPG6W4-AABktthM,5598
-oip_tracking_client-0.0.2.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-oip_tracking_client-0.0.2.dist-info/top_level.txt,sha256=TlX4Qx0OtAJefucshHIOZ2z8FR8BF-Us-9af0zLI3Uc,20
-oip_tracking_client-0.0.2.dist-info/RECORD,,
+oip_tracking_client/rest.py,sha256=IKs8uipUKPIW3VG8dbKIxkclxlVXpaBQElUpy0cQ5Hw,5459
+oip_tracking_client/tracking.py,sha256=jh24V-c1sofJQbecaQSr4qq5CBO9FKWDYCu2oipLM2g,10205
+oip_tracking_client/wavfile.py,sha256=vAYY3NF0KZ-wP0VLCMcya0_99OtNGcoWP5XOeyZfF2g,21096
+oip_tracking_client-0.0.3.dev0.dist-info/METADATA,sha256=3kQPnTPDUhoZbNjlueT1S7ABJidWicrprxI7yweN3s8,5614
+oip_tracking_client-0.0.3.dev0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+oip_tracking_client-0.0.3.dev0.dist-info/top_level.txt,sha256=TlX4Qx0OtAJefucshHIOZ2z8FR8BF-Us-9af0zLI3Uc,20
+oip_tracking_client-0.0.3.dev0.dist-info/RECORD,,
```

