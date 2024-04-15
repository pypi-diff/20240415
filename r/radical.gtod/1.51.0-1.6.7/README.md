# Comparing `tmp/radical_gtod-1.51.0.tar.gz` & `tmp/radical.gtod-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_gtod-1.51.0.tar", last modified: Mon Apr 15 08:34:19 2024, max compression
+gzip compressed data, was "dist/radical.gtod-1.6.7.tar", last modified: Fri Jul  9 08:02:35 2021, max compression
```

## Comparing `radical_gtod-1.51.0.tar` & `radical.gtod-1.6.7.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3103 2024-04-15 08:33:25.000000 radical_gtod-1.51.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8361 2022-12-16 11:50:15.000000 radical_gtod-1.51.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      213 2022-12-16 13:11:13.000000 radical_gtod-1.51.0/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1265 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      640 2021-09-24 08:24:02.000000 radical_gtod-1.51.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 08:33:15.000000 radical_gtod-1.51.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      140 2021-09-24 08:24:02.000000 radical_gtod-1.51.0/bin/radical-gtod-version
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/examples/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      268 2021-09-24 08:24:02.000000 radical_gtod-1.51.0/examples/00_gtod.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       58 2022-12-16 11:50:15.000000 radical_gtod-1.51.0/requirements-docs.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       71 2022-12-16 11:50:15.000000 radical_gtod-1.51.0/requirements-tests.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       16 2022-12-16 13:11:46.000000 radical_gtod-1.51.0/requirements.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    12362 2024-04-15 08:33:15.000000 radical_gtod-1.51.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/src/radical/gtod/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       27 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical/gtod/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical/gtod/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      532 2021-09-24 08:24:02.000000 radical_gtod-1.51.0/src/radical/gtod/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      196 2021-09-24 08:24:02.000000 radical_gtod-1.51.0/src/radical/gtod/gtod.c
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    16096 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical/gtod/radical-gtod
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 08:34:19.978174 radical_gtod-1.51.0/src/radical.gtod.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     1265 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      546 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       14 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 08:34:19.000000 radical_gtod-1.51.0/src/radical.gtod.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1104 2021-07-09 07:58:07.000000 radical.gtod-1.6.7/CHANGES.md
+-rw-r--r--   0 merzky    (1001) merzky    (1001)     8365 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/LICENSE.md
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       79 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/MANIFEST.in
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1029 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/PKG-INFO
+-rw-r--r--   0 merzky    (1001) merzky    (1001)      640 2020-07-21 20:17:36.000000 radical.gtod-1.6.7/README.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-07-09 07:57:01.000000 radical.gtod-1.6.7/VERSION
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/bin/
+-rwxr-xr-x   0 merzky    (1001) merzky    (1001)      140 2020-07-21 20:29:35.000000 radical.gtod-1.6.7/bin/radical-gtod-version
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       67 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/setup.cfg
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11093 2021-07-09 08:02:01.000000 radical.gtod-1.6.7/setup.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical/gtod/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       40 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/SDIST
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      532 2020-10-07 18:41:21.000000 radical.gtod-1.6.7/src/radical/gtod/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      196 2020-08-04 23:56:19.000000 radical.gtod-1.6.7/src/radical/gtod/gtod.c
+-rw-r--r--   0 merzky    (1001) merzky    (1001)      422 2020-07-21 20:11:05.000000 radical.gtod-1.6.7/src/radical/gtod/gtod_module.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8448 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical/gtod/radical-gtod
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-09 08:02:35.629757 radical.gtod-1.6.7/src/radical.gtod.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1029 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      506 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-09 08:02:35.000000 radical.gtod-1.6.7/src/radical.gtod.egg-info/top_level.txt
```

### Comparing `radical_gtod-1.51.0/LICENSE.md` & `radical.gtod-1.6.7/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 ================================================================================
       The GNU Lesser General Public License, version 3.0 (LGPL-3.0)
                             [OSI Approved License]
 ================================================================================
 
