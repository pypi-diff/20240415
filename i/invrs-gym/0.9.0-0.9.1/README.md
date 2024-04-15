# Comparing `tmp/invrs_gym-0.9.0.tar.gz` & `tmp/invrs_gym-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invrs_gym-0.9.0.tar", last modified: Wed Feb 21 00:16:11 2024, max compression
+gzip compressed data, was "invrs_gym-0.9.1.tar", last modified: Fri Feb 23 04:11:23 2024, max compression
```

## Comparing `invrs_gym-0.9.0.tar` & `invrs_gym-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.587384 invrs_gym-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-02-21 00:16:11.587384 invrs_gym-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 00:16:11.587384 invrs_gym-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.579384 invrs_gym-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.579384 invrs_gym-0.9.0/src/invrs_gym/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/challenges/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26614 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19852 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/metagrating_challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/splitter_challenge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21428 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/polarization_challenge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/loss/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/loss/transmission_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/utils/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-21 00:15:58.000000 invrs_gym-0.9.0/src/invrs_gym/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:16:11.583384 invrs_gym-0.9.0/src/invrs_gym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-02-21 00:16:11.000000 invrs_gym-0.9.0/src/invrs_gym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-21 00:16:11.000000 invrs_gym-0.9.0/src/invrs_gym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 00:16:11.000000 invrs_gym-0.9.0/src/invrs_gym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-21 00:16:11.000000 invrs_gym-0.9.0/src/invrs_gym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-21 00:16:11.000000 invrs_gym-0.9.0/src/invrs_gym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.443377 invrs_gym-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-02-23 04:11:23.443377 invrs_gym-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 04:11:23.443377 invrs_gym-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.435377 invrs_gym-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.435377 invrs_gym-0.9.1/src/invrs_gym/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/challenges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26725 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/metagrating_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/splitter_challenge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21428 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/polarization_challenge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.439377 invrs_gym-0.9.1/src/invrs_gym/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/loss/transmission_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.443377 invrs_gym-0.9.1/src/invrs_gym/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/utils/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-23 04:11:04.000000 invrs_gym-0.9.1/src/invrs_gym/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 04:11:23.443377 invrs_gym-0.9.1/src/invrs_gym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-02-23 04:11:23.000000 invrs_gym-0.9.1/src/invrs_gym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-23 04:11:23.000000 invrs_gym-0.9.1/src/invrs_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 04:11:23.000000 invrs_gym-0.9.1/src/invrs_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-23 04:11:23.000000 invrs_gym-0.9.1/src/invrs_gym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-23 04:11:23.000000 invrs_gym-0.9.1/src/invrs_gym.egg-info/top_level.txt
```

### Comparing `invrs_gym-0.9.0/LICENSE` & `invrs_gym-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/PKG-INFO` & `invrs_gym-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_gym
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of inverse design challenges
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -51,15 +51,15 @@
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: invrs_gym[examples,tests]; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-gym - A collection of inverse design challenges
-`v0.9.0`
+`v0.9.1`
 
 ## Overview
 The `invrs_gym` package is an open-source gym containing a diverse set of photonic design challenges, which are relevant for a wide range of applications such as AR/VR, optical networking, LIDAR, and others.
 
 Each of the challenges consists of a high-dimensional problem in which a physical structure (the photonic device) is optimized. The structure includes typically >10,000 degrees of freedom (DoF), generally including one or more arrays representing the structure or patterning of a layer, and may also include scalar variables representing e.g. layer thickness. In general, the DoF must satisfy certain constraints to be physical: thicknesses must be positive, and layer patterns must be _manufacturable_---they must not include features that are too small, or too closely spaced.
 
 In general, we seek optimization techniques that _reliably_ produce manufacturable, high-quality solutions and require reasonable compute resources. Among the techniques that could be applied are topology optimization, inverse design, and AI-guided design.
