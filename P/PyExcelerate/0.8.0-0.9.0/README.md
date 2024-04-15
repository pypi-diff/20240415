# Comparing `tmp/PyExcelerate-0.8.0.tar.gz` & `tmp/PyExcelerate-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyExcelerate-0.8.0.tar", last modified: Sat May  4 16:31:42 2019, max compression
+gzip compressed data, was "dist/PyExcelerate-0.9.0.tar", last modified: Sun Apr  5 03:23:25 2020, max compression
```

## Comparing `PyExcelerate-0.8.0.tar` & `PyExcelerate-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       18 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/requires.txt
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    14278 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/PKG-INFO
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       13 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/top_level.txt
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)        1 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/dependency_links.txt
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1036 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PyExcelerate.egg-info/SOURCES.txt
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     4099 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Style.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      936 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Panes.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    11336 2019-05-04 16:24:58.000000 PyExcelerate-0.8.0/pyexcelerate/Worksheet.py
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/docProps/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      602 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/docProps/core.xml
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1006 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/docProps/app.xml
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1073 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/[Content_Types].xml
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      684 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/workbook.xml
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/_rels/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      564 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/_rels/workbook.xml.rels
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/worksheets/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1368 2019-05-04 16:24:58.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/worksheets/sheet.xml
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      315 2014-12-03 00:08:01.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/styles.empty.xml
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1641 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/xl/styles.xml
-drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/pyexcelerate/templates/_rels/
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      592 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/pyexcelerate/templates/_rels/.rels
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     9142 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Range.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1654 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Fill.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3375 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Alignment.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3508 2019-05-04 16:24:58.000000 PyExcelerate-0.8.0/pyexcelerate/Workbook.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3394 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Writer.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1241 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Format.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       22 2019-05-04 16:28:39.000000 PyExcelerate-0.8.0/pyexcelerate/version.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1864 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Border.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3172 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Borders.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     2755 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/DataTypes.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1278 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Utility.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      247 2017-11-15 19:27:48.000000 PyExcelerate-0.8.0/pyexcelerate/__init__.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3445 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Font.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      692 2018-06-05 21:50:16.000000 PyExcelerate-0.8.0/pyexcelerate/Color.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    14278 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/PKG-INFO
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3030 2019-05-04 16:28:39.000000 PyExcelerate-0.8.0/CHANGELOG.md
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    10374 2017-11-15 19:55:58.000000 PyExcelerate-0.8.0/README.rst
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       91 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/.coveragerc
--rwxrwxr-x   0 kzhang    (1000) kzhang    (1000)     1115 2019-05-04 16:28:39.000000 PyExcelerate-0.8.0/setup.py
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      116 2014-05-20 15:07:34.000000 PyExcelerate-0.8.0/MANIFEST.in
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     9814 2017-11-15 19:55:58.000000 PyExcelerate-0.8.0/README.md
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       18 2015-04-07 20:51:51.000000 PyExcelerate-0.8.0/requirements.txt
--rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       38 2019-05-04 16:31:42.000000 PyExcelerate-0.8.0/setup.cfg
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       18 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/requires.txt
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    14278 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/PKG-INFO
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       13 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/top_level.txt
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)        1 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1036 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PyExcelerate.egg-info/SOURCES.txt
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     4082 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Style.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      924 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Panes.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    12858 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Worksheet.py
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/docProps/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      602 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/docProps/core.xml
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1006 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/docProps/app.xml
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1073 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/[Content_Types].xml
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      684 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/workbook.xml
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/_rels/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      564 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/_rels/workbook.xml.rels
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/worksheets/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1368 2019-05-04 16:24:58.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/worksheets/sheet.xml
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      315 2014-12-03 00:08:01.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/styles.empty.xml
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1641 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/xl/styles.xml
+drwxrwxr-x   0 kzhang    (1000) kzhang    (1000)        0 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/pyexcelerate/templates/_rels/
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      592 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/pyexcelerate/templates/_rels/.rels
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     9255 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Range.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1588 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Fill.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3522 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Alignment.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3460 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Workbook.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3380 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Writer.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1134 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Format.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       22 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/version.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1876 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Border.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3291 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Borders.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     2903 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/DataTypes.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     1296 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Utility.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      246 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/__init__.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3516 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Font.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      753 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/pyexcelerate/Color.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    14278 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/PKG-INFO
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     3173 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)    10374 2017-11-15 19:55:58.000000 PyExcelerate-0.9.0/README.rst
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       91 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/.coveragerc
+-rwxrwxr-x   0 kzhang    (1000) kzhang    (1000)     1268 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/setup.py
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)      116 2014-05-20 15:07:34.000000 PyExcelerate-0.9.0/MANIFEST.in
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)     9814 2017-11-15 19:55:58.000000 PyExcelerate-0.9.0/README.md
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       17 2020-04-05 03:22:25.000000 PyExcelerate-0.9.0/requirements.txt
+-rw-rw-r--   0 kzhang    (1000) kzhang    (1000)       38 2020-04-05 03:23:25.000000 PyExcelerate-0.9.0/setup.cfg
```

### Comparing `PyExcelerate-0.8.0/PyExcelerate.egg-info/PKG-INFO` & `PyExcelerate-0.9.0/PyExcelerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyExcelerate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Accelerated Excel XLSX Writing Library for Python 2/3
 Home-page: https://github.com/kz26/PyExcelerate
 Author: Kevin Wang, Kevin Zhang
 Author-email: kevin+pyexcelerate@kevinzhang.me
 Maintainer: Kevin Zhang
 Maintainer-email: kevin+pyexcelerate@kevinzhang.me
 License: UNKNOWN
