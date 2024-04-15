# Comparing `tmp/geodynamic-0.0.4.tar.gz` & `tmp/geodynamic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.4.tar", last modified: Sat Apr 13 15:41:43 2024, max compression
+gzip compressed data, was "geodynamic-0.0.5.tar", last modified: Mon Apr 15 15:43:39 2024, max compression
```

## Comparing `geodynamic-0.0.4.tar` & `geodynamic-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.555226 geodynamic-0.0.4/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.4/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-13 15:41:43.555140 geodynamic-0.0.4/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.4/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.549727 geodynamic-0.0.4/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.4/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.552781 geodynamic-0.0.4/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.4/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.4/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    23540 2024-04-13 14:55:14.000000 geodynamic-0.0.4/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.4/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.4/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    29798 2024-04-09 12:54:44.000000 geodynamic-0.0.4/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.554211 geodynamic-0.0.4/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.4/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.4/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     7316 2024-04-13 14:58:22.000000 geodynamic-0.0.4/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.4/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.4/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-13 15:41:43.554827 geodynamic-0.0.4/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-13 15:41:43.000000 geodynamic-0.0.4/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-13 15:41:43.555619 geodynamic-0.0.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-13 15:41:09.000000 geodynamic-0.0.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.168465 geodynamic-0.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.5/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-15 15:43:39.168392 geodynamic-0.0.5/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.5/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.162651 geodynamic-0.0.5/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.5/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.165729 geodynamic-0.0.5/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.5/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.5/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.5/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.5/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.5/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    30062 2024-04-15 14:48:54.000000 geodynamic-0.0.5/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.167544 geodynamic-0.0.5/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.5/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.5/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7314 2024-04-15 15:20:08.000000 geodynamic-0.0.5/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.5/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.5/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-15 15:43:39.168103 geodynamic-0.0.5/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-15 15:43:39.000000 geodynamic-0.0.5/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-15 15:43:39.168777 geodynamic-0.0.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-15 15:42:42.000000 geodynamic-0.0.5/setup.py
```

### Comparing `geodynamic-0.0.4/PKG-INFO` & `geodynamic-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.4/geodynamic/geo/construction.py` & `geodynamic-0.0.5/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.5/geodynamic/geo/lib_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,29 @@
 
 def arc_cpp(circle, p1, p2):
     assert(not np.isclose(circle.c, p1.a).all())
     assert(not np.isclose(circle.c, p2.a).all())
     #print('POINTS-ANGLES: ', [(np.arctan2(p.a[1] - circle.c[1], p.a[0] - circle.c[0])) % (2*np.pi) for p in (p1, p2)])
     return Arc(circle.c, circle.r, [np.arctan2(p.a[1] - circle.c[1], p.a[0] - circle.c[0]) for p in (p1, p2)])
 
+def circumcircle_arc_ppp(p1, p2, p3):
+    assert(not np.isclose(p1.a, p2.a).all())
+    assert(not np.isclose(p1.a, p3.a).all())
+    assert(not np.isclose(p2.a, p3.a).all())
+    circle = circle_ppp(p1, p2, p3)
+    arc = Arc(circle.c, circle.r, [np.arctan2(p.a[1] - circle.c[1], p.a[0] - circle.c[0]) for p in (p1, p3)])
+    return arc if arc.contains(p2.a) else Arc(circle.c, circle.r, [np.arctan2(p.a[1] - circle.c[1], p.a[0] - circle.c[0]) for p in (p3, p1)])
+
+def circle_arc_ppp(p1, p2, p3):
+    assert(not np.isclose(p1.a, p2.a).all())
+    assert(not np.isclose(p1.a, p3.a).all())
+    assert(not np.isclose(p2.a, p3.a).all())
+    circle = circle_pp(p1, p2)
+    return Arc(circle.c, circle.r, [np.arctan2(p.a[1] - circle.c[1], p.a[0] - circle.c[0]) for p in (p2, p3)])
+
 def are_collinear_ppp(p1, p2, p3):
     return Boolean(np.linalg.matrix_rank([p1.a-p2.a, p1.a-p3.a]) <= 1)
 
 def are_concurrent_lll(l1, l2, l3):
     lines = l1,l2,l3
     
     differences = []
```

### Comparing `geodynamic-0.0.4/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.5/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.5/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic/manim_dynamic.py` & `geodynamic-0.0.5/geodynamic/manim_dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,17 @@
 style_pandora['line']['aux'] = 1.5
 
 style_pandora['angle']['line'] = 1
 style_pandora['angle']['r_default'] = 12.5
 style_pandora['angle']['r_shift'] = 1.5
 style_pandora['angle']['r_right'] = 10
 
-style_pandora['strich']['len'] = 0.45
-style_pandora['strich']['shift'] = 0.14
+style_pandora['strich']['width'] = 2
+style_pandora['strich']['len'] = 12
+style_pandora['strich']['shift'] = 4
 
 style_pandora['color']['black'] = '#000000'
 style_pandora['color']['main'] = '#2581b5'
 style_pandora['color']['light'] = '#bef3fc'
 style_pandora['color']['aux'] = '#000000'
 style_pandora['color']['acc'] = '#ef60ab'
 style_pandora['color']['acc_light'] = '#ffd2ee'
