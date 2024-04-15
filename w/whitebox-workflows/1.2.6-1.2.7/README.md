# Comparing `tmp/whitebox_workflows-1.2.6-cp38-abi3-win_amd64.whl.zip` & `tmp/whitebox_workflows-1.2.7-cp38-abi3-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 8966941 bytes, number of entries: 15
--rw-r--r--  4.6 unx    11931 b- defN 24-Apr-07 19:19 whitebox_workflows-1.2.6.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-07 19:19 whitebox_workflows-1.2.6.dist-info/WHEEL
--rw-r--r--  4.6 unx      163 b- defN 24-Apr-07 19:19 whitebox_workflows-1.2.6.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx        0 b- defN 24-Apr-07 19:19 whitebox_workflows/py.typed
--rw-r--r--  4.6 unx     8450 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/horton_ratios.py
--rw-r--r--  4.6 unx     2158 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/nibble.py
--rw-r--r--  4.6 unx     1852 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/ridge_and_valley_vectors.py
--rw-r--r--  4.6 unx     1045 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/scripts.py
--rw-r--r--  4.6 unx      967 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/sieve.py
--rw-r--r--  4.6 unx      890 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/utils.py
--rw-r--r--  4.6 unx        0 b- defN 24-Apr-07 19:19 whitebox_workflows/scripts/__init__.py
--rw-r--r--  4.6 unx    91516 b- defN 24-Apr-07 19:19 whitebox_workflows/whitebox_workflows.pyi
--rw-r--r--  4.6 unx    10952 b- defN 24-Apr-07 19:19 whitebox_workflows/__init__.py
--rwxr-xr-x  4.6 unx 29894144 b- defN 24-Apr-07 19:19 whitebox_workflows/whitebox_workflows.pyd
--rw-r--r--  4.6 unx     1398 b- defN 24-Apr-07 19:19 whitebox_workflows-1.2.6.dist-info/RECORD
-15 files, 30025560 bytes uncompressed, 8964577 bytes compressed:  70.1%
+Zip file size: 8563099 bytes, number of entries: 16
+-rw-r--r--  4.6 unx    12328 b- defN 24-Apr-15 17:35 whitebox_workflows-1.2.7.dist-info/METADATA
+-rw-r--r--  4.6 unx      102 b- defN 24-Apr-15 17:35 whitebox_workflows-1.2.7.dist-info/WHEEL
+-rw-r--r--  4.6 unx      161 b- defN 24-Apr-15 17:35 whitebox_workflows-1.2.7.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx    89775 b- defN 24-Apr-15 17:35 whitebox_workflows/whitebox_workflows.pyi
+-rw-r--r--  4.6 unx    15070 b- defN 24-Apr-15 17:35 whitebox_workflows/__init__.py
+-rw-r--r--  4.6 unx     8175 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/horton_ratios.py
+-rw-r--r--  4.6 unx     2108 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/nibble.py
+-rw-r--r--  4.6 unx     1810 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/ridge_and_valley_vectors.py
+-rw-r--r--  4.6 unx     1736 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/improved_ground_point_filter.py
+-rw-r--r--  4.6 unx      942 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/sieve.py
+-rw-r--r--  4.6 unx        0 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/__init__.py
+-rw-r--r--  4.6 unx      872 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/utils.py
+-rw-r--r--  4.6 unx     1021 b- defN 24-Apr-15 17:35 whitebox_workflows/scripts/scripts.py
+-rw-r--r--  4.6 unx        0 b- defN 24-Apr-15 17:35 whitebox_workflows/py.typed
+-rwxr-xr-x  4.6 unx 25697000 b- defN 24-Apr-15 17:35 whitebox_workflows/whitebox_workflows.abi3.so
+-rw-r--r--  4.6 unx     1518 b- defN 24-Apr-15 17:35 whitebox_workflows-1.2.7.dist-info/RECORD
+16 files, 25832618 bytes uncompressed, 8560535 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,46 +1,49 @@
-Filename: whitebox_workflows-1.2.6.dist-info/METADATA
+Filename: whitebox_workflows-1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: whitebox_workflows-1.2.6.dist-info/WHEEL
+Filename: whitebox_workflows-1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: whitebox_workflows-1.2.6.dist-info/license_files/LICENSE.txt
+Filename: whitebox_workflows-1.2.7.dist-info/license_files/LICENSE.txt
 Comment: 
 
-Filename: whitebox_workflows/py.typed
+Filename: whitebox_workflows/whitebox_workflows.pyi
+Comment: 
+
+Filename: whitebox_workflows/__init__.py
 Comment: 
 
 Filename: whitebox_workflows/scripts/horton_ratios.py
 Comment: 
 
 Filename: whitebox_workflows/scripts/nibble.py
 Comment: 
 
 Filename: whitebox_workflows/scripts/ridge_and_valley_vectors.py
 Comment: 
 
-Filename: whitebox_workflows/scripts/scripts.py
+Filename: whitebox_workflows/scripts/improved_ground_point_filter.py
 Comment: 
 
 Filename: whitebox_workflows/scripts/sieve.py
 Comment: 
 
-Filename: whitebox_workflows/scripts/utils.py
+Filename: whitebox_workflows/scripts/__init__.py
 Comment: 
 
-Filename: whitebox_workflows/scripts/__init__.py
+Filename: whitebox_workflows/scripts/utils.py
 Comment: 
 
-Filename: whitebox_workflows/whitebox_workflows.pyi
+Filename: whitebox_workflows/scripts/scripts.py
 Comment: 
 
-Filename: whitebox_workflows/__init__.py
+Filename: whitebox_workflows/py.typed
 Comment: 
 
-Filename: whitebox_workflows/whitebox_workflows.pyd
+Filename: whitebox_workflows/whitebox_workflows.abi3.so
 Comment: 
 
-Filename: whitebox_workflows-1.2.6.dist-info/RECORD
+Filename: whitebox_workflows-1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## whitebox_workflows/scripts/horton_ratios.py

 * *Ordering differences only*

```diff
@@ -1,275 +1,275 @@
-from math import log, log2, exp
-from typing import Tuple
-from whitebox_workflows import PhotometricInterpretation, RasterDataType, Raster, WbEnvironmentBase
-from .utils import print_tool_header
-
-def horton_ratios(wbe: WbEnvironmentBase, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]:
-    
-    reset_verbose = wbe.verbose
-    if wbe.verbose:
-        print_tool_header("horton_ratios")
-        print("\nPerforming operation...")
-
-    wbe.verbose = False # suppress the output from each of the workflow components
-    
-    esri_pntr = False
-    zero_background = True
-
-    if reset_verbose:
-        print("Calculating the D8 pointer raster...")
-    d8_pntr = wbe.d8_pointer(dem, esri_pntr)
-
-    if reset_verbose:
-        print("Calculating the stream order raster...")
-    strahler_order = wbe.strahler_stream_order(d8_pntr, streams_raster, esri_pntr, zero_background)
-
-    if reset_verbose:
-        print("Calculating the stream link ID raster...")
-    out_configs = dem.configs
-    out_configs.data_type = RasterDataType.I16
-    out_configs.photometric_interp = PhotometricInterpretation.Categorical
-    stream_link_id = wbe.new_raster(out_configs)
-    num_inflowing = wbe.new_raster(out_configs)
-
-    dx = (1, 1, 1, 0, -1, -1, -1, 0)
-    dy = (-1, 0, 1, 1, 1, 0, -1, -1)
-    inflowing_neighbour = (16, 32, 64, 128, 1, 2, 4, 8)
-    channel_heads = []
-    for row in range(dem.configs.rows):
-        for col in range(dem.configs.columns):
-            so = strahler_order[row, col]
-            if so > 0.0:
-                inflowing = 0
-                for n in range(8):
-                    fd = d8_pntr[row + dy[n], col + dx[n]]
-                    if fd == inflowing_neighbour[n] and streams_raster[row + dy[n], col + dx[n]] > 0.0:
-                        inflowing += 1
-                
-                if inflowing == 0: # It's a channel head
-                    channel_heads.append((row, col))
-                
-                num_inflowing[row, col] = inflowing
-                
-
-    link_id = 0
-    while len(channel_heads) > 0:
-        (row, col) = channel_heads.pop(0)
-        link_id += 1
-        so = strahler_order[row, col]
-        row_n = row
-        col_n = col
-        flag = True
-        while flag:
-            stream_link_id[row_n, col_n] = link_id
-
-            fd = d8_pntr[row_n, col_n]
-            if fd > 0.0:
-                n = int(log2(fd))
-                row_n += dy[n]
-                col_n += dx[n]
-                if strahler_order[row_n, col_n] > 0: # It's still a stream cell
-                    num_inflowing[row_n, col_n] -= 1
-                    if stream_link_id[row_n, col_n] < 1.0: # It hasn't yet been assigned
-                        if num_inflowing[row_n, col_n] < 1.0: # We've solved all inflowing cells
-                            if strahler_order[row_n, col_n] != so: # We've encountered a differing stream order
-                                so = strahler_order[row_n, col_n]
-                                link_id += 1
-                        else:
-                            flag = False
-                    else:
-                        flag = False
-                else:
-                    flag = False
-            else:
-                flag = False
-
-
-    if reset_verbose:      
-        print("Calculating the stream length raster...")
-    stream_length = wbe.stream_link_length(d8_pntr, stream_link_id, esri_pntr, zero_background)
-    
-    if reset_verbose:
-        print("Calculating the drainage area raster...")
-    drainage_area = wbe.d8_flow_accum(d8_pntr, out_type = "CA", log_transform = False, clip = False, input_is_pointer = True, esri_pntr = esri_pntr)
-
-    if reset_verbose:
-        print("Calculating the stream link slope raster...")
-    stream_link_slope = wbe.stream_link_slope(d8_pntr, stream_link_id, dem, esri_pntr, zero_background)
-
-
-
-    max_order = 0
-    link_order = {}
-    link_length = {}
-    link_area = {}
-    link_slope = {}
-    old_progress = -1 # initialize the variable
-    for row in range(dem.configs.rows):
-        for col in range(dem.configs.columns):
-            id = stream_link_id[row, col]
-            if id > 0.0:
-                order = int(strahler_order[row, col])
-                if order > max_order:
-                    max_order = order
-
-                link_order[id] = order
-                link_length[id] = stream_length[row, col] 
-                link_area[id] = max(link_area.get(id, 0.0), drainage_area[row, col])
-                link_slope[id] = stream_link_slope[row, col]
-                
-        # Update the progress once we've completed another 1% of points.
-        progress = int((row + 1.0) / dem.configs.rows * 100.0)
-        if progress != old_progress and reset_verbose:
-            old_progress = progress
-            print(f'Progress: {progress}%')
-
-    #####################
-    # Bifurcation ratio #
-    #####################
-    stream_num = [0] * max_order
-    for id in link_order:
-        so = link_order[id]
-        stream_num[so-1] += 1
-
-    sum_x = 0.0
-    sum_y = 0.0
-    sum_xy = 0.0
-    sum_xx = 0.0
-    sum_yy = 0.0
-    n = 0.0
-    for so in range(max_order):
-        sn = stream_num[so]
-        if sn > 0.0:
-            x = so + 1.0
-            y = log(sn)
-
-            sum_x += x
-            sum_y += y
-            sum_xy += x * y
-            sum_xx += x * x
-            sum_yy += y * y
-            n += 1.0
-
-
-    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
-
-    bifurcation_ratio = exp(-slope)
-
-
-    #######################
-    # Stream-length ratio #
-    #######################
-
-    # We need to calculate the mean length for each stream order
-    total_length = [0] * max_order
-    for id in link_length:
-        so = link_order[id]
-        length = link_length[id]
-        total_length[so-1] += length
-
-    average_length = []
-    for so in range(max_order):
-        sn = stream_num[so]
-        average_length.append(total_length[so]/ sn)
-
-    sum_x = 0.0
-    sum_y = 0.0
-    sum_xy = 0.0
-    sum_xx = 0.0
-    sum_yy = 0.0
-    n = 0.0
-    for so in range(max_order):
-        sn = stream_num[so]
-        if sn > 0.0:
-            x = so + 1.0
-            y = log(total_length[so] / sn)
-
-            sum_x += x
-            sum_y += y
-            sum_xy += x * y
-            sum_xx += x * x
-            sum_yy += y * y
-            n += 1.0
-
-
-    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
-
-    length_ratio = exp(slope)
-
-
-    #######################
-    # Drainage-area ratio #
-    #######################
-
-    # We need to calculate the mean drainage area for each stream order
-    total_area = [0] * max_order
-    for id in link_area:
-        so = link_order[id]
-        area = link_area[id]
-        total_area[so-1] += area
-
-    sum_x = 0.0
-    sum_y = 0.0
-    sum_xy = 0.0
-    sum_xx = 0.0
-    sum_yy = 0.0
-    n = 0.0
-    for so in range(max_order):
-        sn = stream_num[so]
-        if sn > 0.0:
-            x = so + 1.0
-            y = log(total_area[so] / sn)
-
-            sum_x += x
-            sum_y += y
-            sum_xy += x * y
-            sum_xx += x * x
-            sum_yy += y * y
-            n += 1.0
-
-
-    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
-
-    area_ratio = exp(slope)
-
-
-    ######################
-    # Stream-slope ratio #
-    ######################
-
-    # We need to calculate the mean link slope for each stream order
-    total_slope = [0] * max_order
-    for id in link_slope:
-        so = link_order[id]
-        slope = link_slope[id]
-        total_slope[so-1] += slope
-
-    sum_x = 0.0
-    sum_y = 0.0
-    sum_xy = 0.0
-    sum_xx = 0.0
-    sum_yy = 0.0
-    n = 0.0
-    for so in range(max_order):
-        sn = stream_num[so]
-        if sn > 0.0:
-            x = so + 1.0
-            y = log(total_slope[so] / sn)
-
-            sum_x += x
-            sum_y += y
-            sum_xy += x * y
-            sum_xx += x * x
-            sum_yy += y * y
-            n += 1.0
-
-
-    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
-
-    slope_ratio = exp(-slope)
-
-
-    wbe.verbose = reset_verbose
-
-    return (bifurcation_ratio, length_ratio, area_ratio, slope_ratio)
-
+from math import log, log2, exp
+from typing import Tuple
+from whitebox_workflows import PhotometricInterpretation, RasterDataType, Raster, WbEnvironmentBase
+from .utils import print_tool_header
+
+def horton_ratios(wbe: WbEnvironmentBase, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]:
+    
+    reset_verbose = wbe.verbose
+    if wbe.verbose:
+        print_tool_header("horton_ratios")
+        print("\nPerforming operation...")
+
+    wbe.verbose = False # suppress the output from each of the workflow components
+    
+    esri_pntr = False
+    zero_background = True
+
+    if reset_verbose:
+        print("Calculating the D8 pointer raster...")
+    d8_pntr = wbe.d8_pointer(dem, esri_pntr)
+
+    if reset_verbose:
+        print("Calculating the stream order raster...")
+    strahler_order = wbe.strahler_stream_order(d8_pntr, streams_raster, esri_pntr, zero_background)
+
+    if reset_verbose:
+        print("Calculating the stream link ID raster...")
+    out_configs = dem.configs
+    out_configs.data_type = RasterDataType.I16
+    out_configs.photometric_interp = PhotometricInterpretation.Categorical
+    stream_link_id = wbe.new_raster(out_configs)
+    num_inflowing = wbe.new_raster(out_configs)
+
+    dx = (1, 1, 1, 0, -1, -1, -1, 0)
+    dy = (-1, 0, 1, 1, 1, 0, -1, -1)
+    inflowing_neighbour = (16, 32, 64, 128, 1, 2, 4, 8)
+    channel_heads = []
+    for row in range(dem.configs.rows):
+        for col in range(dem.configs.columns):
+            so = strahler_order[row, col]
+            if so > 0.0:
+                inflowing = 0
+                for n in range(8):
+                    fd = d8_pntr[row + dy[n], col + dx[n]]
+                    if fd == inflowing_neighbour[n] and streams_raster[row + dy[n], col + dx[n]] > 0.0:
+                        inflowing += 1
+                
+                if inflowing == 0: # It's a channel head
+                    channel_heads.append((row, col))
+                
+                num_inflowing[row, col] = inflowing
+                
+
+    link_id = 0
+    while len(channel_heads) > 0:
+        (row, col) = channel_heads.pop(0)
+        link_id += 1
+        so = strahler_order[row, col]
+        row_n = row
+        col_n = col
+        flag = True
+        while flag:
+            stream_link_id[row_n, col_n] = link_id
+
+            fd = d8_pntr[row_n, col_n]
+            if fd > 0.0:
+                n = int(log2(fd))
+                row_n += dy[n]
+                col_n += dx[n]
+                if strahler_order[row_n, col_n] > 0: # It's still a stream cell
+                    num_inflowing[row_n, col_n] -= 1
+                    if stream_link_id[row_n, col_n] < 1.0: # It hasn't yet been assigned
+                        if num_inflowing[row_n, col_n] < 1.0: # We've solved all inflowing cells
+                            if strahler_order[row_n, col_n] != so: # We've encountered a differing stream order
+                                so = strahler_order[row_n, col_n]
+                                link_id += 1
+                        else:
+                            flag = False
+                    else:
+                        flag = False
+                else:
+                    flag = False
+            else:
+                flag = False
+
+
+    if reset_verbose:      
+        print("Calculating the stream length raster...")
+    stream_length = wbe.stream_link_length(d8_pntr, stream_link_id, esri_pntr, zero_background)
+    
+    if reset_verbose:
+        print("Calculating the drainage area raster...")
+    drainage_area = wbe.d8_flow_accum(d8_pntr, out_type = "CA", log_transform = False, clip = False, input_is_pointer = True, esri_pntr = esri_pntr)
+
+    if reset_verbose:
+        print("Calculating the stream link slope raster...")
+    stream_link_slope = wbe.stream_link_slope(d8_pntr, stream_link_id, dem, esri_pntr, zero_background)
+
+
+
+    max_order = 0
+    link_order = {}
+    link_length = {}
+    link_area = {}
+    link_slope = {}
+    old_progress = -1 # initialize the variable
+    for row in range(dem.configs.rows):
+        for col in range(dem.configs.columns):
+            id = stream_link_id[row, col]
+            if id > 0.0:
+                order = int(strahler_order[row, col])
+                if order > max_order:
+                    max_order = order
+
+                link_order[id] = order
+                link_length[id] = stream_length[row, col] 
+                link_area[id] = max(link_area.get(id, 0.0), drainage_area[row, col])
+                link_slope[id] = stream_link_slope[row, col]
+                
+        # Update the progress once we've completed another 1% of points.
+        progress = int((row + 1.0) / dem.configs.rows * 100.0)
+        if progress != old_progress and reset_verbose:
+            old_progress = progress
+            print(f'Progress: {progress}%')
+
+    #####################
+    # Bifurcation ratio #
+    #####################
+    stream_num = [0] * max_order
+    for id in link_order:
+        so = link_order[id]
+        stream_num[so-1] += 1
+
+    sum_x = 0.0
+    sum_y = 0.0
+    sum_xy = 0.0
+    sum_xx = 0.0
+    sum_yy = 0.0
+    n = 0.0
+    for so in range(max_order):
+        sn = stream_num[so]
+        if sn > 0.0:
+            x = so + 1.0
+            y = log(sn)
+
+            sum_x += x
+            sum_y += y
+            sum_xy += x * y
+            sum_xx += x * x
+            sum_yy += y * y
+            n += 1.0
+
+
+    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
+
+    bifurcation_ratio = exp(-slope)
+
+
+    #######################
+    # Stream-length ratio #
+    #######################
+
+    # We need to calculate the mean length for each stream order
+    total_length = [0] * max_order
+    for id in link_length:
+        so = link_order[id]
+        length = link_length[id]
+        total_length[so-1] += length
+
+    average_length = []
+    for so in range(max_order):
+        sn = stream_num[so]
+        average_length.append(total_length[so]/ sn)
+
+    sum_x = 0.0
+    sum_y = 0.0
+    sum_xy = 0.0
+    sum_xx = 0.0
+    sum_yy = 0.0
+    n = 0.0
+    for so in range(max_order):
+        sn = stream_num[so]
+        if sn > 0.0:
+            x = so + 1.0
+            y = log(total_length[so] / sn)
+
+            sum_x += x
+            sum_y += y
+            sum_xy += x * y
+            sum_xx += x * x
+            sum_yy += y * y
+            n += 1.0
+
+
+    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
+
+    length_ratio = exp(slope)
+
+
+    #######################
+    # Drainage-area ratio #
+    #######################
+
+    # We need to calculate the mean drainage area for each stream order
+    total_area = [0] * max_order
+    for id in link_area:
+        so = link_order[id]
+        area = link_area[id]
+        total_area[so-1] += area
+
+    sum_x = 0.0
+    sum_y = 0.0
+    sum_xy = 0.0
+    sum_xx = 0.0
+    sum_yy = 0.0
+    n = 0.0
+    for so in range(max_order):
+        sn = stream_num[so]
+        if sn > 0.0:
+            x = so + 1.0
+            y = log(total_area[so] / sn)
+
+            sum_x += x
+            sum_y += y
+            sum_xy += x * y
+            sum_xx += x * x
+            sum_yy += y * y
+            n += 1.0
+
+
+    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
+
+    area_ratio = exp(slope)
+
+
+    ######################
+    # Stream-slope ratio #
+    ######################
+
+    # We need to calculate the mean link slope for each stream order
+    total_slope = [0] * max_order
+    for id in link_slope:
+        so = link_order[id]
+        slope = link_slope[id]
+        total_slope[so-1] += slope
+
+    sum_x = 0.0
+    sum_y = 0.0
+    sum_xy = 0.0
+    sum_xx = 0.0
+    sum_yy = 0.0
+    n = 0.0
+    for so in range(max_order):
+        sn = stream_num[so]
+        if sn > 0.0:
+            x = so + 1.0
+            y = log(total_slope[so] / sn)
+
+            sum_x += x
+            sum_y += y
+            sum_xy += x * y
+            sum_xx += x * x
+            sum_yy += y * y
+            n += 1.0
+
+
+    slope = (n * sum_xy - (sum_x * sum_y)) / (n * sum_xx - (sum_x * sum_x))
+
+    slope_ratio = exp(-slope)
+
+
+    wbe.verbose = reset_verbose
+
+    return (bifurcation_ratio, length_ratio, area_ratio, slope_ratio)
+
```

## whitebox_workflows/scripts/nibble.py

 * *Ordering differences only*

```diff
@@ -1,51 +1,51 @@
-from whitebox_workflows import LicenseType, Raster, WbEnvironmentBase
-from .utils import LicenseError, print_tool_header
-
-def nibble(wbe: WbEnvironmentBase, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
-    if wbe.license_type != LicenseType.WbWPro:
-        raise LicenseError()
-    
-    reset_verbose = wbe.verbose
-    if wbe.verbose:
-        print_tool_header("nibble")
-        print("\nPerforming operation...")
-
-    wbe.verbose = False # suppress the output from each of the workflow components
-    
-    # Nodata values and zero values are both treated the same in the mask layer
-    mask = mask.con('value==nodata', 0.0, 1.0)
-
-    # Find the nodata values in the input raster
-    input_nodata_mask = input_raster.con('value==nodata', 1.0, 0.0)
-    input_nodata = input_raster.configs.nodata
-
-    max_class_val = input_raster.configs.maximum
-        
-    if use_nodata:
-        # Reset nodata cells in the input raster to some arbitrary, but 
-        # previously unused, class value. This is necessary because the 
-        # eculidean_allocation function will simply ignore nodata values.
-        # This way eculidean_allocation will treat input raster nodata values
-        # like they are non-background values.
-        input_raster = input_raster.con('value==nodata', max_class_val + 1.0, input_raster) 
-    else:
-        # Convert all nodata values in the input raster to 0.0, so that it
-        # is treated like background values by euclidean_allocation. This
-        # will be rectified after the allocation.
-        input_raster = input_raster.con('value==nodata', 0.0, input_raster)
-    
-    tmp1 = input_raster * mask
-    nibble = wbe.euclidean_allocation(tmp1)
-
-    if use_nodata:
-        nibble = nibble.con(f"value=={max_class_val + 1.0}", input_nodata, nibble)
-    else:
-        nibble = (mask*input_nodata_mask).con('value==1.0', input_nodata, nibble)
-
-    if nibble_nodata:
-        tmp1 = (mask==0.0)*input_nodata_mask
-        nibble = tmp1.con('value==1.0', input_nodata, nibble)
-
-    wbe.verbose = reset_verbose
-
+from whitebox_workflows import LicenseType, Raster, WbEnvironmentBase
+from .utils import LicenseError, print_tool_header
+
+def nibble(wbe: WbEnvironmentBase, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
+    if wbe.license_type != LicenseType.WbWPro:
+        raise LicenseError()
+    
+    reset_verbose = wbe.verbose
+    if wbe.verbose:
+        print_tool_header("nibble")
+        print("\nPerforming operation...")
+
+    wbe.verbose = False # suppress the output from each of the workflow components
+    
+    # Nodata values and zero values are both treated the same in the mask layer
+    mask = mask.con('value==nodata', 0.0, 1.0)
+
+    # Find the nodata values in the input raster
+    input_nodata_mask = input_raster.con('value==nodata', 1.0, 0.0)
+    input_nodata = input_raster.configs.nodata
+
+    max_class_val = input_raster.configs.maximum
+        
+    if use_nodata:
+        # Reset nodata cells in the input raster to some arbitrary, but 
+        # previously unused, class value. This is necessary because the 
+        # eculidean_allocation function will simply ignore nodata values.
+        # This way eculidean_allocation will treat input raster nodata values
+        # like they are non-background values.
+        input_raster = input_raster.con('value==nodata', max_class_val + 1.0, input_raster) 
+    else:
+        # Convert all nodata values in the input raster to 0.0, so that it
+        # is treated like background values by euclidean_allocation. This
+        # will be rectified after the allocation.
+        input_raster = input_raster.con('value==nodata', 0.0, input_raster)
+    
+    tmp1 = input_raster * mask
+    nibble = wbe.euclidean_allocation(tmp1)
+
+    if use_nodata:
+        nibble = nibble.con(f"value=={max_class_val + 1.0}", input_nodata, nibble)
+    else:
+        nibble = (mask*input_nodata_mask).con('value==1.0', input_nodata, nibble)
+
+    if nibble_nodata:
+        tmp1 = (mask==0.0)*input_nodata_mask
+        nibble = tmp1.con('value==1.0', input_nodata, nibble)
+
+    wbe.verbose = reset_verbose
+
     return nibble
```

## whitebox_workflows/scripts/ridge_and_valley_vectors.py

 * *Ordering differences only*

```diff
@@ -1,43 +1,43 @@
-from typing import Tuple
-from whitebox_workflows import LicenseType, Raster, Vector, WbEnvironmentBase
-from .utils import LicenseError, print_tool_header
-
-def ridge_and_valley_vectors(wbe: WbEnvironmentBase, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]:
-    if wbe.license_type != LicenseType.WbWPro:
-        raise LicenseError()
-    
-    reset_verbose = wbe.verbose
-    if wbe.verbose:
-        print_tool_header("ridge_and_valley_vectors")
-
-    if ep_threshold < 5.0:
-        ep_threshold = 5.0
-
-    if ep_threshold > 50.0:
-        ep_threshold = 50.0
-
-    if slope_threshold < 0.0:
-        slope_threshold = 0.0
-
-    wbe.verbose = False # suppress the output from each of the workflow components
-    
-    if reset_verbose:
-        print("Calculating EP and slope...")
-    ep = wbe.elevation_percentile(dem, filter_size_x=filter_size, filter_size_y=filter_size, sig_digits=2)
-    slope = wbe.slope(dem)
-
-    if reset_verbose:
-        print("\nMapping ridges and valleys...")
-    ridges = (ep > (100.0 - ep_threshold))*(slope > slope_threshold)
-    ridges = wbe.remove_raster_polygon_holes(ridges, 10, True) # Remove small holes
-    ridges = wbe.closing(ridges, filter_size_x=5, filter_size_y=5) # Simplify the shapes
-    ridge_lines = wbe.river_centerlines(ridges, min_length=min_length, search_radius=9)
-    
-    valleys = (ep < ep_threshold)*(slope > slope_threshold)
-    valleys = wbe.remove_raster_polygon_holes(valleys, 10, True) # Remove small holes
-    valleys = wbe.closing(valleys, filter_size_x=5, filter_size_y=5) # Simplify the shapes
-    valley_lines = wbe.river_centerlines(valleys, min_length=min_length, search_radius=9)
-    
-    wbe.verbose = reset_verbose
-
+from typing import Tuple
+from whitebox_workflows import LicenseType, Raster, Vector, WbEnvironmentBase
+from .utils import LicenseError, print_tool_header
+
+def ridge_and_valley_vectors(wbe: WbEnvironmentBase, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]:
+    if wbe.license_type != LicenseType.WbWPro:
+        raise LicenseError()
+    
+    reset_verbose = wbe.verbose
+    if wbe.verbose:
+        print_tool_header("ridge_and_valley_vectors")
+
+    if ep_threshold < 5.0:
+        ep_threshold = 5.0
+
+    if ep_threshold > 50.0:
+        ep_threshold = 50.0
+
+    if slope_threshold < 0.0:
+        slope_threshold = 0.0
+
+    wbe.verbose = False # suppress the output from each of the workflow components
+    
+    if reset_verbose:
+        print("Calculating EP and slope...")
+    ep = wbe.elevation_percentile(dem, filter_size_x=filter_size, filter_size_y=filter_size, sig_digits=2)
+    slope = wbe.slope(dem)
+
+    if reset_verbose:
+        print("\nMapping ridges and valleys...")
+    ridges = (ep > (100.0 - ep_threshold))*(slope > slope_threshold)
+    ridges = wbe.remove_raster_polygon_holes(ridges, 10, True) # Remove small holes
+    ridges = wbe.closing(ridges, filter_size_x=5, filter_size_y=5) # Simplify the shapes
+    ridge_lines = wbe.river_centerlines(ridges, min_length=min_length, search_radius=9)
+    
+    valleys = (ep < ep_threshold)*(slope > slope_threshold)
+    valleys = wbe.remove_raster_polygon_holes(valleys, 10, True) # Remove small holes
+    valleys = wbe.closing(valleys, filter_size_x=5, filter_size_y=5) # Simplify the shapes
+    valley_lines = wbe.river_centerlines(valleys, min_length=min_length, search_radius=9)
+    
+    wbe.verbose = reset_verbose
+
     return (ridge_lines, valley_lines)
```

## whitebox_workflows/scripts/scripts.py

 * *Ordering differences only*

```diff
@@ -1,25 +1,25 @@
-from whitebox_workflows import Lidar, WbEnvironmentBase, whitebox_workflows
-
-def strip_last_return_points(wbe: WbEnvironmentBase, lidar: Lidar) -> Lidar:
-    num_points = lidar.header.get_num_points()
-
-    # Create a new lidar data set.
-    lidar_out = wbe.new_lidar(lidar.header)
-    lidar_out.vlr_data = lidar.vlr_data
-
-    print('Filtering point data...')
-    old_progress = -1 # initialize the variable
-    for i in range(num_points):
-        point_data, time, colour, waveform = lidar.get_point_record(i)
-
-        # Now let's filter the data based on return data...
-        if not point_data.is_last_return(): # point_data.is_first_return() or point_data.is_intermediate_return():
-            lidar_out.add_point(point_data, time, colour, waveform)
-
-        # Update the progress once we've completed another 1% of points.
-        progress = int((i + 1.0) / num_points * 100.0)
-        if progress != old_progress:
-            old_progress = progress
-            print(f'Progress: {progress}%')
-
+from whitebox_workflows import Lidar, WbEnvironmentBase, whitebox_workflows
+
+def strip_last_return_points(wbe: WbEnvironmentBase, lidar: Lidar) -> Lidar:
+    num_points = lidar.header.get_num_points()
+
+    # Create a new lidar data set.
+    lidar_out = wbe.new_lidar(lidar.header)
+    lidar_out.vlr_data = lidar.vlr_data
+
+    print('Filtering point data...')
+    old_progress = -1 # initialize the variable
+    for i in range(num_points):
+        point_data, time, colour, waveform = lidar.get_point_record(i)
+
+        # Now let's filter the data based on return data...
+        if not point_data.is_last_return(): # point_data.is_first_return() or point_data.is_intermediate_return():
+            lidar_out.add_point(point_data, time, colour, waveform)
+
+        # Update the progress once we've completed another 1% of points.
+        progress = int((i + 1.0) / num_points * 100.0)
+        if progress != old_progress:
+            old_progress = progress
+            print(f'Progress: {progress}%')
+
     return lidar_out
```