@@ -396,13 +396,13 @@
         .. |coverage-status| image:: https://coveralls.io/repos/kz26/PyExcelerate/badge.png
            :target: https://coveralls.io/r/kz26/PyExcelerate
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `PyExcelerate-0.8.0/PyExcelerate.egg-info/SOURCES.txt` & `PyExcelerate-0.9.0/PyExcelerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Style.py` & `PyExcelerate-0.9.0/pyexcelerate/Style.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 from . import Font, Fill, Format, Alignment, Borders
 from . import Utility
 import six
 
 
 class Style(object):
-    __slots__ = ('_font', '_fill', '_format', '_alignment', '_borders',
-                 '_size', 'id')
+    __slots__ = ("_font", "_fill", "_format", "_alignment", "_borders", "_size", "id")
 
-    def __init__(self,
-                 font=None,
-                 fill=None,
-                 format=None,
-                 alignment=None,
-                 borders=None,
-                 size=None):
+    def __init__(
+        self, font=None, fill=None, format=None, alignment=None, borders=None, size=None
+    ):
         self._font = font
         self._fill = fill
         self._format = format
         self._alignment = alignment
         self._borders = borders
         self._size = size
 
     @property
     def size(self):
         return self._size
 
     @property
     def is_default(self):
-        return not (self._font or self._fill or self._format or self._alignment
-                    or self._borders or self._size is not None)
+        return not (
+            self._font
+            or self._fill
+            or self._format
+            or self._alignment
+            or self._borders
+            or self._size is not None
+        )
 
     @property
     def borders(self):
-        return Utility.lazy_get(self, '_borders', Borders.Borders())
+        return Utility.lazy_get(self, "_borders", Borders.Borders())
 
     @borders.setter
     def borders(self, value):
-        Utility.lazy_set(self, '_borders', None, value)
+        Utility.lazy_set(self, "_borders", None, value)
 
     @property
     def alignment(self):
-        return Utility.lazy_get(self, '_alignment', Alignment.Alignment())
+        return Utility.lazy_get(self, "_alignment", Alignment.Alignment())
 
     @alignment.setter
     def alignment(self, value):
-        Utility.lazy_set(self, '_alignment', None, value)
+        Utility.lazy_set(self, "_alignment", None, value)
 
     @property
     def format(self):
         # don't use default because default should be const
-        return Utility.lazy_get(self, '_format', Format.Format())
+        return Utility.lazy_get(self, "_format", Format.Format())
 
     @format.setter
     def format(self, value):
-        Utility.lazy_set(self, '_format', None, value)
+        Utility.lazy_set(self, "_format", None, value)
 
     @property
     def font(self):
-        return Utility.lazy_get(self, '_font', Font.Font())
+        return Utility.lazy_get(self, "_font", Font.Font())
 
     @font.setter
     def font(self, value):
-        Utility.lazy_set(self, '_font', None, value)
+        Utility.lazy_set(self, "_font", None, value)
 
     @property
     def fill(self):
-        return Utility.lazy_get(self, '_fill', Fill.Fill())
+        return Utility.lazy_get(self, "_fill", Fill.Fill())
 
     @fill.setter
     def fill(self, value):
-        Utility.lazy_set(self, '_fill', None, value)
+        Utility.lazy_set(self, "_fill", None, value)
 
     def get_xml_string(self):
         # Precondition: Workbook._align_styles has been run.
         # Be careful when using this function as id's may be inaccurate if precondition not met.
         tag = []
         if not self._format is None:
-            tag.append("numFmtId=\"%d\"" % self._format.id)
+            tag.append('numFmtId="%d"' % self._format.id)
         if not self._font is None:
-            tag.append("applyFont=\"1\" fontId=\"%d\"" % (self._font.id))
+            tag.append('applyFont="1" fontId="%d"' % (self._font.id))
         if not self._fill is None:
-            tag.append("applyFill=\"1\" fillId=\"%d\"" % (self._fill.id + 1))
+            tag.append('applyFill="1" fillId="%d"' % (self._fill.id + 1))
         if not self._borders is None:
-            tag.append("applyBorder=\"1\" borderId=\"%d\"" %
-                       (self._borders.id))
+            tag.append('applyBorder="1" borderId="%d"' % (self._borders.id))
         if self._alignment is None:
-            return "<xf xfId=\"0\" %s/>" % (" ".join(tag))
+            return '<xf xfId="0" %s/>' % (" ".join(tag))
         else:
-            return "<xf xfId=\"0\"  %s applyAlignment=\"1\">%s</xf>" % (
-                " ".join(tag), self._alignment.get_xml_string())
+            return '<xf xfId="0"  %s applyAlignment="1">%s</xf>' % (
+                " ".join(tag),
+                self._alignment.get_xml_string(),
+            )
 
     def __hash__(self):
         return hash((self._font, self._fill, self._format, self._alignment))
 
     def __eq__(self, other):
         if other is None:
             return self.is_default
@@ -104,25 +106,30 @@
     def __and__(self, other):
         return self._binary_operation(other, Utility.nonboolean_and)
 
     def __xor__(self, other):
         return self._binary_operation(other, Utility.nonboolean_xor)
 
     def _binary_operation(self, other, operation):
-        return Style( \
-         font=operation(self.font, other.font), \
-         fill=operation(self.fill, other.fill), \
-         format=operation(self.format, other.format), \
-         alignment=operation(self.alignment, other.alignment), \
-         borders=operation(self.borders, other.borders) \
+        return Style(
+            font=operation(self.font, other.font),
+            fill=operation(self.fill, other.fill),
+            format=operation(self.format, other.format),
+            alignment=operation(self.alignment, other.alignment),
+            borders=operation(self.borders, other.borders),
         )
 
     def _to_tuple(self):
-        return (self._font, self._fill, self._format, self._alignment,
-                self._borders, self._size)
+        return (
+            self._font,
+            self._fill,
+            self._format,
+            self._alignment,
+            self._borders,
+            self._size,
+        )
 
     def __str__(self):
-        return "%s %s %s %s" % (self.font, self.fill, self.format,
-                                self.alignment)
+        return "%s %s %s %s" % (self.font, self.fill, self.format, self.alignment)
 
     def __repr__(self):
         return "<%s>" % self.__str__()
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Panes.py` & `PyExcelerate-0.9.0/pyexcelerate/Panes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import Range
 from .Utility import to_unicode
 
 
 class Panes(object):
-    __slots__ = ('x', 'y', 'freeze')
+    __slots__ = ("x", "y", "freeze")
 
     def __init__(self, x=None, y=None, freeze=True):
         self.x = x or 0
         self.y = y or 0
         self.freeze = freeze
 
     def __bool__(self):
@@ -17,18 +17,17 @@
         return self.__bool__()
 
     def __eq__(self, other):
         return self.x == other.x and self.y == other.y and self.freeze == other.freeze
 
     def get_xml(self):
         attrs = {
-            'topLeftCell':
-            Range.Range.coordinate_to_string((self.y + 1, self.x + 1))
+            "topLeftCell": Range.Range.coordinate_to_string((self.y + 1, self.x + 1))
         }
         if self.freeze:
-            attrs['state'] = 'frozen'
+            attrs["state"] = "frozen"
         if self.x:
-            attrs['xSplit'] = self.x
+            attrs["xSplit"] = self.x
         if self.y:
-            attrs['ySplit'] = self.y
+            attrs["ySplit"] = self.y
         attr_str = " ".join('%s="%s"' % item for item in sorted(attrs.items()))
         return to_unicode("<pane %s/>" % attr_str)
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Worksheet.py` & `PyExcelerate-0.9.0/pyexcelerate/Worksheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,83 @@
-from . import Panes
-from . import Range
-from . import Style
-from . import Format
-from .DataTypes import DataTypes
-from .Utility import to_unicode
+# -*- coding: utf-8 -*-
+
 import collections
 import itertools
-import six
 import math
+import re
+import sys
 from datetime import datetime
 from xml.sax.saxutils import escape
 
+import six
+
+from . import Format, Panes, Range, Style
+from .DataTypes import DataTypes
+from .Utility import to_unicode
+
+# From https://stackoverflow.com/a/22273639/86433
+_illegal_unichrs = [
+    (0x00, 0x08),
+    (0x0B, 0x0C),
+    (0x0E, 0x1F),
+    (0x7F, 0x84),
+    (0x86, 0x9F),
+    (0xFDD0, 0xFDDF),
+    (0xFFFE, 0xFFFF),
+]
+if sys.maxunicode >= 0x10000:  # not narrow build
+    _illegal_unichrs.extend(
+        [
+            (0x1FFFE, 0x1FFFF),
+            (0x2FFFE, 0x2FFFF),
+            (0x3FFFE, 0x3FFFF),
+            (0x4FFFE, 0x4FFFF),
+            (0x5FFFE, 0x5FFFF),
+            (0x6FFFE, 0x6FFFF),
+            (0x7FFFE, 0x7FFFF),
+            (0x8FFFE, 0x8FFFF),
+            (0x9FFFE, 0x9FFFF),
+            (0xAFFFE, 0xAFFFF),
+            (0xBFFFE, 0xBFFFF),
+            (0xCFFFE, 0xCFFFF),
+            (0xDFFFE, 0xDFFFF),
+            (0xEFFFE, 0xEFFFF),
+            (0xFFFFE, 0xFFFFF),
+            (0x10FFFE, 0x10FFFF),
+        ]
+    )
+_illegal_ranges = [
+    "%s-%s" % (six.unichr(low), six.unichr(high)) for (low, high) in _illegal_unichrs
+]
+_illegal_xml_chars_RE = re.compile(u"[%s]" % u"".join(_illegal_ranges))
+
 
 class Worksheet(object):
-    __slots__ = ('_columns', '_name', '_dense_cells', '_sparse_cells',
-                 '_styles', '_row_styles', '_col_styles', '_parent', '_merges',
-                 '_attributes', '_panes', '_show_grid_lines', 'auto_filter')
+    __slots__ = (
+        "_columns",
+        "_name",
+        "_dense_cells",
+        "_sparse_cells",
+        "_styles",
+        "_row_styles",
+        "_col_styles",
+        "_parent",
+        "_merges",
+        "_attributes",
+        "_panes",
+        "_show_grid_lines",
+        "auto_filter",
+    )
 
     def __init__(self, name, workbook, data=None, force_name=False):
         self._columns = 0  # cache this for speed
         if len(name) > 31 and not force_name:
             # http://stackoverflow.com/questions/3681868/is-there-a-limit-on-an-excel-worksheets-name-length
             raise Exception(
-                'Excel does not permit worksheet names longer than 31 characters. Set force_name=True to disable this restriction.'
+                "Excel does not permit worksheet names longer than 31 characters. Set force_name=True to disable this restriction."
             )
         self._name = name
         self._dense_cells = [[]]
         self._sparse_cells = collections.defaultdict(dict)
         self._styles = collections.defaultdict(dict)
         self._row_styles = {}
         self._col_styles = {}
@@ -48,23 +99,23 @@
                     for y, cell in enumerate(row, 1):
                         self._sparse_cells[x][y] = cell
                         self._columns = max(self._columns, y)
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             if key.step is not None and key.step > 1:
-                raise Exception(
-                    "PyExcelerate doesn't support slicing with steps")
+                raise Exception("PyExcelerate doesn't support slicing with steps")
             else:
-                return Range.Range((key.start or 1, 1),
-                                   (key.stop or float('inf'), float('inf')),
-                                   self)
+                return Range.Range(
+                    (key.start or 1, 1), (key.stop or float("inf"), float("inf")), self
+                )
         else:
-            return Range.Range((key, 1), (key, float('inf')),
-                               self)  # return a row range
+            return Range.Range(
+                (key, 1), (key, float("inf")), self
+            )  # return a row range
 
     @property
     def panes(self):
         return self._panes
 
     @panes.setter
     def panes(self, panes):
@@ -84,16 +135,16 @@
     def merges(self):
         return self._merges
 
     @property
     def num_rows(self):
         return max(
             len(self._dense_cells) - 1,
-            max(six.iterkeys(self._sparse_cells))
-            if len(self._sparse_cells) > 0 else 0)
+            max(six.iterkeys(self._sparse_cells)) if len(self._sparse_cells) > 0 else 0,
+        )
 
     @property
     def num_columns(self):
         return self._columns
 
     @property
     def show_grid_lines(self):
@@ -121,15 +172,15 @@
         if x < len(self._dense_cells) and y < len(self._dense_cells[x]):
             return self._dense_cells[x][y]
         # Fallback to sparse cells
         return self._sparse_cells[x].get(y)
 
     def set_cell_value(self, x, y, value):
         if DataTypes.get_type(value) == DataTypes.DATE:
-            self.get_cell_style(x, y).format = Format.Format('yyyy-mm-dd')
+            self.get_cell_style(x, y).format = Format.Format("yyyy-mm-dd")
         if x < len(self._dense_cells) and y < len(self._dense_cells[x]):
             self._dense_cells[x][y] = value
         else:
             self._sparse_cells[x][y] = value
         self._columns = max(self._columns, y)
 
     def get_cell_style(self, x, y):
@@ -137,15 +188,15 @@
             self.set_cell_style(x, y, Style.Style())
         return self._styles[x][y]
 
     def set_cell_style(self, x, y, value):
         self._styles[x][y] = value
         self._parent.add_style(value)
         if self.get_cell_value(x, y) is None:
-            self.set_cell_value(x, y, '')
+            self.set_cell_value(x, y, "")
 
     def get_row_style(self, row):
         if row not in self._row_styles:
             self.set_row_style(row, Style.Style())
         return self._row_styles[row]
 
     def set_row_style(self, row, value):
@@ -182,107 +233,132 @@
         if type == DataTypes.NUMBER:
             if math.isnan(cell):
                 z = '" t="e"><v>#NUM!</v></c>'
             elif math.isinf(cell):
                 z = '" t="e"><v>#DIV/0!</v></c>'
             else:
                 z = '"><v>%.15g</v></c>' % (cell)
-        elif type == DataTypes.INLINE_STRING:
-            z = '" t="inlineStr"><is><t>%s</t></is></c>' % escape(
-                to_unicode(cell))
+        elif type == DataTypes.INLINE_STRING or type == DataTypes.ERROR:
+            # Also serialize errors to string, we'll try our best...
+            z = '" t="inlineStr"><is><t xml:space="preserve">%s</t></is></c>' % escape(
+                _illegal_xml_chars_RE.sub(u"\uFFFD", to_unicode(cell if isinstance(cell, six.string_types) else str(cell)))
+            )
         elif type == DataTypes.DATE:
             z = '"><v>%s</v></c>' % (DataTypes.to_excel_date(cell))
         elif type == DataTypes.FORMULA:
-            z = '"><f>%s</f></c>' % (cell[1:]) # Remove equals sign.
+            z = '"><f>%s</f></c>' % (cell[1:])  # Remove equals sign.
         elif type == DataTypes.BOOLEAN:
             z = '" t="b"><v>%d</v></c>' % (cell)
 
-        if style and hasattr(style, 'id'):
-            return "<c r=\"%s\" s=\"%d%s" % (Range.Range.coordinate_to_string(
-                (x, y)), style.id, z)
+        if style and hasattr(style, "id"):
+            return '<c r="%s" s="%d%s' % (
+                Range.Range.coordinate_to_string((x, y)),
+                style.id,
+                z,
+            )
         else:
-            return "<c r=\"%s%s" % (Range.Range.coordinate_to_string((x, y)),
-                                    z)
+            return '<c r="%s%s' % (Range.Range.coordinate_to_string((x, y)), z)
 
     def get_col_xml_string(self, col):
         if col not in self._col_styles or self._col_styles[col].is_default:
-          return "<col min=\"%d\" max=\"%d\">" % (col, col)
+            return '<col min="%d" max="%d">' % (col, col)
         style = self._col_styles[col]
         if style.size == -1:
-          size = 0
-          
-          def get_size(v):
-            if isinstance(v, six.string_types):
-                v = to_unicode(v)
-            else:
-                v = six.text_type(v)
-            return (len(v) * 7 + 5) / 7
-            
-          for row in self._dense_cells[1:]:
-            if col < len(row):
-              size = max(get_size(row[col]), size)
-          for row in six.itervalues(self._sparse_cells):
-            if col in row:
-              size = max(get_size(row[col]), size)
+            size = 0
+
+            def get_size(v):
+                if isinstance(v, six.string_types):
+                    v = to_unicode(v)
+                else:
+                    v = six.text_type(v)
+                return (len(v) * 7 + 5) / 7
+
+            for row in self._dense_cells[1:]:
+                if col < len(row):
+                    size = max(get_size(row[col]), size)
+            for row in six.itervalues(self._sparse_cells):
+                if col in row:
+                    size = max(get_size(row[col]), size)
         elif DataTypes.get_type(style.size) == DataTypes.NUMBER:
-          size = style.size
+            size = style.size
         else:
-          return "<col min=\"%d\" max=\"%d\" hidden=\"0\" width=\"9.2\" style=\"%d\">" % (col, col, style.id)
-        return "<col min=\"%d\" max=\"%d\" hidden=\"%d\" bestFit=\"%d\" customWidth=\"%d\" width=\"%f\" style=\"%d\">" % (
-            col,
-            col,
-            1 if style.size == 0 else 0,  # hidden
-            1 if style.size == -1 else 0,  # best fit
-            1 if style.size is not None else 0,  # customWidth
-            size,
-            style.id)
+            return '<col min="%d" max="%d" hidden="0" width="9.2" style="%d">' % (
+                col,
+                col,
+                style.id,
+            )
+        return (
+            '<col min="%d" max="%d" hidden="%d" bestFit="%d" customWidth="%d" width="%f" style="%d">'
+            % (
+                col,
+                col,
+                1 if style.size == 0 else 0,  # hidden
+                1 if style.size == -1 else 0,  # best fit
+                1 if style.size is not None else 0,  # customWidth
+                size,
+                style.id,
+            )
+        )
 
     def get_row_xml_string(self, row):
         if row in self._row_styles and not self._row_styles[row].is_default:
             style = self._row_styles[row]
             if style.size == -1:
                 size = 0
-                dense_rows = enumerate(self._dense_cells[row][1:]) if row < len(
-                    self._dense_cells) else []
-                for y, cell in itertools.chain(dense_rows,
-                                               six.iteritems(
-                                                   self._sparse_cells[row])
-                                               if row in self._sparse_cells
-                                               else []):
+                dense_rows = (
+                    enumerate(self._dense_cells[row][1:])
+                    if row < len(self._dense_cells)
+                    else []
+                )
+                for y, cell in itertools.chain(
+                    dense_rows,
+                    six.iteritems(self._sparse_cells[row])
+                    if row in self._sparse_cells
+                    else [],
+                ):
                     try:
                         font_size = self._styles[row][y].font.size
                     except:
                         font_size = 11
-                    lines = cell.count('\n') if DataTypes.get_type(style.size) == DataTypes.STRING else 1
+                    lines = (
+                        cell.count("\n")
+                        if DataTypes.get_type(style.size) == DataTypes.STRING
+                        else 1
+                    )
                     size = max(font_size * (lines + 1) * 4 / 3, size)
             else:
                 size = style.size if style.size else 15
-            return "<row r=\"%d\" s=\"%d\" customFormat=\"1\" hidden=\"%d\" customHeight=\"%d\" ht=\"%f\">" % (
-                row,
-                style.id,
-                1 if style.size == 0 else 0,  # hidden
-                1 if style.size is not None else 0,  # customHeight
-                size)
+            return (
+                '<row r="%d" s="%d" customFormat="1" hidden="%d" customHeight="%d" ht="%f">'
+                % (
+                    row,
+                    style.id,
+                    1 if style.size == 0 else 0,  # hidden
+                    1 if style.size is not None else 0,  # customHeight
+                    size,
+                )
+            )
         else:
-            return "<row r=\"%d\">" % row
+            return '<row r="%d">' % row
 
     def get_xml_data(self):
         # Precondition: styles are aligned. if not, then :v
         # check if we have any row styles that don't have data
         sparse_rows = sorted(
-            filter(lambda x: x[0] >= len(self._dense_cells),
-                   six.iteritems(self._sparse_cells)))
-        for x, row in itertools.chain(
-                enumerate(self._dense_cells[1:], 1), sparse_rows):
+            filter(
+                lambda x: x[0] >= len(self._dense_cells),
+                six.iteritems(self._sparse_cells),
+            )
+        )
+        for x, row in itertools.chain(enumerate(self._dense_cells[1:], 1), sparse_rows):
             row_data = []
-            dense_columns = enumerate(row[1:],
-                                      1) if x < len(self._dense_cells) else []
+            dense_columns = enumerate(row[1:], 1) if x < len(self._dense_cells) else []
             sparse_columns = sorted(
-                six.iteritems(self._sparse_cells[x])
-                if x in self._sparse_cells else [])
+                six.iteritems(self._sparse_cells[x]) if x in self._sparse_cells else []
+            )
             for y, cell in itertools.chain(dense_columns, sparse_columns):
                 if x in self._styles and y in self._styles[x]:
                     style = self._styles[x][y]
                 elif x in self._row_styles:
                     style = self._row_styles[x]
                 elif y in self._col_styles:
                     style = self._col_styles[y]
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/docProps/core.xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/docProps/app.xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/[Content_Types].xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/xl/workbook.xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/xl/workbook.xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/xl/_rels/workbook.xml.rels` & `PyExcelerate-0.9.0/pyexcelerate/templates/xl/_rels/workbook.xml.rels`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/xl/worksheets/sheet.xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/xl/worksheets/sheet.xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/xl/styles.xml` & `PyExcelerate-0.9.0/pyexcelerate/templates/xl/styles.xml`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/templates/_rels/.rels` & `PyExcelerate-0.9.0/pyexcelerate/templates/_rels/.rels`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Range.py` & `PyExcelerate-0.9.0/pyexcelerate/Range.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,64 +6,87 @@
 #
 # Kevin and Kevin's fair warning: this class has been insanely optimized for speed. It is intended
 # to be immutable. Please don't modify attributes after instantiation. :)
 #
 
 
 class Range(object):