@@ -55,14 +56,15 @@
     def __init__(self, scheme = 'book', color = 'blue', theme = 'light', px_size = [1920, 1080]):
         self.dot_size = 0.17   
         self.line_width = 6   
         self.ang_width = 0.75 * self.line_width
         self.strich_rshift = 0.14
         self.ang_rshift = 0.75 * self.strich_rshift
         self.strich_len = 0.45
+        self.strich_width = 6
         self.ang_rdefault = 0.8
         self.ang_right = 0.65
         
         self.background = WHITE
         self.strong = BLACK
 
         if scheme == 'pandora':            
@@ -125,16 +127,17 @@
     def convert_pandora_to_manim(self):
         self.dot_size = 0.02 * style_pandora['dot']['main']
         self.line_width = 2 * style_pandora['line']['main']
         self.ang_width = 2 * style_pandora['angle']['line']
         self.ang_rshift = 2 * style_pandora['angle']['r_shift']
         self.ang_rdefault = 0.02 * style_pandora['angle']['r_default']
         self.ang_right = 0.02 * style_pandora['angle']['r_right']
-        self.strich_len = 2 * style_pandora['strich']['len']
-        self.strich_rshift = 2 * style_pandora['strich']['shift']
+        self.strich_width = 2 * style_pandora['strich']['width']
+        self.strich_len = 0.02 * style_pandora['strich']['len']
+        self.strich_rshift = 0.02 * style_pandora['strich']['shift']
         
         self.background = '#ffffff'
         self.col = style_pandora['color']['main']
         self.col_light = style_pandora['color']['light']
         self.col_accent = style_pandora['color']['acc']
         self.col_accent_light = style_pandora['color']['acc_light']
         self.col_gray = '#eeeeee'
@@ -254,15 +257,17 @@
             style.setViewByGeo(self.geo.style['view'])
         else:
             style.view = self.geo.style['view']
 
         view = style.view
         scale = view['scale']
         for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_rshift', 'strich_len']:
+            print(f'{key} BEFORE: {getattr(style, key)}')
             style.__setattr__(key, getattr(style, key) * 50 / scale)
+            print(f'{key} AFTER: {getattr(style, key)}')
 
         self.camera.frame.set(width = view['width'] / scale)
         dx = self.camera.frame.width / 2 - view['xZero'] / scale
         dy = view['height'] / (2 * scale) - view['yZero'] / scale      
         self.camera.frame.shift(dx * RIGHT + dy * DOWN)
 
         self.setStyle(style)
@@ -652,15 +657,15 @@
                             color = col_s, stroke_opacity = op_s, stroke_width = lw).set_z_index(zz))
 
             if 'lines' in elem.style:
                 num = elem.style['lines']
                 dn = elem.data.n * style.strich_len / 2
                 v = (p2 - p1) / np.linalg.norm(p2 - p1)
                 line = Line([m[0] + dn[0], m[1] + dn[1], 0], [m[0] - dn[0], m[1] - dn[1], 0],
-                            color = col_s, stroke_width = lw, stroke_opacity = op_s).set_z_index(zz)
+                            color = col_s, stroke_width = style.strich_width, stroke_opacity = op_s).set_z_index(zz)
 
                 for i in range(num):
                     d = style.strich_rshift * ((1 - num) * 0.5 + i)
                     arr.append(line.copy().shift([v[0] * d, v[1] * d, 0]))       
 
             if hasParam(elem.style, 'show_label'):
                 label = elem.style['label'] if hasParam(elem.style, 'label') else '$' + elem.name + '$'
```

### Comparing `geodynamic-0.0.4/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.5/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.5/geodynamic/parsers/ggb_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,21 +75,21 @@
                 if elem is not None: 
                     if xelem.attrib['type'] == 'angle':
                         style[name]['r_offset'] = (float(elem.attrib['val']) - 30) / 30
                         
                 elem = xelem.find("objColor")
                 if elem is not None:
                     r, g, b, a = int(elem.attrib['r']), int(elem.attrib['g']), int(elem.attrib['b']), float(elem.attrib['alpha'])
-                    if xelem.attrib['type'] in ['angle', 'polygon', 'arc', 'circle']:
+                    if xelem.attrib['type'] in ['angle', 'polygon', 'arc', 'conic']:
                         style[name]['fill'] = rgb_to_hex(r, g, b)
                         style[name]['fill_opacity'] = a
                     lineStyle = xelem.find("lineStyle")
                     if lineStyle is not None:
                         thick, tt, op = lineStyle.attrib['thickness'], lineStyle.attrib['type'], float(lineStyle.attrib['opacity'])
-                        if xelem.attrib['type'] in ['angle', 'segment', 'arc', 'circle']:
+                        if xelem.attrib['type'] in ['angle', 'segment', 'arc', 'conic']:
                             style[name]['stroke'] = rgb_to_hex(r, g, b)
                             #style[name]['stroke_opacity'] = op / 255
                             #style[name]['stroke_width'] = thick
                             if int(tt) > 0: style[name]['stroke_dash'] = 0.65
                         
         if xelems_left_to_pass:
             xelems_left_to_pass -= 1
```

### Comparing `geodynamic-0.0.4/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.5/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic/parsers/svg_parser.py` & `geodynamic-0.0.5/geodynamic/parsers/svg_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.5/geodynamic.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geodynamic-0.0.4/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.5/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.4/setup.py` & `geodynamic-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.4',
+  version='0.0.5',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

