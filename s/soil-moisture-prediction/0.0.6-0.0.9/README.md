# Comparing `tmp/soil_moisture_prediction-0.0.6.tar.gz` & `tmp/soil_moisture_prediction-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil_moisture_prediction-0.0.6.tar", max compression
+gzip compressed data, was "soil_moisture_prediction-0.0.9.tar", max compression
```

## Comparing `soil_moisture_prediction-0.0.6.tar` & `soil_moisture_prediction-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      299 2024-03-19 16:28:35.347746 soil_moisture_prediction-0.0.6/README.md
--rw-r--r--   0        0        0      999 2024-03-19 16:28:35.347746 soil_moisture_prediction-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1177 2024-03-19 16:28:35.347746 soil_moisture_prediction-0.0.6/soil_moisture_prediction/areaGeometry.py
--rw-r--r--   0        0        0    15538 2024-03-19 16:28:35.347746 soil_moisture_prediction-0.0.6/soil_moisture_prediction/inputData.py
--rw-r--r--   0        0        0    26316 2024-03-19 16:28:35.347746 soil_moisture_prediction-0.0.6/soil_moisture_prediction/plot_functions.py
--rw-r--r--   0        0        0    16111 2024-03-19 16:28:35.351746 soil_moisture_prediction-0.0.6/soil_moisture_prediction/random_forest_model.py
--rw-r--r--   0        0        0     1528 2024-03-19 16:28:35.351746 soil_moisture_prediction-0.0.6/soil_moisture_prediction/soil_moisture_prediction.py
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 soil_moisture_prediction-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-03-21 12:48:14.724125 soil_moisture_prediction-0.0.9/LICENSE
+-rw-r--r--   0        0        0      299 2024-03-21 12:48:14.724125 soil_moisture_prediction-0.0.9/README.md
+-rw-r--r--   0        0        0     1176 2024-03-21 12:48:14.725126 soil_moisture_prediction-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-03-21 12:48:14.725126 soil_moisture_prediction-0.0.9/soil_moisture_prediction/__init__.py
+-rw-r--r--   0        0        0     1177 2024-03-21 12:48:14.726127 soil_moisture_prediction-0.0.9/soil_moisture_prediction/areaGeometry.py
+-rw-r--r--   0        0        0    15538 2024-03-21 12:48:14.726127 soil_moisture_prediction-0.0.9/soil_moisture_prediction/inputData.py
+-rw-r--r--   0        0        0    26305 2024-03-21 12:48:14.727127 soil_moisture_prediction-0.0.9/soil_moisture_prediction/plot_functions.py
+-rw-r--r--   0        0        0    16111 2024-03-21 12:48:14.727127 soil_moisture_prediction-0.0.9/soil_moisture_prediction/random_forest_model.py
+-rw-r--r--   0        0        0     1528 2024-03-21 12:48:14.727127 soil_moisture_prediction-0.0.9/soil_moisture_prediction/smp_cli.py
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 soil_moisture_prediction-0.0.9/PKG-INFO
```

### Comparing `soil_moisture_prediction-0.0.6/pyproject.toml` & `soil_moisture_prediction-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soil-moisture-prediction"
-version = "0.0.6"
+version = "0.0.9"
 description = "Predicts soil moisture from cosmic ray neutron sensor data using a random forest model"
 authors = ["Segolene Dega <segolene.dega@ufz.de>" , "John Anders <john-eric.anders@ufz.de>"]
 license = "EUPL 1.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -34,11 +34,18 @@
 tzdata = "2023.3"
 xycmap = "1.0.1"
 zipp = "3.16.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
+black = "24.2"
+flake8 = "7.0.0"
+isort = "5.13.2"
+flake8-implicit-str-concat = "0.4.0"
+flake8-blind-except = "0.2.1"
+flake8-comprehensions = "3.14.0"
+flake8-docstrings = "1.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `soil_moisture_prediction-0.0.6/soil_moisture_prediction/areaGeometry.py` & `soil_moisture_prediction-0.0.9/soil_moisture_prediction/areaGeometry.py`

 * *Files identical despite different names*

