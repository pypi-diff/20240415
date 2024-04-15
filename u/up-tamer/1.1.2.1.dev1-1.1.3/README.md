# Comparing `tmp/up_tamer-1.1.2.1.dev1.tar.gz` & `tmp/up_tamer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_tamer-1.1.2.1.dev1.tar", last modified: Mon Apr 15 08:13:22 2024, max compression
+gzip compressed data, was "up_tamer-1.1.3.tar", last modified: Mon Apr 15 08:15:52 2024, max compression
```

## Comparing `up_tamer-1.1.2.1.dev1.tar` & `up_tamer-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.210898 up_tamer-1.1.2.1.dev1/up_tamer/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30614 2024-04-15 08:13:19.000000 up_tamer-1.1.2.1.dev1/up_tamer/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:13:22.214898 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 08:13:22.000000 up_tamer-1.1.2.1.dev1/up_tamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:52.734990 up_tamer-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 08:15:48.000000 up_tamer-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 08:15:52.730990 up_tamer-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-15 08:15:48.000000 up_tamer-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:15:52.734990 up_tamer-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:15:48.000000 up_tamer-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:52.730990 up_tamer-1.1.3/up_tamer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:15:48.000000 up_tamer-1.1.3/up_tamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-15 08:15:48.000000 up_tamer-1.1.3/up_tamer/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30614 2024-04-15 08:15:48.000000 up_tamer-1.1.3/up_tamer/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:15:52.730990 up_tamer-1.1.3/up_tamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 08:15:52.000000 up_tamer-1.1.3/up_tamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 08:15:52.000000 up_tamer-1.1.3/up_tamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:15:52.000000 up_tamer-1.1.3/up_tamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 08:15:52.000000 up_tamer-1.1.3/up_tamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 08:15:52.000000 up_tamer-1.1.3/up_tamer.egg-info/top_level.txt
```

### Comparing `up_tamer-1.1.2.1.dev1/LICENSE` & `up_tamer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2.1.dev1/README.md` & `up_tamer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2.1.dev1/setup.py` & `up_tamer-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2.1.dev1/up_tamer/__init__.py` & `up_tamer-1.1.3/up_tamer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import subprocess
 import re
 
 
-VERSION = (1, 1, 2)
+VERSION = (1, 1, 3)
 __version__ = ".".join(str(x) for x in VERSION)
 
 try:
     git_version = subprocess.check_output(["git", "describe", "--tags",
                                            "--dirty=-wip"],
                                           stderr=subprocess.STDOUT)
     output = git_version.strip().decode('ascii')
```

### Comparing `up_tamer-1.1.2.1.dev1/up_tamer/converter.py` & `up_tamer-1.1.3/up_tamer/converter.py`

 * *Files identical despite different names*

### Comparing `up_tamer-1.1.2.1.dev1/up_tamer/engine.py` & `up_tamer-1.1.3/up_tamer/engine.py`

 * *Files identical despite different names*

