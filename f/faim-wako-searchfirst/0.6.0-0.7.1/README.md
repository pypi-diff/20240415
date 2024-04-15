# Comparing `tmp/faim_wako_searchfirst-0.6.0.tar.gz` & `tmp/faim_wako_searchfirst-0.7.1.tar.gz`

## Comparing `faim_wako_searchfirst-0.6.0.tar` & `faim_wako_searchfirst-0.7.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/config.yml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/config_cellpose.yml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0   167410 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/presentations/faim-wako-searchfirst_overview.pdf
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/presentations/faim-wako-searchfirst_overview.pdf.license
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/scripts/Visualize_Sampling.groovy
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/scripts/searchfirst.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/filter.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/main.py
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/sample.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/segment.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/test_cellpose.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/test_main.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/test_sample.py
--rw-r--r--   0        0        0    43316 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/simple_labels.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/simple_labels.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif.license
--rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif.license
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/.gitignore
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/README.md
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/config.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/config_cellpose.yml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0   167410 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf.license
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/scripts/Visualize_Sampling.groovy
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/scripts/searchfirst.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/__init__.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/filter.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/main.py
+-rw-r--r--   0        0        0     7736 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/sample.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/segment.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_cellpose.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_filter.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_main.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/test_sample.py
+-rw-r--r--   0        0        0    43316 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif.license
+-rw-r--r--   0        0        0    65696 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif.license
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/.gitignore
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/README.md
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 faim_wako_searchfirst-0.7.1/PKG-INFO
```

### Comparing `faim_wako_searchfirst-0.6.0/config_cellpose.yml` & `faim_wako_searchfirst-0.7.1/config_cellpose.yml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/.github/workflows/deploy.yml` & `faim_wako_searchfirst-0.7.1/.github/workflows/deploy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -41,12 +41,12 @@
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: artifacts
         path: dist
 
     - name: Push build artifacts to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.6.4
+      uses: pypa/gh-action-pypi-publish@v1.8.14
       with:
         skip_existing: true
         user: __token__
         password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `faim_wako_searchfirst-0.6.0/.github/workflows/test.yml` & `faim_wako_searchfirst-0.7.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/LICENSES/MIT.txt` & `faim_wako_searchfirst-0.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/presentations/faim-wako-searchfirst_overview.pdf` & `faim_wako_searchfirst-0.7.1/presentations/faim-wako-searchfirst_overview.pdf`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/scripts/Visualize_Sampling.groovy` & `faim_wako_searchfirst-0.7.1/scripts/Visualize_Sampling.groovy`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/scripts/searchfirst.py` & `faim_wako_searchfirst-0.7.1/scripts/searchfirst.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Friedrich Miescher Institute for Biomedical Research (FMI), Basel (Switzerland)
 #
 # SPDX-License-Identifier: MIT
 
 """SearchFirst script to run a simple segmentation."""
+
 import typer
 from faim_wako_searchfirst.main import run
 
 
 def main(folder_path: str):
     """Segment images in the given acquisition folder.
```

### Comparing `faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/main.py` & `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/main.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/sample.py` & `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/sample.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 """
 
 import csv
 from pathlib import Path
 
 import numpy as np
 from numpy import ndarray
-from skimage.measure import block_reduce, regionprops
+from skimage.filters.rank import maximum
+from skimage.measure import block_reduce, label, regionprops
+from skimage.morphology import rectangle
 
 
 def dense_grid(
     labels: ndarray,
     output_path: Path,
     binning_factor: int = 50,
 ):
@@ -26,22 +28,22 @@
         block_size=(binning_factor, binning_factor),
         func=np.max,
     )
     with open(output_path, "w", newline="") as csv_file:
         c = csv.writer(csv_file)
         count = 0
         it = np.nditer(downscaled, flags=["multi_index"])
-        for label in it:
-            if label > 0:
+        for label_value in it:
+            if label_value > 0:
                 c.writerow([count] + _grid_coordinate(it.multi_index, binning_factor))
                 count += 1
 
 
 def _grid_coordinate(index, factor):
