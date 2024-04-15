# Comparing `tmp/faster_coco_eval-1.5.1.tar.gz` & `tmp/faster_coco_eval-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_coco_eval-1.5.1.tar", last modified: Sat Apr 13 21:04:00 2024, max compression
+gzip compressed data, was "faster_coco_eval-1.5.2.tar", last modified: Mon Apr 15 09:00:31 2024, max compression
```

## Comparing `faster_coco_eval-1.5.1.tar` & `faster_coco_eval-1.5.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/faster_eval_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.h
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/faster_eval_api.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/common/
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/common/maskApi.c
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/common/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/pycocotools/
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/pycocotools/_mask.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/faster_coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval/core/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/cocoeval.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/faster_eval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.678763 faster_coco_eval-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.670764 faster_coco_eval-1.5.2/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.670764 faster_coco_eval-1.5.2/csrc/faster_eval_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.670764 faster_coco_eval-1.5.2/csrc/faster_eval_api/coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/faster_eval_api/coco_eval/cocoeval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/faster_eval_api/faster_eval_api.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.670764 faster_coco_eval-1.5.2/csrc/mask/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/csrc/mask/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/mask/common/maskApi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/mask/common/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/csrc/mask/pycocotools/
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/csrc/mask/pycocotools/_mask.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/faster_coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/faster_coco_eval/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/core/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/core/cocoeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/core/faster_eval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/core/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/faster_coco_eval/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/extra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/faster_coco_eval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-15 09:00:31.000000 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-15 09:00:31.000000 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:00:31.000000 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 09:00:31.000000 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 09:00:31.000000 faster_coco_eval-1.5.2/faster_coco_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:00:31.674764 faster_coco_eval-1.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/requirements/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:00:31.678763 faster_coco_eval-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-15 09:00:24.000000 faster_coco_eval-1.5.2/setup.py
```

### Comparing `faster_coco_eval-1.5.1/LICENSE` & `faster_coco_eval-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp` & `faster_coco_eval-1.5.2/csrc/faster_eval_api/coco_eval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.h` & `faster_coco_eval-1.5.2/csrc/faster_eval_api/coco_eval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/faster_eval_api/faster_eval_api.cpp` & `faster_coco_eval-1.5.2/csrc/faster_eval_api/faster_eval_api.cpp`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/mask/common/maskApi.c` & `faster_coco_eval-1.5.2/csrc/mask/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/mask/common/maskApi.h` & `faster_coco_eval-1.5.2/csrc/mask/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/csrc/mask/pycocotools/_mask.pyx` & `faster_coco_eval-1.5.2/csrc/mask/pycocotools/_mask.pyx`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/core/coco.py` & `faster_coco_eval-1.5.2/faster_coco_eval/core/coco.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/core/cocoeval.py` & `faster_coco_eval-1.5.2/faster_coco_eval/core/cocoeval.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/core/faster_eval_api.py` & `faster_coco_eval-1.5.2/faster_coco_eval/core/faster_eval_api.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/core/mask.py` & `faster_coco_eval-1.5.2/faster_coco_eval/core/mask.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/extra/curves.py` & `faster_coco_eval-1.5.2/faster_coco_eval/extra/curves.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/extra/display.py` & `faster_coco_eval-1.5.2/faster_coco_eval/extra/display.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/extra/draw.py` & `faster_coco_eval-1.5.2/faster_coco_eval/extra/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import plotly.express as px
 import plotly.graph_objs as go
 from PIL import Image
 
 from ..core import COCO
+from .utils import convert_ann_rle_to_poly
 
 logger = logging.getLogger(__name__)
 
 A = 0.1
 DT_COLOR = (238, 130, 238, A)
 
 GT_COLOR = (0, 255, 0, A)
@@ -30,14 +31,16 @@
     all_y = []
 
     if iouType == "bbox":
         x1, y1, w, h = ann["bbox"]
         all_x = [x1, x1 + w, x1 + w, x1, x1, None]
         all_y = [y1, y1, y1 + h, y1 + h, y1, None]
     else:
+        ann = convert_ann_rle_to_poly(ann)
+
         for poly in ann["segmentation"]:
             if len(poly) > 3:
                 poly += poly[:2]
                 poly = np.array(poly).reshape(-1, 2)
                 all_x += poly[:, 0].tolist() + [None]
                 all_y += poly[:, 1].tolist() + [None]
```

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval/extra/extra.py` & `faster_coco_eval-1.5.2/faster_coco_eval/extra/extra.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self.cocoGt = copy.deepcopy(cocoGt)
         self.cocoDt = copy.deepcopy(cocoDt)
         self.eval = None
 
         assert self.cocoGt is not None, "cocoGt is empty"
 
         if (self.cocoGt is not None) and (self.cocoDt is not None):
+            self.drop_cocodt_by_score(min_score=min_score)
             self.evaluate()
 
     def evaluate(self):
         assert self.cocoDt is not None, "cocoDt is empty"
 
         cocoEval = COCOeval_faster(
             self.cocoGt, self.cocoDt, self.iouType, extra_calc=True
@@ -50,7 +51,33 @@
 
         self.cocoEval = cocoEval
 
         cocoEval.evaluate()
         cocoEval.accumulate()
 
         self.eval = cocoEval.eval
+
+    def drop_cocodt_by_score(self, min_score: float):
+        assert self.cocoDt is not None, "cocoDt is empty"
+
+        if min_score > 0:
+            bad_keys = {}
+            bad_images_keys = []
+
+            for key, ann in self.cocoDt.anns.items():
+                if ann["score"] < min_score:
+                    if bad_keys.get(ann["image_id"]) is None:
+                        bad_keys[ann["image_id"]] = {}
+
+                    bad_keys[ann["image_id"]][key] = True
+
+                    bad_images_keys.append(ann["image_id"])
+
+            for image_id in set(bad_images_keys):
+                self.cocoDt.imgToAnns[image_id] = [
+                    ann
+                    for ann in self.cocoDt.imgToAnns[image_id]
+                    if bad_keys.get(image_id, {}).get(ann["id"]) is None
+                ]
+
+                for ann_id in bad_keys.get(image_id, {}).keys():
+                    del self.cocoDt.anns[ann_id]
```

### Comparing `faster_coco_eval-1.5.1/faster_coco_eval.egg-info/SOURCES.txt` & `faster_coco_eval-1.5.2/faster_coco_eval.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 faster_coco_eval/core/faster_eval_api.py
 faster_coco_eval/core/mask.py
 faster_coco_eval/extra/__init__.py
 faster_coco_eval/extra/curves.py
 faster_coco_eval/extra/display.py
 faster_coco_eval/extra/draw.py
 faster_coco_eval/extra/extra.py
+faster_coco_eval/extra/utils.py
+requirements/extra.txt
 requirements/runtime.txt
```

### Comparing `faster_coco_eval-1.5.1/setup.py` & `faster_coco_eval-1.5.2/setup.py`

 * *Files identical despite different names*

