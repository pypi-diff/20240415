# Comparing `tmp/unravel-python-1.4.9.tar.gz` & `tmp/unravel_python-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.4.9.tar", last modified: Thu Nov  2 13:53:31 2023, max compression
+gzip compressed data, was "unravel_python-1.5.0.tar", last modified: Mon Apr 15 15:22:42 2024, max compression
```

## Comparing `unravel-python-1.4.9.tar` & `unravel_python-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-02 13:53:31.580000 unravel-python-1.4.9/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.4.9/LICENSE
--rw-rw-rw-   0        0        0     4515 2023-11-02 13:53:32.000000 unravel-python-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3801 2023-08-05 19:56:16.000000 unravel-python-1.4.9/README.md
--rw-rw-rw-   0        0        0      970 2023-08-28 14:41:42.000000 unravel-python-1.4.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-02 13:53:32.000000 unravel-python-1.4.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-02 13:53:31.580000 unravel-python-1.4.9/src/
-drwxrwxrwx   0        0        0        0 2023-11-02 13:53:31.590000 unravel-python-1.4.9/src/unravel/
--rw-rw-rw-   0        0        0      358 2023-11-02 13:49:40.000000 unravel-python-1.4.9/src/unravel/__init__.py
--rw-rw-rw-   0        0        0     2603 2023-10-31 15:26:40.000000 unravel-python-1.4.9/src/unravel/analysis.py
--rw-rw-rw-   0        0        0    44450 2023-09-13 14:23:10.000000 unravel-python-1.4.9/src/unravel/core.py
--rw-rw-rw-   0        0        0     4547 2023-09-07 08:09:14.000000 unravel-python-1.4.9/src/unravel/example.py
--rw-rw-rw-   0        0        0    20097 2023-11-02 12:56:36.000000 unravel-python-1.4.9/src/unravel/stream.py
--rw-rw-rw-   0        0        0    15026 2023-10-31 15:26:40.000000 unravel-python-1.4.9/src/unravel/utils.py
--rw-rw-rw-   0        0        0    15386 2023-10-31 15:26:40.000000 unravel-python-1.4.9/src/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-11-02 13:53:31.590000 unravel-python-1.4.9/src/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     4515 2023-11-02 13:53:32.000000 unravel-python-1.4.9/src/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-11-02 13:53:32.000000 unravel-python-1.4.9/src/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-02 13:53:32.000000 unravel-python-1.4.9/src/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-11-02 13:53:32.000000 unravel-python-1.4.9/src/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-02 13:53:32.000000 unravel-python-1.4.9/src/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.380000 unravel_python-1.5.0/
+-rw-rw-rw-   0        0        0    35823 2024-02-01 10:17:26.000000 unravel_python-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4515 2024-04-15 15:22:44.000000 unravel_python-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3801 2024-02-01 10:17:26.000000 unravel_python-1.5.0/README.md
+-rw-rw-rw-   0        0        0      970 2024-02-01 10:17:26.000000 unravel_python-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 15:22:44.000000 unravel_python-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.380000 unravel_python-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.390000 unravel_python-1.5.0/src/unravel/
+-rw-rw-rw-   0        0        0      358 2024-04-15 15:22:00.000000 unravel_python-1.5.0/src/unravel/__init__.py
+-rw-rw-rw-   0        0        0     3038 2024-02-21 12:39:26.000000 unravel_python-1.5.0/src/unravel/analysis.py
+-rw-rw-rw-   0        0        0    44450 2024-02-01 10:17:26.000000 unravel_python-1.5.0/src/unravel/core.py
+-rw-rw-rw-   0        0        0     4547 2024-02-21 12:33:42.000000 unravel_python-1.5.0/src/unravel/example.py
+-rw-rw-rw-   0        0        0    20774 2024-03-11 14:32:18.000000 unravel_python-1.5.0/src/unravel/stream.py
+-rw-rw-rw-   0        0        0    15988 2024-04-15 14:45:40.000000 unravel_python-1.5.0/src/unravel/utils.py
+-rw-rw-rw-   0        0        0    20577 2024-04-15 15:01:06.000000 unravel_python-1.5.0/src/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:22:42.390000 unravel_python-1.5.0/src/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     4515 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 15:22:44.000000 unravel_python-1.5.0/src/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.4.9/LICENSE` & `unravel_python-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.4.9/PKG-INFO` & `unravel_python-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.4.9
+Version: 1.5.0
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel-python-1.4.9/README.md` & `unravel_python-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.4.9/pyproject.toml` & `unravel_python-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unravel-python-1.4.9/src/unravel/analysis.py` & `unravel_python-1.5.0/src/unravel/analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,90 +6,99 @@
 """
 
 import numpy as np
 from itertools import combinations
 from unravel.core import get_microstructure_map, get_weighted_mean
 
 
-def get_metric_along_trajectory(fixel_weights, metric_maps: list, roi_sections):
+def get_metric_along_trajectory(fixel_weights, metric_maps, roi_sections,
+                                weighting: str = 'tsl'):
     '''
 
 
     Parameters
     ----------
     fixel_weights : 4-D array of shape (x,y,z,K)
         Array containing the relative weights of the K fixels in each voxel.
-    metric_maps : list
-        List of K 3-D arrays of shape (x,y,z) containing metric estimations.
+    metric_maps : 4D array of shape (x,y,z,3,k)
+        List of K 4D arrays of shape (x,y,z) containing metric estimations.
     roi_sections : 3D array of size (x,y,z)
         Labeled array containing the volumes of the section of the tract.
+    weighting : str, optional
+        Weighting used for the mean. The default is 'tsl'.
 
     Returns
     -------
     m_array : 1D array of size (n)
         DESCRIPTION.
     std_array : 1D array of size (n)
         DESCRIPTION.
 
     '''
 
-    m_array = np.zeros(np.max(roi_sections))
-    std_array = np.zeros(np.max(roi_sections))
+    m_array = np.zeros(np.max(roi_sections)+1)
+    std_array = np.zeros(np.max(roi_sections)+1)
 
-    if len(metric_maps) == 1:
+    if len(metric_maps.shape) <= 3:
         fixel_weights = fixel_weights[..., np.newaxis]
 
     micro_map = get_microstructure_map(fixel_weights, metric_maps)
 
-    for i in range(np.max(roi_sections)):
+    for i in range(np.max(roi_sections)+1):
 
         if i == 0:
             continue
 
         roi = np.where(roi_sections == i, 1, 0)
-        fixel_weights_roi = fixel_weights * np.repeat(roi[..., np.newaxis],
-                                                      1, axis=-1)
+        fixel_weights_roi = fixel_weights * roi[..., np.newaxis]
 
-        mean, std = get_weighted_mean(micro_map, fixel_weights_roi)
+        mean, std = get_weighted_mean(micro_map, fixel_weights_roi,
+                                      weighting=weighting)
         if mean == 0:
             mean = m_array[i-1]
             std = std_array[i-1]
         m_array[i], std_array[i] = mean, std
 
     return m_array, std_array
 
 
-def connectivity_matrix(streamlines, label_volume):
+def connectivity_matrix(streamlines, label_volume, inclusive: bool = True):
     '''
-    Returns the symetric connectivity matrix of the stramlines. Usage of
+    Returns the symetric connectivity matrix of the streamlines. Usage of
     trk.to_vox(), trk.to_corner() beforehand is highly recommended. This
-    fonction is x60 times faster than the implementation in Dipy.
+    fonction is at least x6 times faster than the implementation in Dipy
+    when inclusive is set to True.
 
     Parameters
     ----------
     streamlines : streamline object
         DESCRIPTION.
     label_volume : 3D array of size (x,y,z)
         Array containing the labels as int.
+    inclusive: bool, optional
+        Whether to analyze the entire streamline, as opposed to just the
+        endpoints.
 
     Returns
     -------
     matrix : 2D array
         Connectivity matrix.
 
     '''
 
+    label_volume = label_volume.astype(int)
     matrix = np.zeros((np.max(label_volume)+1, np.max(label_volume)+1))
 
-    for sl in range(len(streamlines)):
+    if not inclusive:
+        streamlines = [sl[0::len(sl)-1] for sl in streamlines]
 
-        x, y, z = np.floor(streamlines[sl].T).astype(int)
+    for sl in streamlines:
 
-        labels = label_volume[x, y, z]
-        crossed_labels = np.unique(labels)
+        x, y, z = np.floor(sl.T).astype(int)
+        crossed_labels = np.unique(label_volume[x, y, z])
 
         for comb in combinations(crossed_labels, 2):
             matrix[comb] += 1
 
     matrix = matrix+matrix.T
 
     return matrix
```

### Comparing `unravel-python-1.4.9/src/unravel/core.py` & `unravel_python-1.5.0/src/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.4.9/src/unravel/example.py` & `unravel_python-1.5.0/src/unravel/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Apr  4 15:52:33 2022
 
 @author: Delinte Nicolas
 
-An example pyhton script using the main methods and outputs of UNRAVEL. A
+An example python script using the main methods and outputs of UNRAVEL. A
 tractogram of the middle anterior section of the corpus callosum is used as
 tractography input.
 
 """
 
 import os
 import numpy as np
