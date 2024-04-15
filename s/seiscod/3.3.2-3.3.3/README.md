# Comparing `tmp/seiscod-3.3.2-py3-none-any.whl.zip` & `tmp/seiscod-3.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 98770 bytes, number of entries: 51
+Zip file size: 98849 bytes, number of entries: 51
 -rw-rw-r--  2.0 unx      430 b- defN 24-Jan-16 19:46 seiscod/__init__.py
 -rw-rw-r--  2.0 unx     1308 b- defN 23-Jul-17 08:44 seiscod/errors.py
 -rw-rw-r--  2.0 unx    19500 b- defN 24-Jan-16 19:46 seiscod/graphic.py
 -rw-rw-r--  2.0 unx    13076 b- defN 24-Apr-02 21:01 seiscod/picker.py
 -rw-rw-r--  2.0 unx    12762 b- defN 23-Jul-17 08:44 seiscod/sampling.py
 -rw-rw-r--  2.0 unx    35342 b- defN 24-Feb-29 22:01 seiscod/stream.py
--rw-rw-r--  2.0 unx    40245 b- defN 24-Jan-16 19:46 seiscod/trace.py
--rw-rw-r--  2.0 unx       22 b- defN 24-Apr-13 19:36 seiscod/version.py
+-rw-rw-r--  2.0 unx    40533 b- defN 24-Apr-13 20:31 seiscod/trace.py
+-rw-rw-r--  2.0 unx       22 b- defN 24-Apr-15 09:07 seiscod/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 08:44 seiscod/readwrite/__init__.py
 -rw-rw-r--  2.0 unx      683 b- defN 23-Jul-17 08:44 seiscod/readwrite/rawtrace.py
 -rw-rw-r--  2.0 unx       40 b- defN 23-Jul-17 08:44 seiscod/readwrite/mseed/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 08:44 seiscod/readwrite/npz/__init__.py
 -rw-rw-r--  2.0 unx     9645 b- defN 23-Oct-12 11:56 seiscod/readwrite/npz/readnpz.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 08:44 seiscod/readwrite/seg2/__init__.py
 -rw-rw-r--  2.0 unx    11448 b- defN 24-Jan-16 19:46 seiscod/readwrite/seg2/readseg2withobspy.py
@@ -40,14 +40,14 @@
 -rw-rw-r--  2.0 unx     2867 b- defN 23-Jul-17 08:44 seiscod/signal/parseval.py
 -rw-rw-r--  2.0 unx      781 b- defN 23-Jul-17 08:44 seiscod/signal/pws.py
 -rw-rw-r--  2.0 unx     4271 b- defN 23-Jul-17 08:44 seiscod/signal/spectralwhitening.py
 -rw-rw-r--  2.0 unx     1397 b- defN 23-Jul-17 08:44 seiscod/signal/taper.py
 -rw-rw-r--  2.0 unx     6451 b- defN 23-Jul-17 08:44 seiscod/signal/waveformclustering.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 08:44 seiscod/viz/__init__.py
 -rw-rw-r--  2.0 unx    16373 b- defN 24-Mar-04 20:33 seiscod/viz/viz.py
--rwxrwxr-x  2.0 unx    16360 b- defN 24-Apr-13 19:50 seiscod-3.3.2.data/scripts/viz
--rw-rw-r--  2.0 unx     1076 b- defN 24-Apr-13 19:50 seiscod-3.3.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3295 b- defN 24-Apr-13 19:50 seiscod-3.3.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-13 19:50 seiscod-3.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-13 19:50 seiscod-3.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4342 b- defN 24-Apr-13 19:50 seiscod-3.3.2.dist-info/RECORD
-51 files, 352117 bytes uncompressed, 91828 bytes compressed:  73.9%
+-rwxrwxr-x  2.0 unx    16360 b- defN 24-Apr-15 09:08 seiscod-3.3.3.data/scripts/viz
+-rw-rw-r--  2.0 unx     1076 b- defN 24-Apr-15 09:08 seiscod-3.3.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3295 b- defN 24-Apr-15 09:08 seiscod-3.3.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-15 09:08 seiscod-3.3.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-15 09:08 seiscod-3.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4342 b- defN 24-Apr-15 09:08 seiscod-3.3.3.dist-info/RECORD
+51 files, 352405 bytes uncompressed, 91907 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -129,26 +129,26 @@
 
 Filename: seiscod/viz/__init__.py
 Comment: 
 
 Filename: seiscod/viz/viz.py
 Comment: 
 
