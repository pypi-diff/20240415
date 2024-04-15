# Comparing `tmp/blik-0.6.8.tar.gz` & `tmp/blik-0.6.9.tar.gz`

## Comparing `blik-0.6.8.tar` & `blik-0.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 blik-0.6.8/.cruft.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 blik-0.6.8/.github_changelog_generator
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 blik-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 blik-0.6.8/CITATION.cff
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 blik-0.6.8/.github/dependabot.yml
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 blik-0.6.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 blik-0.6.8/docs/_config.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 blik-0.6.8/docs/_toc.yml
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 blik-0.6.8/docs/getting_started.md
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 blik-0.6.8/docs/index.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 blik-0.6.8/docs/requirements.txt
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 blik-0.6.8/docs/images/favicon.ico
--rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 blik-0.6.8/docs/images/logo.png
--rw-r--r--   0        0        0    22651 2020-02-02 00:00:00.000000 blik-0.6.8/docs/images/logo.svg
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/_version.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/napari.yaml
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/reader.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/utils.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/__init__.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/file_reader.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/filter.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/main_widget.py
--rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/picking.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 blik-0.6.8/src/blik/widgets/power_spectrum.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 blik-0.6.8/tests/conftest.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 blik-0.6.8/tests/test_reader.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 blik-0.6.8/tests/test_widget.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 blik-0.6.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 blik-0.6.8/LICENSE
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 blik-0.6.8/README.md
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 blik-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 blik-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 blik-0.6.9/.cruft.json
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 blik-0.6.9/.github_changelog_generator
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 blik-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 blik-0.6.9/CITATION.cff
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 blik-0.6.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 blik-0.6.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 blik-0.6.9/docs/_config.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 blik-0.6.9/docs/_toc.yml
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 blik-0.6.9/docs/getting_started.md
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 blik-0.6.9/docs/index.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 blik-0.6.9/docs/requirements.txt
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 blik-0.6.9/docs/images/favicon.ico
+-rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 blik-0.6.9/docs/images/logo.png
+-rw-r--r--   0        0        0    22651 2020-02-02 00:00:00.000000 blik-0.6.9/docs/images/logo.svg
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/_version.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/napari.yaml
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/reader.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/utils.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/__init__.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/file_reader.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/filter.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/main_widget.py
+-rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/picking.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 blik-0.6.9/src/blik/widgets/power_spectrum.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 blik-0.6.9/tests/conftest.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 blik-0.6.9/tests/test_reader.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 blik-0.6.9/tests/test_widget.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 blik-0.6.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 blik-0.6.9/LICENSE
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 blik-0.6.9/README.md
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 blik-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 blik-0.6.9/PKG-INFO
```

### Comparing `blik-0.6.8/.cruft.json` & `blik-0.6.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/.pre-commit-config.yaml` & `blik-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/.github/workflows/ci.yml` & `blik-0.6.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/docs/_config.yml` & `blik-0.6.9/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/docs/getting_started.md` & `blik-0.6.9/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/docs/images/favicon.ico` & `blik-0.6.9/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/docs/images/logo.png` & `blik-0.6.9/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/docs/images/logo.svg` & `blik-0.6.9/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/napari.yaml` & `blik-0.6.9/src/blik/napari.yaml`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/reader.py` & `blik-0.6.9/src/blik/reader.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/utils.py` & `blik-0.6.9/src/blik/utils.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/writer.py` & `blik-0.6.9/src/blik/writer.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/widgets/file_reader.py` & `blik-0.6.9/src/blik/widgets/file_reader.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/widgets/filter.py` & `blik-0.6.9/src/blik/widgets/filter.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/widgets/main_widget.py` & `blik-0.6.9/src/blik/widgets/main_widget.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/widgets/picking.py` & `blik-0.6.9/src/blik/widgets/picking.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/src/blik/widgets/power_spectrum.py` & `blik-0.6.9/src/blik/widgets/power_spectrum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING
 
 import dask.array as da
 import numpy as np
 from magicgui import magic_factory
-from scipy.fft import fftn, fftshift
+from scipy.fft import fftn, fftshift, ifftshift
 
 if TYPE_CHECKING:
     import napari
 
 
 @magic_factory(
     auto_call=False,
@@ -20,14 +20,14 @@
     Power spectrum (log scale) of the image.
 
     First centers in real space on the origin to remove shift effects.
     """
     axes = (1, 2) if image.metadata["stack"] else None
     raw = da.compute(image.data)[0]
     power_spectrum = np.abs(
-        fftshift(fftn(fftshift(raw, axes=axes), axes=axes), axes=axes)
+        fftshift(fftn(ifftshift(raw, axes=axes), axes=axes), axes=axes)
     )
     return (
         np.log(power_spectrum + 1),
         {"name": f"{image.name} - power spectrum", "scale": image.scale},
         "image",
     )
```

### Comparing `blik-0.6.8/tests/conftest.py` & `blik-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/tests/test_reader.py` & `blik-0.6.9/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/tests/test_widget.py` & `blik-0.6.9/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/.gitignore` & `blik-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/LICENSE` & `blik-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/README.md` & `blik-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/pyproject.toml` & `blik-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blik-0.6.8/PKG-INFO` & `blik-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blik
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python tool for visualising and interacting with cryo-ET and subtomogram averaging data.
 Project-URL: homepage, https://github.com/brisvag/blik
 Project-URL: repository, https://github.com/brisvag/blik
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GPLv3
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

