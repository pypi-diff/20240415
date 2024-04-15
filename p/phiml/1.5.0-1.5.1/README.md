# Comparing `tmp/phiml-1.5.0.tar.gz` & `tmp/phiml-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\phiml-1.5.0.tar", last modified: Sun Mar 31 16:36:10 2024, max compression
+gzip compressed data, was "phiml-1.5.1.tar", last modified: Mon Apr 15 12:12:14 2024, max compression
```

## Comparing `phiml-1.5.0.tar` & `phiml-1.5.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.300458 phiml-1.5.0/
--rw-rw-rw-   0        0        0      107 2023-08-21 09:31:32.000000 phiml-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4553 2024-03-31 16:36:10.301459 phiml-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    12731 2024-03-31 11:05:03.000000 phiml-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.252415 phiml-1.5.0/phiml/
--rw-rw-rw-   0        0        0        5 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/VERSION
--rw-rw-rw-   0        0        0     1084 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/__init__.py
--rw-rw-rw-   0        0        0    11653 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/_troubleshoot.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.270430 phiml-1.5.0/phiml/backend/
--rw-rw-rw-   0        0        0     1117 2024-02-08 17:17:17.000000 phiml-1.5.0/phiml/backend/__init__.py
--rw-rw-rw-   0        0        0    76411 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/_backend.py
--rw-rw-rw-   0        0        0     6187 2024-02-08 17:17:17.000000 phiml-1.5.0/phiml/backend/_dtype.py
--rw-rw-rw-   0        0        0    39515 2024-02-08 17:17:17.000000 phiml-1.5.0/phiml/backend/_linalg.py
--rw-rw-rw-   0        0        0     3101 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/_linalg_preconditioner.py
--rw-rw-rw-   0        0        0    11461 2024-02-08 17:17:17.000000 phiml-1.5.0/phiml/backend/_minimize.py
--rw-rw-rw-   0        0        0    22389 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/_numpy_backend.py
--rw-rw-rw-   0        0        0     1403 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/backend/_object.py
--rw-rw-rw-   0        0        0    19229 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/_partition.py
--rw-rw-rw-   0        0        0    22494 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/_profile.py
--rw-rw-rw-   0        0        0      449 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/_triangular_wip.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.274435 phiml-1.5.0/phiml/backend/jax/
--rw-rw-rw-   0        0        0      163 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/jax/__init__.py
--rw-rw-rw-   0        0        0    26700 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/jax/_jax_backend.py
--rw-rw-rw-   0        0        0    39851 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/jax/stax_nets.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.281441 phiml-1.5.0/phiml/backend/tensorflow/
--rw-rw-rw-   0        0        0      891 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/tensorflow/__init__.py
--rw-rw-rw-   0        0        0     4228 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/tensorflow/_compile_cuda.py
--rw-rw-rw-   0        0        0     1950 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/tensorflow/_profiling.py
--rw-rw-rw-   0        0        0    36969 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/tensorflow/_tf_backend.py
--rw-rw-rw-   0        0        0     3280 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/tensorflow/_tf_cuda_resample.py
--rw-rw-rw-   0        0        0    25715 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/tensorflow/nets.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.284444 phiml-1.5.0/phiml/backend/torch/
--rw-rw-rw-   0        0        0      224 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/backend/torch/__init__.py
--rw-rw-rw-   0        0        0    63322 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/torch/_torch_backend.py
--rw-rw-rw-   0        0        0    30154 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/backend/torch/nets.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.299458 phiml-1.5.0/phiml/math/
--rw-rw-rw-   0        0        0     5461 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/math/__init__.py
--rw-rw-rw-   0        0        0     3777 2023-08-21 09:31:32.000000 phiml-1.5.0/phiml/math/_fit.py
--rw-rw-rw-   0        0        0    65458 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/_functional.py
--rw-rw-rw-   0        0        0    42408 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/_magic_ops.py
--rw-rw-rw-   0        0        0    46493 2024-02-08 17:17:17.000000 phiml-1.5.0/phiml/math/_nd.py
--rw-rw-rw-   0        0        0   150783 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/math/_ops.py
--rw-rw-rw-   0        0        0    48645 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/_optimize.py
--rw-rw-rw-   0        0        0    83888 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/math/_shape.py
--rw-rw-rw-   0        0        0    75958 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/math/_sparse.py
--rw-rw-rw-   0        0        0   112899 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/_tensors.py
--rw-rw-rw-   0        0        0    43689 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/_trace.py
--rw-rw-rw-   0        0        0    71701 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/math/extrapolation.py
--rw-rw-rw-   0        0        0    33748 2024-03-31 11:05:03.000000 phiml-1.5.0/phiml/math/magic.py
--rw-rw-rw-   0        0        0    12852 2024-03-31 11:05:04.000000 phiml-1.5.0/phiml/nn.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:36:10.257419 phiml-1.5.0/phiml.egg-info/
--rw-rw-rw-   0        0        0     4553 2024-03-31 16:36:10.000000 phiml-1.5.0/phiml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-03-31 16:36:10.000000 phiml-1.5.0/phiml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:36:10.000000 phiml-1.5.0/phiml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-03-31 16:36:10.000000 phiml-1.5.0/phiml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 16:36:10.000000 phiml-1.5.0/phiml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-31 16:36:10.301459 phiml-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     6904 2023-08-21 09:31:32.000000 phiml-1.5.0/setup.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.464767 phiml-1.5.1/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1085 2023-09-29 11:02:38.000000 phiml-1.5.1/LICENSE.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)      107 2023-08-31 12:58:16.000000 phiml-1.5.1/MANIFEST.in
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4083 2024-04-15 12:12:14.464767 phiml-1.5.1/PKG-INFO
+-rw-rw-r--   0 holl      (1001) holl      (1001)    12731 2024-03-04 10:04:22.000000 phiml-1.5.1/README.md
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml/
+-rw-rw-r--   0 holl      (1001) holl      (1001)        5 2024-04-15 12:10:41.000000 phiml-1.5.1/phiml/VERSION
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1084 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    11684 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/_troubleshoot.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml/backend/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1117 2023-11-28 11:26:43.000000 phiml-1.5.1/phiml/backend/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    76402 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/backend/_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     6187 2023-10-27 10:58:55.000000 phiml-1.5.1/phiml/backend/_dtype.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    39515 2024-01-11 08:57:24.000000 phiml-1.5.1/phiml/backend/_linalg.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3101 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/_linalg_preconditioner.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    11461 2024-02-02 10:09:48.000000 phiml-1.5.1/phiml/backend/_minimize.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    22415 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/backend/_numpy_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1403 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/backend/_object.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    19229 2024-04-15 12:09:41.000000 phiml-1.5.1/phiml/backend/_partition.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    22494 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/_profile.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)      449 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/_triangular_wip.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml/backend/jax/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      163 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/jax/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    26700 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/backend/jax/_jax_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    39851 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/backend/jax/stax_nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml/backend/tensorflow/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      891 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/tensorflow/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4228 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/tensorflow/_compile_cuda.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1950 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/tensorflow/_profiling.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    37006 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/backend/tensorflow/_tf_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3280 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/tensorflow/_tf_cuda_resample.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    25715 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/backend/tensorflow/nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml/backend/torch/
+-rw-rw-r--   0 holl      (1001) holl      (1001)      224 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/backend/torch/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    63573 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/backend/torch/_torch_backend.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    30154 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/backend/torch/nets.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.464767 phiml-1.5.1/phiml/math/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     5507 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/math/__init__.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)     3777 2023-08-31 12:58:16.000000 phiml-1.5.1/phiml/math/_fit.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    65520 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/math/_functional.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    42781 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/math/_magic_ops.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    46493 2024-02-12 11:26:53.000000 phiml-1.5.1/phiml/math/_nd.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)   150830 2024-04-15 12:09:48.000000 phiml-1.5.1/phiml/math/_ops.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    48969 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/math/_optimize.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    83888 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/math/_shape.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    77746 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/math/_sparse.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)   111869 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/math/_tensors.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    45142 2024-04-15 10:15:30.000000 phiml-1.5.1/phiml/math/_trace.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    71711 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/math/extrapolation.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    33748 2024-03-25 12:45:26.000000 phiml-1.5.1/phiml/math/magic.py
+-rw-rw-r--   0 holl      (1001) holl      (1001)    12852 2024-04-04 10:58:44.000000 phiml-1.5.1/phiml/nn.py
+drwxrwxr-x   0 holl      (1001) holl      (1001)        0 2024-04-15 12:12:14.460767 phiml-1.5.1/phiml.egg-info/
+-rw-rw-r--   0 holl      (1001) holl      (1001)     4083 2024-04-15 12:12:14.000000 phiml-1.5.1/phiml.egg-info/PKG-INFO
+-rw-rw-r--   0 holl      (1001) holl      (1001)     1294 2024-04-15 12:12:14.000000 phiml-1.5.1/phiml.egg-info/SOURCES.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)        1 2024-04-15 12:12:14.000000 phiml-1.5.1/phiml.egg-info/dependency_links.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)       29 2024-04-15 12:12:14.000000 phiml-1.5.1/phiml.egg-info/requires.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)        6 2024-04-15 12:12:14.000000 phiml-1.5.1/phiml.egg-info/top_level.txt
+-rw-rw-r--   0 holl      (1001) holl      (1001)       79 2024-04-15 12:12:14.464767 phiml-1.5.1/setup.cfg
+-rw-rw-r--   0 holl      (1001) holl      (1001)     6904 2023-08-31 12:58:16.000000 phiml-1.5.1/setup.py
```

### Comparing `phiml-1.5.0/README.md` & `phiml-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/__init__.py` & `phiml-1.5.1/phiml/__init__.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/_troubleshoot.py` & `phiml-1.5.1/phiml/_troubleshoot.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,31 +195,31 @@
     from .math._tensors import NativeTensor, TensorStack
     for obj in gc.get_objects():
         if isinstance(obj, NativeTensor):
             if obj._shape != obj._native_shape:
                 if print is not None:
                     print(f"Expanding tensor with shape {obj._shape} from {obj._native_shape} {type(obj._native).__name__} {obj._native}")
                 try:
-                    obj._cache()
+                    obj._contiguous()
                 except BaseException as exc:
                     print(f"ERROR    Expansion failed. {exc}")
                     path = find_variable_reference(obj)
                     print(f"Reference path to tensor: {path}")
                     if hasattr(obj, '_init_stack'):
                         print("Tensor creation stack trace:")
                         for frame in obj._init_stack:
                             filename, line_number, function_name, line = frame
                             print(f"{filename}:{line_number} ({function_name})    {line}")
                     else:
                         print("Enable debug checks to obtain the stack trace for the Tensor's creation.")
         elif isinstance(obj, TensorStack):
             if obj._cached is None and not obj.requires_broadcast:
                 if print is not None:
-                    print(f"Caching tensor stack with shape {obj._shape} from along {obj._stack_dim}")
-                obj._cache()
+                    print(f"Caching tensor stack with shape {obj._shape} along {obj._stack_dim}. Contents: {obj._tensors}")
+                obj._contiguous()
 
 
 def find_variable_reference(obj):
     gc.collect()
     existing_ids = set(id(o) for o in gc.get_objects())
     indexed = set()
     return _find_variable_reference(obj, existing_ids, indexed)[0]
```

### Comparing `phiml-1.5.0/phiml/backend/__init__.py` & `phiml-1.5.1/phiml/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_backend.py` & `phiml-1.5.1/phiml/backend/_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -854,15 +854,15 @@
         """
         Args:
             multi_index: (batch..., index_dim)
             shape: 1D tensor or tuple/list
             mode: `'undefined'`, `'periodic'`, `'clamp'` or an `int` to use for all invalid indices.
 
         Returns:
-            Integer tensor of shape (batch...)
+            Integer tensor of shape (batch...) of same dtype as `multi_index`.
         """
         strides = [self.ones((), self.dtype(multi_index))]
         for size in reversed(shape[1:]):
             strides.append(strides[-1] * size)
         strides = self.stack(strides[::-1])
         if mode == 'periodic':
             multi_index %= self.as_tensor(shape)