```

### Comparing `unravel-python-1.4.9/src/unravel/stream.py` & `unravel_python-1.5.0/src/unravel/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,18 +57,29 @@
     q1, q3 = np.percentile(streams._lengths, [25, 75])
     long_streamlines = streams._lengths > q3
     outlier_streamlines = streams._lengths > q3+1.5*(q3-q1)
     selec_streamlines = long_streamlines*~outlier_streamlines
     m_start = np.mean(start[selec_streamlines], axis=0)
     m_end = np.mean(end[selec_streamlines], axis=0)
 
-    # Re-orders start and end based on main axial direction
-    # !!! does not work on uni-hemisperal left-right tracts
-    main_dir = np.argmax(np.abs(m_start-m_end))
-    if m_start[main_dir] > m_end[main_dir]:
+    # Re-orders start and end based on main axial direction,
+    # first main direction or three-way vote
+    # !!! does not always work
+    diff_abs = np.abs(m_start-m_end)
+    main_dir = np.argmax(diff_abs)
+    small_dir = np.argmin(diff_abs)
+    vote = np.sum(np.where(m_start-m_end > 0, 1, -1))
+    if diff_abs[main_dir] > (np.sum(diff_abs)-diff_abs[main_dir]):
+        if m_start[main_dir] > m_end[main_dir]:
+            m_start, m_end = m_end, m_start
+    elif diff_abs[small_dir] < (np.sum(diff_abs)-diff_abs[small_dir])/4:
+        idx = 1 if small_dir == 0 else 0
+        if m_start[idx] > m_end[idx]:
+            m_start, m_end = m_end, m_start
+    elif vote > 0:
         m_start, m_end = m_end, m_start
 
     # Iterating over specified level ---------------------------------
 
     # point_array = np.vstack((m_start, m_end))
 
     point_array = np.zeros((2**level+1, 3))
