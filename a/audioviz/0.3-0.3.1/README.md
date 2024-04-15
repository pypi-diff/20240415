# Comparing `tmp/audioviz-0.3.tar.gz` & `tmp/audioviz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.3.tar", last modified: Mon Sep 25 15:01:38 2023, max compression
+gzip compressed data, was "audioviz-0.3.1.tar", last modified: Mon Apr 15 13:53:35 2024, max compression
```

## Comparing `audioviz-0.3.tar` & `audioviz-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-09-25 15:01:38.307237 audioviz-0.3/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1982 2023-09-25 15:01:38.307237 audioviz-0.3/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.3/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-09-25 15:01:38.303237 audioviz-0.3/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8574 2023-05-11 03:27:58.000000 audioviz-0.3/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8706 2023-05-10 10:18:06.000000 audioviz-0.3/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.3/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2445 2023-05-19 03:26:11.000000 audioviz-0.3/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10517 2023-08-05 07:58:03.000000 audioviz-0.3/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.3/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6528 2023-05-14 09:22:21.000000 audioviz-0.3/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.3/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1593 2023-05-11 03:27:06.000000 audioviz-0.3/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.3/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-09-25 15:01:38.307237 audioviz-0.3/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1982 2023-09-25 15:01:38.000000 audioviz-0.3/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-09-25 15:01:38.000000 audioviz-0.3/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-09-25 15:01:38.000000 audioviz-0.3/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.3/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-09-25 15:01:38.000000 audioviz-0.3/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-09-25 15:01:38.000000 audioviz-0.3/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-09-25 15:01:38.307237 audioviz-0.3/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1402 2023-09-25 15:00:51.000000 audioviz-0.3/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2024-04-15 13:53:35.749661 audioviz-0.3.1/
+-rw-r--r--   0 yulanchu  (1009) yulanchu  (1012)     2166 2024-04-15 13:53:35.749661 audioviz-0.3.1/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.3.1/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2024-04-15 13:53:35.745661 audioviz-0.3.1/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8574 2023-05-11 03:27:58.000000 audioviz-0.3.1/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8700 2024-04-15 11:29:29.000000 audioviz-0.3.1/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.3.1/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2445 2023-05-19 03:26:11.000000 audioviz-0.3.1/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10517 2023-08-05 07:58:03.000000 audioviz-0.3.1/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14026 2024-04-15 13:47:52.000000 audioviz-0.3.1/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6528 2023-05-14 09:22:21.000000 audioviz-0.3.1/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.3.1/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1593 2023-05-11 03:27:06.000000 audioviz-0.3.1/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.3.1/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2024-04-15 13:53:35.749661 audioviz-0.3.1/audioviz.egg-info/
+-rw-r--r--   0 yulanchu  (1009) yulanchu  (1012)     2166 2024-04-15 13:53:35.000000 audioviz-0.3.1/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2024-04-15 13:53:35.000000 audioviz-0.3.1/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2024-04-15 13:53:35.000000 audioviz-0.3.1/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.3.1/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2024-04-15 13:53:35.000000 audioviz-0.3.1/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2024-04-15 13:53:35.000000 audioviz-0.3.1/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2024-04-15 13:53:35.749661 audioviz-0.3.1/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1404 2024-04-15 11:29:56.000000 audioviz-0.3.1/setup.py
```

### Comparing `audioviz-0.3/PKG-INFO` & `audioviz-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.3
+Version: 0.3.1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,22 @@
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: librosa
+Requires-Dist: libfmp
+Requires-Dist: plotly
+Requires-Dist: soundfile
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
 * Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
