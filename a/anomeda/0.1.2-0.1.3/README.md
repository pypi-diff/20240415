# Comparing `tmp/anomeda-0.1.2.tar.gz` & `tmp/anomeda-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomeda-0.1.2.tar", last modified: Tue Apr  2 12:16:29 2024, max compression
+gzip compressed data, was "anomeda-0.1.3.tar", last modified: Sun Apr 14 18:39:32 2024, max compression
```

## Comparing `anomeda-0.1.2.tar` & `anomeda-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.361674 anomeda-0.1.2/
--rw-rw-rw-   0        0        0     1094 2024-02-09 13:38:25.000000 anomeda-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     8784 2024-04-02 12:16:29.355133 anomeda-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8138 2024-04-02 12:14:34.000000 anomeda-0.1.2/README.md
--rw-rw-rw-   0        0        0      722 2024-04-02 12:12:43.000000 anomeda-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 12:16:29.364113 anomeda-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.213108 anomeda-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.270801 anomeda-0.1.2/src/anomeda/
--rw-rw-rw-   0        0        0    24164 2024-03-29 14:25:00.000000 anomeda-0.1.2/src/anomeda/DataFrame.py
--rw-rw-rw-   0        0        0     1455 2024-02-23 10:11:32.000000 anomeda-0.1.2/src/anomeda/__init__.py
--rw-rw-rw-   0        0        0    64895 2024-04-02 12:05:17.000000 anomeda-0.1.2/src/anomeda/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.345378 anomeda-0.1.2/src/anomeda.egg-info/
--rw-rw-rw-   0        0        0     8784 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 12:16:29.000000 anomeda-0.1.2/src/anomeda.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:29.331799 anomeda-0.1.2/tests/
--rw-rw-rw-   0        0        0    13469 2024-04-02 12:04:18.000000 anomeda-0.1.2/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.113075 anomeda-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-12-21 17:57:18.000000 anomeda-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8784 2024-04-14 18:39:32.107657 anomeda-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8138 2024-04-14 15:40:52.000000 anomeda-0.1.3/README.md
+-rw-rw-rw-   0        0        0      722 2024-04-14 18:23:01.000000 anomeda-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 18:39:32.114073 anomeda-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.019031 anomeda-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.041745 anomeda-0.1.3/src/anomeda/
+-rw-rw-rw-   0        0        0    24164 2024-04-14 15:40:38.000000 anomeda-0.1.3/src/anomeda/DataFrame.py
+-rw-rw-rw-   0        0        0     1455 2024-02-23 19:24:49.000000 anomeda-0.1.3/src/anomeda/__init__.py
+-rw-rw-rw-   0        0        0    65024 2024-04-14 18:36:54.000000 anomeda-0.1.3/src/anomeda/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.104452 anomeda-0.1.3/src/anomeda.egg-info/
+-rw-rw-rw-   0        0        0     8784 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-14 18:39:32.000000 anomeda-0.1.3/src/anomeda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.099616 anomeda-0.1.3/tests/
+-rw-rw-rw-   0        0        0    13469 2024-04-14 15:40:52.000000 anomeda-0.1.3/tests/test_main.py
```

### Comparing `anomeda-0.1.2/LICENSE` & `anomeda-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.2/PKG-INFO` & `anomeda-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anomeda-0.1.2/README.md` & `anomeda-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.2/pyproject.toml` & `anomeda-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anomeda"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Anton Saroka", email="anton.soroka.1313@gmail.com" },
 ]
 description = "Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `anomeda-0.1.2/src/anomeda/DataFrame.py` & `anomeda-0.1.3/src/anomeda/DataFrame.py`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.2/src/anomeda/__init__.py` & `anomeda-0.1.3/src/anomeda/__init__.py`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.2/src/anomeda/utils.py` & `anomeda-0.1.3/src/anomeda/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 def extract_trends(
     x : 'numpy.ndarray[int] | pandas.DatetimeIndex', 
     y : 'numpy.ndarray[float]', 
     freq: 'frequency unit for pandas.DatetimeIndex' = None,
     propagation_strategy: '"zeros" | "ffil" | None' = None,
     max_trends : "int | 'auto'"='auto', 
