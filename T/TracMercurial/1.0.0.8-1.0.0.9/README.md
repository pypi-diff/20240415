# Comparing `tmp/TracMercurial-1.0.0.8.tar.gz` & `tmp/TracMercurial-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TracMercurial-1.0.0.8.tar", last modified: Wed Jan 16 22:23:36 2019, max compression
+gzip compressed data, was "dist/TracMercurial-1.0.0.9.tar", last modified: Thu Jan 17 23:25:13 2019, max compression
```

## Comparing `TracMercurial-1.0.0.8.tar` & `TracMercurial-1.0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/
--rw-r--r--   0 rjollos    (501) staff       (20)      487 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/PKG-INFO
--rw-r--r--   0 rjollos    (501) staff       (20)     2599 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.8/README
--rw-r--r--   0 rjollos    (501) staff       (20)     1738 2019-01-16 22:20:23.000000 TracMercurial-1.0.0.8/setup.py
--rw-r--r--   0 rjollos    (501) staff       (20)      517 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/setup.cfg
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/
--rw-r--r--   0 rjollos    (501) staff       (20)      487 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/PKG-INFO
--rw-r--r--   0 rjollos    (501) staff       (20)        8 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/namespace_packages.txt
--rw-r--r--   0 rjollos    (501) staff       (20)      511 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/SOURCES.txt
--rw-r--r--   0 rjollos    (501) staff       (20)       40 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/entry_points.txt
--rw-r--r--   0 rjollos    (501) staff       (20)       10 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/requires.txt
--rw-r--r--   0 rjollos    (501) staff       (20)        8 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/top_level.txt
--rw-r--r--   0 rjollos    (501) staff       (20)        1 2019-01-16 22:23:33.000000 TracMercurial-1.0.0.8/TracMercurial.egg-info/dependency_links.txt
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/tracext/
--rw-r--r--   0 rjollos    (501) staff       (20)       56 2017-08-25 16:50:58.000000 TracMercurial-1.0.0.8/tracext/__init__.py
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/tracext/hg/
--rw-r--r--   0 rjollos    (501) staff       (20)     4811 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.8/tracext/hg/hooks.py
--rw-r--r--   0 rjollos    (501) staff       (20)    54058 2019-01-16 22:20:23.000000 TracMercurial-1.0.0.8/tracext/hg/backend.py
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/tracext/hg/locale/
--rw-r--r--   0 rjollos    (501) staff       (20)     2860 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.8/tracext/hg/locale/messages.pot
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/tracext/hg/locale/fr/
-drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-16 22:23:36.000000 TracMercurial-1.0.0.8/tracext/hg/locale/fr/LC_MESSAGES/
--rw-r--r--   0 rjollos    (501) staff       (20)     2779 2019-01-16 22:23:32.000000 TracMercurial-1.0.0.8/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.mo
--rw-r--r--   0 rjollos    (501) staff       (20)     4154 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.8/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.po
--rw-r--r--   0 rjollos    (501) staff       (20)        2 2017-08-25 16:50:58.000000 TracMercurial-1.0.0.8/tracext/hg/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/
+-rw-r--r--   0 rjollos    (501) staff       (20)      487 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/PKG-INFO
+-rw-r--r--   0 rjollos    (501) staff       (20)     2599 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.9/README
+-rw-r--r--   0 rjollos    (501) staff       (20)     1786 2019-01-16 23:11:59.000000 TracMercurial-1.0.0.9/setup.py
+-rw-r--r--   0 rjollos    (501) staff       (20)      517 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/setup.cfg
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/
+-rw-r--r--   0 rjollos    (501) staff       (20)      487 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/PKG-INFO
+-rw-r--r--   0 rjollos    (501) staff       (20)        8 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/namespace_packages.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)      511 2019-01-17 23:25:11.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/SOURCES.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)       40 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/entry_points.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)       10 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/requires.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)        8 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/top_level.txt
+-rw-r--r--   0 rjollos    (501) staff       (20)        1 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/TracMercurial.egg-info/dependency_links.txt
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/tracext/
+-rw-r--r--   0 rjollos    (501) staff       (20)       56 2017-08-25 16:50:58.000000 TracMercurial-1.0.0.9/tracext/__init__.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/tracext/hg/
+-rw-r--r--   0 rjollos    (501) staff       (20)     4811 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.9/tracext/hg/hooks.py
+-rw-r--r--   0 rjollos    (501) staff       (20)    54625 2019-01-16 23:11:59.000000 TracMercurial-1.0.0.9/tracext/hg/backend.py
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/tracext/hg/locale/
+-rw-r--r--   0 rjollos    (501) staff       (20)     2860 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.9/tracext/hg/locale/messages.pot
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/tracext/hg/locale/fr/
+drwxr-xr-x   0 rjollos    (501) staff       (20)        0 2019-01-17 23:25:13.000000 TracMercurial-1.0.0.9/tracext/hg/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 rjollos    (501) staff       (20)     2779 2019-01-17 23:25:10.000000 TracMercurial-1.0.0.9/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.mo
+-rw-r--r--   0 rjollos    (501) staff       (20)     4154 2019-01-16 21:18:40.000000 TracMercurial-1.0.0.9/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.po
+-rw-r--r--   0 rjollos    (501) staff       (20)        2 2017-08-25 16:50:58.000000 TracMercurial-1.0.0.9/tracext/hg/__init__.py
```

### Comparing `TracMercurial-1.0.0.8/README` & `TracMercurial-1.0.0.9/README`

 * *Files identical despite different names*

### Comparing `TracMercurial-1.0.0.8/setup.py` & `TracMercurial-1.0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 TracMercurial = 'https://trac.edgewall.org/wiki/TracMercurial'
 
 setup(name='TracMercurial',
       install_requires='Trac >= 1.0',
       description='Mercurial plugin for Trac (1.0 branch)',
       keywords='trac scm plugin mercurial hg',
-      version='1.0.0.8',
+      version='1.0.0.9',
       url=TracMercurial,
       license='GPL',
       author='Christian Boos',
       author_email='cboos@edgewall.org',
       long_description="""
       This plugin for Trac 1.0 provides support for the Mercurial SCM.
 
@@ -51,9 +51,10 @@
       """ % TracMercurial,
       namespace_packages=['tracext'],
       packages=['tracext', 'tracext.hg'],
       package_data={
           '': ['COPYING', 'README'],
           'tracext.hg': ['locale/*.*', 'locale/*/LC_MESSAGES/*.*'],
           },
+      test_suite='tracext.hg.tests.test_suite',
       entry_points={'trac.plugins': 'hg = tracext.hg.backend'},
       **extra)