@@ -1265,18 +1265,17 @@
         """
         values, dense = self.auto_cast(values, dense)
         batch_size, nnz, channel_count = self.staticshape(values)
         batch_size_d, dense_rows, channel_count_d, dense_cols = self.staticshape(dense)
         assert batch_size_d == batch_size
         assert dense_rows == shape[1]
         assert channel_count == channel_count_d
-        assert dense_cols == 1  # not implemented yet
         dense_formatted = self.reshape(dense, (batch_size, dense_rows, channel_count * dense_cols))
         dense_gathered = self.batched_gather_nd(dense_formatted, indices[:, :, 1:2])
-        base_grid = self.zeros((batch_size, shape[0], channel_count), self.dtype(dense))
+        base_grid = self.zeros((batch_size, shape[0], channel_count * dense_cols), self.dtype(dense))
         result = self.scatter(base_grid, indices[:, :, 0:1], values * dense_gathered, mode='add')
         return self.reshape(result, (batch_size, shape[0], channel_count, dense_cols))
 
     def coo_to_dense(self, indices, values, shape, contains_duplicates: bool):
         batch_size, nnz, channel_count = self.staticshape(values)
         base = self.zeros((batch_size, *shape, channel_count), dtype=self.dtype(values))
         result = self.scatter(base, indices, values, mode='add' if contains_duplicates else 'update')
```

### Comparing `phiml-1.5.0/phiml/backend/_dtype.py` & `phiml-1.5.1/phiml/backend/_dtype.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_linalg.py` & `phiml-1.5.1/phiml/backend/_linalg.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_linalg_preconditioner.py` & `phiml-1.5.1/phiml/backend/_linalg_preconditioner.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_minimize.py` & `phiml-1.5.1/phiml/backend/_minimize.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_numpy_backend.py` & `phiml-1.5.1/phiml/backend/_numpy_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 
     def unravel_index(self, flat_index, shape):
         return np.stack(np.unravel_index(flat_index, shape), -1)
 
     def ravel_multi_index(self, multi_index, shape, mode: Union[str, int] = 'undefined'):
         mode = mode if isinstance(mode, int) else {'undefined': 'raise', 'periodic': 'wrap', 'clamp': 'clip'}[mode]
         idx_first = np.transpose(multi_index, (-1,) + tuple(range(self.ndims(multi_index)-1)))
-        result = np.ravel_multi_index(idx_first, shape, mode='wrap' if isinstance(mode, int) else mode)
+        result = np.ravel_multi_index(idx_first, shape, mode='wrap' if isinstance(mode, int) else mode).astype(multi_index.dtype)
         if isinstance(mode, int):
             outside = self.any((multi_index < 0) | (multi_index >= shape), -1)
             result = self.where(outside, mode, result)
         return result
 
     def gather(self, values, indices, axis: int):
         slices = [indices if i == axis else slice(None) for i in range(self.ndims(values))]
```

### Comparing `phiml-1.5.0/phiml/backend/_object.py` & `phiml-1.5.1/phiml/backend/_object.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_partition.py` & `phiml-1.5.1/phiml/backend/_partition.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/_profile.py` & `phiml-1.5.1/phiml/backend/_profile.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/jax/_jax_backend.py` & `phiml-1.5.1/phiml/backend/jax/_jax_backend.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/jax/stax_nets.py` & `phiml-1.5.1/phiml/backend/jax/stax_nets.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/__init__.py` & `phiml-1.5.1/phiml/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/_compile_cuda.py` & `phiml-1.5.1/phiml/backend/tensorflow/_compile_cuda.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/_profiling.py` & `phiml-1.5.1/phiml/backend/tensorflow/_profiling.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/_tf_backend.py` & `phiml-1.5.1/phiml/backend/tensorflow/_tf_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,14 +613,15 @@
             return hist
 
     def bincount(self, x, weights: Optional[TensorType], bins: int, x_sorted=False):
         # if x_sorted:
         #     return tf.math.segment_sum(weights or 1, x)
         # else:
         with self._device_for(x, weights):
+            x = tf.cast(x, tf.int32)
             return tf.math.bincount(x, weights=weights, minlength=bins, maxlength=bins)
 
     def unique(self, x: TensorType, return_inverse: bool, return_counts: bool, axis: int) -> Tuple[TensorType, ...]:
         with self.device_of(x):
             if self.ndims(x) > 1:
                 if return_counts:
                     raise NotImplementedError("TensorFlow multidimensional unique does not support counts")
```

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/_tf_cuda_resample.py` & `phiml-1.5.1/phiml/backend/tensorflow/_tf_cuda_resample.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/tensorflow/nets.py` & `phiml-1.5.1/phiml/backend/tensorflow/nets.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/backend/torch/_torch_backend.py` & `phiml-1.5.1/phiml/backend/torch/_torch_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -846,31 +846,32 @@
         #     raise NotImplementedError
         # else:
         #     # tile
         #     raise NotImplementedError
 
     def conjugate_gradient(self, lin, y, x0, rtol, atol, max_iter, pre) -> SolveResult:
         if callable(lin) or len(max_iter) > 1 or pre:
-            assert self.is_available(y), "Tracing conjugate_gradient with linear operator is not yet supported."
+            assert self.is_available(y), f"JIT-compiling conjugate_gradient with PyTorch is not yet supported for arbitrary functions. Build a matrix from the function '{lin}' first."
             return Backend.conjugate_gradient(self, lin, y, x0, rtol, atol, max_iter, pre)
-        assert isinstance(lin, torch.Tensor), "Batched matrices are not yet supported"
+        assert isinstance(lin, (torch.Tensor, np.ndarray)), "Batched matrices are not yet supported"
         batch_size = self.staticshape(y)[0]
         y = self.to_float(y)
         x0 = self.copy(self.to_float(x0))
         lin, y, x0 = self.auto_cast(lin, y, x0)
         rtol = self.as_tensor(rtol)
         atol = self.as_tensor(atol)
         tol_sq = self.maximum(rtol ** 2 * self.sum(y ** 2, -1), atol ** 2)
         max_iter = self.as_tensor(max_iter[0])
         x, residual, iterations, function_evaluations, converged, diverged = torch_sparse_cg(lin, y, x0, tol_sq, max_iter)
         return SolveResult(f"Φ-ML CG ({'PyTorch*' if self.is_available(y) else 'TorchScript'})", x, residual, iterations, function_evaluations, converged, diverged, [""] * batch_size)
 
     def conjugate_gradient_adaptive(self, lin, y, x0, rtol, atol, max_iter, pre) -> SolveResult:
         if callable(lin) or len(max_iter) > 1 or pre:
-            assert self.is_available(y), "Tracing conjugate_gradient with linear operator is not yet supported."
+            if not self.is_available(y):
+                warnings.warn(f"CG with preconditioners is not optimized for PyTorch and will always run the maximum number of iterations when JIT-compiled (max_iter={max_iter}).", RuntimeWarning)
             return Backend.conjugate_gradient_adaptive(self, lin, y, x0, rtol, atol, max_iter, pre)
         assert isinstance(lin, torch.Tensor), "Batched matrices are not yet supported"
         batch_size = self.staticshape(y)[0]
         y = self.to_float(y)
         x0 = self.copy(self.to_float(x0))
         lin, y, x0 = self.auto_cast(lin, y, x0)
         rtol = self.as_tensor(rtol)
@@ -878,15 +879,15 @@
         tol_sq = self.maximum(rtol ** 2 * self.sum(y ** 2, -1), atol ** 2)
         max_iter = self.as_tensor(max_iter[0])
         x, residual, iterations, function_evaluations, converged, diverged = torch_sparse_cg_adaptive(lin, y, x0, tol_sq, max_iter)
         return SolveResult(f"Φ-ML CG ({'PyTorch*' if self.is_available(y) else 'TorchScript'})", x, residual, iterations, function_evaluations, converged, diverged, [""] * batch_size)
 
     def bi_conjugate_gradient(self, lin, y, x0, rtol, atol, max_iter, pre, poly_order=2) -> SolveResult:
         if not self.is_available(y):
-            warnings.warn("Bi-CG is not optimized for PyTorch and will always run the maximum number of iterations.", RuntimeWarning)
+            warnings.warn(f"Bi-CG is not optimized for PyTorch and will always run the maximum number of iterations when JIT compiled (max_iter={max_iter}).", RuntimeWarning)
         return Backend.bi_conjugate_gradient(self, lin, y, x0, rtol, atol, max_iter, pre, poly_order)
 
     def matrix_solve_least_squares(self, matrix: TensorType, rhs: TensorType) -> Tuple[TensorType, TensorType, TensorType, TensorType]:
         assert version.parse(torch.__version__) >= version.parse('1.9.0'), "least squares requires PyTorch >= 1.9.0"
         matrix, rhs = self.auto_cast(matrix, rhs)
         solution, residuals, rank, singular_values = torch.linalg.lstsq(matrix, rhs)
         return solution, residuals, rank, singular_values
```

### Comparing `phiml-1.5.0/phiml/backend/torch/nets.py` & `phiml-1.5.1/phiml/backend/torch/nets.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/math/__init__.py` & `phiml-1.5.1/phiml/math/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     is_finite, is_nan, is_inf,
     closest_grid_values, grid_sample, scatter, gather,
     histogram,
     fft, ifft, convolve, cumulative_sum,
     dtype, cast,
     close, always_close, assert_close, equal,
     stop_gradient,
-    pairwise_distances, map_pairs,
+    pairwise_differences, pairwise_differences as pairwise_distances, map_pairs,
 )
 
 from ._nd import (
     shift, index_shift,
     vec, const_vec, vec_length, vec_squared, vec_normalize, cross_product, rotate_vector, rotation_matrix, rotation_angles, dim_mask,
     normalize_to,
     l1_loss, l2_loss, frequency_loss,
```

### Comparing `phiml-1.5.0/phiml/math/_fit.py` & `phiml-1.5.1/phiml/math/_fit.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/math/_functional.py` & `phiml-1.5.1/phiml/math/_functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 from functools import wraps, partial
 from typing import Tuple, Callable, Dict, Generic, List, TypeVar, Any, Set, Union, Optional
 
 import numpy as np
 
 from . import _ops as math, all_available, stop_gradient
-from ._magic_ops import stack, slice_, value_attributes
+from ._magic_ops import stack, slice_, value_attributes, find_differences
 from ._shape import EMPTY_SHAPE, Shape, spatial, instance, batch, channel, merge_shapes, DimFilter, shape
 from ._sparse import SparseCoordinateTensor
 from ._tensors import Tensor, disassemble_tree, assemble_tree, disassemble_tensors, assemble_tensors, variable_attributes, wrap, specs_equal, equality_by_shape_and_value, object_dims
 from ._trace import ShiftLinTracer, matrix_from_function, LinearTraceInProgress
 from .magic import PhiTreeNode, Shapable
 from ..backend import Backend
 from ..backend._backend import get_spatial_derivative_order, functional_derivative_evaluation, ML_LOGGER
@@ -45,15 +45,16 @@
 
     def __repr__(self):
         return f"{self.tree} with shapes {self.shapes}"
 
     def __eq__(self, other: 'SignatureKey'):
         assert isinstance(other, SignatureKey)
         with equality_by_shape_and_value():
-            cond_equal = self.auxiliary_kwargs == other.auxiliary_kwargs
+            diff = find_differences(self.auxiliary_kwargs, other.auxiliary_kwargs)
+            cond_equal = not diff
         if isinstance(cond_equal, Tensor):
             cond_equal = cond_equal.all
         # shapes need not be compared because they are included in specs
         specs = specs_equal(self.specs, other.specs)
         return self.tree == other.tree and specs and self.backend == other.backend and self.spatial_derivative_order == other.spatial_derivative_order and cond_equal
 
     def __hash__(self):
```

### Comparing `phiml-1.5.0/phiml/math/_magic_ops.py` & `phiml-1.5.1/phiml/math/_magic_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -832,15 +832,15 @@
         if compare_tensors_by_id:
             if a is not b:
                 result.append(("Tensor ids do not match", path, a, b))
         else:
             from ._ops import equal
             if a.shape != b.shape:
                 result.append(("Tensor shapes do not match", path, a, b))
-            elif not equal(a, b):
+            elif not equal(a, b, equal_nan=True):
                 result.append(("Tensor values do not match", path, a, b))
     elif type(a) != type(b):
         result.append(("Types do not match", path, a, b))
         return
     elif isinstance(a, (tuple, list)):
         if len(a) != len(b):
             result.append(("Lengths do not match", path, a, b))
@@ -861,12 +861,17 @@
         else:
             for k in a_attrs:
                 av = getattr(a, k)
                 bv = getattr(b, k)
                 _recursive_diff(av, bv, f"{path}.{k}", result, compare_tensors_by_id, attr_type)
     else:
         try:
-            b = choose_backend(a, b)
-            raise NotImplementedError
+            backend = choose_backend(a, b)
+            if backend.shape(a) != backend.shape(b):
+                result.append(("Native tensor shapes do not match", path, a, b))
+            equal_tensor = backend.equal(a, b) | (backend.isnan(a) & backend.isnan(b))
+            equal = backend.numpy(backend.all(equal_tensor))
+            if not equal:
+                result.append(("Native tensor values do not match", path, a, b))
         except NoBackendFound:
             if a != b:
                 result.append(("Values do not match", path, a, b))
```

### Comparing `phiml-1.5.0/phiml/math/_nd.py` & `phiml-1.5.1/phiml/math/_nd.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/math/_ops.py` & `phiml-1.5.1/phiml/math/_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
             If a sequence of dimensions is provided, only forces the expansion for groups containing those dimensions.
         to_numpy: If True, converts the native tensor to a `numpy.ndarray`.
 
     Returns:
         Native tensor with dimensions matching `groups`.
     """
     assert isinstance(value, Tensor), f"value must be a Tensor but got {type(value)}"
+    assert not value._is_tracer, f"Failed accessing native values because tensor {value.shape} is a tracer"
     assert value.shape.is_uniform, f"Only uniform (homogenous) tensors can be converted to native but got shape {value.shape}"
     assert isinstance(groups, (tuple, list)), f"groups must be a tuple or list but got {type(value)}"
     order = []
     if Ellipsis in groups:
         ellipsis_dims = value.shape.without([g for g in groups if g is not Ellipsis])
         groups = [ellipsis_dims if g is Ellipsis else g for g in groups]
     groups = [group(value) if callable(group) else group for group in groups]
@@ -1563,16 +1564,15 @@
         result = value.default_backend.all(value.native(value.shape), value.shape.indices(dims))
         return NativeTensor(result, value.shape.without(dims))
     elif isinstance(value, TensorStack):
         reduced_inners = [_all(t, dims.without(value._stack_dim)) for t in value._tensors]
         return functools.reduce(lambda x, y: x & y, reduced_inners) if value._stack_dim in dims else TensorStack(reduced_inners, value._stack_dim)
     elif isinstance(value, (SparseCoordinateTensor, CompressedSparseMatrix)):
         if sparse_dims(value) in dims:
