# Comparing `tmp/PytorchWildlife-1.0.2.9.tar.gz` & `tmp/PytorchWildlife-1.0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PytorchWildlife-1.0.2.9.tar", last modified: Fri Apr 12 00:51:23 2024, max compression
+gzip compressed data, was "PytorchWildlife-1.0.2.9.1.tar", last modified: Fri Apr 12 01:06:15 2024, max compression
```

## Comparing `PytorchWildlife-1.0.2.9.tar` & `PytorchWildlife-1.0.2.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/
--rw-rw-rw-   0        0        0     1091 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/LICENSE
--rw-rw-rw-   0        0        0    20866 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:22.974611 PytorchWildlife-1.0.2.9/PW_FT_classification/
--rw-rw-rw-   0        0        0       38 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PW_FT_classification/__init__.py
--rw-rw-rw-   0        0        0     7627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PW_FT_classification/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:22.984142 PytorchWildlife-1.0.2.9/PytorchWildlife/
--rw-rw-rw-   0        0        0      324 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.046106 PytorchWildlife-1.0.2.9/PytorchWildlife/data/
--rw-rw-rw-   0        0        0       50 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/__init__.py
--rw-rw-rw-   0        0        0     3884 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/datasets.py
--rw-rw-rw-   0        0        0     5685 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.054540 PytorchWildlife-1.0.2.9/PytorchWildlife/models/
--rw-rw-rw-   0        0        0       55 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.063002 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/
--rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.117808 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/
--rw-rw-rw-   0        0        0      103 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/__init__.py
--rw-rw-rw-   0        0        0     3267 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/amazon.py
--rw-rw-rw-   0        0        0     5470 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/base_classifier.py
--rw-rw-rw-   0        0        0     2367 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/opossum.py
--rw-rw-rw-   0        0        0     2627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/serengeti.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.126222 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/
--rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.158140 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/
--rw-rw-rw-   0        0        0       57 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/__init__.py
--rw-rw-rw-   0        0        0     6648 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/base_detector.py
--rw-rw-rw-   0        0        0     1546 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/megadetector.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.188442 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/
--rw-rw-rw-   0        0        0       48 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/misc.py
--rw-rw-rw-   0        0        0    10090 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/post_process.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.017998 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/
--rw-rw-rw-   0        0        0    20866 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1098 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19962 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1472 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.696855 PytorchWildlife-1.0.2.9.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/LICENSE
+-rw-rw-rw-   0        0        0    20868 2024-04-12 01:06:15.695846 PytorchWildlife-1.0.2.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.645619 PytorchWildlife-1.0.2.9.1/PW_FT_classification/
+-rw-rw-rw-   0        0        0       38 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PW_FT_classification/__init__.py
+-rw-rw-rw-   0        0        0     7627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PW_FT_classification/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.646620 PytorchWildlife-1.0.2.9.1/PytorchWildlife/
+-rw-rw-rw-   0        0        0      324 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.673964 PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/
+-rw-rw-rw-   0        0        0       50 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/__init__.py
+-rw-rw-rw-   0        0        0     3884 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/datasets.py
+-rw-rw-rw-   0        0        0     5685 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.675283 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/
+-rw-rw-rw-   0        0        0       55 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.676293 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/
+-rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.681168 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/
+-rw-rw-rw-   0        0        0      103 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/__init__.py
+-rw-rw-rw-   0        0        0     3267 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/amazon.py
+-rw-rw-rw-   0        0        0     5470 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/base_classifier.py
+-rw-rw-rw-   0        0        0     2367 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/opossum.py
+-rw-rw-rw-   0        0        0     2627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/serengeti.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.681168 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/
+-rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.684563 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/
+-rw-rw-rw-   0        0        0       57 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/__init__.py
+-rw-rw-rw-   0        0        0     6648 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/base_detector.py
+-rw-rw-rw-   0        0        0     1546 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/megadetector.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.694845 PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/
+-rw-rw-rw-   0        0        0       48 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/misc.py
+-rw-rw-rw-   0        0        0    10741 2024-04-12 01:05:54.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/post_process.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:06:15.671637 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/
+-rw-rw-rw-   0        0        0    20868 2024-04-12 01:06:15.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2024-04-12 01:06:15.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 01:06:15.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-04-12 01:06:15.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-04-12 01:06:15.000000 PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19962 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 01:06:15.696855 PytorchWildlife-1.0.2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-12 01:05:54.000000 PytorchWildlife-1.0.2.9.1/setup.py
```

### Comparing `PytorchWildlife-1.0.2.9/LICENSE` & `PytorchWildlife-1.0.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PKG-INFO` & `PytorchWildlife-1.0.2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PytorchWildlife
-Version: 1.0.2.9
+Version: 1.0.2.9.1
 Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
 Home-page: https://github.com/microsoft/CameraTraps/
 Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
 License: MIT
 Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9 Summary: a PyTorch
