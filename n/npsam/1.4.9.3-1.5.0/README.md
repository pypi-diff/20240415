# Comparing `tmp/npsam-1.4.9.3.tar.gz` & `tmp/npsam-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npsam-1.4.9.3.tar", last modified: Mon Apr 15 07:49:42 2024, max compression
+gzip compressed data, was "npsam-1.5.0.tar", last modified: Mon Apr 15 09:48:43 2024, max compression
```

## Comparing `npsam-1.4.9.3.tar` & `npsam-1.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.218246 npsam-1.4.9.3/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.9.3/LICENSE.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:49:42.217955 npsam-1.4.9.3/PKG-INFO
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.9.3/README.md
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.209325 npsam-1.4.9.3/npsam/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.4.9.3/npsam/__init__.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.212802 npsam-1.4.9.3/npsam/button_images/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11501 2024-04-14 18:07:35.000000 npsam-1.4.9.3/npsam/button_images/Save_close.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11524 2024-04-14 18:04:36.000000 npsam-1.4.9.3/npsam/button_images/Save_close_dark.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8142 2024-04-14 18:04:53.000000 npsam-1.4.9.3/npsam/button_images/arrow.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8037 2024-04-14 18:05:30.000000 npsam-1.4.9.3/npsam/button_images/arrow_dark.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15018 2024-04-14 18:06:27.000000 npsam-1.4.9.3/npsam/button_images/plus_all.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15098 2024-04-14 18:06:46.000000 npsam-1.4.9.3/npsam/button_images/plus_all_dark.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11171 2024-04-14 18:07:02.000000 npsam-1.4.9.3/npsam/button_images/plus_one.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11326 2024-04-14 18:07:18.000000 npsam-1.4.9.3/npsam/button_images/plus_one_dark.png
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    62035 2024-04-14 19:08:51.000000 npsam-1.4.9.3/npsam/npsam.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.213931 npsam-1.4.9.3/npsam/segment_anything/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/build_sam.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.216208 npsam-1.4.9.3/npsam/segment_anything/modeling/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/common.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/sam.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/predictor.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.217244 npsam-1.4.9.3/npsam/segment_anything/utils/
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/__init__.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/amg.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/onnx.py
--rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.9.3/npsam/segment_anything/utils/transforms.py
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.4.9.3/npsam/utils.py
-drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 07:49:42.217493 npsam-1.4.9.3/npsam.egg-info/
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15168 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/PKG-INFO
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1144 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/SOURCES.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/dependency_links.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/requires.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-15 07:49:42.000000 npsam-1.4.9.3/npsam.egg-info/top_level.txt
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1075 2024-04-15 07:49:20.000000 npsam-1.4.9.3/pyproject.toml
--rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-15 07:49:42.218317 npsam-1.4.9.3/setup.cfg
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.649452 npsam-1.5.0/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.5.0/LICENSE.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-15 09:48:43.649007 npsam-1.5.0/PKG-INFO
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.5.0/README.md
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.639731 npsam-1.5.0/npsam/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.5.0/npsam/__init__.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.643778 npsam-1.5.0/npsam/button_images/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11501 2024-04-14 18:07:35.000000 npsam-1.5.0/npsam/button_images/Save_close.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11524 2024-04-14 18:04:36.000000 npsam-1.5.0/npsam/button_images/Save_close_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8142 2024-04-14 18:04:53.000000 npsam-1.5.0/npsam/button_images/arrow.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     8037 2024-04-14 18:05:30.000000 npsam-1.5.0/npsam/button_images/arrow_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15018 2024-04-14 18:06:27.000000 npsam-1.5.0/npsam/button_images/plus_all.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15098 2024-04-14 18:06:46.000000 npsam-1.5.0/npsam/button_images/plus_all_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11171 2024-04-14 18:07:02.000000 npsam-1.5.0/npsam/button_images/plus_one.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    11326 2024-04-14 18:07:18.000000 npsam-1.5.0/npsam/button_images/plus_one_dark.png
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    61811 2024-04-15 09:48:01.000000 npsam-1.5.0/npsam/npsam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.644957 npsam-1.5.0/npsam/segment_anything/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/build_sam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.647202 npsam-1.5.0/npsam/segment_anything/modeling/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/common.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11688 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/predictor.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.648221 npsam-1.5.0/npsam/segment_anything/utils/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/utils/amg.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2024-04-14 18:58:50.000000 npsam-1.5.0/npsam/segment_anything/utils/transforms.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.5.0/npsam/utils.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-15 09:48:43.648580 npsam-1.5.0/npsam.egg-info/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-15 09:48:43.000000 npsam-1.5.0/npsam.egg-info/PKG-INFO
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1144 2024-04-15 09:48:43.000000 npsam-1.5.0/npsam.egg-info/SOURCES.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-15 09:48:43.000000 npsam-1.5.0/npsam.egg-info/dependency_links.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-15 09:48:43.000000 npsam-1.5.0/npsam.egg-info/requires.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-15 09:48:43.000000 npsam-1.5.0/npsam.egg-info/top_level.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1073 2024-04-15 09:48:30.000000 npsam-1.5.0/pyproject.toml
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-15 09:48:43.649516 npsam-1.5.0/setup.cfg
```

### Comparing `npsam-1.4.9.3/LICENSE.txt` & `npsam-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/PKG-INFO` & `npsam-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.9.3
+Version: 1.5.0
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.9.3/README.md` & `npsam-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/Save_close.png` & `npsam-1.5.0/npsam/button_images/Save_close.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/Save_close_dark.png` & `npsam-1.5.0/npsam/button_images/Save_close_dark.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/arrow.png` & `npsam-1.5.0/npsam/button_images/arrow.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/arrow_dark.png` & `npsam-1.5.0/npsam/button_images/arrow_dark.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/plus_all.png` & `npsam-1.5.0/npsam/button_images/plus_all.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/plus_all_dark.png` & `npsam-1.5.0/npsam/button_images/plus_all_dark.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/plus_one.png` & `npsam-1.5.0/npsam/button_images/plus_one.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/button_images/plus_one_dark.png` & `npsam-1.5.0/npsam/button_images/plus_one_dark.png`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/npsam.py` & `npsam-1.5.0/npsam/npsam.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         self.min_intensity = None
         self.max_intensity = None
         self.min_eccentricity = None
         self.max_eccentricity = None
         self.max_overlap = None
         self.overlapping_masks = None
         self.overlapping_masks_dict = {'All': "Not applied", '0': 0, '1': 2, '2': 3}
-        self.removed_index = []
+        # self.removed_index = []
 
         self.ax_slider_area = None
         self.unit = None
         self.ax_slider_solidity = None
         self.ax_slider_intensity = None
         self.ax_slider_eccentricity = None
         self.ax_slider_overlap = None
@@ -527,16 +527,15 @@
 
         self.directory = Path(__file__).resolve().parent / 'button_images'
 
     def get_df_params(self):
         return ((self.df['area'] >= self.min_area) & (self.df['area'] <= self.max_area) &
                 (self.df['solidity'] >= self.min_solidity) & (self.df['solidity'] <= self.max_solidity) &
                 (self.df['intensity_mean'] >= self.min_intensity) & (self.df['intensity_mean'] <= self.max_intensity) &
-                (self.df['eccentricity'] >= self.min_eccentricity) & (
-                            self.df['eccentricity'] <= self.max_eccentricity) &
+                (self.df['eccentricity'] >= self.min_eccentricity) & (self.df['eccentricity'] <= self.max_eccentricity) &
                 (~self.df['mask_index'].isin(self.removed_index)) &
                 (self.df['number_of_overlapping_masks'] == self.overlapping_masks if type(self.overlapping_masks) == int
                  else self.df['number_of_overlapping_masks'] >= 0) & (self.df['overlap'] <= self.max_overlap))
 
     def plot_df(self, df):
         mask_indices = df.index.to_numpy().astype(np.uint16)
 
@@ -763,16 +762,18 @@
             'min_intensity': self.min_intensity,
             'max_intensity': self.max_intensity,
             'min_eccentricity': self.min_eccentricity,
             'max_eccentricity': self.max_eccentricity,
             'scaling': self.df['scaling [px/unit]'].to_list()[0],
             'overlap': self.max_overlap,
             'overlapping_masks': self.overlapping_masks,
+            'removed_list': self.removed_index,
             'removed': self.df.shape[0] - df_filtered.shape[0],
             'remain': df_filtered.shape[0],
+
         }
 
         self.file_p = self.files_folder / (Path(self.filepath).stem + '_filtered_dataframe.csv')
         df_filtered.to_csv(self.file_p, encoding='utf-8', header='true', index=False)
         save_dictionary(str(self.filepath), filters)
 
         self.filtered_label_image = np.zeros(self.weighted_masks[0].shape)
@@ -811,60 +812,55 @@
         self.slider_area = RangeSlider(ax, '', valmin=self.min_area, valmax=self.max_area, valstep=1,
                                        valinit=(self.min_area_init, self.max_area_init))
         self.slider_area.on_changed(self.update_area)
 
         self.area_val_text = ax.text(0, 1.12, f"Area ({self.unit2}): ({self.min_area}, {self.max_area})",
                                      fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_area.valtext.set_visible(False)
-        self.update_area((self.min_area_init, self.max_area_init))
 
     def create_solidity_slider(self, ax):
         self.slider_solidity = RangeSlider(ax, "", valmin=self.min_solidity, valmax=self.max_solidity, valstep=0.001,
                                            valinit=(self.min_solidity_init, self.max_solidity_init))
         self.slider_solidity.on_changed(self.update_solidity)
 
         self.solidity_val_text = ax.text(0, 1.12, f"Solidity: ({self.min_solidity:.3f}, {self.max_solidity:.3f})",
                                          fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_solidity.valtext.set_visible(False)
-        self.update_solidity((self.min_solidity_init, self.max_solidity_init))
 
     def create_intensity_slider(self, ax):
         self.slider_intensity = RangeSlider(ax, "", valmin=self.min_intensity, valmax=self.max_intensity,
                                             valstep=1, valinit=(self.min_intensity_init, self.max_intensity_init))
         self.slider_intensity.on_changed(self.update_intensity)
 
         self.intensity_val_text = ax.text(0, 1.12, f"Intensity slider: ({self.min_intensity}, {self.max_intensity})",
                                           fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_intensity.valtext.set_visible(False)
-        self.update_intensity((self.min_intensity_init, self.max_intensity_init))
 
     def create_eccentricity_slider(self, ax):
         self.slider_eccentricity = RangeSlider(ax, "", valmin=self.min_eccentricity, valmax=self.max_eccentricity,
                                                valstep=0.01,
                                                valinit=(self.min_eccentricity_init, self.max_eccentricity_init))
         self.slider_eccentricity.on_changed(self.update_eccentricity)
 
         self.eccentricity_val_text = ax.text(0, 1.12,
                                              f"Eccentricity: ({self.min_eccentricity:.2f}, {self.max_eccentricity:.2f})",
                                              fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_eccentricity.valtext.set_visible(False)
-        self.update_eccentricity((self.min_eccentricity_init, self.max_eccentricity_init))
 
     def create_overlap_slider(self, ax):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
             self.slider_overlap = Slider(ax, '', valmin=0, valmax=self.max_overlap, valstep=1,
                                          valinit=self.max_overlap_init)
             self.slider_overlap.on_changed(self.update_overlap)
 
             self.overlap_val_text = ax.text(0, 1.12, f"Overlap: {self.max_overlap}",
                                             fontsize=14, ha='left', va='center', transform=ax.transAxes)
             self.slider_overlap.valtext.set_visible(False)
             self.slider_overlap.vline._linewidth = 0
-            self.update_overlap(self.max_overlap_init)
 
     def create_overlapping_masks_radio(self, ax):
         ax.set_aspect('equal')
         if type(self.overlapping_masks_init) == str:
             self.overlapping_masks_init = -1
         elif self.overlapping_masks_init > 2:
             self.overlapping_masks_init = -1
@@ -882,38 +878,47 @@
             label.set_position((new_x + 0.03, new_y))
             label.set_fontsize(14)
 
         self.overlapping_masks_val_text = ax.text(0, 0.5, "Number of overlapping masks:",
                                                   fontsize=14, ha='left', va='center', transform=ax.transAxes)
 
         self.radio_overlapping_masks.on_clicked(self.update_overlapping_masks)
-        self.update_overlapping_masks(['All', '0', '1', '2'][self.overlapping_masks_init + 1])
 
     def initiate_filter_values(self):
         self.min_area_init = self.min_area
         self.max_area_init = self.max_area
         self.min_solidity_init = self.min_solidity
         self.max_solidity_init = self.max_solidity
         self.min_intensity_init = self.min_intensity
         self.max_intensity_init = self.max_intensity
         self.min_eccentricity_init = self.min_eccentricity
         self.max_eccentricity_init = self.max_eccentricity
         self.max_overlap_init = self.max_overlap
         self.overlapping_masks_init = self.overlapping_masks
+        self.removed_index = []
         if 'min_area' in self.filters_init.keys():
             self.min_area_init = self.filters_init['min_area']
             self.max_area_init = self.filters_init['max_area']
             self.min_solidity_init = self.filters_init['min_solidity']
             self.max_solidity_init = self.filters_init['max_solidity']
             self.min_intensity_init = self.filters_init['min_intensity']
             self.max_intensity_init = self.filters_init['max_intensity']
             self.min_eccentricity_init = self.filters_init['min_eccentricity']
             self.max_eccentricity_init = self.filters_init['max_eccentricity']
             self.max_overlap_init = self.filters_init['overlap']
             self.overlapping_masks_init = self.filters_init['overlapping_masks']
+            self.removed_index = self.filters_init['removed_list']
+
+
+        df_init = self.df.loc[self.get_df_params()]
+
+        self.plot_text(df_init)
+
+        self.plot_df(df_init)
+
 
     def start_plot(self, image, labels):
         self.fig, self.ax = plt.subplot_mosaic([['left', 'right'], ['left2', 'right2'], ['.', '.']],
                                                gridspec_kw=dict(height_ratios=[1, 1, 0.1]),
                                                constrained_layout=True, figsize=(12, 10))
 
         self.ax['left'].imshow(image, cmap='gray')
```