-    A = ord('A')
-    Z = ord('Z')
-    __slots__ = ('_start', '_end', 'worksheet', 'is_cell', 'is_row',
-                 'is_column', 'x', 'y', 'height', 'width')
+    A = ord("A")
+    Z = ord("Z")
+    __slots__ = (
+        "_start",
+        "_end",
+        "worksheet",
+        "is_cell",
+        "is_row",
+        "is_column",
+        "x",
+        "y",
+        "height",
+        "width",
+    )
 
     def __init__(self, start, end, worksheet, validate=True):
-        self._start = (Range.string_to_coordinate(start) if validate
-                       and isinstance(start, six.string_types) else start)
-        self._end = (Range.string_to_coordinate(end) if validate
-                     and isinstance(end, six.string_types) else end)
+        self._start = (
+            Range.string_to_coordinate(start)
+            if validate and isinstance(start, six.string_types)
+            else start
+        )
+        self._end = (
+            Range.string_to_coordinate(end)
+            if validate and isinstance(end, six.string_types)
+            else end
+        )
         # Following http://office.microsoft.com/en-ca/excel-help/excel-specifications-and-limits-HA103980614.aspx
-        if (not (1 <= self._start[0] <= 1048576) and self._start[0] != float('inf')) \
-         or (not (1 <= self._end[0] <= 1048576) and self._end[0] != float('inf')):
+        if (
+            not (1 <= self._start[0] <= 1048576) and self._start[0] != float("inf")
+        ) or (not (1 <= self._end[0] <= 1048576) and self._end[0] != float("inf")):
             raise IndexError("Row index out of bounds")
