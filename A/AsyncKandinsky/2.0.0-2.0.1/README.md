# Comparing `tmp/AsyncKandinsky-2.0.0.tar.gz` & `tmp/AsyncKandinsky-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-2.0.0.tar", last modified: Mon Apr  8 15:50:54 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-2.0.1.tar", last modified: Mon Apr 15 19:05:00 2024, max compression
```

## Comparing `AsyncKandinsky-2.0.0.tar` & `AsyncKandinsky-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-08 15:50:54.703098 AsyncKandinsky-2.0.0/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-08 15:50:54.698276 AsyncKandinsky-2.0.0/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)     2559 2024-04-08 15:36:52.000000 AsyncKandinsky-2.0.0/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)     2804 2024-04-08 15:30:56.000000 AsyncKandinsky-2.0.0/AsyncKandinsky/DefaultParams.py
--rw-r--r--   0 s1rne      (503) staff       (20)      934 2024-04-08 15:36:52.000000 AsyncKandinsky-2.0.0/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-2.0.0/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     6474 2024-04-08 15:39:35.000000 AsyncKandinsky-2.0.0/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-08 15:50:54.702160 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     3564 2024-04-08 15:50:54.000000 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      349 2024-04-08 15:50:54.000000 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-08 15:50:54.000000 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-08 15:50:54.000000 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-08 15:50:54.000000 AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     3564 2024-04-08 15:50:54.702883 AsyncKandinsky-2.0.0/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     2926 2024-04-08 15:50:29.000000 AsyncKandinsky-2.0.0/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-08 15:50:54.703810 AsyncKandinsky-2.0.0/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      922 2024-04-08 15:44:50.000000 AsyncKandinsky-2.0.0/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.011260 AsyncKandinsky-2.0.1/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.006633 AsyncKandinsky-2.0.1/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2559 2024-04-08 15:36:52.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     2804 2024-04-08 15:30:56.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/DefaultParams.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      944 2024-04-15 18:59:15.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     6470 2024-04-15 19:00:24.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.010218 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     3521 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      349 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     3521 2024-04-15 19:05:00.011040 AsyncKandinsky-2.0.1/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     2883 2024-04-08 15:55:29.000000 AsyncKandinsky-2.0.1/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-15 19:05:00.011964 AsyncKandinsky-2.0.1/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      922 2024-04-15 19:02:40.000000 AsyncKandinsky-2.0.1/setup.py
```

### Comparing `AsyncKandinsky-2.0.0/AsyncKandinsky/API_types.py` & `AsyncKandinsky-2.0.1/AsyncKandinsky/API_types.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-2.0.0/AsyncKandinsky/DefaultParams.py` & `AsyncKandinsky-2.0.1/AsyncKandinsky/DefaultParams.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-2.0.0/AsyncKandinsky/URLS.py` & `AsyncKandinsky-2.0.1/AsyncKandinsky/URLS.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
     url_text2image_run = f"{url_web}text2image/run"
     url_text2image_status = f"{url_web}text2image/status/$uuid"
 
     url_text2animation_run = f"{url_web}animation/run?model_id=2"
     url_text2animation_status = f"{url_web}animation/status/$uuid"
 
-    url_text2video_run = f"{url_web}video/run?model_id=2"
-    url_text2video_status = f"{url_web}video/status/$uuid"
+    url_text2video_run = f"{url_web}text2video/run?model_id=3"
+    url_text2video_status = f"{url_web}text2video/status/$uuid"
```

### Comparing `AsyncKandinsky-2.0.0/AsyncKandinsky/api.py` & `AsyncKandinsky-2.0.1/AsyncKandinsky/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         data.add_field("params",
                        json.dumps(params),
                        content_type="application/json",
                        )
         data.add_field("model_id", "3")
 
         async with aiohttp.ClientSession() as session:
-            n_url = self.api.urls.url_text2animation_run
+            n_url = self.api.urls.url_text2video_run
             async with session.post(n_url, data=data, headers=await self.api.get_headers()) as resp:
                 result = await resp.json()
 
         if "error" in result:
             return {"error": True, "data": result}
 
         uuid = result["uuid"]
```

### Comparing `AsyncKandinsky-2.0.0/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 2.0.0
+Version: 2.0.1
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
  + api_key и secret_key:
    + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
    + не самое лучше качество генерации
  + почта и пароль - данные от уже созданного аккаунта:
    + **!!! Обязательно нужен уже зарегистрированный аккаунт**
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
    + лучшее качество генерации
 
 ```
 model = FusionBrainApi(ApiApi("Сюда свой api_key", "Сюда свой secret_key"))
 # Любой способ на выбор
 model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 ```
```

### Comparing `AsyncKandinsky-2.0.0/PKG-INFO` & `AsyncKandinsky-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 2.0.0
+Version: 2.0.1
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,15 @@
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
  + api_key и secret_key:
    + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
    + не самое лучше качество генерации
  + почта и пароль - данные от уже созданного аккаунта:
    + **!!! Обязательно нужен уже зарегистрированный аккаунт**
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
    + лучшее качество генерации
 
 ```
 model = FusionBrainApi(ApiApi("Сюда свой api_key", "Сюда свой secret_key"))
 # Любой способ на выбор
 model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 ```
```

### Comparing `AsyncKandinsky-2.0.0/README.md` & `AsyncKandinsky-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
  + api_key и secret_key:
    + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
    + не самое лучше качество генерации
  + почта и пароль - данные от уже созданного аккаунта:
    + **!!! Обязательно нужен уже зарегистрированный аккаунт**
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
    + лучшее качество генерации
 
 ```
 model = FusionBrainApi(ApiApi("Сюда свой api_key", "Сюда свой secret_key"))
 # Любой способ на выбор
 model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 ```
```

### Comparing `AsyncKandinsky-2.0.0/setup.py` & `AsyncKandinsky-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='2.0.0',
+    version='2.0.1',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