### Comparing `soil_moisture_prediction-0.0.6/soil_moisture_prediction/inputData.py` & `soil_moisture_prediction-0.0.9/soil_moisture_prediction/inputData.py`

 * *Files identical despite different names*

### Comparing `soil_moisture_prediction-0.0.6/soil_moisture_prediction/plot_functions.py` & `soil_moisture_prediction-0.0.9/soil_moisture_prediction/plot_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,80 +38,60 @@
         rfo_model.rect_geom.grid_x / 1000,
         rfo_model.rect_geom.grid_y / 1000,
     )
 
 
 def plot_selection(rfo_model):
     """Plot funciton defined by the input selection."""
-    xaxis, yaxis = set_axis(rfo_model)
     output_dir = rfo_model.work_dir
 
     if rfo_model.what_to_plot["predictors"]:
-        plot_predictors(
-            xaxis, yaxis, rfo_model.input_data.predictors, output_dir=output_dir
-        )
+        plot_predictors(rfo_model, output_dir=output_dir)
 
     if rfo_model.what_to_plot["pred_correlation"]:
-        prediction_correlation_matrix(rfo_model.input_data, output_dir=output_dir)
+        prediction_correlation_matrix(rfo_model, output_dir=output_dir)
 
     for time_step in range(len(rfo_model.input_data.soil_moisture_data.start_times)):
         if rfo_model.what_to_plot["day_measurements"]:
             plot_measurements(
-                rfo_model.input_data.soil_moisture_data,
+                rfo_model,
                 time_step,
-                rfo_model.monte_carlo,
                 output_dir=output_dir,
             )
         if rfo_model.what_to_plot["day_prediction_map"]:
             plot_rfo_model(
-                xaxis,
-                yaxis,
-                rfo_model.input_data.soil_moisture_data,
-                rfo_model.RF_prediction,
-                rfo_model.MC_mean,
-                rfo_model.dispersion_coefficient,
+                rfo_model,
                 time_step,
-                rfo_model.monte_carlo,
                 output_dir=output_dir,
             )
         if rfo_model.what_to_plot["day_predictor_importance"]:
             plot_predictor_importance(
-                rfo_model.input_data.soil_moisture_data,
+                rfo_model,
                 time_step,
-                rfo_model.input_data.number_predictors,
-                rfo_model.monte_carlo,
-                rfo_model.input_data.predictors.keys(),
-                rfo_model.predictor_importance,
                 output_dir=output_dir,
             )
     if rfo_model.what_to_plot["alldays_predictor_importance"]:
-        predictor_importance_along_days(
-            rfo_model.input_data.number_predictors,
-            rfo_model.input_data.soil_moisture_data.start_times,
-            rfo_model.predictor_importance,
-            rfo_model.input_data.predictors,
-            output_dir=output_dir,
-        )
+        predictor_importance_along_days(rfo_model, output_dir=output_dir)
 
 
-# TODO give only needed argument instead of rfo_model
-def plot_predictors(xaxis, yaxis, predictors, output_dir=None, return_base64_img=False):
+def plot_predictors(rfo_model, output_dir=None, return_base64_img=False):
     """Plot all predictors as color maps, with name and unit."""
-    n_cols = np.ceil(len(predictors) / 2).astype(int)
+    n_cols = np.ceil(len(rfo_model.input_data.predictors) / 2).astype(int)
     fig, ax = plt.subplots(
         nrows=2,
         ncols=n_cols,
         sharex=True,
         sharey=True,
         figsize=(17 * CM_PER_INCH, 9 * CM_PER_INCH),
     )
+    xaxis, yaxis = set_axis(rfo_model)
     fig.subplots_adjust(wspace=0.4)
     plt.rcParams.update({"font.size": 5})
     axes_count = 0
-    for pred_name, predictor in predictors.items():
+    for pred_name, predictor in rfo_model.input_data.predictors.items():
         im = ax.flat[axes_count].pcolormesh(xaxis, yaxis, predictor[0], shading="auto")
         ax.flat[axes_count].set_title(pred_name)
         ax.flat[axes_count].set_aspect(1)
         divider = make_axes_locatable(ax.flat[axes_count])
         cax = divider.append_axes("right", size="5%", pad=0.15)
         cbar = plt.colorbar(im, cax=cax)
         cbar.ax.set_title(predictor[1])