-        if (not (1 <= self._start[1] <= 16384) and self._start[1] != float('inf')) \
-         or (not (1 <= self._end[1] <= 16384) and self._end[1] != float('inf')):
+        if (not (1 <= self._start[1] <= 16384) and self._start[1] != float("inf")) or (
+            not (1 <= self._end[1] <= 16384) and self._end[1] != float("inf")
+        ):
             raise IndexError("Column index out of bounds")
         self.worksheet = worksheet
-        self.is_cell = (self._start == self._end)
+        self.is_cell = self._start == self._end
 
-        self.is_row = (self._end[1] == float('inf')
-                       and self._start[0] == self._end[0]
-                       and self._start[1] == 1)
-        self.is_column = (self._end[0] == float('inf')
-                          and self._start[1] == self._end[1]
-                          and self._start[0] == 1)
-
-        self.x = (self._start[0] if self.is_row or self.is_cell else None)
-        self.y = (self._start[1] if self.is_column or self.is_cell else None)
-        self.height = (self._end[0] - self._start[0] + 1)
-        self.width = (self._end[1] - self._start[1] + 1)
+        self.is_row = (
+            self._end[1] == float("inf")
+            and self._start[0] == self._end[0]
+            and self._start[1] == 1
+        )
+        self.is_column = (
+            self._end[0] == float("inf")
+            and self._start[1] == self._end[1]
+            and self._start[0] == 1
+        )
+
+        self.x = self._start[0] if self.is_row or self.is_cell else None
+        self.y = self._start[1] if self.is_column or self.is_cell else None
+        self.height = self._end[0] - self._start[0] + 1
+        self.width = self._end[1] - self._start[1] + 1
         if self.is_cell:
             worksheet._columns = max(worksheet._columns, self.y)
 
     @property
     def coordinate(self):
         if self.is_cell:
             return self._start
         else:
             raise Exception("Non-singleton range selected")
 
     @property
     def style(self):
         if self.is_row:
-            return self.__get_attr(self.worksheet.get_cell_style,
-                                   Range.AttributeInterceptor(
-                                       self.worksheet.get_row_style(self.x),
-                                       ''))
-        return self.__get_attr(self.worksheet.get_cell_style,
-                               Range.AttributeInterceptor(self, 'style'))
+            return self.__get_attr(
+                self.worksheet.get_cell_style,
+                Range.AttributeInterceptor(self.worksheet.get_row_style(self.x), ""),
+            )
+        return self.__get_attr(
+            self.worksheet.get_cell_style, Range.AttributeInterceptor(self, "style")
+        )
 
     @style.setter
     def style(self, data):
         self.__set_attr(self.worksheet.set_cell_style, data)
 
     @property
     def value(self):
@@ -71,46 +94,49 @@
 
     @value.setter
     def value(self, data):
         self.__set_attr(self.worksheet.set_cell_value, data)
 
     # this class permits doing things like range().style.font.bold = True
     class AttributeInterceptor(object):
-        def __init__(self, parent, attribute=''):
-            self.__dict__['_parent'] = parent
-            self.__dict__['_attribute'] = attribute
+        def __init__(self, parent, attribute=""):
+            self.__dict__["_parent"] = parent
+            self.__dict__["_attribute"] = attribute
 
         def __getattr__(self, name):
-            if self._attribute == '':
+            if self._attribute == "":
                 return Range.AttributeInterceptor(self._parent, name)
-            return Range.AttributeInterceptor(self._parent, "%s.%s" %
-                                              (self._attribute, name))
+            return Range.AttributeInterceptor(
+                self._parent, "%s.%s" % (self._attribute, name)
+            )
 
         def __setattr__(self, name, value):
             if isinstance(self._parent, Style.Style):
                 setattr(
-                    reduce(getattr, self._attribute.split('.'), self._parent),
-                    name, value)
+                    reduce(getattr, self._attribute.split("."), self._parent),
+                    name,
+                    value,
+                )
             else:
                 for cell in self._parent:
                     setattr(
-                        reduce(getattr, self._attribute.split('.'), cell),
-                        name, value)
+                        reduce(getattr, self._attribute.split("."), cell), name, value
+                    )
 
     # note that these are not the python __getattr__/__setattr__
     def __get_attr(self, method, default=None):
         if self.is_cell:
             for merge in self.worksheet.merges:
                 if self in merge:
                     return method(merge._start[0], merge._start[1])
             return method(self.x, self.y)
         elif default:
             return default
         else:
-            raise Exception('Non-singleton range selected')
+            raise Exception("Non-singleton range selected")
 
     def __set_attr(self, method, data):
         if self.is_cell:
             for merge in self.worksheet.merges:
                 if self in merge:
                     method(merge._start[0], merge._start[1], data)
                     return
@@ -124,65 +150,71 @@
                 cell.__set_attr(method, data)
         else:
             if len(data) <= self.height:
                 for row in data:
                     if len(row) > self.width:
                         raise Exception(
                             "Row too large for range, row has %s columns, but range only has %s"
-                            % (len(row), self.width))
+                            % (len(row), self.width)
+                        )
                 for x, row in enumerate(data):
                     for y, value in enumerate(row):
                         method(x + self._start[0], y + self._start[1], value)
             else:
                 raise Exception(
                     "Too many rows for range, data has %s rows, but range only has %s"
-                    % (len(data), self.height))
+                    % (len(data), self.height)
+                )
 
     def intersection(self, range):
         """
 		Calculates the intersection with another range object
 		"""
         if self.worksheet != range.worksheet:
             # Different worksheet
             return None
-        start = (max(self._start[0], range._start[0]),
-                 max(self._start[1], range._start[1]))
-        end = (min(self._end[0], range._end[0]),
-               min(self._end[1], range._end[1]))
+        start = (
+            max(self._start[0], range._start[0]),
+            max(self._start[1], range._start[1]),
+        )
+        end = (min(self._end[0], range._end[0]), min(self._end[1], range._end[1]))
         if end[0] < start[0] or end[1] < start[1]:
             return None
         return Range(start, end, self.worksheet, validate=False)
 
     __and__ = intersection
 
     def intersects(self, range):
         return self.intersection(range) is not None
 
     def merge(self):
         self.worksheet.add_merge(self)
 
     def __iter__(self):
         if self.is_row or self.is_column:
-            raise Exception('Can\'t iterate over an infinite row/column')
+            raise Exception("Can't iterate over an infinite row/column")
         for x in range(self._start[0], self._end[0] + 1):
             for y in range(self._start[1], self._end[1] + 1):
                 yield Range((x, y), (x, y), self.worksheet, validate=False)
 
     def __contains__(self, item):
         return self.intersection(item) == item
 
     def __hash__(self):
         def hash(val):
             return val[0] << 8 + val[1]
 
         return hash(self._start) << 24 + hash(self._end)
 
     def __str__(self):