-            values_all = _all(value._values, dims.without(sparse_dims(value)) & instance(value._values))
-            return all_([values_all, value._default], '0') if value._default is not None else values_all
+            return _all(value._values, dims.without(sparse_dims(value)) & instance(value._values))
     raise ValueError(type(value))
 
 
 def max_(value: Union[Tensor, list, tuple, Number, bool], dim: DimFilter = non_batch) -> Tensor:
     """
     Determines the maximum value of `values` along the specified dimensions.
 
@@ -2714,15 +2714,15 @@
             native_result = backend.scatter(native_grid, native_indices, native_values, mode=mode)
         else:  # mean
             zero_grid = backend.zeros_like(native_grid)
             summed = backend.scatter(zero_grid, native_indices, native_values, mode='add')
             count = backend.scatter(zero_grid, native_indices, backend.ones_like(native_values), mode='add')
             native_result = summed / backend.maximum(count, 1)
             native_result = backend.where(count == 0, native_grid, native_result)
-        return reshaped_tensor(native_result, [batches, *indexed_dims, channels], check_sizes=True)
+        return reshaped_tensor(native_result, [batches, *indexed_dims, channels], check_sizes=True, convert=False)
 
     def scatter_backward(args: dict, _output, d_output):
         from ._nd import spatial_gradient
         values_grad = gather(d_output, args['indices'])
         spatial_gradient_indices = gather(spatial_gradient(d_output, dims=indexed_dims), args['indices'])
         indices_grad = mean(spatial_gradient_indices * args['values'], 'vector_')
         return None, indices_grad, values_grad
@@ -3083,18 +3083,20 @@
 
     Args:
         x: `Tensor` or `phiml.math.magic.PhiTreeNode` for which gradients should be disabled.
 
     Returns:
         Copy of `x`.
     """
+    if isinstance(x, Shape):
+        return x
     return _backend_op1(x, Backend.stop_gradient)
 
 
-def pairwise_distances(positions: Tensor,
+def pairwise_differences(positions: Tensor,
                        max_distance: Union[float, Tensor] = None,
                        format: Union[str, Tensor] = 'dense',
                        default: Optional[float] = None,
                        method: str = 'sparse') -> Tensor:
     """
     Computes the distance matrix containing the pairwise position differences between each pair of points.
     Points that are further apart than `max_distance` (if specified) are assigned a distance value of `0`.
@@ -3121,15 +3123,14 @@
     Examples:
         >>> pos = vec(x=0, y=tensor([0, 1, 2.5], instance('particles')))
         >>> dx = pairwise_distances(pos, format='dense', max_distance=2)
         >>> dx.particles[0]
         (x=0.000, y=0.000); (x=0.000, y=1.000); (x=0.000, y=0.000) (~particlesᵈ=3, vectorᶜ=x,y)
     """
     assert isinstance(positions, Tensor), f"positions must be a Tensor but got {type(positions)}"
-    assert default in [0, None], f"default value must be either 0 or None but got '{default}'"
     primal_dims = positions.shape.non_batch.non_channel.non_dual
     dual_dims = primal_dims.as_dual()
     # --- Dense ---
     if (isinstance(format, str) and format == 'dense') or (isinstance(format, Tensor) and get_format(format) == 'dense'):
         if isinstance(format, Tensor):
             dual_dims = dual(format)
         dx = unpack_dim(pack_dims(positions, non_batch(positions).non_channel.non_dual, instance('_tmp')), '_tmp', dual_dims) - positions
@@ -3171,14 +3172,16 @@
     from ..backend._partition import find_neighbors_sparse, find_neighbors_semi_sparse, find_neighbors_matscipy, find_neighbors_sklearn
     if mode == 'loop':
         indices = []
         values = []
         for b in batch_shape.meshgrid():
             native_positions = reshaped_native(positions[b], [primal_dims, channel(positions)])
             native_max_dist = max_distance[b].native()
+            if method == 'auto':
+                method = 'sparse'  # ToDo
             if method == 'sparse':
                 nat_rows, nat_cols, nat_vals = find_neighbors_sparse(native_positions, native_max_dist, None, periodic=False, default=default)
             elif method == 'semi-sparse':
                 nat_rows, nat_cols, nat_vals, req_pair_count, req_max_occupancy = find_neighbors_semi_sparse(native_positions, native_max_dist, None, periodic=False, default=default)
             elif method == 'matscipy':
                 assert positions.available, f"Cannot jit-compile matscipy neighborhood search"
                 nat_rows, nat_cols, nat_vals = find_neighbors_matscipy(native_positions, native_max_dist, None, periodic=False)
@@ -3202,15 +3205,15 @@
         # nat_indices = backend.stack([nat_rows, nat_cols], -1)
         # indices = reshaped_tensor(nat_indices, [batch_shape, instance('pairs'), channel(vector=primal_dims.names + dual_dims.names)], convert=False)
         # values = reshaped_tensor(nat_vals, [batch_shape, instance('pairs'), channel(positions)])
     else:
         raise RuntimeError
     # --- Assemble sparse matrix ---
     dense_shape = primal_dims & dual_dims
-    coo = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, default=default)
+    coo = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, indices_constant=False)
     return to_format(coo, format)
 
 
 def map_pairs(map_function: Callable, values: Tensor, connections: Tensor):
     """
     Evaluates `map_function` on all pairs of elements present in the sparsity pattern of `connections`.
```

### Comparing `phiml-1.5.0/phiml/math/_optimize.py` & `phiml-1.5.1/phiml/math/_optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -571,16 +571,20 @@
     x0_tree, x0_tensors = disassemble_tree(solve.x0, cache=False, attr_type=value_attributes)
     assert solve.x0 is not None, "Please specify the initial guess as Solve(..., x0=initial_guess)"
     assert len(x0_tensors) == len(y_tensors) == 1, "Only single-tensor linear solves are currently supported"
     if y_tree == 'native' and x0_tree == 'native':
         if callable(f):  # assume batch + 1 dim
             rank = y_tensors[0].rank
             assert x0_tensors[0].rank == rank, f"y and x0 must have the same rank but got {y_tensors[0].shape.sizes} for y and {x0_tensors[0].shape.sizes} for x0"
-            y = wrap(y, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
-            x0 = wrap(solve.x0, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+            if rank == 0:
+                y = wrap(y)
+                x0 = wrap(solve.x0)
+            else:
+                y = wrap(y, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
+                x0 = wrap(solve.x0, *[batch(f'batch{i}') for i in range(rank - 1)], channel('vector'))
             solve = copy_with(solve, x0=x0)
             solution = solve_linear(f, y, solve, *f_args, grad_for_f=grad_for_f, f_kwargs=f_kwargs, **f_kwargs_)
             return solution.native(','.join([f'batch{i}' for i in range(rank - 1)]) + ',vector')
         else:
             b = choose_backend(y, solve.x0, f)
             f_dims = b.staticshape(f)
             y_dims = b.staticshape(y)
@@ -763,15 +767,18 @@
         # if tracing and not Backend.supports(Backend.python_call) -> cannot use ILU
         native_triangular = target_backend.supports(Backend.solve_triangular_sparse) if is_sparse(matrix) else target_backend.supports(Backend.solve_triangular_dense)
         if solver in ['direct', 'scipy-direct']:
             method = None
         elif native_triangular:
             method = 'ilu'
         elif spatial(matrix):
-            method = 'cluster'
+            if target_backend.name == 'torch' and not target_backend.is_available(None):  # PyTorch JIT not efficient with preconditioner
+                method = None
+            else:
+                method = 'cluster'
         else:
             method = None
         ML_LOGGER.info(f"Auto-selecting preconditioner '{method}' for '{solver}' on {target_backend}")
     if method == 'ilu':
         n = dual(matrix).volume
         entry_count = stored_values(matrix).shape.volume
         avg_entries_per_element = entry_count / n
@@ -844,16 +851,16 @@
         (l_idx_nat, l_val_nat), (u_idx_nat, u_val_nat) = incomplete_lu_coo(indices, values, shape, iterations, safe)
         col_dims = matrix._shape.only(dual)
         row_dims = matrix._dense_shape.without(col_dims)
         l_indices = matrix._unpack_indices(l_idx_nat[..., 0], l_idx_nat[..., 1], row_dims, col_dims, ind_batch)
         u_indices = matrix._unpack_indices(u_idx_nat[..., 0], u_idx_nat[..., 1], row_dims, col_dims, ind_batch)
         l_values = reshaped_tensor(l_val_nat, [ind_batch, instance(matrix._values), channels], convert=False)
         u_values = reshaped_tensor(u_val_nat, [ind_batch, instance(matrix._values), channels], convert=False)
-        lower = SparseCoordinateTensor(l_indices, l_values, matrix._dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._default)
-        upper = SparseCoordinateTensor(u_indices, u_values, matrix._dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._default)
+        lower = SparseCoordinateTensor(l_indices, l_values, matrix._dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._indices_constant)
+        upper = SparseCoordinateTensor(u_indices, u_values, matrix._dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._indices_constant)
     else:  # dense matrix
         native_matrix = reshaped_native(matrix, [batch, non_batch(matrix).non_dual, dual, EMPTY_SHAPE])
         l_native, u_native = incomplete_lu_dense(native_matrix, iterations, safe)
         lower = reshaped_tensor(l_native, [batch(matrix), non_batch(matrix).non_dual, dual(matrix), EMPTY_SHAPE])
         upper = reshaped_tensor(u_native, [batch(matrix), non_batch(matrix).non_dual, dual(matrix), EMPTY_SHAPE])
     return lower, upper
```

### Comparing `phiml-1.5.0/phiml/math/_shape.py` & `phiml-1.5.1/phiml/math/_shape.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/math/_sparse.py` & `phiml-1.5.1/phiml/math/_sparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import numpy as np
 import scipy.sparse
 from scipy.sparse import csr_matrix
 
 from ._shape import Shape, non_batch, merge_shapes, instance, batch, non_instance, shape, channel, spatial, DimFilter, concat_shapes, EMPTY_SHAPE, dual, DUAL_DIM, SPATIAL_DIM, \
     non_channel, DEBUG_CHECKS
 from ._magic_ops import concat, pack_dims, expand, rename_dims, stack, unpack_dim, unstack
-from ._tensors import Tensor, TensorStack, NativeTensor, cached, wrap
+from ._tensors import Tensor, TensorStack, NativeTensor, cached, wrap, variable_shape
 from ..backend import choose_backend, NUMPY, Backend
 from ..backend._dtype import DType
 
 
 def sparse_tensor(indices: Tensor,
                   values: Tensor,
                   dense_shape: Shape,
                   can_contain_double_entries=True,
                   indices_sorted=False,
                   format='coo',
-                  default: Number or None = 0) -> Tensor:
+                  indices_constant: bool = True) -> Tensor:
     """
     Construct a sparse tensor that stores `values` at the corresponding `indices` and is 0 everywhere else.
     In addition to the sparse dimensions indexed by `indices`, the tensor inherits all batch and channel dimensions from `values`.
 
     Args:
         indices: `Tensor` encoding the positions of stored values. It has the following dimensions:
 
@@ -43,34 +43,37 @@
             * Any number of batch dimensions
 
         dense_shape: Dimensions listed in `indices`.
             The order can differ from the item names of `indices`.
         can_contain_double_entries: Whether some indices might occur more than once.
             If so, values at the same index will be summed.
         indices_sorted: Whether the indices are sorted in ascending order given the dimension order of the item names of `indices`.
+        indices_constant: Whether the positions of the non-zero values are fixed.
+            If `True`, JIT compilation will not create a placeholder for `indices`.
         format: Sparse format in which to store the data, such as `'coo'` or `'csr'`. See `phiml.math.get_format`.
-        default: Value the sparse tensor returns for non-stored values. Must be `0` or `None`.
 
     Returns:
         Sparse `Tensor` with the specified `format`.
     """
-    assert default in [0, None], f"default value must be either 0 or None but got '{default}'"
-    coo = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted, default)
+    if indices_constant is None:
+        indices_constant = indices.default_backend.name == 'numpy'
+    assert isinstance(indices_constant, bool)
+    coo = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted, indices_constant)
     return to_format(coo, format)
 
 
 def tensor_like(existing_tensor: Tensor, values: Union[Tensor, Number, bool], value_order: str = None):
     """
     Creates a tensor with the same format and shape as `existing_tensor`.
 
     Args:
         existing_tensor: Any `Tensor`, sparse or dense.
         values: New values to replace the existing values by.
-            If `existing_tensor` is sparse, `values` must have an instance dimension to list the stored values, matching the sparse indices.
-        value_order: Order of `values` compared to `existing_tensor`.
+            If `existing_tensor` is sparse, `values` must broadcast to the instance dimension listing the stored indices.
+        value_order: Order of `values` compared to `existing_tensor`, only relevant if `existing_tensor` is sparse.
             If `'original'`, the values are ordered like the values that was used to create the first tensor with this sparsity pattern.
             If `'as existing'`, the values match the current order of `existing_tensor`.
             Note that the order of values may be changed upon creating a sparse tensor.
 
     Returns:
         `Tensor`
     """
@@ -97,15 +100,15 @@
     indices: Tensor whose instance dimensions list the sparse entries and whose single channel dimension indexes the sparse dims. Can also have batch dimensions.
     values: Tensor with any of the instance dimensions of `indices` but no others. Can have any other non-instance dimensions to represent batched values.
 
     Batched-value matrices can be converted to explicit sparsity using sparsify_batch_dims().
     When reducing a batch dim (e.g. by summing over it), the dual dim remains, i.e. the input space keeps that dimension.
     """
 