-Collaborative Deep Learning Framework for Conservation. Home-page: https://
-github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
-Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
-Keywords:
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9.1 Summary: a
+PyTorch Collaborative Deep Learning Framework for Conservation. Home-page:
+https://github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi
+Miao Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
+License: MIT Keywords:
 pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `PytorchWildlife-1.0.2.9/PW_FT_classification/main.py` & `PytorchWildlife-1.0.2.9.1/PW_FT_classification/main.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/data/datasets.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/datasets.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/data/transforms.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/data/transforms.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/amazon.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/amazon.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/base_classifier.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/base_classifier.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/opossum.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/opossum.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/serengeti.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/classification/resnet/serengeti.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/base_detector.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/base_detector.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/megadetector.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/models/detection/yolov5/megadetector.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/utils/misc.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife/utils/post_process.py` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife/utils/post_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,38 +79,51 @@
                     image=cv2.cvtColor(cropped_img, cv2.COLOR_RGB2BGR),
                     image_name="{}_{}_{}".format(
                         int(cat), i, entry["img_id"].rsplit(os.sep, 1)[1]
                     ),
                 )
 
 
-def save_detection_json(results, output_dir, categories=None):
+def save_detection_json(results, output_dir, categories=None, exclude_category_ids=[]):
     """
     Save detection results to a JSON file.
 
     Args:
         results (list):
             Detection results containing image ID, bounding boxes, category, and confidence.
         output_dir (str):
             Path to save the output JSON file.
         categories (list, optional):
             List of categories for detected objects. Defaults to None.
+        exclude_category_ids (list, optional):
+            List of category IDs to exclude from the output. Defaults to []. Category IDs can be found in the definition of each models.
     """
     json_results = {"annotations": [], "categories": categories}
     with open(output_dir, "w") as f:
         for r in results:
-            json_results["annotations"].append(
-                {
-                    "img_id": r["img_id"],
-                    "bbox": r["detections"].xyxy.astype(int).tolist(),
-                    "category": r["detections"].class_id.tolist(),
-                    "confidence": r["detections"].confidence.tolist(),
-                }
-            )
-        json.dump(json_results, f)
+
+            # Category filtering
+            img_id = r["img_id"]
+            category = r["detections"].class_id
+
+            bbox = r["detections"].xyxy.astype(int)[~np.isin(category, exclude_category_ids)]
+            confidence =  r["detections"].confidence[~np.isin(category, exclude_category_ids)]
+            category = category[~np.isin(category, exclude_category_ids)]
+
+            if not all([x in exclude_category_ids for x in category]):
+                json_results["annotations"].append(
+                    {
+                        "img_id": img_id,
+                        "bbox": bbox.tolist(),
+                        "category": category.tolist(),
+                        "confidence": confidence.tolist(),
+                    }
+                )
+
+        json.dump(json_results, f, indent=4)
 
 def save_detection_timelapse_json(det_results, output_dir, categories=None):
     """
     Save detection results to a JSON file.
 
     Args:
         results (list):
```

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/PKG-INFO` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PytorchWildlife
-Version: 1.0.2.9
+Version: 1.0.2.9.1
 Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
 Home-page: https://github.com/microsoft/CameraTraps/
 Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
 License: MIT
 Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9 Summary: a PyTorch
-Collaborative Deep Learning Framework for Conservation. Home-page: https://
-github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
-Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
-Keywords:
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9.1 Summary: a
+PyTorch Collaborative Deep Learning Framework for Conservation. Home-page:
+https://github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi
+Miao Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
+License: MIT Keywords:
 pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/SOURCES.txt` & `PytorchWildlife-1.0.2.9.1/PytorchWildlife.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/README.md` & `PytorchWildlife-1.0.2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.9/setup.py` & `PytorchWildlife-1.0.2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding="utf8") as file:
         long_description = file.read()
 setup(
     name='PytorchWildlife',
-    version='1.0.2.9', 
+    version='1.0.2.9.1', 
     packages=find_packages(),
     url='https://github.com/microsoft/CameraTraps/',  
     license='MIT',
     author='Andres Hernandez, Zhongqi Miao',
     author_email='v-herandres@microsoft.com, zhongqimiao@microsoft.com',  
     description='a PyTorch Collaborative Deep Learning Framework for Conservation.',
     long_description=long_description,
```

