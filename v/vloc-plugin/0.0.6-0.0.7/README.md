# Comparing `tmp/vloc_plugin-0.0.6.tar.gz` & `tmp/vloc_plugin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vloc_plugin-0.0.6.tar", last modified: Wed Apr 10 06:50:50 2024, max compression
+gzip compressed data, was "vloc_plugin-0.0.7.tar", last modified: Mon Apr 15 08:06:30 2024, max compression
```

## Comparing `vloc_plugin-0.0.6.tar` & `vloc_plugin-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:50:50.011119 vloc_plugin-0.0.6/
--rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.6/LICENSE.txt
--rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-10 06:50:50.010914 vloc_plugin-0.0.6/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.6/README.md
--rw-r--r--   0 byron      (501) staff       (20)      479 2024-04-10 06:50:06.000000 vloc_plugin-0.0.6/pyproject.toml
--rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-10 06:50:50.011162 vloc_plugin-0.0.6/setup.cfg
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:50:50.009077 vloc_plugin-0.0.6/vloc/
--rw-r--r--   0 byron      (501) staff       (20)       74 2024-04-09 02:40:26.000000 vloc_plugin-0.0.6/vloc/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:50:50.009904 vloc_plugin-0.0.6/vloc/plugin/
--rw-r--r--   0 byron      (501) staff       (20)      368 2024-04-09 07:51:05.000000 vloc_plugin-0.0.6/vloc/plugin/__catalog__.py
--rw-r--r--   0 byron      (501) staff       (20)     1431 2024-04-10 06:42:40.000000 vloc_plugin-0.0.6/vloc/plugin/__info__.py
--rw-r--r--   0 byron      (501) staff       (20)       59 2024-04-10 06:38:02.000000 vloc_plugin-0.0.6/vloc/plugin/__init__.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-10 06:50:50.010715 vloc_plugin-0.0.6/vloc_plugin.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-10 06:50:50.000000 vloc_plugin-0.0.6/vloc_plugin.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)      268 2024-04-10 06:50:50.000000 vloc_plugin-0.0.6/vloc_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-10 06:50:50.000000 vloc_plugin-0.0.6/vloc_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-10 06:50:50.000000 vloc_plugin-0.0.6/vloc_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:06:30.561612 vloc_plugin-0.0.7/
+-rw-r--r--   0 byron      (501) staff       (20)     1064 2024-04-08 05:25:44.000000 vloc_plugin-0.0.7/LICENSE.txt
+-rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-15 08:06:30.561421 vloc_plugin-0.0.7/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)        0 2024-04-08 05:25:44.000000 vloc_plugin-0.0.7/README.md
+-rw-r--r--   0 byron      (501) staff       (20)      479 2024-04-15 07:50:49.000000 vloc_plugin-0.0.7/pyproject.toml
+-rw-r--r--   0 byron      (501) staff       (20)       38 2024-04-15 08:06:30.561649 vloc_plugin-0.0.7/setup.cfg
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:06:30.559489 vloc_plugin-0.0.7/vloc/
+-rw-r--r--   0 byron      (501) staff       (20)      179 2024-04-15 07:34:55.000000 vloc_plugin-0.0.7/vloc/__init__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:06:30.560369 vloc_plugin-0.0.7/vloc/plugin/
+-rw-r--r--   0 byron      (501) staff       (20)     1473 2024-04-15 07:33:32.000000 vloc_plugin-0.0.7/vloc/plugin/__info__.py
+-rw-r--r--   0 byron      (501) staff       (20)      145 2024-04-15 07:48:42.000000 vloc_plugin-0.0.7/vloc/plugin/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)      838 2024-04-14 09:57:44.000000 vloc_plugin-0.0.7/vloc/plugin/__plugin__.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2024-04-15 08:06:30.561226 vloc_plugin-0.0.7/vloc_plugin.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)      388 2024-04-15 08:06:30.000000 vloc_plugin-0.0.7/vloc_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)      267 2024-04-15 08:06:30.000000 vloc_plugin-0.0.7/vloc_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2024-04-15 08:06:30.000000 vloc_plugin-0.0.7/vloc_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)        5 2024-04-15 08:06:30.000000 vloc_plugin-0.0.7/vloc_plugin.egg-info/top_level.txt
```

### Comparing `vloc_plugin-0.0.6/LICENSE.txt` & `vloc_plugin-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vloc_plugin-0.0.6/vloc/plugin/__info__.py` & `vloc_plugin-0.0.7/vloc/plugin/__info__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from importlib.util import find_spec
 from dataclasses import dataclass
 import re
 import cv2
 import pytesseract
-from vloc.config import VL
-from vloc.exception import OcrException
+from vloc.module import VlocModule
+from vloc.exception import VlocOcrError
 if find_spec('vloc.plugin.__selenium__'):
-    from vloc.plugin.__selenium__.__info__ import Action as SeleniumAction
+    from vloc.plugin.__selenium__.__info__ import DetectAction as SeleniumDetectAction
 
 
 @dataclass
 class DetectInfo:
     x: int
     y: int
     label: str
     conf: float
     crop: str
     ocr: str = None
 
     def __post_init__(self):
 
-        if any(cls in str(VL.screenshot_method.__self__) for cls in ['selenium', 'appium']):
-            action = SeleniumAction(self.x, self.y, VL.screenshot_method.__self__)
+        if any(cls in str(VlocModule.screenshot_method.__self__) for cls in ['selenium', 'appium']):
+            action = SeleniumDetectAction(self.x, self.y, VlocModule.screenshot_method.__self__)
 
             self.click = action.click
             self.input = action.input
 
     def click(self):
         ...
 
@@ -43,12 +43,12 @@
         config = '--psm 4' if segment else '--psm 7'
 
         txt = str(pytesseract.image_to_string(img, config=config)).replace('\n', '')
 
         if search:
             txt = re.search(search, txt)
             if not txt:
-                raise OcrException(f'text search pattern not contains:{search}')
+                raise VlocOcrError(f'text search pattern not contains:{search}')
             txt = txt.group(0)
 
         txt = re.sub(remove, '', txt).strip() if remove else txt
         return txt
```