@@ -264,15 +275,18 @@
     return dist, median_array
 
 
 def remove_outlier_streamlines(trk_file, point_array, out_file: str = None,
                                outlier_ratio: float = .5,
                                remove_outlier_dir: bool = False,
                                verbose: bool = True, bandwidth: float = 0.2,
-                               neighbors_required: int = 5):
+                               neighbors_required: int = 5,
+                               bandwidth_dir: float = 1,
+                               neighbors_required_dir: int = 10,
+                               keep_ratio: float = 0.5):
     '''
     Removes streamlines that are outliers for more than half (default) of the
     bundle trajectory based on the distance to the mean trajectory. Can also
     remove streamlines if their main direction is an outlier with the
     remove_outlier_dir parameter.
 
     Parameters
@@ -292,38 +306,40 @@
     verbose : bool, optional
         If True, prints number of streamlines removed. The default is False.
     bandwidth : float, optional.
         Bandwidth for the KDE, recommended values : [0.1-5]. The default is 0.2.
     neighbors_required : int, optional
         Approximative number of neighboring points required to not be removed.
         The default is 5.
+    bandwidth_dir : float, optional.
+        Bandwidth for the KDE, recommended values : [0.1-5]. The default is 1.
+    neighbors_required_dir : int, optional
+        Approximative number of neighboring points required to not be removed.
+        The default is 10.
+    keep_ratio : float, optional
+        Maximum percentage of streamlines that can be removed.
+        The default is 0.5.
 
     Returns
     -------
     None.
 
     '''
 
     trk = load_tractogram(trk_file, 'same')
     trk.to_vox()
     trk.to_corner()
 
     streams = trk.streamlines
 
-    bandwidth = 0.2
-    neighbors_required = 5
     bandwidth = bandwidth*neighbors_required
 
     streams_data = trk.streamlines.get_data()
     dens = np.zeros((point_array.shape[0], len(streams._offsets)))
 
-    kde_model_1 = KernelDensity(
-        kernel='gaussian', bandwidth=bandwidth).fit(np.zeros((1, 2)))
-    t = np.exp(kde_model_1.score_samples(np.zeros((1, 2))))
-
     for i, point in enumerate(point_array):
 
         if i == 0:
             continue
         if i == point_array.shape[0]-1:
             break
 
@@ -351,37 +367,44 @@
         y_comp = z_vec - (z_vec@normal)*normal
         y_comp = y_comp/np.linalg.norm(y_comp)
         x_comp = np.cross(y_comp, normal)
 
         proj_mat = -np.vstack([x_comp, y_comp])  # build projection matrix
         points_2D = proj_onto_plane @ proj_mat.T       # apply projection
 
-        # TODO: replace by analytical equation to reduce number of func calls
         kde_model = KernelDensity(
             kernel='gaussian', bandwidth=bandwidth).fit(points_2D)
         kde = np.exp(kde_model.score_samples(points_2D))*len(points_2D)
 
         n = get_streamline_number_from_index(streams, idx)
 
         # Saves densities in decreasing order to keep worse density of
         # streamlines crossing plane multiple times
         kde_decrease_idx = (-kde).argsort()
         dens[i, n[kde_decrease_idx]] = kde[kde_decrease_idx]
 
     # Compute outliers
-    iqr = t*neighbors_required
-    outliers = dens <= np.repeat(iqr[:, np.newaxis], dens.shape[1], axis=1)
+    t = neighbors_required/(2*np.pi*bandwidth**2)
+    m = np.mean(dens, axis=1, where=dens != 0)
+    m = np.repeat(m[..., np.newaxis], dens.shape[1], axis=1)
+    outliers = dens <= t
     outliers[dens == 0] = False
