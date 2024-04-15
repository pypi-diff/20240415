# Comparing `tmp/pygdsm-1.5.2.tar.gz` & `tmp/pygdsm-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdsm-1.5.2.tar", last modified: Wed Apr  3 07:41:31 2024, max compression
+gzip compressed data, was "pygdsm-1.5.3.tar", last modified: Mon Apr 15 07:44:57 2024, max compression
```

## Comparing `pygdsm-1.5.2.tar` & `pygdsm-1.5.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 07:41:11.000000 pygdsm-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 07:41:11.000000 pygdsm-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 07:41:31.550586 pygdsm-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-03 07:41:11.000000 pygdsm-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.546585 pygdsm-1.5.2/pygdsm/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/base_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/base_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/component_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/gsm08.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/gsm16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/lfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/pygdsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 07:41:11.000000 pygdsm-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 07:41:11.000000 pygdsm-1.5.2/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 07:41:31.550586 pygdsm-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 07:41:11.000000 pygdsm-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm2016.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_lfsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 07:44:37.000000 pygdsm-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:44:37.000000 pygdsm-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 07:44:57.224067 pygdsm-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-15 07:44:37.000000 pygdsm-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.220067 pygdsm-1.5.3/pygdsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/base_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/base_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/component_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/gsm08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/gsm16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/lfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 07:44:37.000000 pygdsm-1.5.3/pygdsm/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/pygdsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:44:57.000000 pygdsm-1.5.3/pygdsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 07:44:37.000000 pygdsm-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 07:44:37.000000 pygdsm-1.5.3/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 07:44:57.224067 pygdsm-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 07:44:37.000000 pygdsm-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:44:57.224067 pygdsm-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm2016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_gsm_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-15 07:44:37.000000 pygdsm-1.5.3/tests/test_lfsm.py
```

### Comparing `pygdsm-1.5.2/LICENSE` & `pygdsm-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/PKG-INFO` & `pygdsm-1.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.2
+Version: 1.5.3
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
 Author: Danny C. Price
 Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
```

### Comparing `pygdsm-1.5.2/README.md` & `pygdsm-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/base_observer.py` & `pygdsm-1.5.3/pygdsm/base_observer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ephem
 import healpy as hp
 import numpy as np
 from astropy.time import Time
 from pygdsm.plot_utils import show_plt
-
+from pygdsm.utils import hpix2sky, sky2hpix
+from astropy.coordinates import SkyCoord
 
 class BaseObserver(ephem.Observer):
     """ Observer of the Global Sky Model.
 
     Generates the Observed sky, for a given point on Earth.
     Applies the necessary rotations and coordinate transformations
     so that the observed 'sky' can be returned, instead of the
@@ -55,61 +56,66 @@
         Returns
         -------
         observed_sky: np.array
             Numpy array representing the healpix image, centered on zenith,
             with below the horizon masked.
         """
         # Check to see if frequency has changed.
-        if freq is not None: 
+        if freq is not None:
             if not np.isclose(freq, self._freq):
                 self.gsm.generate(freq)
                 self._freq = freq
-        
+
         sky = self.gsm.generated_map_data
-        
+
         # Check if time has changed -- astropy allows None == Time() comparison
         if obstime == self._time or obstime is None:
             time_has_changed = False
         else:
             time_has_changed = True
             self._time = Time(obstime)  # This will catch datetimes, but Time() object should be passed
             self.date  = obstime.to_datetime()
 
         # Rotation is quite slow, only recompute if time or frequency has changed, or it has never been run
         if time_has_changed or self.observed_sky is None:
             # Get RA and DEC of zenith
             ra_zen, dec_zen = self.radec_of(0, np.pi/2)
+            sc_zen = SkyCoord(ra_zen, dec_zen, unit=('rad', 'rad'))
+            pix_zen = sky2hpix(self._n_side, sc_zen)
+            vec_zen = hp.pix2vec(self._n_side, pix_zen)
+
+            # Convert to degrees
             ra_zen  *= (180 / np.pi)
             dec_zen *= (180 / np.pi)
 
+            # Generate below-horizon mask using query_disc
+            mask = np.ones(shape=self._n_pix, dtype='bool')
+            pix_visible = hp.query_disc(self._n_side, vec=vec_zen, radius=np.pi/2)
+            mask[pix_visible] = 0
+            self._mask = mask
+
             # Transform from Galactic coordinates to Equatorial
             rot = hp.Rotator(coord=['G', 'C'])
             eq_theta, eq_phi = rot(self._theta, self._phi)
 
             # Convert from Equatorial colatitude and longitude to normal RA and DEC
             dec = 90.0 - np.abs(eq_theta*(180/np.pi))
             ra = ( (eq_phi + 2*np.pi) % (2*np.pi) )*(180/np.pi)
 
-            # Generate a mask for below horizon (distance from zenith > 90 deg)
-            dist = 2 * np.arcsin( np.sqrt( np.sin((dec_zen-dec)*(np.pi/180)/2)**2 + \
-                    np.cos(dec_zen*(np.pi/180))*np.cos(dec*(np.pi/180))*np.sin((ra_zen-ra)*(np.pi/180)/2)**2 ) )
-            mask = dist > (np.pi/2)
-            self._mask = mask
-
             # Apply rotation to convert from Galactic to Equatorial and center on zenith
             hrot = hp.Rotator(rot=[ra_zen, dec_zen], coord=['G', 'C'], inv=True)
             g0, g1 = hrot(self._theta, self._phi)
             pix0 = hp.ang2pix(self._n_side, g0, g1)
             self._pix0 = pix0
 
             dec_rotated = dec[self._pix0]
             ra_rotated = ra[self._pix0]
             self._observed_ra = ra_rotated
             self._observed_dec = dec_rotated