-        return Range.coordinate_to_string(
-            self._start) + ":" + Range.coordinate_to_string(self._end)
+        return (
+            Range.coordinate_to_string(self._start)
+            + ":"
+            + Range.coordinate_to_string(self._end)
+        )
 
     def __len__(self):
         if self._start[0] == self._end[0]:
             return self.width
         else:
             return self.height
 
@@ -195,20 +227,18 @@
         return not (self == other)
 
     def __getitem__(self, key):
         if self.is_row:
             # return the key'th column
             if isinstance(key, six.string_types):
                 key = Range.string_to_coordinate(key)
-            return Range(
-                (self.x, key), (self.x, key), self.worksheet, validate=False)
+            return Range((self.x, key), (self.x, key), self.worksheet, validate=False)
         elif self.is_column:
-            #return the key'th row
-            return Range(
-                (key, self.y), (key, self.y), self.worksheet, validate=False)
+            # return the key'th row
+            return Range((key, self.y), (key, self.y), self.worksheet, validate=False)
         else:
             raise Exception("Selection not valid")
 
     def __setitem__(self, key, value):
         if self.is_row:
             self.worksheet.set_cell_value(self.x, key, value)
         else:
@@ -228,18 +258,18 @@
         if len(s) == l:
             return y
         else:
             return (int(s), y)
 
     @staticmethod
     def coordinate_to_string(coord):
-        if coord[1] == float('inf'):
-            return 'IV%s' % str(coord[0])
+        if coord[1] == float("inf"):
+            return "IV%s" % str(coord[0])
 
         # convert an integer to base-26 name
         y = coord[1] - 1
-        s = ''
+        s = ""
         while y >= 0:
             d, m = divmod(y, 26)
             s = chr(m + Range.A) + s
             y = d - 1
         return s + str(coord[0])
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Fill.py` & `PyExcelerate-0.9.0/pyexcelerate/Fill.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from . import Utility
 from . import Color
 
 
 class Fill(object):
-    __slots__ = ('_background', 'id')
+    __slots__ = ("_background", "id")
 
     def __init__(self, background=None):
         self._background = background
 
     @property
     def background(self):
-        return Utility.lazy_get(self, '_background', Color.Color())
+        return Utility.lazy_get(self, "_background", Color.Color())
 
     @background.setter
     def background(self, value):
-        Utility.lazy_set(self, '_background', None, value)
+        Utility.lazy_set(self, "_background", None, value)
 
     @property
     def is_default(self):
         return self == Fill()
 
     def __eq__(self, other):
         if other is None:
@@ -28,29 +28,32 @@
     def __hash__(self):
         return hash(self.background)
 
     def get_xml_string(self):
         if not self.background:
             return '<fill><patternFill patternType="none"/></fill>'
         else:
-            return "<fill><patternFill patternType=\"solid\"><fgColor rgb=\"%s\"/></patternFill></fill>" % self.background.hex
+            return (
+                '<fill><patternFill patternType="solid"><fgColor rgb="%s"/></patternFill></fill>'
+                % self.background.hex
+            )
 
     def __or__(self, other):
         return Fill(
-            background=Utility.nonboolean_or(self._background,
-                                             other._background, None))
+            background=Utility.nonboolean_or(self._background, other._background, None)
+        )
 
     def __and__(self, other):
         return Fill(
-            background=Utility.nonboolean_and(self._background,
-                                              other._background, None))
+            background=Utility.nonboolean_and(self._background, other._background, None)
+        )
 
     def __xor__(self, other):
         return Fill(
-            background=Utility.nonboolean_xor(self._background,
-                                              other._background, None))
+            background=Utility.nonboolean_xor(self._background, other._background, None)
+        )
 
     def __str__(self):
         return "Fill: #%s" % self.background.hex
 
     def __repr__(self):
         return "<%s>" % self.__str__()
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Alignment.py` & `PyExcelerate-0.9.0/pyexcelerate/Alignment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,102 +1,117 @@
 import six
 from . import Utility
 from . import Color
 
 
 class Alignment(object):
-    __slots__ = ('_horizontal', '_vertical', '_rotation', '_wrap_text', 'id')
+    __slots__ = ("_horizontal", "_vertical", "_rotation", "_wrap_text", "id")
 
-    def __init__(self,
-                 horizontal='left',
-                 vertical='bottom',
-                 rotation=0,
-                 wrap_text=False):
+    def __init__(
+        self, horizontal="left", vertical="bottom", rotation=0, wrap_text=False
+    ):
         self._horizontal = horizontal
         self._vertical = vertical
         self._rotation = rotation
         self._wrap_text = wrap_text
 
     @property
     def wrap_text(self):
         return self._wrap_text
 
     @wrap_text.setter
     def wrap_text(self, value):
         if value not in (True, False):
             raise TypeError(
-                'Invalid wrap text alignment value. Expects either True or False.'
+                "Invalid wrap text alignment value. Expects either True or False."
             )
         self._wrap_text = value
 
     @property
     def horizontal(self):
         return self._horizontal
 
     @horizontal.setter
     def horizontal(self, value):
-        if value not in ('left', 'center', 'right'):
+        if value not in ("left", "center", "right"):
             raise ValueError(
-                'Invalid horizontal alignment value. Expects either \'left\', \'center\', or \'right\'.'
+                "Invalid horizontal alignment value. Expects either 'left', 'center', or 'right'."
             )
         self._horizontal = value
 
     @property
     def vertical(self):
         return self._vertical
 
     @vertical.setter
     def vertical(self, value):
-        if value not in ('top', 'center', 'bottom'):
+        if value not in ("top", "center", "bottom"):
             raise ValueError(
-                'Invalid vertical alignment value. Expects either \'top\', \'center\', or \'bottom\'.'
+                "Invalid vertical alignment value. Expects either 'top', 'center', or 'bottom'."
             )
         self._vertical = value
 
     @property
     def rotation(self):
         return self._rotation
 
     @rotation.setter
     def rotation(self, value):
-        self._rotation = (value % 360)
+        self._rotation = value % 360
 
     @property
     def is_default(self):
-        return self._horizontal == 'left' and self._vertical == 'bottom' and self._rotation == 0 and not self._wrap_text
+        return (
+            self._horizontal == "left"
+            and self._vertical == "bottom"
+            and self._rotation == 0
+            and not self._wrap_text
+        )
 
     def get_xml_string(self):
-        return "<alignment horizontal=\"%s\" vertical=\"%s\" textRotation=\"%.15g\" wrapText=\"%d\"/>" % (
-            self._horizontal, self._vertical, self._rotation, 1
-            if self._wrap_text else 0)
+        return (
+            '<alignment horizontal="%s" vertical="%s" textRotation="%.15g" wrapText="%d"/>'
+            % (
+                self._horizontal,
+                self._vertical,
+                self._rotation,
+                1 if self._wrap_text else 0,
+            )
+        )
 
     def __or__(self, other):
         return self._binary_operation(other, Utility.nonboolean_or)
 
     def __and__(self, other):
         return self._binary_operation(other, Utility.nonboolean_and)
 
     def __xor__(self, other):
         return self._binary_operation(other, Utility.nonboolean_xor)
 
     def _binary_operation(self, other, operation):
-        return Alignment( \
-         horizontal = operation(self._horizontal, other._horizontal, 'left'), \
-         vertical = operation(self._vertical, other._vertical, 'bottom'), \
-         rotation = operation(self._rotation, other._rotation, 0), \
-         wrap_text = operation(self._wrap_text, other._wrap_text, False)
+        return Alignment(
+            horizontal=operation(self._horizontal, other._horizontal, "left"),
+            vertical=operation(self._vertical, other._vertical, "bottom"),
+            rotation=operation(self._rotation, other._rotation, 0),
+            wrap_text=operation(self._wrap_text, other._wrap_text, False),
         )
 
     def __eq__(self, other):
         if other is None:
             return self.is_default
         elif Utility.YOLO:
-            return self._vertical == other._vertical and self._rotation == other._rotation
+            return (
+                self._vertical == other._vertical and self._rotation == other._rotation
+            )
         else:
-            return self._vertical == other._vertical and self._rotation == other._rotation and self._horizontal == other._horizontal and self._wrap_text == other._wrap_text
+            return (
+                self._vertical == other._vertical
+                and self._rotation == other._rotation
+                and self._horizontal == other._horizontal
+                and self._wrap_text == other._wrap_text
+            )
 
     def __hash__(self):
         return hash((self._horizontal, self._wrap_text))
 
     def __str__(self):
-        return "Align: %s %s %s" % (self._horizontal, self._vertical,
-                                    self._rotation)
+        return "Align: %s %s %s" % (self._horizontal, self._vertical, self._rotation)
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Workbook.py` & `PyExcelerate-0.9.0/pyexcelerate/Workbook.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 import six
 import time
 
 
 class Workbook(object):
     # map for attribute sets => style attribute id's
     STYLE_ATTRIBUTE_MAP = {
-        'fonts': '_font',
-        'fills': '_fill',
-        'num_fmts': '_format',
-        'borders': '_borders'
+        "fonts": "_font",
+        "fills": "_fill",
+        "num_fmts": "_format",
+        "borders": "_borders",
     }
-    STYLE_ID_ATTRIBUTE = 'id'
-    __slots__ = ('_worksheets', '_styles', '_items', '_encoding', '_writer')
+    STYLE_ID_ATTRIBUTE = "id"
+    __slots__ = ("_worksheets", "_styles", "_items", "_encoding", "_writer")
 
-    def __init__(self, encoding='utf-8'):
+    def __init__(self, encoding="utf-8"):
         self._worksheets = []
         self._styles = []
-        self._items = {}  #dictionary containing lists of fonts, fills, etc.
+        self._items = {}  # dictionary containing lists of fonts, fills, etc.
         self._encoding = encoding
         self._writer = Writer(self)
 
     def add_sheet(self, worksheet):
         for sheet in self._worksheets:
             if sheet.name == worksheet.name:
                 raise Exception(
                     "There is already a worksheet with the name '%s'. Duplicate worksheet names are not permitted."
-                    % worksheet.name)
+                    % worksheet.name
+                )
         self._worksheets.append(worksheet)
 
     def new_sheet(self, sheet_name, data=None, force_name=False):
         worksheet = Worksheet.Worksheet(sheet_name, self, data, force_name)
         self.add_sheet(worksheet)
         return worksheet
 
