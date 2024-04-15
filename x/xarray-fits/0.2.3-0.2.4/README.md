# Comparing `tmp/xarray_fits-0.2.3.tar.gz` & `tmp/xarray_fits-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_fits-0.2.3.tar", max compression
+gzip compressed data, was "xarray_fits-0.2.4.tar", max compression
```

## Comparing `xarray_fits-0.2.3.tar` & `xarray_fits-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1565 2024-03-22 11:37:15.212084 xarray_fits-0.2.3/LICENSE
--rw-r--r--   0        0        0     1598 2024-03-22 11:37:15.212084 xarray_fits-0.2.3/README.rst
--rw-r--r--   0        0        0      952 2024-03-22 11:37:15.216084 xarray_fits-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      211 2024-03-22 11:37:15.216084 xarray_fits-0.2.3/xarrayfits/__init__.py
--rw-r--r--   0        0        0     6903 2024-03-22 11:37:15.216084 xarray_fits-0.2.3/xarrayfits/fits.py
--rw-r--r--   0        0        0     1916 2024-03-22 11:37:15.216084 xarray_fits-0.2.3/xarrayfits/fits_proxy.py
--rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 xarray_fits-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1565 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/LICENSE
+-rw-r--r--   0        0        0       87 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/README.rst
+-rw-r--r--   0        0        0     1003 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/__init__.py
+-rw-r--r--   0        0        0     7954 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/fits.py
+-rw-r--r--   0        0        0     1961 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/fits_proxy.py
+-rw-r--r--   0        0        0     2123 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/grid.py
+-rw-r--r--   0        0        0      221 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/typing.py
+-rw-r--r--   0        0        0     2947 2024-04-15 15:31:01.791651 xarray_fits-0.2.4/xarrayfits/utils.py
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 xarray_fits-0.2.4/PKG-INFO
```

### Comparing `xarray_fits-0.2.3/LICENSE` & `xarray_fits-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_fits-0.2.3/pyproject.toml` & `xarray_fits-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "xarray-fits"
-version = "0.2.3"
+version = "0.2.4"
 description = "xarray Datasets for FITS-like data"
 authors = ["Simon Perkins <simon.perkins@gmail.com>"]
 packages = [{include = "xarrayfits"}]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 astropy = "^6.0.0"
-dask = {extras = ["array"], version = "^2024.3.1"}
+dask = {extras = ["array"], version = ">= 2024.1.0, < 2024.2.0"}
 xarray = "^2024.2.0"
 pytest = {version = "^8.1.1", optional = true, extras = ["testing"]}
-distributed = {version = "^2024.3.1", optional = true, extras = ["testing"]}
+distributed = {version = ">= 2024.1.0, < 2024.2.0", optional = true, extras = ["testing"]}
 fsspec = "^2024.3.0"
 
 [tool.poetry.extras]
 testing = ["distributed", "pytest"]
 
 [tool.poetry.group.dev.dependencies]
 tbump = "^6.9.0"
@@ -35,10 +35,12 @@
     # isort
     "I001",
     "I002",
     # tidy imports
     "TID"
 ]
 
