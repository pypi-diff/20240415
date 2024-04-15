# Comparing `tmp/miservice_fork-2.4.2.tar.gz` & `tmp/miservice_fork-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.4.2.tar", last modified: Fri Apr 12 15:29:28 2024, max compression
+gzip compressed data, was "miservice_fork-2.4.3.tar", last modified: Mon Apr 15 03:45:06 2024, max compression
```

## Comparing `miservice_fork-2.4.2.tar` & `miservice_fork-2.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.152382 miservice_fork-2.4.2/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.2/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-12 15:29:28.151923 miservice_fork-2.4.2/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     4541 2024-04-03 05:25:43.000000 miservice_fork-2.4.2/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.2/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.146475 miservice_fork-2.4.2/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.2/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.2/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     7927 2024-04-03 05:25:43.000000 miservice_fork-2.4.2/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.2/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.2/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.2/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     4251 2024-04-12 15:28:29.000000 miservice_fork-2.4.2/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.150599 miservice_fork-2.4.2/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       21 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-12 15:29:28.152442 miservice_fork-2.4.2/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-04-12 15:28:11.000000 miservice_fork-2.4.2/setup.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     1067 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/LICENSE
+-rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     4587 2024-04-15 03:44:37.000000 miservice_fork-2.4.3/README.md
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)       96 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/micli.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.055708 miservice_fork-2.4.3/miservice/
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)      178 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/__init__.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       95 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/__main__.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     7911 2024-04-15 03:44:37.000000 miservice_fork-2.4.3/miservice/cli.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)     5647 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miaccount.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)     3818 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miiocommand.py
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)    10620 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miioservice.py
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)     4251 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/minaservice.py
+drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/miservice_fork.egg-info/
+-rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/PKG-INFO
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)      424 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/SOURCES.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)        1 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/dependency_links.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       46 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/entry_points.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       21 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/requires.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       10 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/top_level.txt
+-rw-rw-r--   0 yihong    (1000) yihong    (1000)       38 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/setup.cfg
+-rwxrwxr-x   0 yihong    (1000) yihong    (1000)      919 2024-04-15 03:44:53.000000 miservice_fork-2.4.3/setup.py
```

### Comparing `miservice_fork-2.4.2/LICENSE` & `miservice_fork-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.2/PKG-INFO` & `miservice_fork-2.4.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.2
+Version: 2.4.3
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.2/README.md` & `miservice_fork-2.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
 ## -> 播放 suno.ai trending random
 
 ```
 micli suno_random
 ```
 
+## -> 查看硬件信息
+
+```
+micli mina
+```
+
 ## Install
 ```
 pip3 install -U miservice_fork
 or 
 pip3 install .
 ```
```

### Comparing `miservice_fork-2.4.2/miservice/cli.py` & `miservice_fork-2.4.3/miservice/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,18 @@
                 session,
                 env.get("MI_USER"),
                 env.get("MI_PASS"),
                 os.path.join(str(Path.home()), ".mi.token"),
             )
             result = ""
             mina_service = MiNAService(account)
-            if args.startswith("mina"):
-                if len(args) > 4:
-                    await mina_service.send_message(result, -1, args[4:])
             # TODO refactor this shit
-            elif args.split(" ")[0].strip() in [
+            if args.split(" ")[0].strip() in [
                 "play",
+                "mina",
                 "pause",
                 "loop",
                 "play_list",
                 "suno",
                 "suno_random",
             ]:
                 arg = args.split(" ")[0].strip()
@@ -124,14 +122,16 @@
                 device_id = find_device_id(result, env.get("MI_DID", ""))
                 # tricky add it to global
                 device_id_list.append(device_id)
                 args_list = args.split(" ")
                 if len(args_list) == 1:
                     if args_list[0] == "pause":
                         await mina_service.player_pause(device_id)
+                    elif args_list[0] == "mina" and len(result) > 0:
+                        print(result[0])
                     elif "suno" in args_list[0]:
                         song_dict = await get_suno_playlist()
                         print(song_dict)
                         song_urls = list(song_dict.keys())
                         if args_list[0] == "suno_random":
                             random.shuffle(song_urls)
                             print("Will play suno trending list randomly")
```

### Comparing `miservice_fork-2.4.2/miservice/miaccount.py` & `miservice_fork-2.4.3/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.2/miservice/miiocommand.py` & `miservice_fork-2.4.3/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.2/miservice/miioservice.py` & `miservice_fork-2.4.3/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.2/miservice/minaservice.py` & `miservice_fork-2.4.3/miservice/minaservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.2/miservice_fork.egg-info/PKG-INFO` & `miservice_fork-2.4.3/miservice_fork.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.2
+Version: 2.4.3
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.2/setup.py` & `miservice_fork-2.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.4.2",
+    version="2.4.3",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

