# Comparing `tmp/trollimage-v0.4.0.tar.gz` & `tmp/trollimage-v1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trollimage-v0.4.0.tar", last modified: Tue Sep 30 18:48:23 2014, max compression, from Unix
+gzip compressed data, was "dist/trollimage-v1.0.0.tar", last modified: Mon Dec 14 12:40:15 2015, max compression
```

## Comparing `trollimage-v0.4.0.tar` & `trollimage-v1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2014-09-30 18:48:23.000000 trollimage-v0.4.0/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1711 2014-09-30 18:33:22.000000 trollimage-v0.4.0/setup.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      568 2014-09-30 18:48:23.000000 trollimage-v0.4.0/PKG-INFO
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1303 2014-09-30 18:44:26.000000 trollimage-v0.4.0/README.rst
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2014-09-30 18:48:23.000000 trollimage-v0.4.0/trollimage/
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    39844 2014-09-30 18:44:26.000000 trollimage-v0.4.0/trollimage/image.py
--rw-rw-r--   0 a001673  (62310) man         (15)      806 2013-12-04 21:21:56.000000 trollimage-v0.4.0/trollimage/__init__.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    19057 2014-09-30 18:44:26.000000 trollimage-v0.4.0/trollimage/colormap.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3883 2014-09-30 18:44:26.000000 trollimage-v0.4.0/trollimage/colorspaces.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      917 2014-09-30 18:44:26.000000 trollimage-v0.4.0/trollimage/version.py
--rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       59 2014-09-30 18:48:23.000000 trollimage-v0.4.0/setup.cfg
-drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2014-09-30 18:48:23.000000 trollimage-v0.4.0/trollimage.egg-info/
--rw-rw-r--   0 a001673  (62310) man         (15)        1 2014-09-30 18:48:22.000000 trollimage-v0.4.0/trollimage.egg-info/dependency_links.txt
--rw-rw-r--   0 a001673  (62310) man         (15)       20 2014-09-30 18:48:22.000000 trollimage-v0.4.0/trollimage.egg-info/requires.txt
--rw-rw-r--   0 a001673  (62310) man         (15)       11 2014-09-30 18:48:22.000000 trollimage-v0.4.0/trollimage.egg-info/top_level.txt
--rw-rw-r--   0 a001673  (62310) man         (15)      568 2014-09-30 18:48:22.000000 trollimage-v0.4.0/trollimage.egg-info/PKG-INFO
--rw-rw-r--   0 a001673  (62310) man         (15)        1 2013-11-27 15:30:30.000000 trollimage-v0.4.0/trollimage.egg-info/not-zip-safe
--rw-rw-r--   0 a001673  (62310) man         (15)      335 2014-09-30 18:48:23.000000 trollimage-v0.4.0/trollimage.egg-info/SOURCES.txt
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-12-14 12:40:15.000000 trollimage-v1.0.0/
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      806 2013-12-04 21:21:56.000000 trollimage-v1.0.0/trollimage/__init__.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    19271 2015-12-14 12:38:03.000000 trollimage-v1.0.0/trollimage/colormap.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     3883 2014-09-30 18:44:26.000000 trollimage-v1.0.0/trollimage/colorspaces.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)    41974 2015-12-14 12:38:03.000000 trollimage-v1.0.0/trollimage/image.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      827 2015-12-14 12:38:03.000000 trollimage-v1.0.0/trollimage/version.py
+drwxrwxr-x   0 a001673  (62310) smhiprimgrp  (2000)        0 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      581 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      345 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/SOURCES.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/dependency_links.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)        1 2013-11-27 15:30:30.000000 trollimage-v1.0.0/trollimage.egg-info/not-zip-safe
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       24 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/requires.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)       11 2015-12-14 12:40:15.000000 trollimage-v1.0.0/trollimage.egg-info/top_level.txt
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1303 2014-09-30 18:44:26.000000 trollimage-v1.0.0/README.rst
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)     1731 2015-12-14 12:38:03.000000 trollimage-v1.0.0/setup.py
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      581 2015-12-14 12:40:15.000000 trollimage-v1.0.0/PKG-INFO
+-rw-rw-r--   0 a001673  (62310) smhiprimgrp  (2000)      115 2015-12-14 12:40:15.000000 trollimage-v1.0.0/setup.cfg
```

### Comparing `trollimage-v0.4.0/setup.py` & `trollimage-v1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 version = imp.load_source('trollimage.version', 'trollimage/version.py')
 
 setup(name="trollimage",
       version=version.__version__,
       description='Pytroll imaging library',
       author='Martin Raspaud',
       author_email='martin.raspaud@smhi.se',
-      classifiers=["Development Status :: 4 - Beta",
+      classifiers=["Development Status :: 5 - Production/Stable",
                    "Intended Audience :: Science/Research",
                    "License :: OSI Approved :: GNU General Public License v3 " +
                    "or later (GPLv3+)",
                    "Operating System :: OS Independent",
                    "Programming Language :: Python",
                    "Topic :: Scientific/Engineering"],
       url="https://github.com/mraspaud/trollimage",
       packages=['trollimage'],
       zip_safe=False,
-      install_requires=['numpy >=1.4.1', 'pillow'],
+      install_requires=['numpy >=1.4.1', 'pillow', 'six'],
       test_suite = 'trollimage.tests.suite',
       )
```

### Comparing `trollimage-v0.4.0/README.rst` & `trollimage-v1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `trollimage-v0.4.0/trollimage/image.py` & `trollimage-v1.0.0/trollimage/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2009-2014
+# Copyright (c) 2009-2015
 
 # Author(s):
 
 #   Martin Raspaud <martin.raspaud@smhi.se>
 #   Adam Dybbroe <adam.dybbroe@smhi.se>
 #   Esben S. Nielsen <esn@dmi.dk>
 
@@ -26,38 +26,43 @@
 but has the advandage of using masked arrays as pixel arrays, so that data
 arrays containing invalid values may be properly handled.
 """
 
 import logging
 import os
 import re
+import six
 
 from PIL import Image as Pil
 import numpy as np
+from copy import deepcopy
 
 
 try:
     import numexpr as ne
 except ImportError:
     ne = None
 
 logger = logging.getLogger(__name__)
 
+
 def ensure_dir(filename):
     """Checks if the dir of f exists, otherwise create it.
     """
     directory = os.path.dirname(filename)
     if len(directory) and not os.path.isdir(directory):
         os.makedirs(directory)
 
 
 class UnknownImageFormat(Exception):
+
     """Exception to be raised when image format is unknown to pytroll-image"""
     pass
 
+
 def check_image_format(fformat):
     """Check that *fformat* is valid
     """
     cases = {"jpg": "jpeg",
              "jpeg": "jpeg",
              "tif": "tiff",
              "tiff": "tif",
@@ -76,15 +81,17 @@
     fformat = fformat.lower()
     try:
         fformat = cases[fformat]
     except KeyError:
         raise UnknownImageFormat("Unknown image format '%s'." % fformat)
     return fformat
 
+
 class Image(object):
+
     """This class defines images. As such, it contains data of the different
     *channels* of the image (red, green, and blue for example). The *mode*
     tells if the channels define a black and white image ("L"), an rgb image
     ("RGB"), an YCbCr image ("YCbCr"), or an indexed image ("P"), in which case
     a *palette* is needed. Each mode has also a corresponding alpha mode, which
     is the mode with an "A" in the end: for example "RGBA" is rgb with an alpha
     channel. *fill_value* sets how the image is filled where data is missing,
@@ -99,15 +106,15 @@
     classical [0,255] range and byte type is done automagically when saving the
     image to file.
     """
 
     modes = ["L", "LA", "RGB", "RGBA", "YCbCr", "YCbCrA", "P", "PA"]
 
     def __init__(self, channels=None, mode="L", color_range=None,
-                 fill_value=None, palette=None):
+                 fill_value=None, palette=None, copy=True):
 
         self.channels = None
         self.mode = None
         self.width = 0
         self.height = 0
         self.fill_value = None
         self.palette = None
@@ -120,34 +127,37 @@
            not isinstance(channels, (tuple, set, list,
                                      np.ndarray, np.ma.core.MaskedArray))):
             raise TypeError("Image channels should a tuple, set, list, numpy "
                             "array, or masked array.")
 
         if(isinstance(channels, (tuple, list)) and
            len(channels) != len(re.findall("[A-Z]", mode))):
-            raise ValueError("Number of channels does not match mode.")
+            raise ValueError("Number of channels (%s) does not match mode %s." % (len(channels), mode))
+
+        if copy and channels is not None:
+            channels = deepcopy(channels)
 
         if mode not in self.modes:
             raise ValueError("Unknown mode.")
 
         if(color_range is not None and
            not _is_pair(color_range) and
            not _is_list_of_pairs(color_range)):
             raise ValueError("Color_range should be a pair"
                              " or a list/tuple/set of pairs.")
         if(color_range is not None and
            _is_list_of_pairs(color_range) and
            (channels is None or
-             len(color_range) != len(channels))):
+                len(color_range) != len(channels))):
             raise ValueError("Color_range length does not match number of "
                              "channels.")
 
         if(color_range is not None and
            (((mode == "L" or mode == "P") and not _is_pair(color_range)) and
-             (len(color_range) != len(re.findall("[A-Z]", mode))))):
+                (len(color_range) != len(re.findall("[A-Z]", mode))))):
             raise ValueError("Color_range does not match mode")
 
         self.mode = mode
 
         if isinstance(fill_value, (tuple, list, set)):
             self.fill_value = list(fill_value)
         elif fill_value is not None:
@@ -161,27 +171,32 @@
         if isinstance(channels, (tuple, list)):
             if _areinstances(channels, (np.ma.core.MaskedArray, np.ndarray,
                                         list, tuple)):
                 for i, chn in enumerate(channels):
                     if color_range is not None:
                         color_min = color_range[i][0]
                         color_max = color_range[i][1]
+                        # Add data to image object as a channel
+                        #self._add_channel(chn, color_min, color_max)
                     else:
                         color_min = 0.0
                         color_max = 1.0
-
+                        # self.channels.append(np.ma.array(chn))
                     # Add data to image object as a channel
                     self._add_channel(chn, color_min, color_max)
 
                     self.shape = self.channels[-1].shape
                     if self.shape != self.channels[0].shape:
                         raise ValueError("Image channels must have the same"
                                          " shape.")
                 self.height = self.shape[0]
-                self.width = self.shape[1]
+                try:
+                    self.width = self.shape[1]
+                except IndexError:
+                    self.width = 0
             else:
                 raise ValueError("Image channels must all be arrays tuples.")
         elif channels is not None:
             self.height = channels.shape[0]
             self.width = channels.shape[1]
             self.shape = channels.shape
 
@@ -199,15 +214,14 @@
             self.shape = (0, 0)
             self.width = 0
             self.height = 0
 
     def _add_channel(self, chn, color_min, color_max):
         """Adds a channel to the image object
         """
-
         if isinstance(chn, np.ma.core.MaskedArray):
             chn_data = chn.data
             chn_mask = chn.mask
         else:
             chn_data = np.array(chn)
             chn_mask = False
         scaled = ((chn_data - color_min) *
@@ -229,15 +243,15 @@
             if isinstance(chn, np.ma.core.MaskedArray):
                 final_data = chn.data.clip(0, 1) * np.iinfo(dtype).max
             else:
                 final_data = chn.clip(0, 1) * np.iinfo(dtype).max
 
             channels.append(np.ma.array(final_data,
                                         dtype,
-                                        mask = np.ma.getmaskarray(chn)))
+                                        mask=np.ma.getmaskarray(chn)))
         if self.fill_value is not None:
             fill_value = [int(col * np.iinfo(dtype).max)
                           for col in self.fill_value]
         else:
             fill_value = None
         return channels, fill_value
 
@@ -245,21 +259,19 @@
         """Checks for an empty image.
         """
         if(((self.channels == []) and (not self.shape == (0, 0))) or
            ((not self.channels == []) and (self.shape == (0, 0)))):
             raise RuntimeError("Channels-shape mismatch.")
         return self.channels == [] and self.shape == (0, 0)
 
-
     def show(self):
         """Display the image on screen.
         """
         self.pil_image().show()
 
-
     def pil_image(self):
         """Return a PIL image from the current image.
         """
         channels, fill_value = self._finalize()
 
         if self.is_empty():
             return Pil.new(self.mode, (0, 0))
@@ -331,68 +343,107 @@
 
                 alpha = np.where(mask, 0, channels[3])
                 pil_a = Pil.fromarray(alpha)
 
                 img = Pil.merge("RGBA", (pil_r, pil_g, pil_b, pil_a))
 
         else:
-            raise TypeError("Does not know how to use mode %s."%(self.mode))
+            raise TypeError("Does not know how to use mode %s." % (self.mode))
 
         return img
 
-    def save(self, filename, compression=6, fformat=None):
+    def save(self, filename, compression=6, fformat=None,
+             thumbnail_name=None, thumbnail_size=None):
         """Save the image to the given *filename*. For some formats like jpg
         and png, the work is delegated to :meth:`pil_save`, which doesn't
         support the *compression* option.
         """
-        self.pil_save(filename, compression, fformat)
+        self.pil_save(filename, compression, fformat,
+                      thumbnail_name, thumbnail_size)
 
-    def pil_save(self, filename, compression=6, fformat=None):
+    def pil_save(self, filename, compression=6, fformat=None,
+                 thumbnail_name=None, thumbnail_size=None):
         """Save the image to the given *filename* using PIL. For now, the
         compression level [0-9] is ignored, due to PIL's lack of support. See
         also :meth:`save`.
         """
         # PIL does not support compression option.
         del compression
 
         if self.is_empty():
             raise IOError("Cannot save an empty image")
 
-        ensure_dir(filename)
+        if isinstance(filename, (str, six.text_type)):
+            ensure_dir(filename)
 
         fformat = fformat or os.path.splitext(filename)[1][1:4]
         fformat = check_image_format(fformat)
 
-        self.pil_image().save(filename, fformat)
+        params = {}
+
+        if fformat == 'png':
+            # Take care of GeoImage.tags (if any).
+            params['pnginfo'] = self._pngmeta()
+
+        img = self.pil_image()
+        img.save(filename, fformat, **params)
+
+        if thumbnail_name is not None and thumbnail_size is not None:
+            img.thumbnail(thumbnail_size, Pil.ANTIALIAS)
+            img.save(thumbnail_name, fformat, **params)
+
+    def _pngmeta(self):
+        """It will return GeoImage.tags as a PNG metadata object.
+
+        Inspired by:
+        public domain, Nick Galbreath
+        http://blog.modp.com/2007/08/python-pil-and-png-metadata-take-2.html
+        """
+        reserved = ('interlace', 'gamma', 'dpi', 'transparency', 'aspect')
+
+        try:
+            tags = self.tags
+        except AttributeError:
+            tags = {}
+
+        # Undocumented class
+        from PIL import PngImagePlugin
+        meta = PngImagePlugin.PngInfo()
+
+        # Copy from tags to new dict
+        for k__, v__ in tags.items():
+            if k__ not in reserved:
+                meta.add_text(k__, v__, 0)
+
+        return meta
 
     def putalpha(self, alpha):
         """Adds an *alpha* channel to the current image, or replaces it with
         *alpha* if it already exists.
         """
         alpha = np.ma.array(alpha)
         if(not (alpha.shape[0] == 0 and
                 self.shape[0] == 0) and
            alpha.shape != self.shape):
             raise ValueError("Alpha channel shape should match image shape")
 
         if not self.mode.endswith("A"):
-            self.convert(self.mode+"A")
+            self.convert(self.mode + "A")
         if not self.is_empty():
             self.channels[-1] = alpha
 
     def _rgb2ycbcr(self, mode):
         """Convert the image from RGB mode to YCbCr."""
 
         self._check_modes(("RGB", "RGBA"))
 
-
         (self.channels[0], self.channels[1], self.channels[2]) = \
-                          rgb2ycbcr(self.channels[0],
-                                    self.channels[1],
-                                    self.channels[2])
+            rgb2ycbcr(self.channels[0],
+                      self.channels[1],
+                      self.channels[2])
 
         if self.fill_value is not None:
             self.fill_value[0:3] = rgb2ycbcr(self.fill_value[0],
                                              self.fill_value[1],
                                              self.fill_value[2])
 
         self.mode = mode
@@ -400,26 +451,25 @@
     def _ycbcr2rgb(self, mode):
         """Convert the image from YCbCr mode to RGB.
         """
 
         self._check_modes(("YCbCr", "YCbCrA"))
 
         (self.channels[0], self.channels[1], self.channels[2]) = \
-                          ycbcr2rgb(self.channels[0],
-                                    self.channels[1],
-                                    self.channels[2])
+            ycbcr2rgb(self.channels[0],
+                      self.channels[1],
+                      self.channels[2])
 
         if self.fill_value is not None:
             self.fill_value[0:3] = ycbcr2rgb(self.fill_value[0],
                                              self.fill_value[1],
                                              self.fill_value[2])
 
         self.mode = mode
 
-
     def _to_p(self, mode):
         """Convert the image to P or PA mode.
         """
 
         if self.mode.endswith("A"):
             chans = self.channels[:-1]
             alpha = self.channels[-1]
@@ -427,15 +477,15 @@
         else:
             chans = self.channels
             alpha = None
             self._secondary_mode = self.mode
 
         palette = []
         selfmask = reduce(np.ma.mask_or, [chn.mask for chn in chans])
-        new_chn = np.ma.zeros(self.shape, dtype = int)
+        new_chn = np.ma.zeros(self.shape, dtype=int)
         color_nb = 0
 
         for i in range(self.height):
             for j in range(self.width):
                 current_col = tuple([chn[i, j] for chn in chans])
                 try:
                     (idx
@@ -493,15 +543,15 @@
         for i in range(len(self.palette[0])):
             cdfs.append(np.zeros(len(self.palette)))
             for j in range(len(self.palette)):
                 cdfs[i][j] = self.palette[j][i]
             new_chn = np.ma.array(np.interp(color_chan,
                                             np.arange(len(self.palette)),
                                             cdfs[i]),
-                                  mask = color_chan.mask)
+                                  mask=color_chan.mask)
             chans.append(new_chn)
 
         if self.fill_value is not None:
             if alpha is not None:
                 fill_alpha = self.fill_value[-1]
                 self.fill_value = list(self.palette[int(self.fill_value[0])])
                 self.fill_value += [fill_alpha]
@@ -512,36 +562,34 @@
         self.channels = chans
         if alpha is not None:
             self.channels.append(alpha)
             self.mode = self.mode + "A"
 
         self.convert(mode)
 
-
     def _check_modes(self, modes):
         """Check that the image is in on of the given *modes*, raise an
         exception otherwise.
         """
         if not isinstance(modes, (tuple, list, set)):
             modes = [modes]
         if self.mode not in modes:
-            raise ValueError("Image not in suitable mode: %s"%modes)
-
+            raise ValueError("Image not in suitable mode: %s" % modes)
 
     def _l2rgb(self, mode):
         """Convert from L (black and white) to RGB.
         """
         self._check_modes(("L", "LA"))
         self.channels.append(self.channels[0].copy())
         self.channels.append(self.channels[0].copy())
         if self.fill_value is not None:
             self.fill_value = self.fill_value[:1] * 3 + self.fill_value[1:]
         if self.mode == "LA":
             self.channels[1], self.channels[3] = \
-            self.channels[3], self.channels[1]
+                self.channels[3], self.channels[1]
         self.mode = mode
 
     def _rgb2l(self, mode):
         """Convert from RGB to monochrome L.
         """
         self._check_modes(("RGB", "RGBA"))
 
@@ -560,15 +608,14 @@
                                           self.fill_value[2])[0]] +
                                self.fill_value[3:])
 
         self.channels = [y__] + self.channels[3:]
 
         self.mode = mode
 
-
     def _ycbcr2l(self, mode):
         """Convert from YCbCr to L.
         """
         self._check_modes(("YCbCr", "YCbCrA"))
 
         self.channels = [self.channels[0]] + self.channels[3:]
         if self.fill_value is not None:
@@ -585,29 +632,26 @@
         zeros.mask = luma.mask
 
         self.channels = [luma, zeros, zeros] + self.channels[1:]
 
         if self.fill_value is not None:
             self.fill_value = [self.fill_value[0], 0, 0] + self.fill_value[1:]
 
-
         self.mode = mode
 
-
-
     def convert(self, mode):
         """Convert the current image to the given *mode*. See :class:`Image`
         for a list of available modes.
         """
         if mode == self.mode:
             return
 
         if mode not in ["L", "LA", "RGB", "RGBA",
                         "YCbCr", "YCbCrA", "P", "PA"]:
-            raise ValueError("Mode %s not recognized."%(mode))
+            raise ValueError("Mode %s not recognized." % (mode))
 
         if self.is_empty():
             self.mode = mode
             return
 
         if mode == self.mode + "A":
             self.channels.append(np.ma.ones(self.channels[0].shape))
@@ -649,27 +693,27 @@
                 "LA": {"RGBA": self._l2rgb,
                        "YCbCrA": self._l2ycbcr,
                        "PA": self._to_p},
                 "P": {"RGB": self._from_p,
                       "YCbCr": self._from_p,
                       "L": self._from_p},
                 "PA": {"RGBA": self._from_p,
-                      "YCbCrA": self._from_p,
-                      "LA": self._from_p}}
+                       "YCbCrA": self._from_p,
+                       "LA": self._from_p}}
             try:
                 cases[self.mode][mode](mode)
             except KeyError:
                 raise ValueError("Conversion from %s to %s not implemented !"
-                                 %(self.mode,mode))
+                                 % (self.mode, mode))
 
-    def clip(self, channels = True):
+    def clip(self, channels=True):
         """Limit the values of the array to the default [0,1] range. *channels*
         says which channels should be clipped."""
         if not isinstance(channels, (tuple, list)):
-            channels = [channels]*len(self.channels)
+            channels = [channels] * len(self.channels)
 
         for i in range(len(self.channels)):
             if channels[i]:
                 self.channels[i] = np.ma.clip(self.channels[i], 0.0, 1.0)
 
     def resize(self, shape):
         """Resize the image to the given *shape* tuple, in place. For zooming,
@@ -700,22 +744,22 @@
 
         factor[0] = int(factor[0])
         factor[1] = int(factor[1])
 
         i = 0
         for chn in self.channels:
             if zoom[0]:
-                chn = chn.repeat([factor[0]] * chn.shape[0], axis = 0)
+                chn = chn.repeat([factor[0]] * chn.shape[0], axis=0)
             else:
                 chn = chn[[idx * factor[0]
                            for idx in range(self.height / factor[0])],
                           :]
             if zoom[1]:
                 self.channels[i] = chn.repeat([factor[1]] * chn.shape[1],
-                                              axis = 1)
+                                              axis=1)
             else:
                 self.channels[i] = chn[:,
                                        [idx * factor[1]
                                         for idx in range(self.width /
                                                          factor[1])]]
 
             i = i + 1
@@ -730,15 +774,15 @@
         from that mode.
         """
         if self.is_empty():
             return
 
         if luminance.shape != self.channels[0].shape:
             if ((luminance.shape[0] * 1.0 / luminance.shape[1]) ==
-                 (self.channels[0].shape[0] * 1.0 / self.channels[0].shape[1])):
+                    (self.channels[0].shape[0] * 1.0 / self.channels[0].shape[1])):
                 if luminance.shape[0] > self.channels[0].shape[0]:
                     self.resize(luminance.shape)
                 else:
                     raise NameError("Luminance smaller than the image !")
             else:
                 raise NameError("Not the good shape !")
 
@@ -748,135 +792,133 @@
             self.channels[0] = luminance
             self.convert(mode)
         else:
             self.convert("YCbCr")
             self.channels[0] = luminance
             self.convert(mode)
 
-    def enhance(self, inverse=False, gamma=1.0, stretch="no"):
+    def enhance(self, inverse=False, gamma=1.0, stretch="no", stretch_parameters=None, **kwargs):
         """Image enhancement function. It applies **in this order** inversion,
         gamma correction, and stretching to the current image, with parameters
         *inverse* (see :meth:`Image.invert`), *gamma* (see
         :meth:`Image.gamma`), and *stretch* (see :meth:`Image.stretch`).
         """
         self.invert(inverse)
+        if stretch_parameters is None:
+            stretch_parameters = {}
+        self.stretch(stretch, **stretch_parameters)
         self.gamma(gamma)
-        self.stretch(stretch)
 
     def gamma(self, gamma=1.0):
         """Apply gamma correction to the channels of the image. If *gamma* is a
         tuple, then it should have as many elements as the channels of the
         image, and the gamma correction is applied elementwise. If *gamma* is a
         number, the same gamma correction is applied on every channel, if there
         are several channels in the image. The behaviour of :func:`gamma` is
         undefined outside the normal [0,1] range of the channels.
         """
-        if not isinstance(gamma, (int, long, float)):
-            if(not isinstance(gamma, (tuple, list, set)) or
-               not _areinstances(gamma, (int, long, float))):
-                raise TypeError("Gamma should be a real number, or an iterable "
-                                "of real numbers.")
 
         if(isinstance(gamma, (list, tuple, set)) and
            len(gamma) != len(self.channels)):
             raise ValueError("Number of channels and gamma components differ.")
-
-        if gamma < 0:
-            raise ValueError("Gamma correction must be a positive number.")
-
-        if gamma == 1.0:
-            return
         if isinstance(gamma, (tuple, list)):
             gamma_list = list(gamma)
         else:
             gamma_list = [gamma] * len(self.channels)
         for i in range(len(self.channels)):
+            gamma = float(gamma_list[i])
+            if gamma < 0:
+                raise ValueError("Gamma correction must be a positive number.")
+            logger.debug("Applying gamma %f", gamma)
+            if gamma == 1.0:
+                continue
+
             if isinstance(self.channels[i], np.ma.core.MaskedArray):
                 if ne:
                     self.channels[i] = np.ma.array(
                         ne.evaluate("data ** (1.0 / gamma)",
                                     local_dict={"data": self.channels[i].data,
-                                                'gamma': gamma_list[i]}),
+                                                'gamma': gamma}),
                         mask=self.channels[i].mask,
                         copy=False)
                 else:
                     self.channels[i] = np.ma.array(self.channels[i].data **
-                                                   (1.0 / gamma_list[i]),
+                                                   (1.0 / gamma),
                                                    mask=self.channels[i].mask,
                                                    copy=False)
             else:
                 self.channels[i] = np.where(self.channels[i] >= 0,
                                             self.channels[i] **
-                                            (1.0 / gamma_list[i]),
+                                            (1.0 / gamma),
                                             self.channels[i])
 
-    def stretch(self, stretch="crude", **kwarg):
+    def stretch(self, stretch="crude", **kwargs):
         """Apply stretching to the current image. The value of *stretch* sets
         the type of stretching applied. The values "histogram", "linear",
         "crude" (or "crude-stretch") perform respectively histogram
         equalization, contrast stretching (with 5% cutoff on both sides), and
         contrast stretching without cutoff. The value "logarithmic" or "log"
         will do a logarithmic enhancement towards white. If a tuple or a list
         of two values is given as input, then a contrast stretching is performed
         with the values as cutoff. These values should be normalized in the
         range [0.0,1.0].
         """
 
+        logger.debug("Applying stretch %s with parameters %s", stretch, str(kwargs))
+
         ch_len = len(self.channels)
         if self.mode.endswith("A"):
             ch_len -= 1
 
-
         if((isinstance(stretch, tuple) or
-             isinstance(stretch, list))):
+                isinstance(stretch, list))):
             if len(stretch) == 2:
                 for i in range(ch_len):
-                    self.stretch_linear(i, cutoffs=stretch, **kwarg)
+                    self.stretch_linear(i, cutoffs=stretch, **kwargs)
             else:
-                raise ValueError("Stretch tuple must have exactly two elements")
+                raise ValueError(
+                    "Stretch tuple must have exactly two elements")
         elif stretch == "linear":
             for i in range(ch_len):
-                self.stretch_linear(i, **kwarg)
+                self.stretch_linear(i, **kwargs)
         elif stretch == "histogram":
             for i in range(ch_len):
-                self.stretch_hist_equalize(i, **kwarg)
+                self.stretch_hist_equalize(i, **kwargs)
         elif stretch in ["crude", "crude-stretch"]:
             for i in range(ch_len):
-                self.crude_stretch(i, **kwarg)
+                self.crude_stretch(i, **kwargs)
         elif stretch in ["log", "logarithmic"]:
             for i in range(ch_len):
-                self.stretch_logarithmic(i, **kwarg)
+                self.stretch_logarithmic(i, **kwargs)
         elif stretch == "no":
             return
         elif isinstance(stretch, str):
-            raise ValueError("Stretching method %s not recognized."%stretch)
+            raise ValueError("Stretching method %s not recognized." % stretch)
         else:
             raise TypeError("Stretch parameter must be a string or a tuple.")
 
-
     def invert(self, invert=True):
-        """Inverts all the channels of a image according to *invert*. If invert
-        is a tuple or a list, elementwise invertion is performed, otherwise all
-        channels are inverted if *invert* is true (default).
+        """Inverts all the channels of a image according to *invert*. If invert is a tuple or a list, elementwise
+        invertion is performed, otherwise all channels are inverted if *invert* is true (default).
+
+        Note: 'Inverting' means that black becomes white, and vice-versa, not that the values are negated !
         """
-        if(isinstance(invert, (tuple, list, set)) and
+        if(isinstance(invert, (tuple, list)) and
            len(self.channels) != len(invert)):
-            raise ValueError("Number of channels and invert components differ.")
+            raise ValueError(
+                "Number of channels and invert components differ.")
 
-        if isinstance(invert, (tuple, list, set)):
-            i = 0
-            for chn in self.channels:
+        logger.debug("Applying invert with parameters %s", str(invert))
+        if isinstance(invert, (tuple, list)):
+            for i, chn in enumerate(self.channels):
                 if invert[i]:
-                    self.channels[i] = 1.0 - chn
-                i = i + 1
+                    self.channels[i] = 1 - chn
         elif invert:
-            i = 0
-            for chn in self.channels:
-                self.channels[i] = 1.0 - chn
-                i = i + 1
+            for i, chn in enumerate(self.channels):
+                self.channels[i] = 1 - chn
 
     def stretch_hist_equalize(self, ch_nb):
         """Stretch the current image's colors by performing histogram
         equalization on channel *ch_nb*.
         """
         logger.info("Perform a histogram equalized contrast stretch.")
 
@@ -887,45 +929,44 @@
 
         arr = self.channels[ch_nb]
 
         nwidth = 2048.0
 
         carr = arr.compressed()
 
-        cdf = np.arange(0.0, 1.0, 1/nwidth)
+        cdf = np.arange(0.0, 1.0, 1 / nwidth)
         logger.debug("Make histogram bins having equal amount of data, " +
-                  "using numpy percentile function:")
+                     "using numpy percentile function:")
         bins = np.percentile(carr, list(cdf * 100))
 
         res = np.ma.empty_like(arr)
         res.mask = np.ma.getmaskarray(arr)
         res[~res.mask] = np.interp(carr, bins, cdf)
 
         self.channels[ch_nb] = res
 
-
     def stretch_logarithmic(self, ch_nb, factor=100.):
         """Move data into range [1:factor] and do a normalized logarithmic
         enhancement.
         """
         logger.debug("Perform a logarithmic contrast stretch.")
         if ((self.channels[ch_nb].size ==
              np.ma.count_masked(self.channels[ch_nb])) or
-              (self.channels[ch_nb].min() == self.channels[ch_nb].max())):
+                (self.channels[ch_nb].min() == self.channels[ch_nb].max())):
             logger.warning("Nothing to stretch !")
             return
 
         crange = (0., 1.0)
 
         arr = self.channels[ch_nb]
         b__ = float(crange[1] - crange[0]) / np.log(factor)
         c__ = float(crange[0])
-        slope = (factor-1.)/float(arr.max() - arr.min())
-        arr = 1. + (arr - arr.min())*slope
-        arr = c__ + b__*np.log(arr)
+        slope = (factor - 1.) / float(arr.max() - arr.min())
+        arr = 1. + (arr - arr.min()) * slope
+        arr = c__ + b__ * np.log(arr)
         self.channels[ch_nb] = arr
 
     def stretch_linear(self, ch_nb, cutoffs=(0.005, 0.005)):
         """Stretch linearly the contrast of the current image on channel
         *ch_nb*, using *cutoffs* for left and right trimming.
         """
         logger.debug("Perform a linear contrast stretch.")
@@ -937,42 +978,45 @@
             return
 
         arr = self.channels[ch_nb]
         carr = arr.compressed()
 
         logger.debug("Calculate the histogram percentiles: ")
         logger.debug("Left and right percentiles: " +
-                  str(cutoffs[0]*100) + " " + str(cutoffs[1]*100))
+                     str(cutoffs[0] * 100) + " " + str(cutoffs[1] * 100))
 
-        left, right = np.percentile(carr, [cutoffs[0]*100,
-                                           100. - cutoffs[1]*100])
+        left, right = np.percentile(carr, [cutoffs[0] * 100, 100. - cutoffs[1] * 100])
 
         delta_x = (right - left)
         logger.debug("Interval: left=%f, right=%f width=%f",
-                   left, right, delta_x)
+                     left, right, delta_x)
 
         if delta_x > 0.0:
             self.channels[ch_nb] = np.ma.array((arr - left) / delta_x,
-                                               mask = arr.mask)
+                                               mask=arr.mask)
         else:
             self.channels[ch_nb] = np.ma.zeros(arr.shape)
             logger.warning("Unable to make a contrast stretch!")
 
-
     def crude_stretch(self, ch_nb, min_stretch=None, max_stretch=None):
         """Perform simple linear stretching (without any cutoff) on the channel
         *ch_nb* of the current image and normalize to the [0,1] range."""
 
         if min_stretch is None:
             min_stretch = self.channels[ch_nb].min()
         if max_stretch is None:
             max_stretch = self.channels[ch_nb].max()
 
+        if isinstance(min_stretch, (list, tuple)):
+            min_stretch = min_stretch[ch_nb]
+        if isinstance(max_stretch, (list, tuple)):
+            max_stretch = max_stretch[ch_nb]
+
         if((not self.channels[ch_nb].mask.all()) and
-            max_stretch - min_stretch > 0):
+                abs(max_stretch - min_stretch) > 0):
             stretched = self.channels[ch_nb].data.astype(np.float)
             stretched -= min_stretch
             stretched /= max_stretch - min_stretch
             self.channels[ch_nb] = np.ma.array(stretched,
                                                mask=self.channels[ch_nb].mask,
                                                copy=False)
         else:
@@ -1039,27 +1083,36 @@
         for i in range(3):
             dst.channels[i] = (src.channels[i] * src.channels[3] +
                                dst.channels[i] * dst.channels[3] *
                                (1 - src.channels[3])) / outa
             dst.channels[i][outa == 0] = 0
         dst.channels[3] = outa
 
+    def _repr_png_(self):
+        import io
+        b = io.BytesIO()
+        self.save(b, fformat="png")
+        return b.getvalue()
+
+
 def _areinstances(the_list, types):
     """Check if all the elements of the list are of given type.
     """
     return all([isinstance(item, types) for item in the_list])
 
+
 def _is_pair(item):
     """Check if an item is a pair (tuple of size 2).
     """
     return (isinstance(item, (list, tuple, set)) and
             len(item) == 2 and
             not isinstance(item[0], (list, tuple, set)) and
             not isinstance(item[1], (list, tuple, set)))
 
+
 def _is_list_of_pairs(the_list):
     """Check if a list contains only pairs.
     """
     return all([_is_pair(item) for item in the_list])
 
 
 def ycbcr2rgb(y__, cb_, cr_):
@@ -1071,19 +1124,19 @@
 
     r__ = 2 * cr_ / (1 - kr_) + y__
     b__ = 2 * cb_ / (1 - kb_) + y__
     g__ = (y__ - kr_ * r__ - kb_ * b__) / (1 - kr_ - kb_)
 
     return r__, g__, b__
 
+
 def rgb2ycbcr(r__, g__, b__):
     """Convert the three RGB channels to YCbCr."""
 
     kb_ = 0.114
     kr_ = 0.299
 
     y__ = kr_ * r__ + (1 - kr_ - kb_) * g__ + kb_ * b__
     cb_ = 1. / (2 * (1 - kb_)) * (b__ - y__)
     cr_ = 1. / (2 * (1 - kr_)) * (r__ - y__)
 
     return y__, cb_, cr_
-
```

### Comparing `trollimage-v0.4.0/trollimage/__init__.py` & `trollimage-v1.0.0/trollimage/__init__.py`

 * *Files identical despite different names*

### Comparing `trollimage-v0.4.0/trollimage/colormap.py` & `trollimage-v1.0.0/trollimage/colormap.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,30 @@
 import numpy as np
 from trollimage.colorspaces import rgb2hcl, hcl2rgb
 
 def colorize(arr, colors, values):
     """Colorize a monochromatic array *arr*, based *colors* given for
     *values*. Interpolation is used. *values* must be in ascending order.
     """
-    hcolors = np.array([rgb2hcl(*i) for i in colors])
+    hcolors = np.array([rgb2hcl(*i[:3]) for i in colors])
     # unwrap colormap in hcl space
     hcolors[:, 0] = np.rad2deg(np.unwrap(np.deg2rad(np.array(hcolors)[:, 0])))
     channels = [np.interp(arr,
                           np.array(values),
                           np.array(hcolors)[:, i])
                 for i in range(3)]
 
-    channels = hcl2rgb(*channels)
+    channels = list(hcl2rgb(*channels))
+
+    rest = [np.interp(arr,
+                      np.array(values),
+                      np.array(colors)[:, i + 3])
+            for i in range(np.array(colors).shape[1] - 3)]
+
+    channels.extend(rest)
 
     try:
         return [np.ma.array(channel, mask=arr.mask) for channel in channels]
     except AttributeError:
         return channels
 
 def palettize(arr, colors, values):
```

### Comparing `trollimage-v0.4.0/trollimage/colorspaces.py` & `trollimage-v1.0.0/trollimage/colorspaces.py`

 * *Files identical despite different names*

### Comparing `trollimage-v0.4.0/trollimage/version.py` & `trollimage-v1.0.0/trollimage/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,12 +19,8 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Version file.
 """
 
-__major__ = "0"
-__minor__ = "4"
-__patch__ = "0"
-
-__version__ = "v" + ".".join([__major__, __minor__, __patch__])
+__version__ = "v1.0.0"
```