+extend-select = ["I"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xarray_fits-0.2.3/xarrayfits/fits.py` & `xarray_fits-0.2.4/xarrayfits/fits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 
 """Main module."""
 
+from collections.abc import Iterable, Sequence
 from functools import reduce
 from itertools import product
 import logging
 import os
 import os.path
-from collections.abc import Sequence
+from typing import Union
 
 import dask
 import dask.array as da
-import fsspec
-from fsspec.implementations.local import LocalFileSystem
+import fsspec  # type: ignore
+from fsspec.implementations.local import LocalFileSystem  # type: ignore
 import numpy as np
 
 import xarray as xr
 
+from xarrayfits.grid import AffineGrid
 from xarrayfits.fits_proxy import FitsProxy
+from xarrayfits.typing import HduType, ChunksType
+from xarrayfits.utils import promote_chunks, promote_hdus
 
 log = logging.getLogger("xarray-fits")
 
 
 def short_fits_file(table_name):
     """
     Returns the last part
@@ -90,17 +94,17 @@
     Returns
     -------
     :class:`dask.array.Array`
         Dask array representing the data associated
         with the ``hdu``.
     """
 
-    token = dask.base.tokenize(fits_proxy, hdu, dtype)
+    token = dask.base.tokenize(fits_proxy, shape, chunks, hdu, dtype)
     name = "-".join((short_fits_file(fits_proxy._filename), "slice", token))
-    dsk_chunks = da.core.normalize_chunks(chunks, shape)
+    dsk_chunks = da.core.normalize_chunks(chunks, shape, dtype=dtype)
 
     # Produce keys and slices
     keys = product([name], *[list(range(len(bd))) for bd in dsk_chunks])
     slices_ = product(*[slices(tuple(ranges(c))) for c in dsk_chunks])
     dt = np.dtype(dtype)
 
     # Create dask graph
@@ -110,110 +114,141 @@
     }
 
     return da.Array(dsk, name, dsk_chunks, dtype)
 
 
 def array_from_fits_hdu(
     fits_proxy,
-    prefix,
     hdu_list,
     hdu_index,
+    hdu_name,
     chunks,
+    singleton,
 ):
     """
     Parameters
     ----------
     fits_proxy : FitsProxy
         The FITS proxy
     hdu_list : :class:`astropy.io.fits.hdu.hdulist.HDUList`
         FITS HDU list
     hdu_index : integer
         HDU index for which to generate an :class:`xarray.DataArray`
+    hdu_name : str
+        HDU name
     chunks : list of dictionaries
+    singleton : bool
+        True if only a single hdu is selected.
+        If False, dimensions will be suffixed with hdu indices
 
     Returns
     -------
     :class:`xarray.DataArray`
         Array associated with ``hdu_index``
     """
 
     try:
         hdu = hdu_list[hdu_index]
     except IndexError as e:
         raise IndexError(f"Invalid hdu {hdu_index}") from e
 
-    naxis = hdu.header["NAXIS"]
-    bitpix = hdu.header["BITPIX"]
-    simple = hdu.header["SIMPLE"]
+    try:
+        is_simple = hdu.header["SIMPLE"] is True
+    except KeyError:
+        try:
+            ext = hdu.header["XTENSION"]
+        except KeyError:
+            raise ValueError(
+                f"Neither SIMPLE of XTENSION header card is present"
+            ) from e
+        else:
+            if ext != "IMAGE":
+                raise ValueError(f"{ext} XTENSION is not supported")
+    else:
+        if not is_simple:
+            raise ValueError(f"SIMPLE is not True")
 
-    if simple is False:
-        raise ValueError(
-            f"HDU {hdu} doesn't conform " f"to the FITS standard: " f"SIMPLE={simple}"
-        )
+    bitpix = hdu.header["BITPIX"]
 
     try:
         dtype = INV_BITPIX_MAP[bitpix]
     except KeyError:
         raise ValueError(
             f"Couldn't find a numpy type associated "
             f"with BITPIX {bitpix}. Ignoring hdu {hdu_index}"
         )
 
     shape = []
     flat_chunks = []
+    grid = AffineGrid(hdu.header)
 
-    # At this point we are dealing with FORTRAN ordered axes
-    for i in range(naxis):
-        ax_key = f"NAXIS{naxis - i}"
-        ax_shape = hdu.header[ax_key]
-        shape.append(ax_shape)
+    # Determine shapes and apply chunking
+    for d in range(grid.ndims):
+        shape.append(grid.naxis[d])
 
         try:
             # Try add existing chunking strategies to the list
-            flat_chunks.append(chunks[i])
+            flat_chunks.append(chunks[d])
         except KeyError:
-            flat_chunks.append(ax_shape)
+            flat_chunks.append(grid.naxis[d])
 
     array = generate_slice_gets(
         fits_proxy,
         hdu_index,
         tuple(shape),
         dtype,
         tuple(flat_chunks),
     )
 
-    dims = tuple(f"{prefix}{hdu_index}-{i}" for i in range(0, naxis))
+    dims = []
+
+    for d in range(grid.ndims):
+        if name := grid.name(d):
+            dim_name = name if singleton else f"{hdu_name}-{name}"
+        else:
+            dim_name = f"{hdu_name}-{d}"
+
+        dims.append(dim_name)
+
+    coords = {d: (d, grid.coords(i)) for i, d in enumerate(dims)}
     attrs = {"header": {k: v for k, v in sorted(hdu.header.items())}}
