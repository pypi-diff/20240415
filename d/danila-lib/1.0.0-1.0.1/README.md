# Comparing `tmp/danila-lib-1.0.0.tar.gz` & `tmp/danila-lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.0.0.tar", last modified: Mon Apr 15 13:44:22 2024, max compression
+gzip compressed data, was "danila-lib-1.0.1.tar", last modified: Mon Apr 15 14:35:55 2024, max compression
```

## Comparing `danila-lib-1.0.0.tar` & `danila-lib-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.607286 danila-lib-1.0.0/
--rw-rw-rw-   0        0        0     3342 2024-04-15 13:44:22.605291 danila-lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.244913 danila-lib-1.0.0/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.0/danila/__init__.py
--rw-rw-rw-   0        0        0      409 2024-04-15 12:03:36.000000 danila-lib-1.0.0/danila/danila.py
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.537593 danila-lib-1.0.0/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     3342 2024-04-15 13:44:21.000000 danila-lib-1.0.0/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-15 13:44:21.000000 danila-lib-1.0.0/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 13:44:21.000000 danila-lib-1.0.0/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1442 2024-04-15 13:44:21.000000 danila-lib-1.0.0/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 13:44:21.000000 danila-lib-1.0.0/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.551530 danila-lib-1.0.0/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.592346 danila-lib-1.0.0/data/neuro/
--rw-rw-rw-   0        0        0     2962 2024-04-15 13:04:46.000000 danila-lib-1.0.0/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.0/data/neuro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 13:44:22.596325 danila-lib-1.0.0/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.0/data/result/Class_im.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.0/data/result/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-15 13:44:22.673984 danila-lib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-04-15 13:04:46.000000 danila-lib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.376372 danila-lib-1.0.1/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 14:35:55.373387 danila-lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:08:08.000000 danila-lib-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.052832 danila-lib-1.0.1/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.0.1/danila/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-04-15 12:03:36.000000 danila-lib-1.0.1/danila/danila.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.304703 danila-lib-1.0.1/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-04-15 14:35:54.000000 danila-lib-1.0.1/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-04-15 14:35:54.000000 danila-lib-1.0.1/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:35:54.000000 danila-lib-1.0.1/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1881 2024-04-15 14:35:54.000000 danila-lib-1.0.1/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 14:35:54.000000 danila-lib-1.0.1/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.331572 danila-lib-1.0.1/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.0.1/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.341526 danila-lib-1.0.1/data/neuro/
+-rw-rw-rw-   0        0        0     3052 2024-04-15 14:33:09.000000 danila-lib-1.0.1/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.1/data/neuro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:35:55.363431 danila-lib-1.0.1/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.0.1/data/result/Class_im.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.0.1/data/result/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:35:55.418184 danila-lib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-15 14:35:37.000000 danila-lib-1.0.1/setup.py
```

### Comparing `danila-lib-1.0.0/PKG-INFO` & `danila-lib-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is the module for detecting and classifying text on rama pictures
-Home-page: https://github.com/Arseniy-Zhuck/danilav1
+Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
-Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danilav1
+Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: astunparse==1.6.3
+Requires-Dist: backports.tarfile==1.0.0
 Requires-Dist: cachetools==5.3.2
 Requires-Dist: certifi==2023.11.17
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: contourpy==1.2.0
 Requires-Dist: cycler==0.12.1
+Requires-Dist: docutils==0.21.1
 Requires-Dist: easyocr==1.7.1
 Requires-Dist: filelock==3.13.1
 Requires-Dist: flatbuffers==23.5.26
 Requires-Dist: fonttools==4.46.0
 Requires-Dist: fsspec==2023.12.2
 Requires-Dist: gast==0.5.4
 Requires-Dist: gitdb==4.0.11
@@ -33,44 +35,65 @@
 Requires-Dist: google-pasta==0.2.0
 Requires-Dist: grpcio==1.60.0
 Requires-Dist: h5py==3.10.0
 Requires-Dist: idna==3.6
 Requires-Dist: imageio==2.33.1
 Requires-Dist: importlib-metadata==7.0.0
 Requires-Dist: importlib-resources==6.1.1
