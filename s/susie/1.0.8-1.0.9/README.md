# Comparing `tmp/susie-1.0.8.tar.gz` & `tmp/susie-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "susie-1.0.8.tar", last modified: Wed Feb 21 06:33:38 2024, max compression
+gzip compressed data, was "susie-1.0.9.tar", last modified: Mon Apr 15 19:27:02 2024, max compression
```

## Comparing `susie-1.0.8.tar` & `susie-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-02-21 06:33:38.194480 susie-1.0.8/
--rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.0.8/LICENSE.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)    12069 2024-02-21 06:33:38.194369 susie-1.0.8/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)    10258 2023-12-18 22:41:19.000000 susie-1.0.8/README.md
--rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.0.8/pyproject.toml
--rw-r--r--   0 maliabarker   (501) staff       (20)      836 2024-02-21 06:33:38.194977 susie-1.0.8/setup.cfg
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-02-21 06:33:38.190786 susie-1.0.8/src/
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-02-21 06:33:38.192316 susie-1.0.8/src/susie/
--rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.0.8/src/susie/__init__.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    35942 2024-02-21 06:31:02.000000 susie-1.0.8/src/susie/ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)    13708 2024-02-21 05:57:56.000000 susie-1.0.8/src/susie/transit_times.py
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-02-21 06:33:38.194048 susie-1.0.8/src/susie.egg-info/
--rw-r--r--   0 maliabarker   (501) staff       (20)    12069 2024-02-21 06:33:38.000000 susie-1.0.8/src/susie.egg-info/PKG-INFO
--rw-r--r--   0 maliabarker   (501) staff       (20)      334 2024-02-21 06:33:38.000000 susie-1.0.8/src/susie.egg-info/SOURCES.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-02-21 06:33:38.000000 susie-1.0.8/src/susie.egg-info/dependency_links.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-02-21 06:33:38.000000 susie-1.0.8/src/susie.egg-info/requires.txt
--rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-02-21 06:33:38.000000 susie-1.0.8/src/susie.egg-info/top_level.txt
-drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-02-21 06:33:38.193721 susie-1.0.8/tests/
--rw-r--r--   0 maliabarker   (501) staff       (20)      575 2023-12-11 21:58:52.000000 susie-1.0.8/tests/test_ephemeris.py
--rw-r--r--   0 maliabarker   (501) staff       (20)     7849 2023-12-11 21:58:06.000000 susie-1.0.8/tests/test_transit_times.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.952117 susie-1.0.9/
+-rw-r--r--   0 maliabarker   (501) staff       (20)     1065 2023-09-18 19:40:07.000000 susie-1.0.9/LICENSE.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-04-15 19:27:02.952013 susie-1.0.9/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)    10299 2024-03-27 19:16:09.000000 susie-1.0.9/README.md
+-rw-r--r--   0 maliabarker   (501) staff       (20)       84 2023-10-09 21:44:27.000000 susie-1.0.9/pyproject.toml
+-rw-r--r--   0 maliabarker   (501) staff       (20)      949 2024-04-15 19:27:02.952616 susie-1.0.9/setup.cfg
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.947420 susie-1.0.9/src/
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.949382 susie-1.0.9/src/susie/
+-rw-r--r--   0 maliabarker   (501) staff       (20)       36 2023-08-31 20:39:34.000000 susie-1.0.9/src/susie/__init__.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    37916 2024-04-15 19:23:11.000000 susie-1.0.9/src/susie/ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    14811 2024-04-15 18:59:39.000000 susie-1.0.9/src/susie/transit_times.py
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.951569 susie-1.0.9/src/susie.egg-info/
+-rw-r--r--   0 maliabarker   (501) staff       (20)    12234 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/PKG-INFO
+-rw-r--r--   0 maliabarker   (501) staff       (20)      334 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/SOURCES.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        1 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/dependency_links.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)       31 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/requires.txt
+-rw-r--r--   0 maliabarker   (501) staff       (20)        6 2024-04-15 19:27:02.000000 susie-1.0.9/src/susie.egg-info/top_level.txt
+drwxr-xr-x   0 maliabarker   (501) staff       (20)        0 2024-04-15 19:27:02.950975 susie-1.0.9/tests/
+-rw-r--r--   0 maliabarker   (501) staff       (20)     7689 2024-04-01 20:05:34.000000 susie-1.0.9/tests/test_ephemeris.py
+-rw-r--r--   0 maliabarker   (501) staff       (20)    20366 2024-03-25 19:15:32.000000 susie-1.0.9/tests/test_transit_times.py
```

### Comparing `susie-1.0.8/LICENSE.txt` & `susie-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `susie-1.0.8/PKG-INFO` & `susie-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.0.8
+Version: 1.0.9
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
-Author: Malia Barker, Holly VanLooy
-Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu
+Author: Malia Barker, Holly VanLooy, Adrienne Kirk
+Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
-Project-URL: repository, https://github.com/BoiseStatePlanetary/susie/
+Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
+Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 
 # The Susie Python Package
 A package for exoplanet transit decay calculations and visualizations.
 
+https://susie.readthedocs.io/en/latest/
+
 ![Susie Superpig Cartoon Image](http://www.astrojack.com/wp-content/uploads/2013/12/susie-1024x748.png)
 
 ## Statement of need
 The authors should clearly state what problems the software is designed to solve, who the target audience is, and its relation to other work.
 
 ## Installation instructions
 To download this package, use:
```