@@ -63,27 +64,24 @@
             if not style.is_default:
                 styles[style] = styles.get(style, len(styles) + 1)
                 setattr(style, Workbook.STYLE_ID_ATTRIBUTE, styles[style])
         for style in styles.keys():
             # compress individual attributes
             for attr, attr_id in Workbook.STYLE_ATTRIBUTE_MAP.items():
                 obj = getattr(style, attr_id)
-                if obj and not obj.is_default:  # we only care about it if it's not default
-                    items[attr][obj] = items[attr].get(obj,
-                                                       len(items[attr]) + 1)
+                if (
+                    obj and not obj.is_default
+                ):  # we only care about it if it's not default
+                    items[attr][obj] = items[attr].get(obj, len(items[attr]) + 1)
                     obj.id = items[attr][obj]  # apply
         for k, v in items.items():
             # ensure it's sorted properly
-            items[k] = [
-                tup[0] for tup in sorted(v.items(), key=lambda x: x[1])
-            ]
+            items[k] = [tup[0] for tup in sorted(v.items(), key=lambda x: x[1])]
         self._items = items
-        self._styles = [
-            tup[0] for tup in sorted(styles.items(), key=lambda x: x[1])
-        ]
+        self._styles = [tup[0] for tup in sorted(styles.items(), key=lambda x: x[1])]
         Utility.YOLO = False
 
     def __getattr__(self, name):
         self._align_styles()
         return self._items[name]
 
     def __len__(self):
@@ -91,11 +89,11 @@
 
     def _save(self, file_handle):
         self._align_styles()
         self._writer.save(file_handle)
 
     def save(self, filename_or_filehandle):
         if isinstance(filename_or_filehandle, six.string_types):
-            with open(filename_or_filehandle, 'wb') as fp:
+            with open(filename_or_filehandle, "wb") as fp:
                 self._save(fp)
         else:
             self._save(filename_or_filehandle)
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Writer.py` & `PyExcelerate-0.9.0/pyexcelerate/Writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,81 +3,86 @@
 import tempfile
 from zipfile import ZipFile, ZIP_DEFLATED
 from datetime import datetime
 import time
 from jinja2 import Environment, FileSystemLoader
 from . import Color
 
-if getattr(sys, 'frozen', False):
-    _basedir = os.path.join(sys._MEIPASS, 'pyexcelerate')
+if getattr(sys, "frozen", False):
+    _basedir = os.path.join(sys._MEIPASS, "pyexcelerate")
 else:
     _basedir = os.path.dirname(__file__)
-_TEMPLATE_PATH = os.path.join(_basedir, 'templates')
+_TEMPLATE_PATH = os.path.join(_basedir, "templates")
 
 
 class Writer(object):
-    env = Environment(
-        loader=FileSystemLoader(_TEMPLATE_PATH), auto_reload=False)
+    env = Environment(loader=FileSystemLoader(_TEMPLATE_PATH), auto_reload=False)
     _docProps_app_template = env.get_template("docProps/app.xml")
     _docProps_core_template = env.get_template("docProps/core.xml")
     _content_types_template = env.get_template("[Content_Types].xml")
     _rels_template = env.get_template("_rels/.rels")
     _styles_template = env.get_template("xl/styles.xml")
     _empty_styles_template = env.get_template("xl/styles.empty.xml")
     _workbook_template = env.get_template("xl/workbook.xml")
     _workbook_rels_template = env.get_template("xl/_rels/workbook.xml.rels")
     _worksheet_template = env.get_template("xl/worksheets/sheet.xml")
-    __slots__ = ('workbook', )
+    __slots__ = ("workbook",)
 
     def __init__(self, workbook):
         self.workbook = workbook
 
     def _render_template_wb(self, template, extra_context=None):
-        context = {'workbook': self.workbook}
+        context = {"workbook": self.workbook}
         if extra_context:
             context.update(extra_context)
-        return template.render(context).encode('utf-8')
+        return template.render(context).encode("utf-8")
 
     def _get_utc_now(self):
         now = datetime.utcnow()
         return now.strftime("%Y-%m-%dT%H:%M:00Z")
 
-    def save(self, f):
-        zf = ZipFile(f, 'w', ZIP_DEFLATED)
-        zf.writestr("docProps/app.xml",
-                    self._render_template_wb(self._docProps_app_template))
-        zf.writestr("docProps/core.xml",
-                    self._render_template_wb(self._docProps_core_template, {
-                        'date': self._get_utc_now()
-                    }))
-        zf.writestr("[Content_Types].xml",
-                    self._render_template_wb(self._content_types_template))
-        zf.writestr("_rels/.rels",
-                    self._rels_template.render().encode('utf-8'))
+    def save(self, file, **kwargs):
+        zf = ZipFile(file, "w", ZIP_DEFLATED, **kwargs)
+        zf.writestr(
+            "docProps/app.xml", self._render_template_wb(self._docProps_app_template)
+        )
+        zf.writestr(
+            "docProps/core.xml",
+            self._render_template_wb(
+                self._docProps_core_template, {"date": self._get_utc_now()}
+            ),
+        )
+        zf.writestr(
+            "[Content_Types].xml",
+            self._render_template_wb(self._content_types_template),
+        )
+        zf.writestr("_rels/.rels", self._rels_template.render().encode("utf-8"))
         if self.workbook.has_styles:
-            zf.writestr("xl/styles.xml",
-                        self._render_template_wb(self._styles_template))
+            zf.writestr(
+                "xl/styles.xml", self._render_template_wb(self._styles_template)
+            )
         else:
-            zf.writestr("xl/styles.xml",
-                        self._render_template_wb(self._empty_styles_template))
-        zf.writestr("xl/workbook.xml",
-                    self._render_template_wb(self._workbook_template))
-        zf.writestr("xl/_rels/workbook.xml.rels",
-                    self._render_template_wb(self._workbook_rels_template))
+            zf.writestr(
+                "xl/styles.xml", self._render_template_wb(self._empty_styles_template)
+            )
+        zf.writestr(
+            "xl/workbook.xml", self._render_template_wb(self._workbook_template)
+        )
+        zf.writestr(
+            "xl/_rels/workbook.xml.rels",
+            self._render_template_wb(self._workbook_rels_template),
+        )
         for index, sheet in self.workbook.get_xml_data():
-            sheetStream = self._worksheet_template.generate({
-                'worksheet': sheet
-            })
+            sheetStream = self._worksheet_template.generate({"worksheet": sheet})
             try:
-                with zf.open(
-                        "xl/worksheets/sheet%s.xml" % (index), mode="w") as f:
+                with zf.open("xl/worksheets/sheet%s.xml" % (index), mode="w") as f:
                     for s in sheetStream:
-                        f.write(s.encode('utf-8'))
+                        f.write(s.encode("utf-8"))
             except RuntimeError:
                 tfd, tfn = tempfile.mkstemp()
-                tf = os.fdopen(tfd, 'wb')
+                tf = os.fdopen(tfd, "wb")
                 for s in sheetStream:
-                    tf.write(s.encode('utf-8'))
+                    tf.write(s.encode("utf-8"))
                 tf.close()
                 zf.write(tfn, "xl/worksheets/sheet%s.xml" % (index))
                 os.remove(tfn)
         zf.close()
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Format.py` & `PyExcelerate-0.9.0/pyexcelerate/Format.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from . import Utility
 import six
 
 
 class Format(object):
-    __slots__ = ('_id', 'format')
+    __slots__ = ("_id", "format")
 
     def __init__(self, format=None):
         self._id = 0  # autopopulated by workbook.py
         self.format = format
 
     def __eq__(self, other):
         if other is None:
             return self.is_default
         return self.format == other.format
 
     def __or__(self, other):