```

### Comparing `invrs_gym-0.9.0/README.md` & `invrs_gym-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # invrs-gym - A collection of inverse design challenges
-`v0.9.0`
+`v0.9.1`
 
 ## Overview
 The `invrs_gym` package is an open-source gym containing a diverse set of photonic design challenges, which are relevant for a wide range of applications such as AR/VR, optical networking, LIDAR, and others.
 
 Each of the challenges consists of a high-dimensional problem in which a physical structure (the photonic device) is optimized. The structure includes typically >10,000 degrees of freedom (DoF), generally including one or more arrays representing the structure or patterning of a layer, and may also include scalar variables representing e.g. layer thickness. In general, the DoF must satisfy certain constraints to be physical: thicknesses must be positive, and layer patterns must be _manufacturable_---they must not include features that are too small, or too closely spaced.
 
 In general, we seek optimization techniques that _reliably_ produce manufacturable, high-quality solutions and require reasonable compute resources. Among the techniques that could be applied are topology optimization, inverse design, and AI-guided design.
```

### Comparing `invrs_gym-0.9.0/pyproject.toml` & `invrs_gym-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "invrs_gym"
-version = "v0.9.0"
+version = "v0.9.1"
 description = "A collection of inverse design challenges"
 keywords = ["topology", "optimization", "jax", "inverse design"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
```

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/__init__.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/__init__.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/base.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/base.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/challenge.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 Copyright (c) 2023 The INVRS-IO authors.
 """
 
 import dataclasses
 import functools
 from typing import Any, Optional, Sequence, Tuple
 
-import agjax  # type: ignore[import-untyped]
 import ceviche_challenges as cc  # type: ignore[import-untyped]
 import ceviche_challenges.wdm.model as wdm_model  # type: ignore[import-untyped]
 import jax
 import jax.numpy as jnp
 import numpy as onp
+from agjax.experimental import wrapper
 from ceviche_challenges import units as u  # type: ignore[import-untyped]
 from jax import tree_util
 from totypes import json_utils, types
 
 from invrs_gym import utils
 from invrs_gym.challenges import base
 from invrs_gym.challenges.ceviche import defaults
@@ -77,44 +77,48 @@
         *,
         excite_port_idxs: Sequence[int] = (0,),
         wavelengths_nm: Optional[jnp.ndarray] = None,
         max_parallelizm: Optional[int] = None,
     ) -> Tuple["CevicheResponse", base.AuxDict]:
         """Compute the response of the component and auxilliary quantities."""
 
-        if wavelengths_nm is None:
-            wavelengths_nm = jnp.asarray(self.ceviche_model.output_wavelengths)
+        with jax.ensure_compile_time_eval():
+            if wavelengths_nm is None:
+                wavelengths_nm = jnp.asarray(self.ceviche_model.output_wavelengths)
 
         # The ceviche simulation function is autograd-differentiable. Wrap it so that
         # it can be differentiated using jax.
+        autograd_sim_fn = functools.partial(
+            self.ceviche_model.simulate,
+            excite_port_idxs=excite_port_idxs,
+            wavelengths_nm=wavelengths_nm,
+            max_parallelizm=max_parallelizm,
+        )
 
-        @functools.partial(
-            agjax.wrap_for_jax,
-            nondiff_argnums=(1, 2, 3),
+        s_params_shape = (
+            len(wavelengths_nm),
+            len(excite_port_idxs),
+            len(self.ceviche_model.ports),
+        )
+        fields_shape = s_params_shape[:2] + self.ceviche_model.shape
+        sim_fn = wrapper.wrap_for_jax(
+            autograd_sim_fn,
+            result_shape_dtypes=(
+                jnp.ones(s_params_shape, dtype=complex),
+                jnp.ones(fields_shape, dtype=complex),
+            ),
             nondiff_outputnums=(1,),
         )
-        def sim_fn(
-            design_variable: jnp.ndarray,
-            excite_port_idxs: Sequence[int],
-            wavelengths_nm: jnp.ndarray,
-            max_parallelizm: Optional[int],
-        ) -> Tuple[jnp.ndarray, onp.ndarray[Any, Any]]:
-            s_params, fields = self.ceviche_model.simulate(
-                design_variable, excite_port_idxs, wavelengths_nm, max_parallelizm
-            )
-            return s_params, fields
 
         density_array = utils.transforms.rescaled_density_array(
             params,
             lower_bound=DENSITY_LOWER_BOUND,
             upper_bound=DENSITY_UPPER_BOUND,
         )
-        sparams, fields = sim_fn(
-            density_array, excite_port_idxs, wavelengths_nm, max_parallelizm
-        )
+        sparams, fields = sim_fn(density_array)
         response = CevicheResponse(
             s_parameters=sparams,
             wavelengths_nm=wavelengths_nm,
             excite_port_idxs=jnp.asarray(excite_port_idxs),
         )
         aux = {SPARAMS: sparams, FIELDS: fields}
         return response, aux
```

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/ceviche/defaults.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/ceviche/defaults.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/common.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,16 @@
         jnp.full((1, 1), spec.permittivity_substrate),
     )
 
     in_plane_wavevector = basis.plane_wave_in_plane_wavevector(
         wavelength=wavelength,
         polar_angle=polar_angle,
         azimuthal_angle=azimuthal_angle,
-        permittivity=jnp.asarray(spec.permittivity_ambient),
+        # Polar angle is defined in substrate, since light is incident from substrate.
+        permittivity=jnp.asarray(spec.permittivity_substrate),
     )
     layer_solve_results = [
         fmm.eigensolve_isotropic_media(
             wavelength=jnp.asarray(wavelength),
             in_plane_wavevector=in_plane_wavevector,
             primitive_lattice_vectors=basis.LatticeVectors(
                 u=spec.period_x * basis.X,
```

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/metagrating_challenge.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/metagrating_challenge.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/diffract/splitter_challenge.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/diffract/splitter_challenge.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/challenge.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/challenge.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/extractor/component.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/extractor/component.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/common.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/common.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/challenges/sorter/polarization_challenge.py` & `invrs_gym-0.9.1/src/invrs_gym/challenges/sorter/polarization_challenge.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/loss/transmission_loss.py` & `invrs_gym-0.9.1/src/invrs_gym/loss/transmission_loss.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/utils/initializers.py` & `invrs_gym-0.9.1/src/invrs_gym/utils/initializers.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/utils/metrics.py` & `invrs_gym-0.9.1/src/invrs_gym/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym/utils/transforms.py` & `invrs_gym-0.9.1/src/invrs_gym/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `invrs_gym-0.9.0/src/invrs_gym.egg-info/PKG-INFO` & `invrs_gym-0.9.1/src/invrs_gym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invrs_gym
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of inverse design challenges
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -51,15 +51,15 @@
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: invrs_gym[examples,tests]; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # invrs-gym - A collection of inverse design challenges
-`v0.9.0`
+`v0.9.1`
 
 ## Overview
 The `invrs_gym` package is an open-source gym containing a diverse set of photonic design challenges, which are relevant for a wide range of applications such as AR/VR, optical networking, LIDAR, and others.
 
 Each of the challenges consists of a high-dimensional problem in which a physical structure (the photonic device) is optimized. The structure includes typically >10,000 degrees of freedom (DoF), generally including one or more arrays representing the structure or patterning of a layer, and may also include scalar variables representing e.g. layer thickness. In general, the DoF must satisfy certain constraints to be physical: thicknesses must be positive, and layer patterns must be _manufacturable_---they must not include features that are too small, or too closely spaced.
 
 In general, we seek optimization techniques that _reliably_ produce manufacturable, high-quality solutions and require reasonable compute resources. Among the techniques that could be applied are topology optimization, inverse design, and AI-guided design.
```

### Comparing `invrs_gym-0.9.0/src/invrs_gym.egg-info/SOURCES.txt` & `invrs_gym-0.9.1/src/invrs_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

