# Comparing `tmp/fasttrackpy-0.4.2.tar.gz` & `tmp/fasttrackpy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttrackpy-0.4.2.tar", max compression
+gzip compressed data, was "fasttrackpy-0.4.3.tar", max compression
```

## Comparing `fasttrackpy-0.4.2.tar` & `fasttrackpy-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.2/LICENSE
--rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.2/README.md
--rw-r--r--   0        0        0     1708 2024-04-07 18:52:45.451536 fasttrackpy-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.2/src/fasttrackpy/__init__.py
--rw-r--r--   0        0        0    17445 2024-04-07 18:41:19.124172 fasttrackpy-0.4.2/src/fasttrackpy/cli.py
--rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.2/src/fasttrackpy/patterns/__init__.py
--rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.2/src/fasttrackpy/patterns/audio_textgrid.py
--rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.2/src/fasttrackpy/patterns/corpus.py
--rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.2/src/fasttrackpy/patterns/just_audio.py
--rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.2/src/fasttrackpy/processors/__init__.py
--rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.2/src/fasttrackpy/processors/aggs.py
--rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.2/src/fasttrackpy/processors/losses.py
--rw-r--r--   0        0        0    12670 2024-04-07 18:52:45.451767 fasttrackpy-0.4.2/src/fasttrackpy/processors/outputs.py
--rw-r--r--   0        0        0     3277 2023-11-27 01:47:20.549714 fasttrackpy-0.4.2/src/fasttrackpy/processors/smoothers.py
--rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.2/src/fasttrackpy/resources/config.yml
--rw-r--r--   0        0        0    19345 2024-03-22 21:32:36.644915 fasttrackpy-0.4.2/src/fasttrackpy/tracks.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.2/setup.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.3/LICENSE
+-rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.3/README.md
+-rw-r--r--   0        0        0     1746 2024-04-15 14:22:29.506059 fasttrackpy-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.3/src/fasttrackpy/__init__.py
+-rw-r--r--   0        0        0    17445 2024-04-07 18:41:19.124172 fasttrackpy-0.4.3/src/fasttrackpy/cli.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.3/src/fasttrackpy/patterns/__init__.py
+-rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.3/src/fasttrackpy/patterns/audio_textgrid.py
+-rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.3/src/fasttrackpy/patterns/corpus.py
+-rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.3/src/fasttrackpy/patterns/just_audio.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.3/src/fasttrackpy/processors/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.3/src/fasttrackpy/processors/aggs.py
+-rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.3/src/fasttrackpy/processors/losses.py
+-rw-r--r--   0        0        0    12701 2024-04-15 14:21:09.838269 fasttrackpy-0.4.3/src/fasttrackpy/processors/outputs.py
+-rw-r--r--   0        0        0     3285 2024-04-15 14:21:09.838641 fasttrackpy-0.4.3/src/fasttrackpy/processors/smoothers.py
+-rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.3/src/fasttrackpy/resources/config.yml
+-rw-r--r--   0        0        0    19345 2024-03-22 21:32:36.644915 fasttrackpy-0.4.3/src/fasttrackpy/tracks.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.3/setup.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.3/PKG-INFO
```

### Comparing `fasttrackpy-0.4.2/LICENSE` & `fasttrackpy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/README.md` & `fasttrackpy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/pyproject.toml` & `fasttrackpy-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasttrackpy"
-version = "0.4.2"
+version = "0.4.3"
 description = "A python implementation of FastTrack"
 authors = [
     "JoFrhwld <JoFrhwld@gmail.com>",
     "santiagobarreda <sbarreda@ucdavis.edu>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -46,14 +46,16 @@
 
 
 [tool.poetry.group.docs.dependencies]
 quartodoc = "^0.6.5"
 nbformat = "^5.9.2"
 jupyter = "^1.0.0"
 ipython = "^8.18.0"
+hvplot = "^0.9.2"
+pyarrow = "^15.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/__init__.py` & `fasttrackpy-0.4.3/src/fasttrackpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/cli.py` & `fasttrackpy-0.4.3/src/fasttrackpy/cli.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/patterns/audio_textgrid.py` & `fasttrackpy-0.4.3/src/fasttrackpy/patterns/audio_textgrid.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/patterns/corpus.py` & `fasttrackpy-0.4.3/src/fasttrackpy/patterns/corpus.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/patterns/just_audio.py` & `fasttrackpy-0.4.3/src/fasttrackpy/patterns/just_audio.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/processors/aggs.py` & `fasttrackpy-0.4.3/src/fasttrackpy/processors/aggs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/processors/losses.py` & `fasttrackpy-0.4.3/src/fasttrackpy/processors/losses.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/processors/outputs.py` & `fasttrackpy-0.4.3/src/fasttrackpy/processors/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     ]
     param_df = pl.DataFrame(
         data = self.parameters,schema=schema
     )
 
     param_df = param_df.with_columns(
         error = pl.lit(self.smooth_error)
-    )
+    ).with_row_count(name = "param")
 
     param_df = add_metadata(self, param_df)
 
     return param_df
 
 def get_big_df(self, output):
         all_df = [x.to_df(output = output) for x in self.candidates]