-    def __init__(self, indices: Tensor, values: Tensor, dense_shape: Shape, can_contain_double_entries: bool, indices_sorted: bool, default: Number):
+    def __init__(self, indices: Tensor, values: Tensor, dense_shape: Shape, can_contain_double_entries: bool, indices_sorted: bool, indices_constant: bool):
         """
         Construct a sparse tensor with any number of sparse, dense and batch dimensions.
         """
         super().__init__()
         assert isinstance(indices, Tensor), f"indices must be a Tensor but got {type(indices)}"
         assert isinstance(values, Tensor), f"values must be a Tensor but got {type(values)}"
         assert instance(indices), f"indices must have an instance dimension but got {indices.shape}"
@@ -120,17 +123,15 @@
             warnings.warn(f"You are creating a sparse tensor with only constant values {values.shape}. To have values vary along indices, add the corresponding instance dimension.", RuntimeWarning, stacklevel=3)
         self._shape = merge_shapes(dense_shape, batch(indices), non_instance(values))
         self._dense_shape = dense_shape
         self._indices = indices
         self._values = values
         self._can_contain_double_entries = can_contain_double_entries
         self._indices_sorted = indices_sorted
-        self._default = default
-        # if DEBUG_CHECKS:
-        #     self.compress_rows()
+        self._indices_constant = indices_constant
 
     @property
     def shape(self) -> Shape:
         return self._shape
 
     @property
     def dtype(self) -> DType:
@@ -149,43 +150,41 @@
         return native_matrix(self, self.default_backend)
 
     @property
     def _is_tracer(self) -> bool:
         return self._indices._is_tracer or self._values._is_tracer
 
     def _with_values(self, new_values: Tensor):
-        return SparseCoordinateTensor(self._indices, new_values, self._dense_shape, self._can_contain_double_entries, self._indices_sorted, self._default)
+        return SparseCoordinateTensor(self._indices, new_values, self._dense_shape, self._can_contain_double_entries, self._indices_sorted, self._indices_constant)
 
     def _natives(self) -> tuple:
-        indices_const = self._indices.default_backend is not self._values.default_backend
-        if indices_const:
+        if self._indices_constant:
             return self._values._natives()  # If we return NumPy arrays, they might get converted in function transformations
         else:
             return self._values._natives() + self._indices._natives()
 
     def _spec_dict(self) -> dict:
-        indices_const = self._indices.default_backend is not self._values.default_backend
         return {'type': SparseCoordinateTensor,
                 'shape': self._shape,
                 'dense_shape': self._dense_shape,
-                'indices': self._indices if indices_const else self._indices._spec_dict(),
+                'indices': self._indices if self._indices_constant else self._indices._spec_dict(),
                 'values': self._values._spec_dict(),
                 'can_contain_double_entries': self._can_contain_double_entries,
                 'indices_sorted': self._indices_sorted,
-                'default': self._default}
+                'indices_constant': self._indices_constant}
 
     @classmethod
     def _from_spec_and_natives(cls, spec: dict, natives: list):
         values = spec['values']['type']._from_spec_and_natives(spec['values'], natives)
         indices_or_spec = spec['indices']
         if isinstance(indices_or_spec, Tensor):
             indices = indices_or_spec
         else:
             indices = spec['indices']['type']._from_spec_and_natives(spec['indices'], natives)
-        return SparseCoordinateTensor(indices, values, spec['dense_shape'], spec['can_contain_double_entries'], spec['indices_sorted'], spec['default'])
+        return SparseCoordinateTensor(indices, values, spec['dense_shape'], spec['can_contain_double_entries'], spec['indices_sorted'], spec['indices_constant'])
 
     def _native_coo_components(self, col_dims: DimFilter, matrix=False):
         col_dims = self._shape.only(col_dims)
         row_dims = self._dense_shape.without(col_dims)
         row_idx_packed, col_idx_packed = self._pack_indices(row_dims, col_dims)
         from . import reshaped_native
         ind_batch = batch(self._indices)
@@ -278,15 +277,15 @@
         entries_dim = instance(values).name
         perm = None
         if np.any(scipy_csr.data != idx):
             perm = {entries_dim: wrap(scipy_csr.data - 1, instance(entries_dim))}
             values = values[perm]  # Change order accordingly
         indices = wrap(scipy_csr.indices, instance(entries_dim))
         pointers = wrap(scipy_csr.indptr, instance('pointers'))
-        return CompressedSparseMatrix(indices, pointers, values, u_dims, c_dims, self._default, uncompressed_indices=uncompressed_indices, uncompressed_indices_perm=perm)
+        return CompressedSparseMatrix(indices, pointers, values, u_dims, c_dims, self._indices_constant, uncompressed_indices=uncompressed_indices, uncompressed_indices_perm=perm)
 
     def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Tensor':
         dims = self._shape.only(dims)
         assert dims in self._dense_shape, f"Can only pack sparse dimensions on SparseCoordinateTensor but got {dims} of which {dims.without(self._dense_shape)} are not sparse"
         assert self._indices.default_backend is NUMPY, "Can only pack NumPy indices as of yet"
         from ._ops import reshaped_native, reshaped_tensor
         inst_dim_order = instance(self._indices)
@@ -294,25 +293,25 @@
         values = pack_dims(self._values, inst_dim_order, instance('sp_entries'))
         idx_to_pack = indices.sparse_idx[dims.names]
         idx_packed = np.ravel_multi_index(reshaped_native(idx_to_pack, [channel, instance(idx_to_pack)]), dims.sizes)
         idx_packed = expand(reshaped_tensor(idx_packed, [instance('sp_entries')]), channel(sparse_idx=packed_dim.name))
         indices = concat([indices.sparse_idx[list(self._dense_shape.without(dims).names)], idx_packed], 'sparse_idx')
         dense_shape = concat_shapes(self._dense_shape.without(dims), packed_dim.with_size(dims.volume))
         idx_sorted = self._indices_sorted and False  # ToDo still sorted if dims are ordered correctly and no other dim in between and inserted at right point
-        return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, idx_sorted, self._default)
+        return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, idx_sorted, self._indices_constant)
 
     def _with_shape_replaced(self, new_shape: Shape):
         assert self._shape.rank == new_shape.rank
         dense_shape = new_shape[self._shape.indices(self._dense_shape)]
         new_item_names = new_shape[self._shape.indices(self._indices.shape.get_item_names('sparse_idx'))].names
         values = self._values._with_shape_replaced(self._values.shape.replace(self._shape, new_shape))
         non_vec = self._shape.without('sparse_idx')
         new_non_vec = new_shape[self._shape.indices(non_vec)]
         indices = self._indices._with_shape_replaced(self._indices.shape.replace(non_vec, new_non_vec).with_dim_size('sparse_idx', new_item_names))
-        return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, self._indices_sorted, self._default)
+        return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, self._indices_sorted, self._indices_constant)
 
     def _op1(self, native_function):
         return self._with_values(self._values._op1(native_function))
 
     def _op2(self, other, operator: Callable, native_function: Callable, op_name: str = 'unknown', op_symbol: str = '?') -> 'Tensor':
         other_shape = shape(other)
         affects_only_values = self._dense_shape.isdisjoint(other_shape)
@@ -335,26 +334,26 @@
                 indices = concat([self_indices, other_indices], 'sp_entries')
                 if op_symbol == '+':
                     values = concat([self_values, other_values], instance(self_values), expand_values=True)
                 elif op_name == 'sub':
                     values = concat([self_values, -other_values], instance(self_values), expand_values=True)
                 else:  # op_name == 'rsub':
                     values = concat([-self_values, other_values], instance(self_values), expand_values=True)
-                return SparseCoordinateTensor(indices, values, self._dense_shape & other._dense_shape, can_contain_double_entries=True, indices_sorted=False, default=self._default)
+                return SparseCoordinateTensor(indices, values, self._dense_shape & other._dense_shape, can_contain_double_entries=True, indices_sorted=False, indices_constant=self._indices_constant)
         else:  # other is dense
             if self._dense_shape in other.shape:  # all dims dense -> convert to dense
                 return dense(self)._op2(other, operator, native_function, op_name, op_symbol)
             else:  # only some dims dense -> stay sparse
                 dense_dims = self._dense_shape.only(other.shape)
                 other_values = other[self._indices.sparse_idx[dense_dims.name_list]]
                 values = operator(self._values, other_values)
                 return self._with_values(values)
 
     def _getitem(self, selection: dict) -> 'Tensor':
-        batch_selection = {dim: selection[dim] for dim in self._shape.only(tuple(selection)).names}
+        batch_selection = {dim: selection[dim] for dim in self._shape.without(self.sparse_dims).only(tuple(selection)).names}
         indices = self._indices[{dim: sel for dim, sel in batch_selection.items() if dim != 'sparse_idx'}]
         values = self._values[batch_selection]
         if self._dense_shape.only(tuple(selection)):
             keep = expand(True, instance(self._indices))
             for dim, sel in selection.items():
                 dim_indices = self._indices[dim]
                 if isinstance(sel, int):
@@ -371,23 +370,22 @@
                 keep &= (start <= dim_indices) & (dim_indices < stop)
                 from . import vec
                 indices -= vec('sparse_idx', **{d: start if d == dim else 0 for d in indices.sparse_idx.item_names})
             from ._ops import boolean_mask
             indices = boolean_mask(indices, instance(indices), keep)
             values = boolean_mask(values, instance(indices), keep)
             dense_shape = self._dense_shape.after_gather(selection)
-            return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, self._indices_sorted, self._default)
+            return SparseCoordinateTensor(indices, values, dense_shape, self._can_contain_double_entries, self._indices_sorted, self._indices_constant)
         else:
-            return SparseCoordinateTensor(indices, values, self._dense_shape, self._can_contain_double_entries, self._indices_sorted, self._default)
+            return SparseCoordinateTensor(indices, values, self._dense_shape, self._can_contain_double_entries, self._indices_sorted, self._indices_constant)
 
     def __concat__(self, tensors: tuple, dim: str, **kwargs) -> 'SparseCoordinateTensor':
         if not all(isinstance(t, SparseCoordinateTensor) for t in tensors):
             return NotImplemented
         if dim in self._dense_shape:
-            # assert all default equal
             from . import vec
             indices = []
             values = []
             offset = 0
             for t in tensors:
                 t_indices = stored_indices(t, list_dim=instance(self._indices), index_dim=channel(self._indices))
                 t_values = stored_values(t, list_dim=instance(self._values))
@@ -396,31 +394,47 @@
                 indices.append(t_indices)
                 values.append(t_values)
             indices = concat(indices, instance(self._indices))
             values = concat(values, instance(self._values))
             dense_shape = self._dense_shape.with_dim_size(dim, sum([t.shape.get_size(dim) for t in tensors]))
             can_contain_double_entries = any([t._can_contain_double_entries for t in tensors])
             indices_sorted = all([t._indices_sorted for t in tensors])
-            return SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted, self._default)
+            indices_constant = all([t._indices_constant for t in tensors])
+            return SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted, indices_constant)
+        elif all([same_sparsity_pattern(v, tensors[0]) for v in tensors[1:]]):
+            stored = [v._values for v in tensors]
+            cat = concat(stored, dim, **kwargs)
+            return tensors[0]._with_values(cat)
         else:
             raise NotImplementedError("concatenating compressed sparse tensors along non-sparse dims not yet supported")
 