```

### Comparing `TracMercurial-1.0.0.8/setup.cfg` & `TracMercurial-1.0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `TracMercurial-1.0.0.8/tracext/hg/hooks.py` & `TracMercurial-1.0.0.9/tracext/hg/hooks.py`

 * *Files identical despite different names*

### Comparing `TracMercurial-1.0.0.8/tracext/hg/backend.py` & `TracMercurial-1.0.0.9/tracext/hg/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,20 @@
 import posixpath
 import re
 import sys
 import types
 
 import pkg_resources
 
-from genshi.builder import tag
-
 from trac.core import *
 from trac.config import BoolOption, ChoiceOption, ListOption, PathOption
 from trac.env import ISystemInfoProvider
 from trac.util import arity
 from trac.util.datefmt import FixedOffset, utc
+from trac.util.html import html as tag
 from trac.util.text import exception_to_unicode, shorten_line, to_unicode
 from trac.util.translation import _, domain_functions
 from trac.versioncontrol.api import Changeset, Node, Repository, \
                                     IRepositoryConnector, RepositoryManager, \
                                     NoSuchChangeset, NoSuchNode
 from trac.versioncontrol.web_ui import IPropertyRenderer, RenderedProperty
 from trac.wiki import IWikiSyntaxProvider
@@ -52,27 +51,27 @@
 
 # -- Using internal Mercurial API, see:
 #     * http://mercurial.selenic.com/wiki/MercurialApi
 #     * http://mercurial.selenic.com/wiki/ApiChanges
 
 _stat_float_times = os.stat_float_times()
 
-hg_import_error = []
+hg_import_error = None
 try:
     # The new `demandimport` mechanism doesn't play well with code relying
     # on the `ImportError` exception being caught.
     # OTOH, we can't disable `demandimport` because mercurial relies on it
     # (circular reference issue). So for now, we activate `demandimport`
     # before loading mercurial modules, and desactivate it afterwards.
     #
     # See http://www.selenic.com/mercurial/bts/issue605
 
     try:
         from mercurial import demandimport
-        demandimport.enable();
+        demandimport.enable()
     except ImportError, hg_import_error:
         demandimport = None
 
     from mercurial import hg
     from mercurial.context import filectx
     from mercurial.ui import ui
     from mercurial.node import hex, short, nullid, nullrev
@@ -81,36 +80,43 @@
     from mercurial import encoding
     from mercurial import extensions
     from mercurial.extensions import loadall
     from mercurial.error import RepoLookupError
 
     # Note: due to the nature of demandimport, there will be no actual
     # import error until those symbols get accessed, so here we go:
+    demandimport_errors = []
     for sym in ("filectx ui hex short nullid pathto "
                 "cachefunc loadall".split()):
         if repr(globals()[sym]) == "<unloaded module '%s'>" % sym:
