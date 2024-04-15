# Comparing `tmp/radical.gtod-1.5.0.tar.gz` & `tmp/radical.gtod-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.gtod-1.5.0.tar", last modified: Tue Aug  4 23:59:25 2020, max compression
+gzip compressed data, was "dist/radical.gtod-1.6.7.tar", last modified: Fri Jul  9 08:02:35 2021, max compression
```

## Comparing `radical.gtod-1.5.0.tar` & `radical.gtod-1.6.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      829 2020-08-04 23:58:56.000000 radical.gtod-1.5.0/CHANGES.md
--rw-r--r--   0 merzky    (1000) merzky    (1000)     8365 2020-07-21 20:11:05.000000 radical.gtod-1.5.0/LICENSE.md
--rw-r--r--   0 merzky    (1000) merzky    (1000)       79 2020-07-21 20:11:05.000000 radical.gtod-1.5.0/MANIFEST.in
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1003 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/PKG-INFO
--rw-r--r--   0 merzky    (1000) merzky    (1000)      640 2020-07-21 20:17:36.000000 radical.gtod-1.5.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        6 2020-08-04 23:58:56.000000 radical.gtod-1.5.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/bin/
--rwxr-xr-x   0 merzky    (1000) merzky    (1000)      140 2020-07-21 20:29:35.000000 radical.gtod-1.5.0/bin/radical-gtod-version
--rw-r--r--   0 merzky    (1000) merzky    (1000)       67 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10497 2020-08-04 23:58:56.000000 radical.gtod-1.5.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/src/radical/gtod/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       41 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical/gtod/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       21 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical/gtod/VERSION
--rw-r--r--   0 merzky    (1000) merzky    (1000)      532 2020-07-21 20:29:08.000000 radical.gtod-1.5.0/src/radical/gtod/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      196 2020-08-04 23:56:19.000000 radical.gtod-1.5.0/src/radical/gtod/gtod.c
--rw-r--r--   0 merzky    (1000) merzky    (1000)      422 2020-07-21 20:11:05.000000 radical.gtod-1.5.0/src/radical/gtod/gtod_module.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    16840 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical/gtod/radical-gtod
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2020-08-04 23:59:25.464876 radical.gtod-1.5.0/src/radical.gtod.egg-info/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1003 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      506 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2020-08-04 23:59:25.000000 radical.gtod-1.5.0/src/radical.gtod.egg-info/top_level.txt
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

### Comparing `radical.gtod-1.5.0/CHANGES.md` & `radical.gtod-1.6.7/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,29 @@
     https://github.com/radical-cybertools/radical.gtod/issues\
             ?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
   - For a list of open issues and known problems, see
     https://github.com/radical-cybertools/radical.gtod/issues\
             ?q=is%3Aissue+is%3Aopen+
     
 
-Version 0.0.1 release                                                 2020-07-25
+Version 1.6.7 release                                                 2021-07-09
 --------------------------------------------------------------------------------
+  
+  - remove cached wheel
+  - update license in pypi meta-data
+  - update output destination for an exception
 
-  - initial commit for radical project 'gtod'
 
-    
 Version 1.5.0 release                                                 2020-08-05
 --------------------------------------------------------------------------------
   
   - failsafe deployment (shell/python fallback)
 
 
+Version 0.0.1 release                                                 2020-07-25
+--------------------------------------------------------------------------------
+
+  - initial commit for radical project 'gtod'
+
+    
 --------------------------------------------------------------------------------
```

### Comparing `radical.gtod-1.5.0/LICENSE.md` & `radical.gtod-1.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.gtod-1.5.0/PKG-INFO` & `radical.gtod-1.6.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.2
 Name: radical.gtod
-Version: 1.5.0
+Version: 1.6.7
 Summary: returns seconds since epoch in subsecond resolution.
 Home-page: https://www.github.com/radical-cybertools/radical.gtod/
 Author: RADICAL Team
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: GPL3
 Description: UNKNOWN
 Keywords: radical distributed computing
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `radical.gtod-1.5.0/README.md` & `radical.gtod-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `radical.gtod-1.5.0/setup.py` & `radical.gtod-1.6.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 __author__    = 'RADICAL Team'
 __email__     = 'radical@radical-project.org'
 __copyright__ = 'Copyright date 2020, RADICAL Team'
 __license__   = 'GPL.v3'
 
 
 ''' Setup script, only usable via pip. '''
 
 import re
 import os
 import sys
-import glob
 import time
+import traceback
 import shutil
 
 import subprocess as sp
 
 
 from setuptools import setup, Command, find_namespace_packages
 
@@ -121,26 +121,26 @@
             # pip install stage 2 or easy_install stage 1
             #
             # pip install will untar the sdist in a tmp tree.  In that tmp
             # tree, we won't be able to derive git version tags -- so we pack
             # the formerly derived version as ./VERSION
             shutil.move("VERSION", "VERSION.bak")              # backup
             shutil.copy("%s/VERSION" % _path, "VERSION")       # version to use