+    @staticmethod
+    def __stack__(values: tuple, dim: Shape, **_kwargs) -> 'Tensor':
+        if all(isinstance(v, SparseCoordinateTensor) for v in values) and all([same_sparsity_pattern(v, values[0]) for v in values[1:]]):
+            stored = [v._values for v in values]
+            stacked = stack(stored, dim, **_kwargs)
+            return values[0]._with_values(stacked)
+        return Tensor.__stack__(values, dim, **_kwargs)
+
+    def __expand__(self, dims: Shape, **kwargs) -> 'Tensor':
+        return self._with_values(expand(self._values, dims, **kwargs))
+
 
 class CompressedSparseMatrix(Tensor):
 
     def __init__(self,
                  indices: Tensor,
                  pointers: Tensor,
                  values: Tensor,
                  uncompressed_dims: Shape,
                  compressed_dims: Shape,
-                 default: Number,
+                 indices_constant: bool,
                  uncompressed_offset: int = None,
                  uncompressed_indices: Tensor = None,
-                 uncompressed_indices_perm: Tensor = None):
+                 uncompressed_indices_perm: Tensor = None,):
         """
 
         Args:
             indices: indices must be sorted in ascending order by compressed_dim and other sparse dims.
                 Must have one or multiple instance dimensions and can have any number of batch dimensions.
                 No spatial and channel dimensions allowed.
             pointers:
@@ -449,15 +463,15 @@
             assert instance(uncompressed_indices) == instance(indices), f"Number of uncompressed indices {instance(uncompressed_offset)} does not match compressed indices {instance(indices)}"
         self._shape = merge_shapes(compressed_dims, uncompressed_dims, batch(indices), batch(pointers), non_instance(values))
         self._indices = indices
         self._pointers = rename_dims(pointers, instance, 'pointers')
         self._values = values
         self._uncompressed_dims = uncompressed_dims
         self._compressed_dims = compressed_dims
-        self._default = default
+        self._indices_constant = indices_constant
         self._uncompressed_offset = uncompressed_offset
         self._uncompressed_indices = uncompressed_indices
         self._uncompressed_indices_perm = uncompressed_indices_perm
 
     @property
     def shape(self) -> Shape:
         return self._shape
@@ -475,37 +489,31 @@
         return self._values.dtype
 
     @property
     def _is_tracer(self) -> bool:
         return self._values._is_tracer or self._indices._is_tracer or self._pointers._is_tracer
 
     def _natives(self) -> tuple:
-        indices_const = self._indices.default_backend is not self._values.default_backend
-        pointers_const = self._pointers.default_backend is not self._values.default_backend
-        result = self._values._natives()
-        if not indices_const:
-            result += self._indices._natives()
-        if not pointers_const:
-            result += self._pointers._natives()
-        return result
+        if self._indices_constant:
+            return self._values._natives()
+        else:
+            return self._values._natives() + self._indices._natives() + self._pointers._natives()
 
     def _spec_dict(self) -> dict:
-        indices_const = self._indices.default_backend is not self._values.default_backend
-        pointers_const = self._pointers.default_backend is not self._values.default_backend
         return {'type': CompressedSparseMatrix,
                 'shape': self._shape,
                 'values': self._values._spec_dict(),
-                'indices': self._indices if indices_const else self._indices._spec_dict(),
-                'pointers': self._pointers if pointers_const else self._pointers._spec_dict(),
+                'indices': self._indices if self._indices_constant else self._indices._spec_dict(),
+                'pointers': self._pointers if self._indices_constant else self._pointers._spec_dict(),
                 'uncompressed_dims': self._uncompressed_dims,
                 'compressed_dims': self._compressed_dims,
                 'uncompressed_offset': self._uncompressed_offset,
                 'uncompressed_indices': self._uncompressed_indices,
                 'uncompressed_indices_perm': self._uncompressed_indices_perm,
-                'default': self._default,
+                'indices_constant': self._indices_constant,
                 }
 
     @classmethod
     def _from_spec_and_natives(cls, spec: dict, natives: list):
         values = spec['values']['type']._from_spec_and_natives(spec['values'], natives)
         indices_or_spec = spec['indices']
         if isinstance(indices_or_spec, Tensor):
@@ -513,18 +521,18 @@
         else:
             indices = spec['indices']['type']._from_spec_and_natives(spec['indices'], natives)
         pointers_or_spec = spec['pointers']
         if isinstance(pointers_or_spec, Tensor):
             pointers = pointers_or_spec
         else:
             pointers = spec['pointers']['type']._from_spec_and_natives(spec['pointers'], natives)
-        return CompressedSparseMatrix(indices, pointers, values, spec['uncompressed_dims'], spec['compressed_dims'], spec['default'], spec['uncompressed_offset'], spec['uncompressed_indices'], spec['uncompressed_indices_perm'])
+        return CompressedSparseMatrix(indices, pointers, values, spec['uncompressed_dims'], spec['compressed_dims'], spec['indices_constant'], spec['uncompressed_offset'], spec['uncompressed_indices'], spec['uncompressed_indices_perm'])
 
     def _getitem(self, selection: dict) -> 'Tensor':
-        batch_selection = {dim: selection[dim] for dim in self._shape.only(tuple(selection)).names}
+        batch_selection = {dim: selection[dim] for dim in self._shape.without(self.sparse_dims).only(tuple(selection)).names}
         indices = self._indices[batch_selection]
         pointers = self._pointers[batch_selection]
         values = self._values[batch_selection]
         uncompressed = self._uncompressed_dims
         compressed = self._compressed_dims
         uncompressed_offset = self._uncompressed_offset
         if compressed.only(tuple(selection)):
@@ -552,22 +560,22 @@
             ind_sel = selection[uncompressed.name]
             if isinstance(ind_sel, int):
                 raise NotImplementedError(f"Slicing with int not yet supported for sparse tensors. Use a range instead, e.g. [{ind_sel}:{ind_sel+1}] instead of [{ind_sel}]")
             elif isinstance(ind_sel, slice):
                 assert ind_sel.step in (None, 1), f"Only step size 1 supported for sparse indexing but got {ind_sel.step}"
                 start = ind_sel.start or 0
                 stop = uncompressed.volume if ind_sel.stop is None else ind_sel.stop
-                keep = (start <= self._indices) & (self._indices < stop)
+                keep = (start <= indices) & (indices < stop)
                 from ._ops import where
                 values = where(keep, values, 0)
                 uncompressed_offset = start
                 uncompressed = uncompressed.after_gather({uncompressed.name: ind_sel})
             else:
                 raise NotImplementedError
-        return CompressedSparseMatrix(indices, pointers, values, uncompressed, compressed, self._default, uncompressed_offset)
+        return CompressedSparseMatrix(indices, pointers, values, uncompressed, compressed, self._indices_constant, uncompressed_offset)
 
     def __concat__(self, tensors: tuple, dim: str, **kwargs) -> 'CompressedSparseMatrix':
         if not all(isinstance(t, CompressedSparseMatrix) for t in tensors):
             return NotImplemented
         if dim == self._compressed_dims[0].name:
             indices = concat([t._indices for t in tensors], instance(self._indices), **kwargs)
             values = concat([t._values for t in tensors], instance(self._values), **kwargs)
@@ -575,27 +583,42 @@
             pointer_offset = 0
             for i, t in enumerate(tensors):
                 pointers.append((t._pointers[1:] if i else t._pointers) + pointer_offset)
                 pointer_offset += t._pointers[-1]
             assert pointer_offset == instance(indices).volume
             pointers = concat(pointers, instance(self._pointers))
             compressed = self._compressed_dims.with_dim_size(dim, sum(t.shape.get_size(dim) for t in tensors))
-            return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims, compressed, self._default, self._uncompressed_offset)
+            return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims, compressed, self._indices_constant, self._uncompressed_offset)
         elif dim == self._uncompressed_dims[0].name:
             if all([same_sparsity_pattern(self, t) for t in tensors]):
                 # ToDo test if offsets match and ordered correctly
                 from ._ops import sum_
                 values = sum_([t._values for t in tensors], '0')
                 uncompressed = self._uncompressed_dims.with_dim_size(dim, sum(t.shape.get_size(dim) for t in tensors))
-                return CompressedSparseMatrix(self._indices, self._pointers, values, uncompressed, self._compressed_dims, self._default, uncompressed_offset=None)
+                return CompressedSparseMatrix(self._indices, self._pointers, values, uncompressed, self._compressed_dims, self._indices_constant, uncompressed_offset=None)
             else:
                 raise NotImplementedError("concatenating arbitrary compressed sparse tensors along uncompressed dim is not yet supported")
+        elif all([same_sparsity_pattern(v, tensors[0]) for v in tensors[1:]]):
+            stored = [v._values for v in tensors]
+            cat = concat(stored, dim, **kwargs)
+            return tensors[0]._with_values(cat)
         else:
             raise NotImplementedError("concatenating compressed sparse tensors along non-sparse dims not yet supported")
 
+    @staticmethod
+    def __stack__(values: tuple, dim: Shape, **_kwargs) -> 'Tensor':
+        if all(isinstance(v, CompressedSparseMatrix) for v in values) and all([same_sparsity_pattern(v, values[0]) for v in values[1:]]):
+            stored = [v._values for v in values]
+            stacked = stack(stored, dim, **_kwargs)
+            return values[0]._with_values(stacked)
+        return Tensor.__stack__(values, dim, **_kwargs)
+
+    def __expand__(self, dims: Shape, **kwargs) -> 'Tensor':
+        return self._with_values(expand(self._values, dims, **kwargs))
+
     def _op1(self, native_function):
         return self._with_values(self._values._op1(native_function))
 
     def _op2(self, other, operator: Callable, native_function: Callable, op_name: str = 'unknown', op_symbol: str = '?') -> 'Tensor':
         other_shape = shape(other)
         affects_only_values = self.sparse_dims.isdisjoint(other_shape) and non_instance(self._indices).isdisjoint(other_shape)
         if affects_only_values:
@@ -632,23 +655,23 @@
             if self._uncompressed_offset is not None:
                 result_values = where(self._valid_mask(), result_values, 0)
             return self._with_values(result_values)
         else:
             raise NotImplementedError
 
     def _with_values(self, new_values: Tensor):
-        return CompressedSparseMatrix(self._indices, self._pointers, new_values, self._uncompressed_dims, self._compressed_dims, self._default, self._uncompressed_offset, self._uncompressed_indices, self._uncompressed_indices_perm)
+        return CompressedSparseMatrix(self._indices, self._pointers, new_values, self._uncompressed_dims, self._compressed_dims, self._indices_constant, self._uncompressed_offset, self._uncompressed_indices, self._uncompressed_indices_perm)
 
     def _with_shape_replaced(self, new_shape: Shape):
         assert self._shape.rank == new_shape.rank
         values = self._values._with_shape_replaced(self._values.shape.replace(self._shape, new_shape))
         indices = self._indices._with_shape_replaced(self._indices.shape.replace(self._shape, new_shape))
         pointers = self._pointers._with_shape_replaced(self._pointers.shape.replace(self._shape, new_shape))
         uncompressed_indices = self._uncompressed_indices._with_shape_replaced(self._uncompressed_indices.shape.replace(self._shape, new_shape, replace_item_names=channel)) if self._uncompressed_indices is not None else None
-        return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims.replace(self._shape, new_shape), self._compressed_dims.replace(self._shape, new_shape), self._default, self._uncompressed_offset, uncompressed_indices, self._uncompressed_indices_perm)
+        return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims.replace(self._shape, new_shape), self._compressed_dims.replace(self._shape, new_shape), self._indices_constant, self._uncompressed_offset, uncompressed_indices, self._uncompressed_indices_perm)
 
     def _native_csr_components(self, invalid='clamp', get_values=True):
         assert invalid in ['clamp', 'discard', 'keep']
         from ._ops import reshaped_native
         ind_batch = batch(self._indices) & batch(self._pointers)
         channels = non_instance(self._values).without(ind_batch)
         native_indices = reshaped_native(self._indices, [ind_batch, instance])
@@ -676,15 +699,15 @@
         valid = (self._uncompressed_offset <= self._indices) & (self._indices < self._uncompressed_offset + self._uncompressed_dims.volume)
         indices = boolean_mask(self._indices, instance(self._indices), valid)
         values = boolean_mask(self._values, instance(self._values), valid)
         removed = cumulative_sum(~valid, instance(valid))
         removed = removed[self._pointers.pointers[1:] - 1]
         removed = pad(removed, {'pointers': (1, 0)}, 1)
         pointers = self._pointers - removed
-        return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims, self._compressed_dims, self._default)
+        return CompressedSparseMatrix(indices, pointers, values, self._uncompressed_dims, self._compressed_dims, self._indices_constant)
 
     def _valid_mask(self):
         return (self._uncompressed_offset <= self._indices) & (self._indices < self._uncompressed_offset + self._uncompressed_dims.volume)
 
     def _coo_indices(self, invalid='clamp', stack_dim: Shape = None):
         ind_batch, channels, native_indices, native_pointers, _, native_shape = self._native_csr_components(invalid, get_values=False)
         native_indices = choose_backend(native_indices, native_pointers).csr_to_coo(native_indices, native_pointers)
@@ -704,35 +727,35 @@
             native_indices = choose_backend(native_indices, native_pointers).csr_to_coo(native_indices, native_pointers)
             from ._ops import reshaped_tensor
             if self._compressed_dims.rank == self._uncompressed_dims.rank == 1:
                 indices = reshaped_tensor(native_indices, [ind_batch, instance(self._indices), channel(sparse_idx=(self._compressed_dims.name, self._uncompressed_dims.name))], convert=False)
                 values = reshaped_tensor(native_values, [ind_batch, instance(self._values), channel(self._values)])
             else:
                 raise NotImplementedError()
-            return SparseCoordinateTensor(indices, values, concat_shapes(self._compressed_dims, self._uncompressed_dims), False, True, self._default)
+            return SparseCoordinateTensor(indices, values, concat_shapes(self._compressed_dims, self._uncompressed_dims), False, True, self._indices_constant)
         if self._uncompressed_indices_perm is not None:
             self._uncompressed_indices = self._uncompressed_indices[self._uncompressed_indices_perm]
             self._uncompressed_indices_perm = None
-        return SparseCoordinateTensor(self._uncompressed_indices, self._values, self._compressed_dims & self._uncompressed_dims, False, False, self._default)
+        return SparseCoordinateTensor(self._uncompressed_indices, self._values, self._compressed_dims & self._uncompressed_dims, False, False, self._indices_constant)
 
     def native(self, order: Union[str, tuple, list, Shape] = None, singleton_for_const=False):
         assert order is None, f"sparse matrices are always ordered (primal, dual). For custom ordering, use math.dense(tensor).native() instead."
         return native_matrix(self, self.default_backend)
 
     def __pack_dims__(self, dims: Tuple[str, ...], packed_dim: Shape, pos: Union[int, None], **kwargs) -> 'Tensor':
         assert all(d in self._shape for d in dims)
         dims = self._shape.only(dims, reorder=True)
         if dims.only(self._compressed_dims).is_empty:  # pack cols
             assert self._uncompressed_dims.are_adjacent(dims), f"Can only compress adjacent dims but got {dims} for matrix {self._shape}"
             uncompressed_dims = self._uncompressed_dims.replace(dims, packed_dim.with_size(dims.volume))
-            return CompressedSparseMatrix(self._indices, self._pointers, self._values, uncompressed_dims, self._compressed_dims, self._default, self._uncompressed_offset)
+            return CompressedSparseMatrix(self._indices, self._pointers, self._values, uncompressed_dims, self._compressed_dims, self._indices_constant, self._uncompressed_offset)
         elif dims.only(self._uncompressed_dims).is_empty:   # pack rows
             assert self._compressed_dims.are_adjacent(dims), f"Can only compress adjacent dims but got {dims} for matrix {self._shape}"
             compressed_dims = self._compressed_dims.replace(dims, packed_dim.with_size(dims.volume))
-            return CompressedSparseMatrix(self._indices, self._pointers, self._values, self._uncompressed_dims, compressed_dims, self._default, self._uncompressed_offset)
+            return CompressedSparseMatrix(self._indices, self._pointers, self._values, self._uncompressed_dims, compressed_dims, self._indices_constant, self._uncompressed_offset)
         else:
             raise NotImplementedError(f"Cannot pack dimensions from both columns and rows with compressed sparse matrices but got {dims}")
 
 
 def get_format(x: Tensor) -> str:
     """
     Returns the sparse storage format of a tensor.
