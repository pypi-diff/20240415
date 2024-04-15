# Comparing `tmp/gw-chirpy-0.0.1.tar.gz` & `tmp/gw_chirpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gw-chirpy-0.0.1.tar", last modified: Wed Oct 16 16:10:53 2019, max compression
+gzip compressed data, was "gw_chirpy-0.0.2.tar", last modified: Mon Apr 15 20:09:30 2024, max compression
```

## Comparing `gw-chirpy-0.0.1.tar` & `gw_chirpy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-x---   0 sebastian.khan (100003003) sebastian.khan (100003003)        0 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)      270 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/PKG-INFO
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)      268 2019-10-16 13:43:46.000000 gw-chirpy-0.0.1/README.md
-drwxr-x---   0 sebastian.khan (100003003) sebastian.khan (100003003)        0 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/chirpy/
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)       16 2019-10-16 16:08:42.000000 gw-chirpy-0.0.1/chirpy/__init__.py
-drwxr-x---   0 sebastian.khan (100003003) sebastian.khan (100003003)        0 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)      270 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/PKG-INFO
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)      201 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/SOURCES.txt
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)        1 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/dependency_links.txt
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)       75 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/requires.txt
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)        7 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/gw_chirpy.egg-info/top_level.txt
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)       38 2019-10-16 16:10:52.000000 gw-chirpy-0.0.1/setup.cfg
--rw-r-----   0 sebastian.khan (100003003) sebastian.khan (100003003)      818 2019-10-16 16:10:37.000000 gw-chirpy-0.0.1/setup.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.123426 gw_chirpy-0.0.2/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    35073 2024-04-15 07:03:02.000000 gw_chirpy-0.0.2/LICENSE
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      505 2024-04-15 20:09:30.123254 gw_chirpy-0.0.2/PKG-INFO
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      349 2024-04-15 19:58:31.000000 gw_chirpy-0.0.2/README.md
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.121762 gw_chirpy-0.0.2/chirpy/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)       16 2024-04-15 07:03:02.000000 gw_chirpy-0.0.2/chirpy/__init__.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.122344 gw_chirpy-0.0.2/chirpy/prob_phenom_model/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 07:21:19.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/__init__.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)     7416 2024-04-15 07:04:59.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/collocation.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)     4992 2024-04-15 07:04:59.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/pn.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    28364 2024-04-15 07:50:02.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/ppm_utils.py
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)    10742 2024-04-15 07:24:15.000000 gw_chirpy-0.0.2/chirpy/prob_phenom_model/workflow_utils.py
+drwxr-xr-x   0 sebastian.khan   (501) staff       (20)        0 2024-04-15 20:09:30.123068 gw_chirpy-0.0.2/gw_chirpy.egg-info/
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      505 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      398 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        1 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      104 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/requires.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)        7 2024-04-15 20:09:30.000000 gw_chirpy-0.0.2/gw_chirpy.egg-info/top_level.txt
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)       38 2024-04-15 20:09:30.123461 gw_chirpy-0.0.2/setup.cfg
+-rw-r--r--   0 sebastian.khan   (501) staff       (20)      818 2024-04-15 20:09:27.000000 gw_chirpy-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gw-chirpy-0.0.1/setup.py` & `gw_chirpy-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requirementPath = thelibFolder + '/requirements.txt'
 install_requires = [] # Examples: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 setup(name='gw-chirpy',
-      version='0.0.1',
+      version='0.0.2',
       description='Gravitational Waveforms in python',
       author='Sebastian Khan',
       author_email='sebastian.khan@LIGO.org',
       packages=find_packages(),
       install_requires=install_requires,
       url='https://gitlab.com/SpaceTimeKhantinuum/chirpy'
      )
```