-        return Format(
-            format=Utility.nonboolean_or(self.format, other.format, None))
+        return Format(format=Utility.nonboolean_or(self.format, other.format, None))
 
     def __and__(self, other):
-        return Format(
-            format=Utility.nonboolean_and(self.format, other.format, None))
+        return Format(format=Utility.nonboolean_and(self.format, other.format, None))
 
     def __xor__(self, other):
-        return Format(
-            format=Utility.nonboolean_xor(self.format, other.format, None))
+        return Format(format=Utility.nonboolean_xor(self.format, other.format, None))
 
     def __hash__(self):
         return hash(self.format)
 
     @property
     def is_default(self):
         return self == Format()
@@ -38,12 +35,11 @@
         return self._id
 
     @id.setter
     def id(self, value):
         self._id = value + 1000
 
     def get_xml_string(self):
-        return "<numFmt numFmtId=\"%d\" formatCode=\"%s\"/>" % (self.id,
-                                                                self.format)
+        return '<numFmt numFmtId="%d" formatCode="%s"/>' % (self.id, self.format)
 
     def __str__(self):
         return "Format: %s" % self.format
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Border.py` & `PyExcelerate-0.9.0/pyexcelerate/Border.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 from . import Color
 
 
 #
 # An object representing a single border
 #
 class Border(object):