-Filename: seiscod-3.3.2.data/scripts/viz
+Filename: seiscod-3.3.3.data/scripts/viz
 Comment: 
 
-Filename: seiscod-3.3.2.dist-info/LICENSE
+Filename: seiscod-3.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: seiscod-3.3.2.dist-info/METADATA
+Filename: seiscod-3.3.3.dist-info/METADATA
 Comment: 
 
-Filename: seiscod-3.3.2.dist-info/WHEEL
+Filename: seiscod-3.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: seiscod-3.3.2.dist-info/top_level.txt
+Filename: seiscod-3.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: seiscod-3.3.2.dist-info/RECORD
+Filename: seiscod-3.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seiscod/trace.py

```diff
@@ -182,25 +182,31 @@
             # I don't want anything from obspy in the top imports !!!
             # this may fuck up matplotlib behavior
             from obspy.core.trace import Trace as ObspyTrace, UTCDateTime as ObspyUTCDateTime
         except ImportError as e:
             e.args = ('obspy not installed', )
             raise e
 
-        network, station, location, channel = self.seedid.split('.')
+        try:
+            network, station, location, channel = self.seedid.split('.')
+        except ValueError:
+            # seedid string is not formatted as expected, quick fix
+            network, station, location, channel = "", self.seedid, "", ""
+            
         header = {"network": network,
                   "station": station,
                   "location": location,
                   "channel": channel,
                   "delta": self.delta,
                   "starttime": ObspyUTCDateTime(self.starttime),
                   "coordinates":{"longitude": self.longitude,
                                  "latitude": self.latitude,
                                  "elevation": self.elevation,
-                                 "distance": self.distance}}
+                                 "distance": self.distance},
+                  "seiscod": {key: getattr(self, key) for key in self.additional_keys}}
 
         return ObspyTrace(self.data, header)
 
     def from_rmseed_segment(self, segment):
         self.seedid = segment.seedid
         self.delta = 1. / segment.sprate
         self.starttime = segment.starttime
@@ -1174,8 +1180,8 @@
     tr = Trace(data=data)
     print(tr, tr.__class__, tr.data)
 
     tr.fft()
     print(tr, tr.__class__, tr.data)
 
     tr.ifft()
-    print(tr, tr.__class__, tr.data)
+    print(tr, tr.__class__, tr.data)
```

## seiscod/version.py

```diff
@@ -1 +1 @@
-__version__ = "3.3.2"
+__version__ = "3.3.3"
```

## Comparing `seiscod-3.3.2.data/scripts/viz` & `seiscod-3.3.3.data/scripts/viz`

 * *Files identical despite different names*

## Comparing `seiscod-3.3.2.dist-info/LICENSE` & `seiscod-3.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `seiscod-3.3.2.dist-info/METADATA` & `seiscod-3.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscod
-Version: 3.3.2
+Version: 3.3.3
 Home-page: 
 Author: Maximilien Lehujeur
 Author-email: maximilien.lehujeur@univ-eiffel.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
```

## Comparing `seiscod-3.3.2.dist-info/RECORD` & `seiscod-3.3.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 seiscod/__init__.py,sha256=aVap2e6r59giyF4s6VTWhB-RD0oUfv8d61yr7l4WaH8,430
 seiscod/errors.py,sha256=z2dHSapmdKf14DMhMUItXWUfum_GxN-YCuiXH0tSq1w,1308
 seiscod/graphic.py,sha256=ZXoBn4MIP88jxw3MwZvgxBxXPi5pGiYsCHr1vuEMdWY,19500
 seiscod/picker.py,sha256=YjMumtWXQMMKi6-vYyGhxEOfxJpavxoI9vaGdF_S7nE,13076
 seiscod/sampling.py,sha256=eOSKU7uZSvUEtFMNGdSCguKn1L3egO3KskN2XcFZpPI,12762
 seiscod/stream.py,sha256=3P0UFv3LishjCfhpnqJBRdTnVLzjcba5eB9VzRGc2n4,35342