+Requires-Dist: jaraco.classes==3.4.0
+Requires-Dist: jaraco.context==5.3.0
+Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: keras==2.15.0
+Requires-Dist: keyring==25.1.0
 Requires-Dist: kiwisolver==1.4.5
 Requires-Dist: lazy_loader==0.3
 Requires-Dist: libclang==16.0.6
 Requires-Dist: Markdown==3.5.1
+Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.3
 Requires-Dist: matplotlib==3.8.2
+Requires-Dist: mdurl==0.1.2
 Requires-Dist: ml-dtypes==0.2.0
+Requires-Dist: more-itertools==10.2.0
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: networkx==3.2.1
+Requires-Dist: nh3==0.2.17
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: numpy==1.26.2
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: opencv-python==4.8.1.78
 Requires-Dist: opencv-python-headless==4.8.1.78
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: packaging==23.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: Pillow==10.1.0
+Requires-Dist: pkginfo==1.10.0
 Requires-Dist: protobuf==4.23.4
 Requires-Dist: psutil==5.9.6
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: pyasn1==0.5.1
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pyclipper==1.3.0.post5
+Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: python-bidi==0.4.2
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2023.3.post1
+Requires-Dist: pywin32-ctypes==0.2.2
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: readme_renderer==43.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-oauthlib==1.3.1
+Requires-Dist: requests-toolbelt==1.0.0
+Requires-Dist: rfc3986==2.0.0
+Requires-Dist: rich==13.7.1
+Requires-Dist: rsa==4.9
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: scipy==1.11.4
 Requires-Dist: seaborn==0.13.0
 Requires-Dist: shapely==2.0.2
 Requires-Dist: six==1.16.0
 Requires-Dist: smmap==5.0.1
 Requires-Dist: sympy==1.12
 Requires-Dist: tensorboard==2.15.1
 Requires-Dist: tensorboard-data-server==0.7.2
@@ -80,14 +103,15 @@
 Requires-Dist: tensorflow-io-gcs-filesystem==0.31.0
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: thop==0.1.1.post2209072238
 Requires-Dist: tifffile==2023.12.9
 Requires-Dist: torch==2.1.1
 Requires-Dist: torchvision==0.16.1
 Requires-Dist: tqdm==4.66.1
+Requires-Dist: twine==5.0.0
 Requires-Dist: typing_extensions==4.9.0
 Requires-Dist: tzdata==2023.3
 Requires-Dist: ultralytics==8.0.227
 Requires-Dist: urllib3==2.1.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: zipp==3.17.0
```

### Comparing `danila-lib-1.0.0/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.0.1/danila_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is the module for detecting and classifying text on rama pictures
-Home-page: https://github.com/Arseniy-Zhuck/danilav1
+Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
-Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danilav1
+Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: astunparse==1.6.3
+Requires-Dist: backports.tarfile==1.0.0
 Requires-Dist: cachetools==5.3.2
 Requires-Dist: certifi==2023.11.17
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: contourpy==1.2.0
 Requires-Dist: cycler==0.12.1
+Requires-Dist: docutils==0.21.1
 Requires-Dist: easyocr==1.7.1
 Requires-Dist: filelock==3.13.1
 Requires-Dist: flatbuffers==23.5.26
 Requires-Dist: fonttools==4.46.0
 Requires-Dist: fsspec==2023.12.2
 Requires-Dist: gast==0.5.4
 Requires-Dist: gitdb==4.0.11
@@ -33,44 +35,65 @@
 Requires-Dist: google-pasta==0.2.0
 Requires-Dist: grpcio==1.60.0
 Requires-Dist: h5py==3.10.0
 Requires-Dist: idna==3.6
 Requires-Dist: imageio==2.33.1
 Requires-Dist: importlib-metadata==7.0.0
 Requires-Dist: importlib-resources==6.1.1
