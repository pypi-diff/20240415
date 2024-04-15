# Comparing `tmp/radical.repex-1.47.0.tar.gz` & `tmp/radical_repex-1.47.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical.repex-1.47.0.tar", last modified: Thu Feb  8 22:00:15 2024, max compression
+gzip compressed data, was "radical_repex-1.47.1.tar", last modified: Mon Apr 15 06:14:50 2024, max compression
```

## Comparing `radical.repex-1.47.0.tar` & `radical_repex-1.47.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2753 2024-02-08 22:00:09.000000 radical.repex-1.47.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical.repex-1.47.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical.repex-1.47.0/MANIFEST.in
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-02-08 22:00:15.297839 radical.repex-1.47.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical.repex-1.47.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-02-08 21:59:57.000000 radical.repex-1.47.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical.repex-1.47.0/bin/radical-repex
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical.repex-1.47.0/bin/radical-repex-version
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-02-08 22:00:15.297839 radical.repex-1.47.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10450 2022-08-15 10:38:30.000000 radical.repex-1.47.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical/repex/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical/repex/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical/repex/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical.repex-1.47.0/src/radical/repex/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/algorithms.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/exchange.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/replica.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical.repex-1.47.0/src/radical/repex/utils.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-02-08 22:00:15.297839 radical.repex-1.47.0/src/radical.repex.egg-info/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      984 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      606 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-02-08 22:00:15.000000 radical.repex-1.47.0/src/radical.repex.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     2753 2024-02-08 22:00:18.000000 radical_repex-1.47.1/CHANGES.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1075 2021-09-24 08:25:16.000000 radical_repex-1.47.1/LICENSE.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:25:16.000000 radical_repex-1.47.1/MANIFEST.in
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 06:14:50.606056 radical_repex-1.47.1/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1762 2021-09-24 08:25:16.000000 radical_repex-1.47.1/README.md
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 06:14:14.000000 radical_repex-1.47.1/VERSION
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/bin/
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      926 2021-11-23 18:02:02.000000 radical_repex-1.47.1/bin/radical-repex
+-rwxrwxr-x   0 merzky    (1000) merzky    (1000)      143 2021-09-24 08:25:16.000000 radical_repex-1.47.1/bin/radical-repex-version
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       72 2024-04-15 06:14:50.606056 radical_repex-1.47.1/setup.cfg
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    10332 2024-04-15 06:14:46.000000 radical_repex-1.47.1/setup.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/src/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.602056 radical_repex-1.47.1/src/radical/
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/src/radical/repex/
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       28 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical/repex/SDIST
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical/repex/VERSION
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      685 2021-09-24 08:25:16.000000 radical_repex-1.47.1/src/radical/repex/__init__.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     4354 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/algorithms.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)    11049 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/exchange.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     8590 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/replica.py
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)     1319 2021-11-23 18:02:02.000000 radical_repex-1.47.1/src/radical/repex/utils.py
+drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 06:14:50.606056 radical_repex-1.47.1/src/radical.repex.egg-info/
+-rw-r--r--   0 merzky    (1000) merzky    (1000)     1053 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)      556 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)       39 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 06:14:50.000000 radical_repex-1.47.1/src/radical.repex.egg-info/top_level.txt
```

### Comparing `radical.repex-1.47.0/CHANGES.md` & `radical_repex-1.47.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/LICENSE.md` & `radical_repex-1.47.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/PKG-INFO` & `radical_repex-1.47.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.47.0
+Version: 1.47.1
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
@@ -20,7 +20,9 @@
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 License-File: LICENSE.md
+Requires-Dist: radical.utils>=1.12
+Requires-Dist: radical.entk>=1.12
```

### Comparing `radical.repex-1.47.0/README.md` & `radical_repex-1.47.1/README.md`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/bin/radical-repex` & `radical_repex-1.47.1/bin/radical-repex`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/setup.py` & `radical_repex-1.47.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 import subprocess as sp
 
 from setuptools import setup, Command, find_namespace_packages
 
 
 # ------------------------------------------------------------------------------
-name     = 'radical.repex'
-mod_root = 'src/radical/repex/'
+base     = 'repex'
+name     = 'radical.%s'      % base
+mod_root = 'src/radical/%s/' % base
 
 # ------------------------------------------------------------------------------
 #
 # pip warning:
 # "In-tree builds are now default. pip 22.1 will enforce this behaviour change.
 #  A possible replacement is to remove the --use-feature=in-tree-build flag."
 #