-    STYLE_MAPPING = { \
-     'dashDot': ('.-', '-.', 'dash dot'), \
-     'dashDotDot': ('..-', '-..', 'dash dot dot'), \
-     'dashed': ('--'), \
-     'dotted': ('..', ':'), \
-     'double': ('='), \
-     'hair': ('hairline', '.'), \
-     'medium': (), \
-     'mediumDashDot': ('medium dash dot', 'medium -.', 'medium .-'), \
-     'mediumDashDotDot': ('medium dash dot dot', 'medium -..', 'medium ..-'), \
-     'mediumDashed': ('medium dashed', 'medium --'), \
-     'slantDashDot': ('/-.', 'slant dash dot'), \
-     'thick': (), \
-     'thin': ('_') \
+    STYLE_MAPPING = {
+        "dashDot": (".-", "-.", "dash dot"),
+        "dashDotDot": ("..-", "-..", "dash dot dot"),
+        "dashed": ("--"),
+        "dotted": ("..", ":"),
+        "double": ("="),
+        "hair": ("hairline", "."),
+        "medium": (),
+        "mediumDashDot": ("medium dash dot", "medium -.", "medium .-"),
+        "mediumDashDotDot": ("medium dash dot dot", "medium -..", "medium ..-"),
+        "mediumDashed": ("medium dashed", "medium --"),
+        "slantDashDot": ("/-.", "slant dash dot"),
+        "thick": (),
+        "thin": ("_"),
     }
 
-    __slots__ = ('_color', '_style', 'id')
+    __slots__ = ("_color", "_style", "id")
 
-    def __init__(self, color=None, style='thin'):
+    def __init__(self, color=None, style="thin"):
         self._color = color
         self._style = Border.get_style_name(style)
 
     @property
     def color(self):
-        return Utility.lazy_get(self, '_color', Color.Color(0, 0, 0))
+        return Utility.lazy_get(self, "_color", Color.Color(0, 0, 0))
 
     @color.setter
     def color(self, value):
-        Utility.lazy_set(self, '_color', None, value)
+        Utility.lazy_set(self, "_color", None, value)
 
     @property
     def style(self):
         return self._style
 
     @style.setter
     def style(self, value):
@@ -46,19 +46,19 @@
 
     @staticmethod
     def get_style_name(style):
         for key, values in Border.STYLE_MAPPING.items():
             if style == key or style in values:
                 return key
         # TODO: warn the user?
-        return 'thin'
+        return "thin"
 
     @property
     def is_default(self):
-        return self._color is None and self._style == 'thin'
+        return self._color is None and self._style == "thin"
 
     def __eq__(self, other):
         if other is None:
             return self.is_default
         elif Utility.YOLO:
             return self._color == other._color
         else:
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Borders.py` & `PyExcelerate-0.9.0/pyexcelerate/Borders.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,112 @@
 import six
 from . import Utility
 from . import Border
 
 
 class Borders(object):
-    __slots__ = ('_left', '_right', '_top', '_bottom', 'id')
+    __slots__ = ("_left", "_right", "_top", "_bottom", "id")
 
     def __init__(self, left=None, right=None, top=None, bottom=None):
         self._left = left
         self._right = right
         self._top = top
         self._bottom = bottom
 
     @property
     def left(self):
-        return Utility.lazy_get(self, '_left', Border.Border())
+        return Utility.lazy_get(self, "_left", Border.Border())
 
     @left.setter
     def left(self, value):
-        Utility.lazy_set(self, '_left', None, value)
+        Utility.lazy_set(self, "_left", None, value)
 
     @property
     def right(self):
-        return Utility.lazy_get(self, '_right', Border.Border())
+        return Utility.lazy_get(self, "_right", Border.Border())
 
     @right.setter
     def right(self, value):
-        Utility.lazy_set(self, '_right', None, value)
+        Utility.lazy_set(self, "_right", None, value)
 
     @property
     def top(self):
-        return Utility.lazy_get(self, '_top', Border.Border())
+        return Utility.lazy_get(self, "_top", Border.Border())
 
     @top.setter
     def top(self, value):
-        Utility.lazy_set(self, '_top', None, value)
+        Utility.lazy_set(self, "_top", None, value)
 
     @property
     def bottom(self):
-        return Utility.lazy_get(self, '_bottom', Border.Border())
+        return Utility.lazy_get(self, "_bottom", Border.Border())
 
     @bottom.setter
     def bottom(self, value):
-        Utility.lazy_set(self, '_bottom', None, value)
+        Utility.lazy_set(self, "_bottom", None, value)
 
     @property
     def is_default(self):
         return not (self._left or self._right or self._top or self._bottom)
 
     def get_xml_string(self):
-        tokens = ['<border>']
+        tokens = ["<border>"]
         if self._left:
-            tokens.append("<left style=\"%s\"><color rgb=\"%s\"/></left>" %
-                          (self._left.style, self._left.color.hex))
+            tokens.append(
+                '<left style="%s"><color rgb="%s"/></left>'
+                % (self._left.style, self._left.color.hex)
+            )
         else:
             tokens.append("<left/>")
         if self._right:
-            tokens.append("<right style=\"%s\"><color rgb=\"%s\"/></right>" %
-                          (self._right.style, self._right.color.hex))
+            tokens.append(
+                '<right style="%s"><color rgb="%s"/></right>'
+                % (self._right.style, self._right.color.hex)
+            )
         else:
             tokens.append("<right/>")
         if self._top:
-            tokens.append("<top style=\"%s\"><color rgb=\"%s\"/></top>" %
-                          (self._top.style, self._top.color.hex))
+            tokens.append(
+                '<top style="%s"><color rgb="%s"/></top>'
+                % (self._top.style, self._top.color.hex)
+            )
         else:
             tokens.append("<top/>")
         if self._bottom:
-            tokens.append("<bottom style=\"%s\"><color rgb=\"%s\"/></bottom>" %
-                          (self._bottom.style, self._bottom.color.hex))
+            tokens.append(
+                '<bottom style="%s"><color rgb="%s"/></bottom>'
+                % (self._bottom.style, self._bottom.color.hex)
+            )
         else:
             tokens.append("<bottom/>")
         tokens.append("</border>")
-        return ''.join(tokens)
+        return "".join(tokens)
 
     def __or__(self, other):
         return self._binary_operation(other, Utility.nonboolean_or)
 
     def __and__(self, other):
         return self._binary_operation(other, Utility.nonboolean_and)
 
     def __xor__(self, other):
         return self._binary_operation(other, Utility.nonboolean_xor)
 
     def _binary_operation(self, other, operation):
-        return Borders( \
-         top = operation(self._top, other._top, None), \
-         left = operation(self._left, other._left, None), \
-         right = operation(self._right, other._right, None), \
-         bottom = operation(self._bottom, other._bottom, None) \
+        return Borders(
+            top=operation(self._top, other._top, None),
+            left=operation(self._left, other._left, None),
+            right=operation(self._right, other._right, None),
+            bottom=operation(self._bottom, other._bottom, None),
         )
 
     def __eq__(self, other):
         if other is None:
             return self.is_default
-        return self._right == other._right and self._bottom == other._bottom and self._top == other._top and self._left == other._left
+        return (
+            self._right == other._right
+            and self._bottom == other._bottom
+            and self._top == other._top
+            and self._left == other._left
+        )
 
     def __hash__(self):
         return hash((self._top, self._left))
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/DataTypes.py` & `PyExcelerate-0.9.0/pyexcelerate/DataTypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from datetime import datetime, date, time
 import decimal
-import six
 import warnings
+from datetime import date, datetime, time
+
+import six
+
 try:
     import numpy as np
+
     HAS_NUMPY = True
 except:
     HAS_NUMPY = False
 
 
 class DataTypes(object):
     BOOLEAN = 0
@@ -22,58 +25,66 @@
 
     _numberTypes = six.integer_types + (float, complex, decimal.Decimal)
 
     @staticmethod
     def get_type(value):
         # Using value.__class__ over isinstance for speed
         if value.__class__ in six.string_types:
-            if len(value) > 0 and value[0] == '=':
+            if len(value) > 0 and value[0] == "=":
                 return DataTypes.FORMULA
             else:
                 return DataTypes.INLINE_STRING
         # not using in (int, float, long, complex) for speed
         elif value.__class__ == bool:
             return DataTypes.BOOLEAN
         elif value.__class__ in DataTypes._numberTypes:
             return DataTypes.NUMBER
         # fall back to the slower isinstance
         elif isinstance(value, six.string_types):
-            if len(value) > 0 and value[0] == '=':
+            if len(value) > 0 and value[0] == "=":
                 return DataTypes.FORMULA
             else:
                 return DataTypes.INLINE_STRING
         elif isinstance(value, bool):
             return DataTypes.BOOLEAN
         elif isinstance(value, DataTypes._numberTypes):
             return DataTypes.NUMBER
         elif HAS_NUMPY and isinstance(
-                value,
-            (np.floating, np.integer, np.complexfloating, np.unsignedinteger)):
+            value, (np.floating, np.integer, np.complexfloating, np.unsignedinteger)
+        ):
             return DataTypes.NUMBER
         elif isinstance(value, (datetime, date, time)):
             return DataTypes.DATE
         else:
             return DataTypes.ERROR
 
     @staticmethod
     def to_excel_date(d):
         if isinstance(d, datetime):
             if d.tzinfo is not None:
                 warnings.warn(
-                    'Excel does not support timestamps with time zone information. Time zones will be ignored.'
+                    "Excel does not support timestamps with time zone information. Time zones will be ignored."
                 )
             delta = d.replace(tzinfo=None) - DataTypes.EXCEL_BASE_DATE
-            excel_date = delta.days + (
-                float(delta.seconds) + float(delta.microseconds) / 1E6) / (
-                    60 * 60 * 24) + 1
+            excel_date = (
+                delta.days
+                + (float(delta.seconds) + float(delta.microseconds) / 1e6)
+                / (60 * 60 * 24)
+                + 1
+            )
             return excel_date + (excel_date > 59)
         elif isinstance(d, date):
             # this is why python sucks >.<
             return DataTypes.to_excel_date(datetime(*(d.timetuple()[:6])))
         elif isinstance(d, time):
-            return DataTypes.to_excel_date(
-                datetime(
-                    *(DataTypes.EXCEL_BASE_DATE.timetuple()[:3]),
-                    hour=d.hour,
-                    minute=d.minute,
-                    second=d.second,
-                    microsecond=d.microsecond)) - 1
+            return (
+                DataTypes.to_excel_date(
+                    datetime(
+                        *(DataTypes.EXCEL_BASE_DATE.timetuple()[:3]),
+                        hour=d.hour,
+                        minute=d.minute,
+                        second=d.second,
+                        microsecond=d.microsecond
+                    )
+                )
+                - 1
+            )
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Utility.py` & `PyExcelerate-0.9.0/pyexcelerate/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 def nonboolean_or(left, right, default=False):
     if default == False:
         return left | right
     if left == default:
         return right
     if right == default or left == right:
         return left
-    return left | right  # this scenario doesn't actually make sense, but it might be implemented
+    return (
+        left | right
+    )  # this scenario doesn't actually make sense, but it might be implemented
 
 
 def nonboolean_and(left, right, default=False):
     if default == False:
         return left & right
     if left == right:
         return left
@@ -47,15 +49,17 @@
 
 if six.PY2:
 
     def to_unicode(s):
         if type(s) == unicode:
             return s
         else:
-            return unicode(s, 'utf-8')
+            return unicode(s, "utf-8")
+
+
 else:
 
     def to_unicode(s):
         return s
 
 
 YOLO = False  # are we aligning?
```

### Comparing `PyExcelerate-0.8.0/pyexcelerate/Color.py` & `PyExcelerate-0.9.0/pyexcelerate/Color.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 class Color(object):
-    __slots__ = ('r', 'g', 'b', 'a')
+    __slots__ = ("r", "g", "b", "a")
 
     def __init__(self, r=255, g=255, b=255, a=255):
         self.r = r
         self.g = g
         self.b = b
         self.a = a
 
     @property
     def hex(self):
-        return '%0.2X%0.2X%0.2X%0.2X' % (self.a, self.r, self.g, self.b)
+        return "%0.2X%0.2X%0.2X%0.2X" % (self.a, self.r, self.g, self.b)
 
     def __hash__(self):
         return (self.a << 24) + (self.r << 16) + (self.g << 8) + (self.b)
 
     def __eq__(self, other):
         if not other:
             return False
-        return self.r == other.r and self.g == other.g and self.b == other.b and self.a == other.a
+        return (
+            self.r == other.r
+            and self.g == other.g
+            and self.b == other.b
+            and self.a == other.a
+        )
 
     def __str__(self):
         return self.hex
 
 
 Color.WHITE = Color(255, 255, 255, 255)
-Color.BLACK = Color(0, 0, 0, 255)
+Color.BLACK = Color(0, 0, 0, 255)
```

### Comparing `PyExcelerate-0.8.0/PKG-INFO` & `PyExcelerate-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyExcelerate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Accelerated Excel XLSX Writing Library for Python 2/3
 Home-page: https://github.com/kz26/PyExcelerate
 Author: Kevin Wang, Kevin Zhang
 Author-email: kevin+pyexcelerate@kevinzhang.me
 Maintainer: Kevin Zhang
 Maintainer-email: kevin+pyexcelerate@kevinzhang.me
 License: UNKNOWN
@@ -396,13 +396,13 @@
         .. |coverage-status| image:: https://coveralls.io/repos/kz26/PyExcelerate/badge.png
            :target: https://coveralls.io/r/kz26/PyExcelerate
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
```

### Comparing `PyExcelerate-0.8.0/CHANGELOG.md` & `PyExcelerate-0.9.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.0
+* Fix unintentional trimming of whitespace on strings
+* Filter invalid XML characters to prevent corrupted Excel files from being saved
+
 0.8.0
 * Add ability to enable auto filters
 * Add ability to write to file handle
 
 0.7.3
 * Performance optimizations
 * Fix invalid function/formula references in third-party spreadsheet software
```

### Comparing `PyExcelerate-0.8.0/README.rst` & `PyExcelerate-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyExcelerate-0.8.0/setup.py` & `PyExcelerate-0.9.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 #!/usr/bin/python
 
 from setuptools import setup
 
 setup(
-	name="PyExcelerate",
-	version='0.8.0',
-	author="Kevin Wang, Kevin Zhang",
-	author_email="kevin+pyexcelerate@kevinzhang.me",
-	maintainer="Kevin Zhang",
-	maintainer_email="kevin+pyexcelerate@kevinzhang.me",
-	url="https://github.com/kz26/PyExcelerate",
-	description="Accelerated Excel XLSX Writing Library for Python 2/3",
-	long_description=open('README.rst').read(),
-	install_requires=[
-		'Jinja2',
-		'six>=1.4.0'
-	],
-	packages=[	
-		'pyexcelerate'
-	],
-	package_data={
-		'pyexcelerate': [
-			'templates/*.xml',
-			'templates/_rels/.rels',
-			'templates/docProps/*.xml',
-			'templates/xl/*.xml',
-			'templates/xl/_rels/*',
-			'templates/xl/worksheets/*.xml',
-		]
-	},
-	classifiers=[
-		'Development Status :: 4 - Beta',
-		'Intended Audience :: Developers',
-		'License :: OSI Approved :: BSD License',
-		'Programming Language :: Python :: 2.6',
-		'Programming Language :: Python :: 2.7',
-		'Programming Language :: Python :: 3.3',
-		'Programming Language :: Python :: 3.4',
-		'Programming Language :: Python :: 3.5',
-		'Programming Language :: Python :: 3.6'
-	]
-
+    name="PyExcelerate",
+    version="0.9.0",
+    author="Kevin Wang, Kevin Zhang",
+    author_email="kevin+pyexcelerate@kevinzhang.me",
+    maintainer="Kevin Zhang",
+    maintainer_email="kevin+pyexcelerate@kevinzhang.me",
+    url="https://github.com/kz26/PyExcelerate",
+    description="Accelerated Excel XLSX Writing Library for Python 2/3",
+    long_description=open("README.rst").read(),
+    install_requires=["Jinja2", "six>=1.4.0"],
+    packages=["pyexcelerate"],
+    package_data={
+        "pyexcelerate": [
+            "templates/*.xml",
+            "templates/_rels/.rels",
+            "templates/docProps/*.xml",
+            "templates/xl/*.xml",
+            "templates/xl/_rels/*",
+            "templates/xl/worksheets/*.xml",
+        ]
+    },
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+    ],
 )
```

### Comparing `PyExcelerate-0.8.0/README.md` & `PyExcelerate-0.9.0/README.md`

 * *Files identical despite different names*