```

### Comparing `audioviz-0.3/README.md` & `audioviz-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/BeatAnalysis.py` & `audioviz-0.3.1/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/ChordAnalysis.py` & `audioviz-0.3.1/audioviz/ChordAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     Returns:
         X (np.ndarray): Chromagram
         Fs_X (scalar): Feature reate of chromagram
         x (np.ndarray): Audio signal
         Fs (scalar): Sampling rate of audio signal
         x_dur (float): Duration (seconds) of audio signal
     """
-    x, Fs = librosa.load(fn_wav, sr=Fs)
+    
+    x = librosa.load(fn_wav)
     x_dur = x.shape[0] / Fs
     if version == 'STFT':
         # Compute chroma features with STFT
         X = librosa.stft(x, n_fft=N, hop_length=H, pad_mode='constant', center=True)
         if gamma is not None:
             X = np.log(1 + gamma * np.abs(X) ** 2)
         else:
```

### Comparing `audioviz-0.3/audioviz/GeneralAnalysis.py` & `audioviz-0.3.1/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/Panel.py` & `audioviz-0.3.1/audioviz/Panel.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/PitchAnalysis.py` & `audioviz-0.3.1/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/StructureAnalysis.py` & `audioviz-0.3.1/audioviz/StructureAnalysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,78 +18,61 @@
 import ipywidgets as widgets
 from IPython.display import display
 import functools
 from google.colab import files
 
 from numpy import typing as npt
 
-@jit(nopython=True)
-def compute_sm_dot(X, Y):
-    """Computes similarty matrix from feature sequences using dot (inner) product
+def my_compute_sm_from_filename(fn_wav, L=21, H=5, L_smooth=16, tempo_rel_set=np.array([1]),
+                             shift_set=np.array([0]), strategy='relative', scale=True, thresh=0.15,
+                             penalty=0.0, binarize=False):
+    """Compute an SSM
 
-    Notebook: C4/C4S2_SSM.ipynb
+    Notebook: C4/C4S2_SSM-Thresholding.ipynb
 
     Args:
-        X (np.ndarray): First sequence
-        Y (np.ndarray): Second Sequence
+        fn_wav (str): Path and filename of wav file
+        L (int): Length of smoothing filter (Default value = 21)
+        H (int): Downsampling factor (Default value = 5)
+        L_smooth (int): Length of filter (Default value = 16)
+        tempo_rel_set (np.ndarray):  Set of relative tempo values (Default value = np.array([1]))
+        shift_set (np.ndarray): Set of shift indices (Default value = np.array([0]))
+        strategy (str): Thresholding strategy (see :func:`libfmp.c4.c4s2_ssm.compute_sm_ti`)
+            (Default value = 'relative')
+        scale (bool): If scale=True, then scaling of positive values to range [0,1] (Default value = True)
+        thresh (float): Treshold (meaning depends on strategy) (Default value = 0.15)
+        penalty (float): Set values below treshold to value specified (Default value = 0.0)
+        binarize (bool): Binarizes final matrix (positive: 1; otherwise: 0) (Default value = False)
 
     Returns:
-        S (float): Dot product
+        x (np.ndarray): Audio signal
+        x_duration (float): Duration of audio signal (seconds)
+        X (np.ndarray): Feature sequence
+        Fs_feature (scalar): Feature rate
+        S_thresh (np.ndarray): SSM
+        I (np.ndarray): Index matrix
     """
-    S = np.dot(np.transpose(X), Y)
-    return S
+    # Waveform
 