-seiscod/trace.py,sha256=QV-l2wYEA3po9BfOdZoigwdFQtdCbGOH8LAbTbL_zAg,40245
-seiscod/version.py,sha256=ljnJCYxaT-9Q47JZlNplo0KcLdOZrB0woIJhPq11pD0,22
+seiscod/trace.py,sha256=SLeTsYxls8VzcCb-MNJqsap6W-GLRqrsQyEcLGpf41M,40533
+seiscod/version.py,sha256=Au2yR9CeJDYeCsUV7lIDllPVwz8EynN-QwVbxO3RWOM,22
 seiscod/readwrite/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seiscod/readwrite/rawtrace.py,sha256=RBpsZvjEHWVDpdmFe_wCZX8v3eojoxSUMrPuU45T9jc,683
 seiscod/readwrite/mseed/__init__.py,sha256=_aRMJlfJVrg7zq9zxHYSUY1nMDxciuyWLeQWWj3AX1o,40
 seiscod/readwrite/npz/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seiscod/readwrite/npz/readnpz.py,sha256=2VK5i9IUGnwBndnsGKDCUum4tSqTVRD5DBHdts8ZGUM,9645
 seiscod/readwrite/seg2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seiscod/readwrite/seg2/readseg2withobspy.py,sha256=Gh3Bf9cW4KC2hwxVTaw7II8RPalSbVDyVj6a3B4RVok,11448
@@ -39,13 +39,13 @@
 seiscod/signal/parseval.py,sha256=FVloQOQCD99zWC3-VEM2HaNYEgFRMKPZnHhd_Y_hfHw,2867
 seiscod/signal/pws.py,sha256=vWRtN-PoOK8CiFZdYEXSWNdAZy6kKWBCVGfnYpJtev0,781
 seiscod/signal/spectralwhitening.py,sha256=M_lY9R5dxkqfeZNjkP3Bq2D3ElIuVGkDD6Ysm_k_3cw,4271
 seiscod/signal/taper.py,sha256=QL4SLRwO19UKYYO4sNKY0MWcNz0xy-b3lJ8Uk3XzE6U,1397
 seiscod/signal/waveformclustering.py,sha256=GPipeDWO5SOvssHjSulmgiM1gR5AIyIA-JlX7CtochI,6451
 seiscod/viz/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seiscod/viz/viz.py,sha256=EwPG-hjGdeE4zU1rhdD6jc0xMYVr0Yp1TzjwaWepZDo,16373
-seiscod-3.3.2.data/scripts/viz,sha256=QLczAcaTS-atv6u8bLpr7p1UXfXbTQik4AXYc3hksoY,16360
-seiscod-3.3.2.dist-info/LICENSE,sha256=jyKGGrTCuMxPDRq0NyLgQfv_XFwudDrS_ZBx9JNGm-E,1076
-seiscod-3.3.2.dist-info/METADATA,sha256=0PaP_crMVM8mhmISbSOpojKAKWVn7NpZiuDSYWCaG3U,3295
-seiscod-3.3.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-seiscod-3.3.2.dist-info/top_level.txt,sha256=9XG3kK6SAyau15Y4WKetwOB0V9o6jCa84DwkbTmWbrI,8
-seiscod-3.3.2.dist-info/RECORD,,
+seiscod-3.3.3.data/scripts/viz,sha256=QLczAcaTS-atv6u8bLpr7p1UXfXbTQik4AXYc3hksoY,16360
+seiscod-3.3.3.dist-info/LICENSE,sha256=jyKGGrTCuMxPDRq0NyLgQfv_XFwudDrS_ZBx9JNGm-E,1076
+seiscod-3.3.3.dist-info/METADATA,sha256=Wa8k-jsOJvfUJad0MAqYlOnmiegDiqtZjdFs4Q8Zt3I,3295
+seiscod-3.3.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+seiscod-3.3.3.dist-info/top_level.txt,sha256=9XG3kK6SAyau15Y4WKetwOB0V9o6jCa84DwkbTmWbrI,8
+seiscod-3.3.3.dist-info/RECORD,,
```