@@ -812,15 +835,15 @@
             return x.decompress()
         else:
             return to_format(x.decompress(), format)
     else:  # dense to sparse
         from ._ops import nonzero
         indices = nonzero(rename_dims(x, channel, instance))
         values = x[indices]
-        coo = SparseCoordinateTensor(indices, values, x.shape, can_contain_double_entries=False, indices_sorted=False, default=0)
+        coo = SparseCoordinateTensor(indices, values, x.shape, can_contain_double_entries=False, indices_sorted=False, indices_constant=x.default_backend.name == 'numpy')
         return to_format(coo, format)
 
 
 def sparse_dims(x: Tensor) -> Shape:
     """
     Returns the dimensions of a `Tensor` that are explicitly stored in a sparse format.
 
@@ -864,30 +887,33 @@
     """
     return stored_values(x, invalid='keep').shape.volume / x.shape.volume
 
 
 def stored_values(x: Tensor, list_dim=instance('entries'), invalid='discard') -> Tensor:
     """
     Returns the stored values for a given `Tensor``.
+
     For sparse tensors, this will return only the stored entries.
-    For collapsed tensors, only the stored dimensions will be returned.
-    Dense tensors are returned as-is.
+
+    Dense tensors are reshaped so that all non-batch dimensions are packed into `list_dim`. Batch dimensions are preserved.
 
     Args:
         x: `Tensor`
         list_dim: Dimension along which stored values should be laid out.
         invalid: One of `'discard'`, `'clamp'`, `'keep'` Filter result by valid indices.
             Internally, invalid indices may be stored for performance reasons.
 
     Returns:
         `Tensor` representing all values stored to represent `x`.
     """
     assert invalid in ['discard', 'clamp', 'keep'], f"invalid handling must be one of 'discard', 'clamp', 'keep' but got {invalid}"
     if isinstance(x, NativeTensor):
-        return expand(NativeTensor(x._native, x._native_shape, x._native_shape), list_dim.with_size(1))
+        x = NativeTensor(x._native, x._native_shape, x._native_shape)
+        entries_dims = x.shape.non_batch
+        return pack_dims(x, entries_dims, list_dim)
     if isinstance(x, TensorStack):
         if x.is_cached:
             return stored_values(cached(x))
         return stack([stored_values(t, list_dim) for t in x._tensors], x._stack_dim)
     elif isinstance(x, CompressedSparseMatrix):
         if invalid in ['keep', 'clamp']:
             return rename_dims(x._values, instance, list_dim)
@@ -916,15 +942,15 @@
         `Tensor` representing all indices of stored values.
     """
     assert invalid in ['discard', 'clamp', 'keep'], f"invalid handling must be one of 'discard', 'clamp', 'keep' but got {invalid}"
     if isinstance(x, NativeTensor):
         from ._ops import meshgrid
         if batch(x):
             raise NotImplementedError
-        indices = meshgrid(x._native_shape.non_batch.non_channel)
+        indices = meshgrid(x._native_shape.non_batch.non_channel, stack_dim=index_dim)
         return pack_dims(indices, non_channel, list_dim)
     if isinstance(x, TensorStack):
         if x.is_cached or not x.requires_broadcast:
             return stored_indices(cached(x))
         raise NotImplementedError
         return stack([stored_indices(t, list_dim) for t in x._tensors], x._stack_dim)  # ToDo add index for stack dim
     elif isinstance(x, CompressedSparseMatrix):
@@ -1016,15 +1042,15 @@
         const_entries_dim = instance(sparse._indices).only(sdims.as_instance())
         dense_dims = sparse._dense_shape.only(dense.shape)
         needed_indices = unstack(sparse._indices, const_entries_dim)[0].sparse_idx[dense_dims.name_list]
         dense_gathered = dense[needed_indices]
         values = sparse._values * rename_dims(dense_gathered, ddims, const_entries_dim)
         dense_shape = sparse._dense_shape.without(sdims) & dense.shape.without(ddims)
         indices = sparse._indices[sparse_dims(sparse).without(sdims).name_list]
-        return SparseCoordinateTensor(indices, values, dense_shape, sparse._can_contain_double_entries, sparse._indices_sorted, sparse._default)
+        return SparseCoordinateTensor(indices, values, dense_shape, sparse._can_contain_double_entries, sparse._indices_sorted, sparse._indices_constant)
     backend = choose_backend(*sparse._natives() + dense._natives())
     ind_batch, channels, native_indices, native_values, native_shape = sparse._native_coo_components(sdims, matrix=True)
     rhs_channels = shape(dense).without(ddims).without(channels)
     dense_native = reshaped_native(dense, [ind_batch, ddims, channels, rhs_channels])
     result_native = backend.mul_coo_dense(native_indices, native_values, native_shape, dense_native)
     result = reshaped_tensor(result_native, [ind_batch, sparse._dense_shape.without(sdims), channels, rhs_channels])
     return result
@@ -1039,15 +1065,15 @@
 
     a_gathered = a[{a_dim.name: b._indices[b_dim.name] for a_dim, b_dim in zip(a_dims, b_dims)}]
     values = a_gathered * b._values  # for each value in B, we have all
     i = values._indices[remaining_a]
     j = b._indices[remaining_b][{instance: values._indices[list_dim.name]}]
     indices = concat([i, j], 'sparse_idx')
     values = values._values
-    return SparseCoordinateTensor(indices, values, channel(a) & dual(b), can_contain_double_entries=True, indices_sorted=False, default=a._default)
+    return SparseCoordinateTensor(indices, values, channel(a) & dual(b), can_contain_double_entries=True, indices_sorted=False, indices_constant=a._indices_constant)
 
 
 def native_matrix(value: Tensor, target_backend: Backend):
     target_backend = target_backend or value.default_backend
     cols = dual(value)
     rows = non_batch(value).non_dual
     if not value.available and target_backend != value.default_backend:
@@ -1075,20 +1101,21 @@
         value = value.decompress()  # backend does not support CSR/CSC, use COO instead
     if isinstance(value, SparseCoordinateTensor):  # COO
         ind_batch, channels, indices, values, shape = value._native_coo_components(dual, matrix=True)
         if ind_batch.volume > 1 or channels.volume > 1:
             return b.sparse_coo_tensor_batched(indices, values, shape)
         else:
             return b.sparse_coo_tensor(indices[0], values[0, :, 0], shape)
-    else:
+    else:  # dense matrix
         if batch(value):
             raise NotImplementedError
         v = pack_dims(value, rows, channel('_row'))
         v = pack_dims(v, cols, channel('_col'))
-        from ._ops import reshaped_native
+        from ._ops import convert, reshaped_native
+        v = convert(v, target_backend)
         return reshaped_native(v, ['_row', '_col'])
 
 
 def sparse_dot(x: Tensor, x_dims: Shape, y: Tensor, y_dims: Shape):
     if is_sparse(x) and is_sparse(y) and x_dims in x._values.shape.non_instance and y_dims in y._values.shape.non_instance:
         if same_sparsity_pattern(x, y):
             from ._ops import dot
@@ -1130,15 +1157,15 @@
         indices = concat([arange(channel(sparse_idx=in_dims)), matrix._indices, arange(channel(sparse_idx=out_dims))], 'sparse_idx', expand_values=True)
         offsets = [wrap([*idx.values()] + [0] * non_instance(matrix._indices).volume + [*idx.values()], channel(indices)) for idx in out_dims.meshgrid()]
         offsets = stack(offsets, out_dims.as_instance())
         indices += offsets
         # values = expand(matrix._values, out_dims.as_instance())
         values = matrix._values
         dense_shape = in_dims & matrix._dense_shape & out_dims
-        return SparseCoordinateTensor(indices, values, dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._default)
+        return SparseCoordinateTensor(indices, values, dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._indices_constant)
     raise NotImplementedError
 
 
 # def sparsify_batch_dims(matrix: Tensor, in_dims: Shape, out_dims: Shape):
 #     """
 #     Bakes dimensions non-instance dimensions of the non-zero values in `matrix` into the sparsity pattern.
 #     The number of values stays unchanged but the number of indices increases.
@@ -1161,15 +1188,15 @@
 #             # for idx in dims.meshgrid():
 #             #     if any(i != 0 for i in idx.values()):
 #             #         offset = wrap([*idx.values()] * 2 + [0] * non_instance(matrix._indices).volume, channel(indices))
 #             #         all_indices.append(indices + offset)
 #             # indices = concat(all_indices, instance(indices))
 #             # values = pack_dims(matrix._values, concat_shapes(dims, instance(matrix._values)), instance(matrix._values))
 #             dense_shape = in_dims & matrix._dense_shape & out_dims
-#             return SparseCoordinateTensor(indices, values, dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._default)
+#             return SparseCoordinateTensor(indices, values, dense_shape, matrix._can_contain_double_entries, matrix._indices_sorted, matrix._indices_constant)
 #     raise NotImplementedError
 
 
 def with_sparsified_dim(indices: Tensor, values: Tensor, dims: Shape):
     if indices.sparse_idx.item_names == dims.names and dims.only(values.shape).is_empty:
         return indices, values
     assert indices.sparse_idx.item_names in dims, f"dims must include all sparse dims {dims} but got {indices.sparse_idx.item_names}"
@@ -1220,15 +1247,15 @@
             remaining_sparse_dims = value._dense_shape.without(dims)
             indices = value._indices.sparse_idx[remaining_sparse_dims.names]
             if remaining_sparse_dims.rank == 1:  # return dense result
                 result = scatter(value.shape.without(dims), indices, value._values, mode=mode, outside_handling='undefined')
                 return result
             elif dims.as_instance() in value._values.shape:  # We sum the output batch but keep the input.
                 dense_shape = value._dense_shape.without(dims)
-                return SparseCoordinateTensor(indices, value._values, dense_shape, value._can_contain_double_entries, value._indices_sorted, value._default)
+                return SparseCoordinateTensor(indices, value._values, dense_shape, value._can_contain_double_entries, value._indices_sorted, value._indices_constant)
             else:  # return sparse result
                 keep_sparse = sparse_dims(value).without(dims)
                 value = pack_dims(value, keep_sparse, channel('_not_summed'))
                 summed = sparse_reduce(value, dims, mode)
                 return unpack_dim(summed, '_not_summed', keep_sparse)
     raise ValueError(value)
 
@@ -1263,15 +1290,15 @@
         values_nat = b.batched_bincount(u_ptr[None, :], weights=batched_values, bins=num_entries)
         values = wrap(values_nat, non_instance(values), instance('sp_entries'))
     else:
         values = b.bincount(u_ptr, weights=values.native(), bins=num_entries)
         values = reshaped_tensor(values, [instance('sp_entries')])
     idx_packed = b.unravel_index(u_idx, dims.sizes)
     indices = wrap(idx_packed, instance('sp_entries'), channel(matrix._indices))
-    return SparseCoordinateTensor(indices, values, matrix._dense_shape, False, True, matrix._default)
+    return SparseCoordinateTensor(indices, values, matrix._dense_shape, False, True, matrix._indices_constant)
 
 
 def sparse_gather(matrix: Tensor, indices: Tensor):
     if isinstance(matrix, CompressedSparseMatrix):
         indexed = channel(indices).item_names[0]
         if matrix._uncompressed_dims.only(indexed):
             matrix = matrix.decompress()
@@ -1305,9 +1332,9 @@
             rows = b.unravel_index(rows, non_channel(indices).non_batch.sizes)
             rows = wrap(rows, instance('sp_entries'), channel(sparse_idx=non_channel(indices).names))
             gathered_indices = concat([rows, gathered_cols], 'sparse_idx')
         else:
             gathered_indices = gathered_cols
         gathered_values = matrix._values[lookup]
         dense_shape = matrix._dense_shape.without(channel(indices).item_names[0]) & non_channel(indices)
-        return SparseCoordinateTensor(gathered_indices, gathered_values, dense_shape, can_contain_double_entries=False, indices_sorted=False, default=matrix._default)
+        return SparseCoordinateTensor(gathered_indices, gathered_values, dense_shape, can_contain_double_entries=False, indices_sorted=False, indices_constant=matrix._indices_constant)
     raise NotImplementedError