@@ -43,14 +44,16 @@
 #
 # We thus introduce an env variable `SDIST_LEVEL` which allows us to separate
 # internal calls from the top level invocation - we only clean on the latter
 # (see end of this file).
 sdist_level = int(os.environ.get('SDIST_LEVEL', 0))
 os.environ['SDIST_LEVEL'] = str(sdist_level + 1)
 
+root = os.path.dirname(__file__) or '.'
+
 
 # ------------------------------------------------------------------------------
 #
 def sh_callout(cmd):
 
     p = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.PIPE, shell=True)
 
@@ -61,15 +64,15 @@
 
 # ------------------------------------------------------------------------------
 #
 # versioning mechanism:
 #
 #   - version:          1.2.3            - is used for installation
 #   - version_detail:  v1.2.3-9-g0684b06 - is used for debugging
-#   - version is read from VERSION file in src_root, which then is copied to
+#   - version is read from VERSION file in root, which then is copied to
 #     module dir, and is getting installed from there.
 #   - version_detail is derived from the git tag, and only available when
 #     installed from git.  That is stored in mod_root/VERSION in the install
 #     tree.
 #   - The VERSION file is used to provide the runtime version information.
 #
 def get_version(_mod_root):
@@ -82,34 +85,30 @@
     try:
 
         _version_base   = None
         _version_detail = None
         _sdist_name     = None
 
         # get version from './VERSION'
-        src_root = os.path.dirname(__file__)
-        if not src_root:
-            src_root = '.'
-
-        with open(src_root + '/VERSION', 'r', encoding='utf-8') as f:
-            _version_base = f.readline().strip()
+        with open('%s/VERSION' % root, 'r', encoding='utf-8') as fin:
+            _version_base = fin.readline().strip()
 
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
-            'echo $tag@$branch' % src_root)
+            'echo $tag@$branch' % root)
         _version_detail = out.strip()
         _version_detail = _version_detail.decode()
         _version_detail = _version_detail.replace('detached from ', 'detached-')
 
         # remove all non-alphanumeric (and then some) chars
         _version_detail = re.sub('[/ ]+', '-', _version_detail)
         _version_detail = re.sub('[^a-zA-Z0-9_+@.-]+', '', _version_detail)
@@ -123,25 +122,29 @@
             _version = _version_base
         elif '@' not in _version_base:
             _version = '%s-%s' % (_version_base, _version_detail)
         else:
             _version = _version_base
 
         # make sure the version files exist for the runtime version inspection
-        _path = '%s/%s' % (src_root, _mod_root)
-        with open(_path + '/VERSION', 'w', encoding='utf-8') as f:
-            f.write(_version_base + '\n')
-            f.write(_version      + '\n')
+        _path = '%s/%s' % (root, _mod_root)
+        with open(_path + '/VERSION', 'w', encoding='utf-8') as fout:
+            fout.write(_version_base + '\n')
+            fout.write(_version      + '\n')
 
         _sdist_name = '%s-%s.tar.gz' % (name, _version_base)
       # _sdist_name = _sdist_name.replace('/', '-')
       # _sdist_name = _sdist_name.replace('@', '-')
       # _sdist_name = _sdist_name.replace('#', '-')
       # _sdist_name = _sdist_name.replace('_', '-')
 
+        # setuptools 69.5 does changes naming scheme
+        if not os.path.isfile('%s/%s' % (_path, _sdist_name)):
+            _sdist_name = '%s-%s.tar.gz' % (name.replace('.', '_'), _version_base)
+
         if '--record'    in sys.argv or \
            'bdist_egg'   in sys.argv or \
            'bdist_wheel' in sys.argv    :
             # pip install stage 2 or easy_install stage 1
             #
             # pip install will untar the sdist in a tmp tree.  In that tmp
             # tree, we won't be able to derive git version tags -- so we pack
@@ -149,16 +152,16 @@
             shutil.move('VERSION', 'VERSION.bak')              # backup
             shutil.copy('%s/VERSION' % _path, 'VERSION')       # version to use
             os.system  ('python3 setup.py sdist')              # build sdist
             shutil.copy('dist/%s' % _sdist_name,
                         '%s/%s'   % (_mod_root, _sdist_name))  # copy into tree
             shutil.move('VERSION.bak', 'VERSION')              # restore version
 
-        with open(_path + '/SDIST', 'w', encoding='utf-8') as f:
-            f.write(_sdist_name + '\n')
+        with open(_path + '/SDIST', 'w', encoding='utf-8') as fout:
+            fout.write(_sdist_name + '\n')
 
         return _version_base, _version_detail, _sdist_name, _path
 
     except Exception as e:
         raise RuntimeError('Could not extract/set version: %s' % e) from e
 
 