### Comparing `npsam-1.4.9.3/npsam/segment_anything/automatic_mask_generator.py` & `npsam-1.5.0/npsam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/build_sam.py` & `npsam-1.5.0/npsam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/common.py` & `npsam-1.5.0/npsam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/image_encoder.py` & `npsam-1.5.0/npsam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/mask_decoder.py` & `npsam-1.5.0/npsam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/prompt_encoder.py` & `npsam-1.5.0/npsam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/sam.py` & `npsam-1.5.0/npsam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/modeling/transformer.py` & `npsam-1.5.0/npsam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/predictor.py` & `npsam-1.5.0/npsam/segment_anything/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import numpy as np
 import torch
 
-from segment_anything.modeling import Sam
+# Original: from .segment_anything.modeling import Sam
+from .modeling import Sam
 
 from typing import Optional, Tuple
 
 from .utils.transforms import ResizeLongestSide
 
 
 class SamPredictor:
```

### Comparing `npsam-1.4.9.3/npsam/segment_anything/utils/amg.py` & `npsam-1.5.0/npsam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/utils/onnx.py` & `npsam-1.5.0/npsam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/segment_anything/utils/transforms.py` & `npsam-1.5.0/npsam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam/utils.py` & `npsam-1.5.0/npsam/utils.py`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/npsam.egg-info/PKG-INFO` & `npsam-1.5.0/npsam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npsam
-Version: 1.4.9.3
+Version: 1.5.0
 Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
 Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `npsam-1.4.9.3/npsam.egg-info/SOURCES.txt` & `npsam-1.5.0/npsam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npsam-1.4.9.3/pyproject.toml` & `npsam-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 "npsam.button_images" = ["*.png"]
 
 [project]
 name = "npsam"
-version = "1.4.9.3"
+version = "1.5.0"
 dependencies = [
     "numba==0.58.1",
     "opencv-python==4.9.0.80",
     "pandas==2.1.4",
     "matplotlib==3.8.2",
     "scikit-image==0.22.0",
     "ipympl==0.9.3",
```