-    return xr.DataArray(array, dims=dims, attrs=attrs)
+    return xr.DataArray(array, dims=dims, coords=coords, attrs=attrs)
 
 
-def xds_from_fits(fits_filename, hdus=None, prefix="hdu", chunks=None):
+FilenameType = Union[str, Iterable[str]]
+
+
+def xds_from_fits(
+    fits_filename: FilenameType, hdus: HduType = None, chunks: ChunksType = None
+) -> Iterable[xr.Dataset]:
     """
     Parameters
     ----------
-    fits_filename : str or list of str
+    fits_filename: :code:`str` or :code:`Iterable` of :code:`str`.
         FITS filename or a list of FITS filenames.
         The first case supports a globbed pattern.
-    hdus : integer or list of integers, optional
-        hdus to represent on the returned Dataset.
-        If ``None``, all HDUs are selected
-    prefix : str, optional
-        Array name prefix
-    chunks : dictionary or list of dictionaries, optional
+    hdus : ``int`` or ``Iterable`` of ``int`` or ``str`` or ``Iterable`` of ``str`` or ``Mapping[int, str]``, optional
+        Specifies which HDUs are stored on the returned datasets.
+
+        - If ``None``, all HDUs are selected.
+        - If integers, the DataArray's will be named ``hdu{h}``, where ``h`` is the hdu index.
+        - If strings are provided, the DataArray's will be named by them.
+        - A ``Mapping[int, str]`` will name DataArry hdus at specific indices.
+    chunks : ``Mapping[str, int]`` or ``Iterable`` of ``Mapping[str, int]``, optional
         Chunking strategy for each dimension of each hdu.
         Dimensions should be specified via the
         C order dimensions
         :code:`{0: 513, 1: 513, 2: 33}`
 
     Returns
     -------
-    list of :class:`xarray.Dataset`
+    datasets: list of :class:`xarray.Dataset`
         A list of xarray Datasets corresponding to glob matches
         in the ``fits_filename`` parameter.
-        Each Dataset contains the DataArray's corresponding
+        Each Dataset contains :class:`xarray.DataArray` 's corresponding
         to each HDU on the FITS file.
     """
 
     if isinstance(fits_filename, str):
         openfiles = fsspec.open_files(fits_filename)
     elif isinstance(fits_filename, Sequence):
         openfiles = fsspec.open_files(fits_filename)
@@ -223,42 +258,31 @@
     datasets = []
 
     for of in openfiles:
         fits_proxy = FitsProxy(
             of.full_name, use_fsspec=True, memmap=isinstance(of.fs, LocalFileSystem)
         )
 
-        # Take all hdus if None specified
-        if hdus is None:
-            hdus = list(range(len(fits_proxy.hdu_list)))
-        # promote to list in case of single integer
-        elif isinstance(hdus, int):
-            hdus = [hdus]
-
-        if chunks is None:
-            chunks = [{} for _ in hdus]
-        # Promote to list in case of single dict
-        elif isinstance(chunks, dict):
-            chunks = [chunks]
+        nhdus = len(fits_proxy.hdu_list)
+        phdus = promote_hdus(hdus, nhdus)
+        pchunks = promote_chunks(chunks, len(phdus))
 
-        if not len(hdus) == len(chunks):
+        if len(phdus) > len(pchunks):
             raise ValueError(
-                f"Number of requested hdus ({len(hdus)}) "
+                f"Number of requested hdus ({len(phdus)}) "
                 f"does not match the number of "
-                f"chunks ({len(chunks)})"
+                f"chunks ({len(pchunks)})"
             )
 
+        singleton = len(phdus) == 1
+
         # Generate xarray datavars for each hdu
         xarrays = {
-            f"{prefix}{hdu_index}": array_from_fits_hdu(
-                fits_proxy,
-                prefix,
-                fits_proxy.hdu_list,
-                hdu_index,
-                hdu_chunks,
+            f"{name}": array_from_fits_hdu(
+                fits_proxy, fits_proxy.hdu_list, index, name, hdu_chunks, singleton
             )
-            for hdu_index, hdu_chunks in zip(hdus, chunks)
+            for (index, name), hdu_chunks in zip(sorted(phdus.items()), pchunks)
         }
 
         datasets.append(xr.Dataset(xarrays))
 
     return datasets
```

### Comparing `xarray_fits-0.2.3/xarrayfits/fits_proxy.py` & `xarray_fits-0.2.4/xarrayfits/fits_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from threading import Lock
 import weakref
 
-from astropy.io import fits
+from astropy.io import fits  # type: ignore
 
 TABLE_CACHE_LOCK = Lock()
-TABLE_CACHE = weakref.WeakValueDictionary()
+TABLE_CACHE: weakref.WeakValueDictionary = weakref.WeakValueDictionary()
 
 
 class FitsProxyMetaClass(type):
     """https://en.wikipedia.org/wiki/Multiton_pattern"""
 
     def __call__(cls, *args, **kwargs):
         key = (cls,) + args + tuple(set(kwargs.items()))
```

