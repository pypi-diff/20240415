# Comparing `tmp/bblib-1.2.0.tar.gz` & `tmp/bblib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-1.2.0.tar", max compression
+gzip compressed data, was "bblib-1.2.1.tar", max compression
```

## Comparing `bblib-1.2.0.tar` & `bblib-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-04-12 16:41:40.239125 bblib-1.2.0/LICENSE
--rw-r--r--   0        0        0     3753 2024-04-12 16:41:40.239125 bblib-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/__init__.py
--rwxr-xr-x   0        0        0    35521 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/methods.py
--rwxr-xr-x   0        0        0     9185 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/models.py
--rwxr-xr-x   0        0        0    19615 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-04-12 16:41:49.919210 bblib-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-04-15 09:19:19.691922 bblib-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3753 2024-04-15 09:19:19.691922 bblib-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/__init__.py
+-rwxr-xr-x   0        0        0    35521 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/methods.py
+-rwxr-xr-x   0        0        0     9226 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/models.py
+-rwxr-xr-x   0        0        0    18198 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-04-15 09:19:29.111997 bblib-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-1.2.1/PKG-INFO
```

### Comparing `bblib-1.2.0/LICENSE` & `bblib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-1.2.0/README.md` & `bblib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bblib-1.2.0/bblib/methods.py` & `bblib-1.2.1/bblib/methods.py`

 * *Files identical despite different names*

### Comparing `bblib-1.2.0/bblib/models.py` & `bblib-1.2.1/bblib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     GeometryInformation,
     _read_crystfel_geometry_from_text,
 )
 
 
 @dataclass
 class PF8Info:
-    max_num_peaks: np.int32
-    adc_threshold: np.int32
-    minimum_snr: np.float32
-    min_pixel_count: np.int16
-    max_pixel_count: np.int16
-    local_bg_radius: np.int16
-    min_res: np.int16
-    max_res: np.int16
+    max_num_peaks: np.int32 = 200
+    adc_threshold: np.int32 = 0
+    minimum_snr: np.float32 = 5
+    min_pixel_count: np.int16 = 2
+    max_pixel_count: np.int16 = 2000
+    local_bg_radius: np.int16 = 3
+    min_res: np.int16 = 0 
+    max_res: np.int16 = 1200
     pf8_detector_info: TypeDetectorLayoutInformation = None
     bad_pixel_map_filename: str = None
     bad_pixel_map_hdf5_path: str = None
     pixel_maps: TypePixelMaps = None
     pixel_resolution: float = None
     _shifted_pixel_maps: bool = False
     geometry_txt: list = None
```

### Comparing `bblib-1.2.0/bblib/utils.py` & `bblib-1.2.1/bblib/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -441,62 +441,27 @@
         ax3.set_title("Distance projection in y")
         ax3.legend()
         fig.colorbar(pos1, ax=ax1, shrink=0.6)
     else:
         converged = 0
         xc = -1
         yc = -1
-        
+
     if int(np.sum(proj_y)) == 0 or int(np.sum(proj_x)) == 0:
         converged = 0
         xc = -1
         yc = -1
     else:
         converged = 1
         if plots_flag:
             plt.savefig(f"{output_folder}/distance_map/{label}.png")
     plt.close()
     return [np.round(xc, 1), np.round(yc, 1)]
 
 
-def shift_image_by_n_pixels(data: np.ndarray, n: int, axis: int) -> np.ndarray:
-    """
-    Linear translation of image by n pixels in given axis. Empty values in the shifted image is filled with zero.
-
-    Parameters
-    ----------
-    data: np.ndarray
-        Input image to be shifted
-    n: int
-        Number of pixels to be shifted.
-    axis: int
-        Axis in which the image will be shifted. Axis 0 corresponds to a shift in the rows (y-axis), axis 1 shifts in the columns (x-axis).
-    Returns
-    ----------
-    shifted_data: np.ndarray
-        Data shifted by n pixels in axis.
-    """
-    max_row, max_col = data.shape
-    # print(max_row,max_col)
-    if axis == 1 and n >= 0:
-        shifted_data = np.pad(data, pad_width=[(0, 0), (abs(n), 0)], mode="constant")
-        image_cut = shifted_data[:max_row, :max_col]
-    elif axis == 1 and n < 0:
-        shifted_data = np.pad(data, pad_width=[(0, 0), (0, abs(n))], mode="constant")
-        image_cut = shifted_data[:max_row, abs(n) :]
-    elif axis == 0 and n >= 0:
-        shifted_data = np.pad(data, pad_width=[(abs(n), 0), (0, 0)], mode="constant")
-        image_cut = shifted_data[:max_row, :max_col]
-    elif axis == 0 and n < 0:
-        shifted_data = np.pad(data, pad_width=[(0, abs(n)), (0, 0)], mode="constant")
-        image_cut = shifted_data[abs(n) :, :max_col]
-    # print("Image cut shape", image_cut.shape)
-    return image_cut
-
-
 def circle_mask(data: np.ndarray, center: tuple, radius: int) -> np.ndarray:
     """
     Make a  ring mask for the data
 
     Parameters
     ----------
     data: np.ndarray
```

### Comparing `bblib-1.2.0/pyproject.toml` & `bblib-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "1.2.0"
+version = "1.2.1"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-1.2.0/PKG-INFO` & `bblib-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 1.2.0
+Version: 1.2.1
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