```

### Comparing `phiml-1.5.0/phiml/math/_tensors.py` & `phiml-1.5.1/phiml/math/_tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1227,19 +1227,19 @@
         slices = [slice(None) if dim in self._native_shape else None for dim in order]
         expanded = transposed[tuple(slices)]
         if not singleton_for_const:
             multiples = [self._shape.get_size(dim) if dim in self._shape and dim not in self._native_shape else 1 for dim in order]
             expanded = backend.tile(expanded, multiples)
         return expanded
 
-    def _cache(self):
+    def _contiguous(self):
         if self._shape == self._native_shape:
-            return
-        self._native = self.native(order=self._shape)
-        self._native_shape = self._shape
+            return self
+        expanded = self.native(order=self._shape)
+        return NativeTensor(expanded, self._shape, self._shape)
 
     def _cached(self, dims: Shape = None) -> 'NativeTensor':
         if self._native_shape == self._shape:  # nothing to expand
             return self
         elif dims is None or self._shape in (dims & self._native_shape):  # expand all
             return NativeTensor(self.native(order=self._shape), self._shape, self._shape)
         else:  # expand specific dims
@@ -1366,89 +1366,78 @@
         self._stack_dim = stack_dim.with_sizes([len(components)], keep_item_names=True)
         try:
             merge_shapes(*self._tensors)
             self._varying_shapes = False
         except IncompatibleShapes:
             self._varying_shapes = True
         self._shape = shape_stack(self._stack_dim, *[t.shape for t in self._tensors])
-        self._cached = None
 
     @property
     def _is_tracer(self) -> bool:
         return any([t._is_tracer for t in self._tensors])
 
     @property
     def requires_broadcast(self):
         return self._varying_shapes or not self._shape.well_defined or self._is_tracer or self._tensors[0].shape.is_non_uniform
     
     @property
     def stack_dim(self):
         warnings.warn("TensorStack.stack_dim is deprecated. Use Shape.non_uniform instead.", DeprecationWarning, stacklevel=2)
         return self._stack_dim
 
-    def _cache(self):
-        if self._cached is None:
-            if self.requires_broadcast:
-                return None
-            elif all([t.shape.is_uniform for t in self._tensors]):
-                natives = [t.native(order=self._shape.names) for t in self._tensors]
-                native = choose_backend(*natives).concat(natives, axis=self.shape.index(self._stack_dim.name))
-                self._cached = NativeTensor(native, self._shape)
-            else:  # cache stack_dim on inner tensors
-                non_uniform_dim = self._tensors[0].shape.shape.without('dims')
-                if len(non_uniform_dim) > 1:
-                    raise NotImplementedError
-                unstacked = [t._unstack(non_uniform_dim.name) for t in self._tensors]
-                stacked = []
-                for to_stack in zip(*unstacked):
-                    tensor = TensorStack(to_stack, self._stack_dim)._cache()
-                    stacked.append(tensor)
-                self._cached = TensorStack(stacked, non_uniform_dim)
-        return self._cached
+    def _contiguous(self):
+        if self.requires_broadcast:
+            return None
+        elif all([t.shape.is_uniform for t in self._tensors]):
+            natives = [t.native(order=self._shape.names) for t in self._tensors]
+            native = choose_backend(*natives).concat(natives, axis=self.shape.index(self._stack_dim.name))
+            return NativeTensor(native, self._shape)
+        else:  # cache stack_dim on inner tensors
+            non_uniform_dim = self._tensors[0].shape.shape.without('dims')
+            if len(non_uniform_dim) > 1:
+                raise NotImplementedError
+            unstacked = [t._unstack(non_uniform_dim.name) for t in self._tensors]
+            stacked = []
+            for to_stack in zip(*unstacked):
+                tensor = TensorStack(to_stack, self._stack_dim)._contiguous()
+                stacked.append(tensor)
+            return TensorStack(stacked, non_uniform_dim)
 
     @property
     def dtype(self):
         return combine_types(*[t.dtype for t in self._tensors])
 
     @property
     def shape(self):
         return self._shape
 
     def native(self, order: Union[str, tuple, list, Shape] = None, singleton_for_const=False):
-        if self._cached is not None:
-            return self._cached.native(order=order)
-        else:
-            order = parse_dim_order(order, check_rank=self.rank)
-            # Is only the stack dimension shifted?
-            if order is not None and self._shape.without(self._stack_dim).names == tuple(filter(lambda name: name != self._stack_dim.name, order)):
-                inner_order = [dim for dim in order if dim != self._stack_dim.name]
-                natives = [t.native(inner_order) for t in self._tensors]
-                assert self._stack_dim.name in order, f"Dimension {self._stack_dim} missing from 'order'. Got {order} but tensor has shape {self.shape}."
-                native = choose_backend(*natives).stack(natives, axis=order.index(self._stack_dim.name))
-                return native
-            assert not self.shape.is_non_uniform, f"Cannot convert non-uniform tensor with shape {self.shape} to native tensor."
-            return self._cache().native(order=order)
+        order = parse_dim_order(order, check_rank=self.rank)
+        # Is only the stack dimension shifted?
+        if order is not None and self._shape.without(self._stack_dim).names == tuple(filter(lambda name: name != self._stack_dim.name, order)):
+            inner_order = [dim for dim in order if dim != self._stack_dim.name]
+            natives = [t.native(inner_order) for t in self._tensors]
+            assert self._stack_dim.name in order, f"Dimension {self._stack_dim} missing from 'order'. Got {order} but tensor has shape {self.shape}."
+            native = choose_backend(*natives).stack(natives, axis=order.index(self._stack_dim.name))
+            return native
+        assert not self.shape.is_non_uniform, f"Cannot convert non-uniform tensor with shape {self.shape} to native tensor."
+        return self._contiguous().native(order=order)
 
     def _with_shape_replaced(self, new_shape: Shape):
-        if self._cached is not None:
-            return self._cached._with_shape_replaced(new_shape)
-        else:
-            new_stack_dim = new_shape[self._shape.index(self._stack_dim.name)]
-            new_tensors = []
-            for t in self._tensors:
-                inner_indices = [self.shape.index(d) for d in t.shape.names]
-                new_inner_shape = new_shape[inner_indices]
-                new_tensors.append(t._with_shape_replaced(new_inner_shape))
-            return TensorStack(new_tensors, new_stack_dim)
+        new_stack_dim = new_shape[self._shape.index(self._stack_dim.name)]
+        new_tensors = []
+        for t in self._tensors:
+            inner_indices = [self.shape.index(d) for d in t.shape.names]
+            new_inner_shape = new_shape[inner_indices]
+            new_tensors.append(t._with_shape_replaced(new_inner_shape))
+        return TensorStack(new_tensors, new_stack_dim)
 
     def _getitem(self, selection: dict):
-        if self._cached is not None:
-            return self._cached._getitem(selection)
         if (self._stack_dim.name not in selection or len(selection) != 1) and not self.requires_broadcast:
-            return self._cache()._getitem(selection)
+            return self._contiguous()._getitem(selection)
         # --- Inner dims ---
         inner_dict = {dim: sel for dim, sel in selection.items() if dim != self._stack_dim.name}
         tensors = self._tensors
         if len(inner_dict) > 0:
             tensors = [t[inner_dict] for t in tensors]
         # --- stack dimension ---
         if self._stack_dim.name in selection:
@@ -1459,31 +1448,29 @@
                 return TensorStack(tensors[selection], self._stack_dim)
             else:
                 raise NotImplementedError(f"{type(selection)} not supported. Only (int, slice) allwoed")
         else:
             return TensorStack(tensors, self._stack_dim)
 
     def _unstack(self, dim):
-        if self._cached is not None:
-            return self._cached._unstack(dim)
         if dim == self._stack_dim.name:
             return self._tensors
         else:
             if self.requires_broadcast:
                 unstacked = [t._unstack(dim) for t in self._tensors]
                 return tuple([TensorStack(items, self._stack_dim) for items in zip(*unstacked)])
             else:
-                return self._cache()._unstack(dim)
+                return self._contiguous()._unstack(dim)
 
     def _op1(self, native_function):
         if self.requires_broadcast:
             tensors = [t._op1(native_function) for t in self._tensors]
             return TensorStack(tensors, self._stack_dim)
         else:
-            return self._cache()._op1(native_function)
+            return self._contiguous()._op1(native_function)
 
     def _op2(self, other, operator, native_function, op_name: str = 'unknown', op_symbol: str = '?'):
         other = self._tensor(other)
         if self.requires_broadcast:
             if self._stack_dim.name in other.shape:
                 other_slices = other._unstack(self._stack_dim.name)
                 tensors = [operator(t1, t2) for t1, t2 in zip(self._tensors, other_slices)]
@@ -1501,46 +1488,34 @@
             else:
                 tensors = [operator(self, t) for t in other._tensors]
             return TensorStack(tensors, self._stack_dim)
         else:
             return NotImplemented
 
     def _natives(self) -> tuple:
-        if self._cached is not None:
-            return self._cached._natives()
-        else:
-            return sum([t._natives() for t in self._tensors], ())
+        return sum([t._natives() for t in self._tensors], ())
 
     def _spec_dict(self) -> dict:
-        if self._cached is not None:
-            return self._cached._spec_dict()
-        else:
-            return {'type': TensorStack, 'stack_dim': self._stack_dim, 'tensors': [t._spec_dict() for t in self._tensors]}
+        return {'type': TensorStack, 'stack_dim': self._stack_dim, 'tensors': [t._spec_dict() for t in self._tensors]}
 
     @classmethod
     def _from_spec_and_natives(cls, spec: dict, natives: list):
         tensors = [t['type']._from_spec_and_natives(t, natives) for t in spec['tensors']]
         return TensorStack(tensors, spec['stack_dim'])
 
     def _with_natives_replaced(self, natives: list):
-        if self._cached is not None:
-            return self._cached._with_natives_replaced(natives)
-        else:
-            tensors = [t._with_natives_replaced(natives) for t in self._tensors]
-            return TensorStack(tensors, self._stack_dim)
+        tensors = [t._with_natives_replaced(natives) for t in self._tensors]
+        return TensorStack(tensors, self._stack_dim)
 
     @property
     def is_cached(self):
-        return self._cached is not None
+        return False
 
     def _simplify(self):