+    outliers[dens > m] = False
     outliers = outliers[1:-1, :]
 
     # Remove if more than outlier_ratio of pathway is outlier
     n_sign = np.sum(outliers, axis=0)
     n_val = np.sum(dens > 0, axis=0)
-    n_sign = np.where(n_sign > n_val*outlier_ratio, 1, 0)
-    n_idx = np.argwhere(n_sign == 1)
+    n_idx = np.argwhere(n_sign > n_val*outlier_ratio)
+
+    if len(n_idx) > keep_ratio*len(n_sign):
+
+        sorted_indexes = np.argsort(-n_sign)
+        keep_num_idx = int(len(n_sign)*keep_ratio)
+        n_idx = sorted_indexes[:keep_num_idx]
 
     if remove_outlier_dir:
 
         streams_data = trk.streamlines.get_data()
 
         # Clustering end nodes based on streamline directions
         end_0 = streams_data[streams._offsets, :]
@@ -408,24 +431,21 @@
         # Send to spherical coordinates in degrees centered on average dir
         r, theta, phi = xyz_to_spherical(end-start)
         r_a, theta_a, phi_a = xyz_to_spherical(average_dir[np.newaxis, ...])
         X = np.stack((theta-theta_a, phi-phi_a), axis=1)
         X = np.where(X < -np.pi, X+2*np.pi, X)
         X = X*180/np.pi
 
-        bw = 1
-        nb = 10
+        bw = bandwidth_dir
+        nb = neighbors_required_dir
         bw = bw*nb
         kde_model = KernelDensity(kernel='gaussian', bandwidth=bw).fit(X)
         dens = np.exp(kde_model.score_samples(X))*len(X)
 
-        # TODO: replace by analytical equation to reduce number of func calls
-        kde_model_1 = KernelDensity(
-            kernel='gaussian', bandwidth=bw).fit(np.zeros((1, 2)))
-        thresh = np.exp(kde_model_1.score_samples(np.zeros((1, 2))))*nb
+        thresh = nb/(2*np.pi*bw**2)
 
         n_idx_gaus = np.argwhere(dens < thresh)
 
         if verbose:
             print(str(n_idx_gaus.shape[0]) +
                   ' streamlines removed based on direction')
         n_idx = np.concatenate((n_idx, n_idx_gaus))
@@ -433,16 +453,15 @@
     streams = remove_streamlines(streams, n_idx)
 
     if out_file is None:
         out_file = trk_file
 
     if verbose:
         print(str(len(n_idx))+' streamlines removed from tract')
-    trk_new = StatefulTractogram(streams, trk, Space.VOX,
-                                 origin=Origin.TRACKVIS)
+    trk_new = trk.from_sft(streams, trk)
     save_tractogram(trk_new, out_file)
 
 
 def get_roi_sections_from_nodes(trk_file: str, point_array,
                                 simplify_shape: bool = True):
     '''
     Create a mask containing the subdivisions of a tract along its mean
@@ -573,10 +592,9 @@
     ends = starts-1
     streams._data[starts] = point[starts]
     streams._data[ends] = point[ends]
 
     if out_file is None:
         out_file = trk_file
 
-    trk_new = StatefulTractogram(streams, trk, Space.VOX,
-                                 origin=Origin.TRACKVIS)
+    trk_new = trk.from_sft(streams, trk)
     save_tractogram(trk_new, out_file)
```

### Comparing `unravel-python-1.4.9/src/unravel/utils.py` & `unravel_python-1.5.0/src/unravel/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Created on Sat Jun  4 22:17:13 2022
 
 @author: DELINTE Nicolas
 """
 
 import numpy as np
-from dipy.io.streamline import load_tractogram
+from dipy.io.streamline import load_tractogram, save_tractogram
 
 
 def tract_to_ROI(trk_file: str):
     '''
     Returns a binary mask of each voxel containing a tractography node.The
     voxels containing streamlines segments but no nodes will not be selected.
 
@@ -70,29 +70,30 @@
 
     peaks = np.nan_to_num(peaks)
     if len(peaks.shape) <= 4:
         peaks = peaks[..., np.newaxis]
 
     K = peaks.shape[-1]
 
-    if frac is None and fvf is None:
-        normalize = True
-
     if frac is None:
         frac = np.ones(peaks.shape[:3]+(K,))/K
+    elif len(frac.shape) <= 3:
+        frac = frac[..., np.newaxis]
     frac = np.stack((frac,)*3, axis=3)
 
     if fvf is None:
         fvf = np.ones(peaks.shape[:3]+(K,))
+    elif len(fvf.shape) <= 3:
+        fvf = fvf[..., np.newaxis]
     fvf = np.stack((fvf,)*3, axis=3)
 
     rgb = np.sum(abs(peaks)*frac*fvf, axis=-1)
 
     # Normalize
