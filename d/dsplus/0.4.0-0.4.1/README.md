# Comparing `tmp/dsplus-0.4.0.tar.gz` & `tmp/dsplus-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.0.tar", last modified: Wed Apr  3 03:13:31 2024, max compression
+gzip compressed data, was "dsplus-0.4.1.tar", last modified: Mon Apr 15 02:59:38 2024, max compression
```

## Comparing `dsplus-0.4.0.tar` & `dsplus-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:13:31.484335 dsplus-0.4.0/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      690 2024-04-03 03:13:31.481906 dsplus-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 03:13:31.463779 dsplus-0.4.0/dsplus/
--rw-rw-rw-   0        0        0      171 2024-04-03 03:13:10.000000 dsplus-0.4.0/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.4.0/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    41986 2024-03-29 02:59:14.000000 dsplus-0.4.0/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.0/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    44406 2024-03-29 03:03:20.000000 dsplus-0.4.0/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:13:31.476137 dsplus-0.4.0/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-04-03 03:13:31.000000 dsplus-0.4.0/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-03 03:13:31.000000 dsplus-0.4.0/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:13:31.000000 dsplus-0.4.0/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 03:13:31.000000 dsplus-0.4.0/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:13:31.484335 dsplus-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:13:31.477141 dsplus-0.4.0/tests/
--rw-rw-rw-   0        0        0    12143 2024-03-29 17:35:19.000000 dsplus-0.4.0/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.208908 dsplus-0.4.1/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-04-15 02:59:38.205417 dsplus-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.182100 dsplus-0.4.1/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-04-15 02:59:18.000000 dsplus-0.4.1/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24320 2024-04-02 22:58:04.000000 dsplus-0.4.1/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    41884 2024-04-15 02:58:21.000000 dsplus-0.4.1/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.1/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    44406 2024-04-12 03:03:10.000000 dsplus-0.4.1/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.194354 dsplus-0.4.1/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-15 02:59:38.000000 dsplus-0.4.1/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 02:59:37.000000 dsplus-0.4.1/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 02:59:38.208908 dsplus-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:59:38.200574 dsplus-0.4.1/tests/
+-rw-rw-rw-   0        0        0    12143 2024-03-29 17:35:19.000000 dsplus-0.4.1/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.0/LICENSE` & `dsplus-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.0/PKG-INFO` & `dsplus-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.0
+Version: 0.4.1
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.0/dsplus/pb_functions_general.py` & `dsplus-0.4.1/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.0/dsplus/pb_functions_pandas.py` & `dsplus-0.4.1/dsplus/pb_functions_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -789,19 +789,15 @@
     def _style_negative(v, props=''):
         return props if v < 0 else None
     def _highlight_max(s, props=''):
         return np.where(s == np.nanmax(s.values), props, '')
     def _highlight_min(s, props=''):
         return np.where(s == np.nanmin(s.values), props, '')
     v_col_num = df.select_dtypes('number').columns.to_series()
-    df_style = \
-        (df
-            .assign(value2 = lambda _: _['value2'] - 5)
-            .style
-        )
+    df_style = df.style
 
     if precision is not None:
         df_style = df_style.format(precision = 3)
     if negative:
         df_style = df_style.map(_style_negative,
                                 props='color:red;',
                                 subset=v_col_num)
@@ -944,15 +940,15 @@
 
     df.columns = \
     (df
         .columns
         .str.strip()
         .str.lower()
         .str.replace(r'\s|-', '_', regex=True)
-        .str.replace(r'_+', '_', regex=True)        
+        .str.replace(r'_+', '_', regex=True)
         .str.replace(r'\W+', '', regex=True)
         # .str.replace('(', '')
         # .str.replace(')', '')
         # .str.replace('{', '')
         # .str.replace('}', '')
         # .str.replace('[', '')
         # .str.replace(']', '')
```

### Comparing `dsplus-0.4.0/dsplus/pb_functions_plotly.py` & `dsplus-0.4.1/dsplus/pb_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.0/dsplus/pb_functions_spatial.py` & `dsplus-0.4.1/dsplus/pb_functions_spatial.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.0/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.1/dsplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.0
+Version: 0.4.1
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.0/setup.py` & `dsplus-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.0/tests/Test_pandas.py` & `dsplus-0.4.1/tests/Test_pandas.py`

 * *Files identical despite different names*

