# Comparing `tmp/types-pyinstaller-6.5.0.20240311.tar.gz` & `tmp/types-pyinstaller-6.6.0.20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyinstaller-6.5.0.20240311.tar", last modified: Mon Mar 11 02:17:26 2024, max compression
+gzip compressed data, was "types-pyinstaller-6.6.0.20240415.tar", last modified: Mon Apr 15 04:04:36 2024, max compression
```

## Comparing `types-pyinstaller-6.5.0.20240311.tar` & `types-pyinstaller-6.6.0.20240415.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-11 02:17:25.000000 types-pyinstaller-6.5.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:17:25.000000 types-pyinstaller-6.5.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.201161 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-11 02:17:25.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/__main__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.201161 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/build_main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/datastruct.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/splash.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.201161 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/analysis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/imphookapi.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.201161 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/isolated/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/isolated/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/isolated/_parent.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/modulegraph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/modulegraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/hooks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/hooks/conda.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/win32/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/win32/versioninfo.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/pyi_splash-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-11 02:17:25.000000 types-pyinstaller-6.5.0.20240311/pyi_splash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-11 02:14:35.000000 types-pyinstaller-6.5.0.20240311/pyi_splash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-11 02:17:25.000000 types-pyinstaller-6.5.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:17:26.205162 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-11 02:17:26.000000 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-11 02:17:26.000000 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:17:26.000000 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 02:17:26.000000 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-11 02:17:26.000000 types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.784330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/__main__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.784330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/build_main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/datastruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/splash.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/analysis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/imphookapi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/isolated/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/isolated/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/isolated/_parent.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/modulegraph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/modulegraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/hooks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/hooks/conda.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/win32/versioninfo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/pyi_splash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/pyi_splash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 04:04:15.000000 types-pyinstaller-6.6.0.20240415/pyi_splash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/pyi_splash-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:04:36.788330 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 04:04:36.000000 types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/top_level.txt
```

### Comparing `types-pyinstaller-6.5.0.20240311/CHANGELOG.md` & `types-pyinstaller-6.6.0.20240415/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 6.6.0.20240415 (2024-04-15)
+
+Bump pyinstaller to 6.6.* (#11764)
+
 ## 6.5.0.20240311 (2024-03-11)
 
 Bump pyinstaller to 6.5.* (#11563)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 6.4.0.20240212 (2024-02-12)
```

### Comparing `types-pyinstaller-6.5.0.20240311/PKG-INFO` & `types-pyinstaller-6.6.0.20240415/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 6.5.0.20240311
+Version: 6.6.0.20240415
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`.
 
 This version of `types-pyinstaller` aims to provide accurate annotations
-for `pyinstaller==6.5.*`.
+for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/api.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/build_main.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/build_main.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import Incomplete, StrPath
 from collections.abc import Iterable
-from typing import Any
+from typing import Any, Literal
 
 from PyInstaller.building import _PyiBlockCipher
 from PyInstaller.building.datastruct import Target, _TOCTuple
 
 # Referenced in: https://pyinstaller.org/en/stable/hooks.html#PyInstaller.utils.hooks.get_hook_config
 # Not to be imported during runtime, but is the type reference for hooks and analysis configuration
 # Also referenced in https://pyinstaller.org/en/stable/spec-files.html
@@ -35,8 +35,9 @@
         excludes: Incomplete | None = None,
         runtime_hooks: Incomplete | None = None,
         cipher: _PyiBlockCipher = None,
         win_no_prefer_redirects: bool = False,
         win_private_assemblies: bool = False,
         noarchive: bool = False,
         module_collection_mode: Incomplete | None = None,
+        optimize: Literal[-1, 0, 1, 2] | None = -1,
     ) -> None: ...
```

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/datastruct.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/datastruct.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/building/splash.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/building/splash.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/compat.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/analysis.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/analysis.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/depend/imphookapi.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/depend/imphookapi.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/isolated/_parent.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/isolated/_parent.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/lib/modulegraph/modulegraph.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/hooks/__init__.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/hooks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/hooks/conda.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/hooks/conda.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/PyInstaller-stubs/utils/win32/versioninfo.pyi` & `types-pyinstaller-6.6.0.20240415/PyInstaller-stubs/utils/win32/versioninfo.pyi`

 * *Files identical despite different names*

### Comparing `types-pyinstaller-6.5.0.20240311/setup.py` & `types-pyinstaller-6.6.0.20240415/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`.
 
 This version of `types-pyinstaller` aims to provide accurate annotations
-for `pyinstaller==6.5.*`.
+for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="6.5.0.20240311",
+      version="6.6.0.20240415",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-setuptools'],
-      packages=['PyInstaller-stubs', 'pyi_splash-stubs'],
-      package_data={'PyInstaller-stubs': ['__init__.pyi', '__main__.pyi', 'building/__init__.pyi', 'building/api.pyi', 'building/build_main.pyi', 'building/datastruct.pyi', 'building/splash.pyi', 'compat.pyi', 'depend/__init__.pyi', 'depend/analysis.pyi', 'depend/imphookapi.pyi', 'isolated/__init__.pyi', 'isolated/_parent.pyi', 'lib/__init__.pyi', 'lib/modulegraph/__init__.pyi', 'lib/modulegraph/modulegraph.pyi', 'utils/__init__.pyi', 'utils/hooks/__init__.pyi', 'utils/hooks/conda.pyi', 'utils/win32/versioninfo.pyi', 'METADATA.toml'], 'pyi_splash-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['pyi_splash-stubs', 'PyInstaller-stubs'],
+      package_data={'pyi_splash-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed'], 'PyInstaller-stubs': ['__init__.pyi', '__main__.pyi', 'building/__init__.pyi', 'building/api.pyi', 'building/build_main.pyi', 'building/datastruct.pyi', 'building/splash.pyi', 'compat.pyi', 'depend/__init__.pyi', 'depend/analysis.pyi', 'depend/imphookapi.pyi', 'isolated/__init__.pyi', 'isolated/_parent.pyi', 'lib/__init__.pyi', 'lib/modulegraph/__init__.pyi', 'lib/modulegraph/modulegraph.pyi', 'utils/__init__.pyi', 'utils/hooks/__init__.pyi', 'utils/hooks/conda.pyi', 'utils/win32/versioninfo.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/PKG-INFO` & `types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyinstaller
-Version: 6.5.0.20240311
+Version: 6.6.0.20240415
 Summary: Typing stubs for pyinstaller
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyinstaller.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyinstaller`.
 
 This version of `types-pyinstaller` aims to provide accurate annotations
-for `pyinstaller==6.5.*`.
+for `pyinstaller==6.6.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyinstaller. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7c8e82fe483a40ec4cb0a2505cfdb0f3e7cc81d9` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-pyinstaller-6.5.0.20240311/types_pyinstaller.egg-info/SOURCES.txt` & `types-pyinstaller-6.6.0.20240415/types_pyinstaller.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.md
 MANIFEST.in
 setup.py
 PyInstaller-stubs/METADATA.toml
 PyInstaller-stubs/__init__.pyi
 PyInstaller-stubs/__main__.pyi
 PyInstaller-stubs/compat.pyi
+PyInstaller-stubs/py.typed
 PyInstaller-stubs/building/__init__.pyi
 PyInstaller-stubs/building/api.pyi
 PyInstaller-stubs/building/build_main.pyi
 PyInstaller-stubs/building/datastruct.pyi
 PyInstaller-stubs/building/splash.pyi
 PyInstaller-stubs/depend/__init__.pyi
 PyInstaller-stubs/depend/analysis.pyi
@@ -20,12 +21,13 @@
 PyInstaller-stubs/lib/modulegraph/modulegraph.pyi
 PyInstaller-stubs/utils/__init__.pyi
 PyInstaller-stubs/utils/hooks/__init__.pyi
 PyInstaller-stubs/utils/hooks/conda.pyi
 PyInstaller-stubs/utils/win32/versioninfo.pyi
 pyi_splash-stubs/METADATA.toml
 pyi_splash-stubs/__init__.pyi
+pyi_splash-stubs/py.typed
 types_pyinstaller.egg-info/PKG-INFO
 types_pyinstaller.egg-info/SOURCES.txt
 types_pyinstaller.egg-info/dependency_links.txt
 types_pyinstaller.egg-info/requires.txt
 types_pyinstaller.egg-info/top_level.txt
```