-This license is a set of additional permissions added to version 3 of the GNU
+This license is a set of additional permissions added to version 3 of the GNU 
 General Public License.
 
 
 GNU LESSER GENERAL PUBLIC LICENSE
 =================================
 
 Version 3, 29 June 2007
@@ -65,18 +65,18 @@
 -------------------------------
 
 If you modify a copy of the Library, and, in your modifications, a facility
 refers to a function or data to be supplied by an Application that uses the
 facility (other than as an argument passed when the facility is invoked), then
 you may convey a copy of the modified version:
 
-  a) under this License, provided that you make a good faith effort to ensure
+  a) under this License, provided that you make a good faith effort to ensure 
      that, in the event an Application does not supply the function or data, the
      facility still operates, and performs whatever part of its purpose remains
-     meaningful, or
+     meaningful, or 
 
   b) under the GNU GPL, with none of the additional permissions of this License
      applicable to that copy.
 
 
 3. Object Code Incorporating Material from Library Header Files.
 ----------------------------------------------------------------
@@ -146,15 +146,15 @@
 Applications and are not covered by this License, and convey such a combined
 library under terms of your choice, if you do both of the following:
 
   a) Accompany the combined library with a copy of the same work based on the
      Library, uncombined with any other library facilities, conveyed under the
      terms of this License.  
      
-  b) Give prominent notice with the combined library that part of it is a work
+  b) Give prominent notice with the combined library that part of it is a work 
      based on the Library, and explaining where to find the accompanying
      uncombined form of the same work.
 
 
 6. Revised Versions of the GNU Lesser General Public License.
 -------------------------------------------------------------
```

### Comparing `radical_gtod-1.51.0/PKG-INFO` & `radical.gtod-1.6.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: radical.gtod
-Version: 1.51.0
+Version: 1.6.7
 Summary: returns seconds since epoch in subsecond resolution.
