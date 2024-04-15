# Comparing `tmp/dansplotcore-6.2.0.tar.gz` & `tmp/dansplotcore-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.2.0.tar", last modified: Mon Apr 15 16:07:40 2024, max compression
+gzip compressed data, was "dansplotcore-6.2.1.tar", last modified: Mon Apr 15 18:31:25 2024, max compression
```

## Comparing `dansplotcore-6.2.0.tar` & `dansplotcore-6.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.2.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.2.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9307 2024-04-15 16:00:43.000000 dansplotcore-6.2.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.2.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.2.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.2.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.2.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.2.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-15 16:01:06.000000 dansplotcore-6.2.0/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:31:25.278071 dansplotcore-6.2.1/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 18:31:25.278071 dansplotcore-6.2.1/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:31:25.278071 dansplotcore-6.2.1/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.2.1/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.2.1/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9547 2024-04-15 18:26:47.000000 dansplotcore-6.2.1/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.2.1/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.2.1/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.2.1/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.2.1/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.2.1/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 18:31:25.278071 dansplotcore-6.2.1/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 18:31:25.000000 dansplotcore-6.2.1/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-15 18:31:25.000000 dansplotcore-6.2.1/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-15 18:31:25.000000 dansplotcore-6.2.1/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-15 18:31:25.000000 dansplotcore-6.2.1/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-15 18:31:25.000000 dansplotcore-6.2.1/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-15 18:31:25.278071 dansplotcore-6.2.1/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-15 18:31:19.000000 dansplotcore-6.2.1/setup.py
```

### Comparing `dansplotcore-6.2.0/dansplotcore/media.py` & `dansplotcore-6.2.1/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.0/dansplotcore/plot.py` & `dansplotcore-6.2.1/dansplotcore/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 rect = {'a': float((z - z_min) / z_rng)}
                 a = self.transform(x, y, i, self.series)
                 rect['xi'] = a['x']
                 rect['yi'] = a['y']
                 if 'r' in a: rect['r'] = a['r']
                 if 'g' in a: rect['g'] = a['g']
                 if 'b' in a: rect['b'] = a['b']
-                b = self.transform(x+1, y+1, i, self.series)
+                b = self.transform(self._increment(x), self._increment(y), i, self.series)
                 rect['xf'] = b['x']
                 rect['yf'] = b['y']
                 self.rect(**rect)
         self._plot_common(**kwargs)
 
     def plot_heatmap(self, triples, **kwargs):
         z_min = math.inf
@@ -148,15 +148,15 @@
             rect = {'a': float((z - z_min) / z_rng)}
             a = self.transform(x, y, i, self.series)
             rect['xi'] = a['x']
             rect['yi'] = a['y']
             if 'r' in a: rect['r'] = a['r']
             if 'g' in a: rect['g'] = a['g']
             if 'b' in a: rect['b'] = a['b']
-            b = self.transform(x+1, y+1, i, self.series)
+            b = self.transform(self._increment(x), self._increment(y), i, self.series)
             rect['xf'] = b['x']
             rect['yf'] = b['y']
             self.rect(**rect)
         self._plot_common(**kwargs)
 
     def plot_empty(self, *args, **kwargs):
         self._plot_common(**kwargs)
@@ -223,14 +223,20 @@
                 series = self.series
             kwargs['x'] += self.legend_displacement[0] * series + self.legend_offset[0]
             kwargs['y'] += self.legend_displacement[1] * series + self.legend_offset[1]
             self.text(legend, max_h=abs(self.legend_displacement[1]) or 1, **kwargs)
         if next_series:
             self.next_series()
 
+    def _increment(self, x):
+        if type(x) == datetime.datetime:
+            return x + datetime.timedelta(seconds=self.datetime_unit)
+        else:
+            return x + 1
+
 def plot(
     *args,
     title='plot',
     transform=None,
     hide_axes=False,
     primitive=None,
     **kwargs,
```

### Comparing `dansplotcore-6.2.0/dansplotcore/primitives.py` & `dansplotcore-6.2.1/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.0/dansplotcore/show.py` & `dansplotcore-6.2.1/dansplotcore/show.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.0/dansplotcore/transforms.py` & `dansplotcore-6.2.1/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.2.0/dansplotcore/vector_text.py` & `dansplotcore-6.2.1/dansplotcore/vector_text.py`

 * *Files identical despite different names*