-def plot_feature_ssm(X, Fs_X, S, Fs_S, ann, duration, color_ann=None,
-                    title='', label='Time (seconds)', time=True,
-                    figsize=(5, 6), fontsize=10, clim_X=None, clim=None):
-    """Plot SSM along with feature representation and annotations (standard setting is time in seconds)
+    x, Fs = librosa.load(fn_wav)
+    x_duration = x.shape[0] / Fs
 
-    Notebook: C4/C4S2_SSM.ipynb
+    # Chroma Feature Sequence and SSM (10 Hz)
+    C = librosa.feature.chroma_stft(y=x, sr=Fs, tuning=0, norm=2, hop_length=2205, n_fft=4410)
+    Fs_C = Fs / 2205
 
-    Args:
-        X: Feature representation
-        Fs_X: Feature rate of ``X``
-        S: Similarity matrix (SM)
-        Fs_S: Feature rate of ``S``
-        ann: Annotaions
-        duration: Duration
-        color_ann: Color annotations (see :func:`libfmp.b.b_plot.plot_segments`) (Default value = None)
-        title: Figure title (Default value = '')
-        label: Label for time axes (Default value = 'Time (seconds)')
-        time: Display time axis ticks or not (Default value = True)
-        figsize: Figure size (Default value = (5, 6))
-        fontsize: Font size (Default value = 10)
-        clim_X: Color limits for matrix X (Default value = None)
-        clim: Color limits for matrix ``S`` (Default value = None)
+    # Chroma Feature Sequence and SSM
+    X, Fs_feature = libfmp.c3.smooth_downsample_feature_sequence(C, Fs_C, filt_len=L, down_sampling=H)
+    X = libfmp.c3.normalize_feature_sequence(X, norm='2', threshold=0.001)
 
-    Returns:
-        fig: Handle for figure
-        ax: Handle for axes
-    """
-    cmap = libfmp.b.compressed_gray_cmap(alpha=-10)
-    fig, ax = plt.subplots(3, 3, gridspec_kw={'width_ratios': [0.1, 1, 0.05],
-                                              'wspace': 0.2,
-                                              'height_ratios': [0.3, 1, 0.1]},
-                           figsize=figsize)
-    libfmp.b.plot_matrix(X, Fs=Fs_X, ax=[ax[0, 1], ax[0, 2]], clim=clim_X,
-                         xlabel='', ylabel='', title=title)
-    ax[0, 0].axis('off')
-    libfmp.b.plot_matrix(S, Fs=Fs_S, ax=[ax[1, 1], ax[1, 2]], cmap=cmap, clim=clim,
-                         title='', xlabel='', ylabel='', colorbar=True)
-    ax[1, 1].set_xticks([])
-    ax[1, 1].set_yticks([])
-    libfmp.b.plot_segments(ann, ax=ax[2, 1], time_axis=time, fontsize=fontsize,
-                           colors=color_ann,
-                           time_label=label, time_max=duration*Fs_X)
-    ax[2, 2].axis('off')
-    ax[2, 0].axis('off')
-    libfmp.b.plot_segments(ann, ax=ax[1, 0], time_axis=time, fontsize=fontsize,
-                           direction='vertical', colors=color_ann,
-                           time_label=label, time_max=duration*Fs_X)
-    return fig, ax
+    # Compute SSM
+    S, I = libfmp.c4.compute_sm_ti(X, X, L=L_smooth, tempo_rel_set=tempo_rel_set, shift_set=shift_set, direction=2)
+    S_thresh = libfmp.c4.threshold_matrix(S, thresh=thresh, strategy=strategy,
+                                          scale=scale, penalty=penalty, binarize=binarize)
+    return x, x_duration, X, Fs_feature, S_thresh, I
 
 def SSM_chorma(wav_filename:str, anno_csv: str, hop_size: int = 4096, Nfft: int = 1024) -> None :
 
     '''
     To show the self-similarity matrix calculated by chroma
 
     wav_filename: .wav filename
@@ -105,16 +88,16 @@
     X, Fs_X = libfmp.c3.smooth_downsample_feature_sequence(chromagram, fs/hop_size, filt_len=41, down_sampling=10)
 
     # According to the documentation
     ann, color_ann = libfmp.c4.read_structure_annotation(os.path.join(anno_csv), fn_ann_color=anno_csv)
     ann_frames = libfmp.c4.convert_structure_annotation(ann, Fs=Fs_X) 
     
     X = libfmp.c3.normalize_feature_sequence(X, norm='2', threshold=0.001)
-    S = compute_sm_dot(X,X)
-    fig, ax = plot_feature_ssm(X, 1, S, 1, ann_frames, duration*Fs_X, color_ann=color_ann,
+    S = libfmp.c4.compute_sm_dot(X,X)
+    fig, ax = libfmp.c4.plot_feature_ssm(X, 1, S, 1, ann_frames, duration*Fs_X, color_ann=color_ann,
                                clim_X=[0,1], clim=[0,1], label='Time (frames)',
                                title='Chroma feature (Fs=%0.2f)'%Fs_X)
 
 def plot_self_similarity(y: npt.ArrayLike, sr: int, affinity: bool = False, hop_length: int = 1024) -> None:
   '''
   To visualize the similarity matrix of the signal
 
