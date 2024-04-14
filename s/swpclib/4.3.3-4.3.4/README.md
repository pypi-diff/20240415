# Comparing `tmp/swpclib-4.3.3.tar.gz` & `tmp/swpclib-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.3.3.tar", last modified: Sun Apr 14 21:38:16 2024, max compression
+gzip compressed data, was "swpclib-4.3.4.tar", last modified: Sun Apr 14 23:35:56 2024, max compression
```

## Comparing `swpclib-4.3.3.tar` & `swpclib-4.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:16.318054 swpclib-4.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 21:38:05.000000 swpclib-4.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 21:38:05.000000 swpclib-4.3.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 21:38:05.000000 swpclib-4.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:38:05.000000 swpclib-4.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:38:16.318054 swpclib-4.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 21:38:05.000000 swpclib-4.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:16.314054 swpclib-4.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 21:38:05.000000 swpclib-4.3.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 21:38:05.000000 swpclib-4.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 21:38:16.318054 swpclib-4.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 21:38:05.000000 swpclib-4.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:16.314054 swpclib-4.3.3/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 21:38:05.000000 swpclib-4.3.3/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 21:38:05.000000 swpclib-4.3.3/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 21:38:05.000000 swpclib-4.3.3/swpclib/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-14 21:38:05.000000 swpclib-4.3.3/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 21:38:05.000000 swpclib-4.3.3/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:16.318054 swpclib-4.3.3/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:38:16.000000 swpclib-4.3.3/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:16.318054 swpclib-4.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 21:38:05.000000 swpclib-4.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 21:38:05.000000 swpclib-4.3.3/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 23:35:41.000000 swpclib-4.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 23:35:41.000000 swpclib-4.3.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 23:35:41.000000 swpclib-4.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 23:35:41.000000 swpclib-4.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:35:56.554696 swpclib-4.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 23:35:41.000000 swpclib-4.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 23:35:41.000000 swpclib-4.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 23:35:56.558696 swpclib-4.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 23:35:41.000000 swpclib-4.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 23:35:41.000000 swpclib-4.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 23:35:41.000000 swpclib-4.3.4/tests/test_swpclib.py
```

### Comparing `swpclib-4.3.3/CONTRIBUTING.rst` & `swpclib-4.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/LICENSE` & `swpclib-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/docs/Makefile` & `swpclib-4.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/docs/conf.py` & `swpclib-4.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/docs/installation.rst` & `swpclib-4.3.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/docs/make.bat` & `swpclib-4.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/setup.cfg` & `swpclib-4.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.3.1
+current_version = 4.3.4
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `swpclib-4.3.3/setup.py` & `swpclib-4.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 if __name__ == "__main__":
     setup(
         setup_requires=["setuptools-git-versioning"],
         test_suite="test",
         long_description=long_description,
         long_description_content_type="text/markdown",
         tests_require=test_requirements,
-        install_requires=["aiohttp>=3.8.1", "pillow>=10.3.0"],
+        install_requires=["aiohttp>=3.8.1", "pillow>=10.3.0", "click>=8.1.7"],
         name="swpclib",
     )
```

### Comparing `swpclib-4.3.3/swpclib/alerts.py` & `swpclib-4.3.4/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/swpclib/animate.py` & `swpclib-4.3.4/swpclib/animate.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/swpclib/cli.py` & `swpclib-4.3.4/swpclib/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Console script for swpclib."""
-import argparse
+import click
 import sys
 from . import swpclib
 import asyncio
 
 class bcolors:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
@@ -22,14 +22,15 @@
 '''
 urls = {
     'solar_images': [
         ('/products/animations/suvi-primary-094.json', 'goes_094'),
         ('/products/animations/suvi-primary-195.json', 'goes_195'),
         ('/products/animations/suvi-primary-304.json', 'goes_304'),
         ('/products/animations/suvi-primary-map.json', 'suvi-map'),
+        ('/products/animations/sdo-hmii.json', 'sdo-hmii')
     ],
     'graphs': [
         ('/products/animations/d-rap_f15_global.json', 'd-rap_f15'),
         ('/products/animations/wam-ipe/wfs_ionosphere_new.json', 'global_ionosphere')
     ],
     'cme': [
         ('/products/animations/lasco-c2.json', 'lasco-c2'),
@@ -45,33 +46,34 @@
     ],
 }
 
 async def get_animations(urls):
     swpc = swpclib.Runner()
     await asyncio.gather(*[swpc.gen_gif(endpoint=url[0], name=url[1], write=True) for url in urls], return_exceptions=False)
 
-def animations():
-    if len(sys.argv) > 1 and sys.argv[1] in urls.keys():
+@click.command()
+@click.option('--group', help="Group of images to generate")
+@click.option('--product', help="A swpc product endpoint that is a list of animation frames")
+@click.option('--name', help="Name used for filename creation")
+def animations(group=None, product=None, name=None):
+    if group and group in urls.keys():
         group = sys.argv[1]
         url_group = urls.get(group, [])
         print(f"Generating {len(url_group)} animations for group: {group}")
         asyncio.run(get_animations(url_group))
-    else:
-        if group:
+    elif group:
             print(f"{group} is not a valid group. valid groups are: {[group for group in urls.keys()]}")
-        else:
-            print(f"Must provide a valid group. valid groups are: {[group for group in urls.keys()]}")
+    elif product and name:
+        print(f"Generating animation for: {name}")
+        asyncio.run(get_animations([(product, name)]))
 
 
+@click.command()
 def space_weather():
     """Console script for swpclib."""
-    parser = argparse.ArgumentParser()
-    parser.add_argument("_", nargs="*")
-    args = parser.parse_args()
-
     runner = swpclib.Runner()
     data = asyncio.run(runner.get_standard())
     string = f"""\n{bcolors.OKBLUE}Current Space Weather:{bcolors.ENDC}
 
 \tSFI: {data.get('sfi_data', {}).get('sfi')}
 \tKP Index: {data.get('kp_index_data', {}).get('kp_index')}
 \tA Index: {data['a_index_data']['a_index']}
```

### Comparing `swpclib-4.3.3/swpclib/swpclib.py` & `swpclib-4.3.4/swpclib/swpclib.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/swpclib.egg-info/SOURCES.txt` & `swpclib-4.3.4/swpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.3/tests/test_swpclib.py` & `swpclib-4.3.4/tests/test_swpclib.py`

 * *Files identical despite different names*