## whitebox_workflows/scripts/sieve.py

 * *Ordering differences only*

```diff
@@ -1,26 +1,26 @@
-from whitebox_workflows import LicenseType, Raster, WbEnvironmentBase
-from .utils import LicenseError, print_tool_header
-
-def sieve(wbe: WbEnvironmentBase, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster:
-    if wbe.license_type != LicenseType.WbWPro:
-        raise LicenseError()
-    
-    reset_verbose = wbe.verbose
-    if wbe.verbose:
-        print_tool_header("sieve")
-        print("\nPerforming operation...")
-
-    wbe.verbose = False # suppress the output from each of the workflow components
-
-    clump = wbe.clump(input_raster, diag=True, zero_background=False)
-    area, report = wbe.raster_area(clump, units="cells", zero_background=False)
-    mask = area >= threshold
-    mask = mask.con('value==0', mask.configs.nodata, mask)
-    sieved = wbe.nibble(input_raster, mask)
-
-    if zero_background:
-        sieved = (input_raster != 0.0) * sieved
-
-    wbe.verbose = reset_verbose
-
+from whitebox_workflows import LicenseType, Raster, WbEnvironmentBase
+from .utils import LicenseError, print_tool_header
+
+def sieve(wbe: WbEnvironmentBase, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster:
+    if wbe.license_type != LicenseType.WbWPro:
+        raise LicenseError()
+    
+    reset_verbose = wbe.verbose
+    if wbe.verbose:
+        print_tool_header("sieve")
+        print("\nPerforming operation...")
+
+    wbe.verbose = False # suppress the output from each of the workflow components
+
+    clump = wbe.clump(input_raster, diag=True, zero_background=False)
+    area, report = wbe.raster_area(clump, units="cells", zero_background=False)
+    mask = area >= threshold
+    mask = mask.con('value==0', mask.configs.nodata, mask)
+    sieved = wbe.nibble(input_raster, mask)
+
+    if zero_background:
+        sieved = (input_raster != 0.0) * sieved
+
+    wbe.verbose = reset_verbose
+
     return sieved
```