-    min_var_reduction : 'float[0, 1] | None'=0.5, 
+    min_var_reduction : 'float[0, 1] | None' = 0.5, 
     verbose : 'bool'=False
 ):
     """Fit and return automatocally fitted linear trends for given X and Y.
 
     The method can extract more than 1 trend if the metric significantly changed its behavior. 
     The sensibility of the method to identify trend changes are set by parameters "max_trends" and "min_var_reduction".
     
@@ -222,15 +222,15 @@
                                                                       # metric mean over date points is 10.8,
                                                                       # mae for fitting trend over date points is 0.0
                                                                       # sum for all metric values is 21.6
         1: (4, 6, (-0.2999999999999998, 4.6), (2, 3.25, 0.0, 6.5))
     }
     """
     
-    if max_trends == 'auto':
+    if max_trends == 'auto' or max_trends is None:
         if min_var_reduction is None:
             raise ValueError("Either max_trends or min_var_reduction parameters must be set. max_trends='auto' and min_var_reduction=None at the same time is not permitted.")
         max_trends = np.inf
 
     if min_var_reduction is None:
         min_var_reduction = np.inf
 
@@ -922,16 +922,18 @@
                 clusters = existing_clusters.intersection(provided_clusters)
             else:
                 raise ValueError('In case data is pandas.DataFrame returned from anomeda.fit_trends, breakdowns must be either "all", "no" list of measures to iterate or list of specific clusters')
     else:
         raise ValueError('"data" argument must be either anomeda.DataFrame or pandas.DataFrame returned by anomeda.fit_trends()')
 
     if colors is None:
-            replace = len(clusters) >= len(TABLEAU_COLORS)
-            cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
+        replace = len(clusters) >= len(TABLEAU_COLORS)
+        cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
+    else:
+        cluster_c = colors.copy()
     
     for c in clusters:
         
         # reorder features names in accordance to how they sorted in measures names 
         if c not in ['total', 'skipped']:
             try:
                 c = ' and '.join(sorted(c.split(' and '), key=lambda v: measures_names.index(v.split('==')[0].strip().replace('`', ''))))
@@ -950,16 +952,16 @@
         y_trend_cluster = []
 
         for trend in df_tmp.iterrows():
             i, t = trend
             cluster = t['cluster']
             
             if type(t['trend_start_dt']) == int:
-                x = np.arange(t['trend_start_dt'], t['trend_end_dt'])
-                x_axis = x
+                x_axis = np.arange(t['trend_start_dt'], t['trend_end_dt'])
+                x = np.arange(len(x_axis))
             else:
                 x_axis = pd.date_range(start=t['trend_start_dt'], end=t['trend_end_dt'])
                 x = np.arange(len(x_axis))
             
             y_trend = x * t['slope'] + t['intercept']
             
             x_cluster.append(x_axis)
@@ -1120,14 +1122,16 @@
                             str_arr.append('`' + measure_name + '`' + '==' + quote + str(measure_value) + quote)
                         query = ' and '.join(str_arr)
                         clusters.append(query)
 
     if colors is None:
         replace = len(clusters) >= len(TABLEAU_COLORS)
         cluster_c = dict(zip(clusters, np.random.choice(list(TABLEAU_COLORS.keys()), size=len(clusters), replace=replace)))
+    else:
+        cluster_c = colors.copy()
     
     for query in clusters:
         if query == 'total':
             yseries = data_pandas[columns_to_use].groupby(index_name).agg(agg_func)[metric_name]
         else:
             yseries = data_pandas.query(query)[columns_to_use].groupby(index_name).agg(agg_func)[metric_name]
```

### Comparing `anomeda-0.1.2/src/anomeda.egg-info/PKG-INFO` & `anomeda-0.1.3/src/anomeda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anomeda-0.1.2/tests/test_main.py` & `anomeda-0.1.3/tests/test_main.py`

 * *Files identical despite different names*

