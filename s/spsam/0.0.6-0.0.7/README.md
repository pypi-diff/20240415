# Comparing `tmp/spsam-0.0.6.tar.gz` & `tmp/spsam-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spsam-0.0.6.tar", last modified: Sat Mar  2 14:59:43 2024, max compression
+gzip compressed data, was "spsam-0.0.7.tar", last modified: Mon Apr 15 08:19:14 2024, max compression
```

## Comparing `spsam-0.0.6.tar` & `spsam-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.693776 spsam-0.0.6/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 spsam-0.0.6/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 spsam-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      843 2024-03-02 14:59:43.692774 spsam-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      105 2024-02-22 07:07:45.000000 spsam-0.0.6/README.md
--rw-rw-rw-   0        0        0      755 2024-03-02 13:21:33.000000 spsam-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-02 14:59:43.693776 spsam-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.647602 spsam-0.0.6/src/
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 spsam-0.0.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.648600 spsam-0.0.6/src/spsam/
--rw-rw-rw-   0        0        0      328 2024-03-02 13:54:23.000000 spsam-0.0.6/src/spsam/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.671774 spsam-0.0.6/src/spsam/get/
--rw-rw-rw-   0        0        0       30 2024-01-31 07:57:24.000000 spsam-0.0.6/src/spsam/get/__init__.py
--rw-rw-rw-   0        0        0      607 2024-02-02 06:13:06.000000 spsam-0.0.6/src/spsam/get/get.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.676773 spsam-0.0.6/src/spsam/plotting/
--rw-rw-rw-   0        0        0      232 2024-02-07 09:10:14.000000 spsam-0.0.6/src/spsam/plotting/__init__.py
--rw-rw-rw-   0        0        0     7965 2024-03-02 14:51:50.000000 spsam-0.0.6/src/spsam/plotting/_anndata.py
--rw-rw-rw-   0        0        0    54187 2024-02-07 09:10:14.000000 spsam-0.0.6/src/spsam/plotting/_scatterplots.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.677774 spsam-0.0.6/src/spsam/plotting/_tools/
--rw-rw-rw-   0        0        0        0 2024-02-07 08:44:19.000000 spsam-0.0.6/src/spsam/plotting/_tools/__init__.py
--rw-rw-rw-   0        0        0     4615 2023-08-31 09:31:29.000000 spsam-0.0.6/src/spsam/plotting/palettes.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.687774 spsam-0.0.6/src/spsam/preprocessing/
--rw-rw-rw-   0        0        0      229 2024-02-03 12:53:59.000000 spsam-0.0.6/src/spsam/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1631 2024-02-08 07:55:27.000000 spsam-0.0.6/src/spsam/preprocessing/_cycle_spot_count.py
--rw-rw-rw-   0        0        0     6391 2024-02-01 05:21:17.000000 spsam-0.0.6/src/spsam/preprocessing/_find_core_area.py
--rw-rw-rw-   0        0        0      906 2024-02-08 07:55:01.000000 spsam-0.0.6/src/spsam/preprocessing/_get_cell_abundance.py
--rw-rw-rw-   0        0        0     1112 2024-02-03 12:53:59.000000 spsam-0.0.6/src/spsam/preprocessing/_minmaxscaler.py
--rw-rw-rw-   0        0        0     1119 2024-01-31 08:36:04.000000 spsam-0.0.6/src/spsam/preprocessing/_score_lever.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.689777 spsam-0.0.6/src/spsam/tools/
--rw-rw-rw-   0        0        0       39 2024-02-07 08:17:11.000000 spsam-0.0.6/src/spsam/tools/__init__.py
--rw-rw-rw-   0        0        0     6316 2024-02-07 05:27:41.000000 spsam-0.0.6/src/spsam/tools/_score_genes.py
-drwxrwxrwx   0        0        0        0 2024-03-02 14:59:43.691775 spsam-0.0.6/src/spsam.egg-info/
--rw-rw-rw-   0        0        0      843 2024-03-02 14:59:43.000000 spsam-0.0.6/src/spsam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2024-03-02 14:59:43.000000 spsam-0.0.6/src/spsam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 14:59:43.000000 spsam-0.0.6/src/spsam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2024-03-02 14:59:43.000000 spsam-0.0.6/src/spsam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-02 14:59:43.000000 spsam-0.0.6/src/spsam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.106663 spsam-0.0.7/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 spsam-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 spsam-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      843 2024-04-15 08:19:14.105663 spsam-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2024-02-22 07:07:45.000000 spsam-0.0.7/README.md
+-rw-rw-rw-   0        0        0      755 2024-03-08 01:18:43.000000 spsam-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:19:14.106663 spsam-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.948679 spsam-0.0.7/src/
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 spsam-0.0.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.955663 spsam-0.0.7/src/spsam/
+-rw-rw-rw-   0        0        0      328 2024-03-02 13:54:23.000000 spsam-0.0.7/src/spsam/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:13.994752 spsam-0.0.7/src/spsam/get/
+-rw-rw-rw-   0        0        0       30 2024-01-31 07:57:24.000000 spsam-0.0.7/src/spsam/get/__init__.py
+-rw-rw-rw-   0        0        0      607 2024-02-02 06:13:06.000000 spsam-0.0.7/src/spsam/get/get.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.035678 spsam-0.0.7/src/spsam/plotting/
+-rw-rw-rw-   0        0        0      232 2024-02-07 09:10:14.000000 spsam-0.0.7/src/spsam/plotting/__init__.py
+-rw-rw-rw-   0        0        0     7953 2024-04-14 05:56:59.000000 spsam-0.0.7/src/spsam/plotting/_anndata.py
+-rw-rw-rw-   0        0        0    54187 2024-02-07 09:10:14.000000 spsam-0.0.7/src/spsam/plotting/_scatterplots.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.036663 spsam-0.0.7/src/spsam/plotting/_tools/
+-rw-rw-rw-   0        0        0        0 2024-02-07 08:44:19.000000 spsam-0.0.7/src/spsam/plotting/_tools/__init__.py
+-rw-rw-rw-   0        0        0     4615 2023-08-31 09:31:29.000000 spsam-0.0.7/src/spsam/plotting/palettes.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.086665 spsam-0.0.7/src/spsam/preprocessing/
+-rw-rw-rw-   0        0        0      229 2024-02-03 12:53:59.000000 spsam-0.0.7/src/spsam/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1631 2024-02-08 07:55:27.000000 spsam-0.0.7/src/spsam/preprocessing/_cycle_spot_count.py
+-rw-rw-rw-   0        0        0     6391 2024-02-01 05:21:17.000000 spsam-0.0.7/src/spsam/preprocessing/_find_core_area.py
+-rw-rw-rw-   0        0        0      906 2024-02-08 07:55:01.000000 spsam-0.0.7/src/spsam/preprocessing/_get_cell_abundance.py
+-rw-rw-rw-   0        0        0     1112 2024-02-03 12:53:59.000000 spsam-0.0.7/src/spsam/preprocessing/_minmaxscaler.py
+-rw-rw-rw-   0        0        0     1119 2024-01-31 08:36:04.000000 spsam-0.0.7/src/spsam/preprocessing/_score_lever.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.102762 spsam-0.0.7/src/spsam/tools/
+-rw-rw-rw-   0        0        0       39 2024-02-07 08:17:11.000000 spsam-0.0.7/src/spsam/tools/__init__.py
+-rw-rw-rw-   0        0        0     6316 2024-02-07 05:27:41.000000 spsam-0.0.7/src/spsam/tools/_score_genes.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:14.104663 spsam-0.0.7/src/spsam.egg-info/
+-rw-rw-rw-   0        0        0      843 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 08:19:13.000000 spsam-0.0.7/src/spsam.egg-info/top_level.txt
```

### Comparing `spsam-0.0.6/PKG-INFO` & `spsam-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spsam
-Version: 0.0.6
+Version: 0.0.7
 Summary: spSAM: 10X visium spot Split Align Map
 Author-email: renzhg <rzgedu@163.com>
 Project-URL: Homepage, https://github.com/renzhonggan/spsam
 Project-URL: Bug Tracker, https://github.com/renzhonggan/spsam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spsam-0.0.6/pyproject.toml` & `spsam-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spsam"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name = "renzhg", email = "rzgedu@163.com" },
 ]
 dependencies = ['plotly==5.17.0', 'seaborn==0.12.2', 'matplotlib==3.7.2', 'pandas==2.1.0', 'numpy==1.23.4',
     'anndata==0.9.2', 'scikit-learn==1.3.0']
 description = "spSAM: 10X visium spot Split Align Map"
 readme = "README.md"