-            hg_import_error.append(sym)
-    if hg_import_error:
-        hg_import_error = "Couldn't import symbols: "+','.join(hg_import_error)
+            demandimport_errors.append(sym)
+    if demandimport_errors:
+        raise ImportError("Couldn't import symbols: %s" %
+                          ','.join(demandimport_errors))
+    del demandimport_errors
 
-    # Mercurial versions >= 1.2 won't have mercurial.repo.RepoError anymore
     try:
-        from mercurial.repo import RepoError
-    except ImportError: # Mercurial 2.3.1 doesn't even have mercurial.repo!
-        RepoError = None
-    from mercurial.revlog import LookupError as HgLookupError
-    if RepoError is None or repr(RepoError) == "<unloaded module 'RepoError'>":
         from mercurial.error import RepoError, LookupError as HgLookupError
+    except ImportError:
+        # mercurial.repo.RepoError unavailable if Mercurial >= 1.2
+        from mercurial.repo import RepoError
+        if repr(RepoError).startswith('<unloaded module '):
+            raise ImportError("Couldn't import symbol: RepoError")
+        # mercurial.revlog.LookupError unavailable if Mercurial >= 4.8
+        from mercurial.revlog import LookupError as HgLookupError
+        if repr(HgLookupError).startswith('<unloaded module '):
+            raise ImportError("Couldn't import symbol: LookupError")
 
     # Force local encoding to be non-lossy (#7217)
     os.environ['HGENCODING'] = 'utf-8'
     encoding.tolocal = str
 
     if demandimport:
         demandimport.disable()
+        demandimport = None
 
     # API compatibility (watch http://mercurial.selenic.com/wiki/ApiChanges)
 
     if hasattr(cmdutil, 'match'):
         def match(ctx, *args, **kwargs):
             return cmdutil.match(ctx._repo, *args, **kwargs)
     else:
@@ -126,14 +132,19 @@
     has_bookmarks = bool(listbookmarks)
     has_phasestr = None
 
 except ImportError, e:
     hg_import_error = exception_to_unicode(e)
     ui = object
 
+finally:
+    if demandimport:
+        demandimport.disable()
+        demandimport = None
+
 os.stat_float_times(_stat_float_times) # undo mpm's [341cb90ffd18]
 
 
 ### Helpers
 
 def checked_encode(u, encodings, check):
     """Convert `unicode` to `str` trying several encodings until a
@@ -790,15 +801,17 @@
                     seeds.append(p)
 
     def get_node(self, path, rev=None):
         return MercurialNode(self, self.normalize_path(path),
                              self.changectx(rev))
 
     def get_oldest_rev(self):
-        return 0
+        repo = self.repo
+        n = len(self.repo)
+        return repo[0 if n > 0 else -1].hex()
 
     def get_youngest_rev(self):
         return self.changectx().hex()
 
     def get_path_history(self, path, rev=None, limit=None):
         raise TracError(_('Unsupported "Show only adds and deletes"'))
 
@@ -883,15 +896,15 @@
             for str_path in old_node.manifest:
                 # changes out of scope
                 if str_old_path and not str_path.startswith(str_old_path + '/'):
                     continue
                 # 'deleted' if not present in new manifest
                 str_np = str_new_path + str_path[len(str_old_path):]
                 if str_np not in new_node.manifest:
-                    changes.append((str_path, old_node.subnode(str_np), None,
+                    changes.append((str_path, old_node.subnode(str_path), None,
                                     Node.FILE, Changeset.DELETE))
             # Note: `str_path` only used as a key, no need to convert to_u
             for change in sorted(changes, key=lambda c: c[0]):
                 yield(change[1], change[2], change[3], change[4])
         else:
             if old_node.manifest[old_node.str_path] != \
                    new_node.manifest[new_node.str_path]:
@@ -1242,14 +1255,16 @@
         annotations = []
         if self.filectx:
             for annotateline in self.filectx.annotate(follow=True):
                 if isinstance(annotateline, tuple):
                     fc = annotateline[0]
                     if isinstance(fc, tuple):
                         fc = fc[0]
+                    if not isinstance(fc, filectx):
+                        fc = fc.fctx
                 else:
                     fc = annotateline.fctx
                 annotations.append(fc.rev() or '0')
         return annotations
 
     def get_properties(self):
         if self.isfile and 'x' in self.manifest.flags(self.str_path):
```

### Comparing `TracMercurial-1.0.0.8/tracext/hg/locale/messages.pot` & `TracMercurial-1.0.0.9/tracext/hg/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `TracMercurial-1.0.0.8/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.mo` & `TracMercurial-1.0.0.9/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.mo`

 * *Files identical despite different names*

### Comparing `TracMercurial-1.0.0.8/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.po` & `TracMercurial-1.0.0.9/tracext/hg/locale/fr/LC_MESSAGES/tracmercurial.po`

 * *Files identical despite different names*