-            os.system  ("python setup.py sdist")               # build sdist
+            os.system  ("python3 setup.py sdist")               # build sdist
             shutil.copy('dist/%s' % _sdist_name,
                         '%s/%s'   % (_mod_root, _sdist_name))  # copy into tree
             shutil.move('VERSION.bak', 'VERSION')              # restore version
 
         with open(_path + '/SDIST', 'w') as f:
             f.write(_sdist_name + '\n')
 
         return _version_base, _version_detail, _sdist_name, _path
 
     except Exception as e:
-        raise RuntimeError('Could not extract/set version: %s' % e)
+        raise RuntimeError('Could not extract/set version: %s' % e) from e
 
 
 # ------------------------------------------------------------------------------
 # check python version. we need >= 3.6
 if  sys.hexversion < 0x03060000:
     raise RuntimeError('%s requires Python 3.6 or higher' % name)
 
@@ -162,42 +162,43 @@
 # ------------------------------------------------------------------------------
 #
 class RunTwine(Command):
     user_options = []
     def initialize_options(self): pass
     def finalize_options(self):   pass
     def run(self):
-        out,  err, ret = sh_callout('python setup.py sdist upload -r pypi')
+        _, _, ret = sh_callout('python3 setup.py sdist upload -r pypi')
         raise SystemExit(ret)
 
 
 # ------------------------------------------------------------------------------
+# compile radical-gtod
+#
 # FIXME: pip3 bug: binaries files cannot be installed into bin.
-# NOTE : disable to avoid stupid/inconsequrntial bwheel error
-# compile gtod
-
+# NOTE : disable to avoid stupid/inconsequentially wheel error
+#
+src = 'src/radical/gtod/gtod.c'
+tgt = 'src/radical/gtod/radical-gtod'
 try:
     from distutils.ccompiler import new_compiler
 
-    src      = 'src/radical/gtod/gtod.c'
-    tgt      = 'src/radical/gtod/radical-gtod'
     compiler = new_compiler(verbose=1)
     objs     = compiler.compile(sources=[src])
     exe      = compiler.link_executable(objs, tgt)
 
     # test the resulting binary - and if it does not seem to work, replace it
     # by a shell script which provides a poor-man's version of the C code.
     now_1 = time.time()
-    out, err, ret = sh_callout(tgt)
+    out, _, _ = sh_callout(tgt)
     now_2 = time.time()
     now   = float(out)
 
     assert(now_1 <= now  )
     assert(now   <= now_2)
-    assert(now_2  - now_1 <= 0.01)
+    assert(now_2  - now_1 <= 1.)
 
 except:
     # need a replacement
     with open(tgt, 'w') as fout:
         fout.write('''#!/bin/sh
 
 nsec=$(date +%N | cut -c 1-6)
@@ -206,14 +207,16 @@
 then
     python3 -c 'import time; print("%.6f" % time.time())'
 else
     echo "$(date +%s).$nsec"
 fi
 
 ''')
+        fout.write('# [WARNING] Exception during compilation:\n')
+        fout.write('# %s\n' % '\n# '.join(traceback.format_exc().splitlines()))
     os.system('chmod 0755 %s' % tgt)
 
 
 
 # ------------------------------------------------------------------------------
 #
 # This copies the contents like examples/ dir under sys.prefix/share/$name
@@ -237,15 +240,15 @@
     'license'            : 'GPL3',
     'keywords'           : 'radical distributed computing',
     'python_requires'    : '>=3.6',
     'classifiers'        : [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Environment :: Console',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Topic :: Utilities',
         'Topic :: System :: Distributed Computing',
         'Topic :: Scientific/Engineering',
         'Operating System :: MacOS :: MacOS X',
@@ -292,10 +295,16 @@
 setup(**setup_args)
 
 os.system('rm -rf src/%s.egg-info' % name)
 # os.system('rm -rf %s/VERSION'      % path)
 # os.system('rm -rf %s/VERSION.git'  % path)
 # os.system('rm -rf %s/SDIST'        % path)
 
+# gtod is compiled, and pip tries to cache compiled modules in a wheel.
+# On resources, where $HOME is on a shared filesystem and serves multiple hosts
+# with different architectures, pip will pull the cached wheel for the wrong
+# architecture. The installation then succeeds, but the module is unusable and
+# leads to runtime errors which are hard to trace. Thus, remove cached wheel.
+os.system('pip cache remove %s' % name)
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical.gtod-1.5.0/src/radical/gtod/__init__.py` & `radical.gtod-1.6.7/src/radical/gtod/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.gtod-1.5.0/src/radical.gtod.egg-info/PKG-INFO` & `radical.gtod-1.6.7/src/radical.gtod.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.2
 Name: radical.gtod
-Version: 1.5.0
+Version: 1.6.7
 Summary: returns seconds since epoch in subsecond resolution.
 Home-page: https://www.github.com/radical-cybertools/radical.gtod/
 Author: RADICAL Team
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: GPL3
 Description: UNKNOWN
 Keywords: radical distributed computing
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
```