```

### Comparing `spsam-0.0.6/src/spsam/get/get.py` & `spsam-0.0.7/src/spsam/get/get.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/plotting/_anndata.py` & `spsam-0.0.7/src/spsam/plotting/_anndata.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         title: str = '',
 ):
     if core_type is None:
         pick_type = ['independent', 'adjacent']
     else:
         pick_type = [core_type]
     df = cluster_df[cluster_df['class'].isin(pick_type)]['cycle'].value_counts().reset_index()
-    df = df[df['count'] > 10]  # keep cycle contain at least 10 spots
+    df = df[df['count'] >= 5]  # keep cycle contain at least 5 spots
     x_order = sorted(df['cycle'].tolist())
     fig = px.bar(df, x='cycle', y='count', category_orders={'index': x_order})
     if not title:
         title = f'Spot number in every cycle of {",".join(pick_type)} type，total {len(x_order)} cycles'
     fig.update_layout(title=title,
                       xaxis={'title': xlabel},
                       yaxis={'title': ylabel},
@@ -152,15 +152,15 @@
         height: float = 4,
         xlabel: str = 'cycle',
         ylabel: str = 'cell abundance',
         title: str = 'Cell Abundance In Each Cycle',
 ):
     df = cluster_df[(cluster_df['class'].isin(['independent', 'adjacent'])) & ~(cluster_df['class'] == np.nan)]
     category_counts = cluster_df['cycle'].value_counts()