-    if normalize:
+    if frac is None and fvf is None:
         rgb = normalize_color(rgb, norm_all_voxels=True)
 
     # Color order
     if order == 'brg':
         rgb = rgb[(slice(None),) * 3 + ([2, 0, 1],)]
     elif order == 'gbr':
         rgb = rgb[(slice(None),) * 3 + ([1, 2, 0],)]
@@ -208,40 +209,14 @@
     MD = MD.real.astype('float64')
 
     np.seterr(divide='warn', invalid='warn')
 
     return FA, AD, RD, MD
 
 
-def xyz_to_spherical(xyz):
-    '''
-    X,y,z coordinates to spherical coordinates.
-
-    Parameters
-    ----------
-    xyz : array of size (n,3)
-        X,y,z coordinates of n points
-
-    Returns
-    -------
-    r : array of size (n)
-        DESCRIPTION.
-    theta : array of size (n)
-        DESCRIPTION.
-    phi : array of size (n)
-        DESCRIPTION.
-
-    '''
-    xy = xyz[:, 0]**2 + xyz[:, 1]**2
-    r = np.sqrt(xy + xyz[:, 2]**2)
-    theta = np.arctan2(np.sqrt(xy), xyz[:, 2])
-    phi = np.arctan2(xyz[:, 1], xyz[:, 0])
-    return r, theta, phi
-
-
 def get_streamline_count(trk) -> int:
     '''
     Returns the number of streamlines in a tractogram.
 
     Parameters
     ----------
     trk : tractogram
@@ -315,29 +290,37 @@
 
     angle[num != 0] /= num[num != 0]
 
     return angle
 
 
 def get_streamline_density(trk, resolution_increase: int = 1,
-                           color: bool = False, subsegment: int = 10):
+                           color: bool = False, subsegment: int = 10,
+                           norm_all_voxels: bool = True):
     '''
     Get the total segment length from a tract specified in trk.
 
     Parameters
     ----------
     trk : tractogram
         Content of a .trk file
     resolution_increase : int, optional
         Factor multiplying the resolution/dimensions of output array. The
         default is 1.
     color : bool, optional
         If True, output a RGB volume with colors corresponding to the
         directions of the streamlines, modulated by streamline density.
         The default is False.
+    subsegment : int, optional
+        Divides the streamline segment into n subsegments. Increases spatial
+        resolution of streamline segments and computation time. The default
+        is 10.
+    norm_all_voxels : bool, optional
+        If True, sets all color voxel with a maximum intensity. Else, the
+        intensity is weighted by the number of fibers. The default is True.
 
     Returns
     -------
     density : 3-D array of shape (x,y,z)
         Array containing the streamline density in each voxel.
     '''
 
@@ -369,15 +352,15 @@
         vs[ends, :] = [0, 0, 0]
         del ends
 
         rgb = np.zeros(tuple(trk._dimensions*resolution_increase)+(3,),
                        dtype=np.float32)
         np.add.at(rgb, (x, y, z), abs(vs))
 
-        return normalize_color(rgb, norm_all_voxels=True)
+        return normalize_color(rgb, norm_all_voxels=norm_all_voxels)
 
     else:
         coef = np.ones(x.shape, dtype=np.float32)
 
         coef[ends] = 0
 
         density = np.zeros(trk._dimensions*resolution_increase,
@@ -404,15 +387,15 @@
         RGB volume.
 
     '''
 
     if norm_all_voxels:
         norm = np.linalg.norm(rgb, axis=3)
         norm = np.stack((norm,)*3, axis=3, dtype=np.float32)
-        norm = np.divide(rgb, norm, dtype=np.float32,
+        norm = np.divide(rgb, norm, dtype=np.float64,
                          where=np.sum(rgb, axis=3, keepdims=True) != 0)
     else:
         norm = (rgb/np.max(rgb)).astype(np.float32)
 
     return norm
 
 
@@ -495,38 +478,74 @@
                    origin='lower', cmap='gray')
         plt.plot(x, y, '.-', c=c)
     plt.title('Streamline trajectory')
 
 
 def xyz_to_spherical(xyz):
     '''
-
+    X,y,z coordinates to spherical coordinates.
 
     Parameters
     ----------
     xyz : array of size (n,3)
-        DESCRIPTION.
+        X,y,z coordinates of n points
 
     Returns
     -------
-    r : TYPE
+    r : array of size (n)
         DESCRIPTION.
-    theta : TYPE
+    theta : array of size (n)
         DESCRIPTION.
-    phi : TYPE
+    phi : array of size (n)
         DESCRIPTION.
 
     '''
     xy = xyz[:, 0]**2 + xyz[:, 1]**2
     r = np.sqrt(xy + xyz[:, 2]**2)
     theta = np.arctan2(np.sqrt(xy), xyz[:, 2])
     phi = np.arctan2(xyz[:, 1], xyz[:, 0])
     return r, theta, phi
 
 
 def spherical_to_xyz(theta, phi):
 
