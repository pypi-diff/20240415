# Comparing `tmp/dansplotcore-6.1.0.tar.gz` & `tmp/dansplotcore-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.1.0.tar", last modified: Tue Apr  2 20:20:49 2024, max compression
+gzip compressed data, was "dansplotcore-6.2.0.tar", last modified: Mon Apr 15 16:07:40 2024, max compression
```

## Comparing `dansplotcore-6.1.0.tar` & `dansplotcore-6.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.1.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.1.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     8546 2024-04-02 20:04:39.000000 dansplotcore-6.1.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.1.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.1.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.1.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.1.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.1.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-02 20:06:28.000000 dansplotcore-6.1.0/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.2.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.2.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9307 2024-04-15 16:00:43.000000 dansplotcore-6.2.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.2.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.2.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.2.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.2.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.2.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-15 16:07:40.000000 dansplotcore-6.2.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-15 16:07:40.328371 dansplotcore-6.2.0/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-15 16:01:06.000000 dansplotcore-6.2.0/setup.py
```

### Comparing `dansplotcore-6.1.0/dansplotcore/media.py` & `dansplotcore-6.2.0/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.1.0/dansplotcore/plot.py` & `dansplotcore-6.2.0/dansplotcore/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -108,35 +108,58 @@
         for i in range(steps):
             x_curr = x[0] + (x[1]-x[0]) * i/(steps-1)
             y_curr = f(x_curr)
             self.primitive(**self.transform(x_curr, y_curr, i, self.series))
         self._plot_common(**kwargs)
 
     def plot_2d(self, array, **kwargs):
-        v_min = math.inf
-        v_max = -math.inf
+        z_min = math.inf
+        z_max = -math.inf
         for row in array:
-            v_min = min(v_min, min(row))
-            v_max = max(v_max, max(row))
-        v_rng = v_max - v_min
-        if v_rng == 0: return
+            z_min = min(z_min, min(row))
+            z_max = max(z_max, max(row))
+        z_rng = z_max - z_min
+        if z_rng == 0: return
         i = 0
         for y, row in enumerate(array):
-            for x, v in enumerate(row):
-                kwargs = {'a': float((v - v_min) / v_rng)}
+            for x, z in enumerate(row):
+                rect = {'a': float((z - z_min) / z_rng)}
                 a = self.transform(x, y, i, self.series)
-                kwargs['xi'] = a['x']
-                kwargs['yi'] = a['y']
-                if 'r' in a: kwargs['r'] = a['r']
-                if 'g' in a: kwargs['g'] = a['g']
-                if 'b' in a: kwargs['b'] = a['b']
+                rect['xi'] = a['x']
+                rect['yi'] = a['y']
+                if 'r' in a: rect['r'] = a['r']
+                if 'g' in a: rect['g'] = a['g']
+                if 'b' in a: rect['b'] = a['b']
                 b = self.transform(x+1, y+1, i, self.series)
-                kwargs['xf'] = b['x']
-                kwargs['yf'] = b['y']
-                self.rect(**kwargs)
+                rect['xf'] = b['x']
+                rect['yf'] = b['y']
+                self.rect(**rect)
+        self._plot_common(**kwargs)
+
+    def plot_heatmap(self, triples, **kwargs):
+        z_min = math.inf
+        z_max = -math.inf
+        zs = [i[2] for i in triples]
+        z_min = min(zs)
+        z_max = max(zs)
+        z_rng = z_max - z_min
+        if z_rng == 0: return
+        i = 0
+        for x, y, z in triples:
+            rect = {'a': float((z - z_min) / z_rng)}
+            a = self.transform(x, y, i, self.series)
+            rect['xi'] = a['x']
+            rect['yi'] = a['y']
+            if 'r' in a: rect['r'] = a['r']
+            if 'g' in a: rect['g'] = a['g']
+            if 'b' in a: rect['b'] = a['b']
+            b = self.transform(x+1, y+1, i, self.series)
+            rect['xf'] = b['x']
+            rect['yf'] = b['y']
+            self.rect(**rect)
         self._plot_common(**kwargs)
 
     def plot_empty(self, *args, **kwargs):
         self._plot_common(**kwargs)
 
     def plot(self, *args, **kwargs):
         plot_func = None
```

### Comparing `dansplotcore-6.1.0/dansplotcore/primitives.py` & `dansplotcore-6.2.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.1.0/dansplotcore/show.py` & `dansplotcore-6.2.0/dansplotcore/show.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.1.0/dansplotcore/transforms.py` & `dansplotcore-6.2.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.1.0/dansplotcore/vector_text.py` & `dansplotcore-6.2.0/dansplotcore/vector_text.py`

 * *Files identical despite different names*

