# Comparing `tmp/pyblindrl-0.0.2rc59.post1.tar.gz` & `tmp/pyblindrl-0.0.2rc60.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblindrl-0.0.2rc59.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyblindrl-0.0.2rc60.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyblindrl-0.0.2rc59.post1.tar` & `pyblindrl-0.0.2rc60.post1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0      340 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      418 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1137 2024-04-15 18:13:22.500555 pyblindrl-0.0.2rc59.post1/LICENSE
--rw-r--r--   0        0        0      458 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/Makefile
--rw-r--r--   0        0        0     2320 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/developer.md
--rw-r--r--   0        0        0      461 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/make.bat
--rw-r--r--   0        0        0       57 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/pyproject.md
--rw-r--r--   0        0        0      437 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      406 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/docs/workflows.md
--rw-r--r--   0        0        0     6567 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/pyproject.toml
--rw-r--r--   0        0        0       44 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/src/README.md
--rw-r--r--   0        0        0     5149 2024-04-15 18:13:35.084567 pyblindrl-0.0.2rc59.post1/src/pyBlindRL/__init__.py
--rw-r--r--   0        0        0      584 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/src/pyBlindRL/hello_world.py
--rw-r--r--   0        0        0      989 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/tests/conftest.py
--rw-r--r--   0        0        0     1212 2024-04-15 18:13:22.504555 pyblindrl-0.0.2rc59.post1/tests/test_methods.py
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 pyblindrl-0.0.2rc59.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      418 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1137 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/LICENSE
+-rw-r--r--   0        0        0      458 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/Makefile
+-rw-r--r--   0        0        0     2320 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/developer.md
+-rw-r--r--   0        0        0      461 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/make.bat
+-rw-r--r--   0        0        0       57 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      437 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      406 2024-04-15 19:01:36.707600 pyblindrl-0.0.2rc60.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6567 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/src/README.md
+-rw-r--r--   0        0        0     6360 2024-04-15 19:01:53.065400 pyblindrl-0.0.2rc60.post1/src/pyBlindRL/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/tests/conftest.py
+-rw-r--r--   0        0        0      501 2024-04-15 19:01:36.711600 pyblindrl-0.0.2rc60.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 pyblindrl-0.0.2rc60.post1/PKG-INFO
```

### Comparing `pyblindrl-0.0.2rc59.post1/.devcontainer/devcontainer.json` & `pyblindrl-0.0.2rc60.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/.github/workflows/schedule-update-actions.yml` & `pyblindrl-0.0.2rc60.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/.gitignore` & `pyblindrl-0.0.2rc60.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/.pre-commit-config.yaml` & `pyblindrl-0.0.2rc60.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/.vscode/settings.json` & `pyblindrl-0.0.2rc60.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/LICENSE` & `pyblindrl-0.0.2rc60.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/docs/Makefile` & `pyblindrl-0.0.2rc60.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/docs/conf.py` & `pyblindrl-0.0.2rc60.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/docs/make.bat` & `pyblindrl-0.0.2rc60.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/docs/pylint.md` & `pyblindrl-0.0.2rc60.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/pyproject.toml` & `pyblindrl-0.0.2rc60.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/src/pyBlindRL/__init__.py` & `pyblindrl-0.0.2rc60.post1/src/pyBlindRL/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   -------------------------------------------------------------
 """A Python implementation of blind Richardson-Lucy deconvolution"""
 from __future__ import annotations
 
 import numpy as np
 import torch
 