- 
+
         sky_rotated = sky[self._pix0]
         mask_rotated = self._mask[self._pix0]
 
         self.observed_sky = hp.ma(sky_rotated)
         self.observed_sky.mask = mask_rotated
 
         return self.observed_sky
@@ -128,19 +134,18 @@
 
         hp.orthview(sky, half_sky=True, **kwargs)
 
         if show:
             show_plt()
         return sky
 
-    def view_observed_gsm(self, logged=False, show=False, **kwargs):
-        """ View the GSM (Mollweide), with below-horizon area masked. """
+    @property
+    def observed_gsm(self):
+        """ Return the GSM (Mollweide), with below-horizon area masked. """
         sky = self.observed_sky
-        if logged:
-            sky = np.log2(sky)
 
         # Get RA and DEC of zenith
         ra_rad, dec_rad = self.radec_of(0, np.pi / 2)
         ra_deg  = ra_rad / np.pi * 180
         dec_deg = dec_rad / np.pi * 180
 
         # Apply rotation
@@ -149,14 +154,28 @@
         pix0 = hp.ang2pix(self._n_side, g0, g1)
         sky = sky[pix0]
 
         coordrotate = hp.Rotator(coord=['C', 'G'], inv=True)
         g0, g1 = coordrotate(self._theta, self._phi)
         pix0 = hp.ang2pix(self._n_side, g0, g1)
         sky = sky[pix0]
+        return sky
 
-        hp.mollview(sky, coord='G', **kwargs)
+    def view_observed_gsm(self, logged=False, show=False, **kwargs):
+        """ View the GSM (Mollweide), with below-horizon area masked.
+
+        Args:
+            logged (bool): Apply log2 to data (default False)
+            show (bool): Call plt.show() (default False)
+
+        Returns:
+            sky (np.array): Healpix map of observed GSM.
+        """
+        sky = self.observed_gsm
 
+        if logged:
+            sky = np.log2(sky)
+
+        hp.mollview(sky, coord='G', **kwargs)
         if show:
             show_plt()
-
         return sky
```

### Comparing `pygdsm-1.5.2/pygdsm/base_skymodel.py` & `pygdsm-1.5.3/pygdsm/base_skymodel.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/component_data.py` & `pygdsm-1.5.3/pygdsm/component_data.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/gsm08.py` & `pygdsm-1.5.3/pygdsm/gsm08.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/gsm16.py` & `pygdsm-1.5.3/pygdsm/gsm16.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/haslam.py` & `pygdsm-1.5.3/pygdsm/haslam.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm/lfsm.py` & `pygdsm-1.5.3/pygdsm/lfsm.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/pygdsm.egg-info/PKG-INFO` & `pygdsm-1.5.3/pygdsm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.2
+Version: 1.5.3
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
 Author: Danny C. Price
 Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
```

### Comparing `pygdsm-1.5.2/pygdsm.egg-info/SOURCES.txt` & `pygdsm-1.5.3/pygdsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/setup.py` & `pygdsm-1.5.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 setup(
     name='pygdsm',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.5.2',
+    version='1.5.3',
 
     description='Python Global Sky Model of diffuse Galactic radio emission',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/telegraphic/pygdsm',
@@ -55,18 +55,14 @@
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 
     # What does your project relate to?
     keywords='radio astronomy sky model galactic diffuse emission',
```

### Comparing `pygdsm-1.5.2/tests/test_gsm.py` & `pygdsm-1.5.3/tests/test_gsm.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ===========
 
 Tests for GSM module.
 """
 
 import os
 from pygdsm import GlobalSkyModel
+from pygdsm import init_gsm, init_observer
 
 import time
 import numpy as np
 import h5py
 import healpy as hp
 
 def test_gsm_generate():
@@ -104,15 +105,15 @@
 
     os.remove("test_write_fits.fits")
 
 def test_cmb_removal():
     g = GlobalSkyModel(freq_unit='MHz', include_cmb=False)
     sky_no_cmb = g.generate(400)
     g = GlobalSkyModel(freq_unit='MHz',  include_cmb=True)
-    sky_with_cmb = g.generate(400)    
+    sky_with_cmb = g.generate(400)
 
     T_cmb = (sky_with_cmb - sky_no_cmb).mean()
     print(T_cmb)
     assert np.isclose(T_cmb, 2.725)
 
 
 if __name__ == "__main__":
```

### Comparing `pygdsm-1.5.2/tests/test_gsm2016.py` & `pygdsm-1.5.3/tests/test_gsm2016.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/tests/test_gsm_observer.py` & `pygdsm-1.5.3/tests/test_gsm_observer.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/tests/test_haslam.py` & `pygdsm-1.5.3/tests/test_haslam.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.2/tests/test_lfsm.py` & `pygdsm-1.5.3/tests/test_lfsm.py`

 * *Files identical despite different names*