@@ -120,20 +100,20 @@
     if return_base64_img:
         return convert_plt_to_base64(plt)
 
     fig_file_path = os.path.join(output_dir, "predictors.svg")
     plt.savefig(fig_file_path, dpi=300)
 
 
-def prediction_correlation_matrix(input_data, output_dir=None, return_base64_img=False):
+def prediction_correlation_matrix(rfo_model, output_dir=None, return_base64_img=False):
     """Plot the correlation matrix between all predictors, 2 by 2."""
-    ticks = list(input_data.predictors.keys())
+    ticks = list(rfo_model.input_data.predictors.keys())
     plt.figure(figsize=(12 * CM_PER_INCH, 9 * CM_PER_INCH))
     plt.rcParams.update({"font.size": 5})
-    correlation_matrix = input_data.compute_correlation_matrix()
+    correlation_matrix = rfo_model.input_data.compute_correlation_matrix()
     sns.heatmap(
         correlation_matrix,
         annot=True,
         cmap="seismic",
         vmin=-1,
         vmax=1,
         xticklabels=ticks,
@@ -172,57 +152,69 @@
     vertices = np.block([[x_error_end_point, x[::-1]], [y_error_end_point, y[::-1]]]).T
     codes = np.full(len(vertices), Path.LINETO)
     codes[0] = Path.MOVETO
     return Path(vertices, codes)
 
 
 def plot_measurements_vs_distance(
-    soil_moisture_data, time_step, monte_carlo, output_dir=None, return_base64_img=False
+    rfo_model, time_step, output_dir=None, return_base64_img=False
 ):
     """Plot soil moisture measurements vs. cumulative driven distance.
 
     Includes the corresponding low and up standard deviations.
     """
-    start_time = soil_moisture_data.start_times[time_step]
+    start_time = rfo_model.input_data.soil_moisture_data.start_times[time_step]
 
     plt.rcParams.update({"font.size": 7})
     cumulative_distance = [0]
-    for measurement in range(soil_moisture_data.number_measurements[start_time] - 1):
+    for measurement in range(
+        rfo_model.input_data.soil_moisture_data.number_measurements[start_time] - 1
+    ):
         cumulative_distance.append(
             (
                 cumulative_distance[measurement]
                 + np.sqrt(
                     (
-                        soil_moisture_data.x_measurement[start_time][measurement + 1]
-                        - soil_moisture_data.x_measurement[start_time][measurement]
+                        rfo_model.input_data.soil_moisture_data.x_measurement[
+                            start_time
+                        ][measurement + 1]
+                        - rfo_model.input_data.oil_moisture_data.x_measurement[
+                            start_time
+                        ][measurement]
                     )
                     ** 2
                     + (
-                        soil_moisture_data.y_measurement[start_time][measurement + 1]
-                        - soil_moisture_data.y_measurement[start_time][measurement]
+                        rfo_model.input_data.soil_moisture_data.y_measurement[
+                            start_time
+                        ][measurement + 1]
+                        - rfo_model.input_data.soil_moisture_data.y_measurement[
+                            start_time
+                        ][measurement]
                     )
                     ** 2
                 )
                 / 1000
             )
         )
     plt.figure()
     plt.plot(
         cumulative_distance,
-        soil_moisture_data.soil_moisture[start_time],
+        rfo_model.input_data.soil_moisture_data.soil_moisture[start_time],
         "g",
         label="Measurements",
     )
-    if monte_carlo:
+    if rfo_model.monte_carlo:
         plt.fill_between(
             cumulative_distance,
-            soil_moisture_data.soil_moisture[start_time]
-            - soil_moisture_data.soil_moisture_dev_low[start_time],
-            soil_moisture_data.soil_moisture[start_time]
-            + soil_moisture_data.soil_moisture_dev_high[start_time],
+            rfo_model.input_data.soil_moisture_data.soil_moisture[start_time]
+            - rfo_model.input_data.soil_moisture_data.soil_moisture_dev_low[start_time],
+            rfo_model.input_data.soil_moisture_data.soil_moisture[start_time]
+            + rfo_model.input_data.soil_moisture_data.soil_moisture_dev_high[
+                start_time
+            ],
             edgecolor="none",
             alpha=0.3,
             color="purple",
             label="Lower/upper SD",
         )
     plt.ylim([0.1, 0.8])
     plt.xlabel("Cumulative distance (km)")
@@ -233,53 +225,59 @@
         return convert_plt_to_base64(plt)
     fig_file_path = os.path.join(
         output_dir, "measurements_vs_distance_" + start_time + ".svg"
     )
     plt.savefig(fig_file_path, dpi=300)
 
 
-def plot_measurements(
-    soil_moisture_data, time_step, monte_carlo, output_dir=None, return_base64_img=False
-):
+def plot_measurements(rfo_model, time_step, output_dir=None, return_base64_img=False):
     """Plot soil moisture measurements vs. cumulative driven distance.
 
     Includes the corresponding low and up standard deviations.
     """
-    start_time = soil_moisture_data.start_times[time_step]
+    start_time = rfo_model.input_data.soil_moisture_data.start_times[time_step]
 
     plt.figure()
     plt.gca().set_aspect(1)
-    x = soil_moisture_data.x_measurement[start_time] / 1000
-    y = soil_moisture_data.y_measurement[start_time] / 1000
+    x = rfo_model.input_data.soil_moisture_data.x_measurement[start_time] / 1000
+    y = rfo_model.input_data.soil_moisture_data.y_measurement[start_time] / 1000
     sc = plt.scatter(
         x,
         y,
-        c=soil_moisture_data.soil_moisture[start_time],
+        c=rfo_model.input_data.soil_moisture_data.soil_moisture[start_time],
         cmap="Spectral",
         s=5,
         vmin=0.1,
         vmax=0.6,
         zorder=2,
         label="Measurements",
     )
-    if monte_carlo:
+    if rfo_model.monte_carlo:
         plt.gca().add_patch(
             PathPatch(
                 draw_error_band_path(
-                    x, y, -soil_moisture_data.soil_moisture_dev_low[start_time]
+                    x,
+                    y,
+                    -rfo_model.input_data.soil_moisture_data.soil_moisture_dev_low[
+                        start_time
+                    ],
                 ),
                 alpha=0.3,
                 color="purple",
                 label="Lower/upper SD",
             )
         )
         plt.gca().add_patch(
             PathPatch(
                 draw_error_band_path(
-                    x, y, soil_moisture_data.soil_moisture_dev_high[start_time]
+                    x,
+                    y,
+                    rfo_model.input_data.soil_moisture_data.soil_moisture_dev_high[
+                        start_time
+                    ],
                 ),
                 alpha=0.3,
                 color="purple",
             )
         )
     plt.xlabel("Easting (km)")
     plt.ylabel("Northing (km)")
@@ -290,73 +288,49 @@
     if return_base64_img:
         return convert_plt_to_base64(plt)
 
     fig_file_path = os.path.join(output_dir, "measurements_" + start_time + ".svg")
     plt.savefig(fig_file_path, dpi=300)
 
 
-def plot_rfo_model(
-    xaxis,
-    yaxis,
-    soil_moisture_data,
-    rfo_model,
-    mc_mean,
-    dispersion_coefficient,
-    time_step,
-    monte_carlo,
-    *args,
-    **kwargs
-):
+def plot_rfo_model(rfo_model, time_step, *args, **kwargs):
     """Plot random forest prediction as a color map."""
-    if monte_carlo:
-        return plot_rfo_model_with_dispersion(
-            xaxis,
-            yaxis,
-            soil_moisture_data,
-            mc_mean,
-            dispersion_coefficient,
-            time_step,
-            *args,
-            **kwargs
-        )
+    if rfo_model.monte_carlo:
+        return plot_rfo_model_with_dispersion(rfo_model, time_step, *args, **kwargs)
     else:
-        return plot_rfo_model_no_dispersion(
-            xaxis, yaxis, soil_moisture_data, rfo_model, time_step, *args, **kwargs
-        )
+        return plot_rfo_model_no_dispersion(rfo_model, time_step, *args, **kwargs)
 
 
 def plot_rfo_model_no_dispersion(
-    xaxis,
-    yaxis,
-    soil_moisture_data,
     rfo_model,
     time_step,
     output_dir=None,
     return_base64_img=False,
 ):
     """Plot random forest prediction as a color map."""
     if not output_dir:
         output_dir = rfo_model.work_dir
 
-    start_time = soil_moisture_data.start_times[time_step]
+    xaxis, yaxis = set_axis(rfo_model)
+    start_time = rfo_model.input_data.soil_moisture_data.start_times[time_step]
 
     plt.rcParams.update({"font.size": 6})
     fig, ax = plt.subplots(figsize=(16 * CM_PER_INCH, 14 * CM_PER_INCH))
     im = plt.pcolormesh(
         xaxis,
         yaxis,
-        rfo_model[0, time_step, :, :],
+        rfo_model.RF_prediction[0, time_step, :, :],
         vmin=0.1,
         vmax=0.45,
         cmap="Spectral",
     )
 
     plt.scatter(
-        soil_moisture_data.x_measurement[start_time] / 1000,
-        soil_moisture_data.y_measurement[start_time] / 1000,
+        rfo_model.input_data.soil_moisture_data.x_measurement[start_time] / 1000,
+        rfo_model.input_data.soil_moisture_data.y_measurement[start_time] / 1000,
         c="black",
         s=0.5,
     )
     ax.set_title(start_time)
     ax.set_aspect(1)
     cbar = plt.colorbar(im)
     cbar.ax.tick_params(labelsize=14)
@@ -364,59 +338,56 @@
         return convert_plt_to_base64(plt)
 
     fig_file_path = os.path.join(output_dir, "RF_prediction_" + start_time + ".tif")
     plt.savefig(fig_file_path, dpi=300)
 
 
 def plot_rfo_model_with_dispersion(
-    xaxis,
-    yaxis,
-    soil_moisture_data,
-    mc_mean,
-    dispersion_coefficient,
+    rfo_model,
     time_step,
     output_dir=None,
     return_base64_img=False,
 ):
     """Plot SM mean prediction and coefficient of dispersion maps.
 
     Measurement locations are overlaid.
     """
-    start_time = soil_moisture_data.start_times[time_step]
+    xaxis, yaxis = set_axis(rfo_model)
+    start_time = rfo_model.input_data.soil_moisture_data.start_times[time_step]
 
     plt.rcParams.update({"font.size": 7})
 
     fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(16 / 2.54, 10 / 2.54))
     axes[0].set_aspect(1)
     axes[1].set_aspect(1)
 
     divider = make_axes_locatable(axes[0])
     cax = divider.append_axes("right", size="5%", pad=0.15)
     im = axes.flat[0].pcolormesh(
         xaxis,
         yaxis,
-        mc_mean[time_step],
+        rfo_model.MC_mean[time_step],
         shading="auto",
         vmin=0.2,
         vmax=0.5,
         cmap="Spectral",
     )
     axes.flat[0].scatter(
-        soil_moisture_data.x_measurement[start_time] / 1000,
-        soil_moisture_data.y_measurement[start_time] / 1000,
+        rfo_model.input_data.soil_moisture_data.x_measurement[start_time] / 1000,
+        rfo_model.input_data.soil_moisture_data.y_measurement[start_time] / 1000,
         c="black",
         s=1,
     )
     axes.flat[0].set_title("Mean")
     plt.colorbar(im, cax=cax)
 
     im1 = axes.flat[1].pcolormesh(
         xaxis,
         yaxis,
-        dispersion_coefficient[time_step],
+        rfo_model.dispersion_coefficient[time_step],
         shading="auto",
         vmin=0,
         vmax=0.05,
         cmap="Reds",
     )
     axes.flat[1].set_title("Coefficient of dispersion")
     axes.flat[1].tick_params(axis="y", left=False, labelleft=False)