```

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/processors/smoothers.py` & `fasttrackpy-0.4.3/src/fasttrackpy/processors/smoothers.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,18 +96,19 @@
 
     Returns:
         (Smoothed): See `smoothed`
     """
 
     y = np.array (x)
     N = x.size
-    predictors = np.array (
-        [(np.cos(np.pi * (np.arange(N)/N) * k)) 
-         for k in range(order)]
-        )
+    predictors = (scipy.fft.dct(
+        np.eye(N), 
+        orthogonalize=True,
+        norm = "backward"
+    )[:,0:order]).T
 
     nan_entries = np.isnan(y)
     
     y_to_fit = y[~nan_entries]
     predictors_to_use = predictors[:,~nan_entries].T
 
     try:
```

### Comparing `fasttrackpy-0.4.2/src/fasttrackpy/tracks.py` & `fasttrackpy-0.4.3/src/fasttrackpy/tracks.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.2/setup.py` & `fasttrackpy-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fasttrack = fasttrackpy.cli:fasttrack']}
 
 setup_kwargs = {
     'name': 'fasttrackpy',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'A python implementation of FastTrack',
     'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nGoal: A FastTrack python implementation with importable modules\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\n## Usage\n\n```bash\nfasttrack --file audio.wav --output formants.csv\n```\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fasttrackiverse.github.io/fasttrackpy/',
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0', 'pytest>=7.4.3,<8.0.0',
 'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0'] extras_require = \ {':
 python_version >= "3.10" and python_version < "3.12"': ['scipy>=1.11.3,<2.0.0',
 'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"': ['python-
 magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
 bin>=0.4.14,<0.5.0']} entry_points = \ {'console_scripts': ['fasttrack =
 fasttrackpy.cli:fasttrack']} setup_kwargs = { 'name': 'fasttrackpy', 'version':
-'0.4.2', 'description': 'A python implementation of FastTrack',
+'0.4.3', 'description': 'A python implementation of FastTrack',
 'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/
 fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://
 github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)]
 (https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [!
 [codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/
 badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy)
 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][!
```

### Comparing `fasttrackpy-0.4.2/PKG-INFO` & `fasttrackpy-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttrackpy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python implementation of FastTrack
 Home-page: https://fasttrackiverse.github.io/fasttrackpy/
 License: MIT
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.2 Summary: A python
+Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.3 Summary: A python
 implementation of FastTrack Home-page: https://fasttrackiverse.github.io/
 fasttrackpy/ License: MIT Author: JoFrhwld Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: cloup (>=3.0.3,<4.0.0) Requires-Dist: joblib
```