### Comparing `susie-1.0.8/README.md` & `susie-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # The Susie Python Package
 A package for exoplanet transit decay calculations and visualizations.
 
+https://susie.readthedocs.io/en/latest/
+
 ![Susie Superpig Cartoon Image](http://www.astrojack.com/wp-content/uploads/2013/12/susie-1024x748.png)
 
 ## Statement of need
 The authors should clearly state what problems the software is designed to solve, who the target audience is, and its relation to other work.
 
 ## Installation instructions
 To download this package, use:
```

### Comparing `susie-1.0.8/setup.cfg` & `susie-1.0.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [metadata]
 name = susie
-version = 1.0.8
-author = Malia Barker, Holly VanLooy
-author_email = maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu
+version = 1.0.9
+author = Malia Barker, Holly VanLooy, Adrienne Kirk
+author_email = maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 description = Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 project_urls = 
 	Bug Tracker = https://github.com/BoiseStatePlanetary/susie/issues
-	repository = https://github.com/BoiseStatePlanetary/susie/
+	Repository = https://github.com/BoiseStatePlanetary/susie/
+	Documentation = https://susie.readthedocs.io/en/latest/index.html
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `susie-1.0.8/src/susie/ephemeris.py` & `susie-1.0.9/src/susie/ephemeris.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,48 +12,50 @@
         """Fits a model ephemeris to transit data.
 
         Defines the structure for fitting a model (linear or quadratic) to transit data. 
         All subclasses must implement this method.
 
         Parameters
         ----------
-            x: numpy.ndarray[int]
+            x : numpy.ndarray[int]
                 The epoch data as recieved from the TransitTimes object.
-            y: numpy.ndarray[float]
+            y : numpy.ndarray[float]
                 The mid transit time data as recieved from the TransitTimes object.
-            yerr: numpy.ndarray[float]
+            yerr : numpy.ndarray[float]
                 The mid transit time error data as recieved from the TransitTimes object.
 
         Returns
         ------- 
-            A dictionary containing fitted model parameters.
+            A dictionary containing fitted model parameters. 
+
         """
         pass
 
 
 class LinearModelEphemeris(BaseModelEphemeris):
     """Subclass of BaseModelEphemeris that implements a linear fit."""
     def lin_fit(self, x, P, T0):
         """Calculates a linear function with given data.
 
         Uses the equation (Period * mid transit times + initial epoch) as a linear function for SciPy's 
         curve_fit method.
         
         Parameters
         ----------
-            x: numpy.ndarray[int]
+
+            x: numpy.ndarray[float]
                 The mid-transit times.
-            P: float
+            P : float
                 The exoplanet transit period.
-            T0: float
+            T0 : float
                 The initial epoch associated with a mid-transit time.
         
         Returns
         -------
-            P*x + T0: numpy.ndarray[float]
+            P*x + T0 : numpy.ndarray[float]
                 A linear function calculated with TransitTimes object data to be used with curve_fit.
         """
         return P*x + T0
     
     def fit_model(self, x, y, yerr, **kwargs):
         """Fits a linear model to ephemeris data.
 
@@ -72,21 +74,21 @@
                 The mid transit time error data as recieved from the TransitTimes object.
             **kwargs:
                 Any key word arguments to be used in the scipy.optimize.curve_fit method.
 
         Returns
         ------- 
         return_data: dict
-            A dictionary of parameters from the fit model ephemeris. Example:
-                {
-                    'period': An array of exoplanet periods over time corresponding to epochs,
-                    'period_err': The uncertainities associated with period,
-                    'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
-                    'conjunction_time_err': The uncertainties associated with conjunction_time
-                }
+            A dictionary of parameters from the fit model ephemeris. 
+            
+            Example:
+                * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
+                * 'period_err': The uncertainities associated with period (in units of days),
+                * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
+                * 'conjunction_time_err': The uncertainties associated with conjunction_time
         """
         # Will come back in units of y/x (so will be in days), period is days per orbit (but rly this is days bc orbit is unitless)
         popt, pcov = curve_fit(self.lin_fit, x, y, sigma=yerr, absolute_sigma=True, **kwargs)
         unc = np.sqrt(np.diag(pcov))
         return_data = {
             'period': popt[0],
             'period_err': unc[0],
@@ -143,22 +145,20 @@
             **kwargs:
                 Any key word arguments to be used in the scipy.optimize.curve_fit method.
 
         Returns
         ------- 
         return_data: dict
             A dictionary of parameters from the fit model ephemeris. Example:
-                {
-                    'period': An array of exoplanet periods over time corresponding to epochs,
-                    'period_err': The uncertainities associated with period,
-                    'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
-                    'conjunction_time_err': The uncertainties associated with conjunction_time,
-                    'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch,
-                    'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch
-                }
+                * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
+                * 'period_err': The uncertainities associated with period (in units of days),
+                * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
+                * 'conjunction_time_err': The uncertainties associated with conjunction_time,
+                * 'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch (in units of days),
+                * 'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch (in units of days)
         """
         popt, pcov = curve_fit(self.quad_fit, x, y, sigma=yerr, absolute_sigma=True, **kwargs)
         unc = np.sqrt(np.diag(pcov))
         return_data = {
             'conjunction_time': popt[2],
             'conjunction_time_err': unc[2],
             'period': popt[1],
@@ -189,26 +189,23 @@
             yerr: numpy.ndarray[float]
                 The mid transit time error data as recieved from the TransitTimes object.
             **kwargs:
                 Any keyword arguments to be used in the scipy.optimize.curve_fit method.
 
         Returns
         ------- 
-            A dictionary of parameters from the fit model ephemeris. If a linear model was chosen, these parameters are:
-            {
-                'period': An array of exoplanet periods over time corresponding to epochs,
-                'period_err': The uncertainities associated with period,
-                'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
-                'conjunction_time_err': The uncertainties associated with conjunction_time
-            }
-            If a quadratic model was chosen, the same variables are returned, and an additional parameter is included in the dictionary:
-            {
-                'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch,
-                'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch,
-            }
+            Model : dict
+                A dictionary of parameters from the fit model ephemeris. If a linear model was chosen, these parameters are:
+                    * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
+                    * 'period_err': The uncertainities associated with period (in units of days),
+                    * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
+                    * 'conjunction_time_err': The uncertainties associated with conjunction_time
+                If a quadratic model was chosen, the same variables are returned, and an additional parameter is included in the dictionary:
+                    * 'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch (in units of days),
+                    * 'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch (in units of days)
         
         Raises
         ------
             ValueError:
                 If model specified is not a valid subclass of BaseModelEphemeris, which is either 'linear' or 'quadratic'.
         """
         models = {
@@ -238,14 +235,18 @@
         """Initializing the transit times object and model ephermeris object
         
         Parameters
         -----------
         transit_times: TransitTimes obj
             A successfully instantiated TransitTimes object holding epochs, mid transit times, and uncertainties.
         
+        Raises
+        ------
+            ValueError :
+                error raised if 'transit_times' is not an instance of 'TransitTimes' object.
         """
         self.transit_times = transit_times
         self._validate()
 
     def _validate(self):
         """Check that transit_times is an instance of the TransitTimes object.
         
@@ -254,49 +255,43 @@
             ValueError :
                 error raised if 'transit_times' is not an instance of 'TransitTimes' object.
         """
         if not isinstance(self.transit_times, TransitTimes):
             raise ValueError("Variable 'transit_times' expected type of object 'TransitTimes'.")
         
     def _get_transit_times_data(self):
-        """Normalizes transit time data and returns for use.
-        
-        STEP 1: Normalize the epoch data by subtracting the minimum value of the epochs from each epoch in the array.
+        """Returns transit time data for use.
 
-        STEP 2: Normalize the mid transit time data by subtracting the minimum value of the mid transit times from each mid transit time in the array.
-
-        STEP 3: yerr is created NOTE: I'm confused about this - we didn't do anything???
-
-        STEP 4: return the epoch, mid transit time and mid transit time error data.
+        Returns the epoch, mid transit time, and mid transit time error data from the TransitTimes object.
 
         Returns
         -------
             x: numpy.ndarray[int]
                 The epoch data as recieved from the TransitTimes object.
             y: numpy.ndarray[float]
                 The mid transit time data as recieved from the TransitTimes object.
             yerr: numpy.ndarray[float]
                 The mid transit time error data as recieved from the TransitTimes object.
         """
-        x = self.transit_times.epochs - np.min(self.transit_times.epochs)
-        y = self.transit_times.mid_transit_times - np.min(self.transit_times.mid_transit_times)
+        x = self.transit_times.epochs
+        y = self.transit_times.mid_transit_times
         yerr = self.transit_times.mid_transit_times_uncertainties
         return x, y, yerr
     
     def _get_model_parameters(self, model_type, **kwargs):
         """Creates the model ephemeris object and returns model parameters.
         
         This method processes and fetches data from the TransitTimes object to be used in the model ephemeris. 
         It creates the appropriate subclass of BaseModelEphemeris using the ModelEphemeris factory, then runs 
         the fit_model method to return the model parameters dictionary.
 
         Parameters
         ----------
             model_type: str
-                Either 'linear' or 'quadratic, the ephemeris subclass specified to create and run.
+                Either 'linear' or 'quadratic'. The ephemeris subclass specified to create and run.
 
         Returns
         -------
             model_ephemeris_data: dict
                 A dictionary of parameters from the fit model ephemeris. If a linear model was chosen, these parameters are:
                 {
                     'period': An array of exoplanet periods over time corresponding to epochs,
@@ -390,15 +385,14 @@
         -------
             A list of uncertainties associated with the model ephemeris passed in, calculated with the 
             equation above and the TransitTimes epochs.
         """
         return np.sqrt((T0_err**2) + ((self.transit_times.epochs**2)*(P_err**2)) + ((1/4)*(self.transit_times.epochs**4)*(dPdE_err**2)))
     
     def _calc_linear_ephemeris(self, epochs, period, conjunction_time):
-        # NOTE: Is this actually calculating mid transit times?
         """Calculates the mid transit times using parameters from a linear model ephemeris.
         
         Uses the equation (T0 + PE) to calculate the mid transit times over each epoch where T0 is 
         conjunction time, P is period, and E is epoch.
 
         Parameters
         ----------
@@ -413,16 +407,14 @@
         -------
             A numpy array of mid transit times calculated over each epoch using the equation above.
         """
         return ((period*epochs) + conjunction_time)
     
     def _calc_quadratic_ephemeris(self, epochs, period, conjunction_time, period_change_by_epoch):
         """Calculates the mid transit times using parameters from a quadratic model ephemeris.
-        
-        # Returning 
 
         Uses the equation (T0 + PE + 0.5 * dPdE * E^2) to calculate the mid transit times over each epoch 
         where T0 is conjunction time, P is period, E is epoch, and dPdE is period change with respect to epoch.
 
         Parameters
         ----------
             epochs: numpy.ndarray[int]
@@ -437,31 +429,31 @@
         Returns
         -------
             A numpy array of mid transit times calculated over each epoch using the equation above.
         """
         return((0.5*period_change_by_epoch*(epochs**2)) + (period*epochs) + conjunction_time)
     
     def _calc_chi_squared(self, model_data):
-        # TODO: Docstring - needs editing
         """Calculates the residual chi squared values for the model ephemeris.
 
         STEP 1: Get the observed transit times and observed transit times uncertainties from transit_times.py.
 
         STEP 2: Calculate the chi-squared value for the observed and model data, then return this value.
         
         Parameters
         ----------
-            model_data : 
-                NOTE: a key of the model data dictionary - what data type is this and what is it really doing? This is our predicted data
+            model_data : numpy.ndarray[float]
+                The 'model_data' values from the returned dictionary of fit model ephemeris method, representing the \\
+                    predicted mid-transit time data, the inital period, and the conjunction time.
         
         Returns
         -------
-            Return the calculated chi-squared value
+            Chi-squared value : float
+                The chi-squared value calculated from the observed and model data.
         """
-        # TODO: change model_data to something more descriptive
         # STEP 1: Get observed transit times
         observed_data = self.transit_times.mid_transit_times
         uncertainties = self.transit_times.mid_transit_times_uncertainties
         # STEP 2: calculate X2 with observed data and model data
         return np.sum(((observed_data - model_data)/uncertainties)**2)
     
     def get_model_ephemeris(self, model_type):
@@ -469,46 +461,51 @@
         
         Parameters
         ----------
             model_type: str
                 Either 'linear' or 'quadratic'. Represents the type of ephemeris to fit the data to.
 
         Returns
-        -------
+        ------- 
             A dictionary of parameters from the fit model ephemeris. If a linear model was chosen, these parameters are:
-            {
-                'period': An array of exoplanet periods over time corresponding to epochs,
-                'period_err': The uncertainities associated with period,
-                'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
-                'conjunction_time_err': The uncertainties associated with conjunction_time
-            }
+            
+                * 'period': An array of exoplanet periods over time corresponding to epochs (in units of days),
+                * 'period_err': The uncertainities associated with period (in units of days),
+                * 'conjunction_time': The time of conjunction of exoplanet transit over time corresponding to epochs,
+                * 'conjunction_time_err': The uncertainties associated with conjunction_time
+            
             If a quadratic model was chosen, the same variables are returned, and an additional parameter is included in the dictionary:
-            {
-                'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch,
-                'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch,
-            }
+            
+                * 'period_change_by_epoch': The exoplanet period change over epochs, from first epoch to current epoch (in units of days),
+                * 'period_change_by_epoch_err': The uncertainties associated with period_change_by_epoch (in units of days),
         """
-        # NOTE: Are these values returned in days? ex: conjunction time, orbital period, change in orbital period
         parameters = self._get_model_parameters(model_type)
         parameters['model_type'] = model_type
         # Once we get parameters back, we call _calc_linear_ephemeris 
         if model_type == 'linear':
             # Return dict with parameters and model data
             parameters['model_data'] = self._calc_linear_ephemeris(self.transit_times.epochs, parameters['period'], parameters['conjunction_time'])
         elif model_type == 'quadratic':
             parameters['model_data'] = self._calc_quadratic_ephemeris(self.transit_times.epochs, parameters['period'], parameters['conjunction_time'], parameters['period_change_by_epoch'])
         return parameters
     
     def get_ephemeris_uncertainties(self, model_params):
         """Calculates the uncertainties of a specific model data when compared to the actual data. 
         
-        Uses the equation σ(t pred, tra) = √(σ(T0)^2 + σ(P)^2 * E^2) for linear models and 
-        σ(t pred, tra) = √(σ(T0)^2 + (σ(P)^2 * E^2) + (1/4 * σ(dP/dE)^2 * E^4)) for quadratic models 
-        (where σ(T0)=conjunction time error, E=epoch, σ(P)=period error, and σ(dP/dE)=period change by 
-        epoch error) to calculate the uncertainties between the model data and actual data over epochs.
+        Uses the equation 
+        
+        .. math::
+            \\sigma(\\text{t pred, tra}) = \\sqrt{(\\sigma(T_0)^2 + \\sigma(P)^2 * E^2)}
+        
+        for linear models and 
+
+        .. math::
+            \\sigma(\\text{t pred, tra}) = \\sqrt{(\\sigma(T_0)^2 + (\\sigma(P)^2 * E^2) + (\\frac{1}{4} * \\sigma(\\frac{dP}{dE})^2 * E^4))} 
+        
+        for quadratic models (where :math:`\\sigma(T_0) =` conjunction time error, :math:`E=` epoch, :math:`\\sigma(P)=` period error, and :math:`\\sigma(\\frac{dP}{dE})=` period change by epoch error) to calculate the uncertainties between the model data and actual data over epochs.
         
         Parameters
         ----------
         model_params: dict
             A dictionary of model ephemeris parameters recieved from `Ephemeris.get_model_ephemeris`.
         
         Returns
@@ -531,19 +528,23 @@
             return self._calc_linear_model_uncertainties(model_params['conjunction_time_err'], model_params['period_err'])
         elif model_params['model_type'] == 'quadratic':
             if 'conjunction_time_err' not in model_params or 'period_err' not in model_params or 'period_change_by_epoch_err' not in model_params:
                 raise KeyError("Cannot find conjunction time, period, and/or period change by epoch errors in model data. Please run the get_model_ephemeris method with 'quadratic' model_type to return ephemeris fit parameters.")
             return self._calc_quadratic_model_uncertainties(model_params['conjunction_time_err'], model_params['period_err'], model_params['period_change_by_epoch_err'])
     
     def calc_bic(self, model_data_dict):
-        """Calculates the BIC value for a given model ephemeris. 
+        """
+        Calculates the BIC value for a given model ephemeris. 
         
-        Uses the equation BIC = 𝜒2 + (k * log(N)) where 
-        𝜒2=∑((observed mid transit times - model mid transit times)/observed mid transit time uncertainties)^2, 
-        k=number of fit parameters (2 for linear models, 3 for quadratic models), and N=total number of data points.
+        Uses the equation
+
+        .. math::
+            BIC = \\chi^2 + (k * log(N))
+         
+        where :math:`\\chi^2=\\sum{  \\frac{(\\text{observed mid transit times - model mid transit times})}{\\text{(observed mid transit time uncertainties})^2}   },`  k=number of fit parameters (2 for linear models, 3 for quadratic models), and N=total number of data points.
         
         Parameters
         ----------
             model_data_dict: dict
                 A dictionary of model ephemeris parameters recieved from `Ephemeris.get_model_ephemeris`.
         
         Returns
@@ -554,30 +555,41 @@
         num_params = self._get_k_value(model_data_dict['model_type'])
         # Step 2: Calculate chi-squared
         chi_squared = self._calc_chi_squared(model_data_dict['model_data'])
         # Step 3: Calculate BIC
         return chi_squared + (num_params*np.log(len(model_data_dict['model_data'])))
 
     def calc_delta_bic(self):
-        """Calculates the ΔBIC value between linear and quadratic model ephemerides using the given transit data. 
+        """Calculates the :math:`\\Delta BIC` value between linear and quadratic model ephemerides using the given transit data. 
         
+        STEP 1: Calls get_model_ephemeris for both the linear and quadratic models. 
+
+        STEP 2: Calls calc_bic for both the linear and quadratic sets of data.
+
+        STEP 3: Calculates and returns :math:`\\Delta BIC,` which is the difference between the linear BIC and quadratic BIC.
+
         Returns
         ------- 
-            A float value representing the ΔBIC value for this transit data. NOTE: not done
+            delta_bic : float
+                Represents the :math:`\\Delta BIC` value for this transit data. 
         """
         linear_data = self.get_model_ephemeris('linear')
         quadratic_data = self.get_model_ephemeris('quadratic')
         linear_bic = self.calc_bic(linear_data)
         quadratic_bic = self.calc_bic(quadratic_data)
         delta_bic = linear_bic - quadratic_bic
         return delta_bic
     
     def plot_model_ephemeris(self, model_data_dict, save_plot=False, save_filepath=None):
         """Returns a MatplotLib scatter plot showing predicted mid transit times from the model ephemeris over epochs.
 
+        STEP 1: Plot a scatterplot of epochs (from transit_times.py) vs model_data, which is an array of floats that is a value of 'model_data_dict'.
+
+        STEP 2: Save the plot if indicated by the user.
+
         Parameters
         ----------
             model_data_dict: dict
                 A dictionary of model ephemeris parameters recieved from `Ephemeris.get_model_ephemeris`.
             save_plot: bool 
                 If True, will save the plot as a figure.
             save_filepath: Optional(str)
@@ -593,20 +605,22 @@
         plt.title(f'Predicted {model_data_dict["model_type"]} Model Mid Transit Times over Epochs')
         if save_plot == True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_timing_uncertainties(self, model_data_dict, save_plot=False, save_filepath=None):
         """Returns a MatplotLib scatter plot showing timing uncertainties over epochs.
-        NOTE: these steps need to be checked - I need to clarify what 'model_data' is.
-        STEP 1: Get the uncertianies from the model data dictionary 
 
-        STEP 2: Get the model data, subtract the conjunction time and subtract the initial period
+        STEP 1: Get the uncertianies from the model data dictionary.
+
+        STEP 2: Get the model data, which is an arrary of floats representing the predicted mid-transit time data, the conjunction time and the inital period. Subtract the conjunction time and the initial period from this array.
+
+        STEP 3: Plot this modified model data, showing the maximum and minimum model uncertainity at each point.
 
-        STEP 3: Plot this modified model data, shoing the maximum and minimum model uncertainity at each point.
+        STEP 4: Save the plot if indicated by the user. 
 
         Parameters
         ----------
             model_data_dict: dict
                 A dictionary of model ephemeris parameters recieved from `Ephemeris.get_model_ephemeris`.
             save_plot: bool 
                 If True, will save the plot as a figure.
@@ -631,15 +645,24 @@
         plt.ylabel('Days')
         plt.legend()
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_oc_plot(self, save_plot=False, save_filepath=None):
-        """TODO docstring
+        """Returns a MatplotLib scatter plot showing observed vs. calculated values of mid transit times for linear and quadratic model ephemerides over epochs.
+
+        STEP 1: Call 'get_model_ephemeris' for both the linear and quadratic model types. 
+
+        STEP 2: Calculate the quadratic model curve, which follows the formula :math:`y = 0.5 \\frac{dP_0}{dE} * (E - \\text{median} E)^2.`
+
+        STEP 3: Plot the quadratic model curve vs. epochs from transit_times.py. Plot the error bars at each data point using the \\
+        'mid_transit_times_uncertainties' from transit_times.py.
+
+        STEP 4: Save the plot if indicated by the user. 
 
         Parameters
         ----------
             save_plot: bool 
                 If True, will save the plot as a figure.
             save_filepath: Optional(str)
                 The path used to save the plot if `save_plot` is True.
@@ -664,26 +687,35 @@
         plt.xlabel('E - Median E')
         plt.ylabel('O-C (seconds)')
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
     def plot_running_delta_bic(self, save_plot=False, save_filepath=None):
-        """TODO docstring
+        """Returns a MatPlotlib scatterplot of epochs vs. :math:`\\Delta BIC` for each epoch.
+
+        STEP 1: Get the epochs, mid transit times and mid transit times uncertainties from 'transit_times.py'.
+
+        STEP 2: Create a list of the :math:`\\Delta BIC` values. For the first 3 epochs, the :math:`\\Delta BIC` value is zero. For the subsequent epochs\\
+        call 'calc_delta_bic' and append the returned value to the list of delta bic values.
+
+        STEP 3: Plot a scatterplot of the epochs vs. the :math:`\\Delta BIC` values.
+
+        STEP 4: Save the plot if indicated by the user. 
 
         Parameters
         ----------
             save_plot: bool 
                 If True, will save the plot as a figure.
             save_filepath: Optional(str)
                 The path used to save the plot if `save_plot` is True.
-        
+                
         Returns
         -------
-            A MatplotLib scatter plot of epochs vs. ΔBIC for each epoch.
+            A MatplotLib scatter plot of epochs vs. :math:`\\Delta BIC` for each epoch.
         """
         delta_bics = []
         all_epochs = self.transit_times.epochs
         all_mid_transit_times = self.transit_times.mid_transit_times
         all_uncertainties = self.transit_times.mid_transit_times_uncertainties
         # for each epoch (starting at 3?), calculate the delta bic, plot delta bics over epoch
         for i in range(0, len(all_epochs)):
@@ -699,38 +731,40 @@
         plt.grid(True)
         plt.plot(self.transit_times.epochs, delta_bics)
         if save_plot is True:
             plt.savefig(save_filepath)
         plt.show()
 
 if __name__ == '__main__':
-    # STEP 1: Upload data from file
+    # STEP 1: Upload datra from file
     filepath = "../../malia_examples/WASP12b_transit_ephemeris.csv"
     data = np.genfromtxt(filepath, delimiter=',', names=True)
     # STEP 2: Break data up into epochs, mid transit times, and error
     # STEP 2.5 (Optional): Make sure the epochs are integers and not floats
     epochs = data["epoch"].astype('int')
     mid_transit_times = data["transit_time"]
     mid_transit_times_err = data["sigma_transit_time"]
     # STEP 3: Create new transit times object with above data
     # transit_times_obj1 = TransitTimes('jd', epochs, mid_transit_times, mid_transit_times_err, object_ra=97.64, object_dec=29.67, observatory_lat=43.60, observatory_lon=-116.21)
     # print(vars(transit_times_obj1))
     transit_times_obj1 = TransitTimes('jd', epochs, mid_transit_times, mid_transit_times_err, time_scale='tdb')
-    print(f"EPOCHS: {transit_times_obj1.epochs}\n")
-    print(f"MID TRANSIT TIMES: {transit_times_obj1.mid_transit_times}\n")
-    # STEP 4: Create new ephemeris object with transit times object
-    ephemeris_obj1 = Ephemeris(transit_times_obj1)
-    # STEP 5: Get model ephemeris data
-    linear_model_data = ephemeris_obj1.get_model_ephemeris('linear')
-    quad_model_data = ephemeris_obj1.get_model_ephemeris('quadratic')
-    print(linear_model_data)
-    print(quad_model_data)
-    # ephemeris_obj1.plot_model_ephemeris(linear_model_data)
-    # ephemeris_obj1.plot_model_ephemeris(quad_model_data)
-    ephemeris_obj1.plot_oc_plot()
+
+
+    # print(f"EPOCHS: {transit_times_obj1.epochs}\n")
+    # print(f"MID TRANSIT TIMES: {transit_times_obj1.mid_transit_times}\n")
+    # # STEP 4: Create new ephemeris object with transit times object
+    # ephemeris_obj1 = Ephemeris(transit_times_obj1)
+    # # STEP 5: Get model ephemeris data
+    # linear_model_data = ephemeris_obj1.get_model_ephemeris('linear')
+    # quad_model_data = ephemeris_obj1.get_model_ephemeris('quadratic')
+    # print(linear_model_data)
+    # print(quad_model_data)
+    # # ephemeris_obj1.plot_model_ephemeris(linear_model_data)
+    # # ephemeris_obj1.plot_model_ephemeris(quad_model_data)
+    # ephemeris_obj1.plot_oc_plot()
     # model_uncertainties = ephemeris_obj1.get_ephemeris_uncertainties(model_data)
     # print(model_uncertainties)
     # # STEP 6: Show a plot of the model ephemeris data
     # # ephemeris_obj1.plot_model_ephemeris(model_data, save_plot=False)
     # # # STEP 7: Uncertainties plot
     # # ephemeris_obj1.plot_timing_uncertainties(model_data, save_plot=False)
     # # bic = ephemeris_obj1.calc_bic(model_data)
```

### Comparing `susie-1.0.8/src/susie/transit_times.py` & `susie-1.0.9/src/susie/transit_times.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import numpy as np
 from astropy import time
 from astropy import coordinates as coord
 from astropy import units as u
 import logging
 
-class TransitTimes(object):
+# TESTING
+
+# class TransitTimes():
+#     def __init__(self):
+#         # pass in all the same stuff for transit times
+#         pass
+
+# class OccultationTimes():
+#     def __init__(self):
+#         # pass in all the same stuff for occultation times
+#         pass
+
+class TransitTimes():
     """Represents transit midpoint data over time. Holds data to be accessed by Ephemeris class.
     
     The transit_times object is a class which formats user data to be passed to the ephemeris.py object. \
         This object creates and/or formats the array of uncertainties in mid_transit_times. This object \
             will also correct user data to use the Barycentric Julian Date as the timing system and Barycentric \
                 Dynamical time as the time scale.
+
     STEP 1: Make an array of 1's to be the uncertainities in the same shape as epochs and mid_transit_times.
+
     STEP 2: Check that the time system and scale are correct, and if not correct them to be JD and TBD.
+
     STEP 3: Check that the array's are formatted properly. The appropriate Type or Value Error is raised if there are any issues.
  
     Parameters
     ------------
         time_format: str 
             An abbreviation of the data's timing system. Abbreviations for systems can be found on [Astropy's Time documentation](https://docs.astropy.org/en/stable/time/#id3).
         epochs: numpy.ndarray(int)
@@ -32,45 +47,51 @@
         object_dec: Optional(float)
             The declination in degrees of observed object represented by data.
         observatory_lon: Optional(float)
             The longitude in degrees of observatory data was collected from.
         observatory_lat: Optional(float) 
             The latitude in degrees of observatory data was collected from.
     Raises
-    ------------
-        Error raised if parameters are not NumPy Arrays, parameters are not the same shape of array, the values of epochs are not all ints, the values of mid_transit_times and unertainites are not all floats, or values of uncertainities are not all positive.
+    ------
+        Error raised if  
+            * parameters are not NumPy Arrays 
+            * parameters are not the same shape of array 
+            * the values of epochs are not all ints
+            * the values of mid_transit_times and unertainites are not all floats
+            * values of uncertainities are not all positive.
 
     Side Effects
     -------------
         Variables epochs and mid_transit_times are shifted to start at zero by subtracting the minimum number from each value.
     """
+    # def __init__(self, time_format, epochs, mid_transit_times, mid_transit_times_uncertainties=None, tra_or_occ=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
     def __init__(self, time_format, epochs, mid_transit_times, mid_transit_times_uncertainties=None, time_scale=None, object_ra=None, object_dec=None, observatory_lon=None, observatory_lat=None):
-        # TODO: What would happen here if a non-numpy array is passed in? Should we add validation for that?
         self.epochs = epochs
         self.mid_transit_times = mid_transit_times
         if mid_transit_times_uncertainties is None:
             # Make an array of 1s in the same shape of epochs and mid_transit_times
-            mid_transit_times_uncertainties = np.ones_like(self.epochs, dtype=float)
+            mid_transit_times_uncertainties =  np.ones_like(self.epochs, dtype=float)
         self.mid_transit_times_uncertainties = mid_transit_times_uncertainties
         # Check that timing system and scale are JD and TDB
         if time_format != 'jd' or time_scale != 'tdb':
             # TODO: Make sure they know default scale is UTC
             # If not correct time format and scale, create time objects and run corrections
             logging.warning(f"Recieved time format {time_format} and time scale {time_scale}. " 
                             "Correcting all times to BJD timing system with TDB time scale. If this is incorrect, please set the time format and time scale for TransitTime object.")
             self.mid_transit_times = None
             self.mid_transit_times_uncertainties = None
             mid_transit_times_obj = time.Time(mid_transit_times, format=time_format, scale=time_scale)
             mid_transit_times_uncertainties_obj = time.Time(mid_transit_times_uncertainties, format=time_format, scale=time_scale)
             self._validate_times(mid_transit_times_obj, mid_transit_times_uncertainties_obj, (object_ra, object_dec), (observatory_lon, observatory_lat))
         # Call validation function
         self._validate()
-        # Shift epochs and mid transit times
-        self.epochs = self.epochs - np.min(self.epochs)
-        self.mid_transit_times = self.mid_transit_times - np.min(self.mid_transit_times)
+        # Once everything is validated and corrected, we can separate into transits and occultations if we are given the tra_or_occ data
+        # if tra_or_occ is not None:
+        #     for epoch, mtt, mtt_err in zip(self.epochs, self.mid_transit_times, self.mid_transit_times_uncertainties):
+        #         foiwehf
 
     def _calc_barycentric_time(self, time_obj, obj_location, obs_location):
         """Function to correct non-barycentric time formats to Barycentric Julian Date in TDB time scale.
 
         STEP 1: Checks if given placeholder values of 1. If given placeholder values, no correction needed and array of 1's returned.
 
         STEP 2: If given actual values, correct the values to be Barycentric Julian Date in TDB time scale. Return corrected values.
@@ -176,23 +197,30 @@
             raise TypeError("The variable 'mid_transit_times' expected a NumPy array (np.ndarray) but received a different data type")
         if not isinstance(self.mid_transit_times_uncertainties, np.ndarray):
             raise TypeError("The variable 'mid_transit_times_uncertainties' expected a NumPy array (np.ndarray) but received a different data type")
         # Check that all are same shape
         if self.epochs.shape != self.mid_transit_times.shape != self.mid_transit_times_uncertainties.shape:
             raise ValueError("Shapes of 'epochs', 'mid_transit_times', and 'mid_transit_times_uncertainties' arrays do not match.")
         # Check that all values in arrays are correct
-        if not all(isinstance(value, (int, np.int64)) for value in self.epochs):
-            raise TypeError("All values in 'epochs' must be of type int.")
+        # if not all(isinstance(value, (int, np.int64)) for value in self.epochs) or not all(isinstance(value, (int, np.int32)) for value in self.epochs):
+        if not all(isinstance(value, (int, np.int64, np.int32)) for value in self.epochs):
+            raise TypeError("All values in 'epochs' must be of type int, numpy.int64, or numpy.int32.")
         if not all(isinstance(value, float) for value in self.mid_transit_times):
             raise TypeError("All values in 'mid_transit_times' must be of type float.")
         if not all(isinstance(value, float) for value in self.mid_transit_times_uncertainties):
             raise TypeError("All values in 'mid_transit_times_uncertainties' must be of type float.")
         # Check that there are no null values
         if np.any(np.isnan(self.epochs)):
             raise ValueError("The 'epochs' array contains NaN (Not-a-Number) values.")
         if np.any(np.isnan(self.mid_transit_times)):
             raise ValueError("The 'mid_transit_times' array contains NaN (Not-a-Number) values.")
         if np.any(np.isnan(self.mid_transit_times_uncertainties)):
             raise ValueError("The 'mid_transit_times_uncertainties' array contains NaN (Not-a-Number) values.")
-        # Check that mid_transit_times_uncertainties are positive and non-zero
+        # Check that mid_transit_times_uncertainties are positive and non-zero (greater than zero)
         if not np.all(self.mid_transit_times_uncertainties > 0):
-            raise ValueError("The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values.")
+            raise ValueError("The 'mid_transit_times_uncertainties' array must contain non-negative and non-zero values.")
+        if self.epochs[0] != 0:
+            # Shift epochs and mid transit times
+            self.epochs -= np.min(self.epochs)
+            # TODO import warning that we are minimizing their epochs and transit times
+        if self.mid_transit_times[0] != 0:
+            self.mid_transit_times -= np.min(self.mid_transit_times)
```

### Comparing `susie-1.0.8/src/susie.egg-info/PKG-INFO` & `susie-1.0.9/src/susie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: susie
-Version: 1.0.8
+Version: 1.0.9
 Summary: Susie allows users to input exoplanet transit data and return information detailing possible tidal decay.
-Author: Malia Barker, Holly VanLooy
-Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu
+Author: Malia Barker, Holly VanLooy, Adrienne Kirk
+Author-email: maliabarker@icloud.com, hollyvanlooy@u.boisestate.edu, adriennekirk@u.boisestate.edu
 Project-URL: Bug Tracker, https://github.com/BoiseStatePlanetary/susie/issues
-Project-URL: repository, https://github.com/BoiseStatePlanetary/susie/
+Project-URL: Repository, https://github.com/BoiseStatePlanetary/susie/
+Project-URL: Documentation, https://susie.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: astropy
 
 # The Susie Python Package
 A package for exoplanet transit decay calculations and visualizations.
 
+https://susie.readthedocs.io/en/latest/
+
 ![Susie Superpig Cartoon Image](http://www.astrojack.com/wp-content/uploads/2013/12/susie-1024x748.png)
 
 ## Statement of need
 The authors should clearly state what problems the software is designed to solve, who the target audience is, and its relation to other work.
 
 ## Installation instructions
 To download this package, use:
```