-        if self.is_cached:
-            return self._cached
-        else:
-            return self
+        return self
 
 
 def tensor(data,
            *shape: Shape,
            convert: bool = True,
            default_list_dim=channel('vector')) -> Tensor:  # TODO assume convert_unsupported, add convert_external=False for constants
     """
@@ -1947,27 +1922,25 @@
 
 def cached(t: TensorOrTree) -> TensorOrTree:
     from ._sparse import SparseCoordinateTensor, CompressedSparseMatrix
     assert isinstance(t, (Tensor, PhiTreeNode)), f"All arguments must be Tensors but got {type(t)}"
     if isinstance(t, NativeTensor):
         return t._cached()
     elif isinstance(t, TensorStack):
-        if t._cached is not None:
-            return t._cached
         inners = cached(t._tensors)
         if t.requires_broadcast:
             return TensorStack(inners, t._stack_dim)
         else:
             natives = [t.native(order=t.shape.names) for t in inners]
             native = choose_backend(*natives).stack(natives, axis=t.shape.index(t._stack_dim.name))
             return NativeTensor(native, t.shape)
     elif isinstance(t, SparseCoordinateTensor):
-        return SparseCoordinateTensor(cached(t._indices), cached(t._values), t._dense_shape, t._can_contain_double_entries, t._indices_sorted, t._default)
+        return SparseCoordinateTensor(cached(t._indices), cached(t._values), t._dense_shape, t._can_contain_double_entries, t._indices_sorted, t._indices_constant)
     elif isinstance(t, CompressedSparseMatrix):
-        return CompressedSparseMatrix(cached(t._indices), cached(t._pointers), cached(t._values), t._uncompressed_dims, t._compressed_dims, t._default, t._uncompressed_offset, t._uncompressed_indices, t._uncompressed_indices_perm)
+        return CompressedSparseMatrix(cached(t._indices), cached(t._pointers), cached(t._values), t._uncompressed_dims, t._compressed_dims, t._indices_constant, t._uncompressed_offset, t._uncompressed_indices, t._uncompressed_indices_perm)
     elif isinstance(t, Layout):
         return t
     elif isinstance(t, PhiTreeNode):
         tree, tensors = disassemble_tree(t, cache=True)
         return assemble_tree(tree, tensors)
     else:
         raise AssertionError(f"Cannot cache {type(t)} {t}")
```

### Comparing `phiml-1.5.0/phiml/math/_trace.py` & `phiml-1.5.1/phiml/math/_trace.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import numpy as np
 from scipy.sparse import csr_matrix
 
 from ..backend import choose_backend, NUMPY, Backend
 from ._ops import choose_backend_t, concat_tensor, scatter, zeros_like
 from ._shape import Shape, parse_dim_order, merge_shapes, spatial, instance, batch, concat_shapes, EMPTY_SHAPE, dual, channel, non_batch, primal, non_channel, DEBUG_CHECKS
 from ._magic_ops import stack, expand, rename_dims, unpack_dim, unstack, value_attributes
-from ._tensors import Tensor, wrap, disassemble_tree, disassemble_tensors, assemble_tree, TensorStack, may_vary_along, discard_constant_dims, variable_shape
+from ._tensors import Tensor, wrap, disassemble_tree, disassemble_tensors, assemble_tree, TensorStack, may_vary_along, \
+    discard_constant_dims, variable_shape, NativeTensor
 from ._sparse import SparseCoordinateTensor, is_sparse, sparse_dims, same_sparsity_pattern, sparse_tensor, stored_indices, stored_values, add_sparse_batch_dim
 from . import _ops as math
 from ..backend._dtype import combine_types
 
 TracerSource = namedtuple('TracerSource', ['shape', 'dtype', 'name', 'index'])
 
 
@@ -396,21 +397,21 @@
         shape = self._shape.without(channel(indices).item_names[0]) & non_channel(indices)
         return SparseLinTracer(self._source, matrix, bias, shape)
 
     def _scatter(self, base: Tensor, indices: Tensor) -> Tensor:
         full_shape = base.shape
         add_bias = discard_constant_dims(base)
         min_shape = base.shape.only(channel(indices).item_names[0])
-        row_dims = self._matrix.sparse_dims.only(self._shape)
-        col_dims = self._matrix.sparse_dims.only([n for n in self._matrix.sparse_dims.names if n.endswith('_src')])
+        row_dims = sparse_dims(self._matrix).only(self._shape)
+        col_dims = sparse_dims(self._matrix).only([n for n in self._matrix.sparse_dims.names if n.endswith('_src')])
         rows = rename_dims(indices[self._matrix._indices[row_dims.name_list]], channel, 'sparse_idx')
         cols = self._matrix._indices[col_dims.name_list]
         transformed_indices = concat_tensor([rows, cols], 'sparse_idx')
-        dense_shape = self._matrix.sparse_dims.without(row_dims) & min_shape
-        matrix = SparseCoordinateTensor(transformed_indices, self._matrix._values, dense_shape, can_contain_double_entries=True, indices_sorted=False, default=self._matrix._default)
+        dense_shape = sparse_dims(self._matrix).without(row_dims) & min_shape
+        matrix = SparseCoordinateTensor(transformed_indices, self._matrix._values, dense_shape, can_contain_double_entries=True, indices_sorted=False, indices_constant=True)
         bias = scatter(min_shape, indices, self._bias, outside_handling='undefined') + add_bias
         return SparseLinTracer(self._source, matrix, bias, full_shape)
 
     def __neg__(self):
         return SparseLinTracer(self._source, -self._matrix, -self._bias, self._shape)
 
     def _op1(self, native_function):
@@ -429,15 +430,18 @@
         other = self._tensor(other)
         assert op_symbol in '+-*/', f"Unsupported operation encountered while tracing linear function: {native_function}"
         if other._is_tracer and not isinstance(other, SparseLinTracer):
             other = to_sparse_tracer(other, self)
         if isinstance(other, SparseLinTracer):
             assert op_symbol in '+-', f"Non-linear operation '{op_symbol}' cannot be converted to matrix"
             bias = operator(self._bias, other._bias)
-            matrix = operator(self._matrix, other._matrix)  # ToDo if other has no dependence on vector, it would also be in the output
+            matrix_dims = sparse_dims(self._matrix) & sparse_dims(other._matrix)
+            self_matrix = expand_matrix(self._matrix, matrix_dims)
+            other_matrix = expand_matrix(other._matrix, matrix_dims)
+            matrix = operator(self_matrix, other_matrix)  # ToDo if other has no dependence on vector, it would also be in the output
             shape = self._shape & other._shape
             return SparseLinTracer(self._source, matrix, bias, shape)
         else:
             # other = self._tensor(other)
             if op_symbol in '*/':
                 matrix = operator(self._matrix, other)
                 bias = operator(self._bias, other)
@@ -497,15 +501,15 @@
                 biases.append(expand(discard_constant_dims(t), t.shape[dim]))
             offset += t.shape[dim]
         full_bias = math.concat(biases, dim, expand_values=True)
         indices = concat_tensor(indices, 'entries')
         values = concat_tensor(values, 'entries')
         can_contain_double_entries = any([t._matrix._can_contain_double_entries for t in tracers if t._is_tracer])
         dense_shape = any_tracer._matrix._dense_shape.with_dim_size(dim, full_size)
-        matrix = sparse_tensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted=False, default=any_tracer._matrix._default)
+        matrix = sparse_tensor(indices, values, dense_shape, can_contain_double_entries, indices_sorted=False, indices_constant=True)
         return SparseLinTracer(any_tracer._source, matrix, full_bias, shape)
     elif any(isinstance(t, GatherLinTracer) for t in tracers):
         tracers = [to_gather_tracer(t) if t._is_tracer else t for t in tracers]
         any_tracer = [t for t in tracers if t._is_tracer][0]
         src_dim = any_tracer._renamed.get(dim, dim)
         selection_dims = set(sum([channel(t._selection).item_names[0] for t in tracers if t._is_tracer and t._selection is not None], ()))
         if not selection_dims:
@@ -637,15 +641,15 @@
         bias = stack(biases, tracer._stack_dim)
         if not separate_independent:
             indices = [math.concat_tensor([m._indices, expand(i, instance(m._indices), channel(sparse_idx=tracer._stack_dim.name))], 'sparse_idx') for i, m in enumerate(matrices)]
             indices = math.concat_tensor(indices, 'entries')
             values = math.concat_tensor([m._values for m in matrices], 'entries')
             # matrix = stack(matrices, tracer._stack_dim)
             dense_shape = concat_shapes(matrices[0]._dense_shape, tracer._stack_dim)
-            matrix = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, default=0)
+            matrix = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, indices_constant=True)
         else:
             matrix = stack(matrices, tracer._stack_dim)
         return matrix, bias
     elif not tracer._is_tracer:  # This part of the output is independent of the input
         return expand(0, tracer.shape), tracer
     assert isinstance(tracer, ShiftLinTracer), f"Tracing linear function returned an unsupported construct: {type(tracer)}"
     pattern_dims = tracer._source.shape.only(pattern_dim_names(tracer))
@@ -682,15 +686,15 @@
                 src_idx_all.append(src_idx[out_shape.index(out_dim)])
         src_indices.append(src_idx_all)
     indices_np = np.concatenate([np.concatenate(src_indices, axis=1), np.concatenate(out_indices, axis=1)]).T
     indices = wrap(indices_np, instance('entries'), channel(sparse_idx=(sliced_src_shape if separate_independent else src_shape).names + out_shape.names))
     backend = choose_backend(*values)
     values = math.reshaped_tensor(backend.concat(values, axis=-1), [batch_val, instance('entries')], convert=False)
     dense_shape = concat_shapes((sliced_src_shape if separate_independent else src_shape) & out_shape)
-    matrix = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, default=0)
+    matrix = SparseCoordinateTensor(indices, values, dense_shape, can_contain_double_entries=False, indices_sorted=False, indices_constant=True)
     return matrix, tracer._bias
 
 
 def matrix_dims_for_tracer(tracer: Union[ShiftLinTracer, SparseLinTracer], sparsify_batch: bool):
     renamed_src_names = [o for n, o in tracer._out_name_to_original.items() if n != o]
     removed_dims = tracer._source.shape.without(tracer.shape).without(renamed_src_names)  # these were sliced off
     ignored_dims = tracer._source.shape.without(dependent_out_dims(tracer) if sparsify_batch else pattern_dim_names(tracer)).without(removed_dims).without(renamed_src_names)  # these will be parallelized and not added to the matrix
@@ -735,15 +739,15 @@
     Bias dimensions do not require a batched matrix but are subtracted from the right-hand-side vector.
     They are not included unless also relevant to the matrix.
     """
     if isinstance(tracer, ShiftLinTracer):
         bias_dims = set(variable_shape(tracer._bias).names)
         names = pattern_dim_names(tracer) | set(sum([t.shape.names for t in tracer.val.values()], ())) | bias_dims
         result = tracer.shape.only(names)
-        assert len(result) == len(names)
+        assert len(result) == len(names), f"Tracer was modified along {names} but the dimensions {names - set(result.names)} are not present anymore, probably due to slicing. Make sure the linear function output retains all dimensions relevant to the linear operation."
         return result
     elif isinstance(tracer, GatherLinTracer):
         result = tracer._diag.shape
         if tracer._selection is not None:
             result &= tracer._selection.shape.non_channel
         return result
     elif isinstance(tracer, SparseLinTracer):
@@ -788,21 +792,40 @@
         cols = rename_dims(tracer._selection, non_channel, instance)
     in_dims = rename_dims(in_dims, in_dims, [n + "_src" for n in in_dims.names])
     cols = rename_dims(cols, channel, channel(sparse_idx=in_dims))
     gather_dims = cols.shape.non_channel
     rows = math.meshgrid(gather_dims, stack_dim=channel(sparse_idx=out_dims))
     indices = concat_tensor([rows, cols], 'sparse_idx')
     dense_shape = in_dims & out_dims
-    matrix = sparse_tensor(indices, rename_dims(tracer._diag, indices.shape.non_channel.non_batch, instance), dense_shape, can_contain_double_entries=False, indices_sorted=False, format='coo', default=0)
+    matrix = sparse_tensor(indices, rename_dims(tracer._diag, indices.shape.non_channel.non_batch, instance), dense_shape, can_contain_double_entries=False, indices_sorted=False, format='coo', indices_constant=True)
     # ToDo check renaming
     return SparseLinTracer(tracer._source, matrix, tracer._bias, tracer._shape)
 
 
 def to_gather_tracer(t: Tensor) -> GatherLinTracer:
     if isinstance(t, GatherLinTracer):
         return t
     if isinstance(t, SparseLinTracer):
         raise AssertionError
     assert isinstance(t, ShiftLinTracer)
     if len(t.val) > 1 or next(iter(t.val)):
         raise NotImplementedError(f"Converting off-diagonal elements to sparse tracer not supported")
     return GatherLinTracer(t._source, t.val[EMPTY_SHAPE], t._bias, t._shape, None, t._renamed)
+
+
+def expand_matrix(matrix: Tensor, dims: Shape) -> Tensor:
+    """Add missing dims as diagonals"""
+    if dims in matrix.shape:
+        return matrix
+    missing = dims.without(matrix.shape)
+    src_dims = [d for d in missing if d.name.startswith('~') and d.name.endswith('_src')]
+    out_dims = [d.name[1:-4] for d in src_dims]
+    out_dims = [missing[d] for d in out_dims]
+    if isinstance(matrix, NativeTensor):
+        if len(src_dims) > 1:
+            raise NotImplementedError
+        for src_dim, out_dim in zip(src_dims, out_dims):
+            assert src_dim.size == out_dim.size
+            diagonal_idx = expand(math.arange(instance(diagonal_entries=src_dim.size)), channel(sparse_idx=[src_dim.name, out_dim.name]))
+            values = math.ones(instance(diagonal_entries=src_dim.size))
+            return sparse_tensor(diagonal_idx, values, missing, can_contain_double_entries=False, indices_sorted=True, indices_constant=True)
+    raise NotImplementedError
```

### Comparing `phiml-1.5.0/phiml/math/extrapolation.py` & `phiml-1.5.1/phiml/math/extrapolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
                 else:
                     result_native = value._native
                 if result_native is not NotImplemented:
                     return NativeTensor(result_native, value._native_shape.after_pad(widths), value._shape.after_pad(widths))
             return Extrapolation.pad(self, value, widths, already_padded=already_padded, **kwargs)
         elif isinstance(value, TensorStack):
             if not value.requires_broadcast:
-                return self.pad(value._cache(), widths)
+                return self.pad(value._contiguous(), widths)
             inner_widths = {dim: w for dim, w in widths.items() if dim != value._stack_dim.name}
             tensors = [self[{value._stack_dim.name: i}].pad(t, inner_widths) for i, t in enumerate(value.dimension(value._stack_dim.name))]
             return TensorStack(tensors, value._stack_dim)
         else:
             return Extrapolation.pad(self, value, widths, already_padded=already_padded, **kwargs)
 
     def pad_values(self, value: Tensor, width: int, dim: str, upper_edge: bool, already_padded: Optional[dict] = None, **kwargs) -> Tensor:
@@ -460,15 +460,15 @@
             else:
                 result_native = value._native
             if result_native is not NotImplemented:
                 return NativeTensor(result_native, value._native_shape.after_pad(widths), value._shape.after_pad(widths))
             return Extrapolation.pad(self, value, widths)
         elif isinstance(value, TensorStack):
             if not value.requires_broadcast:
-                return self.pad(value._cache(), widths)
+                return self.pad(value._contiguous(), widths)
             inner_widths = {dim: w for dim, w in widths.items() if dim != value._stack_dim.name}
             tensors = [self.pad(t, inner_widths) for t in value.dimension(value._stack_dim.name)]
             return TensorStack(tensors, value._stack_dim)
         elif isinstance(value, ShiftLinTracer):
             return self._pad_linear_tracer(value, widths)
         else:
             raise NotImplementedError(f'{type(value)} not supported')
```

### Comparing `phiml-1.5.0/phiml/math/magic.py` & `phiml-1.5.1/phiml/math/magic.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml/nn.py` & `phiml-1.5.1/phiml/nn.py`

 * *Files identical despite different names*

### Comparing `phiml-1.5.0/phiml.egg-info/SOURCES.txt` & `phiml-1.5.1/phiml.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 phiml/VERSION
 phiml/__init__.py
 phiml/_troubleshoot.py
```

### Comparing `phiml-1.5.0/setup.py` & `phiml-1.5.1/setup.py`

 * *Files identical despite different names*