## whitebox_workflows/scripts/utils.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-class LicenseError(Exception):
-    def __init__(self, message="This function requires a license for WbW-Pro. Please visit www.whiteboxgeo.com to purchase a license for WbW-Pro."):            
-        self.message = message
-        super().__init__(self.message)
-
-def print_tool_header(tool_name: str):
-    # 44 = length of the 'Powered by' by statement.
-    powered_by_statement_length = 44
-    welcome_len = max(len(f"* Welcome to {tool_name} *", ), powered_by_statement_length)
-    stars = "*" * welcome_len
-    print(f"{stars}")
-    spaces = " " * (welcome_len - 15 - len(tool_name))
-    print(f"* Welcome to {tool_name} {spaces}*")
-    spaces = " " * (welcome_len - powered_by_statement_length)
-    print(f"* Powered by Whitebox Workflows for Python {spaces}*")
-    spaces = " " * (welcome_len - 23)
-    print(f"* www.whiteboxgeo.com {spaces}*")
-    print(f"{stars}")
+class LicenseError(Exception):
+    def __init__(self, message="This function requires a license for WbW-Pro. Please visit www.whiteboxgeo.com to purchase a license for WbW-Pro."):            
+        self.message = message
+        super().__init__(self.message)
+
+def print_tool_header(tool_name: str):
+    # 44 = length of the 'Powered by' by statement.
+    powered_by_statement_length = 44
+    welcome_len = max(len(f"* Welcome to {tool_name} *", ), powered_by_statement_length)
+    stars = "*" * welcome_len
+    print(f"{stars}")
+    spaces = " " * (welcome_len - 15 - len(tool_name))
+    print(f"* Welcome to {tool_name} {spaces}*")
+    spaces = " " * (welcome_len - powered_by_statement_length)
+    print(f"* Powered by Whitebox Workflows for Python {spaces}*")
+    spaces = " " * (welcome_len - 23)
+    print(f"* www.whiteboxgeo.com {spaces}*")
+    print(f"{stars}")
```

## whitebox_workflows/whitebox_workflows.pyi

```diff
@@ -1,2195 +1,2201 @@
-import sys
-from typing import List, Optional, Tuple, Union
-from enum import Enum
-
-def activate_license(key: str, firstname: str, lastname: str, email: str, agree_to_license_terms: bool) -> None: ...
-
-def check_in_license(key: str) -> str: ...
-
-def deactivate_license() -> None: ...
-
-def download_sample_data(data_set: str) -> str: ...
-
-def license_info() -> None: ...
-
-def transfer_license() -> None: ...
-
-class AttributeField():
-
-	@property
-	def name(self) -> str: ...
-    		
-	@property
-	def field_type(self) -> int: ...
-    
-	@property
-	def field_length(self) -> int: ...
-    	
-	@property
-	def decimal_count(self) -> int: ...
-
-	@staticmethod
-	def new(name: str, field_type: FieldDataType, field_length: int, decimal_count: int) -> AttributeField: ...
-
-class AttributeHeader():
-	@property
-	def version(self) -> int: ...
-
-	@property
-	def year(self) -> int: ...
-
-	@property
-	def month(self) -> int: ...
-
-	@property
-	def day(self) -> int: ...
-
-	@property
-	def num_records(self) -> int: ...
-
-	@property
-	def num_fields(self) -> int: ...
-
-	@property
-	def bytes_in_header(self) -> int: ...
-
-	@property
-	def bytes_in_record(self) -> int: ...
-
-	@property
-	def incomplete_tansaction(self) -> int: ...
-
-	@property
-	def encryption_flag(self) -> int: ...
-
-	@property
-	def mdx_flag(self) -> int: ...
-
-	@property
-	def language_driver_id(self) -> int: ...
-
-class BoundingBox():
-	@property
-	def min_x(self) -> float: ...
-
-	@min_x.setter
-	def min_x(self, value: float) -> None: ...
-
-	@property
-	def min_y(self) -> float: ...
-
-	@min_y.setter
-	def min_y(self, value: float) -> None: ...
-
-	@property
-	def max_x(self) -> float: ...
-
-	@max_x.setter
-	def max_x(self, value: float) -> None: ...
-
-	@property
-	def max_y(self) -> float: ...
-
-	@max_y.setter
-	def max_y(self, value: float) -> None: ...
-
-	@staticmethod
-	def new(min_x: float, max_x: float, min_y: float, max_y: float) -> Point2D: ...
-
-	@staticmethod
-	def from_two_points(p1: Point2D, p2: Point2D) -> BoundingBox: ...
-
-	def initialize_to_inf(self) -> None: ...
-
-	def get_height(self) -> float: ...
-
-	def get_width(self) -> float: ...
-
-	def is_point_in_box(self, x: float, y: float) -> bool: ...
-
-	def overlaps(self, other: BoundingBox) -> bool: ...
-
-	def nearly_overlaps(self, other: BoundingBox) -> bool: ...
-
-	def intersects_edge_of(self, other: BoundingBox) -> bool: ...
-
-	def entirely_contained_within(self, other: BoundingBox) -> bool: ...
-
-	def within(self, other: BoundingBox) -> bool: ...
-
-	def entirely_contains(self, other: BoundingBox) -> bool: ...
-
-	def contains(self, other: BoundingBox) -> bool: ...
-
-	def intersect(self, other: BoundingBox) -> BoundingBox: ...
-
-	def expand_to(self, other: BoundingBox) -> None: ...
-
-	def contract_to(self, other: BoundingBox) -> None: ...
-
-	def expand_by(self, value: float) -> None: ...
-
-	def contract_by(self, value: float) -> None: ...
-
-class ColourData():
-	@property
-	def red(self) -> int: ...
-
-	@red.setter
-	def red(self, value: int) -> None: ...
-
-	@property
-	def green(self) -> int: ...
-
-	@green.setter
-	def green(self, value: int) -> None: ...
-
-	@property
-	def blue(self) -> int: ...
-
-	@blue.setter
-	def blue(self, value: int) -> None: ...
-
-	@property
-	def nir(self) -> int: ...
-
-	@nir.setter
-	def nir(self, value: int) -> None: ...
-
-class DateData():
-	@property
-	def year(self) -> int: ...
-
-	@property
-	def month(self) -> int: ...
-
-	@property
-	def day(self) -> int: ...	
-	
-class FieldData():
-	@staticmethod
-	def new() -> FieldData: ...
-
-	@staticmethod
-	def new_int(value: int) -> FieldData: ...
-
-	@staticmethod
-	def new_real(value: float) -> FieldData: ...
-
-	@staticmethod
-	def new_text(value: str) -> FieldData: ...
-
-	@staticmethod
-	def new_date(value: DateData) -> FieldData: ...
-
-	@staticmethod
-	def new_bool(value: bool) -> FieldData: ...
-
-	@staticmethod
-	def new_null() -> FieldData: ...
-
-	def get_type(self) -> FieldDataType: ...
-
-	def get_value_as_f64(self) -> float: ...
-
-	def get_as_string(self) -> str: ...
-
-class FieldDataType(Enum):
-	Bool: int
-	Date: int
-	Int: int
-	Real: int
-	Text: int
-
-class GlobalEncodingField():
-	def __init__(self):
-		self.value = 0
-
-class LicenseType(Enum):
-	WbW: str
-	WbWPro: str
-
-class LidarHeader(): 
-	@property
-	def file_signature(self) -> str: ...
-    
-	@property
-	def file_source_id(self) -> int: ...
-
-	@property
-	def global_encoding(self) -> GlobalEncodingField: ...
-
-	@property
-	def project_id_used(self) -> bool: ...
-	
-	@property
-	def project_id1(self) -> int: ...
-	
-	@property
-	def project_id2(self) -> int: ...
-
-	@property
-	def project_id3(self) -> int: ...
-
-	@property
-	def project_id4(self) -> Tuple[int]: ...
-
-	@property
-	def version_major(self) -> int: ...
-
-	@property
-	def version_minor(self) -> int: ...
-
-	@property
-	def system_id(self) -> str: ...
-
-	@property
-	def generating_software(self) -> str: ...
-
-	@property
-	def file_creation_day(self) -> int: ...
-
-	@property
-	def file_creation_year(self) -> int: ...
-
-	@property
-	def header_size(self) -> int: ...
-
-	@property
-	def offset_to_points(self) -> int: ...
-
-	@property
-	def number_of_vlrs(self) -> int: ...
-
-	@property
-	def number_of_extended_vlrs(self) -> int: ...
-
-	@property
-	def offset_to_ex_vlrs(self) -> int: ...
-
-	@property
-	def point_record_length(self) -> int: ...
-
-	@property
-	def point_format(self) -> int: ...
-
-	@property
-	def number_of_points_old(self) -> int: ...
-
-	@property
-	def number_of_points(self) -> int: ...
-
-	@property
-	def number_of_points_by_return_old(self) -> Tuple[int, int, int, int, int]: ...
-
-	@property
-	def number_of_points_by_return(self) -> Tuple[int, int, int, int, int, int, int, int, int, int, int, int, int, int, int]: ...
-
-	@property
-	def x_scale_factor(self) -> float: ...
-
-	@property
-	def y_scale_factor(self) -> float: ...
-
-	@property
-	def z_scale_factor(self) -> float: ...
-
-	@property
-	def x_offset(self) -> float: ...
-
-	@property
-	def y_offset(self) -> float: ...
-
-	@property
-	def z_offset(self) -> float: ...
-
-	@property
-	def max_x(self) -> float: ...
-
-	@property
-	def min_x(self) -> float: ...
-
-	@property
-	def max_y(self) -> float: ...
-
-	@property
-	def min_y(self) -> float: ...
-
-	@property
-	def max_z(self) -> float: ...
-
-	@property
-	def min_z(self) -> float: ...
-
-	@property
-	def waveform_data_start(self) -> int: ...
-
-	def get_num_points(self) -> int: ...
-
-class LidarPointData():
-	@property
-	def x(self) -> int: ...
-
-	@property
-	def y(self) -> int: ...
-
-	@property
-	def z(self) -> int: ...
-
-	@property
-	def intensity(self) -> int: ...
-
-	@property
-	def point_bit_field(self) -> int: ...
-
-	@property
-	def class_bit_field(self) -> int: ...
-
-	# @property
-	# def classification(self) -> int: ...
-
-	@property
-	def scan_angle(self) -> int: ...
-
-	@property
-	def user_data(self) -> int: ...
-
-	@property
-	def point_source_id(self) -> int: ...
-
-	@property
-	def is_64bit(self) -> bool: ...
-
-	def get_32bit_from_64bit(self) -> Tuple[int, int]: ...
-
-	def return_number(self) -> int: ...
-
-	def set_return_number(self, value: int) -> None: ...
-
-	def number_of_returns(self) -> int: ...
-
-	def set_number_of_returns(self, value: int) -> None: ...
-
-	def is_only_return(self) -> bool: ...
-
-	def is_multiple_return(self) -> bool: ...
-
-	def is_early_return(self) -> bool: ...
-
-	def is_late_return(self) -> bool: ...
-
-	def is_last_return(self) -> bool: ...
-
-	def is_first_return(self) -> bool: ...
-
-	def is_intermediate_return(self) -> bool: ...
-
-	def scan_direction_flag(self) -> bool: ...
-
-	def set_scan_direction_flag(self, value: bool) -> None: ...
-
-	def edge_of_flightline_flag(self) -> bool: ...
-
-	def set_edge_of_flightline_flag(self, value: bool) -> None: ...
-
-	def classification(self) -> int: ...
-
-	def set_classification(self, value: int) -> None: ...
-
-	def classification_string(self) -> str: ...
-
-	def is_classified_vegetation(self) -> bool: ...
-
-	def synthetic(self) -> bool: ...
-
-	def set_synthetic(self, value: bool) -> None: ...
-
-	def keypoint(self) -> bool: ...
-
-	def set_keypoint(self, value: bool) -> None: ...
-
-	def withheld(self) -> bool: ...
-
-	def set_withheld(self, value: bool) -> None: ...
-
-	def overlap(self) -> bool: ...
-
-	def set_overlap(self, value: bool) -> None: ...
-
-	def is_classified_noise(self) -> bool: ...
-
-	def scanner_channel(self) -> int: ...
-
-	def set_scanner_channel(self, value: int) -> None: ...
-
-class Lidar():
-    	
-	@property
-	def file_name(self) -> str: ...
-
-	@file_name.setter
-	def file_name(self, value: str): ...
-
-	@property
-	def header(self) -> LidarHeader: ...
-
-	@property
-	def vlr_data(self) -> List[VariableLengthRecord]: ...
-
-	@vlr_data.setter
-	def vlr_data(self, value: List[VariableLengthRecord]): ...
-
-	@property
-	def wkt(self) -> str: ...
-    
-	@property
-	def use_point_intensity(self) -> bool: ...
-    
-	@property
-	def use_point_userdata(self) -> bool: ...
-
-	def get_point_record(self, index: int) -> Tuple[LidarPointData, Optional[float], Optional[ColourData], Optional[WaveformPacket]]: ...
-
-	def get_transformed_xyz(self, index: int) -> Tuple[float, float, float]: ...
-
-	def add_point(self, point_data: LidarPointData, time: Optional[float] = None, colour_data: Optional[ColourData] = None, waveform_data: Optional[WaveformPacket] = None) -> None: ...
-
-	def has_time_data(self) -> bool: ...
-
-	def has_colour_data(self) -> bool: ...
-
-	def has_waveform_data(self) -> bool: ...
-
-	def get_well_known_text(self) -> str: ...
-
-	def print_variable_length_records(self) -> str: ...
-
-class PhotometricInterpretation(Enum):
-	Continuous: int
-	Categorical: int
-	Boolean: int
-	RGB: int
-	Paletted: int
-	Unknown: int
-
-class Point2D:
-	@property
-	def x(self) -> float: ...
-
-	@x.setter
-	def x(self, value: float) -> None: ...
-
-	@property
-	def y(self) -> float: ...
-
-	@y.setter
-	def y(self, value: float) -> None: ...
-
-	@staticmethod
-	def new(x: float, y: float) -> Point2D: ...
-
-class Point3D:
-	@property
-	def x(self) -> float: ...
-
-	@x.setter
-	def x(self, value: float) -> None: ...
-
-	@property
-	def y(self) -> float: ...
-
-	@y.setter
-	def y(self, value: float) -> None: ...
-
-	@property
-	def z(self) -> float: ...
-
-	@z.setter
-	def z(self, value: float) -> None: ...
-
-	@staticmethod
-	def new(x: float, y: float, z: float) -> Point2D: ...
-
-class RasterDataType(Enum):
-	F64: int
-	F32: int
-	I64: int
-	U64: int
-	RGB48: int
-	I32: int
-	U32: int
-	RGB24: int
-	RGBA32: int
-	I16: int
-	U16: int
-	I8: int
-	U8: int
-	Unknown: int
-
-
-	def get_data_size(self) -> int: ...
-
-	def is_float(self) -> bool: ...
-
-	def is_integer(self) -> bool: ...
-
-	def is_unsigned_integer(self) -> bool: ...
-
-	def is_signed_integer(self) -> bool: ...
-
-	def is_colour_data(self) -> bool: ...
-
-	def return_wider(self, other: RasterDataType) -> RasterDataType: ...
-
-class RasterConfigs():
-	@property
-	def title(self) -> str: ...
-
-	@title.setter
-	def title(self, value): ...
-
-	@property
-	def rows(self) -> int: ...
-
-	@rows.setter
-	def rows(self, value: int) -> None: ...
-
-	@property
-	def columns(self) -> int: ...
-
-	@columns.setter
-	def columns(self, value: int) -> None: ...
-
-	@property
-	def nodata(self) -> float: ...
-
-	@nodata.setter
-	def nodata(self, value: float) -> None: ...
-
-	@property
-	def north(self) -> float: ...
-
-	@north.setter
-	def north(self, value: float) -> None: ...
-
-	@property
-	def south(self) -> float: ...
-
-	@south.setter
-	def south(self, value: float) -> None: ...
-
-	@property
-	def east(self) -> float: ...
-
-	@east.setter
-	def east(self, value: float) -> None: ...
-
-	@property
-	def west(self) -> float: ...
-
-	@west.setter
-	def west(self, value: float) -> None: ...
-
-	@property
-	def resolution_x(self) -> float: ...
-
-	@resolution_x.setter
-	def resolution_x(self, value: float) -> None: ...
-
-	@property
-	def resolution_y(self) -> float: ...
-
-	@resolution_y.setter
-	def resolution_y(self, value: float) -> None: ...
-
-	@property
-	def minimum(self) -> float: ...
-
-	@minimum.setter
-	def minimum(self, value: float) -> None: ...
-
-	@property
-	def maximum(self) -> float: ...
-
-	@maximum.setter
-	def maximum(self, value: float) -> None: ...
-
-	# @property
-	# def display_min(self) -> float: ...
-
-	# @display_min.setter
-	# def display_min(self, value: float) -> None: ...
-
-	# @property
-	# def display_max(self) -> float: ...
-
-	# @display_max.setter
-	# def display_max(self, value: float) -> None: ...
-
-	@property
-	def palette(self) -> str: ...
-
-	@property
-	def projection(self) -> str: ...
-
-	@property
-	def photometric_interp(self) -> PhotometricInterpretation: ...
-
-	@photometric_interp.setter
-	def photometric_interp(self, value: PhotometricInterpretation) -> None: ...
-
-	@property
-	def data_type(self) -> RasterDataType: ...
-
-	@data_type.setter
-	def data_type(self, value: RasterDataType) -> None: ...
-
-	@property
-	def z_units(self) -> str: ...
-
-	@property
-	def xy_units(self) -> str: ...
-
-	@property
-	def reflect_at_edges(self) -> bool: ...
-
-	@reflect_at_edges.setter
-	def reflect_at_edges(self, value: bool) -> None: ...
-
-	@property
-	def pixel_is_area(self) -> bool: ...
-
-	@pixel_is_area.setter
-	def pixel_is_area(self, value: bool) -> None: ...
-
-	@property
-	def epsg_code(self) -> int: ...
-
-	@epsg_code.setter
-	def epsg_code(self, value: int) -> None: ...
-
-	@property
-	def coordinate_ref_system_wkt(self) -> str: ...
-
-	@epsg_code.setter
-	def coordinate_ref_system_wkt(self, value: str) -> None: ...
-
-	@staticmethod
-	def new() -> RasterConfigs: ...
-
-class RasterType():
-	Unknown: int
-	ArcAscii: int
-	ArcBinary: int
-	EsriBil: int
-	GeoTiff: int
-	GrassAscii: int
-	IdrisiBinary: int
-	SagaBinary: int
-	Surfer7Binary: int
-	SurferAscii: int
-	Whitebox: int
-
-class Raster():
-	@property
-	def file_name(self) -> str: ...
-
-	@file_name.setter
-	def file_name(self, value: str) -> None: ...
-
-	@property
-	def file_mode(self) -> str: ...
-	
-	@property
-	def raster_type(self) -> RasterType: ...
-
-	@property
-	def configs(self) -> RasterConfigs: ...
-
-	@staticmethod
-	def new_from_other(other: Raster, data_type: Optional[RasterDataType]) -> Raster: ...
-
-	def get_value(self, row: int, column: int) -> float: ...
-
-	def set_value(self, row: int, column: int, value: float) -> None: ...
-
-	def decrement(self, row: int, column: int, value: float) -> None: ...
-
-	def increment(self, row: int, column: int, value: float) -> None: ...
-
-	def set_row_data(self, row: int, values: List[float]) -> None: ...
-
-	def get_row_data(self, row: int) -> List[float]: ...
-
-	def increment_row_data(self, row: int, values: List[float]) -> None: ...
-
-	def decrement_row_data(self, row: int, values: List[float]) -> None: ...
-
-	def set_data_from_raster(self, other: Raster) -> Optional[str]: ...
-
-	def reinitialize_values(self, value: float) -> None: ...
-
-	def get_value_as_rgba(self, row: int, column: int) -> Tuple[int, int, int, int]: ...
-
-	def get_value_as_hsi(self, row: int, column: int) -> Tuple[float, float, float]: ...
-
-	def set_value_from_rgba(self, row: int, column: int, rgba: Tuple[int, int, int, int]) -> None: ...
-
-	def get_data_size_in_bytes(self) -> int: ...
-
-	def get_x_from_column(self, column: int) -> float: ...
-
-	def get_y_from_row(self, row: int) -> float: ...
-
-	def get_column_from_x(self, x: float) -> int: ...
-
-	def get_row_from_y(self, y: float) -> int: ...
-
-	def size_of(self) -> int: ...
-
-	def __add__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __sub__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __mul__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __truediv__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __floordiv__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __mod__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __pow__(self, other: Union[Raster, float], modulo: Optional[float] = None) -> Raster: ...
-
-	def __neg__(self) -> Raster: ...
-
-	def __abs__(self) -> Raster: ...
-
-	def __iadd__(self, other: Union[Raster, float]) -> None: ...
-
-	def __isub__(self, other: Union[Raster, float]) -> None: ...
-
-	def __imul__(self, other: Union[Raster, float]) -> None: ...
-
-	def __idiv__(self, other: Union[Raster, float]) -> None: ...
-
-	def __getitem__(self, row_column: Tuple[int, int]) -> float: ...
-
-	def __setitem__(self, row_column: Tuple[int, int], value: float) -> None: ...
-
-	def __gt__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __ge__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __lt__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __le__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __eq__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def __ne__(self, other: Union[Raster, float]) -> Raster: ...
-
-	def acos(self) -> Raster: ...
-
-	def acosh(self) -> Raster: ...
-
-	def asin(self) -> Raster: ...
-
-	def asinh(self) -> Raster: ...
-
-	def atan(self) -> Raster: ...
-
-	def atan2(self, other: Union[Raster, float]) -> Raster: ...
-
-	def atanh(self) -> Raster: ...
-
-	def ceil(self) -> Raster: ...
-
-	def con(self, con_statement: str, true_raster_or_float: Union[Raster, float, str], false_raster_or_float: Union[Raster, float, str]) -> Raster: ...
-
-	def cos(self) -> Raster: ...
-
-	def cosh(self) -> Raster: ...
-
-	def exp(self) -> Raster: ...
-
-	def exp2(self) -> Raster: ...
-
-	def floor(self) -> Raster: ...
-
-	def is_nodata(self) -> Raster: ...
-
-	def ln(self) -> Raster: ...
-
-	def log2(self) -> Raster: ...
-
-	def log10(self) -> Raster: ...
-
-	def max(self, other: Union[Raster, float]) -> Raster: ...
-
-	def min(self, other: Union[Raster, float]) -> Raster: ...
-
-	def normalize(self) -> Raster: ...
-
-	def signum(self) -> Raster: ...
-
-	def sin(self) -> Raster: ...
-
-	def sinh(self) -> Raster: ...
-
-	def sqrt(self) -> Raster: ...
-
-	def square(self) -> Raster: ...
-
-	def tan(self) -> Raster: ...
-
-	def tanh(self) -> Raster: ...
-
-	def to_degrees(self) -> Raster: ...
-
-	def to_radians(self) -> Raster: ...
-
-	def trunc(self) -> Raster: ...
-
-	def num_cells(self) -> int: ...
-
-	def num_valid_cells(self) -> int: ...
-
-	def calculate_mean(self) -> float: ...
-
-	def calculate_mean_and_stdev(self) -> Tuple[float, float]: ...
-
-	def calculate_clip_values(self, percent: float) -> Tuple[float, float]: ...
-
-	def deep_copy(self) -> Raster: ...
-
-	def update_min_max(self) -> None: ...
-
-class VariableLengthRecord():
-	@property
-	def reserved(self) -> int: ...
-	
-	@property
-	def user_id(self) -> str: ...
-	
-	@property
-	def record_id(self) -> int: ...
-	
-	@property
-	def record_length_after_header(self) -> int: ...
-	
-	@property
-	def description(self) -> str: ...
-	
-	@property
-	def binary_data(self) -> List[int]: ...
-
-class VectorAttributes():
-	@property
-	def header(self) -> AttributeHeader: ...
-
-	@property
-	def fields(self) -> List[AttributeField]: ...
-
-	@property
-	def is_deleted(self) -> List[bool]: ...
-
-	def get_num_fields(self) -> int: ...
-
-class VectorGeometry():
-	@property
-	def shape_type(self) -> VectorGeometryType: ...
-
-	@property
-	def x_min(self) -> float: ...
-
-	@property
-	def x_max(self) -> float: ...
-
-	@property
-	def y_min(self) -> float: ...
-
-	@property
-	def y_max(self) -> float: ...
-
-	@property
-	def num_parts(self) -> int: ...
-
-	@property
-	def num_points(self) -> int: ...
-
-	@property
-	def parts(self) -> List[int]: ...
-
-	@property
-	def points(self) -> List[Point2D]: ...
-
-	@property
-	def z_min(self) -> float: ...
-
-	@property
-	def z_max(self) -> float: ...
-
-	@property
-	def z_array(self) -> List[float]: ...
-
-	@property
-	def m_min(self) -> float: ...
-
-	@property
-	def m_max(self) -> float: ...
-
-	@property
-	def m_array(self) -> List[float]: ...
-
-	@staticmethod
-	def new_vector_geometry(shape_type: VectorGeometryType) -> VectorGeometry: ...
-
-	def add_point(self, p: Point2D) -> None: ...
-
-	def add_pointm(self, p: Point2D, m: float) -> None: ...
-
-	def add_pointz(self, p: Point2D, m: float, z: float) -> None: ...
-
-	def add_geom_part(self, points: List[Point2D]) -> None: ...
-
-	def add_geom_partm(self, points: List[Point2D], measures: List[float]) -> None: ...
-
-	def add_geom_partz(self, points: List[Point2D], measures: List[float], z_values: List[float]) -> None: ...
-
-	def get_bounding_box(self) -> BoundingBox: ...
-
-	def get_length(self) -> int: ...
-
-	def has_m_data(self) -> bool: ...
-
-	def has_z_data(self) -> bool: ...
-
-	def is_hole(self, part_num: int) -> bool: ...
-
-class VectorGeometryType(Enum):
-	Null: int
-	Point: int
-	PolyLine: int
-	Polygon: int
-	MultiPoint: int
-	PointZ: int
-	PolyLineZ: int
-	PolygonZ: int
-	MultiPointZ: int
-	PointM: int
-	PolyLineM: int
-	PolygonM: int
-	MultiPointM: int
-
-class VectorHeader():
-	@property
-	def file_length(self) -> int: ...
-
-	@property
-	def version(self) -> int: ...
-
-	@property
-	def shape_type(self) -> VectorGeometryType: ...
-
-	@property
-	def x_min(self) -> float: ...
-
-	@property
-	def y_min(self) -> float: ...
-
-	@property
-	def x_max(self) -> float: ...
-
-	@property
-	def y_max(self) -> float: ...
-
-	@property
-	def z_min(self) -> float: ...
-
-	@property
-	def z_max(self) -> float: ...
-
-	@property
-	def m_min(self) -> float: ...
-
-	@property
-	def m_max(self) -> float: ...
-
-class Vector():
-	@property
-	def file_name(self) -> str: ...
-
-	@file_name.setter
-	def file_name(self, value: str) -> None: ...
-
-	@property
-	def file_mode(self) -> str: ...
-
-	@property
-	def header(self) -> VectorHeader: ...
-
-	@property
-	def num_records(self) -> int: ...
-
-	@property
-	def records(self) -> List[VectorGeometry]: ...
-
-	@property
-	def attributes(self) -> VectorAttributes: ...
-
-	@property
-	def projection(self) -> str: ...
-
-	def __getitem__(self, index: int) -> VectorGeometry: ...
-
-	def add_record(self, geometry: VectorGeometry) -> None: ...
-
-	def add_attribute_field(self, field: AttributeField) -> None: ...
-
-	def add_attribute_fields(self, fields: List[AttributeField]) -> None: ...
-
-	def add_attribute_record(self, rec: List[FieldData], deleted: bool) -> None: ...
-
-	def contains_attribute_field(self, field: AttributeField) -> bool: ...
-
-	def get_attribute_fields(self) -> List[AttributeField]: ...
-
-	def get_attribute_record(self, index: int) -> List[FieldData]: ...
-
-	def get_attribute_field_info(self, index: int) -> AttributeField: ...
-
-	def get_attribute_field_num(self, name: str) -> Optional[int]: ...
-
-	def get_num_attributes_fields(self) -> int: ...
-
-	def get_attribute_value(self, record_index: int, field_name: str) -> FieldData: ...
-
-	def is_attribute_field_numeric(self, index: int) -> bool: ...
-
-	def reinitialize_attributes(self) -> None: ...
-
-	def set_attribute_value(self, record_index: int, field_name: str, field_data: FieldData) -> None: ...
-
-class WaveformPacket():
-	@property
-	def packet_descriptor_index(self) -> int: ...
-
-	@packet_descriptor_index.setter
-	def packet_descriptor_index(self, value: int) -> None: ...
-
-	@property
-	def offset_to_waveform_data(self) -> int: ...
-
-	@offset_to_waveform_data.setter
-	def offset_to_waveform_data(self, value: int) -> None: ...
-
-	@property
-	def waveform_packet_size(self) -> int: ...
-
-	@waveform_packet_size.setter
-	def waveform_packet_size(self, value: int) -> None: ...
-
-	@property
-	def ret_point_waveform_loc(self) -> float: ...
-
-	@ret_point_waveform_loc.setter
-	def ret_point_waveform_loc(self, value: float) -> None: ...
-
-	@property
-	def xt(self) -> float: ...
-
-	@xt.setter
-	def xt(self, value: float) -> None: ...
-
-	@property
-	def yt(self) -> float: ...
-
-	@yt.setter
-	def yt(self, value: float) -> None: ...
-
-	@property
-	def zt(self) -> float: ...
-
-	@zt.setter
-	def zt(self, value: float) -> None: ...
-
-class WbEnvironment():
-    	
-	@property
-	def max_procs(self) -> int: ...
-
-	@max_procs.setter
-	def max_procs(self, value: int) -> None: ...
-
-	@property
-	def verbose(self) -> bool: ...
-
-	@verbose.setter
-	def verbose(self, value: bool) -> None: ...
-
-	@property
-	def working_directory(self) -> str: ...
-
-	@working_directory.setter
-	def working_directory(self, value: str) -> None: ...
-
-	def __new__(cls, user_id: str = "") -> WbEnvironment: ...
-
-	def version(self) -> str: ...
-
-	def read_lidar(self, file_name: str, file_mode: str = "r") -> Lidar: ...
-
-	def read_lidars(self, file_names: List[str]) -> List[Lidar]: ...
-
-	def new_lidar(self, header: LidarHeader) -> Lidar: ...
-
-	def write_lidar(self, lidar: Lidar, file_name: str) -> None: ...
-
-	def read_raster(self, file_name: str) -> Raster: ...
-
-	def read_rasters(self, file_name: List[str]) -> List[Raster]: ...
-
-	def new_raster(self, configs: RasterConfigs) -> Raster: ...
-
-	def write_raster(self, raster: Raster, file_name: str, compress: bool = False) -> None: ...
-
-	def read_vector(self, file_name: str) -> Vector: ...
-
-	def read_vectors(self, file_name: List[str]) -> List[Vector]: ...
-
-	def new_vector(self,  shape_type: VectorGeometryType, attributes: Optional[List[AttributeField]] = None, proj: str = "") -> Vector: ...
-
-	def write_vector(self, vector: Vector, file_name: str) -> None: ...
-
-	def write_text(self, text: str, file_name: str) -> None: ...
-
-	def accumulation_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def adaptive_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, threshold: float = 2.0) -> Raster: ...
-	
-	def add_point_coordinates_to_table(self, input: Vector) -> Vector: ...
-
-	def aggregate_raster(self, raster: Raster, aggregation_factor: int = 2, aggregation_type: str = "mean") -> Raster: ...
-
-	def anova(self, input_raster: Raster, features_raster: Raster, output_html_file: str) -> None: ...
-
-	def ascii_to_las(self, input_ascii_files: List[str], pattern: str, epsg_code: int) -> None: ...
-
-	def aspect(self, dem: Raster, z_factor: float = 1.0) -> Raster: ...
-
-	def assess_route(self, routes: Vector, dem: Raster, segment_length: float = 100.0, search_radius: int = 15) -> Vector: ...
-
-	def attribute_correlation(self, input: Vector, output_html_file: str) -> None: ...
-
-	def attribute_histogram(self, input: Vector, field_name: str, output_html_file: str) -> None: ...
-
-	def attribute_scattergram(self, input: Vector, field_name_x: str, field_name_y: str, output_html_file: str, add_trendline: bool = False) -> None: ...
-
-	def average_flowpath_slope(self, dem: Raster) -> Raster: ...
-
-	def average_horizon_distance(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
-
-	def average_normal_vector_angular_deviation(self, dem: Raster, filter_size: int = 11) -> Raster: ...
-
-	def average_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def average_upslope_flowpath_length(self, dem: Raster) -> Raster: ...
-
-	def balance_contrast_enhancement(self, image: Raster, band_mean: float = 100.0) -> Raster: ...
-
-	def basins(self, d8_pntr: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def bilateral_filter(self, raster: Raster, sigma_dist: float = 0.75, sigma_int: float = 1.0) -> Raster: ...
-
-	def block_maximum(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def block_minimum(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def bool_and(self, input1: Raster, input2: Raster) -> Raster: ...
-
-	def bool_not(self, input1: Raster, input2: Raster) -> Raster: ...
-
-	def bool_or(self, input1: Raster, input2: Raster) -> Raster: ...
-
-	def bool_xor(self, input1: Raster, input2: Raster) -> Raster: ...
-
-	def boundary_shape_complexity(self, raster: Raster) -> Raster: ...
-
-	def breach_depressions_least_cost(self, dem: Raster, max_cost: float = float('inf'), max_dist: int = 100, flat_increment: float = float('nan'), fill_deps: bool = False, minimize_dist: bool = False) -> Raster: ...
-
-	def breach_single_cell_pits(self, dem: Raster) -> Raster: ...
-
-	def breakline_mapping(self, dem: Raster, threshold: float = 0.8, min_length: int = 3) -> Vector: ...
-
-	def buffer_raster(self, input: Raster, buffer_size: float, grid_cells_units: bool = False) -> Raster: ...
-
-	def burn_streams_at_roads(self, dem: Raster, streams: Vector, roads: Vector, road_width: float) -> Raster: ...
-
-	def canny_edge_detection(self, input: Raster, sigma: float = 0.5, low_threshold: float = 0.05, high_threshold: float = 0.15, add_back_to_image: bool = False) -> Raster: ...
-
-	def centroid_raster(self, input: Raster) -> Tuple[Raster, str]: ...
-
-	def centroid_vector(self, input: Vector) -> Vector: ...
-
-	def change_vector_analysis(self, date1_rasters: List[Raster], date2_rasters: List[Raster]) -> Tuple[Raster, Raster, str]: ...
-
-	def check_in_license(self, key: str) -> str: ...
-
-	def circular_variance_of_aspect(self, dem: Raster, filter_size: int = 11) -> Raster: ...
-
-	def classify_buildings_in_lidar(self, in_lidar: Lidar, building_footprints: Vector) -> Lidar: ...
-
-	def classify_lidar(self, input_lidar: Optional[Lidar], search_radius: float = 2.5, grd_threshold: float = 0.1, oto_threshold: float = 1.0, linearity_threshold: float = 0.5, planarity_threshold: float = 0.85, num_iter: int = 30, facade_threshold: float = 0.5) -> Optional[Lidar]: ...
-
-	def colourize_based_on_class(self, input_lidar: Optional[Lidar], intensity_blending_amount: float = 50.0, clr_str: str = "", use_unique_clrs_for_buildings: bool = False, search_radius: float = 2.0) -> Optional[Lidar]: ...
-
-	def colourize_based_on_point_returns(self, input_lidar: Optional[Lidar], intensity_blending_amount: float = 50.0, only_ret_colour: str = "(230,214,170)", first_ret_colour:str = "(0,140,0)", intermediate_ret_colour: str = "(255,0,255)", last_ret_colour: str = "(0,0,255)") -> Optional[Lidar]: ...
-	
-	def classify_overlap_points(self, in_lidar: Lidar, resolution: float = 1.0, overlap_criterion: str = "max scan angle", filter: bool = False) -> Lidar: ...
-
-	def clean_vector(self, input: Vector) -> Vector: ...
-
-	def clip(self, input: Vector, clip_layer: Vector) -> Vector: ...
-
-	def clip_lidar_to_polygon(self, input: Lidar, polygons: Vector) -> Lidar: ...
-
-	def clip_raster_to_polygon(self, raster: Raster, polygons: Vector, maintain_dimensions: bool = False) -> Raster: ...
-
-	def closing(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def clump(self, raster: Raster, diag: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def compactness_ratio(self, input: Vector) -> Vector: ...
-
-	def conservative_smoothing_filter(self, raster: Raster, filter_size_x: int = 3, filter_size_y: int = 3) -> Raster: ...
-
-	def construct_vector_tin(self, input_points: Vector, field_name: str = "FID", use_z: bool = False, max_triangle_edge_length: float = float('inf')) -> Vector: ...
-
-	def contours_from_points(self, input: Vector, field_name: str = "", use_z_values: bool = False, max_triangle_edge_length: float = float('inf'), contour_interval: float = 10.0, base_contour: float = 0.0, smoothing_filter_size: int = 9) -> Vector: ...
-
-	def contours_from_raster(self, raster_surface: Raster, contour_interval: float = 10.0, base_contour: float = 0.0, smoothing_filter_size: int = 9, deflection_tolerance: float = 10.0) -> Vector: ...
-
-	def convert_nodata_to_zero(self, raster: Raster) -> Raster: ...
-
-	def corner_detection(self, raster: Raster) -> Raster: ...
-
-	def correct_vignetting(self, image: Raster, principal_point: Vector, focal_length: float = 304.8, image_width: float = 228.6, n_param: float = 4.0) -> Raster: ...
-
-	def cost_allocation(self, source: Raster, backlink: Raster) -> Raster: ...
-
-	def cost_distance(self, source: Raster, cost: Raster) -> Tuple[Raster, Raster]: ...
-
-	def cost_pathway(self, destination: Raster, backlink: Raster, zero_background: bool = False) -> Raster: ...
-
-	def count_if(self, input_rasters: List[Raster], comparison_value: float) -> Raster: ...
-
-	def create_colour_composite(self, red: Raster, green: Raster, blue: Raster, opacity: Optional[Raster] = None, enhance: bool = True, treat_zeros_as_nodata: bool = False) -> Raster: ...
-
-	def create_plane(self, base_file: Raster, gradient: float, aspect: float, constant: float) -> Raster: ...
-
-	def crispness_index(self, raster: Raster, output_html_file: str) -> None: ...
-
-	def cross_tabulation(self, raster1: Raster, raster2: Raster, output_html_file: str) -> None: ...
-
-	def csv_points_to_vector(self, input_file: str, x_field_num: int = 0, y_field_num: int = 1, epsg: int = 0) -> Vector: ...
-
-	def cumulative_distribution(self, raster: Raster) -> Raster: ...
-
-	def curvedness(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def d8_flow_accum(self, raster: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False, esri_pntr: bool = False) -> Raster: ...
-
-	def d8_mass_flux(self, dem: Raster, loading: Raster, efficiency: Raster, absorption: Raster) -> Raster: ...
-
-	def d8_pointer(self, dem: Raster, esri_pointer: bool = False) -> Raster: ...
-
-	def dbscan(self, input_rasters: List[Raster], scaling_method: str = "none", search_distance: float = 1.0, min_points: int = 5) -> Raster: ...
-
-	def dem_void_filling(self, dem: Raster, fill: Raster, mean_plane_dist: int = 20, edge_treatment: str = "use DEM", weight_value: float = 2.0) -> Raster: ...
-	
-	def depth_in_sink(self, dem: Raster, zero_background: bool = False) -> Raster: ...
-
-	def depth_to_water(self, dem: Raster, streams: Optional[Vector] = None, lakes: Optional[Vector] = None) -> Raster: ...
-
-	def deviation_from_mean_elevation(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def deviation_from_regional_direction(self, input: Vector, elongation_threshold: float = 0.75) -> Vector: ...
-
-	def diff_of_gaussians_filter(self, raster: Raster, sigma1: float = 2.0, sigma2: float = 4.0) -> Raster: ...
-
-	def difference(self, input: Vector, overlay: Vector) -> Vector: ...
-
-	def difference_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def difference_from_mean_elevation(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def dinf_flow_accum(self, dem: Raster, out_type: str = "SCA", convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False) -> Raster: ...
-
-	def dinf_mass_flux(self, dem: Raster, loading: Raster, efficiency: Raster, absorption: Raster) -> Raster: ...
-
-	def dinf_pointer(self, dem: Raster) -> Raster: ...
-
-	def direct_decorrelation_stretch(self, image: Raster, achromatic_factor: float = 0.5, clip_percent: float = 1.0) -> Raster: ...
-
-	def directional_relief(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf')) -> Raster: ...
-
-	def dissolve(self, input: Vector, dissolve_field: str = "", snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
-
-	def distance_to_outlet(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def diversity_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def downslope_distance_to_stream(self, dem: Raster, streams: Raster, use_dinf: bool = False) -> Raster: ...
-
-	def downslope_flowpath_length(self, d8_pointer: Raster, watersheds: Raster, weights: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def downslope_index(self, dem: Raster, vertical_drop: float, output_type: str = "tangent") -> Raster: ...
-
-	def edge_contamination(self, dem: Raster, flow_type: str = "mfd", z_factor: float = -1.0) -> Raster: ...
-
-	def edge_density(self, dem: Raster, filter_size: int = 11, normal_diff_threshold: float = 5.0, z_factor: float = 1.0) -> Raster: ...
-
-	def edge_preserving_mean_filter(self, raster: Raster, filter_size: int = 11, threshold: float = 15.0) -> Raster: ...
-
-	def edge_proportion(self, raster: Raster) -> Tuple[Raster, str]: ...
-
-	def elev_relative_to_min_max(self, dem: Raster) -> Raster: ...
-
-	def elev_relative_to_watershed_min_max(self, dem: Raster, watersheds: Raster) -> Raster: ...
-
-	def elevation_above_pit(self, dem: Raster) -> Raster: ...
-
-	def elevation_above_stream(self, dem: Raster, streams: Raster) -> Raster: ...
-
-	def elevation_above_stream_euclidean(self, dem: Raster, streams: Raster) -> Raster: ...
-
-	def elevation_percentile(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
-
-	def eliminate_coincident_points(self, input: Vector, tolerance_dist: float) -> Vector: ...
-
-	def elongation_ratio(self, input: Vector) -> Vector: ...
-
-	def embankment_mapping(self, dem: Raster, roads_vector: Vector, search_dist: float = 2.5, min_road_width: float = 6.0, typical_embankment_width: float = 30.0, typical_embankment_max_height: float = 2.0, embankment_max_width: float = 60.0, max_upwards_increment: float = 0.05, spillout_slope: float = 4.0, remove_embankments: bool = False) -> Tuple[Raster, Optional[Raster]]: ...
-
-	def emboss_filter(self, raster: Raster, direction: str = "n", clip_amount: float = 0.0) -> Raster: ...
-
-	def erase(self, input: Vector, erase_layer: Vector) -> Vector: ...
-
-	def erase_polygon_from_lidar(self, input: Lidar, polygons: Vector) -> Lidar: ...
-
-	def erase_polygon_from_raster(self, raster: Raster, polygons: Vector) -> Raster: ...
-
-	def euclidean_allocation(self, input: Raster) -> Raster: ...
-
-	def euclidean_distance(self, input: Raster) -> Raster: ...
-
-	def evaluate_training_sites(self, input_rasters: List[Raster], training_polygons: Vector, class_field_name: str, output_html_file: str) -> None: ...
-
-	def export_table_to_csv(self, input: Vector, output_csv_file: str, headers: bool = True) -> None: ...
-
-	def exposure_towards_wind_flux(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf'), z_factor: float = 1.0) -> Raster: ...
-
-	def extend_vector_lines(self, input: Vector, distance: float, extend_direction: str = "both ends") -> Vector: ...
-
-	def extract_by_attribute(self, input: Vector, statement: str) -> Vector: ...
-
-	def extract_nodes(self, input: Vector) -> Vector: ...
-
-	def extract_raster_values_at_points(self, rasters: List[Raster], points: Vector) -> Tuple[Vector, str]: ...
-
-	def extract_streams(self, flow_accumulation: Raster, threshold: float = 0.0, zero_background: bool = False) -> Raster: ...
-
-	def extract_valleys(self, dem: Raster, variant: str = "LQ", line_thin: bool = False, filter_size: int = 5) -> Raster: ...
-
-	def farthest_channel_head(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def fast_almost_gaussian_filter(self, raster: Raster, sigma: float = 1.8) -> Raster: ...
-
-	def fd8_flow_accum(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
-
-	def fd8_pointer(self, dem: Raster) -> Raster: ...
-
-	def feature_preserving_smoothing(self, dem: Raster, filter_size: int = 11, normal_diff_threshold: float = 8.0, iterations: int = 3, max_elevation_diff: float = float('inf'), z_factor: float = 1.0) -> Raster: ...
-
-	def fetch_analysis(self, dem: Raster, azimuth: float = 0.0, height_increment: float = 0.05) -> Raster: ...
-
-	def fill_burn(self, dem: Raster, streams: Vector) -> Raster: ...
-
-	def fill_depressions(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan'), max_depth: float = float('inf')) -> Raster: ...
-
-	def fill_depressions_planchon_and_darboux(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan')) -> Raster: ...
-
-	def fill_depressions_wang_and_liu(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan')) -> Raster: ...
-
-	def fill_missing_data(self, dem: Raster, filter_size: int = 11, weight: float = 2.0, exclude_edge_nodata: bool = False) -> Raster: ...
-
-	def fill_pits(self, dem: Raster) -> Raster: ...
-
-	def filter_lidar(self, statement: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
-
-	def filter_lidar_classes(self, input: Lidar, exclusion_classes: List[int]) -> Lidar: ...
-
-	def filter_lidar_scan_angles(self, in_lidar: Lidar, threshold: int) -> Lidar: ...
-
-	def filter_raster_features_by_area(self, input: Raster, threshold: int, zero_background: bool = False) -> Raster: ...
-
-	def find_flightline_edge_points(self, in_lidar: Lidar) -> Lidar: ...
-
-	def find_lowest_or_highest_points(self, raster: Raster, output_type: str = "lowest") -> Vector: ...
-
-	def find_main_stem(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def find_noflow_cells(self, dem: Raster) -> Raster: ...
-
-	def find_parallel_flow(self, d8_pntr: Raster, streams: Raster) -> Raster: ...
-
-	def find_patch_edge_cells(self, raster: Raster) -> Raster: ...
-
-	def find_ridges(self, dem: Raster, line_thin: bool = True) -> Raster: ...
-
-	def fix_dangling_arcs(self, input: Vector, snap_dist: float) -> Vector: ...
-
-	def flatten_lakes(self, dem: Raster, lakes: Vector) -> Raster: ...
-
-	def flightline_overlap(self, input_lidar: Lidar, resolution: float = 1.0) -> Raster: ...
-
-	def flip_image(self, raster: Raster, direction: str = "vertical") -> Raster: ...
-
-	def flood_order(self, dem: Raster) -> Raster: ...
-
-	def flow_accum_full_workflow(self, dem: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, esri_pntr: bool = False) -> Tuple[Raster, Raster, Raster]: ...
-
-	def flow_length_diff(self, d8_pointer: Raster, esri_pointer: bool = False, log_transform: bool = False) -> Raster: ...
-
-	def gamma_correction(self, raster: Raster, gamma_value: float = 0.5) -> Raster: ...
-
-	def gaussian_contrast_stretch(self, raster: Raster, num_tones: int = 256) -> Raster: ...
-
-	def gaussian_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def gaussian_filter(self, raster: Raster, sigma: float = 0.75) -> Raster: ...
-
-	def geomorphons(self, dem: Raster, search_distance: int = 50, flatness_threshold: float = 0.0, flatness_distance: int = 0, skip_distance: int = 0, output_forms: bool = True, analyze_residuals: bool = False) -> Raster: ...
-
-	def generalize_classified_raster(self, raster: Raster, area_threshold: int = 5, method: str = "longest") -> Raster: ...
-
-	def generalize_with_similarity(self, raster: Raster, similarity_rasters: List[Raster], area_threshold: int = 5) -> Raster: ...
-
-	def generating_function(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def hack_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def heat_map(self, points: Vector, field_name: Optional[str] = None, bandwidth: float = 0.0, cell_size: float = 0.0, base_raster: Optional[Raster] = None, kernel_function: str = "quartic") -> Raster: ...
-
-	def height_above_ground(self, input: Lidar) -> Lidar: ...
-
-	def hexagonal_grid_from_raster_base(self, base: Raster, width: float, orientation: str = "h") -> Vector: ...
-
-	def hexagonal_grid_from_vector_base(self, base: Vector, width: float, orientation: str = "h") -> Vector: ...
-
-	def high_pass_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def high_pass_median_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
-
-	def highest_position(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def hillshade(self, dem: Raster, azimuth: float = 315.0, altitude: float = 30.0, z_factor: float = 1.0) -> Raster: ...
-
-	def hillslopes(self, d8_pntr: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def histogram_equalization(self, raster: Raster, num_tones: int = 256) -> Raster: ...
-
-	def histogram_matching(self, image: Raster, histogram: List[List[float]], histo_is_cumulative: bool = False) -> Raster: ...
-
-	def histogram_matching_two_images(self, image1: Raster, image2: Raster) -> Raster: ...
-
-	def hole_proportion(self, input: Vector) -> Vector: ...
-
-	def horizon_angle(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf')) -> Raster: ...
-
-	def horizon_area(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
-
-	def horizontal_excess_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]: ...
-
-	def horton_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def hydrologic_connectivity(self, dem: Raster, exponent: float = 1.1, convergence_threshold: float = 0.0, z_factor: float = 1.0 ) -> Tuple[Raster, Raster]: ...
-
-	def hypsometric_analysis(self, dem_rasters: List[Raster], output_html_file: str, watershed_rasters: Optional[List[Raster]] = None) -> None: ...
-
-	def hypsometrically_tinted_hillshade(self, dem: Raster, solar_altitude: float = 45.0, hillshade_weight: float = 0.5, brightness: float = 0.5, atmospheric_effects: float = 0.0, palette: WbPalette = WbPalette.Atlas, reverse_palette: bool = False, full_360_mode: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def idw_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, weight: float = 2.0, radius: float = 0.0, min_points: int = 0, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def ihs_to_rgb(self, intensity: Raster, hue: Raster, saturation: Raster) -> Tuple[Raster, Raster, Raster]: ...
-
-	def image_autocorrelation(self, rasters: List[Raster], output_html_file: str, contiguity_type: str = "bishop") -> None: ...
-
-	def image_correlation(self, rasters: List[Raster], output_html_file: str) -> None: ...
-
-	def image_correlation_neighbourhood_analysis(self, raster1: Raster, raster2: Raster, filter_size: int = 11, correlation_stat: str = "pearson") -> Tuple[Raster, Raster]: ...
-
-	def image_regression(self, independent_variable: Raster, dependent_variable: Raster, output_html_file: str, standardize_residuals: bool = False, output_scattergram: bool = False, num_samples: int = 1000) -> Raster: ...
-
-	def image_segmentation(self, input_rasters: List[Raster], dist_threshold: float = 0.5, num_steps: int = 10, area_threshold: int = 4) -> Raster: ...
-
-	def image_slider(self, left_raster: Raster, right_raster: Raster, output_html_file: str, left_palette: WbPalette = WbPalette.Grey, left_reverse_palette: bool = False, left_label: str = "",  right_palette: WbPalette = WbPalette.Grey, right_reverse_palette: bool = False, right_label: str = "", image_height: int = 600) -> None: ...
-
-	def image_stack_profile(self, images: List[Raster], points: Vector, output_html_file: str) -> None: ...
-
-	def impoundment_size_index(self, dem: Raster, max_dam_length: float, output_mean: bool = False, output_max: bool = False, output_volume: bool = False, output_area: bool = False, output_height: bool = False) -> Tuple[Optional[Raster], Optional[Raster], Optional[Raster], Optional[Raster], Optional[Raster]]: ...
-
-	def individual_tree_detection(self, input_lidar: Optional[Lidar],  min_search_radius: float = 1.0, min_height: float = 0.0, max_search_radius: Optional[float] = None, max_height: Optional[float] = None, only_use_veg: bool = False) -> Optional[Vector]: ...
-
-	def insert_dams(self, dem: Raster, dam_points: Vector, dam_length: float) -> Raster: ...
-
-	def isobasins(self, dem: Raster, target_size: float, connections: bool = False, csv_file: str = "" ) -> Raster: ...
-
-	def integral_image_transform(self, raster: Raster) -> Raster: ...
-
-	def intersect(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
-
-	def inverse_pca(self, rasters: List[Raster], pca_report_file: str) -> List[Raster]: ...
-
-	def jenson_snap_pour_points(self, pour_pts: Vector, streams: Raster, snap_dist: float = 0.0) -> Vector: ...
-
-	def join_tables(self, primary_vector: Vector, primary_key_field: str, foreign_vector: Vector, foreign_key_field: str, import_field: str = "") -> None: ...
-
-	def k_means_clustering(self, input_rasters: List[Raster], output_html_file: str = "", num_clusters: int = 5, max_iterations: int = 10, percent_changed_threshold: float = 2.0, initialization_mode: str = "diagonal", min_class_size: int = 10) -> Raster: ...
-
-	def k_nearest_mean_filter(self, raster: Raster, filter_size_x: int = 3, filter_size_y: int = 3, k: int = 5) -> Raster: ...
-
-	def kappa_index(self, class_raster: Raster, reference_raster: Raster, output_html_file: str = "") -> None: ...
-
-	def knn_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", k: int = 5, test_proportion: float = 0.2, use_clipping: bool = False, create_output: bool = False) -> Optional[Raster]: ...
-
-	def knn_regression(self, input_rasters: List[Raster], training_data: Vector, field_name: str, scaling_method: str = "none", k: int = 5, distance_weighting: bool = False, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
-
-	def ks_normality_test(self, raster: Raster, output_html_file: str, num_samples: int) -> None: ...
-
-	def laplacian_filter(self, raster: Raster, variant: str = "3x3(1)", clip_amount: float = 0.0) -> Raster: ...
-
-	def laplacian_of_gaussians_filter(self, raster: Raster, sigma: float = 0.75) -> Raster: ...
-
-	def las_to_ascii(self, input_lidar: Optional[Lidar]) -> None: ...
-
-	def las_to_shapefile(self, input_lidar: Optional[Lidar], output_multipoint: bool = False) -> Vector: ...
-
-	def layer_footprint_raster(self, input: Raster) -> Vector: ...
-
-	def layer_footprint_vector(self, input: Vector) -> Vector: ...
-
-	def lee_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sigma: float = 10.0, m_value: float = 5.0) -> Raster: ...
-
-	def length_of_upstream_channels(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def license_type(self) -> LicenseType: ...
-
-	def lidar_block_maximum(self, input_lidar: Optional[Lidar], cell_size: float = 1.0) -> Raster: ...
-
-	def lidar_block_minimum(self, input_lidar: Optional[Lidar], cell_size: float = 1.0) -> Raster: ...
-
-	def lidar_classify_subset(self, base_lidar: Lidar, subset_lidar: Lidar, subset_class_value: int, nonsubset_class_value: int) -> Lidar: ...
-
-	def lidar_colourize(self, in_lidar: Lidar, in_image: Raster) -> Lidar: ...
-
-	def lidar_construct_vector_tin(self, input_lidar: Optional[Lidar], returns_included: str = "all", excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Vector: ...
-
-	def lidar_contour(self, input_lidar: Optional[Lidar], contour_interval: float = 10.0, base_contour: float = 0.0, smooth: int = 5, interpolation_parameter: str = "elevation", returns_included: str = "all",  excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), tile_overlap: float = 0.0, max_triangle_edge_length: float = float('inf')) -> Optional[Vector]: ...
-
-	def lidar_digital_surface_model(self, input_lidar: Optional[Lidar], cell_size: float = 1.0, search_radius: float = 0.5, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Raster: ...
-
-	def lidar_eigenvalue_features(self, input_lidar: Optional[Lidar], num_neighbours: Optional[int], search_radius: Optional[float]) -> None: ...
-
-	def lidar_elevation_slice(self, input: Lidar, minz: float = float('-inf'), maxz: float = float('inf'), classify: bool = False, in_class_value: int = 2, out_class_value: int = 1) -> Lidar: ...
-
-	def lidar_ground_point_filter(self, input_lidar: Optional[Lidar], search_radius: float = 2.0, min_neighbours: int = 0, slope_threshold: float = 45.0, height_threshold: float = 1.0, classify: bool = False, slope_norm: bool = True, height_above_ground: bool = False) -> Lidar: ...
-
-	def lidar_hex_bin(self, input_lidar: Lidar, width: float, orientation: str = "h") -> Vector: ...
-
-	def lidar_hillshade(self, input: Lidar, search_radius: float = -1.0, azimuth: float = 315.0, altitude: float = 30.0) -> Lidar: ...
-
-	def lidar_histogram(self, input_lidar: Lidar, output_html_file: str, parameter: str = "elevation", clip_percent: float = 1.0) -> None: ...
-
-	def lidar_idw_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation",  returns_included: str = "all", cell_size: float = 1.0,  idw_weight: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
-
-	def lidar_info(self, input_lidar: Lidar, output_html_file: Optional[str], show_point_density: bool = True, show_vlrs: bool = True, show_geokeys: bool = True) -> str: ...
-
-	def lidar_join(self, inputs: List[Lidar]) -> Lidar: ...
-
-	def lidar_kappa(self, input_lidar1: Lidar, input_lidar2: Lidar, output_html_file: str, cell_size: float = 1.0, output_class_accuracy: bool = False) -> Raster: ...
-
-	def lidar_nearest_neighbour_gridding(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
-
-	def lidar_point_density(self, input_lidar: Optional[Lidar], returns_included: str = "all", cell_size: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
-
-	def lidar_point_return_analysis(self, input: Lidar, create_output: bool = False) -> Optional[Lidar]: ...
-
-	def lidar_point_stats(self, input_lidar: Optional[Lidar], cell_size: float = 1.0, num_points: bool = False, num_pulses: bool = False, avg_points_per_pulse: bool = False, z_range: bool = False, intensity_range: bool = False, predominant_class: bool = False) : ...
-
-	def lidar_radial_basis_function_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, num_points: int = 15, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), func_type: str = "ThinPlateSpline", poly_order: str = "none", weight: float = 0.1) -> Raster: ...
-
-	def lidar_ransac_planes(self, in_lidar: Lidar, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, classify: bool = False, only_last_returns: bool = False) -> Lidar: ...
-
-	def lidar_remove_outliers(self, input: Lidar, search_radius: float = 2.0, elev_diff: float = 50.0, use_median: bool = False, classify: bool = False) -> Lidar: ...
-
-	def lidar_rooftop_analysis(self, lidar_inputs: List[Lidar], building_footprints: Vector, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, norm_diff_threshold: float = 2.0, azimuth: float = 180.0, altitude: float = 30.0) -> Vector: ...
-
-	def lidar_segmentation(self, in_lidar: Lidar, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, norm_diff_threshold: float = 2.0, max_z_diff: float = 1.0, classes: bool = False, ground: bool = False) -> Lidar: ...
-
-	def lidar_segmentation_based_filter(self, in_lidar: Lidar, search_radius: float = 5.0, norm_diff_threshold: float = 2.0, max_z_diff: float = 1.0, classify_points: bool = False) -> Lidar: ...
-
-	def lidar_shift(self, input: Lidar, x_shift: float = 0.0, y_shift: float = 0.0, z_shift: float = 0.0) -> Lidar: ...
-
-	def lidar_sibson_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", resolution: float = 1.0, returns_included: str = "all", excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Optional[Raster]: ...
-
-	def lidar_thin(self, input: Lidar, resolution: float = 1.0, selection_method: str = "first", save_filtered: bool = False) -> Tuple[Lidar, Optional[Lidar]]: ...
-
-	def lidar_thin_high_density(self, input: Lidar, density: float, resolution: float = 1.0, save_filtered: bool = False) -> Tuple[Lidar, Optional[Lidar]]: ...
-
-	def lidar_tile(self, input_lidar: Lidar, tile_width: float = 1000.0, tile_height: float = 1000.0, origin_x: float = 0.0, origin_y: float = 0.0, min_points_in_tile: int = 2, output_laz_format: bool = True) -> None: ...
-
-	def lidar_tile_footprint(self, input_lidar: Optional[Lidar], output_hulls: bool = False) -> Vector: ...
-
-	def lidar_tin_gridding(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Raster: ...
-
-	def lidar_tophat_transform(self, input: Lidar, search_radius: float) -> Lidar: ...
-
-	def line_detection_filter(self, raster: Raster, variant: str = "vertical", abs_values: bool = False, clip_tails: float = 0.0) -> Raster: ...
-
-	def line_intersections(self, input1: Vector, input2: Vector) -> Vector: ...
-
-	def line_thinning(self, raster: Raster) -> Raster: ...
-
-	def linearity_index(self, input: Vector) -> Vector: ...
-
-	def lines_to_polygons(self, input: Vector) -> Vector: ...
-
-	def list_unique_values(self, input: Vector, field_name: str) -> List[Tuple[str, int]]: ...
-
-	def list_unique_values_raster(self, raster: Raster) -> str: ...
-
-	def local_hypsometric_analysis(self, dem: Raster, min_scale: int = 4, step_size: int = 1,  num_steps: int = 10, step_nonlinearity: float = 1.0) -> Tuple[Raster, Raster]: ...
-
-	def logistic_regression(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
-
-	def long_profile(self, d8_pointer: Raster, streams_raster: Raster, dem: Raster, output_html_file: str, esri_pointer: bool = False) -> None: ...
-
-	def long_profile_from_points(self, d8_pointer: Raster, points: Vector, dem: Raster, output_html_file: str, esri_pointer: bool = False) -> None: ...
-
-	def longest_flowpath(self, dem: Raster, basins: Raster) -> Vector: ...
-
-	def lowest_position(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def low_points_on_headwater_divides(self, dem: Raster, streams: Raster) -> Vector: ...
-
-	def majority_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def map_off_terrain_objects(self, dem: Raster, max_slope: float = float('inf'), min_feature_size: int = 0) -> Raster: ...
-
-	def max_absolute_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def max_anisotropy_dev(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
-
-	def max_anisotropy_dev_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
-
-	def max_branch_length(self, dem: Raster, log_transform: bool = False) -> Raster: ...
-
-	def max_difference_from_mean(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
-
-	def max_downslope_elev_change(self, raster: Raster) -> Raster: ...
-
-	def max_elevation_dev_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
-
-	def max_elevation_deviation(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
-
-	def max_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def max_upslope_elev_change(self, raster: Raster) -> Raster: ...
-
-	def max_upslope_flowpath_length(self, dem: Raster) -> Raster: ...
-
-	def max_upslope_value(self, dem: Raster, values_raster: Raster) -> Raster: ...
-
-	def maximal_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def maximum_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def mdinf_flow_accum(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
-
-	def mean_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def mean_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def median_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
-
-	def medoid(self, input: Vector) -> Vector: ...
-
-	def merge_line_segments(self, input: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
-
-	def merge_table_with_csv(self, primary_vector: Vector, primary_key_field: str, foreign_csv_filename: str, foreign_key_field: str, import_field: str = "") -> None: ...
-
-	def merge_vectors(self, input_vectors: List[Vector]) -> Vector: ...
-
-	def min_absolute_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def min_dist_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, dist_threshold: float = float('inf')) -> Raster: ...
-
-	def min_downslope_elev_change(self, raster: Raster) -> Raster: ...
-
-	def min_max_contrast_stretch(self, raster: Raster, min_val: float, max_val: float, num_tones: int = 256) -> Raster: ...
-
-	def min_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def minimal_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def minimum_bounding_box(self, input: Vector, min_criteria: str = "area", individual_feature_hulls: bool = True) -> Vector: ...
-
-	def minimum_bounding_circle(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
-
-	def minimum_bounding_envelope(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
-
-	def minimum_convex_hull(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
-
-	def minimum_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def modified_k_means_clustering(self, input_rasters: List[Raster], output_html_file: str = "", num_start_clusters: int = 1000, merge_distance: float = 1.0, max_iterations: int = 10, percent_changed_threshold: float = 2.0) -> Raster: ...
-
-	def modify_lidar(self, statement: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
-
-	def modify_nodata_value(self, input: Raster, new_value: float = -32768.0) : ...
-
-	def mosaic(self, images: List[Raster], resampling_method: str = "cc") -> Raster: ...
-
-	def mosaic_with_feathering(self, image1: Raster, image2: Raster, resampling_method: str = "cc", distance_weight: float = 4.0) -> Raster: ...
-
-	def multidirectional_hillshade(self, dem: Raster, altitude: float = 30.0, z_factor: float = 1.0, full_360_mode: bool = False) -> Raster: ...
-
-	def multipart_to_singlepart(self, input: Vector, exclude_holes: bool = False) -> Vector: ...
-
-	def multiply_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def multiscale_curvatures(self, dem: Raster, curv_type: str = 'profile', min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0, log_transform: bool = True, standardize: bool = False) -> Tuple[Raster, Raster]: ...
-
-	def multiscale_elevation_percentile(self, dem: Raster, num_significant_digits: int = 3, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0) -> Tuple[Raster, Raster]: ...
-
-	def multiscale_roughness(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
-
-	def multiscale_roughness_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
-
-	def multiscale_std_dev_normals(self, dem: Raster, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0, html_signature_file: str = "") -> Tuple[Raster, Raster]: ...
-
-	def multiscale_std_dev_normals_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0) -> None: ...
-
-	def multiscale_topographic_position_image(self, local: Raster, meso: Raster, broad: Raster, hillshade: Optional[Raster] = None, lightness: float = 1.2) -> Raster: ...
-
-	def narrowness_index(self, raster: Raster) -> Raster: ...
-
-	def natural_neighbour_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, clip_to_hull: bool = True) -> Raster: ...
-
-	def nearest_neighbour_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, max_dist: float = float('inf')) -> Raster: ...
-
-	def new_raster_from_base_raster(self, base: Raster, out_val: float = float('nan'), data_type: str = "float") -> Raster: ...
-
-	def new_raster_from_base_vector(self, base: Vector, cell_size: float, out_val: float = float('nan'), data_type: str = "float") -> Raster: ...
-
-	def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster: ...
-
-	def normal_vectors(self, input: Lidar, search_radius: float = -1.0) -> Lidar: ...
-
-	def normalized_difference_index(self, nir_image: Raster, red_image: Raster, clip_percent: float = 0.0, correction_value: float = 0.0) -> Raster: ...
-
-	def normalize_lidar(self, input_lidar: Lidar, dtm: Raster) -> Lidar: ...
-
-	def num_downslope_neighbours(self, dem: Raster) -> Raster: ...
-
-	def num_inflowing_neighbours(self, dem: Raster) -> Raster: ...
-
-	def olympic_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def opening(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def openness(self, dem: Raster, dist: int = 20) -> Tuple[Raster, Raster]: ...
-
-	def otsu_thresholding(self, raster: Raster) -> Raster: ...
-
-	def paired_sample_t_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
-
-	def panchromatic_sharpening(self, pan: Raster, colour_composite: Raster, red: Raster, green: Raster, blue: Raster, fusion_method: str = "brovey") -> Raster: ...
-
-	def parallelepiped_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str) -> Raster: ...
-
-	def patch_orientation(self, input: Vector) -> Vector: ...
-
-	def pennock_landform_classification(self, dem: Raster, slope_threshold: float = 3.0, prof_curv_threshold: float = 0.1, plan_curv_threshold: float = 0.0, z_factor: float = 1.0) -> Tuple[Raster, str]: ...
-
-	def percent_elev_range(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def percent_equal_to(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
-
-	def percent_greater_than(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
-
-	def percent_less_than(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
-
-	def percentage_contrast_stretch(self, raster: Raster, clip: float = 1.0, tail: str = "both", num_tones: int = 256) -> Raster: ...
-
-	def percentile_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
-
-	def perimeter_area_ratio(self, input: Vector) -> Vector: ...
-
-	def pick_from_list(self, input_rasters: List[Raster], pos_input: Raster) -> Raster: ...
-
-	def piecewise_contrast_stretch(self, raster: Raster, transformation_statement: str, num_greytones: float = 1024.0) -> Raster: ...
-
-	def phi_coefficient(self, raster1: Raster, raster2: Raster, output_html_file: str) -> None: ...
-
-	def plan_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def polygon_area(self, input: Vector) -> Vector: ...
-
-	def polygon_long_axis(self, input: Vector) -> Vector: ...
-
-	def polygon_perimeter(self, input: Vector) -> Vector: ...
-
-	def polygon_short_axis(self, input: Vector) -> Vector: ...
-
-	def polygonize(self, input_layers: List[Vector]) -> Vector: ...
-
-	def polygons_to_lines(self, input: Vector) -> Vector: ...
-
-	def prewitt_filter(self, raster: Raster, clip_tails: float = 0.0) -> Raster: ...
-
-	def principal_component_analysis(self, rasters: List[Raster], output_html_file: str, num_components: int = 2, standardized: bool = False) -> List[Raster]: ...
-
-	def print_geotiff_tags(self, file_name: str) : ...
-
-	def profile(self, lines_vector: Vector, surface: Raster, output_html_file: str) -> None: ...
-
-	def profile_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def prune_vector_streams(self, streams: Vector, dem: Raster, threshold: float, snap_distance: float = 0.001) -> Vector: ...
-
-	def qin_flow_accumulation(self, dem: Raster, out_type: str = "SCA", exponent: float = 10.0, max_slope: float = 45.0, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
-
-	def quantiles(self, raster: Raster, num_quantiles: int = 5) -> Raster: ...
-
-	def quinn_flow_accumulation(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
-
-	def radial_basis_function_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, radius: float = 0.0, min_points: int = 0, cell_size: float = 0.0, base_raster: Optional[Raster] = None, func_type: str = "ThinPlateSpline", poly_order: str = "none", weight: float = 0.1) -> Raster: ...
-
-	def radius_of_gyration(self, raster: Raster) -> Tuple[Raster, str]: ...
-
-	def raise_walls(self, dem: Raster, walls: Vector, breach_lines: Vector, wall_height: float = 100.0) -> Raster: ...
-
-	def random_field(self, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def random_forest_classification_fit(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, split_criterion: str = "Gini", n_trees: int = 200,  min_samples_leaf: int = 1, min_samples_split: int = 2, test_proportion: float = 0.2) -> List[int]: ...
-
-	def random_forest_classification_predict(self, input_rasters: List[Raster], model_bytes: List[int]) -> Raster: ...
-
-	def random_forest_regression_fit(self, input_rasters: List[Raster], training_data: Vector, field_name: str, n_trees: int = 200,  min_samples_leaf: int = 1, min_samples_split: int = 2, test_proportion: float = 0.2) -> List[int]: ...
-
-	def random_forest_regression_predict(self, input_rasters: List[Raster], model_bytes: List[int]) -> Raster: ...
-
-	def random_sample(self, base_raster: Optional[Raster] = None, num_samples: int = 1000) -> Raster: ...
-
-	def range_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def raster_area(self, raster: Raster, units: str = "map units", zero_background: bool = False) -> Tuple[Raster, str]: ...
-
-	def raster_calculator(self, expression: str, input_rasters: List[Raster]) -> Raster: ...
-
-	def raster_cell_assignment(self, raster: Raster, what_to_assign: str = "column") -> Raster: ...
-
-	def raster_histogram(self, raster: Raster, output_html_file: str, num_bins: Optional[int] = None) -> None: ...
-
-	def raster_perimeter(self, raster: Raster, units: str = "map units", zero_background: bool = False) -> Tuple[Raster, str]: ...
-
-	def raster_streams_to_vector(self, streams: Raster, d8_pointer: Raster, esri_pointer: bool = False, all_vertices: bool = False) -> Vector: ...
-
-	def raster_summary_stats(self, input: Raster) -> str: ...
-
-	def raster_to_vector_lines(self, raster: Raster) -> Vector: ...
-
-	def raster_to_vector_points(self, raster: Raster) -> Vector: ...
-
-	def raster_to_vector_polygons(self, raster: Raster) -> Vector: ...
-
-	def rasterize_streams(self, streams: Vector, base_raster: Optional[Raster] = None, zero_background: bool = False, use_feature_id: bool = False) -> Raster: ...
-
-	def reciprocal(self, raster: Raster) -> Raster: ...
-
-	def reclass(self, raster: Raster, reclass_values: List[List[float]], assign_mode: bool = False) -> Raster: ...
-
-	def reclass_equal_interval(self, raster: Raster, interval_size: float, start_value: float = float('-inf'), end_value: float = float('inf')) -> Raster: ...
-
-	def reconcile_multiple_headers(self, input: Vector, region_field_name: str, yield_field_name: str, radius: float, min_yield: float = float('-inf'),  max_yield: float = float('inf'), mean_tonnage: float = float('-inf')) -> Vector: ...
-
-	def recover_flightline_info(self, input: Lidar, max_time_diff: float = 5.0, pt_src_id: bool = False, user_data: bool = False, rgb: bool = False) -> Lidar: ...
-
-	def recreate_pass_lines(self, input: Vector, yield_field_name: str, max_change_in_heading: float = 25.0, ignore_zeros: bool = False) -> Tuple[Vector, Vector]: ...
-
-	def rectangular_grid_from_raster_base(self, base: Raster, width: float, height: float, x_origin: float = 0.0, y_origin: float = 0.0) -> Vector: ...
-
-	def rectangular_grid_from_vector_base(self, base: Vector, width: float, height: float, x_origin: float = 0.0, y_origin: float = 0.0) -> Vector: ...
-
-	def reinitialize_attribute_table(self, input: Vector) -> None: ...
-
-	def related_circumscribing_circle(self, input: Vector) -> Vector: ...
-
-	def relative_aspect(self, dem: Raster, azimuth: float = 0.0, z_factor: float = 1.0) -> Raster: ...
-
-	def relative_stream_power_index(self, specific_catchment_area: Raster, slope: Raster, exponent: float = 1.0) -> Raster: ...
-
-	def relative_topographic_position(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def remove_duplicates(self, input: Lidar, include_z: bool = False) -> Lidar: ...
-
-	def remove_field_edge_points(self, input: Vector, radius: float,  max_change_in_heading: float = 25.0, flag_edges: bool = False) -> Vector: ...
-
-	def remove_off_terrain_objects(self, dem: Raster, filter_size: int = 11, slope_threshold: float = 15.0) -> Raster: ...
-
-	def remove_polygon_holes(self, input: Vector) -> Vector: ...
-
-	def remove_raster_polygon_holes(self, input: Raster, threshold_size: int = sys.maxsize, use_diagonals: bool = False) -> Raster: ...
-
-	def remove_short_streams(self, d8_pntr: Raster, streams_raster: Raster, min_length: float = 0.0, esri_pntr: bool = False) -> Raster: ...
-
-	def remove_spurs(self, raster: Raster, max_iterations: int = 10) -> Raster: ...
-
-	def repair_stream_vector_topology(self, input: Vector, snap_dist: float) -> Vector: ...
-
-	def resample(self, input_rasters: List[Raster], cell_size: float = 0.0, base_raster: Optional[Raster] = None, method: str = "cc") -> Raster: ...
-
-	def rescale_value_range(self, raster: Raster, out_min_val: float, out_max_val: float, clip_min: float = float('inf'), clip_max: float = float('-inf')) -> Raster: ...
-
-	def rgb_to_ihs(self, red: Optional[Raster] = None, green: Optional[Raster] = None, blue: Optional[Raster] = None, composite: Optional[Raster] = None) -> Tuple[Raster, Raster, Raster]: ...
-
-	def rho8_flow_accum(self, raster: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False, esri_pntr: bool = False) -> Raster: ...
-
-	def rho8_pointer(self, dem: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]: ...
-
-	def ring_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def river_centerlines(self, raster: Raster, min_length: int = 3, search_radius: int = 9) -> Vector: ...
-
-	def roberts_cross_filter(self, raster: Raster, clip_amount: float = 0.0) -> Raster: ...
-
-	def root_mean_square_error(self, input: Raster, reference: Raster) -> str: ...
-
-	def rotor(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def ruggedness_index(self, input: Raster) -> Raster: ...
-
-	def scharr_filter(self, raster: Raster, clip_tails: float = 0.0) -> Raster: ...
-
-	def sediment_transport_index(self, specific_catchment_area: Raster, slope: Raster, sca_exponent: float = 0.4, slope_exponent: float = 1.3) -> Raster: ...
-
-	def select_tiles_by_polygon(self, input_directory: str, output_directory: str, polygons: Vector) -> None: ...
-
-	def set_nodata_value(self, raster: Raster, back_value: float = 0.0) -> Raster: ...
-
-	def shadow_animation(self, dem: Raster, output_html_file: str,  palette: WbPalette = WbPalette.Soft, max_dist: float = float('inf'), date: str = "21/06/2021", time_interval: int = 30, location: str = "43.5448/-80.2482/-4", image_height: int = 600, delay: int = 250, label: str = "") -> None: ...
-
-	def shadow_image(self, dem: Raster, palette: WbPalette = WbPalette.Soft, max_dist: float = float('inf'), date: str = "21/06/2021", time: str = "13:00", location: str = "43.5448/-80.2482/-4") -> Raster: ...
-
-	def shape_complexity_index_raster(self, raster: Raster) -> Raster: ...
-
-	def shape_complexity_index_vector(self, input: Vector) -> Vector: ...
-
-	def shape_index(self, dem: Raster, z_factor: float = 1.0) -> Raster: ...
-
-	def shreve_stream_magnitude(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster: ...
-
-	def sigmoidal_contrast_stretch(self, raster: Raster, cutoff: float = 0.0, gain: float = 1.0, num_tones: int = 256) -> Raster: ...
-
-	def singlepart_to_multipart(self, input: Vector, field_name: str) -> Vector: ...
-
-	def sink(self, dem: Raster, zero_background: bool = False) -> Raster: ...
-
-	def skyline_analysis(self, dem: Raster, points: Vector, output_html_file: str, max_dist: float = float('inf'), observer_hgt_offset: float = 0.0, output_as_polygons: bool = True, az_fraction: float = 1.0) -> Vector: ...
-
-	def sky_view_factor(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
-
-	def slope(self, dem: Raster, units: str = "degrees", z_factor: float = 1.0) -> Raster: ...
-
-	def slope_vs_aspect_plot(self, dem: Raster, output_html_file: str, aspect_bin_size: float = 2.0, min_slope: float = 0.1, z_factor: float = 1.0) -> None: ...
-
-	def slope_vs_elev_plot(self, dem_rasters: List[Raster], output_html_file: str, watershed_rasters: List[Raster]) -> None: ...
-
-	def smooth_vectors(self, input: Vector, filter_size: int = 3) -> Vector: ...
-
-	def smooth_vegetation_residual(self, dem: Raster, max_scale: int = 1, dev_threshold: float = 1.0, scale_threshold: int = 5) -> Raster: ...
-
-	def snap_pour_points(self, pour_pts: Vector, flow_accum: Raster, snap_dist: float = 0.0) -> Vector: ...
-
-	def sobel_filter(self, raster: Raster, variant: str = "3x3", clip_tails: float = 0.0) -> Raster: ...
-
-	def sort_lidar(self, sort_criteria: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
-
-	def spherical_std_dev_of_normals(self, dem: Raster, filter_size: int = 11) -> Raster: ...
-
-	def split_colour_composite(self, composite_image: Raster) -> Tuple[Raster, Raster, Raster]: ...
-
-	def split_lidar(self, split_criterion: str, input_lidar: Optional[Lidar], interval: float = 5.0, min_pts: int = 5) -> None: ...
-
-	def split_vector_lines(self, input: Vector, segment_length: float) -> Vector: ...
-
-	def split_with_lines(self, input: Vector, split_vector: Vector) -> Vector: ...
-
-	def standard_deviation_contrast_stretch(self, raster: Raster, clip: float = 2.0, num_tones: int = 256) -> Raster: ...
-
-	def standard_deviation_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def standard_deviation_of_slope(self, dem: Raster, filter_size: int = 11, z_factor: float = 1.0) -> Raster: ...
-
-	def standard_deviation_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def stochastic_depression_analysis(self, dem: Raster, rmse: float, range: float, iterations: int = 100) -> Raster: ...
-
-	def strahler_order_basins(self, d8_pointer: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def strahler_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def stream_link_class(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def stream_link_identifier(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def stream_link_length(self, d8_pointer: Raster, streams_id_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def stream_link_slope(self, d8_pointer: Raster, streams_id_raster: Raster, dem: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def stream_slope_continuous(self, d8_pointer: Raster, streams_raster: Raster, dem: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def subbasins(self, d8_pntr: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def sum_overlay(self, input_rasters: List[Raster]) -> Raster: ...
-
-	def surface_area_ratio(self, dem: Raster) -> Raster: ...
-
-	def svm_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", c_value: float = 50.0, kernel_gamma: float = 0.5, tolerance: float = 0.1, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
-
-	def svm_regression(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", c_value: float = 50.0, epsilon_value: float = 10.0, kernel_gamma: float = 0.5, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
-
-	def symmetrical_difference(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
-
-	def tangential_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def thicken_raster_line(self, raster: Raster) -> Raster: ...
-
-	def time_in_daylight(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), latitude: float = 0.0, longitude: float = 0.0, utc_offset_str: str = "UTC+00:00", start_day: int = 1, end_day: int = 365, start_time: str = "sunrise", end_time: str = "sunset") -> Raster: ...
-
-	def tin_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, max_triangle_edge_length: float = float('inf')) -> Raster: ...
-
-	def tophat_transform(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, variant: str = "white") -> Raster: ...
-
-	def topological_breach_burn(self, streams: Vector, dem: Raster, snap_distance: float = 0.001) -> Tuple[Raster, Raster, Raster, Raster]: ...
-
-	def topological_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def topographic_hachures(self, dem: Raster, contour_interval: float = 10.0, base_contour: float = 0.0, deflection_tolerance: float = 10.0, filter_size: int = 9, separation: float = 2.0, distmin: float = 0.5, distmax: float = 2.0, discretization: float = 0.5, turnmax: float = 45.0, slopemin: float = 0.5, depth: int = 16) -> Vector: ...
-	    
-	def topo_render(self, dem: Raster, palette: WbPalette = WbPalette.Soft, reverse_palette: bool = False,  azimuth: float = 315.0, altitude: float = 30.0, clipping_polygon: Optional[Vector] = None, background_hgt_offset: float = 10.0, background_clr: Tuple[int, int, int, int] = (255, 255, 255, 255), attenuation_parameter: float = 0.3,  ambient_light: float = 0.2, z_factor: float = 1.0) -> Raster: ...
-
-	def topographic_position_animation(self, dem: Raster, output_html_file: str = "topo_pos.html", palette: WbPalette = WbPalette.Soft,  min_scale: int = 1, num_steps: int = 1, step_nonlinearity: float = 1.0, image_height: int = 600, delay: int = 250, label: str = "", use_dev_max: bool = False) -> None: ...
-
-	def total_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def total_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
-
-	def trace_downslope_flowpaths(self, seed_points: Vector, d8_pointer: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def travelling_salesman_problem(self, input: Vector, duration: int = 60) -> Vector: ...
-
-	def trend_surface(self, raster: Raster, output_html_file: str, polynomial_order: int = 1) -> Raster: ...
-
-	def trend_surface_vector_points(self, input: Vector, cell_size: float, output_html_file: str, field_name: str = "FID", polynomial_order: int = 1) -> Raster: ...
-
-	def tributary_identifier(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
-
-	def turning_bands_simulation(self, base_raster: Optional[Raster] = None, range: float = 1.0, iterations: int = 1000) -> Raster: ...
-
-	def two_sample_ks_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
-
-	def union(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
-
-	def unnest_basins(self, d8_pointer: Raster, pour_points: Vector, esri_pntr: bool = False) -> List[Raster]: ...
-
-	def unsharp_masking(self, raster: Raster, sigma: float = 0.75, amount: float = 100.0, threshold: float = 0.0) -> Raster: ...
-
-	def unsphericity(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def update_nodata_cells(self, input1: Raster, input2: Raster) -> Raster: ...
-
-	def upslope_depression_storage(self, dem: Raster) -> Raster: ...
-
-	def user_defined_weights_filter(self, raster: Raster, weights: List[List[float]], kernel_center: str = "center", normalize_weights: bool = False) -> Raster: ...
-
-	def vector_hex_binning(self, vector_points: Vector, width: float, orientation: str = "horizontal") -> Vector: ...
-
-	def vector_lines_to_raster(self, input: Vector, field_name: str = "FID", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def vector_points_to_raster(self, input: Vector, field_name: str = "FID", assign_op: str = "last", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def vector_polygons_to_raster(self, input: Vector, field_name: str = "FID", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
-
-	def vertical_excess_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
-
-	def vector_stream_network_analysis(self, streams: Vector, dem: Raster, max_ridge_cutting_height: float = 10.0, snap_distance: float = 0.001) -> Tuple[Vector, Vector, Vector, Vector]: ...
-
-	def viewshed(self, dem: Raster, station_points: Vector, station_height: float = 2.0) -> Raster: ...
-
-	def visibility_index(self, dem: Raster, station_height: float = 2.0, resolution_factor: int = 8) -> Raster: ...
-
-	def voronoi_diagram(self, input_points: Vector) -> Vector: ...
-
-	def watershed(self, d8_pointer: Raster, pour_points: Vector, esri_pntr: bool = False) -> Raster: ...
-
-	def watershed_from_raster_pour_points(self, d8_pointer: Raster, pour_points: Raster, esri_pntr: bool = False) -> Raster: ...
-
-	def weighted_overlay(self, factors: List[Raster], weights: List[float], cost: Optional[List[Raster]] = None, constraints: Optional[List[Raster]] = None, scale_max: float = 1.0) -> Raster: ...
-
-	def weighted_sum(self, input_rasters: List[Raster], weights: List[float]) -> Raster: ...
-
-	def wetness_index(self, specific_catchment_area: Raster, slope: Raster) -> Raster: ...
-
-	def wilcoxon_signed_rank_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
-
-	def write_function_memory_insertion(self, image1: Raster, image2: Raster, image3: Raster) -> Raster: ...
-
-	def yield_filter(self, input: Vector, yield_field_name: str, pass_field_name: str,  swath_width: float = 6.096, z_score_threshold: float = 2.5, min_yield: float = 0.0, max_yield: float = float('inf')) -> Vector: ...
-
-	def yield_map(self, input: Vector, pass_field_name: str, swath_width: float = 6.096, max_change_in_heading: float = 25.0) -> Vector: ...
-
-	def yield_normalization(self, input: Vector, yield_field_name: str,  radius: float, standardize: bool = False, min_yield: float = 0.0, max_yield: float = float('inf')) -> Vector: ...
-
-	def z_scores(self, raster: Raster) -> Raster: ...
-
-	def zonal_statistics(self, data_raster: Raster, feature_definitions_raster: Raster, stat_type: str = "mean", zero_is_background: bool = False) -> Tuple[Raster, str]: ...
-
-
-class WbPalette(Enum):
-	Atlas: int
-	HighRelief: int
-	Arid: int
-	Earthtones: int
-	Soft: int
-	Muted: int
-	LightQuant: int 
-	Turbo: int
-	Purple: int
-	Viridis: int
-	GreenYellow: int
-	PinkYellowGreen: int
-	BlueYellowRed: int
-	Deep: int
-	Imhof: int
-	White: int
+import sys
+from typing import List, Optional, Tuple, Union
+from enum import Enum
+
+def activate_license(key: str, firstname: str, lastname: str, email: str, agree_to_license_terms: bool) -> None: ...
+
+def check_in_license(key: str) -> str: ...
+
+def deactivate_license() -> None: ...
+
+def download_sample_data(data_set: str) -> str: ...
+
+def license_info() -> None: ...
+
+def transfer_license() -> None: ...
+
+class AttributeField():
+
+	@property
+	def name(self) -> str: ...
+    		
+	@property
+	def field_type(self) -> int: ...
+    
+	@property
+	def field_length(self) -> int: ...
+    	
+	@property
+	def decimal_count(self) -> int: ...
+
+	@staticmethod
+	def new(name: str, field_type: FieldDataType, field_length: int, decimal_count: int) -> AttributeField: ...
+
+class AttributeHeader():
+	@property
+	def version(self) -> int: ...
+
+	@property
+	def year(self) -> int: ...
+
+	@property
+	def month(self) -> int: ...
+
+	@property
+	def day(self) -> int: ...
+
+	@property
+	def num_records(self) -> int: ...
+
+	@property
+	def num_fields(self) -> int: ...
+
+	@property
+	def bytes_in_header(self) -> int: ...
+
+	@property
+	def bytes_in_record(self) -> int: ...
+
+	@property
+	def incomplete_tansaction(self) -> int: ...
+
+	@property
+	def encryption_flag(self) -> int: ...
+
+	@property
+	def mdx_flag(self) -> int: ...
+
+	@property
+	def language_driver_id(self) -> int: ...
+
+class BoundingBox():
+	@property
+	def min_x(self) -> float: ...
+
+	@min_x.setter
+	def min_x(self, value: float) -> None: ...
+
+	@property
+	def min_y(self) -> float: ...
+
+	@min_y.setter
+	def min_y(self, value: float) -> None: ...
+
+	@property
+	def max_x(self) -> float: ...
+
+	@max_x.setter
+	def max_x(self, value: float) -> None: ...
+
+	@property
+	def max_y(self) -> float: ...
+
+	@max_y.setter
+	def max_y(self, value: float) -> None: ...
+
+	@staticmethod
+	def new(min_x: float, max_x: float, min_y: float, max_y: float) -> Point2D: ...
+
+	@staticmethod
+	def from_two_points(p1: Point2D, p2: Point2D) -> BoundingBox: ...
+
+	def initialize_to_inf(self) -> None: ...
+
+	def get_height(self) -> float: ...
+
+	def get_width(self) -> float: ...
+
+	def is_point_in_box(self, x: float, y: float) -> bool: ...
+
+	def overlaps(self, other: BoundingBox) -> bool: ...
+
+	def nearly_overlaps(self, other: BoundingBox) -> bool: ...
+
+	def intersects_edge_of(self, other: BoundingBox) -> bool: ...
+
+	def entirely_contained_within(self, other: BoundingBox) -> bool: ...
+
+	def within(self, other: BoundingBox) -> bool: ...
+
+	def entirely_contains(self, other: BoundingBox) -> bool: ...
+
+	def contains(self, other: BoundingBox) -> bool: ...
+
+	def intersect(self, other: BoundingBox) -> BoundingBox: ...
+
+	def expand_to(self, other: BoundingBox) -> None: ...
+
+	def contract_to(self, other: BoundingBox) -> None: ...
+
+	def expand_by(self, value: float) -> None: ...
+
+	def contract_by(self, value: float) -> None: ...
+
+class ColourData():
+	@property
+	def red(self) -> int: ...
+
+	@red.setter
+	def red(self, value: int) -> None: ...
+
+	@property
+	def green(self) -> int: ...
+
+	@green.setter
+	def green(self, value: int) -> None: ...
+
+	@property
+	def blue(self) -> int: ...
+
+	@blue.setter
+	def blue(self, value: int) -> None: ...
+
+	@property
+	def nir(self) -> int: ...
+
+	@nir.setter
+	def nir(self, value: int) -> None: ...
+
+class DateData():
+	@property
+	def year(self) -> int: ...
+
+	@property
+	def month(self) -> int: ...
+
+	@property
+	def day(self) -> int: ...	
+	
+class FieldData():
+	@staticmethod
+	def new() -> FieldData: ...
+
+	@staticmethod
+	def new_int(value: int) -> FieldData: ...
+
+	@staticmethod
+	def new_real(value: float) -> FieldData: ...
+
+	@staticmethod
+	def new_text(value: str) -> FieldData: ...
+
+	@staticmethod
+	def new_date(value: DateData) -> FieldData: ...
+
+	@staticmethod
+	def new_bool(value: bool) -> FieldData: ...
+
+	@staticmethod
+	def new_null() -> FieldData: ...
+
+	def get_type(self) -> FieldDataType: ...
+
+	def get_value_as_f64(self) -> float: ...
+
+	def get_as_string(self) -> str: ...
+
+class FieldDataType(Enum):
+	Bool: int
+	Date: int
+	Int: int
+	Real: int
+	Text: int
+
+class GlobalEncodingField():
+	def __init__(self):
+		self.value = 0
+
+class LicenseType(Enum):
+	WbW: str
+	WbWPro: str
+
+class LidarHeader(): 
+	@property
+	def file_signature(self) -> str: ...
+    
+	@property
+	def file_source_id(self) -> int: ...
+
+	@property
+	def global_encoding(self) -> GlobalEncodingField: ...
+
+	@property
+	def project_id_used(self) -> bool: ...
+	
+	@property
+	def project_id1(self) -> int: ...
+	
+	@property
+	def project_id2(self) -> int: ...
+
+	@property
+	def project_id3(self) -> int: ...
+
+	@property
+	def project_id4(self) -> Tuple[int]: ...
+
+	@property
+	def version_major(self) -> int: ...
+
+	@property
+	def version_minor(self) -> int: ...
+
+	@property
+	def system_id(self) -> str: ...
+
+	@property
+	def generating_software(self) -> str: ...
+
+	@property
+	def file_creation_day(self) -> int: ...
+
+	@property
+	def file_creation_year(self) -> int: ...
+
+	@property
+	def header_size(self) -> int: ...
+
+	@property
+	def offset_to_points(self) -> int: ...
+
+	@property
+	def number_of_vlrs(self) -> int: ...
+
+	@property
+	def number_of_extended_vlrs(self) -> int: ...
+
+	@property
+	def offset_to_ex_vlrs(self) -> int: ...
+
+	@property
+	def point_record_length(self) -> int: ...
+
+	@property
+	def point_format(self) -> int: ...
+
+	@property
+	def number_of_points_old(self) -> int: ...
+
+	@property
+	def number_of_points(self) -> int: ...
+
+	@property
+	def number_of_points_by_return_old(self) -> Tuple[int, int, int, int, int]: ...
+
+	@property
+	def number_of_points_by_return(self) -> Tuple[int, int, int, int, int, int, int, int, int, int, int, int, int, int, int]: ...
+
+	@property
+	def x_scale_factor(self) -> float: ...
+
+	@property
+	def y_scale_factor(self) -> float: ...
+
+	@property
+	def z_scale_factor(self) -> float: ...
+
+	@property
+	def x_offset(self) -> float: ...
+
+	@property
+	def y_offset(self) -> float: ...
+
+	@property
+	def z_offset(self) -> float: ...
+
+	@property
+	def max_x(self) -> float: ...
+
+	@property
+	def min_x(self) -> float: ...
+
+	@property
+	def max_y(self) -> float: ...
+
+	@property
+	def min_y(self) -> float: ...
+
+	@property
+	def max_z(self) -> float: ...
+
+	@property
+	def min_z(self) -> float: ...
+
+	@property
+	def waveform_data_start(self) -> int: ...
+
+	def get_num_points(self) -> int: ...
+
+class LidarPointData():
+	@property
+	def x(self) -> int: ...
+
+	@property
+	def y(self) -> int: ...
+
+	@property
+	def z(self) -> int: ...
+
+	@property
+	def intensity(self) -> int: ...
+
+	@property
+	def point_bit_field(self) -> int: ...
+
+	@property
+	def class_bit_field(self) -> int: ...
+
+	# @property
+	# def classification(self) -> int: ...
+
+	@property
+	def scan_angle(self) -> int: ...
+
+	@property
+	def user_data(self) -> int: ...
+
+	@property
+	def point_source_id(self) -> int: ...
+
+	@property
+	def is_64bit(self) -> bool: ...
+
+	def get_32bit_from_64bit(self) -> Tuple[int, int]: ...
+
+	def return_number(self) -> int: ...
+
+	def set_return_number(self, value: int) -> None: ...
+
+	def number_of_returns(self) -> int: ...
+
+	def set_number_of_returns(self, value: int) -> None: ...
+
+	def is_only_return(self) -> bool: ...
+
+	def is_multiple_return(self) -> bool: ...
+
+	def is_early_return(self) -> bool: ...
+
+	def is_late_return(self) -> bool: ...
+
+	def is_last_return(self) -> bool: ...
+
+	def is_first_return(self) -> bool: ...
+
+	def is_intermediate_return(self) -> bool: ...
+
+	def scan_direction_flag(self) -> bool: ...
+
+	def set_scan_direction_flag(self, value: bool) -> None: ...
+
+	def edge_of_flightline_flag(self) -> bool: ...
+
+	def set_edge_of_flightline_flag(self, value: bool) -> None: ...
+
+	def classification(self) -> int: ...
+
+	def set_classification(self, value: int) -> None: ...
+
+	def classification_string(self) -> str: ...
+
+	def is_classified_vegetation(self) -> bool: ...
+
+	def synthetic(self) -> bool: ...
+
+	def set_synthetic(self, value: bool) -> None: ...
+
+	def keypoint(self) -> bool: ...
+
+	def set_keypoint(self, value: bool) -> None: ...
+
+	def withheld(self) -> bool: ...
+
+	def set_withheld(self, value: bool) -> None: ...
+
+	def overlap(self) -> bool: ...
+
+	def set_overlap(self, value: bool) -> None: ...
+
+	def is_classified_noise(self) -> bool: ...
+
+	def scanner_channel(self) -> int: ...
+
+	def set_scanner_channel(self, value: int) -> None: ...
+
+class Lidar():
+    	
+	@property
+	def file_name(self) -> str: ...
+
+	@file_name.setter
+	def file_name(self, value: str): ...
+
+	@property
+	def header(self) -> LidarHeader: ...
+
+	@property
+	def vlr_data(self) -> List[VariableLengthRecord]: ...
+
+	@vlr_data.setter
+	def vlr_data(self, value: List[VariableLengthRecord]): ...
+
+	@property
+	def wkt(self) -> str: ...
+    
+	@property
+	def use_point_intensity(self) -> bool: ...
+    
+	@property
+	def use_point_userdata(self) -> bool: ...
+
+	def get_point_record(self, index: int) -> Tuple[LidarPointData, Optional[float], Optional[ColourData], Optional[WaveformPacket]]: ...
+
+	def get_transformed_xyz(self, index: int) -> Tuple[float, float, float]: ...
+
+	def add_point(self, point_data: LidarPointData, time: Optional[float] = None, colour_data: Optional[ColourData] = None, waveform_data: Optional[WaveformPacket] = None) -> None: ...
+
+	def has_time_data(self) -> bool: ...
+
+	def has_colour_data(self) -> bool: ...
+
+	def has_waveform_data(self) -> bool: ...
+
+	def get_well_known_text(self) -> str: ...
+
+	def print_variable_length_records(self) -> str: ...
+
+class PhotometricInterpretation(Enum):
+	Continuous: int
+	Categorical: int
+	Boolean: int
+	RGB: int
+	Paletted: int
+	Unknown: int
+
+class Point2D:
+	@property
+	def x(self) -> float: ...
+
+	@x.setter
+	def x(self, value: float) -> None: ...
+
+	@property
+	def y(self) -> float: ...
+
+	@y.setter
+	def y(self, value: float) -> None: ...
+
+	@staticmethod
+	def new(x: float, y: float) -> Point2D: ...
+
+class Point3D:
+	@property
+	def x(self) -> float: ...
+
+	@x.setter
+	def x(self, value: float) -> None: ...
+
+	@property
+	def y(self) -> float: ...
+
+	@y.setter
+	def y(self, value: float) -> None: ...
+
+	@property
+	def z(self) -> float: ...
+
+	@z.setter
+	def z(self, value: float) -> None: ...
+
+	@staticmethod
+	def new(x: float, y: float, z: float) -> Point2D: ...
+
+class RasterDataType(Enum):
+	F64: int
+	F32: int
+	I64: int
+	U64: int
+	RGB48: int
+	I32: int
+	U32: int
+	RGB24: int
+	RGBA32: int
+	I16: int
+	U16: int
+	I8: int
+	U8: int
+	Unknown: int
+
+
+	def get_data_size(self) -> int: ...
+
+	def is_float(self) -> bool: ...
+
+	def is_integer(self) -> bool: ...
+
+	def is_unsigned_integer(self) -> bool: ...
+
+	def is_signed_integer(self) -> bool: ...
+
+	def is_colour_data(self) -> bool: ...
+
+	def return_wider(self, other: RasterDataType) -> RasterDataType: ...
+
+class RasterConfigs():
+	@property
+	def title(self) -> str: ...
+
+	@title.setter
+	def title(self, value): ...
+
+	@property
+	def rows(self) -> int: ...
+
+	@rows.setter
+	def rows(self, value: int) -> None: ...
+
+	@property
+	def columns(self) -> int: ...
+
+	@columns.setter
+	def columns(self, value: int) -> None: ...
+
+	@property
+	def nodata(self) -> float: ...
+
+	@nodata.setter
+	def nodata(self, value: float) -> None: ...
+
+	@property
+	def north(self) -> float: ...
+
+	@north.setter
+	def north(self, value: float) -> None: ...
+
+	@property
+	def south(self) -> float: ...
+
+	@south.setter
+	def south(self, value: float) -> None: ...
+
+	@property
+	def east(self) -> float: ...
+
+	@east.setter
+	def east(self, value: float) -> None: ...
+
+	@property
+	def west(self) -> float: ...
+
+	@west.setter
+	def west(self, value: float) -> None: ...
+
+	@property
+	def resolution_x(self) -> float: ...
+
+	@resolution_x.setter
+	def resolution_x(self, value: float) -> None: ...
+
+	@property
+	def resolution_y(self) -> float: ...
+
+	@resolution_y.setter
+	def resolution_y(self, value: float) -> None: ...
+
+	@property
+	def minimum(self) -> float: ...
+
+	@minimum.setter
+	def minimum(self, value: float) -> None: ...
+
+	@property
+	def maximum(self) -> float: ...
+
+	@maximum.setter
+	def maximum(self, value: float) -> None: ...
+
+	# @property
+	# def display_min(self) -> float: ...
+
+	# @display_min.setter
+	# def display_min(self, value: float) -> None: ...
+
+	# @property
+	# def display_max(self) -> float: ...
+
+	# @display_max.setter
+	# def display_max(self, value: float) -> None: ...
+
+	@property
+	def palette(self) -> str: ...
+
+	@property
+	def projection(self) -> str: ...
+
+	@property
+	def photometric_interp(self) -> PhotometricInterpretation: ...
+
+	@photometric_interp.setter
+	def photometric_interp(self, value: PhotometricInterpretation) -> None: ...
+
+	@property
+	def data_type(self) -> RasterDataType: ...
+
+	@data_type.setter
+	def data_type(self, value: RasterDataType) -> None: ...
+
+	@property
+	def z_units(self) -> str: ...
+
+	@property
+	def xy_units(self) -> str: ...
+
+	@property
+	def reflect_at_edges(self) -> bool: ...
+
+	@reflect_at_edges.setter
+	def reflect_at_edges(self, value: bool) -> None: ...
+
+	@property
+	def pixel_is_area(self) -> bool: ...
+
+	@pixel_is_area.setter
+	def pixel_is_area(self, value: bool) -> None: ...
+
+	@property
+	def epsg_code(self) -> int: ...
+
+	@epsg_code.setter
+	def epsg_code(self, value: int) -> None: ...
+
+	@property
+	def coordinate_ref_system_wkt(self) -> str: ...
+
+	@epsg_code.setter
+	def coordinate_ref_system_wkt(self, value: str) -> None: ...
+
+	@staticmethod
+	def new() -> RasterConfigs: ...
+
+class RasterType():
+	Unknown: int
+	ArcAscii: int
+	ArcBinary: int
+	EsriBil: int
+	GeoTiff: int
+	GrassAscii: int
+	IdrisiBinary: int
+	SagaBinary: int
+	Surfer7Binary: int
+	SurferAscii: int
+	Whitebox: int
+
+class Raster():
+	@property
+	def file_name(self) -> str: ...
+
+	@file_name.setter
+	def file_name(self, value: str) -> None: ...
+
+	@property
+	def file_mode(self) -> str: ...
+	
+	@property
+	def raster_type(self) -> RasterType: ...
+
+	@property
+	def configs(self) -> RasterConfigs: ...
+
+	@staticmethod
+	def new_from_other(other: Raster, data_type: Optional[RasterDataType]) -> Raster: ...
+
+	def get_value(self, row: int, column: int) -> float: ...
+
+	def set_value(self, row: int, column: int, value: float) -> None: ...
+
+	def decrement(self, row: int, column: int, value: float) -> None: ...
+
+	def increment(self, row: int, column: int, value: float) -> None: ...
+
+	def set_row_data(self, row: int, values: List[float]) -> None: ...
+
+	def get_row_data(self, row: int) -> List[float]: ...
+
+	def increment_row_data(self, row: int, values: List[float]) -> None: ...
+
+	def decrement_row_data(self, row: int, values: List[float]) -> None: ...
+
+	def set_data_from_raster(self, other: Raster) -> Optional[str]: ...
+
+	def reinitialize_values(self, value: float) -> None: ...
+
+	def get_value_as_rgba(self, row: int, column: int) -> Tuple[int, int, int, int]: ...
+
+	def get_value_as_hsi(self, row: int, column: int) -> Tuple[float, float, float]: ...
+
+	def set_value_from_rgba(self, row: int, column: int, rgba: Tuple[int, int, int, int]) -> None: ...
+
+	def get_data_size_in_bytes(self) -> int: ...
+
+	def get_x_from_column(self, column: int) -> float: ...
+
+	def get_y_from_row(self, row: int) -> float: ...
+
+	def get_column_from_x(self, x: float) -> int: ...
+
+	def get_row_from_y(self, y: float) -> int: ...
+
+	def size_of(self) -> int: ...
+
+	def __add__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __sub__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __mul__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __truediv__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __floordiv__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __mod__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __pow__(self, other: Union[Raster, float], modulo: Optional[float] = None) -> Raster: ...
+
+	def __neg__(self) -> Raster: ...
+
+	def __abs__(self) -> Raster: ...
+
+	def __iadd__(self, other: Union[Raster, float]) -> None: ...
+
+	def __isub__(self, other: Union[Raster, float]) -> None: ...
+
+	def __imul__(self, other: Union[Raster, float]) -> None: ...
+
+	def __idiv__(self, other: Union[Raster, float]) -> None: ...
+
+	def __getitem__(self, row_column: Tuple[int, int]) -> float: ...
+
+	def __setitem__(self, row_column: Tuple[int, int], value: float) -> None: ...
+
+	def __gt__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __ge__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __lt__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __le__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __eq__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def __ne__(self, other: Union[Raster, float]) -> Raster: ...
+
+	def acos(self) -> Raster: ...
+
+	def acosh(self) -> Raster: ...
+
+	def asin(self) -> Raster: ...
+
+	def asinh(self) -> Raster: ...
+
+	def atan(self) -> Raster: ...
+
+	def atan2(self, other: Union[Raster, float]) -> Raster: ...
+
+	def atanh(self) -> Raster: ...
+
+	def ceil(self) -> Raster: ...
+
+	def con(self, con_statement: str, true_raster_or_float: Union[Raster, float, str], false_raster_or_float: Union[Raster, float, str]) -> Raster: ...
+
+	def cos(self) -> Raster: ...
+
+	def cosh(self) -> Raster: ...
+
+	def exp(self) -> Raster: ...
+
+	def exp2(self) -> Raster: ...
+
+	def floor(self) -> Raster: ...
+
+	def is_nodata(self) -> Raster: ...
+
+	def ln(self) -> Raster: ...
+
+	def log2(self) -> Raster: ...
+
+	def log10(self) -> Raster: ...
+
+	def max(self, other: Union[Raster, float]) -> Raster: ...
+
+	def min(self, other: Union[Raster, float]) -> Raster: ...
+
+	def normalize(self) -> Raster: ...
+
+	def signum(self) -> Raster: ...
+
+	def sin(self) -> Raster: ...
+
+	def sinh(self) -> Raster: ...
+
+	def sqrt(self) -> Raster: ...
+
+	def square(self) -> Raster: ...
+
+	def tan(self) -> Raster: ...
+
+	def tanh(self) -> Raster: ...
+
+	def to_degrees(self) -> Raster: ...
+
+	def to_radians(self) -> Raster: ...
+
+	def trunc(self) -> Raster: ...
+
+	def num_cells(self) -> int: ...
+
+	def num_valid_cells(self) -> int: ...
+
+	def calculate_mean(self) -> float: ...
+
+	def calculate_mean_and_stdev(self) -> Tuple[float, float]: ...
+
+	def calculate_clip_values(self, percent: float) -> Tuple[float, float]: ...
+
+	def deep_copy(self) -> Raster: ...
+
+	def update_min_max(self) -> None: ...
+
+class VariableLengthRecord():
+	@property
+	def reserved(self) -> int: ...
+	
+	@property
+	def user_id(self) -> str: ...
+	
+	@property
+	def record_id(self) -> int: ...
+	
+	@property
+	def record_length_after_header(self) -> int: ...
+	
+	@property
+	def description(self) -> str: ...
+	
+	@property
+	def binary_data(self) -> List[int]: ...
+
+class VectorAttributes():
+	@property
+	def header(self) -> AttributeHeader: ...
+
+	@property
+	def fields(self) -> List[AttributeField]: ...
+
+	@property
+	def is_deleted(self) -> List[bool]: ...
+
+	def get_num_fields(self) -> int: ...
+
+class VectorGeometry():
+	@property
+	def shape_type(self) -> VectorGeometryType: ...
+
+	@property
+	def x_min(self) -> float: ...
+
+	@property
+	def x_max(self) -> float: ...
+
+	@property
+	def y_min(self) -> float: ...
+
+	@property
+	def y_max(self) -> float: ...
+
+	@property
+	def num_parts(self) -> int: ...
+
+	@property
+	def num_points(self) -> int: ...
+
+	@property
+	def parts(self) -> List[int]: ...
+
+	@property
+	def points(self) -> List[Point2D]: ...
+
+	@property
+	def z_min(self) -> float: ...
+
+	@property
+	def z_max(self) -> float: ...
+
+	@property
+	def z_array(self) -> List[float]: ...
+
+	@property
+	def m_min(self) -> float: ...
+
+	@property
+	def m_max(self) -> float: ...
+
+	@property
+	def m_array(self) -> List[float]: ...
+
+	@staticmethod
+	def new_vector_geometry(shape_type: VectorGeometryType) -> VectorGeometry: ...
+
+	def add_point(self, p: Point2D) -> None: ...
+
+	def add_pointm(self, p: Point2D, m: float) -> None: ...
+
+	def add_pointz(self, p: Point2D, m: float, z: float) -> None: ...
+
+	def add_geom_part(self, points: List[Point2D]) -> None: ...
+
+	def add_geom_partm(self, points: List[Point2D], measures: List[float]) -> None: ...
+
+	def add_geom_partz(self, points: List[Point2D], measures: List[float], z_values: List[float]) -> None: ...
+
+	def get_bounding_box(self) -> BoundingBox: ...
+
+	def get_length(self) -> int: ...
+
+	def has_m_data(self) -> bool: ...
+
+	def has_z_data(self) -> bool: ...
+
+	def is_hole(self, part_num: int) -> bool: ...
+
+class VectorGeometryType(Enum):
+	Null: int
+	Point: int
+	PolyLine: int
+	Polygon: int
+	MultiPoint: int
+	PointZ: int
+	PolyLineZ: int
+	PolygonZ: int
+	MultiPointZ: int
+	PointM: int
+	PolyLineM: int
+	PolygonM: int
+	MultiPointM: int
+
+class VectorHeader():
+	@property
+	def file_length(self) -> int: ...
+
+	@property
+	def version(self) -> int: ...
+
+	@property
+	def shape_type(self) -> VectorGeometryType: ...
+
+	@property
+	def x_min(self) -> float: ...
+
+	@property
+	def y_min(self) -> float: ...
+
+	@property
+	def x_max(self) -> float: ...
+
+	@property
+	def y_max(self) -> float: ...
+
+	@property
+	def z_min(self) -> float: ...
+
+	@property
+	def z_max(self) -> float: ...
+
+	@property
+	def m_min(self) -> float: ...
+
+	@property
+	def m_max(self) -> float: ...
+
+class Vector():
+	@property
+	def file_name(self) -> str: ...
+
+	@file_name.setter
+	def file_name(self, value: str) -> None: ...
+
+	@property
+	def file_mode(self) -> str: ...
+
+	@property
+	def header(self) -> VectorHeader: ...
+
+	@property
+	def num_records(self) -> int: ...
+
+	@property
+	def records(self) -> List[VectorGeometry]: ...
+
+	@property
+	def attributes(self) -> VectorAttributes: ...
+
+	@property
+	def projection(self) -> str: ...
+
+	def __getitem__(self, index: int) -> VectorGeometry: ...
+
+	def add_record(self, geometry: VectorGeometry) -> None: ...
+
+	def add_attribute_field(self, field: AttributeField) -> None: ...
+
+	def add_attribute_fields(self, fields: List[AttributeField]) -> None: ...
+
+	def add_attribute_record(self, rec: List[FieldData], deleted: bool) -> None: ...
+
+	def contains_attribute_field(self, field: AttributeField) -> bool: ...
+
+	def get_attribute_fields(self) -> List[AttributeField]: ...
+
+	def get_attribute_record(self, index: int) -> List[FieldData]: ...
+
+	def get_attribute_field_info(self, index: int) -> AttributeField: ...
+
+	def get_attribute_field_num(self, name: str) -> Optional[int]: ...
+
+	def get_num_attributes_fields(self) -> int: ...
+
+	def get_attribute_value(self, record_index: int, field_name: str) -> FieldData: ...
+
+	def is_attribute_field_numeric(self, index: int) -> bool: ...
+
+	def reinitialize_attributes(self) -> None: ...
+
+	def set_attribute_value(self, record_index: int, field_name: str, field_data: FieldData) -> None: ...
+
+class WaveformPacket():
+	@property
+	def packet_descriptor_index(self) -> int: ...
+
+	@packet_descriptor_index.setter
+	def packet_descriptor_index(self, value: int) -> None: ...
+
+	@property
+	def offset_to_waveform_data(self) -> int: ...
+
+	@offset_to_waveform_data.setter
+	def offset_to_waveform_data(self, value: int) -> None: ...
+
+	@property
+	def waveform_packet_size(self) -> int: ...
+
+	@waveform_packet_size.setter
+	def waveform_packet_size(self, value: int) -> None: ...
+
+	@property
+	def ret_point_waveform_loc(self) -> float: ...
+
+	@ret_point_waveform_loc.setter
+	def ret_point_waveform_loc(self, value: float) -> None: ...
+
+	@property
+	def xt(self) -> float: ...
+
+	@xt.setter
+	def xt(self, value: float) -> None: ...
+
+	@property
+	def yt(self) -> float: ...
+
+	@yt.setter
+	def yt(self, value: float) -> None: ...
+
+	@property
+	def zt(self) -> float: ...
+
+	@zt.setter
+	def zt(self, value: float) -> None: ...
+
+class WbEnvironment():
+    	
+	@property
+	def max_procs(self) -> int: ...
+
+	@max_procs.setter
+	def max_procs(self, value: int) -> None: ...
+
+	@property
+	def verbose(self) -> bool: ...
+
+	@verbose.setter
+	def verbose(self, value: bool) -> None: ...
+
+	@property
+	def working_directory(self) -> str: ...
+
+	@working_directory.setter
+	def working_directory(self, value: str) -> None: ...
+
+	def __new__(cls, user_id: str = "") -> WbEnvironment: ...
+
+	def version(self) -> str: ...
+
+	def read_lidar(self, file_name: str, file_mode: str = "r") -> Lidar: ...
+
+	def read_lidars(self, file_names: List[str]) -> List[Lidar]: ...
+
+	def new_lidar(self, header: LidarHeader) -> Lidar: ...
+
+	def write_lidar(self, lidar: Lidar, file_name: str) -> None: ...
+
+	def read_raster(self, file_name: str) -> Raster: ...
+
+	def read_rasters(self, file_name: List[str]) -> List[Raster]: ...
+
+	def new_raster(self, configs: RasterConfigs) -> Raster: ...
+
+	def write_raster(self, raster: Raster, file_name: str, compress: bool = False) -> None: ...
+
+	def read_vector(self, file_name: str) -> Vector: ...
+
+	def read_vectors(self, file_name: List[str]) -> List[Vector]: ...
+
+	def new_vector(self,  shape_type: VectorGeometryType, attributes: Optional[List[AttributeField]] = None, proj: str = "") -> Vector: ...
+
+	def write_vector(self, vector: Vector, file_name: str) -> None: ...
+
+	def write_text(self, text: str, file_name: str) -> None: ...
+
+	def accumulation_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def adaptive_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, threshold: float = 2.0) -> Raster: ...
+	
+	def add_point_coordinates_to_table(self, input: Vector) -> Vector: ...
+
+	def aggregate_raster(self, raster: Raster, aggregation_factor: int = 2, aggregation_type: str = "mean") -> Raster: ...
+
+	def anova(self, input_raster: Raster, features_raster: Raster, output_html_file: str) -> None: ...
+
+	def ascii_to_las(self, input_ascii_files: List[str], pattern: str, epsg_code: int) -> None: ...
+
+	def aspect(self, dem: Raster, z_factor: float = 1.0) -> Raster: ...
+
+	def assess_route(self, routes: Vector, dem: Raster, segment_length: float = 100.0, search_radius: int = 15) -> Vector: ...
+
+	def attribute_correlation(self, input: Vector, output_html_file: str) -> None: ...
+
+	def attribute_histogram(self, input: Vector, field_name: str, output_html_file: str) -> None: ...
+
+	def attribute_scattergram(self, input: Vector, field_name_x: str, field_name_y: str, output_html_file: str, add_trendline: bool = False) -> None: ...
+
+	def average_flowpath_slope(self, dem: Raster) -> Raster: ...
+
+	def average_horizon_distance(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
+
+	def average_normal_vector_angular_deviation(self, dem: Raster, filter_size: int = 11) -> Raster: ...
+
+	def average_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def average_upslope_flowpath_length(self, dem: Raster) -> Raster: ...
+
+	def balance_contrast_enhancement(self, image: Raster, band_mean: float = 100.0) -> Raster: ...
+
+	def basins(self, d8_pntr: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def bilateral_filter(self, raster: Raster, sigma_dist: float = 0.75, sigma_int: float = 1.0) -> Raster: ...
+
+	def block_maximum(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def block_minimum(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def bool_and(self, input1: Raster, input2: Raster) -> Raster: ...
+
+	def bool_not(self, input1: Raster, input2: Raster) -> Raster: ...
+
+	def bool_or(self, input1: Raster, input2: Raster) -> Raster: ...
+
+	def bool_xor(self, input1: Raster, input2: Raster) -> Raster: ...
+
+	def boundary_shape_complexity(self, raster: Raster) -> Raster: ...
+
+	def breach_depressions_least_cost(self, dem: Raster, max_cost: float = float('inf'), max_dist: int = 100, flat_increment: float = float('nan'), fill_deps: bool = False, minimize_dist: bool = False) -> Raster: ...
+
+	def breach_single_cell_pits(self, dem: Raster) -> Raster: ...
+
+	def breakline_mapping(self, dem: Raster, threshold: float = 0.8, min_length: int = 3) -> Vector: ...
+
+	def buffer_raster(self, input: Raster, buffer_size: float, grid_cells_units: bool = False) -> Raster: ...
+
+	def burn_streams_at_roads(self, dem: Raster, streams: Vector, roads: Vector, road_width: float) -> Raster: ...
+
+	def canny_edge_detection(self, input: Raster, sigma: float = 0.5, low_threshold: float = 0.05, high_threshold: float = 0.15, add_back_to_image: bool = False) -> Raster: ...
+
+	def centroid_raster(self, input: Raster) -> Tuple[Raster, str]: ...
+
+	def centroid_vector(self, input: Vector) -> Vector: ...
+
+	def change_vector_analysis(self, date1_rasters: List[Raster], date2_rasters: List[Raster]) -> Tuple[Raster, Raster, str]: ...
+
+	def check_in_license(self, key: str) -> str: ...
+
+	def circular_variance_of_aspect(self, dem: Raster, filter_size: int = 11) -> Raster: ...
+
+	def classify_buildings_in_lidar(self, in_lidar: Lidar, building_footprints: Vector) -> Lidar: ...
+
+	def classify_lidar(self, input_lidar: Optional[Lidar], search_radius: float = 2.5, grd_threshold: float = 0.1, oto_threshold: float = 1.0, linearity_threshold: float = 0.5, planarity_threshold: float = 0.85, num_iter: int = 30, facade_threshold: float = 0.5) -> Optional[Lidar]: ...
+
+	def colourize_based_on_class(self, input_lidar: Optional[Lidar], intensity_blending_amount: float = 50.0, clr_str: str = "", use_unique_clrs_for_buildings: bool = False, search_radius: float = 2.0) -> Optional[Lidar]: ...
+
+	def colourize_based_on_point_returns(self, input_lidar: Optional[Lidar], intensity_blending_amount: float = 50.0, only_ret_colour: str = "(230,214,170)", first_ret_colour:str = "(0,140,0)", intermediate_ret_colour: str = "(255,0,255)", last_ret_colour: str = "(0,0,255)") -> Optional[Lidar]: ...
+	
+	def classify_overlap_points(self, in_lidar: Lidar, resolution: float = 1.0, overlap_criterion: str = "max scan angle", filter: bool = False) -> Lidar: ...
+
+	def clean_vector(self, input: Vector) -> Vector: ...
+
+	def clip(self, input: Vector, clip_layer: Vector) -> Vector: ...
+
+	def clip_lidar_to_polygon(self, input: Lidar, polygons: Vector) -> Lidar: ...
+
+	def clip_raster_to_polygon(self, raster: Raster, polygons: Vector, maintain_dimensions: bool = False) -> Raster: ...
+
+	def closing(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def clump(self, raster: Raster, diag: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def compactness_ratio(self, input: Vector) -> Vector: ...
+
+	def conservative_smoothing_filter(self, raster: Raster, filter_size_x: int = 3, filter_size_y: int = 3) -> Raster: ...
+
+	def construct_vector_tin(self, input_points: Vector, field_name: str = "FID", use_z: bool = False, max_triangle_edge_length: float = float('inf')) -> Vector: ...
+
+	def contours_from_points(self, input: Vector, field_name: str = "", use_z_values: bool = False, max_triangle_edge_length: float = float('inf'), contour_interval: float = 10.0, base_contour: float = 0.0, smoothing_filter_size: int = 9) -> Vector: ...
+
+	def contours_from_raster(self, raster_surface: Raster, contour_interval: float = 10.0, base_contour: float = 0.0, smoothing_filter_size: int = 9, deflection_tolerance: float = 10.0) -> Vector: ...
+
+	def convert_nodata_to_zero(self, raster: Raster) -> Raster: ...
+
+	def corner_detection(self, raster: Raster) -> Raster: ...
+
+	def correct_vignetting(self, image: Raster, principal_point: Vector, focal_length: float = 304.8, image_width: float = 228.6, n_param: float = 4.0) -> Raster: ...
+
+	def cost_allocation(self, source: Raster, backlink: Raster) -> Raster: ...
+
+	def cost_distance(self, source: Raster, cost: Raster) -> Tuple[Raster, Raster]: ...
+
+	def cost_pathway(self, destination: Raster, backlink: Raster, zero_background: bool = False) -> Raster: ...
+
+	def count_if(self, input_rasters: List[Raster], comparison_value: float) -> Raster: ...
+
+	def create_colour_composite(self, red: Raster, green: Raster, blue: Raster, opacity: Optional[Raster] = None, enhance: bool = True, treat_zeros_as_nodata: bool = False) -> Raster: ...
+
+	def create_plane(self, base_file: Raster, gradient: float, aspect: float, constant: float) -> Raster: ...
+
+	def crispness_index(self, raster: Raster, output_html_file: str) -> None: ...
+
+	def cross_tabulation(self, raster1: Raster, raster2: Raster, output_html_file: str) -> None: ...
+
+	def csv_points_to_vector(self, input_file: str, x_field_num: int = 0, y_field_num: int = 1, epsg: int = 0) -> Vector: ...
+
+	def cumulative_distribution(self, raster: Raster) -> Raster: ...
+
+	def curvedness(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def d8_flow_accum(self, raster: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False, esri_pntr: bool = False) -> Raster: ...
+
+	def d8_mass_flux(self, dem: Raster, loading: Raster, efficiency: Raster, absorption: Raster) -> Raster: ...
+
+	def d8_pointer(self, dem: Raster, esri_pointer: bool = False) -> Raster: ...
+
+	def dbscan(self, input_rasters: List[Raster], scaling_method: str = "none", search_distance: float = 1.0, min_points: int = 5) -> Raster: ...
+
+	def dem_void_filling(self, dem: Raster, fill: Raster, mean_plane_dist: int = 20, edge_treatment: str = "use DEM", weight_value: float = 2.0) -> Raster: ...
+	
+	def depth_in_sink(self, dem: Raster, zero_background: bool = False) -> Raster: ...
+
+	def depth_to_water(self, dem: Raster, streams: Optional[Vector] = None, lakes: Optional[Vector] = None) -> Raster: ...
+
+	def deviation_from_mean_elevation(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def deviation_from_regional_direction(self, input: Vector, elongation_threshold: float = 0.75) -> Vector: ...
+
+	def diff_of_gaussians_filter(self, raster: Raster, sigma1: float = 2.0, sigma2: float = 4.0) -> Raster: ...
+
+	def difference(self, input: Vector, overlay: Vector) -> Vector: ...
+
+	def difference_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def difference_from_mean_elevation(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def dinf_flow_accum(self, dem: Raster, out_type: str = "SCA", convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False) -> Raster: ...
+
+	def dinf_mass_flux(self, dem: Raster, loading: Raster, efficiency: Raster, absorption: Raster) -> Raster: ...
+
+	def dinf_pointer(self, dem: Raster) -> Raster: ...
+
+	def direct_decorrelation_stretch(self, image: Raster, achromatic_factor: float = 0.5, clip_percent: float = 1.0) -> Raster: ...
+
+	def directional_relief(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf')) -> Raster: ...
+
+	def dissolve(self, input: Vector, dissolve_field: str = "", snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
+
+	def distance_to_outlet(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def diversity_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def downslope_distance_to_stream(self, dem: Raster, streams: Raster, use_dinf: bool = False) -> Raster: ...
+
+	def downslope_flowpath_length(self, d8_pointer: Raster, watersheds: Raster, weights: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def downslope_index(self, dem: Raster, vertical_drop: float, output_type: str = "tangent") -> Raster: ...
+
+	def edge_contamination(self, dem: Raster, flow_type: str = "mfd", z_factor: float = -1.0) -> Raster: ...
+
+	def edge_density(self, dem: Raster, filter_size: int = 11, normal_diff_threshold: float = 5.0, z_factor: float = 1.0) -> Raster: ...
+
+	def edge_preserving_mean_filter(self, raster: Raster, filter_size: int = 11, threshold: float = 15.0) -> Raster: ...
+
+	def edge_proportion(self, raster: Raster) -> Tuple[Raster, str]: ...
+
+	def elev_relative_to_min_max(self, dem: Raster) -> Raster: ...
+
+	def elev_relative_to_watershed_min_max(self, dem: Raster, watersheds: Raster) -> Raster: ...
+
+	def elevation_above_pit(self, dem: Raster) -> Raster: ...
+
+	def elevation_above_stream(self, dem: Raster, streams: Raster) -> Raster: ...
+
+	def elevation_above_stream_euclidean(self, dem: Raster, streams: Raster) -> Raster: ...
+
+	def elevation_percentile(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
+
+	def eliminate_coincident_points(self, input: Vector, tolerance_dist: float) -> Vector: ...
+
+	def elongation_ratio(self, input: Vector) -> Vector: ...
+
+	def embankment_mapping(self, dem: Raster, roads_vector: Vector, search_dist: float = 2.5, min_road_width: float = 6.0, typical_embankment_width: float = 30.0, typical_embankment_max_height: float = 2.0, embankment_max_width: float = 60.0, max_upwards_increment: float = 0.05, spillout_slope: float = 4.0, remove_embankments: bool = False) -> Tuple[Raster, Optional[Raster]]: ...
+
+	def emboss_filter(self, raster: Raster, direction: str = "n", clip_amount: float = 0.0) -> Raster: ...
+
+	def erase(self, input: Vector, erase_layer: Vector) -> Vector: ...
+
+	def erase_polygon_from_lidar(self, input: Lidar, polygons: Vector) -> Lidar: ...
+
+	def erase_polygon_from_raster(self, raster: Raster, polygons: Vector) -> Raster: ...
+
+	def euclidean_allocation(self, input: Raster) -> Raster: ...
+
+	def euclidean_distance(self, input: Raster) -> Raster: ...
+
+	def evaluate_training_sites(self, input_rasters: List[Raster], training_polygons: Vector, class_field_name: str, output_html_file: str) -> None: ...
+
+	def export_table_to_csv(self, input: Vector, output_csv_file: str, headers: bool = True) -> None: ...
+
+	def exposure_towards_wind_flux(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf'), z_factor: float = 1.0) -> Raster: ...
+
+	def extend_vector_lines(self, input: Vector, distance: float, extend_direction: str = "both ends") -> Vector: ...
+
+	def extract_by_attribute(self, input: Vector, statement: str) -> Vector: ...
+
+	def extract_nodes(self, input: Vector) -> Vector: ...
+
+	def extract_raster_values_at_points(self, rasters: List[Raster], points: Vector) -> Tuple[Vector, str]: ...
+
+	def extract_streams(self, flow_accumulation: Raster, threshold: float = 0.0, zero_background: bool = False) -> Raster: ...
+
+	def extract_valleys(self, dem: Raster, variant: str = "LQ", line_thin: bool = False, filter_size: int = 5) -> Raster: ...
+
+	def farthest_channel_head(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def fast_almost_gaussian_filter(self, raster: Raster, sigma: float = 1.8) -> Raster: ...
+
+	def fd8_flow_accum(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
+
+	def fd8_pointer(self, dem: Raster) -> Raster: ...
+
+	def feature_preserving_smoothing(self, dem: Raster, filter_size: int = 11, normal_diff_threshold: float = 8.0, iterations: int = 3, max_elevation_diff: float = float('inf'), z_factor: float = 1.0) -> Raster: ...
+
+	def fetch_analysis(self, dem: Raster, azimuth: float = 0.0, height_increment: float = 0.05) -> Raster: ...
+
+	def fill_burn(self, dem: Raster, streams: Vector) -> Raster: ...
+
+	def fill_depressions(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan'), max_depth: float = float('inf')) -> Raster: ...
+
+	def fill_depressions_planchon_and_darboux(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan')) -> Raster: ...
+
+	def fill_depressions_wang_and_liu(self, dem: Raster, fix_flats: bool = True, flat_increment: float = float('nan')) -> Raster: ...
+
+	def fill_missing_data(self, dem: Raster, filter_size: int = 11, weight: float = 2.0, exclude_edge_nodata: bool = False) -> Raster: ...
+
+	def fill_pits(self, dem: Raster) -> Raster: ...
+
+	def filter_lidar(self, statement: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
+
+	def filter_lidar_by_percentile(self, input_lidar: Optional[Lidar],  percentile: float = 0.0, block_size: float = 1.0) -> Optional[Lidar]: ...
+
+	def filter_lidar_by_reference_surface(self, input_lidar: Lidar, ref_surface: Raster, query: str = "within", threshold: float = 0.0) -> Lidar: ...
+
+	def filter_lidar_classes(self, input: Lidar, exclusion_classes: List[int]) -> Lidar: ...
+
+	def filter_lidar_scan_angles(self, in_lidar: Lidar, threshold: int) -> Lidar: ...
+
+	def filter_raster_features_by_area(self, input: Raster, threshold: int, zero_background: bool = False) -> Raster: ...
+
+	def find_flightline_edge_points(self, in_lidar: Lidar) -> Lidar: ...
+
+	def find_lowest_or_highest_points(self, raster: Raster, output_type: str = "lowest") -> Vector: ...
+
+	def find_main_stem(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def find_noflow_cells(self, dem: Raster) -> Raster: ...
+
+	def find_parallel_flow(self, d8_pntr: Raster, streams: Raster) -> Raster: ...
+
+	def find_patch_edge_cells(self, raster: Raster) -> Raster: ...
+
+	def find_ridges(self, dem: Raster, line_thin: bool = True) -> Raster: ...
+
+	def fix_dangling_arcs(self, input: Vector, snap_dist: float) -> Vector: ...
+
+	def flatten_lakes(self, dem: Raster, lakes: Vector) -> Raster: ...
+
+	def flightline_overlap(self, input_lidar: Lidar, resolution: float = 1.0) -> Raster: ...
+
+	def flip_image(self, raster: Raster, direction: str = "vertical") -> Raster: ...
+
+	def flood_order(self, dem: Raster) -> Raster: ...
+
+	def flow_accum_full_workflow(self, dem: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, esri_pntr: bool = False) -> Tuple[Raster, Raster, Raster]: ...
+
+	def flow_length_diff(self, d8_pointer: Raster, esri_pointer: bool = False, log_transform: bool = False) -> Raster: ...
+
+	def gamma_correction(self, raster: Raster, gamma_value: float = 0.5) -> Raster: ...
+
+	def gaussian_contrast_stretch(self, raster: Raster, num_tones: int = 256) -> Raster: ...
+
+	def gaussian_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def gaussian_filter(self, raster: Raster, sigma: float = 0.75) -> Raster: ...
+
+	def geomorphons(self, dem: Raster, search_distance: int = 50, flatness_threshold: float = 0.0, flatness_distance: int = 0, skip_distance: int = 0, output_forms: bool = True, analyze_residuals: bool = False) -> Raster: ...
+
+	def generalize_classified_raster(self, raster: Raster, area_threshold: int = 5, method: str = "longest") -> Raster: ...
+
+	def generalize_with_similarity(self, raster: Raster, similarity_rasters: List[Raster], area_threshold: int = 5) -> Raster: ...
+
+	def generating_function(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def hack_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def heat_map(self, points: Vector, field_name: Optional[str] = None, bandwidth: float = 0.0, cell_size: float = 0.0, base_raster: Optional[Raster] = None, kernel_function: str = "quartic") -> Raster: ...
+
+	def height_above_ground(self, input: Lidar) -> Lidar: ...
+
+	def hexagonal_grid_from_raster_base(self, base: Raster, width: float, orientation: str = "h") -> Vector: ...
+
+	def hexagonal_grid_from_vector_base(self, base: Vector, width: float, orientation: str = "h") -> Vector: ...
+
+	def high_pass_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def high_pass_median_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
+
+	def highest_position(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def hillshade(self, dem: Raster, azimuth: float = 315.0, altitude: float = 30.0, z_factor: float = 1.0) -> Raster: ...
+
+	def hillslopes(self, d8_pntr: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def histogram_equalization(self, raster: Raster, num_tones: int = 256) -> Raster: ...
+
+	def histogram_matching(self, image: Raster, histogram: List[List[float]], histo_is_cumulative: bool = False) -> Raster: ...
+
+	def histogram_matching_two_images(self, image1: Raster, image2: Raster) -> Raster: ...
+
+	def hole_proportion(self, input: Vector) -> Vector: ...
+
+	def horizon_angle(self, dem: Raster, azimuth: float = 0.0, max_dist: float = float('inf')) -> Raster: ...
+
+	def horizon_area(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
+
+	def horizontal_excess_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]: ...
+
+	def horton_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def hydrologic_connectivity(self, dem: Raster, exponent: float = 1.1, convergence_threshold: float = 0.0, z_factor: float = 1.0 ) -> Tuple[Raster, Raster]: ...
+
+	def hypsometric_analysis(self, dem_rasters: List[Raster], output_html_file: str, watershed_rasters: Optional[List[Raster]] = None) -> None: ...
+
+	def hypsometrically_tinted_hillshade(self, dem: Raster, solar_altitude: float = 45.0, hillshade_weight: float = 0.5, brightness: float = 0.5, atmospheric_effects: float = 0.0, palette: WbPalette = WbPalette.Atlas, reverse_palette: bool = False, full_360_mode: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def idw_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, weight: float = 2.0, radius: float = 0.0, min_points: int = 0, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def ihs_to_rgb(self, intensity: Raster, hue: Raster, saturation: Raster) -> Tuple[Raster, Raster, Raster]: ...
+
+	def image_autocorrelation(self, rasters: List[Raster], output_html_file: str, contiguity_type: str = "bishop") -> None: ...
+
+	def image_correlation(self, rasters: List[Raster], output_html_file: str) -> None: ...
+
+	def image_correlation_neighbourhood_analysis(self, raster1: Raster, raster2: Raster, filter_size: int = 11, correlation_stat: str = "pearson") -> Tuple[Raster, Raster]: ...
+
+	def image_regression(self, independent_variable: Raster, dependent_variable: Raster, output_html_file: str, standardize_residuals: bool = False, output_scattergram: bool = False, num_samples: int = 1000) -> Raster: ...
+
+	def image_segmentation(self, input_rasters: List[Raster], dist_threshold: float = 0.5, num_steps: int = 10, area_threshold: int = 4) -> Raster: ...
+
+	def image_slider(self, left_raster: Raster, right_raster: Raster, output_html_file: str, left_palette: WbPalette = WbPalette.Grey, left_reverse_palette: bool = False, left_label: str = "",  right_palette: WbPalette = WbPalette.Grey, right_reverse_palette: bool = False, right_label: str = "", image_height: int = 600) -> None: ...
+
+	def image_stack_profile(self, images: List[Raster], points: Vector, output_html_file: str) -> None: ...
+
+	def impoundment_size_index(self, dem: Raster, max_dam_length: float, output_mean: bool = False, output_max: bool = False, output_volume: bool = False, output_area: bool = False, output_height: bool = False) -> Tuple[Optional[Raster], Optional[Raster], Optional[Raster], Optional[Raster], Optional[Raster]]: ...
+
+	def improved_ground_point_filter(self, input: Lidar, block_size = 1.0, max_building_size = 150.0, slope_threshold = 15.0, elev_threshold = 0.15) -> Lidar: ...
+
+	def individual_tree_detection(self, input_lidar: Optional[Lidar],  min_search_radius: float = 1.0, min_height: float = 0.0, max_search_radius: Optional[float] = None, max_height: Optional[float] = None, only_use_veg: bool = False) -> Optional[Vector]: ...
+
+	def insert_dams(self, dem: Raster, dam_points: Vector, dam_length: float) -> Raster: ...
+
+	def isobasins(self, dem: Raster, target_size: float, connections: bool = False, csv_file: str = "" ) -> Raster: ...
+
+	def integral_image_transform(self, raster: Raster) -> Raster: ...
+
+	def intersect(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
+
+	def inverse_pca(self, rasters: List[Raster], pca_report_file: str) -> List[Raster]: ...
+
+	def jenson_snap_pour_points(self, pour_pts: Vector, streams: Raster, snap_dist: float = 0.0) -> Vector: ...
+
+	def join_tables(self, primary_vector: Vector, primary_key_field: str, foreign_vector: Vector, foreign_key_field: str, import_field: str = "") -> None: ...
+
+	def k_means_clustering(self, input_rasters: List[Raster], output_html_file: str = "", num_clusters: int = 5, max_iterations: int = 10, percent_changed_threshold: float = 2.0, initialization_mode: str = "diagonal", min_class_size: int = 10) -> Raster: ...
+
+	def k_nearest_mean_filter(self, raster: Raster, filter_size_x: int = 3, filter_size_y: int = 3, k: int = 5) -> Raster: ...
+
+	def kappa_index(self, class_raster: Raster, reference_raster: Raster, output_html_file: str = "") -> None: ...
+
+	def knn_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", k: int = 5, test_proportion: float = 0.2, use_clipping: bool = False, create_output: bool = False) -> Optional[Raster]: ...
+
+	def knn_regression(self, input_rasters: List[Raster], training_data: Vector, field_name: str, scaling_method: str = "none", k: int = 5, distance_weighting: bool = False, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
+
+	def ks_normality_test(self, raster: Raster, output_html_file: str, num_samples: int) -> None: ...
+
+	def laplacian_filter(self, raster: Raster, variant: str = "3x3(1)", clip_amount: float = 0.0) -> Raster: ...
+
+	def laplacian_of_gaussians_filter(self, raster: Raster, sigma: float = 0.75) -> Raster: ...
+
+	def las_to_ascii(self, input_lidar: Optional[Lidar]) -> None: ...
+
+	def las_to_shapefile(self, input_lidar: Optional[Lidar], output_multipoint: bool = False) -> Vector: ...
+
+	def layer_footprint_raster(self, input: Raster) -> Vector: ...
+
+	def layer_footprint_vector(self, input: Vector) -> Vector: ...
+
+	def lee_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sigma: float = 10.0, m_value: float = 5.0) -> Raster: ...
+
+	def length_of_upstream_channels(self, d8_pointer: Raster, streams_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def license_type(self) -> LicenseType: ...
+
+	def lidar_block_maximum(self, input_lidar: Optional[Lidar], cell_size: float = 1.0) -> Raster: ...
+
+	def lidar_block_minimum(self, input_lidar: Optional[Lidar], cell_size: float = 1.0) -> Raster: ...
+
+	def lidar_classify_subset(self, base_lidar: Lidar, subset_lidar: Lidar, subset_class_value: int, nonsubset_class_value: int) -> Lidar: ...
+
+	def lidar_colourize(self, in_lidar: Lidar, in_image: Raster) -> Lidar: ...
+
+	def lidar_construct_vector_tin(self, input_lidar: Optional[Lidar], returns_included: str = "all", excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Vector: ...
+
+	def lidar_contour(self, input_lidar: Optional[Lidar], contour_interval: float = 10.0, base_contour: float = 0.0, smooth: int = 5, interpolation_parameter: str = "elevation", returns_included: str = "all",  excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), tile_overlap: float = 0.0, max_triangle_edge_length: float = float('inf')) -> Optional[Vector]: ...
+
+	def lidar_digital_surface_model(self, input_lidar: Optional[Lidar], cell_size: float = 1.0, search_radius: float = 0.5, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Raster: ...
+
+	def lidar_eigenvalue_features(self, input_lidar: Optional[Lidar], num_neighbours: Optional[int], search_radius: Optional[float]) -> None: ...
+
+	def lidar_elevation_slice(self, input: Lidar, minz: float = float('-inf'), maxz: float = float('inf'), classify: bool = False, in_class_value: int = 2, out_class_value: int = 1) -> Lidar: ...
+
+	def lidar_ground_point_filter(self, input_lidar: Optional[Lidar], search_radius: float = 2.0, min_neighbours: int = 0, slope_threshold: float = 45.0, height_threshold: float = 1.0, classify: bool = False, slope_norm: bool = True, height_above_ground: bool = False) -> Lidar: ...
+
+	def lidar_hex_bin(self, input_lidar: Lidar, width: float, orientation: str = "h") -> Vector: ...
+
+	def lidar_hillshade(self, input: Lidar, search_radius: float = -1.0, azimuth: float = 315.0, altitude: float = 30.0) -> Lidar: ...
+
+	def lidar_histogram(self, input_lidar: Lidar, output_html_file: str, parameter: str = "elevation", clip_percent: float = 1.0) -> None: ...
+
+	def lidar_idw_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation",  returns_included: str = "all", cell_size: float = 1.0,  idw_weight: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
+
+	def lidar_info(self, input_lidar: Lidar, output_html_file: Optional[str], show_point_density: bool = True, show_vlrs: bool = True, show_geokeys: bool = True) -> str: ...
+
+	def lidar_join(self, inputs: List[Lidar]) -> Lidar: ...
+
+	def lidar_kappa(self, input_lidar1: Lidar, input_lidar2: Lidar, output_html_file: str, cell_size: float = 1.0, output_class_accuracy: bool = False) -> Raster: ...
+
+	def lidar_nearest_neighbour_gridding(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
+
+	def lidar_point_density(self, input_lidar: Optional[Lidar], returns_included: str = "all", cell_size: float = 1.0, search_radius: float = 2.5, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Raster: ...
+
+	def lidar_point_return_analysis(self, input: Lidar, create_output: bool = False) -> Optional[Lidar]: ...
+
+	def lidar_point_stats(self, input_lidar: Optional[Lidar], cell_size: float = 1.0, num_points: bool = False, num_pulses: bool = False, avg_points_per_pulse: bool = False, z_range: bool = False, intensity_range: bool = False, predominant_class: bool = False) : ...
+
+	def lidar_radial_basis_function_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, num_points: int = 15, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), func_type: str = "ThinPlateSpline", poly_order: str = "none", weight: float = 0.1) -> Raster: ...
+
+	def lidar_ransac_planes(self, in_lidar: Lidar, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, classify: bool = False, only_last_returns: bool = False) -> Lidar: ...
+
+	def lidar_remove_outliers(self, input: Lidar, search_radius: float = 2.0, elev_diff: float = 50.0, use_median: bool = False, classify: bool = False) -> Lidar: ...
+
+	def lidar_rooftop_analysis(self, lidar_inputs: List[Lidar], building_footprints: Vector, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, norm_diff_threshold: float = 2.0, azimuth: float = 180.0, altitude: float = 30.0) -> Vector: ...
+
+	def lidar_segmentation(self, in_lidar: Lidar, search_radius: float = 2.0, num_iterations: int = 50, num_samples: int = 10, inlier_threshold: float = 0.15, acceptable_model_size: int = 30, max_planar_slope: float = 75.0, norm_diff_threshold: float = 2.0, max_z_diff: float = 1.0, classes: bool = False, ground: bool = False) -> Lidar: ...
+
+	def lidar_segmentation_based_filter(self, in_lidar: Lidar, search_radius: float = 5.0, norm_diff_threshold: float = 2.0, max_z_diff: float = 1.0, classify_points: bool = False) -> Lidar: ...
+
+	def lidar_shift(self, input: Lidar, x_shift: float = 0.0, y_shift: float = 0.0, z_shift: float = 0.0) -> Lidar: ...
+
+	def lidar_sibson_interpolation(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", resolution: float = 1.0, returns_included: str = "all", excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf')) -> Optional[Raster]: ...
+
+	def lidar_thin(self, input: Lidar, resolution: float = 1.0, selection_method: str = "first", save_filtered: bool = False) -> Tuple[Lidar, Optional[Lidar]]: ...
+
+	def lidar_thin_high_density(self, input: Lidar, density: float, resolution: float = 1.0, save_filtered: bool = False) -> Tuple[Lidar, Optional[Lidar]]: ...
+
+	def lidar_tile(self, input_lidar: Lidar, tile_width: float = 1000.0, tile_height: float = 1000.0, origin_x: float = 0.0, origin_y: float = 0.0, min_points_in_tile: int = 2, output_laz_format: bool = True) -> None: ...
+
+	def lidar_tile_footprint(self, input_lidar: Optional[Lidar], output_hulls: bool = False) -> Vector: ...
+
+	def lidar_tin_gridding(self, input_lidar: Optional[Lidar], interpolation_parameter: str = "elevation", returns_included: str = "all", cell_size: float = 1.0, excluded_classes: Optional[List[int]] = None, min_elev: float = float('-inf'), max_elev: float = float('inf'), max_triangle_edge_length: float = float('inf')) -> Raster: ...
+
+	def lidar_tophat_transform(self, input: Lidar, search_radius: float) -> Lidar: ...
+
+	def line_detection_filter(self, raster: Raster, variant: str = "vertical", abs_values: bool = False, clip_tails: float = 0.0) -> Raster: ...
+
+	def line_intersections(self, input1: Vector, input2: Vector) -> Vector: ...
+
+	def line_thinning(self, raster: Raster) -> Raster: ...
+
+	def linearity_index(self, input: Vector) -> Vector: ...
+
+	def lines_to_polygons(self, input: Vector) -> Vector: ...
+
+	def list_unique_values(self, input: Vector, field_name: str) -> List[Tuple[str, int]]: ...
+
+	def list_unique_values_raster(self, raster: Raster) -> str: ...
+
+	def local_hypsometric_analysis(self, dem: Raster, min_scale: int = 4, step_size: int = 1,  num_steps: int = 10, step_nonlinearity: float = 1.0) -> Tuple[Raster, Raster]: ...
+
+	def logistic_regression(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
+
+	def long_profile(self, d8_pointer: Raster, streams_raster: Raster, dem: Raster, output_html_file: str, esri_pointer: bool = False) -> None: ...
+
+	def long_profile_from_points(self, d8_pointer: Raster, points: Vector, dem: Raster, output_html_file: str, esri_pointer: bool = False) -> None: ...
+
+	def longest_flowpath(self, dem: Raster, basins: Raster) -> Vector: ...
+
+	def lowest_position(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def low_points_on_headwater_divides(self, dem: Raster, streams: Raster) -> Vector: ...
+
+	def majority_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def map_off_terrain_objects(self, dem: Raster, max_slope: float = float('inf'), min_feature_size: int = 0) -> Raster: ...
+
+	def max_absolute_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def max_anisotropy_dev(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
+
+	def max_anisotropy_dev_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
+
+	def max_branch_length(self, dem: Raster, log_transform: bool = False) -> Raster: ...
+
+	def max_difference_from_mean(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
+
+	def max_downslope_elev_change(self, raster: Raster) -> Raster: ...
+
+	def max_elevation_dev_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
+
+	def max_elevation_deviation(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
+
+	def max_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def max_upslope_elev_change(self, raster: Raster) -> Raster: ...
+
+	def max_upslope_flowpath_length(self, dem: Raster) -> Raster: ...
+
+	def max_upslope_value(self, dem: Raster, values_raster: Raster) -> Raster: ...
+
+	def maximal_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def maximum_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def mdinf_flow_accum(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
+
+	def mean_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def mean_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def median_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
+
+	def medoid(self, input: Vector) -> Vector: ...
+
+	def merge_line_segments(self, input: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
+
+	def merge_table_with_csv(self, primary_vector: Vector, primary_key_field: str, foreign_csv_filename: str, foreign_key_field: str, import_field: str = "") -> None: ...
+
+	def merge_vectors(self, input_vectors: List[Vector]) -> Vector: ...
+
+	def min_absolute_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def min_dist_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, dist_threshold: float = float('inf')) -> Raster: ...
+
+	def min_downslope_elev_change(self, raster: Raster) -> Raster: ...
+
+	def min_max_contrast_stretch(self, raster: Raster, min_val: float, max_val: float, num_tones: int = 256) -> Raster: ...
+
+	def min_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def minimal_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def minimum_bounding_box(self, input: Vector, min_criteria: str = "area", individual_feature_hulls: bool = True) -> Vector: ...
+
+	def minimum_bounding_circle(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
+
+	def minimum_bounding_envelope(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
+
+	def minimum_convex_hull(self, input: Vector, individual_feature_hulls: bool = True) -> Vector: ...
+
+	def minimum_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def modified_k_means_clustering(self, input_rasters: List[Raster], output_html_file: str = "", num_start_clusters: int = 1000, merge_distance: float = 1.0, max_iterations: int = 10, percent_changed_threshold: float = 2.0) -> Raster: ...
+
+	def modify_lidar(self, statement: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
+
+	def modify_nodata_value(self, input: Raster, new_value: float = -32768.0) : ...
+
+	def mosaic(self, images: List[Raster], resampling_method: str = "cc") -> Raster: ...
+
+	def mosaic_with_feathering(self, image1: Raster, image2: Raster, resampling_method: str = "cc", distance_weight: float = 4.0) -> Raster: ...
+
+	def multidirectional_hillshade(self, dem: Raster, altitude: float = 30.0, z_factor: float = 1.0, full_360_mode: bool = False) -> Raster: ...
+
+	def multipart_to_singlepart(self, input: Vector, exclude_holes: bool = False) -> Vector: ...
+
+	def multiply_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def multiscale_curvatures(self, dem: Raster, curv_type: str = 'profile', min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0, log_transform: bool = True, standardize: bool = False) -> Tuple[Raster, Raster]: ...
+
+	def multiscale_elevation_percentile(self, dem: Raster, num_significant_digits: int = 3, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0) -> Tuple[Raster, Raster]: ...
+
+	def multiscale_roughness(self, dem: Raster, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> Tuple[Raster, Raster]: ...
+
+	def multiscale_roughness_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 1, max_scale: int = 100, step_size: int = 1) -> None: ...
+
+	def multiscale_std_dev_normals(self, dem: Raster, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0, html_signature_file: str = "") -> Tuple[Raster, Raster]: ...
+
+	def multiscale_std_dev_normals_signature(self, dem: Raster, points: Vector, output_html_file: str, min_scale: int = 4, step_size: int = 1, num_steps: int = 10, step_nonlinearity: float = 1.0) -> None: ...
+
+	def multiscale_topographic_position_image(self, local: Raster, meso: Raster, broad: Raster, hillshade: Optional[Raster] = None, lightness: float = 1.2) -> Raster: ...
+
+	def narrowness_index(self, raster: Raster) -> Raster: ...
+
+	def natural_neighbour_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, clip_to_hull: bool = True) -> Raster: ...
+
+	def nearest_neighbour_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, max_dist: float = float('inf')) -> Raster: ...
+
+	def new_raster_from_base_raster(self, base: Raster, out_val: float = float('nan'), data_type: str = "float") -> Raster: ...
+
+	def new_raster_from_base_vector(self, base: Vector, cell_size: float, out_val: float = float('nan'), data_type: str = "float") -> Raster: ...
+
+	def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster: ...
+
+	def normal_vectors(self, input: Lidar, search_radius: float = -1.0) -> Lidar: ...
+
+	def normalized_difference_index(self, nir_image: Raster, red_image: Raster, clip_percent: float = 0.0, correction_value: float = 0.0) -> Raster: ...
+
+	def normalize_lidar(self, input_lidar: Lidar, dtm: Raster) -> Lidar: ...
+
+	def num_downslope_neighbours(self, dem: Raster) -> Raster: ...
+
+	def num_inflowing_neighbours(self, dem: Raster) -> Raster: ...
+
+	def olympic_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def opening(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def openness(self, dem: Raster, dist: int = 20) -> Tuple[Raster, Raster]: ...
+
+	def otsu_thresholding(self, raster: Raster) -> Raster: ...
+
+	def paired_sample_t_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
+
+	def panchromatic_sharpening(self, pan: Raster, colour_composite: Raster, red: Raster, green: Raster, blue: Raster, fusion_method: str = "brovey") -> Raster: ...
+
+	def parallelepiped_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str) -> Raster: ...
+
+	def patch_orientation(self, input: Vector) -> Vector: ...
+
+	def pennock_landform_classification(self, dem: Raster, slope_threshold: float = 3.0, prof_curv_threshold: float = 0.1, plan_curv_threshold: float = 0.0, z_factor: float = 1.0) -> Tuple[Raster, str]: ...
+
+	def percent_elev_range(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def percent_equal_to(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
+
+	def percent_greater_than(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
+
+	def percent_less_than(self, input_rasters: List[Raster], comparison: Raster) -> Raster: ...
+
+	def percentage_contrast_stretch(self, raster: Raster, clip: float = 1.0, tail: str = "both", num_tones: int = 256) -> Raster: ...
+
+	def percentile_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, sig_digits: int = 2) -> Raster: ...
+
+	def perimeter_area_ratio(self, input: Vector) -> Vector: ...
+
+	def pick_from_list(self, input_rasters: List[Raster], pos_input: Raster) -> Raster: ...
+
+	def piecewise_contrast_stretch(self, raster: Raster, transformation_statement: str, num_greytones: float = 1024.0) -> Raster: ...
+
+	def phi_coefficient(self, raster1: Raster, raster2: Raster, output_html_file: str) -> None: ...
+
+	def plan_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def polygon_area(self, input: Vector) -> Vector: ...
+
+	def polygon_long_axis(self, input: Vector) -> Vector: ...
+
+	def polygon_perimeter(self, input: Vector) -> Vector: ...
+
+	def polygon_short_axis(self, input: Vector) -> Vector: ...
+
+	def polygonize(self, input_layers: List[Vector]) -> Vector: ...
+
+	def polygons_to_lines(self, input: Vector) -> Vector: ...
+
+	def prewitt_filter(self, raster: Raster, clip_tails: float = 0.0) -> Raster: ...
+
+	def principal_component_analysis(self, rasters: List[Raster], output_html_file: str, num_components: int = 2, standardized: bool = False) -> List[Raster]: ...
+
+	def print_geotiff_tags(self, file_name: str) : ...
+
+	def profile(self, lines_vector: Vector, surface: Raster, output_html_file: str) -> None: ...
+
+	def profile_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def prune_vector_streams(self, streams: Vector, dem: Raster, threshold: float, snap_distance: float = 0.001) -> Vector: ...
+
+	def qin_flow_accumulation(self, dem: Raster, out_type: str = "SCA", exponent: float = 10.0, max_slope: float = 45.0, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
+
+	def quantiles(self, raster: Raster, num_quantiles: int = 5) -> Raster: ...
+
+	def quinn_flow_accumulation(self, dem: Raster, out_type: str = "SCA", exponent: float = 1.1, convergence_threshold: float = float('inf'), log_transform: bool = False, clip: bool = False) -> Raster: ...
+
+	def radial_basis_function_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, radius: float = 0.0, min_points: int = 0, cell_size: float = 0.0, base_raster: Optional[Raster] = None, func_type: str = "ThinPlateSpline", poly_order: str = "none", weight: float = 0.1) -> Raster: ...
+
+	def radius_of_gyration(self, raster: Raster) -> Tuple[Raster, str]: ...
+
+	def raise_walls(self, dem: Raster, walls: Vector, breach_lines: Vector, wall_height: float = 100.0) -> Raster: ...
+
+	def random_field(self, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def random_forest_classification_fit(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, split_criterion: str = "Gini", n_trees: int = 200,  min_samples_leaf: int = 1, min_samples_split: int = 2, test_proportion: float = 0.2) -> List[int]: ...
+
+	def random_forest_classification_predict(self, input_rasters: List[Raster], model_bytes: List[int]) -> Raster: ...
+
+	def random_forest_regression_fit(self, input_rasters: List[Raster], training_data: Vector, field_name: str, n_trees: int = 200,  min_samples_leaf: int = 1, min_samples_split: int = 2, test_proportion: float = 0.2) -> List[int]: ...
+
+	def random_forest_regression_predict(self, input_rasters: List[Raster], model_bytes: List[int]) -> Raster: ...
+
+	def random_sample(self, base_raster: Optional[Raster] = None, num_samples: int = 1000) -> Raster: ...
+
+	def range_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def raster_area(self, raster: Raster, units: str = "map units", zero_background: bool = False) -> Tuple[Raster, str]: ...
+
+	def raster_calculator(self, expression: str, input_rasters: List[Raster]) -> Raster: ...
+
+	def raster_cell_assignment(self, raster: Raster, what_to_assign: str = "column") -> Raster: ...
+
+	def raster_histogram(self, raster: Raster, output_html_file: str, num_bins: Optional[int] = None) -> None: ...
+
+	def raster_perimeter(self, raster: Raster, units: str = "map units", zero_background: bool = False) -> Tuple[Raster, str]: ...
+
+	def raster_streams_to_vector(self, streams: Raster, d8_pointer: Raster, esri_pointer: bool = False, all_vertices: bool = False) -> Vector: ...
+
+	def raster_summary_stats(self, input: Raster) -> str: ...
+
+	def raster_to_vector_lines(self, raster: Raster) -> Vector: ...
+
+	def raster_to_vector_points(self, raster: Raster) -> Vector: ...
+
+	def raster_to_vector_polygons(self, raster: Raster) -> Vector: ...
+
+	def rasterize_streams(self, streams: Vector, base_raster: Optional[Raster] = None, zero_background: bool = False, use_feature_id: bool = False) -> Raster: ...
+
+	def reciprocal(self, raster: Raster) -> Raster: ...
+
+	def reclass(self, raster: Raster, reclass_values: List[List[float]], assign_mode: bool = False) -> Raster: ...
+
+	def reclass_equal_interval(self, raster: Raster, interval_size: float, start_value: float = float('-inf'), end_value: float = float('inf')) -> Raster: ...
+
+	def reconcile_multiple_headers(self, input: Vector, region_field_name: str, yield_field_name: str, radius: float, min_yield: float = float('-inf'),  max_yield: float = float('inf'), mean_tonnage: float = float('-inf')) -> Vector: ...
+
+	def recover_flightline_info(self, input: Lidar, max_time_diff: float = 5.0, pt_src_id: bool = False, user_data: bool = False, rgb: bool = False) -> Lidar: ...
+
+	def recreate_pass_lines(self, input: Vector, yield_field_name: str, max_change_in_heading: float = 25.0, ignore_zeros: bool = False) -> Tuple[Vector, Vector]: ...
+
+	def rectangular_grid_from_raster_base(self, base: Raster, width: float, height: float, x_origin: float = 0.0, y_origin: float = 0.0) -> Vector: ...
+
+	def rectangular_grid_from_vector_base(self, base: Vector, width: float, height: float, x_origin: float = 0.0, y_origin: float = 0.0) -> Vector: ...
+
+	def reinitialize_attribute_table(self, input: Vector) -> None: ...
+
+	def related_circumscribing_circle(self, input: Vector) -> Vector: ...
+
+	def relative_aspect(self, dem: Raster, azimuth: float = 0.0, z_factor: float = 1.0) -> Raster: ...
+
+	def relative_stream_power_index(self, specific_catchment_area: Raster, slope: Raster, exponent: float = 1.0) -> Raster: ...
+
+	def relative_topographic_position(self, dem: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def remove_duplicates(self, input: Lidar, include_z: bool = False) -> Lidar: ...
+
+	def remove_field_edge_points(self, input: Vector, radius: float,  max_change_in_heading: float = 25.0, flag_edges: bool = False) -> Vector: ...
+
+	def remove_off_terrain_objects(self, dem: Raster, filter_size: int = 11, slope_threshold: float = 15.0) -> Raster: ...
+
+	def remove_polygon_holes(self, input: Vector) -> Vector: ...
+
+	def remove_raster_polygon_holes(self, input: Raster, threshold_size: int = sys.maxsize, use_diagonals: bool = False) -> Raster: ...
+
+	def remove_short_streams(self, d8_pntr: Raster, streams_raster: Raster, min_length: float = 0.0, esri_pntr: bool = False) -> Raster: ...
+
+	def remove_spurs(self, raster: Raster, max_iterations: int = 10) -> Raster: ...
+
+	def repair_stream_vector_topology(self, input: Vector, snap_dist: float) -> Vector: ...
+
+	def resample(self, input_rasters: List[Raster], cell_size: float = 0.0, base_raster: Optional[Raster] = None, method: str = "cc") -> Raster: ...
+
+	def rescale_value_range(self, raster: Raster, out_min_val: float, out_max_val: float, clip_min: float = float('inf'), clip_max: float = float('-inf')) -> Raster: ...
+
+	def rgb_to_ihs(self, red: Optional[Raster] = None, green: Optional[Raster] = None, blue: Optional[Raster] = None, composite: Optional[Raster] = None) -> Tuple[Raster, Raster, Raster]: ...
+
+	def rho8_flow_accum(self, raster: Raster, out_type: str = "SCA", log_transform: bool = False, clip: bool = False, input_is_pointer: bool = False, esri_pntr: bool = False) -> Raster: ...
+
+	def rho8_pointer(self, dem: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]: ...
+
+	def ring_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def river_centerlines(self, raster: Raster, min_length: int = 3, search_radius: int = 9) -> Vector: ...
+
+	def roberts_cross_filter(self, raster: Raster, clip_amount: float = 0.0) -> Raster: ...
+
+	def root_mean_square_error(self, input: Raster, reference: Raster) -> str: ...
+
+	def rotor(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def ruggedness_index(self, input: Raster) -> Raster: ...
+
+	def scharr_filter(self, raster: Raster, clip_tails: float = 0.0) -> Raster: ...
+
+	def sediment_transport_index(self, specific_catchment_area: Raster, slope: Raster, sca_exponent: float = 0.4, slope_exponent: float = 1.3) -> Raster: ...
+
+	def select_tiles_by_polygon(self, input_directory: str, output_directory: str, polygons: Vector) -> None: ...
+
+	def set_nodata_value(self, raster: Raster, back_value: float = 0.0) -> Raster: ...
+
+	def shadow_animation(self, dem: Raster, output_html_file: str,  palette: WbPalette = WbPalette.Soft, max_dist: float = float('inf'), date: str = "21/06/2021", time_interval: int = 30, location: str = "43.5448/-80.2482/-4", image_height: int = 600, delay: int = 250, label: str = "") -> None: ...
+
+	def shadow_image(self, dem: Raster, palette: WbPalette = WbPalette.Soft, max_dist: float = float('inf'), date: str = "21/06/2021", time: str = "13:00", location: str = "43.5448/-80.2482/-4") -> Raster: ...
+
+	def shape_complexity_index_raster(self, raster: Raster) -> Raster: ...
+
+	def shape_complexity_index_vector(self, input: Vector) -> Vector: ...
+
+	def shape_index(self, dem: Raster, z_factor: float = 1.0) -> Raster: ...
+
+	def shreve_stream_magnitude(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster: ...
+
+	def sigmoidal_contrast_stretch(self, raster: Raster, cutoff: float = 0.0, gain: float = 1.0, num_tones: int = 256) -> Raster: ...
+
+	def singlepart_to_multipart(self, input: Vector, field_name: str) -> Vector: ...
+
+	def sink(self, dem: Raster, zero_background: bool = False) -> Raster: ...
+
+	def skyline_analysis(self, dem: Raster, points: Vector, output_html_file: str, max_dist: float = float('inf'), observer_hgt_offset: float = 0.0, output_as_polygons: bool = True, az_fraction: float = 1.0) -> Vector: ...
+
+	def sky_view_factor(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), observer_hgt_offset: float = 0.05) -> Raster: ...
+
+	def slope(self, dem: Raster, units: str = "degrees", z_factor: float = 1.0) -> Raster: ...
+
+	def slope_vs_aspect_plot(self, dem: Raster, output_html_file: str, aspect_bin_size: float = 2.0, min_slope: float = 0.1, z_factor: float = 1.0) -> None: ...
+
+	def slope_vs_elev_plot(self, dem_rasters: List[Raster], output_html_file: str, watershed_rasters: List[Raster]) -> None: ...
+
+	def smooth_vectors(self, input: Vector, filter_size: int = 3) -> Vector: ...
+
+	def smooth_vegetation_residual(self, dem: Raster, max_scale: int = 1, dev_threshold: float = 1.0, scale_threshold: int = 5) -> Raster: ...
+
+	def snap_pour_points(self, pour_pts: Vector, flow_accum: Raster, snap_dist: float = 0.0) -> Vector: ...
+
+	def sobel_filter(self, raster: Raster, variant: str = "3x3", clip_tails: float = 0.0) -> Raster: ...
+
+	def sort_lidar(self, sort_criteria: str, input_lidar: Optional[Lidar]) -> Optional[Lidar]: ...
+
+	def spherical_std_dev_of_normals(self, dem: Raster, filter_size: int = 11) -> Raster: ...
+
+	def split_colour_composite(self, composite_image: Raster) -> Tuple[Raster, Raster, Raster]: ...
+
+	def split_lidar(self, split_criterion: str, input_lidar: Optional[Lidar], interval: float = 5.0, min_pts: int = 5) -> None: ...
+
+	def split_vector_lines(self, input: Vector, segment_length: float) -> Vector: ...
+
+	def split_with_lines(self, input: Vector, split_vector: Vector) -> Vector: ...
+
+	def standard_deviation_contrast_stretch(self, raster: Raster, clip: float = 2.0, num_tones: int = 256) -> Raster: ...
+
+	def standard_deviation_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def standard_deviation_of_slope(self, dem: Raster, filter_size: int = 11, z_factor: float = 1.0) -> Raster: ...
+
+	def standard_deviation_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def stochastic_depression_analysis(self, dem: Raster, rmse: float, range: float, iterations: int = 100) -> Raster: ...
+
+	def strahler_order_basins(self, d8_pointer: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def strahler_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def stream_link_class(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def stream_link_identifier(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def stream_link_length(self, d8_pointer: Raster, streams_id_raster: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def stream_link_slope(self, d8_pointer: Raster, streams_id_raster: Raster, dem: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def stream_slope_continuous(self, d8_pointer: Raster, streams_raster: Raster, dem: Raster, esri_pointer: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def subbasins(self, d8_pntr: Raster, streams: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def sum_overlay(self, input_rasters: List[Raster]) -> Raster: ...
+
+	def surface_area_ratio(self, dem: Raster) -> Raster: ...
+
+	def svm_classification(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", c_value: float = 50.0, kernel_gamma: float = 0.5, tolerance: float = 0.1, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
+
+	def svm_regression(self, input_rasters: List[Raster], training_data: Vector, class_field_name: str, scaling_method: str = "none", c_value: float = 50.0, epsilon_value: float = 10.0, kernel_gamma: float = 0.5, test_proportion: float = 0.2, create_output: bool = False) -> Optional[Raster]: ...
+
+	def symmetrical_difference(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
+
+	def tangential_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def thicken_raster_line(self, raster: Raster) -> Raster: ...
+
+	def time_in_daylight(self, dem: Raster, az_fraction: float = 5.0, max_dist: float = float('inf'), latitude: float = 0.0, longitude: float = 0.0, utc_offset_str: str = "UTC+00:00", start_day: int = 1, end_day: int = 365, start_time: str = "sunrise", end_time: str = "sunset") -> Raster: ...
+
+	def tin_interpolation(self, points: Vector, field_name: str = "FID", use_z: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None, max_triangle_edge_length: float = float('inf')) -> Raster: ...
+
+	def tophat_transform(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11, variant: str = "white") -> Raster: ...
+
+	def topological_breach_burn(self, streams: Vector, dem: Raster, snap_distance: float = 0.001) -> Tuple[Raster, Raster, Raster, Raster]: ...
+
+	def topological_stream_order(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def topographic_hachures(self, dem: Raster, contour_interval: float = 10.0, base_contour: float = 0.0, deflection_tolerance: float = 10.0, filter_size: int = 9, separation: float = 2.0, distmin: float = 0.5, distmax: float = 2.0, discretization: float = 0.5, turnmax: float = 45.0, slopemin: float = 0.5, depth: int = 16) -> Vector: ...
+	    
+	def topo_render(self, dem: Raster, palette: WbPalette = WbPalette.Soft, reverse_palette: bool = False,  azimuth: float = 315.0, altitude: float = 30.0, clipping_polygon: Optional[Vector] = None, background_hgt_offset: float = 10.0, background_clr: Tuple[int, int, int, int] = (255, 255, 255, 255), attenuation_parameter: float = 0.3,  ambient_light: float = 0.2, z_factor: float = 1.0) -> Raster: ...
+
+	def topographic_position_animation(self, dem: Raster, output_html_file: str = "topo_pos.html", palette: WbPalette = WbPalette.Soft,  min_scale: int = 1, num_steps: int = 1, step_nonlinearity: float = 1.0, image_height: int = 600, delay: int = 250, label: str = "", use_dev_max: bool = False) -> None: ...
+
+	def total_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def total_filter(self, raster: Raster, filter_size_x: int = 11, filter_size_y: int = 11) -> Raster: ...
+
+	def trace_downslope_flowpaths(self, seed_points: Vector, d8_pointer: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def travelling_salesman_problem(self, input: Vector, duration: int = 60) -> Vector: ...
+
+	def trend_surface(self, raster: Raster, output_html_file: str, polynomial_order: int = 1) -> Raster: ...
+
+	def trend_surface_vector_points(self, input: Vector, cell_size: float, output_html_file: str, field_name: str = "FID", polynomial_order: int = 1) -> Raster: ...
+
+	def tributary_identifier(self, d8_pntr: Raster, streams_raster: Raster, esri_pntr: bool = False, zero_background: bool = False) -> Raster: ...
+
+	def turning_bands_simulation(self, base_raster: Optional[Raster] = None, range: float = 1.0, iterations: int = 1000) -> Raster: ...
+
+	def two_sample_ks_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
+
+	def union(self, input: Vector, overlay: Vector, snap_tolerance: float = 2.220446049250313e-16) -> Vector: ...
+
+	def unnest_basins(self, d8_pointer: Raster, pour_points: Vector, esri_pntr: bool = False) -> List[Raster]: ...
+
+	def unsharp_masking(self, raster: Raster, sigma: float = 0.75, amount: float = 100.0, threshold: float = 0.0) -> Raster: ...
+
+	def unsphericity(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def update_nodata_cells(self, input1: Raster, input2: Raster) -> Raster: ...
+
+	def upslope_depression_storage(self, dem: Raster) -> Raster: ...
+
+	def user_defined_weights_filter(self, raster: Raster, weights: List[List[float]], kernel_center: str = "center", normalize_weights: bool = False) -> Raster: ...
+
+	def vector_hex_binning(self, vector_points: Vector, width: float, orientation: str = "horizontal") -> Vector: ...
+
+	def vector_lines_to_raster(self, input: Vector, field_name: str = "FID", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def vector_points_to_raster(self, input: Vector, field_name: str = "FID", assign_op: str = "last", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def vector_polygons_to_raster(self, input: Vector, field_name: str = "FID", zero_background: bool = False, cell_size: float = 0.0, base_raster: Optional[Raster] = None) -> Raster: ...
+
+	def vertical_excess_curvature(self, dem: Raster, log_transform: bool = False, z_factor: float = 1.0) -> Raster: ...
+
+	def vector_stream_network_analysis(self, streams: Vector, dem: Raster, max_ridge_cutting_height: float = 10.0, snap_distance: float = 0.001) -> Tuple[Vector, Vector, Vector, Vector]: ...
+
+	def viewshed(self, dem: Raster, station_points: Vector, station_height: float = 2.0) -> Raster: ...
+
+	def visibility_index(self, dem: Raster, station_height: float = 2.0, resolution_factor: int = 8) -> Raster: ...
+
+	def voronoi_diagram(self, input_points: Vector) -> Vector: ...
+
+	def watershed(self, d8_pointer: Raster, pour_points: Vector, esri_pntr: bool = False) -> Raster: ...
+
+	def watershed_from_raster_pour_points(self, d8_pointer: Raster, pour_points: Raster, esri_pntr: bool = False) -> Raster: ...
+
+	def weighted_overlay(self, factors: List[Raster], weights: List[float], cost: Optional[List[Raster]] = None, constraints: Optional[List[Raster]] = None, scale_max: float = 1.0) -> Raster: ...
+
+	def weighted_sum(self, input_rasters: List[Raster], weights: List[float]) -> Raster: ...
+
+	def wetness_index(self, specific_catchment_area: Raster, slope: Raster) -> Raster: ...
+
+	def wilcoxon_signed_rank_test(self, raster1: Raster, raster2: Raster, output_html_file: str, num_samples: int) -> None: ...
+
+	def write_function_memory_insertion(self, image1: Raster, image2: Raster, image3: Raster) -> Raster: ...
+
+	def yield_filter(self, input: Vector, yield_field_name: str, pass_field_name: str,  swath_width: float = 6.096, z_score_threshold: float = 2.5, min_yield: float = 0.0, max_yield: float = float('inf')) -> Vector: ...
+
+	def yield_map(self, input: Vector, pass_field_name: str, swath_width: float = 6.096, max_change_in_heading: float = 25.0) -> Vector: ...
+
+	def yield_normalization(self, input: Vector, yield_field_name: str,  radius: float, standardize: bool = False, min_yield: float = 0.0, max_yield: float = float('inf')) -> Vector: ...
+
+	def z_scores(self, raster: Raster) -> Raster: ...
+
+	def zonal_statistics(self, data_raster: Raster, feature_definitions_raster: Raster, stat_type: str = "mean", zero_is_background: bool = False) -> Tuple[Raster, str]: ...
+
+
+class WbPalette(Enum):
+	Atlas: int
+	HighRelief: int
+	Arid: int
+	Earthtones: int
+	Soft: int
+	Muted: int
+	LightQuant: int 
+	Turbo: int
+	Purple: int
+	Viridis: int
+	GreenYellow: int
+	PinkYellowGreen: int
+	BlueYellowRed: int
+	Deep: int
+	Imhof: int
+	White: int
 	Grey: int
```

## whitebox_workflows/__init__.py

```diff
@@ -1,219 +1,280 @@
-from typing import Tuple
-from .whitebox_workflows import *
-from .scripts.horton_ratios import horton_ratios
-from .scripts.nibble import nibble
-from .scripts.ridge_and_valley_vectors import ridge_and_valley_vectors
-from .scripts.sieve import sieve
-from whitebox_workflows import Raster, Vector
-
-__doc__ = whitebox_workflows.__doc__
-if hasattr(whitebox_workflows, "__all__"):
-    __all__ = whitebox_workflows.__all__
-
-class WbEnvironment(WbEnvironmentBase):
-    """The WbEnvironment class can be used to configure WbW settings (e.g. the working
-directory, number of processors used, and verbose mode). It is also used to call
-the various tool functions, which appear as methods of this class, and to read/write
-spatial data."""
-    def __init__(self, user_id: str = None):
-        """Initializes a new WbEnvironment object with an optional user_id, i.e. a floating
-license ID string used in WbW-Pro licenses.
-        """
-        # WbEnvironmentBase(user_id)
-
-    def available_functions(self) -> None:
-        """This function will list all of the available functions associated with a
-WbEnvironment (wbe). The functions that are accessible will depend on the 
-license level (WbW or WbWPro).
-        """
-
-        # Are we running a pro license?
-        pro_license = self.license_type == LicenseType.WbWPro
-
-        # Get all the non-dunder methods of WbEnvironment
-        method_list = [func for func in dir(WbEnvironment) if callable(getattr(WbEnvironment, func)) and not func.startswith("__")]
-
-        print(f"Available Methods ({self.license_type}):")
-
-        j = 0
-        s = ''
-        for i in range(len(method_list)):
-            val = method_list[i]
-            val_len = len(f"{j}. {val}")
-            is_pro_func = whitebox_workflows.is_wbw_pro_function(val)
-            
-            added = True
-            if not is_pro_func and j % 2 == 0:
-                s += f"{j+1}. {val}{' '* (50 - val_len)}"
-                j += 1
-            elif not is_pro_func and j % 2 == 1:
-                s += f"{j+1}. {val}"
-                j += 1
-            elif (is_pro_func and pro_license) and j % 2 == 0:
-                s += f"{j+1}. {val}{' '* (50 - val_len)}"
-                j += 1
-            elif (is_pro_func and pro_license) and j % 2 == 1:
-                s += f"{j+1}. {val}"
-                j += 1
-            else:
-                added = False
-                
-
-            if added and (j % 2 == 0 or i == len(method_list)-1):
-                print(s)
-                s = ''
-
-
-    def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]:
-        '''This function can be used to calculate Horton's so-called laws of drainage network composition for a
-input stream network. The user must specify an input DEM (which has been suitably hydrologically pre-processed
-to remove any topographic depressions) and a raster stream network. The function will output a 4-element 
-tuple containing the bifurcation ratio (Rb), the length ratio (Rl), the area ratio (Ra), and the slope ratio
-(Rs). These indices are related to drainage network geometry and are used in some geomorphological analysis.
-The calculation of the ratios is based on the method described by Knighton (1998) Fluvial Forms and Processes: 
-A New Perspective.
-
-# Code Example
-
-```python
-from whitebox_workflows import WbEnvironment
-
-# Set up the WbW environment
-wbe = WbEnvironment()
-wbe.verbose = True
-wbe.working_directory = '/path/to/data'
-
-# Read the inputs
-dem = wbe.read_raster('DEM.tif')
-streams = wbe.read_raster('streams.tif')
-
-# Calculate the Horton ratios
-(bifurcation_ratio, length_ratio, area_ratio, slope_ratio) = wbe.horton_ratios(dem, streams)
-
-# Outputs
-print(f"Bifurcation ratio (Rb): {bifurcation_ratio:.3f}")
-print(f"Length ratio (Rl): {length_ratio:.3f}")
-print(f"Area ratio (Ra): {area_ratio:.3f}")
-print(f"Slope ratio (Rs): {slope_ratio:.3f}")
-```
-
-# See Also
-<a href="tool_help_wbwpro.md#horton_stream_order">horton_stream_order</a>
-
-# Function Signature
-```python
-def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]: ...
-```
-'''
-        return horton_ratios(self, dem, streams_raster)
-
-
-    def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
-        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
-Please visit www.whiteboxgeo.com to purchase a license.
-
-The nibble function assigns areas within an input class map raster that are coincident with a mask the value 
-of their nearest neighbour. Nibble is typically used to replace erroneous sections in a class map. Cells in the mask
-raster that are either NoData or zero values will be replaced in the input image with their nearest non-masked
-value. All input raster values in non-mask areas will be unmodified.
-
-There are two input parameters that are related to how NoData cells in the input raster are handled during
-the nibble operation. The use_nodata Boolean determines whether or not input NoData cells, not contained within masked
-areas, are treated as ordinary values during the nibble. It is False by default, meaning that NoData cells 
-in the input raster do not extend into nibbled areas. When the nibble_nodata parameter is True, any NoData cells
-in the input raster that are within the masked area are also NoData in the output raster; when nibble_nodata is False
-these cells will be nibbled.
-
-# See Also:
-<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#sieve'>sieve</a>
-
-# Function Signature
-```python
-def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
-```
-'''
-        return nibble(self, input_raster, mask, use_nodata, nibble_nodata)
-
-
-    def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]:
-        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
-Please visit www.whiteboxgeo.com to purchase a license.
-
-This function can be used to extract ridge and channel vectors from an input digital elevation model (DEM).
-The function works by first calculating elevation percentile (EP) from an input DEM using a neighbourhood size set by
-the user-specified filter_size parameter. Increasing the value of filter_size can result in more continuous mapped ridge
-and valley bottom networks. A thresholding operation is then applied to identify cells that have an EP less than the 
-user-specified ep_threshold (valley bottom regions) and a second thresholding operation maps regions where EP is 
-greater than 100 - ep_threshold (ridges). Each of these ridge and valley region maps are also multiplied by a slope 
-mask created by identify all cells with a slope greater than the user-specified slope_threshold value, which is set 
-to zero by default. This second thresholding can be helpful if the input DEM contains extensive flat areas, which 
-can be confused for valleys otherwise. The filter_size and ep_threshold parameters are somewhat dependent on one 
-another. Increasing the filter_size parameter generally requires also increasing the value of the ep_threshold. The 
-ep_threshold can take values between 5.0 and 50.0, where larger values will generally result in more extensive and 
-continuous mapped ridge and valley bottom networks. For many DEMs, a value on the higher end of the scale tends to 
-work best.
-
-After applying the thresholding operations, the function then applies specialized shape generalization, line thinning, 
-and vectorization alorithms to produce the final ridge and valley vectors. The user must also specify the value of the
-min_length parameter, which determines the minimum size, in grid cells, of a mapped line feature. The function outputs
-a tuple of two vector, the first being the ridge network and the second vector being the valley-bottom network.
-
-![](./img/ridge_and_valley_vectors.jpeg)
-
-# Code Example
-
-```python
-from whitebox_workflows import WbEnvironment
-
-# Set up the WbW environment
-license_id = 'my-license-id' # Note, this tool requires a license for WbW-Pro
-wbe = WbEnvironment(license_id)
-try:
-    wbe.verbose = True
-    wbe.working_directory = '/path/to/data'
-
-    # Read the input DEM
-    dem = wbe.read_raster('DEM.tif')
-
-    # Run the operation
-    ridges, valleys = wbe.ridge_and_valley_vectors(dem, filter_size=21, ep_threshold=45.0, slope_threshold=1.0, min_length=25)
-    wbe.write_vector(ridges, 'ridges_lines.shp')
-    wbe.write_vector(valley, 'valley_lines.shp')
-
-    print('Done!')
-except Exception as e:
-  print("Error: ", e)
-finally:
-    wbe.check_in_license(license_id)
-```
-
-# See Also:
-<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help.html#extract_valleys'>extract_valleys</a>
-
-# Function Signature
-```python
-def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Raster, Raster]:
-```
-'''
-        return ridge_and_valley_vectors(self, dem, filter_size, ep_threshold, slope_threshold, min_length)
-
-
-    def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster:
-        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
-Please visit www.whiteboxgeo.com to purchase a license.
-
-The sieve function removes individual objects in a class map that are less than a threshold
-area, in grid cells. Pixels contained within the removed small polygons will be replaced with the nearest
-remaining class value. This operation is common when generalizing class maps, e.g. those derived from an
-image classification. Thus, this tool provides a similar function to the <a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_classified_raster'>generalize_classified_raster</a> and
-<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_with_similarity'>generalize_with_similarity</a> functions.
-
-# See Also:
-<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_classified_raster'>generalize_classified_raster</a>, <a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_with_similarity'>generalize_with_similarity</a>
-
-# Function Signature
-```python
-def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster: ...
-```
-        '''
-        return sieve(self, input_raster, threshold, zero_background)
+from typing import Tuple
+from .whitebox_workflows import *
+from .scripts.horton_ratios import horton_ratios
+from .scripts.improved_ground_point_filter import improved_ground_point_filter
+from .scripts.nibble import nibble
+from .scripts.ridge_and_valley_vectors import ridge_and_valley_vectors
+from .scripts.sieve import sieve
+from whitebox_workflows import Raster, Vector
+
+__doc__ = whitebox_workflows.__doc__
+if hasattr(whitebox_workflows, "__all__"):
+    __all__ = whitebox_workflows.__all__
+
+class WbEnvironment(WbEnvironmentBase):
+    """The WbEnvironment class can be used to configure WbW settings (e.g. the working
+directory, number of processors used, and verbose mode). It is also used to call
+the various tool functions, which appear as methods of this class, and to read/write
+spatial data."""
+    def __init__(self, user_id: str = None):
+        """Initializes a new WbEnvironment object with an optional user_id, i.e. a floating
+license ID string used in WbW-Pro licenses.
+        """
+        # WbEnvironmentBase(user_id)
+
+    def available_functions(self) -> None:
+        """This function will list all of the available functions associated with a
+WbEnvironment (wbe). The functions that are accessible will depend on the 
+license level (WbW or WbWPro).
+        """
+
+        # Are we running a pro license?
+        pro_license = self.license_type == LicenseType.WbWPro
+
+        # Get all the non-dunder methods of WbEnvironment
+        method_list = [func for func in dir(WbEnvironment) if callable(getattr(WbEnvironment, func)) and not func.startswith("__")]
+
+        print(f"Available Methods ({self.license_type}):")
+
+        j = 0
+        s = ''
+        for i in range(len(method_list)):
+            val = method_list[i]
+            val_len = len(f"{j}. {val}")
+            is_pro_func = whitebox_workflows.is_wbw_pro_function(val)
+            
+            added = True
+            if not is_pro_func and j % 2 == 0:
+                s += f"{j+1}. {val}{' '* (50 - val_len)}"
+                j += 1
+            elif not is_pro_func and j % 2 == 1:
+                s += f"{j+1}. {val}"
+                j += 1
+            elif (is_pro_func and pro_license) and j % 2 == 0:
+                s += f"{j+1}. {val}{' '* (50 - val_len)}"
+                j += 1
+            elif (is_pro_func and pro_license) and j % 2 == 1:
+                s += f"{j+1}. {val}"
+                j += 1
+            else:
+                added = False
+                
+
+            if added and (j % 2 == 0 or i == len(method_list)-1):
+                print(s)
+                s = ''
+
+
+    def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]:
+        '''This function can be used to calculate Horton's so-called laws of drainage network composition for a
+input stream network. The user must specify an input DEM (which has been suitably hydrologically pre-processed
+to remove any topographic depressions) and a raster stream network. The function will output a 4-element 
+tuple containing the bifurcation ratio (Rb), the length ratio (Rl), the area ratio (Ra), and the slope ratio
+(Rs). These indices are related to drainage network geometry and are used in some geomorphological analysis.
+The calculation of the ratios is based on the method described by Knighton (1998) Fluvial Forms and Processes: 
+A New Perspective.
+
+# Code Example
+
+```python
+from whitebox_workflows import WbEnvironment
+
+# Set up the WbW environment
+wbe = WbEnvironment()
+wbe.verbose = True
+wbe.working_directory = '/path/to/data'
+
+# Read the inputs
+dem = wbe.read_raster('DEM.tif')
+streams = wbe.read_raster('streams.tif')
+
+# Calculate the Horton ratios
+(bifurcation_ratio, length_ratio, area_ratio, slope_ratio) = wbe.horton_ratios(dem, streams)
+
+# Outputs
+print(f"Bifurcation ratio (Rb): {bifurcation_ratio:.3f}")
+print(f"Length ratio (Rl): {length_ratio:.3f}")
+print(f"Area ratio (Ra): {area_ratio:.3f}")
+print(f"Slope ratio (Rs): {slope_ratio:.3f}")
+```
+
+# See Also
+<a href="tool_help_wbwpro.md#horton_stream_order">horton_stream_order</a>
+
+# Function Signature
+```python
+def horton_ratios(self, dem: Raster, streams_raster: Raster) -> Tuple[float, float, float, float]: ...
+```
+'''
+        return horton_ratios(self, dem, streams_raster)
+
+
+    def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
+        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
+Please visit www.whiteboxgeo.com to purchase a license.
+
+The nibble function assigns areas within an input class map raster that are coincident with a mask the value 
+of their nearest neighbour. Nibble is typically used to replace erroneous sections in a class map. Cells in the mask
+raster that are either NoData or zero values will be replaced in the input image with their nearest non-masked
+value. All input raster values in non-mask areas will be unmodified.
+
+There are two input parameters that are related to how NoData cells in the input raster are handled during
+the nibble operation. The use_nodata Boolean determines whether or not input NoData cells, not contained within masked
+areas, are treated as ordinary values during the nibble. It is False by default, meaning that NoData cells 
+in the input raster do not extend into nibbled areas. When the nibble_nodata parameter is True, any NoData cells
+in the input raster that are within the masked area are also NoData in the output raster; when nibble_nodata is False
+these cells will be nibbled.
+
+# See Also:
+<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#sieve'>sieve</a>
+
+# Function Signature
+```python
+def nibble(self, input_raster: Raster, mask: Raster, use_nodata: bool = False, nibble_nodata: bool = True) -> Raster:
+```
+'''
+        return nibble(self, input_raster, mask, use_nodata, nibble_nodata)
+
+
+    def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Vector, Vector]:
+        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
+Please visit www.whiteboxgeo.com to purchase a license.
+
+This function can be used to extract ridge and channel vectors from an input digital elevation model (DEM).
+The function works by first calculating elevation percentile (EP) from an input DEM using a neighbourhood size set by
+the user-specified filter_size parameter. Increasing the value of filter_size can result in more continuous mapped ridge
+and valley bottom networks. A thresholding operation is then applied to identify cells that have an EP less than the 
+user-specified ep_threshold (valley bottom regions) and a second thresholding operation maps regions where EP is 
+greater than 100 - ep_threshold (ridges). Each of these ridge and valley region maps are also multiplied by a slope 
+mask created by identify all cells with a slope greater than the user-specified slope_threshold value, which is set 
+to zero by default. This second thresholding can be helpful if the input DEM contains extensive flat areas, which 
+can be confused for valleys otherwise. The filter_size and ep_threshold parameters are somewhat dependent on one 
+another. Increasing the filter_size parameter generally requires also increasing the value of the ep_threshold. The 
+ep_threshold can take values between 5.0 and 50.0, where larger values will generally result in more extensive and 
+continuous mapped ridge and valley bottom networks. For many DEMs, a value on the higher end of the scale tends to 
+work best.
+
+After applying the thresholding operations, the function then applies specialized shape generalization, line thinning, 
+and vectorization alorithms to produce the final ridge and valley vectors. The user must also specify the value of the
+min_length parameter, which determines the minimum size, in grid cells, of a mapped line feature. The function outputs
+a tuple of two vector, the first being the ridge network and the second vector being the valley-bottom network.
+
+![](./img/ridge_and_valley_vectors.jpeg)
+
+# Code Example
+
+```python
+from whitebox_workflows import WbEnvironment
+
+# Set up the WbW environment
+license_id = 'my-license-id' # Note, this tool requires a license for WbW-Pro
+wbe = WbEnvironment(license_id)
+try:
+    wbe.verbose = True
+    wbe.working_directory = '/path/to/data'
+
+    # Read the input DEM
+    dem = wbe.read_raster('DEM.tif')
+
+    # Run the operation
+    ridges, valleys = wbe.ridge_and_valley_vectors(dem, filter_size=21, ep_threshold=45.0, slope_threshold=1.0, min_length=25)
+    wbe.write_vector(ridges, 'ridges_lines.shp')
+    wbe.write_vector(valley, 'valley_lines.shp')
+
+    print('Done!')
+except Exception as e:
+  print("Error: ", e)
+finally:
+    wbe.check_in_license(license_id)
+```
+
+# See Also:
+<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help.html#extract_valleys'>extract_valleys</a>
+
+# Function Signature
+```python
+def ridge_and_valley_vectors(self, dem: Raster, filter_size: int = 11, ep_threshold: float = 30.0, slope_threshold: float = 0.0, min_length: int = 20) -> Tuple[Raster, Raster]:
+```
+'''
+        return ridge_and_valley_vectors(self, dem, filter_size, ep_threshold, slope_threshold, min_length)
+
+
+    def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster:
+        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
+Please visit www.whiteboxgeo.com to purchase a license.
+
+The sieve function removes individual objects in a class map that are less than a threshold
+area, in grid cells. Pixels contained within the removed small polygons will be replaced with the nearest
+remaining class value. This operation is common when generalizing class maps, e.g. those derived from an
+image classification. Thus, this tool provides a similar function to the <a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_classified_raster'>generalize_classified_raster</a> and
+<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_with_similarity'>generalize_with_similarity</a> functions.
+
+# See Also:
+<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_classified_raster'>generalize_classified_raster</a>, <a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help_wbwpro.html#generalize_with_similarity'>generalize_with_similarity</a>
+
+# Function Signature
+```python
+def sieve(self, input_raster: Raster, threshold: int = 1, zero_background: bool = False) -> Raster: ...
+```
+        '''
+        return sieve(self, input_raster, threshold, zero_background)
+    
+    def improved_ground_point_filter(self, input: Lidar, block_size = 1.0, max_building_size = 150.0, slope_threshold = 15.0, elev_threshold = 0.15) -> Lidar:
+        '''Use of this function requires a license for Whitebox Workflows for Python Professional (WbW-Pro).
+Please visit www.whiteboxgeo.com to purchase a license.
+
+This function provides a faster alternative to the `lidar_ground_point_filter` algorithm, provided in the free
+version of Whitebox Workflows, for the extraction of ground points from within a LiDAR point cloud. The algorithm
+works by placing a grid overtop of the point cloud of a specified resolution (`block_size`, in xy-units) and identifying the
+subset of lidar points associated with the lowest position in each block. A raster surface is then created by 
+TINing these points. The surface is further processed by removing any off-terrain objects (OTOs), including buildings
+smaller than the `max_building_size` parameter (xy-units). Removing OTOs also requires the user to specify the value of
+a `slope_threshold`, in degrees. Finally, the algorithm then extracts all of the points in the input LiDAR point cloud 
+(`input`) that are within a specified absolute vertical distance (`elev_threshold`) of this surface model.
+
+Conceptually, this method of ground-point filtering is somewhat similar in concept to the cloth-simulation approach of 
+Zhang et al. (2016). The difference is that the cloth is first fitted to the minimum surface with infinite flexibility 
+and then the rigidity of the cloth is subsequently increased, via the identification and removal of OTOs from the minimal 
+surface. The `slope_threshold` parameter effectively controls the eventual rigidity of the fitted surface.
+
+Compared with the `lidar_ground_point_filter` algorithm, the `improved_ground_point_filter` algorithm is generally far faster and is
+able to more effectively remove points associated with larger buildings. Removing large buildings from point clouds with the 
+`lidar_ground_point_filter` algorithm requires use of very large search distances, which slows the operation considerably.
+However, `lidar_ground_point_filter` is perhaps more flexible overall because it provides the option to either extract
+ground points or simply to classify them. The `improved_ground_point_filter` function, by comparison, only allows for the 
+extraction of ground points (i.e., filtering) and not the classification of ground points. Thus, this function is more suited
+to the efficient creation of ground point clouds of bare-earth digital elevation models (i.e., digital terrain models) from
+unclassified LiDAR data assets.
+
+As a comparison of the two available methods, one test tile of LiDAR containing numerous large buildings and abundant 
+vegetation required 600.5 seconds to process on the test system using the `lidar_ground_point_filter` algorithm 
+(removing all but the largest buildings) and 9.8 seconds to process using the `improved_ground_point_filter` algorithm 
+(with complete building removal), i.e., 61x faster.
+
+The original test LiDAR tile, containing abundant vegetation and buildings:
+
+![](./img/improved_ground_point_filter1.png)
+
+The result of applying the `lidar_ground_point_filter` function, with a search radius of 25 m and max inter-point slope of 
+15 degrees:
+
+![](./img/improved_ground_point_filter2.png)
+
+The result of applying the `improved_ground_point_filter` method, with `block_size` = 1.0 m, `max_building_size` = 150.0 m, 
+`slope_threshold` = 15.0 degrees, and `elev_threshold` = 0.15 m:
+
+![](./img/improved_ground_point_filter3.png)
+
+# References:
+Zhang, W., Qi, J., Wan, P., Wang, H., Xie, D., Wang, X., & Yan, G. (2016). An easy-to-use airborne LiDAR data filtering 
+method based on cloth simulation. Remote sensing, 8(6), 501.
+
+# See Also:
+<a href='https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help.html#lidar_ground_point_filter'>lidar_ground_point_filter</a>
+
+# Function Signature
+```python
+def improved_ground_point_filter(self, input: Lidar, block_size = 1.0, max_building_size = 150.0, slope_threshold = 15.0, elev_threshold = 0.15) -> Lidar: ...
+```
+        '''
+        return improved_ground_point_filter(self, input, block_size, max_building_size, slope_threshold, elev_threshold)
```

## Comparing `whitebox_workflows-1.2.6.dist-info/METADATA` & `whitebox_workflows-1.2.7.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,207 +1,216 @@
 Metadata-Version: 2.3
 Name: whitebox_workflows
-Version: 1.2.6
+Version: 1.2.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.txt
 Summary: whitebox_workflows is a Python library for advanced spatial analysis.
 Keywords: spatial analysis,GIS,remote sensing
 Author: Whitebox Geospatial Inc.
 Author-email: support@whiteboxgeo.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# Whitebox Workflows for Python
-
-
-## What is Whitebox Workflows?
-
-Whitebox Workflows (WbW) is a Python library for advanced geoprocessing, including [more than 400 functions](https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help.html) for GIS and remote sensing analysis operations and for for manipulating common types of raster, vector and LiDAR geospatial data.
-
-> For more details about the project, see [the User Manual](https://www.whiteboxgeo.com/manual/wbw-user-manual/book/introduction.html).
-
-
-## Why Whitebox Workflows when there already is WhiteboxTools Open Core?
-
-**Whitebox Workflows** (WbW) is based on the **WhiteboxTools Open Core** (WbOC) open-source codebase. While the two products share many characteristics and functionality, there are important differences.
-
-The WhiteboxTools Open Core is a command line back-end program that interfaces with various front-end applications, such as QGIS, ArcGIS and the R and Python scripting languages. Front-end/back-end communication is very limited. Front-ends can only communicate with WbOC by passing text-based commands and receive text-based outputs. Data files are provided as file names and are read into memory during tool operation and output data are written to disc. This design allows WbOC to be readily integrated into other projects. However, it doesn't allow front-ends to directly interact with Whitebox data,  and it isn't well suited to longer geoprocessing workflows. Tools in a WbOC based geoprocessing script are essentially run independently of other tools in the same workflow.
-
-By comparison, **Whitebox Workflows is a native Python extension library**; it has been designed to work with Python, providing a geoprocessing scripting environment. Like the open-core, WbW is developed using the fast programming language Rust, but is compiled to a shared library that can be directly imported into Python scripts, much like NumPy and other common Python scientific libraries. 
-
-**Each of the more than 400 geoprocessing tools that users love about the WbOC are also found in WbW.** The library design of WbW affords a much more intimate level of communication between it and your Python geoprocessing script. For instance, with WbW **you can directly manipulate raster, vector, and lidar data objects**, to perform low-level geoprocessing in a way that is impossible with the open-core. For example, below we manipulate raster data directly in Python using WbW:
-
-```python
-import whitebox_workflows as wbw
-
-wbe = wbw.WbEnvironment()
-dem = wbe.read_raster('/path/to/data/dem.tif')
-high_areas = wbe.new_raster(dem.configs)
-
-print("Finding high elevations")
-
-for row in range(dem.configs.rows):
-  for col in range(dem.configs.columns):
-    elev = dem[row, col]
-    if elev != dem.configs.nodata and elev > 1000.0:
-      high_areas[row, col] = 1.0
-    else:
-      high_areas[row, col] = 0.0
-
-wbe.write_raster(high_areas, 'high_areas.tif', compress=True)
-```
-
-Where tools in the open-core take file name strings as inputs, the WbW equivalent functions take in-memory geospatial objects as input parameters. WbW functions also return output objects. This means that for a typical geoprocessing workflow there is significantly less reading/writing of data to the disc. **There is no performance cost incurred by read/write operations during the intermediate processing.** WbW has been designed to meet enterprise-scale geoprocessing workflow needs. 
-
-The following example Python script interpolates a lidar file to a digital elevation model (DEM), performs some common pre-processing steps on the DEM, and then runs a flow accumulation operation, before outputting the flow accumulation grid to file:
-
-```python
-import whitebox_workflows as wbw
-
-wbe = wbw.WbEnvironment()
-
-lidar = wbe.read_lidar('/path/to/data/myfile.laz')
-dem = wbe.lidar_tin_gridding(input_lidar=lidar, returns_included='last', cell_size=1.0)
-dem_nodata_filled = wbe.fill_missing_data(dem, filter_size=21)
-dem_breached = wbe.breach_depressions_least_cost(dem_nodata_filled, fill_deps=True)
-dem_smoothed = wbe.feature_preserving_smoothing(dem_breached, filter_size=15)
-flow_accum = wbe.dinf_flow_accum(dem_smoothed, log_transform=True)
-wbe.write_raster(flow_accum, "flow_accumulation_grid.tif", compress=True)
-```
-
-Notice how each of the five tool functions return data objects that then serve as the inputs for later operations. While there's only one read operation and one write operation in the script, an equivalent WbOC workflow would result in 10 individual read/write operations. This characteristic **can result in significant gains in overall workflow performance**. It is often the case that read/write operations can be the bottle-neck in geoprocessing performance. Fewer read/write operations also means significantly **less wear on your hardware**.
-
-The design of WbW also allows for **more natural geoprocessing of data objects**. For example, rather than using individual raster math tools (e.g. ``Add``, ``Divide``, ``Sin`` etc.), with WbW, you can often treat raster objects like any other numerical variables in scripts--with WbW, Python becomes your raster calculator!
-
-```python
-new_raster = 1.0 - (raster1 - raster2) / (raster1 + raster2)
-new_raster = dem > 1000.0   # Note: This single line is equivalent to one of the example Python scripts above
-new_raster = raster.sin().to_degrees()
-new_raster = raster1.max(raster2)   # You can use a number instead of a raster as the parameter, e.g. raster.max(100.0)
-```
-
-**Overall, if you're using the Whitebox platform to develop Python scripts for geoprocessing tasks, Whitebox Workflows is the clear winner.** It provides easier-to-write and faster-running scripting with less strain on your expensive hardware. Simply put, **it's a more productive geoprocessing environment**. 
-
-There is, however, one small downside to using WbW over WbOC. Developing WbW was not a matter of simply compiling the existing WbOC codebase as a library; it took a substantial development effort to create this great product. Whitebox Workflows is not free. **You need to [purchase a valid license activation code](https://www.whiteboxgeo.com/whitebox-workflows-for-python/) to use WbW**. The good news is, annual licenses for WbW are very reasonably priced--only about $10. We want as many people using this wonderful product as possible!
-
-
-## Installation
-
-If you have Python installed on your machine, simply type ``pip install whitebox-workflows`` at the command prompt. Windows (64-bit), Mac (Intel and ARM), and Linux (x86_64) operating systems are supported.
-
-If you have installed whitebox-workflows Python package before and want to upgrade to the latest version, you can use the following command:
-
-```pip install whitebox-workflows -U```
-
-It is recommended that you use a Python virtual environment to test the whitebox-workflows package.
-
-
-## Usage
-
-```python
-import whitebox_workflows as wbw
-
-##########################
-# Set up the environment #
-##########################
-wbe = wbw.WbEnvironment() # A WbEnvironment object is needed to read/write data and run tools.
-wbe.verbose = True # Determines if tools output to std::out
-wbe.max_procs = -1
-wbe.working_directory = '/path/to/my/data'
-
-############################
-# Read some data from disc #
-############################
-dem = wbe.read_raster('DEM_5m.tif')
-points = wbe.read_vector('points.shp')
-lidar = wbe.read_lidar('my_lidar_tile.laz')
-
-######################
-# Run some functions #
-#######################
-hillshade_raster = wbe.hillshade(dem, azimuth=270.0)
-pointer = wbe.d8_pointer(dem)
-watersheds = wbe.watershed(pointer, points)
-
-###########################
-# Write some data to disc #
-###########################
-wbe.write_raster(hillshade_raster, 'hillshade.tif', compress=True)
-wbe.write_raster(watersheds, 'watersheds.tif', compress=True)
-
-######################
-# Raster map algebra #
-######################
-elev_in_ft = dem * 3.28084
-high_in_watershed = (dem > 500.0) * (watersheds == 1.0)
-tan_elev = dem.tan()
-dem += 10.0 
-raster3 = raster1 / raster2
-
-###############################
-# Manipulate lidar point data #
-###############################
-lidar = wbe.read_lidar('/path/to/data/lidar_tile.laz')
-lidar_out = wbe.new_lidar(lidar.header) # Create a new file
-
-print('Filtering point data...')
-for a in range(lidar.header.number_of_points):
-    (point_data, time, colour, waveform) = lidar.get_point_record(a)
-    if point_data.is_first_return() or point_data.is_intermediate_return():
-        lidar_out.add_point(point_data, time)
-
-wbe.write_lidar(lidar_out, "new_lidar.laz")
-```
-
-## Release history
-
-## Version 1.2.6 (April 4, 2024)
-- Added the sieve and nibble functions for class map generalization.
-- Added the ridge_and_valley_vectors function for extracting ridge and valley
-  lines from digital elevation models.
-- Added the skyline_analysis tool for performing local landscape visibility
-  analysis.
-- Fixed a bug with the RandomForestRegressionPredict tool, where output
-  rasters had an integer data type.
-
-## Version 1.2.4 (March 17, 2024)
-- Fixed an issue with the stub file (pyi) being saved in the wrong location for
-  a mixed Rust/Python PyO3 project. This issue resulted in WbW not having correct
-  type hinting in Python coding environments since we migrated to a mixed project
-  format. 
-
-## Version 1.2.3 (March 17, 2024)
-- Added the average_horizon_distance, horizon_area, and sky_view_factor functions.
-- Added the standard_deviation_overlay tool.
-- Split the random_forest_regression and random_forest_classification tools into
-  model fitting and prediction stages, e.g. random_forest_regression_fit and
-  random_forest_regression_prediction.
-
-### Version 1.2.1 (February 25, 2024)
-- Added the horton_ratios function for calculating the laws of drainage network composition.
-- Fixed a bug with the depth_to_water function, where it threw an error that the input
-  stream network was not of the correct shape type, even when it was.
-
-### Version 1.1.2 (October 2, 2023)
-- Added the ability to use the string 'value' as the TRUE and FALSE parameters of a raster 
-  con statement (conditional evaluation). Previously these statements had to be either a
-  raster object, a numerical constant, or the strings 'null' or 'nodata'.
-- Fixed an issue with the aspect function that had previously been fixed in WbTools, but no
-  ported to Workflows.
-
-### Version 1.1.1 (September 10, 2023)
-- Made several minor bug fixes, including one important one that affected the mosaic function.
-
-### Version 1.1 (June 17, 2023)
-- Added ability to read COPC lidar files.
-- Added the extract_by_attribute tool to filter out vector features by attribute characteristics.
-- Added the deviation_from_regional_direction tool.
-- Added the otsu_thresholding tool, which uses Ostu's method for optimal binary thresholding,
-  transforming the input image into background and foreground pixels.
-- Added the topographic_hachures tool.
-- Fixed a bug with polygon holes in the raster_to_vector_polygons tool.
-- Fixed a bug with the individual_tree_detection tool that prevented use of the min_height parameter
-  when applied in batch mode.
-- Fixed a bug with the breakline_mapping tool in WbW-Pro.
+# Whitebox Workflows for Python
+
+
+## What is Whitebox Workflows?
+
+Whitebox Workflows (WbW) is a Python library for advanced geoprocessing, including [more than 400 functions](https://www.whiteboxgeo.com/manual/wbw-user-manual/book/tool_help.html) for GIS and remote sensing analysis operations and for for manipulating common types of raster, vector and LiDAR geospatial data.
+
+> For more details about the project, see [the User Manual](https://www.whiteboxgeo.com/manual/wbw-user-manual/book/introduction.html).
+
+
+## Why Whitebox Workflows when there already is WhiteboxTools Open Core?
+
+**Whitebox Workflows** (WbW) is based on the **WhiteboxTools Open Core** (WbOC) open-source codebase. While the two products share many characteristics and functionality, there are important differences.
+
+The WhiteboxTools Open Core is a command line back-end program that interfaces with various front-end applications, such as QGIS, ArcGIS and the R and Python scripting languages. Front-end/back-end communication is very limited. Front-ends can only communicate with WbOC by passing text-based commands and receive text-based outputs. Data files are provided as file names and are read into memory during tool operation and output data are written to disc. This design allows WbOC to be readily integrated into other projects. However, it doesn't allow front-ends to directly interact with Whitebox data,  and it isn't well suited to longer geoprocessing workflows. Tools in a WbOC based geoprocessing script are essentially run independently of other tools in the same workflow.
+
+By comparison, **Whitebox Workflows is a native Python extension library**; it has been designed to work with Python, providing a geoprocessing scripting environment. Like the open-core, WbW is developed using the fast programming language Rust, but is compiled to a shared library that can be directly imported into Python scripts, much like NumPy and other common Python scientific libraries. 
+
+**Each of the more than 400 geoprocessing tools that users love about the WbOC are also found in WbW.** The library design of WbW affords a much more intimate level of communication between it and your Python geoprocessing script. For instance, with WbW **you can directly manipulate raster, vector, and lidar data objects**, to perform low-level geoprocessing in a way that is impossible with the open-core. For example, below we manipulate raster data directly in Python using WbW:
+
+```python
+import whitebox_workflows as wbw
+
+wbe = wbw.WbEnvironment()
+dem = wbe.read_raster('/path/to/data/dem.tif')
+high_areas = wbe.new_raster(dem.configs)
+
+print("Finding high elevations")
+
+for row in range(dem.configs.rows):
+  for col in range(dem.configs.columns):
+    elev = dem[row, col]
+    if elev != dem.configs.nodata and elev > 1000.0:
+      high_areas[row, col] = 1.0
+    else:
+      high_areas[row, col] = 0.0
+
+wbe.write_raster(high_areas, 'high_areas.tif', compress=True)
+```
+
+Where tools in the open-core take file name strings as inputs, the WbW equivalent functions take in-memory geospatial objects as input parameters. WbW functions also return output objects. This means that for a typical geoprocessing workflow there is significantly less reading/writing of data to the disc. **There is no performance cost incurred by read/write operations during the intermediate processing.** WbW has been designed to meet enterprise-scale geoprocessing workflow needs. 
+
+The following example Python script interpolates a lidar file to a digital elevation model (DEM), performs some common pre-processing steps on the DEM, and then runs a flow accumulation operation, before outputting the flow accumulation grid to file:
+
+```python
+import whitebox_workflows as wbw
+
+wbe = wbw.WbEnvironment()
+
+lidar = wbe.read_lidar('/path/to/data/myfile.laz')
+dem = wbe.lidar_tin_gridding(input_lidar=lidar, returns_included='last', cell_size=1.0)
+dem_nodata_filled = wbe.fill_missing_data(dem, filter_size=21)
+dem_breached = wbe.breach_depressions_least_cost(dem_nodata_filled, fill_deps=True)
+dem_smoothed = wbe.feature_preserving_smoothing(dem_breached, filter_size=15)
+flow_accum = wbe.dinf_flow_accum(dem_smoothed, log_transform=True)
+wbe.write_raster(flow_accum, "flow_accumulation_grid.tif", compress=True)
+```
+
+Notice how each of the five tool functions return data objects that then serve as the inputs for later operations. While there's only one read operation and one write operation in the script, an equivalent WbOC workflow would result in 10 individual read/write operations. This characteristic **can result in significant gains in overall workflow performance**. It is often the case that read/write operations can be the bottle-neck in geoprocessing performance. Fewer read/write operations also means significantly **less wear on your hardware**.
+
+The design of WbW also allows for **more natural geoprocessing of data objects**. For example, rather than using individual raster math tools (e.g. ``Add``, ``Divide``, ``Sin`` etc.), with WbW, you can often treat raster objects like any other numerical variables in scripts--with WbW, Python becomes your raster calculator!
+
+```python
+new_raster = 1.0 - (raster1 - raster2) / (raster1 + raster2)
+new_raster = dem > 1000.0   # Note: This single line is equivalent to one of the example Python scripts above
+new_raster = raster.sin().to_degrees()
+new_raster = raster1.max(raster2)   # You can use a number instead of a raster as the parameter, e.g. raster.max(100.0)
+```
+
+**Overall, if you're using the Whitebox platform to develop Python scripts for geoprocessing tasks, Whitebox Workflows is the clear winner.** It provides easier-to-write and faster-running scripting with less strain on your expensive hardware. Simply put, **it's a more productive geoprocessing environment**. 
+
+There is, however, one small downside to using WbW over WbOC. Developing WbW was not a matter of simply compiling the existing WbOC codebase as a library; it took a substantial development effort to create this great product. Whitebox Workflows is not free. **You need to [purchase a valid license activation code](https://www.whiteboxgeo.com/whitebox-workflows-for-python/) to use WbW**. The good news is, annual licenses for WbW are very reasonably priced--only about $10. We want as many people using this wonderful product as possible!
+
+
+## Installation
+
+If you have Python installed on your machine, simply type ``pip install whitebox-workflows`` at the command prompt. Windows (64-bit), Mac (Intel and ARM), and Linux (x86_64) operating systems are supported.
+
+If you have installed whitebox-workflows Python package before and want to upgrade to the latest version, you can use the following command:
+
+```pip install whitebox-workflows -U```
+
+It is recommended that you use a Python virtual environment to test the whitebox-workflows package.
+
+
+## Usage
+
+```python
+from whitebox_workflows import WbEnvironment
+
+##########################
+# Set up the environment #
+##########################
+wbe = WbEnvironment() # A WbEnvironment object is needed to read/write data and run tools.
+wbe.verbose = True # Determines if tools output to std::out
+wbe.max_procs = -1
+wbe.working_directory = '/path/to/my/data'
+
+############################
+# Read some data from disc #
+############################
+dem = wbe.read_raster('DEM_5m.tif')
+points = wbe.read_vector('points.shp')
+lidar = wbe.read_lidar('my_lidar_tile.laz')
+
+######################
+# Run some functions #
+#######################
+hillshade_raster = wbe.hillshade(dem, azimuth=270.0)
+pointer = wbe.d8_pointer(dem)
+watersheds = wbe.watershed(pointer, points)
+
+###########################
+# Write some data to disc #
+###########################
+wbe.write_raster(hillshade_raster, 'hillshade.tif', compress=True)
+wbe.write_raster(watersheds, 'watersheds.tif', compress=True)
+
+######################
+# Raster map algebra #
+######################
+elev_in_ft = dem * 3.28084
+high_in_watershed = (dem > 500.0) * (watersheds == 1.0)
+tan_elev = dem.tan()
+dem += 10.0 
+raster3 = raster1 / raster2
+
+###############################
+# Manipulate lidar point data #
+###############################
+lidar = wbe.read_lidar('/path/to/data/lidar_tile.laz')
+lidar_out = wbe.new_lidar(lidar.header) # Create a new file
+
+print('Filtering point data...')
+for a in range(lidar.header.number_of_points):
+    (point_data, time, colour, waveform) = lidar.get_point_record(a)
+    if point_data.is_first_return() or point_data.is_intermediate_return():
+        lidar_out.add_point(point_data, time)
+
+wbe.write_lidar(lidar_out, "new_lidar.laz")
+```
+
+## Release history
+
+## Version 1.2.7 (April 15, 2024)
+- Added the filter_lidar_by_percentile function, which extracts a subset of points from an 
+  input LiDAR point cloud that correspond to a user-specified percentile of the points within 
+  the local neighbourhood.
+- Added the filter_lidar_by_reference_surface function, which extract a subset of points from an 
+  input LiDAR point cloud that satisfy a query relation with a user-specified raster reference surface.
+- Added the improved_ground_point_filter function, which identifies and extracts ground points from
+  an input LiDAR point cloud.
+
+## Version 1.2.6 (April 4, 2024)
+- Added the sieve and nibble functions for class map generalization.
+- Added the ridge_and_valley_vectors function for extracting ridge and valley
+  lines from digital elevation models.
+- Added the skyline_analysis tool for performing local landscape visibility
+  analysis.
+- Fixed a bug with the RandomForestRegressionPredict tool, where output
+  rasters had an integer data type.
+
+## Version 1.2.4 (March 17, 2024)
+- Fixed an issue with the stub file (pyi) being saved in the wrong location for
+  a mixed Rust/Python PyO3 project. This issue resulted in WbW not having correct
+  type hinting in Python coding environments since we migrated to a mixed project
+  format. 
+
+## Version 1.2.3 (March 17, 2024)
+- Added the average_horizon_distance, horizon_area, and sky_view_factor functions.
+- Added the standard_deviation_overlay tool.
+- Split the random_forest_regression and random_forest_classification tools into
+  model fitting and prediction stages, e.g. random_forest_regression_fit and
+  random_forest_regression_prediction.
+
+### Version 1.2.1 (February 25, 2024)
+- Added the horton_ratios function for calculating the laws of drainage network composition.
+- Fixed a bug with the depth_to_water function, where it threw an error that the input
+  stream network was not of the correct shape type, even when it was.
+
+### Version 1.1.2 (October 2, 2023)
+- Added the ability to use the string 'value' as the TRUE and FALSE parameters of a raster 
+  con statement (conditional evaluation). Previously these statements had to be either a
+  raster object, a numerical constant, or the strings 'null' or 'nodata'.
+- Fixed an issue with the aspect function that had previously been fixed in WbTools, but no
+  ported to Workflows.
+
+### Version 1.1.1 (September 10, 2023)
+- Made several minor bug fixes, including one important one that affected the mosaic function.
+
+### Version 1.1 (June 17, 2023)
+- Added ability to read COPC lidar files.
+- Added the extract_by_attribute tool to filter out vector features by attribute characteristics.
+- Added the deviation_from_regional_direction tool.
+- Added the otsu_thresholding tool, which uses Ostu's method for optimal binary thresholding,
+  transforming the input image into background and foreground pixels.
+- Added the topographic_hachures tool.
+- Fixed a bug with polygon holes in the raster_to_vector_polygons tool.
+- Fixed a bug with the individual_tree_detection tool that prevented use of the min_height parameter
+  when applied in batch mode.
+- Fixed a bug with the breakline_mapping tool in WbW-Pro.
```

## Comparing `whitebox_workflows-1.2.6.dist-info/RECORD` & `whitebox_workflows-1.2.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-whitebox_workflows-1.2.6.dist-info/METADATA,sha256=r3woTGCTIb7hA7AIthlcnuhqjBzL-COeXbkZjYCQIhM,11931
-whitebox_workflows-1.2.6.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-whitebox_workflows-1.2.6.dist-info/license_files/LICENSE.txt,sha256=uBmnn03dDa5bOiHwTs9qtqcTwrWnhNbulJZYGJUJGyc,163
-whitebox_workflows/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-whitebox_workflows/scripts/horton_ratios.py,sha256=Rk93Flpuq4xfwtUrZDOKm0fHg9G-zhqMUnDGHuSSWTQ,8450
-whitebox_workflows/scripts/nibble.py,sha256=NhcgqqC_5efH0LQPgUeUHncqSRQOkE4ERGUg-VEKYo0,2158
-whitebox_workflows/scripts/ridge_and_valley_vectors.py,sha256=ipLbFdRY3l0D1cyQ6BY5bsTUR5hjNihcl8msc9CSux0,1852
-whitebox_workflows/scripts/scripts.py,sha256=B1t8uiSjyZc1JbLbeKCflhtSfF5JirVLhBk9LiTdtUk,1045
-whitebox_workflows/scripts/sieve.py,sha256=kdHFJvjJT_YpF02GHuB1rwO5YLL7IQovWUhWkVoQDJc,967
-whitebox_workflows/scripts/utils.py,sha256=OGx5UiGeVmdoyQ1ft-zb91UvSWC1CfAmM3p3S_Me-eg,890
+whitebox_workflows-1.2.7.dist-info/METADATA,sha256=UrBNsoT-Xh7En9mf3HVQYzKDuaNr5laBvmsbvRMFDB8,12328
+whitebox_workflows-1.2.7.dist-info/WHEEL,sha256=n0czgnEgzrz3uJexVYlQ1gGghm0_NNCKB0gCqYwVNn8,102
+whitebox_workflows-1.2.7.dist-info/license_files/LICENSE.txt,sha256=81hwVZcj5cV3fKP2h66KoD70cR90XP74jD7cZlItQ5g,161
+whitebox_workflows/whitebox_workflows.pyi,sha256=eFKrDmz-SqrwaNErFUJD6Xfz2AMA0Bt_4DH-zxaMo8A,89775
+whitebox_workflows/__init__.py,sha256=yXD2_p1-jqnIw8om04skAAIMppP5rkEIM8Uar3u0EL8,15070
+whitebox_workflows/scripts/horton_ratios.py,sha256=RsOgwJDauFdJZjJf9nZrG8WiEM8Bfkj2n9iRVqffXPA,8175
+whitebox_workflows/scripts/nibble.py,sha256=3T1sBsS2KzlLzz2MoOmmfrIecpkAfRitIYelK4Jn8cg,2108
+whitebox_workflows/scripts/ridge_and_valley_vectors.py,sha256=yWZIjIwqX6uPxNTkoSpYVYEBBnzaUGPhxay5SuJiQKg,1810
+whitebox_workflows/scripts/improved_ground_point_filter.py,sha256=D9StUawNQhX1BPPHMbR_6qmyT1OKneK3e107JAwlD00,1736
+whitebox_workflows/scripts/sieve.py,sha256=9VP8p2SuSwzAKeTrhmmRxGnzCBmWWqf0cnaCF4aajjY,942
 whitebox_workflows/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-whitebox_workflows/whitebox_workflows.pyi,sha256=mVXt9knGJC2_zylKvBd64C3lBlqTHm44Hrq6qer96b4,91516
-whitebox_workflows/__init__.py,sha256=49bgDqoMAqr6WEFXJyss-OqkQM3-Wu4dIl5r5SmnfN8,10952
-whitebox_workflows/whitebox_workflows.pyd,sha256=3sQeYqr15bNdNEbV63ACbFkud72ZM0CrE59m2ffoHEg,29894144
-whitebox_workflows-1.2.6.dist-info/RECORD,,
+whitebox_workflows/scripts/utils.py,sha256=la1yitl1Kf6LxlgnuNtu6E-HlIu_DGckOerFgtEog6k,872
+whitebox_workflows/scripts/scripts.py,sha256=YhyUrSm_YWqe6SZ8ZbV3edbG-0zWjkWLcxWgVAaShUU,1021
+whitebox_workflows/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+whitebox_workflows/whitebox_workflows.abi3.so,sha256=_VxvdIRkBKWpA753YUOnoOi55mFtxiFVXanPyjsN5V4,25697000
+whitebox_workflows-1.2.7.dist-info/RECORD,,
```