-    df = df[df['cycle'].isin(category_counts[category_counts >= 10].index)]
+    df = df[df['cycle'].isin(category_counts[category_counts >= 5].index)]
     fig = px.histogram(df, x='cycle', y=cell_type_lt, histfunc='avg')
     fig.update_layout(
         title=title, barmode='group',
         xaxis={'title': xlabel},
         yaxis={'title': ylabel},
         width=width * 100,
         height=height * 100,
@@ -175,26 +175,27 @@
         width: float = 8,
         height: float = 5,
         xlabel: str = 'cycle',
         ylabel: str = 'cell abundance',
         title: str = 'Cell Abundance In Each Cycle',
 ):
     idx_lt = [i for i, j in cluster_scale_df['cycle'].value_counts().items() if
-              j > 10]  # keep cycle contain at least 10 spots
+              j >= 5]  # keep cycle contain at least 10 spots
     plt.figure(figsize=(width, height), dpi=80)
+    df = cluster_scale_df[cluster_scale_df['cycle'].isin(idx_lt)]
     for cell_type in cell_type_lt:
-        sns.lineplot(data=cluster_scale_df[cluster_scale_df['cycle'].isin(idx_lt)], x='cycle', y=cell_type,
+        sns.lineplot(data=df, x='cycle', y=cell_type,
                      label=cell_type, estimator='mean', errorbar=None)
-    sns.lineplot(data=cluster_scale_df[cluster_scale_df['cycle'].isin(idx_lt)], x='cycle', y='mean_abundance',
-                 label='mean_abundance', estimator='mean', errorbar=None, color='black')
+    sns.lineplot(data=df, x=df['cycle'].astype(int),
+                 y='mean_abundance', label='mean_abundance', estimator='mean', errorbar=None, color='black')
     plt.title(title, fontsize=22)
     # 设置 x 轴和 y 轴标题
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
-    plt.legend(loc='center left', bbox_to_anchor=(1, 0.6))
+    plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
     # plt.legend()
     # plt.savefig('my_plot.png')
     plt.show()
 
 
 def plot_cell_abundance(
         cluster_scale_df: DataFrame,
@@ -209,15 +210,15 @@
         ylabel = cell_type
     if not title:
         title = cell_type
     if cell_type not in cluster_scale_df.columns:
         raise KeyError(f'{cell_type} is not in cluster_scale_df')
     plt.figure(figsize=(width, height), dpi=80)
     category_counts = cluster_scale_df['cycle'].value_counts()
-    df = cluster_scale_df[cluster_scale_df['cycle'].isin(category_counts[category_counts >= 10].index)]
-    sns.boxplot(data=df, x='cycle', y=cell_type)
+    df = cluster_scale_df[cluster_scale_df['cycle'].isin(category_counts[category_counts >= 5].index)]
+    sns.boxplot(data=df, x=df['cycle'].astype(int), y=cell_type)
     plt.title(title, fontsize=22)
     # 设置 x 轴和 y 轴标题
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.legend()
     plt.show()
```

### Comparing `spsam-0.0.6/src/spsam/plotting/_scatterplots.py` & `spsam-0.0.7/src/spsam/plotting/_scatterplots.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/plotting/palettes.py` & `spsam-0.0.7/src/spsam/plotting/palettes.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/preprocessing/_cycle_spot_count.py` & `spsam-0.0.7/src/spsam/preprocessing/_cycle_spot_count.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/preprocessing/_find_core_area.py` & `spsam-0.0.7/src/spsam/preprocessing/_find_core_area.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/preprocessing/_get_cell_abundance.py` & `spsam-0.0.7/src/spsam/preprocessing/_get_cell_abundance.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/preprocessing/_minmaxscaler.py` & `spsam-0.0.7/src/spsam/preprocessing/_minmaxscaler.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/preprocessing/_score_lever.py` & `spsam-0.0.7/src/spsam/preprocessing/_score_lever.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam/tools/_score_genes.py` & `spsam-0.0.7/src/spsam/tools/_score_genes.py`

 * *Files identical despite different names*

### Comparing `spsam-0.0.6/src/spsam.egg-info/PKG-INFO` & `spsam-0.0.7/src/spsam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spsam
-Version: 0.0.6
+Version: 0.0.7
 Summary: spSAM: 10X visium spot Split Align Map
 Author-email: renzhg <rzgedu@163.com>
 Project-URL: Homepage, https://github.com/renzhonggan/spsam
 Project-URL: Bug Tracker, https://github.com/renzhonggan/spsam/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spsam-0.0.6/src/spsam.egg-info/SOURCES.txt` & `spsam-0.0.7/src/spsam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