-__version__ = "0.0.2""-rc59-post1"
+__version__ = "0.0.2""-rc60-post1"
 
 
 def gaussian_3d(shape, center=None, sigma=None):
     """
     Generate a 3D Gaussian array.
 
     Parameters:
@@ -36,32 +36,78 @@
     gaussian_array -= gaussian_array.min()
     gaussian_array /= gaussian_array.max()
 
     return gaussian_array
 
 
 def generate_initial_psf(img):
+    """
+    Creates a PSF image based on a Gaussian centered on the corners
+
+    Parameters:
+        img (3d numpy array): Image to use as a template
+    """
     out = np.zeros_like(img, dtype=np.complex128)
     out += 1
 
     psf = gaussian_3d(shape, sigma=(1, 1, 2))
 
-    otf[
+    out[
         int(img.shape[0] / 2 - psf.shape[0] / 2) :,
         int(img.shape[1] / 2 - psf.shape[1] / 2) :,
         int(img.shape[2] / 2 - psf.shape[2] / 2) :,
     ][: psf.shape[0], : psf.shape[1], : psf.shape[2]] += psf
 
+    out = roll_psf(out)
+
+    return out
+    # return np.fft.fftn(out)
+
+
+def roll_psf(img):
+    """
+    Roll PSF at center of image to edge of image.
+
+    Parameters:
+        img (3d numpy array): Image to roll
+    """
+
+    for axis, axis_size in enumerate(img.shape):
+        img = np.roll(img, -int(axis_size / 2), axis=axis)
+
+    return img
+
+
+def unroll_psf(img):
+    """
+    Move PSF aligned with corners and roll to center.
+
+    Parameters:
+        img (3d numpy array): Image to unroll
+    """
+
     for axis, axis_size in enumerate(img.shape):
-        otf = np.roll(otf, -int(axis_size / 2), axis=axis)
+        img = np.roll(img, int(axis_size / 2), axis=axis)
 
-    return np.fft.fftn(otf)
+    return img
 
 
-def RL_deconv(image, otf, iterations, target_device="cpu", eps=1e-10):
+def RL_deconv(image, otf, iterations, target_device="cpu", eps=1e-10, approx=True):
+    """
+    Perform unblinded RL deconvolution
+
+    Parameters:
+        img (3d numpy array): Image to deconvolute
+        otf (3d numpy array): OTF to deconvolute with
+        iterations (int): number of iterations to perform
+        target_device (str): torch device to creat output on
+        eps (float): value added to prevent zero-division error
+        approx (bool): flag to enable fast approximation optimizations
+    """
+
     with torch.no_grad():
         out = torch.clone(image).detach().to(target_device)
 
         depth, height, width = out.shape
         window = 25
         masks = [
             (slice(0, window), slice(0, window), slice(0, window)),  # Top left corner
@@ -81,17 +127,19 @@
                 slice(width - window, width),
             ),  # Front bottom right corner
         ]
 
         for _ in range(iterations):
             tmp = torch.fft.fftn(out)
 
-            # tmp *= otf
-            for mask in masks:
-                tmp[mask] *= otf[mask]
+            if approx:
+                for mask in masks:
+                    tmp[mask] *= otf[mask]
+            else:
+                tmp *= otf
 
             tmp = torch.fft.ifftn(tmp)
 
             tmp += eps  # prevent 0-division
             tmp = image / tmp
 
             tmp = torch.fft.fftn(tmp)
@@ -101,18 +149,22 @@
             tmp = torch.fft.ifftn(tmp)
 
             out *= tmp
 
         return out
 
 
-def RL_deconv_otf(image, otf, iterations, rl_iter=10, target_device="cpu"):
+def RL_deconv_otf(image, psf, iterations, rl_iter=10, target_device="cpu"):
+    """
+    Perform Blinded RL deconvolution
+    """
+
     with torch.no_grad():
         out = torch.clone(image).detach().to(target_device)
-        out_psf = torch.clone(otf).detach().to(target_device)
+        out_psf = torch.clone(psf).detach().to(target_device)
 
         for _bld in tqdm.trange(iterations):
             out = torch.fft.fftn(out)
             for _ in range(rl_iter):
                 tmp = torch.fft.fftn(out_psf)
                 tmp *= out
                 tmp = torch.fft.ifftn(tmp)
@@ -137,15 +189,15 @@
                 tmp = image / tmp
 
                 tmp = torch.fft.fftn(tmp)
                 tmp *= out_psf.conj()
                 tmp = torch.fft.ifftn(tmp)
 
                 out *= tmp
-                out += 0.01 * image
+                #                out += 0.01 * image
 
                 del tmp
             out_psf = torch.fft.ifftn(out_psf)
 
         oout = torch.abs(out).to("cpu").numpy().astype(float)
         oout_psf = torch.abs(out_psf).to("cpu").numpy().astype(float)
```

### Comparing `pyblindrl-0.0.2rc59.post1/tests/conftest.py` & `pyblindrl-0.0.2rc60.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyblindrl-0.0.2rc59.post1/PKG-INFO` & `pyblindrl-0.0.2rc60.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBlindRL
-Version: 0.0.2rc59.post1
+Version: 0.0.2rc60.post1
 Summary: A Python implementation of blind Richardson-Lucy deconvolution
 Author-email: "Logan Walker, PhD" <loganaw@umich.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