+Requires-Dist: jaraco.classes==3.4.0
+Requires-Dist: jaraco.context==5.3.0
+Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: keras==2.15.0
+Requires-Dist: keyring==25.1.0
 Requires-Dist: kiwisolver==1.4.5
 Requires-Dist: lazy_loader==0.3
 Requires-Dist: libclang==16.0.6
 Requires-Dist: Markdown==3.5.1
+Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.3
 Requires-Dist: matplotlib==3.8.2
+Requires-Dist: mdurl==0.1.2
 Requires-Dist: ml-dtypes==0.2.0
+Requires-Dist: more-itertools==10.2.0
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: networkx==3.2.1
+Requires-Dist: nh3==0.2.17
 Requires-Dist: ninja==1.11.1.1
 Requires-Dist: numpy==1.26.2
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: opencv-python==4.8.1.78
 Requires-Dist: opencv-python-headless==4.8.1.78
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: packaging==23.2
 Requires-Dist: pandas==2.1.4
 Requires-Dist: Pillow==10.1.0
+Requires-Dist: pkginfo==1.10.0
 Requires-Dist: protobuf==4.23.4
 Requires-Dist: psutil==5.9.6
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: pyasn1==0.5.1
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pyclipper==1.3.0.post5
+Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: python-bidi==0.4.2
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pytz==2023.3.post1
+Requires-Dist: pywin32-ctypes==0.2.2
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: readme_renderer==43.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-oauthlib==1.3.1
+Requires-Dist: requests-toolbelt==1.0.0
+Requires-Dist: rfc3986==2.0.0
+Requires-Dist: rich==13.7.1
+Requires-Dist: rsa==4.9
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: scipy==1.11.4
 Requires-Dist: seaborn==0.13.0
 Requires-Dist: shapely==2.0.2
 Requires-Dist: six==1.16.0
 Requires-Dist: smmap==5.0.1
 Requires-Dist: sympy==1.12
 Requires-Dist: tensorboard==2.15.1
 Requires-Dist: tensorboard-data-server==0.7.2
@@ -80,14 +103,15 @@
 Requires-Dist: tensorflow-io-gcs-filesystem==0.31.0
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: thop==0.1.1.post2209072238
 Requires-Dist: tifffile==2023.12.9
 Requires-Dist: torch==2.1.1
 Requires-Dist: torchvision==0.16.1
 Requires-Dist: tqdm==4.66.1
+Requires-Dist: twine==5.0.0
 Requires-Dist: typing_extensions==4.9.0
 Requires-Dist: tzdata==2023.3
 Requires-Dist: ultralytics==8.0.227
 Requires-Dist: urllib3==2.1.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: zipp==3.17.0
```

### Comparing `danila-lib-1.0.0/data/neuro/Rama_classify_class.py` & `danila-lib-1.0.1/data/neuro/Rama_classify_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 
 import cv2
 import keras
 import numpy as np
 
 from data.result.Class_im import Class_im
-
+import zipfile
 
 class Rama_classify_class:
     def __init__(self):
-        self.rama_classify_model = keras.models.load_model('models/rama_classify/17_model')
+        with zipfile.ZipFile('17_model.zip', 'r') as zip_ref:
+            zip_ref.extractall()
+        self.rama_classify_model = keras.models.load_model('17_model')
     # сделать картинку чб 512-512
     def prepare_img(self, image_initial):
         img_grey = cv2.cvtColor(image_initial, cv2.COLOR_BGR2GRAY)
         img_grey_size = cv2.resize(img_grey, (512, 512))
         data = np.array(img_grey_size, dtype="float") / 255.0
         data = data.reshape((1, 512, 512))
         return data
```

### Comparing `danila-lib-1.0.0/setup.py` & `danila-lib-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.0.0',
+  version='1.0.1',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
-  url='https://github.com/Arseniy-Zhuck/danilav1',
+  url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
   install_requires=requirements(),
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='rama detect machine-learning computer-vision',
   project_urls={
-    'GitHub': 'https://github.com/Arseniy-Zhuck/danilav1'
+    'GitHub': 'https://github.com/Arseniy-Zhuck/danila_lib'
   },
   python_requires='>=3.6'
 )
```