-Home-page: http://radical-cybertools.github.io/radical.gtod/
+Home-page: https://www.github.com/radical-cybertools/radical.gtod/
 Author: RADICAL Team
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: GPL3
-Project-URL: Documentation, https://radicalgtod.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/radical-cybertools/radical.gtod/
-Project-URL: Issues, https://github.com/radical-cybertools/radical.gtod/issues
+Description: UNKNOWN
 Keywords: radical distributed computing
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
-License-File: LICENSE.md
-Requires-Dist: radical.utils
```

### Comparing `radical_gtod-1.51.0/README.md` & `radical.gtod-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `radical_gtod-1.51.0/setup.py` & `radical.gtod-1.6.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,53 @@
 #!/usr/bin/env python3
 
-__author__    = 'RADICAL-Cybertools Team'
-__email__     = 'info@radical-cybertools.org'
-__copyright__ = 'Copyright 2013-23, The RADICAL-Cybertools Team'
-__license__   = 'MIT'
+__author__    = 'RADICAL Team'
+__email__     = 'radical@radical-project.org'
+__copyright__ = 'Copyright date 2020, RADICAL Team'
+__license__   = 'GPL.v3'
 
 
 ''' Setup script, only usable via pip. '''
 
 import re
 import os
 import sys
-import glob
 import time
 import traceback
 import shutil
 
 import subprocess as sp
 
-from setuptools import setup, Command, find_namespace_packages
 
+from setuptools import setup, Command, find_namespace_packages
 
-# ------------------------------------------------------------------------------
-base     = 'gtod'
-name     = 'radical.%s'      % base
-mod_root = 'src/radical/%s/' % base
 
 # ------------------------------------------------------------------------------
-#
-# pip warning:
-# "In-tree builds are now default. pip 22.1 will enforce this behaviour change.
-#  A possible replacement is to remove the --use-feature=in-tree-build flag."
-#
-# With this change we need to make sure to clean out all temporary files from
-# the src tree. Specifically create (and thus need to clean)
-#   - VERSION
-#   - SDIST
-#   - the sdist file itself (a tarball)
-#
-# `pip install` (or any other direct or indirect invocation of `setup.py`) will
-# in fact run `setup.py` multiple times: one on the top level, and internally
-# again with other arguments to build sdist and bwheel packages.  We must *not*
-# clean out temporary files in those internal runs as that would invalidate the
-# install.
-#
-# We thus introduce an env variable `SDIST_LEVEL` which allows us to separate
-# internal calls from the top level invocation - we only clean on the latter
-# (see end of this file).
-sdist_level = int(os.environ.get('SDIST_LEVEL', 0))
-os.environ['SDIST_LEVEL'] = str(sdist_level + 1)
-
-root = os.path.dirname(__file__) or '.'
+name     = 'radical.gtod'
+mod_root = 'src/radical/gtod/'
 
 
 # ------------------------------------------------------------------------------
 #
 def sh_callout(cmd):
 
     p = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.PIPE, shell=True)
 
-    stdout, stderr = p.communicate()
-    ret            = p.returncode
-    return stdout, stderr, ret
+    out, err = p.communicate()
+    ret      = p.returncode
+    return out, err, ret
 
 
 # ------------------------------------------------------------------------------
 #
 # versioning mechanism:
 #
 #   - version:          1.2.3            - is used for installation
 #   - version_detail:  v1.2.3-9-g0684b06 - is used for debugging
-#   - version is read from VERSION file in root, which then is copied to
+#   - version is read from VERSION file in src_root, which then is copied to
 #     module dir, and is getting installed from there.
 #   - version_detail is derived from the git tag, and only available when
 #     installed from git.  That is stored in mod_root/VERSION in the install
 #     tree.
 #   - The VERSION file is used to provide the runtime version information.
 #
 def get_version(_mod_root):
@@ -87,30 +60,34 @@
     try:
 
         _version_base   = None
         _version_detail = None
         _sdist_name     = None
 
         # get version from './VERSION'
-        with open('%s/VERSION' % root, 'r', encoding='utf-8') as fin:
-            _version_base = fin.readline().strip()
+        src_root = os.path.dirname(__file__)
+        if not src_root:
+            src_root = '.'
+
+        with open(src_root + '/VERSION', 'r') as f:
+            _version_base = f.readline().strip()
 
         # attempt to get version detail information from git
         # We only do that though if we are in a repo root dir,
         # ie. if 'git rev-parse --show-prefix' returns an empty string --
         # otherwise we get confused if the ve lives beneath another repository,
         # and the pip version used uses an install tmp dir in the ve space
         # instead of /tmp (which seems to happen with some pip/setuptools
         # versions).
         out, _, ret = sh_callout(
             'cd %s ; '
             'test -z `git rev-parse --show-prefix` || exit -1; '
             'tag=`git describe --tags --always` 2>/dev/null ; '
             'branch=`git branch | grep -e "^*" | cut -f 2- -d " "` 2>/dev/null ; '
-            'echo $tag@$branch' % root)
+            'echo $tag@$branch' % src_root)
         _version_detail = out.strip()
         _version_detail = _version_detail.decode()
         _version_detail = _version_detail.replace('detached from ', 'detached-')
 
         # remove all non-alphanumeric (and then some) chars
         _version_detail = re.sub('[/ ]+', '-', _version_detail)
         _version_detail = re.sub('[^a-zA-Z0-9_+@.-]+', '', _version_detail)
@@ -124,62 +101,66 @@
             _version = _version_base
         elif '@' not in _version_base:
             _version = '%s-%s' % (_version_base, _version_detail)
         else:
             _version = _version_base
 
         # make sure the version files exist for the runtime version inspection
-        _path = '%s/%s' % (root, _mod_root)
-        with open(_path + '/VERSION', 'w', encoding='utf-8') as fout:
-            fout.write(_version_base + '\n')
-            fout.write(_version      + '\n')
-
-        _sdist_name = '%s-%s.tar.gz' % (name, _version_base)
-      # _sdist_name = _sdist_name.replace('/', '-')
-      # _sdist_name = _sdist_name.replace('@', '-')
-      # _sdist_name = _sdist_name.replace('#', '-')
-      # _sdist_name = _sdist_name.replace('_', '-')
-
-        # setuptools 69.5 does changes naming scheme
-        if not os.path.isfile('dist/%s' % _sdist_name):
-            _sdist_name = '%s-%s.tar.gz' % (name.replace('.', '_'), _version_base)
+        _path = '%s/%s' % (src_root, _mod_root)
+        with open(_path + '/VERSION', 'w') as f:
+            f.write(_version + '\n')
+
+        _sdist_name = '%s-%s.tar.gz' % (name, _version)
+        _sdist_name = _sdist_name.replace('/', '-')
+        _sdist_name = _sdist_name.replace('@', '-')
+        _sdist_name = _sdist_name.replace('#', '-')
+        _sdist_name = _sdist_name.replace('_', '-')
 
         if '--record'    in sys.argv or \
            'bdist_egg'   in sys.argv or \
            'bdist_wheel' in sys.argv    :
             # pip install stage 2 or easy_install stage 1
             #
             # pip install will untar the sdist in a tmp tree.  In that tmp
             # tree, we won't be able to derive git version tags -- so we pack
             # the formerly derived version as ./VERSION
-            shutil.move('VERSION', 'VERSION.bak')              # backup
-            shutil.copy('%s/VERSION' % _path, 'VERSION')       # version to use
-            os.system  ('python3 setup.py sdist')              # build sdist
+            shutil.move("VERSION", "VERSION.bak")              # backup
+            shutil.copy("%s/VERSION" % _path, "VERSION")       # version to use
+            os.system  ("python3 setup.py sdist")               # build sdist
             shutil.copy('dist/%s' % _sdist_name,
                         '%s/%s'   % (_mod_root, _sdist_name))  # copy into tree
             shutil.move('VERSION.bak', 'VERSION')              # restore version
 
-        with open(_path + '/SDIST', 'w', encoding='utf-8') as fout:
-            fout.write(_sdist_name + '\n')
+        with open(_path + '/SDIST', 'w') as f:
+            f.write(_sdist_name + '\n')
 
         return _version_base, _version_detail, _sdist_name, _path
 
     except Exception as e:
         raise RuntimeError('Could not extract/set version: %s' % e) from e
 
 
 # ------------------------------------------------------------------------------
+# check python version. we need >= 3.6
+if  sys.hexversion < 0x03060000:
+    raise RuntimeError('%s requires Python 3.6 or higher' % name)
+
+
+# ------------------------------------------------------------------------------
 # get version info -- this will create VERSION and srcroot/VERSION
 version, version_detail, sdist_name, path = get_version(mod_root)
 
 
 # ------------------------------------------------------------------------------
-# check python version, should be >= 3.6
-if sys.hexversion < 0x03060000:
-    raise RuntimeError('ERROR: %s requires Python 3.6 or newer' % name)
+#
+def read(fname):
+    try:
+        return open(fname).read()
+    except Exception:
+        return ''
 
 
 # ------------------------------------------------------------------------------
 #
 class RunTwine(Command):
     user_options = []
     def initialize_options(self): pass
@@ -236,40 +217,30 @@
 
 
 
 # ------------------------------------------------------------------------------
 #
 # This copies the contents like examples/ dir under sys.prefix/share/$name
 # It needs the MANIFEST.in entries to work.
+base = 'bin'
 df   = [('bin/', ['src/radical/gtod/radical-gtod'])]
 
 
 # ------------------------------------------------------------------------------
 #
-with open('%s/requirements.txt' % root, encoding='utf-8') as freq:
-    requirements = freq.readlines()
-
-
-# ------------------------------------------------------------------------------
-#
 setup_args = {
     'name'               : name,
-  # 'namespace_packages' : ['radical'],
+    'namespace_packages' : ['radical'],
     'version'            : version,
     'description'        : 'returns seconds since epoch in subsecond resolution.',
     'author'             : 'RADICAL Team',
     'author_email'       : 'radical@rutgers.edu',
     'maintainer'         : 'The RADICAL Group',
     'maintainer_email'   : 'radical@rutgers.edu',
-    'url'                : 'http://radical-cybertools.github.io/%s/' % name,
-    'project_urls'       : {
-        'Documentation': 'https://radical%s.readthedocs.io/en/latest/' % base,
-        'Source'       : 'https://github.com/radical-cybertools/%s/'   % name,
-        'Issues' : 'https://github.com/radical-cybertools/%s/issues'   % name,
-    },
+    'url'                : 'https://www.github.com/radical-cybertools/radical.gtod/',
     'license'            : 'GPL3',
     'keywords'           : 'radical distributed computing',
     'python_requires'    : '>=3.6',
     'classifiers'        : [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Environment :: Console',
@@ -289,40 +260,51 @@
     'scripts'            : [
                          #  'bin/radical-gtod',
                             'bin/radical-gtod-version',
                            ],
     'package_data'       : {'': ['*.txt', '*.sh', '*.json', '*.gz', '*.c',
                                  '*.md', 'VERSION', 'SDIST', sdist_name,
                                  'radical-gtod']},
-    'install_requires'   : requirements,
+  # 'setup_requires'     : ['pytest-runner'],
+    'install_requires'   : [],
+    'tests_require'      : ['pytest',
+                            'pylint',
+                            'flake8',
+                            'coverage',
+                            'mock==2.0.0.',
+                           ],
+    'test_suite'         : '%s.tests' % name,
     'zip_safe'           : False,
+  # 'build_sphinx'       : {
+  #     'source-dir'     : 'docs/',
+  #     'build-dir'      : 'docs/build',
+  #     'all_files'      : 1,
+  # },
+  # 'upload_sphinx'      : {
+  #     'upload-dir'     : 'docs/build/html',
+  # },
+    # This copies the contents of the examples/ dir under
+    # sys.prefix/share/$name
+    # It needs the MANIFEST.in entries to work.
     'data_files'         : df,
     'cmdclass'           : {'upload': RunTwine},
 }
 
 
 # ------------------------------------------------------------------------------
 #
 setup(**setup_args)
 
-
-# ------------------------------------------------------------------------------
-# clean temporary files from source tree
-if sdist_level == 0:
-    os.system('rm -vrf src/%s.egg-info' % name)
-    os.system('rm -vf  %s/%s'           % (path, sdist_name))
-    os.system('rm -vf  %s/VERSION'      % path)
-    os.system('rm -vf  %s/SDIST'        % path)
-    os.system('rm -vf  %s/gtod.o'       % path)
-    os.system('rm -vf  %s/radical-gtod' % path)
-
+os.system('rm -rf src/%s.egg-info' % name)
+# os.system('rm -rf %s/VERSION'      % path)
+# os.system('rm -rf %s/VERSION.git'  % path)
+# os.system('rm -rf %s/SDIST'        % path)
 
 # gtod is compiled, and pip tries to cache compiled modules in a wheel.
 # On resources, where $HOME is on a shared filesystem and serves multiple hosts
 # with different architectures, pip will pull the cached wheel for the wrong
 # architecture. The installation then succeeds, but the module is unusable and
 # leads to runtime errors which are hard to trace. Thus, remove cached wheel.
 os.system('pip cache remove %s' % name)
 
-
 # ------------------------------------------------------------------------------
```

### Comparing `radical_gtod-1.51.0/src/radical/gtod/__init__.py` & `radical.gtod-1.6.7/src/radical/gtod/__init__.py`

 * *Files identical despite different names*

### Comparing `radical_gtod-1.51.0/src/radical.gtod.egg-info/PKG-INFO` & `radical.gtod-1.6.7/src/radical.gtod.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: radical.gtod
-Version: 1.51.0
+Version: 1.6.7
 Summary: returns seconds since epoch in subsecond resolution.
-Home-page: http://radical-cybertools.github.io/radical.gtod/
+Home-page: https://www.github.com/radical-cybertools/radical.gtod/
 Author: RADICAL Team
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: GPL3
-Project-URL: Documentation, https://radicalgtod.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/radical-cybertools/radical.gtod/
-Project-URL: Issues, https://github.com/radical-cybertools/radical.gtod/issues
+Description: UNKNOWN
 Keywords: radical distributed computing
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
-License-File: LICENSE.md
-Requires-Dist: radical.utils
```