-    return [(index[1] + 0.5) * factor, (index[0] + 0.5) * factor]
+    return [(index[1] + 0.5) * factor, (index[0] + 0.5) * factor]  # TODO add 0.5 here?
 
 
 def grid_overlap(
     labeled_img: ndarray,
     path,
     mag_first_pass,
     mag_second_pass,
@@ -93,35 +95,19 @@
         within_threshold[i] = False
         if np.any(within_threshold):
             less_weight_indices = np.where((weights < weights[i]) & within_threshold)[0]
             keep_indices[less_weight_indices] = False
     return keep_indices
 
 
-def object_centered_grid(
+def _sample_grid_on_regions(
     labeled_img: ndarray,
-    path: Path,
-    mag_first_pass: float,
-    mag_second_pass: float,
-    overlap_ratio: float = 0.0,
+    tile_size_y: float,
+    tile_size_x: float,
 ):
-    """Sample each labeled object with a centered grid of tiles.
-
-    If the object fits into a single field of view, record just the centroid coordinate.
-    Otherwise, compute how many tiles are required to fit the object, and record only
-    those grid coordinates that cover the object mask.
-
-    For objects where the resulting fields of view would be overlapping,
-    only keep the largest object and discard all others.
-    """
-    factor = mag_first_pass / mag_second_pass
-    shift_percent = 1.0 - overlap_ratio
-    tile_size_y = labeled_img.shape[0] * factor * shift_percent
-    tile_size_x = labeled_img.shape[1] * factor * shift_percent
-
     props = regionprops(label_image=labeled_img)
     labels = []
     coordinates = []
     areas = []
     # loop over labels (and sort by descending size?)
     for p in props:
         # compute bounding box of label
@@ -148,24 +134,90 @@
 
             if np.any(labeled_img[y_min:y_max, x_min:x_max] == p.label):
                 valid_points.append((y, x))
 
         coordinates.extend(valid_points)
         areas.extend([p.area] * len(valid_points))
         labels.extend([p.label] * len(valid_points))
+    return coordinates, areas, labels
+
+
+def object_centered_grid(
+    labeled_img: ndarray,
+    path: Path,
+    mag_first_pass: float,
+    mag_second_pass: float,
+    overlap_ratio: float = 0.0,
+):
+    """Sample each labeled object with a centered grid of tiles.
+
+    If the object fits into a single field of view, record just the centroid coordinate.
+    Otherwise, compute how many tiles are required to fit the object, and record only
+    those grid coordinates that cover the object mask.
+
+    For objects where the resulting fields of view would be overlapping,
+    only keep the largest object and discard all others.
+    """
+    factor = mag_first_pass / mag_second_pass
+    shift_percent = 1.0 - overlap_ratio
+    tile_size_y = labeled_img.shape[0] * factor * shift_percent
+    tile_size_x = labeled_img.shape[1] * factor * shift_percent
+
+    coordinates, areas, labels = _sample_grid_on_regions(
+        labeled_img=labeled_img,
+        tile_size_y=tile_size_y,
+        tile_size_x=tile_size_x,
+    )
 
     # filter overlapping coordinates
     keep_points = _filter_points(
         points=coordinates,
         weights=areas,
         y_threshold=tile_size_y,
         x_threshold=tile_size_x,
     )
 
     coordinates = np.array(coordinates)[keep_points]
-    areas = np.array(areas)[keep_points]
     labels = np.array(labels)[keep_points]
 
     with open(path, "w", newline="") as csv_file:
         c = csv.writer(csv_file)
-        for label, point in zip(labels, coordinates):
-            c.writerow([label, point[1], point[0]])
+        for label_value, point in zip(labels, coordinates):
+            c.writerow([label_value, *reversed(point)])
+
+
+def region_centered_grid(
+    labeled_img: ndarray,
+    path: Path,
+    mag_first_pass: float,
+    mag_second_pass: float,
+    overlap_ratio: float = 0.0,
+):
+    """Sample optimal grid for each region of objects that are close to each other.
+
+    The grid is computed centered on each region, with an optional specified overlap.
+    """
+    factor = mag_first_pass / mag_second_pass
+    shift_percent = 1.0 - overlap_ratio
+    tile_size_y = labeled_img.shape[0] * factor * shift_percent
+    tile_size_x = labeled_img.shape[1] * factor * shift_percent
+    # dilate
+    mask = labeled_img > 0
+    footprint = rectangle(
+        np.ceil(tile_size_y).astype(int), np.ceil(tile_size_x).astype(int)
+    )  # , decomposition="separable"
+    dilated = maximum(image=mask.astype(np.uint8), footprint=footprint)
+    # label
+    regions = label(dilated)
+    # reconstruct
+    reconstructed = np.where(mask, regions, 0)
+
+    coordinates, _, labels = _sample_grid_on_regions(
+        labeled_img=reconstructed,
+        tile_size_y=tile_size_y,
+        tile_size_x=tile_size_x,
+    )
+
+    with open(path, "w", newline="") as csv_file:
+        c = csv.writer(csv_file)
+        for label_value, point in zip(labels, coordinates):
+            c.writerow([label_value, *reversed(point)])
```

### Comparing `faim_wako_searchfirst-0.6.0/src/faim_wako_searchfirst/segment.py` & `faim_wako_searchfirst-0.7.1/src/faim_wako_searchfirst/segment.py`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/tests/test_cellpose.py` & `faim_wako_searchfirst-0.7.1/tests/test_cellpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Friedrich Miescher Institute for Biomedical Research (FMI), Basel (Switzerland)
 #
 # SPDX-License-Identifier: MIT
 
 """Test faim_wako_searchfirst module."""
+
 import csv
 import shutil
 from pathlib import Path
 
 import pytest
 from faim_wako_searchfirst.main import run
```

### Comparing `faim_wako_searchfirst-0.6.0/tests/test_main.py` & `faim_wako_searchfirst-0.7.1/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Friedrich Miescher Institute for Biomedical Research (FMI), Basel (Switzerland)
 #
 # SPDX-License-Identifier: MIT
 
 """Test faim_wako_searchfirst module."""
+
 import csv
 import shutil
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pytest
```

### Comparing `faim_wako_searchfirst-0.6.0/tests/resources/simple_labels.tif` & `faim_wako_searchfirst-0.7.1/tests/resources/simple_labels.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif` & `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/Other_name_D07_T0001F002L01A02Z01C01.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif` & `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_C03_T0001F002L01A03Z01C03.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif` & `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A02Z01C01.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif` & `faim_wako_searchfirst-0.7.1/tests/resources/TestSet/TestSet_D07_T0001F002L01A03Z01C03.tif`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/README.md` & `faim_wako_searchfirst-0.7.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -29,40 +29,75 @@
 
 ## Usage
 
 Configuration is managed in a `config.yml` file:
 
 ```yaml
 # Required
-file_selection:  # criteria for file selection in case of multiple channels/slices per position
+
+# criteria for file selection in case of multiple channels/slices per position
+file_selection:
     channel: C01
-process:  # choose method how to segment, filter, and sample the objects
-    segment: threshold  # choices: threshold, cellpose
-    filter: [bounding_box, area, solidity, intensity]
-    sample: centers  # choices: centers, grid_overlap, dense_grid
 
-# Each subsequent section provides arguments to one of the methods defined in 'process'
+# choose method how to segment, filter, and sample the objects
+process:
+    # segment methods: threshold, cellpose
+    segment: threshold
+    # filter methods: bounding_box, area, solidity, intensity
+    filter: [bounding_box, area, solidity, feature, dilate, intensity]
+    # sample methods: centers, grid_overlap, dense_grid,
+    #                 object_centered_grid, region_centered_grid
+    sample: centers
+
+# Each section below provides arguments to one of the methods set in 'process'.
+# Config sections for methods not selected above will be ignored.
+
+# segment
 threshold:
     threshold: 128
-    include_holes: yes
-    gaussian_sigma: 2.0 # optional 
+    include_holes: true
+    gaussian_sigma: 0.0  # default: 0.0
+
+# filter
 bounding_box:
     min_x: 64
     min_y: 0
     max_x: 256
     max_y: 190
 area:
     min_area: 100
     max_area: 10000
 solidity:
     min_solidity: 0.9
     max_solidity: 1.0
+feature:
+    feature: eccentricity
+    min_value: 0.0
+    max_value: 0.99
+dilate:
+    pixel_distance: 1.0
 intensity:
     target_channel: C03
     min_intensity: 128
+
+# sample
+dense_grid:
+    binning_factor: 50  # default: 50
+grid_overlap:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
+object_centered_grid:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
+region_centered_grid:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
 ```
 
 The Python script called by Wako Automation Software needs to accept the acquisition folder `folder_path` as only parameter:
 
 ```python
 import typer
 from faim_wako_searchfirst.main import run
```

### Comparing `faim_wako_searchfirst-0.6.0/pyproject.toml` & `faim_wako_searchfirst-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faim_wako_searchfirst-0.6.0/PKG-INFO` & `faim_wako_searchfirst-0.7.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: faim-wako-searchfirst
-Version: 0.6.0
+Version: 0.7.1
 Project-URL: Documentation, https://github.com/fmi-faim/faim-wako-searchfirst#readme
 Project-URL: Issues, https://github.com/fmi-faim/faim-wako-searchfirst/issues
 Project-URL: Source, https://github.com/fmi-faim/faim-wako-searchfirst
 Author-email: Jan Eglinger <jan.eglinger@fmi.ch>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -54,40 +54,75 @@
 
 ## Usage
 
 Configuration is managed in a `config.yml` file:
 
 ```yaml
 # Required
-file_selection:  # criteria for file selection in case of multiple channels/slices per position
+
+# criteria for file selection in case of multiple channels/slices per position
+file_selection:
     channel: C01
-process:  # choose method how to segment, filter, and sample the objects
-    segment: threshold  # choices: threshold, cellpose
-    filter: [bounding_box, area, solidity, intensity]
-    sample: centers  # choices: centers, grid_overlap, dense_grid
 
-# Each subsequent section provides arguments to one of the methods defined in 'process'
+# choose method how to segment, filter, and sample the objects
+process:
+    # segment methods: threshold, cellpose
+    segment: threshold
+    # filter methods: bounding_box, area, solidity, intensity
+    filter: [bounding_box, area, solidity, feature, dilate, intensity]
+    # sample methods: centers, grid_overlap, dense_grid,
+    #                 object_centered_grid, region_centered_grid
+    sample: centers
+
+# Each section below provides arguments to one of the methods set in 'process'.
+# Config sections for methods not selected above will be ignored.
+
+# segment
 threshold:
     threshold: 128
-    include_holes: yes
-    gaussian_sigma: 2.0 # optional 
+    include_holes: true
+    gaussian_sigma: 0.0  # default: 0.0
+
+# filter
 bounding_box:
     min_x: 64
     min_y: 0
     max_x: 256
     max_y: 190
 area:
     min_area: 100
     max_area: 10000
 solidity:
     min_solidity: 0.9
     max_solidity: 1.0
+feature:
+    feature: eccentricity
+    min_value: 0.0
+    max_value: 0.99
+dilate:
+    pixel_distance: 1.0
 intensity:
     target_channel: C03
     min_intensity: 128
+
+# sample
+dense_grid:
+    binning_factor: 50  # default: 50
+grid_overlap:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
+object_centered_grid:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
+region_centered_grid:
+    mag_first_pass: 4
+    mag_second_pass: 60
+    overlap_ratio: 0.05  # default: 0
 ```
 
 The Python script called by Wako Automation Software needs to accept the acquisition folder `folder_path` as only parameter:
 
 ```python
 import typer
 from faim_wako_searchfirst.main import run
```

