# Comparing `tmp/swpclib-4.3.4.tar.gz` & `tmp/swpclib-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.3.4.tar", last modified: Sun Apr 14 23:35:56 2024, max compression
+gzip compressed data, was "swpclib-4.3.5.tar", last modified: Sun Apr 14 23:40:04 2024, max compression
```

## Comparing `swpclib-4.3.4.tar` & `swpclib-4.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 23:35:41.000000 swpclib-4.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 23:35:41.000000 swpclib-4.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 23:35:41.000000 swpclib-4.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 23:35:41.000000 swpclib-4.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:35:56.554696 swpclib-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 23:35:41.000000 swpclib-4.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 23:35:41.000000 swpclib-4.3.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 23:35:41.000000 swpclib-4.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 23:35:56.558696 swpclib-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 23:35:41.000000 swpclib-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 23:35:41.000000 swpclib-4.3.4/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 23:35:56.000000 swpclib-4.3.4/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:35:56.554696 swpclib-4.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 23:35:41.000000 swpclib-4.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 23:35:41.000000 swpclib-4.3.4/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:40:04.461917 swpclib-4.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 23:39:53.000000 swpclib-4.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 23:39:53.000000 swpclib-4.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 23:39:53.000000 swpclib-4.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 23:39:53.000000 swpclib-4.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:40:04.461917 swpclib-4.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 23:39:53.000000 swpclib-4.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:40:04.457917 swpclib-4.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 23:39:53.000000 swpclib-4.3.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 23:39:53.000000 swpclib-4.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 23:40:04.461917 swpclib-4.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 23:39:53.000000 swpclib-4.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:40:04.457917 swpclib-4.3.5/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 23:39:53.000000 swpclib-4.3.5/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 23:39:53.000000 swpclib-4.3.5/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 23:39:53.000000 swpclib-4.3.5/swpclib/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-14 23:39:53.000000 swpclib-4.3.5/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 23:39:53.000000 swpclib-4.3.5/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:40:04.461917 swpclib-4.3.5/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 23:40:04.000000 swpclib-4.3.5/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:40:04.461917 swpclib-4.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 23:39:53.000000 swpclib-4.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 23:39:53.000000 swpclib-4.3.5/tests/test_swpclib.py
```

### Comparing `swpclib-4.3.4/CONTRIBUTING.rst` & `swpclib-4.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/LICENSE` & `swpclib-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/docs/Makefile` & `swpclib-4.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/docs/conf.py` & `swpclib-4.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/docs/installation.rst` & `swpclib-4.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/docs/make.bat` & `swpclib-4.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/setup.cfg` & `swpclib-4.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.3.4
+current_version = 4.3.5
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `swpclib-4.3.4/setup.py` & `swpclib-4.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/swpclib/alerts.py` & `swpclib-4.3.5/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/swpclib/animate.py` & `swpclib-4.3.5/swpclib/animate.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/swpclib/cli.py` & `swpclib-4.3.5/swpclib/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 @click.command()
 @click.option('--group', help="Group of images to generate")
 @click.option('--product', help="A swpc product endpoint that is a list of animation frames")
 @click.option('--name', help="Name used for filename creation")
 def animations(group=None, product=None, name=None):
     if group and group in urls.keys():
-        group = sys.argv[1]
         url_group = urls.get(group, [])
         print(f"Generating {len(url_group)} animations for group: {group}")
         asyncio.run(get_animations(url_group))
     elif group:
             print(f"{group} is not a valid group. valid groups are: {[group for group in urls.keys()]}")
     elif product and name:
         print(f"Generating animation for: {name}")
```

### Comparing `swpclib-4.3.4/swpclib/swpclib.py` & `swpclib-4.3.5/swpclib/swpclib.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/swpclib.egg-info/SOURCES.txt` & `swpclib-4.3.5/swpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.4/tests/test_swpclib.py` & `swpclib-4.3.5/tests/test_swpclib.py`

 * *Files identical despite different names*