-    x = np.sin(theta)*np.cos(phi)
-    y = np.sin(theta)*np.sin(phi)
-    z = np.cos(theta)
+    x = r*np.sin(theta)*np.cos(phi)
+    y = r*np.sin(theta)*np.sin(phi)
+    z = r*np.cos(theta)
 
     return x, y, z
+
+
+def fuse_trk(trk_file_1: str, trk_file_2: str, output_file: str):
+    '''
+    Creates a new .trk file with all streamlines contained in the two input .trk
+    files. The input files must be in the same space.
+
+    Parameters
+    ----------
+    trk_file_1 : str
+        Filename of first input .trk file.
+    trk_file_2 : str
+        Filename of second input .trk file.
+    output_file : str
+        Filename of output .trk file.
+
+    Returns
+    -------
+    None.
+
+    '''
+
+    trk = load_tractogram(trk_file_1, 'same')
+    trk.to_vox()
+    trk.to_corner()
+    streams_1 = trk.streamlines
+
+    trk = load_tractogram(trk_file_2, 'same')
+    trk.to_vox()
+    trk.to_corner()
+    streams_2 = trk.streamlines
+
+    streams_1.extend(streams_2)
+
+    trk_new = trk.from_sft(streams_1, trk)
+    save_tractogram(trk_new, output_file)
```

### Comparing `unravel-python-1.4.9/src/unravel/viz.py` & `unravel_python-1.5.0/src/unravel/viz.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 """
 
 import numpy as np
 from tqdm import tqdm
 from PIL import Image
 from scipy.ndimage import zoom
 from scipy.interpolate import Akima1DInterpolator
-import pyvista
+import pyvista as pv
 import matplotlib.pyplot as plt
 from matplotlib import cm
+from matplotlib.colors import LinearSegmentedColormap
+from dipy.io.streamline import load_tractogram
 from unravel.core import (angular_weighting,  relative_angular_weighting,
                           closest_fixel_only)
+from unravel.utils import get_streamline_density
 
 
 def grayscale_to_rgb(array):
     '''
     Reapeats a 3D array three times to create a 3D rgb image.
 
     Parameters
@@ -205,17 +208,18 @@
                 ax.plot([-v[0, 0], v[0, 0]], [-v[0, 1], v[0, 1]],
                         zs=[-v[0, 2], v[0, 2]], color='white')
     ax.set_aspect('equal')
 
     plt.show()
 
 
-def plot_alpha_surface_pyvista(vf, method: str = 'raw',
-                               weighting_function=None,
-                               show_v: bool = False):
+def plot_alpha_surface_pyvista(vf, method: str = 'raw', weighting_function=None,
+                               show_v: bool = False, v_color: str = 'white',
+                               mesh_size: int = 200,
+                               background_color: str = 'grey'):
     '''
     Computes and plots the mesh for the alpha coefficient surface based on the
     vectors of vf.
 
     Parameters
     ----------
     vf : list
@@ -228,26 +232,33 @@
             'vol' : relative volume weighting.
         The default is 'raw'.
     weighing_function : function, optional
         Overwrites the weighing function given in method to this method. Used
         for testing. The default is None.
     show_v : bool, optional
         Show vectors. The default is False.
+    v_color : str, optional
+        Vector color. The default is white.
+    mesh_size : int, optional
+        Resolution of the 3D surface. The default is 200.
+    background_color: str, otpional
+        Color of the background in the 3D render. The default is grey.
 
     Returns
     -------
     None.
 
     '''
 
     x, y, z, coef = compute_alpha_surface(vf, method=method,
-                                          weighting_function=weighting_function)
+                                          weighting_function=weighting_function,
+                                          mesh_size=mesh_size)
 
-    pc = pyvista.StructuredGrid(x, y, z)
-    pl = pyvista.Plotter()
+    pc = pv.StructuredGrid(x, y, z)
+    pl = pv.Plotter()
     _ = pl.add_mesh(pc, cmap='plasma', scalars=coef.T.flatten(),
                     smooth_shading=True, show_scalar_bar=False)
     if show_v:
         points = []
         for j in range(vf.shape[2]):
             v = vf[:, :, j]
             v = np.squeeze(v)
@@ -255,22 +266,23 @@
             points.append(v*-1)
             points.append(v)
             if j == 0:
                 _ = pl.add_lines(np.array(points),
                                  label=str(v), color='orange')
             else:
                 _ = pl.add_lines(np.array(points),
-                                 label=str(v), color='white')
+                                 label=str(v), color=v_color)
             points = []
         pl.add_legend()
+    pl.background_color = background_color
     pl.show()
 
 
-def compute_alpha_surface(vf, method: str = 'raw',
-                          weighting_function=None, mesh_size: int = 200):
+def compute_alpha_surface(vf, method: str = 'raw', weighting_function=None,
+                          mesh_size: int = 200):
     '''
     Computes the mesh for the alpha coefficient surface based on the vectors of
     vf.
 
     Parameters
     ----------
     vf : list
@@ -312,15 +324,18 @@
 
     if weighting_function is not None:
         a = weighting_function(vs, vf, nf)[:, 0]
     elif method == 'raw':
         a = relative_angular_weighting(vs, vf, nf)[:, 0]
     elif method == 'cfo':
         a = closest_fixel_only(vs, vf, nf)[:, 0]
+    elif method == 'ang':
+        a = angular_weighting(vs, vf, nf)[:, 0]
     else:
+        print('Warning: method not implemented, angular weighting is used.')
         a = angular_weighting(vs, vf, nf)[:, 0]
 
     x *= (a+1)
     y *= (a+1)
     z *= (a+1)
     coef = a
 
@@ -328,63 +343,75 @@
     y = np.reshape(y, (mesh_size,  mesh_size))
     z = np.reshape(z, (mesh_size,  mesh_size))
     coef = np.reshape(coef, (mesh_size,  mesh_size))
 
     return x, y, z, coef
 
 
-def export_alpha_surface(vList: list, output_path: str, method: str = 'raw',
-                         show_v: bool = True):
+def export_alpha_surface(vf, output_path: str, method: str = 'raw',
+                         show_v: bool = True, v_color: str = 'white',
+                         weighting_function=None, mesh_size: int = 200):
     '''
     Computes and exports the mesh for the alpha coefficient surface based on the
     vectors of vList.
 
     Tutorial to powerpoint: save as .gltf, open with 3D viewer, save as .glb,
     open with 3D builder then repair then save as .3mf
 
-    TODO: update to new architecture
-
     Parameters
     ----------
     vList : list
         List of the k vectors corresponding to each fiber population
     output_path : str
         Output filename.
     method : str, optional
         Method used for the relative contribution, either;
             'ang' : angular weighting
             'raw' : relative angular weighting
             'cfo' : closest-fixel-only
             'vol' : relative volume weighting.
         The default is 'raw'.
+    weighing_function : function, optional
+        Overwrites the weighing function given in method to this method. Used
+        for testing. The default is None.
     show_v : bool, optional
         Show vectors. The default is True.
+    v_color : str, optional
+        Vector color. The default is white.
+    mesh_size : int, optional
+        Resolution of the 3D surface. The default is 200.
 
     Returns
     -------
     None.
 
     '''
 
-    x, y, z, coef = compute_alpha_surface(vList, method=method)
+    x, y, z, coef = compute_alpha_surface(vf, method=method,
+                                          weighting_function=weighting_function,
+                                          mesh_size=mesh_size)
 
-    pc = pyvista.StructuredGrid(x, y, z)
-    pl = pyvista.Plotter()
+    pc = pv.StructuredGrid(x, y, z)
+    pl = pv.Plotter()
     _ = pl.add_mesh(pc, cmap='plasma', scalars=coef.T.flatten(),
                     smooth_shading=True, show_scalar_bar=False)
     if show_v:
         points = []
-        for j, v in enumerate(vList):
+        for j in range(vf.shape[2]):
+            v = vf[:, :, j]
+            v = np.squeeze(v)
             v = v/np.linalg.norm(v)*2.5
-            points.append([i*-1 for i in v])
+            points.append(v*-1)
             points.append(v)
             if j == 0:
-                _ = pl.add_lines(np.array(points), label=str(v), color='orange')
+                _ = pl.add_lines(np.array(points),
+                                 label=str(v), color='orange')
             else:
-                _ = pl.add_lines(np.array(points), label=str(v), color='white')
+                _ = pl.add_lines(np.array(points),
+                                 label=str(v), color=v_color)
             points = []
     pl.export_gltf(output_path)
 
 
 def plot_nodes_and_surfaces(point_array, only_nodes: bool = False):
     '''
     Visualize output of stream.extract_nodes
@@ -446,45 +473,164 @@
             ax.plot_surface(xx, yy, zz, color='grey', alpha=0.5)
     ax.set_xlim(x_lim)
     ax.set_ylim(y_lim)
     ax.set_zlim(z_lim)
     plt.show()
 
 
-def plot_roi_sections(roi, voxel: bool = False, background: str = 'grey'):
+def plot_roi_sections(roi, voxel: bool = False, background: str = 'grey',
+                      color_map: str = 'Set3'):
     '''
 
 
     Parameters
     ----------
     roi : 3D array of shape (x,y,z)
         Labeled volume of n sections of a tract.
     voxel : bool, optional
         If true, plots voxels. I False, plots a smoothed surface.
         The default is False.
     background : str, optional
         Color of the background. The default is 'grey'.
+    color_map : str, optional
+        Color map for the labels. The default is 'Set3'.
 
     Returns
     -------
     None.
 
     '''
 
-    datapv = pyvista.wrap(roi)
+    datapv = pv.wrap(roi)
     datapv.cell_data['labels'] = roi[:-1, :-1, :-1].flatten(order='F')
     vol = datapv.threshold(value=1, scalars='labels')
     mesh = vol.extract_surface()
 
     smooth = mesh.smooth_taubin(n_iter=12)
 
+    # Colormap
+    N = np.max(roi)
+    cmaplist = getattr(plt.cm, color_map).colors
+    cmaplistext = cmaplist*np.ceil(N/len(cmaplist)).astype(int)
+    color_map = LinearSegmentedColormap.from_list(
+        'Custom cmap', cmaplistext[:N], N)
+    color_lim = [1, N+1]
+
     if voxel:
-        vol.plot(cmap='Set3', background=background, scalars='labels')
+        vol.plot(cmap=color_map, clim=color_lim, background=background,
+                 scalars='labels')
+    else:
+        smooth.plot(cmap=color_map, clim=color_lim, background=background,
+                    scalars='labels')
+
+
+def plot_trk(trk_file, scalar=None, opacity: float = 1,
+             show_points: bool = False, color_map=None,
+             resolution_increase: int = 2, background: str = 'black',
+             plotter=None):
+    '''
+    3D render for .trk files.
+
+    Parameters
+    ----------
+    trk_file : str
+        Path to tractography file (.trk)
+    scalar : TYPE, optional
+        DESCRIPTION. The default is None.
+    opacity : float, optional
+        DESCRIPTION. The default is 1.
+    show_points : bool, optional
+        Enable to show points instead of lines. The default is False.
+    color_map : str, optional
+        Color map for the labels The default is None.
+    resolution_increase : int, optional
+        DESCRIPTION. The default is 2.
+    background : str, optional
+        DESCRIPTION. The default is 'black'.
+    plotter : TYPE, optional
+        If not specifed, creates a new figure. The default is None.
+
+    Returns
+    -------
+    None.
+
+    '''
+
+    trk = load_tractogram(trk_file, 'same')
+    trk.to_vox()
+    trk.to_corner()
+    streamlines = trk.streamlines
+
+    coord = np.floor(streamlines._data).astype(int)
+
+    if scalar is None:
+        rgb = get_streamline_density(
+            trk, color=True, resolution_increase=resolution_increase)
+        coord_increase = np.floor(
+            streamlines._data*resolution_increase).astype(int)
+        rgb_points = rgb[coord_increase[:, 0],
+                         coord_increase[:, 1],
+                         coord_increase[:, 2]]
+    else:
+        scalar_points = scalar[coord[:, 0], coord[:, 1], coord[:, 2]]
+
+    l1 = np.ones(len(coord))*2
+    l2 = np.linspace(0, len(coord)-1, len(coord))
+    l3 = np.linspace(1, len(coord), len(coord))
+
+    lines = np.stack((l1, l2, l3), axis=-1).astype(int)
+    lines[streamlines._offsets-1] = 0
+
+    mesh = pv.PolyData(streamlines._data)
+
+    if not show_points:
+        mesh.lines = lines
+        point_size = 0
+        ambient = 0.3
+    else:
+        point_size = 2
+        ambient = 0
+
+    if scalar is None:
+        scalars = rgb_points
+        rgb = True
+    else:
+        scalars = scalar_points
+        rgb = False
+
+    if plotter is None:
+        p = pv.Plotter()
+    else:
+        p = plotter
+    if color_map is not None:
+
+        N = np.max(scalar)
+        cmaplist = getattr(plt.cm, color_map).colors
+        cmaplistext = cmaplist*np.ceil(N/len(cmaplist)).astype(int)
+        color_map = LinearSegmentedColormap.from_list(
+            'Custom cmap', cmaplistext[:N], N)
+
+        color_lim = [1, N+1]
+
+        p.add_mesh(mesh, ambient=ambient, opacity=opacity,
+                   interpolate_before_map=False,
+                   render_lines_as_tubes=True, line_width=2,
+                   point_size=point_size,
+                   cmap=color_map,
+                   clim=color_lim,
+                   scalars=scalars, rgb=rgb)
     else:
-        smooth.plot(cmap='Set3', background=background, scalars='labels')
+        p.add_mesh(mesh, ambient=ambient, opacity=opacity,
+                   render_lines_as_tubes=True, line_width=2,
+                   point_size=point_size,
+                   cmap='plasma',
+                   scalars=scalars, rgb=rgb)
+    p.background_color = background
+    if plotter is None:
+        p.show()
 
 
 def plot_metric_along_trajectory(mean, dev, new_fig: bool = True,
                                  label: str = ''):
     '''
     Plots the output of unravel.analysis.get_metric_along_trajectory.
```

### Comparing `unravel-python-1.4.9/src/unravel_python.egg-info/PKG-INFO` & `unravel_python-1.5.0/src/unravel_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.4.9
+Version: 1.5.0
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```

