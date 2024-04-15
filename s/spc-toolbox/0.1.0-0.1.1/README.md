# Comparing `tmp/spc_toolbox-0.1.0.tar.gz` & `tmp/spc_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spc_toolbox-0.1.0.tar", max compression
+gzip compressed data, was "spc_toolbox-0.1.1.tar", max compression
```

## Comparing `spc_toolbox-0.1.0.tar` & `spc_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-04 18:11:46.861269 spc_toolbox-0.1.0/LICENSE
--rw-r--r--   0        0        0     2392 2024-04-04 18:12:45.362203 spc_toolbox-0.1.0/README.md
--rw-r--r--   0        0        0      460 2024-04-04 19:41:38.770523 spc_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14997 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/ControlChart.py
--rw-r--r--   0        0        0     1689 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/IChart.py
--rw-r--r--   0        0        0     1624 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/MRChart.py
--rw-r--r--   0        0        0     1743 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/PChart.py
--rw-r--r--   0        0        0     2440 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/RChart.py
--rw-r--r--   0        0        0     2309 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/SChart.py
--rw-r--r--   0        0        0     1808 2024-04-04 18:12:44.562190 spc_toolbox-0.1.0/spc_toolbox/UChart.py
--rw-r--r--   0        0        0     3384 2024-04-04 18:12:44.582191 spc_toolbox-0.1.0/spc_toolbox/XBarChart.py
--rw-r--r--   0        0        0      258 2024-04-04 18:12:44.582191 spc_toolbox-0.1.0/spc_toolbox/__init__.py
--rw-r--r--   0        0        0     2877 2024-04-04 18:12:44.582191 spc_toolbox-0.1.0/spc_toolbox/utils.py
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 spc_toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 18:11:46.861269 spc_toolbox-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2392 2024-04-04 18:12:45.362203 spc_toolbox-0.1.1/README.md
+-rw-r--r--   0        0        0      460 2024-04-15 19:00:53.023774 spc_toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14913 2024-04-15 19:28:06.702897 spc_toolbox-0.1.1/spc_toolbox/ControlChart.py
+-rw-r--r--   0        0        0     1689 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/IChart.py
+-rw-r--r--   0        0        0     1624 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/MRChart.py
+-rw-r--r--   0        0        0     1822 2024-04-15 18:54:12.966686 spc_toolbox-0.1.1/spc_toolbox/PChart.py
+-rw-r--r--   0        0        0     2440 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/RChart.py
+-rw-r--r--   0        0        0     2309 2024-04-04 18:12:44.562190 spc_toolbox-0.1.1/spc_toolbox/SChart.py
+-rw-r--r--   0        0        0     1820 2024-04-15 18:53:18.006678 spc_toolbox-0.1.1/spc_toolbox/UChart.py
+-rw-r--r--   0        0        0     3384 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/XBarChart.py
+-rw-r--r--   0        0        0      258 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/__init__.py
+-rw-r--r--   0        0        0     2877 2024-04-04 18:12:44.582191 spc_toolbox-0.1.1/spc_toolbox/utils.py
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 spc_toolbox-0.1.1/PKG-INFO
```

### Comparing `spc_toolbox-0.1.0/LICENSE` & `spc_toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/README.md` & `spc_toolbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/ControlChart.py` & `spc_toolbox-0.1.1/spc_toolbox/ControlChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
             rules = self.rules
 
         results = {}
 
         for name, rule in rules.items():
             results[name] = rule(self)
         return results
