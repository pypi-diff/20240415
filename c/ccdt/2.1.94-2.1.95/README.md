# Comparing `tmp/ccdt-2.1.94.tar.gz` & `tmp/ccdt-2.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.94.tar", last modified: Mon Apr  8 09:54:32 2024, max compression
+gzip compressed data, was "ccdt-2.1.95.tar", last modified: Mon Apr 15 03:39:48 2024, max compression
```

## Comparing `ccdt-2.1.94.tar` & `ccdt-2.1.95.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.854778 ccdt-2.1.94/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.94/LICENSE
--rw-rw-rw-   0        0        0     4806 2024-04-08 09:54:32.853781 ccdt-2.1.94/PKG-INFO
--rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.94/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.643366 ccdt-2.1.94/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.94/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.657307 ccdt-2.1.94/ccdt/dataset/
--rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.94/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.660299 ccdt-2.1.94/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.94/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.94/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.706211 ccdt-2.1.94/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    15199 2023-11-27 03:47:20.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0   115258 2024-03-07 07:48:12.000000 ccdt-2.1.94/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.772036 ccdt-2.1.94/ccdt/dataset/base_voc/
--rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.94/ccdt/dataset/base_voc/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_sys.py
--rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_txt.py
--rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.94/ccdt/dataset/base_voc/base_voc.py
--rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.94/ccdt/dataset/base_voc/coco_to_labelme.py
--rw-rw-rw-   0        0        0    23667 2024-03-07 03:40:15.000000 ccdt-2.1.94/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.778982 ccdt-2.1.94/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.94/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.94/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    27068 2024-02-02 07:58:30.000000 ccdt-2.1.94/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.825856 ccdt-2.1.94/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.94/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.94/ccdt/video_tool/intercept.py
--rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.94/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.94/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.851790 ccdt-2.1.94/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4806 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 09:54:32.000000 ccdt-2.1.94/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 09:54:32.855777 ccdt-2.1.94/setup.cfg
--rw-rw-rw-   0        0        0     2524 2024-04-08 09:54:17.000000 ccdt-2.1.94/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:54:32.840817 ccdt-2.1.94/test/
--rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.94/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.619943 ccdt-2.1.95/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.95/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-15 03:39:48.617973 ccdt-2.1.95/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.95/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.401528 ccdt-2.1.95/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.95/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.417484 ccdt-2.1.95/ccdt/dataset/
+-rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.95/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.460370 ccdt-2.1.95/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.95/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.95/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.496273 ccdt-2.1.95/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    15199 2023-11-27 03:47:20.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0   115264 2024-04-15 03:38:56.000000 ccdt-2.1.95/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.539159 ccdt-2.1.95/ccdt/dataset/base_voc/
+-rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.95/ccdt/dataset/base_voc/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_sys.py
+-rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_txt.py
+-rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.95/ccdt/dataset/base_voc/base_voc.py
+-rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.95/ccdt/dataset/base_voc/coco_to_labelme.py
+-rw-rw-rw-   0        0        0    23667 2024-03-07 03:40:15.000000 ccdt-2.1.95/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.556113 ccdt-2.1.95/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.95/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.95/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    27068 2024-02-02 07:58:30.000000 ccdt-2.1.95/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.594037 ccdt-2.1.95/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.95/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.95/ccdt/video_tool/intercept.py
+-rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.95/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.95/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.616951 ccdt-2.1.95/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 03:39:48.000000 ccdt-2.1.95/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:39:48.619943 ccdt-2.1.95/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2024-04-15 03:39:24.000000 ccdt-2.1.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:39:48.608001 ccdt-2.1.95/test/
+-rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.95/test/test.py
```

### Comparing `ccdt-2.1.94/LICENSE` & `ccdt-2.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/PKG-INFO` & `ccdt-2.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.94
+Version: 2.1.95
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.94/README.md` & `ccdt-2.1.95/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.95/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.95/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.95/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,17 +394,17 @@
         for dataset in tqdm(reversed(self.datasets)):
             if dataset.get('labelme_info'):
                 if dataset.get('labelme_info').get('flags'):  # 如果flags字典不为空
                     # 有=true、没有=false；训练=true、不训练=false；要=true、不要=false；真=true、假=false；1=true、0=false；开=true、关=false；勾选=true、不勾选=false；
                     if parameter.right_check and dataset.get('labelme_info').get('flags').get('1'):  # 勾选1代表保留勾选图像及对应标注的json文件
                         filter_images.append(dataset)
                         # dataset.update({'background': True})  # 同时更新没有标注框的图像不为背景
-                    if parameter.right_check and dataset.get('labelme_info').get('flags').get('0'):  # 勾选0代表删除图像及对应的标注json文件---修改为移动比较靠谱
-                        os.remove(dataset.get('full_path'))  # 删除图像文件
-                        os.remove(dataset.get('json_path'))  # 删除图像对应的标注json文件
+                    # if parameter.right_check and dataset.get('labelme_info').get('flags').get('0'):  # 勾选0代表删除图像及对应的标注json文件---修改为移动比较靠谱
+                    #     os.remove(dataset.get('full_path'))  # 删除图像文件
+                    #     os.remove(dataset.get('json_path'))  # 删除图像对应的标注json文件
         print(f'保存筛选数据开始')
         self.save_labelme(filter_images, self.output_dir, None)
 
     def merge_labelme(self, parameter):
         """
         针对筛选数据集进行合并，筛选后保存的首级目录可以被修改，不影响合并功能
         根据图像文件唯一MD5值，查找标注shape属性并进行合并
```

### Comparing `ccdt-2.1.94/ccdt/dataset/base_voc/base_sys.py` & `ccdt-2.1.95/ccdt/dataset/base_voc/base_sys.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_voc/base_txt.py` & `ccdt-2.1.95/ccdt/dataset/base_voc/base_txt.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_voc/base_voc.py` & `ccdt-2.1.95/ccdt/dataset/base_voc/base_voc.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/base_voc/coco_to_labelme.py` & `ccdt-2.1.95/ccdt/dataset/base_voc/coco_to_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/main.py` & `ccdt-2.1.95/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.95/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.95/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/video_tool/intercept.py` & `ccdt-2.1.95/ccdt/video_tool/intercept.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/video_tool/split.py` & `ccdt-2.1.95/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt/video_tool/video_main.py` & `ccdt-2.1.95/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.95/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.94
+Version: 2.1.95
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.94/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.95/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.94/setup.py` & `ccdt-2.1.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.94',
+    version='2.1.95',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.94/test/test.py` & `ccdt-2.1.95/test/test.py`

 * *Files identical despite different names*