@@ -430,89 +401,89 @@
         return convert_plt_to_base64(plt)
 
     fig_file_path = os.path.join(output_dir, "RF_prediction_" + start_time + ".svg")
     plt.savefig(fig_file_path, dpi=300)
 
 
 def plot_predictor_importance(
-    soil_moisture_data,
+    rfo_model,
     time_step,
-    number_predictors,
-    monte_carlo,
-    predictors,
-    predictor_importance,
     output_dir=None,
     return_base64_img=False,
 ):
     """Plot predictor importance from the RF model."""
-    start_time = soil_moisture_data.start_times[time_step]
+    start_time = rfo_model.input_data.soil_moisture_data.start_times[time_step]
 
     plt.rcParams.update({"font.size": 7})
-    x = np.arange(number_predictors)
+    x = np.arange(rfo_model.input_data.number_predictors)
     plt.figure(figsize=(16 / 2.54, 7 / 2.54))
-    if monte_carlo:
+    if rfo_model.monte_carlo:
         plt.bar(
-            predictors,
+            rfo_model.input_data.predictors.keys(),
             np.percentile(
-                predictor_importance[:, time_step, :],
+                rfo_model.predictor_importance[:, time_step, :],
                 95,
                 axis=0,
             ),
             color="deepskyblue",
             label="q95",
         )
         plt.bar(
-            predictors,
+            rfo_model.input_data.predictors.keys(),
             np.percentile(
-                predictor_importance[:, time_step, :],
+                rfo_model.predictor_importance[:, time_step, :],
                 50,
                 axis=0,
             ),
             color="blue",
             label="median",
         )
         plt.bar(
-            predictors,
+            rfo_model.input_data.predictors.keys(),
             np.percentile(
-                predictor_importance[:, time_step, :],
+                rfo_model.predictor_importance[:, time_step, :],
                 5,
                 axis=0,
             ),
             color="navy",
             label="q5",
         )
         plt.legend()
     else:
-        plt.bar(predictors, predictor_importance[0, time_step, :])
-    plt.xticks(x, predictors)
+        plt.bar(
+            rfo_model.input_data.predictors.keys(),
+            rfo_model.predictor_importance[0, time_step, :],
+        )
+    plt.xticks(x, rfo_model.input_data.predictors.keys())
     plt.title(start_time)
 
     if return_base64_img:
         return convert_plt_to_base64(plt)
 
     fig_file_path = os.path.join(
         output_dir, "predictor_importance_" + start_time + ".svg"
     )
     plt.savefig(fig_file_path, dpi=300)
 
 
 def predictor_importance_along_days(
-    number_predictors,
-    start_times,
-    predictor_importance,
-    predictors,
+    rfo_model,
     apply_pca=False,
     output_dir=None,
     return_base64_img=False,
 ):
     """Plot predictor importance from the RF model.
 
-    input_data     : input_data object containing the list of all predictors
     rfo_model : rfo_model object
     """
+    number_predictors = rfo_model.input_data.number_predictors
+    start_times = rfo_model.input_data.soil_moisture_data.start_times
+    predictor_importance = rfo_model.predictor_importance
+    predictors = rfo_model.input_data.predictors
+
     plt.rcParams.update({"font.size": 7})
     fig, ax = plt.subplots(
         number_predictors,
         sharex=True,
         figsize=(17 / 2.54, 16 / 2.54),
     )
     if not apply_pca:
```

### Comparing `soil_moisture_prediction-0.0.6/soil_moisture_prediction/random_forest_model.py` & `soil_moisture_prediction-0.0.9/soil_moisture_prediction/random_forest_model.py`

 * *Files identical despite different names*

### Comparing `soil_moisture_prediction-0.0.6/soil_moisture_prediction/soil_moisture_prediction.py` & `soil_moisture_prediction-0.0.9/soil_moisture_prediction/smp_cli.py`

 * *Files identical despite different names*

### Comparing `soil_moisture_prediction-0.0.6/PKG-INFO` & `soil_moisture_prediction-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soil-moisture-prediction
-Version: 0.0.6
+Version: 0.0.9
 Summary: Predicts soil moisture from cosmic ray neutron sensor data using a random forest model
 License: EUPL 1.2
 Author: Segolene Dega
 Author-email: segolene.dega@ufz.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

