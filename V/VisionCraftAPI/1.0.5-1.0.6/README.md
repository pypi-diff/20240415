# Comparing `tmp/VisionCraftAPI-1.0.5.tar.gz` & `tmp/VisionCraftAPI-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraftAPI-1.0.5.tar", last modified: Thu Apr 11 19:08:07 2024, max compression
+gzip compressed data, was "VisionCraftAPI-1.0.6.tar", last modified: Mon Apr 15 18:43:07 2024, max compression
```

## Comparing `VisionCraftAPI-1.0.5.tar` & `VisionCraftAPI-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:07.005238 VisionCraftAPI-1.0.5/
--rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2542 2024-04-11 19:08:07.006241 VisionCraftAPI-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.951244 VisionCraftAPI-1.0.5/VisionCraftAPI/
--rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/__init__.py
--rw-rw-rw-   0        0        0    20917 2024-04-11 18:50:01.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.976238 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/
--rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/__init__.py
--rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/modes.py
--rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/enums/task_statuses.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.981240 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/
--rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/types.py
--rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/http_client.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.997240 VisionCraftAPI-1.0.5/VisionCraftAPI/models/
--rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/__init__.py
--rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/limits.py
--rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/llm.py
--rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/midjourney.py
--rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/models/whisper.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:07.004239 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/
--rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.5/VisionCraftAPI/utils/checker.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:08:06.969246 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/
--rw-rw-rw-   0        0        0     2542 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2024-04-11 19:08:06.000000 VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 19:08:07.008240 VisionCraftAPI-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-11 19:07:26.000000 VisionCraftAPI-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.674317 VisionCraftAPI-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-03-28 06:00:02.000000 VisionCraftAPI-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2542 2024-04-15 18:43:07.674317 VisionCraftAPI-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-15 18:35:25.000000 VisionCraftAPI-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.597757 VisionCraftAPI-1.0.6/VisionCraftAPI/
+-rw-rw-rw-   0        0        0       34 2024-03-26 11:28:25.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/__init__.py
+-rw-rw-rw-   0        0        0    21066 2024-04-15 18:36:20.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.653300 VisionCraftAPI-1.0.6/VisionCraftAPI/enums/
+-rw-rw-rw-   0        0        0      125 2024-03-26 22:05:26.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/enums/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-03-26 22:04:43.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/enums/modes.py
+-rw-rw-rw-   0        0        0      162 2024-03-26 22:04:35.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/enums/task_statuses.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.660260 VisionCraftAPI-1.0.6/VisionCraftAPI/exceptions/
+-rw-rw-rw-   0        0        0      309 2024-03-27 16:35:37.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-03-27 16:42:14.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/exceptions/types.py
+-rw-rw-rw-   0        0        0     2067 2024-04-15 18:35:25.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/http_client.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.667251 VisionCraftAPI-1.0.6/VisionCraftAPI/models/
+-rw-rw-rw-   0        0        0      303 2024-03-27 20:35:50.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      336 2024-03-27 20:24:16.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/models/limits.py
+-rw-rw-rw-   0        0        0      147 2024-03-26 17:31:11.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/models/llm.py
+-rw-rw-rw-   0        0        0      488 2024-03-27 20:28:11.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/models/midjourney.py
+-rw-rw-rw-   0        0        0      823 2024-03-27 20:30:01.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/models/whisper.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.674317 VisionCraftAPI-1.0.6/VisionCraftAPI/utils/
+-rw-rw-rw-   0        0        0       69 2024-03-26 22:05:35.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-03-27 16:55:54.000000 VisionCraftAPI-1.0.6/VisionCraftAPI/utils/checker.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:43:07.646356 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/
+-rw-rw-rw-   0        0        0     2542 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2024-04-15 18:43:07.000000 VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 18:43:07.681146 VisionCraftAPI-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-15 18:42:35.000000 VisionCraftAPI-1.0.6/setup.py
```

### Comparing `VisionCraftAPI-1.0.5/LICENSE` & `VisionCraftAPI-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/PKG-INFO` & `VisionCraftAPI-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.5/README.md` & `VisionCraftAPI-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI/api.py` & `VisionCraftAPI-1.0.6/VisionCraftAPI/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,16 @@
                                 model: str,
                                 sampler: str,
                                 width: Optional[int] = 1024,
                                 height: Optional[int] = 1024,
                                 negative_prompt: Optional[str] = str(),
                                 cfg_scale: Optional[int] = 10,
                                 steps: Optional[int] = 30,
-                                image_count: Optional[int] = 1) -> list[str]:
+                                image_count: Optional[int] = 1,
+                                loras: Optional[dict] = {}) -> list[str]:
         """
         Generate an image using StableDiffusion XL models.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/stablediffusion-xl-models/image-generation
         SDK Docs: https://vision.b2k.tech/docs/api-methods/stablediffusion-xl-models/generate_xl_image
         
         :param prompt: A text prompt for image generation
@@ -242,29 +243,31 @@
         :param sampler: A sampler from the list of available samplers
         :param width: Width of the generated image (min: 512, max: 1024, default: 1024)
         :param height: Height of the generated image (min: 512, max: 1024, default: 1024)
         :param negative_prompt: A negative text prompt for image generation
         :param cfg_scale: A scale for the configuration (min: 1, max: 20, default: 10)
         :param steps: Number of steps for image generation (min: 1, max: 30, default: 30)
         :param image_count: Number of images to generate (max: 5, default: 1)
+        :param loras: A dictionary of LORAs for the model
         
         :return: A list of image URLs
         """
         
         json = {
             "prompt": prompt,
             "model": model,
             "negative_prompt": negative_prompt,
             "token": self.api_key,
             "height": height,
             "width": width,
             "sampler": sampler,
             "cfg_scale": cfg_scale,
             "steps": steps,
-            "image_count": image_count
+            "image_count": image_count,
+            "loras": loras
         }
         
         result = await self.__post(f'{self.API_HOST}/generate-xl', json=json)
         return result['images']
         
     async def create_midjourney_task(self,
                                      prompt: str) -> MidjourneyTask:
```

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI/exceptions/types.py` & `VisionCraftAPI-1.0.6/VisionCraftAPI/exceptions/types.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI/http_client.py` & `VisionCraftAPI-1.0.6/VisionCraftAPI/http_client.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI/models/whisper.py` & `VisionCraftAPI-1.0.6/VisionCraftAPI/models/whisper.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI/utils/checker.py` & `VisionCraftAPI-1.0.6/VisionCraftAPI/utils/checker.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/PKG-INFO` & `VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.5/VisionCraftAPI.egg-info/SOURCES.txt` & `VisionCraftAPI-1.0.6/VisionCraftAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.5/setup.py` & `VisionCraftAPI-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.5'
+version = '1.0.6'
 
 with open('README.md', 'r') as f:
       long_description = f.read()
 
 setup(name='VisionCraftAPI',
       version=version,
```