@@ -184,23 +187,22 @@
         raise SystemExit(ret)
 
 
 # ------------------------------------------------------------------------------
 #
 # This copies the contents like examples/ dir under sys.prefix/share/$name
 # It needs the MANIFEST.in entries to work.
-base = 'share/%s' % name
-df = [('%s/' % base, glob.glob('examples/*.{py,cfg}'))]
+df = [('share/%s/' % name, glob.glob('examples/*.{py,cfg}'))]
 
 
 # ------------------------------------------------------------------------------
 #
 setup_args = {
     'name'               : name,
-    'namespace_packages' : ['radical'],
+  # 'namespace_packages' : ['radical'],
     'version'            : version,
     'description'        : 'RADICAL Replica Exchange Framework.',
     'author'             : 'RADICAL Group at Rutgers University',
     'author_email'       : 'radical@rutgers.edu',
     'maintainer'         : 'The RADICAL Group',
     'maintainer_email'   : 'radical@rutgers.edu',
     'url'                : 'https://www.github.com/radical-cybertools/radical.repex/',
@@ -231,29 +233,18 @@
   # 'setup_requires'     : ['pytest-runner'],
     'install_requires'   : ['radical.utils>=1.12',
                             'radical.entk>=1.12'],
     'tests_require'      : ['pytest',
                             'pylint',
                             'flake8',
                             'coverage',
-                            'mock==2.0.0.',
+                            'mock==2.0.0',
                            ],
     'test_suite'         : '%s.tests' % name,
     'zip_safe'           : False,
-  # 'build_sphinx'       : {
-  #     'source-dir'     : 'docs/',
-  #     'build-dir'      : 'docs/build',
-  #     'all_files'      : 1,
-  # },
-  # 'upload_sphinx'      : {
-  #     'upload-dir'     : 'docs/build/html',
-  # },
-    # This copies the contents of the examples/ dir under
-    # sys.prefix/share/$name
-    # It needs the MANIFEST.in entries to work.
     'data_files'         : df,
     'cmdclass'           : {'upload': RunTwine},
 }
 
 
 # ------------------------------------------------------------------------------
 #
@@ -265,7 +256,9 @@
 if sdist_level == 0:
     os.system('rm -vrf src/%s.egg-info' % name)
     os.system('rm -vf  %s/%s'           % (path, sdist_name))
     os.system('rm -vf  %s/VERSION'      % path)
     os.system('rm -vf  %s/SDIST'        % path)
 
 
+# ------------------------------------------------------------------------------
+
```

### Comparing `radical.repex-1.47.0/src/radical/repex/__init__.py` & `radical_repex-1.47.1/src/radical/repex/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/src/radical/repex/algorithms.py` & `radical_repex-1.47.1/src/radical/repex/algorithms.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/src/radical/repex/exchange.py` & `radical_repex-1.47.1/src/radical/repex/exchange.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/src/radical/repex/replica.py` & `radical_repex-1.47.1/src/radical/repex/replica.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/src/radical/repex/utils.py` & `radical_repex-1.47.1/src/radical/repex/utils.py`

 * *Files identical despite different names*

### Comparing `radical.repex-1.47.0/src/radical.repex.egg-info/PKG-INFO` & `radical_repex-1.47.1/src/radical.repex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radical.repex
-Version: 1.47.0
+Version: 1.47.1
 Summary: RADICAL Replica Exchange Framework.
 Home-page: https://www.github.com/radical-cybertools/radical.repex/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
@@ -20,7 +20,9 @@
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 License-File: LICENSE.md
+Requires-Dist: radical.utils>=1.12
+Requires-Dist: radical.entk>=1.12
```

### Comparing `radical.repex-1.47.0/src/radical.repex.egg-info/SOURCES.txt` & `radical_repex-1.47.1/src/radical.repex.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 setup.cfg
 setup.py
 bin/radical-repex
 bin/radical-repex-version
 src/radical.repex.egg-info/PKG-INFO
 src/radical.repex.egg-info/SOURCES.txt
 src/radical.repex.egg-info/dependency_links.txt
-src/radical.repex.egg-info/namespace_packages.txt
 src/radical.repex.egg-info/not-zip-safe
 src/radical.repex.egg-info/requires.txt
 src/radical.repex.egg-info/top_level.txt
 src/radical/repex/SDIST
 src/radical/repex/VERSION
 src/radical/repex/__init__.py
 src/radical/repex/algorithms.py
```