@@ -246,26 +229,29 @@
 
     fn_wav = os.path.join(wav_filename)
     ann, color_ann = libfmp.c4.read_structure_annotation(os.path.join(anno_csv), 
                                                         fn_ann_color=anno_csv)
 
     S_dict = {}
     Fs_dict = {}
-    x, x_duration, X, Fs_X, S, I = libfmp.c4.compute_sm_from_filename(fn_wav, 
+    x, x_duration, X, Fs_X, S, I = my_compute_sm_from_filename(fn_wav, 
                                                     L=11, H=5, L_smooth=1, thresh=1)
+    # Change compute_sm_from_filename to my_compute_sm_from_filename
 
     S_dict[0], Fs_dict[0] = S, Fs_X
     ann_frames = libfmp.c4.convert_structure_annotation(ann, Fs=Fs_X) 
     fig, ax = libfmp.c4.plot_feature_ssm(X, 1, S, 1, ann_frames, x_duration*Fs_X,
                 label='Time (frames)', color_ann=color_ann, clim_X=[0,1], clim=[0,1], 
                 title='Feature rate: %0.0f Hz'%(Fs_X), figsize=(4.5, 5.5))
     float_box.add_fig(fig)
 
-    x, x_duration, X, Fs_X, S, I = libfmp.c4.compute_sm_from_filename(fn_wav, 
+    x, x_duration, X, Fs_X, S, I = my_compute_sm_from_filename(fn_wav, 
                                                     L=41, H=10, L_smooth=1, thresh=1)
+    # Change compute_sm_from_filename to my_compute_sm_from_filename
+
     S_dict[1], Fs_dict[1] = S, Fs_X
     ann_frames = libfmp.c4.convert_structure_annotation(ann, Fs=Fs_X) 
     fig, ax = libfmp.c4.plot_feature_ssm(X, 1, S, 1, ann_frames, x_duration*Fs_X,
                 label='Time (frames)', color_ann=color_ann, clim_X=[0,1], clim=[0,1], 
                 title='Feature rate: %0.0f Hz'%(Fs_X), figsize=(4.5, 5.5))
     float_box.add_fig(fig)
     float_box.show()
@@ -323,16 +309,17 @@
 
     float_box = libfmp.b.FloatingBox()
 
     fn_wav = os.path.join(wav_filename)
     ann, color_ann = libfmp.c4.read_structure_annotation(os.path.join(anno_csv), 
                                                         fn_ann_color=anno_csv)
 
-    x, x_duration, X, Fs_X, S, I = libfmp.c4.compute_sm_from_filename(fn_wav, 
+    x, x_duration, X, Fs_X, S, I = my_compute_sm_from_filename(fn_wav, 
                                                     L=L_filter, H=hopsize, L_smooth=1, thresh=1)
+    # Change compute_sm_from_filename to my_compute_sm_from_filename
 
     ann_frames = libfmp.c4.convert_structure_annotation(ann, Fs=Fs_X) 
     fig, ax = libfmp.c4.plot_feature_ssm(X, 1, S, 1, ann_frames, x_duration*Fs_X,
                 label='Time (frames)', color_ann=color_ann, clim_X=[0,1], clim=[0,1], 
                 title='Feature rate: %0.0f Hz'%(Fs_X), figsize=(4.5, 5.5))
     float_box.add_fig(fig)
     float_box.show()
```

### Comparing `audioviz-0.3/audioviz/TimbreAnalysis.py` & `audioviz-0.3.1/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/colabInterface.py` & `audioviz-0.3.1/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz/utils.py` & `audioviz-0.3.1/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.3/audioviz.egg-info/PKG-INFO` & `audioviz-0.3.1/audioviz.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.3
+Version: 0.3.1
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,22 @@
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: librosa
+Requires-Dist: libfmp
+Requires-Dist: plotly
+Requires-Dist: soundfile
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
 * Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
```

### Comparing `audioviz-0.3/setup.py` & `audioviz-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.3',
+    version='0.3.1',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
```