-        return pd.DataFrame(results)
 
     def fit(self,
             x: pd.Series,
             y: pd.Series,
             lower_control_limit: Union[pd.Series, float],
             center_line: Union[pd.Series, float],
             upper_control_limit: Union[pd.Series, float]
@@ -201,15 +200,14 @@
             raise ValueError("The length of center_line must match the length of x.")
 
         if isinstance(upper_control_limit, pd.Series) and not len(upper_control_limit) == len(x):
             raise ValueError("The length of upper_control_limit must match the length of x.")
 
         self.x = x
         self.y = y
-        self.df = pd.concat([x, y], axis=1)
 
         if isinstance(lower_control_limit, pd.Series):
             self.lower_control_limit = lower_control_limit
         else:
             self.lower_control_limit = pd.Series([lower_control_limit] * len(x), index=x.index)
 
         if isinstance(center_line, pd.Series):
@@ -218,14 +216,19 @@
             self.center_line = pd.Series([center_line] * len(x), index=x.index)
 
         if isinstance(upper_control_limit, pd.Series):
             self.upper_control_limit = upper_control_limit
         else:
             self.upper_control_limit = pd.Series([upper_control_limit] * len(x), index=x.index)
 
+
+        self.center_line.name = "CL"
+        self.upper_control_limit.name = "UCL"
+        self.lower_control_limit.name = "LCL"
+        self.df = pd.concat([self.x, self.y, self.lower_control_limit, self.center_line, self.upper_control_limit], axis=1)
         return self
 
     def plot(self, fig: Optional[plt.Figure] = None, ax: Optional[plt.Axes] = None):
         """
         Plots the ControlChart object.
         
         Parameters:
@@ -260,17 +263,17 @@
         
         if fig is None and ax is None:
             fig, ax = plt.subplots(figsize=(10, 6))
 
         ax.set_title(f"{self.__class__.__name__}")
         ax.set_xlabel(self.x.name)
         ax.set_ylabel(self.y.name)
-        ax.step(self.x, self.upper_control_limit, 'r--', label='UCL')
-        ax.step(self.x, self.center_line, color='green', linestyle='-', label='CL')
-        ax.step(self.x, self.lower_control_limit, 'r--', label='LCL')
+        ax.plot(self.x, self.upper_control_limit, 'r--', label='UCL')
+        ax.plot(self.x, self.center_line, color='green', linestyle='-', label='CL')
+        ax.plot(self.x, self.lower_control_limit, 'r--', label='LCL')
         ax.plot(self.x, self.y, marker='o', linestyle='-')
 
 class CompositeControlChart:
     def __init__(self, charts: List[ControlChart]):
         """
         Initializes a CompositeControlChart object with a list of ControlChart objects.
         
@@ -353,42 +356,34 @@
         
         Parameters:
         - rules (Dict[str, Callable]): A dictionary with rule names as keys and rule functions as values.
         
         Returns:
         - A dictionary with rule names as keys and rule evaluation results as values for each ControlChart object in the list.
         """
-        dfs = []
         results = {}
 
         for chart in self.charts:
             results[chart.__class__.__name__] = chart.evaluate_rules(rules)
         return results
-        for chart in self.charts:
-            df = chart.evaluate_rules(rules)
-            dfs.append(df)
-        
-        df = pd.concat(dfs, axis=1, keys=[chart.__class__.__name__ for chart in self.charts])
-        return df
-        
 
     def fit(self, **kwargs):
         """
         Fits the data for each ControlChart object in the list.
         
         Parameters:
         - kwargs: Keyword arguments to be passed to the fit method of each ControlChart object.
         
         Returns:
         - The CompositeControlChart object with the data fitted for each ControlChart object in the list.
         """
         for chart in self.charts:
             chart.fit(**kwargs)
         return self
-    
+
     def plot(self):
         """
         Plots the CompositeControlChart object.
         """
         fig, axs = plt.subplots(1, len(self.charts), figsize=(len(self.charts) * 10, 6))
         for chart, ax in zip(self.charts, axs):
             chart.plot(fig, ax)
```

### Comparing `spc_toolbox-0.1.0/spc_toolbox/IChart.py` & `spc_toolbox-0.1.1/spc_toolbox/IChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/MRChart.py` & `spc_toolbox-0.1.1/spc_toolbox/MRChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/PChart.py` & `spc_toolbox-0.1.1/spc_toolbox/PChart.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 class PChart(ControlChart):
     def __init__(self, rules: Dict[str, Callable[Concatenate[ControlChart, P], R]] = {}):
         """Initializes a PChart object."""
         super().__init__(rules)
 
     def fit(self,
             index: Union[pd.Series, pd.Index],
-            defective_items: pd.Series, # values: pd.Series
-            total_items: Union[pd.Series, int], # sample_sizes: Union[pd.Series, int]
+            defectives: pd.Series, # defectives: pd.Series
+            sample_sizes: Union[pd.Series, int], # sample_sizes: Union[pd.Series, int]
             z: float = 3.0,
             **kwargs
         ):
         if not isinstance(index, pd.Series) and not isinstance(index, pd.Index):
             raise TypeError("index must be a Series or an Index.")
         if isinstance(index, pd.Index):
             index = pd.Series(index)
-        if not isinstance(defective_items, pd.Series):
-            raise TypeError("defective_items must be a Series.")
-        if not isinstance(total_items, pd.Series) and not isinstance(total_items, int):
-            raise TypeError("total_items must be a Series or an integer.")
+        if not isinstance(defectives, pd.Series):
+            raise TypeError("defectives must be a Series.")
+        if not isinstance(sample_sizes, pd.Series) and not isinstance(sample_sizes, int):
+            raise TypeError("sample_sizes must be a Series or an integer.")
         if type(z) != float:
             raise TypeError("z must be a float.")
 
-        proportions = defective_items / total_items
-        average_proportion = proportions.mean()
+        proportions = defectives / sample_sizes
 
-        std_dev = np.sqrt(proportions * (1 - proportions) / total_items)
+        overall_proportion = defectives.sum() / sample_sizes.sum()
+
+        std_dev = np.sqrt(proportions * (1 - proportions) / sample_sizes)
         self.sigma = std_dev
 
-        center_line = average_proportion
-        upper_control_limit = average_proportion + z * std_dev
-        lower_control_limit = np.maximum(average_proportion - z * std_dev, 0)
+        center_line = overall_proportion
+        # center_line = pd.Series([average_proportion] * len(index))
+        upper_control_limit = overall_proportion + z * std_dev
+        lower_control_limit = np.maximum(overall_proportion - z * std_dev, 0)
 
         super().fit(index, proportions, lower_control_limit, center_line, upper_control_limit)
         return self
```

### Comparing `spc_toolbox-0.1.0/spc_toolbox/RChart.py` & `spc_toolbox-0.1.1/spc_toolbox/RChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/SChart.py` & `spc_toolbox-0.1.1/spc_toolbox/SChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/UChart.py` & `spc_toolbox-0.1.1/spc_toolbox/UChart.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,27 @@
             **kwargs
         ):
         if not isinstance(index, pd.Series) and not isinstance(index, pd.Index):
             raise TypeError("index must be a Series or an Index.")
         if isinstance(index, pd.Index):
             index = pd.Series(index)
         if not isinstance(defects, pd.Series):
-            raise TypeError("defective_items must be a Series.")
+            raise TypeError("defects must be a Series.")
         if not isinstance(sample_sizes, pd.Series) and not isinstance(sample_sizes, int):
             raise TypeError("sample_sizes must be a Series or an integer.")
         if type(z) != float:
             raise TypeError("z must be a float.")
 
-        defects_per_item = defects / sample_sizes
-        defects_per_item.name = "Defects Per Item"
-        average_defects_per_item = defects_per_item.mean()
+        defects_per_unit = defects / sample_sizes
+        defects_per_unit.name = "Defects Per Unit"
 
-        std_dev = np.sqrt(average_defects_per_item / sample_sizes)
+        average_defects_per_unit = defects.sum() / sample_sizes.sum()
+        
+        std_dev = np.sqrt(average_defects_per_unit / sample_sizes)
         self.sigma = std_dev
 
-        center_line = average_defects_per_item
-        upper_control_limit = average_defects_per_item + z * std_dev
-        lower_control_limit = np.maximum(average_defects_per_item - z * std_dev, 0)
+        center_line = average_defects_per_unit
+        upper_control_limit = average_defects_per_unit + z * std_dev
+        lower_control_limit = np.maximum(average_defects_per_unit - z * std_dev, 0)
 
-        super().fit(index, defects_per_item, lower_control_limit, center_line, upper_control_limit)
+        super().fit(index, defects_per_unit, lower_control_limit, center_line, upper_control_limit)
         return self
```

### Comparing `spc_toolbox-0.1.0/spc_toolbox/XBarChart.py` & `spc_toolbox-0.1.1/spc_toolbox/XBarChart.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/spc_toolbox/utils.py` & `spc_toolbox-0.1.1/spc_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `spc_toolbox-0.1.0/PKG-INFO` & `spc_toolbox-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spc-toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolbox for Statistical Process Control
 Author: Philip Solarz
 Author-email: philip.solarz@teliacompany.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

