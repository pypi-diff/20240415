# Comparing `tmp/darfix-1.0.1rc0.tar.gz` & `tmp/darfix-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darfix-1.0.1rc0.tar", last modified: Mon Mar 25 17:22:48 2024, max compression
+gzip compressed data, was "darfix-1.0.1rc1.tar", last modified: Mon Apr 15 12:10:21 2024, max compression
```

## Comparing `darfix-1.0.1rc0.tar` & `darfix-1.0.1rc1.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.726016 darfix-1.0.1rc0/
--rw-rw-rw-   0 root         (0) root         (0)     1110 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5225 2024-03-25 17:22:48.726016 darfix-1.0.1rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1759 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-03-25 17:22:48.726016 darfix-1.0.1rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.522016 darfix-1.0.1rc0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.526016 darfix-1.0.1rc0/src/darfix/
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-03-25 16:04:12.000000 darfix-1.0.1rc0/src/darfix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.526016 darfix-1.0.1rc0/src/darfix/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2903 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/app/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.530016 darfix-1.0.1rc0/src/darfix/core/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/autofocus.py
--rw-rw-rw-   0 root         (0) root         (0)     9947 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/componentsMatching.py
--rw-rw-rw-   0 root         (0) root         (0)     3610 2024-03-25 17:04:41.000000 darfix-1.0.1rc0/src/darfix/core/data_selection.py
--rw-rw-rw-   0 root         (0) root         (0)   103543 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9180 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/geneticShiftDetection.py
--rw-rw-rw-   0 root         (0) root         (0)     6945 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/imageOperations.py
--rw-rw-rw-   0 root         (0) root         (0)    12049 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/imageRegistration.py
--rw-rw-rw-   0 root         (0) root         (0)    19114 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/mapping.py
--rw-rw-rw-   0 root         (0) root         (0)    17222 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/roi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.530016 darfix-1.0.1rc0/src/darfix/core/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/core/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2677 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_components_matching.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_data_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31816 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    15661 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     4119 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_ga.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_image_operations.py
--rw-rw-rw-   0 root         (0) root         (0)    15939 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_image_registration.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_roi.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/test/test_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.534016 darfix-1.0.1rc0/src/darfix/decomposition/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6589 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10875 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/ipca.py
--rw-rw-rw-   0 root         (0) root         (0)     3997 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/nica.py
--rw-rw-rw-   0 root         (0) root         (0)     4463 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/nmf.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.534016 darfix-1.0.1rc0/src/darfix/decomposition/test/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/test_ipca.py
--rw-rw-rw-   0 root         (0) root         (0)     4709 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/test_nica.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/test_nmf.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/decomposition/test/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/dtypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.538016 darfix-1.0.1rc0/src/darfix/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1886 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/PCAWidget.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5275 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/binningWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     7057 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/blindSourceSeparationWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6123 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/dataPartitionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    14225 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/datasetSelectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    25338 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/dimensionsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    13147 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/displayComponentsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    19805 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/grainPlotWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/lineProfileWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     7928 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/linkComponentsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6617 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/magnificationWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     3538 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/metadataWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    21760 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/noiseRemovalWidget.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/operationThread.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/projectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    22733 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/rockingCurvesWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/roiLimitsToolbar.py
--rw-rw-rw-   0 root         (0) root         (0)     9458 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/roiSelectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/rsmHistogramWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/rsmWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    13880 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/shiftCorrectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/showStackWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6627 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3869 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/weakBeamWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/gui/zSumWidget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.538016 darfix-1.0.1rc0/src/darfix/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/io/dataset_io.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/io/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/io/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.538016 darfix-1.0.1rc0/src/darfix/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.538016 darfix-1.0.1rc0/src/darfix/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.542016 darfix-1.0.1rc0/src/darfix/resources/gui/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/curves.png
--rw-rw-rw-   0 root         (0) root         (0)     6830 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/curves.svg
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/resize.png
--rw-rw-rw-   0 root         (0) root         (0)     8233 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/resize.svg
--rw-rw-rw-   0 root         (0) root         (0)     1068 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/scatter.png
--rw-rw-rw-   0 root         (0) root         (0)    20421 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/resources/gui/icons/scatter.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.542016 darfix-1.0.1rc0/src/darfix/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/darfix/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8871 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/darfix/test/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.706016 darfix-1.0.1rc0/src/darfix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5225 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6752 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      293 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1482 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:22:48.000000 darfix-1.0.1rc0/src/darfix.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.522016 darfix-1.0.1rc0/src/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.542016 darfix-1.0.1rc0/src/orangecontrib/darfix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.542016 darfix-1.0.1rc0/src/orangecontrib/darfix/test/
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/test/test_ewoks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.610016 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7661 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/darfix_example1.ows
--rw-rw-rw-   0 root         (0) root         (0)     5116 2024-03-25 07:59:37.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/darfix_example2.ows
--rw-rw-rw-   0 root         (0) root         (0)  8391680 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/strain_0000.edf
--rw-rw-rw-   0 root         (0) root         (0)  8403250 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/strain_0001.edf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.678016 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/binning.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/blindsourceseparation.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/datacopy.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/datapartition.py
--rw-rw-rw-   0 root         (0) root         (0)     4405 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/dataselection.py
--rw-rw-rw-   0 root         (0) root         (0)     4075 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/flash.py
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/grainplot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.706016 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 17:22:42.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/axes.png
--rw-rw-rw-   0 root         (0) root         (0)     5038 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/axes.svg
--rw-rw-rw-   0 root         (0) root         (0)     3212 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/bss.png
--rw-rw-rw-   0 root         (0) root         (0)     4986 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/bss.svg
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     8068 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/copy.svg
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/curves.png
--rw-rw-rw-   0 root         (0) root         (0)    51435 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/curves.svg
--rw-rw-rw-   0 root         (0) root         (0)   233309 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon.png
--rw-rw-rw-   0 root         (0) root         (0)    35611 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg
--rw-rw-rw-   0 root         (0) root         (0)   236860 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/filter.png
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/filter.svg
--rw-rw-rw-   0 root         (0) root         (0)     2709 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/flash.svg
--rw-rw-rw-   0 root         (0) root         (0)     4286 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/gaussian.png
--rw-rw-rw-   0 root         (0) root         (0)    10053 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/gaussian.svg
--rw-rw-rw-   0 root         (0) root         (0)    22180 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/grainplot.png
--rw-rw-rw-   0 root         (0) root         (0)  2409867 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/grainplot.svg
--rw-rw-rw-   0 root         (0) root         (0)    64642 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/image-select-box.svg
--rw-rw-rw-   0 root         (0) root         (0)    16836 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/line_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   132131 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/line_profile.svg
--rw-rw-rw-   0 root         (0) root         (0)     9458 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/link.png
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/link.svg
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/metadata.png
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/metadata.svg
--rw-rw-rw-   0 root         (0) root         (0)      631 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/mywidget.svg
--rw-rw-rw-   0 root         (0) root         (0)     6218 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal.png
--rw-rw-rw-   0 root         (0) root         (0)     4375 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal.svg
--rw-rw-rw-   0 root         (0) root         (0)     6897 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg
--rw-rw-rw-   0 root         (0) root         (0)     3583 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/param_dims.png
--rw-rw-rw-   0 root         (0) root         (0)     9708 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/param_dims.svg
--rw-rw-rw-   0 root         (0) root         (0)     4325 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/pca.png
--rw-rw-rw-   0 root         (0) root         (0)    21388 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/pca.svg
--rw-rw-rw-   0 root         (0) root         (0)     2140 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/random.svg
--rw-rw-rw-   0 root         (0) root         (0)      857 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/resize.png
--rw-rw-rw-   0 root         (0) root         (0)     6668 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/roi.png
--rw-rw-rw-   0 root         (0) root         (0)    66544 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/roi.svg
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/save.svg
--rw-rw-rw-   0 root         (0) root         (0)     8108 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/shift_correction.svg
--rw-rw-rw-   0 root         (0) root         (0)     4978 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/upload.svg
--rw-rw-rw-   0 root         (0) root         (0)     2853 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/zsum.svg
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/lineprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/linkcomponents.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/noiseremoval.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/pca.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/projection.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/rockingcurves.py
--rw-rw-rw-   0 root         (0) root         (0)     2655 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/roiselection.py
--rw-rw-rw-   0 root         (0) root         (0)     2715 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/rsmhistogram.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/shiftcorrection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:22:48.706016 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/test/
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/test/test_data_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     5740 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/weakbeam.py
--rw-rw-rw-   0 root         (0) root         (0)     1172 2024-03-25 07:59:38.000000 darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/zsum.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.592047 darfix-1.0.1rc1/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1110 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     5255 2024-04-15 12:10:21.592047 darfix-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     2778 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/README.rst
+-rw-r--r--   0 payno     (1000) payno     (1000)      302 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)     2120 2024-04-15 12:10:21.592047 darfix-1.0.1rc1/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       69 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/darfix/
+-rw-r--r--   0 payno     (1000) payno     (1000)      546 2024-04-15 09:58:22.000000 darfix-1.0.1rc1/src/darfix/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      654 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/_config.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/darfix/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/app/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2903 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/app/__main__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/darfix/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      344 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/core/autofocus.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9947 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/componentsMatching.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3610 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/core/data_selection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)   104214 2024-04-15 09:53:18.000000 darfix-1.0.1rc1/src/darfix/core/dataset.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9183 2024-04-15 09:53:22.000000 darfix-1.0.1rc1/src/darfix/core/dimension.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7361 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/geneticShiftDetection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6945 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/imageOperations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12049 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/core/imageRegistration.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19114 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/core/mapping.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    17222 2024-02-13 08:51:56.000000 darfix-1.0.1rc1/src/darfix/core/process.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3234 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/roi.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/darfix/core/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2677 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_components_matching.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1104 2024-02-13 08:51:56.000000 darfix-1.0.1rc1/src/darfix/core/test/test_data_selection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    32117 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/core/test/test_dataset.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15661 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_dimension.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4119 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/test/test_ga.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7140 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_image_operations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15939 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_image_registration.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5153 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/test/test_mapping.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3500 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_roi.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3550 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/core/test/test_workflow.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      950 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/decomposition/
+-rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6589 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/base.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10875 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/decomposition/ipca.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3997 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/nica.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4463 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/nmf.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3540 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/pca.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/decomposition/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1792 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/test_base.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3449 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/test_ipca.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4709 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/test_nica.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1396 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/test_nmf.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1497 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/decomposition/test/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1494 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/dtypes.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/gui/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1886 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/PCAWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       73 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5275 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/gui/binningWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7057 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/blindSourceSeparationWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6123 2024-03-20 10:11:33.000000 darfix-1.0.1rc1/src/darfix/gui/dataPartitionWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    14268 2024-04-15 09:53:18.000000 darfix-1.0.1rc1/src/darfix/gui/datasetSelectionWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    25221 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/gui/dimensionsWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13147 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/displayComponentsWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    19805 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/grainPlotWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2018 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/lineProfileWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7928 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/linkComponentsWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6617 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/magnificationWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3410 2024-04-15 09:53:18.000000 darfix-1.0.1rc1/src/darfix/gui/metadataWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    21925 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/darfix/gui/noiseRemovalWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      716 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/operationThread.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4105 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/projectionWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    22733 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/rockingCurvesWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3527 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/roiLimitsToolbar.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9458 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/roiSelectionWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10021 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/rsmHistogramWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2610 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/rsmWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    13880 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/shiftCorrectionWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1707 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/showStackWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6627 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3869 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/gui/weakBeamWidget.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2449 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/gui/zSumWidget.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/io/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/io/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2284 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/io/dataset_io.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       64 2024-02-13 08:51:56.000000 darfix-1.0.1rc1/src/darfix/io/hdf5.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    10758 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/io/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/resources/gui/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/resources/gui/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1363 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/curves.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6830 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/curves.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2555 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/resize.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     8233 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/resize.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     1068 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/scatter.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    20421 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/resources/gui/icons/scatter.svg
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/darfix/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/darfix/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1159 2024-02-13 15:27:02.000000 darfix-1.0.1rc1/src/darfix/test/conftest.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8871 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/darfix/test/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.584047 darfix-1.0.1rc1/src/darfix.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     5255 2024-04-15 12:10:19.000000 darfix-1.0.1rc1/src/darfix.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     6816 2024-04-15 12:10:20.000000 darfix-1.0.1rc1/src/darfix.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-15 12:10:19.000000 darfix-1.0.1rc1/src/darfix.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      293 2024-04-15 12:10:19.000000 darfix-1.0.1rc1/src/darfix.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     1497 2024-04-15 12:10:19.000000 darfix-1.0.1rc1/src/darfix.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       30 2024-04-15 12:10:19.000000 darfix-1.0.1rc1/src/darfix.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.568047 darfix-1.0.1rc1/src/orangecontrib/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/orangecontrib/darfix/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.572047 darfix-1.0.1rc1/src/orangecontrib/darfix/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)      482 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/test/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1782 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/test/test_ewoks.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.576047 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7661 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/darfix_example1.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)     5116 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/darfix_example2.ows
+-rw-r--r--   0 payno     (1000) payno     (1000)  8391680 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/strain_0000.edf
+-rw-r--r--   0 payno     (1000) payno     (1000)  8403250 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/strain_0001.edf
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.584047 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1133 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1920 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/binning.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2182 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/blindsourceseparation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1462 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/datacopy.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2145 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/datapartition.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4491 2024-04-15 09:19:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/dataselection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     4075 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/dimensions.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1425 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/flash.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1390 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/grainplot.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.584047 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1599 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/axes.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     5038 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/axes.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3212 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/bss.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4986 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/bss.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      506 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/category.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8068 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/copy.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      912 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/curves.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    51435 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/curves.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   233309 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    35611 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)   236860 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png
+-rw-r--r--   0 payno     (1000) payno     (1000)      621 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/filter.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2253 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/filter.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2709 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/flash.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4286 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/gaussian.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    10053 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/gaussian.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    22180 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/grainplot.png
+-rw-r--r--   0 payno     (1000) payno     (1000)  2409867 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/grainplot.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    64642 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/image-select-box.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)    16836 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/line_profile.png
+-rw-r--r--   0 payno     (1000) payno     (1000)   132131 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/line_profile.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     9458 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/link.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     2431 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/link.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      593 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/metadata.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     3126 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/metadata.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      631 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/mywidget.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     6218 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     4375 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     6897 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3583 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/param_dims.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     9708 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/param_dims.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4325 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/pca.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    21388 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/pca.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2140 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/random.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      857 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/resize.png
+-rw-r--r--   0 payno     (1000) payno     (1000)     6668 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/roi.png
+-rw-r--r--   0 payno     (1000) payno     (1000)    66544 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/roi.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     3260 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/save.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     8108 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/shift_correction.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     4978 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/upload.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)     2853 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/zsum.svg
+-rw-r--r--   0 payno     (1000) payno     (1000)      554 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/lineprofile.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      561 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/linkcomponents.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1014 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/metadata.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3887 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/noiseremoval.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1294 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/pca.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1987 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/projection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1523 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/rockingcurves.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2655 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/roiselection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2715 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/rsmhistogram.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2469 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/shiftcorrection.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.584047 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1279 2024-03-20 10:11:34.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/test/test_data_selection.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5740 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1942 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/weakbeam.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1172 2024-01-26 09:09:46.000000 darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/zsum.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-15 12:10:21.584047 darfix-1.0.1rc1/src/snippets/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1691 2024-02-13 12:43:36.000000 darfix-1.0.1rc1/src/snippets/convert_edf_to_hdf5.py
```

### Comparing `darfix-1.0.1rc0/LICENSE` & `darfix-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/PKG-INFO` & `darfix-1.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darfix
-Version: 1.0.1rc0
+Version: 1.0.1rc1
 Summary: Computer vision software for the interpretation of diffraction images
 Home-page: https://gitlab.esrf.fr/XRD/darfix
 Author: J.Garriga
 Author-email: julia.garriga@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/XRD/darfix/
 Project-URL: Documentation, http://www.edna-site.org/pub/doc/darfix/latest
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: silx<2.0.0,>=1.1.2
+Requires-Dist: matplotlib<3.9
 Requires-Dist: ewoks>=0.1.0
 Requires-Dist: ewokscore>=0.1.1
 Requires-Dist: chardet<5.0.0; python_version < "3.7"
 Requires-Dist: packaging
 Provides-Extra: full
 Requires-Dist: matplotlib>=1.2.0; extra == "full"
 Requires-Dist: opencv-python-headless<4.7,>=4.3.0.36; extra == "full"
```

### Comparing `darfix-1.0.1rc0/setup.cfg` & `darfix-1.0.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 package_dir = 
 	=src
 packages = find_namespace:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	silx >=1.1.2,<2.0.0
+	matplotlib<3.9
 	ewoks >=0.1.0
 	ewokscore >=0.1.1
 	chardet <5.0.0; python_version < "3.7"
 	packaging
 
 [options.packages.find]
 where = src
@@ -90,14 +91,13 @@
 
 [flake8_nb]
 ignore = E501, E203, W503, E402
 max-line-length = 88
 
 [coverage:run]
 omit = 
-	src/darfix/tests/*
-	src/orangecontrib/tests/*
+	*/test/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `darfix-1.0.1rc0/src/darfix/__init__.py` & `darfix-1.0.1rc1/src/darfix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 - silx.io: Functions for input/output operations
 - silx.utils: Miscellaneous convenient functions
 """
 
 __authors__ = ["J. Garriga"]
 __license__ = "MIT"
 __date__ = "16/12/2019"
-__version__ = "1.0.1rc0"
+__version__ = "1.0.1rc1"
 
 from ._config import Config as _Config
 
 config = _Config()
 """Global configuration shared with the whole library"""
```

### Comparing `darfix-1.0.1rc0/src/darfix/_config.py` & `darfix-1.0.1rc1/src/darfix/_config.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/app/__main__.py` & `darfix-1.0.1rc1/src/darfix/app/__main__.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/componentsMatching.py` & `darfix-1.0.1rc1/src/darfix/core/componentsMatching.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/data_selection.py` & `darfix-1.0.1rc1/src/darfix/core/data_selection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/dataset.py` & `darfix-1.0.1rc1/src/darfix/core/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,5886 +587,5928 @@
 000024a0: 5f48 4446 354d 6574 6164 6174 6152 6561  _HDF5MetadataRea
 000024b0: 6465 7228 6d65 7461 6461 7461 3d6d 6574  der(metadata=met
 000024c0: 6164 6174 6129 0a0a 2020 2020 2020 2020  adata)..        
 000024d0: 2020 2020 2020 2020 7769 7468 2073 696c          with sil
 000024e0: 782e 696f 2e6f 7065 6e28 7572 6c2e 6669  x.io.open(url.fi
 000024f0: 6c65 5f70 6174 6828 2929 2061 7320 6835  le_path()) as h5
 00002500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002510: 2020 2020 2020 6e5f 6672 616d 6573 203d        n_frames =
-00002520: 2068 355b 7572 6c2e 6461 7461 5f70 6174   h5[url.data_pat
-00002530: 6828 295d 2e73 6861 7065 5b30 5d0a 2020  h()].shape[0].  
-00002540: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00002550: 7220 6920 696e 2072 616e 6765 286e 5f66  r i in range(n_f
-00002560: 7261 6d65 7329 3a0a 2020 2020 2020 2020  rames):.        
-00002570: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00002580: 5f75 726c 732e 6170 7065 6e64 280a 2020  _urls.append(.  
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 2020 2020 2020 4461 7461 5572 6c28 0a20        DataUrl(. 
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-000025d0: 7061 7468 3d75 726c 2e66 696c 655f 7061  path=url.file_pa
-000025e0: 7468 2829 2c0a 2020 2020 2020 2020 2020  th(),.          
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 6461 7461 5f70 6174 683d 7572 6c2e    data_path=url.
-00002610: 6461 7461 5f70 6174 6828 292c 0a20 2020  data_path(),.   
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 2064 6174 615f 736c           data_sl
-00002640: 6963 653d 692c 0a20 2020 2020 2020 2020  ice=i,.         
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2073 6368 656d 653d 2273 696c 7822     scheme="silx"
-00002670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002680: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000026b0: 2020 2020 2020 6d65 7461 6461 7461 2e61        metadata.a
-000026c0: 7070 656e 6428 6765 745f 6d65 7461 6461  ppend(get_metada
-000026d0: 7461 2864 6174 615f 736c 6963 653d 6929  ta(data_slice=i)
-000026e0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000026f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00002700: 2020 2020 7769 7468 2066 6162 696f 2e6f      with fabio.o
-00002710: 7065 6e5f 7365 7269 6573 280a 2020 2020  pen_series(.    
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 6669 6c65 6e61 6d65 733d 6669 6c65 6e61  filenames=filena
-00002740: 6d65 732c 2066 6972 7374 5f66 696c 656e  mes, first_filen
-00002750: 616d 653d 6669 7273 745f 6669 6c65 6e61  ame=first_filena
-00002760: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-00002770: 2020 2029 2061 7320 7365 7269 6573 3a0a     ) as series:.
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2020 2020 666f 7220 6672 616d 6520 696e      for frame in
-000027a0: 2073 6572 6965 732e 6672 616d 6573 2829   series.frames()
-000027b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000027c0: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
-000027d0: 6d65 203d 2066 7261 6d65 2e66 696c 655f  me = frame.file_
-000027e0: 636f 6e74 6169 6e65 722e 6669 6c65 6e61  container.filena
-000027f0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-00002800: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00002810: 7572 6c73 2e61 7070 656e 6428 4461 7461  urls.append(Data
-00002820: 5572 6c28 6669 6c65 5f70 6174 683d 6669  Url(file_path=fi
-00002830: 6c65 6e61 6d65 2c20 7363 6865 6d65 3d22  lename, scheme="
-00002840: 6661 6269 6f22 2929 0a20 2020 2020 2020  fabio")).       
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2066 6162 696f 5f72 6561 6465 7220 3d20   fabio_reader = 
-00002870: 6661 6269 6f68 352e 4564 6646 6162 696f  fabioh5.EdfFabio
-00002880: 5265 6164 6572 2866 696c 655f 6e61 6d65  Reader(file_name
-00002890: 3d66 696c 656e 616d 6529 0a20 2020 2020  =filename).     
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 206d 6574 6164 6174 612e 6170 7065     metadata.appe
-000028c0: 6e64 2866 6162 696f 5f72 6561 6465 7229  nd(fabio_reader)
-000028d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028e0: 2020 2020 2020 2020 2066 6162 696f 5f72           fabio_r
-000028f0: 6561 6465 722e 636c 6f73 6528 290a 2020  eader.close().  
-00002900: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002910: 6461 7461 203d 2044 6174 6128 0a20 2020  data = Data(.   
-00002920: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00002930: 7079 2e61 7272 6179 2864 6174 615f 7572  py.array(data_ur
-00002940: 6c73 292c 206d 6574 6164 6174 613d 6d65  ls), metadata=me
-00002950: 7461 6461 7461 2c20 696e 5f6d 656d 6f72  tadata, in_memor
-00002960: 793d 7365 6c66 2e5f 696e 5f6d 656d 6f72  y=self._in_memor
-00002970: 790a 2020 2020 2020 2020 2020 2020 290a  y.            ).
-00002980: 0a20 2020 2064 6566 2073 746f 705f 6f70  .    def stop_op
-00002990: 6572 6174 696f 6e28 7365 6c66 2c20 6f70  eration(self, op
-000029a0: 6572 6174 696f 6e29 3a0a 2020 2020 2020  eration):.      
-000029b0: 2020 2222 220a 2020 2020 2020 2020 4d65    """.        Me
-000029c0: 7468 6f64 2075 7365 6420 666f 7220 6361  thod used for ca
-000029d0: 7365 7320 7768 6572 6520 7468 7265 6164  ses where thread
-000029e0: 7320 6172 6520 6372 6561 7465 6420 746f  s are created to
-000029f0: 2061 7070 6c79 2066 756e 6374 696f 6e73   apply functions
-00002a00: 2074 6f20 7468 6520 6461 7461 7365 742e   to the dataset.
-00002a10: 0a20 2020 2020 2020 2049 6620 6d65 7468  .        If meth
-00002a20: 6f64 2069 7320 6361 6c6c 6564 2c20 7468  od is called, th
-00002a30: 6520 666c 6167 2063 6f6e 6365 726e 696e  e flag concernin
-00002a40: 6720 7468 6520 7374 6f70 2069 7320 7365  g the stop is se
-00002a50: 7420 746f 2030 2073 6f20 7468 6174 2069  t to 0 so that i
-00002a60: 6620 7468 6520 636f 6e63 6572 6e65 640a  f the concerned.
-00002a70: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-00002a80: 6e20 6973 2072 756e 6e69 6e67 2069 6e20  n is running in 
-00002a90: 616e 6f74 6865 7220 7468 7265 6164 2069  another thread i
-00002aa0: 7420 6b6e 6f77 7320 746f 2073 746f 702e  t knows to stop.
-00002ab0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002ac0: 2069 6e74 206f 7065 7261 7469 6f6e 3a20   int operation: 
-00002ad0: 6f70 6572 6174 696f 6e20 746f 2073 746f  operation to sto
-00002ae0: 700a 2020 2020 2020 2020 3a74 7970 6520  p.        :type 
-00002af0: 696e 743a 2055 6e69 6f6e 5b69 6e74 2c20  int: Union[int, 
-00002b00: 604f 7065 7261 7469 6f6e 605d 0a20 2020  `Operation`].   
-00002b10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002b20: 2069 6620 7365 6c66 2e73 7461 7465 5f6f   if self.state_o
-00002b30: 665f 6f70 6572 6174 696f 6e73 2e69 735f  f_operations.is_
-00002b40: 7275 6e6e 696e 6728 6f70 6572 6174 696f  running(operatio
-00002b50: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00002b60: 7365 6c66 2e73 7461 7465 5f6f 665f 6f70  self.state_of_op
-00002b70: 6572 6174 696f 6e73 2e73 746f 7028 6f70  erations.stop(op
-00002b80: 6572 6174 696f 6e29 0a20 2020 2020 2020  eration).       
-00002b90: 2069 6620 7365 6c66 2e72 756e 6e69 6e67   if self.running
-00002ba0: 5f64 6174 6120 6973 206e 6f74 204e 6f6e  _data is not Non
-00002bb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00002bc0: 656c 662e 7275 6e6e 696e 675f 6461 7461  elf.running_data
-00002bd0: 2e73 746f 705f 6f70 6572 6174 696f 6e28  .stop_operation(
-00002be0: 6f70 6572 6174 696f 6e29 0a0a 2020 2020  operation)..    
-00002bf0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00002c00: 6620 7472 616e 7366 6f72 6d61 7469 6f6e  f transformation
-00002c10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00002c20: 7265 7475 726e 2073 656c 662e 5f74 7261  return self._tra
-00002c30: 6e73 666f 726d 6174 696f 6e0a 0a20 2020  nsformation..   
-00002c40: 2040 7472 616e 7366 6f72 6d61 7469 6f6e   @transformation
-00002c50: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00002c60: 7472 616e 7366 6f72 6d61 7469 6f6e 2873  transformation(s
-00002c70: 656c 662c 2076 616c 7565 293a 0a20 2020  elf, value):.   
-00002c80: 2020 2020 2073 656c 662e 5f74 7261 6e73       self._trans
-00002c90: 666f 726d 6174 696f 6e20 3d20 7661 6c75  formation = valu
-00002ca0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-00002cb0: 0a20 2020 2064 6566 2074 6974 6c65 2873  .    def title(s
-00002cc0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00002cd0: 7475 726e 2073 656c 662e 5f74 6974 6c65  turn self._title
-00002ce0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00002cf0: 2020 2020 6465 6620 6469 7228 7365 6c66      def dir(self
-00002d00: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00002d10: 6e20 7365 6c66 2e5f 6469 720a 0a20 2020  n self._dir..   
-00002d20: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00002d30: 6566 2069 735f 6835 2873 656c 6629 3a0a  ef is_h5(self):.
-00002d40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002d50: 656c 662e 5f69 7348 350a 0a20 2020 2064  elf._isH5..    d
-00002d60: 6566 2063 6f6d 7075 7465 5f66 7261 6d65  ef compute_frame
-00002d70: 735f 696e 7465 6e73 6974 7928 7365 6c66  s_intensity(self
-00002d80: 2c20 6b65 726e 656c 3d28 332c 2033 292c  , kernel=(3, 3),
-00002d90: 2073 6967 6d61 3d32 3029 3a0a 2020 2020   sigma=20):.    
-00002da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002db0: 5265 7475 726e 7320 666f 7220 6576 6572  Returns for ever
-00002dc0: 7920 696d 6167 6520 6120 6e75 6d62 6572  y image a number
-00002dd0: 2072 6570 7265 7365 6e74 696e 6720 6974   representing it
-00002de0: 7320 696e 7465 6e73 6974 792e 2054 6869  s intensity. Thi
-00002df0: 7320 6e75 6d62 6572 0a20 2020 2020 2020  s number.       
-00002e00: 2069 7320 6f62 7461 696e 6564 2062 7920   is obtained by 
-00002e10: 6669 7273 7420 626c 7572 7269 6e67 2074  first blurring t
-00002e20: 6865 2069 6d61 6765 2061 6e64 2074 6865  he image and the
-00002e30: 6e20 636f 6d70 7574 696e 6720 6974 7320  n computing its 
-00002e40: 7661 7269 616e 6365 2e0a 2020 2020 2020  variance..      
-00002e50: 2020 2222 220a 2020 2020 2020 2020 5f6c    """.        _l
-00002e60: 6f67 6765 722e 696e 666f 2822 436f 6d70  ogger.info("Comp
-00002e70: 7574 696e 6720 696e 7465 6e73 6974 7920  uting intensity 
-00002e80: 7065 7220 6672 616d 6522 290a 2020 2020  per frame").    
-00002e90: 2020 2020 696f 5f75 7469 6c73 2e61 6476      io_utils.adv
-00002ea0: 616e 6365 6d65 6e74 5f64 6973 706c 6179  ancement_display
-00002eb0: 2830 2c20 7365 6c66 2e6e 6672 616d 6573  (0, self.nframes
-00002ec0: 2c20 2243 6f6d 7075 7469 6e67 2069 6e74  , "Computing int
-00002ed0: 656e 7369 7479 2229 0a20 2020 2020 2020  ensity").       
-00002ee0: 2066 7261 6d65 735f 696e 7465 6e73 6974   frames_intensit
-00002ef0: 7920 3d20 5b5d 0a20 2020 2020 2020 2077  y = [].        w
-00002f00: 6974 6820 7365 6c66 2e73 7461 7465 5f6f  ith self.state_o
-00002f10: 665f 6f70 6572 6174 696f 6e73 2e72 756e  f_operations.run
-00002f20: 5f63 6f6e 7465 7874 284f 7065 7261 7469  _context(Operati
-00002f30: 6f6e 2e50 4152 5449 5449 4f4e 293a 0a20  on.PARTITION):. 
-00002f40: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00002f50: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00002f60: 6672 616d 6573 293a 0a20 2020 2020 2020  frames):.       
-00002f70: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
-00002f80: 6376 320a 0a20 2020 2020 2020 2020 2020  cv2..           
-00002f90: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00002fa0: 2e73 7461 7465 5f6f 665f 6f70 6572 6174  .state_of_operat
-00002fb0: 696f 6e73 2e69 735f 7275 6e6e 696e 6728  ions.is_running(
-00002fc0: 4f70 6572 6174 696f 6e2e 5041 5254 4954  Operation.PARTIT
-00002fd0: 494f 4e29 3a0a 2020 2020 2020 2020 2020  ION):.          
-00002fe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003000: 2066 7261 6d65 735f 696e 7465 6e73 6974   frames_intensit
-00003010: 7920 2b3d 205b 0a20 2020 2020 2020 2020  y += [.         
-00003020: 2020 2020 2020 2020 2020 2063 7632 2e47             cv2.G
-00003030: 6175 7373 6961 6e42 6c75 7228 7365 6c66  aussianBlur(self
-00003040: 2e67 6574 5f64 6174 6128 6929 2c20 6b65  .get_data(i), ke
-00003050: 726e 656c 2c20 7369 676d 6129 2e76 6172  rnel, sigma).var
-00003060: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00003070: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00003080: 2020 2020 2069 6f5f 7574 696c 732e 6164       io_utils.ad
-00003090: 7661 6e63 656d 656e 745f 6469 7370 6c61  vancement_displa
-000030a0: 7928 6920 2b20 312c 2073 656c 662e 6e66  y(i + 1, self.nf
-000030b0: 7261 6d65 732c 2022 436f 6d70 7574 696e  rames, "Computin
-000030c0: 6720 696e 7465 6e73 6974 7922 290a 2020  g intensity").  
-000030d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000030e0: 6672 616d 6573 5f69 6e74 656e 7369 7479  frames_intensity
-000030f0: 203d 2066 7261 6d65 735f 696e 7465 6e73   = frames_intens
-00003100: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
-00003110: 7265 7475 726e 2066 7261 6d65 735f 696e  return frames_in
-00003120: 7465 6e73 6974 790a 0a20 2020 2064 6566  tensity..    def
-00003130: 2070 6172 7469 7469 6f6e 5f62 795f 696e   partition_by_in
-00003140: 7465 6e73 6974 7928 7365 6c66 2c20 6269  tensity(self, bi
-00003150: 6e73 3d4e 6f6e 652c 2062 6f74 746f 6d5f  ns=None, bottom_
-00003160: 6269 6e3d 4e6f 6e65 2c20 746f 705f 6269  bin=None, top_bi
-00003170: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00003180: 2022 2222 0a20 2020 2020 2020 2046 756e   """.        Fun
-00003190: 6374 696f 6e20 7468 6174 2063 6f6d 7075  ction that compu
-000031a0: 7465 7320 7468 6520 6461 7461 2066 726f  tes the data fro
-000031b0: 6d20 7468 6520 7365 7420 6f66 2075 726c  m the set of url
-000031c0: 732e 0a20 2020 2020 2020 2049 6620 7468  s..        If th
-000031d0: 6520 6669 6c74 6572 5f64 6174 6120 666c  e filter_data fl
-000031e0: 6167 2069 7320 6163 7469 7661 7465 6420  ag is activated 
-000031f0: 6974 2066 696c 7465 7273 2074 6865 2064  it filters the d
-00003200: 6174 6120 666f 6c6c 6f77 696e 6720 7468  ata following th
-00003210: 6520 6e65 7874 3a0a 2020 2020 2020 2020  e next:.        
-00003220: 2d2d 2046 6972 7374 2c20 6974 2063 6f6d  -- First, it com
-00003230: 7075 7465 7320 7468 6520 696e 7465 6e73  putes the intens
-00003240: 6974 7920 666f 7220 6561 6368 2066 7261  ity for each fra
-00003250: 6d65 2c20 6279 2063 616c 6375 6c61 7469  me, by calculati
-00003260: 6e67 2074 6865 2076 6172 6961 6e63 6520  ng the variance 
-00003270: 6166 7465 720a 2020 2020 2020 2020 7061  after.        pa
-00003280: 7373 696e 6720 6120 6761 7573 7369 616e  ssing a gaussian
-00003290: 2066 696c 7465 722e 0a20 2020 2020 2020   filter..       
-000032a0: 202d 2d20 5365 636f 6e64 2c20 636f 6d70   -- Second, comp
-000032b0: 7574 6573 2074 6865 2068 6973 746f 6772  utes the histogr
-000032c0: 616d 206f 6620 7468 6520 696e 7465 6e73  am of the intens
-000032d0: 6974 792e 0a20 2020 2020 2020 202d 2d20  ity..        -- 
-000032e0: 4669 6e61 6c6c 792c 2073 6176 6573 2074  Finally, saves t
-000032f0: 6865 2064 6174 6120 6f66 2074 6865 2066  he data of the f
-00003300: 7261 6d65 7320 7769 7468 2061 6e20 696e  rames with an in
-00003310: 7465 6e73 6974 7920 6269 6767 6572 2074  tensity bigger t
-00003320: 6861 6e20 6120 7468 7265 7368 6f6c 642e  han a threshold.
-00003330: 0a20 2020 2020 2020 2054 6865 2074 6872  .        The thr
-00003340: 6573 686f 6c64 2069 7320 7365 7420 746f  eshold is set to
-00003350: 2062 6520 7468 6520 7365 636f 6e64 2062   be the second b
-00003360: 696e 206f 6620 7468 6520 6869 7374 6f67  in of the histog
-00003370: 7261 6d2e 0a0a 2020 2020 2020 2020 3a70  ram...        :p
-00003380: 6172 616d 2069 6e74 206e 756d 5f62 696e  aram int num_bin
-00003390: 733a 204e 756d 6265 7220 6f66 2062 696e  s: Number of bin
-000033a0: 7320 746f 2075 7365 2061 7320 7468 7265  s to use as thre
-000033b0: 7368 6f6c 642e 0a20 2020 2020 2020 2022  shold..        "
-000033c0: 2222 0a20 2020 2020 2020 2066 7261 6d65  "".        frame
-000033d0: 735f 696e 7465 6e73 6974 7920 3d20 280a  s_intensity = (.
-000033e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000033f0: 2e5f 6672 616d 6573 5f69 6e74 656e 7369  ._frames_intensi
-00003400: 7479 0a20 2020 2020 2020 2020 2020 2069  ty.            i
-00003410: 6620 7365 6c66 2e5f 6672 616d 6573 5f69  f self._frames_i
-00003420: 6e74 656e 7369 7479 0a20 2020 2020 2020  ntensity.       
-00003430: 2020 2020 2065 6c73 6520 7365 6c66 2e63       else self.c
-00003440: 6f6d 7075 7465 5f66 7261 6d65 735f 696e  ompute_frames_in
-00003450: 7465 6e73 6974 7928 290a 2020 2020 2020  tensity().      
-00003460: 2020 290a 2020 2020 2020 2020 6966 2066    ).        if f
-00003470: 7261 6d65 735f 696e 7465 6e73 6974 7920  rames_intensity 
-00003480: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00003490: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000034a0: 2020 2020 7661 6c75 6573 2c20 6269 6e73      values, bins
-000034b0: 203d 206e 756d 7079 2e68 6973 746f 6772   = numpy.histogr
-000034c0: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-000034d0: 6672 616d 6573 5f69 6e74 656e 7369 7479  frames_intensity
-000034e0: 2c20 7365 6c66 2e6e 6672 616d 6573 2069  , self.nframes i
-000034f0: 6620 6269 6e73 2069 7320 4e6f 6e65 2065  f bins is None e
-00003500: 6c73 6520 6269 6e73 0a20 2020 2020 2020  lse bins.       
-00003510: 2029 0a20 2020 2020 2020 2066 7261 6d65   ).        frame
-00003520: 735f 696e 7465 6e73 6974 7920 3d20 6e75  s_intensity = nu
-00003530: 6d70 792e 6173 616e 7961 7272 6179 2866  mpy.asanyarray(f
-00003540: 7261 6d65 735f 696e 7465 6e73 6974 7929  rames_intensity)
-00003550: 0a20 2020 2020 2020 2069 6620 746f 705f  .        if top_
-00003560: 6269 6e20 6973 204e 6f6e 653a 0a20 2020  bin is None:.   
-00003570: 2020 2020 2020 2020 2074 6f70 5f62 696e           top_bin
-00003580: 203d 206c 656e 2862 696e 7329 202d 2031   = len(bins) - 1
-00003590: 0a20 2020 2020 2020 2069 6620 626f 7474  .        if bott
-000035a0: 6f6d 5f62 696e 2069 7320 4e6f 6e65 3a0a  om_bin is None:.
-000035b0: 2020 2020 2020 2020 2020 2020 626f 7474              bott
-000035c0: 6f6d 5f62 696e 203d 2030 0a0a 2020 2020  om_bin = 0..    
-000035d0: 2020 2020 626f 7474 6f6d 5f74 6872 6573      bottom_thres
-000035e0: 686f 6c64 203d 2066 7261 6d65 735f 696e  hold = frames_in
-000035f0: 7465 6e73 6974 7920 3e3d 2062 696e 735b  tensity >= bins[
-00003600: 626f 7474 6f6d 5f62 696e 5d0a 2020 2020  bottom_bin].    
-00003610: 2020 2020 746f 705f 7468 7265 7368 6f6c      top_threshol
-00003620: 6420 3d20 6672 616d 6573 5f69 6e74 656e  d = frames_inten
-00003630: 7369 7479 203c 3d20 6269 6e73 5b74 6f70  sity <= bins[top
-00003640: 5f62 696e 5d0a 2020 2020 2020 2020 7468  _bin].        th
-00003650: 7265 7368 6f6c 6420 3d20 6e75 6d70 792e  reshold = numpy.
-00003660: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
-00003670: 2020 205b 6120 616e 6420 6220 666f 7220     [a and b for 
-00003680: 612c 2062 2069 6e20 7a69 7028 626f 7474  a, b in zip(bott
-00003690: 6f6d 5f74 6872 6573 686f 6c64 2c20 746f  om_threshold, to
-000036a0: 705f 7468 7265 7368 6f6c 6429 5d0a 2020  p_threshold)].  
-000036b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000036c0: 7265 7475 726e 206e 756d 7079 2e66 6c61  return numpy.fla
-000036d0: 746e 6f6e 7a65 726f 2874 6872 6573 686f  tnonzero(thresho
-000036e0: 6c64 292c 206e 756d 7079 2e66 6c61 746e  ld), numpy.flatn
-000036f0: 6f6e 7a65 726f 287e 7468 7265 7368 6f6c  onzero(~threshol
-00003700: 6429 0a0a 2020 2020 4070 726f 7065 7274  d)..    @propert
-00003710: 790a 2020 2020 6465 6620 696e 5f6d 656d  y.    def in_mem
-00003720: 6f72 7928 7365 6c66 293a 0a20 2020 2020  ory(self):.     
-00003730: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00003740: 696e 5f6d 656d 6f72 790a 0a20 2020 2040  in_memory..    @
-00003750: 696e 5f6d 656d 6f72 792e 7365 7474 6572  in_memory.setter
-00003760: 0a20 2020 2064 6566 2069 6e5f 6d65 6d6f  .    def in_memo
-00003770: 7279 2873 656c 662c 2069 6e5f 6d65 6d6f  ry(self, in_memo
-00003780: 7279 293a 0a20 2020 2020 2020 2022 2222  ry):.        """
-00003790: 0a20 2020 2020 2020 2052 656d 6f76 6573  .        Removes
-000037a0: 2064 6174 6120 6672 6f6d 206d 656d 6f72   data from memor
-000037b0: 7920 616e 6420 7365 7473 2074 6861 7420  y and sets that 
-000037c0: 6672 6f6d 206e 6f77 206f 6e20 6461 7461  from now on data
-000037d0: 2077 696c 6c20 6265 2072 6561 6420 6672   will be read fr
-000037e0: 6f6d 2064 6973 6b2e 0a20 2020 2020 2020  om disk..       
-000037f0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00003800: 7365 6c66 2e5f 696e 5f6d 656d 6f72 7920  self._in_memory 
-00003810: 6973 206e 6f74 2069 6e5f 6d65 6d6f 7279  is not in_memory
-00003820: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00003830: 6c66 2e5f 696e 5f6d 656d 6f72 7920 3d20  lf._in_memory = 
-00003840: 696e 5f6d 656d 6f72 790a 2020 2020 2020  in_memory.      
-00003850: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
-00003860: 203d 2044 6174 6128 7365 6c66 2e64 6174   = Data(self.dat
-00003870: 612e 7572 6c73 2c20 7365 6c66 2e64 6174  a.urls, self.dat
-00003880: 612e 6d65 7461 6461 7461 2c20 7365 6c66  a.metadata, self
-00003890: 2e5f 696e 5f6d 656d 6f72 7929 0a0a 2020  ._in_memory)..  
-000038a0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-000038b0: 6465 6620 6461 7461 2873 656c 6629 3a0a  def data(self):.
-000038c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000038d0: 656c 662e 5f64 6174 610a 0a20 2020 2064  elf._data..    d
-000038e0: 6566 2067 6574 5f64 6174 6128 7365 6c66  ef get_data(self
-000038f0: 2c20 696e 6469 6365 733d 4e6f 6e65 2c20  , indices=None, 
-00003900: 6469 6d65 6e73 696f 6e3d 4e6f 6e65 2c20  dimension=None, 
-00003910: 7265 7475 726e 5f69 6e64 6963 6573 3d46  return_indices=F
-00003920: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
-00003930: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00003940: 6e73 2074 6865 2064 6174 6120 636f 7272  ns the data corr
-00003950: 6573 706f 6e64 696e 6720 746f 2063 6572  esponding to cer
-00003960: 7461 696e 7320 696e 6469 6365 7320 616e  tains indices an
-00003970: 6420 6769 7665 6e20 736f 6d65 2064 696d  d given some dim
-00003980: 656e 7369 6f6e 7320 7661 6c75 6573 2e0a  ensions values..
-00003990: 2020 2020 2020 2020 5468 6520 6461 7461          The data
-000039a0: 2069 7320 616c 7761 7973 2066 6c61 7474   is always flatt
-000039b0: 656e 6564 2074 6f20 6265 2061 2073 7461  ened to be a sta
-000039c0: 636b 206f 6620 696d 6167 6573 2e0a 0a20  ck of images... 
-000039d0: 2020 2020 2020 203a 7061 7261 6d20 6172         :param ar
-000039e0: 7261 795f 6c69 6b65 2069 6e64 6963 6573  ray_like indices
-000039f0: 3a20 4966 206e 6f74 204e 6f6e 652c 2064  : If not None, d
-00003a00: 6174 6120 6973 2066 696c 7465 7265 6420  ata is filtered 
-00003a10: 7573 696e 6720 7468 6973 2061 7272 6179  using this array
-00003a20: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00003a30: 2061 7272 6179 5f6c 696b 6520 6469 6d65   array_like dime
-00003a40: 6e73 696f 6e3a 2049 6620 6e6f 7420 4e6f  nsion: If not No
-00003a50: 6e65 2c20 7265 7475 726e 206f 6e6c 7920  ne, return only 
-00003a60: 7468 6520 6461 7461 2063 6f72 7265 7370  the data corresp
-00003a70: 6f6e 6469 6e67 2074 6f0a 2020 2020 2020  onding to.      
-00003a80: 2020 2020 2020 7468 6520 6769 7665 6e20        the given 
-00003a90: 6469 6d65 6e73 696f 6e2e 2044 696d 656e  dimension. Dimen
-00003aa0: 7369 6f6e 2069 7320 6120 3264 2076 6563  sion is a 2d vec
-00003ab0: 746f 722c 2077 6865 7265 2074 6865 2066  tor, where the f
-00003ac0: 6972 7374 2063 6f6d 706f 6e65 6e74 2069  irst component i
-00003ad0: 730a 2020 2020 2020 2020 2020 2020 6120  s.            a 
-00003ae0: 6c69 7374 206f 6620 7468 6520 6178 6973  list of the axis
-00003af0: 2061 6e64 2074 6865 2073 6563 6f6e 6420   and the second 
-00003b00: 6973 2061 206c 6973 7420 6f66 2074 6865  is a list of the
-00003b10: 2069 6e64 6963 6573 206f 6620 7468 6520   indices of the 
-00003b20: 7661 6c75 6573 2074 6f20 6578 7472 6163  values to extrac
-00003b30: 742e 0a20 2020 2020 2020 2020 2020 2054  t..            T
-00003b40: 6865 2064 696d 656e 7369 6f6e 2061 6e64  he dimension and
-00003b50: 2076 616c 7565 206c 6973 7420 6c65 6e67   value list leng
-00003b60: 7468 2063 616e 2062 6520 7570 2074 6f20  th can be up to 
-00003b70: 7468 6520 6e75 6d62 6572 206f 6620 6469  the number of di
-00003b80: 6d65 6e73 696f 6e73 202d 2031 2e0a 2020  mensions - 1..  
-00003b90: 2020 2020 2020 2020 2020 5468 6520 6361            The ca
-00003ba0: 6c6c 2067 6574 5f64 6174 6128 6469 6d65  ll get_data(dime
-00003bb0: 6e73 696f 6e3d 5b5b 312c 2032 5d2c 205b  nsion=[[1, 2], [
-00003bc0: 322c 2033 5d5d 2920 6973 2065 7175 6976  2, 3]]) is equiv
-00003bd0: 616c 656e 7420 746f 2064 6174 615b 3a2c  alent to data[:,
-00003be0: 2032 2c20 335d 2077 6865 6e20 6461 7461   2, 3] when data
-00003bf0: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
-00003c00: 696e 206d 656d 6f72 792e 0a20 2020 2020  in memory..     
-00003c10: 2020 2020 2020 2054 6865 2061 7869 7320         The axis 
-00003c20: 6f66 2074 6865 2064 696d 656e 7369 6f6e  of the dimension
-00003c30: 2069 7320 736f 2074 6861 7420 6c6f 7765   is so that lowe
-00003c40: 7220 7468 6520 6178 6973 2c20 6661 7374  r the axis, fast
-00003c50: 6573 7420 7468 6520 6469 6d65 6e73 696f  est the dimensio
-00003c60: 6e20 2868 6967 6865 7220 6368 616e 6769  n (higher changi
-00003c70: 6e67 0a20 2020 2020 2020 2020 2020 2076  ng.            v
-00003c80: 616c 7565 292e 0a0a 2020 2020 2020 2020  alue)...        
-00003c90: 3a72 6574 7572 6e3a 2041 7272 6179 2077  :return: Array w
-00003ca0: 6974 6820 7468 6520 6e65 7720 6461 7461  ith the new data
-00003cb0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00003cc0: 2020 2020 2020 6966 2064 696d 656e 7369        if dimensi
-00003cd0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2061  on is not None a
-00003ce0: 6e64 206c 656e 2873 656c 662e 5f64 6174  nd len(self._dat
-00003cf0: 612e 7368 6170 6529 203e 2033 3a0a 2020  a.shape) > 3:.  
-00003d00: 2020 2020 2020 2020 2020 2320 4d61 6b65            # Make
-00003d10: 2073 7572 6520 6469 6d65 6e73 696f 6e20   sure dimension 
-00003d20: 616e 6420 7661 6c75 6520 6172 6520 6c69  and value are li
-00003d30: 7374 730a 2020 2020 2020 2020 2020 2020  sts.            
-00003d40: 6966 2069 7369 6e73 7461 6e63 6528 6469  if isinstance(di
-00003d50: 6d65 6e73 696f 6e5b 305d 2c20 696e 7429  mension[0], int)
-00003d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003d70: 2020 6469 6d65 6e73 696f 6e5b 305d 203d    dimension[0] =
-00003d80: 205b 6469 6d65 6e73 696f 6e5b 305d 5d0a   [dimension[0]].
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 6469 6d65 6e73 696f 6e5b 315d 203d 205b  dimension[1] = [
-00003db0: 6469 6d65 6e73 696f 6e5b 315d 5d0a 2020  dimension[1]].  
-00003dc0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00003dd0: 2073 656c 662e 6461 7461 0a0a 2020 2020   self.data..    
-00003de0: 2020 2020 2020 2020 2320 496e 6974 206c          # Init l
-00003df0: 6973 7420 6f66 2062 6f6f 6c20 696e 6469  ist of bool indi
-00003e00: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
-00003e10: 626f 6f6c 5f69 6e64 6963 6573 203d 206e  bool_indices = n
-00003e20: 756d 7079 2e7a 6572 6f73 2873 656c 662e  umpy.zeros(self.
-00003e30: 6461 7461 2e6e 6672 616d 6573 2c20 6474  data.nframes, dt
-00003e40: 7970 653d 626f 6f6c 290a 2020 2020 2020  ype=bool).      
-00003e50: 2020 2020 2020 6966 2069 6e64 6963 6573        if indices
-00003e60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00003e70: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00003e80: 7320 3d20 6e75 6d70 792e 6172 616e 6765  s = numpy.arange
-00003e90: 2873 656c 662e 6e66 7261 6d65 7329 0a20  (self.nframes). 
-00003ea0: 2020 2020 2020 2020 2020 2062 6f6f 6c5f             bool_
-00003eb0: 696e 6469 6365 735b 696e 6469 6365 735d  indices[indices]
-00003ec0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00003ed0: 2020 2020 626f 6f6c 5f69 6e64 6963 6573      bool_indices
-00003ee0: 203d 2062 6f6f 6c5f 696e 6469 6365 732e   = bool_indices.
-00003ef0: 7265 7368 6170 6528 7365 6c66 2e64 6174  reshape(self.dat
-00003f00: 612e 7363 616e 5f73 6861 7065 290a 2020  a.scan_shape).  
-00003f10: 2020 2020 2020 2020 2020 696e 6478 203d            indx =
-00003f20: 206e 756d 7079 2e61 7261 6e67 6528 7365   numpy.arange(se
-00003f30: 6c66 2e6e 6672 616d 6573 292e 7265 7368  lf.nframes).resh
-00003f40: 6170 6528 7365 6c66 2e64 6174 612e 7363  ape(self.data.sc
-00003f50: 616e 5f73 6861 7065 290a 0a20 2020 2020  an_shape)..     
-00003f60: 2020 2020 2020 2023 2046 6f72 2065 7665         # For eve
-00003f70: 7279 2061 7869 732c 2067 6574 2063 6f72  ry axis, get cor
-00003f80: 7265 7370 6f6e 6469 6e67 2065 6c65 6d65  responding eleme
-00003f90: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00003fa0: 666f 7220 692c 2064 696d 2069 6e20 656e  for i, dim in en
-00003fb0: 756d 6572 6174 6528 736f 7274 6564 2864  umerate(sorted(d
-00003fc0: 696d 656e 7369 6f6e 5b30 5d29 293a 0a20  imension[0])):. 
-00003fd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003fe0: 2046 6c69 7020 6178 6973 2074 6f20 6265   Flip axis to be
-00003ff0: 2063 6f6e 7369 7374 656e 7420 7769 7468   consistent with
-00004000: 2074 6865 2064 6174 6120 7368 6170 650a   the data shape.
-00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004020: 6178 6973 203d 2073 656c 662e 6469 6d73  axis = self.dims
-00004030: 2e6e 6469 6d20 2d20 6469 6d20 2d20 310a  .ndim - dim - 1.
-00004040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004050: 6461 7461 203d 2064 6174 612e 7461 6b65  data = data.take
-00004060: 2869 6e64 6963 6573 3d64 696d 656e 7369  (indices=dimensi
-00004070: 6f6e 5b31 5d5b 695d 2c20 6178 6973 3d61  on[1][i], axis=a
-00004080: 7869 7329 0a20 2020 2020 2020 2020 2020  xis).           
-00004090: 2020 2020 2062 6f6f 6c5f 696e 6469 6365       bool_indice
-000040a0: 7320 3d20 626f 6f6c 5f69 6e64 6963 6573  s = bool_indices
-000040b0: 2e74 616b 6528 696e 6469 6365 733d 6469  .take(indices=di
-000040c0: 6d65 6e73 696f 6e5b 315d 5b69 5d2c 2061  mension[1][i], a
-000040d0: 7869 733d 6178 6973 290a 2020 2020 2020  xis=axis).      
-000040e0: 2020 2020 2020 2020 2020 696e 6478 203d            indx =
-000040f0: 2069 6e64 782e 7461 6b65 2869 6e64 6963   indx.take(indic
-00004100: 6573 3d64 696d 656e 7369 6f6e 5b31 5d5b  es=dimension[1][
-00004110: 695d 2c20 6178 6973 3d61 7869 7329 0a0a  i], axis=axis)..
-00004120: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004130: 203d 2064 6174 615b 626f 6f6c 5f69 6e64   = data[bool_ind
-00004140: 6963 6573 5d0a 2020 2020 2020 2020 2020  ices].          
-00004150: 2020 696e 6478 203d 2069 6e64 785b 626f    indx = indx[bo
-00004160: 6f6c 5f69 6e64 6963 6573 5d0a 2020 2020  ol_indices].    
-00004170: 2020 2020 2020 2020 6966 2072 6574 7572          if retur
-00004180: 6e5f 696e 6469 6365 733a 0a20 2020 2020  n_indices:.     
-00004190: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000041a0: 6e20 6461 7461 2e66 6c61 7474 656e 2829  n data.flatten()
-000041b0: 2c20 696e 6478 2e66 6c61 7474 656e 2829  , indx.flatten()
-000041c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000041d0: 7572 6e20 6461 7461 2e66 6c61 7474 656e  urn data.flatten
-000041e0: 2829 0a0a 2020 2020 2020 2020 6461 7461  ()..        data
-000041f0: 203d 2073 656c 662e 6461 7461 2e66 6c61   = self.data.fla
-00004200: 7474 656e 2829 0a20 2020 2020 2020 2069  tten().        i
-00004210: 6620 7265 7475 726e 5f69 6e64 6963 6573  f return_indices
-00004220: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00004230: 2069 6e64 6963 6573 2069 7320 4e6f 6e65   indices is None
-00004240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004250: 2020 696e 6469 6365 7320 3d20 6e75 6d70    indices = nump
-00004260: 792e 6172 616e 6765 2873 656c 662e 6e66  y.arange(self.nf
-00004270: 7261 6d65 7329 0a20 2020 2020 2020 2020  rames).         
-00004280: 2020 2072 6574 7572 6e20 6461 7461 5b69     return data[i
-00004290: 6e64 6963 6573 5d2c 2069 6e64 6963 6573  ndices], indices
-000042a0: 0a20 2020 2020 2020 2069 6620 696e 6469  .        if indi
-000042b0: 6365 7320 6973 204e 6f6e 653a 0a20 2020  ces is None:.   
-000042c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000042d0: 6461 7461 0a20 2020 2020 2020 2072 6574  data.        ret
-000042e0: 7572 6e20 6461 7461 5b69 6e64 6963 6573  urn data[indices
-000042f0: 5d0a 0a20 2020 2040 7072 6f70 6572 7479  ]..    @property
-00004300: 0a20 2020 2064 6566 206e 6672 616d 6573  .    def nframes
-00004310: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004320: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-00004330: 726e 206e 756d 6265 7220 6f66 2066 7261  rn number of fra
-00004340: 6d65 730a 2020 2020 2020 2020 2222 220a  mes.        """.
-00004350: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004360: 6461 7461 2069 7320 4e6f 6e65 3a0a 2020  data is None:.  
-00004370: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004380: 2030 0a20 2020 2020 2020 2072 6574 7572   0.        retur
-00004390: 6e20 7365 6c66 2e64 6174 612e 6e66 7261  n self.data.nfra
-000043a0: 6d65 730a 0a20 2020 2064 6566 2074 6f5f  mes..    def to_
-000043b0: 6d65 6d6f 7279 2873 656c 662c 2069 6e64  memory(self, ind
-000043c0: 6963 6573 293a 0a20 2020 2020 2020 2022  ices):.        "
-000043d0: 2222 0a20 2020 2020 2020 204d 6574 686f  "".        Metho
-000043e0: 6420 746f 206c 6f61 6420 6f6e 6c79 2070  d to load only p
-000043f0: 6172 7420 6f66 2074 6865 2064 6174 6120  art of the data 
-00004400: 696e 746f 206d 656d 6f72 792e 0a20 2020  into memory..   
-00004410: 2020 2020 2052 6574 7572 6e73 2061 206e       Returns a n
-00004420: 6577 2064 6174 6173 6574 2077 6974 6820  ew dataset with 
-00004430: 7468 6520 6461 7461 2063 6f72 7265 7370  the data corresp
-00004440: 6f6e 6469 6e67 2074 6f20 6769 7665 6e20  onding to given 
-00004450: 696e 6469 6365 7320 696e 746f 206d 656d  indices into mem
-00004460: 6f72 792e 0a20 2020 2020 2020 2054 6865  ory..        The
-00004470: 206e 6577 2069 6e64 6963 6573 2061 7272   new indices arr
-00004480: 6179 2068 6173 2074 6f20 6265 2067 6976  ay has to be giv
-00004490: 656e 2c20 6966 2061 6c6c 2074 6865 2064  en, if all the d
-000044a0: 6174 6120 6861 7320 746f 2062 6520 7365  ata has to be se
-000044b0: 7420 696e 746f 0a20 2020 2020 2020 206d  t into.        m
-000044c0: 656d 6f72 7920 706c 6561 7365 2073 6574  emory please set
-000044d0: 2060 696e 5f6d 656d 6f72 7960 2074 6f20   `in_memory` to 
-000044e0: 5472 7565 2069 6e73 7465 6164 2c20 7468  True instead, th
-000044f0: 6973 2077 6179 206e 6f20 6e65 7720 6461  is way no new da
-00004500: 7461 7365 7420 7769 6c6c 2062 650a 2020  taset will be.  
-00004510: 2020 2020 2020 6372 6561 7465 642e 0a0a        created...
-00004520: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-00004530: 7272 6179 5f6c 696b 6520 696e 6469 6365  rray_like indice
-00004540: 733a 2049 6e64 6963 6573 206f 6620 7468  s: Indices of th
-00004550: 6520 6e65 7720 6461 7461 7365 742e 0a20  e new dataset.. 
-00004560: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004570: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00004580: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
-00004590: 2020 2020 2020 2064 6174 6120 3d20 7365         data = se
-000045a0: 6c66 2e67 6574 5f64 6174 6128 696e 6469  lf.get_data(indi
-000045b0: 6365 7329 0a20 2020 2020 2020 2020 2020  ces).           
-000045c0: 206e 6577 5f64 6174 6120 3d20 4461 7461   new_data = Data
-000045d0: 2864 6174 612e 7572 6c73 2c20 6461 7461  (data.urls, data
-000045e0: 2e6d 6574 6164 6174 612c 2054 7275 6529  .metadata, True)
-000045f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00004600: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
-00004610: 6174 6120 3d20 7365 6c66 2e67 6574 5f64  ata = self.get_d
-00004620: 6174 6128 696e 6469 6365 7329 0a20 2020  ata(indices).   
-00004630: 2020 2020 2072 6574 7572 6e20 4461 7461       return Data
-00004640: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
-00004650: 205f 6469 723d 7365 6c66 2e5f 6469 722c   _dir=self._dir,
-00004660: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00004670: 613d 6e65 775f 6461 7461 2c0a 2020 2020  a=new_data,.    
-00004680: 2020 2020 2020 2020 6469 6d73 3d73 656c          dims=sel
-00004690: 662e 5f5f 6469 6d73 2c0a 2020 2020 2020  f.__dims,.      
-000046a0: 2020 2020 2020 696e 5f6d 656d 6f72 793d        in_memory=
-000046b0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-000046c0: 2020 7469 746c 653d 7365 6c66 2e74 6974    title=self.tit
-000046d0: 6c65 2c0a 2020 2020 2020 2020 290a 0a20  le,.        ).. 
-000046e0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000046f0: 2064 6566 2064 696d 7328 7365 6c66 293a   def dims(self):
-00004700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004710: 7365 6c66 2e5f 5f64 696d 730a 0a20 2020  self.__dims..   
-00004720: 2040 6469 6d73 2e73 6574 7465 720a 2020   @dims.setter.  
-00004730: 2020 6465 6620 6469 6d73 2873 656c 662c    def dims(self,
-00004740: 205f 6469 6d73 293a 0a20 2020 2020 2020   _dims):.       
-00004750: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00004760: 6365 285f 6469 6d73 2c20 4163 7175 6973  ce(_dims, Acquis
-00004770: 6974 696f 6e44 696d 7329 2c20 280a 2020  itionDims), (.  
-00004780: 2020 2020 2020 2020 2020 2244 696d 656e            "Dimen
-00004790: 7369 6f6e 7320 6469 6374 696f 6e61 7279  sions dictionary
-000047a0: 2068 6173 2022 2022 746f 2062 6520 6f66   has " "to be of
-000047b0: 2063 6c61 7373 2060 4163 7175 6973 6974   class `Acquisit
-000047c0: 696f 6e44 696d 7360 220a 2020 2020 2020  ionDims`".      
-000047d0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-000047e0: 2e5f 5f64 696d 7320 3d20 5f64 696d 730a  .__dims = _dims.
-000047f0: 0a20 2020 2064 6566 2063 6c65 6172 5f64  .    def clear_d
-00004800: 696d 7328 7365 6c66 293a 0a20 2020 2020  ims(self):.     
-00004810: 2020 2073 656c 662e 5f5f 6469 6d73 203d     self.__dims =
-00004820: 2041 6371 7569 7369 7469 6f6e 4469 6d73   AcquisitionDims
-00004830: 2829 0a0a 2020 2020 6465 6620 6164 645f  ()..    def add_
-00004840: 6469 6d28 7365 6c66 2c20 6178 6973 2c20  dim(self, axis, 
-00004850: 6469 6d29 3a0a 2020 2020 2020 2020 2222  dim):.        ""
-00004860: 220a 2020 2020 2020 2020 4164 6473 2061  ".        Adds a
-00004870: 2064 696d 656e 7369 6f6e 2074 6f20 7468   dimension to th
-00004880: 6520 6469 6d65 6e73 696f 6e27 7320 6469  e dimension's di
-00004890: 6374 696f 6e61 7279 2e0a 0a20 2020 2020  ctionary...     
-000048a0: 2020 203a 7061 7261 6d20 696e 7420 6178     :param int ax
-000048b0: 6973 3a20 6178 6973 206f 6620 7468 6520  is: axis of the 
-000048c0: 6469 6d65 6e73 696f 6e2e 0a20 2020 2020  dimension..     
-000048d0: 2020 203a 7061 7261 6d20 6044 696d 656e     :param `Dimen
-000048e0: 7369 6f6e 6020 6469 6d3a 2064 696d 656e  sion` dim: dimen
-000048f0: 7369 6f6e 2074 6f20 6265 2061 6464 6564  sion to be added
-00004900: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00004910: 2020 2020 2020 7365 6c66 2e5f 5f64 696d        self.__dim
-00004920: 732e 6164 645f 6469 6d28 6178 6973 2c20  s.add_dim(axis, 
-00004930: 6469 6d29 0a0a 2020 2020 6465 6620 7265  dim)..    def re
-00004940: 6d6f 7665 5f64 696d 2873 656c 662c 2061  move_dim(self, a
-00004950: 7869 7329 3a0a 2020 2020 2020 2020 2222  xis):.        ""
-00004960: 220a 2020 2020 2020 2020 5265 6d6f 7665  ".        Remove
-00004970: 7320 6120 6469 6d65 6e73 696f 6e20 6672  s a dimension fr
-00004980: 6f6d 2074 6865 2064 696d 656e 7369 6f6e  om the dimension
-00004990: 2773 2064 6963 7469 6f6e 6172 792e 0a0a  's dictionary...
-000049a0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-000049b0: 6e74 2061 7869 733a 2061 7869 7320 6f66  nt axis: axis of
-000049c0: 2074 6865 2064 696d 656e 7369 6f6e 2e0a   the dimension..
-000049d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000049e0: 2020 2020 7365 6c66 2e5f 5f64 696d 732e      self.__dims.
-000049f0: 7265 6d6f 7665 5f64 696d 2861 7869 7329  remove_dim(axis)
-00004a00: 0a0a 2020 2020 6465 6620 7a73 756d 2873  ..    def zsum(s
-00004a10: 656c 662c 2069 6e64 6963 6573 3d4e 6f6e  elf, indices=Non
-00004a20: 652c 2064 696d 656e 7369 6f6e 3d4e 6f6e  e, dimension=Non
-00004a30: 6529 3a0a 2020 2020 2020 2020 6461 7461  e):.        data
-00004a40: 203d 2073 656c 662e 6765 745f 6461 7461   = self.get_data
-00004a50: 2869 6e64 6963 6573 2c20 6469 6d65 6e73  (indices, dimens
-00004a60: 696f 6e29 0a20 2020 2020 2020 2072 6574  ion).        ret
-00004a70: 7572 6e20 6461 7461 2e73 756d 2861 7869  urn data.sum(axi
-00004a80: 733d 3029 0a0a 2020 2020 6465 6620 7265  s=0)..    def re
-00004a90: 7368 6170 655f 6461 7461 2873 656c 6629  shape_data(self)
-00004aa0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00004ab0: 2020 2020 2020 4675 6e63 7469 6f6e 2074        Function t
-00004ac0: 6861 7420 7265 7368 6170 6573 2074 6865  hat reshapes the
-00004ad0: 2064 6174 6120 746f 2066 6974 2074 6865   data to fit the
-00004ae0: 2064 696d 656e 7369 6f6e 732e 0a20 2020   dimensions..   
-00004af0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004b00: 2069 6620 7365 6c66 2e5f 5f64 696d 732e   if self.__dims.
-00004b10: 6e64 696d 203d 3d20 3120 616e 6420 7365  ndim == 1 and se
-00004b20: 6c66 2e5f 5f64 696d 732e 6765 7428 3029  lf.__dims.get(0)
-00004b30: 2e73 697a 6520 3d3d 2073 656c 662e 6e66  .size == self.nf
-00004b40: 7261 6d65 733a 0a20 2020 2020 2020 2020  rames:.         
-00004b50: 2020 2072 6574 7572 6e20 7365 6c66 0a20     return self. 
-00004b60: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00004b70: 2e5f 5f64 696d 732e 6e64 696d 203e 2031  .__dims.ndim > 1
-00004b80: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00004b90: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00004ba0: 2020 2073 6861 7065 203d 206c 6973 7428     shape = list(
-00004bb0: 7365 6c66 2e5f 5f64 696d 732e 7368 6170  self.__dims.shap
-00004bc0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00004bd0: 2020 2073 6861 7065 2e61 7070 656e 6428     shape.append(
-00004be0: 7365 6c66 2e67 6574 5f64 6174 6128 292e  self.get_data().
-00004bf0: 7368 6170 655b 2d32 5d29 0a20 2020 2020  shape[-2]).     
-00004c00: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00004c10: 2e61 7070 656e 6428 7365 6c66 2e67 6574  .append(self.get
-00004c20: 5f64 6174 6128 292e 7368 6170 655b 2d31  _data().shape[-1
-00004c30: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00004c40: 2020 2064 6174 6120 3d20 7365 6c66 2e67     data = self.g
-00004c50: 6574 5f64 6174 6128 292e 7265 7368 6170  et_data().reshap
-00004c60: 6528 7368 6170 6529 0a20 2020 2020 2020  e(shape).       
-00004c70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00004c80: 4461 7461 7365 7428 0a20 2020 2020 2020  Dataset(.       
-00004c90: 2020 2020 2020 2020 2020 2020 205f 6469               _di
-00004ca0: 723d 7365 6c66 2e64 6972 2c0a 2020 2020  r=self.dir,.    
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 6461 7461 3d64 6174 612c 0a20 2020 2020  data=data,.     
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004ce0: 696d 733d 7365 6c66 2e5f 5f64 696d 732c  ims=self.__dims,
-00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 2020 2020 2069 6e5f 6d65 6d6f 7279 3d73       in_memory=s
-00004d10: 656c 662e 5f69 6e5f 6d65 6d6f 7279 2c0a  elf._in_memory,.
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d30: 2020 2020 7469 746c 653d 7365 6c66 2e74      title=self.t
-00004d40: 6974 6c65 2c0a 2020 2020 2020 2020 2020  itle,.          
-00004d50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004d60: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00004d70: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00004d80: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00004d90: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00004da0: 2020 2020 2020 2020 2020 2020 2246 6169              "Fai
-00004db0: 6c65 6420 746f 2072 6573 6861 7065 2064  led to reshape d
-00004dc0: 6174 6120 696e 746f 2064 696d 656e 7369  ata into dimensi
-00004dd0: 6f6e 7320 7b7d 205c 0a20 2020 2020 2020  ons {} \.       
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 2020 2054 7279 2075             Try u
-00004e00: 7369 6e67 2061 6e6f 7468 6572 2074 6f6c  sing another tol
-00004e10: 6572 616e 6365 206f 7220 7369 7a65 2076  erance or size v
-00004e20: 616c 7565 732e 222e 666f 726d 6174 280a  alues.".format(.
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 2020 2020 2220 222e 6a6f 696e          " ".join
-00004e50: 2873 656c 662e 5f5f 6469 6d73 2e67 6574  (self.__dims.get
-00004e60: 5f6e 616d 6573 2829 290a 2020 2020 2020  _names()).      
-00004e70: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00004ea0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004eb0: 6520 5661 6c75 6545 7272 6f72 2822 4e6f  e ValueError("No
-00004ec0: 7420 656e 6f75 6768 2064 696d 656e 7369  t enough dimensi
-00004ed0: 6f6e 7320 7768 6572 6520 666f 756e 6422  ons where found"
-00004ee0: 290a 0a20 2020 2064 6566 2066 696e 645f  )..    def find_
-00004ef0: 6469 6d65 6e73 696f 6e73 2873 656c 662c  dimensions(self,
-00004f00: 206b 696e 642c 2074 6f6c 6572 616e 6365   kind, tolerance
-00004f10: 3d31 652d 3929 202d 3e20 4e6f 6e65 3a0a  =1e-9) -> None:.
-00004f20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004f30: 2020 2020 476f 6573 206f 7665 7220 616c      Goes over al
-00004f40: 6c20 7468 6520 6865 6164 6572 7320 6672  l the headers fr
-00004f50: 6f6d 2061 2067 6976 656e 206b 696e 6420  om a given kind 
-00004f60: 616e 6420 6669 6e64 7320 7468 6520 6469  and finds the di
-00004f70: 6d65 6e73 696f 6e73 0a20 2020 2020 2020  mensions.       
-00004f80: 2074 6861 7420 6d6f 7665 2028 6861 7665   that move (have
-00004f90: 206d 6f72 6520 7468 616e 206f 6e65 2076   more than one v
-00004fa0: 616c 7565 2920 616c 6f6e 6720 7468 6520  alue) along the 
-00004fb0: 6461 7461 2e0a 0a20 2020 2020 2020 204e  data...        N
-00004fc0: 6f74 653a 2042 6566 6f72 652c 206f 6e6c  ote: Before, onl
-00004fd0: 7920 7468 6520 6469 6d65 6e73 696f 6e73  y the dimensions
-00004fe0: 2074 6861 7420 636f 756c 6420 6669 7420   that could fit 
-00004ff0: 7768 6572 6520 7368 6f77 6e2c 206e 6f77  where shown, now
-00005000: 2069 740a 2020 2020 2020 2020 7368 6f77   it.        show
-00005010: 7320 616c 6c20 7468 6520 6469 6d65 6e73  s all the dimens
-00005020: 696f 6e73 2061 6e64 206c 6574 2074 6865  ions and let the
-00005030: 2075 7365 7220 6368 6f6f 7365 2074 6865   user choose the
-00005040: 2076 616c 6964 206f 6e65 732e 0a0a 2020   valid ones...  
-00005050: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
-00005060: 206b 696e 643a 2054 7970 6520 6f66 206d   kind: Type of m
-00005070: 6574 6164 6174 6120 746f 2066 696e 6420  etadata to find 
-00005080: 7468 6520 6469 6d65 6e73 696f 6e73 2e0a  the dimensions..
-00005090: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-000050a0: 6c6f 6174 2074 6f6c 6572 616e 6365 3a20  loat tolerance: 
-000050b0: 546f 6c65 7261 6e63 6520 7468 6174 2077  Tolerance that w
-000050c0: 696c 6c20 6265 2075 7365 6420 746f 2063  ill be used to c
-000050d0: 6f6d 7075 7465 2074 6865 0a20 2020 2020  ompute the.     
-000050e0: 2020 2020 2020 2075 6e69 7175 6520 7661         unique va
-000050f0: 6c75 6573 2e0a 2020 2020 2020 2020 2222  lues..        ""
-00005100: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
-00005110: 5f64 696d 732e 636c 6561 7228 290a 2020  _dims.clear().  
-00005120: 2020 2020 2020 7365 6c66 2e5f 6469 6d65        self._dime
-00005130: 6e73 696f 6e73 5f76 616c 7565 7320 3d20  nsions_values = 
-00005140: 7b7d 0a0a 2020 2020 2020 2020 6b65 7973  {}..        keys
-00005150: 203d 206e 756d 7079 2e61 7272 6179 286c   = numpy.array(l
-00005160: 6973 7428 7365 6c66 2e64 6174 612e 6d65  ist(self.data.me
-00005170: 7461 6461 7461 5b30 5d2e 6765 745f 6b65  tadata[0].get_ke
-00005180: 7973 286b 696e 6429 2929 0a20 2020 2020  ys(kind))).     
-00005190: 2020 2076 616c 7565 7320 3d20 6e75 6d70     values = nump
-000051a0: 792e 6173 6172 7261 7928 0a20 2020 2020  y.asarray(.     
-000051b0: 2020 2020 2020 205b 7365 6c66 2e67 6574         [self.get
-000051c0: 5f6d 6574 6164 6174 615f 7661 6c75 6573  _metadata_values
-000051d0: 286b 696e 643d 6b69 6e64 2c20 6b65 793d  (kind=kind, key=
-000051e0: 6b65 7929 2066 6f72 206b 6579 2069 6e20  key) for key in 
-000051f0: 6b65 7973 5d0a 2020 2020 2020 2020 290a  keys].        ).
-00005200: 2020 2020 2020 2020 2320 556e 6971 7565          # Unique
-00005210: 2076 616c 7565 7320 666f 7220 6561 6368   values for each
-00005220: 206b 6579 2e0a 2020 2020 2020 2020 756e   key..        un
-00005230: 6971 7565 5f76 616c 7565 7320 3d20 5b0a  ique_values = [.
-00005240: 2020 2020 2020 2020 2020 2020 6e75 6d70              nump
-00005250: 792e 756e 6971 7565 2876 616c 7565 2c20  y.unique(value, 
-00005260: 7265 7475 726e 5f69 6e64 6578 3d54 7275  return_index=Tru
-00005270: 652c 2072 6574 7572 6e5f 636f 756e 7473  e, return_counts
-00005280: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00005290: 2020 2066 6f72 2076 616c 7565 2069 6e20     for value in 
-000052a0: 7661 6c75 6573 0a20 2020 2020 2020 205d  values.        ]
-000052b0: 0a20 2020 2020 2020 2064 696d 656e 7369  .        dimensi
-000052c0: 6f6e 7320 3d20 5b5d 0a20 2020 2020 2020  ons = [].       
-000052d0: 2064 6174 6173 6574 5f73 697a 6520 3d20   dataset_size = 
-000052e0: 6c65 6e28 7365 6c66 2e64 6174 612e 6d65  len(self.data.me
-000052f0: 7461 6461 7461 290a 2020 2020 2020 2020  tadata).        
-00005300: 2320 466f 7220 6576 6572 7920 6b65 7920  # For every key 
-00005310: 7468 6174 2068 6173 206d 6f72 6520 7468  that has more th
-00005320: 616e 206f 6e65 2064 6966 6665 7265 6e74  an one different
-00005330: 2076 616c 7565 2c20 6372 6561 7465 7320   value, creates 
-00005340: 6120 6e65 7720 4469 6d65 6e73 696f 6e2e  a new Dimension.
-00005350: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00005360: 7661 6c75 6520 696e 2065 6e75 6d65 7261  value in enumera
-00005370: 7465 2875 6e69 7175 655f 7661 6c75 6573  te(unique_values
-00005380: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00005390: 6620 7661 6c75 655b 325d 5b30 5d20 213d  f value[2][0] !=
-000053a0: 2064 6174 6173 6574 5f73 697a 653a 0a20   dataset_size:. 
-000053b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000053c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000053d0: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
-000053e0: 6e20 3d20 4469 6d65 6e73 696f 6e28 6b69  n = Dimension(ki
-000053f0: 6e64 2c20 6b65 7973 5b69 5d2c 2074 6f6c  nd, keys[i], tol
-00005400: 6572 616e 6365 3d74 6f6c 6572 616e 6365  erance=tolerance
-00005410: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005420: 2020 2020 2020 6469 6d65 6e73 696f 6e2e        dimension.
-00005430: 7365 745f 756e 6971 7565 5f76 616c 7565  set_unique_value
-00005440: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00005450: 2020 2020 2020 2020 2020 206e 756d 7079             numpy
-00005460: 2e61 7272 6179 2876 616c 7565 735b 695d  .array(values[i]
-00005470: 5b6e 756d 7079 2e73 6f72 7428 7661 6c75  [numpy.sort(valu
-00005480: 655b 315d 295d 2c20 6474 7970 653d 666c  e[1])], dtype=fl
-00005490: 6f61 7429 0a20 2020 2020 2020 2020 2020  oat).           
-000054a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000054c0: 2056 616c 7565 2074 6861 7420 7465 6c6c   Value that tell
-000054d0: 7320 7768 656e 2064 6f65 7320 7468 6520  s when does the 
-000054e0: 6368 616e 6765 206f 6620 7661 6c75 6520  change of value 
-000054f0: 6f63 6375 722e 2049 7420 6973 2075 7365  occur. It is use
-00005500: 6420 746f 206b 6e6f 7720 7468 6520 6f72  d to know the or
-00005510: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00005520: 2020 2020 2020 2020 2320 6f66 2074 6865          # of the
-00005530: 2072 6573 6861 7069 6e67 2e0a 2020 2020   reshaping..    
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 6469 6d65 6e73 696f 6e2e 6368 616e 6769  dimension.changi
-00005560: 6e67 5f76 616c 7565 203d 2073 656c 662e  ng_value = self.
-00005570: 5f5f 636f 6d70 7574 655f 6368 616e 6769  __compute_changi
-00005580: 6e67 5f76 616c 7565 2876 616c 7565 735b  ng_value(values[
-00005590: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-000055a0: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
-000055b0: 6e73 2e61 7070 656e 6428 6469 6d65 6e73  ns.append(dimens
-000055c0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-000055d0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-000055e0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-000055f0: 2020 2020 2020 2020 2020 2020 5f6c 6f67              _log
-00005600: 6765 722e 7761 726e 696e 6728 2243 6f75  ger.warning("Cou
-00005610: 6c64 6e27 7420 636f 6e76 6572 7420 746f  ldn't convert to
-00005620: 2066 6c6f 6174 2229 0a0a 2020 2020 2020   float")..      
-00005630: 2020 666f 7220 6469 6d65 6e73 696f 6e20    for dimension 
-00005640: 696e 2073 6f72 7465 6428 0a20 2020 2020  in sorted(.     
-00005650: 2020 2020 2020 2064 696d 656e 7369 6f6e         dimension
-00005660: 732c 206b 6579 3d6c 616d 6264 6120 783a  s, key=lambda x:
-00005670: 2078 2e63 6861 6e67 696e 675f 7661 6c75   x.changing_valu
-00005680: 652c 2072 6576 6572 7365 3d54 7275 650a  e, reverse=True.
-00005690: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000056a0: 2020 2020 2020 2073 656c 662e 5f5f 6469         self.__di
-000056b0: 6d73 2e61 6464 5f64 696d 2861 7869 733d  ms.add_dim(axis=
-000056c0: 7365 6c66 2e5f 5f64 696d 732e 6e64 696d  self.__dims.ndim
-000056d0: 2c20 6469 6d3d 6469 6d65 6e73 696f 6e29  , dim=dimension)
-000056e0: 0a20 2020 2020 2020 2020 2020 205f 6c6f  .            _lo
-000056f0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-00005700: 2020 2020 2020 2020 2020 2022 4469 6d65             "Dime
-00005710: 6e73 696f 6e20 7b7d 206f 6620 7369 7a65  nsion {} of size
-00005720: 207b 7d20 6861 7320 6265 656e 2061 6464   {} has been add
-00005730: 6564 2066 6f72 2072 6573 6861 7069 6e67  ed for reshaping
-00005740: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00005750: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00005760: 6d65 6e73 696f 6e2e 6e61 6d65 2c20 6469  mension.name, di
-00005770: 6d65 6e73 696f 6e2e 7369 7a65 0a20 2020  mension.size.   
-00005780: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00005790: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000057a0: 2020 6465 6620 6765 745f 6d65 7461 6461    def get_metada
-000057b0: 7461 5f76 616c 7565 7328 0a20 2020 2020  ta_values(.     
-000057c0: 2020 2073 656c 662c 206b 696e 642c 206b     self, kind, k
-000057d0: 6579 2c20 696e 6469 6365 733d 4e6f 6e65  ey, indices=None
-000057e0: 2c20 6469 6d65 6e73 696f 6e3d 4e6f 6e65  , dimension=None
-000057f0: 0a20 2020 2029 202d 3e20 6e75 6d70 792e  .    ) -> numpy.
-00005800: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
-00005810: 2076 616c 7565 7320 3d20 5b5d 0a20 2020   values = [].   
-00005820: 2020 2020 206d 6973 7369 6e67 5f76 616c       missing_val
-00005830: 7565 203d 2046 616c 7365 0a20 2020 2020  ue = False.     
-00005840: 2020 2066 6f72 2064 6174 6120 696e 2073     for data in s
-00005850: 656c 662e 6765 745f 6461 7461 2869 6e64  elf.get_data(ind
-00005860: 6963 6573 2c20 6469 6d65 6e73 696f 6e29  ices, dimension)
-00005870: 2e6d 6574 6164 6174 613a 0a20 2020 2020  .metadata:.     
-00005880: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00005890: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-000058a0: 6520 3d20 6461 7461 2e67 6574 5f76 616c  e = data.get_val
-000058b0: 7565 286b 696e 643d 6b69 6e64 2c20 6e61  ue(kind=kind, na
-000058c0: 6d65 3d6b 6579 290a 2020 2020 2020 2020  me=key).        
-000058d0: 2020 2020 6578 6365 7074 204b 6579 4572      except KeyEr
-000058e0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-000058f0: 2020 2020 206d 6973 7369 6e67 5f76 616c       missing_val
-00005900: 7565 203d 2054 7275 650a 2020 2020 2020  ue = True.      
-00005910: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00005920: 2876 616c 7565 7329 3a0a 2020 2020 2020  (values):.      
-00005930: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00005940: 6c75 6573 2e61 7070 656e 6428 7661 6c75  lues.append(valu
-00005950: 6573 5b2d 315d 290a 2020 2020 2020 2020  es[-1]).        
-00005960: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 2020 7661 6c75 6573 2e61 7070 656e 6428    values.append(
-00005990: 6e75 6d70 792e 6e61 6e29 0a20 2020 2020  numpy.nan).     
-000059a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000059b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000059c0: 6e6f 7420 6973 696e 7374 616e 6365 2864  not isinstance(d
-000059d0: 6174 612c 205f 4844 4635 4d65 7461 6461  ata, _HDF5Metada
-000059e0: 7461 5265 6164 6572 293a 0a20 2020 2020  taReader):.     
-000059f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005a00: 205f 4844 4635 4d65 7461 6461 7461 5265   _HDF5MetadataRe
-00005a10: 6164 6572 2061 6c72 6561 6479 2072 6574  ader already ret
-00005a20: 7572 6e20 6120 7363 616c 6172 2077 6865  urn a scalar whe
-00005a30: 6e20 7369 6c78 2046 6162 696f 5265 6164  n silx FabioRead
-00005a40: 6572 2072 6574 7572 6e20 616e 2061 7272  er return an arr
-00005a50: 6179 206f 6620 6120 7369 6e67 6c65 2065  ay of a single e
-00005a60: 6c65 6d65 6e74 0a20 2020 2020 2020 2020  lement.         
-00005a70: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00005a80: 203d 2076 616c 7565 5b30 5d0a 2020 2020   = value[0].    
-00005a90: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00005aa0: 6573 2e61 7070 656e 6428 7661 6c75 6529  es.append(value)
-00005ab0: 0a0a 2020 2020 2020 2020 6966 206d 6973  ..        if mis
-00005ac0: 7369 6e67 5f76 616c 7565 206f 7220 5472  sing_value or Tr
-00005ad0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00005ae0: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
-00005af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b00: 2022 4d69 7373 696e 6720 7661 6c75 6528   "Missing value(
-00005b10: 7329 2066 696c 6c65 6420 746f 2070 7265  s) filled to pre
-00005b20: 7669 6f75 7320 7661 6c75 6520 666f 7220  vious value for 
-00005b30: 6b69 6e64 2027 2573 2720 616e 6420 6b65  kind '%s' and ke
-00005b40: 7920 2725 7327 222c 0a20 2020 2020 2020  y '%s'",.       
-00005b50: 2020 2020 2020 2020 206b 696e 642c 0a20           kind,. 
-00005b60: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00005b70: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
-00005b80: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00005b90: 6e20 6e75 6d70 792e 6173 6172 7261 7928  n numpy.asarray(
-00005ba0: 7661 6c75 6573 2920 2023 206d 616b 6573  values)  # makes
-00005bb0: 2073 7572 6520 7468 6579 2061 6c6c 2068   sure they all h
-00005bc0: 6176 6520 7468 6520 7361 6d65 2064 7479  ave the same dty
-00005bd0: 7065 0a0a 2020 2020 6465 6620 5f5f 636f  pe..    def __co
-00005be0: 6d70 7574 655f 6368 616e 6769 6e67 5f76  mpute_changing_v
-00005bf0: 616c 7565 2873 656c 662c 2076 616c 7565  alue(self, value
-00005c00: 732c 2063 6861 6e67 696e 675f 7661 6c75  s, changing_valu
-00005c10: 653d 3129 3a0a 2020 2020 2020 2020 2222  e=1):.        ""
-00005c20: 220a 2020 2020 2020 2020 5265 6375 7273  ".        Recurs
-00005c30: 6976 6520 6d65 7468 6f64 2075 7365 6420  ive method used 
-00005c40: 746f 2063 616c 6375 6c61 7465 2068 6f77  to calculate how
-00005c50: 2066 6173 7420 6973 2061 2064 696d 656e   fast is a dimen
-00005c60: 7369 6f6e 2e20 5468 6520 7370 6565 6420  sion. The speed 
-00005c70: 6f66 2061 2064 696d 656e 7369 6f6e 2069  of a dimension i
-00005c80: 7320 7468 6520 6e75 6d62 6572 206f 660a  s the number of.
-00005c90: 2020 2020 2020 2020 7469 6d65 7320 7468          times th
-00005ca0: 6520 6469 6d65 6e73 696f 6e20 6368 616e  e dimension chan
-00005cb0: 6765 7320 6f66 2076 616c 7565 2077 6869  ges of value whi
-00005cc0: 6c65 206d 6f76 696e 6720 7468 726f 7567  le moving throug
-00005cd0: 6820 7468 6520 6461 7461 7365 742e 0a20  h the dataset.. 
-00005ce0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005cf0: 2020 2069 6620 6c65 6e28 6e75 6d70 792e     if len(numpy.
-00005d00: 756e 6971 7565 2876 616c 7565 7329 2920  unique(values)) 
-00005d10: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-00005d20: 2072 6574 7572 6e20 7365 6c66 2e5f 5f63   return self.__c
-00005d30: 6f6d 7075 7465 5f63 6861 6e67 696e 675f  ompute_changing_
-00005d40: 7661 6c75 6528 0a20 2020 2020 2020 2020  value(.         
-00005d50: 2020 2020 2020 2076 616c 7565 735b 3a20         values[: 
-00005d60: 696e 7428 6c65 6e28 7661 6c75 6573 2920  int(len(values) 
-00005d70: 2f20 3229 5d2c 2063 6861 6e67 696e 675f  / 2)], changing_
-00005d80: 7661 6c75 6520 2b20 310a 2020 2020 2020  value + 1.      
-00005d90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005da0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005db0: 2020 7265 7475 726e 2063 6861 6e67 696e    return changin
-00005dc0: 675f 7661 6c75 650a 0a20 2020 2064 6566  g_value..    def
-00005dd0: 2067 6574 5f64 696d 656e 7369 6f6e 735f   get_dimensions_
-00005de0: 7661 6c75 6573 2873 656c 662c 2069 6e64  values(self, ind
-00005df0: 6963 6573 3d4e 6f6e 6529 3a0a 2020 2020  ices=None):.    
-00005e00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005e10: 5265 7475 726e 7320 616c 6c20 7468 6520  Returns all the 
-00005e20: 6d65 7461 6461 7461 2076 616c 7565 7320  metadata values 
-00005e30: 6f66 2074 6865 2064 696d 656e 7369 6f6e  of the dimension
-00005e40: 732e 0a20 2020 2020 2020 2054 6865 2076  s..        The v
-00005e50: 616c 7565 7320 6172 6520 6173 7375 6d65  alues are assume
-00005e60: 6420 746f 2062 6520 6e75 6d62 6572 732e  d to be numbers.
-00005e70: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00005e80: 6e73 3a20 6172 7261 795f 6c69 6b65 0a20  ns: array_like. 
-00005e90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005ea0: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00005eb0: 6469 6d65 6e73 696f 6e73 5f76 616c 7565  dimensions_value
-00005ec0: 7320 6f72 2069 6e64 6963 6573 2069 7320  s or indices is 
-00005ed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00005ee0: 2020 2020 2020 666f 7220 6469 6d65 6e73        for dimens
-00005ef0: 696f 6e20 696e 2073 656c 662e 5f5f 6469  ion in self.__di
-00005f00: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00005f10: 2020 2020 7365 6c66 2e5f 6469 6d65 6e73      self._dimens
-00005f20: 696f 6e73 5f76 616c 7565 735b 6469 6d65  ions_values[dime
-00005f30: 6e73 696f 6e5b 315d 2e6e 616d 655d 203d  nsion[1].name] =
-00005f40: 2073 656c 662e 6765 745f 6d65 7461 6461   self.get_metada
-00005f50: 7461 5f76 616c 7565 7328 0a20 2020 2020  ta_values(.     
-00005f60: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00005f70: 696e 643d 6469 6d65 6e73 696f 6e5b 315d  ind=dimension[1]
-00005f80: 2e6b 696e 642c 206b 6579 3d64 696d 656e  .kind, key=dimen
-00005f90: 7369 6f6e 5b31 5d2e 6e61 6d65 2c20 696e  sion[1].name, in
-00005fa0: 6469 6365 733d 696e 6469 6365 730a 2020  dices=indices.  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00005fc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005fd0: 656c 662e 5f64 696d 656e 7369 6f6e 735f  elf._dimensions_
-00005fe0: 7661 6c75 6573 0a0a 2020 2020 6465 6620  values..    def 
-00005ff0: 636f 6d70 7574 655f 6d6f 7361 6963 6974  compute_mosaicit
-00006000: 795f 636f 6c6f 726b 6579 280a 2020 2020  y_colorkey(.    
-00006010: 2020 2020 7365 6c66 2c20 6469 6d65 6e73      self, dimens
-00006020: 696f 6e73 3d5b 302c 2031 5d2c 2073 6361  ions=[0, 1], sca
-00006030: 6c65 3d31 3030 2c20 696e 6469 6365 733d  le=100, indices=
-00006040: 4e6f 6e65 2c20 7468 6972 645f 6d6f 746f  None, third_moto
-00006050: 723d 4e6f 6e65 0a20 2020 2029 3a0a 2020  r=None.    ):.  
-00006060: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006070: 2020 436f 6d70 7574 6573 2061 206d 6f73    Computes a mos
-00006080: 6169 6369 7479 2063 6f6c 6f72 6b65 7920  aicity colorkey 
-00006090: 6672 6f6d 2074 6865 2064 696d 656e 7369  from the dimensi
-000060a0: 6f6e 732c 2061 6e64 2072 6574 7572 6e73  ons, and returns
-000060b0: 2061 6c73 6f20 7468 650a 2020 2020 2020   also the.      
-000060c0: 2020 6f72 6965 6e74 6174 696f 6e20 6469    orientation di
-000060d0: 7374 7269 6275 7469 6f6e 2069 6d61 6765  stribution image
-000060e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000060f0: 2020 2020 2020 2320 6f6e 6c79 2077 6f72        # only wor
-00006100: 6b20 7769 7468 2032 2064 696d 656e 7369  k with 2 dimensi
-00006110: 6f6e 730a 2020 2020 2020 2020 6173 7365  ons.        asse
-00006120: 7274 206c 656e 2864 696d 656e 7369 6f6e  rt len(dimension
-00006130: 7329 203d 3d20 322c 2022 4f6e 6c79 2077  s) == 2, "Only w
-00006140: 6f72 6b73 2077 6974 6820 7477 6f20 6d6f  orks with two mo
-00006150: 746f 7273 220a 2020 2020 2020 2020 6966  tors".        if
-00006160: 2073 656c 662e 5f5f 6469 6d73 2061 6e64   self.__dims and
-00006170: 2073 656c 662e 5f5f 6469 6d73 2e6e 6469   self.__dims.ndi
-00006180: 6d20 3e20 313a 0a20 2020 2020 2020 2020  m > 1:.         
-00006190: 2020 206e 6577 5f73 6861 7065 203d 205b     new_shape = [
-000061a0: 5d0a 2020 2020 2020 2020 2020 2020 6469  ].            di
-000061b0: 6d73 5f6c 6973 7420 3d20 5b5d 0a20 2020  ms_list = [].   
-000061c0: 2020 2020 2020 2020 2066 6f72 2061 7869           for axi
-000061d0: 7320 696e 2064 696d 656e 7369 6f6e 733a  s in dimensions:
-000061e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000061f0: 2064 696d 203d 2073 656c 662e 5f5f 6469   dim = self.__di
-00006200: 6d73 2e67 6574 2861 7869 7329 0a20 2020  ms.get(axis).   
-00006210: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00006220: 735f 6c69 7374 202b 3d20 5b6e 756d 7079  s_list += [numpy
-00006230: 2e6c 696e 7370 6163 6528 2d31 2c20 312c  .linspace(-1, 1,
-00006240: 2064 696d 2e73 697a 6520 2a20 7363 616c   dim.size * scal
-00006250: 6529 5d0a 2020 2020 2020 2020 2020 2020  e)].            
-00006260: 2020 2020 6e65 775f 7368 6170 6520 2b3d      new_shape +=
-00006270: 205b 6469 6d2e 7369 7a65 5d0a 2020 2020   [dim.size].    
-00006280: 2020 2020 2020 2020 6469 6d73 5f6c 6973          dims_lis
-00006290: 742e 7265 7665 7273 6528 290a 2020 2020  t.reverse().    
-000062a0: 2020 2020 2020 2020 6d65 7368 203d 206e          mesh = n
-000062b0: 756d 7079 2e6d 6573 6867 7269 6428 2a64  umpy.meshgrid(*d
-000062c0: 696d 735f 6c69 7374 290a 2020 2020 2020  ims_list).      
-000062d0: 2020 2020 2020 6461 7461 203d 206e 756d        data = num
-000062e0: 7079 2e61 7263 7461 6e32 286d 6573 685b  py.arctan2(mesh[
-000062f0: 305d 2c20 6d65 7368 5b31 5d29 0a20 2020  0], mesh[1]).   
-00006300: 2020 2020 2020 2020 206e 6f72 6d61 6c69           normali
-00006310: 7a65 645f 6461 7461 203d 2077 7261 7054  zed_data = wrapT
-00006320: 6f32 7069 2864 6174 6129 202f 206e 756d  o2pi(data) / num
-00006330: 7079 2e70 6920 2f20 320a 2020 2020 2020  py.pi / 2.      
-00006340: 2020 2020 2020 7371 7220 3d20 6e75 6d70        sqr = nump
-00006350: 792e 7371 7274 280a 2020 2020 2020 2020  y.sqrt(.        
-00006360: 2020 2020 2020 2020 6e75 6d70 792e 706f          numpy.po
-00006370: 7765 7228 6d65 7368 5b30 5d2c 2032 2920  wer(mesh[0], 2) 
-00006380: 2b20 6e75 6d70 792e 706f 7765 7228 6d65  + numpy.power(me
-00006390: 7368 5b31 5d2c 2032 290a 2020 2020 2020  sh[1], 2).      
-000063a0: 2020 2020 2020 2920 2f20 6e75 6d70 792e        ) / numpy.
-000063b0: 7371 7274 2832 290a 2020 2020 2020 2020  sqrt(2).        
-000063c0: 2020 2020 6873 765f 6b65 7920 3d20 6e75      hsv_key = nu
-000063d0: 6d70 792e 7374 6163 6b28 0a20 2020 2020  mpy.stack(.     
-000063e0: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 206e 6f72 6d61 6c69 7a65 645f 6461 7461   normalized_data
-00006410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006420: 2020 2020 2020 7371 722c 0a20 2020 2020        sqr,.     
-00006430: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00006440: 756d 7079 2e6f 6e65 7328 286c 656e 2864  umpy.ones((len(d
-00006450: 696d 735f 6c69 7374 5b31 5d29 2c20 6c65  ims_list[1]), le
-00006460: 6e28 6469 6d73 5f6c 6973 745b 305d 2929  n(dims_list[0]))
-00006470: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00006480: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00006490: 2020 2020 2020 6178 6973 3d32 2c0a 2020        axis=2,.  
-000064a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000064b0: 2020 2020 2020 2020 206f 7269 5f64 6973           ori_dis
-000064c0: 7420 3d20 6e75 6d70 792e 7a65 726f 7328  t = numpy.zeros(
-000064d0: 6e65 775f 7368 6170 655b 305d 202a 206e  new_shape[0] * n
-000064e0: 6577 5f73 6861 7065 5b31 5d29 0a20 2020  ew_shape[1]).   
-000064f0: 2020 2020 2020 2020 205f 736c 6963 6531           _slice1
-00006500: 203d 206f 7269 5f64 6973 742e 7368 6170   = ori_dist.shap
-00006510: 655b 305d 202a 2074 6869 7264 5f6d 6f74  e[0] * third_mot
-00006520: 6f72 0a20 2020 2020 2020 2020 2020 205f  or.            _
-00006530: 736c 6963 6532 203d 206f 7269 5f64 6973  slice2 = ori_dis
-00006540: 742e 7368 6170 655b 305d 202a 2028 7468  t.shape[0] * (th
-00006550: 6972 645f 6d6f 746f 7220 2b20 3129 0a20  ird_motor + 1). 
-00006560: 2020 2020 2020 2020 2020 206f 7269 5f64             ori_d
-00006570: 6973 745b 696e 6469 6365 735d 203d 2073  ist[indices] = s
-00006580: 656c 662e 6765 745f 6461 7461 2869 6e64  elf.get_data(ind
-00006590: 6963 6573 292e 7375 6d28 6178 6973 3d31  ices).sum(axis=1
-000065a0: 295b 5f73 6c69 6365 313a 5f73 6c69 6365  )[_slice1:_slice
-000065b0: 325d 0a20 2020 2020 2020 2020 2020 2072  2].            r
-000065c0: 6574 7572 6e20 6f72 695f 6469 7374 2e72  eturn ori_dist.r
-000065d0: 6573 6861 7065 286e 756d 7079 2e66 6c69  eshape(numpy.fli
-000065e0: 7028 6e65 775f 7368 6170 6529 292e 542c  p(new_shape)).T,
-000065f0: 2068 7376 5f6b 6579 0a20 2020 2020 2020   hsv_key.       
-00006600: 2072 6574 7572 6e20 4e6f 6e65 2c20 4e6f   return None, No
-00006610: 6e65 0a0a 2020 2020 6465 6620 6170 706c  ne..    def appl
-00006620: 795f 6261 636b 6772 6f75 6e64 5f73 7562  y_background_sub
-00006630: 7472 6163 7469 6f6e 280a 2020 2020 2020  traction(.      
-00006640: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00006650: 6261 636b 6772 6f75 6e64 3d4e 6f6e 652c  background=None,
-00006660: 0a20 2020 2020 2020 206d 6574 686f 643d  .        method=
-00006670: 226d 6564 6961 6e22 2c0a 2020 2020 2020  "median",.      
-00006680: 2020 696e 6469 6365 733d 4e6f 6e65 2c0a    indices=None,.
-00006690: 2020 2020 2020 2020 7374 6570 3d4e 6f6e          step=Non
-000066a0: 652c 0a20 2020 2020 2020 2063 6875 6e6b  e,.        chunk
-000066b0: 5f73 6861 7065 3d5b 3130 302c 2031 3030  _shape=[100, 100
-000066c0: 5d2c 0a20 2020 2020 2020 205f 6469 723d  ],.        _dir=
-000066d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000066e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000066f0: 2041 7070 6c69 6573 2062 6163 6b67 726f   Applies backgro
-00006700: 756e 6420 7375 6274 7261 6374 696f 6e20  und subtraction 
-00006710: 746f 2074 6865 2064 6174 6120 616e 6420  to the data and 
-00006720: 7361 7665 7320 7468 6520 6e65 7720 6461  saves the new da
-00006730: 7461 0a20 2020 2020 2020 2069 6e74 6f20  ta.        into 
-00006740: 6469 736b 2e0a 0a20 2020 2020 2020 203a  disk...        :
-00006750: 7061 7261 6d20 6261 636b 6772 6f75 6e64  param background
-00006760: 3a20 4461 7461 2074 6f20 6265 2075 7365  : Data to be use
-00006770: 6420 6173 2062 6163 6b67 726f 756e 642e  d as background.
-00006780: 2049 6620 4e6f 6e65 2c20 6461 7461 2077   If None, data w
-00006790: 6974 6820 696e 6469 6365 7320 6069 6e64  ith indices `ind
-000067a0: 6963 6573 6020 6973 2075 7365 642e 0a20  ices` is used.. 
-000067b0: 2020 2020 2020 2020 2020 2049 6620 4461             If Da
-000067c0: 7461 7365 742c 2064 6174 6120 6f66 2074  taset, data of t
-000067d0: 6865 2064 6174 6173 6574 2069 7320 7573  he dataset is us
-000067e0: 6564 2e20 4966 2061 7272 6179 2c20 7573  ed. If array, us
-000067f0: 6520 6461 7461 2077 6974 6820 696e 6469  e data with indi
-00006800: 6365 7320 696e 2074 6865 2061 7272 6179  ces in the array
-00006810: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00006820: 6261 636b 6772 6f75 6e64 3a20 556e 696f  background: Unio
-00006830: 6e5b 4e6f 6e65 2c20 6172 7261 795f 6c69  n[None, array_li
-00006840: 6b65 2c20 4461 7461 7365 745d 0a20 2020  ke, Dataset].   
-00006850: 2020 2020 203a 7061 7261 6d20 6d65 7468       :param meth
-00006860: 6f64 3a20 4d65 7468 6f64 2074 6f20 7573  od: Method to us
-00006870: 6520 746f 2063 6f6d 7075 7465 2074 6865  e to compute the
-00006880: 2062 6163 6b67 726f 756e 642e 0a20 2020   background..   
-00006890: 2020 2020 203a 7479 7065 206d 6574 686f       :type metho
-000068a0: 643a 204d 6574 686f 640a 2020 2020 2020  d: Method.      
-000068b0: 2020 3a70 6172 616d 2069 6e64 6963 6573    :param indices
-000068c0: 3a20 496e 6469 6365 7320 6f66 2074 6865  : Indices of the
-000068d0: 2069 6d61 6765 7320 746f 2061 7070 6c79   images to apply
-000068e0: 2062 6163 6b67 726f 756e 6420 7375 6274   background subt
-000068f0: 7261 6374 696f 6e2e 0a20 2020 2020 2020  raction..       
-00006900: 2020 2020 2049 6620 4e6f 6e65 2c20 7468       If None, th
-00006910: 6520 6261 636b 6772 6f75 6e64 2073 7562  e background sub
-00006920: 7472 6163 7469 6f6e 2069 7320 6170 706c  traction is appl
-00006930: 6965 6420 746f 2061 6c6c 2074 6865 2064  ied to all the d
-00006940: 6174 612e 0a20 2020 2020 2020 203a 7479  ata..        :ty
-00006950: 7065 2069 6e64 6963 6573 3a20 556e 696f  pe indices: Unio
-00006960: 6e5b 4e6f 6e65 2c20 6172 7261 795f 6c69  n[None, array_li
-00006970: 6b65 5d0a 2020 2020 2020 2020 3a70 6172  ke].        :par
-00006980: 616d 2069 6e74 2073 7465 703a 2044 6973  am int step: Dis
-00006990: 7461 6e63 6520 6265 7477 6565 6e20 696d  tance between im
-000069a0: 6167 6573 2074 6f20 6265 2075 7365 6420  ages to be used 
-000069b0: 7768 656e 2063 6f6d 7075 7469 6e67 2074  when computing t
-000069c0: 6865 206d 6564 6961 6e2e 0a20 2020 2020  he median..     
-000069d0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000069e0: 2075 7365 6420 6f6e 6c79 2077 6865 6e20   used only when 
-000069f0: 666c 6167 2069 6e5f 6d65 6d6f 7279 2069  flag in_memory i
-00006a00: 7320 4661 6c73 6520 616e 6420 6d65 7468  s False and meth
-00006a10: 6f64 2069 7320 604d 6574 686f 642e 6d65  od is `Method.me
-00006a20: 6469 616e 602e 0a20 2020 2020 2020 2020  dian`..         
-00006a30: 2020 2049 6620 6073 7465 7060 2069 7320     If `step` is 
-00006a40: 6e6f 7420 4e6f 6e65 2c20 616c 6c20 696d  not None, all im
-00006a50: 6167 6573 2077 6974 6820 6469 7374 616e  ages with distan
-00006a60: 6365 206f 6620 6073 7465 7060 2c20 7374  ce of `step`, st
-00006a70: 6172 7469 6e67 2061 7420 302c 0a20 2020  arting at 0,.   
-00006a80: 2020 2020 2020 2020 2077 696c 6c20 6265           will be
-00006a90: 206c 6f61 6465 6420 696e 746f 206d 656d   loaded into mem
-00006aa0: 6f72 7920 666f 7220 636f 6d70 7574 696e  ory for computin
-00006ab0: 6720 7468 6520 6d65 6469 616e 2c20 6966  g the median, if
-00006ac0: 2074 6865 2064 6174 6120 6c6f 6164 696e   the data loadin
-00006ad0: 6720 7468 726f 7773 0a20 2020 2020 2020  g throws.       
-00006ae0: 2020 2020 2061 204d 656d 6f72 7945 7272       a MemoryErr
-00006af0: 6f72 2c20 7468 6520 6d65 6469 616e 2063  or, the median c
-00006b00: 6f6d 7075 7461 7469 6f6e 2069 7320 7472  omputation is tr
-00006b10: 6965 6420 7769 7468 2060 7374 6570 202b  ied with `step +
-00006b20: 3d20 3160 2e0a 2020 2020 2020 2020 3a70  = 1`..        :p
-00006b30: 6172 616d 2063 6875 6e6b 5f73 6861 7065  aram chunk_shape
-00006b40: 3a20 5368 6170 6520 6f66 2074 6865 2063  : Shape of the c
-00006b50: 6875 6e6b 2069 6d61 6765 2074 6f20 7573  hunk image to us
-00006b60: 6520 7065 7220 6974 6572 6174 696f 6e2e  e per iteration.
-00006b70: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
-00006b80: 616d 6574 6572 2075 7365 6420 6f6e 6c79  ameter used only
-00006b90: 2077 6865 6e20 666c 6167 2069 6e5f 6d65   when flag in_me
-00006ba0: 6d6f 7279 2069 7320 4661 6c73 6520 616e  mory is False an
-00006bb0: 6420 6d65 7468 6f64 2069 7320 604d 6574  d method is `Met
-00006bc0: 686f 642e 6d65 6469 616e 602e 0a20 2020  hod.median`..   
-00006bd0: 2020 2020 203a 7479 7065 2063 6875 6e6b       :type chunk
-00006be0: 5f73 6861 7065 3a20 6172 7261 795f 6c69  _shape: array_li
-00006bf0: 6b65 0a20 2020 2020 2020 203a 7265 7475  ke.        :retu
-00006c00: 726e 733a 2064 6174 6173 6574 2077 6974  rns: dataset wit
-00006c10: 6820 6461 7461 206f 6620 7361 6d65 2073  h data of same s
-00006c20: 697a 6520 6173 2060 7365 6c66 2e64 6174  ize as `self.dat
-00006c30: 6160 2062 7574 2077 6974 6820 7468 650a  a` but with the.
-00006c40: 2020 2020 2020 2020 2020 2020 6d6f 6469              modi
-00006c50: 6669 6564 2069 6d61 6765 732e 2054 6865  fied images. The
-00006c60: 2075 726c 7320 6f66 2074 6865 206d 6f64   urls of the mod
-00006c70: 6966 6965 6420 696d 6167 6573 2061 7265  ified images are
-00006c80: 2072 6570 6c61 6365 6420 7769 7468 0a20   replaced with. 
-00006c90: 2020 2020 2020 2020 2020 2074 6865 206e             the n
-00006ca0: 6577 2075 726c 732e 0a20 2020 2020 2020  ew urls..       
-00006cb0: 203a 7274 7970 653a 2044 6174 6173 6574   :rtype: Dataset
-00006cc0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00006cd0: 2020 2020 2020 5f64 6972 203d 2073 656c        _dir = sel
-00006ce0: 662e 6469 7220 6966 205f 6469 7220 6973  f.dir if _dir is
-00006cf0: 204e 6f6e 6520 656c 7365 205f 6469 720a   None else _dir.
-00006d00: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
-00006d10: 6469 7273 285f 6469 722c 2065 7869 7374  dirs(_dir, exist
-00006d20: 5f6f 6b3d 5472 7565 290a 0a20 2020 2020  _ok=True)..     
-00006d30: 2020 2074 656d 705f 6469 7220 3d20 6f73     temp_dir = os
-00006d40: 2e70 6174 682e 6a6f 696e 285f 6469 722c  .path.join(_dir,
-00006d50: 2022 7465 6d70 5f64 6972 2229 0a0a 2020   "temp_dir")..  
-00006d60: 2020 2020 2020 6f73 2e6d 616b 6564 6972        os.makedir
-00006d70: 7328 7465 6d70 5f64 6972 2c20 6578 6973  s(temp_dir, exis
-00006d80: 745f 6f6b 3d54 7275 6529 0a0a 2020 2020  t_ok=True)..    
-00006d90: 2020 2020 6d65 7468 6f64 203d 204d 6574      method = Met
-00006da0: 686f 642e 6672 6f6d 5f76 616c 7565 286d  hod.from_value(m
-00006db0: 6574 686f 6429 0a0a 2020 2020 2020 2020  ethod)..        
-00006dc0: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
-00006dd0: 6120 3d20 7365 6c66 2e67 6574 5f64 6174  a = self.get_dat
-00006de0: 6128 696e 6469 6365 7329 0a0a 2020 2020  a(indices)..    
-00006df0: 2020 2020 7769 7468 2073 656c 662e 7374      with self.st
-00006e00: 6174 655f 6f66 5f6f 7065 7261 7469 6f6e  ate_of_operation
-00006e10: 732e 7275 6e5f 636f 6e74 6578 7428 4f70  s.run_context(Op
-00006e20: 6572 6174 696f 6e2e 4253 293a 0a20 2020  eration.BS):.   
-00006e30: 2020 2020 2020 2020 2069 6620 6261 636b           if back
-00006e40: 6772 6f75 6e64 2069 7320 4e6f 6e65 3a0a  ground is None:.
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 6267 5f64 6174 6120 3d20 7365 6c66 2e72  bg_data = self.r
-00006e70: 756e 6e69 6e67 5f64 6174 610a 2020 2020  unning_data.    
-00006e80: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00006e90: 6e64 6963 6573 2069 7320 4e6f 6e65 3a0a  ndices is None:.
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 5f6c 6f67 6765 722e 696e 666f      _logger.info
-00006ec0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006ed0: 2020 2020 2020 2020 2020 2243 6f6d 7075            "Compu
-00006ee0: 7469 6e67 2062 6163 6b67 726f 756e 6420  ting background 
-00006ef0: 6672 6f6d 2025 7320 6f66 2072 6177 2064  from %s of raw d
-00006f00: 6174 6122 2c20 6d65 7468 6f64 2e6e 616d  ata", method.nam
-00006f10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00006f20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006f30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f50: 2020 5f6c 6f67 6765 722e 696e 666f 280a    _logger.info(.
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 2243 6f6d 7075 7469          "Computi
-00006f80: 6e67 2062 6163 6b67 726f 756e 6420 6672  ng background fr
-00006f90: 6f6d 2025 7320 6f66 2068 6967 6820 696e  om %s of high in
-00006fa0: 7465 6e73 6974 7920 6461 7461 222c 0a20  tensity data",. 
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2020 206d 6574 686f 642e 6e61         method.na
-00006fd0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00006fe0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006ff0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00007000: 7461 6e63 6528 6261 636b 6772 6f75 6e64  tance(background
-00007010: 2c20 4461 7461 7365 7429 3a0a 2020 2020  , Dataset):.    
-00007020: 2020 2020 2020 2020 2020 2020 6267 5f64              bg_d
-00007030: 6174 6120 3d20 6261 636b 6772 6f75 6e64  ata = background
-00007040: 2e64 6174 610a 2020 2020 2020 2020 2020  .data.          
-00007050: 2020 2020 2020 5f6c 6f67 6765 722e 696e        _logger.in
-00007060: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-00007070: 2020 2020 2020 2020 2243 6f6d 7075 7469          "Computi
-00007080: 6e67 2062 6163 6b67 726f 756e 6420 6672  ng background fr
-00007090: 6f6d 2025 7320 6f66 2060 6261 636b 6772  om %s of `backgr
-000070a0: 6f75 6e64 6020 7365 7422 2c20 6d65 7468  ound` set", meth
-000070b0: 6f64 2e6e 616d 650a 2020 2020 2020 2020  od.name.        
-000070c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000070d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000070e0: 2020 2020 2020 2020 2020 2020 6267 5f64              bg_d
-000070f0: 6174 6120 3d20 7365 6c66 2e67 6574 5f64  ata = self.get_d
-00007100: 6174 6128 6261 636b 6772 6f75 6e64 290a  ata(background).
-00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007120: 5f6c 6f67 6765 722e 696e 666f 280a 2020  _logger.info(.  
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2243 6f6d 7075 7469 6e67 2062 6163    "Computing bac
-00007150: 6b67 726f 756e 6420 6672 6f6d 2025 7320  kground from %s 
-00007160: 6f66 206c 6f77 2069 6e74 656e 7369 7479  of low intensity
-00007170: 2064 6174 6122 2c20 6d65 7468 6f64 2e6e   data", method.n
-00007180: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00007190: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-000071a0: 2020 2069 6620 7365 6c66 2e5f 696e 5f6d     if self._in_m
-000071b0: 656d 6f72 793a 0a20 2020 2020 2020 2020  emory:.         
-000071c0: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
-000071d0: 3d20 6261 636b 6772 6f75 6e64 5f73 7562  = background_sub
-000071e0: 7472 6163 7469 6f6e 280a 2020 2020 2020  traction(.      
-000071f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007200: 6c66 2e72 756e 6e69 6e67 5f64 6174 612c  lf.running_data,
-00007210: 2062 675f 6461 7461 2c20 6d65 7468 6f64   bg_data, method
-00007220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007230: 2029 2e76 6965 7728 4461 7461 290a 2020   ).view(Data).  
-00007240: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00007250: 775f 6461 7461 2e73 6176 6528 6f73 2e70  w_data.save(os.p
-00007260: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
-00007270: 722c 2022 6461 7461 2e68 6466 3522 2929  r, "data.hdf5"))
-00007280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007290: 2075 726c 7320 3d20 6e65 775f 6461 7461   urls = new_data
-000072a0: 2e75 726c 730a 2020 2020 2020 2020 2020  .urls.          
-000072b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000072c0: 2020 2020 2020 2020 6267 203d 206e 756d          bg = num
-000072d0: 7079 2e7a 6572 6f73 2873 656c 662e 7275  py.zeros(self.ru
-000072e0: 6e6e 696e 675f 6461 7461 5b30 5d2e 7368  nning_data[0].sh
-000072f0: 6170 652c 2073 656c 662e 7275 6e6e 696e  ape, self.runnin
-00007300: 675f 6461 7461 2e64 7479 7065 290a 2020  g_data.dtype).  
-00007310: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00007320: 206d 6574 686f 6420 3d3d 204d 6574 686f   method == Metho
-00007330: 642e 6d65 616e 3a0a 2020 2020 2020 2020  d.mean:.        
-00007340: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-00007350: 675f 6461 7461 2e69 6e5f 6d65 6d6f 7279  g_data.in_memory
-00007360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007370: 2020 2020 2020 2020 2020 6e75 6d70 792e            numpy.
-00007380: 6d65 616e 2862 675f 6461 7461 2c20 6f75  mean(bg_data, ou
-00007390: 743d 6267 2c20 6178 6973 3d30 290a 2020  t=bg, axis=0).  
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 696f 5f75 7469 6c73 2e61 6476 616e 6365  io_utils.advance
-000073e0: 6d65 6e74 5f64 6973 706c 6179 280a 2020  ment_display(.  
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007400: 2020 2020 2020 2020 2020 302c 206c 656e            0, len
-00007410: 2862 675f 6461 7461 292c 2022 436f 6d70  (bg_data), "Comp
-00007420: 7574 696e 6720 6d65 616e 2069 6d61 6765  uting mean image
-00007430: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00007440: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00007470: 6765 286c 656e 2862 675f 6461 7461 2929  ge(len(bg_data))
-00007480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007490: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000074a0: 206e 6f74 2073 656c 662e 7374 6174 655f   not self.state_
-000074b0: 6f66 5f6f 7065 7261 7469 6f6e 732e 6973  of_operations.is
-000074c0: 5f72 756e 6e69 6e67 284f 7065 7261 7469  _running(Operati
-000074d0: 6f6e 2e42 5329 3a0a 2020 2020 2020 2020  on.BS):.        
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 2020 2020 2020 2020 2020 2062 6720 3d20             bg = 
-00007520: 696d 6732 696d 675f 6d65 616e 2862 675f  img2img_mean(bg_
-00007530: 6461 7461 5b69 5d2c 2062 672c 2069 290a  data[i], bg, i).
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 2020 2020 2020 696f 5f75              io_u
-00007560: 7469 6c73 2e61 6476 616e 6365 6d65 6e74  tils.advancement
-00007570: 5f64 6973 706c 6179 280a 2020 2020 2020  _display(.      
+00002510: 2020 2020 2020 6864 6635 5f69 7465 6d20        hdf5_item 
+00002520: 3d20 6835 5b75 726c 2e64 6174 615f 7061  = h5[url.data_pa
+00002530: 7468 2829 5d0a 2020 2020 2020 2020 2020  th()].          
+00002540: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00002550: 2069 7369 6e73 7461 6e63 6528 6864 6635   isinstance(hdf5
+00002560: 5f69 7465 6d2c 2068 3570 792e 4461 7461  _item, h5py.Data
+00002570: 7365 7429 3a0a 2020 2020 2020 2020 2020  set):.          
+00002580: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002590: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 2020 2020 6622 7572              f"ur
+000025c0: 6c20 6461 7461 2070 6174 6820 6973 206e  l data path is n
+000025d0: 6f74 2070 6f69 6e74 696e 6720 746f 2061  ot pointing to a
+000025e0: 2048 4446 3520 6461 7461 7365 7420 6275   HDF5 dataset bu
+000025f0: 7420 746f 207b 7479 7065 2868 6466 355f  t to {type(hdf5_
+00002600: 6974 656d 297d 220a 2020 2020 2020 2020  item)}".        
+00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002620: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002630: 2020 2020 2020 6e5f 6672 616d 6573 203d        n_frames =
+00002640: 2068 6466 355f 6974 656d 2e73 6861 7065   hdf5_item.shape
+00002650: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00002660: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00002670: 6765 286e 5f66 7261 6d65 7329 3a0a 2020  ge(n_frames):.  
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2020 6461 7461 5f75 726c 732e 6170 7065    data_urls.appe
+000026a0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+000026b0: 2020 2020 2020 2020 2020 2020 4461 7461              Data
+000026c0: 5572 6c28 0a20 2020 2020 2020 2020 2020  Url(.           
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 2066 696c 655f 7061 7468 3d75 726c 2e66   file_path=url.f
+000026f0: 696c 655f 7061 7468 2829 2c0a 2020 2020  ile_path(),.    
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 6461 7461 5f70 6174          data_pat
+00002720: 683d 7572 6c2e 6461 7461 5f70 6174 6828  h=url.data_path(
+00002730: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00002740: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00002750: 6174 615f 736c 6963 653d 692c 0a20 2020  ata_slice=i,.   
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 2020 2073 6368 656d 653d           scheme=
+00002780: 2273 696c 7822 2c0a 2020 2020 2020 2020  "silx",.        
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000027b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000027c0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+000027d0: 6461 7461 2e61 7070 656e 6428 6765 745f  data.append(get_
+000027e0: 6d65 7461 6461 7461 2864 6174 615f 736c  metadata(data_sl
+000027f0: 6963 653d 6929 290a 2020 2020 2020 2020  ice=i)).        
+00002800: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002810: 2020 2020 2020 2020 2020 7769 7468 2066            with f
+00002820: 6162 696f 2e6f 7065 6e5f 7365 7269 6573  abio.open_series
+00002830: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002840: 2020 2020 2020 6669 6c65 6e61 6d65 733d        filenames=
+00002850: 6669 6c65 6e61 6d65 732c 2066 6972 7374  filenames, first
+00002860: 5f66 696c 656e 616d 653d 6669 7273 745f  _filename=first_
+00002870: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
+00002880: 2020 2020 2020 2020 2029 2061 7320 7365           ) as se
+00002890: 7269 6573 3a0a 2020 2020 2020 2020 2020  ries:.          
+000028a0: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
+000028b0: 616d 6520 696e 2073 6572 6965 732e 6672  ame in series.fr
+000028c0: 616d 6573 2829 3a0a 2020 2020 2020 2020  ames():.        
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 6669 6c65 6e61 6d65 203d 2066 7261 6d65  filename = frame
+000028f0: 2e66 696c 655f 636f 6e74 6169 6e65 722e  .file_container.
+00002900: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2064 6174 615f 7572 6c73 2e61 7070 656e   data_urls.appen
+00002930: 6428 4461 7461 5572 6c28 6669 6c65 5f70  d(DataUrl(file_p
+00002940: 6174 683d 6669 6c65 6e61 6d65 2c20 7363  ath=filename, sc
+00002950: 6865 6d65 3d22 6661 6269 6f22 2929 0a20  heme="fabio")). 
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 2020 2020 2020 2066 6162 696f 5f72 6561         fabio_rea
+00002980: 6465 7220 3d20 6661 6269 6f68 352e 4564  der = fabioh5.Ed
+00002990: 6646 6162 696f 5265 6164 6572 2866 696c  fFabioReader(fil
+000029a0: 655f 6e61 6d65 3d66 696c 656e 616d 6529  e_name=filename)
+000029b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029c0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+000029d0: 612e 6170 7065 6e64 2866 6162 696f 5f72  a.append(fabio_r
+000029e0: 6561 6465 7229 0a20 2020 2020 2020 2020  eader).         
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002a00: 6162 696f 5f72 6561 6465 722e 636c 6f73  abio_reader.clos
+00002a10: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00002a20: 7365 6c66 2e5f 6461 7461 203d 2044 6174  self._data = Dat
+00002a30: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
+00002a40: 2020 206e 756d 7079 2e61 7272 6179 2864     numpy.array(d
+00002a50: 6174 615f 7572 6c73 292c 206d 6574 6164  ata_urls), metad
+00002a60: 6174 613d 6d65 7461 6461 7461 2c20 696e  ata=metadata, in
+00002a70: 5f6d 656d 6f72 793d 7365 6c66 2e5f 696e  _memory=self._in
+00002a80: 5f6d 656d 6f72 790a 2020 2020 2020 2020  _memory.        
+00002a90: 2020 2020 290a 0a20 2020 2064 6566 2073      )..    def s
+00002aa0: 746f 705f 6f70 6572 6174 696f 6e28 7365  top_operation(se
+00002ab0: 6c66 2c20 6f70 6572 6174 696f 6e29 3a0a  lf, operation):.
+00002ac0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002ad0: 2020 2020 4d65 7468 6f64 2075 7365 6420      Method used 
+00002ae0: 666f 7220 6361 7365 7320 7768 6572 6520  for cases where 
+00002af0: 7468 7265 6164 7320 6172 6520 6372 6561  threads are crea
+00002b00: 7465 6420 746f 2061 7070 6c79 2066 756e  ted to apply fun
+00002b10: 6374 696f 6e73 2074 6f20 7468 6520 6461  ctions to the da
+00002b20: 7461 7365 742e 0a20 2020 2020 2020 2049  taset..        I
+00002b30: 6620 6d65 7468 6f64 2069 7320 6361 6c6c  f method is call
+00002b40: 6564 2c20 7468 6520 666c 6167 2063 6f6e  ed, the flag con
+00002b50: 6365 726e 696e 6720 7468 6520 7374 6f70  cerning the stop
+00002b60: 2069 7320 7365 7420 746f 2030 2073 6f20   is set to 0 so 
+00002b70: 7468 6174 2069 6620 7468 6520 636f 6e63  that if the conc
+00002b80: 6572 6e65 640a 2020 2020 2020 2020 6f70  erned.        op
+00002b90: 6572 6174 696f 6e20 6973 2072 756e 6e69  eration is runni
+00002ba0: 6e67 2069 6e20 616e 6f74 6865 7220 7468  ng in another th
+00002bb0: 7265 6164 2069 7420 6b6e 6f77 7320 746f  read it knows to
+00002bc0: 2073 746f 702e 0a0a 2020 2020 2020 2020   stop...        
+00002bd0: 3a70 6172 616d 2069 6e74 206f 7065 7261  :param int opera
+00002be0: 7469 6f6e 3a20 6f70 6572 6174 696f 6e20  tion: operation 
+00002bf0: 746f 2073 746f 700a 2020 2020 2020 2020  to stop.        
+00002c00: 3a74 7970 6520 696e 743a 2055 6e69 6f6e  :type int: Union
+00002c10: 5b69 6e74 2c20 604f 7065 7261 7469 6f6e  [int, `Operation
+00002c20: 605d 0a20 2020 2020 2020 2022 2222 0a20  `].        """. 
+00002c30: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00002c40: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
+00002c50: 6e73 2e69 735f 7275 6e6e 696e 6728 6f70  ns.is_running(op
+00002c60: 6572 6174 696f 6e29 3a0a 2020 2020 2020  eration):.      
+00002c70: 2020 2020 2020 7365 6c66 2e73 7461 7465        self.state
+00002c80: 5f6f 665f 6f70 6572 6174 696f 6e73 2e73  _of_operations.s
+00002c90: 746f 7028 6f70 6572 6174 696f 6e29 0a20  top(operation). 
+00002ca0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00002cb0: 756e 6e69 6e67 5f64 6174 6120 6973 206e  unning_data is n
+00002cc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002cd0: 2020 2020 2073 656c 662e 7275 6e6e 696e       self.runnin
+00002ce0: 675f 6461 7461 2e73 746f 705f 6f70 6572  g_data.stop_oper
+00002cf0: 6174 696f 6e28 6f70 6572 6174 696f 6e29  ation(operation)
+00002d00: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00002d10: 2020 2020 6465 6620 7472 616e 7366 6f72      def transfor
+00002d20: 6d61 7469 6f6e 2873 656c 6629 3a0a 2020  mation(self):.  
+00002d30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002d40: 662e 5f74 7261 6e73 666f 726d 6174 696f  f._transformatio
+00002d50: 6e0a 0a20 2020 2040 7472 616e 7366 6f72  n..    @transfor
+00002d60: 6d61 7469 6f6e 2e73 6574 7465 720a 2020  mation.setter.  
+00002d70: 2020 6465 6620 7472 616e 7366 6f72 6d61    def transforma
+00002d80: 7469 6f6e 2873 656c 662c 2076 616c 7565  tion(self, value
+00002d90: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00002da0: 5f74 7261 6e73 666f 726d 6174 696f 6e20  _transformation 
+00002db0: 3d20 7661 6c75 650a 0a20 2020 2040 7072  = value..    @pr
+00002dc0: 6f70 6572 7479 0a20 2020 2064 6566 2074  operty.    def t
+00002dd0: 6974 6c65 2873 656c 6629 3a0a 2020 2020  itle(self):.    
+00002de0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002df0: 5f74 6974 6c65 0a0a 2020 2020 4070 726f  _title..    @pro
+00002e00: 7065 7274 790a 2020 2020 6465 6620 6469  perty.    def di
+00002e10: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00002e20: 2072 6574 7572 6e20 7365 6c66 2e5f 6469   return self._di
+00002e30: 720a 0a20 2020 2040 7072 6f70 6572 7479  r..    @property
+00002e40: 0a20 2020 2064 6566 2069 735f 6835 2873  .    def is_h5(s
+00002e50: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00002e60: 7475 726e 2073 656c 662e 5f69 7348 350a  turn self._isH5.
+00002e70: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+00002e80: 5f66 7261 6d65 735f 696e 7465 6e73 6974  _frames_intensit
+00002e90: 7928 7365 6c66 2c20 6b65 726e 656c 3d28  y(self, kernel=(
+00002ea0: 332c 2033 292c 2073 6967 6d61 3d32 3029  3, 3), sigma=20)
+00002eb0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00002ec0: 2020 2020 2020 5265 7475 726e 7320 666f        Returns fo
+00002ed0: 7220 6576 6572 7920 696d 6167 6520 6120  r every image a 
+00002ee0: 6e75 6d62 6572 2072 6570 7265 7365 6e74  number represent
+00002ef0: 696e 6720 6974 7320 696e 7465 6e73 6974  ing its intensit
+00002f00: 792e 2054 6869 7320 6e75 6d62 6572 0a20  y. This number. 
+00002f10: 2020 2020 2020 2069 7320 6f62 7461 696e         is obtain
+00002f20: 6564 2062 7920 6669 7273 7420 626c 7572  ed by first blur
+00002f30: 7269 6e67 2074 6865 2069 6d61 6765 2061  ring the image a
+00002f40: 6e64 2074 6865 6e20 636f 6d70 7574 696e  nd then computin
+00002f50: 6720 6974 7320 7661 7269 616e 6365 2e0a  g its variance..
+00002f60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002f70: 2020 2020 5f6c 6f67 6765 722e 696e 666f      _logger.info
+00002f80: 2822 436f 6d70 7574 696e 6720 696e 7465  ("Computing inte
+00002f90: 6e73 6974 7920 7065 7220 6672 616d 6522  nsity per frame"
+00002fa0: 290a 2020 2020 2020 2020 696f 5f75 7469  ).        io_uti
+00002fb0: 6c73 2e61 6476 616e 6365 6d65 6e74 5f64  ls.advancement_d
+00002fc0: 6973 706c 6179 2830 2c20 7365 6c66 2e6e  isplay(0, self.n
+00002fd0: 6672 616d 6573 2c20 2243 6f6d 7075 7469  frames, "Computi
+00002fe0: 6e67 2069 6e74 656e 7369 7479 2229 0a20  ng intensity"). 
+00002ff0: 2020 2020 2020 2066 7261 6d65 735f 696e         frames_in
+00003000: 7465 6e73 6974 7920 3d20 5b5d 0a20 2020  tensity = [].   
+00003010: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00003020: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
+00003030: 6e73 2e72 756e 5f63 6f6e 7465 7874 284f  ns.run_context(O
+00003040: 7065 7261 7469 6f6e 2e50 4152 5449 5449  peration.PARTITI
+00003050: 4f4e 293a 0a20 2020 2020 2020 2020 2020  ON):.           
+00003060: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00003070: 7365 6c66 2e6e 6672 616d 6573 293a 0a20  self.nframes):. 
+00003080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003090: 6d70 6f72 7420 6376 320a 0a20 2020 2020  mport cv2..     
+000030a0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000030b0: 7420 7365 6c66 2e73 7461 7465 5f6f 665f  t self.state_of_
+000030c0: 6f70 6572 6174 696f 6e73 2e69 735f 7275  operations.is_ru
+000030d0: 6e6e 696e 6728 4f70 6572 6174 696f 6e2e  nning(Operation.
+000030e0: 5041 5254 4954 494f 4e29 3a0a 2020 2020  PARTITION):.    
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003100: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00003110: 2020 2020 2020 2066 7261 6d65 735f 696e         frames_in
+00003120: 7465 6e73 6974 7920 2b3d 205b 0a20 2020  tensity += [.   
+00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003140: 2063 7632 2e47 6175 7373 6961 6e42 6c75   cv2.GaussianBlu
+00003150: 7228 7365 6c66 2e67 6574 5f64 6174 6128  r(self.get_data(
+00003160: 6929 2c20 6b65 726e 656c 2c20 7369 676d  i), kernel, sigm
+00003170: 6129 2e76 6172 2829 0a20 2020 2020 2020  a).var().       
+00003180: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00003190: 2020 2020 2020 2020 2020 2069 6f5f 7574             io_ut
+000031a0: 696c 732e 6164 7661 6e63 656d 656e 745f  ils.advancement_
+000031b0: 6469 7370 6c61 7928 6920 2b20 312c 2073  display(i + 1, s
+000031c0: 656c 662e 6e66 7261 6d65 732c 2022 436f  elf.nframes, "Co
+000031d0: 6d70 7574 696e 6720 696e 7465 6e73 6974  mputing intensit
+000031e0: 7922 290a 2020 2020 2020 2020 2020 2020  y").            
+000031f0: 7365 6c66 2e5f 6672 616d 6573 5f69 6e74  self._frames_int
+00003200: 656e 7369 7479 203d 2066 7261 6d65 735f  ensity = frames_
+00003210: 696e 7465 6e73 6974 790a 2020 2020 2020  intensity.      
+00003220: 2020 2020 2020 7265 7475 726e 2066 7261        return fra
+00003230: 6d65 735f 696e 7465 6e73 6974 790a 0a20  mes_intensity.. 
+00003240: 2020 2064 6566 2070 6172 7469 7469 6f6e     def partition
+00003250: 5f62 795f 696e 7465 6e73 6974 7928 7365  _by_intensity(se
+00003260: 6c66 2c20 6269 6e73 3d4e 6f6e 652c 2062  lf, bins=None, b
+00003270: 6f74 746f 6d5f 6269 6e3d 4e6f 6e65 2c20  ottom_bin=None, 
+00003280: 746f 705f 6269 6e3d 4e6f 6e65 293a 0a20  top_bin=None):. 
+00003290: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000032a0: 2020 2046 756e 6374 696f 6e20 7468 6174     Function that
+000032b0: 2063 6f6d 7075 7465 7320 7468 6520 6461   computes the da
+000032c0: 7461 2066 726f 6d20 7468 6520 7365 7420  ta from the set 
+000032d0: 6f66 2075 726c 732e 0a20 2020 2020 2020  of urls..       
+000032e0: 2049 6620 7468 6520 6669 6c74 6572 5f64   If the filter_d
+000032f0: 6174 6120 666c 6167 2069 7320 6163 7469  ata flag is acti
+00003300: 7661 7465 6420 6974 2066 696c 7465 7273  vated it filters
+00003310: 2074 6865 2064 6174 6120 666f 6c6c 6f77   the data follow
+00003320: 696e 6720 7468 6520 6e65 7874 3a0a 2020  ing the next:.  
+00003330: 2020 2020 2020 2d2d 2046 6972 7374 2c20        -- First, 
+00003340: 6974 2063 6f6d 7075 7465 7320 7468 6520  it computes the 
+00003350: 696e 7465 6e73 6974 7920 666f 7220 6561  intensity for ea
+00003360: 6368 2066 7261 6d65 2c20 6279 2063 616c  ch frame, by cal
+00003370: 6375 6c61 7469 6e67 2074 6865 2076 6172  culating the var
+00003380: 6961 6e63 6520 6166 7465 720a 2020 2020  iance after.    
+00003390: 2020 2020 7061 7373 696e 6720 6120 6761      passing a ga
+000033a0: 7573 7369 616e 2066 696c 7465 722e 0a20  ussian filter.. 
+000033b0: 2020 2020 2020 202d 2d20 5365 636f 6e64         -- Second
+000033c0: 2c20 636f 6d70 7574 6573 2074 6865 2068  , computes the h
+000033d0: 6973 746f 6772 616d 206f 6620 7468 6520  istogram of the 
+000033e0: 696e 7465 6e73 6974 792e 0a20 2020 2020  intensity..     
+000033f0: 2020 202d 2d20 4669 6e61 6c6c 792c 2073     -- Finally, s
+00003400: 6176 6573 2074 6865 2064 6174 6120 6f66  aves the data of
+00003410: 2074 6865 2066 7261 6d65 7320 7769 7468   the frames with
+00003420: 2061 6e20 696e 7465 6e73 6974 7920 6269   an intensity bi
+00003430: 6767 6572 2074 6861 6e20 6120 7468 7265  gger than a thre
+00003440: 7368 6f6c 642e 0a20 2020 2020 2020 2054  shold..        T
+00003450: 6865 2074 6872 6573 686f 6c64 2069 7320  he threshold is 
+00003460: 7365 7420 746f 2062 6520 7468 6520 7365  set to be the se
+00003470: 636f 6e64 2062 696e 206f 6620 7468 6520  cond bin of the 
+00003480: 6869 7374 6f67 7261 6d2e 0a0a 2020 2020  histogram...    
+00003490: 2020 2020 3a70 6172 616d 2069 6e74 206e      :param int n
+000034a0: 756d 5f62 696e 733a 204e 756d 6265 7220  um_bins: Number 
+000034b0: 6f66 2062 696e 7320 746f 2075 7365 2061  of bins to use a
+000034c0: 7320 7468 7265 7368 6f6c 642e 0a20 2020  s threshold..   
+000034d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000034e0: 2066 7261 6d65 735f 696e 7465 6e73 6974   frames_intensit
+000034f0: 7920 3d20 280a 2020 2020 2020 2020 2020  y = (.          
+00003500: 2020 7365 6c66 2e5f 6672 616d 6573 5f69    self._frames_i
+00003510: 6e74 656e 7369 7479 0a20 2020 2020 2020  ntensity.       
+00003520: 2020 2020 2069 6620 7365 6c66 2e5f 6672       if self._fr
+00003530: 616d 6573 5f69 6e74 656e 7369 7479 0a20  ames_intensity. 
+00003540: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00003550: 7365 6c66 2e63 6f6d 7075 7465 5f66 7261  self.compute_fra
+00003560: 6d65 735f 696e 7465 6e73 6974 7928 290a  mes_intensity().
+00003570: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003580: 2020 6966 2066 7261 6d65 735f 696e 7465    if frames_inte
+00003590: 6e73 6974 7920 6973 204e 6f6e 653a 0a20  nsity is None:. 
+000035a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000035b0: 6e0a 2020 2020 2020 2020 7661 6c75 6573  n.        values
+000035c0: 2c20 6269 6e73 203d 206e 756d 7079 2e68  , bins = numpy.h
+000035d0: 6973 746f 6772 616d 280a 2020 2020 2020  istogram(.      
+000035e0: 2020 2020 2020 6672 616d 6573 5f69 6e74        frames_int
+000035f0: 656e 7369 7479 2c20 7365 6c66 2e6e 6672  ensity, self.nfr
+00003600: 616d 6573 2069 6620 6269 6e73 2069 7320  ames if bins is 
+00003610: 4e6f 6e65 2065 6c73 6520 6269 6e73 0a20  None else bins. 
+00003620: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00003630: 2066 7261 6d65 735f 696e 7465 6e73 6974   frames_intensit
+00003640: 7920 3d20 6e75 6d70 792e 6173 616e 7961  y = numpy.asanya
+00003650: 7272 6179 2866 7261 6d65 735f 696e 7465  rray(frames_inte
+00003660: 6e73 6974 7929 0a20 2020 2020 2020 2069  nsity).        i
+00003670: 6620 746f 705f 6269 6e20 6973 204e 6f6e  f top_bin is Non
+00003680: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00003690: 6f70 5f62 696e 203d 206c 656e 2862 696e  op_bin = len(bin
+000036a0: 7329 202d 2031 0a20 2020 2020 2020 2069  s) - 1.        i
+000036b0: 6620 626f 7474 6f6d 5f62 696e 2069 7320  f bottom_bin is 
+000036c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000036d0: 2020 626f 7474 6f6d 5f62 696e 203d 2030    bottom_bin = 0
+000036e0: 0a0a 2020 2020 2020 2020 626f 7474 6f6d  ..        bottom
+000036f0: 5f74 6872 6573 686f 6c64 203d 2066 7261  _threshold = fra
+00003700: 6d65 735f 696e 7465 6e73 6974 7920 3e3d  mes_intensity >=
+00003710: 2062 696e 735b 626f 7474 6f6d 5f62 696e   bins[bottom_bin
+00003720: 5d0a 2020 2020 2020 2020 746f 705f 7468  ].        top_th
+00003730: 7265 7368 6f6c 6420 3d20 6672 616d 6573  reshold = frames
+00003740: 5f69 6e74 656e 7369 7479 203c 3d20 6269  _intensity <= bi
+00003750: 6e73 5b74 6f70 5f62 696e 5d0a 2020 2020  ns[top_bin].    
+00003760: 2020 2020 7468 7265 7368 6f6c 6420 3d20      threshold = 
+00003770: 6e75 6d70 792e 6172 7261 7928 0a20 2020  numpy.array(.   
+00003780: 2020 2020 2020 2020 205b 6120 616e 6420           [a and 
+00003790: 6220 666f 7220 612c 2062 2069 6e20 7a69  b for a, b in zi
+000037a0: 7028 626f 7474 6f6d 5f74 6872 6573 686f  p(bottom_thresho
+000037b0: 6c64 2c20 746f 705f 7468 7265 7368 6f6c  ld, top_threshol
+000037c0: 6429 5d0a 2020 2020 2020 2020 290a 2020  d)].        ).  
+000037d0: 2020 2020 2020 7265 7475 726e 206e 756d        return num
+000037e0: 7079 2e66 6c61 746e 6f6e 7a65 726f 2874  py.flatnonzero(t
+000037f0: 6872 6573 686f 6c64 292c 206e 756d 7079  hreshold), numpy
+00003800: 2e66 6c61 746e 6f6e 7a65 726f 287e 7468  .flatnonzero(~th
+00003810: 7265 7368 6f6c 6429 0a0a 2020 2020 4070  reshold)..    @p
+00003820: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00003830: 696e 5f6d 656d 6f72 7928 7365 6c66 293a  in_memory(self):
+00003840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003850: 7365 6c66 2e5f 696e 5f6d 656d 6f72 790a  self._in_memory.
+00003860: 0a20 2020 2040 696e 5f6d 656d 6f72 792e  .    @in_memory.
+00003870: 7365 7474 6572 0a20 2020 2064 6566 2069  setter.    def i
+00003880: 6e5f 6d65 6d6f 7279 2873 656c 662c 2069  n_memory(self, i
+00003890: 6e5f 6d65 6d6f 7279 293a 0a20 2020 2020  n_memory):.     
+000038a0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+000038b0: 656d 6f76 6573 2064 6174 6120 6672 6f6d  emoves data from
+000038c0: 206d 656d 6f72 7920 616e 6420 7365 7473   memory and sets
+000038d0: 2074 6861 7420 6672 6f6d 206e 6f77 206f   that from now o
+000038e0: 6e20 6461 7461 2077 696c 6c20 6265 2072  n data will be r
+000038f0: 6561 6420 6672 6f6d 2064 6973 6b2e 0a20  ead from disk.. 
+00003900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003910: 2020 2069 6620 7365 6c66 2e5f 696e 5f6d     if self._in_m
+00003920: 656d 6f72 7920 6973 206e 6f74 2069 6e5f  emory is not in_
+00003930: 6d65 6d6f 7279 3a0a 2020 2020 2020 2020  memory:.        
+00003940: 2020 2020 7365 6c66 2e5f 696e 5f6d 656d      self._in_mem
+00003950: 6f72 7920 3d20 696e 5f6d 656d 6f72 790a  ory = in_memory.
+00003960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003970: 2e5f 6461 7461 203d 2044 6174 6128 7365  ._data = Data(se
+00003980: 6c66 2e64 6174 612e 7572 6c73 2c20 7365  lf.data.urls, se
+00003990: 6c66 2e64 6174 612e 6d65 7461 6461 7461  lf.data.metadata
+000039a0: 2c20 7365 6c66 2e5f 696e 5f6d 656d 6f72  , self._in_memor
+000039b0: 7929 0a0a 2020 2020 4070 726f 7065 7274  y)..    @propert
+000039c0: 790a 2020 2020 6465 6620 6461 7461 2873  y.    def data(s
+000039d0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+000039e0: 7475 726e 2073 656c 662e 5f64 6174 610a  turn self._data.
+000039f0: 0a20 2020 2064 6566 2067 6574 5f64 6174  .    def get_dat
+00003a00: 6128 7365 6c66 2c20 696e 6469 6365 733d  a(self, indices=
+00003a10: 4e6f 6e65 2c20 6469 6d65 6e73 696f 6e3d  None, dimension=
+00003a20: 4e6f 6e65 2c20 7265 7475 726e 5f69 6e64  None, return_ind
+00003a30: 6963 6573 3d46 616c 7365 293a 0a20 2020  ices=False):.   
+00003a40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003a50: 2052 6574 7572 6e73 2074 6865 2064 6174   Returns the dat
+00003a60: 6120 636f 7272 6573 706f 6e64 696e 6720  a corresponding 
+00003a70: 746f 2063 6572 7461 696e 7320 696e 6469  to certains indi
+00003a80: 6365 7320 616e 6420 6769 7665 6e20 736f  ces and given so
+00003a90: 6d65 2064 696d 656e 7369 6f6e 7320 7661  me dimensions va
+00003aa0: 6c75 6573 2e0a 2020 2020 2020 2020 5468  lues..        Th
+00003ab0: 6520 6461 7461 2069 7320 616c 7761 7973  e data is always
+00003ac0: 2066 6c61 7474 656e 6564 2074 6f20 6265   flattened to be
+00003ad0: 2061 2073 7461 636b 206f 6620 696d 6167   a stack of imag
+00003ae0: 6573 2e0a 0a20 2020 2020 2020 203a 7061  es...        :pa
+00003af0: 7261 6d20 6172 7261 795f 6c69 6b65 2069  ram array_like i
+00003b00: 6e64 6963 6573 3a20 4966 206e 6f74 204e  ndices: If not N
+00003b10: 6f6e 652c 2064 6174 6120 6973 2066 696c  one, data is fil
+00003b20: 7465 7265 6420 7573 696e 6720 7468 6973  tered using this
+00003b30: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+00003b40: 3a70 6172 616d 2061 7272 6179 5f6c 696b  :param array_lik
+00003b50: 6520 6469 6d65 6e73 696f 6e3a 2049 6620  e dimension: If 
+00003b60: 6e6f 7420 4e6f 6e65 2c20 7265 7475 726e  not None, return
+00003b70: 206f 6e6c 7920 7468 6520 6461 7461 2063   only the data c
+00003b80: 6f72 7265 7370 6f6e 6469 6e67 2074 6f0a  orresponding to.
+00003b90: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00003ba0: 6769 7665 6e20 6469 6d65 6e73 696f 6e2e  given dimension.
+00003bb0: 2044 696d 656e 7369 6f6e 2069 7320 6120   Dimension is a 
+00003bc0: 3264 2076 6563 746f 722c 2077 6865 7265  2d vector, where
+00003bd0: 2074 6865 2066 6972 7374 2063 6f6d 706f   the first compo
+00003be0: 6e65 6e74 2069 730a 2020 2020 2020 2020  nent is.        
+00003bf0: 2020 2020 6120 6c69 7374 206f 6620 7468      a list of th
+00003c00: 6520 6178 6973 2061 6e64 2074 6865 2073  e axis and the s
+00003c10: 6563 6f6e 6420 6973 2061 206c 6973 7420  econd is a list 
+00003c20: 6f66 2074 6865 2069 6e64 6963 6573 206f  of the indices o
+00003c30: 6620 7468 6520 7661 6c75 6573 2074 6f20  f the values to 
+00003c40: 6578 7472 6163 742e 0a20 2020 2020 2020  extract..       
+00003c50: 2020 2020 2054 6865 2064 696d 656e 7369       The dimensi
+00003c60: 6f6e 2061 6e64 2076 616c 7565 206c 6973  on and value lis
+00003c70: 7420 6c65 6e67 7468 2063 616e 2062 6520  t length can be 
+00003c80: 7570 2074 6f20 7468 6520 6e75 6d62 6572  up to the number
+00003c90: 206f 6620 6469 6d65 6e73 696f 6e73 202d   of dimensions -
+00003ca0: 2031 2e0a 2020 2020 2020 2020 2020 2020   1..            
+00003cb0: 5468 6520 6361 6c6c 2067 6574 5f64 6174  The call get_dat
+00003cc0: 6128 6469 6d65 6e73 696f 6e3d 5b5b 312c  a(dimension=[[1,
+00003cd0: 2032 5d2c 205b 322c 2033 5d5d 2920 6973   2], [2, 3]]) is
+00003ce0: 2065 7175 6976 616c 656e 7420 746f 2064   equivalent to d
+00003cf0: 6174 615b 3a2c 2032 2c20 335d 2077 6865  ata[:, 2, 3] whe
+00003d00: 6e20 6461 7461 0a20 2020 2020 2020 2020  n data.         
+00003d10: 2020 2069 7320 696e 206d 656d 6f72 792e     is in memory.
+00003d20: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00003d30: 2061 7869 7320 6f66 2074 6865 2064 696d   axis of the dim
+00003d40: 656e 7369 6f6e 2069 7320 736f 2074 6861  ension is so tha
+00003d50: 7420 6c6f 7765 7220 7468 6520 6178 6973  t lower the axis
+00003d60: 2c20 6661 7374 6573 7420 7468 6520 6469  , fastest the di
+00003d70: 6d65 6e73 696f 6e20 2868 6967 6865 7220  mension (higher 
+00003d80: 6368 616e 6769 6e67 0a20 2020 2020 2020  changing.       
+00003d90: 2020 2020 2076 616c 7565 292e 0a0a 2020       value)...  
+00003da0: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
+00003db0: 7272 6179 2077 6974 6820 7468 6520 6e65  rray with the ne
+00003dc0: 7720 6461 7461 2e0a 2020 2020 2020 2020  w data..        
+00003dd0: 2222 220a 2020 2020 2020 2020 6966 2064  """.        if d
+00003de0: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
+00003df0: 4e6f 6e65 2061 6e64 206c 656e 2873 656c  None and len(sel
+00003e00: 662e 5f64 6174 612e 7368 6170 6529 203e  f._data.shape) >
+00003e10: 2033 3a0a 2020 2020 2020 2020 2020 2020   3:.            
+00003e20: 2320 4d61 6b65 2073 7572 6520 6469 6d65  # Make sure dime
+00003e30: 6e73 696f 6e20 616e 6420 7661 6c75 6520  nsion and value 
+00003e40: 6172 6520 6c69 7374 730a 2020 2020 2020  are lists.      
+00003e50: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00003e60: 6e63 6528 6469 6d65 6e73 696f 6e5b 305d  nce(dimension[0]
+00003e70: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+00003e80: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
+00003e90: 6e5b 305d 203d 205b 6469 6d65 6e73 696f  n[0] = [dimensio
+00003ea0: 6e5b 305d 5d0a 2020 2020 2020 2020 2020  n[0]].          
+00003eb0: 2020 2020 2020 6469 6d65 6e73 696f 6e5b        dimension[
+00003ec0: 315d 203d 205b 6469 6d65 6e73 696f 6e5b  1] = [dimension[
+00003ed0: 315d 5d0a 2020 2020 2020 2020 2020 2020  1]].            
+00003ee0: 6461 7461 203d 2073 656c 662e 6461 7461  data = self.data
+00003ef0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003f00: 496e 6974 206c 6973 7420 6f66 2062 6f6f  Init list of boo
+00003f10: 6c20 696e 6469 6365 730a 2020 2020 2020  l indices.      
+00003f20: 2020 2020 2020 626f 6f6c 5f69 6e64 6963        bool_indic
+00003f30: 6573 203d 206e 756d 7079 2e7a 6572 6f73  es = numpy.zeros
+00003f40: 2873 656c 662e 6461 7461 2e6e 6672 616d  (self.data.nfram
+00003f50: 6573 2c20 6474 7970 653d 626f 6f6c 290a  es, dtype=bool).
+00003f60: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00003f70: 6e64 6963 6573 2069 7320 4e6f 6e65 3a0a  ndices is None:.
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f90: 696e 6469 6365 7320 3d20 6e75 6d70 792e  indices = numpy.
+00003fa0: 6172 616e 6765 2873 656c 662e 6e66 7261  arange(self.nfra
+00003fb0: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
+00003fc0: 2062 6f6f 6c5f 696e 6469 6365 735b 696e   bool_indices[in
+00003fd0: 6469 6365 735d 203d 2054 7275 650a 2020  dices] = True.  
+00003fe0: 2020 2020 2020 2020 2020 626f 6f6c 5f69            bool_i
+00003ff0: 6e64 6963 6573 203d 2062 6f6f 6c5f 696e  ndices = bool_in
+00004000: 6469 6365 732e 7265 7368 6170 6528 7365  dices.reshape(se
+00004010: 6c66 2e64 6174 612e 7363 616e 5f73 6861  lf.data.scan_sha
+00004020: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+00004030: 696e 6478 203d 206e 756d 7079 2e61 7261  indx = numpy.ara
+00004040: 6e67 6528 7365 6c66 2e6e 6672 616d 6573  nge(self.nframes
+00004050: 292e 7265 7368 6170 6528 7365 6c66 2e64  ).reshape(self.d
+00004060: 6174 612e 7363 616e 5f73 6861 7065 290a  ata.scan_shape).
+00004070: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+00004080: 6f72 2065 7665 7279 2061 7869 732c 2067  or every axis, g
+00004090: 6574 2063 6f72 7265 7370 6f6e 6469 6e67  et corresponding
+000040a0: 2065 6c65 6d65 6e74 730a 2020 2020 2020   elements.      
+000040b0: 2020 2020 2020 666f 7220 692c 2064 696d        for i, dim
+000040c0: 2069 6e20 656e 756d 6572 6174 6528 736f   in enumerate(so
+000040d0: 7274 6564 2864 696d 656e 7369 6f6e 5b30  rted(dimension[0
+000040e0: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
+000040f0: 2020 2020 2023 2046 6c69 7020 6178 6973       # Flip axis
+00004100: 2074 6f20 6265 2063 6f6e 7369 7374 656e   to be consisten
+00004110: 7420 7769 7468 2074 6865 2064 6174 6120  t with the data 
+00004120: 7368 6170 650a 2020 2020 2020 2020 2020  shape.          
+00004130: 2020 2020 2020 6178 6973 203d 2073 656c        axis = sel
+00004140: 662e 6469 6d73 2e6e 6469 6d20 2d20 6469  f.dims.ndim - di
+00004150: 6d20 2d20 310a 2020 2020 2020 2020 2020  m - 1.          
+00004160: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00004170: 612e 7461 6b65 2869 6e64 6963 6573 3d64  a.take(indices=d
+00004180: 696d 656e 7369 6f6e 5b31 5d5b 695d 2c20  imension[1][i], 
+00004190: 6178 6973 3d61 7869 7329 0a20 2020 2020  axis=axis).     
+000041a0: 2020 2020 2020 2020 2020 2062 6f6f 6c5f             bool_
+000041b0: 696e 6469 6365 7320 3d20 626f 6f6c 5f69  indices = bool_i
+000041c0: 6e64 6963 6573 2e74 616b 6528 696e 6469  ndices.take(indi
+000041d0: 6365 733d 6469 6d65 6e73 696f 6e5b 315d  ces=dimension[1]
+000041e0: 5b69 5d2c 2061 7869 733d 6178 6973 290a  [i], axis=axis).
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 696e 6478 203d 2069 6e64 782e 7461 6b65  indx = indx.take
+00004210: 2869 6e64 6963 6573 3d64 696d 656e 7369  (indices=dimensi
+00004220: 6f6e 5b31 5d5b 695d 2c20 6178 6973 3d61  on[1][i], axis=a
+00004230: 7869 7329 0a0a 2020 2020 2020 2020 2020  xis)..          
+00004240: 2020 6461 7461 203d 2064 6174 615b 626f    data = data[bo
+00004250: 6f6c 5f69 6e64 6963 6573 5d0a 2020 2020  ol_indices].    
+00004260: 2020 2020 2020 2020 696e 6478 203d 2069          indx = i
+00004270: 6e64 785b 626f 6f6c 5f69 6e64 6963 6573  ndx[bool_indices
+00004280: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00004290: 2072 6574 7572 6e5f 696e 6469 6365 733a   return_indices:
+000042a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042b0: 2072 6574 7572 6e20 6461 7461 2e66 6c61   return data.fla
+000042c0: 7474 656e 2829 2c20 696e 6478 2e66 6c61  tten(), indx.fla
+000042d0: 7474 656e 2829 0a20 2020 2020 2020 2020  tten().         
+000042e0: 2020 2072 6574 7572 6e20 6461 7461 2e66     return data.f
+000042f0: 6c61 7474 656e 2829 0a0a 2020 2020 2020  latten()..      
+00004300: 2020 6461 7461 203d 2073 656c 662e 6461    data = self.da
+00004310: 7461 2e66 6c61 7474 656e 2829 0a20 2020  ta.flatten().   
+00004320: 2020 2020 2069 6620 7265 7475 726e 5f69       if return_i
+00004330: 6e64 6963 6573 3a0a 2020 2020 2020 2020  ndices:.        
+00004340: 2020 2020 6966 2069 6e64 6963 6573 2069      if indices i
+00004350: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00004360: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+00004370: 3d20 6e75 6d70 792e 6172 616e 6765 2873  = numpy.arange(s
+00004380: 656c 662e 6e66 7261 6d65 7329 0a20 2020  elf.nframes).   
+00004390: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000043a0: 6461 7461 5b69 6e64 6963 6573 5d2c 2069  data[indices], i
+000043b0: 6e64 6963 6573 0a20 2020 2020 2020 2069  ndices.        i
+000043c0: 6620 696e 6469 6365 7320 6973 204e 6f6e  f indices is Non
+000043d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000043e0: 6574 7572 6e20 6461 7461 0a20 2020 2020  eturn data.     
+000043f0: 2020 2072 6574 7572 6e20 6461 7461 5b69     return data[i
+00004400: 6e64 6963 6573 5d0a 0a20 2020 2040 7072  ndices]..    @pr
+00004410: 6f70 6572 7479 0a20 2020 2064 6566 206e  operty.    def n
+00004420: 6672 616d 6573 2873 656c 6629 3a0a 2020  frames(self):.  
+00004430: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004440: 2020 5265 7475 726e 206e 756d 6265 7220    Return number 
+00004450: 6f66 2066 7261 6d65 730a 2020 2020 2020  of frames.      
+00004460: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00004470: 2073 656c 662e 6461 7461 2069 7320 4e6f   self.data is No
+00004480: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004490: 7265 7475 726e 2030 0a20 2020 2020 2020  return 0.       
+000044a0: 2072 6574 7572 6e20 7365 6c66 2e64 6174   return self.dat
+000044b0: 612e 6e66 7261 6d65 730a 0a20 2020 2064  a.nframes..    d
+000044c0: 6566 2074 6f5f 6d65 6d6f 7279 2873 656c  ef to_memory(sel
+000044d0: 662c 2069 6e64 6963 6573 293a 0a20 2020  f, indices):.   
+000044e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000044f0: 204d 6574 686f 6420 746f 206c 6f61 6420   Method to load 
+00004500: 6f6e 6c79 2070 6172 7420 6f66 2074 6865  only part of the
+00004510: 2064 6174 6120 696e 746f 206d 656d 6f72   data into memor
+00004520: 792e 0a20 2020 2020 2020 2052 6574 7572  y..        Retur
+00004530: 6e73 2061 206e 6577 2064 6174 6173 6574  ns a new dataset
+00004540: 2077 6974 6820 7468 6520 6461 7461 2063   with the data c
+00004550: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
+00004560: 6769 7665 6e20 696e 6469 6365 7320 696e  given indices in
+00004570: 746f 206d 656d 6f72 792e 0a20 2020 2020  to memory..     
+00004580: 2020 2054 6865 206e 6577 2069 6e64 6963     The new indic
+00004590: 6573 2061 7272 6179 2068 6173 2074 6f20  es array has to 
+000045a0: 6265 2067 6976 656e 2c20 6966 2061 6c6c  be given, if all
+000045b0: 2074 6865 2064 6174 6120 6861 7320 746f   the data has to
+000045c0: 2062 6520 7365 7420 696e 746f 0a20 2020   be set into.   
+000045d0: 2020 2020 206d 656d 6f72 7920 706c 6561       memory plea
+000045e0: 7365 2073 6574 2060 696e 5f6d 656d 6f72  se set `in_memor
+000045f0: 7960 2074 6f20 5472 7565 2069 6e73 7465  y` to True inste
+00004600: 6164 2c20 7468 6973 2077 6179 206e 6f20  ad, this way no 
+00004610: 6e65 7720 6461 7461 7365 7420 7769 6c6c  new dataset will
+00004620: 2062 650a 2020 2020 2020 2020 6372 6561   be.        crea
+00004630: 7465 642e 0a0a 2020 2020 2020 2020 3a70  ted...        :p
+00004640: 6172 616d 2061 7272 6179 5f6c 696b 6520  aram array_like 
+00004650: 696e 6469 6365 733a 2049 6e64 6963 6573  indices: Indices
+00004660: 206f 6620 7468 6520 6e65 7720 6461 7461   of the new data
+00004670: 7365 742e 0a20 2020 2020 2020 2022 2222  set..        """
+00004680: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00004690: 7365 6c66 2e5f 696e 5f6d 656d 6f72 793a  self._in_memory:
+000046a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000046b0: 6120 3d20 7365 6c66 2e67 6574 5f64 6174  a = self.get_dat
+000046c0: 6128 696e 6469 6365 7329 0a20 2020 2020  a(indices).     
+000046d0: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
+000046e0: 3d20 4461 7461 2864 6174 612e 7572 6c73  = Data(data.urls
+000046f0: 2c20 6461 7461 2e6d 6574 6164 6174 612c  , data.metadata,
+00004700: 2054 7275 6529 0a20 2020 2020 2020 2065   True).        e
+00004710: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00004720: 206e 6577 5f64 6174 6120 3d20 7365 6c66   new_data = self
+00004730: 2e67 6574 5f64 6174 6128 696e 6469 6365  .get_data(indice
+00004740: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00004750: 6e20 4461 7461 7365 7428 0a20 2020 2020  n Dataset(.     
+00004760: 2020 2020 2020 205f 6469 723d 7365 6c66         _dir=self
+00004770: 2e5f 6469 722c 0a20 2020 2020 2020 2020  ._dir,.         
+00004780: 2020 2064 6174 613d 6e65 775f 6461 7461     data=new_data
+00004790: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000047a0: 6d73 3d73 656c 662e 5f5f 6469 6d73 2c0a  ms=self.__dims,.
+000047b0: 2020 2020 2020 2020 2020 2020 696e 5f6d              in_m
+000047c0: 656d 6f72 793d 5472 7565 2c0a 2020 2020  emory=True,.    
+000047d0: 2020 2020 2020 2020 7469 746c 653d 7365          title=se
+000047e0: 6c66 2e74 6974 6c65 2c0a 2020 2020 2020  lf.title,.      
+000047f0: 2020 290a 0a20 2020 2040 7072 6f70 6572    )..    @proper
+00004800: 7479 0a20 2020 2064 6566 2064 696d 7328  ty.    def dims(
+00004810: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00004820: 6574 7572 6e20 7365 6c66 2e5f 5f64 696d  eturn self.__dim
+00004830: 730a 0a20 2020 2040 6469 6d73 2e73 6574  s..    @dims.set
+00004840: 7465 720a 2020 2020 6465 6620 6469 6d73  ter.    def dims
+00004850: 2873 656c 662c 205f 6469 6d73 293a 0a20  (self, _dims):. 
+00004860: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+00004870: 696e 7374 616e 6365 285f 6469 6d73 2c20  instance(_dims, 
+00004880: 4163 7175 6973 6974 696f 6e44 696d 7329  AcquisitionDims)
+00004890: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
+000048a0: 2244 696d 656e 7369 6f6e 7320 6469 6374  "Dimensions dict
+000048b0: 696f 6e61 7279 2068 6173 2022 2022 746f  ionary has " "to
+000048c0: 2062 6520 6f66 2063 6c61 7373 2060 4163   be of class `Ac
+000048d0: 7175 6973 6974 696f 6e44 696d 7360 220a  quisitionDims`".
+000048e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000048f0: 2020 7365 6c66 2e5f 5f64 696d 7320 3d20    self.__dims = 
+00004900: 5f64 696d 730a 0a20 2020 2064 6566 2063  _dims..    def c
+00004910: 6c65 6172 5f64 696d 7328 7365 6c66 293a  lear_dims(self):
+00004920: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00004930: 6469 6d73 203d 2041 6371 7569 7369 7469  dims = Acquisiti
+00004940: 6f6e 4469 6d73 2829 0a0a 2020 2020 6465  onDims()..    de
+00004950: 6620 6164 645f 6469 6d28 7365 6c66 2c20  f add_dim(self, 
+00004960: 6178 6973 2c20 6469 6d29 3a0a 2020 2020  axis, dim):.    
+00004970: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004980: 4164 6473 2061 2064 696d 656e 7369 6f6e  Adds a dimension
+00004990: 2074 6f20 7468 6520 6469 6d65 6e73 696f   to the dimensio
+000049a0: 6e27 7320 6469 6374 696f 6e61 7279 2e0a  n's dictionary..
+000049b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000049c0: 696e 7420 6178 6973 3a20 6178 6973 206f  int axis: axis o
+000049d0: 6620 7468 6520 6469 6d65 6e73 696f 6e2e  f the dimension.
+000049e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000049f0: 6044 696d 656e 7369 6f6e 6020 6469 6d3a  `Dimension` dim:
+00004a00: 2064 696d 656e 7369 6f6e 2074 6f20 6265   dimension to be
+00004a10: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
+00004a20: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00004a30: 2e5f 5f64 696d 732e 6164 645f 6469 6d28  .__dims.add_dim(
+00004a40: 6178 6973 2c20 6469 6d29 0a0a 2020 2020  axis, dim)..    
+00004a50: 6465 6620 7265 6d6f 7665 5f64 696d 2873  def remove_dim(s
+00004a60: 656c 662c 2061 7869 7329 3a0a 2020 2020  elf, axis):.    
+00004a70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004a80: 5265 6d6f 7665 7320 6120 6469 6d65 6e73  Removes a dimens
+00004a90: 696f 6e20 6672 6f6d 2074 6865 2064 696d  ion from the dim
+00004aa0: 656e 7369 6f6e 2773 2064 6963 7469 6f6e  ension's diction
+00004ab0: 6172 792e 0a0a 2020 2020 2020 2020 3a70  ary...        :p
+00004ac0: 6172 616d 2069 6e74 2061 7869 733a 2061  aram int axis: a
+00004ad0: 7869 7320 6f66 2074 6865 2064 696d 656e  xis of the dimen
+00004ae0: 7369 6f6e 2e0a 2020 2020 2020 2020 2222  sion..        ""
+00004af0: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+00004b00: 5f64 696d 732e 7265 6d6f 7665 5f64 696d  _dims.remove_dim
+00004b10: 2861 7869 7329 0a0a 2020 2020 6465 6620  (axis)..    def 
+00004b20: 7a73 756d 2873 656c 662c 2069 6e64 6963  zsum(self, indic
+00004b30: 6573 3d4e 6f6e 652c 2064 696d 656e 7369  es=None, dimensi
+00004b40: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+00004b50: 2020 6461 7461 203d 2073 656c 662e 6765    data = self.ge
+00004b60: 745f 6461 7461 2869 6e64 6963 6573 2c20  t_data(indices, 
+00004b70: 6469 6d65 6e73 696f 6e29 0a20 2020 2020  dimension).     
+00004b80: 2020 2072 6574 7572 6e20 6461 7461 2e73     return data.s
+00004b90: 756d 2861 7869 733d 3029 0a0a 2020 2020  um(axis=0)..    
+00004ba0: 6465 6620 7265 7368 6170 655f 6461 7461  def reshape_data
+00004bb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004bc0: 2222 220a 2020 2020 2020 2020 4675 6e63  """.        Func
+00004bd0: 7469 6f6e 2074 6861 7420 7265 7368 6170  tion that reshap
+00004be0: 6573 2074 6865 2064 6174 6120 746f 2066  es the data to f
+00004bf0: 6974 2074 6865 2064 696d 656e 7369 6f6e  it the dimension
+00004c00: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00004c10: 2020 2020 2020 206e 6469 6d20 3d20 7365         ndim = se
+00004c20: 6c66 2e5f 5f64 696d 732e 6e64 696d 0a20  lf.__dims.ndim. 
+00004c30: 2020 2020 2020 2069 6620 6e64 696d 203d         if ndim =
+00004c40: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00004c50: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00004c60: 7228 224e 6f20 6469 6d65 6e73 696f 6e73  r("No dimensions
+00004c70: 2061 7265 206c 6973 7465 6422 290a 0a20   are listed").. 
+00004c80: 2020 2020 2020 2069 6620 6e64 696d 203d         if ndim =
+00004c90: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00004ca0: 206e 6672 616d 6573 5f65 7870 6563 7465   nframes_expecte
+00004cb0: 6420 3d20 7365 6c66 2e5f 5f64 696d 732e  d = self.__dims.
+00004cc0: 6765 7428 3029 2e73 697a 650a 2020 2020  get(0).size.    
+00004cd0: 2020 2020 2020 2020 6966 206e 6672 616d          if nfram
+00004ce0: 6573 5f65 7870 6563 7465 6420 213d 2073  es_expected != s
+00004cf0: 656c 662e 6e66 7261 6d65 733a 0a20 2020  elf.nframes:.   
+00004d00: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+00004d10: 656e 7369 6f6e 203d 2022 2022 2e6a 6f69  ension = " ".joi
+00004d20: 6e28 7365 6c66 2e5f 5f64 696d 732e 6765  n(self.__dims.ge
+00004d30: 745f 6e61 6d65 7328 2929 0a20 2020 2020  t_names()).     
+00004d40: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004d50: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2066 2244 696d 656e 7369 6f6e 207b 6469   f"Dimension {di
+00004d80: 6d65 6e73 696f 6e7d 2068 6173 207b 6e66  mension} has {nf
+00004d90: 7261 6d65 735f 6578 7065 6374 6564 7d20  rames_expected} 
+00004da0: 706f 696e 7473 2077 6869 6c65 2074 6865  points while the
+00004db0: 7265 2061 7265 207b 7365 6c66 2e6e 6672  re are {self.nfr
+00004dc0: 616d 6573 7d20 696d 6167 6573 2e20 5472  ames} images. Tr
+00004dd0: 7920 7573 696e 6720 6f74 6865 7220 746f  y using other to
+00004de0: 6c65 7261 6e63 6520 6f72 2073 7465 7020  lerance or step 
+00004df0: 7661 6c75 6573 2e22 0a20 2020 2020 2020  values.".       
+00004e00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00004e10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00004e20: 6c66 0a0a 2020 2020 2020 2020 6469 6d73  lf..        dims
+00004e30: 5f73 6861 7065 203d 2073 656c 662e 5f5f  _shape = self.__
+00004e40: 6469 6d73 2e73 6861 7065 0a20 2020 2020  dims.shape.     
+00004e50: 2020 206f 7267 5f64 6174 6120 3d20 7365     org_data = se
+00004e60: 6c66 2e67 6574 5f64 6174 6128 290a 2020  lf.get_data().  
+00004e70: 2020 2020 2020 6f72 675f 7368 6170 6520        org_shape 
+00004e80: 3d20 6f72 675f 6461 7461 2e73 6861 7065  = org_data.shape
+00004e90: 0a20 2020 2020 2020 2069 6d67 5f73 6861  .        img_sha
+00004ea0: 7065 203d 2028 6f72 675f 7368 6170 655b  pe = (org_shape[
+00004eb0: 2d32 5d2c 206f 7267 5f73 6861 7065 5b2d  -2], org_shape[-
+00004ec0: 315d 290a 2020 2020 2020 2020 6e65 775f  1]).        new_
+00004ed0: 7368 6170 6520 3d20 6469 6d73 5f73 6861  shape = dims_sha
+00004ee0: 7065 202b 2069 6d67 5f73 6861 7065 0a20  pe + img_shape. 
+00004ef0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00004f00: 2020 2020 2020 2020 6461 7461 203d 206f          data = o
+00004f10: 7267 5f64 6174 612e 7265 7368 6170 6528  rg_data.reshape(
+00004f20: 6e65 775f 7368 6170 6529 0a20 2020 2020  new_shape).     
+00004f30: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00004f40: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00004f50: 2064 696d 656e 7369 6f6e 7320 3d20 2220   dimensions = " 
+00004f60: 222e 6a6f 696e 2873 656c 662e 5f5f 6469  ".join(self.__di
+00004f70: 6d73 2e67 6574 5f6e 616d 6573 2829 290a  ms.get_names()).
+00004f80: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00004f90: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00004fb0: 4469 6d65 6e73 696f 6e73 207b 6469 6d65  Dimensions {dime
+00004fc0: 6e73 696f 6e73 7d20 6861 7665 207b 6469  nsions} have {di
+00004fd0: 6d73 5f73 6861 7065 7d20 706f 696e 7473  ms_shape} points
+00004fe0: 2077 6869 6c65 2074 6865 7265 2061 7265   while there are
+00004ff0: 207b 6f72 675f 7368 6170 655b 3a2d 325d   {org_shape[:-2]
+00005000: 7d20 696d 6167 6573 2e20 5472 7920 7573  } images. Try us
+00005010: 696e 6720 6f74 6865 7220 746f 6c65 7261  ing other tolera
+00005020: 6e63 6520 6f72 2073 7465 7020 7661 6c75  nce or step valu
+00005030: 6573 2e22 0a20 2020 2020 2020 2020 2020  es.".           
+00005040: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00005050: 726e 2044 6174 6173 6574 280a 2020 2020  rn Dataset(.    
+00005060: 2020 2020 2020 2020 5f64 6972 3d73 656c          _dir=sel
+00005070: 662e 6469 722c 0a20 2020 2020 2020 2020  f.dir,.         
+00005080: 2020 2064 6174 613d 6461 7461 2c0a 2020     data=data,.  
+00005090: 2020 2020 2020 2020 2020 6469 6d73 3d73            dims=s
+000050a0: 656c 662e 5f5f 6469 6d73 2c0a 2020 2020  elf.__dims,.    
+000050b0: 2020 2020 2020 2020 696e 5f6d 656d 6f72          in_memor
+000050c0: 793d 7365 6c66 2e5f 696e 5f6d 656d 6f72  y=self._in_memor
+000050d0: 792c 0a20 2020 2020 2020 2020 2020 2074  y,.            t
+000050e0: 6974 6c65 3d73 656c 662e 7469 746c 652c  itle=self.title,
+000050f0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00005100: 6465 6620 6669 6e64 5f64 696d 656e 7369  def find_dimensi
+00005110: 6f6e 7328 7365 6c66 2c20 6b69 6e64 2c20  ons(self, kind, 
+00005120: 746f 6c65 7261 6e63 653d 3165 2d39 2920  tolerance=1e-9) 
+00005130: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00005140: 2022 2222 0a20 2020 2020 2020 2047 6f65   """.        Goe
+00005150: 7320 6f76 6572 2061 6c6c 2074 6865 2068  s over all the h
+00005160: 6561 6465 7273 2066 726f 6d20 6120 6769  eaders from a gi
+00005170: 7665 6e20 6b69 6e64 2061 6e64 2066 696e  ven kind and fin
+00005180: 6473 2074 6865 2064 696d 656e 7369 6f6e  ds the dimension
+00005190: 730a 2020 2020 2020 2020 7468 6174 206d  s.        that m
+000051a0: 6f76 6520 2868 6176 6520 6d6f 7265 2074  ove (have more t
+000051b0: 6861 6e20 6f6e 6520 7661 6c75 6529 2061  han one value) a
+000051c0: 6c6f 6e67 2074 6865 2064 6174 612e 0a0a  long the data...
+000051d0: 2020 2020 2020 2020 4e6f 7465 3a20 4265          Note: Be
+000051e0: 666f 7265 2c20 6f6e 6c79 2074 6865 2064  fore, only the d
+000051f0: 696d 656e 7369 6f6e 7320 7468 6174 2063  imensions that c
+00005200: 6f75 6c64 2066 6974 2077 6865 7265 2073  ould fit where s
+00005210: 686f 776e 2c20 6e6f 7720 6974 0a20 2020  hown, now it.   
+00005220: 2020 2020 2073 686f 7773 2061 6c6c 2074       shows all t
+00005230: 6865 2064 696d 656e 7369 6f6e 7320 616e  he dimensions an
+00005240: 6420 6c65 7420 7468 6520 7573 6572 2063  d let the user c
+00005250: 686f 6f73 6520 7468 6520 7661 6c69 6420  hoose the valid 
+00005260: 6f6e 6573 2e0a 0a20 2020 2020 2020 203a  ones...        :
+00005270: 7061 7261 6d20 696e 7420 6b69 6e64 3a20  param int kind: 
+00005280: 5479 7065 206f 6620 6d65 7461 6461 7461  Type of metadata
+00005290: 2074 6f20 6669 6e64 2074 6865 2064 696d   to find the dim
+000052a0: 656e 7369 6f6e 732e 0a20 2020 2020 2020  ensions..       
+000052b0: 203a 7061 7261 6d20 666c 6f61 7420 746f   :param float to
+000052c0: 6c65 7261 6e63 653a 2054 6f6c 6572 616e  lerance: Toleran
+000052d0: 6365 2074 6861 7420 7769 6c6c 2062 6520  ce that will be 
+000052e0: 7573 6564 2074 6f20 636f 6d70 7574 6520  used to compute 
+000052f0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00005300: 756e 6971 7565 2076 616c 7565 732e 0a20  unique values.. 
+00005310: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005320: 2020 2073 656c 662e 5f5f 6469 6d73 2e63     self.__dims.c
+00005330: 6c65 6172 2829 0a20 2020 2020 2020 2073  lear().        s
+00005340: 656c 662e 5f64 696d 656e 7369 6f6e 735f  elf._dimensions_
+00005350: 7661 6c75 6573 203d 207b 7d0a 0a20 2020  values = {}..   
+00005360: 2020 2020 206b 6579 7320 3d20 6e75 6d70       keys = nump
+00005370: 792e 6172 7261 7928 6c69 7374 2873 656c  y.array(list(sel
+00005380: 662e 6461 7461 2e6d 6574 6164 6174 615b  f.data.metadata[
+00005390: 305d 2e67 6574 5f6b 6579 7328 6b69 6e64  0].get_keys(kind
+000053a0: 2929 290a 2020 2020 2020 2020 7661 6c75  ))).        valu
+000053b0: 6573 203d 206e 756d 7079 2e61 7361 7272  es = numpy.asarr
+000053c0: 6179 280a 2020 2020 2020 2020 2020 2020  ay(.            
+000053d0: 5b73 656c 662e 6765 745f 6d65 7461 6461  [self.get_metada
+000053e0: 7461 5f76 616c 7565 7328 6b69 6e64 3d6b  ta_values(kind=k
+000053f0: 696e 642c 206b 6579 3d6b 6579 2920 666f  ind, key=key) fo
+00005400: 7220 6b65 7920 696e 206b 6579 735d 0a20  r key in keys]. 
+00005410: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005420: 2023 2055 6e69 7175 6520 7661 6c75 6573   # Unique values
+00005430: 2066 6f72 2065 6163 6820 6b65 792e 0a20   for each key.. 
+00005440: 2020 2020 2020 2075 6e69 7175 655f 7661         unique_va
+00005450: 6c75 6573 203d 205b 0a20 2020 2020 2020  lues = [.       
+00005460: 2020 2020 206e 756d 7079 2e75 6e69 7175       numpy.uniqu
+00005470: 6528 7661 6c75 652c 2072 6574 7572 6e5f  e(value, return_
+00005480: 696e 6465 783d 5472 7565 2c20 7265 7475  index=True, retu
+00005490: 726e 5f63 6f75 6e74 733d 5472 7565 290a  rn_counts=True).
+000054a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000054b0: 7661 6c75 6520 696e 2076 616c 7565 730a  value in values.
+000054c0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000054d0: 2020 6469 6d65 6e73 696f 6e73 203d 205b    dimensions = [
+000054e0: 5d0a 2020 2020 2020 2020 6461 7461 7365  ].        datase
+000054f0: 745f 7369 7a65 203d 206c 656e 2873 656c  t_size = len(sel
+00005500: 662e 6461 7461 2e6d 6574 6164 6174 6129  f.data.metadata)
+00005510: 0a20 2020 2020 2020 2023 2046 6f72 2065  .        # For e
+00005520: 7665 7279 206b 6579 2074 6861 7420 6861  very key that ha
+00005530: 7320 6d6f 7265 2074 6861 6e20 6f6e 6520  s more than one 
+00005540: 6469 6666 6572 656e 7420 7661 6c75 652c  different value,
+00005550: 2063 7265 6174 6573 2061 206e 6577 2044   creates a new D
+00005560: 696d 656e 7369 6f6e 2e0a 2020 2020 2020  imension..      
+00005570: 2020 666f 7220 692c 2076 616c 7565 2069    for i, value i
+00005580: 6e20 656e 756d 6572 6174 6528 756e 6971  n enumerate(uniq
+00005590: 7565 5f76 616c 7565 7329 3a0a 2020 2020  ue_values):.    
+000055a0: 2020 2020 2020 2020 6966 2076 616c 7565          if value
+000055b0: 5b32 5d5b 305d 2021 3d20 6461 7461 7365  [2][0] != datase
+000055c0: 745f 7369 7a65 3a0a 2020 2020 2020 2020  t_size:.        
+000055d0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2064 696d 656e 7369 6f6e 203d 2044 696d   dimension = Dim
+00005600: 656e 7369 6f6e 286b 696e 642c 206b 6579  ension(kind, key
+00005610: 735b 695d 2c20 746f 6c65 7261 6e63 653d  s[i], tolerance=
+00005620: 746f 6c65 7261 6e63 6529 0a20 2020 2020  tolerance).     
+00005630: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005640: 696d 656e 7369 6f6e 2e73 6574 5f75 6e69  imension.set_uni
+00005650: 7175 655f 7661 6c75 6573 280a 2020 2020  que_values(.    
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 2020 2020 6e75 6d70 792e 6172 7261 7928      numpy.array(
+00005680: 7661 6c75 6573 5b69 5d5b 6e75 6d70 792e  values[i][numpy.
+00005690: 736f 7274 2876 616c 7565 5b31 5d29 5d2c  sort(value[1])],
+000056a0: 2064 7479 7065 3d66 6c6f 6174 290a 2020   dtype=float).  
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000056d0: 2020 2020 2020 2020 2320 5661 6c75 6520          # Value 
+000056e0: 7468 6174 2074 656c 6c73 2077 6865 6e20  that tells when 
+000056f0: 646f 6573 2074 6865 2063 6861 6e67 6520  does the change 
+00005700: 6f66 2076 616c 7565 206f 6363 7572 2e20  of value occur. 
+00005710: 4974 2069 7320 7573 6564 2074 6f20 6b6e  It is used to kn
+00005720: 6f77 2074 6865 206f 7264 6572 0a20 2020  ow the order.   
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2023 206f 6620 7468 6520 7265 7368 6170   # of the reshap
+00005750: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+00005760: 2020 2020 2020 2020 2064 696d 656e 7369           dimensi
+00005770: 6f6e 2e63 6861 6e67 696e 675f 7661 6c75  on.changing_valu
+00005780: 6520 3d20 7365 6c66 2e5f 5f63 6f6d 7075  e = self.__compu
+00005790: 7465 5f63 6861 6e67 696e 675f 7661 6c75  te_changing_valu
+000057a0: 6528 7661 6c75 6573 5b69 5d29 0a20 2020  e(values[i]).   
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2064 696d 656e 7369 6f6e 732e 6170 7065   dimensions.appe
+000057d0: 6e64 2864 696d 656e 7369 6f6e 290a 2020  nd(dimension).  
+000057e0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000057f0: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00005800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005810: 2020 2020 205f 6c6f 6767 6572 2e77 6172       _logger.war
+00005820: 6e69 6e67 2822 436f 756c 646e 2774 2063  ning("Couldn't c
+00005830: 6f6e 7665 7274 2074 6f20 666c 6f61 7422  onvert to float"
+00005840: 290a 0a20 2020 2020 2020 2066 6f72 2064  )..        for d
+00005850: 696d 656e 7369 6f6e 2069 6e20 736f 7274  imension in sort
+00005860: 6564 280a 2020 2020 2020 2020 2020 2020  ed(.            
+00005870: 6469 6d65 6e73 696f 6e73 2c20 6b65 793d  dimensions, key=
+00005880: 6c61 6d62 6461 2078 3a20 782e 6368 616e  lambda x: x.chan
+00005890: 6769 6e67 5f76 616c 7565 2c20 7265 7665  ging_value, reve
+000058a0: 7273 653d 5472 7565 0a20 2020 2020 2020  rse=True.       
+000058b0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000058c0: 7365 6c66 2e5f 5f64 696d 732e 6164 645f  self.__dims.add_
+000058d0: 6469 6d28 6178 6973 3d73 656c 662e 5f5f  dim(axis=self.__
+000058e0: 6469 6d73 2e6e 6469 6d2c 2064 696d 3d64  dims.ndim, dim=d
+000058f0: 696d 656e 7369 6f6e 290a 2020 2020 2020  imension).      
+00005900: 2020 2020 2020 5f6c 6f67 6765 722e 696e        _logger.in
+00005910: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+00005920: 2020 2020 2244 696d 656e 7369 6f6e 207b      "Dimension {
+00005930: 7d20 6f66 2073 697a 6520 7b7d 2068 6173  } of size {} has
+00005940: 2062 6565 6e20 6164 6465 6420 666f 7220   been added for 
+00005950: 7265 7368 6170 696e 6722 2e66 6f72 6d61  reshaping".forma
+00005960: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00005970: 2020 2020 2020 2064 696d 656e 7369 6f6e         dimension
+00005980: 2e6e 616d 652c 2064 696d 656e 7369 6f6e  .name, dimension
+00005990: 2e73 697a 650a 2020 2020 2020 2020 2020  .size.          
+000059a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000059b0: 2020 2020 290a 0a20 2020 2064 6566 2067      )..    def g
+000059c0: 6574 5f6d 6574 6164 6174 615f 7661 6c75  et_metadata_valu
+000059d0: 6573 280a 2020 2020 2020 2020 7365 6c66  es(.        self
+000059e0: 2c20 6b69 6e64 2c20 6b65 792c 2069 6e64  , kind, key, ind
+000059f0: 6963 6573 3d4e 6f6e 652c 2064 696d 656e  ices=None, dimen
+00005a00: 7369 6f6e 3d4e 6f6e 650a 2020 2020 2920  sion=None.    ) 
+00005a10: 2d3e 206e 756d 7079 2e6e 6461 7272 6179  -> numpy.ndarray
+00005a20: 3a0a 2020 2020 2020 2020 7661 6c75 6573  :.        values
+00005a30: 203d 205b 5d0a 2020 2020 2020 2020 6d69   = [].        mi
+00005a40: 7373 696e 675f 7661 6c75 6520 3d20 4661  ssing_value = Fa
+00005a50: 6c73 650a 2020 2020 2020 2020 666f 7220  lse.        for 
+00005a60: 6461 7461 2069 6e20 7365 6c66 2e67 6574  data in self.get
+00005a70: 5f64 6174 6128 696e 6469 6365 732c 2064  _data(indices, d
+00005a80: 696d 656e 7369 6f6e 292e 6d65 7461 6461  imension).metada
+00005a90: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+00005aa0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00005ab0: 2020 2020 2076 616c 7565 203d 2064 6174       value = dat
+00005ac0: 612e 6765 745f 7661 6c75 6528 6b69 6e64  a.get_value(kind
+00005ad0: 3d6b 696e 642c 206e 616d 653d 6b65 7929  =kind, name=key)
+00005ae0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00005af0: 6570 7420 4b65 7945 7272 6f72 3a0a 2020  ept KeyError:.  
+00005b00: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00005b10: 7373 696e 675f 7661 6c75 6520 3d20 5472  ssing_value = Tr
+00005b20: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00005b30: 2020 2069 6620 6c65 6e28 7661 6c75 6573     if len(values
+00005b40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005b50: 2020 2020 2020 2076 616c 7565 732e 6170         values.ap
+00005b60: 7065 6e64 2876 616c 7565 735b 2d31 5d29  pend(values[-1])
+00005b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005b90: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00005ba0: 732e 6170 7065 6e64 286e 756d 7079 2e6e  s.append(numpy.n
+00005bb0: 616e 290a 2020 2020 2020 2020 2020 2020  an).            
+00005bc0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00005bd0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+00005be0: 6e73 7461 6e63 6528 6461 7461 2c20 5f48  nstance(data, _H
+00005bf0: 4446 354d 6574 6164 6174 6152 6561 6465  DF5MetadataReade
+00005c00: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00005c10: 2020 2020 2020 2020 2320 5f48 4446 354d          # _HDF5M
+00005c20: 6574 6164 6174 6152 6561 6465 7220 616c  etadataReader al
+00005c30: 7265 6164 7920 7265 7475 726e 2061 2073  ready return a s
+00005c40: 6361 6c61 7220 7768 656e 2073 696c 7820  calar when silx 
+00005c50: 4661 6269 6f52 6561 6465 7220 7265 7475  FabioReader retu
+00005c60: 726e 2061 6e20 6172 7261 7920 6f66 2061  rn an array of a
+00005c70: 2073 696e 676c 6520 656c 656d 656e 740a   single element.
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 2020 2020 7661 6c75 6520 3d20 7661 6c75      value = valu
+00005ca0: 655b 305d 0a20 2020 2020 2020 2020 2020  e[0].           
+00005cb0: 2020 2020 2076 616c 7565 732e 6170 7065       values.appe
+00005cc0: 6e64 2876 616c 7565 290a 0a20 2020 2020  nd(value)..     
+00005cd0: 2020 2069 6620 6d69 7373 696e 675f 7661     if missing_va
+00005ce0: 6c75 6520 6f72 2054 7275 653a 0a20 2020  lue or True:.   
+00005cf0: 2020 2020 2020 2020 205f 6c6f 6767 6572           _logger
+00005d00: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+00005d10: 2020 2020 2020 2020 2020 224d 6973 7369            "Missi
+00005d20: 6e67 2076 616c 7565 2873 2920 6669 6c6c  ng value(s) fill
+00005d30: 6564 2074 6f20 7072 6576 696f 7573 2076  ed to previous v
+00005d40: 616c 7565 2066 6f72 206b 696e 6420 2725  alue for kind '%
+00005d50: 7327 2061 6e64 206b 6579 2027 2573 2722  s' and key '%s'"
+00005d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005d70: 2020 6b69 6e64 2c0a 2020 2020 2020 2020    kind,.        
+00005d80: 2020 2020 2020 2020 6b65 792c 0a20 2020          key,.   
+00005d90: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00005da0: 2020 2020 7265 7475 726e 206e 756d 7079      return numpy
+00005db0: 2e61 7361 7272 6179 2876 616c 7565 7329  .asarray(values)
+00005dc0: 2020 2320 6d61 6b65 7320 7375 7265 2074    # makes sure t
+00005dd0: 6865 7920 616c 6c20 6861 7665 2074 6865  hey all have the
+00005de0: 2073 616d 6520 6474 7970 650a 0a20 2020   same dtype..   
+00005df0: 2064 6566 205f 5f63 6f6d 7075 7465 5f63   def __compute_c
+00005e00: 6861 6e67 696e 675f 7661 6c75 6528 7365  hanging_value(se
+00005e10: 6c66 2c20 7661 6c75 6573 2c20 6368 616e  lf, values, chan
+00005e20: 6769 6e67 5f76 616c 7565 3d31 293a 0a20  ging_value=1):. 
+00005e30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005e40: 2020 2052 6563 7572 7369 7665 206d 6574     Recursive met
+00005e50: 686f 6420 7573 6564 2074 6f20 6361 6c63  hod used to calc
+00005e60: 756c 6174 6520 686f 7720 6661 7374 2069  ulate how fast i
+00005e70: 7320 6120 6469 6d65 6e73 696f 6e2e 2054  s a dimension. T
+00005e80: 6865 2073 7065 6564 206f 6620 6120 6469  he speed of a di
+00005e90: 6d65 6e73 696f 6e20 6973 2074 6865 206e  mension is the n
+00005ea0: 756d 6265 7220 6f66 0a20 2020 2020 2020  umber of.       
+00005eb0: 2074 696d 6573 2074 6865 2064 696d 656e   times the dimen
+00005ec0: 7369 6f6e 2063 6861 6e67 6573 206f 6620  sion changes of 
+00005ed0: 7661 6c75 6520 7768 696c 6520 6d6f 7669  value while movi
+00005ee0: 6e67 2074 6872 6f75 6768 2074 6865 2064  ng through the d
+00005ef0: 6174 6173 6574 2e0a 2020 2020 2020 2020  ataset..        
+00005f00: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
+00005f10: 656e 286e 756d 7079 2e75 6e69 7175 6528  en(numpy.unique(
+00005f20: 7661 6c75 6573 2929 203e 2031 3a0a 2020  values)) > 1:.  
+00005f30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00005f40: 2073 656c 662e 5f5f 636f 6d70 7574 655f   self.__compute_
+00005f50: 6368 616e 6769 6e67 5f76 616c 7565 280a  changing_value(.
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 7661 6c75 6573 5b3a 2069 6e74 286c 656e  values[: int(len
+00005f80: 2876 616c 7565 7329 202f 2032 295d 2c20  (values) / 2)], 
+00005f90: 6368 616e 6769 6e67 5f76 616c 7565 202b  changing_value +
+00005fa0: 2031 0a20 2020 2020 2020 2020 2020 2029   1.            )
+00005fb0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00005fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00005fd0: 6e20 6368 616e 6769 6e67 5f76 616c 7565  n changing_value
+00005fe0: 0a0a 2020 2020 6465 6620 6765 745f 6469  ..    def get_di
+00005ff0: 6d65 6e73 696f 6e73 5f76 616c 7565 7328  mensions_values(
+00006000: 7365 6c66 2c20 696e 6469 6365 733d 4e6f  self, indices=No
+00006010: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
+00006020: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00006030: 2061 6c6c 2074 6865 206d 6574 6164 6174   all the metadat
+00006040: 6120 7661 6c75 6573 206f 6620 7468 6520  a values of the 
+00006050: 6469 6d65 6e73 696f 6e73 2e0a 2020 2020  dimensions..    
+00006060: 2020 2020 5468 6520 7661 6c75 6573 2061      The values a
+00006070: 7265 2061 7373 756d 6564 2074 6f20 6265  re assumed to be
+00006080: 206e 756d 6265 7273 2e0a 0a20 2020 2020   numbers...     
+00006090: 2020 203a 7265 7475 726e 733a 2061 7272     :returns: arr
+000060a0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+000060b0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+000060c0: 6f74 2073 656c 662e 5f64 696d 656e 7369  ot self._dimensi
+000060d0: 6f6e 735f 7661 6c75 6573 206f 7220 696e  ons_values or in
+000060e0: 6469 6365 7320 6973 206e 6f74 204e 6f6e  dices is not Non
+000060f0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00006100: 6f72 2064 696d 656e 7369 6f6e 2069 6e20  or dimension in 
+00006110: 7365 6c66 2e5f 5f64 696d 733a 0a20 2020  self.__dims:.   
+00006120: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006130: 662e 5f64 696d 656e 7369 6f6e 735f 7661  f._dimensions_va
+00006140: 6c75 6573 5b64 696d 656e 7369 6f6e 5b31  lues[dimension[1
+00006150: 5d2e 6e61 6d65 5d20 3d20 7365 6c66 2e67  ].name] = self.g
+00006160: 6574 5f6d 6574 6164 6174 615f 7661 6c75  et_metadata_valu
+00006170: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00006180: 2020 2020 2020 2020 6b69 6e64 3d64 696d          kind=dim
+00006190: 656e 7369 6f6e 5b31 5d2e 6b69 6e64 2c20  ension[1].kind, 
+000061a0: 6b65 793d 6469 6d65 6e73 696f 6e5b 315d  key=dimension[1]
+000061b0: 2e6e 616d 652c 2069 6e64 6963 6573 3d69  .name, indices=i
+000061c0: 6e64 6963 6573 0a20 2020 2020 2020 2020  ndices.         
+000061d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000061e0: 2072 6574 7572 6e20 7365 6c66 2e5f 6469   return self._di
+000061f0: 6d65 6e73 696f 6e73 5f76 616c 7565 730a  mensions_values.
+00006200: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
+00006210: 5f6d 6f73 6169 6369 7479 5f63 6f6c 6f72  _mosaicity_color
+00006220: 6b65 7928 0a20 2020 2020 2020 2073 656c  key(.        sel
+00006230: 662c 2064 696d 656e 7369 6f6e 733d 5b30  f, dimensions=[0
+00006240: 2c20 315d 2c20 7363 616c 653d 3130 302c  , 1], scale=100,
+00006250: 2069 6e64 6963 6573 3d4e 6f6e 652c 2074   indices=None, t
+00006260: 6869 7264 5f6d 6f74 6f72 3d4e 6f6e 650a  hird_motor=None.
+00006270: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00006280: 2222 0a20 2020 2020 2020 2043 6f6d 7075  "".        Compu
+00006290: 7465 7320 6120 6d6f 7361 6963 6974 7920  tes a mosaicity 
+000062a0: 636f 6c6f 726b 6579 2066 726f 6d20 7468  colorkey from th
+000062b0: 6520 6469 6d65 6e73 696f 6e73 2c20 616e  e dimensions, an
+000062c0: 6420 7265 7475 726e 7320 616c 736f 2074  d returns also t
+000062d0: 6865 0a20 2020 2020 2020 206f 7269 656e  he.        orien
+000062e0: 7461 7469 6f6e 2064 6973 7472 6962 7574  tation distribut
+000062f0: 696f 6e20 696d 6167 652e 0a20 2020 2020  ion image..     
+00006300: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+00006310: 206f 6e6c 7920 776f 726b 2077 6974 6820   only work with 
+00006320: 3220 6469 6d65 6e73 696f 6e73 0a20 2020  2 dimensions.   
+00006330: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+00006340: 6469 6d65 6e73 696f 6e73 2920 3d3d 2032  dimensions) == 2
+00006350: 2c20 224f 6e6c 7920 776f 726b 7320 7769  , "Only works wi
+00006360: 7468 2074 776f 206d 6f74 6f72 7322 0a20  th two motors". 
+00006370: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00006380: 5f64 696d 7320 616e 6420 7365 6c66 2e5f  _dims and self._
+00006390: 5f64 696d 732e 6e64 696d 203e 2031 3a0a  _dims.ndim > 1:.
+000063a0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+000063b0: 7368 6170 6520 3d20 5b5d 0a20 2020 2020  shape = [].     
+000063c0: 2020 2020 2020 2064 696d 735f 6c69 7374         dims_list
+000063d0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+000063e0: 2020 666f 7220 6178 6973 2069 6e20 6469    for axis in di
+000063f0: 6d65 6e73 696f 6e73 3a0a 2020 2020 2020  mensions:.      
+00006400: 2020 2020 2020 2020 2020 6469 6d20 3d20            dim = 
+00006410: 7365 6c66 2e5f 5f64 696d 732e 6765 7428  self.__dims.get(
+00006420: 6178 6973 290a 2020 2020 2020 2020 2020  axis).          
+00006430: 2020 2020 2020 6469 6d73 5f6c 6973 7420        dims_list 
+00006440: 2b3d 205b 6e75 6d70 792e 6c69 6e73 7061  += [numpy.linspa
+00006450: 6365 282d 312c 2031 2c20 6469 6d2e 7369  ce(-1, 1, dim.si
+00006460: 7a65 202a 2073 6361 6c65 295d 0a20 2020  ze * scale)].   
+00006470: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00006480: 5f73 6861 7065 202b 3d20 5b64 696d 2e73  _shape += [dim.s
+00006490: 697a 655d 0a20 2020 2020 2020 2020 2020  ize].           
+000064a0: 2064 696d 735f 6c69 7374 2e72 6576 6572   dims_list.rever
+000064b0: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
+000064c0: 206d 6573 6820 3d20 6e75 6d70 792e 6d65   mesh = numpy.me
+000064d0: 7368 6772 6964 282a 6469 6d73 5f6c 6973  shgrid(*dims_lis
+000064e0: 7429 0a20 2020 2020 2020 2020 2020 2064  t).            d
+000064f0: 6174 6120 3d20 6e75 6d70 792e 6172 6374  ata = numpy.arct
+00006500: 616e 3228 6d65 7368 5b30 5d2c 206d 6573  an2(mesh[0], mes
+00006510: 685b 315d 290a 2020 2020 2020 2020 2020  h[1]).          
+00006520: 2020 6e6f 726d 616c 697a 6564 5f64 6174    normalized_dat
+00006530: 6120 3d20 7772 6170 546f 3270 6928 6461  a = wrapTo2pi(da
+00006540: 7461 2920 2f20 6e75 6d70 792e 7069 202f  ta) / numpy.pi /
+00006550: 2032 0a20 2020 2020 2020 2020 2020 2073   2.            s
+00006560: 7172 203d 206e 756d 7079 2e73 7172 7428  qr = numpy.sqrt(
+00006570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006580: 206e 756d 7079 2e70 6f77 6572 286d 6573   numpy.power(mes
+00006590: 685b 305d 2c20 3229 202b 206e 756d 7079  h[0], 2) + numpy
+000065a0: 2e70 6f77 6572 286d 6573 685b 315d 2c20  .power(mesh[1], 
+000065b0: 3229 0a20 2020 2020 2020 2020 2020 2029  2).            )
+000065c0: 202f 206e 756d 7079 2e73 7172 7428 3229   / numpy.sqrt(2)
+000065d0: 0a20 2020 2020 2020 2020 2020 2068 7376  .            hsv
+000065e0: 5f6b 6579 203d 206e 756d 7079 2e73 7461  _key = numpy.sta
+000065f0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+00006600: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00006610: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
+00006620: 697a 6564 5f64 6174 612c 0a20 2020 2020  ized_data,.     
+00006630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006640: 7172 2c0a 2020 2020 2020 2020 2020 2020  qr,.            
+00006650: 2020 2020 2020 2020 6e75 6d70 792e 6f6e          numpy.on
+00006660: 6573 2828 6c65 6e28 6469 6d73 5f6c 6973  es((len(dims_lis
+00006670: 745b 315d 292c 206c 656e 2864 696d 735f  t[1]), len(dims_
+00006680: 6c69 7374 5b30 5d29 2929 2c0a 2020 2020  list[0]))),.    
+00006690: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000066b0: 7869 733d 322c 0a20 2020 2020 2020 2020  xis=2,.         
+000066c0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+000066d0: 2020 6f72 695f 6469 7374 203d 206e 756d    ori_dist = num
+000066e0: 7079 2e7a 6572 6f73 286e 6577 5f73 6861  py.zeros(new_sha
+000066f0: 7065 5b30 5d20 2a20 6e65 775f 7368 6170  pe[0] * new_shap
+00006700: 655b 315d 290a 2020 2020 2020 2020 2020  e[1]).          
+00006710: 2020 5f73 6c69 6365 3120 3d20 6f72 695f    _slice1 = ori_
+00006720: 6469 7374 2e73 6861 7065 5b30 5d20 2a20  dist.shape[0] * 
+00006730: 7468 6972 645f 6d6f 746f 720a 2020 2020  third_motor.    
+00006740: 2020 2020 2020 2020 5f73 6c69 6365 3220          _slice2 
+00006750: 3d20 6f72 695f 6469 7374 2e73 6861 7065  = ori_dist.shape
+00006760: 5b30 5d20 2a20 2874 6869 7264 5f6d 6f74  [0] * (third_mot
+00006770: 6f72 202b 2031 290a 2020 2020 2020 2020  or + 1).        
+00006780: 2020 2020 6f72 695f 6469 7374 5b69 6e64      ori_dist[ind
+00006790: 6963 6573 5d20 3d20 7365 6c66 2e67 6574  ices] = self.get
+000067a0: 5f64 6174 6128 696e 6469 6365 7329 2e73  _data(indices).s
+000067b0: 756d 2861 7869 733d 3129 5b5f 736c 6963  um(axis=1)[_slic
+000067c0: 6531 3a5f 736c 6963 6532 5d0a 2020 2020  e1:_slice2].    
+000067d0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+000067e0: 7269 5f64 6973 742e 7265 7368 6170 6528  ri_dist.reshape(
+000067f0: 6e75 6d70 792e 666c 6970 286e 6577 5f73  numpy.flip(new_s
+00006800: 6861 7065 2929 2e54 2c20 6873 765f 6b65  hape)).T, hsv_ke
+00006810: 790a 2020 2020 2020 2020 7265 7475 726e  y.        return
+00006820: 204e 6f6e 652c 204e 6f6e 650a 0a20 2020   None, None..   
+00006830: 2064 6566 2061 7070 6c79 5f62 6163 6b67   def apply_backg
+00006840: 726f 756e 645f 7375 6274 7261 6374 696f  round_subtractio
+00006850: 6e28 0a20 2020 2020 2020 2073 656c 662c  n(.        self,
+00006860: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
+00006870: 756e 643d 4e6f 6e65 2c0a 2020 2020 2020  und=None,.      
+00006880: 2020 6d65 7468 6f64 3d22 6d65 6469 616e    method="median
+00006890: 222c 0a20 2020 2020 2020 2069 6e64 6963  ",.        indic
+000068a0: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
+000068b0: 2073 7465 703d 4e6f 6e65 2c0a 2020 2020   step=None,.    
+000068c0: 2020 2020 6368 756e 6b5f 7368 6170 653d      chunk_shape=
+000068d0: 5b31 3030 2c20 3130 305d 2c0a 2020 2020  [100, 100],.    
+000068e0: 2020 2020 5f64 6972 3d4e 6f6e 652c 0a20      _dir=None,. 
+000068f0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00006900: 220a 2020 2020 2020 2020 4170 706c 6965  ".        Applie
+00006910: 7320 6261 636b 6772 6f75 6e64 2073 7562  s background sub
+00006920: 7472 6163 7469 6f6e 2074 6f20 7468 6520  traction to the 
+00006930: 6461 7461 2061 6e64 2073 6176 6573 2074  data and saves t
+00006940: 6865 206e 6577 2064 6174 610a 2020 2020  he new data.    
+00006950: 2020 2020 696e 746f 2064 6973 6b2e 0a0a      into disk...
+00006960: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+00006970: 6163 6b67 726f 756e 643a 2044 6174 6120  ackground: Data 
+00006980: 746f 2062 6520 7573 6564 2061 7320 6261  to be used as ba
+00006990: 636b 6772 6f75 6e64 2e20 4966 204e 6f6e  ckground. If Non
+000069a0: 652c 2064 6174 6120 7769 7468 2069 6e64  e, data with ind
+000069b0: 6963 6573 2060 696e 6469 6365 7360 2069  ices `indices` i
+000069c0: 7320 7573 6564 2e0a 2020 2020 2020 2020  s used..        
+000069d0: 2020 2020 4966 2044 6174 6173 6574 2c20      If Dataset, 
+000069e0: 6461 7461 206f 6620 7468 6520 6461 7461  data of the data
+000069f0: 7365 7420 6973 2075 7365 642e 2049 6620  set is used. If 
+00006a00: 6172 7261 792c 2075 7365 2064 6174 6120  array, use data 
+00006a10: 7769 7468 2069 6e64 6963 6573 2069 6e20  with indices in 
+00006a20: 7468 6520 6172 7261 792e 0a20 2020 2020  the array..     
+00006a30: 2020 203a 7479 7065 2062 6163 6b67 726f     :type backgro
+00006a40: 756e 643a 2055 6e69 6f6e 5b4e 6f6e 652c  und: Union[None,
+00006a50: 2061 7272 6179 5f6c 696b 652c 2044 6174   array_like, Dat
+00006a60: 6173 6574 5d0a 2020 2020 2020 2020 3a70  aset].        :p
+00006a70: 6172 616d 206d 6574 686f 643a 204d 6574  aram method: Met
+00006a80: 686f 6420 746f 2075 7365 2074 6f20 636f  hod to use to co
+00006a90: 6d70 7574 6520 7468 6520 6261 636b 6772  mpute the backgr
+00006aa0: 6f75 6e64 2e0a 2020 2020 2020 2020 3a74  ound..        :t
+00006ab0: 7970 6520 6d65 7468 6f64 3a20 4d65 7468  ype method: Meth
+00006ac0: 6f64 0a20 2020 2020 2020 203a 7061 7261  od.        :para
+00006ad0: 6d20 696e 6469 6365 733a 2049 6e64 6963  m indices: Indic
+00006ae0: 6573 206f 6620 7468 6520 696d 6167 6573  es of the images
+00006af0: 2074 6f20 6170 706c 7920 6261 636b 6772   to apply backgr
+00006b00: 6f75 6e64 2073 7562 7472 6163 7469 6f6e  ound subtraction
+00006b10: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00006b20: 204e 6f6e 652c 2074 6865 2062 6163 6b67   None, the backg
+00006b30: 726f 756e 6420 7375 6274 7261 6374 696f  round subtractio
+00006b40: 6e20 6973 2061 7070 6c69 6564 2074 6f20  n is applied to 
+00006b50: 616c 6c20 7468 6520 6461 7461 2e0a 2020  all the data..  
+00006b60: 2020 2020 2020 3a74 7970 6520 696e 6469        :type indi
+00006b70: 6365 733a 2055 6e69 6f6e 5b4e 6f6e 652c  ces: Union[None,
+00006b80: 2061 7272 6179 5f6c 696b 655d 0a20 2020   array_like].   
+00006b90: 2020 2020 203a 7061 7261 6d20 696e 7420       :param int 
+00006ba0: 7374 6570 3a20 4469 7374 616e 6365 2062  step: Distance b
+00006bb0: 6574 7765 656e 2069 6d61 6765 7320 746f  etween images to
+00006bc0: 2062 6520 7573 6564 2077 6865 6e20 636f   be used when co
+00006bd0: 6d70 7574 696e 6720 7468 6520 6d65 6469  mputing the medi
+00006be0: 616e 2e0a 2020 2020 2020 2020 2020 2020  an..            
+00006bf0: 5061 7261 6d65 7465 7220 7573 6564 206f  Parameter used o
+00006c00: 6e6c 7920 7768 656e 2066 6c61 6720 696e  nly when flag in
+00006c10: 5f6d 656d 6f72 7920 6973 2046 616c 7365  _memory is False
+00006c20: 2061 6e64 206d 6574 686f 6420 6973 2060   and method is `
+00006c30: 4d65 7468 6f64 2e6d 6564 6961 6e60 2e0a  Method.median`..
+00006c40: 2020 2020 2020 2020 2020 2020 4966 2060              If `
+00006c50: 7374 6570 6020 6973 206e 6f74 204e 6f6e  step` is not Non
+00006c60: 652c 2061 6c6c 2069 6d61 6765 7320 7769  e, all images wi
+00006c70: 7468 2064 6973 7461 6e63 6520 6f66 2060  th distance of `
+00006c80: 7374 6570 602c 2073 7461 7274 696e 6720  step`, starting 
+00006c90: 6174 2030 2c0a 2020 2020 2020 2020 2020  at 0,.          
+00006ca0: 2020 7769 6c6c 2062 6520 6c6f 6164 6564    will be loaded
+00006cb0: 2069 6e74 6f20 6d65 6d6f 7279 2066 6f72   into memory for
+00006cc0: 2063 6f6d 7075 7469 6e67 2074 6865 206d   computing the m
+00006cd0: 6564 6961 6e2c 2069 6620 7468 6520 6461  edian, if the da
+00006ce0: 7461 206c 6f61 6469 6e67 2074 6872 6f77  ta loading throw
+00006cf0: 730a 2020 2020 2020 2020 2020 2020 6120  s.            a 
+00006d00: 4d65 6d6f 7279 4572 726f 722c 2074 6865  MemoryError, the
+00006d10: 206d 6564 6961 6e20 636f 6d70 7574 6174   median computat
+00006d20: 696f 6e20 6973 2074 7269 6564 2077 6974  ion is tried wit
+00006d30: 6820 6073 7465 7020 2b3d 2031 602e 0a20  h `step += 1`.. 
+00006d40: 2020 2020 2020 203a 7061 7261 6d20 6368         :param ch
+00006d50: 756e 6b5f 7368 6170 653a 2053 6861 7065  unk_shape: Shape
+00006d60: 206f 6620 7468 6520 6368 756e 6b20 696d   of the chunk im
+00006d70: 6167 6520 746f 2075 7365 2070 6572 2069  age to use per i
+00006d80: 7465 7261 7469 6f6e 2e0a 2020 2020 2020  teration..      
+00006d90: 2020 2020 2020 5061 7261 6d65 7465 7220        Parameter 
+00006da0: 7573 6564 206f 6e6c 7920 7768 656e 2066  used only when f
+00006db0: 6c61 6720 696e 5f6d 656d 6f72 7920 6973  lag in_memory is
+00006dc0: 2046 616c 7365 2061 6e64 206d 6574 686f   False and metho
+00006dd0: 6420 6973 2060 4d65 7468 6f64 2e6d 6564  d is `Method.med
+00006de0: 6961 6e60 2e0a 2020 2020 2020 2020 3a74  ian`..        :t
+00006df0: 7970 6520 6368 756e 6b5f 7368 6170 653a  ype chunk_shape:
+00006e00: 2061 7272 6179 5f6c 696b 650a 2020 2020   array_like.    
+00006e10: 2020 2020 3a72 6574 7572 6e73 3a20 6461      :returns: da
+00006e20: 7461 7365 7420 7769 7468 2064 6174 6120  taset with data 
+00006e30: 6f66 2073 616d 6520 7369 7a65 2061 7320  of same size as 
+00006e40: 6073 656c 662e 6461 7461 6020 6275 7420  `self.data` but 
+00006e50: 7769 7468 2074 6865 0a20 2020 2020 2020  with the.       
+00006e60: 2020 2020 206d 6f64 6966 6965 6420 696d       modified im
+00006e70: 6167 6573 2e20 5468 6520 7572 6c73 206f  ages. The urls o
+00006e80: 6620 7468 6520 6d6f 6469 6669 6564 2069  f the modified i
+00006e90: 6d61 6765 7320 6172 6520 7265 706c 6163  mages are replac
+00006ea0: 6564 2077 6974 680a 2020 2020 2020 2020  ed with.        
+00006eb0: 2020 2020 7468 6520 6e65 7720 7572 6c73      the new urls
+00006ec0: 2e0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00006ed0: 3a20 4461 7461 7365 740a 2020 2020 2020  : Dataset.      
+00006ee0: 2020 2222 220a 0a20 2020 2020 2020 205f    """..        _
+00006ef0: 6469 7220 3d20 7365 6c66 2e64 6972 2069  dir = self.dir i
+00006f00: 6620 5f64 6972 2069 7320 4e6f 6e65 2065  f _dir is None e
+00006f10: 6c73 6520 5f64 6972 0a0a 2020 2020 2020  lse _dir..      
+00006f20: 2020 6f73 2e6d 616b 6564 6972 7328 5f64    os.makedirs(_d
+00006f30: 6972 2c20 6578 6973 745f 6f6b 3d54 7275  ir, exist_ok=Tru
+00006f40: 6529 0a0a 2020 2020 2020 2020 7465 6d70  e)..        temp
+00006f50: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
+00006f60: 6f69 6e28 5f64 6972 2c20 2274 656d 705f  oin(_dir, "temp_
+00006f70: 6469 7222 290a 0a20 2020 2020 2020 206f  dir")..        o
+00006f80: 732e 6d61 6b65 6469 7273 2874 656d 705f  s.makedirs(temp_
+00006f90: 6469 722c 2065 7869 7374 5f6f 6b3d 5472  dir, exist_ok=Tr
+00006fa0: 7565 290a 0a20 2020 2020 2020 206d 6574  ue)..        met
+00006fb0: 686f 6420 3d20 4d65 7468 6f64 2e66 726f  hod = Method.fro
+00006fc0: 6d5f 7661 6c75 6528 6d65 7468 6f64 290a  m_value(method).
+00006fd0: 0a20 2020 2020 2020 2073 656c 662e 7275  .        self.ru
+00006fe0: 6e6e 696e 675f 6461 7461 203d 2073 656c  nning_data = sel
+00006ff0: 662e 6765 745f 6461 7461 2869 6e64 6963  f.get_data(indic
+00007000: 6573 290a 0a20 2020 2020 2020 2077 6974  es)..        wit
+00007010: 6820 7365 6c66 2e73 7461 7465 5f6f 665f  h self.state_of_
+00007020: 6f70 6572 6174 696f 6e73 2e72 756e 5f63  operations.run_c
+00007030: 6f6e 7465 7874 284f 7065 7261 7469 6f6e  ontext(Operation
+00007040: 2e42 5329 3a0a 2020 2020 2020 2020 2020  .BS):.          
+00007050: 2020 6966 2062 6163 6b67 726f 756e 6420    if background 
+00007060: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00007070: 2020 2020 2020 2020 2062 675f 6461 7461           bg_data
+00007080: 203d 2073 656c 662e 7275 6e6e 696e 675f   = self.running_
+00007090: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+000070a0: 2020 2020 2069 6620 696e 6469 6365 7320       if indices 
+000070b0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000070c0: 2020 2020 2020 2020 2020 2020 205f 6c6f               _lo
+000070d0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2022 436f 6d70 7574 696e 6720 6261     "Computing ba
+00007100: 636b 6772 6f75 6e64 2066 726f 6d20 2573  ckground from %s
+00007110: 206f 6620 7261 7720 6461 7461 222c 206d   of raw data", m
+00007120: 6574 686f 642e 6e61 6d65 0a20 2020 2020  ethod.name.     
+00007130: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00007140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007150: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007160: 2020 2020 2020 2020 2020 205f 6c6f 6767             _logg
+00007170: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2022 436f 6d70 7574 696e 6720 6261 636b   "Computing back
+000071a0: 6772 6f75 6e64 2066 726f 6d20 2573 206f  ground from %s o
+000071b0: 6620 6869 6768 2069 6e74 656e 7369 7479  f high intensity
+000071c0: 2064 6174 6122 2c0a 2020 2020 2020 2020   data",.        
+000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071e0: 6d65 7468 6f64 2e6e 616d 652c 0a20 2020  method.name,.   
+000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007200: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+00007210: 6c69 6620 6973 696e 7374 616e 6365 2862  lif isinstance(b
+00007220: 6163 6b67 726f 756e 642c 2044 6174 6173  ackground, Datas
+00007230: 6574 293a 0a20 2020 2020 2020 2020 2020  et):.           
+00007240: 2020 2020 2062 675f 6461 7461 203d 2062       bg_data = b
+00007250: 6163 6b67 726f 756e 642e 6461 7461 0a20  ackground.data. 
+00007260: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00007270: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007290: 2022 436f 6d70 7574 696e 6720 6261 636b   "Computing back
+000072a0: 6772 6f75 6e64 2066 726f 6d20 2573 206f  ground from %s o
+000072b0: 6620 6062 6163 6b67 726f 756e 6460 2073  f `background` s
+000072c0: 6574 222c 206d 6574 686f 642e 6e61 6d65  et", method.name
+000072d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000072e0: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+000072f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007300: 2020 2020 2062 675f 6461 7461 203d 2073       bg_data = s
+00007310: 656c 662e 6765 745f 6461 7461 2862 6163  elf.get_data(bac
+00007320: 6b67 726f 756e 6429 0a20 2020 2020 2020  kground).       
+00007330: 2020 2020 2020 2020 205f 6c6f 6767 6572           _logger
+00007340: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+00007350: 2020 2020 2020 2020 2020 2022 436f 6d70             "Comp
+00007360: 7574 696e 6720 6261 636b 6772 6f75 6e64  uting background
+00007370: 2066 726f 6d20 2573 206f 6620 6c6f 7720   from %s of low 
+00007380: 696e 7465 6e73 6974 7920 6461 7461 222c  intensity data",
+00007390: 206d 6574 686f 642e 6e61 6d65 0a20 2020   method.name.   
+000073a0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+000073b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000073c0: 656c 662e 5f69 6e5f 6d65 6d6f 7279 3a0a  elf._in_memory:.
+000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073e0: 6e65 775f 6461 7461 203d 2062 6163 6b67  new_data = backg
+000073f0: 726f 756e 645f 7375 6274 7261 6374 696f  round_subtractio
+00007400: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00007410: 2020 2020 2020 2073 656c 662e 7275 6e6e         self.runn
+00007420: 696e 675f 6461 7461 2c20 6267 5f64 6174  ing_data, bg_dat
+00007430: 612c 206d 6574 686f 640a 2020 2020 2020  a, method.      
+00007440: 2020 2020 2020 2020 2020 292e 7669 6577            ).view
+00007450: 2844 6174 6129 0a20 2020 2020 2020 2020  (Data).         
+00007460: 2020 2020 2020 206e 6577 5f64 6174 612e         new_data.
+00007470: 7361 7665 286f 732e 7061 7468 2e6a 6f69  save(os.path.joi
+00007480: 6e28 7465 6d70 5f64 6972 2c20 2264 6174  n(temp_dir, "dat
+00007490: 612e 6864 6635 2229 290a 2020 2020 2020  a.hdf5")).      
+000074a0: 2020 2020 2020 2020 2020 7572 6c73 203d            urls =
+000074b0: 206e 6577 5f64 6174 612e 7572 6c73 0a20   new_data.urls. 
+000074c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000074d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000074e0: 2062 6720 3d20 6e75 6d70 792e 7a65 726f   bg = numpy.zero
+000074f0: 7328 7365 6c66 2e72 756e 6e69 6e67 5f64  s(self.running_d
+00007500: 6174 615b 305d 2e73 6861 7065 2c20 7365  ata[0].shape, se
+00007510: 6c66 2e72 756e 6e69 6e67 5f64 6174 612e  lf.running_data.
+00007520: 6474 7970 6529 0a20 2020 2020 2020 2020  dtype).         
+00007530: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+00007540: 203d 3d20 4d65 7468 6f64 2e6d 6561 6e3a   == Method.mean:
+00007550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007560: 2020 2020 2069 6620 6267 5f64 6174 612e       if bg_data.
+00007570: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
 00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 6920 2b20 312c            i + 1,
-000075a0: 206c 656e 2862 675f 6461 7461 292c 2022   len(bg_data), "
-000075b0: 436f 6d70 7574 696e 6720 6d65 616e 2069  Computing mean i
-000075c0: 6d61 6765 220a 2020 2020 2020 2020 2020  mage".          
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000075f0: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
-00007600: 3d3d 204d 6574 686f 642e 6d65 6469 616e  == Method.median
-00007610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007620: 2020 2020 2020 6966 2062 675f 6461 7461        if bg_data
-00007630: 2e69 6e5f 6d65 6d6f 7279 3a0a 2020 2020  .in_memory:.    
-00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007650: 2020 2020 6e75 6d70 792e 6d65 6469 616e      numpy.median
-00007660: 2862 675f 6461 7461 2c20 6f75 743d 6267  (bg_data, out=bg
-00007670: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-00007680: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00007690: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000076a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000076b0: 7465 7020 6973 206e 6f74 204e 6f6e 653a  tep is not None:
-000076c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000076d0: 2020 2020 2020 2020 2020 2020 2062 675f               bg_
-000076e0: 696e 6469 6365 7320 3d20 6e75 6d70 792e  indices = numpy.
-000076f0: 6172 616e 6765 2830 2c20 6c65 6e28 6267  arange(0, len(bg
-00007700: 5f64 6174 6129 2c20 7374 6570 290a 2020  _data), step).  
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00007750: 756d 7079 2e6d 6564 6961 6e28 0a20 2020  umpy.median(.   
+00007590: 2020 206e 756d 7079 2e6d 6561 6e28 6267     numpy.mean(bg
+000075a0: 5f64 6174 612c 206f 7574 3d62 672c 2061  _data, out=bg, a
+000075b0: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
+000075c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000075d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000075e0: 2020 2020 2020 2020 2069 6f5f 7574 696c           io_util
+000075f0: 732e 6164 7661 6e63 656d 656e 745f 6469  s.advancement_di
+00007600: 7370 6c61 7928 0a20 2020 2020 2020 2020  splay(.         
+00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007620: 2020 2030 2c20 6c65 6e28 6267 5f64 6174     0, len(bg_dat
+00007630: 6129 2c20 2243 6f6d 7075 7469 6e67 206d  a), "Computing m
+00007640: 6561 6e20 696d 6167 6522 0a20 2020 2020  ean image".     
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00007670: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00007680: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00007690: 6267 5f64 6174 6129 293a 0a20 2020 2020  bg_data)):.     
+000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076b0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+000076c0: 6c66 2e73 7461 7465 5f6f 665f 6f70 6572  lf.state_of_oper
+000076d0: 6174 696f 6e73 2e69 735f 7275 6e6e 696e  ations.is_runnin
+000076e0: 6728 4f70 6572 6174 696f 6e2e 4253 293a  g(Operation.BS):
+000076f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007710: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 6267 203d 2069 6d67 3269 6d67      bg = img2img
+00007740: 5f6d 6561 6e28 6267 5f64 6174 615b 695d  _mean(bg_data[i]
+00007750: 2c20 6267 2c20 6929 0a20 2020 2020 2020  , bg, i).       
 00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 2044 6174 6128 0a20 2020 2020 2020 2020   Data(.         
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000077b0: 675f 6461 7461 2e75 726c 735b 6267 5f69  g_data.urls[bg_i
-000077c0: 6e64 6963 6573 5d2c 0a20 2020 2020 2020  ndices],.       
-000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007770: 2020 2020 2069 6f5f 7574 696c 732e 6164       io_utils.ad
+00007780: 7661 6e63 656d 656e 745f 6469 7370 6c61  vancement_displa
+00007790: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 2020 2069 202b 2031 2c20 6c65 6e28 6267     i + 1, len(bg
+000077c0: 5f64 6174 6129 2c20 2243 6f6d 7075 7469  _data), "Computi
+000077d0: 6e67 206d 6561 6e20 696d 6167 6522 0a20  ng mean image". 
 000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077f0: 2062 675f 6461 7461 2e6d 6574 6164 6174   bg_data.metadat
-00007800: 615b 6267 5f69 6e64 6963 6573 5d2c 0a20  a[bg_indices],. 
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2020 2020 6f75 743d 6267            out=bg
-00007860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 2020 2020 2020 6178 6973 3d30 2c0a 2020        axis=0,.  
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000077f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00007800: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00007810: 6620 6d65 7468 6f64 203d 3d20 4d65 7468  f method == Meth
+00007820: 6f64 2e6d 6564 6961 6e3a 0a20 2020 2020  od.median:.     
+00007830: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007840: 6620 6267 5f64 6174 612e 696e 5f6d 656d  f bg_data.in_mem
+00007850: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
+00007860: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00007870: 7079 2e6d 6564 6961 6e28 6267 5f64 6174  py.median(bg_dat
+00007880: 612c 206f 7574 3d62 672c 2061 7869 733d  a, out=bg, axis=
+00007890: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+000078a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000078d0: 7074 204d 656d 6f72 7945 7272 6f72 3a0a  pt MemoryError:.
+000078c0: 2020 2020 2069 6620 7374 6570 2069 7320       if step is 
+000078d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
 000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007900: 6966 206e 6f74 2073 656c 662e 7374 6174  if not self.stat
-00007910: 655f 6f66 5f6f 7065 7261 7469 6f6e 732e  e_of_operations.
-00007920: 6973 5f72 756e 6e69 6e67 280a 2020 2020  is_running(.    
+000078f0: 2020 2020 2020 6267 5f69 6e64 6963 6573        bg_indices
+00007900: 203d 206e 756d 7079 2e61 7261 6e67 6528   = numpy.arange(
+00007910: 302c 206c 656e 2862 675f 6461 7461 292c  0, len(bg_data),
+00007920: 2073 7465 7029 0a20 2020 2020 2020 2020   step).         
 00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007950: 4f70 6572 6174 696f 6e2e 4253 0a20 2020  Operation.BS.   
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00007940: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007960: 2020 2020 2020 2020 6e75 6d70 792e 6d65          numpy.me
+00007970: 6469 616e 280a 2020 2020 2020 2020 2020  dian(.          
 00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00007990: 2020 2020 2020 2020 2020 4461 7461 280a            Data(.
+000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 2020 2020 2020 2020 205f 6c6f 6767             _logg
-000079d0: 6572 2e65 7272 6f72 280a 2020 2020 2020  er.error(.      
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2020 2020 2020 2020 224d                "M
-00007a00: 656d 6f72 7945 7272 6f72 2c20 7472 7969  emoryError, tryi
-00007a10: 6e67 2077 6974 6820 7374 6570 2025 7322  ng with step %s"
-00007a20: 2c20 7374 6570 202b 2031 0a20 2020 2020  , step + 1.     
+000079c0: 2020 2020 2020 2020 6267 5f64 6174 612e          bg_data.
+000079d0: 7572 6c73 5b62 675f 696e 6469 6365 735d  urls[bg_indices]
+000079e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 2020 2020 2020 2020 2020 6267 5f64 6174            bg_dat
+00007a10: 612e 6d65 7461 6461 7461 5b62 675f 696e  a.metadata[bg_in
+00007a20: 6469 6365 735d 2c0a 2020 2020 2020 2020  dices],.        
 00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00007a40: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
 00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00007a70: 7572 6e20 7365 6c66 2e61 7070 6c79 5f62  urn self.apply_b
-00007a80: 6163 6b67 726f 756e 645f 7375 6274 7261  ackground_subtra
-00007a90: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 2020 2020 2020 2062 6163 6b67             backg
-00007ac0: 726f 756e 642c 206d 6574 686f 642c 2069  round, method, i
-00007ad0: 6e64 6963 6573 2c20 7374 6570 202b 2031  ndices, step + 1
-00007ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00007b10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b30: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00007b40: 7274 203d 205b 302c 2030 5d0a 2020 2020  rt = [0, 0].    
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 206f 7574 3d62 672c 0a20 2020 2020     out=bg,.     
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00007aa0: 7869 733d 302c 0a20 2020 2020 2020 2020  xis=0,.         
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ae0: 2020 2020 2065 7863 6570 7420 4d65 6d6f       except Memo
+00007af0: 7279 4572 726f 723a 0a20 2020 2020 2020  ryError:.       
+00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b10: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00007b20: 7365 6c66 2e73 7461 7465 5f6f 665f 6f70  self.state_of_op
+00007b30: 6572 6174 696f 6e73 2e69 735f 7275 6e6e  erations.is_runn
+00007b40: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
 00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 2020 2020 696d 6720 3d20 7365          img = se
-00007b70: 6c66 2e72 756e 6e69 6e67 5f64 6174 615b  lf.running_data[
-00007b80: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00007ba0: 6720 3d20 6e75 6d70 792e 656d 7074 7928  g = numpy.empty(
-00007bb0: 696d 672e 7368 6170 652c 2069 6d67 2e64  img.shape, img.d
-00007bc0: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
+00007b60: 2020 2020 2020 2020 204f 7065 7261 7469           Operati
+00007b70: 6f6e 2e42 530a 2020 2020 2020 2020 2020  on.BS.          
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bb0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007bc0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
 00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 6368 756e 6b73 5f31 203d 2069 6e74    chunks_1 = int
-00007bf0: 286e 756d 7079 2e63 6569 6c28 696d 672e  (numpy.ceil(img.
-00007c00: 7368 6170 655b 305d 202f 2063 6875 6e6b  shape[0] / chunk
-00007c10: 5f73 6861 7065 5b30 5d29 290a 2020 2020  _shape[0])).    
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 6368 756e 6b73 5f32          chunks_2
-00007c40: 203d 2069 6e74 286e 756d 7079 2e63 6569   = int(numpy.cei
-00007c50: 6c28 696d 672e 7368 6170 655b 315d 202f  l(img.shape[1] /
-00007c60: 2063 6875 6e6b 5f73 6861 7065 5b31 5d29   chunk_shape[1])
-00007c70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007c80: 2020 2020 2020 2020 2020 2020 2020 696f                io
-00007c90: 5f75 7469 6c73 2e61 6476 616e 6365 6d65  _utils.advanceme
-00007ca0: 6e74 5f64 6973 706c 6179 280a 2020 2020  nt_display(.    
+00007be0: 2020 2020 5f6c 6f67 6765 722e 6572 726f      _logger.erro
+00007bf0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2020 2020 2020 2022 4d65 6d6f 7279 4572         "MemoryEr
+00007c20: 726f 722c 2074 7279 696e 6720 7769 7468  ror, trying with
+00007c30: 2073 7465 7020 2573 222c 2073 7465 7020   step %s", step 
+00007c40: 2b20 310a 2020 2020 2020 2020 2020 2020  + 1.            
+00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c60: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00007c90: 662e 6170 706c 795f 6261 636b 6772 6f75  f.apply_backgrou
+00007ca0: 6e64 5f73 7562 7472 6163 7469 6f6e 280a  nd_subtraction(.
 00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007cf0: 6875 6e6b 735f 3120 2a20 6368 756e 6b73  hunks_1 * chunks
-00007d00: 5f32 202a 206c 656e 2862 675f 6461 7461  _2 * len(bg_data
-00007d10: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2020 6261 636b 6772 6f75 6e64 2c20      background, 
+00007ce0: 6d65 7468 6f64 2c20 696e 6469 6365 732c  method, indices,
+00007cf0: 2073 7465 7020 2b20 310a 2020 2020 2020   step + 1.      
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2022 436f 6d70 7574 696e 6720 6d65     "Computing me
-00007d40: 6469 616e 2069 6d61 6765 222c 0a20 2020  dian image",.   
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00007d30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2020 2020 2020 7374 6172 7420 3d20 5b30        start = [0
+00007d60: 2c20 305d 0a20 2020 2020 2020 2020 2020  , 0].           
 00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00007d90: 7261 6e67 6528 6368 756e 6b73 5f31 293a  range(chunks_1):
-00007da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dc0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-00007dd0: 6368 756e 6b73 5f32 293a 0a20 2020 2020  chunks_2):.     
+00007d80: 2069 6d67 203d 2073 656c 662e 7275 6e6e   img = self.runn
+00007d90: 696e 675f 6461 7461 5b30 5d0a 2020 2020  ing_data[0].    
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007db0: 2020 2020 2020 2020 6267 203d 206e 756d          bg = num
+00007dc0: 7079 2e65 6d70 7479 2869 6d67 2e73 6861  py.empty(img.sha
+00007dd0: 7065 2c20 696d 672e 6474 7970 6529 0a20  pe, img.dtype). 
 00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007e00: 6620 6e6f 7420 7365 6c66 2e73 7461 7465  f not self.state
-00007e10: 5f6f 665f 6f70 6572 6174 696f 6e73 2e69  _of_operations.i
-00007e20: 735f 7275 6e6e 696e 6728 0a20 2020 2020  s_running(.     
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007df0: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
+00007e00: 735f 3120 3d20 696e 7428 6e75 6d70 792e  s_1 = int(numpy.
+00007e10: 6365 696c 2869 6d67 2e73 6861 7065 5b30  ceil(img.shape[0
+00007e20: 5d20 2f20 6368 756e 6b5f 7368 6170 655b  ] / chunk_shape[
+00007e30: 305d 2929 0a20 2020 2020 2020 2020 2020  0])).           
 00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e50: 2020 204f 7065 7261 7469 6f6e 2e42 530a     Operation.BS.
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e80: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00007e50: 2063 6875 6e6b 735f 3220 3d20 696e 7428   chunks_2 = int(
+00007e60: 6e75 6d70 792e 6365 696c 2869 6d67 2e73  numpy.ceil(img.s
+00007e70: 6861 7065 5b31 5d20 2f20 6368 756e 6b5f  hape[1] / chunk_
+00007e80: 7368 6170 655b 315d 2929 0a20 2020 2020  shape[1])).     
 00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007eb0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 2020 2020 635f 696d 6167            c_imag
-00007ee0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+00007ea0: 2020 2020 2020 2069 6f5f 7574 696c 732e         io_utils.
+00007eb0: 6164 7661 6e63 656d 656e 745f 6469 7370  advancement_disp
+00007ec0: 6c61 7928 0a20 2020 2020 2020 2020 2020  lay(.           
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
 00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 6370 7573              cpus
-00007f10: 203d 206d 756c 7469 7072 6f63 6573 7369   = multiprocessi
-00007f20: 6e67 2e63 7075 5f63 6f75 6e74 2829 0a20  ng.cpu_count(). 
+00007f00: 2020 2020 2020 2020 6368 756e 6b73 5f31          chunks_1
+00007f10: 202a 2063 6875 6e6b 735f 3220 2a20 6c65   * chunks_2 * le
+00007f20: 6e28 6267 5f64 6174 6129 2c0a 2020 2020  n(bg_data),.    
 00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 2077 6974 6820 506f 6f6c 2863 7075     with Pool(cpu
-00007f60: 7320 2d20 3129 2061 7320 703a 0a20 2020  s - 1) as p:.   
+00007f40: 2020 2020 2020 2020 2020 2020 2243 6f6d              "Com
+00007f50: 7075 7469 6e67 206d 6564 6961 6e20 696d  puting median im
+00007f60: 6167 6522 2c0a 2020 2020 2020 2020 2020  age",.          
 00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2020 2063 5f69 6d61 6765 7320 3d20       c_images = 
-00007fa0: 702e 6d61 7028 0a20 2020 2020 2020 2020  p.map(.         
-00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 666f 7220 6920 696e 2072 616e 6765 2863  for i in range(c
+00007fb0: 6875 6e6b 735f 3129 3a0a 2020 2020 2020  hunks_1):.      
 00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2070 6172 7469 616c 2863 6875 6e6b     partial(chunk
-00007fe0: 5f69 6d61 6765 2c20 7374 6172 742c 2063  _image, start, c
-00007ff0: 6875 6e6b 5f73 6861 7065 292c 0a20 2020  hunk_shape),.   
+00007fd0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+00007fe0: 696e 2072 616e 6765 2863 6875 6e6b 735f  in range(chunks_
+00007ff0: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
 00008000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 2062 675f 6461 7461           bg_data
-00008030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008050: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 696f 5f75 7469 6c73 2e61 6476 616e 6365  io_utils.advance
-00008090: 6d65 6e74 5f64 6973 706c 6179 280a 2020  ment_display(.  
+00008010: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00008020: 656c 662e 7374 6174 655f 6f66 5f6f 7065  elf.state_of_ope
+00008030: 7261 7469 6f6e 732e 6973 5f72 756e 6e69  rations.is_runni
+00008040: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2020 2020 4f70 6572              Oper
+00008070: 6174 696f 6e2e 4253 0a20 2020 2020 2020  ation.BS.       
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2020 2020 2020 6920 2a20 6368 756e 6b73        i * chunks
-000080d0: 5f32 202b 206a 202b 2031 2c0a 2020 2020  _2 + j + 1,.    
+000080c0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 6368 756e 6b73 5f31 202a 2063      chunks_1 * c
-00008110: 6875 6e6b 735f 322c 0a20 2020 2020 2020  hunks_2,.       
-00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2022 436f 6d70 7574 696e 6720 6d65 6469   "Computing medi
-00008150: 616e 2069 6d61 6765 222c 0a20 2020 2020  an image",.     
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000080f0: 2020 2063 5f69 6d61 6765 7320 3d20 5b5d     c_images = []
+00008100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 2063 7075 7320 3d20 6d75 6c74       cpus = mult
+00008130: 6970 726f 6365 7373 696e 672e 6370 755f  iprocessing.cpu_
+00008140: 636f 756e 7428 290a 2020 2020 2020 2020  count().        
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00008170: 2050 6f6f 6c28 6370 7573 202d 2031 2920   Pool(cpus - 1) 
+00008180: 6173 2070 3a0a 2020 2020 2020 2020 2020  as p:.          
 00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2020 2020 206e 756d 7079 2e6d 6564 6961       numpy.media
-000081b0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+000081a0: 2020 2020 2020 2020 2020 2020 2020 635f                c_
+000081b0: 696d 6167 6573 203d 2070 2e6d 6170 280a  images = p.map(.
 000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081d0: 2020 2020 2020 2020 2020 2063 5f69 6d61             c_ima
-000081e0: 6765 732c 0a20 2020 2020 2020 2020 2020  ges,.           
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00008210: 3d62 675b 0a20 2020 2020 2020 2020 2020  =bg[.           
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 2020 2020 2020 7061 7274              part
+000081f0: 6961 6c28 6368 756e 6b5f 696d 6167 652c  ial(chunk_image,
+00008200: 2073 7461 7274 2c20 6368 756e 6b5f 7368   start, chunk_sh
+00008210: 6170 6529 2c0a 2020 2020 2020 2020 2020  ape),.          
 00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2073 7461 7274 5b30 5d20 3a20 7374 6172   start[0] : star
-00008250: 745b 305d 202b 2063 6875 6e6b 5f73 6861  t[0] + chunk_sha
-00008260: 7065 5b30 5d2c 0a20 2020 2020 2020 2020  pe[0],.         
-00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 6267 5f64 6174 612c 0a20 2020 2020    bg_data,.     
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 2020 2073 7461 7274 5b31 5d20 3a20 7374     start[1] : st
-000082a0: 6172 745b 315d 202b 2063 6875 6e6b 5f73  art[1] + chunk_s
-000082b0: 6861 7065 5b31 5d2c 0a20 2020 2020 2020  hape[1],.       
+00008290: 2020 2020 2020 2020 2069 6f5f 7574 696c           io_util
+000082a0: 732e 6164 7661 6e63 656d 656e 745f 6469  s.advancement_di
+000082b0: 7370 6c61 7928 0a20 2020 2020 2020 2020  splay(.         
 000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008300: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00008310: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000082d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000082e0: 202a 2063 6875 6e6b 735f 3220 2b20 6a20   * chunks_2 + j 
+000082f0: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2020 2020 2020 2063 6875               chu
+00008320: 6e6b 735f 3120 2a20 6368 756e 6b73 5f32  nks_1 * chunks_2
+00008330: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008350: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00008360: 6172 745b 315d 203d 2063 6875 6e6b 5f73  art[1] = chunk_s
-00008370: 6861 7065 5b31 5d20 2a20 286a 202b 2031  hape[1] * (j + 1
-00008380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2020 7374 6172 745b 305d 203d 2063 6875    start[0] = chu
-000083b0: 6e6b 5f73 6861 7065 5b30 5d20 2a20 2869  nk_shape[0] * (i
-000083c0: 202b 2031 290a 2020 2020 2020 2020 2020   + 1).          
+00008350: 2020 2020 2020 2020 2020 2243 6f6d 7075            "Compu
+00008360: 7469 6e67 206d 6564 6961 6e20 696d 6167  ting median imag
+00008370: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008390: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+000083c0: 6d70 792e 6d65 6469 616e 280a 2020 2020  mpy.median(.    
 000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 2020 2020 7374 6172 745b 315d 203d        start[1] =
-000083f0: 2030 0a0a 2020 2020 2020 2020 2020 2020   0..            
-00008400: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00008410: 7374 6174 655f 6f66 5f6f 7065 7261 7469  state_of_operati
-00008420: 6f6e 732e 6973 5f72 756e 6e69 6e67 284f  ons.is_running(O
-00008430: 7065 7261 7469 6f6e 2e42 5329 3a0a 2020  peration.BS):.  
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 2020 635f 696d 6167 6573 2c0a 2020      c_images,.  
+00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 2020 2020 2020 6f75 743d 6267 5b0a 2020        out=bg[.  
+00008430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00008460: 2020 2020 2020 2020 2075 726c 7320 3d20           urls = 
-00008470: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
-00008480: 612e 6170 706c 795f 6675 6e63 7328 0a20  a.apply_funcs(. 
+00008450: 2020 2020 2020 2020 2020 7374 6172 745b            start[
+00008460: 305d 203a 2073 7461 7274 5b30 5d20 2b20  0] : start[0] + 
+00008470: 6368 756e 6b5f 7368 6170 655b 305d 2c0a  chunk_shape[0],.
+00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084a0: 2020 205b 2862 6163 6b67 726f 756e 645f     [(background_
-000084b0: 7375 6274 7261 6374 696f 6e5f 3244 2c20  subtraction_2D, 
-000084c0: 5b62 675d 295d 2c0a 2020 2020 2020 2020  [bg])],.        
-000084d0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000084e0: 3d6f 732e 7061 7468 2e6a 6f69 6e28 7465  =os.path.join(te
-000084f0: 6d70 5f64 6972 2c20 2264 6174 612e 6864  mp_dir, "data.hd
-00008500: 6635 2229 2c0a 2020 2020 2020 2020 2020  f5"),.          
-00008510: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
-00008520: 4170 706c 7969 6e67 2062 6163 6b67 726f  Applying backgro
-00008530: 756e 6420 7375 6274 7261 6374 696f 6e22  und subtraction"
-00008540: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008550: 2020 2020 2020 6f70 6572 6174 696f 6e3d        operation=
-00008560: 4f70 6572 6174 696f 6e2e 4253 2c0a 2020  Operation.BS,.  
-00008570: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008590: 6966 2075 726c 7320 6973 204e 6f6e 653a  if urls is None:
-000085a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000085b0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-000085c0: 2020 2020 2023 2053 6574 2075 726c 7320       # Set urls 
-000085d0: 6173 2073 6861 7065 2061 6e64 2064 696d  as shape and dim
-000085e0: 656e 7369 6f6e 206f 6620 6f72 6967 696e  ension of origin
-000085f0: 616c 2075 726c 732e 0a20 2020 2020 2020  al urls..       
-00008600: 2069 6620 696e 6469 6365 7320 6973 206e   if indices is n
-00008610: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008620: 2020 2020 206e 6577 5f75 726c 7320 3d20       new_urls = 
-00008630: 6e75 6d70 792e 6172 7261 7928 7365 6c66  numpy.array(self
-00008640: 2e67 6574 5f64 6174 6128 292e 7572 6c73  .get_data().urls
-00008650: 2c20 6474 7970 653d 6f62 6a65 6374 290a  , dtype=object).
-00008660: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00008670: 7572 6c73 5b69 6e64 6963 6573 5d20 3d20  urls[indices] = 
-00008680: 7572 6c73 0a20 2020 2020 2020 2020 2020  urls.           
-00008690: 206e 6577 5f64 6174 6120 3d20 4461 7461   new_data = Data
-000086a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000086b0: 2020 6e65 775f 7572 6c73 2e72 6573 6861    new_urls.resha
-000086c0: 7065 2873 656c 662e 6461 7461 2e75 726c  pe(self.data.url
-000086d0: 732e 7368 6170 6529 2c0a 2020 2020 2020  s.shape),.      
-000086e0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000086f0: 6174 612e 6d65 7461 6461 7461 2c0a 2020  ata.metadata,.  
-00008700: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008710: 6c66 2e5f 696e 5f6d 656d 6f72 792c 0a20  lf._in_memory,. 
-00008720: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00008740: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
-00008750: 3d20 4461 7461 280a 2020 2020 2020 2020  = Data(.        
-00008760: 2020 2020 2020 2020 7572 6c73 2e72 6573          urls.res
-00008770: 6861 7065 2873 656c 662e 6461 7461 2e75  hape(self.data.u
-00008780: 726c 732e 7368 6170 6529 2c20 7365 6c66  rls.shape), self
-00008790: 2e64 6174 612e 6d65 7461 6461 7461 2c20  .data.metadata, 
-000087a0: 7365 6c66 2e5f 696e 5f6d 656d 6f72 790a  self._in_memory.
-000087b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000087c0: 2020 2020 2020 206e 6577 5f64 6174 612e         new_data.
-000087d0: 7361 7665 286f 732e 7061 7468 2e6a 6f69  save(os.path.joi
-000087e0: 6e28 5f64 6972 2c20 2264 6174 612e 6864  n(_dir, "data.hd
-000087f0: 6635 2229 2c20 696e 6469 6365 733d 696e  f5"), indices=in
-00008800: 6469 6365 7329 0a0a 2020 2020 2020 2020  dices)..        
-00008810: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00008820: 206f 732e 7265 6d6f 7665 286f 732e 7061   os.remove(os.pa
-00008830: 7468 2e6a 6f69 6e28 7465 6d70 5f64 6972  th.join(temp_dir
-00008840: 2c20 2264 6174 612e 6864 6635 2229 290a  , "data.hdf5")).
-00008850: 2020 2020 2020 2020 2020 2020 6f73 2e72              os.r
-00008860: 6d64 6972 2874 656d 705f 6469 7229 0a20  mdir(temp_dir). 
-00008870: 2020 2020 2020 2065 7863 6570 7420 4f53         except OS
-00008880: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00008890: 2020 2020 2020 2020 5f6c 6f67 6765 722e          _logger.
-000088a0: 7761 726e 696e 6728 2245 7272 6f72 3a20  warning("Error: 
-000088b0: 2573 2220 2520 2865 2e73 7472 6572 726f  %s" % (e.strerro
-000088c0: 7229 290a 0a20 2020 2020 2020 2072 6574  r))..        ret
-000088d0: 7572 6e20 4461 7461 7365 7428 0a20 2020  urn Dataset(.   
-000088e0: 2020 2020 2020 2020 205f 6469 723d 5f64           _dir=_d
-000088f0: 6972 2c0a 2020 2020 2020 2020 2020 2020  ir,.            
-00008900: 6461 7461 3d6e 6577 5f64 6174 612c 0a20  data=new_data,. 
-00008910: 2020 2020 2020 2020 2020 2064 696d 733d             dims=
-00008920: 7365 6c66 2e5f 5f64 696d 732c 0a20 2020  self.__dims,.   
-00008930: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00008940: 726d 6174 696f 6e3d 7365 6c66 2e74 7261  rmation=self.tra
-00008950: 6e73 666f 726d 6174 696f 6e2c 0a20 2020  nsformation,.   
-00008960: 2020 2020 2020 2020 2069 6e5f 6d65 6d6f           in_memo
-00008970: 7279 3d73 656c 662e 5f69 6e5f 6d65 6d6f  ry=self._in_memo
-00008980: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-00008990: 7469 746c 653d 7365 6c66 2e74 6974 6c65  title=self.title
-000089a0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000089b0: 2064 6566 2061 7070 6c79 5f68 6f74 5f70   def apply_hot_p
-000089c0: 6978 656c 5f72 656d 6f76 616c 2873 656c  ixel_removal(sel
-000089d0: 662c 206b 6572 6e65 6c3d 332c 2069 6e64  f, kernel=3, ind
-000089e0: 6963 6573 3d4e 6f6e 652c 205f 6469 723d  ices=None, _dir=
-000089f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00008a00: 2222 0a20 2020 2020 2020 2041 7070 6c69  "".        Appli
-00008a10: 6573 2068 6f74 2070 6978 656c 2072 656d  es hot pixel rem
-00008a20: 6f76 616c 2074 6f20 4461 7461 2c20 616e  oval to Data, an
-00008a30: 6420 7361 7665 7320 7468 6520 6e65 7720  d saves the new 
-00008a40: 6461 7461 0a20 2020 2020 2020 2069 6e74  data.        int
-00008a50: 6f20 6469 736b 2e0a 0a20 2020 2020 2020  o disk...       
-00008a60: 203a 7061 7261 6d20 696e 7420 6b65 726e   :param int kern
-00008a70: 656c 3a20 7369 7a65 206f 6620 7468 6520  el: size of the 
-00008a80: 6b65 726e 656c 2075 7365 6420 746f 2066  kernel used to f
-00008a90: 696e 6420 7468 6520 686f 740a 2020 2020  ind the hot.    
-00008aa0: 2020 2020 2020 2020 7069 7865 6c73 2e0a          pixels..
-00008ab0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00008ac0: 6e64 6963 6573 3a20 496e 6469 6365 7320  ndices: Indices 
-00008ad0: 6f66 2074 6865 2069 6d61 6765 7320 746f  of the images to
-00008ae0: 2061 7070 6c79 2062 6163 6b67 726f 756e   apply backgroun
-00008af0: 6420 7375 6274 7261 6374 696f 6e2e 0a20  d subtraction.. 
-00008b00: 2020 2020 2020 2020 2020 2049 6620 4e6f             If No
-00008b10: 6e65 2c20 7468 6520 686f 7420 7069 7865  ne, the hot pixe
-00008b20: 6c20 7265 6d6f 7661 6c20 6973 2061 7070  l removal is app
-00008b30: 6c69 6564 2074 6f20 616c 6c20 7468 6520  lied to all the 
-00008b40: 6461 7461 2e0a 2020 2020 2020 2020 3a74  data..        :t
-00008b50: 7970 6520 696e 6469 6365 733a 2055 6e69  ype indices: Uni
-00008b60: 6f6e 5b4e 6f6e 652c 2061 7272 6179 5f6c  on[None, array_l
-00008b70: 696b 655d 0a20 2020 2020 2020 203a 7265  ike].        :re
-00008b80: 7475 726e 3a20 6461 7461 7365 7420 7769  turn: dataset wi
-00008b90: 7468 2064 6174 6120 6f66 2073 616d 6520  th data of same 
-00008ba0: 7369 7a65 2061 7320 6073 656c 662e 6461  size as `self.da
-00008bb0: 7461 6020 6275 7420 7769 7468 2074 6865  ta` but with the
-00008bc0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-00008bd0: 6966 6965 6420 696d 6167 6573 2e20 5468  ified images. Th
-00008be0: 6520 7572 6c73 206f 6620 7468 6520 6d6f  e urls of the mo
-00008bf0: 6469 6669 6564 2069 6d61 6765 7320 6172  dified images ar
-00008c00: 6520 7265 706c 6163 6564 2077 6974 680a  e replaced with.
-00008c10: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00008c20: 6e65 7720 7572 6c73 2e0a 2020 2020 2020  new urls..      
-00008c30: 2020 3a72 7479 7065 3a20 4461 7461 7365    :rtype: Datase
-00008c40: 740a 2020 2020 2020 2020 2222 220a 0a20  t.        """.. 
-00008c50: 2020 2020 2020 2073 656c 662e 7275 6e6e         self.runn
-00008c60: 696e 675f 6461 7461 203d 2073 656c 662e  ing_data = self.
-00008c70: 6765 745f 6461 7461 2869 6e64 6963 6573  get_data(indices
-00008c80: 290a 0a20 2020 2020 2020 205f 6469 7220  )..        _dir 
-00008c90: 3d20 7365 6c66 2e64 6972 2069 6620 5f64  = self.dir if _d
-00008ca0: 6972 2069 7320 4e6f 6e65 2065 6c73 6520  ir is None else 
-00008cb0: 5f64 6972 0a0a 2020 2020 2020 2020 6f73  _dir..        os
-00008cc0: 2e6d 616b 6564 6972 7328 5f64 6972 2c20  .makedirs(_dir, 
-00008cd0: 6578 6973 745f 6f6b 3d54 7275 6529 0a0a  exist_ok=True)..
-00008ce0: 2020 2020 2020 2020 7465 6d70 5f64 6972          temp_dir
-00008cf0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00008d00: 5f64 6972 2c20 2274 656d 705f 6469 7222  _dir, "temp_dir"
-00008d10: 290a 0a20 2020 2020 2020 206f 732e 6d61  )..        os.ma
-00008d20: 6b65 6469 7273 2874 656d 705f 6469 722c  kedirs(temp_dir,
-00008d30: 2065 7869 7374 5f6f 6b3d 5472 7565 290a   exist_ok=True).
-00008d40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00008d50: 2e5f 696e 5f6d 656d 6f72 793a 0a20 2020  ._in_memory:.   
-00008d60: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
-00008d70: 6120 3d20 686f 745f 7069 7865 6c5f 7265  a = hot_pixel_re
-00008d80: 6d6f 7661 6c5f 3344 2873 656c 662e 7275  moval_3D(self.ru
-00008d90: 6e6e 696e 675f 6461 7461 2c20 6b65 726e  nning_data, kern
-00008da0: 656c 292e 7669 6577 2844 6174 6129 0a20  el).view(Data). 
-00008db0: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
-00008dc0: 6174 612e 7361 7665 286f 732e 7061 7468  ata.save(os.path
-00008dd0: 2e6a 6f69 6e28 7465 6d70 5f64 6972 2c20  .join(temp_dir, 
-00008de0: 2264 6174 612e 6864 6635 2229 290a 2020  "data.hdf5")).  
-00008df0: 2020 2020 2020 2020 2020 7572 6c73 203d            urls =
-00008e00: 206e 6577 5f64 6174 612e 7572 6c73 0a20   new_data.urls. 
-00008e10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008e20: 2020 2020 2020 2020 2075 726c 7320 3d20           urls = 
-00008e30: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
-00008e40: 612e 6170 706c 795f 6675 6e63 7328 0a20  a.apply_funcs(. 
-00008e50: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00008e60: 2868 6f74 5f70 6978 656c 5f72 656d 6f76  (hot_pixel_remov
-00008e70: 616c 5f32 442c 205b 6b65 726e 656c 5d29  al_2D, [kernel])
-00008e80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00008e90: 2020 2073 6176 653d 6f73 2e70 6174 682e     save=os.path.
-00008ea0: 6a6f 696e 2874 656d 705f 6469 722c 2022  join(temp_dir, "
-00008eb0: 6461 7461 2e68 6466 3522 292c 0a20 2020  data.hdf5"),.   
-00008ec0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00008ed0: 743d 2241 7070 6c79 696e 6720 686f 7420  t="Applying hot 
-00008ee0: 7069 7865 6c20 7265 6d6f 7661 6c22 2c0a  pixel removal",.
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 6f70 6572 6174 696f 6e3d 4f70 6572 6174  operation=Operat
-00008f10: 696f 6e2e 4850 2c0a 2020 2020 2020 2020  ion.HP,.        
-00008f20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008f30: 2020 6966 2075 726c 7320 6973 204e 6f6e    if urls is Non
-00008f40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00008f50: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
-00008f60: 2020 2069 6620 696e 6469 6365 7320 6973     if indices is
-00008f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008f80: 2020 2020 2020 206e 6577 5f75 726c 7320         new_urls 
-00008f90: 3d20 6e75 6d70 792e 6172 7261 7928 7365  = numpy.array(se
-00008fa0: 6c66 2e67 6574 5f64 6174 6128 292e 7572  lf.get_data().ur
-00008fb0: 6c73 2c20 6474 7970 653d 6f62 6a65 6374  ls, dtype=object
-00008fc0: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-00008fd0: 775f 7572 6c73 5b69 6e64 6963 6573 5d20  w_urls[indices] 
-00008fe0: 3d20 7572 6c73 0a20 2020 2020 2020 2020  = urls.         
-00008ff0: 2020 206e 6577 5f64 6174 6120 3d20 4461     new_data = Da
-00009000: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
-00009010: 2020 2020 6e65 775f 7572 6c73 2e72 6573      new_urls.res
-00009020: 6861 7065 2873 656c 662e 6461 7461 2e75  hape(self.data.u
-00009030: 726c 732e 7368 6170 6529 2c0a 2020 2020  rls.shape),.    
-00009040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009050: 2e64 6174 612e 6d65 7461 6461 7461 2c0a  .data.metadata,.
-00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009070: 7365 6c66 2e5f 696e 5f6d 656d 6f72 792c  self._in_memory,
-00009080: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00009090: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000090a0: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
-000090b0: 6120 3d20 4461 7461 280a 2020 2020 2020  a = Data(.      
-000090c0: 2020 2020 2020 2020 2020 7572 6c73 2e72            urls.r
-000090d0: 6573 6861 7065 2873 656c 662e 6461 7461  eshape(self.data
-000090e0: 2e75 726c 732e 7368 6170 6529 2c20 7365  .urls.shape), se
-000090f0: 6c66 2e64 6174 612e 6d65 7461 6461 7461  lf.data.metadata
-00009100: 2c20 7365 6c66 2e5f 696e 5f6d 656d 6f72  , self._in_memor
-00009110: 790a 2020 2020 2020 2020 2020 2020 290a  y.            ).
-00009120: 0a20 2020 2020 2020 206e 6577 5f64 6174  .        new_dat
-00009130: 612e 7361 7665 286f 732e 7061 7468 2e6a  a.save(os.path.j
-00009140: 6f69 6e28 5f64 6972 2c20 2264 6174 612e  oin(_dir, "data.
-00009150: 6864 6635 2229 2c20 696e 6469 6365 733d  hdf5"), indices=
-00009160: 696e 6469 6365 7329 0a20 2020 2020 2020  indices).       
-00009170: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00009180: 2020 6f73 2e72 656d 6f76 6528 6f73 2e70    os.remove(os.p
-00009190: 6174 682e 6a6f 696e 2874 656d 705f 6469  ath.join(temp_di
-000091a0: 722c 2022 6461 7461 2e68 6466 3522 2929  r, "data.hdf5"))
-000091b0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-000091c0: 726d 6469 7228 7465 6d70 5f64 6972 290a  rmdir(temp_dir).
-000091d0: 2020 2020 2020 2020 6578 6365 7074 204f          except O
-000091e0: 5345 7272 6f72 2061 7320 653a 0a20 2020  SError as e:.   
-000091f0: 2020 2020 2020 2020 205f 6c6f 6767 6572           _logger
-00009200: 2e77 6172 6e69 6e67 2822 4572 726f 723a  .warning("Error:
-00009210: 2025 7322 2025 2028 652e 7374 7265 7272   %s" % (e.strerr
-00009220: 6f72 2929 0a0a 2020 2020 2020 2020 7265  or))..        re
-00009230: 7475 726e 2044 6174 6173 6574 280a 2020  turn Dataset(.  
-00009240: 2020 2020 2020 2020 2020 5f64 6972 3d5f            _dir=_
-00009250: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
-00009260: 2064 6174 613d 6e65 775f 6461 7461 2c0a   data=new_data,.
-00009270: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
-00009280: 3d73 656c 662e 5f5f 6469 6d73 2c0a 2020  =self.__dims,.  
-00009290: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-000092a0: 6f72 6d61 7469 6f6e 3d73 656c 662e 7472  ormation=self.tr
-000092b0: 616e 7366 6f72 6d61 7469 6f6e 2c0a 2020  ansformation,.  
-000092c0: 2020 2020 2020 2020 2020 696e 5f6d 656d            in_mem
-000092d0: 6f72 793d 7365 6c66 2e5f 696e 5f6d 656d  ory=self._in_mem
-000092e0: 6f72 792c 0a20 2020 2020 2020 2020 2020  ory,.           
-000092f0: 2074 6974 6c65 3d73 656c 662e 7469 746c   title=self.titl
-00009300: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-00009310: 2020 6465 6620 6170 706c 795f 7468 7265    def apply_thre
-00009320: 7368 6f6c 645f 7265 6d6f 7661 6c28 7365  shold_removal(se
-00009330: 6c66 2c20 626f 7474 6f6d 3d4e 6f6e 652c  lf, bottom=None,
-00009340: 2074 6f70 3d4e 6f6e 652c 2069 6e64 6963   top=None, indic
-00009350: 6573 3d4e 6f6e 652c 205f 6469 723d 4e6f  es=None, _dir=No
-00009360: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
-00009370: 0a20 2020 2020 2020 2041 7070 6c69 6573  .        Applies
-00009380: 2062 6f74 746f 6d20 7468 7265 7368 6f6c   bottom threshol
-00009390: 6420 746f 2044 6174 612c 2061 6e64 2073  d to Data, and s
-000093a0: 6176 6573 2074 6865 206e 6577 2064 6174  aves the new dat
-000093b0: 610a 2020 2020 2020 2020 696e 746f 2064  a.        into d
-000093c0: 6973 6b2e 0a0a 2020 2020 2020 2020 3a70  isk...        :p
-000093d0: 6172 616d 2069 6e74 2062 6f74 746f 6d3a  aram int bottom:
-000093e0: 2062 6f74 746f 6d20 7468 7265 7368 6f6c   bottom threshol
-000093f0: 6420 746f 2061 7070 6c79 2e0a 2020 2020  d to apply..    
-00009400: 2020 2020 3a70 6172 616d 2069 6e74 2074      :param int t
-00009410: 6f70 3a20 746f 7020 7468 7265 7368 6f6c  op: top threshol
-00009420: 6420 746f 2061 7070 6c79 2e0a 2020 2020  d to apply..    
-00009430: 2020 2020 3a70 6172 616d 2069 6e64 6963      :param indic
-00009440: 6573 3a20 496e 6469 6365 7320 6f66 2074  es: Indices of t
-00009450: 6865 2069 6d61 6765 7320 746f 2061 7070  he images to app
-00009460: 6c79 2062 6163 6b67 726f 756e 6420 7375  ly background su
-00009470: 6274 7261 6374 696f 6e2e 0a20 2020 2020  btraction..     
-00009480: 2020 2020 2020 2049 6620 4e6f 6e65 2c20         If None, 
-00009490: 7468 6520 686f 7420 7069 7865 6c20 7265  the hot pixel re
-000094a0: 6d6f 7661 6c20 6973 2061 7070 6c69 6564  moval is applied
-000094b0: 2074 6f20 616c 6c20 7468 6520 6461 7461   to all the data
-000094c0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000094d0: 696e 6469 6365 733a 2055 6e69 6f6e 5b4e  indices: Union[N
-000094e0: 6f6e 652c 2061 7272 6179 5f6c 696b 655d  one, array_like]
-000094f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00009500: 3a20 6461 7461 7365 7420 7769 7468 2064  : dataset with d
-00009510: 6174 6120 6f66 2073 616d 6520 7369 7a65  ata of same size
-00009520: 2061 7320 6073 656c 662e 6461 7461 6020   as `self.data` 
-00009530: 6275 7420 7769 7468 2074 6865 0a20 2020  but with the.   
-00009540: 2020 2020 2020 2020 206d 6f64 6966 6965           modifie
-00009550: 6420 696d 6167 6573 2e20 5468 6520 7572  d images. The ur
-00009560: 6c73 206f 6620 7468 6520 6d6f 6469 6669  ls of the modifi
-00009570: 6564 2069 6d61 6765 7320 6172 6520 7265  ed images are re
-00009580: 706c 6163 6564 2077 6974 680a 2020 2020  placed with.    
-00009590: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
-000095a0: 7572 6c73 2e0a 2020 2020 2020 2020 3a72  urls..        :r
-000095b0: 7479 7065 3a20 4461 7461 7365 740a 2020  type: Dataset.  
-000095c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000095d0: 2020 2073 656c 662e 7275 6e6e 696e 675f     self.running_
-000095e0: 6461 7461 203d 2073 656c 662e 6765 745f  data = self.get_
-000095f0: 6461 7461 2869 6e64 6963 6573 290a 0a20  data(indices).. 
-00009600: 2020 2020 2020 205f 6469 7220 3d20 7365         _dir = se
-00009610: 6c66 2e64 6972 2069 6620 5f64 6972 2069  lf.dir if _dir i
-00009620: 7320 4e6f 6e65 2065 6c73 6520 5f64 6972  s None else _dir
-00009630: 0a0a 2020 2020 2020 2020 6f73 2e6d 616b  ..        os.mak
-00009640: 6564 6972 7328 5f64 6972 2c20 6578 6973  edirs(_dir, exis
-00009650: 745f 6f6b 3d54 7275 6529 0a0a 2020 2020  t_ok=True)..    
-00009660: 2020 2020 7465 6d70 5f64 6972 203d 206f      temp_dir = o
-00009670: 732e 7061 7468 2e6a 6f69 6e28 5f64 6972  s.path.join(_dir
-00009680: 2c20 2274 656d 705f 6469 7222 290a 0a20  , "temp_dir").. 
-00009690: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
-000096a0: 7273 2874 656d 705f 6469 722c 2065 7869  rs(temp_dir, exi
-000096b0: 7374 5f6f 6b3d 5472 7565 290a 0a20 2020  st_ok=True)..   
-000096c0: 2020 2020 2069 6620 7365 6c66 2e5f 696e       if self._in
-000096d0: 5f6d 656d 6f72 793a 0a20 2020 2020 2020  _memory:.       
-000096e0: 2020 2020 206e 6577 5f64 6174 6120 3d20       new_data = 
-000096f0: 7468 7265 7368 6f6c 645f 7265 6d6f 7661  threshold_remova
-00009700: 6c28 7365 6c66 2e72 756e 6e69 6e67 5f64  l(self.running_d
-00009710: 6174 612c 2062 6f74 746f 6d2c 2074 6f70  ata, bottom, top
-00009720: 292e 7669 6577 2844 6174 6129 0a20 2020  ).view(Data).   
-00009730: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
-00009740: 612e 7361 7665 286f 732e 7061 7468 2e6a  a.save(os.path.j
-00009750: 6f69 6e28 7465 6d70 5f64 6972 2c20 2264  oin(temp_dir, "d
-00009760: 6174 612e 6864 6635 2229 290a 2020 2020  ata.hdf5")).    
-00009770: 2020 2020 2020 2020 7572 6c73 203d 206e          urls = n
-00009780: 6577 5f64 6174 612e 7572 6c73 0a20 2020  ew_data.urls.   
-00009790: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000097a0: 2020 2020 2020 2075 726c 7320 3d20 7365         urls = se
-000097b0: 6c66 2e72 756e 6e69 6e67 5f64 6174 612e  lf.running_data.
-000097c0: 6170 706c 795f 6675 6e63 7328 0a20 2020  apply_funcs(.   
-000097d0: 2020 2020 2020 2020 2020 2020 205b 2874               [(t
-000097e0: 6872 6573 686f 6c64 5f72 656d 6f76 616c  hreshold_removal
-000097f0: 2c20 5b62 6f74 746f 6d2c 2074 6f70 5d29  , [bottom, top])
-00009800: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00009810: 2020 2073 6176 653d 6f73 2e70 6174 682e     save=os.path.
-00009820: 6a6f 696e 2874 656d 705f 6469 722c 2022  join(temp_dir, "
-00009830: 6461 7461 2e68 6466 3522 292c 0a20 2020  data.hdf5"),.   
-00009840: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-00009850: 743d 2241 7070 6c79 696e 6720 7468 7265  t="Applying thre
-00009860: 7368 6f6c 6422 2c0a 2020 2020 2020 2020  shold",.        
-00009870: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-00009880: 6e3d 4f70 6572 6174 696f 6e2e 5448 5245  n=Operation.THRE
-00009890: 5348 4f4c 442c 0a20 2020 2020 2020 2020  SHOLD,.         
-000098a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000098b0: 2069 6620 7572 6c73 2069 7320 4e6f 6e65   if urls is None
-000098c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000098d0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000098e0: 2069 6620 696e 6469 6365 7320 6973 206e   if indices is n
-000098f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00009900: 2020 2020 206e 6577 5f75 726c 7320 3d20       new_urls = 
-00009910: 6e75 6d70 792e 6172 7261 7928 7365 6c66  numpy.array(self
-00009920: 2e67 6574 5f64 6174 6128 292e 7572 6c73  .get_data().urls
-00009930: 2c20 6474 7970 653d 6f62 6a65 6374 290a  , dtype=object).
-00009940: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00009950: 7572 6c73 5b69 6e64 6963 6573 5d20 3d20  urls[indices] = 
-00009960: 7572 6c73 0a20 2020 2020 2020 2020 2020  urls.           
-00009970: 206e 6577 5f64 6174 6120 3d20 4461 7461   new_data = Data
-00009980: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00009990: 2020 6e65 775f 7572 6c73 2e72 6573 6861    new_urls.resha
-000099a0: 7065 2873 656c 662e 6461 7461 2e75 726c  pe(self.data.url
-000099b0: 732e 7368 6170 6529 2c0a 2020 2020 2020  s.shape),.      
-000099c0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000099d0: 6174 612e 6d65 7461 6461 7461 2c0a 2020  ata.metadata,.  
-000099e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000099f0: 6c66 2e5f 696e 5f6d 656d 6f72 792c 0a20  lf._in_memory,. 
-00009a00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00009a10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00009a20: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
-00009a30: 3d20 4461 7461 280a 2020 2020 2020 2020  = Data(.        
-00009a40: 2020 2020 2020 2020 7572 6c73 2e72 6573          urls.res
-00009a50: 6861 7065 2873 656c 662e 6461 7461 2e75  hape(self.data.u
-00009a60: 726c 732e 7368 6170 6529 2c20 7365 6c66  rls.shape), self
-00009a70: 2e64 6174 612e 6d65 7461 6461 7461 2c20  .data.metadata, 
-00009a80: 7365 6c66 2e5f 696e 5f6d 656d 6f72 790a  self._in_memory.
-00009a90: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00009aa0: 2020 2020 2020 206e 6577 5f64 6174 612e         new_data.
-00009ab0: 7361 7665 286f 732e 7061 7468 2e6a 6f69  save(os.path.joi
-00009ac0: 6e28 5f64 6972 2c20 2264 6174 612e 6864  n(_dir, "data.hd
-00009ad0: 6635 2229 2c20 696e 6469 6365 733d 696e  f5"), indices=in
-00009ae0: 6469 6365 7329 0a20 2020 2020 2020 2074  dices).        t
-00009af0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00009b00: 6f73 2e72 656d 6f76 6528 6f73 2e70 6174  os.remove(os.pat
-00009b10: 682e 6a6f 696e 2874 656d 705f 6469 722c  h.join(temp_dir,
-00009b20: 2022 6461 7461 2e68 6466 3522 2929 0a20   "data.hdf5")). 
-00009b30: 2020 2020 2020 2020 2020 206f 732e 726d             os.rm
-00009b40: 6469 7228 7465 6d70 5f64 6972 290a 2020  dir(temp_dir).  
-00009b50: 2020 2020 2020 6578 6365 7074 204f 5345        except OSE
-00009b60: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-00009b70: 2020 2020 2020 205f 6c6f 6767 6572 2e77         _logger.w
-00009b80: 6172 6e69 6e67 2822 4572 726f 723a 2025  arning("Error: %
-00009b90: 7322 2025 2028 652e 7374 7265 7272 6f72  s" % (e.strerror
-00009ba0: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
-00009bb0: 726e 2044 6174 6173 6574 280a 2020 2020  rn Dataset(.    
-00009bc0: 2020 2020 2020 2020 5f64 6972 3d5f 6469          _dir=_di
-00009bd0: 722c 0a20 2020 2020 2020 2020 2020 2064  r,.            d
-00009be0: 6174 613d 6e65 775f 6461 7461 2c0a 2020  ata=new_data,.  
-00009bf0: 2020 2020 2020 2020 2020 6469 6d73 3d73            dims=s
-00009c00: 656c 662e 5f5f 6469 6d73 2c0a 2020 2020  elf.__dims,.    
-00009c10: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-00009c20: 6d61 7469 6f6e 3d73 656c 662e 7472 616e  mation=self.tran
-00009c30: 7366 6f72 6d61 7469 6f6e 2c0a 2020 2020  sformation,.    
-00009c40: 2020 2020 2020 2020 696e 5f6d 656d 6f72          in_memor
-00009c50: 793d 7365 6c66 2e5f 696e 5f6d 656d 6f72  y=self._in_memor
-00009c60: 792c 0a20 2020 2020 2020 2020 2020 2074  y,.            t
-00009c70: 6974 6c65 3d73 656c 662e 7469 746c 652c  itle=self.title,
-00009c80: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00009c90: 6465 6620 6170 706c 795f 6d61 736b 5f72  def apply_mask_r
-00009ca0: 656d 6f76 616c 2873 656c 662c 206d 6173  emoval(self, mas
-00009cb0: 6b2c 2069 6e64 6963 6573 3d4e 6f6e 652c  k, indices=None,
-00009cc0: 205f 6469 723d 4e6f 6e65 293a 0a20 2020   _dir=None):.   
-00009cd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009ce0: 2041 7070 6c69 6573 206d 6173 6b20 746f   Applies mask to
-00009cf0: 2044 6174 612c 2061 6e64 2073 6176 6573   Data, and saves
-00009d00: 2074 6865 206e 6577 2064 6174 6120 696e   the new data in
-00009d10: 746f 2064 6973 6b2e 0a0a 2020 2020 2020  to disk...      
-00009d20: 2020 3a70 6172 616d 206e 642e 6172 7261    :param nd.arra
-00009d30: 7920 6d61 736b 3a20 4d61 736b 2074 6f20  y mask: Mask to 
-00009d40: 6170 706c 7920 7769 7468 2030 2773 206f  apply with 0's o
-00009d50: 6e20 7468 6520 6d61 736b 2e0a 2020 2020  n the mask..    
-00009d60: 2020 2020 3a70 6172 616d 2069 6e64 6963      :param indic
-00009d70: 6573 3a20 496e 6469 6365 7320 6f66 2074  es: Indices of t
-00009d80: 6865 2069 6d61 6765 7320 746f 2061 7070  he images to app
-00009d90: 6c79 2062 6163 6b67 726f 756e 6420 7375  ly background su
-00009da0: 6274 7261 6374 696f 6e2e 0a20 2020 2020  btraction..     
-00009db0: 2020 2020 2020 2049 6620 4e6f 6e65 2c20         If None, 
-00009dc0: 7468 6520 686f 7420 7069 7865 6c20 7265  the hot pixel re
-00009dd0: 6d6f 7661 6c20 6973 2061 7070 6c69 6564  moval is applied
-00009de0: 2074 6f20 616c 6c20 7468 6520 6461 7461   to all the data
-00009df0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00009e00: 696e 6469 6365 733a 2055 6e69 6f6e 5b4e  indices: Union[N
-00009e10: 6f6e 652c 2061 7272 6179 5f6c 696b 655d  one, array_like]
-00009e20: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00009e30: 3a20 6461 7461 7365 7420 7769 7468 2064  : dataset with d
-00009e40: 6174 6120 6f66 2073 616d 6520 7369 7a65  ata of same size
-00009e50: 2061 7320 6073 656c 662e 6461 7461 6020   as `self.data` 
-00009e60: 6275 7420 7769 7468 2074 6865 0a20 2020  but with the.   
-00009e70: 2020 2020 2020 2020 206d 6f64 6966 6965           modifie
-00009e80: 6420 696d 6167 6573 2e20 5468 6520 7572  d images. The ur
-00009e90: 6c73 206f 6620 7468 6520 6d6f 6469 6669  ls of the modifi
-00009ea0: 6564 2069 6d61 6765 7320 6172 6520 7265  ed images are re
-00009eb0: 706c 6163 6564 2077 6974 680a 2020 2020  placed with.    
-00009ec0: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
-00009ed0: 7572 6c73 2e0a 2020 2020 2020 2020 3a72  urls..        :r
-00009ee0: 7479 7065 3a20 4461 7461 7365 740a 2020  type: Dataset.  
-00009ef0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00009f00: 2020 2069 6620 6e6f 7420 6e75 6d70 792e     if not numpy.
-00009f10: 616e 7928 6d61 736b 293a 0a20 2020 2020  any(mask):.     
-00009f20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009f30: 6c66 0a0a 2020 2020 2020 2020 7365 6c66  lf..        self
-00009f40: 2e72 756e 6e69 6e67 5f64 6174 6120 3d20  .running_data = 
-00009f50: 7365 6c66 2e67 6574 5f64 6174 6128 696e  self.get_data(in
-00009f60: 6469 6365 7329 0a0a 2020 2020 2020 2020  dices)..        
-00009f70: 5f64 6972 203d 2073 656c 662e 6469 7220  _dir = self.dir 
-00009f80: 6966 205f 6469 7220 6973 204e 6f6e 6520  if _dir is None 
-00009f90: 656c 7365 205f 6469 720a 0a20 2020 2020  else _dir..     
-00009fa0: 2020 206f 732e 6d61 6b65 6469 7273 285f     os.makedirs(_
-00009fb0: 6469 722c 2065 7869 7374 5f6f 6b3d 5472  dir, exist_ok=Tr
-00009fc0: 7565 290a 0a20 2020 2020 2020 2074 656d  ue)..        tem
-00009fd0: 705f 6469 7220 3d20 6f73 2e70 6174 682e  p_dir = os.path.
-00009fe0: 6a6f 696e 285f 6469 722c 2022 7465 6d70  join(_dir, "temp
-00009ff0: 5f64 6972 2229 0a0a 2020 2020 2020 2020  _dir")..        
-0000a000: 6f73 2e6d 616b 6564 6972 7328 7465 6d70  os.makedirs(temp
-0000a010: 5f64 6972 2c20 6578 6973 745f 6f6b 3d54  _dir, exist_ok=T
-0000a020: 7275 6529 0a0a 2020 2020 2020 2020 6966  rue)..        if
-0000a030: 2073 656c 662e 5f69 6e5f 6d65 6d6f 7279   self._in_memory
-0000a040: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-0000a050: 775f 6461 7461 203d 206d 6173 6b5f 7265  w_data = mask_re
-0000a060: 6d6f 7661 6c28 7365 6c66 2e72 756e 6e69  moval(self.runni
-0000a070: 6e67 5f64 6174 612c 206d 6173 6b29 2e76  ng_data, mask).v
-0000a080: 6965 7728 4461 7461 290a 2020 2020 2020  iew(Data).      
-0000a090: 2020 2020 2020 6e65 775f 6461 7461 2e73        new_data.s
-0000a0a0: 6176 6528 6f73 2e70 6174 682e 6a6f 696e  ave(os.path.join
-0000a0b0: 2874 656d 705f 6469 722c 2022 6461 7461  (temp_dir, "data
-0000a0c0: 2e68 6466 3522 2929 0a20 2020 2020 2020  .hdf5")).       
-0000a0d0: 2020 2020 2075 726c 7320 3d20 6e65 775f       urls = new_
-0000a0e0: 6461 7461 2e75 726c 730a 2020 2020 2020  data.urls.      
-0000a0f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a100: 2020 2020 7572 6c73 203d 2073 656c 662e      urls = self.
-0000a110: 7275 6e6e 696e 675f 6461 7461 2e61 7070  running_data.app
-0000a120: 6c79 5f66 756e 6373 280a 2020 2020 2020  ly_funcs(.      
-0000a130: 2020 2020 2020 2020 2020 5b28 6d61 736b            [(mask
-0000a140: 5f72 656d 6f76 616c 2c20 5b6d 6173 6b5d  _removal, [mask]
-0000a150: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-0000a160: 2020 2020 7361 7665 3d6f 732e 7061 7468      save=os.path
-0000a170: 2e6a 6f69 6e28 7465 6d70 5f64 6972 2c20  .join(temp_dir, 
-0000a180: 2264 6174 612e 6864 6635 2229 2c0a 2020  "data.hdf5"),.  
-0000a190: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000a1a0: 7874 3d22 5265 6d6f 7669 6e67 206d 6173  xt="Removing mas
-0000a1b0: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
-0000a1c0: 2020 2020 6f70 6572 6174 696f 6e3d 4f70      operation=Op
-0000a1d0: 6572 6174 696f 6e2e 4d41 534b 2c0a 2020  eration.MASK,.  
-0000a1e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000a1f0: 2020 2020 2020 2020 6966 2075 726c 7320          if urls 
-0000a200: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000a210: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000a220: 2020 2020 2020 2020 6966 2069 6e64 6963          if indic
-0000a230: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-0000a240: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000a250: 7572 6c73 203d 206e 756d 7079 2e61 7272  urls = numpy.arr
-0000a260: 6179 2873 656c 662e 6765 745f 6461 7461  ay(self.get_data
-0000a270: 2829 2e75 726c 732c 2064 7479 7065 3d6f  ().urls, dtype=o
-0000a280: 626a 6563 7429 0a20 2020 2020 2020 2020  bject).         
-0000a290: 2020 206e 6577 5f75 726c 735b 696e 6469     new_urls[indi
-0000a2a0: 6365 735d 203d 2075 726c 730a 2020 2020  ces] = urls.    
-0000a2b0: 2020 2020 2020 2020 6e65 775f 6461 7461          new_data
-0000a2c0: 203d 2044 6174 6128 0a20 2020 2020 2020   = Data(.       
-0000a2d0: 2020 2020 2020 2020 206e 6577 5f75 726c           new_url
-0000a2e0: 732e 7265 7368 6170 6528 7365 6c66 2e64  s.reshape(self.d
-0000a2f0: 6174 612e 7572 6c73 2e73 6861 7065 292c  ata.urls.shape),
-0000a300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a310: 2073 656c 662e 6461 7461 2e6d 6574 6164   self.data.metad
-0000a320: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000a330: 2020 2020 2073 656c 662e 5f69 6e5f 6d65       self._in_me
-0000a340: 6d6f 7279 2c0a 2020 2020 2020 2020 2020  mory,.          
-0000a350: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-0000a360: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-0000a370: 775f 6461 7461 203d 2044 6174 6128 0a20  w_data = Data(. 
-0000a380: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0000a390: 726c 732e 7265 7368 6170 6528 7365 6c66  rls.reshape(self
-0000a3a0: 2e64 6174 612e 7572 6c73 2e73 6861 7065  .data.urls.shape
-0000a3b0: 292c 2073 656c 662e 6461 7461 2e6d 6574  ), self.data.met
-0000a3c0: 6164 6174 612c 2073 656c 662e 5f69 6e5f  adata, self._in_
-0000a3d0: 6d65 6d6f 7279 0a20 2020 2020 2020 2020  memory.         
-0000a3e0: 2020 2029 0a0a 2020 2020 2020 2020 6e65     )..        ne
-0000a3f0: 775f 6461 7461 2e73 6176 6528 6f73 2e70  w_data.save(os.p
-0000a400: 6174 682e 6a6f 696e 285f 6469 722c 2022  ath.join(_dir, "
-0000a410: 6461 7461 2e68 6466 3522 292c 2069 6e64  data.hdf5"), ind
-0000a420: 6963 6573 3d69 6e64 6963 6573 290a 2020  ices=indices).  
-0000a430: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000a440: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
-0000a450: 286f 732e 7061 7468 2e6a 6f69 6e28 7465  (os.path.join(te
-0000a460: 6d70 5f64 6972 2c20 2264 6174 612e 6864  mp_dir, "data.hd
-0000a470: 6635 2229 290a 2020 2020 2020 2020 2020  f5")).          
-0000a480: 2020 6f73 2e72 6d64 6972 2874 656d 705f    os.rmdir(temp_
-0000a490: 6469 7229 0a20 2020 2020 2020 2065 7863  dir).        exc
-0000a4a0: 6570 7420 4f53 4572 726f 7220 6173 2065  ept OSError as e
-0000a4b0: 3a0a 2020 2020 2020 2020 2020 2020 5f6c  :.            _l
-0000a4c0: 6f67 6765 722e 7761 726e 696e 6728 2245  ogger.warning("E
-0000a4d0: 7272 6f72 3a20 2573 2220 2520 2865 2e73  rror: %s" % (e.s
-0000a4e0: 7472 6572 726f 7229 290a 0a20 2020 2020  trerror))..     
-0000a4f0: 2020 2072 6574 7572 6e20 4461 7461 7365     return Datase
-0000a500: 7428 0a20 2020 2020 2020 2020 2020 205f  t(.            _
-0000a510: 6469 723d 5f64 6972 2c0a 2020 2020 2020  dir=_dir,.      
-0000a520: 2020 2020 2020 6461 7461 3d6e 6577 5f64        data=new_d
-0000a530: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-0000a540: 2064 696d 733d 7365 6c66 2e5f 5f64 696d   dims=self.__dim
-0000a550: 732c 0a20 2020 2020 2020 2020 2020 2074  s,.            t
-0000a560: 7261 6e73 666f 726d 6174 696f 6e3d 7365  ransformation=se
-0000a570: 6c66 2e74 7261 6e73 666f 726d 6174 696f  lf.transformatio
-0000a580: 6e2c 0a20 2020 2020 2020 2020 2020 2069  n,.            i
-0000a590: 6e5f 6d65 6d6f 7279 3d73 656c 662e 5f69  n_memory=self._i
-0000a5a0: 6e5f 6d65 6d6f 7279 2c0a 2020 2020 2020  n_memory,.      
-0000a5b0: 2020 2020 2020 7469 746c 653d 7365 6c66        title=self
-0000a5c0: 2e74 6974 6c65 2c0a 2020 2020 2020 2020  .title,.        
-0000a5d0: 290a 0a20 2020 2064 6566 2061 7070 6c79  )..    def apply
-0000a5e0: 5f72 6f69 280a 2020 2020 2020 2020 7365  _roi(.        se
-0000a5f0: 6c66 2c20 6f72 6967 696e 3d4e 6f6e 652c  lf, origin=None,
-0000a600: 2073 697a 653d 4e6f 6e65 2c20 6365 6e74   size=None, cent
-0000a610: 6572 3d4e 6f6e 652c 2069 6e64 6963 6573  er=None, indices
-0000a620: 3d4e 6f6e 652c 2072 6f69 5f64 6972 3d4e  =None, roi_dir=N
-0000a630: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
-0000a640: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
-0000a650: 7070 6c69 6573 2061 2072 6567 696f 6e20  pplies a region 
-0000a660: 6f66 2069 6e74 6572 6573 7420 746f 2074  of interest to t
-0000a670: 6865 2064 6174 612e 0a0a 2020 2020 2020  he data...      
-0000a680: 2020 3a70 6172 616d 206f 7269 6769 6e3a    :param origin:
-0000a690: 204f 7269 6769 6e20 6f66 2074 6865 2072   Origin of the r
-0000a6a0: 6f69 0a20 2020 2020 2020 203a 7061 7261  oi.        :para
-0000a6b0: 6d20 7369 7a65 3a20 5b48 6569 6768 742c  m size: [Height,
-0000a6c0: 2057 6964 7468 5d20 6f66 2074 6865 2072   Width] of the r
-0000a6d0: 6f69 2e0a 2020 2020 2020 2020 3a70 6172  oi..        :par
-0000a6e0: 616d 2063 656e 7465 723a 2043 656e 7465  am center: Cente
-0000a6f0: 7220 6f66 2074 6865 2072 6f69 0a20 2020  r of the roi.   
-0000a700: 2020 2020 203a 7479 7065 206f 7269 6769       :type origi
-0000a710: 6e3a 2055 6e69 6f6e 5b32 6420 7665 6374  n: Union[2d vect
-0000a720: 6f72 2c20 4e6f 6e65 5d0a 2020 2020 2020  or, None].      
-0000a730: 2020 3a74 7970 6520 6365 6e74 6572 3a20    :type center: 
-0000a740: 556e 696f 6e5b 3264 2076 6563 746f 722c  Union[2d vector,
-0000a750: 204e 6f6e 655d 0a20 2020 2020 2020 203a   None].        :
-0000a760: 7479 7065 2073 697a 653a 2055 6e69 6f6e  type size: Union
-0000a770: 5b32 6420 7665 6374 6f72 2c20 4e6f 6e65  [2d vector, None
-0000a780: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-0000a790: 2069 6e64 6963 6573 3a20 496e 6469 6365   indices: Indice
-0000a7a0: 7320 6f66 2074 6865 2069 6d61 6765 7320  s of the images 
-0000a7b0: 746f 2061 7070 6c79 2062 6163 6b67 726f  to apply backgro
-0000a7c0: 756e 6420 7375 6274 7261 6374 696f 6e2e  und subtraction.
-0000a7d0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000a7e0: 4e6f 6e65 2c20 7468 6520 726f 6920 6973  None, the roi is
-0000a7f0: 2061 7070 6c69 6564 2074 6f20 616c 6c20   applied to all 
-0000a800: 7468 6520 6461 7461 2e0a 2020 2020 2020  the data..      
-0000a810: 2020 3a74 7970 6520 696e 6469 6365 733a    :type indices:
-0000a820: 2055 6e69 6f6e 5b4e 6f6e 652c 2061 7272   Union[None, arr
-0000a830: 6179 5f6c 696b 655d 0a20 2020 2020 2020  ay_like].       
-0000a840: 203a 7061 7261 6d20 726f 695f 6469 723a   :param roi_dir:
-0000a850: 2044 6972 6563 746f 7279 2070 6174 6820   Directory path 
-0000a860: 666f 7220 7468 6520 6e65 7720 6461 7461  for the new data
-0000a870: 7365 740a 2020 2020 2020 2020 3a74 7970  set.        :typ
-0000a880: 6520 726f 695f 6469 723a 2073 7472 0a20  e roi_dir: str. 
-0000a890: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
-0000a8a0: 2064 6174 6173 6574 2077 6974 6820 6461   dataset with da
-0000a8b0: 7461 2077 6974 6820 726f 6920 6170 706c  ta with roi appl
-0000a8c0: 6965 642e 0a20 2020 2020 2020 2020 2020  ied..           
-0000a8d0: 204e 6f74 653a 2054 6f20 7072 6573 6572   Note: To preser
-0000a8e0: 7665 2063 6f6e 7369 7374 656e 6365 206f  ve consistence o
-0000a8f0: 6620 7368 6170 6520 6265 7477 6565 6e20  f shape between 
-0000a900: 696d 6167 6573 2c20 6966 2060 696e 6469  images, if `indi
-0000a910: 6365 7360 0a20 2020 2020 2020 2020 2020  ces`.           
-0000a920: 2069 7320 6e6f 7420 4e6f 6e65 2c20 6f6e   is not None, on
-0000a930: 6c79 2074 6865 2064 6174 6120 6d6f 6469  ly the data modi
-0000a940: 6669 6564 2069 7320 7265 7475 726e 6564  fied is returned
-0000a950: 2e0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-0000a960: 3a20 4461 7461 7365 740a 2020 2020 2020  : Dataset.      
-0000a970: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-0000a980: 6f69 5f64 6972 203d 2073 656c 662e 6469  oi_dir = self.di
-0000a990: 7220 6966 2072 6f69 5f64 6972 2069 7320  r if roi_dir is 
-0000a9a0: 4e6f 6e65 2065 6c73 6520 726f 695f 6469  None else roi_di
-0000a9b0: 720a 2020 2020 2020 2020 6f73 2e6d 616b  r.        os.mak
-0000a9c0: 6564 6972 7328 726f 695f 6469 722c 2065  edirs(roi_dir, e
-0000a9d0: 7869 7374 5f6f 6b3d 5472 7565 290a 0a20  xist_ok=True).. 
-0000a9e0: 2020 2020 2020 2073 656c 662e 7275 6e6e         self.runn
-0000a9f0: 696e 675f 6461 7461 203d 2073 656c 662e  ing_data = self.
-0000aa00: 6765 745f 6461 7461 2869 6e64 6963 6573  get_data(indices
-0000aa10: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000aa20: 662e 5f69 6e5f 6d65 6d6f 7279 3a0a 2020  f._in_memory:.  
-0000aa30: 2020 2020 2020 2020 2020 6e65 775f 6461            new_da
-0000aa40: 7461 203d 2028 0a20 2020 2020 2020 2020  ta = (.         
-0000aa50: 2020 2020 2020 2061 7070 6c79 5f33 445f         apply_3D_
-0000aa60: 524f 4928 7365 6c66 2e72 756e 6e69 6e67  ROI(self.running
-0000aa70: 5f64 6174 612c 206f 7269 6769 6e2c 2073  _data, origin, s
-0000aa80: 697a 652c 2063 656e 7465 7229 2e76 6965  ize, center).vie
-0000aa90: 7728 4461 7461 292e 636f 7079 2829 0a20  w(Data).copy(). 
-0000aaa0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000aab0: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
-0000aac0: 612e 7361 7665 286f 732e 7061 7468 2e6a  a.save(os.path.j
-0000aad0: 6f69 6e28 726f 695f 6469 722c 2022 6461  oin(roi_dir, "da
-0000aae0: 7461 2e68 6466 3522 292c 206e 6577 5f73  ta.hdf5"), new_s
-0000aaf0: 6861 7065 3d6e 6577 5f64 6174 612e 7368  hape=new_data.sh
-0000ab00: 6170 6529 0a20 2020 2020 2020 2065 6c73  ape).        els
-0000ab10: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000ab20: 6861 7065 203d 206e 756d 7079 2e61 7070  hape = numpy.app
-0000ab30: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-0000ab40: 2020 2020 205b 7365 6c66 2e72 756e 6e69       [self.runni
-0000ab50: 6e67 5f64 6174 612e 7368 6170 655b 305d  ng_data.shape[0]
-0000ab60: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000ab70: 2020 2061 7070 6c79 5f32 445f 524f 4928     apply_2D_ROI(
-0000ab80: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
-0000ab90: 615b 305d 2c20 6f72 6967 696e 2c20 7369  a[0], origin, si
-0000aba0: 7a65 2c20 6365 6e74 6572 292e 7368 6170  ze, center).shap
-0000abb0: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-0000abc0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
-0000abd0: 7320 3d20 7365 6c66 2e72 756e 6e69 6e67  s = self.running
-0000abe0: 5f64 6174 612e 6170 706c 795f 6675 6e63  _data.apply_func
-0000abf0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-0000ac00: 2020 205b 2861 7070 6c79 5f32 445f 524f     [(apply_2D_RO
-0000ac10: 492c 205b 6f72 6967 696e 2c20 7369 7a65  I, [origin, size
-0000ac20: 2c20 6365 6e74 6572 5d29 5d2c 0a20 2020  , center])],.   
-0000ac30: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0000ac40: 653d 6f73 2e70 6174 682e 6a6f 696e 2872  e=os.path.join(r
-0000ac50: 6f69 5f64 6972 2c20 2264 6174 612e 6864  oi_dir, "data.hd
-0000ac60: 6635 2229 2c0a 2020 2020 2020 2020 2020  f5"),.          
-0000ac70: 2020 2020 2020 7465 7874 3d22 4170 706c        text="Appl
-0000ac80: 7969 6e67 2072 6f69 222c 0a20 2020 2020  ying roi",.     
-0000ac90: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-0000aca0: 7469 6f6e 3d4f 7065 7261 7469 6f6e 2e52  tion=Operation.R
-0000acb0: 4f49 2c0a 2020 2020 2020 2020 2020 2020  OI,.            
-0000acc0: 2020 2020 6e65 775f 7368 6170 653d 7368      new_shape=sh
-0000acd0: 6170 652c 0a20 2020 2020 2020 2020 2020  ape,.           
-0000ace0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000acf0: 6620 7572 6c73 2069 7320 4e6f 6e65 3a0a  f urls is None:.
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad10: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-0000ad20: 2020 206e 6577 5f64 6174 6120 3d20 4461     new_data = Da
-0000ad30: 7461 2875 726c 732c 2073 656c 662e 7275  ta(urls, self.ru
-0000ad40: 6e6e 696e 675f 6461 7461 2e6d 6574 6164  nning_data.metad
-0000ad50: 6174 612c 2073 656c 662e 5f69 6e5f 6d65  ata, self._in_me
-0000ad60: 6d6f 7279 290a 0a20 2020 2020 2020 2074  mory)..        t
-0000ad70: 7261 6e73 666f 726d 6174 696f 6e20 3d20  ransformation = 
-0000ad80: 7365 6c66 2e74 7261 6e73 666f 726d 6174  self.transformat
-0000ad90: 696f 6e0a 2020 2020 2020 2020 6966 2074  ion.        if t
-0000ada0: 7261 6e73 666f 726d 6174 696f 6e20 6973  ransformation is
-0000adb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000adc0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-0000add0: 6174 696f 6e20 3d20 5472 616e 7366 6f72  ation = Transfor
-0000ade0: 6d61 7469 6f6e 280a 2020 2020 2020 2020  mation(.        
-0000adf0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-0000ae00: 6d61 7469 6f6e 2e6b 696e 642c 0a20 2020  mation.kind,.   
-0000ae10: 2020 2020 2020 2020 2020 2020 2061 7070               app
-0000ae20: 6c79 5f32 445f 524f 4928 7472 616e 7366  ly_2D_ROI(transf
-0000ae30: 6f72 6d61 7469 6f6e 2e78 2c20 6f72 6967  ormation.x, orig
-0000ae40: 696e 2c20 7369 7a65 2c20 6365 6e74 6572  in, size, center
-0000ae50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000ae60: 2020 2061 7070 6c79 5f32 445f 524f 4928     apply_2D_ROI(
-0000ae70: 7472 616e 7366 6f72 6d61 7469 6f6e 2e79  transformation.y
-0000ae80: 2c20 6f72 6967 696e 2c20 7369 7a65 2c20  , origin, size, 
-0000ae90: 6365 6e74 6572 292c 0a20 2020 2020 2020  center),.       
-0000aea0: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-0000aeb0: 726d 6174 696f 6e2e 726f 7461 7465 2c0a  rmation.rotate,.
-0000aec0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000aed0: 2020 2020 2020 2069 6620 696e 6469 6365         if indice
-0000aee0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0000aef0: 2020 2020 2020 2073 6861 7065 203d 206c         shape = l
-0000af00: 6973 7428 7365 6c66 2e64 6174 612e 7368  ist(self.data.sh
-0000af10: 6170 6529 5b3a 2d32 5d0a 2020 2020 2020  ape)[:-2].      
-0000af20: 2020 2020 2020 7368 6170 652e 6170 7065        shape.appe
-0000af30: 6e64 286e 6577 5f64 6174 612e 7368 6170  nd(new_data.shap
-0000af40: 655b 2d32 5d29 0a20 2020 2020 2020 2020  e[-2]).         
-0000af50: 2020 2073 6861 7065 2e61 7070 656e 6428     shape.append(
-0000af60: 6e65 775f 6461 7461 2e73 6861 7065 5b2d  new_data.shape[-
-0000af70: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-0000af80: 6e65 775f 6461 7461 203d 206e 6577 5f64  new_data = new_d
-0000af90: 6174 612e 7265 7368 6170 6528 7368 6170  ata.reshape(shap
-0000afa0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-0000afb0: 6e20 4461 7461 7365 7428 0a20 2020 2020  n Dataset(.     
-0000afc0: 2020 2020 2020 205f 6469 723d 726f 695f         _dir=roi_
-0000afd0: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
-0000afe0: 2064 6174 613d 6e65 775f 6461 7461 2c0a   data=new_data,.
-0000aff0: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
-0000b000: 3d73 656c 662e 5f5f 6469 6d73 2c0a 2020  =self.__dims,.  
-0000b010: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-0000b020: 6f72 6d61 7469 6f6e 3d74 7261 6e73 666f  ormation=transfo
-0000b030: 726d 6174 696f 6e2c 0a20 2020 2020 2020  rmation,.       
-0000b040: 2020 2020 2069 6e5f 6d65 6d6f 7279 3d73       in_memory=s
-0000b050: 656c 662e 5f69 6e5f 6d65 6d6f 7279 2c0a  elf._in_memory,.
-0000b060: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-0000b070: 653d 7365 6c66 2e74 6974 6c65 2c0a 2020  e=self.title,.  
-0000b080: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000b090: 2066 696e 645f 7368 6966 7428 7365 6c66   find_shift(self
-0000b0a0: 2c20 6469 6d65 6e73 696f 6e3d 4e6f 6e65  , dimension=None
-0000b0b0: 2c20 7374 6570 733d 3530 2c20 696e 6469  , steps=50, indi
-0000b0c0: 6365 733d 4e6f 6e65 293a 0a20 2020 2020  ces=None):.     
-0000b0d0: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-0000b0e0: 696e 6420 7368 6966 7420 6f66 2074 6865  ind shift of the
-0000b0f0: 2064 6174 6120 6f72 2070 6172 7420 6f66   data or part of
-0000b100: 2069 742e 0a0a 2020 2020 2020 2020 3a70   it...        :p
-0000b110: 6172 616d 2064 696d 656e 7369 6f6e 3a20  aram dimension: 
-0000b120: 5061 7261 6d65 7465 7273 2077 6974 6820  Parameters with 
-0000b130: 7468 6520 706f 7369 7469 6f6e 206f 6620  the position of 
-0000b140: 7468 6520 6461 7461 2069 6e20 7468 6520  the data in the 
-0000b150: 7265 7368 6170 6564 0a20 2020 2020 2020  reshaped.       
-0000b160: 2020 2020 2061 7272 6179 2e0a 2020 2020       array..    
-0000b170: 2020 2020 3a74 7970 6520 6469 6d65 6e73      :type dimens
-0000b180: 696f 6e3a 2055 6e69 6f6e 5b4e 6f6e 652c  ion: Union[None,
-0000b190: 2074 7570 6c65 2c20 6172 7261 795f 6c69   tuple, array_li
-0000b1a0: 6b65 5d0a 2020 2020 2020 2020 3a70 6172  ke].        :par
-0000b1b0: 616d 2066 6c6f 6174 2068 5f6d 6178 3a20  am float h_max: 
-0000b1c0: 5365 6520 6063 6f72 652e 696d 6167 6552  See `core.imageR
-0000b1d0: 6567 6973 7472 6174 696f 6e2e 7368 6966  egistration.shif
-0000b1e0: 745f 6465 7465 6374 696f 6e60 0a20 2020  t_detection`.   
-0000b1f0: 2020 2020 203a 7061 7261 6d20 666c 6f61       :param floa
-0000b200: 7420 685f 7374 6570 3a20 5365 6520 6063  t h_step: See `c
-0000b210: 6f72 652e 696d 6167 6552 6567 6973 7472  ore.imageRegistr
-0000b220: 6174 696f 6e2e 7368 6966 745f 6465 7465  ation.shift_dete
-0000b230: 6374 696f 6e60 0a20 2020 2020 2020 203a  ction`.        :
-0000b240: 7061 7261 6d20 696e 6469 6365 733a 2042  param indices: B
-0000b250: 6f6f 6c65 616e 2069 6e64 6578 206c 6973  oolean index lis
-0000b260: 7420 7769 7468 2054 7275 6520 696e 2074  t with True in t
-0000b270: 6865 2069 6d61 6765 7320 746f 2061 7070  he images to app
-0000b280: 6c79 2074 6865 2073 6869 6674 2074 6f2e  ly the shift to.
-0000b290: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000b2a0: 4e6f 6e65 2c20 7468 6520 686f 7420 7069  None, the hot pi
-0000b2b0: 7865 6c20 7265 6d6f 7661 6c20 6973 2061  xel removal is a
-0000b2c0: 7070 6c69 6564 2074 6f20 616c 6c20 7468  pplied to all th
-0000b2d0: 6520 6461 7461 2e0a 2020 2020 2020 2020  e data..        
-0000b2e0: 3a74 7970 6520 696e 6469 6365 733a 2055  :type indices: U
-0000b2f0: 6e69 6f6e 5b4e 6f6e 652c 2061 7272 6179  nion[None, array
-0000b300: 5f6c 696b 655d 0a20 2020 2020 2020 203a  _like].        :
-0000b310: 7265 7475 726e 733a 2041 7272 6179 2077  returns: Array w
-0000b320: 6974 6820 7368 6966 7420 7065 7220 6672  ith shift per fr
-0000b330: 616d 652e 0a20 2020 2020 2020 2022 2222  ame..        """
-0000b340: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0000b350: 7365 6c66 2e67 6574 5f64 6174 6128 696e  self.get_data(in
-0000b360: 6469 6365 733d 696e 6469 6365 732c 2064  dices=indices, d
-0000b370: 696d 656e 7369 6f6e 3d64 696d 656e 7369  imension=dimensi
-0000b380: 6f6e 290a 2020 2020 2020 2020 7265 7475  on).        retu
-0000b390: 726e 2073 6869 6674 5f64 6574 6563 7469  rn shift_detecti
-0000b3a0: 6f6e 2864 6174 612c 2073 7465 7073 290a  on(data, steps).
-0000b3b0: 0a20 2020 2064 6566 2066 696e 645f 7368  .    def find_sh
-0000b3c0: 6966 745f 616c 6f6e 675f 6469 6d65 6e73  ift_along_dimens
-0000b3d0: 696f 6e28 7365 6c66 2c20 6469 6d65 6e73  ion(self, dimens
-0000b3e0: 696f 6e2c 2073 7465 7073 3d35 302c 2069  ion, steps=50, i
-0000b3f0: 6e64 6963 6573 3d4e 6f6e 6529 3a0a 2020  ndices=None):.  
-0000b400: 2020 2020 2020 7368 6966 7420 3d20 5b5d        shift = []
-0000b410: 0a20 2020 2020 2020 2066 6f72 2076 616c  .        for val
-0000b420: 7565 2069 6e20 7261 6e67 6528 7365 6c66  ue in range(self
-0000b430: 2e64 696d 732e 6765 7428 6469 6d65 6e73  .dims.get(dimens
-0000b440: 696f 6e5b 305d 292e 7369 7a65 293a 0a20  ion[0]).size):. 
-0000b450: 2020 2020 2020 2020 2020 2073 6869 6674             shift
-0000b460: 2e61 7070 656e 6428 7365 6c66 2e66 696e  .append(self.fin
-0000b470: 645f 7368 6966 7428 5b64 696d 656e 7369  d_shift([dimensi
-0000b480: 6f6e 5b30 5d2c 2076 616c 7565 5d2c 2073  on[0], value], s
-0000b490: 7465 7073 2c20 696e 6469 6365 7329 290a  teps, indices)).
-0000b4a0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-0000b4b0: 756d 7079 2e61 7272 6179 2873 6869 6674  umpy.array(shift
-0000b4c0: 290a 0a20 2020 2064 6566 2061 7070 6c79  )..    def apply
-0000b4d0: 5f73 6869 6674 5f61 6c6f 6e67 5f64 696d  _shift_along_dim
-0000b4e0: 656e 7369 6f6e 280a 2020 2020 2020 2020  ension(.        
-0000b4f0: 7365 6c66 2c0a 2020 2020 2020 2020 7368  self,.        sh
-0000b500: 6966 742c 0a20 2020 2020 2020 2064 696d  ift,.        dim
-0000b510: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
-0000b520: 7368 6966 745f 6170 7072 6f61 6368 3d22  shift_approach="
-0000b530: 6666 7422 2c0a 2020 2020 2020 2020 696e  fft",.        in
-0000b540: 6469 6365 733d 4e6f 6e65 2c0a 2020 2020  dices=None,.    
-0000b550: 2020 2020 6361 6c6c 6261 636b 3d4e 6f6e      callback=Non
-0000b560: 652c 0a20 2020 2020 2020 205f 6469 723d  e,.        _dir=
-0000b570: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000b580: 2020 2020 2064 6174 6173 6574 203d 2073       dataset = s
-0000b590: 656c 660a 2020 2020 2020 2020 666f 7220  elf.        for 
-0000b5a0: 7661 6c75 6520 696e 2072 616e 6765 2873  value in range(s
-0000b5b0: 656c 662e 6469 6d73 2e67 6574 2864 696d  elf.dims.get(dim
-0000b5c0: 656e 7369 6f6e 5b30 5d29 2e73 697a 6529  ension[0]).size)
-0000b5d0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-0000b5e0: 7461 2c20 7269 6e64 6963 6573 203d 2073  ta, rindices = s
-0000b5f0: 656c 662e 6765 745f 6461 7461 280a 2020  elf.get_data(.  
-0000b600: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000b610: 6469 6365 733d 696e 6469 6365 732c 2064  dices=indices, d
-0000b620: 696d 656e 7369 6f6e 3d5b 6469 6d65 6e73  imension=[dimens
-0000b630: 696f 6e5b 305d 2c20 7661 6c75 655d 2c20  ion[0], value], 
-0000b640: 7265 7475 726e 5f69 6e64 6963 6573 3d54  return_indices=T
-0000b650: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000b660: 290a 2020 2020 2020 2020 2020 2020 6672  ).            fr
-0000b670: 616d 6573 203d 206e 756d 7079 2e61 7261  ames = numpy.ara
-0000b680: 6e67 6528 0a20 2020 2020 2020 2020 2020  nge(.           
-0000b690: 2020 2020 2073 656c 662e 6765 745f 6461       self.get_da
-0000b6a0: 7461 2869 6e64 6963 6573 3d69 6e64 6963  ta(indices=indic
-0000b6b0: 6573 2c20 6469 6d65 6e73 696f 6e3d 5b64  es, dimension=[d
-0000b6c0: 696d 656e 7369 6f6e 5b30 5d2c 2076 616c  imension[0], val
-0000b6d0: 7565 5d29 2e73 6861 7065 5b30 5d0a 2020  ue]).shape[0].  
-0000b6e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b6f0: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-0000b700: 3d20 6461 7461 7365 742e 6170 706c 795f  = dataset.apply_
-0000b710: 7368 6966 7428 0a20 2020 2020 2020 2020  shift(.         
-0000b720: 2020 2020 2020 206e 756d 7079 2e6f 7574         numpy.out
-0000b730: 6572 2873 6869 6674 5b76 616c 7565 5d2c  er(shift[value],
-0000b740: 2066 7261 6d65 7329 2c0a 2020 2020 2020   frames),.      
-0000b750: 2020 2020 2020 2020 2020 5b64 696d 656e            [dimen
-0000b760: 7369 6f6e 5b30 5d2c 2076 616c 7565 5d2c  sion[0], value],
-0000b770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b780: 2073 6869 6674 5f61 7070 726f 6163 682c   shift_approach,
-0000b790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7a0: 2069 6e64 6963 6573 2c0a 2020 2020 2020   indices,.      
-0000b7b0: 2020 2020 2020 2020 2020 6361 6c6c 6261            callba
-0000b7c0: 636b 2c0a 2020 2020 2020 2020 2020 2020  ck,.            
-0000b7d0: 2020 2020 5f64 6972 2c0a 2020 2020 2020      _dir,.      
-0000b7e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000b7f0: 2072 6574 7572 6e20 6461 7461 7365 740a   return dataset.
-0000b800: 0a20 2020 2064 6566 2061 7070 6c79 5f73  .    def apply_s
-0000b810: 6869 6674 280a 2020 2020 2020 2020 7365  hift(.        se
-0000b820: 6c66 2c0a 2020 2020 2020 2020 7368 6966  lf,.        shif
-0000b830: 742c 0a20 2020 2020 2020 2064 696d 656e  t,.        dimen
-0000b840: 7369 6f6e 3d4e 6f6e 652c 0a20 2020 2020  sion=None,.     
-0000b850: 2020 2073 6869 6674 5f61 7070 726f 6163     shift_approac
-0000b860: 683d 2266 6674 222c 0a20 2020 2020 2020  h="fft",.       
-0000b870: 2069 6e64 6963 6573 3d4e 6f6e 652c 0a20   indices=None,. 
-0000b880: 2020 2020 2020 2063 616c 6c62 6163 6b3d         callback=
-0000b890: 4e6f 6e65 2c0a 2020 2020 2020 2020 5f64  None,.        _d
-0000b8a0: 6972 3d4e 6f6e 652c 0a20 2020 2029 3a0a  ir=None,.    ):.
-0000b8b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b8c0: 2020 2020 4170 706c 7920 7368 6966 7420      Apply shift 
-0000b8d0: 6f66 2074 6865 2064 6174 6120 6f72 2070  of the data or p
-0000b8e0: 6172 7420 6f66 2069 7420 616e 6420 7361  art of it and sa
-0000b8f0: 7665 206e 6577 2064 6174 6120 696e 746f  ve new data into
-0000b900: 2064 6973 6b2e 0a0a 2020 2020 2020 2020   disk...        
-0000b910: 3a70 6172 616d 2061 7272 6179 5f6c 696b  :param array_lik
-0000b920: 6520 7368 6966 743a 2053 6869 6674 2070  e shift: Shift p
-0000b930: 6572 2066 7261 6d65 2e0a 2020 2020 2020  er frame..      
-0000b940: 2020 3a70 6172 616d 2064 696d 656e 7369    :param dimensi
-0000b950: 6f6e 3a20 5061 7261 6d65 7465 7320 7769  on: Parametes wi
-0000b960: 7468 2074 6865 2070 6f73 6974 696f 6e20  th the position 
-0000b970: 6f66 2074 6865 2064 6174 6120 696e 2074  of the data in t
-0000b980: 6865 2072 6573 6861 7065 640a 2020 2020  he reshaped.    
-0000b990: 2020 2020 2020 2020 6172 7261 792e 0a20          array.. 
-0000b9a0: 2020 2020 2020 203a 7479 7065 2064 696d         :type dim
-0000b9b0: 656e 7369 6f6e 3a20 556e 696f 6e5b 4e6f  ension: Union[No
-0000b9c0: 6e65 2c20 7475 706c 652c 2061 7272 6179  ne, tuple, array
-0000b9d0: 5f6c 696b 655d 0a20 2020 2020 2020 203a  _like].        :
-0000b9e0: 7061 7261 6d20 556e 696f 6e5b 2766 6674  param Union['fft
-0000b9f0: 272c 2027 6c69 6e65 6172 275d 2073 6869  ', 'linear'] shi
-0000ba00: 6674 5f61 7070 726f 6163 683a 204d 6574  ft_approach: Met
-0000ba10: 686f 6420 746f 2075 7365 2074 6f20 6170  hod to use to ap
-0000ba20: 706c 7920 7468 6520 7368 6966 742e 0a20  ply the shift.. 
-0000ba30: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-0000ba40: 6469 6365 733a 2042 6f6f 6c65 616e 2069  dices: Boolean i
-0000ba50: 6e64 6578 206c 6973 7420 7769 7468 2054  ndex list with T
-0000ba60: 7275 6520 696e 2074 6865 2069 6d61 6765  rue in the image
-0000ba70: 7320 746f 2061 7070 6c79 2074 6865 2073  s to apply the s
-0000ba80: 6869 6674 2074 6f2e 0a20 2020 2020 2020  hift to..       
-0000ba90: 2020 2020 2049 6620 4e6f 6e65 2c20 7468       If None, th
-0000baa0: 6520 686f 7420 7069 7865 6c20 7265 6d6f  e hot pixel remo
-0000bab0: 7661 6c20 6973 2061 7070 6c69 6564 2074  val is applied t
-0000bac0: 6f20 616c 6c20 7468 6520 6461 7461 2e0a  o all the data..
-0000bad0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-0000bae0: 6469 6365 733a 2055 6e69 6f6e 5b4e 6f6e  dices: Union[Non
-0000baf0: 652c 2061 7272 6179 5f6c 696b 655d 0a20  e, array_like]. 
-0000bb00: 2020 2020 2020 203a 7061 7261 6d20 556e         :param Un
-0000bb10: 696f 6e5b 6675 6e63 7469 6f6e 2c20 4e6f  ion[function, No
-0000bb20: 6e65 5d20 6361 6c6c 6261 636b 3a20 4361  ne] callback: Ca
-0000bb30: 6c6c 6261 636b 0a20 2020 2020 2020 203a  llback.        :
-0000bb40: 7265 7475 726e 733a 2064 6174 6173 6574  returns: dataset
-0000bb50: 2077 6974 6820 6461 7461 206f 6620 7361   with data of sa
-0000bb60: 6d65 2073 697a 6520 6173 2060 7365 6c66  me size as `self
-0000bb70: 2e64 6174 6160 2062 7574 2077 6974 6820  .data` but with 
-0000bb80: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-0000bb90: 6d6f 6469 6669 6564 2069 6d61 6765 732e  modified images.
-0000bba0: 2054 6865 2075 726c 7320 6f66 2074 6865   The urls of the
-0000bbb0: 206d 6f64 6966 6965 6420 696d 6167 6573   modified images
-0000bbc0: 2061 7265 2072 6570 6c61 6365 6420 7769   are replaced wi
-0000bbd0: 7468 0a20 2020 2020 2020 2020 2020 2074  th.            t
-0000bbe0: 6865 206e 6577 2075 726c 732e 0a20 2020  he new urls..   
-0000bbf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bc00: 2061 7373 6572 7420 6c65 6e28 7368 6966   assert len(shif
-0000bc10: 7429 203e 2030 2c20 2253 6869 6674 206c  t) > 0, "Shift l
-0000bc20: 6973 7420 6361 6e27 7420 6265 2065 6d70  ist can't be emp
-0000bc30: 7479 220a 0a20 2020 2020 2020 2069 6620  ty"..        if 
-0000bc40: 6e6f 7420 6e75 6d70 792e 616e 7928 7368  not numpy.any(sh
-0000bc50: 6966 7429 3a0a 2020 2020 2020 2020 2020  ift):.          
-0000bc60: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-0000bc70: 2020 2020 2020 205f 6469 7220 3d20 7365         _dir = se
-0000bc80: 6c66 2e64 6972 2069 6620 5f64 6972 2069  lf.dir if _dir i
-0000bc90: 7320 4e6f 6e65 2065 6c73 6520 5f64 6972  s None else _dir
-0000bca0: 0a0a 2020 2020 2020 2020 6f73 2e6d 616b  ..        os.mak
-0000bcb0: 6564 6972 7328 5f64 6972 2c20 6578 6973  edirs(_dir, exis
-0000bcc0: 745f 6f6b 3d54 7275 6529 0a0a 2020 2020  t_ok=True)..    
-0000bcd0: 2020 2020 6461 7461 2c20 7269 6e64 6963      data, rindic
-0000bce0: 6573 203d 2073 656c 662e 6765 745f 6461  es = self.get_da
-0000bcf0: 7461 2869 6e64 6963 6573 2c20 6469 6d65  ta(indices, dime
-0000bd00: 6e73 696f 6e2c 2072 6574 7572 6e5f 696e  nsion, return_in
-0000bd10: 6469 6365 733d 5472 7565 290a 0a20 2020  dices=True)..   
-0000bd20: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000bd30: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
-0000bd40: 6e73 2e72 756e 5f63 6f6e 7465 7874 284f  ns.run_context(O
-0000bd50: 7065 7261 7469 6f6e 2e53 4849 4654 293a  peration.SHIFT):
-0000bd60: 0a20 2020 2020 2020 2020 2020 205f 6669  .            _fi
-0000bd70: 6c65 203d 204e 6f6e 650a 2020 2020 2020  le = None.      
-0000bd80: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000bd90: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 6669 6c65 6e61 6d65 203d 206f      filename = o
-0000bdc0: 732e 7061 7468 2e6a 6f69 6e28 5f64 6972  s.path.join(_dir
-0000bdd0: 2c20 2264 6174 612e 6864 6635 2229 0a20  , "data.hdf5"). 
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdf0: 2020 205f 6669 6c65 203d 2068 3570 792e     _file = h5py.
-0000be00: 4669 6c65 2866 696c 656e 616d 652c 2022  File(filename, "
-0000be10: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
-0000be20: 2020 2020 6578 6365 7074 204f 5345 7272      except OSErr
-0000be30: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000be40: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-0000be50: 7468 2e65 7869 7374 7328 6669 6c65 6e61  th.exists(filena
-0000be60: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
-0000be70: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-0000be80: 7265 6d6f 7665 2866 696c 656e 616d 6529  remove(filename)
-0000be90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bea0: 2020 2020 205f 6669 6c65 203d 2068 3570       _file = h5p
-0000beb0: 792e 4669 6c65 2866 696c 656e 616d 652c  y.File(filename,
-0000bec0: 2022 7722 290a 2020 2020 2020 2020 2020   "w").          
-0000bed0: 2020 2020 2020 6461 7461 7365 745f 6e61        dataset_na
-0000bee0: 6d65 203d 2022 6461 7461 7365 7422 0a20  me = "dataset". 
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000bf00: 6620 2264 6174 6173 6574 2220 6e6f 7420  f "dataset" not 
-0000bf10: 696e 205f 6669 6c65 3a0a 2020 2020 2020  in _file:.      
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
-0000bf30: 696c 652e 6372 6561 7465 5f64 6174 6173  ile.create_datas
-0000bf40: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000bf50: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-0000bf60: 6173 6574 222c 2073 656c 662e 6765 745f  aset", self.get_
-0000bf70: 6461 7461 2829 2e73 6861 7065 2c20 6474  data().shape, dt
-0000bf80: 7970 653d 7365 6c66 2e64 6174 612e 6474  ype=self.data.dt
-0000bf90: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-0000bfa0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000bfb0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-0000bfc0: 656c 662e 6765 745f 6461 7461 2829 2e73  elf.get_data().s
-0000bfd0: 6861 7065 2021 3d20 5f66 696c 655b 2264  hape != _file["d
-0000bfe0: 6174 6173 6574 225d 2e73 6861 7065 3a0a  ataset"].shape:.
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c000: 2020 2020 6465 6c20 5f66 696c 655b 2264      del _file["d
-0000c010: 6174 6173 6574 225d 0a20 2020 2020 2020  ataset"].       
-0000c020: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
-0000c030: 6c65 2e63 7265 6174 655f 6461 7461 7365  le.create_datase
-0000c040: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000c050: 2020 2020 2020 2020 2020 2022 6461 7461             "data
-0000c060: 7365 7422 2c20 7365 6c66 2e67 6574 5f64  set", self.get_d
-0000c070: 6174 6128 292e 7368 6170 652c 2064 7479  ata().shape, dty
-0000c080: 7065 3d73 656c 662e 6461 7461 2e64 7479  pe=self.data.dty
-0000c090: 7065 0a20 2020 2020 2020 2020 2020 2020  pe.             
-0000c0a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000c0b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0d0: 2020 2064 6174 6173 6574 5f6e 616d 6520     dataset_name 
-0000c0e0: 3d20 2275 7064 6174 655f 6461 7461 7365  = "update_datase
-0000c0f0: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-0000c100: 2020 2020 2020 205f 6669 6c65 2e63 6f70         _file.cop
-0000c110: 7928 2264 6174 6173 6574 222c 2022 7570  y("dataset", "up
-0000c120: 6461 7465 5f64 6174 6173 6574 2229 0a0a  date_dataset")..
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c140: 696f 5f75 7469 6c73 2e61 6476 616e 6365  io_utils.advance
-0000c150: 6d65 6e74 5f64 6973 706c 6179 2830 2c20  ment_display(0, 
-0000c160: 6c65 6e28 6461 7461 292c 2022 4170 706c  len(data), "Appl
-0000c170: 7969 6e67 2073 6869 6674 2229 0a20 2020  ying shift").   
-0000c180: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c190: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
-0000c1a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c1b0: 2020 2020 2020 2020 2020 2023 2043 6f6e             # Con
-0000c1c0: 7665 7274 2064 696d 656e 7369 6f6e 2061  vert dimension a
-0000c1d0: 6e64 2076 616c 7565 2069 6e74 6f20 6c69  nd value into li
-0000c1e0: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
-0000c1f0: 2020 2020 2020 2069 6620 7479 7065 2864         if type(d
-0000c200: 696d 656e 7369 6f6e 5b30 5d29 2069 7320  imension[0]) is 
-0000c210: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
-0000c220: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000c230: 656e 7369 6f6e 5b30 5d20 3d20 5b64 696d  ension[0] = [dim
-0000c240: 656e 7369 6f6e 5b30 5d5d 0a20 2020 2020  ension[0]].     
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 2020 2064 696d 656e 7369 6f6e 5b31 5d20     dimension[1] 
-0000c270: 3d20 5b64 696d 656e 7369 6f6e 5b31 5d5d  = [dimension[1]]
-0000c280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c290: 2020 2020 2075 726c 7320 3d20 5b5d 0a20       urls = []. 
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2b0: 2020 2066 6f72 2069 2c20 6964 7820 696e     for i, idx in
-0000c2c0: 2065 6e75 6d65 7261 7465 2872 696e 6469   enumerate(rindi
-0000c2d0: 6365 7329 3a0a 2020 2020 2020 2020 2020  ces):.          
-0000c2e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c2f0: 206e 6f74 2073 656c 662e 7374 6174 655f   not self.state_
-0000c300: 6f66 5f6f 7065 7261 7469 6f6e 732e 6973  of_operations.is
-0000c310: 5f72 756e 6e69 6e67 284f 7065 7261 7469  _running(Operati
-0000c320: 6f6e 2e53 4849 4654 293a 0a20 2020 2020  on.SHIFT):.     
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2020 2069 6620 2275 7064 6174         if "updat
-0000c350: 655f 6461 7461 7365 7422 2069 6e20 5f66  e_dataset" in _f
-0000c360: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2020 2020 2064 656c 205f 6669 6c65 5b22       del _file["
-0000c390: 7570 6461 7465 5f64 6174 6173 6574 225d  update_dataset"]
-0000c3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c3b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000c3c0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-0000c3d0: 2020 2020 2020 2020 2020 2020 696d 6720              img 
-0000c3e0: 3d20 6170 706c 795f 7368 6966 7428 6461  = apply_shift(da
-0000c3f0: 7461 5b69 5d2c 2073 6869 6674 5b3a 2c20  ta[i], shift[:, 
-0000c400: 695d 2c20 7368 6966 745f 6170 7072 6f61  i], shift_approa
-0000c410: 6368 290a 2020 2020 2020 2020 2020 2020  ch).            
-0000c420: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000c430: 6869 6674 5b3a 2c20 695d 2e61 6c6c 2829  hift[:, i].all()
-0000c440: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 7368 6966 745f 6170 7072 6f61 6368    shift_approach
-0000c470: 203d 2022 6c69 6e65 6172 220a 2020 2020   = "linear".    
-0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c490: 2020 2020 5f66 696c 655b 6461 7461 7365      _file[datase
-0000c4a0: 745f 6e61 6d65 5d5b 6964 785d 203d 2069  t_name][idx] = i
-0000c4b0: 6d67 0a20 2020 2020 2020 2020 2020 2020  mg.             
-0000c4c0: 2020 2020 2020 2020 2020 2075 726c 732e             urls.
-0000c4d0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2020 2020 4461 7461 5572 6c28 0a20 2020      DataUrl(.   
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000c520: 655f 7061 7468 3d5f 6469 7220 2b20 222f  e_path=_dir + "/
-0000c530: 6461 7461 2e68 6466 3522 2c0a 2020 2020  data.hdf5",.    
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000c560: 5f70 6174 683d 222f 6461 7461 7365 7422  _path="/dataset"
-0000c570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000084a0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+000084b0: 745b 315d 203a 2073 7461 7274 5b31 5d20  t[1] : start[1] 
+000084c0: 2b20 6368 756e 6b5f 7368 6170 655b 315d  + chunk_shape[1]
+000084d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008520: 2020 2020 2061 7869 733d 302c 0a20 2020       axis=0,.   
+00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008550: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 2020 2073 7461 7274 5b31 5d20         start[1] 
+00008580: 3d20 6368 756e 6b5f 7368 6170 655b 315d  = chunk_shape[1]
+00008590: 202a 2028 6a20 2b20 3129 0a20 2020 2020   * (j + 1).     
+000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085b0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000085c0: 5b30 5d20 3d20 6368 756e 6b5f 7368 6170  [0] = chunk_shap
+000085d0: 655b 305d 202a 2028 6920 2b20 3129 0a20  e[0] * (i + 1). 
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008600: 7461 7274 5b31 5d20 3d20 300a 0a20 2020  tart[1] = 0..   
+00008610: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00008620: 6e6f 7420 7365 6c66 2e73 7461 7465 5f6f  not self.state_o
+00008630: 665f 6f70 6572 6174 696f 6e73 2e69 735f  f_operations.is_
+00008640: 7275 6e6e 696e 6728 4f70 6572 6174 696f  running(Operatio
+00008650: 6e2e 4253 293a 0a20 2020 2020 2020 2020  n.BS):.         
+00008660: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008670: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00008680: 2020 7572 6c73 203d 2073 656c 662e 7275    urls = self.ru
+00008690: 6e6e 696e 675f 6461 7461 2e61 7070 6c79  nning_data.apply
+000086a0: 5f66 756e 6373 280a 2020 2020 2020 2020  _funcs(.        
+000086b0: 2020 2020 2020 2020 2020 2020 5b28 6261              [(ba
+000086c0: 636b 6772 6f75 6e64 5f73 7562 7472 6163  ckground_subtrac
+000086d0: 7469 6f6e 5f32 442c 205b 6267 5d29 5d2c  tion_2D, [bg])],
+000086e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000086f0: 2020 2020 2073 6176 653d 6f73 2e70 6174       save=os.pat
+00008700: 682e 6a6f 696e 2874 656d 705f 6469 722c  h.join(temp_dir,
+00008710: 2022 6461 7461 2e68 6466 3522 292c 0a20   "data.hdf5"),. 
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2020 2074 6578 743d 2241 7070 6c79 696e     text="Applyin
+00008740: 6720 6261 636b 6772 6f75 6e64 2073 7562  g background sub
+00008750: 7472 6163 7469 6f6e 222c 0a20 2020 2020  traction",.     
+00008760: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00008770: 7065 7261 7469 6f6e 3d4f 7065 7261 7469  peration=Operati
+00008780: 6f6e 2e42 532c 0a20 2020 2020 2020 2020  on.BS,.         
+00008790: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000087a0: 2020 2020 2020 2020 2069 6620 7572 6c73           if urls
+000087b0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000087c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000087d0: 7475 726e 0a0a 2020 2020 2020 2020 2320  turn..        # 
+000087e0: 5365 7420 7572 6c73 2061 7320 7368 6170  Set urls as shap
+000087f0: 6520 616e 6420 6469 6d65 6e73 696f 6e20  e and dimension 
+00008800: 6f66 206f 7269 6769 6e61 6c20 7572 6c73  of original urls
+00008810: 2e0a 2020 2020 2020 2020 6966 2069 6e64  ..        if ind
+00008820: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
+00008830: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00008840: 775f 7572 6c73 203d 206e 756d 7079 2e61  w_urls = numpy.a
+00008850: 7272 6179 2873 656c 662e 6765 745f 6461  rray(self.get_da
+00008860: 7461 2829 2e75 726c 732c 2064 7479 7065  ta().urls, dtype
+00008870: 3d6f 626a 6563 7429 0a20 2020 2020 2020  =object).       
+00008880: 2020 2020 206e 6577 5f75 726c 735b 696e       new_urls[in
+00008890: 6469 6365 735d 203d 2075 726c 730a 2020  dices] = urls.  
+000088a0: 2020 2020 2020 2020 2020 6e65 775f 6461            new_da
+000088b0: 7461 203d 2044 6174 6128 0a20 2020 2020  ta = Data(.     
+000088c0: 2020 2020 2020 2020 2020 206e 6577 5f75             new_u
+000088d0: 726c 732e 7265 7368 6170 6528 7365 6c66  rls.reshape(self
+000088e0: 2e64 6174 612e 7572 6c73 2e73 6861 7065  .data.urls.shape
+000088f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008900: 2020 2073 656c 662e 6461 7461 2e6d 6574     self.data.met
+00008910: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+00008920: 2020 2020 2020 2073 656c 662e 5f69 6e5f         self._in_
+00008930: 6d65 6d6f 7279 2c0a 2020 2020 2020 2020  memory,.        
+00008940: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00008950: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008960: 6e65 775f 6461 7461 203d 2044 6174 6128  new_data = Data(
+00008970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008980: 2075 726c 732e 7265 7368 6170 6528 7365   urls.reshape(se
+00008990: 6c66 2e64 6174 612e 7572 6c73 2e73 6861  lf.data.urls.sha
+000089a0: 7065 292c 2073 656c 662e 6461 7461 2e6d  pe), self.data.m
+000089b0: 6574 6164 6174 612c 2073 656c 662e 5f69  etadata, self._i
+000089c0: 6e5f 6d65 6d6f 7279 0a20 2020 2020 2020  n_memory.       
+000089d0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000089e0: 6e65 775f 6461 7461 2e73 6176 6528 6f73  new_data.save(os
+000089f0: 2e70 6174 682e 6a6f 696e 285f 6469 722c  .path.join(_dir,
+00008a00: 2022 6461 7461 2e68 6466 3522 292c 2069   "data.hdf5"), i
+00008a10: 6e64 6963 6573 3d69 6e64 6963 6573 290a  ndices=indices).
+00008a20: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00008a30: 2020 2020 2020 2020 2020 6f73 2e72 656d            os.rem
+00008a40: 6f76 6528 6f73 2e70 6174 682e 6a6f 696e  ove(os.path.join
+00008a50: 2874 656d 705f 6469 722c 2022 6461 7461  (temp_dir, "data
+00008a60: 2e68 6466 3522 2929 0a20 2020 2020 2020  .hdf5")).       
+00008a70: 2020 2020 206f 732e 726d 6469 7228 7465       os.rmdir(te
+00008a80: 6d70 5f64 6972 290a 2020 2020 2020 2020  mp_dir).        
+00008a90: 6578 6365 7074 204f 5345 7272 6f72 2061  except OSError a
+00008aa0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00008ab0: 205f 6c6f 6767 6572 2e77 6172 6e69 6e67   _logger.warning
+00008ac0: 2822 4572 726f 723a 2025 7322 2025 2028  ("Error: %s" % (
+00008ad0: 652e 7374 7265 7272 6f72 2929 0a0a 2020  e.strerror))..  
+00008ae0: 2020 2020 2020 7265 7475 726e 2044 6174        return Dat
+00008af0: 6173 6574 280a 2020 2020 2020 2020 2020  aset(.          
+00008b00: 2020 5f64 6972 3d5f 6469 722c 0a20 2020    _dir=_dir,.   
+00008b10: 2020 2020 2020 2020 2064 6174 613d 6e65           data=ne
+00008b20: 775f 6461 7461 2c0a 2020 2020 2020 2020  w_data,.        
+00008b30: 2020 2020 6469 6d73 3d73 656c 662e 5f5f      dims=self.__
+00008b40: 6469 6d73 2c0a 2020 2020 2020 2020 2020  dims,.          
+00008b50: 2020 7472 616e 7366 6f72 6d61 7469 6f6e    transformation
+00008b60: 3d73 656c 662e 7472 616e 7366 6f72 6d61  =self.transforma
+00008b70: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+00008b80: 2020 696e 5f6d 656d 6f72 793d 7365 6c66    in_memory=self
+00008b90: 2e5f 696e 5f6d 656d 6f72 792c 0a20 2020  ._in_memory,.   
+00008ba0: 2020 2020 2020 2020 2074 6974 6c65 3d73           title=s
+00008bb0: 656c 662e 7469 746c 652c 0a20 2020 2020  elf.title,.     
+00008bc0: 2020 2029 0a0a 2020 2020 6465 6620 6170     )..    def ap
+00008bd0: 706c 795f 686f 745f 7069 7865 6c5f 7265  ply_hot_pixel_re
+00008be0: 6d6f 7661 6c28 7365 6c66 2c20 6b65 726e  moval(self, kern
+00008bf0: 656c 3d33 2c20 696e 6469 6365 733d 4e6f  el=3, indices=No
+00008c00: 6e65 2c20 5f64 6972 3d4e 6f6e 6529 3a0a  ne, _dir=None):.
+00008c10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008c20: 2020 2020 4170 706c 6965 7320 686f 7420      Applies hot 
+00008c30: 7069 7865 6c20 7265 6d6f 7661 6c20 746f  pixel removal to
+00008c40: 2044 6174 612c 2061 6e64 2073 6176 6573   Data, and saves
+00008c50: 2074 6865 206e 6577 2064 6174 610a 2020   the new data.  
+00008c60: 2020 2020 2020 696e 746f 2064 6973 6b2e        into disk.
+00008c70: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00008c80: 2069 6e74 206b 6572 6e65 6c3a 2073 697a   int kernel: siz
+00008c90: 6520 6f66 2074 6865 206b 6572 6e65 6c20  e of the kernel 
+00008ca0: 7573 6564 2074 6f20 6669 6e64 2074 6865  used to find the
+00008cb0: 2068 6f74 0a20 2020 2020 2020 2020 2020   hot.           
+00008cc0: 2070 6978 656c 732e 0a20 2020 2020 2020   pixels..       
+00008cd0: 203a 7061 7261 6d20 696e 6469 6365 733a   :param indices:
+00008ce0: 2049 6e64 6963 6573 206f 6620 7468 6520   Indices of the 
+00008cf0: 696d 6167 6573 2074 6f20 6170 706c 7920  images to apply 
+00008d00: 6261 636b 6772 6f75 6e64 2073 7562 7472  background subtr
+00008d10: 6163 7469 6f6e 2e0a 2020 2020 2020 2020  action..        
+00008d20: 2020 2020 4966 204e 6f6e 652c 2074 6865      If None, the
+00008d30: 2068 6f74 2070 6978 656c 2072 656d 6f76   hot pixel remov
+00008d40: 616c 2069 7320 6170 706c 6965 6420 746f  al is applied to
+00008d50: 2061 6c6c 2074 6865 2064 6174 612e 0a20   all the data.. 
+00008d60: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
+00008d70: 6963 6573 3a20 556e 696f 6e5b 4e6f 6e65  ices: Union[None
+00008d80: 2c20 6172 7261 795f 6c69 6b65 5d0a 2020  , array_like].  
+00008d90: 2020 2020 2020 3a72 6574 7572 6e3a 2064        :return: d
+00008da0: 6174 6173 6574 2077 6974 6820 6461 7461  ataset with data
+00008db0: 206f 6620 7361 6d65 2073 697a 6520 6173   of same size as
+00008dc0: 2060 7365 6c66 2e64 6174 6160 2062 7574   `self.data` but
+00008dd0: 2077 6974 6820 7468 650a 2020 2020 2020   with the.      
+00008de0: 2020 2020 2020 6d6f 6469 6669 6564 2069        modified i
+00008df0: 6d61 6765 732e 2054 6865 2075 726c 7320  mages. The urls 
+00008e00: 6f66 2074 6865 206d 6f64 6966 6965 6420  of the modified 
+00008e10: 696d 6167 6573 2061 7265 2072 6570 6c61  images are repla
+00008e20: 6365 6420 7769 7468 0a20 2020 2020 2020  ced with.       
+00008e30: 2020 2020 2074 6865 206e 6577 2075 726c       the new url
+00008e40: 732e 0a20 2020 2020 2020 203a 7274 7970  s..        :rtyp
+00008e50: 653a 2044 6174 6173 6574 0a20 2020 2020  e: Dataset.     
+00008e60: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00008e70: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
+00008e80: 6120 3d20 7365 6c66 2e67 6574 5f64 6174  a = self.get_dat
+00008e90: 6128 696e 6469 6365 7329 0a0a 2020 2020  a(indices)..    
+00008ea0: 2020 2020 5f64 6972 203d 2073 656c 662e      _dir = self.
+00008eb0: 6469 7220 6966 205f 6469 7220 6973 204e  dir if _dir is N
+00008ec0: 6f6e 6520 656c 7365 205f 6469 720a 0a20  one else _dir.. 
+00008ed0: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
+00008ee0: 7273 285f 6469 722c 2065 7869 7374 5f6f  rs(_dir, exist_o
+00008ef0: 6b3d 5472 7565 290a 0a20 2020 2020 2020  k=True)..       
+00008f00: 2074 656d 705f 6469 7220 3d20 6f73 2e70   temp_dir = os.p
+00008f10: 6174 682e 6a6f 696e 285f 6469 722c 2022  ath.join(_dir, "
+00008f20: 7465 6d70 5f64 6972 2229 0a0a 2020 2020  temp_dir")..    
+00008f30: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+00008f40: 7465 6d70 5f64 6972 2c20 6578 6973 745f  temp_dir, exist_
+00008f50: 6f6b 3d54 7275 6529 0a0a 2020 2020 2020  ok=True)..      
+00008f60: 2020 6966 2073 656c 662e 5f69 6e5f 6d65    if self._in_me
+00008f70: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
+00008f80: 2020 6e65 775f 6461 7461 203d 2068 6f74    new_data = hot
+00008f90: 5f70 6978 656c 5f72 656d 6f76 616c 5f33  _pixel_removal_3
+00008fa0: 4428 7365 6c66 2e72 756e 6e69 6e67 5f64  D(self.running_d
+00008fb0: 6174 612c 206b 6572 6e65 6c29 2e76 6965  ata, kernel).vie
+00008fc0: 7728 4461 7461 290a 2020 2020 2020 2020  w(Data).        
+00008fd0: 2020 2020 6e65 775f 6461 7461 2e73 6176      new_data.sav
+00008fe0: 6528 6f73 2e70 6174 682e 6a6f 696e 2874  e(os.path.join(t
+00008ff0: 656d 705f 6469 722c 2022 6461 7461 2e68  emp_dir, "data.h
+00009000: 6466 3522 2929 0a20 2020 2020 2020 2020  df5")).         
+00009010: 2020 2075 726c 7320 3d20 6e65 775f 6461     urls = new_da
+00009020: 7461 2e75 726c 730a 2020 2020 2020 2020  ta.urls.        
+00009030: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009040: 2020 7572 6c73 203d 2073 656c 662e 7275    urls = self.ru
+00009050: 6e6e 696e 675f 6461 7461 2e61 7070 6c79  nning_data.apply
+00009060: 5f66 756e 6373 280a 2020 2020 2020 2020  _funcs(.        
+00009070: 2020 2020 2020 2020 5b28 686f 745f 7069          [(hot_pi
+00009080: 7865 6c5f 7265 6d6f 7661 6c5f 3244 2c20  xel_removal_2D, 
+00009090: 5b6b 6572 6e65 6c5d 295d 2c0a 2020 2020  [kernel])],.    
+000090a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000090b0: 3d6f 732e 7061 7468 2e6a 6f69 6e28 7465  =os.path.join(te
+000090c0: 6d70 5f64 6972 2c20 2264 6174 612e 6864  mp_dir, "data.hd
+000090d0: 6635 2229 2c0a 2020 2020 2020 2020 2020  f5"),.          
+000090e0: 2020 2020 2020 7465 7874 3d22 4170 706c        text="Appl
+000090f0: 7969 6e67 2068 6f74 2070 6978 656c 2072  ying hot pixel r
+00009100: 656d 6f76 616c 222c 0a20 2020 2020 2020  emoval",.       
+00009110: 2020 2020 2020 2020 206f 7065 7261 7469           operati
+00009120: 6f6e 3d4f 7065 7261 7469 6f6e 2e48 502c  on=Operation.HP,
+00009130: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00009140: 2020 2020 2020 2020 2020 2069 6620 7572             if ur
+00009150: 6c73 2069 7320 4e6f 6e65 3a0a 2020 2020  ls is None:.    
+00009160: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009170: 726e 0a0a 2020 2020 2020 2020 6966 2069  rn..        if i
+00009180: 6e64 6963 6573 2069 7320 6e6f 7420 4e6f  ndices is not No
+00009190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000091a0: 6e65 775f 7572 6c73 203d 206e 756d 7079  new_urls = numpy
+000091b0: 2e61 7272 6179 2873 656c 662e 6765 745f  .array(self.get_
+000091c0: 6461 7461 2829 2e75 726c 732c 2064 7479  data().urls, dty
+000091d0: 7065 3d6f 626a 6563 7429 0a20 2020 2020  pe=object).     
+000091e0: 2020 2020 2020 206e 6577 5f75 726c 735b         new_urls[
+000091f0: 696e 6469 6365 735d 203d 2075 726c 730a  indices] = urls.
+00009200: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00009210: 6461 7461 203d 2044 6174 6128 0a20 2020  data = Data(.   
+00009220: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00009230: 5f75 726c 732e 7265 7368 6170 6528 7365  _urls.reshape(se
+00009240: 6c66 2e64 6174 612e 7572 6c73 2e73 6861  lf.data.urls.sha
+00009250: 7065 292c 0a20 2020 2020 2020 2020 2020  pe),.           
+00009260: 2020 2020 2073 656c 662e 6461 7461 2e6d       self.data.m
+00009270: 6574 6164 6174 612c 0a20 2020 2020 2020  etadata,.       
+00009280: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
+00009290: 6e5f 6d65 6d6f 7279 2c0a 2020 2020 2020  n_memory,.      
+000092a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000092b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000092c0: 2020 6e65 775f 6461 7461 203d 2044 6174    new_data = Dat
+000092d0: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
+000092e0: 2020 2075 726c 732e 7265 7368 6170 6528     urls.reshape(
+000092f0: 7365 6c66 2e64 6174 612e 7572 6c73 2e73  self.data.urls.s
+00009300: 6861 7065 292c 2073 656c 662e 6461 7461  hape), self.data
+00009310: 2e6d 6574 6164 6174 612c 2073 656c 662e  .metadata, self.
+00009320: 5f69 6e5f 6d65 6d6f 7279 0a20 2020 2020  _in_memory.     
+00009330: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00009340: 2020 6e65 775f 6461 7461 2e73 6176 6528    new_data.save(
+00009350: 6f73 2e70 6174 682e 6a6f 696e 285f 6469  os.path.join(_di
+00009360: 722c 2022 6461 7461 2e68 6466 3522 292c  r, "data.hdf5"),
+00009370: 2069 6e64 6963 6573 3d69 6e64 6963 6573   indices=indices
+00009380: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+00009390: 2020 2020 2020 2020 2020 206f 732e 7265             os.re
+000093a0: 6d6f 7665 286f 732e 7061 7468 2e6a 6f69  move(os.path.joi
+000093b0: 6e28 7465 6d70 5f64 6972 2c20 2264 6174  n(temp_dir, "dat
+000093c0: 612e 6864 6635 2229 290a 2020 2020 2020  a.hdf5")).      
+000093d0: 2020 2020 2020 6f73 2e72 6d64 6972 2874        os.rmdir(t
+000093e0: 656d 705f 6469 7229 0a20 2020 2020 2020  emp_dir).       
+000093f0: 2065 7863 6570 7420 4f53 4572 726f 7220   except OSError 
+00009400: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00009410: 2020 5f6c 6f67 6765 722e 7761 726e 696e    _logger.warnin
+00009420: 6728 2245 7272 6f72 3a20 2573 2220 2520  g("Error: %s" % 
+00009430: 2865 2e73 7472 6572 726f 7229 290a 0a20  (e.strerror)).. 
+00009440: 2020 2020 2020 2072 6574 7572 6e20 4461         return Da
+00009450: 7461 7365 7428 0a20 2020 2020 2020 2020  taset(.         
+00009460: 2020 205f 6469 723d 5f64 6972 2c0a 2020     _dir=_dir,.  
+00009470: 2020 2020 2020 2020 2020 6461 7461 3d6e            data=n
+00009480: 6577 5f64 6174 612c 0a20 2020 2020 2020  ew_data,.       
+00009490: 2020 2020 2064 696d 733d 7365 6c66 2e5f       dims=self._
+000094a0: 5f64 696d 732c 0a20 2020 2020 2020 2020  _dims,.         
+000094b0: 2020 2074 7261 6e73 666f 726d 6174 696f     transformatio
+000094c0: 6e3d 7365 6c66 2e74 7261 6e73 666f 726d  n=self.transform
+000094d0: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+000094e0: 2020 2069 6e5f 6d65 6d6f 7279 3d73 656c     in_memory=sel
+000094f0: 662e 5f69 6e5f 6d65 6d6f 7279 2c0a 2020  f._in_memory,.  
+00009500: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+00009510: 7365 6c66 2e74 6974 6c65 2c0a 2020 2020  self.title,.    
+00009520: 2020 2020 290a 0a20 2020 2064 6566 2061      )..    def a
+00009530: 7070 6c79 5f74 6872 6573 686f 6c64 5f72  pply_threshold_r
+00009540: 656d 6f76 616c 2873 656c 662c 2062 6f74  emoval(self, bot
+00009550: 746f 6d3d 4e6f 6e65 2c20 746f 703d 4e6f  tom=None, top=No
+00009560: 6e65 2c20 696e 6469 6365 733d 4e6f 6e65  ne, indices=None
+00009570: 2c20 5f64 6972 3d4e 6f6e 6529 3a0a 2020  , _dir=None):.  
+00009580: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009590: 2020 4170 706c 6965 7320 626f 7474 6f6d    Applies bottom
+000095a0: 2074 6872 6573 686f 6c64 2074 6f20 4461   threshold to Da
+000095b0: 7461 2c20 616e 6420 7361 7665 7320 7468  ta, and saves th
+000095c0: 6520 6e65 7720 6461 7461 0a20 2020 2020  e new data.     
+000095d0: 2020 2069 6e74 6f20 6469 736b 2e0a 0a20     into disk... 
+000095e0: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+000095f0: 7420 626f 7474 6f6d 3a20 626f 7474 6f6d  t bottom: bottom
+00009600: 2074 6872 6573 686f 6c64 2074 6f20 6170   threshold to ap
+00009610: 706c 792e 0a20 2020 2020 2020 203a 7061  ply..        :pa
+00009620: 7261 6d20 696e 7420 746f 703a 2074 6f70  ram int top: top
+00009630: 2074 6872 6573 686f 6c64 2074 6f20 6170   threshold to ap
+00009640: 706c 792e 0a20 2020 2020 2020 203a 7061  ply..        :pa
+00009650: 7261 6d20 696e 6469 6365 733a 2049 6e64  ram indices: Ind
+00009660: 6963 6573 206f 6620 7468 6520 696d 6167  ices of the imag
+00009670: 6573 2074 6f20 6170 706c 7920 6261 636b  es to apply back
+00009680: 6772 6f75 6e64 2073 7562 7472 6163 7469  ground subtracti
+00009690: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+000096a0: 4966 204e 6f6e 652c 2074 6865 2068 6f74  If None, the hot
+000096b0: 2070 6978 656c 2072 656d 6f76 616c 2069   pixel removal i
+000096c0: 7320 6170 706c 6965 6420 746f 2061 6c6c  s applied to all
+000096d0: 2074 6865 2064 6174 612e 0a20 2020 2020   the data..     
+000096e0: 2020 203a 7479 7065 2069 6e64 6963 6573     :type indices
+000096f0: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 6172  : Union[None, ar
+00009700: 7261 795f 6c69 6b65 5d0a 2020 2020 2020  ray_like].      
+00009710: 2020 3a72 6574 7572 6e3a 2064 6174 6173    :return: datas
+00009720: 6574 2077 6974 6820 6461 7461 206f 6620  et with data of 
+00009730: 7361 6d65 2073 697a 6520 6173 2060 7365  same size as `se
+00009740: 6c66 2e64 6174 6160 2062 7574 2077 6974  lf.data` but wit
+00009750: 6820 7468 650a 2020 2020 2020 2020 2020  h the.          
+00009760: 2020 6d6f 6469 6669 6564 2069 6d61 6765    modified image
+00009770: 732e 2054 6865 2075 726c 7320 6f66 2074  s. The urls of t
+00009780: 6865 206d 6f64 6966 6965 6420 696d 6167  he modified imag
+00009790: 6573 2061 7265 2072 6570 6c61 6365 6420  es are replaced 
+000097a0: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
+000097b0: 2074 6865 206e 6577 2075 726c 732e 0a20   the new urls.. 
+000097c0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+000097d0: 6174 6173 6574 0a20 2020 2020 2020 2022  ataset.        "
+000097e0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000097f0: 2e72 756e 6e69 6e67 5f64 6174 6120 3d20  .running_data = 
+00009800: 7365 6c66 2e67 6574 5f64 6174 6128 696e  self.get_data(in
+00009810: 6469 6365 7329 0a0a 2020 2020 2020 2020  dices)..        
+00009820: 5f64 6972 203d 2073 656c 662e 6469 7220  _dir = self.dir 
+00009830: 6966 205f 6469 7220 6973 204e 6f6e 6520  if _dir is None 
+00009840: 656c 7365 205f 6469 720a 0a20 2020 2020  else _dir..     
+00009850: 2020 206f 732e 6d61 6b65 6469 7273 285f     os.makedirs(_
+00009860: 6469 722c 2065 7869 7374 5f6f 6b3d 5472  dir, exist_ok=Tr
+00009870: 7565 290a 0a20 2020 2020 2020 2074 656d  ue)..        tem
+00009880: 705f 6469 7220 3d20 6f73 2e70 6174 682e  p_dir = os.path.
+00009890: 6a6f 696e 285f 6469 722c 2022 7465 6d70  join(_dir, "temp
+000098a0: 5f64 6972 2229 0a0a 2020 2020 2020 2020  _dir")..        
+000098b0: 6f73 2e6d 616b 6564 6972 7328 7465 6d70  os.makedirs(temp
+000098c0: 5f64 6972 2c20 6578 6973 745f 6f6b 3d54  _dir, exist_ok=T
+000098d0: 7275 6529 0a0a 2020 2020 2020 2020 6966  rue)..        if
+000098e0: 2073 656c 662e 5f69 6e5f 6d65 6d6f 7279   self._in_memory
+000098f0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00009900: 775f 6461 7461 203d 2074 6872 6573 686f  w_data = thresho
+00009910: 6c64 5f72 656d 6f76 616c 2873 656c 662e  ld_removal(self.
+00009920: 7275 6e6e 696e 675f 6461 7461 2c20 626f  running_data, bo
+00009930: 7474 6f6d 2c20 746f 7029 2e76 6965 7728  ttom, top).view(
+00009940: 4461 7461 290a 2020 2020 2020 2020 2020  Data).          
+00009950: 2020 6e65 775f 6461 7461 2e73 6176 6528    new_data.save(
+00009960: 6f73 2e70 6174 682e 6a6f 696e 2874 656d  os.path.join(tem
+00009970: 705f 6469 722c 2022 6461 7461 2e68 6466  p_dir, "data.hdf
+00009980: 3522 2929 0a20 2020 2020 2020 2020 2020  5")).           
+00009990: 2075 726c 7320 3d20 6e65 775f 6461 7461   urls = new_data
+000099a0: 2e75 726c 730a 2020 2020 2020 2020 656c  .urls.        el
+000099b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000099c0: 7572 6c73 203d 2073 656c 662e 7275 6e6e  urls = self.runn
+000099d0: 696e 675f 6461 7461 2e61 7070 6c79 5f66  ing_data.apply_f
+000099e0: 756e 6373 280a 2020 2020 2020 2020 2020  uncs(.          
+000099f0: 2020 2020 2020 5b28 7468 7265 7368 6f6c        [(threshol
+00009a00: 645f 7265 6d6f 7661 6c2c 205b 626f 7474  d_removal, [bott
+00009a10: 6f6d 2c20 746f 705d 295d 2c0a 2020 2020  om, top])],.    
+00009a20: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00009a30: 3d6f 732e 7061 7468 2e6a 6f69 6e28 7465  =os.path.join(te
+00009a40: 6d70 5f64 6972 2c20 2264 6174 612e 6864  mp_dir, "data.hd
+00009a50: 6635 2229 2c0a 2020 2020 2020 2020 2020  f5"),.          
+00009a60: 2020 2020 2020 7465 7874 3d22 4170 706c        text="Appl
+00009a70: 7969 6e67 2074 6872 6573 686f 6c64 222c  ying threshold",
+00009a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a90: 206f 7065 7261 7469 6f6e 3d4f 7065 7261   operation=Opera
+00009aa0: 7469 6f6e 2e54 4852 4553 484f 4c44 2c0a  tion.THRESHOLD,.
+00009ab0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00009ac0: 2020 2020 2020 2020 2020 6966 2075 726c            if url
+00009ad0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+00009ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009af0: 6e0a 2020 2020 2020 2020 6966 2069 6e64  n.        if ind
+00009b00: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
+00009b10: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00009b20: 775f 7572 6c73 203d 206e 756d 7079 2e61  w_urls = numpy.a
+00009b30: 7272 6179 2873 656c 662e 6765 745f 6461  rray(self.get_da
+00009b40: 7461 2829 2e75 726c 732c 2064 7479 7065  ta().urls, dtype
+00009b50: 3d6f 626a 6563 7429 0a20 2020 2020 2020  =object).       
+00009b60: 2020 2020 206e 6577 5f75 726c 735b 696e       new_urls[in
+00009b70: 6469 6365 735d 203d 2075 726c 730a 2020  dices] = urls.  
+00009b80: 2020 2020 2020 2020 2020 6e65 775f 6461            new_da
+00009b90: 7461 203d 2044 6174 6128 0a20 2020 2020  ta = Data(.     
+00009ba0: 2020 2020 2020 2020 2020 206e 6577 5f75             new_u
+00009bb0: 726c 732e 7265 7368 6170 6528 7365 6c66  rls.reshape(self
+00009bc0: 2e64 6174 612e 7572 6c73 2e73 6861 7065  .data.urls.shape
+00009bd0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00009be0: 2020 2073 656c 662e 6461 7461 2e6d 6574     self.data.met
+00009bf0: 6164 6174 612c 0a20 2020 2020 2020 2020  adata,.         
+00009c00: 2020 2020 2020 2073 656c 662e 5f69 6e5f         self._in_
+00009c10: 6d65 6d6f 7279 2c0a 2020 2020 2020 2020  memory,.        
+00009c20: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00009c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009c40: 6e65 775f 6461 7461 203d 2044 6174 6128  new_data = Data(
+00009c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c60: 2075 726c 732e 7265 7368 6170 6528 7365   urls.reshape(se
+00009c70: 6c66 2e64 6174 612e 7572 6c73 2e73 6861  lf.data.urls.sha
+00009c80: 7065 292c 2073 656c 662e 6461 7461 2e6d  pe), self.data.m
+00009c90: 6574 6164 6174 612c 2073 656c 662e 5f69  etadata, self._i
+00009ca0: 6e5f 6d65 6d6f 7279 0a20 2020 2020 2020  n_memory.       
+00009cb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00009cc0: 6e65 775f 6461 7461 2e73 6176 6528 6f73  new_data.save(os
+00009cd0: 2e70 6174 682e 6a6f 696e 285f 6469 722c  .path.join(_dir,
+00009ce0: 2022 6461 7461 2e68 6466 3522 292c 2069   "data.hdf5"), i
+00009cf0: 6e64 6963 6573 3d69 6e64 6963 6573 290a  ndices=indices).
+00009d00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00009d10: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
+00009d20: 7665 286f 732e 7061 7468 2e6a 6f69 6e28  ve(os.path.join(
+00009d30: 7465 6d70 5f64 6972 2c20 2264 6174 612e  temp_dir, "data.
+00009d40: 6864 6635 2229 290a 2020 2020 2020 2020  hdf5")).        
+00009d50: 2020 2020 6f73 2e72 6d64 6972 2874 656d      os.rmdir(tem
+00009d60: 705f 6469 7229 0a20 2020 2020 2020 2065  p_dir).        e
+00009d70: 7863 6570 7420 4f53 4572 726f 7220 6173  xcept OSError as
+00009d80: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00009d90: 5f6c 6f67 6765 722e 7761 726e 696e 6728  _logger.warning(
+00009da0: 2245 7272 6f72 3a20 2573 2220 2520 2865  "Error: %s" % (e
+00009db0: 2e73 7472 6572 726f 7229 290a 0a20 2020  .strerror))..   
+00009dc0: 2020 2020 2072 6574 7572 6e20 4461 7461       return Data
+00009dd0: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
+00009de0: 205f 6469 723d 5f64 6972 2c0a 2020 2020   _dir=_dir,.    
+00009df0: 2020 2020 2020 2020 6461 7461 3d6e 6577          data=new
+00009e00: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+00009e10: 2020 2064 696d 733d 7365 6c66 2e5f 5f64     dims=self.__d
+00009e20: 696d 732c 0a20 2020 2020 2020 2020 2020  ims,.           
+00009e30: 2074 7261 6e73 666f 726d 6174 696f 6e3d   transformation=
+00009e40: 7365 6c66 2e74 7261 6e73 666f 726d 6174  self.transformat
+00009e50: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00009e60: 2069 6e5f 6d65 6d6f 7279 3d73 656c 662e   in_memory=self.
+00009e70: 5f69 6e5f 6d65 6d6f 7279 2c0a 2020 2020  _in_memory,.    
+00009e80: 2020 2020 2020 2020 7469 746c 653d 7365          title=se
+00009e90: 6c66 2e74 6974 6c65 2c0a 2020 2020 2020  lf.title,.      
+00009ea0: 2020 290a 0a20 2020 2064 6566 2061 7070    )..    def app
+00009eb0: 6c79 5f6d 6173 6b5f 7265 6d6f 7661 6c28  ly_mask_removal(
+00009ec0: 7365 6c66 2c20 6d61 736b 2c20 696e 6469  self, mask, indi
+00009ed0: 6365 733d 4e6f 6e65 2c20 5f64 6972 3d4e  ces=None, _dir=N
+00009ee0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
+00009ef0: 220a 2020 2020 2020 2020 4170 706c 6965  ".        Applie
+00009f00: 7320 6d61 736b 2074 6f20 4461 7461 2c20  s mask to Data, 
+00009f10: 616e 6420 7361 7665 7320 7468 6520 6e65  and saves the ne
+00009f20: 7720 6461 7461 2069 6e74 6f20 6469 736b  w data into disk
+00009f30: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00009f40: 6d20 6e64 2e61 7272 6179 206d 6173 6b3a  m nd.array mask:
+00009f50: 204d 6173 6b20 746f 2061 7070 6c79 2077   Mask to apply w
+00009f60: 6974 6820 3027 7320 6f6e 2074 6865 206d  ith 0's on the m
+00009f70: 6173 6b2e 0a20 2020 2020 2020 203a 7061  ask..        :pa
+00009f80: 7261 6d20 696e 6469 6365 733a 2049 6e64  ram indices: Ind
+00009f90: 6963 6573 206f 6620 7468 6520 696d 6167  ices of the imag
+00009fa0: 6573 2074 6f20 6170 706c 7920 6261 636b  es to apply back
+00009fb0: 6772 6f75 6e64 2073 7562 7472 6163 7469  ground subtracti
+00009fc0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+00009fd0: 4966 204e 6f6e 652c 2074 6865 2068 6f74  If None, the hot
+00009fe0: 2070 6978 656c 2072 656d 6f76 616c 2069   pixel removal i
+00009ff0: 7320 6170 706c 6965 6420 746f 2061 6c6c  s applied to all
+0000a000: 2074 6865 2064 6174 612e 0a20 2020 2020   the data..     
+0000a010: 2020 203a 7479 7065 2069 6e64 6963 6573     :type indices
+0000a020: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 6172  : Union[None, ar
+0000a030: 7261 795f 6c69 6b65 5d0a 2020 2020 2020  ray_like].      
+0000a040: 2020 3a72 6574 7572 6e3a 2064 6174 6173    :return: datas
+0000a050: 6574 2077 6974 6820 6461 7461 206f 6620  et with data of 
+0000a060: 7361 6d65 2073 697a 6520 6173 2060 7365  same size as `se
+0000a070: 6c66 2e64 6174 6160 2062 7574 2077 6974  lf.data` but wit
+0000a080: 6820 7468 650a 2020 2020 2020 2020 2020  h the.          
+0000a090: 2020 6d6f 6469 6669 6564 2069 6d61 6765    modified image
+0000a0a0: 732e 2054 6865 2075 726c 7320 6f66 2074  s. The urls of t
+0000a0b0: 6865 206d 6f64 6966 6965 6420 696d 6167  he modified imag
+0000a0c0: 6573 2061 7265 2072 6570 6c61 6365 6420  es are replaced 
+0000a0d0: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
+0000a0e0: 2074 6865 206e 6577 2075 726c 732e 0a20   the new urls.. 
+0000a0f0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+0000a100: 6174 6173 6574 0a20 2020 2020 2020 2022  ataset.        "
+0000a110: 2222 0a0a 2020 2020 2020 2020 6966 206e  ""..        if n
+0000a120: 6f74 206e 756d 7079 2e61 6e79 286d 6173  ot numpy.any(mas
+0000a130: 6b29 3a0a 2020 2020 2020 2020 2020 2020  k):.            
+0000a140: 7265 7475 726e 2073 656c 660a 0a20 2020  return self..   
+0000a150: 2020 2020 2073 656c 662e 7275 6e6e 696e       self.runnin
+0000a160: 675f 6461 7461 203d 2073 656c 662e 6765  g_data = self.ge
+0000a170: 745f 6461 7461 2869 6e64 6963 6573 290a  t_data(indices).
+0000a180: 0a20 2020 2020 2020 205f 6469 7220 3d20  .        _dir = 
+0000a190: 7365 6c66 2e64 6972 2069 6620 5f64 6972  self.dir if _dir
+0000a1a0: 2069 7320 4e6f 6e65 2065 6c73 6520 5f64   is None else _d
+0000a1b0: 6972 0a0a 2020 2020 2020 2020 6f73 2e6d  ir..        os.m
+0000a1c0: 616b 6564 6972 7328 5f64 6972 2c20 6578  akedirs(_dir, ex
+0000a1d0: 6973 745f 6f6b 3d54 7275 6529 0a0a 2020  ist_ok=True)..  
+0000a1e0: 2020 2020 2020 7465 6d70 5f64 6972 203d        temp_dir =
+0000a1f0: 206f 732e 7061 7468 2e6a 6f69 6e28 5f64   os.path.join(_d
+0000a200: 6972 2c20 2274 656d 705f 6469 7222 290a  ir, "temp_dir").
+0000a210: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
+0000a220: 6469 7273 2874 656d 705f 6469 722c 2065  dirs(temp_dir, e
+0000a230: 7869 7374 5f6f 6b3d 5472 7565 290a 0a20  xist_ok=True).. 
+0000a240: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000a250: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
+0000a260: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
+0000a270: 3d20 6d61 736b 5f72 656d 6f76 616c 2873  = mask_removal(s
+0000a280: 656c 662e 7275 6e6e 696e 675f 6461 7461  elf.running_data
+0000a290: 2c20 6d61 736b 292e 7669 6577 2844 6174  , mask).view(Dat
+0000a2a0: 6129 0a20 2020 2020 2020 2020 2020 206e  a).            n
+0000a2b0: 6577 5f64 6174 612e 7361 7665 286f 732e  ew_data.save(os.
+0000a2c0: 7061 7468 2e6a 6f69 6e28 7465 6d70 5f64  path.join(temp_d
+0000a2d0: 6972 2c20 2264 6174 612e 6864 6635 2229  ir, "data.hdf5")
+0000a2e0: 290a 2020 2020 2020 2020 2020 2020 7572  ).            ur
+0000a2f0: 6c73 203d 206e 6577 5f64 6174 612e 7572  ls = new_data.ur
+0000a300: 6c73 0a20 2020 2020 2020 2065 6c73 653a  ls.        else:
+0000a310: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+0000a320: 7320 3d20 7365 6c66 2e72 756e 6e69 6e67  s = self.running
+0000a330: 5f64 6174 612e 6170 706c 795f 6675 6e63  _data.apply_func
+0000a340: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000a350: 2020 205b 286d 6173 6b5f 7265 6d6f 7661     [(mask_remova
+0000a360: 6c2c 205b 6d61 736b 5d29 5d2c 0a20 2020  l, [mask])],.   
+0000a370: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+0000a380: 653d 6f73 2e70 6174 682e 6a6f 696e 2874  e=os.path.join(t
+0000a390: 656d 705f 6469 722c 2022 6461 7461 2e68  emp_dir, "data.h
+0000a3a0: 6466 3522 292c 0a20 2020 2020 2020 2020  df5"),.         
+0000a3b0: 2020 2020 2020 2074 6578 743d 2252 656d         text="Rem
+0000a3c0: 6f76 696e 6720 6d61 736b 222c 0a20 2020  oving mask",.   
+0000a3d0: 2020 2020 2020 2020 2020 2020 206f 7065               ope
+0000a3e0: 7261 7469 6f6e 3d4f 7065 7261 7469 6f6e  ration=Operation
+0000a3f0: 2e4d 4153 4b2c 0a20 2020 2020 2020 2020  .MASK,.         
+0000a400: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000a410: 2069 6620 7572 6c73 2069 7320 4e6f 6e65   if urls is None
+0000a420: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a430: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000a440: 2069 6620 696e 6469 6365 7320 6973 206e   if indices is n
+0000a450: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000a460: 2020 2020 206e 6577 5f75 726c 7320 3d20       new_urls = 
+0000a470: 6e75 6d70 792e 6172 7261 7928 7365 6c66  numpy.array(self
+0000a480: 2e67 6574 5f64 6174 6128 292e 7572 6c73  .get_data().urls
+0000a490: 2c20 6474 7970 653d 6f62 6a65 6374 290a  , dtype=object).
+0000a4a0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000a4b0: 7572 6c73 5b69 6e64 6963 6573 5d20 3d20  urls[indices] = 
+0000a4c0: 7572 6c73 0a20 2020 2020 2020 2020 2020  urls.           
+0000a4d0: 206e 6577 5f64 6174 6120 3d20 4461 7461   new_data = Data
+0000a4e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a4f0: 2020 6e65 775f 7572 6c73 2e72 6573 6861    new_urls.resha
+0000a500: 7065 2873 656c 662e 6461 7461 2e75 726c  pe(self.data.url
+0000a510: 732e 7368 6170 6529 2c0a 2020 2020 2020  s.shape),.      
+0000a520: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000a530: 6174 612e 6d65 7461 6461 7461 2c0a 2020  ata.metadata,.  
+0000a540: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a550: 6c66 2e5f 696e 5f6d 656d 6f72 792c 0a20  lf._in_memory,. 
+0000a560: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a570: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a580: 2020 2020 2020 206e 6577 5f64 6174 6120         new_data 
+0000a590: 3d20 4461 7461 280a 2020 2020 2020 2020  = Data(.        
+0000a5a0: 2020 2020 2020 2020 7572 6c73 2e72 6573          urls.res
+0000a5b0: 6861 7065 2873 656c 662e 6461 7461 2e75  hape(self.data.u
+0000a5c0: 726c 732e 7368 6170 6529 2c20 7365 6c66  rls.shape), self
+0000a5d0: 2e64 6174 612e 6d65 7461 6461 7461 2c20  .data.metadata, 
+0000a5e0: 7365 6c66 2e5f 696e 5f6d 656d 6f72 790a  self._in_memory.
+0000a5f0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000a600: 2020 2020 2020 206e 6577 5f64 6174 612e         new_data.
+0000a610: 7361 7665 286f 732e 7061 7468 2e6a 6f69  save(os.path.joi
+0000a620: 6e28 5f64 6972 2c20 2264 6174 612e 6864  n(_dir, "data.hd
+0000a630: 6635 2229 2c20 696e 6469 6365 733d 696e  f5"), indices=in
+0000a640: 6469 6365 7329 0a20 2020 2020 2020 2074  dices).        t
+0000a650: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000a660: 6f73 2e72 656d 6f76 6528 6f73 2e70 6174  os.remove(os.pat
+0000a670: 682e 6a6f 696e 2874 656d 705f 6469 722c  h.join(temp_dir,
+0000a680: 2022 6461 7461 2e68 6466 3522 2929 0a20   "data.hdf5")). 
+0000a690: 2020 2020 2020 2020 2020 206f 732e 726d             os.rm
+0000a6a0: 6469 7228 7465 6d70 5f64 6972 290a 2020  dir(temp_dir).  
+0000a6b0: 2020 2020 2020 6578 6365 7074 204f 5345        except OSE
+0000a6c0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
+0000a6d0: 2020 2020 2020 205f 6c6f 6767 6572 2e77         _logger.w
+0000a6e0: 6172 6e69 6e67 2822 4572 726f 723a 2025  arning("Error: %
+0000a6f0: 7322 2025 2028 652e 7374 7265 7272 6f72  s" % (e.strerror
+0000a700: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
+0000a710: 726e 2044 6174 6173 6574 280a 2020 2020  rn Dataset(.    
+0000a720: 2020 2020 2020 2020 5f64 6972 3d5f 6469          _dir=_di
+0000a730: 722c 0a20 2020 2020 2020 2020 2020 2064  r,.            d
+0000a740: 6174 613d 6e65 775f 6461 7461 2c0a 2020  ata=new_data,.  
+0000a750: 2020 2020 2020 2020 2020 6469 6d73 3d73            dims=s
+0000a760: 656c 662e 5f5f 6469 6d73 2c0a 2020 2020  elf.__dims,.    
+0000a770: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+0000a780: 6d61 7469 6f6e 3d73 656c 662e 7472 616e  mation=self.tran
+0000a790: 7366 6f72 6d61 7469 6f6e 2c0a 2020 2020  sformation,.    
+0000a7a0: 2020 2020 2020 2020 696e 5f6d 656d 6f72          in_memor
+0000a7b0: 793d 7365 6c66 2e5f 696e 5f6d 656d 6f72  y=self._in_memor
+0000a7c0: 792c 0a20 2020 2020 2020 2020 2020 2074  y,.            t
+0000a7d0: 6974 6c65 3d73 656c 662e 7469 746c 652c  itle=self.title,
+0000a7e0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000a7f0: 6465 6620 6170 706c 795f 726f 6928 0a20  def apply_roi(. 
+0000a800: 2020 2020 2020 2073 656c 662c 206f 7269         self, ori
+0000a810: 6769 6e3d 4e6f 6e65 2c20 7369 7a65 3d4e  gin=None, size=N
+0000a820: 6f6e 652c 2063 656e 7465 723d 4e6f 6e65  one, center=None
+0000a830: 2c20 696e 6469 6365 733d 4e6f 6e65 2c20  , indices=None, 
+0000a840: 726f 695f 6469 723d 4e6f 6e65 0a20 2020  roi_dir=None.   
+0000a850: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
+0000a860: 2020 2020 2020 2020 4170 706c 6965 7320          Applies 
+0000a870: 6120 7265 6769 6f6e 206f 6620 696e 7465  a region of inte
+0000a880: 7265 7374 2074 6f20 7468 6520 6461 7461  rest to the data
+0000a890: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+0000a8a0: 6d20 6f72 6967 696e 3a20 4f72 6967 696e  m origin: Origin
+0000a8b0: 206f 6620 7468 6520 726f 690a 2020 2020   of the roi.    
+0000a8c0: 2020 2020 3a70 6172 616d 2073 697a 653a      :param size:
+0000a8d0: 205b 4865 6967 6874 2c20 5769 6474 685d   [Height, Width]
+0000a8e0: 206f 6620 7468 6520 726f 692e 0a20 2020   of the roi..   
+0000a8f0: 2020 2020 203a 7061 7261 6d20 6365 6e74       :param cent
+0000a900: 6572 3a20 4365 6e74 6572 206f 6620 7468  er: Center of th
+0000a910: 6520 726f 690a 2020 2020 2020 2020 3a74  e roi.        :t
+0000a920: 7970 6520 6f72 6967 696e 3a20 556e 696f  ype origin: Unio
+0000a930: 6e5b 3264 2076 6563 746f 722c 204e 6f6e  n[2d vector, Non
+0000a940: 655d 0a20 2020 2020 2020 203a 7479 7065  e].        :type
+0000a950: 2063 656e 7465 723a 2055 6e69 6f6e 5b32   center: Union[2
+0000a960: 6420 7665 6374 6f72 2c20 4e6f 6e65 5d0a  d vector, None].
+0000a970: 2020 2020 2020 2020 3a74 7970 6520 7369          :type si
+0000a980: 7a65 3a20 556e 696f 6e5b 3264 2076 6563  ze: Union[2d vec
+0000a990: 746f 722c 204e 6f6e 655d 0a20 2020 2020  tor, None].     
+0000a9a0: 2020 203a 7061 7261 6d20 696e 6469 6365     :param indice
+0000a9b0: 733a 2049 6e64 6963 6573 206f 6620 7468  s: Indices of th
+0000a9c0: 6520 696d 6167 6573 2074 6f20 6170 706c  e images to appl
+0000a9d0: 7920 6261 636b 6772 6f75 6e64 2073 7562  y background sub
+0000a9e0: 7472 6163 7469 6f6e 2e0a 2020 2020 2020  traction..      
+0000a9f0: 2020 2020 2020 4966 204e 6f6e 652c 2074        If None, t
+0000aa00: 6865 2072 6f69 2069 7320 6170 706c 6965  he roi is applie
+0000aa10: 6420 746f 2061 6c6c 2074 6865 2064 6174  d to all the dat
+0000aa20: 612e 0a20 2020 2020 2020 203a 7479 7065  a..        :type
+0000aa30: 2069 6e64 6963 6573 3a20 556e 696f 6e5b   indices: Union[
+0000aa40: 4e6f 6e65 2c20 6172 7261 795f 6c69 6b65  None, array_like
+0000aa50: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+0000aa60: 2072 6f69 5f64 6972 3a20 4469 7265 6374   roi_dir: Direct
+0000aa70: 6f72 7920 7061 7468 2066 6f72 2074 6865  ory path for the
+0000aa80: 206e 6577 2064 6174 6173 6574 0a20 2020   new dataset.   
+0000aa90: 2020 2020 203a 7479 7065 2072 6f69 5f64       :type roi_d
+0000aaa0: 6972 3a20 7374 720a 2020 2020 2020 2020  ir: str.        
+0000aab0: 3a72 6574 7572 6e73 3a20 6461 7461 7365  :returns: datase
+0000aac0: 7420 7769 7468 2064 6174 6120 7769 7468  t with data with
+0000aad0: 2072 6f69 2061 7070 6c69 6564 2e0a 2020   roi applied..  
+0000aae0: 2020 2020 2020 2020 2020 4e6f 7465 3a20            Note: 
+0000aaf0: 546f 2070 7265 7365 7276 6520 636f 6e73  To preserve cons
+0000ab00: 6973 7465 6e63 6520 6f66 2073 6861 7065  istence of shape
+0000ab10: 2062 6574 7765 656e 2069 6d61 6765 732c   between images,
+0000ab20: 2069 6620 6069 6e64 6963 6573 600a 2020   if `indices`.  
+0000ab30: 2020 2020 2020 2020 2020 6973 206e 6f74            is not
+0000ab40: 204e 6f6e 652c 206f 6e6c 7920 7468 6520   None, only the 
+0000ab50: 6461 7461 206d 6f64 6966 6965 6420 6973  data modified is
+0000ab60: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
+0000ab70: 2020 203a 7274 7970 653a 2044 6174 6173     :rtype: Datas
+0000ab80: 6574 0a20 2020 2020 2020 2022 2222 0a0a  et.        """..
+0000ab90: 2020 2020 2020 2020 726f 695f 6469 7220          roi_dir 
+0000aba0: 3d20 7365 6c66 2e64 6972 2069 6620 726f  = self.dir if ro
+0000abb0: 695f 6469 7220 6973 204e 6f6e 6520 656c  i_dir is None el
+0000abc0: 7365 2072 6f69 5f64 6972 0a20 2020 2020  se roi_dir.     
+0000abd0: 2020 206f 732e 6d61 6b65 6469 7273 2872     os.makedirs(r
+0000abe0: 6f69 5f64 6972 2c20 6578 6973 745f 6f6b  oi_dir, exist_ok
+0000abf0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+0000ac00: 7365 6c66 2e72 756e 6e69 6e67 5f64 6174  self.running_dat
+0000ac10: 6120 3d20 7365 6c66 2e67 6574 5f64 6174  a = self.get_dat
+0000ac20: 6128 696e 6469 6365 7329 0a20 2020 2020  a(indices).     
+0000ac30: 2020 2069 6620 7365 6c66 2e5f 696e 5f6d     if self._in_m
+0000ac40: 656d 6f72 793a 0a20 2020 2020 2020 2020  emory:.         
+0000ac50: 2020 206e 6577 5f64 6174 6120 3d20 280a     new_data = (.
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac70: 6170 706c 795f 3344 5f52 4f49 2873 656c  apply_3D_ROI(sel
+0000ac80: 662e 7275 6e6e 696e 675f 6461 7461 2c20  f.running_data, 
+0000ac90: 6f72 6967 696e 2c20 7369 7a65 2c20 6365  origin, size, ce
+0000aca0: 6e74 6572 292e 7669 6577 2844 6174 6129  nter).view(Data)
+0000acb0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+0000acc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000acd0: 2020 6e65 775f 6461 7461 2e73 6176 6528    new_data.save(
+0000ace0: 6f73 2e70 6174 682e 6a6f 696e 2872 6f69  os.path.join(roi
+0000acf0: 5f64 6972 2c20 2264 6174 612e 6864 6635  _dir, "data.hdf5
+0000ad00: 2229 2c20 6e65 775f 7368 6170 653d 6e65  "), new_shape=ne
+0000ad10: 775f 6461 7461 2e73 6861 7065 290a 2020  w_data.shape).  
+0000ad20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ad30: 2020 2020 2020 2020 7368 6170 6520 3d20          shape = 
+0000ad40: 6e75 6d70 792e 6170 7065 6e64 280a 2020  numpy.append(.  
+0000ad50: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
+0000ad60: 656c 662e 7275 6e6e 696e 675f 6461 7461  elf.running_data
+0000ad70: 2e73 6861 7065 5b30 5d5d 2c0a 2020 2020  .shape[0]],.    
+0000ad80: 2020 2020 2020 2020 2020 2020 6170 706c              appl
+0000ad90: 795f 3244 5f52 4f49 2873 656c 662e 7275  y_2D_ROI(self.ru
+0000ada0: 6e6e 696e 675f 6461 7461 5b30 5d2c 206f  nning_data[0], o
+0000adb0: 7269 6769 6e2c 2073 697a 652c 2063 656e  rigin, size, cen
+0000adc0: 7465 7229 2e73 6861 7065 2c0a 2020 2020  ter).shape,.    
+0000add0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000ade0: 2020 2020 2020 7572 6c73 203d 2073 656c        urls = sel
+0000adf0: 662e 7275 6e6e 696e 675f 6461 7461 2e61  f.running_data.a
+0000ae00: 7070 6c79 5f66 756e 6373 280a 2020 2020  pply_funcs(.    
+0000ae10: 2020 2020 2020 2020 2020 2020 5b28 6170              [(ap
+0000ae20: 706c 795f 3244 5f52 4f49 2c20 5b6f 7269  ply_2D_ROI, [ori
+0000ae30: 6769 6e2c 2073 697a 652c 2063 656e 7465  gin, size, cente
+0000ae40: 725d 295d 2c0a 2020 2020 2020 2020 2020  r])],.          
+0000ae50: 2020 2020 2020 7361 7665 3d6f 732e 7061        save=os.pa
+0000ae60: 7468 2e6a 6f69 6e28 726f 695f 6469 722c  th.join(roi_dir,
+0000ae70: 2022 6461 7461 2e68 6466 3522 292c 0a20   "data.hdf5"),. 
+0000ae80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000ae90: 6578 743d 2241 7070 6c79 696e 6720 726f  ext="Applying ro
+0000aea0: 6922 2c0a 2020 2020 2020 2020 2020 2020  i",.            
+0000aeb0: 2020 2020 6f70 6572 6174 696f 6e3d 4f70      operation=Op
+0000aec0: 6572 6174 696f 6e2e 524f 492c 0a20 2020  eration.ROI,.   
+0000aed0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000aee0: 5f73 6861 7065 3d73 6861 7065 2c0a 2020  _shape=shape,.  
+0000aef0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000af00: 2020 2020 2020 2020 6966 2075 726c 7320          if urls 
+0000af10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000af20: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000af30: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000af40: 6461 7461 203d 2044 6174 6128 7572 6c73  data = Data(urls
+0000af50: 2c20 7365 6c66 2e72 756e 6e69 6e67 5f64  , self.running_d
+0000af60: 6174 612e 6d65 7461 6461 7461 2c20 7365  ata.metadata, se
+0000af70: 6c66 2e5f 696e 5f6d 656d 6f72 7929 0a0a  lf._in_memory)..
+0000af80: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+0000af90: 6d61 7469 6f6e 203d 2073 656c 662e 7472  mation = self.tr
+0000afa0: 616e 7366 6f72 6d61 7469 6f6e 0a20 2020  ansformation.   
+0000afb0: 2020 2020 2069 6620 7472 616e 7366 6f72       if transfor
+0000afc0: 6d61 7469 6f6e 2069 7320 6e6f 7420 4e6f  mation is not No
+0000afd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000afe0: 7472 616e 7366 6f72 6d61 7469 6f6e 203d  transformation =
+0000aff0: 2054 7261 6e73 666f 726d 6174 696f 6e28   Transformation(
+0000b000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b010: 2074 7261 6e73 666f 726d 6174 696f 6e2e   transformation.
+0000b020: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
+0000b030: 2020 2020 2020 6170 706c 795f 3244 5f52        apply_2D_R
+0000b040: 4f49 2874 7261 6e73 666f 726d 6174 696f  OI(transformatio
+0000b050: 6e2e 782c 206f 7269 6769 6e2c 2073 697a  n.x, origin, siz
+0000b060: 652c 2063 656e 7465 7229 2c0a 2020 2020  e, center),.    
+0000b070: 2020 2020 2020 2020 2020 2020 6170 706c              appl
+0000b080: 795f 3244 5f52 4f49 2874 7261 6e73 666f  y_2D_ROI(transfo
+0000b090: 726d 6174 696f 6e2e 792c 206f 7269 6769  rmation.y, origi
+0000b0a0: 6e2c 2073 697a 652c 2063 656e 7465 7229  n, size, center)
+0000b0b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b0c0: 2020 7472 616e 7366 6f72 6d61 7469 6f6e    transformation
+0000b0d0: 2e72 6f74 6174 652c 0a20 2020 2020 2020  .rotate,.       
+0000b0e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b0f0: 6966 2069 6e64 6963 6573 2069 7320 4e6f  if indices is No
+0000b100: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000b110: 7368 6170 6520 3d20 6c69 7374 2873 656c  shape = list(sel
+0000b120: 662e 6461 7461 2e73 6861 7065 295b 3a2d  f.data.shape)[:-
+0000b130: 325d 0a20 2020 2020 2020 2020 2020 2073  2].            s
+0000b140: 6861 7065 2e61 7070 656e 6428 6e65 775f  hape.append(new_
+0000b150: 6461 7461 2e73 6861 7065 5b2d 325d 290a  data.shape[-2]).
+0000b160: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+0000b170: 652e 6170 7065 6e64 286e 6577 5f64 6174  e.append(new_dat
+0000b180: 612e 7368 6170 655b 2d31 5d29 0a20 2020  a.shape[-1]).   
+0000b190: 2020 2020 2020 2020 206e 6577 5f64 6174           new_dat
+0000b1a0: 6120 3d20 6e65 775f 6461 7461 2e72 6573  a = new_data.res
+0000b1b0: 6861 7065 2873 6861 7065 290a 2020 2020  hape(shape).    
+0000b1c0: 2020 2020 7265 7475 726e 2044 6174 6173      return Datas
+0000b1d0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000b1e0: 5f64 6972 3d72 6f69 5f64 6972 2c0a 2020  _dir=roi_dir,.  
+0000b1f0: 2020 2020 2020 2020 2020 6461 7461 3d6e            data=n
+0000b200: 6577 5f64 6174 612c 0a20 2020 2020 2020  ew_data,.       
+0000b210: 2020 2020 2064 696d 733d 7365 6c66 2e5f       dims=self._
+0000b220: 5f64 696d 732c 0a20 2020 2020 2020 2020  _dims,.         
+0000b230: 2020 2074 7261 6e73 666f 726d 6174 696f     transformatio
+0000b240: 6e3d 7472 616e 7366 6f72 6d61 7469 6f6e  n=transformation
+0000b250: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+0000b260: 5f6d 656d 6f72 793d 7365 6c66 2e5f 696e  _memory=self._in
+0000b270: 5f6d 656d 6f72 792c 0a20 2020 2020 2020  _memory,.       
+0000b280: 2020 2020 2074 6974 6c65 3d73 656c 662e       title=self.
+0000b290: 7469 746c 652c 0a20 2020 2020 2020 2029  title,.        )
+0000b2a0: 0a0a 2020 2020 6465 6620 6669 6e64 5f73  ..    def find_s
+0000b2b0: 6869 6674 2873 656c 662c 2064 696d 656e  hift(self, dimen
+0000b2c0: 7369 6f6e 3d4e 6f6e 652c 2073 7465 7073  sion=None, steps
+0000b2d0: 3d35 302c 2069 6e64 6963 6573 3d4e 6f6e  =50, indices=Non
+0000b2e0: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+0000b2f0: 2020 2020 2020 2020 4669 6e64 2073 6869          Find shi
+0000b300: 6674 206f 6620 7468 6520 6461 7461 206f  ft of the data o
+0000b310: 7220 7061 7274 206f 6620 6974 2e0a 0a20  r part of it... 
+0000b320: 2020 2020 2020 203a 7061 7261 6d20 6469         :param di
+0000b330: 6d65 6e73 696f 6e3a 2050 6172 616d 6574  mension: Paramet
+0000b340: 6572 7320 7769 7468 2074 6865 2070 6f73  ers with the pos
+0000b350: 6974 696f 6e20 6f66 2074 6865 2064 6174  ition of the dat
+0000b360: 6120 696e 2074 6865 2072 6573 6861 7065  a in the reshape
+0000b370: 640a 2020 2020 2020 2020 2020 2020 6172  d.            ar
+0000b380: 7261 792e 0a20 2020 2020 2020 203a 7479  ray..        :ty
+0000b390: 7065 2064 696d 656e 7369 6f6e 3a20 556e  pe dimension: Un
+0000b3a0: 696f 6e5b 4e6f 6e65 2c20 7475 706c 652c  ion[None, tuple,
+0000b3b0: 2061 7272 6179 5f6c 696b 655d 0a20 2020   array_like].   
+0000b3c0: 2020 2020 203a 7061 7261 6d20 666c 6f61       :param floa
+0000b3d0: 7420 685f 6d61 783a 2053 6565 2060 636f  t h_max: See `co
+0000b3e0: 7265 2e69 6d61 6765 5265 6769 7374 7261  re.imageRegistra
+0000b3f0: 7469 6f6e 2e73 6869 6674 5f64 6574 6563  tion.shift_detec
+0000b400: 7469 6f6e 600a 2020 2020 2020 2020 3a70  tion`.        :p
+0000b410: 6172 616d 2066 6c6f 6174 2068 5f73 7465  aram float h_ste
+0000b420: 703a 2053 6565 2060 636f 7265 2e69 6d61  p: See `core.ima
+0000b430: 6765 5265 6769 7374 7261 7469 6f6e 2e73  geRegistration.s
+0000b440: 6869 6674 5f64 6574 6563 7469 6f6e 600a  hift_detection`.
+0000b450: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+0000b460: 6e64 6963 6573 3a20 426f 6f6c 6561 6e20  ndices: Boolean 
+0000b470: 696e 6465 7820 6c69 7374 2077 6974 6820  index list with 
+0000b480: 5472 7565 2069 6e20 7468 6520 696d 6167  True in the imag
+0000b490: 6573 2074 6f20 6170 706c 7920 7468 6520  es to apply the 
+0000b4a0: 7368 6966 7420 746f 2e0a 2020 2020 2020  shift to..      
+0000b4b0: 2020 2020 2020 4966 204e 6f6e 652c 2074        If None, t
+0000b4c0: 6865 2068 6f74 2070 6978 656c 2072 656d  he hot pixel rem
+0000b4d0: 6f76 616c 2069 7320 6170 706c 6965 6420  oval is applied 
+0000b4e0: 746f 2061 6c6c 2074 6865 2064 6174 612e  to all the data.
+0000b4f0: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
+0000b500: 6e64 6963 6573 3a20 556e 696f 6e5b 4e6f  ndices: Union[No
+0000b510: 6e65 2c20 6172 7261 795f 6c69 6b65 5d0a  ne, array_like].
+0000b520: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+0000b530: 3a20 4172 7261 7920 7769 7468 2073 6869  : Array with shi
+0000b540: 6674 2070 6572 2066 7261 6d65 2e0a 2020  ft per frame..  
+0000b550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b560: 2020 6461 7461 203d 2073 656c 662e 6765    data = self.ge
+0000b570: 745f 6461 7461 2869 6e64 6963 6573 3d69  t_data(indices=i
+0000b580: 6e64 6963 6573 2c20 6469 6d65 6e73 696f  ndices, dimensio
+0000b590: 6e3d 6469 6d65 6e73 696f 6e29 0a20 2020  n=dimension).   
+0000b5a0: 2020 2020 2072 6574 7572 6e20 7368 6966       return shif
+0000b5b0: 745f 6465 7465 6374 696f 6e28 6461 7461  t_detection(data
+0000b5c0: 2c20 7374 6570 7329 0a0a 2020 2020 6465  , steps)..    de
+0000b5d0: 6620 6669 6e64 5f73 6869 6674 5f61 6c6f  f find_shift_alo
+0000b5e0: 6e67 5f64 696d 656e 7369 6f6e 2873 656c  ng_dimension(sel
+0000b5f0: 662c 2064 696d 656e 7369 6f6e 2c20 7374  f, dimension, st
+0000b600: 6570 733d 3530 2c20 696e 6469 6365 733d  eps=50, indices=
+0000b610: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+0000b620: 6869 6674 203d 205b 5d0a 2020 2020 2020  hift = [].      
+0000b630: 2020 666f 7220 7661 6c75 6520 696e 2072    for value in r
+0000b640: 616e 6765 2873 656c 662e 6469 6d73 2e67  ange(self.dims.g
+0000b650: 6574 2864 696d 656e 7369 6f6e 5b30 5d29  et(dimension[0])
+0000b660: 2e73 697a 6529 3a0a 2020 2020 2020 2020  .size):.        
+0000b670: 2020 2020 7368 6966 742e 6170 7065 6e64      shift.append
+0000b680: 2873 656c 662e 6669 6e64 5f73 6869 6674  (self.find_shift
+0000b690: 285b 6469 6d65 6e73 696f 6e5b 305d 2c20  ([dimension[0], 
+0000b6a0: 7661 6c75 655d 2c20 7374 6570 732c 2069  value], steps, i
+0000b6b0: 6e64 6963 6573 2929 0a20 2020 2020 2020  ndices)).       
+0000b6c0: 2072 6574 7572 6e20 6e75 6d70 792e 6172   return numpy.ar
+0000b6d0: 7261 7928 7368 6966 7429 0a0a 2020 2020  ray(shift)..    
+0000b6e0: 6465 6620 6170 706c 795f 7368 6966 745f  def apply_shift_
+0000b6f0: 616c 6f6e 675f 6469 6d65 6e73 696f 6e28  along_dimension(
+0000b700: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000b710: 2020 2020 2020 2073 6869 6674 2c0a 2020         shift,.  
+0000b720: 2020 2020 2020 6469 6d65 6e73 696f 6e2c        dimension,
+0000b730: 0a20 2020 2020 2020 2073 6869 6674 5f61  .        shift_a
+0000b740: 7070 726f 6163 683d 2266 6674 222c 0a20  pproach="fft",. 
+0000b750: 2020 2020 2020 2069 6e64 6963 6573 3d4e         indices=N
+0000b760: 6f6e 652c 0a20 2020 2020 2020 2063 616c  one,.        cal
+0000b770: 6c62 6163 6b3d 4e6f 6e65 2c0a 2020 2020  lback=None,.    
+0000b780: 2020 2020 5f64 6972 3d4e 6f6e 652c 0a20      _dir=None,. 
+0000b790: 2020 2029 3a0a 2020 2020 2020 2020 6461     ):.        da
+0000b7a0: 7461 7365 7420 3d20 7365 6c66 0a20 2020  taset = self.   
+0000b7b0: 2020 2020 2066 6f72 2076 616c 7565 2069       for value i
+0000b7c0: 6e20 7261 6e67 6528 7365 6c66 2e64 696d  n range(self.dim
+0000b7d0: 732e 6765 7428 6469 6d65 6e73 696f 6e5b  s.get(dimension[
+0000b7e0: 305d 292e 7369 7a65 293a 0a20 2020 2020  0]).size):.     
+0000b7f0: 2020 2020 2020 2064 6174 612c 2072 696e         data, rin
+0000b800: 6469 6365 7320 3d20 7365 6c66 2e67 6574  dices = self.get
+0000b810: 5f64 6174 6128 0a20 2020 2020 2020 2020  _data(.         
+0000b820: 2020 2020 2020 2069 6e64 6963 6573 3d69         indices=i
+0000b830: 6e64 6963 6573 2c20 6469 6d65 6e73 696f  ndices, dimensio
+0000b840: 6e3d 5b64 696d 656e 7369 6f6e 5b30 5d2c  n=[dimension[0],
+0000b850: 2076 616c 7565 5d2c 2072 6574 7572 6e5f   value], return_
+0000b860: 696e 6469 6365 733d 5472 7565 0a20 2020  indices=True.   
+0000b870: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000b880: 2020 2020 2020 2066 7261 6d65 7320 3d20         frames = 
+0000b890: 6e75 6d70 792e 6172 616e 6765 280a 2020  numpy.arange(.  
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b8b0: 6c66 2e67 6574 5f64 6174 6128 696e 6469  lf.get_data(indi
+0000b8c0: 6365 733d 696e 6469 6365 732c 2064 696d  ces=indices, dim
+0000b8d0: 656e 7369 6f6e 3d5b 6469 6d65 6e73 696f  ension=[dimensio
+0000b8e0: 6e5b 305d 2c20 7661 6c75 655d 292e 7368  n[0], value]).sh
+0000b8f0: 6170 655b 305d 0a20 2020 2020 2020 2020  ape[0].         
+0000b900: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000b910: 2064 6174 6173 6574 203d 2064 6174 6173   dataset = datas
+0000b920: 6574 2e61 7070 6c79 5f73 6869 6674 280a  et.apply_shift(.
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 6e75 6d70 792e 6f75 7465 7228 7368 6966  numpy.outer(shif
+0000b950: 745b 7661 6c75 655d 2c20 6672 616d 6573  t[value], frames
+0000b960: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000b970: 2020 205b 6469 6d65 6e73 696f 6e5b 305d     [dimension[0]
+0000b980: 2c20 7661 6c75 655d 2c0a 2020 2020 2020  , value],.      
+0000b990: 2020 2020 2020 2020 2020 7368 6966 745f            shift_
+0000b9a0: 6170 7072 6f61 6368 2c0a 2020 2020 2020  approach,.      
+0000b9b0: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+0000b9c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000b9d0: 2020 2063 616c 6c62 6163 6b2c 0a20 2020     callback,.   
+0000b9e0: 2020 2020 2020 2020 2020 2020 205f 6469               _di
+0000b9f0: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
+0000ba00: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000ba10: 2064 6174 6173 6574 0a0a 2020 2020 6465   dataset..    de
+0000ba20: 6620 6170 706c 795f 7368 6966 7428 0a20  f apply_shift(. 
+0000ba30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000ba40: 2020 2020 2073 6869 6674 2c0a 2020 2020       shift,.    
+0000ba50: 2020 2020 6469 6d65 6e73 696f 6e3d 4e6f      dimension=No
+0000ba60: 6e65 2c0a 2020 2020 2020 2020 7368 6966  ne,.        shif
+0000ba70: 745f 6170 7072 6f61 6368 3d22 6666 7422  t_approach="fft"
+0000ba80: 2c0a 2020 2020 2020 2020 696e 6469 6365  ,.        indice
+0000ba90: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+0000baa0: 6361 6c6c 6261 636b 3d4e 6f6e 652c 0a20  callback=None,. 
+0000bab0: 2020 2020 2020 205f 6469 723d 4e6f 6e65         _dir=None
+0000bac0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000bad0: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
+0000bae0: 6c79 2073 6869 6674 206f 6620 7468 6520  ly shift of the 
+0000baf0: 6461 7461 206f 7220 7061 7274 206f 6620  data or part of 
+0000bb00: 6974 2061 6e64 2073 6176 6520 6e65 7720  it and save new 
+0000bb10: 6461 7461 2069 6e74 6f20 6469 736b 2e0a  data into disk..
+0000bb20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000bb30: 6172 7261 795f 6c69 6b65 2073 6869 6674  array_like shift
+0000bb40: 3a20 5368 6966 7420 7065 7220 6672 616d  : Shift per fram
+0000bb50: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
+0000bb60: 6d20 6469 6d65 6e73 696f 6e3a 2050 6172  m dimension: Par
+0000bb70: 616d 6574 6573 2077 6974 6820 7468 6520  ametes with the 
+0000bb80: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
+0000bb90: 6461 7461 2069 6e20 7468 6520 7265 7368  data in the resh
+0000bba0: 6170 6564 0a20 2020 2020 2020 2020 2020  aped.           
+0000bbb0: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+0000bbc0: 3a74 7970 6520 6469 6d65 6e73 696f 6e3a  :type dimension:
+0000bbd0: 2055 6e69 6f6e 5b4e 6f6e 652c 2074 7570   Union[None, tup
+0000bbe0: 6c65 2c20 6172 7261 795f 6c69 6b65 5d0a  le, array_like].
+0000bbf0: 2020 2020 2020 2020 3a70 6172 616d 2055          :param U
+0000bc00: 6e69 6f6e 5b27 6666 7427 2c20 276c 696e  nion['fft', 'lin
+0000bc10: 6561 7227 5d20 7368 6966 745f 6170 7072  ear'] shift_appr
+0000bc20: 6f61 6368 3a20 4d65 7468 6f64 2074 6f20  oach: Method to 
+0000bc30: 7573 6520 746f 2061 7070 6c79 2074 6865  use to apply the
+0000bc40: 2073 6869 6674 2e0a 2020 2020 2020 2020   shift..        
+0000bc50: 3a70 6172 616d 2069 6e64 6963 6573 3a20  :param indices: 
+0000bc60: 426f 6f6c 6561 6e20 696e 6465 7820 6c69  Boolean index li
+0000bc70: 7374 2077 6974 6820 5472 7565 2069 6e20  st with True in 
+0000bc80: 7468 6520 696d 6167 6573 2074 6f20 6170  the images to ap
+0000bc90: 706c 7920 7468 6520 7368 6966 7420 746f  ply the shift to
+0000bca0: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+0000bcb0: 204e 6f6e 652c 2074 6865 2068 6f74 2070   None, the hot p
+0000bcc0: 6978 656c 2072 656d 6f76 616c 2069 7320  ixel removal is 
+0000bcd0: 6170 706c 6965 6420 746f 2061 6c6c 2074  applied to all t
+0000bce0: 6865 2064 6174 612e 0a20 2020 2020 2020  he data..       
+0000bcf0: 203a 7479 7065 2069 6e64 6963 6573 3a20   :type indices: 
+0000bd00: 556e 696f 6e5b 4e6f 6e65 2c20 6172 7261  Union[None, arra
+0000bd10: 795f 6c69 6b65 5d0a 2020 2020 2020 2020  y_like].        
+0000bd20: 3a70 6172 616d 2055 6e69 6f6e 5b66 756e  :param Union[fun
+0000bd30: 6374 696f 6e2c 204e 6f6e 655d 2063 616c  ction, None] cal
+0000bd40: 6c62 6163 6b3a 2043 616c 6c62 6163 6b0a  lback: Callback.
+0000bd50: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+0000bd60: 3a20 6461 7461 7365 7420 7769 7468 2064  : dataset with d
+0000bd70: 6174 6120 6f66 2073 616d 6520 7369 7a65  ata of same size
+0000bd80: 2061 7320 6073 656c 662e 6461 7461 6020   as `self.data` 
+0000bd90: 6275 7420 7769 7468 2074 6865 0a20 2020  but with the.   
+0000bda0: 2020 2020 2020 2020 206d 6f64 6966 6965           modifie
+0000bdb0: 6420 696d 6167 6573 2e20 5468 6520 7572  d images. The ur
+0000bdc0: 6c73 206f 6620 7468 6520 6d6f 6469 6669  ls of the modifi
+0000bdd0: 6564 2069 6d61 6765 7320 6172 6520 7265  ed images are re
+0000bde0: 706c 6163 6564 2077 6974 680a 2020 2020  placed with.    
+0000bdf0: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
+0000be00: 7572 6c73 2e0a 2020 2020 2020 2020 2222  urls..        ""
+0000be10: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+0000be20: 206c 656e 2873 6869 6674 2920 3e20 302c   len(shift) > 0,
+0000be30: 2022 5368 6966 7420 6c69 7374 2063 616e   "Shift list can
+0000be40: 2774 2062 6520 656d 7074 7922 0a0a 2020  't be empty"..  
+0000be50: 2020 2020 2020 6966 206e 6f74 206e 756d        if not num
+0000be60: 7079 2e61 6e79 2873 6869 6674 293a 0a20  py.any(shift):. 
+0000be70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000be80: 6e20 7365 6c66 0a0a 2020 2020 2020 2020  n self..        
+0000be90: 5f64 6972 203d 2073 656c 662e 6469 7220  _dir = self.dir 
+0000bea0: 6966 205f 6469 7220 6973 204e 6f6e 6520  if _dir is None 
+0000beb0: 656c 7365 205f 6469 720a 0a20 2020 2020  else _dir..     
+0000bec0: 2020 206f 732e 6d61 6b65 6469 7273 285f     os.makedirs(_
+0000bed0: 6469 722c 2065 7869 7374 5f6f 6b3d 5472  dir, exist_ok=Tr
+0000bee0: 7565 290a 0a20 2020 2020 2020 2064 6174  ue)..        dat
+0000bef0: 612c 2072 696e 6469 6365 7320 3d20 7365  a, rindices = se
+0000bf00: 6c66 2e67 6574 5f64 6174 6128 696e 6469  lf.get_data(indi
+0000bf10: 6365 732c 2064 696d 656e 7369 6f6e 2c20  ces, dimension, 
+0000bf20: 7265 7475 726e 5f69 6e64 6963 6573 3d54  return_indices=T
+0000bf30: 7275 6529 0a0a 2020 2020 2020 2020 7769  rue)..        wi
+0000bf40: 7468 2073 656c 662e 7374 6174 655f 6f66  th self.state_of
+0000bf50: 5f6f 7065 7261 7469 6f6e 732e 7275 6e5f  _operations.run_
+0000bf60: 636f 6e74 6578 7428 4f70 6572 6174 696f  context(Operatio
+0000bf70: 6e2e 5348 4946 5429 3a0a 2020 2020 2020  n.SHIFT):.      
+0000bf80: 2020 2020 2020 5f66 696c 6520 3d20 4e6f        _file = No
+0000bf90: 6e65 0a20 2020 2020 2020 2020 2020 2074  ne.            t
+0000bfa0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000bfb0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000bfc0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000bfd0: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
+0000bfe0: 6a6f 696e 285f 6469 722c 2022 6461 7461  join(_dir, "data
+0000bff0: 2e68 6466 3522 290a 2020 2020 2020 2020  .hdf5").        
+0000c000: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
+0000c010: 6520 3d20 6835 7079 2e46 696c 6528 6669  e = h5py.File(fi
+0000c020: 6c65 6e61 6d65 2c20 2261 2229 0a20 2020  lename, "a").   
+0000c030: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0000c040: 6570 7420 4f53 4572 726f 723a 0a20 2020  ept OSError:.   
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 2069 6620 6f73 2e70 6174 682e 6578 6973   if os.path.exis
+0000c070: 7473 2866 696c 656e 616d 6529 3a0a 2020  ts(filename):.  
+0000c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c090: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
+0000c0a0: 6669 6c65 6e61 6d65 290a 2020 2020 2020  filename).      
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
+0000c0c0: 696c 6520 3d20 6835 7079 2e46 696c 6528  ile = h5py.File(
+0000c0d0: 6669 6c65 6e61 6d65 2c20 2277 2229 0a20  filename, "w"). 
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000c0f0: 6174 6173 6574 5f6e 616d 6520 3d20 2264  ataset_name = "d
+0000c100: 6174 6173 6574 220a 2020 2020 2020 2020  ataset".        
+0000c110: 2020 2020 2020 2020 6966 2022 6461 7461          if "data
+0000c120: 7365 7422 206e 6f74 2069 6e20 5f66 696c  set" not in _fil
+0000c130: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c140: 2020 2020 2020 205f 6669 6c65 2e63 7265         _file.cre
+0000c150: 6174 655f 6461 7461 7365 7428 0a20 2020  ate_dataset(.   
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 2022 6461 7461 7365 7422 2c20       "dataset", 
+0000c180: 7365 6c66 2e67 6574 5f64 6174 6128 292e  self.get_data().
+0000c190: 7368 6170 652c 2064 7479 7065 3d73 656c  shape, dtype=sel
+0000c1a0: 662e 6461 7461 2e64 7479 7065 0a20 2020  f.data.dtype.   
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000c1d0: 2020 2065 6c69 6620 7365 6c66 2e67 6574     elif self.get
+0000c1e0: 5f64 6174 6128 292e 7368 6170 6520 213d  _data().shape !=
+0000c1f0: 205f 6669 6c65 5b22 6461 7461 7365 7422   _file["dataset"
+0000c200: 5d2e 7368 6170 653a 0a20 2020 2020 2020  ].shape:.       
+0000c210: 2020 2020 2020 2020 2020 2020 2064 656c               del
+0000c220: 205f 6669 6c65 5b22 6461 7461 7365 7422   _file["dataset"
+0000c230: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000c240: 2020 2020 2020 5f66 696c 652e 6372 6561        _file.crea
+0000c250: 7465 5f64 6174 6173 6574 280a 2020 2020  te_dataset(.    
+0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c270: 2020 2020 2264 6174 6173 6574 222c 2073      "dataset", s
+0000c280: 656c 662e 6765 745f 6461 7461 2829 2e73  elf.get_data().s
+0000c290: 6861 7065 2c20 6474 7970 653d 7365 6c66  hape, dtype=self
+0000c2a0: 2e64 6174 612e 6474 7970 650a 2020 2020  .data.dtype.    
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c2d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c2e0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000c2f0: 7365 745f 6e61 6d65 203d 2022 7570 6461  set_name = "upda
+0000c300: 7465 5f64 6174 6173 6574 220a 2020 2020  te_dataset".    
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 5f66 696c 652e 636f 7079 2822 6461 7461  _file.copy("data
+0000c330: 7365 7422 2c20 2275 7064 6174 655f 6461  set", "update_da
+0000c340: 7461 7365 7422 290a 0a20 2020 2020 2020  taset")..       
+0000c350: 2020 2020 2020 2020 2069 6f5f 7574 696c           io_util
+0000c360: 732e 6164 7661 6e63 656d 656e 745f 6469  s.advancement_di
+0000c370: 7370 6c61 7928 302c 206c 656e 2864 6174  splay(0, len(dat
+0000c380: 6129 2c20 2241 7070 6c79 696e 6720 7368  a), "Applying sh
+0000c390: 6966 7422 290a 2020 2020 2020 2020 2020  ift").          
+0000c3a0: 2020 2020 2020 6966 2064 696d 656e 7369        if dimensi
+0000c3b0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3d0: 2020 2020 2320 436f 6e76 6572 7420 6469      # Convert di
+0000c3e0: 6d65 6e73 696f 6e20 616e 6420 7661 6c75  mension and valu
+0000c3f0: 6520 696e 746f 206c 6973 740a 2020 2020  e into list.    
+0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c410: 6966 2074 7970 6528 6469 6d65 6e73 696f  if type(dimensio
+0000c420: 6e5b 305d 2920 6973 2069 6e74 3a0a 2020  n[0]) is int:.  
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c440: 2020 2020 2020 6469 6d65 6e73 696f 6e5b        dimension[
+0000c450: 305d 203d 205b 6469 6d65 6e73 696f 6e5b  0] = [dimension[
+0000c460: 305d 5d0a 2020 2020 2020 2020 2020 2020  0]].            
+0000c470: 2020 2020 2020 2020 2020 2020 6469 6d65              dime
+0000c480: 6e73 696f 6e5b 315d 203d 205b 6469 6d65  nsion[1] = [dime
+0000c490: 6e73 696f 6e5b 315d 5d0a 2020 2020 2020  nsion[1]].      
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 7572                ur
+0000c4b0: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
+0000c4c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000c4d0: 692c 2069 6478 2069 6e20 656e 756d 6572  i, idx in enumer
+0000c4e0: 6174 6528 7269 6e64 6963 6573 293a 0a20  ate(rindices):. 
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c500: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c510: 6c66 2e73 7461 7465 5f6f 665f 6f70 6572  lf.state_of_oper
+0000c520: 6174 696f 6e73 2e69 735f 7275 6e6e 696e  ations.is_runnin
+0000c530: 6728 4f70 6572 6174 696f 6e2e 5348 4946  g(Operation.SHIF
+0000c540: 5429 3a0a 2020 2020 2020 2020 2020 2020  T):.            
+0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c560: 6966 2022 7570 6461 7465 5f64 6174 6173  if "update_datas
+0000c570: 6574 2220 696e 205f 6669 6c65 3a0a 2020  et" in _file:.  
 0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 6461 7461 5f73 6c69 6365 3d69 6478    data_slice=idx
-0000c5a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5c0: 2020 7363 6865 6d65 3d22 7369 6c78 222c    scheme="silx",
-0000c5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c5e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2069 6f5f 7574 696c 732e 6164 7661 6e63   io_utils.advanc
-0000c630: 656d 656e 745f 6469 7370 6c61 7928 0a20  ement_display(. 
-0000c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c650: 2020 2020 2020 2020 2020 2069 202b 2031             i + 1
-0000c660: 2c20 6c65 6e28 7269 6e64 6963 6573 292c  , len(rindices),
-0000c670: 2022 4170 706c 7969 6e67 2073 6869 6674   "Applying shift
-0000c680: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000c690: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6b0: 2023 2052 6570 6c61 6365 2073 7065 6369   # Replace speci
-0000c6c0: 6669 6320 7572 6c73 2074 6861 7420 636f  fic urls that co
-0000c6d0: 7272 6573 706f 6e64 2074 6f20 7468 6520  rrespond to the 
-0000c6e0: 6d6f 6469 6669 6564 2064 6174 610a 2020  modified data.  
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c700: 2020 6e65 775f 7572 6c73 203d 206e 756d    new_urls = num
-0000c710: 7079 2e61 7272 6179 2873 656c 662e 6461  py.array(self.da
-0000c720: 7461 2e75 726c 732c 2064 7479 7065 3d6f  ta.urls, dtype=o
-0000c730: 626a 6563 7429 0a20 2020 2020 2020 2020  bject).         
-0000c740: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-0000c750: 7572 6c73 203d 206e 6577 5f75 726c 730a  urls = new_urls.
+0000c590: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000c5a0: 6c20 5f66 696c 655b 2275 7064 6174 655f  l _file["update_
+0000c5b0: 6461 7461 7365 7422 5d0a 2020 2020 2020  dataset"].      
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2069 6d67 203d 2061 7070 6c79       img = apply
+0000c600: 5f73 6869 6674 2864 6174 615b 695d 2c20  _shift(data[i], 
+0000c610: 7368 6966 745b 3a2c 2069 5d2c 2073 6869  shift[:, i], shi
+0000c620: 6674 5f61 7070 726f 6163 6829 0a20 2020  ft_approach).   
+0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c640: 2020 2020 2069 6620 7368 6966 745b 3a2c       if shift[:,
+0000c650: 2069 5d2e 616c 6c28 2920 3e20 313a 0a20   i].all() > 1:. 
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 2020 2020 2020 2020 2020 2073 6869 6674             shift
+0000c680: 5f61 7070 726f 6163 6820 3d20 226c 696e  _approach = "lin
+0000c690: 6561 7222 0a20 2020 2020 2020 2020 2020  ear".           
+0000c6a0: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
+0000c6b0: 6c65 5b64 6174 6173 6574 5f6e 616d 655d  le[dataset_name]
+0000c6c0: 5b69 6478 5d20 3d20 696d 670a 2020 2020  [idx] = img.    
+0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6e0: 2020 2020 7572 6c73 2e61 7070 656e 6428      urls.append(
+0000c6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c700: 2020 2020 2020 2020 2020 2020 2044 6174               Dat
+0000c710: 6155 726c 280a 2020 2020 2020 2020 2020  aUrl(.          
+0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c730: 2020 2020 2020 6669 6c65 5f70 6174 683d        file_path=
+0000c740: 5f64 6972 202b 2022 2f64 6174 612e 6864  _dir + "/data.hd
+0000c750: 6635 222c 0a20 2020 2020 2020 2020 2020  f5",.           
 0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 6966 2069 6e64 6963 6573 2069      if indices i
-0000c780: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000c770: 2020 2020 2064 6174 615f 7061 7468 3d22       data_path="
+0000c780: 2f64 6174 6173 6574 222c 0a20 2020 2020  /dataset",.     
 0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2320 4372 6561 7465 2061 7272      # Create arr
-0000c7b0: 6179 206f 6620 626f 6f6c 6561 6e73 2074  ay of booleans t
-0000c7c0: 6f20 6b6e 6f77 2077 6869 6368 2069 6e64  o know which ind
-0000c7d0: 6963 6573 2077 6520 6861 7665 0a20 2020  ices we have.   
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7f0: 2020 2020 2062 6f6f 6c5f 696e 6469 6365       bool_indice
-0000c800: 7320 3d20 6e75 6d70 792e 7a65 726f 7328  s = numpy.zeros(
-0000c810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c830: 662e 6765 745f 6461 7461 2829 2e73 6861  f.get_data().sha
-0000c840: 7065 5b3a 2d32 5d2c 2064 7479 7065 3d62  pe[:-2], dtype=b
-0000c850: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-0000c860: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c880: 2020 2020 2020 626f 6f6c 5f69 6e64 6963        bool_indic
-0000c890: 6573 5b69 6e64 6963 6573 5d20 3d20 5472  es[indices] = Tr
-0000c8a0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0000c8b0: 2020 2020 2020 2020 2020 2062 6f6f 6c5f             bool_
-0000c8c0: 696e 6469 6365 7320 3d20 626f 6f6c 5f69  indices = bool_i
-0000c8d0: 6e64 6963 6573 2e72 6573 6861 7065 2873  ndices.reshape(s
-0000c8e0: 656c 662e 6461 7461 2e73 6361 6e5f 7368  elf.data.scan_sh
-0000c8f0: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
-0000c900: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000c910: 2069 2c20 6469 6d20 696e 2065 6e75 6d65   i, dim in enume
-0000c920: 7261 7465 2873 6f72 7465 6428 6469 6d65  rate(sorted(dime
-0000c930: 6e73 696f 6e5b 305d 2929 3a0a 2020 2020  nsion[0])):.    
-0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c950: 2020 2020 2020 2020 2320 466c 6970 2061          # Flip a
-0000c960: 7869 7320 746f 2062 6520 636f 6e73 6973  xis to be consis
-0000c970: 7465 6e74 2077 6974 6820 7468 6520 6461  tent with the da
-0000c980: 7461 2073 6861 7065 0a20 2020 2020 2020  ta shape.       
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2020 2061 7869 7320 3d20 7365 6c66       axis = self
-0000c9b0: 2e64 696d 732e 6e64 696d 202d 2064 696d  .dims.ndim - dim
-0000c9c0: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 2063 6f70 795f 7572 6c73 203d 206e 756d   copy_urls = num
-0000c9f0: 7079 2e73 7761 7061 7865 7328 636f 7079  py.swapaxes(copy
-0000ca00: 5f75 726c 732c 2030 2c20 6178 6973 295b  _urls, 0, axis)[
-0000ca10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2064 696d 656e 7369 6f6e 5b31 5d5b 695d   dimension[1][i]
-0000ca40: 2c20 3a0a 2020 2020 2020 2020 2020 2020  , :.            
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-0000ca80: 6f6c 5f69 6e64 6963 6573 203d 206e 756d  ol_indices = num
-0000ca90: 7079 2e73 7761 7061 7865 7328 626f 6f6c  py.swapaxes(bool
-0000caa0: 5f69 6e64 6963 6573 2c20 302c 2061 7869  _indices, 0, axi
-0000cab0: 7329 5b0a 2020 2020 2020 2020 2020 2020  s)[.            
+0000c7a0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+0000c7b0: 736c 6963 653d 6964 782c 0a20 2020 2020  slice=idx,.     
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7d0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+0000c7e0: 653d 2273 696c 7822 2c0a 2020 2020 2020  e="silx",.      
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c830: 2020 2020 2020 2020 2020 696f 5f75 7469            io_uti
+0000c840: 6c73 2e61 6476 616e 6365 6d65 6e74 5f64  ls.advancement_d
+0000c850: 6973 706c 6179 280a 2020 2020 2020 2020  isplay(.        
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2020 2020 6920 2b20 312c 206c 656e 2872      i + 1, len(r
+0000c880: 696e 6469 6365 7329 2c20 2241 7070 6c79  indices), "Apply
+0000c890: 696e 6720 7368 6966 7422 0a20 2020 2020  ing shift".     
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8b0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0000c8c0: 2020 2020 2020 2020 2020 2320 5265 706c            # Repl
+0000c8d0: 6163 6520 7370 6563 6966 6963 2075 726c  ace specific url
+0000c8e0: 7320 7468 6174 2063 6f72 7265 7370 6f6e  s that correspon
+0000c8f0: 6420 746f 2074 6865 206d 6f64 6966 6965  d to the modifie
+0000c900: 6420 6461 7461 0a20 2020 2020 2020 2020  d data.         
+0000c910: 2020 2020 2020 2020 2020 206e 6577 5f75             new_u
+0000c920: 726c 7320 3d20 6e75 6d70 792e 6172 7261  rls = numpy.arra
+0000c930: 7928 7365 6c66 2e64 6174 612e 7572 6c73  y(self.data.urls
+0000c940: 2c20 6474 7970 653d 6f62 6a65 6374 290a  , dtype=object).
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2020 636f 7079 5f75 726c 7320 3d20      copy_urls = 
+0000c970: 6e65 775f 7572 6c73 0a20 2020 2020 2020  new_urls.       
+0000c980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000c990: 696e 6469 6365 7320 6973 206e 6f74 204e  indices is not N
+0000c9a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000c9b0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+0000c9c0: 7265 6174 6520 6172 7261 7920 6f66 2062  reate array of b
+0000c9d0: 6f6f 6c65 616e 7320 746f 206b 6e6f 7720  ooleans to know 
+0000c9e0: 7768 6963 6820 696e 6469 6365 7320 7765  which indices we
+0000c9f0: 2068 6176 650a 2020 2020 2020 2020 2020   have.          
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0000ca10: 6f6c 5f69 6e64 6963 6573 203d 206e 756d  ol_indices = num
+0000ca20: 7079 2e7a 6572 6f73 280a 2020 2020 2020  py.zeros(.      
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 2020 7365 6c66 2e67 6574 5f64        self.get_d
+0000ca50: 6174 6128 292e 7368 6170 655b 3a2d 325d  ata().shape[:-2]
+0000ca60: 2c20 6474 7970 653d 626f 6f6c 0a20 2020  , dtype=bool.   
+0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000caa0: 6f6f 6c5f 696e 6469 6365 735b 696e 6469  ool_indices[indi
+0000cab0: 6365 735d 203d 2054 7275 650a 2020 2020  ces] = True.    
 0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 2020 2020 6469 6d65 6e73 696f 6e5b 315d      dimension[1]
-0000cae0: 5b69 5d2c 203a 0a20 2020 2020 2020 2020  [i], :.         
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-0000cb10: 2020 2020 2020 2020 2020 2020 2063 6f70               cop
-0000cb20: 795f 7572 6c73 5b62 6f6f 6c5f 696e 6469  y_urls[bool_indi
-0000cb30: 6365 735d 203d 2075 726c 730a 2020 2020  ces] = urls.    
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000cb60: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000cb70: 7220 692c 2064 696d 2069 6e20 656e 756d  r i, dim in enum
-0000cb80: 6572 6174 6528 736f 7274 6564 2864 696d  erate(sorted(dim
-0000cb90: 656e 7369 6f6e 5b30 5d29 293a 0a20 2020  ension[0])):.   
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbb0: 2020 2020 2020 2020 2023 2046 6c69 7020           # Flip 
-0000cbc0: 6178 6973 2074 6f20 6265 2063 6f6e 7369  axis to be consi
-0000cbd0: 7374 656e 7420 7769 7468 2074 6865 2064  stent with the d
-0000cbe0: 6174 6120 7368 6170 650a 2020 2020 2020  ata shape.      
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 2020 2020 2020 6178 6973 203d 2073 656c        axis = sel
-0000cc10: 662e 6469 6d73 2e6e 6469 6d20 2d20 6469  f.dims.ndim - di
-0000cc20: 6d20 2d20 310a 2020 2020 2020 2020 2020  m - 1.          
+0000cad0: 2020 2020 626f 6f6c 5f69 6e64 6963 6573      bool_indices
+0000cae0: 203d 2062 6f6f 6c5f 696e 6469 6365 732e   = bool_indices.
+0000caf0: 7265 7368 6170 6528 7365 6c66 2e64 6174  reshape(self.dat
+0000cb00: 612e 7363 616e 5f73 6861 7065 290a 2020  a.scan_shape).  
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb20: 2020 2020 2020 666f 7220 692c 2064 696d        for i, dim
+0000cb30: 2069 6e20 656e 756d 6572 6174 6528 736f   in enumerate(so
+0000cb40: 7274 6564 2864 696d 656e 7369 6f6e 5b30  rted(dimension[0
+0000cb50: 5d29 293a 0a20 2020 2020 2020 2020 2020  ])):.           
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb70: 2023 2046 6c69 7020 6178 6973 2074 6f20   # Flip axis to 
+0000cb80: 6265 2063 6f6e 7369 7374 656e 7420 7769  be consistent wi
+0000cb90: 7468 2074 6865 2064 6174 6120 7368 6170  th the data shap
+0000cba0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0000cbc0: 6973 203d 2073 656c 662e 6469 6d73 2e6e  is = self.dims.n
+0000cbd0: 6469 6d20 2d20 6469 6d20 2d20 310a 2020  dim - dim - 1.  
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbf0: 2020 2020 2020 2020 2020 636f 7079 5f75            copy_u
+0000cc00: 726c 7320 3d20 6e75 6d70 792e 7377 6170  rls = numpy.swap
+0000cc10: 6178 6573 2863 6f70 795f 7572 6c73 2c20  axes(copy_urls, 
+0000cc20: 302c 2061 7869 7329 5b0a 2020 2020 2020  0, axis)[.      
 0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc40: 2020 636f 7079 5f75 726c 7320 3d20 6e75    copy_urls = nu
-0000cc50: 6d70 792e 7377 6170 6178 6573 2863 6f70  mpy.swapaxes(cop
-0000cc60: 795f 7572 6c73 2c20 302c 2061 7869 7329  y_urls, 0, axis)
-0000cc70: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0000cc40: 2020 2020 2020 2020 2020 6469 6d65 6e73            dimens
+0000cc50: 696f 6e5b 315d 5b69 5d2c 203a 0a20 2020  ion[1][i], :.   
+0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
 0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2020 6469 6d65 6e73 696f 6e5b 315d 5b69    dimension[1][i
-0000cca0: 5d2c 203a 0a20 2020 2020 2020 2020 2020  ], :.           
-0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-0000ccd0: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-0000cce0: 7572 6c73 5b3a 5d20 3d20 7572 6c73 0a20  urls[:] = urls. 
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000cd00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cd10: 2020 2020 2020 2020 2075 726c 7320 3d20           urls = 
-0000cd20: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-0000cd30: 2020 2020 2020 2066 6f72 2069 2c20 6964         for i, id
-0000cd40: 7820 696e 2065 6e75 6d65 7261 7465 2872  x in enumerate(r
-0000cd50: 696e 6469 6365 7329 3a0a 2020 2020 2020  indices):.      
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 6966 206e 6f74 2073 656c 662e 7374    if not self.st
-0000cd80: 6174 655f 6f66 5f6f 7065 7261 7469 6f6e  ate_of_operation
-0000cd90: 732e 6973 5f72 756e 6e69 6e67 284f 7065  s.is_running(Ope
-0000cda0: 7261 7469 6f6e 2e53 4849 4654 293a 0a20  ration.SHIFT):. 
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2020 2020 2020 2020 2069 6620 2275             if "u
-0000cdd0: 7064 6174 655f 6461 7461 7365 7422 2069  pdate_dataset" i
-0000cde0: 6e20 5f66 696c 653a 0a20 2020 2020 2020  n _file:.       
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 2020 2020 2020 2064 656c 205f 6669           del _fi
-0000ce10: 6c65 5b22 7570 6461 7465 5f64 6174 6173  le["update_datas
-0000ce20: 6574 225d 0a20 2020 2020 2020 2020 2020  et"].           
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce40: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 6966 2073 6869 6674 5b3a 2c20 695d 2e61  if shift[:, i].a
-0000ce70: 6c6c 2829 203e 2031 3a0a 2020 2020 2020  ll() > 1:.      
-0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce90: 2020 2020 2020 7368 6966 745f 6170 7072        shift_appr
-0000cea0: 6f61 6368 203d 2022 6c69 6e65 6172 220a  oach = "linear".
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 2020 2020 696d 6720 3d20 6170          img = ap
-0000ced0: 706c 795f 7368 6966 7428 6461 7461 5b69  ply_shift(data[i
-0000cee0: 5d2c 2073 6869 6674 5b3a 2c20 695d 2c20  ], shift[:, i], 
-0000cef0: 7368 6966 745f 6170 7072 6f61 6368 290a  shift_approach).
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2020 2020 5f66 696c 655b 6461          _file[da
-0000cf20: 7461 7365 745f 6e61 6d65 5d5b 6964 785d  taset_name][idx]
-0000cf30: 203d 2069 6d67 0a20 2020 2020 2020 2020   = img.         
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0000cf50: 726c 732e 6170 7065 6e64 280a 2020 2020  rls.append(.    
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2020 2020 2020 2020 4461 7461 5572 6c28          DataUrl(
-0000cf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfa0: 2066 696c 655f 7061 7468 3d5f 6469 7220   file_path=_dir 
-0000cfb0: 2b20 222f 6461 7461 2e68 6466 3522 2c0a  + "/data.hdf5",.
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2020 2020 2020 2062 6f6f 6c5f 696e 6469         bool_indi
+0000cca0: 6365 7320 3d20 6e75 6d70 792e 7377 6170  ces = numpy.swap
+0000ccb0: 6178 6573 2862 6f6f 6c5f 696e 6469 6365  axes(bool_indice
+0000ccc0: 732c 2030 2c20 6178 6973 295b 0a20 2020  s, 0, axis)[.   
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+0000ccf0: 656e 7369 6f6e 5b31 5d5b 695d 2c20 3a0a  ension[1][i], :.
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd30: 2020 2020 2020 636f 7079 5f75 726c 735b        copy_urls[
+0000cd40: 626f 6f6c 5f69 6e64 6963 6573 5d20 3d20  bool_indices] = 
+0000cd50: 7572 6c73 0a20 2020 2020 2020 2020 2020  urls.           
+0000cd60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd80: 2020 2020 2020 2066 6f72 2069 2c20 6469         for i, di
+0000cd90: 6d20 696e 2065 6e75 6d65 7261 7465 2873  m in enumerate(s
+0000cda0: 6f72 7465 6428 6469 6d65 6e73 696f 6e5b  orted(dimension[
+0000cdb0: 305d 2929 3a0a 2020 2020 2020 2020 2020  0])):.          
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 2020 2320 466c 6970 2061 7869 7320 746f    # Flip axis to
+0000cde0: 2062 6520 636f 6e73 6973 7465 6e74 2077   be consistent w
+0000cdf0: 6974 6820 7468 6520 6461 7461 2073 6861  ith the data sha
+0000ce00: 7065 0a20 2020 2020 2020 2020 2020 2020  pe.             
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000ce20: 7869 7320 3d20 7365 6c66 2e64 696d 732e  xis = self.dims.
+0000ce30: 6e64 696d 202d 2064 696d 202d 2031 0a20  ndim - dim - 1. 
+0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce50: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
+0000ce60: 7572 6c73 203d 206e 756d 7079 2e73 7761  urls = numpy.swa
+0000ce70: 7061 7865 7328 636f 7079 5f75 726c 732c  paxes(copy_urls,
+0000ce80: 2030 2c20 6178 6973 295b 0a20 2020 2020   0, axis)[.     
+0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cea0: 2020 2020 2020 2020 2020 2064 696d 656e             dimen
+0000ceb0: 7369 6f6e 5b31 5d5b 695d 2c20 3a0a 2020  sion[1][i], :.  
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 2020 2020 636f 7079 5f75 726c 735b 3a5d      copy_urls[:]
+0000cf00: 203d 2075 726c 730a 2020 2020 2020 2020   = urls.        
+0000cf10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 7572 6c73 203d 205b 5d0a 2020 2020    urls = [].    
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 666f 7220 692c 2069 6478 2069 6e20 656e  for i, idx in en
+0000cf60: 756d 6572 6174 6528 7269 6e64 6963 6573  umerate(rindices
+0000cf70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000cf80: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000cf90: 7420 7365 6c66 2e73 7461 7465 5f6f 665f  t self.state_of_
+0000cfa0: 6f70 6572 6174 696f 6e73 2e69 735f 7275  operations.is_ru
+0000cfb0: 6e6e 696e 6728 4f70 6572 6174 696f 6e2e  nning(Operation.
+0000cfc0: 5348 4946 5429 3a0a 2020 2020 2020 2020  SHIFT):.        
 0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 6461 7461 5f70 6174 683d 222f 6461 7461  data_path="/data
-0000cff0: 7365 7422 2c0a 2020 2020 2020 2020 2020  set",.          
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 6461 7461 5f73 6c69 6365        data_slice
-0000d020: 3d69 6478 2c0a 2020 2020 2020 2020 2020  =idx,.          
-0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d040: 2020 2020 2020 7363 6865 6d65 3d22 7369        scheme="si
-0000d050: 6c78 222c 0a20 2020 2020 2020 2020 2020  lx",.           
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000d080: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0a0: 2020 2020 2069 6f5f 7574 696c 732e 6164       io_utils.ad
-0000d0b0: 7661 6e63 656d 656e 745f 6469 7370 6c61  vancement_displa
-0000d0c0: 7928 6920 2b20 312c 206c 656e 2864 6174  y(i + 1, len(dat
-0000d0d0: 6129 2c20 2241 7070 6c79 696e 6720 7368  a), "Applying sh
-0000d0e0: 6966 7422 290a 2020 2020 2020 2020 2020  ift").          
-0000d0f0: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
-0000d100: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
-0000d110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d120: 2020 2020 2020 2020 2020 6e65 775f 7572            new_ur
-0000d130: 6c73 203d 206e 756d 7079 2e61 7272 6179  ls = numpy.array
-0000d140: 2873 656c 662e 6461 7461 2e75 726c 732c  (self.data.urls,
-0000d150: 2064 7479 7065 3d6f 626a 6563 7429 2e66   dtype=object).f
-0000d160: 6c61 7474 656e 2829 0a20 2020 2020 2020  latten().       
-0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 206e 756d 7079 2e70 7574 286e 6577 5f75   numpy.put(new_u
-0000d190: 726c 732c 2069 6e64 6963 6573 2c20 7572  rls, indices, ur
-0000d1a0: 6c73 290a 2020 2020 2020 2020 2020 2020  ls).            
-0000d1b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1d0: 2020 2020 2020 6e65 775f 7572 6c73 203d        new_urls =
-0000d1e0: 206e 756d 7079 2e61 7272 6179 2875 726c   numpy.array(url
-0000d1f0: 7329 0a0a 2020 2020 2020 2020 2020 2020  s)..            
-0000d200: 2020 2020 6966 2064 6174 6173 6574 5f6e      if dataset_n
-0000d210: 616d 6520 3d3d 2022 7570 6461 7465 5f64  ame == "update_d
-0000d220: 6174 6173 6574 223a 0a20 2020 2020 2020  ataset":.       
-0000d230: 2020 2020 2020 2020 2020 2020 2064 656c               del
-0000d240: 205f 6669 6c65 5b22 6461 7461 7365 7422   _file["dataset"
-0000d250: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000d260: 2020 2020 2020 5f66 696c 655b 2264 6174        _file["dat
-0000d270: 6173 6574 225d 203d 205f 6669 6c65 5b22  aset"] = _file["
-0000d280: 7570 6461 7465 5f64 6174 6173 6574 225d  update_dataset"]
-0000d290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d2a0: 2020 2020 2064 656c 205f 6669 6c65 5b22       del _file["
-0000d2b0: 7570 6461 7465 5f64 6174 6173 6574 225d  update_dataset"]
-0000d2c0: 0a20 2020 2020 2020 2020 2020 2066 696e  .            fin
-0000d2d0: 616c 6c79 3a0a 2020 2020 2020 2020 2020  ally:.          
-0000d2e0: 2020 2020 2020 6966 205f 6669 6c65 2069        if _file i
-0000d2f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000cfe0: 2020 2020 6966 2022 7570 6461 7465 5f64      if "update_d
+0000cff0: 6174 6173 6574 2220 696e 205f 6669 6c65  ataset" in _file
+0000d000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 6465 6c20 5f66 696c 655b 2275 7064    del _file["upd
+0000d030: 6174 655f 6461 7461 7365 7422 5d0a 2020  ate_dataset"].  
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000d060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d070: 2020 2020 2020 2020 2069 6620 7368 6966           if shif
+0000d080: 745b 3a2c 2069 5d2e 616c 6c28 2920 3e20  t[:, i].all() > 
+0000d090: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d0b0: 6869 6674 5f61 7070 726f 6163 6820 3d20  hift_approach = 
+0000d0c0: 226c 696e 6561 7222 0a20 2020 2020 2020  "linear".       
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2069 6d67 203d 2061 7070 6c79 5f73 6869   img = apply_shi
+0000d0f0: 6674 2864 6174 615b 695d 2c20 7368 6966  ft(data[i], shif
+0000d100: 745b 3a2c 2069 5d2c 2073 6869 6674 5f61  t[:, i], shift_a
+0000d110: 7070 726f 6163 6829 0a20 2020 2020 2020  pproach).       
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 205f 6669 6c65 5b64 6174 6173 6574 5f6e   _file[dataset_n
+0000d140: 616d 655d 5b69 6478 5d20 3d20 696d 670a  ame][idx] = img.
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 7572 6c73 2e61 7070          urls.app
+0000d170: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d190: 2044 6174 6155 726c 280a 2020 2020 2020   DataUrl(.      
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
+0000d1c0: 6174 683d 5f64 6972 202b 2022 2f64 6174  ath=_dir + "/dat
+0000d1d0: 612e 6864 6635 222c 0a20 2020 2020 2020  a.hdf5",.       
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2020 2020 2020 2020 2064 6174 615f 7061           data_pa
+0000d200: 7468 3d22 2f64 6174 6173 6574 222c 0a20  th="/dataset",. 
+0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000d230: 6174 615f 736c 6963 653d 6964 782c 0a20  ata_slice=idx,. 
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d260: 6368 656d 653d 2273 696c 7822 2c0a 2020  cheme="silx",.  
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 696f                io
+0000d2c0: 5f75 7469 6c73 2e61 6476 616e 6365 6d65  _utils.advanceme
+0000d2d0: 6e74 5f64 6973 706c 6179 2869 202b 2031  nt_display(i + 1
+0000d2e0: 2c20 6c65 6e28 6461 7461 292c 2022 4170  , len(data), "Ap
+0000d2f0: 706c 7969 6e67 2073 6869 6674 2229 0a20  plying shift"). 
 0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 5f66 696c 652e 636c 6f73 6528 290a 0a20  _file.close().. 
-0000d320: 2020 2020 2020 2064 6174 6120 3d20 4461         data = Da
-0000d330: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
-0000d340: 6e65 775f 7572 6c73 2e72 6573 6861 7065  new_urls.reshape
-0000d350: 2873 656c 662e 6461 7461 2e75 726c 732e  (self.data.urls.
-0000d360: 7368 6170 6529 2c0a 2020 2020 2020 2020  shape),.        
-0000d370: 2020 2020 7365 6c66 2e64 6174 612e 6d65      self.data.me
-0000d380: 7461 6461 7461 2c0a 2020 2020 2020 2020  tadata,.        
-0000d390: 2020 2020 696e 5f6d 656d 6f72 793d 7365      in_memory=se
-0000d3a0: 6c66 2e5f 696e 5f6d 656d 6f72 792c 0a20  lf._in_memory,. 
-0000d3b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d3c0: 2072 6574 7572 6e20 4461 7461 7365 7428   return Dataset(
-0000d3d0: 0a20 2020 2020 2020 2020 2020 205f 6469  .            _di
-0000d3e0: 723d 5f64 6972 2c0a 2020 2020 2020 2020  r=_dir,.        
-0000d3f0: 2020 2020 6461 7461 3d64 6174 612c 0a20      data=data,. 
-0000d400: 2020 2020 2020 2020 2020 2064 696d 733d             dims=
-0000d410: 7365 6c66 2e5f 5f64 696d 732c 0a20 2020  self.__dims,.   
-0000d420: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-0000d430: 726d 6174 696f 6e3d 7365 6c66 2e74 7261  rmation=self.tra
-0000d440: 6e73 666f 726d 6174 696f 6e2c 0a20 2020  nsformation,.   
-0000d450: 2020 2020 2020 2020 2069 6e5f 6d65 6d6f           in_memo
-0000d460: 7279 3d73 656c 662e 5f69 6e5f 6d65 6d6f  ry=self._in_memo
-0000d470: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-0000d480: 7469 746c 653d 7365 6c66 2e74 6974 6c65  title=self.title
-0000d490: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000d4a0: 2064 6566 2066 696e 645f 616e 645f 6170   def find_and_ap
-0000d4b0: 706c 795f 7368 6966 7428 0a20 2020 2020  ply_shift(.     
-0000d4c0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000d4d0: 2064 696d 656e 7369 6f6e 3d4e 6f6e 652c   dimension=None,
-0000d4e0: 0a20 2020 2020 2020 2073 7465 7073 3d31  .        steps=1
-0000d4f0: 3030 2c0a 2020 2020 2020 2020 7368 6966  00,.        shif
-0000d500: 745f 6170 7072 6f61 6368 3d22 6666 7422  t_approach="fft"
-0000d510: 2c0a 2020 2020 2020 2020 696e 6469 6365  ,.        indice
-0000d520: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0000d530: 6361 6c6c 6261 636b 3d4e 6f6e 652c 0a20  callback=None,. 
-0000d540: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000d550: 220a 2020 2020 2020 2020 4669 6e64 2074  ".        Find t
-0000d560: 6865 2073 6869 6674 206f 6620 7468 6520  he shift of the 
-0000d570: 6461 7461 206f 7220 7061 7274 206f 6620  data or part of 
-0000d580: 6974 2061 6e64 2061 7070 6c79 2069 742e  it and apply it.
-0000d590: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000d5a0: 2064 696d 656e 7369 6f6e 3a20 5061 7261   dimension: Para
-0000d5b0: 6d65 7465 7320 7769 7468 2074 6865 2070  metes with the p
-0000d5c0: 6f73 6974 696f 6e20 6f66 2074 6865 2064  osition of the d
-0000d5d0: 6174 6120 696e 2074 6865 2072 6573 6861  ata in the resha
-0000d5e0: 7065 640a 2020 2020 2020 2020 2020 2020  ped.            
-0000d5f0: 6172 7261 792e 0a20 2020 2020 2020 203a  array..        :
-0000d600: 7479 7065 2064 696d 656e 7369 6f6e 3a20  type dimension: 
-0000d610: 556e 696f 6e5b 4e6f 6e65 2c20 7475 706c  Union[None, tupl
-0000d620: 652c 2061 7272 6179 5f6c 696b 655d 0a20  e, array_like]. 
-0000d630: 2020 2020 2020 203a 7061 7261 6d20 666c         :param fl
-0000d640: 6f61 7420 685f 6d61 783a 2053 6565 2060  oat h_max: See `
-0000d650: 636f 7265 2e69 6d61 6765 5265 6769 7374  core.imageRegist
-0000d660: 7261 7469 6f6e 2e73 6869 6674 5f64 6574  ration.shift_det
-0000d670: 6563 7469 6f6e 600a 2020 2020 2020 2020  ection`.        
-0000d680: 3a70 6172 616d 2066 6c6f 6174 2068 5f73  :param float h_s
-0000d690: 7465 703a 2053 6565 2060 636f 7265 2e69  tep: See `core.i
-0000d6a0: 6d61 6765 5265 6769 7374 7261 7469 6f6e  mageRegistration
-0000d6b0: 2e73 6869 6674 5f64 6574 6563 7469 6f6e  .shift_detection
-0000d6c0: 600a 2020 2020 2020 2020 3a70 6172 616d  `.        :param
-0000d6d0: 2055 6e69 6f6e 5b27 6666 7427 2c20 276c   Union['fft', 'l
-0000d6e0: 696e 6561 7227 5d20 7368 6966 745f 6170  inear'] shift_ap
-0000d6f0: 7072 6f61 6368 3a20 4d65 7468 6f64 2074  proach: Method t
-0000d700: 6f20 7573 6520 746f 2061 7070 6c79 2074  o use to apply t
-0000d710: 6865 2073 6869 6674 2e0a 2020 2020 2020  he shift..      
-0000d720: 2020 3a70 6172 616d 2069 6e64 6963 6573    :param indices
-0000d730: 3a20 496e 6469 6365 7320 6f66 2074 6865  : Indices of the
-0000d740: 2069 6d61 6765 7320 746f 2066 696e 6420   images to find 
-0000d750: 616e 6420 6170 706c 7920 7468 6520 7368  and apply the sh
-0000d760: 6966 7420 746f 2e0a 2020 2020 2020 2020  ift to..        
-0000d770: 2020 2020 4966 204e 6f6e 652c 2074 6865      If None, the
-0000d780: 2068 6f74 2070 6978 656c 2072 656d 6f76   hot pixel remov
-0000d790: 616c 2069 7320 6170 706c 6965 6420 746f  al is applied to
-0000d7a0: 2061 6c6c 2074 6865 2064 6174 612e 0a20   all the data.. 
-0000d7b0: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
-0000d7c0: 6963 6573 3a20 556e 696f 6e5b 4e6f 6e65  ices: Union[None
-0000d7d0: 2c20 6172 7261 795f 6c69 6b65 5d0a 2020  , array_like].  
-0000d7e0: 2020 2020 2020 3a70 6172 616d 2055 6e69        :param Uni
-0000d7f0: 6f6e 5b66 756e 6374 696f 6e2c 204e 6f6e  on[function, Non
-0000d800: 655d 2063 616c 6c62 6163 6b3a 2043 616c  e] callback: Cal
-0000d810: 6c62 6163 6b0a 2020 2020 2020 2020 3a72  lback.        :r
-0000d820: 6574 7572 6e73 3a20 4461 7461 7365 7420  eturns: Dataset 
-0000d830: 7769 7468 2074 6865 206e 6577 2064 6174  with the new dat
-0000d840: 612e 0a20 2020 2020 2020 2022 2222 0a20  a..        """. 
-0000d850: 2020 2020 2020 2073 6869 6674 203d 2073         shift = s
-0000d860: 656c 662e 6669 6e64 5f73 6869 6674 2864  elf.find_shift(d
-0000d870: 696d 656e 7369 6f6e 2c20 7374 6570 732c  imension, steps,
-0000d880: 2069 6e64 6963 6573 3d69 6e64 6963 6573   indices=indices
-0000d890: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d8a0: 2073 656c 662e 6170 706c 795f 7368 6966   self.apply_shif
-0000d8b0: 7428 7368 6966 742c 2064 696d 656e 7369  t(shift, dimensi
-0000d8c0: 6f6e 2c20 696e 6469 6365 733d 696e 6469  on, indices=indi
-0000d8d0: 6365 7329 0a0a 2020 2020 6465 6620 5f77  ces)..    def _w
-0000d8e0: 6174 6572 6661 6c6c 5f6e 6d66 280a 2020  aterfall_nmf(.  
-0000d8f0: 2020 2020 2020 7365 6c66 2c20 6e75 6d5f        self, num_
-0000d900: 636f 6d70 6f6e 656e 7473 2c20 6974 6572  components, iter
-0000d910: 6174 696f 6e73 2c20 7673 7465 703d 4e6f  ations, vstep=No
-0000d920: 6e65 2c20 6873 7465 703d 4e6f 6e65 2c20  ne, hstep=None, 
-0000d930: 696e 6469 6365 733d 4e6f 6e65 0a20 2020  indices=None.   
-0000d940: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-0000d950: 2020 2020 2020 2020 5468 6973 206d 6574          This met
-0000d960: 686f 6420 6973 2075 7365 6420 6173 2061  hod is used as a
-0000d970: 2077 6179 2074 6f20 696d 7072 6f76 6520   way to improve 
-0000d980: 7468 6520 7370 6565 6420 6f66 2063 6f6e  the speed of con
-0000d990: 7665 7267 656e 6365 206f 660a 2020 2020  vergence of.    
-0000d9a0: 2020 2020 7468 6520 4e4d 4620 6d65 7468      the NMF meth
-0000d9b0: 6f64 2e20 466f 7220 7468 6973 2c20 6974  od. For this, it
-0000d9c0: 2075 7365 7320 6120 7761 7465 7266 616c   uses a waterfal
-0000d9d0: 6c20 6d6f 6465 6c20 7768 6572 6520 6174  l model where at
-0000d9e0: 2065 7665 7279 2073 7465 700a 2020 2020   every step.    
-0000d9f0: 2020 2020 7468 6520 6f75 7470 7574 206d      the output m
-0000da00: 6174 7269 6365 7320 7365 7276 6520 6173  atrices serve as
-0000da10: 2069 6e70 7574 2066 6f72 2074 6865 206e   input for the n
-0000da20: 6578 742e 0a20 2020 2020 2020 2054 6861  ext..        Tha
-0000da30: 7420 6973 2c20 7468 6520 6d65 7468 6f64  t is, the method
-0000da40: 2073 7461 7274 7320 7769 7468 2061 2073   starts with a s
-0000da50: 6d61 6c6c 6572 2072 6573 697a 6564 2069  maller resized i
-0000da60: 6d61 6765 7320 6f66 2074 6865 2064 6174  mages of the dat
-0000da70: 612c 0a20 2020 2020 2020 2061 6e64 2063  a,.        and c
-0000da80: 6f6d 7075 7465 7320 7468 6520 4e4d 4620  omputes the NMF 
-0000da90: 6465 636f 6d70 6f73 6974 696f 6e2e 2054  decomposition. T
-0000daa0: 6865 206e 6578 7420 7374 6570 2069 7320  he next step is 
-0000dab0: 7468 6520 7361 6d65 2062 7574 2077 6974  the same but wit
-0000dac0: 680a 2020 2020 2020 2020 6269 6767 6572  h.        bigger
-0000dad0: 2069 6d61 6765 732c 2061 6e64 2075 7369   images, and usi
-0000dae0: 6e67 2061 7320 696e 6974 6961 6c20 4820  ng as initial H 
-0000daf0: 616e 6420 5720 7468 6520 7072 6563 6f6d  and W the precom
-0000db00: 7075 7465 6420 6d61 7472 6963 6573 2e0a  puted matrices..
-0000db10: 2020 2020 2020 2020 5468 6520 6c61 7374          The last
-0000db20: 2073 7465 7020 6973 2064 6f6e 6520 7573   step is done us
-0000db30: 696e 6720 7468 6520 6163 7475 616c 2073  ing the actual s
-0000db40: 697a 6520 6f66 2074 6865 2069 6d61 6765  ize of the image
-0000db50: 732e 0a20 2020 2020 2020 2054 6869 7320  s..        This 
-0000db60: 7761 792c 2074 6865 206e 756d 6265 7220  way, the number 
-0000db70: 6f66 2069 7465 7261 7469 6f6e 7320 7769  of iterations wi
-0000db80: 7468 2062 6967 2069 6d61 6765 7320 6361  th big images ca
-0000db90: 6e20 6265 2064 696d 696e 6973 6865 642c  n be diminished,
-0000dba0: 2061 6e64 0a20 2020 2020 2020 2074 6865   and.        the
-0000dbb0: 206d 6574 686f 6420 636f 6e76 6572 6765   method converge
-0000dbc0: 7320 6661 7374 6572 2e0a 0a20 2020 2020  s faster...     
-0000dbd0: 2020 203a 7061 7261 6d20 696e 7420 6e75     :param int nu
-0000dbe0: 6d5f 636f 6d70 6f6e 656e 7473 3a20 4e75  m_components: Nu
-0000dbf0: 6d62 6572 206f 6620 636f 6d70 6f6e 656e  mber of componen
-0000dc00: 7473 2074 6f20 6669 6e64 2e0a 2020 2020  ts to find..    
-0000dc10: 2020 2020 3a70 6172 616d 2061 7272 6179      :param array
-0000dc20: 5f6c 696b 6520 6974 6572 6174 696f 6e73  _like iterations
-0000dc30: 3a20 4172 7261 7920 7769 7468 206e 756d  : Array with num
-0000dc40: 6265 7220 6f66 2069 7465 7261 7469 6f6e  ber of iteration
-0000dc50: 7320 7065 7220 7374 6570 206f 6620 7468  s per step of th
-0000dc60: 6520 7761 7465 7266 616c 6c2e 0a20 2020  e waterfall..   
-0000dc70: 2020 2020 2020 2020 2054 6865 2073 697a           The siz
-0000dc80: 6520 6f66 2074 6865 2061 7272 6179 2073  e of the array s
-0000dc90: 6574 7320 7468 6520 7369 7a65 206f 6620  ets the size of 
-0000dca0: 7468 6520 7761 7465 7266 616c 6c2e 0a20  the waterfall.. 
-0000dcb0: 2020 2020 2020 203a 7061 7261 6d20 556e         :param Un
-0000dcc0: 696f 6e5b 4e6f 6e65 2c20 6172 7261 795f  ion[None, array_
-0000dcd0: 6c69 6b65 5d20 696e 6469 6365 733a 2049  like] indices: I
-0000dce0: 6620 6e6f 7420 4e6f 6e65 2c20 6170 706c  f not None, appl
-0000dcf0: 7920 6d65 7468 6f64 206f 6e6c 7920 746f  y method only to
-0000dd00: 2069 6e64 6963 6573 206f 6620 6461 7461   indices of data
-0000dd10: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-0000dd20: 2020 2020 2020 2066 726f 6d20 736b 696d         from skim
-0000dd30: 6167 652e 7472 616e 7366 6f72 6d20 696d  age.transform im
-0000dd40: 706f 7274 2072 6573 697a 650a 2020 2020  port resize.    
-0000dd50: 2020 2020 696d 706f 7274 2073 6875 7469      import shuti
-0000dd60: 6c0a 0a20 2020 2020 2020 2057 203d 204e  l..        W = N
-0000dd70: 6f6e 650a 2020 2020 2020 2020 4820 3d20  one.        H = 
-0000dd80: 4e6f 6e65 0a20 2020 2020 2020 2073 6861  None.        sha
-0000dd90: 7065 203d 206e 756d 7079 2e61 7361 7272  pe = numpy.asarr
-0000dda0: 6179 2873 656c 662e 6765 745f 6461 7461  ay(self.get_data
-0000ddb0: 2830 292e 7368 6170 6529 0a20 2020 2020  (0).shape).     
-0000ddc0: 2020 2066 6972 7374 5f73 697a 6520 3d20     first_size = 
-0000ddd0: 2873 6861 7065 202f 2028 6c65 6e28 6974  (shape / (len(it
-0000dde0: 6572 6174 696f 6e73 2920 2b20 3129 292e  erations) + 1)).
-0000ddf0: 6173 7479 7065 2869 6e74 290a 2020 2020  astype(int).    
-0000de00: 2020 2020 7369 7a65 203d 2066 6972 7374      size = first
-0000de10: 5f73 697a 650a 0a20 2020 2020 2020 206f  _size..        o
-0000de20: 732e 6d61 6b65 6469 7273 286f 732e 7061  s.makedirs(os.pa
-0000de30: 7468 2e6a 6f69 6e28 7365 6c66 2e64 6972  th.join(self.dir
-0000de40: 2c20 2277 6174 6572 6661 6c6c 2229 2c20  , "waterfall"), 
-0000de50: 6578 6973 745f 6f6b 3d54 7275 6529 0a0a  exist_ok=True)..
-0000de60: 2020 2020 2020 2020 5f6c 6f67 6765 722e          _logger.
-0000de70: 696e 666f 2822 5374 6172 7469 6e67 2077  info("Starting w
-0000de80: 6174 6572 6661 6c6c 204e 4d46 2229 0a0a  aterfall NMF")..
-0000de90: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000dea0: 2072 616e 6765 286c 656e 2869 7465 7261   range(len(itera
-0000deb0: 7469 6f6e 7329 293a 0a20 2020 2020 2020  tions)):.       
-0000dec0: 2020 2020 206e 6577 5f75 726c 7320 3d20       new_urls = 
-0000ded0: 5b5d 0a20 2020 2020 2020 2020 2020 2069  [].            i
-0000dee0: 6620 696e 6469 6365 7320 6973 204e 6f6e  f indices is Non
-0000def0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000df00: 2020 2069 6e64 6963 6573 203d 2072 616e     indices = ran
-0000df10: 6765 2873 656c 662e 6e66 7261 6d65 7329  ge(self.nframes)
-0000df20: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000df30: 206a 2069 6e20 696e 6469 6365 733a 0a20   j in indices:. 
-0000df40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000df50: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
-0000df60: 682e 6a6f 696e 2873 656c 662e 6469 722c  h.join(self.dir,
-0000df70: 2022 7761 7465 7266 616c 6c22 2c20 7374   "waterfall", st
-0000df80: 7228 6a29 202b 2022 2e6e 7079 2229 0a20  r(j) + ".npy"). 
-0000df90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000dfa0: 756d 7079 2e73 6176 6528 6669 6c65 6e61  umpy.save(filena
-0000dfb0: 6d65 2c20 7265 7369 7a65 2873 656c 662e  me, resize(self.
-0000dfc0: 6765 745f 6461 7461 286a 292c 2073 697a  get_data(j), siz
-0000dfd0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-0000dfe0: 2020 2020 6e65 775f 7572 6c73 2e61 7070      new_urls.app
-0000dff0: 656e 6428 4461 7461 5572 6c28 6669 6c65  end(DataUrl(file
-0000e000: 5f70 6174 683d 6669 6c65 6e61 6d65 2c20  _path=filename, 
-0000e010: 7363 6865 6d65 3d22 6661 6269 6f22 2929  scheme="fabio"))
-0000e020: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000e030: 6120 3d20 4461 7461 286e 6577 5f75 726c  a = Data(new_url
-0000e040: 732c 2073 656c 662e 6765 745f 6461 7461  s, self.get_data
-0000e050: 2869 6e64 6963 6573 292e 6d65 7461 6461  (indices).metada
-0000e060: 7461 2c20 7365 6c66 2e5f 696e 5f6d 656d  ta, self._in_mem
-0000e070: 6f72 7929 0a20 2020 2020 2020 2020 2020  ory).           
-0000e080: 2064 6174 6173 6574 203d 2044 6174 6173   dataset = Datas
-0000e090: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000e0a0: 2020 2020 5f64 6972 3d6f 732e 7061 7468      _dir=os.path
-0000e0b0: 2e6a 6f69 6e28 7365 6c66 2e64 6972 2c20  .join(self.dir, 
-0000e0c0: 2277 6174 6572 6661 6c6c 2229 2c0a 2020  "waterfall"),.  
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000e0e0: 7461 3d64 6174 612c 0a20 2020 2020 2020  ta=data,.       
-0000e0f0: 2020 2020 2020 2020 2069 6e5f 6d65 6d6f           in_memo
-0000e100: 7279 3d73 656c 662e 5f69 6e5f 6d65 6d6f  ry=self._in_memo
-0000e110: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-0000e120: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000e130: 2076 7374 6570 3a0a 2020 2020 2020 2020   vstep:.        
-0000e140: 2020 2020 2020 2020 765f 7374 6570 203d          v_step =
-0000e150: 2076 7374 6570 202a 2028 6c65 6e28 6974   vstep * (len(it
-0000e160: 6572 6174 696f 6e73 2920 2d20 6929 0a20  erations) - i). 
-0000e170: 2020 2020 2020 2020 2020 2069 6620 6873             if hs
-0000e180: 7465 703a 0a20 2020 2020 2020 2020 2020  tep:.           
-0000e190: 2020 2020 2068 5f73 7465 7020 3d20 6873       h_step = hs
-0000e1a0: 7465 7020 2a20 286c 656e 2869 7465 7261  tep * (len(itera
-0000e1b0: 7469 6f6e 7329 202d 2069 290a 2020 2020  tions) - i).    
-0000e1c0: 2020 2020 2020 2020 482c 2057 203d 2064          H, W = d
-0000e1d0: 6174 6173 6574 2e6e 6d66 280a 2020 2020  ataset.nmf(.    
-0000e1e0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-0000e1f0: 636f 6d70 6f6e 656e 7473 2c20 6974 6572  components, iter
-0000e200: 6174 696f 6e73 5b69 5d2c 2057 3d57 2c20  ations[i], W=W, 
-0000e210: 483d 482c 2076 7374 6570 3d76 5f73 7465  H=H, vstep=v_ste
-0000e220: 702c 2068 7374 6570 3d68 5f73 7465 700a  p, hstep=h_step.
-0000e230: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000e240: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
-0000e250: 2066 6972 7374 5f73 697a 6520 2a20 2869   first_size * (i
-0000e260: 202b 2032 290a 2020 2020 2020 2020 2020   + 2).          
-0000e270: 2020 4832 203d 206e 756d 7079 2e65 6d70    H2 = numpy.emp
-0000e280: 7479 2828 482e 7368 6170 655b 305d 2c20  ty((H.shape[0], 
-0000e290: 7369 7a65 5b30 5d20 2a20 7369 7a65 5b31  size[0] * size[1
-0000e2a0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-0000e2b0: 666f 7220 726f 7720 696e 2072 616e 6765  for row in range
-0000e2c0: 2848 2e73 6861 7065 5b30 5d29 3a0a 2020  (H.shape[0]):.  
-0000e2d0: 2020 2020 2020 2020 2020 2020 2020 4832                H2
-0000e2e0: 5b72 6f77 5d20 3d20 7265 7369 7a65 2848  [row] = resize(H
-0000e2f0: 5b72 6f77 5d2e 7265 7368 6170 6528 2869  [row].reshape((i
-0000e300: 202b 2031 2920 2a20 6669 7273 745f 7369   + 1) * first_si
-0000e310: 7a65 292c 2073 697a 6529 2e66 6c61 7474  ze), size).flatt
-0000e320: 656e 2829 0a20 2020 2020 2020 2020 2020  en().           
-0000e330: 2048 203d 2048 320a 0a20 2020 2020 2020   H = H2..       
-0000e340: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000e350: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
-0000e360: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-0000e370: 662e 6469 722c 2022 7761 7465 7266 616c  f.dir, "waterfal
-0000e380: 6c22 2929 0a20 2020 2020 2020 2065 7863  l")).        exc
-0000e390: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-0000e3a0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-0000e3b0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0000e3c0: 2020 2020 2020 2022 4661 696c 6564 2074         "Failed t
-0000e3d0: 6f20 6465 6c65 7465 2025 732e 2052 6561  o delete %s. Rea
-0000e3e0: 736f 6e3a 2025 7322 0a20 2020 2020 2020  son: %s".       
-0000e3f0: 2020 2020 2020 2020 2025 2028 6f73 2e70           % (os.p
-0000e400: 6174 682e 6a6f 696e 2873 656c 662e 6469  ath.join(self.di
-0000e410: 722c 2022 7761 7465 7266 616c 6c22 292c  r, "waterfall"),
-0000e420: 2065 290a 2020 2020 2020 2020 2020 2020   e).            
-0000e430: 290a 0a20 2020 2020 2020 2048 203d 2072  )..        H = r
-0000e440: 6573 697a 6528 482c 2028 6e75 6d5f 636f  esize(H, (num_co
-0000e450: 6d70 6f6e 656e 7473 2c20 7368 6170 655b  mponents, shape[
-0000e460: 305d 202a 2073 6861 7065 5b31 5d29 290a  0] * shape[1])).
-0000e470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e480: 482c 2057 0a0a 2020 2020 6465 6620 7063  H, W..    def pc
-0000e490: 6128 7365 6c66 2c20 6e75 6d5f 636f 6d70  a(self, num_comp
-0000e4a0: 6f6e 656e 7473 3d4e 6f6e 652c 2063 6875  onents=None, chu
-0000e4b0: 6e6b 5f73 697a 653d 3530 302c 2069 6e64  nk_size=500, ind
-0000e4c0: 6963 6573 3d4e 6f6e 652c 2072 6574 7572  ices=None, retur
-0000e4d0: 6e5f 7661 6c73 3d46 616c 7365 293a 0a20  n_vals=False):. 
-0000e4e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e4f0: 2020 2043 6f6d 7075 7465 2050 7269 6e63     Compute Princ
-0000e500: 6970 616c 2043 6f6d 706f 6e65 6e74 2041  ipal Component A
-0000e510: 6e61 6c79 7369 7320 6f6e 2074 6865 2064  nalysis on the d
-0000e520: 6174 612e 0a20 2020 2020 2020 2054 6865  ata..        The
-0000e530: 206d 6574 686f 642c 2066 6972 7374 2063   method, first c
-0000e540: 6f6e 7665 7274 732c 2069 6620 6e6f 7420  onverts, if not 
-0000e550: 616c 7265 6164 792c 2074 6865 2064 6174  already, the dat
-0000e560: 6120 696e 746f 2061 6e20 6864 6635 2066  a into an hdf5 f
-0000e570: 696c 6520 6f62 6a65 6374 0a20 2020 2020  ile object.     
-0000e580: 2020 2077 6974 6820 7468 6520 696d 6167     with the imag
-0000e590: 6573 2066 6c61 7474 656e 6564 2069 6e20  es flattened in 
-0000e5a0: 7468 6520 726f 7773 2e0a 0a20 2020 2020  the rows...     
-0000e5b0: 2020 203a 7061 7261 6d20 6e75 6d5f 636f     :param num_co
-0000e5c0: 6d70 6f6e 656e 7473 3a20 4e75 6d62 6572  mponents: Number
-0000e5d0: 206f 6620 636f 6d70 6f6e 656e 7473 2074   of components t
-0000e5e0: 6f20 6669 6e64 2e0a 2020 2020 2020 2020  o find..        
-0000e5f0: 2020 2020 4966 204e 6f6e 652c 2069 7420      If None, it 
-0000e600: 7573 6573 2074 6865 206d 696e 696d 756d  uses the minimum
-0000e610: 2062 6574 7765 656e 2074 6865 206e 756d   between the num
-0000e620: 6265 7220 6f66 2069 6d61 6765 7320 616e  ber of images an
-0000e630: 6420 7468 650a 2020 2020 2020 2020 2020  d the.          
-0000e640: 2020 6e75 6d62 6572 206f 6620 7069 7865    number of pixe
-0000e650: 6c73 2e0a 2020 2020 2020 2020 3a74 7970  ls..        :typ
-0000e660: 6520 6e75 6d5f 636f 6d70 6f6e 656e 7473  e num_components
-0000e670: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 696e  : Union[None, in
-0000e680: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
-0000e690: 6d20 6368 756e 6b5f 7369 7a65 3a20 4e75  m chunk_size: Nu
-0000e6a0: 6d62 6572 206f 6620 6368 756e 6b73 2066  mber of chunks f
-0000e6b0: 6f72 2077 6869 6368 2074 6865 2077 6869  or which the whi
-0000e6c0: 7465 6e69 6e67 206d 7573 7420 6265 2063  tening must be c
-0000e6d0: 6f6d 7075 7465 642c 0a20 2020 2020 2020  omputed,.       
-0000e6e0: 2020 2020 2069 6e63 7265 6d65 6e74 616c       incremental
-0000e6f0: 6c79 2c20 6465 6661 756c 7473 2074 6f20  ly, defaults to 
-0000e700: 4e6f 6e65 0a20 2020 2020 2020 203a 7479  None.        :ty
-0000e710: 7065 2063 6875 6e6b 7369 7a65 3a20 556e  pe chunksize: Un
-0000e720: 696f 6e5b 4e6f 6e65 2c20 696e 745d 2c20  ion[None, int], 
-0000e730: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000e740: 203a 7061 7261 6d20 696e 6469 6365 733a   :param indices:
-0000e750: 2049 6620 6e6f 7420 4e6f 6e65 2c20 6170   If not None, ap
-0000e760: 706c 7920 6d65 7468 6f64 206f 6e6c 7920  ply method only 
-0000e770: 746f 2069 6e64 6963 6573 206f 6620 6461  to indices of da
-0000e780: 7461 2c20 6465 6661 756c 7473 2074 6f20  ta, defaults to 
-0000e790: 4e6f 6e65 0a20 2020 2020 2020 203a 7479  None.        :ty
-0000e7a0: 7065 2069 6e64 6963 6573 3a20 556e 696f  pe indices: Unio
-0000e7b0: 6e5b 4e6f 6e65 2c20 6172 7261 795f 6c69  n[None, array_li
-0000e7c0: 6b65 5d2c 206f 7074 696f 6e61 6c0a 2020  ke], optional.  
-0000e7d0: 2020 2020 2020 3a70 6172 616d 2072 6574        :param ret
-0000e7e0: 7572 6e5f 7661 6c73 3a20 4966 2054 7275  urn_vals: If Tru
-0000e7f0: 652c 2072 6574 7572 6e73 206f 6e6c 7920  e, returns only 
-0000e800: 7468 6520 7369 6e67 756c 6172 2076 616c  the singular val
-0000e810: 7565 7320 6f66 2050 4341 2c20 656c 7365  ues of PCA, else
-0000e820: 2072 6574 7572 6e73 0a20 2020 2020 2020   returns.       
-0000e830: 2020 2020 2074 6865 2063 6f6d 706f 6e65       the compone
-0000e840: 6e74 7320 616e 6420 7468 6520 6d69 7869  nts and the mixi
-0000e850: 6e67 206d 6174 7269 782c 2064 6566 6175  ng matrix, defau
-0000e860: 6c74 7320 746f 2046 616c 7365 0a20 2020  lts to False.   
-0000e870: 2020 2020 203a 7479 7065 2072 6574 7572       :type retur
-0000e880: 6e5f 7661 6c73 3a20 626f 6f6c 2c20 6f70  n_vals: bool, op
-0000e890: 7469 6f6e 616c 0a0a 2020 2020 2020 2020  tional..        
-0000e8a0: 3a72 6574 7572 6e3a 2028 482c 2057 293a  :return: (H, W):
-0000e8b0: 2054 6865 2063 6f6d 706f 6e65 6e74 7320   The components 
-0000e8c0: 6d61 7472 6978 2061 6e64 2074 6865 206d  matrix and the m
-0000e8d0: 6978 696e 6720 6d61 7472 6978 2e0a 2020  ixing matrix..  
-0000e8e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e8f0: 2020 6273 735f 6469 7220 3d20 6f73 2e70    bss_dir = os.p
-0000e900: 6174 682e 6a6f 696e 2873 656c 662e 6469  ath.join(self.di
-0000e910: 722c 2022 6273 7322 290a 2020 2020 2020  r, "bss").      
-0000e920: 2020 6f73 2e6d 616b 6564 6972 7328 6273    os.makedirs(bs
-0000e930: 735f 6469 722c 2065 7869 7374 5f6f 6b3d  s_dir, exist_ok=
-0000e940: 5472 7565 290a 2020 2020 2020 2020 6966  True).        if
-0000e950: 2073 656c 662e 5f69 6e5f 6d65 6d6f 7279   self._in_memory
-0000e960: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
-0000e970: 6f6d 2073 6b6c 6561 726e 2069 6d70 6f72  om sklearn impor
-0000e980: 7420 6465 636f 6d70 6f73 6974 696f 6e0a  t decomposition.
-0000e990: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-0000e9a0: 656c 203d 2064 6563 6f6d 706f 7369 7469  el = decompositi
-0000e9b0: 6f6e 2e50 4341 286e 5f63 6f6d 706f 6e65  on.PCA(n_compone
-0000e9c0: 6e74 733d 6e75 6d5f 636f 6d70 6f6e 656e  nts=num_componen
-0000e9d0: 7473 290a 0a20 2020 2020 2020 2020 2020  ts)..           
-0000e9e0: 2077 6974 6820 7365 6c66 2e64 6174 612e   with self.data.
-0000e9f0: 6f70 656e 5f61 735f 6864 6635 2862 7373  open_as_hdf5(bss
-0000ea00: 5f64 6972 2920 6173 2068 3564 7365 743a  _dir) as h5dset:
-0000ea10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea20: 2069 6620 696e 6469 6365 7320 6973 206e   if indices is n
-0000ea30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ea40: 2020 2020 2020 2020 2020 2020 2057 203d               W =
-0000ea50: 206d 6f64 656c 2e66 6974 5f74 7261 6e73   model.fit_trans
-0000ea60: 666f 726d 2868 3564 7365 745b 696e 6469  form(h5dset[indi
-0000ea70: 6365 735d 290a 2020 2020 2020 2020 2020  ces]).          
-0000ea80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 5720 3d20 6d6f 6465 6c2e 6669 745f 7472  W = model.fit_tr
-0000eab0: 616e 7366 6f72 6d28 6835 6473 6574 5b3a  ansform(h5dset[:
-0000eac0: 2c20 3a5d 290a 0a20 2020 2020 2020 2020  , :])..         
-0000ead0: 2020 2048 2c20 7661 6c73 2c20 5720 3d20     H, vals, W = 
-0000eae0: 6d6f 6465 6c2e 636f 6d70 6f6e 656e 7473  model.components
-0000eaf0: 5f2c 206d 6f64 656c 2e73 696e 6775 6c61  _, model.singula
-0000eb00: 725f 7661 6c75 6573 5f2c 2057 0a20 2020  r_values_, W.   
-0000eb10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000eb20: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000eb30: 2e64 6174 612e 6f70 656e 5f61 735f 6864  .data.open_as_hd
-0000eb40: 6635 2862 7373 5f64 6972 2920 6173 2068  f5(bss_dir) as h
-0000eb50: 3564 7365 743a 0a20 2020 2020 2020 2020  5dset:.         
-0000eb60: 2020 2020 2020 206d 6f64 656c 203d 2049         model = I
-0000eb70: 5043 4128 0a20 2020 2020 2020 2020 2020  PCA(.           
-0000eb80: 2020 2020 2020 2020 2068 3564 7365 742c           h5dset,
-0000eb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eba0: 2020 2020 2063 6875 6e6b 5f73 697a 652c       chunk_size,
-0000ebb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebc0: 2020 2020 206e 756d 5f63 6f6d 706f 6e65       num_compone
-0000ebd0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
-0000ebe0: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-0000ebf0: 3d69 6e64 6963 6573 2c0a 2020 2020 2020  =indices,.      
-0000ec00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000ec10: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000ec20: 2068 3570 792e 4669 6c65 286f 732e 7061   h5py.File(os.pa
-0000ec30: 7468 2e6a 6f69 6e28 6273 735f 6469 722c  th.join(bss_dir,
-0000ec40: 2022 6970 6361 2e68 6466 3522 292c 2022   "ipca.hdf5"), "
-0000ec50: 7722 2920 6173 2066 696c 653a 0a20 2020  w") as file:.   
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2066 696c 655b 2257 225d 203d 206e 756d   file["W"] = num
-0000ec80: 7079 2e72 616e 646f 6d2e 7261 6e64 6f6d  py.random.random
-0000ec90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000eca0: 2020 2020 2020 2020 2020 286d 6f64 656c            (model
-0000ecb0: 2e6e 756d 5f73 616d 706c 6573 2c20 6d6f  .num_samples, mo
-0000ecc0: 6465 6c2e 6e75 6d5f 636f 6d70 6f6e 656e  del.num_componen
-0000ecd0: 7473 290a 2020 2020 2020 2020 2020 2020  ts).            
-0000ece0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000ed00: 6c65 5b22 4822 5d20 3d20 6e75 6d70 792e  le["H"] = numpy.
-0000ed10: 7261 6e64 6f6d 2e72 616e 646f 6d28 0a20  random.random(. 
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 2020 2028 6d6f 6465 6c2e 6e75         (model.nu
-0000ed40: 6d5f 636f 6d70 6f6e 656e 7473 2c20 6d6f  m_components, mo
-0000ed50: 6465 6c2e 6e75 6d5f 6665 6174 7572 6573  del.num_features
-0000ed60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ed70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000ed80: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000ed90: 2077 6172 6e69 6e67 732e 6361 7463 685f   warnings.catch_
-0000eda0: 7761 726e 696e 6773 2829 3a0a 2020 2020  warnings():.    
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edc0: 2020 2020 2320 7363 696b 6974 5f6c 6561      # scikit_lea
-0000edd0: 726e 3c31 2e31 2e31 0a20 2020 2020 2020  rn<1.1.1.       
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 2077 6172 6e69 6e67 732e 6669 6c74 6572   warnings.filter
-0000ee00: 7761 726e 696e 6773 280a 2020 2020 2020  warnings(.      
-0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee20: 2020 2020 2020 2261 6c77 6179 7322 2c20        "always", 
-0000ee30: 224d 6561 6e20 6f66 2065 6d70 7479 2073  "Mean of empty s
-0000ee40: 6c69 6365 2e22 2c20 5275 6e74 696d 6557  lice.", RuntimeW
-0000ee50: 6172 6e69 6e67 0a20 2020 2020 2020 2020  arning.         
-0000ee60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000ee70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ee80: 2020 2020 2020 2020 2077 6974 6820 6e75           with nu
-0000ee90: 6d70 792e 6572 7273 7461 7465 2869 6e76  mpy.errstate(inv
-0000eea0: 616c 6964 3d22 6967 6e6f 7265 222c 2064  alid="ignore", d
-0000eeb0: 6976 6964 653d 2269 676e 6f72 6522 293a  ivide="ignore"):
-0000eec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eed0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0000eee0: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
-0000eef0: 2857 3d66 696c 655b 2257 225d 2c20 483d  (W=file["W"], H=
-0000ef00: 6669 6c65 5b22 4822 5d29 0a0a 2020 2020  file["H"])..    
-0000ef10: 2020 2020 2020 2020 482c 2076 616c 732c          H, vals,
-0000ef20: 2057 203d 206d 6f64 656c 2e48 2c20 6d6f   W = model.H, mo
-0000ef30: 6465 6c2e 7369 6e67 756c 6172 5f76 616c  del.singular_val
-0000ef40: 7565 732c 206d 6f64 656c 2e57 0a20 2020  ues, model.W.   
-0000ef50: 2020 2020 2072 6574 7572 6e20 7661 6c73       return vals
-0000ef60: 2069 6620 7265 7475 726e 5f76 616c 7320   if return_vals 
-0000ef70: 656c 7365 2028 482c 2057 290a 0a20 2020  else (H, W)..   
-0000ef80: 2064 6566 206e 6963 6128 0a20 2020 2020   def nica(.     
-0000ef90: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000efa0: 206e 756d 5f63 6f6d 706f 6e65 6e74 732c   num_components,
-0000efb0: 0a20 2020 2020 2020 2063 6875 6e6b 7369  .        chunksi
-0000efc0: 7a65 3d4e 6f6e 652c 0a20 2020 2020 2020  ze=None,.       
-0000efd0: 206e 756d 5f69 7465 723d 3530 302c 0a20   num_iter=500,. 
-0000efe0: 2020 2020 2020 2065 7272 6f72 5f73 7465         error_ste
-0000eff0: 703d 4e6f 6e65 2c0a 2020 2020 2020 2020  p=None,.        
-0000f000: 696e 6469 6365 733d 4e6f 6e65 2c0a 2020  indices=None,.  
-0000f010: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000f020: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
-0000f030: 204e 6f6e 2d6e 6567 6174 6976 6520 496e   Non-negative In
-0000f040: 6465 7065 6e64 656e 7420 436f 6d70 6f6e  dependent Compon
-0000f050: 656e 7420 416e 616c 7973 6973 206f 6e20  ent Analysis on 
-0000f060: 7468 6520 6461 7461 2e0a 2020 2020 2020  the data..      
-0000f070: 2020 5468 6520 6d65 7468 6f64 2c20 6669    The method, fi
-0000f080: 7273 7420 636f 6e76 6572 7473 2c20 6966  rst converts, if
-0000f090: 206e 6f74 2061 6c72 6561 6479 2c20 7468   not already, th
-0000f0a0: 6520 6461 7461 2069 6e74 6f20 616e 2068  e data into an h
-0000f0b0: 6466 3520 6669 6c65 206f 626a 6563 740a  df5 file object.
-0000f0c0: 2020 2020 2020 2020 7769 7468 2074 6865          with the
-0000f0d0: 2069 6d61 6765 7320 666c 6174 7465 6e65   images flattene
-0000f0e0: 6420 696e 2074 6865 2072 6f77 732e 0a0a  d in the rows...
-0000f0f0: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
-0000f100: 756d 5f63 6f6d 706f 6e65 6e74 733a 204e  um_components: N
-0000f110: 756d 6265 7220 6f66 2063 6f6d 706f 6e65  umber of compone
-0000f120: 6e74 7320 746f 2066 696e 640a 2020 2020  nts to find.    
-0000f130: 2020 2020 3a74 7970 6520 6e75 6d5f 636f      :type num_co
-0000f140: 6d70 6f6e 656e 7473 3a20 556e 696f 6e5b  mponents: Union[
-0000f150: 4e6f 6e65 2c20 696e 745d 0a20 2020 2020  None, int].     
-0000f160: 2020 203a 7061 7261 6d20 6368 756e 6b73     :param chunks
-0000f170: 697a 653a 204e 756d 6265 7220 6f66 2063  ize: Number of c
-0000f180: 6875 6e6b 7320 666f 7220 7768 6963 6820  hunks for which 
-0000f190: 7468 6520 7768 6974 656e 696e 6720 6d75  the whitening mu
-0000f1a0: 7374 2062 6520 636f 6d70 7574 6564 2c0a  st be computed,.
-0000f1b0: 2020 2020 2020 2020 2020 2020 696e 6372              incr
-0000f1c0: 656d 656e 7461 6c6c 792c 2064 6566 6175  ementally, defau
-0000f1d0: 6c74 7320 746f 204e 6f6e 650a 2020 2020  lts to None.    
-0000f1e0: 2020 2020 3a74 7970 6520 6368 756e 6b73      :type chunks
-0000f1f0: 697a 653a 2055 6e69 6f6e 5b4e 6f6e 652c  ize: Union[None,
-0000f200: 2069 6e74 5d2c 206f 7074 696f 6e61 6c0a   int], optional.
-0000f210: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
-0000f220: 756d 5f69 7465 723a 204e 756d 6265 7220  um_iter: Number 
-0000f230: 6f66 2069 7465 7261 7469 6f6e 732c 2064  of iterations, d
-0000f240: 6566 6175 6c74 7320 746f 2035 3030 0a20  efaults to 500. 
-0000f250: 2020 2020 2020 203a 7479 7065 206e 756d         :type num
-0000f260: 5f69 7465 723a 2069 6e74 2c20 6f70 7469  _iter: int, opti
-0000f270: 6f6e 616c 0a20 2020 2020 2020 203a 7061  onal.        :pa
-0000f280: 7261 6d20 6572 726f 725f 7374 6570 3a20  ram error_step: 
-0000f290: 4966 206e 6f74 204e 6f6e 652c 2066 696e  If not None, fin
-0000f2a0: 6420 7468 6520 6572 726f 7220 6576 6572  d the error ever
-0000f2b0: 7920 6572 726f 725f 7374 6570 2061 6e64  y error_step and
-0000f2c0: 2063 6f6d 7061 7265 7320 6974 0a20 2020   compares it.   
-0000f2d0: 2020 2020 2020 2020 2074 6f20 6368 6563           to chec
-0000f2e0: 6b20 666f 7220 636f 6e76 6572 6765 6e63  k for convergenc
-0000f2f0: 652e 2054 4f44 4f3a 206e 6f74 2061 626c  e. TODO: not abl
-0000f300: 6520 666f 7220 6875 6765 2064 6174 6173  e for huge datas
-0000f310: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
-0000f320: 7261 6d20 696e 6469 6365 733a 2049 6620  ram indices: If 
-0000f330: 6e6f 7420 4e6f 6e65 2c20 6170 706c 7920  not None, apply 
-0000f340: 6d65 7468 6f64 206f 6e6c 7920 746f 2069  method only to i
-0000f350: 6e64 6963 6573 206f 6620 6461 7461 2c20  ndices of data, 
-0000f360: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
-0000f370: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-0000f380: 6e64 6963 6573 3a20 556e 696f 6e5b 4e6f  ndices: Union[No
-0000f390: 6e65 2c20 6172 7261 795f 6c69 6b65 5d2c  ne, array_like],
-0000f3a0: 206f 7074 696f 6e61 6c0a 0a20 2020 2020   optional..     
-0000f3b0: 2020 203a 7265 7475 726e 3a20 2848 2c20     :return: (H, 
-0000f3c0: 5729 3a20 5468 6520 636f 6d70 6f6e 656e  W): The componen
-0000f3d0: 7473 206d 6174 7269 7820 616e 6420 7468  ts matrix and th
-0000f3e0: 6520 6d69 7869 6e67 206d 6174 7269 782e  e mixing matrix.
-0000f3f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f400: 2020 2020 2062 7373 5f64 6972 203d 206f       bss_dir = o
-0000f410: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-0000f420: 2e64 6972 2c20 2262 7373 2229 0a20 2020  .dir, "bss").   
-0000f430: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
-0000f440: 2862 7373 5f64 6972 2c20 6578 6973 745f  (bss_dir, exist_
-0000f450: 6f6b 3d54 7275 6529 0a0a 2020 2020 2020  ok=True)..      
-0000f460: 2020 6966 2073 656c 662e 5f69 6e5f 6d65    if self._in_me
-0000f470: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
-0000f480: 2020 6368 756e 6b73 697a 6520 3d20 4e6f    chunksize = No
-0000f490: 6e65 0a20 2020 2020 2020 2077 6974 6820  ne.        with 
-0000f4a0: 7365 6c66 2e64 6174 612e 6f70 656e 5f61  self.data.open_a
-0000f4b0: 735f 6864 6635 2862 7373 5f64 6972 2920  s_hdf5(bss_dir) 
-0000f4c0: 6173 2068 3564 6573 743a 0a20 2020 2020  as h5dest:.     
-0000f4d0: 2020 2020 2020 206d 6f64 656c 203d 204e         model = N
-0000f4e0: 4943 4128 0a20 2020 2020 2020 2020 2020  ICA(.           
-0000f4f0: 2020 2020 2068 3564 6573 742c 0a20 2020       h5dest,.   
-0000f500: 2020 2020 2020 2020 2020 2020 206e 756d               num
-0000f510: 5f63 6f6d 706f 6e65 6e74 732c 0a20 2020  _components,.   
-0000f520: 2020 2020 2020 2020 2020 2020 2063 6875               chu
-0000f530: 6e6b 7369 7a65 2c0a 2020 2020 2020 2020  nksize,.        
-0000f540: 2020 2020 2020 2020 696e 6469 6365 733d          indices=
-0000f550: 696e 6469 6365 732c 0a20 2020 2020 2020  indices,.       
-0000f560: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000f570: 2020 206d 6f64 656c 2e66 6974 5f74 7261     model.fit_tra
-0000f580: 6e73 666f 726d 286d 6178 5f69 7465 723d  nsform(max_iter=
-0000f590: 6e75 6d5f 6974 6572 2c20 6572 726f 725f  num_iter, error_
-0000f5a0: 7374 6570 3d65 7272 6f72 5f73 7465 7029  step=error_step)
-0000f5b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000f5c0: 7572 6e20 6e75 6d70 792e 6162 7328 6d6f  urn numpy.abs(mo
-0000f5d0: 6465 6c2e 4829 2c20 6e75 6d70 792e 6162  del.H), numpy.ab
-0000f5e0: 7328 6d6f 6465 6c2e 5729 0a0a 2020 2020  s(model.W)..    
-0000f5f0: 6465 6620 6e6d 6628 0a20 2020 2020 2020  def nmf(.       
-0000f600: 2073 656c 662c 0a20 2020 2020 2020 206e   self,.        n
-0000f610: 756d 5f63 6f6d 706f 6e65 6e74 732c 0a20  um_components,. 
-0000f620: 2020 2020 2020 206e 756d 5f69 7465 723d         num_iter=
-0000f630: 3130 302c 0a20 2020 2020 2020 2065 7272  100,.        err
-0000f640: 6f72 5f73 7465 703d 4e6f 6e65 2c0a 2020  or_step=None,.  
-0000f650: 2020 2020 2020 7761 7465 7266 616c 6c3d        waterfall=
-0000f660: 4e6f 6e65 2c0a 2020 2020 2020 2020 483d  None,.        H=
-0000f670: 4e6f 6e65 2c0a 2020 2020 2020 2020 573d  None,.        W=
-0000f680: 4e6f 6e65 2c0a 2020 2020 2020 2020 7673  None,.        vs
-0000f690: 7465 703d 3130 302c 0a20 2020 2020 2020  tep=100,.       
-0000f6a0: 2068 7374 6570 3d31 3030 302c 0a20 2020   hstep=1000,.   
-0000f6b0: 2020 2020 2069 6e64 6963 6573 3d4e 6f6e       indices=Non
-0000f6c0: 652c 0a20 2020 2020 2020 2069 6e69 743d  e,.        init=
-0000f6d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000f6e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f6f0: 2043 6f6d 7075 7465 204e 6f6e 2d6e 6567   Compute Non-neg
-0000f700: 6174 6976 6520 4d61 7472 6978 2046 6163  ative Matrix Fac
-0000f710: 746f 7269 7a61 7469 6f6e 206f 6e20 7468  torization on th
-0000f720: 6520 6461 7461 2e0a 2020 2020 2020 2020  e data..        
-0000f730: 5468 6520 6d65 7468 6f64 2c20 6669 7273  The method, firs
-0000f740: 7420 636f 6e76 6572 7473 2c20 6966 206e  t converts, if n
-0000f750: 6f74 2061 6c72 6561 6479 2c20 7468 6520  ot already, the 
-0000f760: 6461 7461 2069 6e74 6f20 616e 2068 6466  data into an hdf
-0000f770: 3520 6669 6c65 206f 626a 6563 740a 2020  5 file object.  
-0000f780: 2020 2020 2020 7769 7468 2074 6865 2069        with the i
-0000f790: 6d61 6765 7320 666c 6174 7465 6e65 6420  mages flattened 
-0000f7a0: 696e 2074 6865 2072 6f77 732e 0a0a 2020  in the rows...  
-0000f7b0: 2020 2020 2020 3a70 6172 616d 206e 756d        :param num
-0000f7c0: 5f63 6f6d 706f 6e65 6e74 733a 204e 756d  _components: Num
-0000f7d0: 6265 7220 6f66 2063 6f6d 706f 6e65 6e74  ber of component
-0000f7e0: 7320 746f 2066 696e 640a 2020 2020 2020  s to find.      
-0000f7f0: 2020 3a74 7970 6520 6e75 6d5f 636f 6d70    :type num_comp
-0000f800: 6f6e 656e 7473 3a20 556e 696f 6e5b 4e6f  onents: Union[No
-0000f810: 6e65 2c20 696e 745d 0a20 2020 2020 2020  ne, int].       
-0000f820: 203a 7061 7261 6d20 6e75 6d5f 6974 6572   :param num_iter
-0000f830: 3a20 4e75 6d62 6572 206f 6620 6974 6572  : Number of iter
-0000f840: 6174 696f 6e73 2c20 6465 6661 756c 7473  ations, defaults
-0000f850: 2074 6f20 3130 300a 2020 2020 2020 2020   to 100.        
-0000f860: 3a74 7970 6520 6e75 6d5f 6974 6572 3a20  :type num_iter: 
-0000f870: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0000f880: 2020 2020 2020 3a70 6172 616d 2065 7272        :param err
-0000f890: 6f72 5f73 7465 703a 2049 6620 6e6f 7420  or_step: If not 
-0000f8a0: 4e6f 6e65 2c20 6669 6e64 2074 6865 2065  None, find the e
-0000f8b0: 7272 6f72 2065 7665 7279 2065 7272 6f72  rror every error
-0000f8c0: 5f73 7465 7020 616e 6420 636f 6d70 6172  _step and compar
-0000f8d0: 6573 2069 740a 2020 2020 2020 2020 2020  es it.          
-0000f8e0: 2020 746f 2063 6865 636b 2066 6f72 2063    to check for c
-0000f8f0: 6f6e 7665 7267 656e 6365 2c20 6465 6661  onvergence, defa
-0000f900: 756c 7473 2074 6f20 4e6f 6e65 0a20 2020  ults to None.   
-0000f910: 2020 2020 2020 2020 2054 4f44 4f3a 206e           TODO: n
-0000f920: 6f74 2061 626c 6520 666f 7220 6875 6765  ot able for huge
-0000f930: 2064 6174 6173 6574 732e 0a20 2020 2020   datasets..     
-0000f940: 2020 203a 7479 7065 2065 7272 6f72 5f73     :type error_s
-0000f950: 7465 703a 2055 6e69 6f6e 5b4e 6f6e 652c  tep: Union[None,
-0000f960: 2069 6e74 5d2c 206f 7074 696f 6e61 6c0a   int], optional.
-0000f970: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
-0000f980: 6174 6572 6661 6c6c 3a20 4966 206e 6f74  aterfall: If not
-0000f990: 204e 6f6e 652c 204e 4d46 2069 7320 636f   None, NMF is co
-0000f9a0: 6d70 7574 6564 2075 7369 6e67 2074 6865  mputed using the
-0000f9b0: 2077 6174 6572 6661 6c6c 206d 6574 686f   waterfall metho
-0000f9c0: 642e 0a20 2020 2020 2020 2020 2020 2054  d..            T
-0000f9d0: 6865 2070 6172 616d 6574 6572 2073 686f  he parameter sho
-0000f9e0: 756c 6420 6265 2061 6e20 6172 7261 7920  uld be an array 
-0000f9f0: 7769 7468 2074 6865 206e 756d 6265 7220  with the number 
-0000fa00: 6f66 2069 7465 7261 7469 6f6e 7320 7065  of iterations pe
-0000fa10: 720a 2020 2020 2020 2020 2020 2020 7375  r.            su
-0000fa20: 622d 636f 6d70 7574 6174 696f 6e2c 2064  b-computation, d
-0000fa30: 6566 6175 6c74 7320 746f 204e 6f6e 650a  efaults to None.
-0000fa40: 2020 2020 2020 2020 3a74 7970 6520 7761          :type wa
-0000fa50: 7465 7266 616c 6c3a 2055 6e69 6f6e 5b4e  terfall: Union[N
-0000fa60: 6f6e 652c 2061 7272 6179 5f6c 696b 655d  one, array_like]
-0000fa70: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000fa80: 2020 203a 7061 7261 6d20 483a 2049 6e69     :param H: Ini
-0000fa90: 7420 6d61 7472 6978 2066 6f72 2048 206f  t matrix for H o
-0000faa0: 6620 7368 6170 6520 286e 5f63 6f6d 706f  f shape (n_compo
-0000fab0: 6e65 6e74 732c 206e 5f73 616d 706c 6573  nents, n_samples
-0000fac0: 292c 2064 6566 6175 6c74 7320 746f 204e  ), defaults to N
-0000fad0: 6f6e 650a 2020 2020 2020 2020 3a74 7970  one.        :typ
-0000fae0: 6520 483a 2055 6e69 6f6e 5b4e 6f6e 652c  e H: Union[None,
-0000faf0: 2061 7272 6179 5f6c 696b 655d 2c20 6f70   array_like], op
-0000fb00: 7469 6f6e 616c 0a20 2020 2020 2020 203a  tional.        :
-0000fb10: 7061 7261 6d20 573a 2049 6e69 7420 6d61  param W: Init ma
-0000fb20: 7472 6978 2066 6f72 2057 206f 6620 7368  trix for W of sh
-0000fb30: 6170 6520 286e 5f66 6561 7475 7265 732c  ape (n_features,
-0000fb40: 206e 5f63 6f6d 706f 6e65 6e74 7329 2c20   n_components), 
-0000fb50: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
-0000fb60: 0a20 2020 2020 2020 203a 7479 7065 2057  .        :type W
-0000fb70: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 6172  : Union[None, ar
-0000fb80: 7261 795f 6c69 6b65 5d2c 206f 7074 696f  ray_like], optio
-0000fb90: 6e61 6c0a 2020 2020 2020 2020 3a70 6172  nal.        :par
-0000fba0: 616d 2069 6e64 6963 6573 3a20 4966 206e  am indices: If n
-0000fbb0: 6f74 204e 6f6e 652c 2061 7070 6c79 206d  ot None, apply m
-0000fbc0: 6574 686f 6420 6f6e 6c79 2074 6f20 696e  ethod only to in
-0000fbd0: 6469 6365 7320 6f66 2064 6174 612c 2064  dices of data, d
-0000fbe0: 6566 6175 6c74 7320 746f 204e 6f6e 650a  efaults to None.
-0000fbf0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-0000fc00: 6469 6365 733a 2055 6e69 6f6e 5b4e 6f6e  dices: Union[Non
-0000fc10: 652c 2061 7272 6179 5f6c 696b 655d 2c20  e, array_like], 
-0000fc20: 6f70 7469 6f6e 616c 0a0a 2020 2020 2020  optional..      
-0000fc30: 2020 3a72 6574 7572 6e3a 2028 482c 2057    :return: (H, W
-0000fc40: 293a 2054 6865 2063 6f6d 706f 6e65 6e74  ): The component
-0000fc50: 7320 6d61 7472 6978 2061 6e64 2074 6865  s matrix and the
-0000fc60: 206d 6978 696e 6720 6d61 7472 6978 2e0a   mixing matrix..
-0000fc70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000fc80: 2020 2020 6273 735f 6469 7220 3d20 6f73      bss_dir = os
-0000fc90: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-0000fca0: 6469 722c 2022 6273 7322 290a 2020 2020  dir, "bss").    
-0000fcb0: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
-0000fcc0: 6273 735f 6469 722c 2065 7869 7374 5f6f  bss_dir, exist_o
-0000fcd0: 6b3d 5472 7565 290a 0a20 2020 2020 2020  k=True)..       
-0000fce0: 2069 6620 7365 6c66 2e5f 696e 5f6d 656d   if self._in_mem
-0000fcf0: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
-0000fd00: 2066 726f 6d20 736b 6c65 6172 6e20 696d   from sklearn im
-0000fd10: 706f 7274 2064 6563 6f6d 706f 7369 7469  port decompositi
-0000fd20: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-0000fd30: 6d6f 6465 6c20 3d20 6465 636f 6d70 6f73  model = decompos
-0000fd40: 6974 696f 6e2e 4e4d 4628 0a20 2020 2020  ition.NMF(.     
-0000fd50: 2020 2020 2020 2020 2020 206e 5f63 6f6d             n_com
-0000fd60: 706f 6e65 6e74 733d 6e75 6d5f 636f 6d70  ponents=num_comp
-0000fd70: 6f6e 656e 7473 2c20 696e 6974 3d69 6e69  onents, init=ini
-0000fd80: 742c 206d 6178 5f69 7465 723d 6e75 6d5f  t, max_iter=num_
-0000fd90: 6974 6572 0a20 2020 2020 2020 2020 2020  iter.           
-0000fda0: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
-0000fdb0: 6974 6820 7365 6c66 2e64 6174 612e 6f70  ith self.data.op
-0000fdc0: 656e 5f61 735f 6864 6635 2862 7373 5f64  en_as_hdf5(bss_d
-0000fdd0: 6972 2920 6173 2068 3564 6573 743a 0a20  ir) as h5dest:. 
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fdf0: 6620 696e 6469 6365 7320 6973 206e 6f74  f indices is not
-0000fe00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000fe10: 2020 2020 2020 2020 2020 2058 203d 2068             X = h
-0000fe20: 3564 6573 745b 696e 6469 6365 735d 0a20  5dest[indices]. 
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000fe40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000fe50: 2020 2020 2020 2020 2058 203d 2068 3564           X = h5d
-0000fe60: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
-0000fe70: 2020 2020 6966 206e 756d 7079 2e61 6e79      if numpy.any
-0000fe80: 2858 5b3a 2c20 3a5d 203c 2030 293a 0a20  (X[:, :] < 0):. 
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 205f 6c6f 6767 6572 2e77 6172 6e69     _logger.warni
-0000feb0: 6e67 2822 5365 7474 696e 6720 6e65 6761  ng("Setting nega
-0000fec0: 7469 7665 2076 616c 7565 7320 746f 2030  tive values to 0
-0000fed0: 2074 6f20 636f 6d70 7574 6520 4e4d 4622   to compute NMF"
-0000fee0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fef0: 2020 2020 2020 585b 585b 3a2c 203a 5d20        X[X[:, :] 
-0000ff00: 3c20 305d 203d 2030 0a20 2020 2020 2020  < 0] = 0.       
-0000ff10: 2020 2020 2020 2020 2069 6620 4820 6973           if H is
-0000ff20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2058                 X
-0000ff40: 203d 2058 2e61 7374 7970 6528 482e 6474   = X.astype(H.dt
-0000ff50: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
-0000ff60: 2020 2020 2065 6c69 6620 5720 6973 206e       elif W is n
-0000ff70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ff80: 2020 2020 2020 2020 2020 2020 2058 203d               X =
-0000ff90: 2058 2e61 7374 7970 6528 572e 6474 7970   X.astype(W.dtyp
-0000ffa0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000ffb0: 2020 2077 6974 6820 7761 726e 696e 6773     with warnings
-0000ffc0: 2e63 6174 6368 5f77 6172 6e69 6e67 7328  .catch_warnings(
-0000ffd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ffe0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-0000fff0: 7369 6d70 6c65 6669 6c74 6572 2822 616c  simplefilter("al
-00010000: 7761 7973 222c 2043 6f6e 7665 7267 656e  ways", Convergen
-00010010: 6365 5761 726e 696e 6729 0a20 2020 2020  ceWarning).     
-00010020: 2020 2020 2020 2020 2020 2020 2020 2057                 W
-00010030: 203d 206d 6f64 656c 2e66 6974 5f74 7261   = model.fit_tra
-00010040: 6e73 666f 726d 2858 2c20 573d 572c 2048  nsform(X, W=W, H
-00010050: 3d48 290a 2020 2020 2020 2020 2020 2020  =H).            
-00010060: 2020 2020 7265 7475 726e 206d 6f64 656c      return model
-00010070: 2e63 6f6d 706f 6e65 6e74 735f 2c20 570a  .components_, W.
-00010080: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010090: 2020 2020 2020 2020 2020 6966 2077 6174            if wat
-000100a0: 6572 6661 6c6c 2069 7320 6e6f 7420 4e6f  erfall is not No
-000100b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000100c0: 2020 2020 482c 2057 203d 2073 656c 662e      H, W = self.
-000100d0: 5f77 6174 6572 6661 6c6c 5f6e 6d66 280a  _waterfall_nmf(.
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 2020 2020 6e75 6d5f 636f 6d70 6f6e 656e      num_componen
-00010100: 7473 2c20 7761 7465 7266 616c 6c2c 2076  ts, waterfall, v
-00010110: 7374 6570 2c20 6873 7465 702c 2069 6e64  step, hstep, ind
-00010120: 6963 6573 3d69 6e64 6963 6573 0a20 2020  ices=indices.   
-00010130: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00010140: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00010150: 2073 656c 662e 6461 7461 2e6f 7065 6e5f   self.data.open_
-00010160: 6173 5f68 6466 3528 6273 735f 6469 7229  as_hdf5(bss_dir)
-00010170: 2061 7320 6835 6465 7374 3a0a 2020 2020   as h5dest:.    
-00010180: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00010190: 6c20 3d20 4e4d 4628 6835 6465 7374 2c20  l = NMF(h5dest, 
-000101a0: 6e75 6d5f 636f 6d70 6f6e 656e 7473 2c20  num_components, 
-000101b0: 696e 6469 6365 733d 696e 6469 6365 7329  indices=indices)
-000101c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101d0: 2077 6974 6820 7761 726e 696e 6773 2e63   with warnings.c
-000101e0: 6174 6368 5f77 6172 6e69 6e67 7328 293a  atch_warnings():
-000101f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010200: 2020 2020 2077 6172 6e69 6e67 732e 7369       warnings.si
-00010210: 6d70 6c65 6669 6c74 6572 2822 616c 7761  mplefilter("alwa
-00010220: 7973 222c 2043 6f6e 7665 7267 656e 6365  ys", Convergence
-00010230: 5761 726e 696e 6729 0a20 2020 2020 2020  Warning).       
-00010240: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00010250: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
-00010260: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010270: 2020 2020 2020 2020 2020 6d61 785f 6974            max_it
-00010280: 6572 3d6e 756d 5f69 7465 722c 0a20 2020  er=num_iter,.   
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 2048 3d48 2c0a 2020 2020 2020       H=H,.      
-000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2020 573d 572c 0a20 2020 2020 2020 2020    W=W,.         
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000102e0: 7374 6570 3d76 7374 6570 2c0a 2020 2020  step=vstep,.    
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 6873 7465 703d 6873 7465 702c      hstep=hstep,
-00010310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010320: 2020 2020 2020 2020 2065 7272 6f72 5f73           error_s
-00010330: 7465 703d 6572 726f 725f 7374 6570 2c0a  tep=error_step,.
-00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010350: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010360: 2020 2020 2020 7265 7475 726e 206d 6f64        return mod
-00010370: 656c 2e48 2c20 6d6f 6465 6c2e 570a 0a20  el.H, model.W.. 
-00010380: 2020 2064 6566 206e 6963 615f 6e6d 6628     def nica_nmf(
-00010390: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000103a0: 2020 2020 2020 206e 756d 5f63 6f6d 706f         num_compo
-000103b0: 6e65 6e74 732c 0a20 2020 2020 2020 2063  nents,.        c
-000103c0: 6875 6e6b 7369 7a65 3d4e 6f6e 652c 0a20  hunksize=None,. 
-000103d0: 2020 2020 2020 206e 756d 5f69 7465 723d         num_iter=
-000103e0: 3530 302c 0a20 2020 2020 2020 2077 6174  500,.        wat
-000103f0: 6572 6661 6c6c 3d4e 6f6e 652c 0a20 2020  erfall=None,.   
-00010400: 2020 2020 2065 7272 6f72 5f73 7465 703d       error_step=
-00010410: 4e6f 6e65 2c0a 2020 2020 2020 2020 7673  None,.        vs
-00010420: 7465 703d 3130 302c 0a20 2020 2020 2020  tep=100,.       
-00010430: 2068 7374 6570 3d31 3030 302c 0a20 2020   hstep=1000,.   
-00010440: 2020 2020 2069 6e64 6963 6573 3d4e 6f6e       indices=Non
-00010450: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00010460: 2020 2222 220a 2020 2020 2020 2020 4170    """.        Ap
-00010470: 706c 6965 7320 626f 7468 204e 4943 4120  plies both NICA 
-00010480: 616e 6420 4e4d 4620 746f 2074 6865 2064  and NMF to the d
-00010490: 6174 612e 2054 6865 2069 6e69 7420 4820  ata. The init H 
-000104a0: 616e 6420 5720 666f 7220 4e4d 4620 6172  and W for NMF ar
-000104b0: 6520 7468 650a 2020 2020 2020 2020 7265  e the.        re
-000104c0: 7375 6c74 206f 6620 4e49 4341 2e0a 2020  sult of NICA..  
-000104d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000104e0: 2020 482c 2057 203d 2073 656c 662e 6e69    H, W = self.ni
-000104f0: 6361 286e 756d 5f63 6f6d 706f 6e65 6e74  ca(num_component
-00010500: 732c 2063 6875 6e6b 7369 7a65 2c20 6e75  s, chunksize, nu
-00010510: 6d5f 6974 6572 2c20 696e 6469 6365 733d  m_iter, indices=
-00010520: 696e 6469 6365 7329 0a0a 2020 2020 2020  indices)..      
-00010530: 2020 2320 496e 6974 6961 6c20 4e4d 4620    # Initial NMF 
-00010540: 6661 6374 6f72 697a 6174 696f 6e3a 2058  factorization: X
-00010550: 203d 2046 3020 2a20 4730 0a20 2020 2020   = F0 * G0.     
-00010560: 2020 2057 203d 206e 756d 7079 2e61 6273     W = numpy.abs
-00010570: 2857 290a 2020 2020 2020 2020 4820 3d20  (W).        H = 
-00010580: 6e75 6d70 792e 6162 7328 4829 0a0a 2020  numpy.abs(H)..  
-00010590: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000105a0: 662e 6e6d 6628 0a20 2020 2020 2020 2020  f.nmf(.         
-000105b0: 2020 206d 696e 286e 756d 5f63 6f6d 706f     min(num_compo
-000105c0: 6e65 6e74 732c 2048 2e73 6861 7065 5b30  nents, H.shape[0
-000105d0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000105e0: 6e75 6d5f 6974 6572 2c0a 2020 2020 2020  num_iter,.      
-000105f0: 2020 2020 2020 6572 726f 725f 7374 6570        error_step
-00010600: 2c0a 2020 2020 2020 2020 2020 2020 7761  ,.            wa
-00010610: 7465 7266 616c 6c2c 0a20 2020 2020 2020  terfall,.       
-00010620: 2020 2020 2048 2c0a 2020 2020 2020 2020       H,.        
-00010630: 2020 2020 572c 0a20 2020 2020 2020 2020      W,.         
-00010640: 2020 2076 7374 6570 2c0a 2020 2020 2020     vstep,.      
-00010650: 2020 2020 2020 6873 7465 702c 0a20 2020        hstep,.   
-00010660: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-00010670: 3d69 6e64 6963 6573 2c0a 2020 2020 2020  =indices,.      
-00010680: 2020 2020 2020 696e 6974 3d22 6375 7374        init="cust
-00010690: 6f6d 222c 0a20 2020 2020 2020 2029 0a0a  om",.        )..
-000106a0: 2020 2020 6465 6620 6170 706c 795f 6d6f      def apply_mo
-000106b0: 6d65 6e74 7328 7365 6c66 2c20 696e 6469  ments(self, indi
-000106c0: 6365 733d 4e6f 6e65 2c20 6368 756e 6b5f  ces=None, chunk_
-000106d0: 7368 6170 653d 5b35 3030 2c20 3530 305d  shape=[500, 500]
-000106e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000106f0: 2020 2020 2020 2043 6f6d 7075 7465 2074         Compute t
-00010700: 6865 2043 4f4d 2c20 4657 484d 2c20 736b  he COM, FWHM, sk
-00010710: 6577 6e65 7373 2061 6e64 206b 7572 746f  ewness and kurto
-00010720: 7369 7320 6f66 2074 6865 2064 6174 6120  sis of the data 
-00010730: 666f 7220 7665 7279 2064 696d 656e 7369  for very dimensi
-00010740: 6f6e 2e0a 0a20 2020 2020 2020 203a 7061  on...        :pa
-00010750: 7261 6d20 696e 6469 6365 733a 2049 6620  ram indices: If 
-00010760: 6e6f 7420 4e6f 6e65 2c20 6170 706c 7920  not None, apply 
-00010770: 6d65 7468 6f64 206f 6e6c 7920 746f 2069  method only to i
-00010780: 6e64 6963 6573 206f 6620 6461 7461 2c20  ndices of data, 
-00010790: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
-000107a0: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-000107b0: 6e64 6963 6573 3a20 556e 696f 6e5b 4e6f  ndices: Union[No
-000107c0: 6e65 2c20 6172 7261 795f 6c69 6b65 5d2c  ne, array_like],
-000107d0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000107e0: 2020 3a70 6172 616d 2063 6875 6e6b 5f73    :param chunk_s
-000107f0: 6861 7065 3a20 5368 6170 6520 6f66 2074  hape: Shape of t
-00010800: 6865 2063 6875 6e6b 2069 6d61 6765 2074  he chunk image t
-00010810: 6f20 7573 6520 7065 7220 6974 6572 6174  o use per iterat
-00010820: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-00010830: 2050 6172 616d 6574 6572 2075 7365 6420   Parameter used 
-00010840: 6f6e 6c79 2077 6865 6e20 666c 6167 2069  only when flag i
-00010850: 6e5f 6d65 6d6f 7279 2069 7320 4661 6c73  n_memory is Fals
-00010860: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-00010870: 2063 6875 6e6b 5f73 6861 7065 3a20 6172   chunk_shape: ar
-00010880: 7261 795f 6c69 6b65 2c20 6f70 7469 6f6e  ray_like, option
-00010890: 616c 0a20 2020 2020 2020 2022 2222 0a0a  al.        """..
-000108a0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000108b0: 656c 662e 6469 6d73 2e6e 6469 6d3a 0a20  elf.dims.ndim:. 
-000108c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000108d0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2073  n None.        s
-000108e0: 656c 662e 7275 6e6e 696e 675f 6461 7461  elf.running_data
-000108f0: 203d 2073 656c 662e 6765 745f 6461 7461   = self.get_data
-00010900: 2869 6e64 6963 6573 290a 2020 2020 2020  (indices).      
-00010910: 2020 6966 2069 6e64 6963 6573 2069 7320    if indices is 
-00010920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010930: 2020 696e 6469 6365 7320 3d20 7261 6e67    indices = rang
-00010940: 6528 7365 6c66 2e6e 6672 616d 6573 290a  e(self.nframes).
-00010950: 2020 2020 2020 2020 666f 7220 6178 6973          for axis
-00010960: 2c20 6469 6d20 696e 2073 656c 662e 6469  , dim in self.di
-00010970: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00010980: 2320 4765 7420 6d6f 746f 7220 7661 6c75  # Get motor valu
-00010990: 6573 2070 6572 2069 6d61 6765 206f 6620  es per image of 
-000109a0: 7468 6520 7374 6163 6b0a 2020 2020 2020  the stack.      
-000109b0: 2020 2020 2020 7661 6c75 6573 203d 2073        values = s
-000109c0: 656c 662e 6765 745f 6469 6d65 6e73 696f  elf.get_dimensio
-000109d0: 6e73 5f76 616c 7565 7328 696e 6469 6365  ns_values(indice
-000109e0: 7329 5b64 696d 2e6e 616d 655d 0a20 2020  s)[dim.name].   
-000109f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010a00: 2e5f 696e 5f6d 656d 6f72 793a 0a20 2020  ._in_memory:.   
-00010a10: 2020 2020 2020 2020 2020 2020 2023 2044               # D
-00010a20: 6174 6120 696e 206d 656d 6f72 790a 2020  ata in memory.  
-00010a30: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00010a40: 6d65 6e74 7320 3d20 6e75 6d70 792e 6173  ments = numpy.as
-00010a50: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
-00010a60: 2020 2020 2020 2020 2020 2063 6f6d 7075             compu
-00010a70: 7465 5f6d 6f6d 656e 7473 2876 616c 7565  te_moments(value
-00010a80: 732c 2073 656c 662e 7275 6e6e 696e 675f  s, self.running_
-00010a90: 6461 7461 292c 2064 7479 7065 3d6e 756d  data), dtype=num
-00010aa0: 7079 2e66 6c6f 6174 3634 0a20 2020 2020  py.float64.     
-00010ab0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00010ac0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010ae0: 2044 6174 6120 6f6e 2064 6973 6b0a 2020   Data on disk.  
-00010af0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00010b00: 6172 7420 3d20 5b30 2c20 305d 0a20 2020  art = [0, 0].   
-00010b10: 2020 2020 2020 2020 2020 2020 2069 6d67               img
-00010b20: 203d 2073 656c 662e 7275 6e6e 696e 675f   = self.running_
-00010b30: 6461 7461 5b30 5d0a 2020 2020 2020 2020  data[0].        
-00010b40: 2020 2020 2020 2020 6d6f 6d65 6e74 7320          moments 
-00010b50: 3d20 6e75 6d70 792e 656d 7074 7928 0a20  = numpy.empty(. 
-00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b70: 2020 2028 342c 2069 6d67 2e73 6861 7065     (4, img.shape
-00010b80: 5b30 5d2c 2069 6d67 2e73 6861 7065 5b31  [0], img.shape[1
-00010b90: 5d29 2c20 6474 7970 653d 6e75 6d70 792e  ]), dtype=numpy.
-00010ba0: 666c 6f61 7436 340a 2020 2020 2020 2020  float64.        
-00010bb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010bc0: 2020 2020 2020 2020 2020 6368 756e 6b73            chunks
-00010bd0: 5f31 203d 2069 6e74 286e 756d 7079 2e63  _1 = int(numpy.c
-00010be0: 6569 6c28 696d 672e 7368 6170 655b 305d  eil(img.shape[0]
-00010bf0: 202f 2063 6875 6e6b 5f73 6861 7065 5b30   / chunk_shape[0
-00010c00: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00010c10: 2020 2020 6368 756e 6b73 5f32 203d 2069      chunks_2 = i
-00010c20: 6e74 286e 756d 7079 2e63 6569 6c28 696d  nt(numpy.ceil(im
-00010c30: 672e 7368 6170 655b 315d 202f 2063 6875  g.shape[1] / chu
-00010c40: 6e6b 5f73 6861 7065 5b31 5d29 290a 2020  nk_shape[1])).  
-00010c50: 2020 2020 2020 2020 2020 2020 2020 696f                io
-00010c60: 5f75 7469 6c73 2e61 6476 616e 6365 6d65  _utils.advanceme
-00010c70: 6e74 5f64 6973 706c 6179 280a 2020 2020  nt_display(.    
-00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c90: 302c 2063 6875 6e6b 735f 3120 2a20 6368  0, chunks_1 * ch
-00010ca0: 756e 6b73 5f32 202a 206c 656e 2873 656c  unks_2 * len(sel
-00010cb0: 662e 7275 6e6e 696e 675f 6461 7461 292c  f.running_data),
-00010cc0: 2022 436f 6d70 7574 696e 6720 6d6f 6d65   "Computing mome
-00010cd0: 6e74 7322 0a20 2020 2020 2020 2020 2020  nts".           
-00010ce0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010cf0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00010d00: 7261 6e67 6528 6368 756e 6b73 5f31 293a  range(chunks_1):
-00010d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d20: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00010d30: 6e67 6528 6368 756e 6b73 5f32 293a 0a20  nge(chunks_2):. 
-00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2020 2020 2020 2063 5f69 6d61 6765 7320         c_images 
-00010d60: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00010d70: 2020 2020 2020 2020 2020 2020 2063 7075               cpu
-00010d80: 7320 3d20 6d75 6c74 6970 726f 6365 7373  s = multiprocess
-00010d90: 696e 672e 6370 755f 636f 756e 7428 290a  ing.cpu_count().
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 2020 2020 2020 2020 7769 7468 2050 6f6f          with Poo
-00010dc0: 6c28 6370 7573 202d 2031 2920 6173 2070  l(cpus - 1) as p
-00010dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010de0: 2020 2020 2020 2020 2020 2020 2020 635f                c_
-00010df0: 696d 6167 6573 203d 2070 2e6d 6170 280a  images = p.map(.
-00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e20: 7061 7274 6961 6c28 6368 756e 6b5f 696d  partial(chunk_im
-00010e30: 6167 652c 2073 7461 7274 2c20 6368 756e  age, start, chun
-00010e40: 6b5f 7368 6170 6529 2c0a 2020 2020 2020  k_shape),.      
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010e70: 756e 6e69 6e67 5f64 6174 612c 0a20 2020  unning_data,.   
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 2020 2069 6f5f 7574 696c 732e 6164 7661     io_utils.adva
-00010ec0: 6e63 656d 656e 745f 6469 7370 6c61 7928  ncement_display(
-00010ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ee0: 2020 2020 2020 2020 2020 2020 2069 202a               i *
-00010ef0: 2063 6875 6e6b 735f 3220 2b20 6a20 2b20   chunks_2 + j + 
-00010f00: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010f20: 6875 6e6b 735f 3120 2a20 6368 756e 6b73  hunks_1 * chunks
-00010f30: 5f32 2c0a 2020 2020 2020 2020 2020 2020  _2,.            
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2243 6f6d 7075 7469 6e67 206d 6f6d 656e  "Computing momen
-00010f60: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-00010f70: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000d310: 2020 2069 6620 696e 6469 6365 7320 6973     if indices is
+0000d320: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 206e 6577 5f75 726c 7320 3d20 6e75     new_urls = nu
+0000d350: 6d70 792e 6172 7261 7928 7365 6c66 2e64  mpy.array(self.d
+0000d360: 6174 612e 7572 6c73 2c20 6474 7970 653d  ata.urls, dtype=
+0000d370: 6f62 6a65 6374 292e 666c 6174 7465 6e28  object).flatten(
+0000d380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d390: 2020 2020 2020 2020 2020 6e75 6d70 792e            numpy.
+0000d3a0: 7075 7428 6e65 775f 7572 6c73 2c20 696e  put(new_urls, in
+0000d3b0: 6469 6365 732c 2075 726c 7329 0a20 2020  dices, urls).   
+0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000d3f0: 6577 5f75 726c 7320 3d20 6e75 6d70 792e  ew_urls = numpy.
+0000d400: 6172 7261 7928 7572 6c73 290a 0a20 2020  array(urls)..   
+0000d410: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d420: 6461 7461 7365 745f 6e61 6d65 203d 3d20  dataset_name == 
+0000d430: 2275 7064 6174 655f 6461 7461 7365 7422  "update_dataset"
+0000d440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d450: 2020 2020 2020 6465 6c20 5f66 696c 655b        del _file[
+0000d460: 2264 6174 6173 6574 225d 0a20 2020 2020  "dataset"].     
+0000d470: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0000d480: 6669 6c65 5b22 6461 7461 7365 7422 5d20  file["dataset"] 
+0000d490: 3d20 5f66 696c 655b 2275 7064 6174 655f  = _file["update_
+0000d4a0: 6461 7461 7365 7422 5d0a 2020 2020 2020  dataset"].      
+0000d4b0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000d4c0: 6c20 5f66 696c 655b 2275 7064 6174 655f  l _file["update_
+0000d4d0: 6461 7461 7365 7422 5d0a 2020 2020 2020  dataset"].      
+0000d4e0: 2020 2020 2020 6669 6e61 6c6c 793a 0a20        finally:. 
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d500: 6620 5f66 696c 6520 6973 206e 6f74 204e  f _file is not N
+0000d510: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d520: 2020 2020 2020 2020 205f 6669 6c65 2e63           _file.c
+0000d530: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+0000d540: 6461 7461 203d 2044 6174 6128 0a20 2020  data = Data(.   
+0000d550: 2020 2020 2020 2020 206e 6577 5f75 726c           new_url
+0000d560: 732e 7265 7368 6170 6528 7365 6c66 2e64  s.reshape(self.d
+0000d570: 6174 612e 7572 6c73 2e73 6861 7065 292c  ata.urls.shape),
+0000d580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d590: 662e 6461 7461 2e6d 6574 6164 6174 612c  f.data.metadata,
+0000d5a0: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
+0000d5b0: 6d65 6d6f 7279 3d73 656c 662e 5f69 6e5f  memory=self._in_
+0000d5c0: 6d65 6d6f 7279 2c0a 2020 2020 2020 2020  memory,.        
+0000d5d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d5e0: 2044 6174 6173 6574 280a 2020 2020 2020   Dataset(.      
+0000d5f0: 2020 2020 2020 5f64 6972 3d5f 6469 722c        _dir=_dir,
+0000d600: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d610: 613d 6461 7461 2c0a 2020 2020 2020 2020  a=data,.        
+0000d620: 2020 2020 6469 6d73 3d73 656c 662e 5f5f      dims=self.__
+0000d630: 6469 6d73 2c0a 2020 2020 2020 2020 2020  dims,.          
+0000d640: 2020 7472 616e 7366 6f72 6d61 7469 6f6e    transformation
+0000d650: 3d73 656c 662e 7472 616e 7366 6f72 6d61  =self.transforma
+0000d660: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0000d670: 2020 696e 5f6d 656d 6f72 793d 7365 6c66    in_memory=self
+0000d680: 2e5f 696e 5f6d 656d 6f72 792c 0a20 2020  ._in_memory,.   
+0000d690: 2020 2020 2020 2020 2074 6974 6c65 3d73           title=s
+0000d6a0: 656c 662e 7469 746c 652c 0a20 2020 2020  elf.title,.     
+0000d6b0: 2020 2029 0a0a 2020 2020 6465 6620 6669     )..    def fi
+0000d6c0: 6e64 5f61 6e64 5f61 7070 6c79 5f73 6869  nd_and_apply_shi
+0000d6d0: 6674 280a 2020 2020 2020 2020 7365 6c66  ft(.        self
+0000d6e0: 2c0a 2020 2020 2020 2020 6469 6d65 6e73  ,.        dimens
+0000d6f0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+0000d700: 2020 7374 6570 733d 3130 302c 0a20 2020    steps=100,.   
+0000d710: 2020 2020 2073 6869 6674 5f61 7070 726f       shift_appro
+0000d720: 6163 683d 2266 6674 222c 0a20 2020 2020  ach="fft",.     
+0000d730: 2020 2069 6e64 6963 6573 3d4e 6f6e 652c     indices=None,
+0000d740: 0a20 2020 2020 2020 2063 616c 6c62 6163  .        callbac
+0000d750: 6b3d 4e6f 6e65 2c0a 2020 2020 293a 0a20  k=None,.    ):. 
+0000d760: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d770: 2020 2046 696e 6420 7468 6520 7368 6966     Find the shif
+0000d780: 7420 6f66 2074 6865 2064 6174 6120 6f72  t of the data or
+0000d790: 2070 6172 7420 6f66 2069 7420 616e 6420   part of it and 
+0000d7a0: 6170 706c 7920 6974 2e0a 0a20 2020 2020  apply it...     
+0000d7b0: 2020 203a 7061 7261 6d20 6469 6d65 6e73     :param dimens
+0000d7c0: 696f 6e3a 2050 6172 616d 6574 6573 2077  ion: Parametes w
+0000d7d0: 6974 6820 7468 6520 706f 7369 7469 6f6e  ith the position
+0000d7e0: 206f 6620 7468 6520 6461 7461 2069 6e20   of the data in 
+0000d7f0: 7468 6520 7265 7368 6170 6564 0a20 2020  the reshaped.   
+0000d800: 2020 2020 2020 2020 2061 7272 6179 2e0a           array..
+0000d810: 2020 2020 2020 2020 3a74 7970 6520 6469          :type di
+0000d820: 6d65 6e73 696f 6e3a 2055 6e69 6f6e 5b4e  mension: Union[N
+0000d830: 6f6e 652c 2074 7570 6c65 2c20 6172 7261  one, tuple, arra
+0000d840: 795f 6c69 6b65 5d0a 2020 2020 2020 2020  y_like].        
+0000d850: 3a70 6172 616d 2066 6c6f 6174 2068 5f6d  :param float h_m
+0000d860: 6178 3a20 5365 6520 6063 6f72 652e 696d  ax: See `core.im
+0000d870: 6167 6552 6567 6973 7472 6174 696f 6e2e  ageRegistration.
+0000d880: 7368 6966 745f 6465 7465 6374 696f 6e60  shift_detection`
+0000d890: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000d8a0: 666c 6f61 7420 685f 7374 6570 3a20 5365  float h_step: Se
+0000d8b0: 6520 6063 6f72 652e 696d 6167 6552 6567  e `core.imageReg
+0000d8c0: 6973 7472 6174 696f 6e2e 7368 6966 745f  istration.shift_
+0000d8d0: 6465 7465 6374 696f 6e60 0a20 2020 2020  detection`.     
+0000d8e0: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
+0000d8f0: 2766 6674 272c 2027 6c69 6e65 6172 275d  'fft', 'linear']
+0000d900: 2073 6869 6674 5f61 7070 726f 6163 683a   shift_approach:
+0000d910: 204d 6574 686f 6420 746f 2075 7365 2074   Method to use t
+0000d920: 6f20 6170 706c 7920 7468 6520 7368 6966  o apply the shif
+0000d930: 742e 0a20 2020 2020 2020 203a 7061 7261  t..        :para
+0000d940: 6d20 696e 6469 6365 733a 2049 6e64 6963  m indices: Indic
+0000d950: 6573 206f 6620 7468 6520 696d 6167 6573  es of the images
+0000d960: 2074 6f20 6669 6e64 2061 6e64 2061 7070   to find and app
+0000d970: 6c79 2074 6865 2073 6869 6674 2074 6f2e  ly the shift to.
+0000d980: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+0000d990: 4e6f 6e65 2c20 7468 6520 686f 7420 7069  None, the hot pi
+0000d9a0: 7865 6c20 7265 6d6f 7661 6c20 6973 2061  xel removal is a
+0000d9b0: 7070 6c69 6564 2074 6f20 616c 6c20 7468  pplied to all th
+0000d9c0: 6520 6461 7461 2e0a 2020 2020 2020 2020  e data..        
+0000d9d0: 3a74 7970 6520 696e 6469 6365 733a 2055  :type indices: U
+0000d9e0: 6e69 6f6e 5b4e 6f6e 652c 2061 7272 6179  nion[None, array
+0000d9f0: 5f6c 696b 655d 0a20 2020 2020 2020 203a  _like].        :
+0000da00: 7061 7261 6d20 556e 696f 6e5b 6675 6e63  param Union[func
+0000da10: 7469 6f6e 2c20 4e6f 6e65 5d20 6361 6c6c  tion, None] call
+0000da20: 6261 636b 3a20 4361 6c6c 6261 636b 0a20  back: Callback. 
+0000da30: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
+0000da40: 2044 6174 6173 6574 2077 6974 6820 7468   Dataset with th
+0000da50: 6520 6e65 7720 6461 7461 2e0a 2020 2020  e new data..    
+0000da60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000da70: 7368 6966 7420 3d20 7365 6c66 2e66 696e  shift = self.fin
+0000da80: 645f 7368 6966 7428 6469 6d65 6e73 696f  d_shift(dimensio
+0000da90: 6e2c 2073 7465 7073 2c20 696e 6469 6365  n, steps, indice
+0000daa0: 733d 696e 6469 6365 7329 0a20 2020 2020  s=indices).     
+0000dab0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+0000dac0: 7070 6c79 5f73 6869 6674 2873 6869 6674  pply_shift(shift
+0000dad0: 2c20 6469 6d65 6e73 696f 6e2c 2069 6e64  , dimension, ind
+0000dae0: 6963 6573 3d69 6e64 6963 6573 290a 0a20  ices=indices).. 
+0000daf0: 2020 2064 6566 205f 7761 7465 7266 616c     def _waterfal
+0000db00: 6c5f 6e6d 6628 0a20 2020 2020 2020 2073  l_nmf(.        s
+0000db10: 656c 662c 206e 756d 5f63 6f6d 706f 6e65  elf, num_compone
+0000db20: 6e74 732c 2069 7465 7261 7469 6f6e 732c  nts, iterations,
+0000db30: 2076 7374 6570 3d4e 6f6e 652c 2068 7374   vstep=None, hst
+0000db40: 6570 3d4e 6f6e 652c 2069 6e64 6963 6573  ep=None, indices
+0000db50: 3d4e 6f6e 650a 2020 2020 293a 0a20 2020  =None.    ):.   
+0000db60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000db70: 2054 6869 7320 6d65 7468 6f64 2069 7320   This method is 
+0000db80: 7573 6564 2061 7320 6120 7761 7920 746f  used as a way to
+0000db90: 2069 6d70 726f 7665 2074 6865 2073 7065   improve the spe
+0000dba0: 6564 206f 6620 636f 6e76 6572 6765 6e63  ed of convergenc
+0000dbb0: 6520 6f66 0a20 2020 2020 2020 2074 6865  e of.        the
+0000dbc0: 204e 4d46 206d 6574 686f 642e 2046 6f72   NMF method. For
+0000dbd0: 2074 6869 732c 2069 7420 7573 6573 2061   this, it uses a
+0000dbe0: 2077 6174 6572 6661 6c6c 206d 6f64 656c   waterfall model
+0000dbf0: 2077 6865 7265 2061 7420 6576 6572 7920   where at every 
+0000dc00: 7374 6570 0a20 2020 2020 2020 2074 6865  step.        the
+0000dc10: 206f 7574 7075 7420 6d61 7472 6963 6573   output matrices
+0000dc20: 2073 6572 7665 2061 7320 696e 7075 7420   serve as input 
+0000dc30: 666f 7220 7468 6520 6e65 7874 2e0a 2020  for the next..  
+0000dc40: 2020 2020 2020 5468 6174 2069 732c 2074        That is, t
+0000dc50: 6865 206d 6574 686f 6420 7374 6172 7473  he method starts
+0000dc60: 2077 6974 6820 6120 736d 616c 6c65 7220   with a smaller 
+0000dc70: 7265 7369 7a65 6420 696d 6167 6573 206f  resized images o
+0000dc80: 6620 7468 6520 6461 7461 2c0a 2020 2020  f the data,.    
+0000dc90: 2020 2020 616e 6420 636f 6d70 7574 6573      and computes
+0000dca0: 2074 6865 204e 4d46 2064 6563 6f6d 706f   the NMF decompo
+0000dcb0: 7369 7469 6f6e 2e20 5468 6520 6e65 7874  sition. The next
+0000dcc0: 2073 7465 7020 6973 2074 6865 2073 616d   step is the sam
+0000dcd0: 6520 6275 7420 7769 7468 0a20 2020 2020  e but with.     
+0000dce0: 2020 2062 6967 6765 7220 696d 6167 6573     bigger images
+0000dcf0: 2c20 616e 6420 7573 696e 6720 6173 2069  , and using as i
+0000dd00: 6e69 7469 616c 2048 2061 6e64 2057 2074  nitial H and W t
+0000dd10: 6865 2070 7265 636f 6d70 7574 6564 206d  he precomputed m
+0000dd20: 6174 7269 6365 732e 0a20 2020 2020 2020  atrices..       
+0000dd30: 2054 6865 206c 6173 7420 7374 6570 2069   The last step i
+0000dd40: 7320 646f 6e65 2075 7369 6e67 2074 6865  s done using the
+0000dd50: 2061 6374 7561 6c20 7369 7a65 206f 6620   actual size of 
+0000dd60: 7468 6520 696d 6167 6573 2e0a 2020 2020  the images..    
+0000dd70: 2020 2020 5468 6973 2077 6179 2c20 7468      This way, th
+0000dd80: 6520 6e75 6d62 6572 206f 6620 6974 6572  e number of iter
+0000dd90: 6174 696f 6e73 2077 6974 6820 6269 6720  ations with big 
+0000dda0: 696d 6167 6573 2063 616e 2062 6520 6469  images can be di
+0000ddb0: 6d69 6e69 7368 6564 2c20 616e 640a 2020  minished, and.  
+0000ddc0: 2020 2020 2020 7468 6520 6d65 7468 6f64        the method
+0000ddd0: 2063 6f6e 7665 7267 6573 2066 6173 7465   converges faste
+0000dde0: 722e 0a0a 2020 2020 2020 2020 3a70 6172  r...        :par
+0000ddf0: 616d 2069 6e74 206e 756d 5f63 6f6d 706f  am int num_compo
+0000de00: 6e65 6e74 733a 204e 756d 6265 7220 6f66  nents: Number of
+0000de10: 2063 6f6d 706f 6e65 6e74 7320 746f 2066   components to f
+0000de20: 696e 642e 0a20 2020 2020 2020 203a 7061  ind..        :pa
+0000de30: 7261 6d20 6172 7261 795f 6c69 6b65 2069  ram array_like i
+0000de40: 7465 7261 7469 6f6e 733a 2041 7272 6179  terations: Array
+0000de50: 2077 6974 6820 6e75 6d62 6572 206f 6620   with number of 
+0000de60: 6974 6572 6174 696f 6e73 2070 6572 2073  iterations per s
+0000de70: 7465 7020 6f66 2074 6865 2077 6174 6572  tep of the water
+0000de80: 6661 6c6c 2e0a 2020 2020 2020 2020 2020  fall..          
+0000de90: 2020 5468 6520 7369 7a65 206f 6620 7468    The size of th
+0000dea0: 6520 6172 7261 7920 7365 7473 2074 6865  e array sets the
+0000deb0: 2073 697a 6520 6f66 2074 6865 2077 6174   size of the wat
+0000dec0: 6572 6661 6c6c 2e0a 2020 2020 2020 2020  erfall..        
+0000ded0: 3a70 6172 616d 2055 6e69 6f6e 5b4e 6f6e  :param Union[Non
+0000dee0: 652c 2061 7272 6179 5f6c 696b 655d 2069  e, array_like] i
+0000def0: 6e64 6963 6573 3a20 4966 206e 6f74 204e  ndices: If not N
+0000df00: 6f6e 652c 2061 7070 6c79 206d 6574 686f  one, apply metho
+0000df10: 6420 6f6e 6c79 2074 6f20 696e 6469 6365  d only to indice
+0000df20: 7320 6f66 2064 6174 612e 0a20 2020 2020  s of data..     
+0000df30: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000df40: 6672 6f6d 2073 6b69 6d61 6765 2e74 7261  from skimage.tra
+0000df50: 6e73 666f 726d 2069 6d70 6f72 7420 7265  nsform import re
+0000df60: 7369 7a65 0a20 2020 2020 2020 2069 6d70  size.        imp
+0000df70: 6f72 7420 7368 7574 696c 0a0a 2020 2020  ort shutil..    
+0000df80: 2020 2020 5720 3d20 4e6f 6e65 0a20 2020      W = None.   
+0000df90: 2020 2020 2048 203d 204e 6f6e 650a 2020       H = None.  
+0000dfa0: 2020 2020 2020 7368 6170 6520 3d20 6e75        shape = nu
+0000dfb0: 6d70 792e 6173 6172 7261 7928 7365 6c66  mpy.asarray(self
+0000dfc0: 2e67 6574 5f64 6174 6128 3029 2e73 6861  .get_data(0).sha
+0000dfd0: 7065 290a 2020 2020 2020 2020 6669 7273  pe).        firs
+0000dfe0: 745f 7369 7a65 203d 2028 7368 6170 6520  t_size = (shape 
+0000dff0: 2f20 286c 656e 2869 7465 7261 7469 6f6e  / (len(iteration
+0000e000: 7329 202b 2031 2929 2e61 7374 7970 6528  s) + 1)).astype(
+0000e010: 696e 7429 0a20 2020 2020 2020 2073 697a  int).        siz
+0000e020: 6520 3d20 6669 7273 745f 7369 7a65 0a0a  e = first_size..
+0000e030: 2020 2020 2020 2020 6f73 2e6d 616b 6564          os.maked
+0000e040: 6972 7328 6f73 2e70 6174 682e 6a6f 696e  irs(os.path.join
+0000e050: 2873 656c 662e 6469 722c 2022 7761 7465  (self.dir, "wate
+0000e060: 7266 616c 6c22 292c 2065 7869 7374 5f6f  rfall"), exist_o
+0000e070: 6b3d 5472 7565 290a 0a20 2020 2020 2020  k=True)..       
+0000e080: 205f 6c6f 6767 6572 2e69 6e66 6f28 2253   _logger.info("S
+0000e090: 7461 7274 696e 6720 7761 7465 7266 616c  tarting waterfal
+0000e0a0: 6c20 4e4d 4622 290a 0a20 2020 2020 2020  l NMF")..       
+0000e0b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0000e0c0: 6c65 6e28 6974 6572 6174 696f 6e73 2929  len(iterations))
+0000e0d0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+0000e0e0: 775f 7572 6c73 203d 205b 5d0a 2020 2020  w_urls = [].    
+0000e0f0: 2020 2020 2020 2020 6966 2069 6e64 6963          if indic
+0000e100: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+0000e110: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+0000e120: 6365 7320 3d20 7261 6e67 6528 7365 6c66  ces = range(self
+0000e130: 2e6e 6672 616d 6573 290a 2020 2020 2020  .nframes).      
+0000e140: 2020 2020 2020 666f 7220 6a20 696e 2069        for j in i
+0000e150: 6e64 6963 6573 3a0a 2020 2020 2020 2020  ndices:.        
+0000e160: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+0000e170: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000e180: 7365 6c66 2e64 6972 2c20 2277 6174 6572  self.dir, "water
+0000e190: 6661 6c6c 222c 2073 7472 286a 2920 2b20  fall", str(j) + 
+0000e1a0: 222e 6e70 7922 290a 2020 2020 2020 2020  ".npy").        
+0000e1b0: 2020 2020 2020 2020 6e75 6d70 792e 7361          numpy.sa
+0000e1c0: 7665 2866 696c 656e 616d 652c 2072 6573  ve(filename, res
+0000e1d0: 697a 6528 7365 6c66 2e67 6574 5f64 6174  ize(self.get_dat
+0000e1e0: 6128 6a29 2c20 7369 7a65 2929 0a20 2020  a(j), size)).   
+0000e1f0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000e200: 5f75 726c 732e 6170 7065 6e64 2844 6174  _urls.append(Dat
+0000e210: 6155 726c 2866 696c 655f 7061 7468 3d66  aUrl(file_path=f
+0000e220: 696c 656e 616d 652c 2073 6368 656d 653d  ilename, scheme=
+0000e230: 2266 6162 696f 2229 290a 2020 2020 2020  "fabio")).      
+0000e240: 2020 2020 2020 6461 7461 203d 2044 6174        data = Dat
+0000e250: 6128 6e65 775f 7572 6c73 2c20 7365 6c66  a(new_urls, self
+0000e260: 2e67 6574 5f64 6174 6128 696e 6469 6365  .get_data(indice
+0000e270: 7329 2e6d 6574 6164 6174 612c 2073 656c  s).metadata, sel
+0000e280: 662e 5f69 6e5f 6d65 6d6f 7279 290a 2020  f._in_memory).  
+0000e290: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+0000e2a0: 7420 3d20 4461 7461 7365 7428 0a20 2020  t = Dataset(.   
+0000e2b0: 2020 2020 2020 2020 2020 2020 205f 6469               _di
+0000e2c0: 723d 6f73 2e70 6174 682e 6a6f 696e 2873  r=os.path.join(s
+0000e2d0: 656c 662e 6469 722c 2022 7761 7465 7266  elf.dir, "waterf
+0000e2e0: 616c 6c22 292c 0a20 2020 2020 2020 2020  all"),.         
+0000e2f0: 2020 2020 2020 2064 6174 613d 6461 7461         data=data
+0000e300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e310: 2020 696e 5f6d 656d 6f72 793d 7365 6c66    in_memory=self
+0000e320: 2e5f 696e 5f6d 656d 6f72 792c 0a20 2020  ._in_memory,.   
+0000e330: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000e340: 2020 2020 2020 2069 6620 7673 7465 703a         if vstep:
+0000e350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e360: 2076 5f73 7465 7020 3d20 7673 7465 7020   v_step = vstep 
+0000e370: 2a20 286c 656e 2869 7465 7261 7469 6f6e  * (len(iteration
+0000e380: 7329 202d 2069 290a 2020 2020 2020 2020  s) - i).        
+0000e390: 2020 2020 6966 2068 7374 6570 3a0a 2020      if hstep:.  
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 685f                h_
+0000e3b0: 7374 6570 203d 2068 7374 6570 202a 2028  step = hstep * (
+0000e3c0: 6c65 6e28 6974 6572 6174 696f 6e73 2920  len(iterations) 
+0000e3d0: 2d20 6929 0a20 2020 2020 2020 2020 2020  - i).           
+0000e3e0: 2048 2c20 5720 3d20 6461 7461 7365 742e   H, W = dataset.
+0000e3f0: 6e6d 6628 0a20 2020 2020 2020 2020 2020  nmf(.           
+0000e400: 2020 2020 206e 756d 5f63 6f6d 706f 6e65       num_compone
+0000e410: 6e74 732c 2069 7465 7261 7469 6f6e 735b  nts, iterations[
+0000e420: 695d 2c20 573d 572c 2048 3d48 2c20 7673  i], W=W, H=H, vs
+0000e430: 7465 703d 765f 7374 6570 2c20 6873 7465  tep=v_step, hste
+0000e440: 703d 685f 7374 6570 0a20 2020 2020 2020  p=h_step.       
+0000e450: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000e460: 2020 2073 697a 6520 3d20 6669 7273 745f     size = first_
+0000e470: 7369 7a65 202a 2028 6920 2b20 3229 0a20  size * (i + 2). 
+0000e480: 2020 2020 2020 2020 2020 2048 3220 3d20             H2 = 
+0000e490: 6e75 6d70 792e 656d 7074 7928 2848 2e73  numpy.empty((H.s
+0000e4a0: 6861 7065 5b30 5d2c 2073 697a 655b 305d  hape[0], size[0]
+0000e4b0: 202a 2073 697a 655b 315d 2929 0a20 2020   * size[1])).   
+0000e4c0: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
+0000e4d0: 2069 6e20 7261 6e67 6528 482e 7368 6170   in range(H.shap
+0000e4e0: 655b 305d 293a 0a20 2020 2020 2020 2020  e[0]):.         
+0000e4f0: 2020 2020 2020 2048 325b 726f 775d 203d         H2[row] =
+0000e500: 2072 6573 697a 6528 485b 726f 775d 2e72   resize(H[row].r
+0000e510: 6573 6861 7065 2828 6920 2b20 3129 202a  eshape((i + 1) *
+0000e520: 2066 6972 7374 5f73 697a 6529 2c20 7369   first_size), si
+0000e530: 7a65 292e 666c 6174 7465 6e28 290a 2020  ze).flatten().  
+0000e540: 2020 2020 2020 2020 2020 4820 3d20 4832            H = H2
+0000e550: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
+0000e560: 2020 2020 2020 2020 2020 2073 6875 7469             shuti
+0000e570: 6c2e 726d 7472 6565 286f 732e 7061 7468  l.rmtree(os.path
+0000e580: 2e6a 6f69 6e28 7365 6c66 2e64 6972 2c20  .join(self.dir, 
+0000e590: 2277 6174 6572 6661 6c6c 2229 290a 2020  "waterfall")).  
+0000e5a0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0000e5b0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0000e5c0: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2246 6169 6c65 6420 746f 2064 656c 6574  "Failed to delet
+0000e5f0: 6520 2573 2e20 5265 6173 6f6e 3a20 2573  e %s. Reason: %s
+0000e600: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000e610: 2020 2520 286f 732e 7061 7468 2e6a 6f69    % (os.path.joi
+0000e620: 6e28 7365 6c66 2e64 6972 2c20 2277 6174  n(self.dir, "wat
+0000e630: 6572 6661 6c6c 2229 2c20 6529 0a20 2020  erfall"), e).   
+0000e640: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000e650: 2020 2020 4820 3d20 7265 7369 7a65 2848      H = resize(H
+0000e660: 2c20 286e 756d 5f63 6f6d 706f 6e65 6e74  , (num_component
+0000e670: 732c 2073 6861 7065 5b30 5d20 2a20 7368  s, shape[0] * sh
+0000e680: 6170 655b 315d 2929 0a0a 2020 2020 2020  ape[1]))..      
+0000e690: 2020 7265 7475 726e 2048 2c20 570a 0a20    return H, W.. 
+0000e6a0: 2020 2064 6566 2070 6361 2873 656c 662c     def pca(self,
+0000e6b0: 206e 756d 5f63 6f6d 706f 6e65 6e74 733d   num_components=
+0000e6c0: 4e6f 6e65 2c20 6368 756e 6b5f 7369 7a65  None, chunk_size
+0000e6d0: 3d35 3030 2c20 696e 6469 6365 733d 4e6f  =500, indices=No
+0000e6e0: 6e65 2c20 7265 7475 726e 5f76 616c 733d  ne, return_vals=
+0000e6f0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+0000e700: 2222 220a 2020 2020 2020 2020 436f 6d70  """.        Comp
+0000e710: 7574 6520 5072 696e 6369 7061 6c20 436f  ute Principal Co
+0000e720: 6d70 6f6e 656e 7420 416e 616c 7973 6973  mponent Analysis
+0000e730: 206f 6e20 7468 6520 6461 7461 2e0a 2020   on the data..  
+0000e740: 2020 2020 2020 5468 6520 6d65 7468 6f64        The method
+0000e750: 2c20 6669 7273 7420 636f 6e76 6572 7473  , first converts
+0000e760: 2c20 6966 206e 6f74 2061 6c72 6561 6479  , if not already
+0000e770: 2c20 7468 6520 6461 7461 2069 6e74 6f20  , the data into 
+0000e780: 616e 2068 6466 3520 6669 6c65 206f 626a  an hdf5 file obj
+0000e790: 6563 740a 2020 2020 2020 2020 7769 7468  ect.        with
+0000e7a0: 2074 6865 2069 6d61 6765 7320 666c 6174   the images flat
+0000e7b0: 7465 6e65 6420 696e 2074 6865 2072 6f77  tened in the row
+0000e7c0: 732e 0a0a 2020 2020 2020 2020 3a70 6172  s...        :par
+0000e7d0: 616d 206e 756d 5f63 6f6d 706f 6e65 6e74  am num_component
+0000e7e0: 733a 204e 756d 6265 7220 6f66 2063 6f6d  s: Number of com
+0000e7f0: 706f 6e65 6e74 7320 746f 2066 696e 642e  ponents to find.
+0000e800: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+0000e810: 4e6f 6e65 2c20 6974 2075 7365 7320 7468  None, it uses th
+0000e820: 6520 6d69 6e69 6d75 6d20 6265 7477 6565  e minimum betwee
+0000e830: 6e20 7468 6520 6e75 6d62 6572 206f 6620  n the number of 
+0000e840: 696d 6167 6573 2061 6e64 2074 6865 0a20  images and the. 
+0000e850: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+0000e860: 7220 6f66 2070 6978 656c 732e 0a20 2020  r of pixels..   
+0000e870: 2020 2020 203a 7479 7065 206e 756d 5f63       :type num_c
+0000e880: 6f6d 706f 6e65 6e74 733a 2055 6e69 6f6e  omponents: Union
+0000e890: 5b4e 6f6e 652c 2069 6e74 5d0a 2020 2020  [None, int].    
+0000e8a0: 2020 2020 3a70 6172 616d 2063 6875 6e6b      :param chunk
+0000e8b0: 5f73 697a 653a 204e 756d 6265 7220 6f66  _size: Number of
+0000e8c0: 2063 6875 6e6b 7320 666f 7220 7768 6963   chunks for whic
+0000e8d0: 6820 7468 6520 7768 6974 656e 696e 6720  h the whitening 
+0000e8e0: 6d75 7374 2062 6520 636f 6d70 7574 6564  must be computed
+0000e8f0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+0000e900: 6372 656d 656e 7461 6c6c 792c 2064 6566  crementally, def
+0000e910: 6175 6c74 7320 746f 204e 6f6e 650a 2020  aults to None.  
+0000e920: 2020 2020 2020 3a74 7970 6520 6368 756e        :type chun
+0000e930: 6b73 697a 653a 2055 6e69 6f6e 5b4e 6f6e  ksize: Union[Non
+0000e940: 652c 2069 6e74 5d2c 206f 7074 696f 6e61  e, int], optiona
+0000e950: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
+0000e960: 2069 6e64 6963 6573 3a20 4966 206e 6f74   indices: If not
+0000e970: 204e 6f6e 652c 2061 7070 6c79 206d 6574   None, apply met
+0000e980: 686f 6420 6f6e 6c79 2074 6f20 696e 6469  hod only to indi
+0000e990: 6365 7320 6f66 2064 6174 612c 2064 6566  ces of data, def
+0000e9a0: 6175 6c74 7320 746f 204e 6f6e 650a 2020  aults to None.  
+0000e9b0: 2020 2020 2020 3a74 7970 6520 696e 6469        :type indi
+0000e9c0: 6365 733a 2055 6e69 6f6e 5b4e 6f6e 652c  ces: Union[None,
+0000e9d0: 2061 7272 6179 5f6c 696b 655d 2c20 6f70   array_like], op
+0000e9e0: 7469 6f6e 616c 0a20 2020 2020 2020 203a  tional.        :
+0000e9f0: 7061 7261 6d20 7265 7475 726e 5f76 616c  param return_val
+0000ea00: 733a 2049 6620 5472 7565 2c20 7265 7475  s: If True, retu
+0000ea10: 726e 7320 6f6e 6c79 2074 6865 2073 696e  rns only the sin
+0000ea20: 6775 6c61 7220 7661 6c75 6573 206f 6620  gular values of 
+0000ea30: 5043 412c 2065 6c73 6520 7265 7475 726e  PCA, else return
+0000ea40: 730a 2020 2020 2020 2020 2020 2020 7468  s.            th
+0000ea50: 6520 636f 6d70 6f6e 656e 7473 2061 6e64  e components and
+0000ea60: 2074 6865 206d 6978 696e 6720 6d61 7472   the mixing matr
+0000ea70: 6978 2c20 6465 6661 756c 7473 2074 6f20  ix, defaults to 
+0000ea80: 4661 6c73 650a 2020 2020 2020 2020 3a74  False.        :t
+0000ea90: 7970 6520 7265 7475 726e 5f76 616c 733a  ype return_vals:
+0000eaa0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+0000eab0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000eac0: 3a20 2848 2c20 5729 3a20 5468 6520 636f  : (H, W): The co
+0000ead0: 6d70 6f6e 656e 7473 206d 6174 7269 7820  mponents matrix 
+0000eae0: 616e 6420 7468 6520 6d69 7869 6e67 206d  and the mixing m
+0000eaf0: 6174 7269 782e 0a20 2020 2020 2020 2022  atrix..        "
+0000eb00: 2222 0a20 2020 2020 2020 2062 7373 5f64  "".        bss_d
+0000eb10: 6972 203d 206f 732e 7061 7468 2e6a 6f69  ir = os.path.joi
+0000eb20: 6e28 7365 6c66 2e64 6972 2c20 2262 7373  n(self.dir, "bss
+0000eb30: 2229 0a20 2020 2020 2020 206f 732e 6d61  ").        os.ma
+0000eb40: 6b65 6469 7273 2862 7373 5f64 6972 2c20  kedirs(bss_dir, 
+0000eb50: 6578 6973 745f 6f6b 3d54 7275 6529 0a20  exist_ok=True). 
+0000eb60: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000eb70: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
+0000eb80: 2020 2020 2020 2066 726f 6d20 736b 6c65         from skle
+0000eb90: 6172 6e20 696d 706f 7274 2064 6563 6f6d  arn import decom
+0000eba0: 706f 7369 7469 6f6e 0a0a 2020 2020 2020  position..      
+0000ebb0: 2020 2020 2020 6d6f 6465 6c20 3d20 6465        model = de
+0000ebc0: 636f 6d70 6f73 6974 696f 6e2e 5043 4128  composition.PCA(
+0000ebd0: 6e5f 636f 6d70 6f6e 656e 7473 3d6e 756d  n_components=num
+0000ebe0: 5f63 6f6d 706f 6e65 6e74 7329 0a0a 2020  _components)..  
+0000ebf0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000ec00: 656c 662e 6461 7461 2e6f 7065 6e5f 6173  elf.data.open_as
+0000ec10: 5f68 6466 3528 6273 735f 6469 7229 2061  _hdf5(bss_dir) a
+0000ec20: 7320 6835 6473 6574 3a0a 2020 2020 2020  s h5dset:.      
+0000ec30: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
+0000ec40: 6963 6573 2069 7320 6e6f 7420 4e6f 6e65  ices is not None
+0000ec50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ec60: 2020 2020 2020 5720 3d20 6d6f 6465 6c2e        W = model.
+0000ec70: 6669 745f 7472 616e 7366 6f72 6d28 6835  fit_transform(h5
+0000ec80: 6473 6574 5b69 6e64 6963 6573 5d29 0a20  dset[indices]). 
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000eca0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ecb0: 2020 2020 2020 2020 2057 203d 206d 6f64           W = mod
+0000ecc0: 656c 2e66 6974 5f74 7261 6e73 666f 726d  el.fit_transform
+0000ecd0: 2868 3564 7365 745b 3a2c 203a 5d29 0a0a  (h5dset[:, :])..
+0000ece0: 2020 2020 2020 2020 2020 2020 482c 2076              H, v
+0000ecf0: 616c 732c 2057 203d 206d 6f64 656c 2e63  als, W = model.c
+0000ed00: 6f6d 706f 6e65 6e74 735f 2c20 6d6f 6465  omponents_, mode
+0000ed10: 6c2e 7369 6e67 756c 6172 5f76 616c 7565  l.singular_value
+0000ed20: 735f 2c20 570a 2020 2020 2020 2020 656c  s_, W.        el
+0000ed30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000ed40: 7769 7468 2073 656c 662e 6461 7461 2e6f  with self.data.o
+0000ed50: 7065 6e5f 6173 5f68 6466 3528 6273 735f  pen_as_hdf5(bss_
+0000ed60: 6469 7229 2061 7320 6835 6473 6574 3a0a  dir) as h5dset:.
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed80: 6d6f 6465 6c20 3d20 4950 4341 280a 2020  model = IPCA(.  
+0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eda0: 2020 6835 6473 6574 2c0a 2020 2020 2020    h5dset,.      
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+0000edc0: 756e 6b5f 7369 7a65 2c0a 2020 2020 2020  unk_size,.      
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+0000ede0: 6d5f 636f 6d70 6f6e 656e 7473 2c0a 2020  m_components,.  
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 696e 6469 6365 733d 696e 6469 6365    indices=indice
+0000ee10: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000ee20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000ee30: 2020 2020 2077 6974 6820 6835 7079 2e46       with h5py.F
+0000ee40: 696c 6528 6f73 2e70 6174 682e 6a6f 696e  ile(os.path.join
+0000ee50: 2862 7373 5f64 6972 2c20 2269 7063 612e  (bss_dir, "ipca.
+0000ee60: 6864 6635 2229 2c20 2277 2229 2061 7320  hdf5"), "w") as 
+0000ee70: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+0000ee80: 2020 2020 2020 2020 2020 6669 6c65 5b22            file["
+0000ee90: 5722 5d20 3d20 6e75 6d70 792e 7261 6e64  W"] = numpy.rand
+0000eea0: 6f6d 2e72 616e 646f 6d28 0a20 2020 2020  om.random(.     
+0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eec0: 2020 2028 6d6f 6465 6c2e 6e75 6d5f 7361     (model.num_sa
+0000eed0: 6d70 6c65 732c 206d 6f64 656c 2e6e 756d  mples, model.num
+0000eee0: 5f63 6f6d 706f 6e65 6e74 7329 0a20 2020  _components).   
+0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef00: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000ef10: 2020 2020 2020 2066 696c 655b 2248 225d         file["H"]
+0000ef20: 203d 206e 756d 7079 2e72 616e 646f 6d2e   = numpy.random.
+0000ef30: 7261 6e64 6f6d 280a 2020 2020 2020 2020  random(.        
+0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef50: 286d 6f64 656c 2e6e 756d 5f63 6f6d 706f  (model.num_compo
+0000ef60: 6e65 6e74 732c 206d 6f64 656c 2e6e 756d  nents, model.num
+0000ef70: 5f66 6561 7475 7265 7329 0a20 2020 2020  _features).     
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000ef90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000efa0: 2020 2020 2077 6974 6820 7761 726e 696e       with warnin
+0000efb0: 6773 2e63 6174 6368 5f77 6172 6e69 6e67  gs.catch_warning
+0000efc0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+0000efd0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+0000efe0: 6369 6b69 745f 6c65 6172 6e3c 312e 312e  cikit_learn<1.1.
+0000eff0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0000f000: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0000f010: 6773 2e66 696c 7465 7277 6172 6e69 6e67  gs.filterwarning
+0000f020: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000f030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000f040: 616c 7761 7973 222c 2022 4d65 616e 206f  always", "Mean o
+0000f050: 6620 656d 7074 7920 736c 6963 652e 222c  f empty slice.",
+0000f060: 2052 756e 7469 6d65 5761 726e 696e 670a   RuntimeWarning.
+0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f080: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0a0: 2020 7769 7468 206e 756d 7079 2e65 7272    with numpy.err
+0000f0b0: 7374 6174 6528 696e 7661 6c69 643d 2269  state(invalid="i
+0000f0c0: 676e 6f72 6522 2c20 6469 7669 6465 3d22  gnore", divide="
+0000f0d0: 6967 6e6f 7265 2229 3a0a 2020 2020 2020  ignore"):.      
+0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0f0: 2020 2020 2020 6d6f 6465 6c2e 6669 745f        model.fit_
+0000f100: 7472 616e 7366 6f72 6d28 573d 6669 6c65  transform(W=file
+0000f110: 5b22 5722 5d2c 2048 3d66 696c 655b 2248  ["W"], H=file["H
+0000f120: 225d 290a 0a20 2020 2020 2020 2020 2020  "])..           
+0000f130: 2048 2c20 7661 6c73 2c20 5720 3d20 6d6f   H, vals, W = mo
+0000f140: 6465 6c2e 482c 206d 6f64 656c 2e73 696e  del.H, model.sin
+0000f150: 6775 6c61 725f 7661 6c75 6573 2c20 6d6f  gular_values, mo
+0000f160: 6465 6c2e 570a 2020 2020 2020 2020 7265  del.W.        re
+0000f170: 7475 726e 2076 616c 7320 6966 2072 6574  turn vals if ret
+0000f180: 7572 6e5f 7661 6c73 2065 6c73 6520 2848  urn_vals else (H
+0000f190: 2c20 5729 0a0a 2020 2020 6465 6620 6e69  , W)..    def ni
+0000f1a0: 6361 280a 2020 2020 2020 2020 7365 6c66  ca(.        self
+0000f1b0: 2c0a 2020 2020 2020 2020 6e75 6d5f 636f  ,.        num_co
+0000f1c0: 6d70 6f6e 656e 7473 2c0a 2020 2020 2020  mponents,.      
+0000f1d0: 2020 6368 756e 6b73 697a 653d 4e6f 6e65    chunksize=None
+0000f1e0: 2c0a 2020 2020 2020 2020 6e75 6d5f 6974  ,.        num_it
+0000f1f0: 6572 3d35 3030 2c0a 2020 2020 2020 2020  er=500,.        
+0000f200: 6572 726f 725f 7374 6570 3d4e 6f6e 652c  error_step=None,
+0000f210: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+0000f220: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+0000f230: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f240: 2020 436f 6d70 7574 6520 4e6f 6e2d 6e65    Compute Non-ne
+0000f250: 6761 7469 7665 2049 6e64 6570 656e 6465  gative Independe
+0000f260: 6e74 2043 6f6d 706f 6e65 6e74 2041 6e61  nt Component Ana
+0000f270: 6c79 7369 7320 6f6e 2074 6865 2064 6174  lysis on the dat
+0000f280: 612e 0a20 2020 2020 2020 2054 6865 206d  a..        The m
+0000f290: 6574 686f 642c 2066 6972 7374 2063 6f6e  ethod, first con
+0000f2a0: 7665 7274 732c 2069 6620 6e6f 7420 616c  verts, if not al
+0000f2b0: 7265 6164 792c 2074 6865 2064 6174 6120  ready, the data 
+0000f2c0: 696e 746f 2061 6e20 6864 6635 2066 696c  into an hdf5 fil
+0000f2d0: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+0000f2e0: 2077 6974 6820 7468 6520 696d 6167 6573   with the images
+0000f2f0: 2066 6c61 7474 656e 6564 2069 6e20 7468   flattened in th
+0000f300: 6520 726f 7773 2e0a 0a20 2020 2020 2020  e rows...       
+0000f310: 203a 7061 7261 6d20 6e75 6d5f 636f 6d70   :param num_comp
+0000f320: 6f6e 656e 7473 3a20 4e75 6d62 6572 206f  onents: Number o
+0000f330: 6620 636f 6d70 6f6e 656e 7473 2074 6f20  f components to 
+0000f340: 6669 6e64 0a20 2020 2020 2020 203a 7479  find.        :ty
+0000f350: 7065 206e 756d 5f63 6f6d 706f 6e65 6e74  pe num_component
+0000f360: 733a 2055 6e69 6f6e 5b4e 6f6e 652c 2069  s: Union[None, i
+0000f370: 6e74 5d0a 2020 2020 2020 2020 3a70 6172  nt].        :par
+0000f380: 616d 2063 6875 6e6b 7369 7a65 3a20 4e75  am chunksize: Nu
+0000f390: 6d62 6572 206f 6620 6368 756e 6b73 2066  mber of chunks f
+0000f3a0: 6f72 2077 6869 6368 2074 6865 2077 6869  or which the whi
+0000f3b0: 7465 6e69 6e67 206d 7573 7420 6265 2063  tening must be c
+0000f3c0: 6f6d 7075 7465 642c 0a20 2020 2020 2020  omputed,.       
+0000f3d0: 2020 2020 2069 6e63 7265 6d65 6e74 616c       incremental
+0000f3e0: 6c79 2c20 6465 6661 756c 7473 2074 6f20  ly, defaults to 
+0000f3f0: 4e6f 6e65 0a20 2020 2020 2020 203a 7479  None.        :ty
+0000f400: 7065 2063 6875 6e6b 7369 7a65 3a20 556e  pe chunksize: Un
+0000f410: 696f 6e5b 4e6f 6e65 2c20 696e 745d 2c20  ion[None, int], 
+0000f420: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000f430: 203a 7061 7261 6d20 6e75 6d5f 6974 6572   :param num_iter
+0000f440: 3a20 4e75 6d62 6572 206f 6620 6974 6572  : Number of iter
+0000f450: 6174 696f 6e73 2c20 6465 6661 756c 7473  ations, defaults
+0000f460: 2074 6f20 3530 300a 2020 2020 2020 2020   to 500.        
+0000f470: 3a74 7970 6520 6e75 6d5f 6974 6572 3a20  :type num_iter: 
+0000f480: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
+0000f490: 2020 2020 2020 3a70 6172 616d 2065 7272        :param err
+0000f4a0: 6f72 5f73 7465 703a 2049 6620 6e6f 7420  or_step: If not 
+0000f4b0: 4e6f 6e65 2c20 6669 6e64 2074 6865 2065  None, find the e
+0000f4c0: 7272 6f72 2065 7665 7279 2065 7272 6f72  rror every error
+0000f4d0: 5f73 7465 7020 616e 6420 636f 6d70 6172  _step and compar
+0000f4e0: 6573 2069 740a 2020 2020 2020 2020 2020  es it.          
+0000f4f0: 2020 746f 2063 6865 636b 2066 6f72 2063    to check for c
+0000f500: 6f6e 7665 7267 656e 6365 2e20 544f 444f  onvergence. TODO
+0000f510: 3a20 6e6f 7420 6162 6c65 2066 6f72 2068  : not able for h
+0000f520: 7567 6520 6461 7461 7365 7473 2e0a 2020  uge datasets..  
+0000f530: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
+0000f540: 6963 6573 3a20 4966 206e 6f74 204e 6f6e  ices: If not Non
+0000f550: 652c 2061 7070 6c79 206d 6574 686f 6420  e, apply method 
+0000f560: 6f6e 6c79 2074 6f20 696e 6469 6365 7320  only to indices 
+0000f570: 6f66 2064 6174 612c 2064 6566 6175 6c74  of data, default
+0000f580: 7320 746f 204e 6f6e 650a 2020 2020 2020  s to None.      
+0000f590: 2020 3a74 7970 6520 696e 6469 6365 733a    :type indices:
+0000f5a0: 2055 6e69 6f6e 5b4e 6f6e 652c 2061 7272   Union[None, arr
+0000f5b0: 6179 5f6c 696b 655d 2c20 6f70 7469 6f6e  ay_like], option
+0000f5c0: 616c 0a0a 2020 2020 2020 2020 3a72 6574  al..        :ret
+0000f5d0: 7572 6e3a 2028 482c 2057 293a 2054 6865  urn: (H, W): The
+0000f5e0: 2063 6f6d 706f 6e65 6e74 7320 6d61 7472   components matr
+0000f5f0: 6978 2061 6e64 2074 6865 206d 6978 696e  ix and the mixin
+0000f600: 6720 6d61 7472 6978 2e0a 2020 2020 2020  g matrix..      
+0000f610: 2020 2222 220a 2020 2020 2020 2020 6273    """.        bs
+0000f620: 735f 6469 7220 3d20 6f73 2e70 6174 682e  s_dir = os.path.
+0000f630: 6a6f 696e 2873 656c 662e 6469 722c 2022  join(self.dir, "
+0000f640: 6273 7322 290a 2020 2020 2020 2020 6f73  bss").        os
+0000f650: 2e6d 616b 6564 6972 7328 6273 735f 6469  .makedirs(bss_di
+0000f660: 722c 2065 7869 7374 5f6f 6b3d 5472 7565  r, exist_ok=True
+0000f670: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000f680: 6c66 2e5f 696e 5f6d 656d 6f72 793a 0a20  lf._in_memory:. 
+0000f690: 2020 2020 2020 2020 2020 2063 6875 6e6b             chunk
+0000f6a0: 7369 7a65 203d 204e 6f6e 650a 2020 2020  size = None.    
+0000f6b0: 2020 2020 7769 7468 2073 656c 662e 6461      with self.da
+0000f6c0: 7461 2e6f 7065 6e5f 6173 5f68 6466 3528  ta.open_as_hdf5(
+0000f6d0: 6273 735f 6469 7229 2061 7320 6835 6465  bss_dir) as h5de
+0000f6e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+0000f6f0: 6d6f 6465 6c20 3d20 4e49 4341 280a 2020  model = NICA(.  
+0000f700: 2020 2020 2020 2020 2020 2020 2020 6835                h5
+0000f710: 6465 7374 2c0a 2020 2020 2020 2020 2020  dest,.          
+0000f720: 2020 2020 2020 6e75 6d5f 636f 6d70 6f6e        num_compon
+0000f730: 656e 7473 2c0a 2020 2020 2020 2020 2020  ents,.          
+0000f740: 2020 2020 2020 6368 756e 6b73 697a 652c        chunksize,
+0000f750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f760: 2069 6e64 6963 6573 3d69 6e64 6963 6573   indices=indices
+0000f770: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000f780: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0000f790: 6c2e 6669 745f 7472 616e 7366 6f72 6d28  l.fit_transform(
+0000f7a0: 6d61 785f 6974 6572 3d6e 756d 5f69 7465  max_iter=num_ite
+0000f7b0: 722c 2065 7272 6f72 5f73 7465 703d 6572  r, error_step=er
+0000f7c0: 726f 725f 7374 6570 290a 2020 2020 2020  ror_step).      
+0000f7d0: 2020 2020 2020 7265 7475 726e 206e 756d        return num
+0000f7e0: 7079 2e61 6273 286d 6f64 656c 2e48 292c  py.abs(model.H),
+0000f7f0: 206e 756d 7079 2e61 6273 286d 6f64 656c   numpy.abs(model
+0000f800: 2e57 290a 0a20 2020 2064 6566 206e 6d66  .W)..    def nmf
+0000f810: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000f820: 2020 2020 2020 2020 6e75 6d5f 636f 6d70          num_comp
+0000f830: 6f6e 656e 7473 2c0a 2020 2020 2020 2020  onents,.        
+0000f840: 6e75 6d5f 6974 6572 3d31 3030 2c0a 2020  num_iter=100,.  
+0000f850: 2020 2020 2020 6572 726f 725f 7374 6570        error_step
+0000f860: 3d4e 6f6e 652c 0a20 2020 2020 2020 2077  =None,.        w
+0000f870: 6174 6572 6661 6c6c 3d4e 6f6e 652c 0a20  aterfall=None,. 
+0000f880: 2020 2020 2020 2048 3d4e 6f6e 652c 0a20         H=None,. 
+0000f890: 2020 2020 2020 2057 3d4e 6f6e 652c 0a20         W=None,. 
+0000f8a0: 2020 2020 2020 2076 7374 6570 3d31 3030         vstep=100
+0000f8b0: 2c0a 2020 2020 2020 2020 6873 7465 703d  ,.        hstep=
+0000f8c0: 3130 3030 2c0a 2020 2020 2020 2020 696e  1000,.        in
+0000f8d0: 6469 6365 733d 4e6f 6e65 2c0a 2020 2020  dices=None,.    
+0000f8e0: 2020 2020 696e 6974 3d4e 6f6e 652c 0a20      init=None,. 
+0000f8f0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000f900: 220a 2020 2020 2020 2020 436f 6d70 7574  ".        Comput
+0000f910: 6520 4e6f 6e2d 6e65 6761 7469 7665 204d  e Non-negative M
+0000f920: 6174 7269 7820 4661 6374 6f72 697a 6174  atrix Factorizat
+0000f930: 696f 6e20 6f6e 2074 6865 2064 6174 612e  ion on the data.
+0000f940: 0a20 2020 2020 2020 2054 6865 206d 6574  .        The met
+0000f950: 686f 642c 2066 6972 7374 2063 6f6e 7665  hod, first conve
+0000f960: 7274 732c 2069 6620 6e6f 7420 616c 7265  rts, if not alre
+0000f970: 6164 792c 2074 6865 2064 6174 6120 696e  ady, the data in
+0000f980: 746f 2061 6e20 6864 6635 2066 696c 6520  to an hdf5 file 
+0000f990: 6f62 6a65 6374 0a20 2020 2020 2020 2077  object.        w
+0000f9a0: 6974 6820 7468 6520 696d 6167 6573 2066  ith the images f
+0000f9b0: 6c61 7474 656e 6564 2069 6e20 7468 6520  lattened in the 
+0000f9c0: 726f 7773 2e0a 0a20 2020 2020 2020 203a  rows...        :
+0000f9d0: 7061 7261 6d20 6e75 6d5f 636f 6d70 6f6e  param num_compon
+0000f9e0: 656e 7473 3a20 4e75 6d62 6572 206f 6620  ents: Number of 
+0000f9f0: 636f 6d70 6f6e 656e 7473 2074 6f20 6669  components to fi
+0000fa00: 6e64 0a20 2020 2020 2020 203a 7479 7065  nd.        :type
+0000fa10: 206e 756d 5f63 6f6d 706f 6e65 6e74 733a   num_components:
+0000fa20: 2055 6e69 6f6e 5b4e 6f6e 652c 2069 6e74   Union[None, int
+0000fa30: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+0000fa40: 206e 756d 5f69 7465 723a 204e 756d 6265   num_iter: Numbe
+0000fa50: 7220 6f66 2069 7465 7261 7469 6f6e 732c  r of iterations,
+0000fa60: 2064 6566 6175 6c74 7320 746f 2031 3030   defaults to 100
+0000fa70: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+0000fa80: 756d 5f69 7465 723a 2069 6e74 2c20 6f70  um_iter: int, op
+0000fa90: 7469 6f6e 616c 0a20 2020 2020 2020 203a  tional.        :
+0000faa0: 7061 7261 6d20 6572 726f 725f 7374 6570  param error_step
+0000fab0: 3a20 4966 206e 6f74 204e 6f6e 652c 2066  : If not None, f
+0000fac0: 696e 6420 7468 6520 6572 726f 7220 6576  ind the error ev
+0000fad0: 6572 7920 6572 726f 725f 7374 6570 2061  ery error_step a
+0000fae0: 6e64 2063 6f6d 7061 7265 7320 6974 0a20  nd compares it. 
+0000faf0: 2020 2020 2020 2020 2020 2074 6f20 6368             to ch
+0000fb00: 6563 6b20 666f 7220 636f 6e76 6572 6765  eck for converge
+0000fb10: 6e63 652c 2064 6566 6175 6c74 7320 746f  nce, defaults to
+0000fb20: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000fb30: 2020 544f 444f 3a20 6e6f 7420 6162 6c65    TODO: not able
+0000fb40: 2066 6f72 2068 7567 6520 6461 7461 7365   for huge datase
+0000fb50: 7473 2e0a 2020 2020 2020 2020 3a74 7970  ts..        :typ
+0000fb60: 6520 6572 726f 725f 7374 6570 3a20 556e  e error_step: Un
+0000fb70: 696f 6e5b 4e6f 6e65 2c20 696e 745d 2c20  ion[None, int], 
+0000fb80: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000fb90: 203a 7061 7261 6d20 7761 7465 7266 616c   :param waterfal
+0000fba0: 6c3a 2049 6620 6e6f 7420 4e6f 6e65 2c20  l: If not None, 
+0000fbb0: 4e4d 4620 6973 2063 6f6d 7075 7465 6420  NMF is computed 
+0000fbc0: 7573 696e 6720 7468 6520 7761 7465 7266  using the waterf
+0000fbd0: 616c 6c20 6d65 7468 6f64 2e0a 2020 2020  all method..    
+0000fbe0: 2020 2020 2020 2020 5468 6520 7061 7261          The para
+0000fbf0: 6d65 7465 7220 7368 6f75 6c64 2062 6520  meter should be 
+0000fc00: 616e 2061 7272 6179 2077 6974 6820 7468  an array with th
+0000fc10: 6520 6e75 6d62 6572 206f 6620 6974 6572  e number of iter
+0000fc20: 6174 696f 6e73 2070 6572 0a20 2020 2020  ations per.     
+0000fc30: 2020 2020 2020 2073 7562 2d63 6f6d 7075         sub-compu
+0000fc40: 7461 7469 6f6e 2c20 6465 6661 756c 7473  tation, defaults
+0000fc50: 2074 6f20 4e6f 6e65 0a20 2020 2020 2020   to None.       
+0000fc60: 203a 7479 7065 2077 6174 6572 6661 6c6c   :type waterfall
+0000fc70: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 6172  : Union[None, ar
+0000fc80: 7261 795f 6c69 6b65 5d2c 206f 7074 696f  ray_like], optio
+0000fc90: 6e61 6c0a 2020 2020 2020 2020 3a70 6172  nal.        :par
+0000fca0: 616d 2048 3a20 496e 6974 206d 6174 7269  am H: Init matri
+0000fcb0: 7820 666f 7220 4820 6f66 2073 6861 7065  x for H of shape
+0000fcc0: 2028 6e5f 636f 6d70 6f6e 656e 7473 2c20   (n_components, 
+0000fcd0: 6e5f 7361 6d70 6c65 7329 2c20 6465 6661  n_samples), defa
+0000fce0: 756c 7473 2074 6f20 4e6f 6e65 0a20 2020  ults to None.   
+0000fcf0: 2020 2020 203a 7479 7065 2048 3a20 556e       :type H: Un
+0000fd00: 696f 6e5b 4e6f 6e65 2c20 6172 7261 795f  ion[None, array_
+0000fd10: 6c69 6b65 5d2c 206f 7074 696f 6e61 6c0a  like], optional.
+0000fd20: 2020 2020 2020 2020 3a70 6172 616d 2057          :param W
+0000fd30: 3a20 496e 6974 206d 6174 7269 7820 666f  : Init matrix fo
+0000fd40: 7220 5720 6f66 2073 6861 7065 2028 6e5f  r W of shape (n_
+0000fd50: 6665 6174 7572 6573 2c20 6e5f 636f 6d70  features, n_comp
+0000fd60: 6f6e 656e 7473 292c 2064 6566 6175 6c74  onents), default
+0000fd70: 7320 746f 204e 6f6e 650a 2020 2020 2020  s to None.      
+0000fd80: 2020 3a74 7970 6520 573a 2055 6e69 6f6e    :type W: Union
+0000fd90: 5b4e 6f6e 652c 2061 7272 6179 5f6c 696b  [None, array_lik
+0000fda0: 655d 2c20 6f70 7469 6f6e 616c 0a20 2020  e], optional.   
+0000fdb0: 2020 2020 203a 7061 7261 6d20 696e 6469       :param indi
+0000fdc0: 6365 733a 2049 6620 6e6f 7420 4e6f 6e65  ces: If not None
+0000fdd0: 2c20 6170 706c 7920 6d65 7468 6f64 206f  , apply method o
+0000fde0: 6e6c 7920 746f 2069 6e64 6963 6573 206f  nly to indices o
+0000fdf0: 6620 6461 7461 2c20 6465 6661 756c 7473  f data, defaults
+0000fe00: 2074 6f20 4e6f 6e65 0a20 2020 2020 2020   to None.       
+0000fe10: 203a 7479 7065 2069 6e64 6963 6573 3a20   :type indices: 
+0000fe20: 556e 696f 6e5b 4e6f 6e65 2c20 6172 7261  Union[None, arra
+0000fe30: 795f 6c69 6b65 5d2c 206f 7074 696f 6e61  y_like], optiona
+0000fe40: 6c0a 0a20 2020 2020 2020 203a 7265 7475  l..        :retu
+0000fe50: 726e 3a20 2848 2c20 5729 3a20 5468 6520  rn: (H, W): The 
+0000fe60: 636f 6d70 6f6e 656e 7473 206d 6174 7269  components matri
+0000fe70: 7820 616e 6420 7468 6520 6d69 7869 6e67  x and the mixing
+0000fe80: 206d 6174 7269 782e 0a20 2020 2020 2020   matrix..       
+0000fe90: 2022 2222 0a20 2020 2020 2020 2062 7373   """.        bss
+0000fea0: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
+0000feb0: 6f69 6e28 7365 6c66 2e64 6972 2c20 2262  oin(self.dir, "b
+0000fec0: 7373 2229 0a20 2020 2020 2020 206f 732e  ss").        os.
+0000fed0: 6d61 6b65 6469 7273 2862 7373 5f64 6972  makedirs(bss_dir
+0000fee0: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
+0000fef0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000ff00: 662e 5f69 6e5f 6d65 6d6f 7279 3a0a 2020  f._in_memory:.  
+0000ff10: 2020 2020 2020 2020 2020 6672 6f6d 2073            from s
+0000ff20: 6b6c 6561 726e 2069 6d70 6f72 7420 6465  klearn import de
+0000ff30: 636f 6d70 6f73 6974 696f 6e0a 0a20 2020  composition..   
+0000ff40: 2020 2020 2020 2020 206d 6f64 656c 203d           model =
+0000ff50: 2064 6563 6f6d 706f 7369 7469 6f6e 2e4e   decomposition.N
+0000ff60: 4d46 280a 2020 2020 2020 2020 2020 2020  MF(.            
+0000ff70: 2020 2020 6e5f 636f 6d70 6f6e 656e 7473      n_components
+0000ff80: 3d6e 756d 5f63 6f6d 706f 6e65 6e74 732c  =num_components,
+0000ff90: 2069 6e69 743d 696e 6974 2c20 6d61 785f   init=init, max_
+0000ffa0: 6974 6572 3d6e 756d 5f69 7465 720a 2020  iter=num_iter.  
+0000ffb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000ffc0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000ffd0: 662e 6461 7461 2e6f 7065 6e5f 6173 5f68  f.data.open_as_h
+0000ffe0: 6466 3528 6273 735f 6469 7229 2061 7320  df5(bss_dir) as 
+0000fff0: 6835 6465 7374 3a0a 2020 2020 2020 2020  h5dest:.        
+00010000: 2020 2020 2020 2020 6966 2069 6e64 6963          if indic
+00010010: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010030: 2020 2020 5820 3d20 6835 6465 7374 5b69      X = h5dest[i
+00010040: 6e64 6963 6573 5d0a 2020 2020 2020 2020  ndices].        
+00010050: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 5820 3d20 6835 6465 7374 0a20 2020    X = h5dest.   
+00010080: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010090: 6e75 6d70 792e 616e 7928 585b 3a2c 203a  numpy.any(X[:, :
+000100a0: 5d20 3c20 3029 3a0a 2020 2020 2020 2020  ] < 0):.        
+000100b0: 2020 2020 2020 2020 2020 2020 5f6c 6f67              _log
+000100c0: 6765 722e 7761 726e 696e 6728 2253 6574  ger.warning("Set
+000100d0: 7469 6e67 206e 6567 6174 6976 6520 7661  ting negative va
+000100e0: 6c75 6573 2074 6f20 3020 746f 2063 6f6d  lues to 0 to com
+000100f0: 7075 7465 204e 4d46 2229 0a20 2020 2020  pute NMF").     
+00010100: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+00010110: 5b58 5b3a 2c20 3a5d 203c 2030 5d20 3d20  [X[:, :] < 0] = 
+00010120: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00010130: 2020 6966 2048 2069 7320 6e6f 7420 4e6f    if H is not No
+00010140: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00010150: 2020 2020 2020 2020 5820 3d20 582e 6173          X = X.as
+00010160: 7479 7065 2848 2e64 7479 7065 290a 2020  type(H.dtype).  
+00010170: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00010180: 6966 2057 2069 7320 6e6f 7420 4e6f 6e65  if W is not None
+00010190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000101a0: 2020 2020 2020 5820 3d20 582e 6173 7479        X = X.asty
+000101b0: 7065 2857 2e64 7479 7065 290a 2020 2020  pe(W.dtype).    
+000101c0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000101d0: 2077 6172 6e69 6e67 732e 6361 7463 685f   warnings.catch_
+000101e0: 7761 726e 696e 6773 2829 3a0a 2020 2020  warnings():.    
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 7761 726e 696e 6773 2e73 696d 706c 6566  warnings.simplef
+00010210: 696c 7465 7228 2261 6c77 6179 7322 2c20  ilter("always", 
+00010220: 436f 6e76 6572 6765 6e63 6557 6172 6e69  ConvergenceWarni
+00010230: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
+00010240: 2020 2020 2020 2020 5720 3d20 6d6f 6465          W = mode
+00010250: 6c2e 6669 745f 7472 616e 7366 6f72 6d28  l.fit_transform(
+00010260: 582c 2057 3d57 2c20 483d 4829 0a20 2020  X, W=W, H=H).   
+00010270: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010280: 7572 6e20 6d6f 6465 6c2e 636f 6d70 6f6e  urn model.compon
+00010290: 656e 7473 5f2c 2057 0a20 2020 2020 2020  ents_, W.       
+000102a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000102b0: 2020 2069 6620 7761 7465 7266 616c 6c20     if waterfall 
+000102c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000102d0: 2020 2020 2020 2020 2020 2020 2048 2c20               H, 
+000102e0: 5720 3d20 7365 6c66 2e5f 7761 7465 7266  W = self._waterf
+000102f0: 616c 6c5f 6e6d 6628 0a20 2020 2020 2020  all_nmf(.       
+00010300: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00010310: 5f63 6f6d 706f 6e65 6e74 732c 2077 6174  _components, wat
+00010320: 6572 6661 6c6c 2c20 7673 7465 702c 2068  erfall, vstep, h
+00010330: 7374 6570 2c20 696e 6469 6365 733d 696e  step, indices=in
+00010340: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
+00010350: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010360: 2020 2020 2077 6974 6820 7365 6c66 2e64       with self.d
+00010370: 6174 612e 6f70 656e 5f61 735f 6864 6635  ata.open_as_hdf5
+00010380: 2862 7373 5f64 6972 2920 6173 2068 3564  (bss_dir) as h5d
+00010390: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
+000103a0: 2020 2020 206d 6f64 656c 203d 204e 4d46       model = NMF
+000103b0: 2868 3564 6573 742c 206e 756d 5f63 6f6d  (h5dest, num_com
+000103c0: 706f 6e65 6e74 732c 2069 6e64 6963 6573  ponents, indices
+000103d0: 3d69 6e64 6963 6573 290a 2020 2020 2020  =indices).      
+000103e0: 2020 2020 2020 2020 2020 7769 7468 2077            with w
+000103f0: 6172 6e69 6e67 732e 6361 7463 685f 7761  arnings.catch_wa
+00010400: 726e 696e 6773 2829 3a0a 2020 2020 2020  rnings():.      
+00010410: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+00010420: 726e 696e 6773 2e73 696d 706c 6566 696c  rnings.simplefil
+00010430: 7465 7228 2261 6c77 6179 7322 2c20 436f  ter("always", Co
+00010440: 6e76 6572 6765 6e63 6557 6172 6e69 6e67  nvergenceWarning
+00010450: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010460: 2020 2020 2020 6d6f 6465 6c2e 6669 745f        model.fit_
+00010470: 7472 616e 7366 6f72 6d28 0a20 2020 2020  transform(.     
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 206d 6178 5f69 7465 723d 6e75 6d5f     max_iter=num_
+000104a0: 6974 6572 2c0a 2020 2020 2020 2020 2020  iter,.          
+000104b0: 2020 2020 2020 2020 2020 2020 2020 483d                H=
+000104c0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+000104d0: 2020 2020 2020 2020 2020 2057 3d57 2c0a             W=W,.
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104f0: 2020 2020 2020 2020 7673 7465 703d 7673          vstep=vs
+00010500: 7465 702c 0a20 2020 2020 2020 2020 2020  tep,.           
+00010510: 2020 2020 2020 2020 2020 2020 2068 7374               hst
+00010520: 6570 3d68 7374 6570 2c0a 2020 2020 2020  ep=hstep,.      
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 2020 6572 726f 725f 7374 6570 3d65 7272    error_step=err
+00010550: 6f72 5f73 7465 702c 0a20 2020 2020 2020  or_step,.       
+00010560: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00010570: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010580: 6574 7572 6e20 6d6f 6465 6c2e 482c 206d  eturn model.H, m
+00010590: 6f64 656c 2e57 0a0a 2020 2020 6465 6620  odel.W..    def 
+000105a0: 6e69 6361 5f6e 6d66 280a 2020 2020 2020  nica_nmf(.      
+000105b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000105c0: 6e75 6d5f 636f 6d70 6f6e 656e 7473 2c0a  num_components,.
+000105d0: 2020 2020 2020 2020 6368 756e 6b73 697a          chunksiz
+000105e0: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+000105f0: 6e75 6d5f 6974 6572 3d35 3030 2c0a 2020  num_iter=500,.  
+00010600: 2020 2020 2020 7761 7465 7266 616c 6c3d        waterfall=
+00010610: 4e6f 6e65 2c0a 2020 2020 2020 2020 6572  None,.        er
+00010620: 726f 725f 7374 6570 3d4e 6f6e 652c 0a20  ror_step=None,. 
+00010630: 2020 2020 2020 2076 7374 6570 3d31 3030         vstep=100
+00010640: 2c0a 2020 2020 2020 2020 6873 7465 703d  ,.        hstep=
+00010650: 3130 3030 2c0a 2020 2020 2020 2020 696e  1000,.        in
+00010660: 6469 6365 733d 4e6f 6e65 2c0a 2020 2020  dices=None,.    
+00010670: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00010680: 2020 2020 2020 2041 7070 6c69 6573 2062         Applies b
+00010690: 6f74 6820 4e49 4341 2061 6e64 204e 4d46  oth NICA and NMF
+000106a0: 2074 6f20 7468 6520 6461 7461 2e20 5468   to the data. Th
+000106b0: 6520 696e 6974 2048 2061 6e64 2057 2066  e init H and W f
+000106c0: 6f72 204e 4d46 2061 7265 2074 6865 0a20  or NMF are the. 
+000106d0: 2020 2020 2020 2072 6573 756c 7420 6f66         result of
+000106e0: 204e 4943 412e 0a20 2020 2020 2020 2022   NICA..        "
+000106f0: 2222 0a20 2020 2020 2020 2048 2c20 5720  "".        H, W 
+00010700: 3d20 7365 6c66 2e6e 6963 6128 6e75 6d5f  = self.nica(num_
+00010710: 636f 6d70 6f6e 656e 7473 2c20 6368 756e  components, chun
+00010720: 6b73 697a 652c 206e 756d 5f69 7465 722c  ksize, num_iter,
+00010730: 2069 6e64 6963 6573 3d69 6e64 6963 6573   indices=indices
+00010740: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
+00010750: 7469 616c 204e 4d46 2066 6163 746f 7269  tial NMF factori
+00010760: 7a61 7469 6f6e 3a20 5820 3d20 4630 202a  zation: X = F0 *
+00010770: 2047 300a 2020 2020 2020 2020 5720 3d20   G0.        W = 
+00010780: 6e75 6d70 792e 6162 7328 5729 0a20 2020  numpy.abs(W).   
+00010790: 2020 2020 2048 203d 206e 756d 7079 2e61       H = numpy.a
+000107a0: 6273 2848 290a 0a20 2020 2020 2020 2072  bs(H)..        r
+000107b0: 6574 7572 6e20 7365 6c66 2e6e 6d66 280a  eturn self.nmf(.
+000107c0: 2020 2020 2020 2020 2020 2020 6d69 6e28              min(
+000107d0: 6e75 6d5f 636f 6d70 6f6e 656e 7473 2c20  num_components, 
+000107e0: 482e 7368 6170 655b 305d 292c 0a20 2020  H.shape[0]),.   
+000107f0: 2020 2020 2020 2020 206e 756d 5f69 7465           num_ite
+00010800: 722c 0a20 2020 2020 2020 2020 2020 2065  r,.            e
+00010810: 7272 6f72 5f73 7465 702c 0a20 2020 2020  rror_step,.     
+00010820: 2020 2020 2020 2077 6174 6572 6661 6c6c         waterfall
+00010830: 2c0a 2020 2020 2020 2020 2020 2020 482c  ,.            H,
+00010840: 0a20 2020 2020 2020 2020 2020 2057 2c0a  .            W,.
+00010850: 2020 2020 2020 2020 2020 2020 7673 7465              vste
+00010860: 702c 0a20 2020 2020 2020 2020 2020 2068  p,.            h
+00010870: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+00010880: 2020 696e 6469 6365 733d 696e 6469 6365    indices=indice
+00010890: 732c 0a20 2020 2020 2020 2020 2020 2069  s,.            i
+000108a0: 6e69 743d 2263 7573 746f 6d22 2c0a 2020  nit="custom",.  
+000108b0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+000108c0: 2061 7070 6c79 5f6d 6f6d 656e 7473 2873   apply_moments(s
+000108d0: 656c 662c 2069 6e64 6963 6573 3d4e 6f6e  elf, indices=Non
+000108e0: 652c 2063 6875 6e6b 5f73 6861 7065 3d5b  e, chunk_shape=[
+000108f0: 3530 302c 2035 3030 5d29 3a0a 2020 2020  500, 500]):.    
+00010900: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010910: 436f 6d70 7574 6520 7468 6520 434f 4d2c  Compute the COM,
+00010920: 2046 5748 4d2c 2073 6b65 776e 6573 7320   FWHM, skewness 
+00010930: 616e 6420 6b75 7274 6f73 6973 206f 6620  and kurtosis of 
+00010940: 7468 6520 6461 7461 2066 6f72 2076 6572  the data for ver
+00010950: 7920 6469 6d65 6e73 696f 6e2e 0a0a 2020  y dimension...  
+00010960: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
+00010970: 6963 6573 3a20 4966 206e 6f74 204e 6f6e  ices: If not Non
+00010980: 652c 2061 7070 6c79 206d 6574 686f 6420  e, apply method 
+00010990: 6f6e 6c79 2074 6f20 696e 6469 6365 7320  only to indices 
+000109a0: 6f66 2064 6174 612c 2064 6566 6175 6c74  of data, default
+000109b0: 7320 746f 204e 6f6e 650a 2020 2020 2020  s to None.      
+000109c0: 2020 3a74 7970 6520 696e 6469 6365 733a    :type indices:
+000109d0: 2055 6e69 6f6e 5b4e 6f6e 652c 2061 7272   Union[None, arr
+000109e0: 6179 5f6c 696b 655d 2c20 6f70 7469 6f6e  ay_like], option
+000109f0: 616c 0a20 2020 2020 2020 203a 7061 7261  al.        :para
+00010a00: 6d20 6368 756e 6b5f 7368 6170 653a 2053  m chunk_shape: S
+00010a10: 6861 7065 206f 6620 7468 6520 6368 756e  hape of the chun
+00010a20: 6b20 696d 6167 6520 746f 2075 7365 2070  k image to use p
+00010a30: 6572 2069 7465 7261 7469 6f6e 2e0a 2020  er iteration..  
+00010a40: 2020 2020 2020 2020 2020 5061 7261 6d65            Parame
+00010a50: 7465 7220 7573 6564 206f 6e6c 7920 7768  ter used only wh
+00010a60: 656e 2066 6c61 6720 696e 5f6d 656d 6f72  en flag in_memor
+00010a70: 7920 6973 2046 616c 7365 2e0a 2020 2020  y is False..    
+00010a80: 2020 2020 3a74 7970 6520 6368 756e 6b5f      :type chunk_
+00010a90: 7368 6170 653a 2061 7272 6179 5f6c 696b  shape: array_lik
+00010aa0: 652c 206f 7074 696f 6e61 6c0a 2020 2020  e, optional.    
+00010ab0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00010ac0: 2069 6620 6e6f 7420 7365 6c66 2e64 696d   if not self.dim
+00010ad0: 732e 6e64 696d 3a0a 2020 2020 2020 2020  s.ndim:.        
+00010ae0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00010af0: 2020 2020 2020 2020 7365 6c66 2e72 756e          self.run
+00010b00: 6e69 6e67 5f64 6174 6120 3d20 7365 6c66  ning_data = self
+00010b10: 2e67 6574 5f64 6174 6128 696e 6469 6365  .get_data(indice
+00010b20: 7329 0a20 2020 2020 2020 2069 6620 696e  s).        if in
+00010b30: 6469 6365 7320 6973 204e 6f6e 653a 0a20  dices is None:. 
+00010b40: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+00010b50: 6573 203d 2072 616e 6765 2873 656c 662e  es = range(self.
+00010b60: 6e66 7261 6d65 7329 0a20 2020 2020 2020  nframes).       
+00010b70: 2066 6f72 2061 7869 732c 2064 696d 2069   for axis, dim i
+00010b80: 6e20 7365 6c66 2e64 696d 733a 0a20 2020  n self.dims:.   
+00010b90: 2020 2020 2020 2020 2023 2047 6574 206d           # Get m
+00010ba0: 6f74 6f72 2076 616c 7565 7320 7065 7220  otor values per 
+00010bb0: 696d 6167 6520 6f66 2074 6865 2073 7461  image of the sta
+00010bc0: 636b 0a20 2020 2020 2020 2020 2020 2076  ck.            v
+00010bd0: 616c 7565 7320 3d20 7365 6c66 2e67 6574  alues = self.get
+00010be0: 5f64 696d 656e 7369 6f6e 735f 7661 6c75  _dimensions_valu
+00010bf0: 6573 2869 6e64 6963 6573 295b 6469 6d2e  es(indices)[dim.
+00010c00: 6e61 6d65 5d0a 2020 2020 2020 2020 2020  name].          
+00010c10: 2020 6966 2073 656c 662e 5f69 6e5f 6d65    if self._in_me
+00010c20: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
+00010c30: 2020 2020 2020 2320 4461 7461 2069 6e20        # Data in 
+00010c40: 6d65 6d6f 7279 0a20 2020 2020 2020 2020  memory.         
+00010c50: 2020 2020 2020 206d 6f6d 656e 7473 203d         moments =
+00010c60: 206e 756d 7079 2e61 7361 7272 6179 280a   numpy.asarray(.
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 2020 636f 6d70 7574 655f 6d6f 6d65      compute_mome
+00010c90: 6e74 7328 7661 6c75 6573 2c20 7365 6c66  nts(values, self
+00010ca0: 2e72 756e 6e69 6e67 5f64 6174 6129 2c20  .running_data), 
+00010cb0: 6474 7970 653d 6e75 6d70 792e 666c 6f61  dtype=numpy.floa
+00010cc0: 7436 340a 2020 2020 2020 2020 2020 2020  t64.            
+00010cd0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010cf0: 2020 2020 2020 2020 2320 4461 7461 206f          # Data o
+00010d00: 6e20 6469 736b 0a20 2020 2020 2020 2020  n disk.         
+00010d10: 2020 2020 2020 2073 7461 7274 203d 205b         start = [
+00010d20: 302c 2030 5d0a 2020 2020 2020 2020 2020  0, 0].          
+00010d30: 2020 2020 2020 696d 6720 3d20 7365 6c66        img = self
+00010d40: 2e72 756e 6e69 6e67 5f64 6174 615b 305d  .running_data[0]
+00010d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d60: 206d 6f6d 656e 7473 203d 206e 756d 7079   moments = numpy
+00010d70: 2e65 6d70 7479 280a 2020 2020 2020 2020  .empty(.        
+00010d80: 2020 2020 2020 2020 2020 2020 2834 2c20              (4, 
+00010d90: 696d 672e 7368 6170 655b 305d 2c20 696d  img.shape[0], im
+00010da0: 672e 7368 6170 655b 315d 292c 2064 7479  g.shape[1]), dty
+00010db0: 7065 3d6e 756d 7079 2e66 6c6f 6174 3634  pe=numpy.float64
+00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dd0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00010de0: 2020 2063 6875 6e6b 735f 3120 3d20 696e     chunks_1 = in
+00010df0: 7428 6e75 6d70 792e 6365 696c 2869 6d67  t(numpy.ceil(img
+00010e00: 2e73 6861 7065 5b30 5d20 2f20 6368 756e  .shape[0] / chun
+00010e10: 6b5f 7368 6170 655b 305d 2929 0a20 2020  k_shape[0])).   
+00010e20: 2020 2020 2020 2020 2020 2020 2063 6875               chu
+00010e30: 6e6b 735f 3220 3d20 696e 7428 6e75 6d70  nks_2 = int(nump
+00010e40: 792e 6365 696c 2869 6d67 2e73 6861 7065  y.ceil(img.shape
+00010e50: 5b31 5d20 2f20 6368 756e 6b5f 7368 6170  [1] / chunk_shap
+00010e60: 655b 315d 2929 0a20 2020 2020 2020 2020  e[1])).         
+00010e70: 2020 2020 2020 2069 6f5f 7574 696c 732e         io_utils.
+00010e80: 6164 7661 6e63 656d 656e 745f 6469 7370  advancement_disp
+00010e90: 6c61 7928 0a20 2020 2020 2020 2020 2020  lay(.           
+00010ea0: 2020 2020 2020 2020 2030 2c20 6368 756e           0, chun
+00010eb0: 6b73 5f31 202a 2063 6875 6e6b 735f 3220  ks_1 * chunks_2 
+00010ec0: 2a20 6c65 6e28 7365 6c66 2e72 756e 6e69  * len(self.runni
+00010ed0: 6e67 5f64 6174 6129 2c20 2243 6f6d 7075  ng_data), "Compu
+00010ee0: 7469 6e67 206d 6f6d 656e 7473 220a 2020  ting moments".  
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 666f 7220 6920 696e 2072 616e 6765 2863  for i in range(c
+00010f20: 6875 6e6b 735f 3129 3a0a 2020 2020 2020  hunks_1):.      
+00010f30: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010f40: 7220 6a20 696e 2072 616e 6765 2863 6875  r j in range(chu
+00010f50: 6e6b 735f 3229 3a0a 2020 2020 2020 2020  nks_2):.        
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 635f 696d 6167 6573 203d 205b 5d0a 2020  c_images = [].  
 00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 2020 2020 2063 6f6d 2c20 7374 642c         com, std,
-00010fa0: 2073 6b65 772c 206b 7572 7420 3d20 636f   skew, kurt = co
-00010fb0: 6d70 7574 655f 6d6f 6d65 6e74 7328 7661  mpute_moments(va
-00010fc0: 6c75 6573 2c20 635f 696d 6167 6573 290a  lues, c_images).
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2020 2020 2020 6d6f 6d65 6e74 735b          moments[
-00010ff0: 305d 5b0a 2020 2020 2020 2020 2020 2020  0][.            
-00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011010: 7374 6172 745b 305d 203a 2073 7461 7274  start[0] : start
-00011020: 5b30 5d20 2b20 6368 756e 6b5f 7368 6170  [0] + chunk_shap
-00011030: 655b 305d 2c0a 2020 2020 2020 2020 2020  e[0],.          
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 7374 6172 745b 315d 203a 2073 7461    start[1] : sta
-00011060: 7274 5b31 5d20 2b20 6368 756e 6b5f 7368  rt[1] + chunk_sh
-00011070: 6170 655b 315d 2c0a 2020 2020 2020 2020  ape[1],.        
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 5d20 3d20 636f 6d0a 2020 2020 2020 2020  ] = com.        
+00010f90: 2020 2020 2020 6370 7573 203d 206d 756c        cpus = mul
+00010fa0: 7469 7072 6f63 6573 7369 6e67 2e63 7075  tiprocessing.cpu
+00010fb0: 5f63 6f75 6e74 2829 0a20 2020 2020 2020  _count().       
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2077 6974 6820 506f 6f6c 2863 7075 7320   with Pool(cpus 
+00010fe0: 2d20 3129 2061 7320 703a 0a20 2020 2020  - 1) as p:.     
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 2020 2020 2063 5f69 6d61 6765 7320         c_images 
+00011010: 3d20 702e 6d61 7028 0a20 2020 2020 2020  = p.map(.       
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2020 2020 2020 2020 2070 6172 7469 616c           partial
+00011040: 2863 6875 6e6b 5f69 6d61 6765 2c20 7374  (chunk_image, st
+00011050: 6172 742c 2063 6875 6e6b 5f73 6861 7065  art, chunk_shape
+00011060: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2073 656c 662e 7275 6e6e 696e 675f     self.running_
+00011090: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
 000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 6d6f 6d65 6e74 735b 315d 5b0a 2020 2020  moments[1][.    
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110d0: 2020 2020 2020 2020 7374 6172 745b 305d          start[0]
-000110e0: 203a 2073 7461 7274 5b30 5d20 2b20 6368   : start[0] + ch
-000110f0: 756e 6b5f 7368 6170 655b 305d 2c0a 2020  unk_shape[0],.  
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2020 2020 7374 6172 745b            start[
-00011120: 315d 203a 2073 7461 7274 5b31 5d20 2b20  1] : start[1] + 
-00011130: 6368 756e 6b5f 7368 6170 655b 315d 2c0a  chunk_shape[1],.
-00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011150: 2020 2020 2020 2020 5d20 3d20 7374 640a          ] = std.
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 6d6f 6d65 6e74 735b          moments[
-00011180: 325d 5b0a 2020 2020 2020 2020 2020 2020  2][.            
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 7374 6172 745b 305d 203a 2073 7461 7274  start[0] : start
-000111b0: 5b30 5d20 2b20 6368 756e 6b5f 7368 6170  [0] + chunk_shap
-000111c0: 655b 305d 2c0a 2020 2020 2020 2020 2020  e[0],.          
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 7374 6172 745b 315d 203a 2073 7461    start[1] : sta
-000111f0: 7274 5b31 5d20 2b20 6368 756e 6b5f 7368  rt[1] + chunk_sh
-00011200: 6170 655b 315d 2c0a 2020 2020 2020 2020  ape[1],.        
+000110b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000110c0: 2020 2020 2020 2020 2020 2020 696f 5f75              io_u
+000110d0: 7469 6c73 2e61 6476 616e 6365 6d65 6e74  tils.advancement
+000110e0: 5f64 6973 706c 6179 280a 2020 2020 2020  _display(.      
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011100: 2020 2020 2020 6920 2a20 6368 756e 6b73        i * chunks
+00011110: 5f32 202b 206a 202b 2031 2c0a 2020 2020  _2 + j + 1,.    
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011130: 2020 2020 2020 2020 6368 756e 6b73 5f31          chunks_1
+00011140: 202a 2063 6875 6e6b 735f 322c 0a20 2020   * chunks_2,.   
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 2020 2020 2020 2022 436f 6d70 7574           "Comput
+00011170: 696e 6720 6d6f 6d65 6e74 7322 2c0a 2020  ing moments",.  
+00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011190: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 636f 6d2c 2073 7464 2c20 736b 6577 2c20  com, std, skew, 
+000111c0: 6b75 7274 203d 2063 6f6d 7075 7465 5f6d  kurt = compute_m
+000111d0: 6f6d 656e 7473 2876 616c 7565 732c 2063  oments(values, c
+000111e0: 5f69 6d61 6765 7329 0a20 2020 2020 2020  _images).       
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011200: 206d 6f6d 656e 7473 5b30 5d5b 0a20 2020   moments[0][.   
 00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 5d20 3d20 736b 6577 0a20 2020 2020 2020  ] = skew.       
-00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 206d 6f6d 656e 7473 5b33 5d5b 0a20 2020   moments[3][.   
+00011220: 2020 2020 2020 2020 2073 7461 7274 5b30           start[0
+00011230: 5d20 3a20 7374 6172 745b 305d 202b 2063  ] : start[0] + c
+00011240: 6875 6e6b 5f73 6861 7065 5b30 5d2c 0a20  hunk_shape[0],. 
 00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011260: 2020 2020 2020 2020 2073 7461 7274 5b30           start[0
-00011270: 5d20 3a20 7374 6172 745b 305d 202b 2063  ] : start[0] + c
-00011280: 6875 6e6b 5f73 6861 7065 5b30 5d2c 0a20  hunk_shape[0],. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-000112b0: 5b31 5d20 3a20 7374 6172 745b 315d 202b  [1] : start[1] +
-000112c0: 2063 6875 6e6b 5f73 6861 7065 5b31 5d2c   chunk_shape[1],
-000112d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112e0: 2020 2020 2020 2020 205d 203d 206b 7572           ] = kur
-000112f0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00011300: 2020 2020 2020 2020 2020 7374 6172 745b            start[
-00011310: 315d 203d 2063 6875 6e6b 5f73 6861 7065  1] = chunk_shape
-00011320: 5b31 5d20 2a20 286a 202b 2031 290a 2020  [1] * (j + 1).  
-00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011340: 2020 7374 6172 745b 305d 203d 2063 6875    start[0] = chu
-00011350: 6e6b 5f73 6861 7065 5b30 5d20 2a20 2869  nk_shape[0] * (i
-00011360: 202b 2031 290a 2020 2020 2020 2020 2020   + 1).          
-00011370: 2020 2020 2020 2020 2020 7374 6172 745b            start[
-00011380: 315d 203d 2030 0a20 2020 2020 2020 2020  1] = 0.         
-00011390: 2020 2073 656c 662e 6d6f 6d65 6e74 735f     self.moments_
-000113a0: 6469 6d73 5b61 7869 735d 203d 206d 6f6d  dims[axis] = mom
-000113b0: 656e 7473 0a0a 2020 2020 2020 2020 7265  ents..        re
-000113c0: 7475 726e 2073 656c 662e 6d6f 6d65 6e74  turn self.moment
-000113d0: 735f 6469 6d73 0a0a 2020 2020 6465 6620  s_dims..    def 
-000113e0: 6170 706c 795f 6669 7428 0a20 2020 2020  apply_fit(.     
-000113f0: 2020 2073 656c 662c 2069 6e64 6963 6573     self, indices
-00011400: 3d4e 6f6e 652c 2069 6e74 5f74 6872 6573  =None, int_thres
-00011410: 683d 4e6f 6e65 2c20 6368 756e 6b5f 7368  h=None, chunk_sh
-00011420: 6170 653d 5b31 3030 2c20 3130 305d 2c20  ape=[100, 100], 
-00011430: 5f64 6972 3d4e 6f6e 650a 2020 2020 293a  _dir=None.    ):
-00011440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011450: 2020 2020 2046 6974 7320 7468 6520 6461       Fits the da
-00011460: 7461 2061 726f 756e 6420 6178 6973 2030  ta around axis 0
-00011470: 2061 6e64 2073 6176 6573 2074 6865 206e   and saves the n
-00011480: 6577 2064 6174 6120 696e 746f 2064 6973  ew data into dis
-00011490: 6b2e 0a0a 2020 2020 2020 2020 3a70 6172  k...        :par
-000114a0: 616d 2069 6e64 6963 6573 3a20 496e 6469  am indices: Indi
-000114b0: 6365 7320 6f66 2074 6865 2069 6d61 6765  ces of the image
-000114c0: 7320 746f 2066 6974 2e0a 2020 2020 2020  s to fit..      
-000114d0: 2020 2020 2020 4966 204e 6f6e 652c 2074        If None, t
-000114e0: 6865 2066 6974 2069 7320 646f 6e65 2074  he fit is done t
-000114f0: 6f20 616c 6c20 7468 6520 6461 7461 2e0a  o all the data..
-00011500: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-00011510: 6469 6365 733a 2055 6e69 6f6e 5b4e 6f6e  dices: Union[Non
-00011520: 652c 2061 7272 6179 5f6c 696b 655d 0a20  e, array_like]. 
-00011530: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00011540: 745f 7468 7265 7368 3a20 7365 6520 606d  t_thresh: see `m
-00011550: 6170 7069 6e67 2e66 6974 5f70 6978 656c  apping.fit_pixel
-00011560: 600a 2020 2020 2020 2020 3a74 7970 6520  `.        :type 
-00011570: 696e 745f 7468 7265 7368 3a20 556e 696f  int_thresh: Unio
-00011580: 6e5b 4e6f 6e65 2c20 666c 6f61 745d 0a20  n[None, float]. 
-00011590: 2020 2020 2020 203a 7061 7261 6d20 6368         :param ch
-000115a0: 756e 6b5f 7368 6170 653a 2053 6861 7065  unk_shape: Shape
-000115b0: 206f 6620 7468 6520 6368 756e 6b20 696d   of the chunk im
-000115c0: 6167 6520 746f 2075 7365 2070 6572 2069  age to use per i
-000115d0: 7465 7261 7469 6f6e 2e0a 2020 2020 2020  teration..      
-000115e0: 2020 2020 2020 5061 7261 6d65 7465 7220        Parameter 
-000115f0: 7573 6564 206f 6e6c 7920 7768 656e 2066  used only when f
-00011600: 6c61 6720 696e 5f6d 656d 6f72 7920 6973  lag in_memory is
-00011610: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00011620: 3a74 7970 6520 6368 756e 6b5f 7368 6170  :type chunk_shap
-00011630: 653a 2061 7272 6179 5f6c 696b 650a 2020  e: array_like.  
-00011640: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
-00011650: 6461 7461 7365 7420 7769 7468 2064 6174  dataset with dat
-00011660: 6120 6f66 2073 616d 6520 7369 7a65 2061  a of same size a
-00011670: 7320 6073 656c 662e 6461 7461 6020 6275  s `self.data` bu
-00011680: 7420 7769 7468 2074 6865 0a20 2020 2020  t with the.     
-00011690: 2020 2020 2020 206d 6f64 6966 6965 6420         modified 
-000116a0: 696d 6167 6573 2e20 5468 6520 7572 6c73  images. The urls
-000116b0: 206f 6620 7468 6520 6d6f 6469 6669 6564   of the modified
-000116c0: 2069 6d61 6765 7320 6172 6520 7265 706c   images are repl
-000116d0: 6163 6564 2077 6974 680a 2020 2020 2020  aced with.      
-000116e0: 2020 2020 2020 7468 6520 6e65 7720 7572        the new ur
-000116f0: 6c73 2e0a 2020 2020 2020 2020 3a72 7479  ls..        :rty
-00011700: 7065 3a20 4461 7461 7365 740a 2020 2020  pe: Dataset.    
-00011710: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00011720: 205f 6469 7220 3d20 7365 6c66 2e64 6972   _dir = self.dir
-00011730: 2069 6620 5f64 6972 2069 7320 4e6f 6e65   if _dir is None
-00011740: 2065 6c73 6520 5f64 6972 0a20 2020 2020   else _dir.     
-00011750: 2020 205f 6469 7220 3d20 6f73 2e70 6174     _dir = os.pat
-00011760: 682e 6a6f 696e 285f 6469 722c 2022 6669  h.join(_dir, "fi
-00011770: 7422 290a 0a20 2020 2020 2020 206f 732e  t")..        os.
-00011780: 6d61 6b65 6469 7273 285f 6469 722c 2065  makedirs(_dir, e
-00011790: 7869 7374 5f6f 6b3d 5472 7565 290a 0a20  xist_ok=True).. 
-000117a0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-000117b0: 2e73 7461 7465 5f6f 665f 6f70 6572 6174  .state_of_operat
-000117c0: 696f 6e73 2e72 756e 5f63 6f6e 7465 7874  ions.run_context
-000117d0: 284f 7065 7261 7469 6f6e 2e46 4954 293a  (Operation.FIT):
-000117e0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
-000117f0: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-00011800: 2020 2076 616c 7565 7320 3d20 4e6f 6e65     values = None
-00011810: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00011820: 7065 203d 204e 6f6e 650a 2020 2020 2020  pe = None.      
-00011830: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-00011840: 662e 6765 745f 6461 7461 2869 6e64 6963  f.get_data(indic
-00011850: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00011860: 2320 4669 7420 6361 6e20 6f6e 6c79 2062  # Fit can only b
-00011870: 6520 646f 6e65 2069 6620 726f 636b 696e  e done if rockin
-00011880: 6720 6375 7276 6573 2061 7265 2061 7420  g curves are at 
-00011890: 6c65 6173 7420 6f66 2073 697a 6520 330a  least of size 3.
-000118a0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000118b0: 656e 2864 6174 6129 203c 2033 3a0a 2020  en(data) < 3:.  
-000118c0: 2020 2020 2020 2020 2020 2020 2020 5f6c                _l
-000118d0: 6f67 6765 722e 7761 726e 696e 6728 224e  ogger.warning("N
-000118e0: 6f74 2065 6e6f 7567 6820 7661 6c75 6573  ot enough values
-000118f0: 2066 6f72 2066 6974 7469 6e67 2229 0a20   for fitting"). 
-00011900: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011910: 6574 7572 6e20 7365 6c66 0a20 2020 2020  eturn self.     
-00011920: 2020 2020 2020 2069 6620 696e 6469 6365         if indice
-00011930: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-00011940: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-00011950: 6573 203d 2072 616e 6765 2864 6174 612e  es = range(data.
-00011960: 7368 6170 655b 305d 290a 0a20 2020 2020  shape[0])..     
-00011970: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011980: 696d 732e 6e64 696d 203d 3d20 323a 0a20  ims.ndim == 2:. 
-00011990: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000119a0: 6469 6d20 3d20 7365 6c66 2e64 696d 732e  dim = self.dims.
-000119b0: 6765 7428 3029 0a20 2020 2020 2020 2020  get(0).         
-000119c0: 2020 2020 2020 2079 6469 6d20 3d20 7365         ydim = se
-000119d0: 6c66 2e64 696d 732e 6765 7428 3129 0a20  lf.dims.get(1). 
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000119f0: 616c 7565 7320 3d20 5b0a 2020 2020 2020  alues = [.      
-00011a00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011a10: 6c66 2e67 6574 5f6d 6574 6164 6174 615f  lf.get_metadata_
-00011a20: 7661 6c75 6573 286b 696e 643d 7864 696d  values(kind=xdim
-00011a30: 2e6b 696e 642c 206b 6579 3d78 6469 6d2e  .kind, key=xdim.
-00011a40: 6e61 6d65 292c 0a20 2020 2020 2020 2020  name),.         
-00011a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011a60: 6765 745f 6d65 7461 6461 7461 5f76 616c  get_metadata_val
-00011a70: 7565 7328 6b69 6e64 3d79 6469 6d2e 6b69  ues(kind=ydim.ki
-00011a80: 6e64 2c20 6b65 793d 7964 696d 2e6e 616d  nd, key=ydim.nam
-00011a90: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00011aa0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00011ab0: 2020 2020 2020 7368 6170 6520 3d20 5b78        shape = [x
-00011ac0: 6469 6d2e 7369 7a65 2c20 7964 696d 2e73  dim.size, ydim.s
-00011ad0: 697a 655d 0a20 2020 2020 2020 2020 2020  ize].           
-00011ae0: 2020 2020 205f 6669 7420 3d20 6669 745f       _fit = fit_
-00011af0: 3264 5f64 6174 610a 2020 2020 2020 2020  2d_data.        
-00011b00: 2020 2020 2020 2020 6461 7461 203d 2073          data = s
-00011b10: 656c 662e 6765 745f 6461 7461 2829 0a20  elf.get_data(). 
-00011b20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00011b30: 6170 7320 3d20 6e75 6d70 792e 656d 7074  aps = numpy.empt
-00011b40: 7928 2837 2c29 202b 2064 6174 615b 305d  y((7,) + data[0]
-00011b50: 2e73 6861 7065 290a 2020 2020 2020 2020  .shape).        
-00011b60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011b70: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00011b80: 2073 656c 662e 6765 745f 6461 7461 2869   self.get_data(i
-00011b90: 6e64 6963 6573 290a 2020 2020 2020 2020  ndices).        
-00011ba0: 2020 2020 2020 2020 5f66 6974 203d 2066          _fit = f
-00011bb0: 6974 5f64 6174 610a 2020 2020 2020 2020  it_data.        
-00011bc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011bd0: 6469 6d73 2e6e 6469 6d20 3e20 303a 0a20  dims.ndim > 0:. 
-00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bf0: 2020 2076 616c 7565 7320 3d20 7365 6c66     values = self
-00011c00: 2e67 6574 5f6d 6574 6164 6174 615f 7661  .get_metadata_va
-00011c10: 6c75 6573 280a 2020 2020 2020 2020 2020  lues(.          
-00011c20: 2020 2020 2020 2020 2020 2020 2020 6b69                ki
-00011c30: 6e64 3d73 656c 662e 6469 6d73 2e67 6574  nd=self.dims.get
-00011c40: 2830 292e 6b69 6e64 2c0a 2020 2020 2020  (0).kind,.      
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 6b65 793d 7365 6c66 2e64 696d 732e    key=self.dims.
-00011c70: 6765 7428 3029 2e6e 616d 652c 0a20 2020  get(0).name,.   
-00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c90: 2020 2020 2069 6e64 6963 6573 3d69 6e64       indices=ind
-00011ca0: 6963 6573 2c0a 2020 2020 2020 2020 2020  ices,.          
-00011cb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00011cc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00011cd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011ce0: 2020 2020 2020 7661 6c75 6573 203d 204e        values = N
-00011cf0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00011d00: 2020 2020 6d61 7073 203d 206e 756d 7079      maps = numpy
-00011d10: 2e65 6d70 7479 2828 342c 2920 2b20 6461  .empty((4,) + da
-00011d20: 7461 5b30 5d2e 7368 6170 6529 0a20 2020  ta[0].shape).   
-00011d30: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00011d40: 6461 7461 2e69 6e5f 6d65 6d6f 7279 3a0a  data.in_memory:.
-00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d60: 2320 5573 6520 6368 756e 6b73 2074 6f20  # Use chunks to 
-00011d70: 6c6f 6164 2074 6865 2064 6174 6120 696e  load the data in
-00011d80: 746f 206d 656d 6f72 790a 2020 2020 2020  to memory.      
-00011d90: 2020 2020 2020 2020 2020 7374 6172 7420            start 
-00011da0: 3d20 5b30 2c20 305d 0a20 2020 2020 2020  = [0, 0].       
-00011db0: 2020 2020 2020 2020 2063 6875 6e6b 735f           chunks_
-00011dc0: 3120 3d20 696e 7428 6e75 6d70 792e 6365  1 = int(numpy.ce
-00011dd0: 696c 2864 6174 612e 7368 6170 655b 315d  il(data.shape[1]
-00011de0: 202f 2063 6875 6e6b 5f73 6861 7065 5b30   / chunk_shape[0
-00011df0: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00011e00: 2020 2020 6368 756e 6b73 5f32 203d 2069      chunks_2 = i
-00011e10: 6e74 286e 756d 7079 2e63 6569 6c28 6461  nt(numpy.ceil(da
-00011e20: 7461 2e73 6861 7065 5b32 5d20 2f20 6368  ta.shape[2] / ch
-00011e30: 756e 6b5f 7368 6170 655b 315d 2929 0a20  unk_shape[1])). 
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011e50: 6d67 203d 206e 756d 7079 2e65 6d70 7479  mg = numpy.empty
-00011e60: 2828 6461 7461 2e73 6861 7065 5b31 5d2c  ((data.shape[1],
-00011e70: 2064 6174 612e 7368 6170 655b 325d 2929   data.shape[2]))
-00011e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e90: 2069 6f5f 7574 696c 732e 6164 7661 6e63   io_utils.advanc
-00011ea0: 656d 656e 745f 6469 7370 6c61 7928 0a20  ement_display(. 
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2030 2c20 6368 756e 6b73 5f31 202a     0, chunks_1 *
-00011ed0: 2063 6875 6e6b 735f 3220 2a20 6c65 6e28   chunks_2 * len(
-00011ee0: 6461 7461 292c 2022 4669 7474 696e 6720  data), "Fitting 
-00011ef0: 726f 636b 696e 6720 6375 7276 6573 220a  rocking curves".
-00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011f20: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00011f30: 2863 6875 6e6b 735f 3129 3a0a 2020 2020  (chunks_1):.    
-00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 666f 7220 6a20 696e 2072 616e 6765 2863  for j in range(c
-00011f60: 6875 6e6b 735f 3229 3a0a 2020 2020 2020  hunks_2):.      
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 6966 206e 6f74 2073 656c 662e 7374    if not self.st
-00011f90: 6174 655f 6f66 5f6f 7065 7261 7469 6f6e  ate_of_operation
-00011fa0: 732e 6973 5f72 756e 6e69 6e67 284f 7065  s.is_running(Ope
-00011fb0: 7261 7469 6f6e 2e46 4954 293a 0a20 2020  ration.FIT):.   
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ff0: 2020 2020 2020 2020 2320 5573 6520 6d75          # Use mu
-00012000: 6c74 6970 726f 6365 7373 696e 6720 746f  ltiprocessing to
-00012010: 2063 6875 6e6b 2074 6865 2069 6d61 6765   chunk the image
-00012020: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00012030: 2020 2020 2020 2020 2020 6370 7573 203d            cpus =
-00012040: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
-00012050: 2e63 7075 5f63 6f75 6e74 2829 0a20 2020  .cpu_count().   
-00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012070: 2020 2020 2077 6974 6820 506f 6f6c 2863       with Pool(c
-00012080: 7075 7320 2d20 3129 2061 7320 703a 0a20  pus - 1) as p:. 
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 2020 2020 2020 2063 5f69 6d61             c_ima
-000120b0: 6765 7320 3d20 702e 6d61 7028 0a20 2020  ges = p.map(.   
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-000120e0: 7469 616c 2863 6875 6e6b 5f69 6d61 6765  tial(chunk_image
-000120f0: 2c20 7374 6172 742c 2063 6875 6e6b 5f73  , start, chunk_s
-00012100: 6861 7065 292c 2064 6174 610a 2020 2020  hape), data.    
-00012110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012120: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 6669 7474 6564 5f64 6174 612c 2063    fitted_data, c
-00012150: 6875 6e6b 6564 5f6d 6170 7320 3d20 5f66  hunked_maps = _f
-00012160: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012180: 6e75 6d70 792e 6173 6172 7261 7928 635f  numpy.asarray(c_
-00012190: 696d 6167 6573 292c 0a20 2020 2020 2020  images),.       
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121b0: 2020 2020 2076 616c 7565 733d 7661 6c75       values=valu
-000121c0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 7368 6170 653d 7368 6170 652c 0a20 2020  shape=shape,.   
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-00012210: 3d69 6e64 6963 6573 2c0a 2020 2020 2020  =indices,.      
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 2020 2020 2020 696e 745f 7468 7265 7368        int_thresh
-00012240: 3d69 6e74 5f74 6872 6573 682c 0a20 2020  =int_thresh,.   
-00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012260: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00012270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012280: 6f72 206b 2069 6e20 7261 6e67 6528 6c65  or k in range(le
-00012290: 6e28 6669 7474 6564 5f64 6174 6129 293a  n(fitted_data)):
-000122a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000122b0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000122c0: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
-000122d0: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
+00011260: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00011270: 5b31 5d20 3a20 7374 6172 745b 315d 202b  [1] : start[1] +
+00011280: 2063 6875 6e6b 5f73 6861 7065 5b31 5d2c   chunk_shape[1],
+00011290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112a0: 2020 2020 2020 2020 205d 203d 2063 6f6d           ] = com
+000112b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112c0: 2020 2020 2020 2020 206d 6f6d 656e 7473           moments
+000112d0: 5b31 5d5b 0a20 2020 2020 2020 2020 2020  [1][.           
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2073 7461 7274 5b30 5d20 3a20 7374 6172   start[0] : star
+00011300: 745b 305d 202b 2063 6875 6e6b 5f73 6861  t[0] + chunk_sha
+00011310: 7065 5b30 5d2c 0a20 2020 2020 2020 2020  pe[0],.         
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 2073 7461 7274 5b31 5d20 3a20 7374     start[1] : st
+00011340: 6172 745b 315d 202b 2063 6875 6e6b 5f73  art[1] + chunk_s
+00011350: 6861 7065 5b31 5d2c 0a20 2020 2020 2020  hape[1],.       
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 205d 203d 2073 7464 0a20 2020 2020 2020   ] = std.       
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 206d 6f6d 656e 7473 5b32 5d5b 0a20 2020   moments[2][.   
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 2073 7461 7274 5b30           start[0
+000113c0: 5d20 3a20 7374 6172 745b 305d 202b 2063  ] : start[0] + c
+000113d0: 6875 6e6b 5f73 6861 7065 5b30 5d2c 0a20  hunk_shape[0],. 
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00011400: 5b31 5d20 3a20 7374 6172 745b 315d 202b  [1] : start[1] +
+00011410: 2063 6875 6e6b 5f73 6861 7065 5b31 5d2c   chunk_shape[1],
+00011420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011430: 2020 2020 2020 2020 205d 203d 2073 6b65           ] = ske
+00011440: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+00011450: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
+00011460: 735b 335d 5b0a 2020 2020 2020 2020 2020  s[3][.          
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2020 7374 6172 745b 305d 203a 2073 7461    start[0] : sta
+00011490: 7274 5b30 5d20 2b20 6368 756e 6b5f 7368  rt[0] + chunk_sh
+000114a0: 6170 655b 305d 2c0a 2020 2020 2020 2020  ape[0],.        
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2020 7374 6172 745b 315d 203a 2073      start[1] : s
+000114d0: 7461 7274 5b31 5d20 2b20 6368 756e 6b5f  tart[1] + chunk_
+000114e0: 7368 6170 655b 315d 2c0a 2020 2020 2020  shape[1],.      
+000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011500: 2020 5d20 3d20 6b75 7274 0a20 2020 2020    ] = kurt.     
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2073 7461 7274 5b31 5d20 3d20 6368     start[1] = ch
+00011530: 756e 6b5f 7368 6170 655b 315d 202a 2028  unk_shape[1] * (
+00011540: 6a20 2b20 3129 0a20 2020 2020 2020 2020  j + 1).         
+00011550: 2020 2020 2020 2020 2020 2073 7461 7274             start
+00011560: 5b30 5d20 3d20 6368 756e 6b5f 7368 6170  [0] = chunk_shap
+00011570: 655b 305d 202a 2028 6920 2b20 3129 0a20  e[0] * (i + 1). 
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2073 7461 7274 5b31 5d20 3d20 300a     start[1] = 0.
+000115a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000115b0: 2e6d 6f6d 656e 7473 5f64 696d 735b 6178  .moments_dims[ax
+000115c0: 6973 5d20 3d20 6d6f 6d65 6e74 730a 0a20  is] = moments.. 
+000115d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000115e0: 6c66 2e6d 6f6d 656e 7473 5f64 696d 730a  lf.moments_dims.
+000115f0: 0a20 2020 2064 6566 2061 7070 6c79 5f66  .    def apply_f
+00011600: 6974 280a 2020 2020 2020 2020 7365 6c66  it(.        self
+00011610: 2c20 696e 6469 6365 733d 4e6f 6e65 2c20  , indices=None, 
+00011620: 696e 745f 7468 7265 7368 3d4e 6f6e 652c  int_thresh=None,
+00011630: 2063 6875 6e6b 5f73 6861 7065 3d5b 3130   chunk_shape=[10
+00011640: 302c 2031 3030 5d2c 205f 6469 723d 4e6f  0, 100], _dir=No
+00011650: 6e65 0a20 2020 2029 3a0a 2020 2020 2020  ne.    ):.      
+00011660: 2020 2222 220a 2020 2020 2020 2020 4669    """.        Fi
+00011670: 7473 2074 6865 2064 6174 6120 6172 6f75  ts the data arou
+00011680: 6e64 2061 7869 7320 3020 616e 6420 7361  nd axis 0 and sa
+00011690: 7665 7320 7468 6520 6e65 7720 6461 7461  ves the new data
+000116a0: 2069 6e74 6f20 6469 736b 2e0a 0a20 2020   into disk...   
+000116b0: 2020 2020 203a 7061 7261 6d20 696e 6469       :param indi
+000116c0: 6365 733a 2049 6e64 6963 6573 206f 6620  ces: Indices of 
+000116d0: 7468 6520 696d 6167 6573 2074 6f20 6669  the images to fi
+000116e0: 742e 0a20 2020 2020 2020 2020 2020 2049  t..            I
+000116f0: 6620 4e6f 6e65 2c20 7468 6520 6669 7420  f None, the fit 
+00011700: 6973 2064 6f6e 6520 746f 2061 6c6c 2074  is done to all t
+00011710: 6865 2064 6174 612e 0a20 2020 2020 2020  he data..       
+00011720: 203a 7479 7065 2069 6e64 6963 6573 3a20   :type indices: 
+00011730: 556e 696f 6e5b 4e6f 6e65 2c20 6172 7261  Union[None, arra
+00011740: 795f 6c69 6b65 5d0a 2020 2020 2020 2020  y_like].        
+00011750: 3a70 6172 616d 2069 6e74 5f74 6872 6573  :param int_thres
+00011760: 683a 2073 6565 2060 6d61 7070 696e 672e  h: see `mapping.
+00011770: 6669 745f 7069 7865 6c60 0a20 2020 2020  fit_pixel`.     
+00011780: 2020 203a 7479 7065 2069 6e74 5f74 6872     :type int_thr
+00011790: 6573 683a 2055 6e69 6f6e 5b4e 6f6e 652c  esh: Union[None,
+000117a0: 2066 6c6f 6174 5d0a 2020 2020 2020 2020   float].        
+000117b0: 3a70 6172 616d 2063 6875 6e6b 5f73 6861  :param chunk_sha
+000117c0: 7065 3a20 5368 6170 6520 6f66 2074 6865  pe: Shape of the
+000117d0: 2063 6875 6e6b 2069 6d61 6765 2074 6f20   chunk image to 
+000117e0: 7573 6520 7065 7220 6974 6572 6174 696f  use per iteratio
+000117f0: 6e2e 0a20 2020 2020 2020 2020 2020 2050  n..            P
+00011800: 6172 616d 6574 6572 2075 7365 6420 6f6e  arameter used on
+00011810: 6c79 2077 6865 6e20 666c 6167 2069 6e5f  ly when flag in_
+00011820: 6d65 6d6f 7279 2069 7320 4661 6c73 652e  memory is False.
+00011830: 0a20 2020 2020 2020 203a 7479 7065 2063  .        :type c
+00011840: 6875 6e6b 5f73 6861 7065 3a20 6172 7261  hunk_shape: arra
+00011850: 795f 6c69 6b65 0a20 2020 2020 2020 203a  y_like.        :
+00011860: 7265 7475 726e 733a 2064 6174 6173 6574  returns: dataset
+00011870: 2077 6974 6820 6461 7461 206f 6620 7361   with data of sa
+00011880: 6d65 2073 697a 6520 6173 2060 7365 6c66  me size as `self
+00011890: 2e64 6174 6160 2062 7574 2077 6974 6820  .data` but with 
+000118a0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+000118b0: 6d6f 6469 6669 6564 2069 6d61 6765 732e  modified images.
+000118c0: 2054 6865 2075 726c 7320 6f66 2074 6865   The urls of the
+000118d0: 206d 6f64 6966 6965 6420 696d 6167 6573   modified images
+000118e0: 2061 7265 2072 6570 6c61 6365 6420 7769   are replaced wi
+000118f0: 7468 0a20 2020 2020 2020 2020 2020 2074  th.            t
+00011900: 6865 206e 6577 2075 726c 732e 0a20 2020  he new urls..   
+00011910: 2020 2020 203a 7274 7970 653a 2044 6174       :rtype: Dat
+00011920: 6173 6574 0a20 2020 2020 2020 2022 2222  aset.        """
+00011930: 0a0a 2020 2020 2020 2020 5f64 6972 203d  ..        _dir =
+00011940: 2073 656c 662e 6469 7220 6966 205f 6469   self.dir if _di
+00011950: 7220 6973 204e 6f6e 6520 656c 7365 205f  r is None else _
+00011960: 6469 720a 2020 2020 2020 2020 5f64 6972  dir.        _dir
+00011970: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00011980: 5f64 6972 2c20 2266 6974 2229 0a0a 2020  _dir, "fit")..  
+00011990: 2020 2020 2020 6f73 2e6d 616b 6564 6972        os.makedir
+000119a0: 7328 5f64 6972 2c20 6578 6973 745f 6f6b  s(_dir, exist_ok
+000119b0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+000119c0: 7769 7468 2073 656c 662e 7374 6174 655f  with self.state_
+000119d0: 6f66 5f6f 7065 7261 7469 6f6e 732e 7275  of_operations.ru
+000119e0: 6e5f 636f 6e74 6578 7428 4f70 6572 6174  n_context(Operat
+000119f0: 696f 6e2e 4649 5429 3a0a 2020 2020 2020  ion.FIT):.      
+00011a00: 2020 2020 2020 7572 6c73 203d 205b 5d0a        urls = [].
+00011a10: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00011a20: 6573 203d 204e 6f6e 650a 2020 2020 2020  es = None.      
+00011a30: 2020 2020 2020 7368 6170 6520 3d20 4e6f        shape = No
+00011a40: 6e65 0a20 2020 2020 2020 2020 2020 2064  ne.            d
+00011a50: 6174 6120 3d20 7365 6c66 2e67 6574 5f64  ata = self.get_d
+00011a60: 6174 6128 696e 6469 6365 7329 0a20 2020  ata(indices).   
+00011a70: 2020 2020 2020 2020 2023 2046 6974 2063           # Fit c
+00011a80: 616e 206f 6e6c 7920 6265 2064 6f6e 6520  an only be done 
+00011a90: 6966 2072 6f63 6b69 6e67 2063 7572 7665  if rocking curve
+00011aa0: 7320 6172 6520 6174 206c 6561 7374 206f  s are at least o
+00011ab0: 6620 7369 7a65 2033 0a20 2020 2020 2020  f size 3.       
+00011ac0: 2020 2020 2069 6620 6c65 6e28 6461 7461       if len(data
+00011ad0: 2920 3c20 333a 0a20 2020 2020 2020 2020  ) < 3:.         
+00011ae0: 2020 2020 2020 205f 6c6f 6767 6572 2e77         _logger.w
+00011af0: 6172 6e69 6e67 2822 4e6f 7420 656e 6f75  arning("Not enou
+00011b00: 6768 2076 616c 7565 7320 666f 7220 6669  gh values for fi
+00011b10: 7474 696e 6722 290a 2020 2020 2020 2020  tting").        
+00011b20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011b30: 656c 660a 2020 2020 2020 2020 2020 2020  elf.            
+00011b40: 6966 2069 6e64 6963 6573 2069 7320 4e6f  if indices is No
+00011b50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011b60: 2020 2020 696e 6469 6365 7320 3d20 7261      indices = ra
+00011b70: 6e67 6528 6461 7461 2e73 6861 7065 5b30  nge(data.shape[0
+00011b80: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+00011b90: 6966 2073 656c 662e 6469 6d73 2e6e 6469  if self.dims.ndi
+00011ba0: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
+00011bb0: 2020 2020 2020 2020 7864 696d 203d 2073          xdim = s
+00011bc0: 656c 662e 6469 6d73 2e67 6574 2830 290a  elf.dims.get(0).
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 7964 696d 203d 2073 656c 662e 6469 6d73  ydim = self.dims
+00011bf0: 2e67 6574 2831 290a 2020 2020 2020 2020  .get(1).        
+00011c00: 2020 2020 2020 2020 7661 6c75 6573 203d          values =
+00011c10: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00011c20: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
+00011c30: 6d65 7461 6461 7461 5f76 616c 7565 7328  metadata_values(
+00011c40: 6b69 6e64 3d78 6469 6d2e 6b69 6e64 2c20  kind=xdim.kind, 
+00011c50: 6b65 793d 7864 696d 2e6e 616d 6529 2c0a  key=xdim.name),.
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 7365 6c66 2e67 6574 5f6d 6574      self.get_met
+00011c80: 6164 6174 615f 7661 6c75 6573 286b 696e  adata_values(kin
+00011c90: 643d 7964 696d 2e6b 696e 642c 206b 6579  d=ydim.kind, key
+00011ca0: 3d79 6469 6d2e 6e61 6d65 292c 0a20 2020  =ydim.name),.   
+00011cb0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011cd0: 6861 7065 203d 205b 7864 696d 2e73 697a  hape = [xdim.siz
+00011ce0: 652c 2079 6469 6d2e 7369 7a65 5d0a 2020  e, ydim.size].  
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
+00011d00: 6974 203d 2066 6974 5f32 645f 6461 7461  it = fit_2d_data
+00011d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d20: 2064 6174 6120 3d20 7365 6c66 2e67 6574   data = self.get
+00011d30: 5f64 6174 6128 290a 2020 2020 2020 2020  _data().        
+00011d40: 2020 2020 2020 2020 6d61 7073 203d 206e          maps = n
+00011d50: 756d 7079 2e65 6d70 7479 2828 372c 2920  umpy.empty((7,) 
+00011d60: 2b20 6461 7461 5b30 5d2e 7368 6170 6529  + data[0].shape)
+00011d70: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00011d80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011d90: 2020 2064 6174 6120 3d20 7365 6c66 2e67     data = self.g
+00011da0: 6574 5f64 6174 6128 696e 6469 6365 7329  et_data(indices)
+00011db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011dc0: 205f 6669 7420 3d20 6669 745f 6461 7461   _fit = fit_data
+00011dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011de0: 2069 6620 7365 6c66 2e64 696d 732e 6e64   if self.dims.nd
+00011df0: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
+00011e00: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00011e10: 6573 203d 2073 656c 662e 6765 745f 6d65  es = self.get_me
+00011e20: 7461 6461 7461 5f76 616c 7565 7328 0a20  tadata_values(. 
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 2020 2020 2020 206b 696e 643d 7365 6c66         kind=self
+00011e50: 2e64 696d 732e 6765 7428 3029 2e6b 696e  .dims.get(0).kin
+00011e60: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00011e70: 2020 2020 2020 2020 2020 206b 6579 3d73             key=s
+00011e80: 656c 662e 6469 6d73 2e67 6574 2830 292e  elf.dims.get(0).
+00011e90: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00011ea0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00011eb0: 6469 6365 733d 696e 6469 6365 732c 0a20  dices=indices,. 
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00011ee0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00011f00: 616c 7565 7320 3d20 4e6f 6e65 0a20 2020  alues = None.   
+00011f10: 2020 2020 2020 2020 2020 2020 206d 6170               map
+00011f20: 7320 3d20 6e75 6d70 792e 656d 7074 7928  s = numpy.empty(
+00011f30: 2834 2c29 202b 2064 6174 615b 305d 2e73  (4,) + data[0].s
+00011f40: 6861 7065 290a 2020 2020 2020 2020 2020  hape).          
+00011f50: 2020 6966 206e 6f74 2064 6174 612e 696e    if not data.in
+00011f60: 5f6d 656d 6f72 793a 0a20 2020 2020 2020  _memory:.       
+00011f70: 2020 2020 2020 2020 2023 2055 7365 2063           # Use c
+00011f80: 6875 6e6b 7320 746f 206c 6f61 6420 7468  hunks to load th
+00011f90: 6520 6461 7461 2069 6e74 6f20 6d65 6d6f  e data into memo
+00011fa0: 7279 0a20 2020 2020 2020 2020 2020 2020  ry.             
+00011fb0: 2020 2073 7461 7274 203d 205b 302c 2030     start = [0, 0
+00011fc0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00011fd0: 2020 6368 756e 6b73 5f31 203d 2069 6e74    chunks_1 = int
+00011fe0: 286e 756d 7079 2e63 6569 6c28 6461 7461  (numpy.ceil(data
+00011ff0: 2e73 6861 7065 5b31 5d20 2f20 6368 756e  .shape[1] / chun
+00012000: 6b5f 7368 6170 655b 305d 2929 0a20 2020  k_shape[0])).   
+00012010: 2020 2020 2020 2020 2020 2020 2063 6875               chu
+00012020: 6e6b 735f 3220 3d20 696e 7428 6e75 6d70  nks_2 = int(nump
+00012030: 792e 6365 696c 2864 6174 612e 7368 6170  y.ceil(data.shap
+00012040: 655b 325d 202f 2063 6875 6e6b 5f73 6861  e[2] / chunk_sha
+00012050: 7065 5b31 5d29 290a 2020 2020 2020 2020  pe[1])).        
+00012060: 2020 2020 2020 2020 696d 6720 3d20 6e75          img = nu
+00012070: 6d70 792e 656d 7074 7928 2864 6174 612e  mpy.empty((data.
+00012080: 7368 6170 655b 315d 2c20 6461 7461 2e73  shape[1], data.s
+00012090: 6861 7065 5b32 5d29 290a 2020 2020 2020  hape[2])).      
+000120a0: 2020 2020 2020 2020 2020 696f 5f75 7469            io_uti
+000120b0: 6c73 2e61 6476 616e 6365 6d65 6e74 5f64  ls.advancement_d
+000120c0: 6973 706c 6179 280a 2020 2020 2020 2020  isplay(.        
+000120d0: 2020 2020 2020 2020 2020 2020 302c 2063              0, c
+000120e0: 6875 6e6b 735f 3120 2a20 6368 756e 6b73  hunks_1 * chunks
+000120f0: 5f32 202a 206c 656e 2864 6174 6129 2c20  _2 * len(data), 
+00012100: 2246 6974 7469 6e67 2072 6f63 6b69 6e67  "Fitting rocking
+00012110: 2063 7572 7665 7322 0a20 2020 2020 2020   curves".       
+00012120: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00012130: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00012140: 2069 6e20 7261 6e67 6528 6368 756e 6b73   in range(chunks
+00012150: 5f31 293a 0a20 2020 2020 2020 2020 2020  _1):.           
+00012160: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00012170: 6e20 7261 6e67 6528 6368 756e 6b73 5f32  n range(chunks_2
+00012180: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012190: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000121a0: 7420 7365 6c66 2e73 7461 7465 5f6f 665f  t self.state_of_
+000121b0: 6f70 6572 6174 696f 6e73 2e69 735f 7275  operations.is_ru
+000121c0: 6e6e 696e 6728 4f70 6572 6174 696f 6e2e  nning(Operation.
+000121d0: 4649 5429 3a0a 2020 2020 2020 2020 2020  FIT):.          
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2023 2055 7365 206d 756c 7469 7072 6f63   # Use multiproc
+00012220: 6573 7369 6e67 2074 6f20 6368 756e 6b20  essing to chunk 
+00012230: 7468 6520 696d 6167 6573 0a20 2020 2020  the images.     
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 2020 2063 7075 7320 3d20 6d75 6c74 6970     cpus = multip
+00012260: 726f 6365 7373 696e 672e 6370 755f 636f  rocessing.cpu_co
+00012270: 756e 7428 290a 2020 2020 2020 2020 2020  unt().          
+00012280: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00012290: 7468 2050 6f6f 6c28 6370 7573 202d 2031  th Pool(cpus - 1
+000122a0: 2920 6173 2070 3a0a 2020 2020 2020 2020  ) as p:.        
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2020 635f 696d 6167 6573 203d 2070      c_images = p
+000122d0: 2e6d 6170 280a 2020 2020 2020 2020 2020  .map(.          
 000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2020 2020 5f64 6972 2c20 2264 6174        _dir, "dat
-00012300: 615f 6669 745f 2220 2b20 7374 7228 696e  a_fit_" + str(in
-00012310: 6469 6365 735b 6b5d 292e 7a66 696c 6c28  dices[k]).zfill(
-00012320: 3429 202b 2022 2e6e 7079 220a 2020 2020  4) + ".npy".    
+000122f0: 2020 2020 2020 7061 7274 6961 6c28 6368        partial(ch
+00012300: 756e 6b5f 696d 6167 652c 2073 7461 7274  unk_image, start
+00012310: 2c20 6368 756e 6b5f 7368 6170 6529 2c20  , chunk_shape), 
+00012320: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
 00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012340: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012360: 2020 2020 2020 6966 2028 692c 206a 2920        if (i, j) 
-00012370: 213d 2028 302c 2030 293a 0a20 2020 2020  != (0, 0):.     
+00012340: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00012350: 2020 2020 2020 2020 2020 2066 6974 7465             fitte
+00012360: 645f 6461 7461 2c20 6368 756e 6b65 645f  d_data, chunked_
+00012370: 6d61 7073 203d 205f 6669 7428 0a20 2020  maps = _fit(.   
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-000123a0: 6368 756e 6b20 6973 206e 6f74 2074 6865  chunk is not the
-000123b0: 2066 6972 7374 2c20 6c6f 6164 2069 6d61   first, load ima
-000123c0: 6765 2066 726f 6d20 6469 736b 0a20 2020  ge from disk.   
-000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123e0: 2020 2020 2020 2020 2020 2020 2069 6d67               img
-000123f0: 203d 206e 756d 7079 2e6c 6f61 6428 6669   = numpy.load(fi
-00012400: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
+00012390: 2020 2020 2020 2020 206e 756d 7079 2e61           numpy.a
+000123a0: 7361 7272 6179 2863 5f69 6d61 6765 7329  sarray(c_images)
+000123b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000123c0: 2020 2020 2020 2020 2020 2020 2020 7661                va
+000123d0: 6c75 6573 3d76 616c 7565 732c 0a20 2020  lues=values,.   
+000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123f0: 2020 2020 2020 2020 2073 6861 7065 3d73           shape=s
+00012400: 6861 7065 2c0a 2020 2020 2020 2020 2020  hape,.          
 00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012420: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 2020 2020 2020 2020 2020 7572 6c73 2e61            urls.a
-00012450: 7070 656e 6428 4461 7461 5572 6c28 6669  ppend(DataUrl(fi
-00012460: 6c65 5f70 6174 683d 6669 6c65 6e61 6d65  le_path=filename
-00012470: 2c20 7363 6865 6d65 3d22 6661 6269 6f22  , scheme="fabio"
-00012480: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00012490: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000124a0: 6d67 5b0a 2020 2020 2020 2020 2020 2020  mg[.            
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 7374 6172 745b 305d 203a 2073      start[0] : s
-000124d0: 7461 7274 5b30 5d20 2b20 6368 756e 6b5f  tart[0] + chunk_
-000124e0: 7368 6170 655b 305d 2c0a 2020 2020 2020  shape[0],.      
+00012420: 2020 696e 6469 6365 733d 696e 6469 6365    indices=indice
+00012430: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00012440: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012450: 6e74 5f74 6872 6573 683d 696e 745f 7468  nt_thresh=int_th
+00012460: 7265 7368 2c0a 2020 2020 2020 2020 2020  resh,.          
+00012470: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012490: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+000124a0: 2072 616e 6765 286c 656e 2866 6974 7465   range(len(fitte
+000124b0: 645f 6461 7461 2929 3a0a 2020 2020 2020  d_data)):.      
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
+000124e0: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
 000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 2020 2020 2020 2020 2020 7374 6172 745b            start[
-00012510: 315d 203a 2073 7461 7274 5b31 5d20 2b20  1] : start[1] + 
-00012520: 6368 756e 6b5f 7368 6170 655b 315d 2c0a  chunk_shape[1],.
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2020 2020 2020 2020 2020 2020 5d20 3d20              ] = 
-00012550: 6669 7474 6564 5f64 6174 615b 6b5d 0a20  fitted_data[k]. 
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2020 2020 2020 2020 206e 756d 7079             numpy
-00012580: 2e73 6176 6528 6669 6c65 6e61 6d65 2c20  .save(filename, 
-00012590: 696d 6729 0a20 2020 2020 2020 2020 2020  img).           
+00012500: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00012510: 6469 722c 2022 6461 7461 5f66 6974 5f22  dir, "data_fit_"
+00012520: 202b 2073 7472 2869 6e64 6963 6573 5b6b   + str(indices[k
+00012530: 5d29 2e7a 6669 6c6c 2834 2920 2b20 222e  ]).zfill(4) + ".
+00012540: 6e70 7922 0a20 2020 2020 2020 2020 2020  npy".           
+00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012560: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00012570: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012580: 6620 2869 2c20 6a29 2021 3d20 2830 2c20  f (i, j) != (0, 
+00012590: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
 000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2069 6f5f 7574 696c 732e 6164 7661 6e63   io_utils.advanc
-000125c0: 656d 656e 745f 6469 7370 6c61 7928 0a20  ement_display(. 
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000125f0: 202a 2063 6875 6e6b 735f 3220 2a20 6c65   * chunks_2 * le
-00012600: 6e28 6461 7461 2920 2b20 6a20 2a20 6c65  n(data) + j * le
-00012610: 6e28 6461 7461 2920 2b20 6b20 2b20 312c  n(data) + k + 1,
+000125b0: 2020 2020 2320 4966 2063 6875 6e6b 2069      # If chunk i
+000125c0: 7320 6e6f 7420 7468 6520 6669 7273 742c  s not the first,
+000125d0: 206c 6f61 6420 696d 6167 6520 6672 6f6d   load image from
+000125e0: 2064 6973 6b0a 2020 2020 2020 2020 2020   disk.          
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 2020 2020 696d 6720 3d20 6e75 6d70        img = nump
+00012610: 792e 6c6f 6164 2866 696c 656e 616d 6529  y.load(filename)
 00012620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2063 6875 6e6b 735f 3120 2a20 6368 756e   chunks_1 * chun
-00012650: 6b73 5f32 202a 206c 656e 2864 6174 6129  ks_2 * len(data)
-00012660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2246 6974 7469 6e67 2072 6f63 6b69    "Fitting rocki
-00012690: 6e67 2063 7572 7665 7322 2c0a 2020 2020  ng curves",.    
+00012630: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00012640: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012660: 2020 2075 726c 732e 6170 7065 6e64 2844     urls.append(D
+00012670: 6174 6155 726c 2866 696c 655f 7061 7468  ataUrl(file_path
+00012680: 3d66 696c 656e 616d 652c 2073 6368 656d  =filename, schem
+00012690: 653d 2266 6162 696f 2229 290a 2020 2020  e="fabio")).    
 000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000126b0: 2020 2020 2020 2020 696d 675b 0a20 2020          img[.   
 000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 2020 6d61 7073 5b0a 2020 2020 2020 2020    maps[.        
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 2020 3a2c 0a20 2020 2020 2020 2020      :,.         
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2073 7461 7274 5b30 5d20 3a20 7374     start[0] : st
-00012720: 6172 745b 305d 202b 2063 6875 6e6b 5f73  art[0] + chunk_s
-00012730: 6861 7065 5b30 5d2c 0a20 2020 2020 2020  hape[0],.       
-00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012750: 2020 2020 2073 7461 7274 5b31 5d20 3a20       start[1] : 
-00012760: 7374 6172 745b 315d 202b 2063 6875 6e6b  start[1] + chunk
-00012770: 5f73 6861 7065 5b31 5d2c 0a20 2020 2020  _shape[1],.     
+000126d0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+000126e0: 7274 5b30 5d20 3a20 7374 6172 745b 305d  rt[0] : start[0]
+000126f0: 202b 2063 6875 6e6b 5f73 6861 7065 5b30   + chunk_shape[0
+00012700: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012720: 2020 2073 7461 7274 5b31 5d20 3a20 7374     start[1] : st
+00012730: 6172 745b 315d 202b 2063 6875 6e6b 5f73  art[1] + chunk_s
+00012740: 6861 7065 5b31 5d2c 0a20 2020 2020 2020  hape[1],.       
+00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012760: 2020 2020 205d 203d 2066 6974 7465 645f       ] = fitted_
+00012770: 6461 7461 5b6b 5d0a 2020 2020 2020 2020  data[k].        
 00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012790: 2020 205d 203d 2063 6875 6e6b 6564 5f6d     ] = chunked_m
-000127a0: 6170 730a 2020 2020 2020 2020 2020 2020  aps.            
-000127b0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-000127c0: 745b 315d 203d 2063 6875 6e6b 5f73 6861  t[1] = chunk_sha
-000127d0: 7065 5b31 5d20 2a20 286a 202b 2031 290a  pe[1] * (j + 1).
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 2020 7374 6172 745b 305d 203d 2063      start[0] = c
-00012800: 6875 6e6b 5f73 6861 7065 5b30 5d20 2a20  hunk_shape[0] * 
-00012810: 2869 202b 2031 290a 2020 2020 2020 2020  (i + 1).        
-00012820: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00012830: 745b 315d 203d 2030 0a20 2020 2020 2020  t[1] = 0.       
-00012840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012850: 2020 2020 2020 2020 2020 2066 6974 7465             fitte
-00012860: 645f 6461 7461 2c20 6d61 7073 203d 205f  d_data, maps = _
-00012870: 6669 7428 0a20 2020 2020 2020 2020 2020  fit(.           
-00012880: 2020 2020 2020 2020 2064 6174 612c 0a20           data,. 
-00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128a0: 2020 2076 616c 7565 733d 7661 6c75 6573     values=values
-000128b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000128c0: 2020 2020 2020 7368 6170 653d 7368 6170        shape=shap
-000128d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000128e0: 2020 2020 2020 2069 6e74 5f74 6872 6573         int_thres
-000128f0: 683d 696e 745f 7468 7265 7368 2c0a 2020  h=int_thresh,.  
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 696e 6469 6365 733d 696e 6469 6365    indices=indice
-00012920: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00012930: 2020 2020 2020 205f 7471 646d 3d54 7275         _tqdm=Tru
-00012940: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00012950: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012960: 2020 2020 2066 6f72 2069 2c20 696d 6167       for i, imag
-00012970: 6520 696e 2065 6e75 6d65 7261 7465 2866  e in enumerate(f
-00012980: 6974 7465 645f 6461 7461 293a 0a20 2020  itted_data):.   
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2066 696c 656e 616d 6520 3d20 6f73 2e70   filename = os.p
-000129b0: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
+00012790: 2020 2020 6e75 6d70 792e 7361 7665 2866      numpy.save(f
+000127a0: 696c 656e 616d 652c 2069 6d67 290a 2020  ilename, img).  
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2020 2020 696f 5f75 7469            io_uti
+000127d0: 6c73 2e61 6476 616e 6365 6d65 6e74 5f64  ls.advancement_d
+000127e0: 6973 706c 6179 280a 2020 2020 2020 2020  isplay(.        
+000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012800: 2020 2020 2020 2020 6920 2a20 6368 756e          i * chun
+00012810: 6b73 5f32 202a 206c 656e 2864 6174 6129  ks_2 * len(data)
+00012820: 202b 206a 202a 206c 656e 2864 6174 6129   + j * len(data)
+00012830: 202b 206b 202b 2031 2c0a 2020 2020 2020   + k + 1,.      
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 2020 2020 2020 2020 2020 6368 756e 6b73            chunks
+00012860: 5f31 202a 2063 6875 6e6b 735f 3220 2a20  _1 * chunks_2 * 
+00012870: 6c65 6e28 6461 7461 292c 0a20 2020 2020  len(data),.     
+00012880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012890: 2020 2020 2020 2020 2020 2022 4669 7474             "Fitt
+000128a0: 696e 6720 726f 636b 696e 6720 6375 7276  ing rocking curv
+000128b0: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128d0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000128e0: 2020 2020 2020 2020 2020 206d 6170 735b             maps[
+000128f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012900: 2020 2020 2020 2020 2020 2020 203a 2c0a               :,.
+00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012920: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00012930: 745b 305d 203a 2073 7461 7274 5b30 5d20  t[0] : start[0] 
+00012940: 2b20 6368 756e 6b5f 7368 6170 655b 305d  + chunk_shape[0]
+00012950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012960: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00012970: 6172 745b 315d 203a 2073 7461 7274 5b31  art[1] : start[1
+00012980: 5d20 2b20 6368 756e 6b5f 7368 6170 655b  ] + chunk_shape[
+00012990: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+000129a0: 2020 2020 2020 2020 2020 2020 5d20 3d20              ] = 
+000129b0: 6368 756e 6b65 645f 6d61 7073 0a20 2020  chunked_maps.   
 000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129d0: 2020 5f64 6972 2c20 2264 6174 615f 6669    _dir, "data_fi
-000129e0: 7422 202b 2073 7472 2869 6e64 6963 6573  t" + str(indices
-000129f0: 5b69 5d29 2e7a 6669 6c6c 2834 2920 2b20  [i]).zfill(4) + 
-00012a00: 222e 6e70 7922 0a20 2020 2020 2020 2020  ".npy".         
-00012a10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 206e 756d 7079 2e73 6176 6528 6669 6c65   numpy.save(file
-00012a40: 6e61 6d65 2c20 696d 6167 6529 0a20 2020  name, image).   
-00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a60: 2075 726c 732e 6170 7065 6e64 2844 6174   urls.append(Dat
-00012a70: 6155 726c 2866 696c 655f 7061 7468 3d66  aUrl(file_path=f
-00012a80: 696c 656e 616d 652c 2073 6368 656d 653d  ilename, scheme=
-00012a90: 2266 6162 696f 2229 290a 0a20 2020 2020  "fabio"))..     
-00012aa0: 2020 2069 6620 696e 6469 6365 7320 6973     if indices is
-00012ab0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00012ac0: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
-00012ad0: 206f 6e6c 7920 6669 7474 6564 2064 6174   only fitted dat
-00012ae0: 6120 7572 6c73 0a20 2020 2020 2020 2020  a urls.         
-00012af0: 2020 206e 6577 5f75 726c 7320 3d20 6e75     new_urls = nu
-00012b00: 6d70 792e 6172 7261 7928 7365 6c66 2e64  mpy.array(self.d
-00012b10: 6174 612e 7572 6c73 2c20 6474 7970 653d  ata.urls, dtype=
-00012b20: 6f62 6a65 6374 292e 666c 6174 7465 6e28  object).flatten(
-00012b30: 290a 2020 2020 2020 2020 2020 2020 6e75  ).            nu
-00012b40: 6d70 792e 7075 7428 6e65 775f 7572 6c73  mpy.put(new_urls
-00012b50: 2c20 696e 6469 6365 732c 2075 726c 7329  , indices, urls)
-00012b60: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00012b70: 2020 2020 2020 2020 2020 206e 6577 5f75             new_u
-00012b80: 726c 7320 3d20 6e75 6d70 792e 6172 7261  rls = numpy.arra
-00012b90: 7928 7572 6c73 290a 0a20 2020 2020 2020  y(urls)..       
-00012ba0: 2064 6174 6120 3d20 4461 7461 280a 2020   data = Data(.  
-00012bb0: 2020 2020 2020 2020 2020 6e65 775f 7572            new_ur
-00012bc0: 6c73 2e72 6573 6861 7065 2873 656c 662e  ls.reshape(self.
-00012bd0: 6461 7461 2e75 726c 732e 7368 6170 6529  data.urls.shape)
-00012be0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00012bf0: 6c66 2e64 6174 612e 6d65 7461 6461 7461  lf.data.metadata
-00012c00: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-00012c10: 5f6d 656d 6f72 793d 7365 6c66 2e5f 696e  _memory=self._in
-00012c20: 5f6d 656d 6f72 792c 0a20 2020 2020 2020  _memory,.       
-00012c30: 2029 2020 2320 746f 206d 6f64 6966 790a   )  # to modify.
-00012c40: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00012c50: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-00012c60: 6173 6574 280a 2020 2020 2020 2020 2020  aset(.          
-00012c70: 2020 2020 2020 5f64 6972 3d5f 6469 722c        _dir=_dir,
-00012c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c90: 2064 6174 613d 6461 7461 2c0a 2020 2020   data=data,.    
-00012ca0: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
-00012cb0: 3d73 656c 662e 5f5f 6469 6d73 2c0a 2020  =self.__dims,.  
-00012cc0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00012cd0: 616e 7366 6f72 6d61 7469 6f6e 3d73 656c  ansformation=sel
-00012ce0: 662e 7472 616e 7366 6f72 6d61 7469 6f6e  f.transformation
-00012cf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012d00: 2020 696e 5f6d 656d 6f72 793d 7365 6c66    in_memory=self
-00012d10: 2e5f 696e 5f6d 656d 6f72 792c 0a20 2020  ._in_memory,.   
-00012d20: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-00012d30: 6c65 3d73 656c 662e 7469 746c 652c 0a20  le=self.title,. 
-00012d40: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00012d50: 2020 2020 2020 2020 2020 6d61 7073 2c0a            maps,.
-00012d60: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00012d70: 6566 2063 6f6d 7075 7465 5f74 7261 6e73  ef compute_trans
-00012d80: 666f 726d 6174 696f 6e28 0a20 2020 2020  formation(.     
-00012d90: 2020 2073 656c 662c 2064 2c20 6b69 6e64     self, d, kind
-00012da0: 3d22 6d61 676e 6966 6963 6174 696f 6e22  ="magnification"
-00012db0: 2c20 726f 7461 7465 3d46 616c 7365 2c20  , rotate=False, 
-00012dc0: 746f 706f 6772 6170 6879 3d5b 4661 6c73  topography=[Fals
-00012dd0: 652c 2030 5d2c 2063 656e 7465 723d 5472  e, 0], center=Tr
-00012de0: 7565 0a20 2020 2029 3a0a 2020 2020 2020  ue.    ):.      
-00012df0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
-00012e00: 6d70 7574 6573 2074 7261 6e73 666f 726d  mputes transform
-00012e10: 6174 696f 6e20 6d61 7472 6978 2e0a 2020  ation matrix..  
-00012e20: 2020 2020 2020 4465 7065 6e64 696e 6720        Depending 
-00012e30: 6f6e 2074 6865 206b 696e 6420 6f66 2074  on the kind of t
-00012e40: 7261 6e73 666f 726d 6174 696f 6e2c 2063  ransformation, c
-00012e50: 6f6d 7075 7465 7320 6569 7468 6572 2052  omputes either R
-00012e60: 534d 206f 7220 6d61 676e 6966 6963 6174  SM or magnificat
-00012e70: 696f 6e0a 2020 2020 2020 2020 6178 6573  ion.        axes
-00012e80: 2074 6f20 6265 2075 7365 6420 6f6e 2066   to be used on f
-00012e90: 7574 7572 6520 7769 6467 6574 732e 0a0a  uture widgets...
-00012ea0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00012eb0: 3a20 5369 7a65 206f 6620 7468 6520 7069  : Size of the pi
-00012ec0: 7865 6c0a 2020 2020 2020 2020 3a74 7970  xel.        :typ
-00012ed0: 6520 643a 2066 6c6f 6174 0a20 2020 2020  e d: float.     
-00012ee0: 2020 203a 7061 7261 6d20 6b69 6e64 3a20     :param kind: 
-00012ef0: 5472 616e 7366 6f72 6d61 7469 6f6e 2074  Transformation t
-00012f00: 6f20 6170 706c 792c 2065 6974 6865 7220  o apply, either 
-00012f10: 276d 6167 6e69 6669 6361 7469 6f6e 2720  'magnification' 
-00012f20: 6f72 2027 7273 6d27 0a20 2020 2020 2020  or 'rsm'.       
-00012f30: 203a 7479 7065 206b 696e 643a 2073 7472   :type kind: str
-00012f40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012f50: 726f 7461 7465 3a20 546f 2062 6520 7573  rotate: To be us
-00012f60: 6564 206f 6e6c 7920 7769 7468 206b 696e  ed only with kin
-00012f70: 643d 2772 736d 272c 2069 6620 5472 7565  d='rsm', if True
-00012f80: 2074 6865 2069 6d61 6765 7320 7769 7468   the images with
-00012f90: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00012fa0: 6e73 666f 726d 6174 696f 6e20 6172 6520  nsformation are 
-00012fb0: 726f 7461 7465 6420 3930 2064 6567 7265  rotated 90 degre
-00012fc0: 6573 2e0a 2020 2020 2020 2020 3a74 7970  es..        :typ
-00012fd0: 6520 726f 7461 7465 3a20 626f 6f6c 0a20  e rotate: bool. 
-00012fe0: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
-00012ff0: 706f 6772 6170 6879 3a20 546f 2062 6520  pography: To be 
-00013000: 7573 6564 206f 6e6c 7920 7769 7468 206b  used only with k
-00013010: 696e 643d 276d 6167 6e69 6669 6361 7469  ind='magnificati
-00013020: 6f6e 272c 2069 6620 5472 7565 0a20 2020  on', if True.   
-00013030: 2020 2020 2020 2020 206f 6270 6974 6368           obpitch
-00013040: 2076 616c 7565 7320 6172 6520 6469 7669   values are divi
-00013050: 6465 6420 6279 2069 7473 2073 696e 652e  ded by its sine.
-00013060: 0a20 2020 2020 2020 203a 7479 7065 2074  .        :type t
-00013070: 6f70 6f67 7261 7068 793a 2062 6f6f 6c0a  opography: bool.
-00013080: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00013090: 2020 2020 2048 2c20 5720 3d20 7365 6c66       H, W = self
-000130a0: 2e67 6574 5f64 6174 6128 3029 2e73 6861  .get_data(0).sha
-000130b0: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-000130c0: 726f 7461 7465 203d 2072 6f74 6174 650a  rotate = rotate.
-000130d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000130e0: 2e64 696d 732e 6e64 696d 203d 3d20 3120  .dims.ndim == 1 
-000130f0: 616e 6420 6b69 6e64 203d 3d20 2272 736d  and kind == "rsm
-00013100: 223a 0a20 2020 2020 2020 2020 2020 2066  ":.            f
-00013110: 667a 203d 2073 656c 662e 6765 745f 6d65  fz = self.get_me
-00013120: 7461 6461 7461 5f76 616c 7565 7328 504f  tadata_values(PO
-00013130: 5349 5449 4f4e 4552 5f4d 4554 4144 4154  SITIONER_METADAT
-00013140: 412c 2022 6666 7a22 295b 305d 0a20 2020  A, "ffz")[0].   
-00013150: 2020 2020 2020 2020 206d 6169 6e78 203d           mainx =
-00013160: 202d 7365 6c66 2e67 6574 5f6d 6574 6164   -self.get_metad
-00013170: 6174 615f 7661 6c75 6573 2850 4f53 4954  ata_values(POSIT
-00013180: 494f 4e45 525f 4d45 5441 4441 5441 2c20  IONER_METADATA, 
-00013190: 226d 6169 6e78 2229 5b30 5d0a 2020 2020  "mainx")[0].    
-000131a0: 2020 2020 2020 2020 782c 2079 203d 2063          x, y = c
-000131b0: 6f6d 7075 7465 5f72 736d 2848 2c20 572c  ompute_rsm(H, W,
-000131c0: 2064 2c20 6666 7a2c 206d 6169 6e78 2c20   d, ffz, mainx, 
-000131d0: 726f 7461 7465 290a 2020 2020 2020 2020  rotate).        
-000131e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000131f0: 2020 6f62 7820 3d20 7365 6c66 2e67 6574    obx = self.get
-00013200: 5f6d 6574 6164 6174 615f 7661 6c75 6573  _metadata_values
-00013210: 2850 4f53 4954 494f 4e45 525f 4d45 5441  (POSITIONER_META
-00013220: 4441 5441 2c20 226f 6278 2229 5b30 5d0a  DATA, "obx")[0].
-00013230: 2020 2020 2020 2020 2020 2020 6f62 7069              obpi
-00013240: 7463 6820 3d20 6e75 6d70 792e 756e 6971  tch = numpy.uniq
-00013250: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-00013260: 2020 2020 7365 6c66 2e67 6574 5f6d 6574      self.get_met
-00013270: 6164 6174 615f 7661 6c75 6573 2850 4f53  adata_values(POS
-00013280: 4954 494f 4e45 525f 4d45 5441 4441 5441  ITIONER_METADATA
-00013290: 2c20 226f 6270 6974 6368 2229 0a20 2020  , "obpitch").   
-000132a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000132b0: 2020 2020 2020 206f 6270 6974 6368 203d         obpitch =
-000132c0: 206f 6270 6974 6368 5b6c 656e 286f 6270   obpitch[len(obp
-000132d0: 6974 6368 2920 2f2f 2032 5d0a 2020 2020  itch) // 2].    
-000132e0: 2020 2020 2020 2020 6d61 696e 7820 3d20          mainx = 
-000132f0: 2d73 656c 662e 6765 745f 6d65 7461 6461  -self.get_metada
-00013300: 7461 5f76 616c 7565 7328 504f 5349 5449  ta_values(POSITI
-00013310: 4f4e 4552 5f4d 4554 4144 4154 412c 2022  ONER_METADATA, "
-00013320: 6d61 696e 7822 295b 305d 0a20 2020 2020  mainx")[0].     
-00013330: 2020 2020 2020 2078 2c20 7920 3d20 636f         x, y = co
-00013340: 6d70 7574 655f 6d61 676e 6966 6963 6174  mpute_magnificat
-00013350: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00013360: 2020 2020 2048 2c20 572c 2064 2c20 6f62       H, W, d, ob
-00013370: 782c 206f 6270 6974 6368 2c20 6d61 696e  x, obpitch, main
-00013380: 782c 2074 6f70 6f67 7261 7068 792c 2063  x, topography, c
-00013390: 656e 7465 720a 2020 2020 2020 2020 2020  enter.          
-000133a0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-000133b0: 2e74 7261 6e73 666f 726d 6174 696f 6e20  .transformation 
-000133c0: 3d20 5472 616e 7366 6f72 6d61 7469 6f6e  = Transformation
-000133d0: 286b 696e 642c 2078 2c20 792c 2072 6f74  (kind, x, y, rot
-000133e0: 6174 6529 0a0a 2020 2020 6465 6620 7072  ate)..    def pr
-000133f0: 6f6a 6563 745f 6461 7461 2873 656c 662c  oject_data(self,
-00013400: 2064 696d 656e 7369 6f6e 2c20 696e 6469   dimension, indi
-00013410: 6365 733d 4e6f 6e65 2c20 5f64 6972 3d4e  ces=None, _dir=N
-00013420: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-00013430: 220a 2020 2020 2020 2020 4170 706c 6965  ".        Applie
-00013440: 7320 6120 7072 6f6a 6563 7469 6f6e 2074  s a projection t
-00013450: 6f20 7468 6520 6461 7461 2e0a 2020 2020  o the data..    
-00013460: 2020 2020 5468 6520 6e65 7720 4461 7461      The new Data
-00013470: 7365 7420 7769 6c6c 2068 6176 6520 7468  set will have th
-00013480: 6520 7361 6d65 2073 697a 6520 6173 2074  e same size as t
-00013490: 6865 2063 686f 7365 6e20 6469 6d65 6e73  he chosen dimens
-000134a0: 696f 6e2c 2077 6865 7265 0a20 2020 2020  ion, where.     
-000134b0: 2020 2074 6865 2064 6174 6120 6973 2070     the data is p
-000134c0: 726f 6a65 6374 6564 206f 6e2e 0a0a 2020  rojected on...  
-000134d0: 2020 2020 2020 3a70 6172 616d 2064 696d        :param dim
-000134e0: 656e 7369 6f6e 3a20 4469 6d65 6e73 696f  ension: Dimensio
-000134f0: 6e73 2074 6f20 7072 6f6a 6563 7420 7468  ns to project th
-00013500: 6520 6461 7461 206f 6e74 6f0a 2020 2020  e data onto.    
-00013510: 2020 2020 3a74 7970 6520 6469 6d65 6e73      :type dimens
-00013520: 696f 6e3a 2061 7272 6179 5f6c 696b 650a  ion: array_like.
-00013530: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00013540: 6e64 6963 6573 3a20 496e 6469 6365 7320  ndices: Indices 
-00013550: 6f66 2074 6865 2069 6d61 6765 7320 746f  of the images to
-00013560: 2075 7365 2066 6f72 2074 6865 2070 726f   use for the pro
-00013570: 6a65 6374 696f 6e2e 0a20 2020 2020 2020  jection..       
-00013580: 2020 2020 2049 6620 4e6f 6e65 2c20 7468       If None, th
-00013590: 6520 7072 6f6a 6563 7469 6f6e 2069 7320  e projection is 
-000135a0: 646f 6e65 2075 7369 6e67 2061 6c6c 2064  done using all d
-000135b0: 6174 612e 0a20 2020 2020 2020 203a 7479  ata..        :ty
-000135c0: 7065 2069 6e64 6963 6573 3a20 556e 696f  pe indices: Unio
-000135d0: 6e5b 4e6f 6e65 2c20 6172 7261 795f 6c69  n[None, array_li
-000135e0: 6b65 5d0a 2020 2020 2020 2020 3a70 6172  ke].        :par
-000135f0: 616d 2073 7472 205f 6469 723a 2044 6972  am str _dir: Dir
-00013600: 6563 746f 7279 2066 696c 656e 616d 6520  ectory filename 
-00013610: 746f 2073 6176 6520 7468 6520 6e65 7720  to save the new 
-00013620: 6461 7461 0a20 2020 2020 2020 2022 2222  data.        """
-00013630: 0a0a 2020 2020 2020 2020 5f64 6972 203d  ..        _dir =
-00013640: 2073 656c 662e 6469 7220 6966 205f 6469   self.dir if _di
-00013650: 7220 6973 204e 6f6e 6520 656c 7365 205f  r is None else _
-00013660: 6469 720a 2020 2020 2020 2020 6f73 2e6d  dir.        os.m
-00013670: 616b 6564 6972 7328 5f64 6972 2c20 6578  akedirs(_dir, ex
-00013680: 6973 745f 6f6b 3d54 7275 6529 0a0a 2020  ist_ok=True)..  
-00013690: 2020 2020 2020 6469 6d73 203d 2041 6371        dims = Acq
-000136a0: 7569 7369 7469 6f6e 4469 6d73 2829 0a20  uisitionDims(). 
-000136b0: 2020 2020 2020 2069 6620 6c65 6e28 6469         if len(di
-000136c0: 6d65 6e73 696f 6e29 203d 3d20 313a 0a20  mension) == 1:. 
-000136d0: 2020 2020 2020 2020 2020 2061 7869 7320             axis 
-000136e0: 3d20 7365 6c66 2e64 696d 732e 6e64 696d  = self.dims.ndim
-000136f0: 202d 2064 696d 656e 7369 6f6e 5b30 5d20   - dimension[0] 
-00013700: 2d20 310a 2020 2020 2020 2020 2020 2020  - 1.            
-00013710: 6469 6d20 3d20 7365 6c66 2e64 696d 732e  dim = self.dims.
-00013720: 6765 7428 6469 6d65 6e73 696f 6e5b 305d  get(dimension[0]
-00013730: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
-00013740: 7461 203d 205b 5d0a 2020 2020 2020 2020  ta = [].        
-00013750: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00013760: 6765 2864 696d 2e73 697a 6529 3a0a 2020  ge(dim.size):.  
-00013770: 2020 2020 2020 2020 2020 2020 2020 5f73                _s
-00013780: 756d 203d 2073 656c 662e 7a73 756d 2869  um = self.zsum(i
-00013790: 6e64 6963 6573 3d69 6e64 6963 6573 2c20  ndices=indices, 
-000137a0: 6469 6d65 6e73 696f 6e3d 5b64 696d 656e  dimension=[dimen
-000137b0: 7369 6f6e 5b30 5d2c 2069 5d29 0a20 2020  sion[0], i]).   
-000137c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000137d0: 6c65 6e28 5f73 756d 293a 0a20 2020 2020  len(_sum):.     
-000137e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000137f0: 6174 6120 2b3d 205b 5f73 756d 5d0a 2020  ata += [_sum].  
-00013800: 2020 2020 2020 2020 2020 6469 6d73 2e61            dims.a
-00013810: 6464 5f64 696d 2830 2c20 6469 6d29 0a20  dd_dim(0, dim). 
-00013820: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
-00013830: 6469 6d65 6e73 696f 6e29 203d 3d20 323a  dimension) == 2:
-00013840: 0a20 2020 2020 2020 2020 2020 2061 7869  .            axi
-00013850: 7320 3d20 696e 7428 6e75 6d70 792e 7365  s = int(numpy.se
-00013860: 7464 6966 6631 6428 7261 6e67 6528 7365  tdiff1d(range(se
-00013870: 6c66 2e64 696d 732e 6e64 696d 292c 2064  lf.dims.ndim), d
-00013880: 696d 656e 7369 6f6e 295b 305d 290a 2020  imension)[0]).  
-00013890: 2020 2020 2020 2020 2020 6469 6d31 203d            dim1 =
-000138a0: 2073 656c 662e 6469 6d73 2e67 6574 2864   self.dims.get(d
-000138b0: 696d 656e 7369 6f6e 5b30 5d29 0a20 2020  imension[0]).   
-000138c0: 2020 2020 2020 2020 2064 696d 3220 3d20           dim2 = 
-000138d0: 7365 6c66 2e64 696d 732e 6765 7428 6469  self.dims.get(di
-000138e0: 6d65 6e73 696f 6e5b 315d 290a 2020 2020  mension[1]).    
-000138f0: 2020 2020 2020 2020 6469 6d73 2e61 6464          dims.add
-00013900: 5f64 696d 2830 2c20 6469 6d31 290a 2020  _dim(0, dim1).  
-00013910: 2020 2020 2020 2020 2020 6469 6d73 2e61            dims.a
-00013920: 6464 5f64 696d 2831 2c20 6469 6d32 290a  dd_dim(1, dim2).
-00013930: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00013940: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00013950: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00013960: 2864 696d 312e 7369 7a65 293a 0a20 2020  (dim1.size):.   
-00013970: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00013980: 206a 2069 6e20 7261 6e67 6528 6469 6d32   j in range(dim2
-00013990: 2e73 697a 6529 3a0a 2020 2020 2020 2020  .size):.        
-000139a0: 2020 2020 2020 2020 2020 2020 5f73 756d              _sum
-000139b0: 203d 2073 656c 662e 7a73 756d 2869 6e64   = self.zsum(ind
-000139c0: 6963 6573 3d69 6e64 6963 6573 2c20 6469  ices=indices, di
-000139d0: 6d65 6e73 696f 6e3d 5b64 696d 656e 7369  mension=[dimensi
-000139e0: 6f6e 2c20 5b69 2c20 6a5d 5d29 0a20 2020  on, [i, j]]).   
-000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a00: 2069 6620 6c65 6e28 5f73 756d 293a 0a20   if len(_sum):. 
-00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a20: 2020 2020 2020 2064 6174 6120 2b3d 205b         data += [
-00013a30: 5f73 756d 5d0a 2020 2020 2020 2020 656c  _sum].        el
-00013a40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00013a50: 7265 7475 726e 2056 616c 7565 4572 726f  return ValueErro
-00013a60: 7228 224f 6e6c 7920 3144 2061 6e64 2032  r("Only 1D and 2
-00013a70: 4420 7072 6f6a 6563 7469 6f6e 2069 7320  D projection is 
-00013a80: 616c 6c6f 7765 6422 290a 2020 2020 2020  allowed").      
-00013a90: 2020 6469 6d20 3d20 7365 6c66 2e64 696d    dim = self.dim
-00013aa0: 732e 6765 7428 6178 6973 290a 2020 2020  s.get(axis).    
-00013ab0: 2020 2020 6461 7461 203d 206e 756d 7079      data = numpy
-00013ac0: 2e61 7272 6179 2864 6174 6129 2e76 6965  .array(data).vie
-00013ad0: 7728 4461 7461 290a 2020 2020 2020 2020  w(Data).        
-00013ae0: 6d65 7461 6461 7461 203d 206e 756d 7079  metadata = numpy
-00013af0: 2e73 7761 7061 7865 7328 7365 6c66 2e64  .swapaxes(self.d
-00013b00: 6174 612e 6d65 7461 6461 7461 2c20 7365  ata.metadata, se
-00013b10: 6c66 2e64 696d 732e 6e64 696d 202d 2031  lf.dims.ndim - 1
-00013b20: 2c20 6178 6973 290a 2020 2020 2020 2020  , axis).        
-00013b30: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
-00013b40: 656c 662e 6469 6d73 2e6e 6469 6d20 2d20  elf.dims.ndim - 
-00013b50: 6c65 6e28 6469 6d65 6e73 696f 6e29 293a  len(dimension)):
-00013b60: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00013b70: 6164 6174 6120 3d20 6d65 7461 6461 7461  adata = metadata
-00013b80: 5b30 5d0a 2020 2020 2020 2020 6461 7461  [0].        data
-00013b90: 2e73 6176 6528 0a20 2020 2020 2020 2020  .save(.         
-00013ba0: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
-00013bb0: 5f64 6972 2c20 2270 726f 6a65 6374 5f22  _dir, "project_"
-00013bc0: 202b 2064 696d 2e6e 616d 6520 2b20 222e   + dim.name + ".
-00013bd0: 6864 6635 2229 2c0a 2020 2020 2020 2020  hdf5"),.        
-00013be0: 2020 2020 696e 5f6d 656d 6f72 793d 7365      in_memory=se
-00013bf0: 6c66 2e5f 696e 5f6d 656d 6f72 792c 0a20  lf._in_memory,. 
-00013c00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00013c10: 2064 6174 612e 6d65 7461 6461 7461 203d   data.metadata =
-00013c20: 206d 6574 6164 6174 610a 0a20 2020 2020   metadata..     
-00013c30: 2020 2064 6174 6173 6574 203d 2044 6174     dataset = Dat
-00013c40: 6173 6574 280a 2020 2020 2020 2020 2020  aset(.          
-00013c50: 2020 5f64 6972 3d5f 6469 722c 0a20 2020    _dir=_dir,.   
-00013c60: 2020 2020 2020 2020 2064 6174 613d 6461           data=da
-00013c70: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00013c80: 6469 6d73 3d64 696d 732c 0a20 2020 2020  dims=dims,.     
-00013c90: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00013ca0: 6174 696f 6e3d 7365 6c66 2e74 7261 6e73  ation=self.trans
-00013cb0: 666f 726d 6174 696f 6e2c 0a20 2020 2020  formation,.     
-00013cc0: 2020 2020 2020 2069 6e5f 6d65 6d6f 7279         in_memory
-00013cd0: 3d73 656c 662e 5f69 6e5f 6d65 6d6f 7279  =self._in_memory
-00013ce0: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00013cf0: 746c 653d 7365 6c66 2e74 6974 6c65 2c0a  tle=self.title,.
-00013d00: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00013d10: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
-00013d20: 742e 7265 7368 6170 655f 6461 7461 2829  t.reshape_data()
-00013d30: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
-00013d40: 655f 7273 6d28 0a20 2020 2020 2020 2073  e_rsm(.        s
-00013d50: 656c 662c 0a20 2020 2020 2020 2051 2c0a  elf,.        Q,.
-00013d60: 2020 2020 2020 2020 612c 0a20 2020 2020          a,.     
-00013d70: 2020 206d 6170 5f72 616e 6765 2c0a 2020     map_range,.  
-00013d80: 2020 2020 2020 7069 7865 6c5f 7369 7a65        pixel_size
-00013d90: 2c0a 2020 2020 2020 2020 756e 6974 732c  ,.        units,
-00013da0: 0a20 2020 2020 2020 206e 2c0a 2020 2020  .        n,.    
-00013db0: 2020 2020 6d61 705f 7368 6170 652c 0a20      map_shape,. 
-00013dc0: 2020 2020 2020 2065 6e65 7267 793d 3137         energy=17
-00013dd0: 2c0a 2020 2020 2020 2020 7472 616e 7366  ,.        transf
-00013de0: 6f72 6d61 7469 6f6e 3d4e 6f6e 652c 0a20  ormation=None,. 
-00013df0: 2020 2029 3a0a 2020 2020 2020 2020 6469     ):.        di
-00013e00: 6666 7279 203d 2073 656c 662e 6765 745f  ffry = self.get_
-00013e10: 6d65 7461 6461 7461 5f76 616c 7565 7328  metadata_values(
-00013e20: 504f 5349 5449 4f4e 4552 5f4d 4554 4144  POSITIONER_METAD
-00013e30: 4154 412c 2022 6469 6666 7279 2229 0a20  ATA, "diffry"). 
-00013e40: 2020 2020 2020 2069 6620 7472 616e 7366         if transf
-00013e50: 6f72 6d61 7469 6f6e 2069 7320 4e6f 6e65  ormation is None
-00013e60: 2061 6e64 2073 656c 662e 7472 616e 7366   and self.transf
-00013e70: 6f72 6d61 7469 6f6e 2069 7320 6e6f 7420  ormation is not 
-00013e80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013e90: 2020 7472 616e 7366 6f72 6d61 7469 6f6e    transformation
-00013ea0: 203d 2073 656c 662e 7472 616e 7366 6f72   = self.transfor
-00013eb0: 6d61 7469 6f6e 0a20 2020 2020 2020 2065  mation.        e
-00013ec0: 6c69 6620 7365 6c66 2e74 7261 6e73 666f  lif self.transfo
-00013ed0: 726d 6174 696f 6e20 6973 204e 6f6e 653a  rmation is None:
-00013ee0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00013ef0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00013f00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013f10: 5472 616e 7366 6f72 6d61 7469 6f6e 2068  Transformation h
-00013f20: 6173 2074 6f20 6669 7273 7420 6265 2063  as to first be c
-00013f30: 6f6d 7075 7465 6420 7573 696e 6720 7468  omputed using th
-00013f40: 6520 5472 616e 7366 6f72 6d61 7469 6f6e  e Transformation
-00013f50: 2057 6964 6765 7420 2862 6566 6f72 6520   Widget (before 
-00013f60: 616e 7920 524f 4929 220a 2020 2020 2020  any ROI)".      
-00013f70: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00013f80: 2072 6574 7572 6e20 6361 6c63 756c 6174   return calculat
-00013f90: 655f 5253 4d5f 6869 7374 6f67 7261 6d28  e_RSM_histogram(
-00013fa0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00013fb0: 613d 7365 6c66 2e67 6574 5f64 6174 6128  a=self.get_data(
-00013fc0: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
-00013fd0: 6966 6672 795f 7661 6c75 6573 3d64 6966  iffry_values=dif
-00013fe0: 6672 792c 0a20 2020 2020 2020 2020 2020  fry,.           
-00013ff0: 2074 776f 7468 6574 613d 7472 616e 7366   twotheta=transf
-00014000: 6f72 6d61 7469 6f6e 2e79 2c0a 2020 2020  ormation.y,.    
-00014010: 2020 2020 2020 2020 6574 613d 7472 616e          eta=tran
-00014020: 7366 6f72 6d61 7469 6f6e 2e78 2c0a 2020  sformation.x,.  
-00014030: 2020 2020 2020 2020 2020 513d 512c 0a20            Q=Q,. 
-00014040: 2020 2020 2020 2020 2020 2061 3d61 2c0a             a=a,.
-00014050: 2020 2020 2020 2020 2020 2020 6d61 705f              map_
-00014060: 7261 6e67 653d 6d61 705f 7261 6e67 652c  range=map_range,
-00014070: 0a20 2020 2020 2020 2020 2020 2075 6e69  .            uni
-00014080: 7473 3d75 6e69 7473 2c0a 2020 2020 2020  ts=units,.      
-00014090: 2020 2020 2020 6d61 705f 7368 6170 653d        map_shape=
-000140a0: 6d61 705f 7368 6170 652c 0a20 2020 2020  map_shape,.     
-000140b0: 2020 2020 2020 206e 3d6e 2c0a 2020 2020         n=n,.    
-000140c0: 2020 2020 2020 2020 453d 656e 6572 6779          E=energy
-000140d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000140e0: 2064 6566 2061 7070 6c79 5f62 696e 6e69   def apply_binni
-000140f0: 6e67 2873 656c 662c 2073 6361 6c65 2c20  ng(self, scale, 
-00014100: 5f64 6972 3d4e 6f6e 6529 3a0a 2020 2020  _dir=None):.    
-00014110: 2020 2020 5f64 6972 203d 2073 656c 662e      _dir = self.
-00014120: 6469 7220 6966 205f 6469 7220 6973 204e  dir if _dir is N
-00014130: 6f6e 6520 656c 7365 205f 6469 720a 2020  one else _dir.  
-00014140: 2020 2020 2020 6f73 2e6d 616b 6564 6972        os.makedir
-00014150: 7328 5f64 6972 2c20 6578 6973 745f 6f6b  s(_dir, exist_ok
-00014160: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-00014170: 6461 7461 203d 2072 6573 6361 6c65 5f64  data = rescale_d
-00014180: 6174 6128 7365 6c66 2e67 6574 5f64 6174  ata(self.get_dat
-00014190: 6128 292c 2073 6361 6c65 290a 2020 2020  a(), scale).    
-000141a0: 2020 2020 7368 6170 6520 3d20 6461 7461      shape = data
-000141b0: 2e73 6861 7065 0a20 2020 2020 2020 2064  .shape.        d
-000141c0: 6174 6120 3d20 6461 7461 2e76 6965 7728  ata = data.view(
-000141d0: 4461 7461 290a 2020 2020 2020 2020 6461  Data).        da
-000141e0: 7461 2e73 6176 6528 0a20 2020 2020 2020  ta.save(.       
-000141f0: 2020 2020 206f 732e 7061 7468 2e6a 6f69       os.path.joi
-00014200: 6e28 5f64 6972 2c20 2262 696e 6e65 645f  n(_dir, "binned_
-00014210: 6461 7461 2e68 6466 3522 292c 0a20 2020  data.hdf5"),.   
-00014220: 2020 2020 2020 2020 2069 6e5f 6d65 6d6f           in_memo
-00014230: 7279 3d73 656c 662e 5f69 6e5f 6d65 6d6f  ry=self._in_memo
-00014240: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-00014250: 6e65 775f 7368 6170 653d 7368 6170 652c  new_shape=shape,
-00014260: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00014270: 2020 2064 6174 612e 6d65 7461 6461 7461     data.metadata
-00014280: 203d 2073 656c 662e 6461 7461 2e6d 6574   = self.data.met
-00014290: 6164 6174 610a 2020 2020 2020 2020 7368  adata.        sh
-000142a0: 6170 6520 3d20 6c69 7374 2873 656c 662e  ape = list(self.
-000142b0: 6461 7461 2e73 6861 7065 295b 3a2d 325d  data.shape)[:-2]
-000142c0: 0a20 2020 2020 2020 2073 6861 7065 2e61  .        shape.a
-000142d0: 7070 656e 6428 6461 7461 2e73 6861 7065  ppend(data.shape
-000142e0: 5b2d 325d 290a 2020 2020 2020 2020 7368  [-2]).        sh
-000142f0: 6170 652e 6170 7065 6e64 2864 6174 612e  ape.append(data.
-00014300: 7368 6170 655b 2d31 5d29 0a20 2020 2020  shape[-1]).     
-00014310: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-00014320: 6573 6861 7065 2873 6861 7065 290a 0a20  eshape(shape).. 
-00014330: 2020 2020 2020 2072 6574 7572 6e20 4461         return Da
-00014340: 7461 7365 7428 0a20 2020 2020 2020 2020  taset(.         
-00014350: 2020 205f 6469 723d 5f64 6972 2c0a 2020     _dir=_dir,.  
-00014360: 2020 2020 2020 2020 2020 6461 7461 3d64            data=d
-00014370: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00014380: 2064 696d 733d 7365 6c66 2e64 696d 732c   dims=self.dims,
-00014390: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-000143a0: 6e73 666f 726d 6174 696f 6e3d 7365 6c66  nsformation=self
-000143b0: 2e74 7261 6e73 666f 726d 6174 696f 6e2c  .transformation,
-000143c0: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
-000143d0: 6d65 6d6f 7279 3d54 7275 652c 0a20 2020  memory=True,.   
-000143e0: 2020 2020 2020 2020 2074 6974 6c65 3d73           title=s
-000143f0: 656c 662e 7469 746c 652c 0a20 2020 2020  elf.title,.     
-00014400: 2020 2029 0a0a 2020 2020 6465 6620 7265     )..    def re
-00014410: 636f 7665 725f 7765 616b 5f62 6561 6d28  cover_weak_beam(
-00014420: 7365 6c66 2c20 6e2c 2069 6e64 6963 6573  self, n, indices
-00014430: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00014440: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-00014450: 746f 207a 6572 6f20 616c 6c20 7069 7865  to zero all pixe
-00014460: 6c73 2068 6967 6865 7220 7468 616e 206e  ls higher than n
-00014470: 2074 696d 6573 2074 6865 2073 7461 6e64   times the stand
-00014480: 6172 6420 6465 7669 6174 696f 6e20 6163  ard deviation ac
-00014490: 726f 7373 2074 6865 2073 7461 636b 2064  ross the stack d
-000144a0: 696d 656e 7369 6f6e 0a0a 2020 2020 2020  imension..      
-000144b0: 2020 3a70 6172 616d 206e 3a20 496e 6372    :param n: Incr
-000144c0: 6561 7365 206f 7220 6465 6372 6561 7365  ease or decrease
-000144d0: 2074 6865 2074 6f70 2074 6872 6573 686f   the top thresho
-000144e0: 6c64 2062 7920 7468 6973 2066 6978 6564  ld by this fixed
-000144f0: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
-00014500: 3a74 7970 6520 6e3a 2066 6c6f 6174 0a20  :type n: float. 
-00014510: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00014520: 6469 6365 733a 2049 6e64 6963 6573 206f  dices: Indices o
-00014530: 6620 7468 6520 696d 6167 6573 2074 6f20  f the images to 
-00014540: 7573 6520 666f 7220 7468 6520 6669 6c74  use for the filt
-00014550: 6572 696e 672e 0a20 2020 2020 2020 2020  ering..         
-00014560: 2020 2049 6620 4e6f 6e65 2c20 7468 6520     If None, the 
-00014570: 6669 6c74 6572 696e 6720 6973 2064 6f6e  filtering is don
-00014580: 6520 7573 696e 6720 616c 6c20 6461 7461  e using all data
-00014590: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000145a0: 696e 6469 6365 733a 2055 6e69 6f6e 5b4e  indices: Union[N
-000145b0: 6f6e 652c 2061 7272 6179 5f6c 696b 655d  one, array_like]
-000145c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000145d0: 2020 2020 2073 7464 203d 206e 756d 7079       std = numpy
-000145e0: 2e73 7464 2873 656c 662e 6765 745f 6461  .std(self.get_da
-000145f0: 7461 2869 6e64 6963 6573 292e 7669 6577  ta(indices).view
-00014600: 286e 756d 7079 2e6e 6461 7272 6179 292c  (numpy.ndarray),
-00014610: 2061 7869 733d 3029 0a0a 2020 2020 2020   axis=0)..      
-00014620: 2020 7265 7475 726e 2073 656c 662e 6170    return self.ap
-00014630: 706c 795f 7468 7265 7368 6f6c 645f 7265  ply_threshold_re
-00014640: 6d6f 7661 6c28 746f 703d 6e20 2a20 7374  moval(top=n * st
-00014650: 642c 2069 6e64 6963 6573 3d69 6e64 6963  d, indices=indic
-00014660: 6573 290a 0a20 2020 2064 6566 205f 5f64  es)..    def __d
-00014670: 6565 7063 6f70 795f 5f28 7365 6c66 2c20  eepcopy__(self, 
-00014680: 6d65 6d6f 293a 0a20 2020 2020 2020 2022  memo):.        "
-00014690: 2222 0a20 2020 2020 2020 2043 7265 6174  "".        Creat
-000146a0: 6520 636f 7079 206f 6620 7468 6520 6461  e copy of the da
-000146b0: 7461 7365 742e 2054 6865 2064 6174 6120  taset. The data 
-000146c0: 6e75 6d70 7920 6172 7261 7920 6973 2061  numpy array is a
-000146d0: 6c73 6f20 636f 7069 6564 2075 7369 6e67  lso copied using
-000146e0: 0a20 2020 2020 2020 2064 6565 7020 636f  .        deep co
-000146f0: 7079 2e20 5468 6520 7265 7374 206f 6620  py. The rest of 
-00014700: 7468 6520 6174 7472 6962 7574 6573 2061  the attributes a
-00014710: 7265 2074 6865 2073 616d 652e 0a20 2020  re the same..   
-00014720: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014730: 2064 6174 6173 6574 203d 2074 7970 6528   dataset = type(
-00014740: 7365 6c66 2928 0a20 2020 2020 2020 2020  self)(.         
-00014750: 2020 2073 656c 662e 6469 722c 0a20 2020     self.dir,.   
-00014760: 2020 2020 2020 2020 2064 6174 613d 7365           data=se
-00014770: 6c66 2e64 6174 612c 0a20 2020 2020 2020  lf.data,.       
-00014780: 2020 2020 2064 696d 733d 7365 6c66 2e5f       dims=self._
-00014790: 5f64 696d 732c 0a20 2020 2020 2020 2020  _dims,.         
-000147a0: 2020 2069 6e5f 6d65 6d6f 7279 3d73 656c     in_memory=sel
-000147b0: 662e 696e 5f6d 656d 6f72 792c 0a20 2020  f.in_memory,.   
-000147c0: 2020 2020 2020 2020 2063 6f70 795f 6669           copy_fi
-000147d0: 6c65 733d 5472 7565 2c0a 2020 2020 2020  les=True,.      
-000147e0: 2020 290a 2020 2020 2020 2020 6461 7461    ).        data
-000147f0: 7365 742e 6469 6d73 203d 2063 6f70 792e  set.dims = copy.
-00014800: 6465 6570 636f 7079 2873 656c 662e 5f5f  deepcopy(self.__
-00014810: 6469 6d73 2c20 6d65 6d6f 290a 2020 2020  dims, memo).    
-00014820: 2020 2020 7265 7475 726e 2064 6174 6173      return datas
-00014830: 6574 0a0a 0a63 6c61 7373 2044 6174 6128  et...class Data(
-00014840: 6e75 6d70 792e 6e64 6172 7261 7929 3a0a  numpy.ndarray):.
-00014850: 2020 2020 2222 220a 2020 2020 436c 6173      """.    Clas
-00014860: 7320 746f 2073 7472 7563 7475 7265 2074  s to structure t
-00014870: 6865 2064 6174 6120 616e 6420 6c69 6e6b  he data and link
-00014880: 2065 7665 7279 2069 6d61 6765 2077 6974   every image wit
-00014890: 6820 6974 7320 636f 7272 6573 706f 6e64  h its correspond
-000148a0: 696e 6720 7572 6c20 616e 640a 2020 2020  ing url and.    
-000148b0: 6d65 7461 6461 7461 2e20 4974 2069 6e68  metadata. It inh
-000148c0: 6572 6974 7320 6672 6f6d 206e 756d 7079  erits from numpy
-000148d0: 2e6e 6461 7272 6179 2061 6e64 204f 7665  .ndarray and Ove
-000148e0: 7272 6964 6573 2074 6865 206e 6563 6573  rrides the neces
-000148f0: 7361 7279 206d 6574 686f 6473 2c0a 2020  sary methods,.  
-00014900: 2020 7461 6b69 6e67 2069 6e74 6f20 6163    taking into ac
-00014910: 636f 756e 7420 7468 6520 6069 6e5f 6d65  count the `in_me
-00014920: 6d6f 7279 6020 6174 7472 6962 7574 652e  mory` attribute.
-00014930: 0a0a 2020 2020 3a70 6172 616d 2075 726c  ..    :param url
-00014940: 733a 2041 7272 6179 2077 6974 6820 7468  s: Array with th
-00014950: 6520 7572 6c73 206f 6620 7468 6520 6461  e urls of the da
-00014960: 7461 0a20 2020 203a 7479 7065 2075 726c  ta.    :type url
-00014970: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
-00014980: 2020 3a70 6172 616d 206d 6574 6164 6174    :param metadat
-00014990: 613a 2041 7272 6179 2077 6974 6820 7468  a: Array with th
-000149a0: 6520 6d65 7461 6461 7461 206f 6620 7468  e metadata of th
-000149b0: 6520 6461 7461 0a20 2020 203a 7479 7065  e data.    :type
-000149c0: 206d 6574 6164 6174 613a 2061 7272 6179   metadata: array
-000149d0: 5f6c 696b 650a 2020 2020 3a70 6172 616d  _like.    :param
-000149e0: 2069 6e5f 6d65 6d6f 7279 3a20 4966 2054   in_memory: If T
-000149f0: 7275 652c 2074 6865 2064 6174 6120 6973  rue, the data is
-00014a00: 206c 6f61 6465 6420 696e 746f 206d 656d   loaded into mem
-00014a10: 6f72 792c 2064 6566 6175 6c74 2054 7275  ory, default Tru
-00014a20: 650a 2020 2020 3a74 7970 6520 696e 5f6d  e.    :type in_m
-00014a30: 656d 6f72 793a 2062 6f6f 6c2c 206f 7074  emory: bool, opt
-00014a40: 696f 6e61 6c0a 2020 2020 2222 220a 0a20  ional.    """.. 
-00014a50: 2020 2064 6566 205f 5f6e 6577 5f5f 2863     def __new__(c
-00014a60: 6c73 2c20 7572 6c73 2c20 6d65 7461 6461  ls, urls, metada
-00014a70: 7461 2c20 696e 5f6d 656d 6f72 793d 5472  ta, in_memory=Tr
-00014a80: 7565 2c20 6461 7461 3d4e 6f6e 6529 3a0a  ue, data=None):.
-00014a90: 2020 2020 2020 2020 7572 6c73 203d 206e          urls = n
-00014aa0: 756d 7079 2e61 7361 7272 6179 2875 726c  umpy.asarray(url
-00014ab0: 7329 0a20 2020 2020 2020 2069 6d67 5f73  s).        img_s
-00014ac0: 6861 7065 203d 204e 6f6e 650a 2020 2020  hape = None.    
-00014ad0: 2020 2020 6966 2069 6e5f 6d65 6d6f 7279      if in_memory
-00014ae0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014af0: 2064 6174 6120 6973 206e 6f74 204e 6f6e   data is not Non
-00014b00: 6520 616e 6420 7572 6c73 2e73 6861 7065  e and urls.shape
-00014b10: 2021 3d20 6461 7461 2e73 6861 7065 5b3a   != data.shape[:
-00014b20: 2d32 5d3a 0a20 2020 2020 2020 2020 2020  -2]:.           
-00014b30: 2020 2020 2064 6174 6120 3d20 4e6f 6e65       data = None
-00014b40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014b50: 6461 7461 2069 7320 4e6f 6e65 3a0a 2020  data is None:.  
-00014b60: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-00014b70: 6c5f 7368 6170 6520 3d20 7572 6c73 2e73  l_shape = urls.s
-00014b80: 6861 7065 0a20 2020 2020 2020 2020 2020  hape.           
-00014b90: 2020 2020 2075 726c 5f69 6478 7320 3d20       url_idxs = 
-00014ba0: 6e75 6d70 792e 756e 7261 7665 6c5f 696e  numpy.unravel_in
-00014bb0: 6465 7828 6e75 6d70 792e 6172 616e 6765  dex(numpy.arange
-00014bc0: 2875 726c 732e 7369 7a65 292c 2075 726c  (urls.size), url
-00014bd0: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
-00014be0: 2020 2020 2020 2020 696d 6720 3d20 7574          img = ut
-00014bf0: 696c 732e 6765 745f 6461 7461 286e 6578  ils.get_data(nex
-00014c00: 7428 7572 6c73 2e66 6c61 7429 290a 2020  t(urls.flat)).  
-00014c10: 2020 2020 2020 2020 2020 2020 2020 696d                im
-00014c20: 675f 7368 6170 6520 3d20 696d 672e 7368  g_shape = img.sh
-00014c30: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
-00014c40: 2020 2020 6461 7461 203d 206e 756d 7079      data = numpy
-00014c50: 2e65 6d70 7479 2875 726c 5f73 6861 7065  .empty(url_shape
-00014c60: 202b 2069 6d67 5f73 6861 7065 2c20 696d   + img_shape, im
-00014c70: 672e 6474 7970 6529 0a20 2020 2020 2020  g.dtype).       
-00014c80: 2020 2020 2020 2020 2066 6f72 2075 726c           for url
-00014c90: 2c20 2a75 726c 5f69 6478 2069 6e20 7a69  , *url_idx in zi
-00014ca0: 7028 7572 6c73 2e66 6c61 742c 202a 7572  p(urls.flat, *ur
-00014cb0: 6c5f 6964 7873 293a 0a20 2020 2020 2020  l_idxs):.       
-00014cc0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00014cd0: 615b 7475 706c 6528 7572 6c5f 6964 7829  a[tuple(url_idx)
-00014ce0: 5d20 3d20 7574 696c 732e 6765 745f 6461  ] = utils.get_da
-00014cf0: 7461 2875 726c 290a 2020 2020 2020 2020  ta(url).        
-00014d00: 2020 2020 6f62 6a20 3d20 6461 7461 2e76      obj = data.v
-00014d10: 6965 7728 636c 7329 0a20 2020 2020 2020  iew(cls).       
-00014d20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00014d30: 2020 2023 2041 6363 6573 7320 696d 6167     # Access imag
-00014d40: 6520 6f6e 6520 6174 2061 2074 696d 6520  e one at a time 
-00014d50: 7573 696e 6720 7572 6c0a 2020 2020 2020  using url.      
-00014d60: 2020 2020 2020 6f62 6a20 3d20 7375 7065        obj = supe
-00014d70: 7228 292e 5f5f 6e65 775f 5f28 636c 732c  r().__new__(cls,
-00014d80: 2075 726c 732e 7368 6170 6529 0a0a 2020   urls.shape)..  
-00014d90: 2020 2020 2020 6f62 6a2e 696e 5f6d 656d        obj.in_mem
-00014da0: 6f72 7920 3d20 696e 5f6d 656d 6f72 790a  ory = in_memory.
-00014db0: 2020 2020 2020 2020 6f62 6a2e 7572 6c73          obj.urls
-00014dc0: 203d 2075 726c 730a 2020 2020 2020 2020   = urls.        
-00014dd0: 6f62 6a2e 6d65 7461 6461 7461 203d 206e  obj.metadata = n
-00014de0: 756d 7079 2e61 7361 7272 6179 286d 6574  umpy.asarray(met
-00014df0: 6164 6174 6129 0a20 2020 2020 2020 206f  adata).        o
-00014e00: 626a 2e5f 6669 6c65 203d 204e 6f6e 650a  bj._file = None.
-00014e10: 2020 2020 2020 2020 6f62 6a2e 5f69 6d67          obj._img
-00014e20: 5f73 6861 7065 203d 2069 6d67 5f73 6861  _shape = img_sha
-00014e30: 7065 0a20 2020 2020 2020 206f 626a 2e73  pe.        obj.s
-00014e40: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
-00014e50: 6e73 203d 205f 5374 6174 654f 664f 7065  ns = _StateOfOpe
-00014e60: 7261 7469 6f6e 7328 290a 0a20 2020 2020  rations()..     
-00014e70: 2020 2072 6574 7572 6e20 6f62 6a0a 0a20     return obj.. 
-00014e80: 2020 2064 6566 205f 5f61 7272 6179 5f66     def __array_f
-00014e90: 696e 616c 697a 655f 5f28 7365 6c66 2c20  inalize__(self, 
-00014ea0: 6f62 6a29 3a0a 2020 2020 2020 2020 6966  obj):.        if
-00014eb0: 206f 626a 2069 7320 4e6f 6e65 3a0a 2020   obj is None:.  
-00014ec0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014ed0: 0a20 2020 2020 2020 2073 656c 662e 7572  .        self.ur
-00014ee0: 6c73 203d 2067 6574 6174 7472 286f 626a  ls = getattr(obj
-00014ef0: 2c20 2275 726c 7322 2c20 4e6f 6e65 290a  , "urls", None).
-00014f00: 2020 2020 2020 2020 7365 6c66 2e6d 6574          self.met
-00014f10: 6164 6174 6120 3d20 6765 7461 7474 7228  adata = getattr(
-00014f20: 6f62 6a2c 2022 6d65 7461 6461 7461 222c  obj, "metadata",
-00014f30: 204e 6f6e 6529 0a20 2020 2020 2020 2073   None).        s
-00014f40: 656c 662e 696e 5f6d 656d 6f72 7920 3d20  elf.in_memory = 
-00014f50: 6765 7461 7474 7228 6f62 6a2c 2022 696e  getattr(obj, "in
-00014f60: 5f6d 656d 6f72 7922 2c20 4e6f 6e65 290a  _memory", None).
-00014f70: 0a20 2020 2064 6566 205f 5f67 6574 6974  .    def __getit
-00014f80: 656d 5f5f 2873 656c 662c 2069 6e64 6963  em__(self, indic
-00014f90: 6573 293a 0a20 2020 2020 2020 2022 2222  es):.        """
-00014fa0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00014fb0: 7365 6c66 5b69 6e64 6963 6573 5d0a 2020  self[indices].  
-00014fc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014fd0: 2020 6966 2073 656c 662e 696e 5f6d 656d    if self.in_mem
-00014fe0: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
-00014ff0: 2064 6174 6120 3d20 7375 7065 7228 292e   data = super().
-00015000: 5f5f 6765 7469 7465 6d5f 5f28 696e 6469  __getitem__(indi
-00015010: 6365 7329 0a20 2020 2020 2020 2020 2020  ces).           
-00015020: 2069 6620 6c65 6e28 6461 7461 2e73 6861   if len(data.sha
-00015030: 7065 2920 3c20 333a 0a20 2020 2020 2020  pe) < 3:.       
-00015040: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-00015050: 6461 7461 2e76 6965 7728 6e75 6d70 792e  data.view(numpy.
-00015060: 6e64 6172 7261 7929 0a20 2020 2020 2020  ndarray).       
-00015070: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015080: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00015090: 696e 7374 616e 6365 2869 6e64 6963 6573  instance(indices
-000150a0: 2c20 7475 706c 6529 3a0a 2020 2020 2020  , tuple):.      
-000150b0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000150c0: 7461 2e75 726c 7320 3d20 7365 6c66 2e75  ta.urls = self.u
-000150d0: 726c 735b 696e 6469 6365 735b 305d 5d0a  rls[indices[0]].
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2020 2020 6461 7461 2e6d 6574 6164 6174      data.metadat
-00015100: 6120 3d20 7365 6c66 2e6d 6574 6164 6174  a = self.metadat
-00015110: 615b 696e 6469 6365 735b 305d 5d0a 2020  a[indices[0]].  
-00015120: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00015130: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00015140: 2020 2020 2020 2020 6461 7461 2e75 726c          data.url
-00015150: 7320 3d20 7365 6c66 2e75 726c 735b 696e  s = self.urls[in
-00015160: 6469 6365 735d 0a20 2020 2020 2020 2020  dices].         
-00015170: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-00015180: 6d65 7461 6461 7461 203d 2073 656c 662e  metadata = self.
-00015190: 6d65 7461 6461 7461 5b69 6e64 6963 6573  metadata[indices
-000151a0: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
-000151b0: 7475 726e 2064 6174 610a 2020 2020 2020  turn data.      
-000151c0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-000151d0: 696e 6469 6365 732c 2074 7570 6c65 293a  indices, tuple):
-000151e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000151f0: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
-00015200: 656c 662e 7572 6c73 5b69 6e64 6963 6573  elf.urls[indices
-00015210: 5b30 5d5d 2c20 6e75 6d70 792e 6e64 6172  [0]], numpy.ndar
-00015220: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
-00015230: 2020 2020 2020 7265 7475 726e 2075 7469        return uti
-00015240: 6c73 2e67 6574 5f64 6174 6128 7365 6c66  ls.get_data(self
-00015250: 2e75 726c 735b 696e 6469 6365 735b 305d  .urls[indices[0]
-00015260: 5d29 5b69 6e64 6963 6573 5b31 5d2c 2069  ])[indices[1], i
-00015270: 6e64 6963 6573 5b32 5d5d 0a20 2020 2020  ndices[2]].     
-00015280: 2020 2020 2020 2072 6574 7572 6e20 4461         return Da
-00015290: 7461 2873 656c 662e 7572 6c73 5b69 6e64  ta(self.urls[ind
-000152a0: 6963 6573 5b30 5d5d 2c20 7365 6c66 2e6d  ices[0]], self.m
-000152b0: 6574 6164 6174 615b 696e 6469 6365 735d  etadata[indices]
-000152c0: 2c20 7365 6c66 2e69 6e5f 6d65 6d6f 7279  , self.in_memory
-000152d0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-000152e0: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
-000152f0: 2e75 726c 735b 696e 6469 6365 735d 2c20  .urls[indices], 
-00015300: 6e75 6d70 792e 6e64 6172 7261 7929 3a0a  numpy.ndarray):.
-00015310: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015320: 726e 2075 7469 6c73 2e67 6574 5f64 6174  rn utils.get_dat
-00015330: 6128 7365 6c66 2e75 726c 735b 696e 6469  a(self.urls[indi
-00015340: 6365 735d 290a 2020 2020 2020 2020 7265  ces]).        re
-00015350: 7475 726e 2044 6174 6128 7365 6c66 2e75  turn Data(self.u
-00015360: 726c 735b 696e 6469 6365 735d 2c20 7365  rls[indices], se
-00015370: 6c66 2e6d 6574 6164 6174 615b 696e 6469  lf.metadata[indi
-00015380: 6365 735d 2c20 7365 6c66 2e69 6e5f 6d65  ces], self.in_me
-00015390: 6d6f 7279 290a 0a20 2020 2064 6566 205f  mory)..    def _
-000153a0: 6974 6572 5f66 7261 6d65 7328 7365 6c66  iter_frames(self
-000153b0: 2920 2d3e 2047 656e 6572 6174 6f72 5b6e  ) -> Generator[n
-000153c0: 756d 7079 2e6e 6461 7272 6179 2c20 4e6f  umpy.ndarray, No
-000153d0: 6e65 2c20 4e6f 6e65 5d3a 0a20 2020 2020  ne, None]:.     
-000153e0: 2020 2069 6620 7365 6c66 2e69 6e5f 6d65     if self.in_me
-000153f0: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
-00015400: 2020 6673 6861 7065 203d 2028 7365 6c66    fshape = (self
-00015410: 2e6e 6672 616d 6573 2c29 202b 2073 656c  .nframes,) + sel
-00015420: 662e 6672 616d 655f 7368 6170 650a 2020  f.frame_shape.  
-00015430: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00015440: 6672 6f6d 2073 7570 6572 2829 2e72 6573  from super().res
-00015450: 6861 7065 2866 7368 6170 6529 0a20 2020  hape(fshape).   
-00015460: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015470: 2020 2020 2020 2066 6f72 2075 726c 2069         for url i
-00015480: 6e20 7365 6c66 2e75 726c 732e 666c 6174  n self.urls.flat
-00015490: 7465 6e28 293a 0a20 2020 2020 2020 2020  ten():.         
-000154a0: 2020 2020 2020 2079 6965 6c64 2075 7469         yield uti
-000154b0: 6c73 2e67 6574 5f64 6174 6128 7572 6c29  ls.get_data(url)
-000154c0: 0a0a 2020 2020 6465 6620 5f5f 7265 6475  ..    def __redu
-000154d0: 6365 5f5f 2873 656c 6629 3a0a 2020 2020  ce__(self):.    
-000154e0: 2020 2020 2320 4765 7420 7468 6520 7061      # Get the pa
-000154f0: 7265 6e74 2773 205f 5f72 6564 7563 655f  rent's __reduce_
-00015500: 5f20 7475 706c 650a 2020 2020 2020 2020  _ tuple.        
-00015510: 7069 636b 6c65 645f 7374 6174 6520 3d20  pickled_state = 
-00015520: 7375 7065 7228 292e 5f5f 7265 6475 6365  super().__reduce
-00015530: 5f5f 2829 0a20 2020 2020 2020 2023 2043  __().        # C
-00015540: 7265 6174 6520 6f75 7220 6f77 6e20 7475  reate our own tu
-00015550: 706c 6520 746f 2070 6173 7320 746f 205f  ple to pass to _
-00015560: 5f73 6574 7374 6174 655f 5f0a 2020 2020  _setstate__.    
-00015570: 2020 2020 6e65 775f 7374 6174 6520 3d20      new_state = 
-00015580: 7069 636b 6c65 645f 7374 6174 655b 325d  pickled_state[2]
-00015590: 202b 2028 2873 656c 662e 7572 6c73 2c20   + ((self.urls, 
-000155a0: 7365 6c66 2e6d 6574 6164 6174 612c 2073  self.metadata, s
-000155b0: 656c 662e 696e 5f6d 656d 6f72 7929 2c29  elf.in_memory),)
-000155c0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-000155d0: 6e20 6120 7475 706c 6520 7468 6174 2072  n a tuple that r
-000155e0: 6570 6c61 6365 7320 7468 6520 7061 7265  eplaces the pare
-000155f0: 6e74 2773 205f 5f73 6574 7374 6174 655f  nt's __setstate_
-00015600: 5f20 7475 706c 6520 7769 7468 206f 7572  _ tuple with our
-00015610: 206f 776e 0a20 2020 2020 2020 2072 6574   own.        ret
-00015620: 7572 6e20 2870 6963 6b6c 6564 5f73 7461  urn (pickled_sta
-00015630: 7465 5b30 5d2c 2070 6963 6b6c 6564 5f73  te[0], pickled_s
-00015640: 7461 7465 5b31 5d2c 206e 6577 5f73 7461  tate[1], new_sta
-00015650: 7465 290a 0a20 2020 2064 6566 205f 5f73  te)..    def __s
-00015660: 6574 7374 6174 655f 5f28 7365 6c66 2c20  etstate__(self, 
-00015670: 7374 6174 6529 3a0a 2020 2020 2020 2020  state):.        
-00015680: 7365 6c66 2e75 726c 732c 2073 656c 662e  self.urls, self.
-00015690: 6d65 7461 6461 7461 2c20 7365 6c66 2e69  metadata, self.i
-000156a0: 6e5f 6d65 6d6f 7279 203d 2073 7461 7465  n_memory = state
-000156b0: 5b2d 315d 2020 2320 5365 7420 7468 6520  [-1]  # Set the 
-000156c0: 6174 7472 6962 7574 6573 0a20 2020 2020  attributes.     
-000156d0: 2020 2073 7570 6572 2829 2e5f 5f73 6574     super().__set
-000156e0: 7374 6174 655f 5f28 7374 6174 655b 303a  state__(state[0:
-000156f0: 2d31 5d29 0a0a 2020 2020 6465 6620 7374  -1])..    def st
-00015700: 6f70 5f6f 7065 7261 7469 6f6e 2873 656c  op_operation(sel
-00015710: 662c 206f 7065 7261 7469 6f6e 3a20 4f70  f, operation: Op
-00015720: 6572 6174 696f 6e29 3a0a 2020 2020 2020  eration):.      
-00015730: 2020 2222 220a 2020 2020 2020 2020 4d65    """.        Me
-00015740: 7468 6f64 2075 7365 6420 666f 7220 6361  thod used for ca
-00015750: 7365 7320 7768 6572 6520 7468 7265 6164  ses where thread
-00015760: 7320 6172 6520 6372 6561 7465 6420 746f  s are created to
-00015770: 2061 7070 6c79 2066 756e 6374 696f 6e73   apply functions
-00015780: 2074 6f20 7468 6520 6461 7461 2e0a 2020   to the data..  
-00015790: 2020 2020 2020 4966 206d 6574 686f 6420        If method 
-000157a0: 6973 2063 616c 6c65 642c 2074 6865 2066  is called, the f
-000157b0: 6c61 6720 636f 6e63 6572 6e69 6e67 2074  lag concerning t
-000157c0: 6865 2073 746f 7020 6973 2073 6574 2074  he stop is set t
-000157d0: 6f20 3020 736f 2074 6861 7420 6966 2074  o 0 so that if t
-000157e0: 6865 2063 6f6e 6365 726e 6564 0a20 2020  he concerned.   
-000157f0: 2020 2020 206f 7065 7261 7469 6f6e 2069       operation i
-00015800: 7320 7275 6e6e 696e 6720 696e 2061 6e6f  s running in ano
-00015810: 7468 6572 2074 6872 6561 6420 6974 206b  ther thread it k
-00015820: 6e6f 7773 2074 6f20 7374 6f70 2e0a 0a20  nows to stop... 
-00015830: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00015840: 7420 6f70 6572 6174 696f 6e3a 206f 7065  t operation: ope
-00015850: 7261 7469 6f6e 2074 6f20 7374 6f70 0a20  ration to stop. 
-00015860: 2020 2020 2020 203a 7479 7065 2069 6e74         :type int
-00015870: 3a20 556e 696f 6e5b 696e 742c 2060 4f70  : Union[int, `Op
-00015880: 6572 6174 696f 6e60 5d0a 2020 2020 2020  eration`].      
-00015890: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000158a0: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
-000158b0: 7374 6174 655f 6f66 5f6f 7065 7261 7469  state_of_operati
-000158c0: 6f6e 7322 2920 616e 6420 7365 6c66 2e73  ons") and self.s
-000158d0: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
-000158e0: 6e73 2e69 735f 7275 6e6e 696e 6728 0a20  ns.is_running(. 
-000158f0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-00015900: 7469 6f6e 0a20 2020 2020 2020 2029 3a0a  tion.        ):.
-00015910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015920: 2e73 7461 7465 5f6f 665f 6f70 6572 6174  .state_of_operat
-00015930: 696f 6e73 2e73 746f 7028 6f70 6572 6174  ions.stop(operat
-00015940: 696f 6e29 0a0a 2020 2020 4070 726f 7065  ion)..    @prope
-00015950: 7274 790a 2020 2020 6465 6620 7368 6170  rty.    def shap
-00015960: 6528 7365 6c66 2920 2d3e 2054 7570 6c65  e(self) -> Tuple
-00015970: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-00015980: 2222 546f 7461 6c20 7368 6170 6520 3d20  ""Total shape = 
-00015990: 7363 616e 2073 6861 7065 202b 2066 7261  scan shape + fra
-000159a0: 6d65 2073 6861 7065 2222 220a 2020 2020  me shape""".    
-000159b0: 2020 2020 7368 6170 6520 3d20 7375 7065      shape = supe
-000159c0: 7228 292e 7368 6170 650a 2020 2020 2020  r().shape.      
-000159d0: 2020 6966 2073 656c 662e 696e 5f6d 656d    if self.in_mem
-000159e0: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
-000159f0: 2072 6574 7572 6e20 7368 6170 650a 2020   return shape.  
-00015a00: 2020 2020 2020 7265 7475 726e 2073 6861        return sha
-00015a10: 7065 202b 2073 656c 662e 6672 616d 655f  pe + self.frame_
-00015a20: 7368 6170 650a 0a20 2020 2040 7072 6f70  shape..    @prop
-00015a30: 6572 7479 0a20 2020 2064 6566 2073 6361  erty.    def sca
-00015a40: 6e5f 7368 6170 6528 7365 6c66 2920 2d3e  n_shape(self) ->
-00015a50: 2054 7570 6c65 5b69 6e74 5d3a 0a20 2020   Tuple[int]:.   
-00015a60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00015a70: 2e73 6861 7065 5b3a 2d32 5d0a 0a20 2020  .shape[:-2]..   
-00015a80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00015a90: 6566 2066 7261 6d65 5f73 6861 7065 2873  ef frame_shape(s
-00015aa0: 656c 6629 202d 3e20 5475 706c 655b 696e  elf) -> Tuple[in
-00015ab0: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
-00015ac0: 2069 6620 7365 6c66 2e69 6e5f 6d65 6d6f   if self.in_memo
-00015ad0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00015ae0: 7265 7475 726e 2073 7570 6572 2829 2e73  return super().s
-00015af0: 6861 7065 5b2d 323a 5d0a 2020 2020 2020  hape[-2:].      
-00015b00: 2020 6966 2073 656c 662e 5f69 6d67 5f73    if self._img_s
-00015b10: 6861 7065 2069 7320 6e6f 7420 4e6f 6e65  hape is not None
-00015b20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00015b30: 7475 726e 2073 656c 662e 5f69 6d67 5f73  turn self._img_s
-00015b40: 6861 7065 0a20 2020 2020 2020 2069 6620  hape.        if 
-00015b50: 7365 6c66 2e6e 6672 616d 6573 203d 3d20  self.nframes == 
-00015b60: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00015b70: 6574 7572 6e20 302c 2030 0a20 2020 2020  eturn 0, 0.     
-00015b80: 2020 2069 6d67 5f73 6861 7065 203d 2075     img_shape = u
-00015b90: 7469 6c73 2e67 6574 5f64 6174 6128 6e65  tils.get_data(ne
-00015ba0: 7874 2873 656c 662e 7572 6c73 2e66 6c61  xt(self.urls.fla
-00015bb0: 7429 292e 7368 6170 650a 2020 2020 2020  t)).shape.      
-00015bc0: 2020 7365 6c66 2e5f 696d 675f 7368 6170    self._img_shap
-00015bd0: 6520 3d20 696d 675f 7368 6170 650a 2020  e = img_shape.  
-00015be0: 2020 2020 2020 7265 7475 726e 2069 6d67        return img
-00015bf0: 5f73 6861 7065 0a0a 2020 2020 4070 726f  _shape..    @pro
-00015c00: 7065 7274 790a 2020 2020 6465 6620 6e66  perty.    def nf
-00015c10: 7261 6d65 7328 7365 6c66 2920 2d3e 2069  rames(self) -> i
-00015c20: 6e74 3a0a 2020 2020 2020 2020 6966 2073  nt:.        if s
-00015c30: 656c 662e 7572 6c73 2069 7320 4e6f 6e65  elf.urls is None
-00015c40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00015c50: 7475 726e 2030 0a20 2020 2020 2020 2072  turn 0.        r
-00015c60: 6574 7572 6e20 7365 6c66 2e75 726c 732e  eturn self.urls.
-00015c70: 7369 7a65 0a0a 2020 2020 4070 726f 7065  size..    @prope
-00015c80: 7274 790a 2020 2020 6465 6620 6e64 696d  rty.    def ndim
-00015c90: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00015ca0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00015cb0: 2020 204e 756d 6265 7220 6f66 2061 7272     Number of arr
-00015cc0: 6179 2064 696d 656e 7369 6f6e 732e 0a20  ay dimensions.. 
-00015cd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00015ce0: 2020 2069 6620 7365 6c66 2e69 6e5f 6d65     if self.in_me
-00015cf0: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
-00015d00: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00015d10: 2e6e 6469 6d0a 2020 2020 2020 2020 7265  .ndim.        re
-00015d20: 7475 726e 2073 7570 6572 2829 2e6e 6469  turn super().ndi
-00015d30: 6d20 2b20 320a 0a20 2020 2064 6566 2061  m + 2..    def a
-00015d40: 7070 6c79 5f66 756e 6373 280a 2020 2020  pply_funcs(.    
-00015d50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00015d60: 2020 6675 6e63 733d 5b5d 2c0a 2020 2020    funcs=[],.    
-00015d70: 2020 2020 696e 6469 6365 733d 4e6f 6e65      indices=None
-00015d80: 2c0a 2020 2020 2020 2020 7361 7665 3d46  ,.        save=F
-00015d90: 616c 7365 2c0a 2020 2020 2020 2020 7465  alse,.        te
-00015da0: 7874 3d22 222c 0a20 2020 2020 2020 206f  xt="",.        o
-00015db0: 7065 7261 7469 6f6e 3d4e 6f6e 652c 0a20  peration=None,. 
-00015dc0: 2020 2020 2020 206e 6577 5f73 6861 7065         new_shape
-00015dd0: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
-00015de0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00015df0: 2020 4d65 7468 6f64 2074 6861 7420 6170    Method that ap
-00015e00: 706c 6965 7320 6120 7365 7269 6573 206f  plies a series o
-00015e10: 6620 6675 6e63 7469 6f6e 7320 696e 746f  f functions into
-00015e20: 2074 6865 2064 6174 612e 2049 7420 6361   the data. It ca
-00015e30: 6e20 7361 7665 2074 6865 2069 6d61 6765  n save the image
-00015e40: 730a 2020 2020 2020 2020 696e 746f 2064  s.        into d
-00015e50: 6973 6b20 6f72 2072 6574 7572 6e20 7468  isk or return th
-00015e60: 656d 2e0a 0a20 2020 2020 2020 203a 7061  em...        :pa
-00015e70: 7261 6d20 6675 6e63 733a 204c 6973 7420  ram funcs: List 
-00015e80: 6f66 2074 7570 706c 6573 2e20 4576 6572  of tupples. Ever
-00015e90: 7920 7475 7070 6c65 7320 636f 6e74 6169  y tupples contai
-00015ea0: 6e73 2074 6865 2066 756e 6374 696f 6e20  ns the function 
-00015eb0: 746f 0a20 2020 2020 2020 2020 2020 2061  to.            a
-00015ec0: 7070 6c79 2061 6e64 2069 7473 2070 6172  pply and its par
-00015ed0: 616d 6574 6572 732c 2064 6566 6175 6c74  ameters, default
-00015ee0: 7320 746f 205b 5d0a 2020 2020 2020 2020  s to [].        
-00015ef0: 3a74 7970 6520 6675 6e63 733a 2061 7272  :type funcs: arr
-00015f00: 6179 5f6c 696b 652c 206f 7074 696f 6e61  ay_like, optiona
-00015f10: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
-00015f20: 2069 6e64 6963 6573 3a20 496e 6469 6365   indices: Indice
-00015f30: 7320 6f66 2074 6865 2064 6174 6120 746f  s of the data to
-00015f40: 2061 7070 6c79 2074 6865 2066 756e 6374   apply the funct
-00015f50: 696f 6e73 2074 6f2c 0a20 2020 2020 2020  ions to,.       
-00015f60: 2020 2020 2064 6566 6175 6c74 7320 746f       defaults to
-00015f70: 204e 6f6e 650a 2020 2020 2020 2020 3a74   None.        :t
-00015f80: 7970 6520 696e 6469 6365 733a 2055 6e69  ype indices: Uni
-00015f90: 6f6e 5b4e 6f6e 652c 2061 7272 6179 5f6c  on[None, array_l
-00015fa0: 696b 655d 2c20 6f70 7469 6f6e 616c 0a20  ike], optional. 
-00015fb0: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-00015fc0: 7665 3a20 4966 2054 7275 652c 2073 6176  ve: If True, sav
-00015fd0: 6573 2074 6865 2069 6d61 6765 7320 696e  es the images in
-00015fe0: 746f 2064 6973 6b2c 2064 6566 6175 6c74  to disk, default
-00015ff0: 7320 746f 2046 616c 7365 0a20 2020 2020  s to False.     
-00016000: 2020 203a 7479 7065 2073 6176 653a 2062     :type save: b
-00016010: 6f6f 6c0a 2020 2020 2020 2020 3a70 6172  ool.        :par
-00016020: 616d 2073 7472 2074 6578 743a 2054 6578  am str text: Tex
-00016030: 7420 746f 2073 686f 7720 696e 2074 6865  t to show in the
-00016040: 2061 6476 616e 6365 6d65 6e74 2064 6973   advancement dis
-00016050: 706c 6179 2e0a 2020 2020 2020 2020 3a70  play..        :p
-00016060: 6172 616d 2069 6e74 206f 7065 7261 7469  aram int operati
-00016070: 6f6e 3a20 6f70 6572 6174 696f 6e20 746f  on: operation to
-00016080: 2073 746f 700a 2020 2020 2020 2020 3a74   stop.        :t
-00016090: 7970 6520 696e 743a 2055 6e69 6f6e 5b69  ype int: Union[i
-000160a0: 6e74 2c20 604f 7065 7261 7469 6f6e 605d  nt, `Operation`]
-000160b0: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-000160c0: 6e73 3a20 4172 7261 7920 7769 7468 2074  ns: Array with t
-000160d0: 6865 206e 6577 2075 726c 7320 2869 6620  he new urls (if 
-000160e0: 6461 7461 2077 6173 2073 6176 6564 290a  data was saved).
-000160f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016100: 2020 2020 6966 2069 6e64 6963 6573 2069      if indices i
-00016110: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00016120: 2020 2020 696e 6469 6365 7320 3d20 7261      indices = ra
-00016130: 6e67 6528 6c65 6e28 7365 6c66 2929 0a20  nge(len(self)). 
-00016140: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00016150: 616e 6365 2869 6e64 6963 6573 2c20 696e  ance(indices, in
-00016160: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00016170: 696e 6469 6365 7320 3d20 5b69 6e64 6963  indices = [indic
-00016180: 6573 5d0a 2020 2020 2020 2020 7572 6c73  es].        urls
-00016190: 203d 205b 5d0a 2020 2020 2020 2020 696f   = [].        io
-000161a0: 5f75 7469 6c73 2e61 6476 616e 6365 6d65  _utils.advanceme
-000161b0: 6e74 5f64 6973 706c 6179 2830 2c20 7365  nt_display(0, se
-000161c0: 6c66 2e6e 6672 616d 6573 2c20 7465 7874  lf.nframes, text
-000161d0: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-000161e0: 7420 6861 7361 7474 7228 7365 6c66 2c20  t hasattr(self, 
-000161f0: 2273 7461 7465 5f6f 665f 6f70 6572 6174  "state_of_operat
-00016200: 696f 6e73 2229 3a0a 2020 2020 2020 2020  ions"):.        
-00016210: 2020 2020 7365 6c66 2e73 7461 7465 5f6f      self.state_o
-00016220: 665f 6f70 6572 6174 696f 6e73 203d 205f  f_operations = _
-00016230: 5374 6174 654f 664f 7065 7261 7469 6f6e  StateOfOperation
-00016240: 7328 290a 0a20 2020 2020 2020 2077 6974  s()..        wit
-00016250: 6820 7365 6c66 2e73 7461 7465 5f6f 665f  h self.state_of_
-00016260: 6f70 6572 6174 696f 6e73 2e72 756e 5f63  operations.run_c
-00016270: 6f6e 7465 7874 286f 7065 7261 7469 6f6e  ontext(operation
-00016280: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
-00016290: 6669 6c65 203d 204e 6f6e 650a 2020 2020  file = None.    
-000162a0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-000162b0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-000162c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000162d0: 2020 2020 2020 5f66 696c 6520 3d20 6835        _file = h5
-000162e0: 7079 2e46 696c 6528 7361 7665 2c20 2261  py.File(save, "a
-000162f0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00016300: 2020 2065 7863 6570 7420 4f53 4572 726f     except OSErro
-00016310: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00016320: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00016330: 682e 6578 6973 7473 2873 6176 6529 3a0a  h.exists(save):.
-00016340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016350: 2020 2020 2020 2020 6f73 2e72 656d 6f76          os.remov
-00016360: 6528 7361 7665 290a 2020 2020 2020 2020  e(save).        
-00016370: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
-00016380: 6520 3d20 6835 7079 2e46 696c 6528 7361  e = h5py.File(sa
-00016390: 7665 2c20 2277 2229 0a0a 2020 2020 2020  ve, "w")..      
-000163a0: 2020 2020 2020 2020 2020 6461 7461 7365            datase
-000163b0: 745f 6e61 6d65 203d 2022 6461 7461 7365  t_name = "datase
-000163c0: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-000163d0: 2020 206e 6577 5f73 6861 7065 203d 2073     new_shape = s
-000163e0: 656c 662e 7368 6170 6520 6966 206e 6577  elf.shape if new
-000163f0: 5f73 6861 7065 2069 7320 4e6f 6e65 2065  _shape is None e
-00016400: 6c73 6520 7475 706c 6528 6e65 775f 7368  lse tuple(new_sh
-00016410: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
-00016420: 2020 2020 2069 6620 2264 6174 6173 6574       if "dataset
-00016430: 2220 696e 205f 6669 6c65 3a0a 2020 2020  " in _file:.    
-00016440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016450: 6966 206e 6577 5f73 6861 7065 2021 3d20  if new_shape != 
-00016460: 5f66 696c 655b 2264 6174 6173 6574 225d  _file["dataset"]
-00016470: 2e73 6861 7065 3a0a 2020 2020 2020 2020  .shape:.        
-00016480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016490: 5f66 696c 652e 6372 6561 7465 5f64 6174  _file.create_dat
-000164a0: 6173 6574 280a 2020 2020 2020 2020 2020  aset(.          
-000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164c0: 2020 2275 7064 6174 655f 6461 7461 7365    "update_datase
-000164d0: 7422 2c20 6e65 775f 7368 6170 652c 2064  t", new_shape, d
-000164e0: 7479 7065 3d73 656c 662e 6474 7970 650a  type=self.dtype.
-000164f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016500: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00016510: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00016520: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016530: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
-00016540: 652e 6372 6561 7465 5f64 6174 6173 6574  e.create_dataset
-00016550: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00016560: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00016570: 7064 6174 655f 6461 7461 7365 7422 2c0a  pdate_dataset",.
-00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016590: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-000165a0: 653d 5f66 696c 655b 2264 6174 6173 6574  e=_file["dataset
-000165b0: 225d 2e73 6861 7065 2c0a 2020 2020 2020  "].shape,.      
-000165c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165d0: 2020 2020 2020 6474 7970 653d 5f66 696c        dtype=_fil
-000165e0: 655b 2264 6174 6173 6574 225d 2e64 7479  e["dataset"].dty
-000165f0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00016600: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016620: 2020 2020 2020 666f 7220 692c 2069 6d67        for i, img
-00016630: 2069 6e20 656e 756d 6572 6174 6528 5f66   in enumerate(_f
-00016640: 696c 655b 2264 6174 6173 6574 225d 293a  ile["dataset"]):
-00016650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016660: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
-00016670: 6c65 5b22 7570 6461 7465 5f64 6174 6173  le["update_datas
-00016680: 6574 225d 5b69 5d20 3d20 696d 670a 2020  et"][i] = img.  
-00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166a0: 2020 6461 7461 7365 745f 6e61 6d65 203d    dataset_name =
-000166b0: 2022 7570 6461 7465 5f64 6174 6173 6574   "update_dataset
-000166c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000166d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000166e0: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
-000166f0: 652e 6372 6561 7465 5f64 6174 6173 6574  e.create_dataset
-00016700: 2822 6461 7461 7365 7422 2c20 6e65 775f  ("dataset", new_
-00016710: 7368 6170 652c 2064 7479 7065 3d73 656c  shape, dtype=sel
-00016720: 662e 6474 7970 6529 0a0a 2020 2020 2020  f.dtype)..      
-00016730: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00016740: 696e 2069 6e64 6963 6573 3a0a 2020 2020  in indices:.    
+000129d0: 2020 2020 2073 7461 7274 5b31 5d20 3d20       start[1] = 
+000129e0: 6368 756e 6b5f 7368 6170 655b 315d 202a  chunk_shape[1] *
+000129f0: 2028 6a20 2b20 3129 0a20 2020 2020 2020   (j + 1).       
+00012a00: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00012a10: 7274 5b30 5d20 3d20 6368 756e 6b5f 7368  rt[0] = chunk_sh
+00012a20: 6170 655b 305d 202a 2028 6920 2b20 3129  ape[0] * (i + 1)
+00012a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a40: 2020 2020 2073 7461 7274 5b31 5d20 3d20       start[1] = 
+00012a50: 300a 2020 2020 2020 2020 2020 2020 656c  0.            el
+00012a60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012a70: 2020 2020 6669 7474 6564 5f64 6174 612c      fitted_data,
+00012a80: 206d 6170 7320 3d20 5f66 6974 280a 2020   maps = _fit(.  
+00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012aa0: 2020 6461 7461 2c0a 2020 2020 2020 2020    data,.        
+00012ab0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00012ac0: 6573 3d76 616c 7565 732c 0a20 2020 2020  es=values,.     
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012ae0: 6861 7065 3d73 6861 7065 2c0a 2020 2020  hape=shape,.    
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 696e 745f 7468 7265 7368 3d69 6e74 5f74  int_thresh=int_t
+00012b10: 6872 6573 682c 0a20 2020 2020 2020 2020  hresh,.         
+00012b20: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+00012b30: 6573 3d69 6e64 6963 6573 2c0a 2020 2020  es=indices,.    
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 5f74 7164 6d3d 5472 7565 2c0a 2020 2020  _tqdm=True,.    
+00012b60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012b70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00012b80: 7220 692c 2069 6d61 6765 2069 6e20 656e  r i, image in en
+00012b90: 756d 6572 6174 6528 6669 7474 6564 5f64  umerate(fitted_d
+00012ba0: 6174 6129 3a0a 2020 2020 2020 2020 2020  ata):.          
+00012bb0: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
+00012bc0: 6d65 203d 206f 732e 7061 7468 2e6a 6f69  me = os.path.joi
+00012bd0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00012be0: 2020 2020 2020 2020 2020 205f 6469 722c             _dir,
+00012bf0: 2022 6461 7461 5f66 6974 2220 2b20 7374   "data_fit" + st
+00012c00: 7228 696e 6469 6365 735b 695d 292e 7a66  r(indices[i]).zf
+00012c10: 696c 6c28 3429 202b 2022 2e6e 7079 220a  ill(4) + ".npy".
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00012c40: 2020 2020 2020 2020 2020 6e75 6d70 792e            numpy.
+00012c50: 7361 7665 2866 696c 656e 616d 652c 2069  save(filename, i
+00012c60: 6d61 6765 290a 2020 2020 2020 2020 2020  mage).          
+00012c70: 2020 2020 2020 2020 2020 7572 6c73 2e61            urls.a
+00012c80: 7070 656e 6428 4461 7461 5572 6c28 6669  ppend(DataUrl(fi
+00012c90: 6c65 5f70 6174 683d 6669 6c65 6e61 6d65  le_path=filename
+00012ca0: 2c20 7363 6865 6d65 3d22 6661 6269 6f22  , scheme="fabio"
+00012cb0: 2929 0a0a 2020 2020 2020 2020 6966 2069  ))..        if i
+00012cc0: 6e64 6963 6573 2069 7320 6e6f 7420 4e6f  ndices is not No
+00012cd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012ce0: 2320 5265 706c 6163 6520 6f6e 6c79 2066  # Replace only f
+00012cf0: 6974 7465 6420 6461 7461 2075 726c 730a  itted data urls.
+00012d00: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00012d10: 7572 6c73 203d 206e 756d 7079 2e61 7272  urls = numpy.arr
+00012d20: 6179 2873 656c 662e 6461 7461 2e75 726c  ay(self.data.url
+00012d30: 732c 2064 7479 7065 3d6f 626a 6563 7429  s, dtype=object)
+00012d40: 2e66 6c61 7474 656e 2829 0a20 2020 2020  .flatten().     
+00012d50: 2020 2020 2020 206e 756d 7079 2e70 7574         numpy.put
+00012d60: 286e 6577 5f75 726c 732c 2069 6e64 6963  (new_urls, indic
+00012d70: 6573 2c20 7572 6c73 290a 2020 2020 2020  es, urls).      
+00012d80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012d90: 2020 2020 6e65 775f 7572 6c73 203d 206e      new_urls = n
+00012da0: 756d 7079 2e61 7272 6179 2875 726c 7329  umpy.array(urls)
+00012db0: 0a0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+00012dc0: 2044 6174 6128 0a20 2020 2020 2020 2020   Data(.         
+00012dd0: 2020 206e 6577 5f75 726c 732e 7265 7368     new_urls.resh
+00012de0: 6170 6528 7365 6c66 2e64 6174 612e 7572  ape(self.data.ur
+00012df0: 6c73 2e73 6861 7065 292c 0a20 2020 2020  ls.shape),.     
+00012e00: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00012e10: 2e6d 6574 6164 6174 612c 0a20 2020 2020  .metadata,.     
+00012e20: 2020 2020 2020 2069 6e5f 6d65 6d6f 7279         in_memory
+00012e30: 3d73 656c 662e 5f69 6e5f 6d65 6d6f 7279  =self._in_memory
+00012e40: 2c0a 2020 2020 2020 2020 2920 2023 2074  ,.        )  # t
+00012e50: 6f20 6d6f 6469 6679 0a20 2020 2020 2020  o modify.       
+00012e60: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
+00012e70: 2020 2020 2020 4461 7461 7365 7428 0a20        Dataset(. 
+00012e80: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00012e90: 6469 723d 5f64 6972 2c0a 2020 2020 2020  dir=_dir,.      
+00012ea0: 2020 2020 2020 2020 2020 6461 7461 3d64            data=d
+00012eb0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00012ec0: 2020 2020 2064 696d 733d 7365 6c66 2e5f       dims=self._
+00012ed0: 5f64 696d 732c 0a20 2020 2020 2020 2020  _dims,.         
+00012ee0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00012ef0: 6174 696f 6e3d 7365 6c66 2e74 7261 6e73  ation=self.trans
+00012f00: 666f 726d 6174 696f 6e2c 0a20 2020 2020  formation,.     
+00012f10: 2020 2020 2020 2020 2020 2069 6e5f 6d65             in_me
+00012f20: 6d6f 7279 3d73 656c 662e 5f69 6e5f 6d65  mory=self._in_me
+00012f30: 6d6f 7279 2c0a 2020 2020 2020 2020 2020  mory,.          
+00012f40: 2020 2020 2020 7469 746c 653d 7365 6c66        title=self
+00012f50: 2e74 6974 6c65 2c0a 2020 2020 2020 2020  .title,.        
+00012f60: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00012f70: 2020 206d 6170 732c 0a20 2020 2020 2020     maps,.       
+00012f80: 2029 0a0a 2020 2020 6465 6620 636f 6d70   )..    def comp
+00012f90: 7574 655f 7472 616e 7366 6f72 6d61 7469  ute_transformati
+00012fa0: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
+00012fb0: 2c20 642c 206b 696e 643d 226d 6167 6e69  , d, kind="magni
+00012fc0: 6669 6361 7469 6f6e 222c 2072 6f74 6174  fication", rotat
+00012fd0: 653d 4661 6c73 652c 2074 6f70 6f67 7261  e=False, topogra
+00012fe0: 7068 793d 5b46 616c 7365 2c20 305d 2c20  phy=[False, 0], 
+00012ff0: 6365 6e74 6572 3d54 7275 650a 2020 2020  center=True.    
+00013000: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00013010: 2020 2020 2020 2043 6f6d 7075 7465 7320         Computes 
+00013020: 7472 616e 7366 6f72 6d61 7469 6f6e 206d  transformation m
+00013030: 6174 7269 782e 0a20 2020 2020 2020 2044  atrix..        D
+00013040: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+00013050: 6b69 6e64 206f 6620 7472 616e 7366 6f72  kind of transfor
+00013060: 6d61 7469 6f6e 2c20 636f 6d70 7574 6573  mation, computes
+00013070: 2065 6974 6865 7220 5253 4d20 6f72 206d   either RSM or m
+00013080: 6167 6e69 6669 6361 7469 6f6e 0a20 2020  agnification.   
+00013090: 2020 2020 2061 7865 7320 746f 2062 6520       axes to be 
+000130a0: 7573 6564 206f 6e20 6675 7475 7265 2077  used on future w
+000130b0: 6964 6765 7473 2e0a 0a20 2020 2020 2020  idgets...       
+000130c0: 203a 7061 7261 6d20 643a 2053 697a 6520   :param d: Size 
+000130d0: 6f66 2074 6865 2070 6978 656c 0a20 2020  of the pixel.   
+000130e0: 2020 2020 203a 7479 7065 2064 3a20 666c       :type d: fl
+000130f0: 6f61 740a 2020 2020 2020 2020 3a70 6172  oat.        :par
+00013100: 616d 206b 696e 643a 2054 7261 6e73 666f  am kind: Transfo
+00013110: 726d 6174 696f 6e20 746f 2061 7070 6c79  rmation to apply
+00013120: 2c20 6569 7468 6572 2027 6d61 676e 6966  , either 'magnif
+00013130: 6963 6174 696f 6e27 206f 7220 2772 736d  ication' or 'rsm
+00013140: 270a 2020 2020 2020 2020 3a74 7970 6520  '.        :type 
+00013150: 6b69 6e64 3a20 7374 720a 2020 2020 2020  kind: str.      
+00013160: 2020 3a70 6172 616d 2072 6f74 6174 653a    :param rotate:
+00013170: 2054 6f20 6265 2075 7365 6420 6f6e 6c79   To be used only
+00013180: 2077 6974 6820 6b69 6e64 3d27 7273 6d27   with kind='rsm'
+00013190: 2c20 6966 2054 7275 6520 7468 6520 696d  , if True the im
+000131a0: 6167 6573 2077 6974 680a 2020 2020 2020  ages with.      
+000131b0: 2020 2020 2020 7472 616e 7366 6f72 6d61        transforma
+000131c0: 7469 6f6e 2061 7265 2072 6f74 6174 6564  tion are rotated
+000131d0: 2039 3020 6465 6772 6565 732e 0a20 2020   90 degrees..   
+000131e0: 2020 2020 203a 7479 7065 2072 6f74 6174       :type rotat
+000131f0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00013200: 3a70 6172 616d 2074 6f70 6f67 7261 7068  :param topograph
+00013210: 793a 2054 6f20 6265 2075 7365 6420 6f6e  y: To be used on
+00013220: 6c79 2077 6974 6820 6b69 6e64 3d27 6d61  ly with kind='ma
+00013230: 676e 6966 6963 6174 696f 6e27 2c20 6966  gnification', if
+00013240: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00013250: 2020 6f62 7069 7463 6820 7661 6c75 6573    obpitch values
+00013260: 2061 7265 2064 6976 6964 6564 2062 7920   are divided by 
+00013270: 6974 7320 7369 6e65 2e0a 2020 2020 2020  its sine..      
+00013280: 2020 3a74 7970 6520 746f 706f 6772 6170    :type topograp
+00013290: 6879 3a20 626f 6f6c 0a20 2020 2020 2020  hy: bool.       
+000132a0: 2022 2222 0a0a 2020 2020 2020 2020 482c   """..        H,
+000132b0: 2057 203d 2073 656c 662e 6765 745f 6461   W = self.get_da
+000132c0: 7461 2830 292e 7368 6170 650a 2020 2020  ta(0).shape.    
+000132d0: 2020 2020 7365 6c66 2e72 6f74 6174 6520      self.rotate 
+000132e0: 3d20 726f 7461 7465 0a0a 2020 2020 2020  = rotate..      
+000132f0: 2020 6966 2073 656c 662e 6469 6d73 2e6e    if self.dims.n
+00013300: 6469 6d20 3d3d 2031 2061 6e64 206b 696e  dim == 1 and kin
+00013310: 6420 3d3d 2022 7273 6d22 3a0a 2020 2020  d == "rsm":.    
+00013320: 2020 2020 2020 2020 6666 7a20 3d20 7365          ffz = se
+00013330: 6c66 2e67 6574 5f6d 6574 6164 6174 615f  lf.get_metadata_
+00013340: 7661 6c75 6573 2850 4f53 4954 494f 4e45  values(POSITIONE
+00013350: 525f 4d45 5441 4441 5441 2c20 2266 667a  R_METADATA, "ffz
+00013360: 2229 5b30 5d0a 2020 2020 2020 2020 2020  ")[0].          
+00013370: 2020 6d61 696e 7820 3d20 2d73 656c 662e    mainx = -self.
+00013380: 6765 745f 6d65 7461 6461 7461 5f76 616c  get_metadata_val
+00013390: 7565 7328 504f 5349 5449 4f4e 4552 5f4d  ues(POSITIONER_M
+000133a0: 4554 4144 4154 412c 2022 6d61 696e 7822  ETADATA, "mainx"
+000133b0: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
+000133c0: 2078 2c20 7920 3d20 636f 6d70 7574 655f   x, y = compute_
+000133d0: 7273 6d28 482c 2057 2c20 642c 2066 667a  rsm(H, W, d, ffz
+000133e0: 2c20 6d61 696e 782c 2072 6f74 6174 6529  , mainx, rotate)
+000133f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00013400: 2020 2020 2020 2020 2020 206f 6278 203d             obx =
+00013410: 2073 656c 662e 6765 745f 6d65 7461 6461   self.get_metada
+00013420: 7461 5f76 616c 7565 7328 504f 5349 5449  ta_values(POSITI
+00013430: 4f4e 4552 5f4d 4554 4144 4154 412c 2022  ONER_METADATA, "
+00013440: 6f62 7822 295b 305d 0a20 2020 2020 2020  obx")[0].       
+00013450: 2020 2020 206f 6270 6974 6368 203d 206e       obpitch = n
+00013460: 756d 7079 2e75 6e69 7175 6528 0a20 2020  umpy.unique(.   
+00013470: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013480: 662e 6765 745f 6d65 7461 6461 7461 5f76  f.get_metadata_v
+00013490: 616c 7565 7328 504f 5349 5449 4f4e 4552  alues(POSITIONER
+000134a0: 5f4d 4554 4144 4154 412c 2022 6f62 7069  _METADATA, "obpi
+000134b0: 7463 6822 290a 2020 2020 2020 2020 2020  tch").          
+000134c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000134d0: 6f62 7069 7463 6820 3d20 6f62 7069 7463  obpitch = obpitc
+000134e0: 685b 6c65 6e28 6f62 7069 7463 6829 202f  h[len(obpitch) /
+000134f0: 2f20 325d 0a20 2020 2020 2020 2020 2020  / 2].           
+00013500: 206d 6169 6e78 203d 202d 7365 6c66 2e67   mainx = -self.g
+00013510: 6574 5f6d 6574 6164 6174 615f 7661 6c75  et_metadata_valu
+00013520: 6573 2850 4f53 4954 494f 4e45 525f 4d45  es(POSITIONER_ME
+00013530: 5441 4441 5441 2c20 226d 6169 6e78 2229  TADATA, "mainx")
+00013540: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00013550: 782c 2079 203d 2063 6f6d 7075 7465 5f6d  x, y = compute_m
+00013560: 6167 6e69 6669 6361 7469 6f6e 280a 2020  agnification(.  
+00013570: 2020 2020 2020 2020 2020 2020 2020 482c                H,
+00013580: 2057 2c20 642c 206f 6278 2c20 6f62 7069   W, d, obx, obpi
+00013590: 7463 682c 206d 6169 6e78 2c20 746f 706f  tch, mainx, topo
+000135a0: 6772 6170 6879 2c20 6365 6e74 6572 0a20  graphy, center. 
+000135b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000135c0: 2020 2020 2073 656c 662e 7472 616e 7366       self.transf
+000135d0: 6f72 6d61 7469 6f6e 203d 2054 7261 6e73  ormation = Trans
+000135e0: 666f 726d 6174 696f 6e28 6b69 6e64 2c20  formation(kind, 
+000135f0: 782c 2079 2c20 726f 7461 7465 290a 0a20  x, y, rotate).. 
+00013600: 2020 2064 6566 2070 726f 6a65 6374 5f64     def project_d
+00013610: 6174 6128 7365 6c66 2c20 6469 6d65 6e73  ata(self, dimens
+00013620: 696f 6e2c 2069 6e64 6963 6573 3d4e 6f6e  ion, indices=Non
+00013630: 652c 205f 6469 723d 4e6f 6e65 293a 0a20  e, _dir=None):. 
+00013640: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013650: 2020 2041 7070 6c69 6573 2061 2070 726f     Applies a pro
+00013660: 6a65 6374 696f 6e20 746f 2074 6865 2064  jection to the d
+00013670: 6174 612e 0a20 2020 2020 2020 2054 6865  ata..        The
+00013680: 206e 6577 2044 6174 6173 6574 2077 696c   new Dataset wil
+00013690: 6c20 6861 7665 2074 6865 2073 616d 6520  l have the same 
+000136a0: 7369 7a65 2061 7320 7468 6520 6368 6f73  size as the chos
+000136b0: 656e 2064 696d 656e 7369 6f6e 2c20 7768  en dimension, wh
+000136c0: 6572 650a 2020 2020 2020 2020 7468 6520  ere.        the 
+000136d0: 6461 7461 2069 7320 7072 6f6a 6563 7465  data is projecte
+000136e0: 6420 6f6e 2e0a 0a20 2020 2020 2020 203a  d on...        :
+000136f0: 7061 7261 6d20 6469 6d65 6e73 696f 6e3a  param dimension:
+00013700: 2044 696d 656e 7369 6f6e 7320 746f 2070   Dimensions to p
+00013710: 726f 6a65 6374 2074 6865 2064 6174 6120  roject the data 
+00013720: 6f6e 746f 0a20 2020 2020 2020 203a 7479  onto.        :ty
+00013730: 7065 2064 696d 656e 7369 6f6e 3a20 6172  pe dimension: ar
+00013740: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+00013750: 203a 7061 7261 6d20 696e 6469 6365 733a   :param indices:
+00013760: 2049 6e64 6963 6573 206f 6620 7468 6520   Indices of the 
+00013770: 696d 6167 6573 2074 6f20 7573 6520 666f  images to use fo
+00013780: 7220 7468 6520 7072 6f6a 6563 7469 6f6e  r the projection
+00013790: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+000137a0: 204e 6f6e 652c 2074 6865 2070 726f 6a65   None, the proje
+000137b0: 6374 696f 6e20 6973 2064 6f6e 6520 7573  ction is done us
+000137c0: 696e 6720 616c 6c20 6461 7461 2e0a 2020  ing all data..  
+000137d0: 2020 2020 2020 3a74 7970 6520 696e 6469        :type indi
+000137e0: 6365 733a 2055 6e69 6f6e 5b4e 6f6e 652c  ces: Union[None,
+000137f0: 2061 7272 6179 5f6c 696b 655d 0a20 2020   array_like].   
+00013800: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+00013810: 5f64 6972 3a20 4469 7265 6374 6f72 7920  _dir: Directory 
+00013820: 6669 6c65 6e61 6d65 2074 6f20 7361 7665  filename to save
+00013830: 2074 6865 206e 6577 2064 6174 610a 2020   the new data.  
+00013840: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00013850: 2020 205f 6469 7220 3d20 7365 6c66 2e64     _dir = self.d
+00013860: 6972 2069 6620 5f64 6972 2069 7320 4e6f  ir if _dir is No
+00013870: 6e65 2065 6c73 6520 5f64 6972 0a20 2020  ne else _dir.   
+00013880: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
+00013890: 285f 6469 722c 2065 7869 7374 5f6f 6b3d  (_dir, exist_ok=
+000138a0: 5472 7565 290a 0a20 2020 2020 2020 2064  True)..        d
+000138b0: 696d 7320 3d20 4163 7175 6973 6974 696f  ims = Acquisitio
+000138c0: 6e44 696d 7328 290a 2020 2020 2020 2020  nDims().        
+000138d0: 6966 206c 656e 2864 696d 656e 7369 6f6e  if len(dimension
+000138e0: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
+000138f0: 2020 2020 6178 6973 203d 2073 656c 662e      axis = self.
+00013900: 6469 6d73 2e6e 6469 6d20 2d20 6469 6d65  dims.ndim - dime
+00013910: 6e73 696f 6e5b 305d 202d 2031 0a20 2020  nsion[0] - 1.   
+00013920: 2020 2020 2020 2020 2064 696d 203d 2073           dim = s
+00013930: 656c 662e 6469 6d73 2e67 6574 2864 696d  elf.dims.get(dim
+00013940: 656e 7369 6f6e 5b30 5d29 0a20 2020 2020  ension[0]).     
+00013950: 2020 2020 2020 2064 6174 6120 3d20 5b5d         data = []
+00013960: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013970: 2069 2069 6e20 7261 6e67 6528 6469 6d2e   i in range(dim.
+00013980: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
+00013990: 2020 2020 2020 205f 7375 6d20 3d20 7365         _sum = se
+000139a0: 6c66 2e7a 7375 6d28 696e 6469 6365 733d  lf.zsum(indices=
+000139b0: 696e 6469 6365 732c 2064 696d 656e 7369  indices, dimensi
+000139c0: 6f6e 3d5b 6469 6d65 6e73 696f 6e5b 305d  on=[dimension[0]
+000139d0: 2c20 695d 290a 2020 2020 2020 2020 2020  , i]).          
+000139e0: 2020 2020 2020 6966 206c 656e 285f 7375        if len(_su
+000139f0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
+00013a00: 2020 2020 2020 2020 6461 7461 202b 3d20          data += 
+00013a10: 5b5f 7375 6d5d 0a20 2020 2020 2020 2020  [_sum].         
+00013a20: 2020 2064 696d 732e 6164 645f 6469 6d28     dims.add_dim(
+00013a30: 302c 2064 696d 290a 2020 2020 2020 2020  0, dim).        
+00013a40: 656c 6966 206c 656e 2864 696d 656e 7369  elif len(dimensi
+00013a50: 6f6e 2920 3d3d 2032 3a0a 2020 2020 2020  on) == 2:.      
+00013a60: 2020 2020 2020 6178 6973 203d 2069 6e74        axis = int
+00013a70: 286e 756d 7079 2e73 6574 6469 6666 3164  (numpy.setdiff1d
+00013a80: 2872 616e 6765 2873 656c 662e 6469 6d73  (range(self.dims
+00013a90: 2e6e 6469 6d29 2c20 6469 6d65 6e73 696f  .ndim), dimensio
+00013aa0: 6e29 5b30 5d29 0a20 2020 2020 2020 2020  n)[0]).         
+00013ab0: 2020 2064 696d 3120 3d20 7365 6c66 2e64     dim1 = self.d
+00013ac0: 696d 732e 6765 7428 6469 6d65 6e73 696f  ims.get(dimensio
+00013ad0: 6e5b 305d 290a 2020 2020 2020 2020 2020  n[0]).          
+00013ae0: 2020 6469 6d32 203d 2073 656c 662e 6469    dim2 = self.di
+00013af0: 6d73 2e67 6574 2864 696d 656e 7369 6f6e  ms.get(dimension
+00013b00: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+00013b10: 2064 696d 732e 6164 645f 6469 6d28 302c   dims.add_dim(0,
+00013b20: 2064 696d 3129 0a20 2020 2020 2020 2020   dim1).         
+00013b30: 2020 2064 696d 732e 6164 645f 6469 6d28     dims.add_dim(
+00013b40: 312c 2064 696d 3229 0a20 2020 2020 2020  1, dim2).       
+00013b50: 2020 2020 2064 6174 6120 3d20 5b5d 0a20       data = []. 
+00013b60: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00013b70: 2069 6e20 7261 6e67 6528 6469 6d31 2e73   in range(dim1.s
+00013b80: 697a 6529 3a0a 2020 2020 2020 2020 2020  ize):.          
+00013b90: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+00013ba0: 616e 6765 2864 696d 322e 7369 7a65 293a  ange(dim2.size):
+00013bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013bc0: 2020 2020 205f 7375 6d20 3d20 7365 6c66       _sum = self
+00013bd0: 2e7a 7375 6d28 696e 6469 6365 733d 696e  .zsum(indices=in
+00013be0: 6469 6365 732c 2064 696d 656e 7369 6f6e  dices, dimension
+00013bf0: 3d5b 6469 6d65 6e73 696f 6e2c 205b 692c  =[dimension, [i,
+00013c00: 206a 5d5d 290a 2020 2020 2020 2020 2020   j]]).          
+00013c10: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00013c20: 285f 7375 6d29 3a0a 2020 2020 2020 2020  (_sum):.        
+00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c40: 6461 7461 202b 3d20 5b5f 7375 6d5d 0a20  data += [_sum]. 
+00013c50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013c60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013c70: 5661 6c75 6545 7272 6f72 2822 4f6e 6c79  ValueError("Only
+00013c80: 2031 4420 616e 6420 3244 2070 726f 6a65   1D and 2D proje
+00013c90: 6374 696f 6e20 6973 2061 6c6c 6f77 6564  ction is allowed
+00013ca0: 2229 0a20 2020 2020 2020 2064 696d 203d  ").        dim =
+00013cb0: 2073 656c 662e 6469 6d73 2e67 6574 2861   self.dims.get(a
+00013cc0: 7869 7329 0a20 2020 2020 2020 2064 6174  xis).        dat
+00013cd0: 6120 3d20 6e75 6d70 792e 6172 7261 7928  a = numpy.array(
+00013ce0: 6461 7461 292e 7669 6577 2844 6174 6129  data).view(Data)
+00013cf0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+00013d00: 6120 3d20 6e75 6d70 792e 7377 6170 6178  a = numpy.swapax
+00013d10: 6573 2873 656c 662e 6461 7461 2e6d 6574  es(self.data.met
+00013d20: 6164 6174 612c 2073 656c 662e 6469 6d73  adata, self.dims
+00013d30: 2e6e 6469 6d20 2d20 312c 2061 7869 7329  .ndim - 1, axis)
+00013d40: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00013d50: 6e20 7261 6e67 6528 7365 6c66 2e64 696d  n range(self.dim
+00013d60: 732e 6e64 696d 202d 206c 656e 2864 696d  s.ndim - len(dim
+00013d70: 656e 7369 6f6e 2929 3a0a 2020 2020 2020  ension)):.      
+00013d80: 2020 2020 2020 6d65 7461 6461 7461 203d        metadata =
+00013d90: 206d 6574 6164 6174 615b 305d 0a20 2020   metadata[0].   
+00013da0: 2020 2020 2064 6174 612e 7361 7665 280a       data.save(.
+00013db0: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
+00013dc0: 6174 682e 6a6f 696e 285f 6469 722c 2022  ath.join(_dir, "
+00013dd0: 7072 6f6a 6563 745f 2220 2b20 6469 6d2e  project_" + dim.
+00013de0: 6e61 6d65 202b 2022 2e68 6466 3522 292c  name + ".hdf5"),
+00013df0: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
+00013e00: 6d65 6d6f 7279 3d73 656c 662e 5f69 6e5f  memory=self._in_
+00013e10: 6d65 6d6f 7279 2c0a 2020 2020 2020 2020  memory,.        
+00013e20: 290a 2020 2020 2020 2020 6461 7461 2e6d  ).        data.m
+00013e30: 6574 6164 6174 6120 3d20 6d65 7461 6461  etadata = metada
+00013e40: 7461 0a0a 2020 2020 2020 2020 6461 7461  ta..        data
+00013e50: 7365 7420 3d20 4461 7461 7365 7428 0a20  set = Dataset(. 
+00013e60: 2020 2020 2020 2020 2020 205f 6469 723d             _dir=
+00013e70: 5f64 6972 2c0a 2020 2020 2020 2020 2020  _dir,.          
+00013e80: 2020 6461 7461 3d64 6174 612c 0a20 2020    data=data,.   
+00013e90: 2020 2020 2020 2020 2064 696d 733d 6469           dims=di
+00013ea0: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
+00013eb0: 7472 616e 7366 6f72 6d61 7469 6f6e 3d73  transformation=s
+00013ec0: 656c 662e 7472 616e 7366 6f72 6d61 7469  elf.transformati
+00013ed0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00013ee0: 696e 5f6d 656d 6f72 793d 7365 6c66 2e5f  in_memory=self._
+00013ef0: 696e 5f6d 656d 6f72 792c 0a20 2020 2020  in_memory,.     
+00013f00: 2020 2020 2020 2074 6974 6c65 3d73 656c         title=sel
+00013f10: 662e 7469 746c 652c 0a20 2020 2020 2020  f.title,.       
+00013f20: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00013f30: 726e 2064 6174 6173 6574 2e72 6573 6861  rn dataset.resha
+00013f40: 7065 5f64 6174 6128 290a 0a20 2020 2064  pe_data()..    d
+00013f50: 6566 2063 6f6d 7075 7465 5f72 736d 280a  ef compute_rsm(.
+00013f60: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00013f70: 2020 2020 2020 512c 0a20 2020 2020 2020        Q,.       
+00013f80: 2061 2c0a 2020 2020 2020 2020 6d61 705f   a,.        map_
+00013f90: 7261 6e67 652c 0a20 2020 2020 2020 2070  range,.        p
+00013fa0: 6978 656c 5f73 697a 652c 0a20 2020 2020  ixel_size,.     
+00013fb0: 2020 2075 6e69 7473 2c0a 2020 2020 2020     units,.      
+00013fc0: 2020 6e2c 0a20 2020 2020 2020 206d 6170    n,.        map
+00013fd0: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
+00013fe0: 656e 6572 6779 3d31 372c 0a20 2020 2020  energy=17,.     
+00013ff0: 2020 2074 7261 6e73 666f 726d 6174 696f     transformatio
+00014000: 6e3d 4e6f 6e65 2c0a 2020 2020 293a 0a20  n=None,.    ):. 
+00014010: 2020 2020 2020 2064 6966 6672 7920 3d20         diffry = 
+00014020: 7365 6c66 2e67 6574 5f6d 6574 6164 6174  self.get_metadat
+00014030: 615f 7661 6c75 6573 2850 4f53 4954 494f  a_values(POSITIO
+00014040: 4e45 525f 4d45 5441 4441 5441 2c20 2264  NER_METADATA, "d
+00014050: 6966 6672 7922 290a 2020 2020 2020 2020  iffry").        
+00014060: 6966 2074 7261 6e73 666f 726d 6174 696f  if transformatio
+00014070: 6e20 6973 204e 6f6e 6520 616e 6420 7365  n is None and se
+00014080: 6c66 2e74 7261 6e73 666f 726d 6174 696f  lf.transformatio
+00014090: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+000140a0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+000140b0: 666f 726d 6174 696f 6e20 3d20 7365 6c66  formation = self
+000140c0: 2e74 7261 6e73 666f 726d 6174 696f 6e0a  .transformation.
+000140d0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+000140e0: 662e 7472 616e 7366 6f72 6d61 7469 6f6e  f.transformation
+000140f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00014100: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00014110: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00014120: 2020 2020 2020 2020 2254 7261 6e73 666f          "Transfo
+00014130: 726d 6174 696f 6e20 6861 7320 746f 2066  rmation has to f
+00014140: 6972 7374 2062 6520 636f 6d70 7574 6564  irst be computed
+00014150: 2075 7369 6e67 2074 6865 2054 7261 6e73   using the Trans
+00014160: 666f 726d 6174 696f 6e20 5769 6467 6574  formation Widget
+00014170: 2028 6265 666f 7265 2061 6e79 2052 4f49   (before any ROI
+00014180: 2922 0a20 2020 2020 2020 2020 2020 2029  )".            )
+00014190: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000141a0: 2063 616c 6375 6c61 7465 5f52 534d 5f68   calculate_RSM_h
+000141b0: 6973 746f 6772 616d 280a 2020 2020 2020  istogram(.      
+000141c0: 2020 2020 2020 6461 7461 3d73 656c 662e        data=self.
+000141d0: 6765 745f 6461 7461 2829 2c0a 2020 2020  get_data(),.    
+000141e0: 2020 2020 2020 2020 6469 6666 7279 5f76          diffry_v
+000141f0: 616c 7565 733d 6469 6666 7279 2c0a 2020  alues=diffry,.  
+00014200: 2020 2020 2020 2020 2020 7477 6f74 6865            twothe
+00014210: 7461 3d74 7261 6e73 666f 726d 6174 696f  ta=transformatio
+00014220: 6e2e 792c 0a20 2020 2020 2020 2020 2020  n.y,.           
+00014230: 2065 7461 3d74 7261 6e73 666f 726d 6174   eta=transformat
+00014240: 696f 6e2e 782c 0a20 2020 2020 2020 2020  ion.x,.         
+00014250: 2020 2051 3d51 2c0a 2020 2020 2020 2020     Q=Q,.        
+00014260: 2020 2020 613d 612c 0a20 2020 2020 2020      a=a,.       
+00014270: 2020 2020 206d 6170 5f72 616e 6765 3d6d       map_range=m
+00014280: 6170 5f72 616e 6765 2c0a 2020 2020 2020  ap_range,.      
+00014290: 2020 2020 2020 756e 6974 733d 756e 6974        units=unit
+000142a0: 732c 0a20 2020 2020 2020 2020 2020 206d  s,.            m
+000142b0: 6170 5f73 6861 7065 3d6d 6170 5f73 6861  ap_shape=map_sha
+000142c0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+000142d0: 6e3d 6e2c 0a20 2020 2020 2020 2020 2020  n=n,.           
+000142e0: 2045 3d65 6e65 7267 792c 0a20 2020 2020   E=energy,.     
+000142f0: 2020 2029 0a0a 2020 2020 6465 6620 6170     )..    def ap
+00014300: 706c 795f 6269 6e6e 696e 6728 7365 6c66  ply_binning(self
+00014310: 2c20 7363 616c 652c 205f 6469 723d 4e6f  , scale, _dir=No
+00014320: 6e65 293a 0a20 2020 2020 2020 205f 6469  ne):.        _di
+00014330: 7220 3d20 7365 6c66 2e64 6972 2069 6620  r = self.dir if 
+00014340: 5f64 6972 2069 7320 4e6f 6e65 2065 6c73  _dir is None els
+00014350: 6520 5f64 6972 0a20 2020 2020 2020 206f  e _dir.        o
+00014360: 732e 6d61 6b65 6469 7273 285f 6469 722c  s.makedirs(_dir,
+00014370: 2065 7869 7374 5f6f 6b3d 5472 7565 290a   exist_ok=True).
+00014380: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00014390: 7265 7363 616c 655f 6461 7461 2873 656c  rescale_data(sel
+000143a0: 662e 6765 745f 6461 7461 2829 2c20 7363  f.get_data(), sc
+000143b0: 616c 6529 0a20 2020 2020 2020 2073 6861  ale).        sha
+000143c0: 7065 203d 2064 6174 612e 7368 6170 650a  pe = data.shape.
+000143d0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000143e0: 6174 612e 7669 6577 2844 6174 6129 0a20  ata.view(Data). 
+000143f0: 2020 2020 2020 2064 6174 612e 7361 7665         data.save
+00014400: 280a 2020 2020 2020 2020 2020 2020 6f73  (.            os
+00014410: 2e70 6174 682e 6a6f 696e 285f 6469 722c  .path.join(_dir,
+00014420: 2022 6269 6e6e 6564 5f64 6174 612e 6864   "binned_data.hd
+00014430: 6635 2229 2c0a 2020 2020 2020 2020 2020  f5"),.          
+00014440: 2020 696e 5f6d 656d 6f72 793d 7365 6c66    in_memory=self
+00014450: 2e5f 696e 5f6d 656d 6f72 792c 0a20 2020  ._in_memory,.   
+00014460: 2020 2020 2020 2020 206e 6577 5f73 6861           new_sha
+00014470: 7065 3d73 6861 7065 2c0a 2020 2020 2020  pe=shape,.      
+00014480: 2020 290a 2020 2020 2020 2020 6461 7461    ).        data
+00014490: 2e6d 6574 6164 6174 6120 3d20 7365 6c66  .metadata = self
+000144a0: 2e64 6174 612e 6d65 7461 6461 7461 0a20  .data.metadata. 
+000144b0: 2020 2020 2020 2073 6861 7065 203d 206c         shape = l
+000144c0: 6973 7428 7365 6c66 2e64 6174 612e 7368  ist(self.data.sh
+000144d0: 6170 6529 5b3a 2d32 5d0a 2020 2020 2020  ape)[:-2].      
+000144e0: 2020 7368 6170 652e 6170 7065 6e64 2864    shape.append(d
+000144f0: 6174 612e 7368 6170 655b 2d32 5d29 0a20  ata.shape[-2]). 
+00014500: 2020 2020 2020 2073 6861 7065 2e61 7070         shape.app
+00014510: 656e 6428 6461 7461 2e73 6861 7065 5b2d  end(data.shape[-
+00014520: 315d 290a 2020 2020 2020 2020 6461 7461  1]).        data
+00014530: 203d 2064 6174 612e 7265 7368 6170 6528   = data.reshape(
+00014540: 7368 6170 6529 0a0a 2020 2020 2020 2020  shape)..        
+00014550: 7265 7475 726e 2044 6174 6173 6574 280a  return Dataset(.
+00014560: 2020 2020 2020 2020 2020 2020 5f64 6972              _dir
+00014570: 3d5f 6469 722c 0a20 2020 2020 2020 2020  =_dir,.         
+00014580: 2020 2064 6174 613d 6461 7461 2c0a 2020     data=data,.  
+00014590: 2020 2020 2020 2020 2020 6469 6d73 3d73            dims=s
+000145a0: 656c 662e 6469 6d73 2c0a 2020 2020 2020  elf.dims,.      
+000145b0: 2020 2020 2020 7472 616e 7366 6f72 6d61        transforma
+000145c0: 7469 6f6e 3d73 656c 662e 7472 616e 7366  tion=self.transf
+000145d0: 6f72 6d61 7469 6f6e 2c0a 2020 2020 2020  ormation,.      
+000145e0: 2020 2020 2020 696e 5f6d 656d 6f72 793d        in_memory=
+000145f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00014600: 2020 7469 746c 653d 7365 6c66 2e74 6974    title=self.tit
+00014610: 6c65 2c0a 2020 2020 2020 2020 290a 0a20  le,.        ).. 
+00014620: 2020 2064 6566 2072 6563 6f76 6572 5f77     def recover_w
+00014630: 6561 6b5f 6265 616d 2873 656c 662c 206e  eak_beam(self, n
+00014640: 2c20 696e 6469 6365 733d 4e6f 6e65 293a  , indices=None):
+00014650: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014660: 2020 2020 2053 6574 2074 6f20 7a65 726f       Set to zero
+00014670: 2061 6c6c 2070 6978 656c 7320 6869 6768   all pixels high
+00014680: 6572 2074 6861 6e20 6e20 7469 6d65 7320  er than n times 
+00014690: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
+000146a0: 6961 7469 6f6e 2061 6372 6f73 7320 7468  iation across th
+000146b0: 6520 7374 6163 6b20 6469 6d65 6e73 696f  e stack dimensio
+000146c0: 6e0a 0a20 2020 2020 2020 203a 7061 7261  n..        :para
+000146d0: 6d20 6e3a 2049 6e63 7265 6173 6520 6f72  m n: Increase or
+000146e0: 2064 6563 7265 6173 6520 7468 6520 746f   decrease the to
+000146f0: 7020 7468 7265 7368 6f6c 6420 6279 2074  p threshold by t
+00014700: 6869 7320 6669 7865 6420 7661 6c75 652e  his fixed value.
+00014710: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+00014720: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+00014730: 3a70 6172 616d 2069 6e64 6963 6573 3a20  :param indices: 
+00014740: 496e 6469 6365 7320 6f66 2074 6865 2069  Indices of the i
+00014750: 6d61 6765 7320 746f 2075 7365 2066 6f72  mages to use for
+00014760: 2074 6865 2066 696c 7465 7269 6e67 2e0a   the filtering..
+00014770: 2020 2020 2020 2020 2020 2020 4966 204e              If N
+00014780: 6f6e 652c 2074 6865 2066 696c 7465 7269  one, the filteri
+00014790: 6e67 2069 7320 646f 6e65 2075 7369 6e67  ng is done using
+000147a0: 2061 6c6c 2064 6174 612e 0a20 2020 2020   all data..     
+000147b0: 2020 203a 7479 7065 2069 6e64 6963 6573     :type indices
+000147c0: 3a20 556e 696f 6e5b 4e6f 6e65 2c20 6172  : Union[None, ar
+000147d0: 7261 795f 6c69 6b65 5d0a 2020 2020 2020  ray_like].      
+000147e0: 2020 2222 220a 2020 2020 2020 2020 7374    """.        st
+000147f0: 6420 3d20 6e75 6d70 792e 7374 6428 7365  d = numpy.std(se
+00014800: 6c66 2e67 6574 5f64 6174 6128 696e 6469  lf.get_data(indi
+00014810: 6365 7329 2e76 6965 7728 6e75 6d70 792e  ces).view(numpy.
+00014820: 6e64 6172 7261 7929 2c20 6178 6973 3d30  ndarray), axis=0
+00014830: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00014840: 6e20 7365 6c66 2e61 7070 6c79 5f74 6872  n self.apply_thr
+00014850: 6573 686f 6c64 5f72 656d 6f76 616c 2874  eshold_removal(t
+00014860: 6f70 3d6e 202a 2073 7464 2c20 696e 6469  op=n * std, indi
+00014870: 6365 733d 696e 6469 6365 7329 0a0a 2020  ces=indices)..  
+00014880: 2020 6465 6620 5f5f 6465 6570 636f 7079    def __deepcopy
+00014890: 5f5f 2873 656c 662c 206d 656d 6f29 3a0a  __(self, memo):.
+000148a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000148b0: 2020 2020 4372 6561 7465 2063 6f70 7920      Create copy 
+000148c0: 6f66 2074 6865 2064 6174 6173 6574 2e20  of the dataset. 
+000148d0: 5468 6520 6461 7461 206e 756d 7079 2061  The data numpy a
+000148e0: 7272 6179 2069 7320 616c 736f 2063 6f70  rray is also cop
+000148f0: 6965 6420 7573 696e 670a 2020 2020 2020  ied using.      
+00014900: 2020 6465 6570 2063 6f70 792e 2054 6865    deep copy. The
+00014910: 2072 6573 7420 6f66 2074 6865 2061 7474   rest of the att
+00014920: 7269 6275 7465 7320 6172 6520 7468 6520  ributes are the 
+00014930: 7361 6d65 2e0a 2020 2020 2020 2020 2222  same..        ""
+00014940: 220a 2020 2020 2020 2020 6461 7461 7365  ".        datase
+00014950: 7420 3d20 7479 7065 2873 656c 6629 280a  t = type(self)(.
+00014960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014970: 2e64 6972 2c0a 2020 2020 2020 2020 2020  .dir,.          
+00014980: 2020 6461 7461 3d73 656c 662e 6461 7461    data=self.data
+00014990: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000149a0: 6d73 3d73 656c 662e 5f5f 6469 6d73 2c0a  ms=self.__dims,.
+000149b0: 2020 2020 2020 2020 2020 2020 696e 5f6d              in_m
+000149c0: 656d 6f72 793d 7365 6c66 2e69 6e5f 6d65  emory=self.in_me
+000149d0: 6d6f 7279 2c0a 2020 2020 2020 2020 2020  mory,.          
+000149e0: 2020 636f 7079 5f66 696c 6573 3d54 7275    copy_files=Tru
+000149f0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+00014a00: 2020 2020 2064 6174 6173 6574 2e64 696d       dataset.dim
+00014a10: 7320 3d20 636f 7079 2e64 6565 7063 6f70  s = copy.deepcop
+00014a20: 7928 7365 6c66 2e5f 5f64 696d 732c 206d  y(self.__dims, m
+00014a30: 656d 6f29 0a20 2020 2020 2020 2072 6574  emo).        ret
+00014a40: 7572 6e20 6461 7461 7365 740a 0a0a 636c  urn dataset...cl
+00014a50: 6173 7320 4461 7461 286e 756d 7079 2e6e  ass Data(numpy.n
+00014a60: 6461 7272 6179 293a 0a20 2020 2022 2222  darray):.    """
+00014a70: 0a20 2020 2043 6c61 7373 2074 6f20 7374  .    Class to st
+00014a80: 7275 6374 7572 6520 7468 6520 6461 7461  ructure the data
+00014a90: 2061 6e64 206c 696e 6b20 6576 6572 7920   and link every 
+00014aa0: 696d 6167 6520 7769 7468 2069 7473 2063  image with its c
+00014ab0: 6f72 7265 7370 6f6e 6469 6e67 2075 726c  orresponding url
+00014ac0: 2061 6e64 0a20 2020 206d 6574 6164 6174   and.    metadat
+00014ad0: 612e 2049 7420 696e 6865 7269 7473 2066  a. It inherits f
+00014ae0: 726f 6d20 6e75 6d70 792e 6e64 6172 7261  rom numpy.ndarra
+00014af0: 7920 616e 6420 4f76 6572 7269 6465 7320  y and Overrides 
+00014b00: 7468 6520 6e65 6365 7373 6172 7920 6d65  the necessary me
+00014b10: 7468 6f64 732c 0a20 2020 2074 616b 696e  thods,.    takin
+00014b20: 6720 696e 746f 2061 6363 6f75 6e74 2074  g into account t
+00014b30: 6865 2060 696e 5f6d 656d 6f72 7960 2061  he `in_memory` a
+00014b40: 7474 7269 6275 7465 2e0a 0a20 2020 203a  ttribute...    :
+00014b50: 7061 7261 6d20 7572 6c73 3a20 4172 7261  param urls: Arra
+00014b60: 7920 7769 7468 2074 6865 2075 726c 7320  y with the urls 
+00014b70: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
+00014b80: 3a74 7970 6520 7572 6c73 3a20 6172 7261  :type urls: arra
+00014b90: 795f 6c69 6b65 0a20 2020 203a 7061 7261  y_like.    :para
+00014ba0: 6d20 6d65 7461 6461 7461 3a20 4172 7261  m metadata: Arra
+00014bb0: 7920 7769 7468 2074 6865 206d 6574 6164  y with the metad
+00014bc0: 6174 6120 6f66 2074 6865 2064 6174 610a  ata of the data.
+00014bd0: 2020 2020 3a74 7970 6520 6d65 7461 6461      :type metada
+00014be0: 7461 3a20 6172 7261 795f 6c69 6b65 0a20  ta: array_like. 
+00014bf0: 2020 203a 7061 7261 6d20 696e 5f6d 656d     :param in_mem
+00014c00: 6f72 793a 2049 6620 5472 7565 2c20 7468  ory: If True, th
+00014c10: 6520 6461 7461 2069 7320 6c6f 6164 6564  e data is loaded
+00014c20: 2069 6e74 6f20 6d65 6d6f 7279 2c20 6465   into memory, de
+00014c30: 6661 756c 7420 5472 7565 0a20 2020 203a  fault True.    :
+00014c40: 7479 7065 2069 6e5f 6d65 6d6f 7279 3a20  type in_memory: 
+00014c50: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
+00014c60: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00014c70: 5f5f 6e65 775f 5f28 636c 732c 2075 726c  __new__(cls, url
+00014c80: 732c 206d 6574 6164 6174 612c 2069 6e5f  s, metadata, in_
+00014c90: 6d65 6d6f 7279 3d54 7275 652c 2064 6174  memory=True, dat
+00014ca0: 613d 4e6f 6e65 293a 0a20 2020 2020 2020  a=None):.       
+00014cb0: 2075 726c 7320 3d20 6e75 6d70 792e 6173   urls = numpy.as
+00014cc0: 6172 7261 7928 7572 6c73 290a 2020 2020  array(urls).    
+00014cd0: 2020 2020 696d 675f 7368 6170 6520 3d20      img_shape = 
+00014ce0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00014cf0: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
+00014d00: 2020 2020 2020 2023 204c 6f61 6420 616c         # Load al
+00014d10: 6c20 696d 6167 6573 2069 6e20 6d65 6d6f  l images in memo
+00014d20: 7279 0a20 2020 2020 2020 2020 2020 2069  ry.            i
+00014d30: 6620 6461 7461 2069 7320 6e6f 7420 4e6f  f data is not No
+00014d40: 6e65 2061 6e64 2075 726c 732e 7368 6170  ne and urls.shap
+00014d50: 6520 213d 2064 6174 612e 7368 6170 655b  e != data.shape[
+00014d60: 3a2d 325d 3a0a 2020 2020 2020 2020 2020  :-2]:.          
+00014d70: 2020 2020 2020 6461 7461 203d 204e 6f6e        data = Non
+00014d80: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+00014d90: 2064 6174 6120 6973 204e 6f6e 653a 0a20   data is None:. 
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00014db0: 726c 5f73 6861 7065 203d 2075 726c 732e  rl_shape = urls.
+00014dc0: 7368 6170 650a 2020 2020 2020 2020 2020  shape.          
+00014dd0: 2020 2020 2020 7572 6c5f 6964 7873 203d        url_idxs =
+00014de0: 206e 756d 7079 2e75 6e72 6176 656c 5f69   numpy.unravel_i
+00014df0: 6e64 6578 286e 756d 7079 2e61 7261 6e67  ndex(numpy.arang
+00014e00: 6528 7572 6c73 2e73 697a 6529 2c20 7572  e(urls.size), ur
+00014e10: 6c5f 7368 6170 6529 0a20 2020 2020 2020  l_shape).       
+00014e20: 2020 2020 2020 2020 2069 6620 7572 6c73           if urls
+00014e30: 2e73 697a 6520 3d3d 2030 3a0a 2020 2020  .size == 0:.    
+00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e50: 6461 7461 203d 206e 756d 7079 2e65 6d70  data = numpy.emp
+00014e60: 7479 2875 726c 5f73 6861 7065 202b 2028  ty(url_shape + (
+00014e70: 302c 2030 2929 0a20 2020 2020 2020 2020  0, 0)).         
+00014e80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 2069 6d67 203d 2075 7469 6c73 2e67 6574   img = utils.get
+00014eb0: 5f64 6174 6128 6e65 7874 2875 726c 732e  _data(next(urls.
+00014ec0: 666c 6174 2929 0a20 2020 2020 2020 2020  flat)).         
+00014ed0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00014ee0: 3d20 6e75 6d70 792e 656d 7074 7928 7572  = numpy.empty(ur
+00014ef0: 6c5f 7368 6170 6520 2b20 696d 672e 7368  l_shape + img.sh
+00014f00: 6170 652c 2069 6d67 2e64 7479 7065 290a  ape, img.dtype).
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2020 666f 7220 7572 6c2c 202a 7572      for url, *ur
+00014f30: 6c5f 6964 7820 696e 207a 6970 2875 726c  l_idx in zip(url
+00014f40: 732e 666c 6174 2c20 2a75 726c 5f69 6478  s.flat, *url_idx
+00014f50: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00014f60: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00014f70: 5b74 7570 6c65 2875 726c 5f69 6478 295d  [tuple(url_idx)]
+00014f80: 203d 2075 7469 6c73 2e67 6574 5f64 6174   = utils.get_dat
+00014f90: 6128 7572 6c29 0a20 2020 2020 2020 2020  a(url).         
+00014fa0: 2020 206f 626a 203d 2064 6174 612e 7669     obj = data.vi
+00014fb0: 6577 2863 6c73 290a 2020 2020 2020 2020  ew(cls).        
+00014fc0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014fd0: 2020 2320 4163 6365 7373 2069 6d61 6765    # Access image
+00014fe0: 206f 6e65 2061 7420 6120 7469 6d65 2075   one at a time u
+00014ff0: 7369 6e67 2075 726c 0a20 2020 2020 2020  sing url.       
+00015000: 2020 2020 206f 626a 203d 2073 7570 6572       obj = super
+00015010: 2829 2e5f 5f6e 6577 5f5f 2863 6c73 2c20  ().__new__(cls, 
+00015020: 7572 6c73 2e73 6861 7065 290a 0a20 2020  urls.shape)..   
+00015030: 2020 2020 206f 626a 2e69 6e5f 6d65 6d6f       obj.in_memo
+00015040: 7279 203d 2069 6e5f 6d65 6d6f 7279 0a20  ry = in_memory. 
+00015050: 2020 2020 2020 206f 626a 2e75 726c 7320         obj.urls 
+00015060: 3d20 7572 6c73 0a20 2020 2020 2020 206f  = urls.        o
+00015070: 626a 2e6d 6574 6164 6174 6120 3d20 6e75  bj.metadata = nu
+00015080: 6d70 792e 6173 6172 7261 7928 6d65 7461  mpy.asarray(meta
+00015090: 6461 7461 290a 2020 2020 2020 2020 6f62  data).        ob
+000150a0: 6a2e 5f66 696c 6520 3d20 4e6f 6e65 0a20  j._file = None. 
+000150b0: 2020 2020 2020 206f 626a 2e5f 696d 675f         obj._img_
+000150c0: 7368 6170 6520 3d20 696d 675f 7368 6170  shape = img_shap
+000150d0: 650a 2020 2020 2020 2020 6f62 6a2e 7374  e.        obj.st
+000150e0: 6174 655f 6f66 5f6f 7065 7261 7469 6f6e  ate_of_operation
+000150f0: 7320 3d20 5f53 7461 7465 4f66 4f70 6572  s = _StateOfOper
+00015100: 6174 696f 6e73 2829 0a0a 2020 2020 2020  ations()..      
+00015110: 2020 7265 7475 726e 206f 626a 0a0a 2020    return obj..  
+00015120: 2020 6465 6620 5f5f 6172 7261 795f 6669    def __array_fi
+00015130: 6e61 6c69 7a65 5f5f 2873 656c 662c 206f  nalize__(self, o
+00015140: 626a 293a 0a20 2020 2020 2020 2069 6620  bj):.        if 
+00015150: 6f62 6a20 6973 204e 6f6e 653a 0a20 2020  obj is None:.   
+00015160: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00015170: 2020 2020 2020 2020 7365 6c66 2e75 726c          self.url
+00015180: 7320 3d20 6765 7461 7474 7228 6f62 6a2c  s = getattr(obj,
+00015190: 2022 7572 6c73 222c 204e 6f6e 6529 0a20   "urls", None). 
+000151a0: 2020 2020 2020 2073 656c 662e 6d65 7461         self.meta
+000151b0: 6461 7461 203d 2067 6574 6174 7472 286f  data = getattr(o
+000151c0: 626a 2c20 226d 6574 6164 6174 6122 2c20  bj, "metadata", 
+000151d0: 4e6f 6e65 290a 2020 2020 2020 2020 7365  None).        se
+000151e0: 6c66 2e69 6e5f 6d65 6d6f 7279 203d 2067  lf.in_memory = g
+000151f0: 6574 6174 7472 286f 626a 2c20 2269 6e5f  etattr(obj, "in_
+00015200: 6d65 6d6f 7279 222c 204e 6f6e 6529 0a0a  memory", None)..
+00015210: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00015220: 6d5f 5f28 7365 6c66 2c20 696e 6469 6365  m__(self, indice
+00015230: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
+00015240: 2020 2020 2020 2020 5265 7475 726e 2073          Return s
+00015250: 656c 665b 696e 6469 6365 735d 0a20 2020  elf[indices].   
+00015260: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00015270: 2069 6620 7365 6c66 2e69 6e5f 6d65 6d6f   if self.in_memo
+00015280: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00015290: 6461 7461 203d 2073 7570 6572 2829 2e5f  data = super()._
+000152a0: 5f67 6574 6974 656d 5f5f 2869 6e64 6963  _getitem__(indic
+000152b0: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+000152c0: 6966 206c 656e 2864 6174 612e 7368 6170  if len(data.shap
+000152d0: 6529 203c 2033 3a0a 2020 2020 2020 2020  e) < 3:.        
+000152e0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000152f0: 6174 612e 7669 6577 286e 756d 7079 2e6e  ata.view(numpy.n
+00015300: 6461 7272 6179 290a 2020 2020 2020 2020  darray).        
+00015310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015320: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00015330: 6e73 7461 6e63 6528 696e 6469 6365 732c  nstance(indices,
+00015340: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
+00015350: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00015360: 612e 7572 6c73 203d 2073 656c 662e 7572  a.urls = self.ur
+00015370: 6c73 5b69 6e64 6963 6573 5b30 5d5d 0a20  ls[indices[0]]. 
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 2020 2064 6174 612e 6d65 7461 6461 7461     data.metadata
+000153a0: 203d 2073 656c 662e 6d65 7461 6461 7461   = self.metadata
+000153b0: 5b69 6e64 6963 6573 5b30 5d5d 0a20 2020  [indices[0]].   
+000153c0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000153d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000153e0: 2020 2020 2020 2064 6174 612e 7572 6c73         data.urls
+000153f0: 203d 2073 656c 662e 7572 6c73 5b69 6e64   = self.urls[ind
+00015400: 6963 6573 5d0a 2020 2020 2020 2020 2020  ices].          
+00015410: 2020 2020 2020 2020 2020 6461 7461 2e6d            data.m
+00015420: 6574 6164 6174 6120 3d20 7365 6c66 2e6d  etadata = self.m
+00015430: 6574 6164 6174 615b 696e 6469 6365 735d  etadata[indices]
+00015440: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015450: 7572 6e20 6461 7461 0a20 2020 2020 2020  urn data.       
+00015460: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
+00015470: 6e64 6963 6573 2c20 7475 706c 6529 3a0a  ndices, tuple):.
+00015480: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00015490: 6f74 2069 7369 6e73 7461 6e63 6528 7365  ot isinstance(se
+000154a0: 6c66 2e75 726c 735b 696e 6469 6365 735b  lf.urls[indices[
+000154b0: 305d 5d2c 206e 756d 7079 2e6e 6461 7272  0]], numpy.ndarr
+000154c0: 6179 293a 0a20 2020 2020 2020 2020 2020  ay):.           
+000154d0: 2020 2020 2072 6574 7572 6e20 7574 696c       return util
+000154e0: 732e 6765 745f 6461 7461 2873 656c 662e  s.get_data(self.
+000154f0: 7572 6c73 5b69 6e64 6963 6573 5b30 5d5d  urls[indices[0]]
+00015500: 295b 696e 6469 6365 735b 315d 2c20 696e  )[indices[1], in
+00015510: 6469 6365 735b 325d 5d0a 2020 2020 2020  dices[2]].      
+00015520: 2020 2020 2020 7265 7475 726e 2044 6174        return Dat
+00015530: 6128 7365 6c66 2e75 726c 735b 696e 6469  a(self.urls[indi
+00015540: 6365 735b 305d 5d2c 2073 656c 662e 6d65  ces[0]], self.me
+00015550: 7461 6461 7461 5b69 6e64 6963 6573 5d2c  tadata[indices],
+00015560: 2073 656c 662e 696e 5f6d 656d 6f72 7929   self.in_memory)
+00015570: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00015580: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
+00015590: 7572 6c73 5b69 6e64 6963 6573 5d2c 206e  urls[indices], n
+000155a0: 756d 7079 2e6e 6461 7272 6179 293a 0a20  umpy.ndarray):. 
+000155b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000155c0: 6e20 7574 696c 732e 6765 745f 6461 7461  n utils.get_data
+000155d0: 2873 656c 662e 7572 6c73 5b69 6e64 6963  (self.urls[indic
+000155e0: 6573 5d29 0a20 2020 2020 2020 2072 6574  es]).        ret
+000155f0: 7572 6e20 4461 7461 2873 656c 662e 7572  urn Data(self.ur
+00015600: 6c73 5b69 6e64 6963 6573 5d2c 2073 656c  ls[indices], sel
+00015610: 662e 6d65 7461 6461 7461 5b69 6e64 6963  f.metadata[indic
+00015620: 6573 5d2c 2073 656c 662e 696e 5f6d 656d  es], self.in_mem
+00015630: 6f72 7929 0a0a 2020 2020 6465 6620 5f69  ory)..    def _i
+00015640: 7465 725f 6672 616d 6573 2873 656c 6629  ter_frames(self)
+00015650: 202d 3e20 4765 6e65 7261 746f 725b 6e75   -> Generator[nu
+00015660: 6d70 792e 6e64 6172 7261 792c 204e 6f6e  mpy.ndarray, Non
+00015670: 652c 204e 6f6e 655d 3a0a 2020 2020 2020  e, None]:.      
+00015680: 2020 6966 2073 656c 662e 696e 5f6d 656d    if self.in_mem
+00015690: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
+000156a0: 2066 7368 6170 6520 3d20 2873 656c 662e   fshape = (self.
+000156b0: 6e66 7261 6d65 732c 2920 2b20 7365 6c66  nframes,) + self
+000156c0: 2e66 7261 6d65 5f73 6861 7065 0a20 2020  .frame_shape.   
+000156d0: 2020 2020 2020 2020 2079 6965 6c64 2066           yield f
+000156e0: 726f 6d20 7375 7065 7228 292e 7265 7368  rom super().resh
+000156f0: 6170 6528 6673 6861 7065 290a 2020 2020  ape(fshape).    
+00015700: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00015710: 2020 2020 2020 666f 7220 7572 6c20 696e        for url in
+00015720: 2073 656c 662e 7572 6c73 2e66 6c61 7474   self.urls.flatt
+00015730: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+00015740: 2020 2020 2020 7969 656c 6420 7574 696c        yield util
+00015750: 732e 6765 745f 6461 7461 2875 726c 290a  s.get_data(url).
+00015760: 0a20 2020 2064 6566 205f 5f72 6564 7563  .    def __reduc
+00015770: 655f 5f28 7365 6c66 293a 0a20 2020 2020  e__(self):.     
+00015780: 2020 2023 2047 6574 2074 6865 2070 6172     # Get the par
+00015790: 656e 7427 7320 5f5f 7265 6475 6365 5f5f  ent's __reduce__
+000157a0: 2074 7570 6c65 0a20 2020 2020 2020 2070   tuple.        p
+000157b0: 6963 6b6c 6564 5f73 7461 7465 203d 2073  ickled_state = s
+000157c0: 7570 6572 2829 2e5f 5f72 6564 7563 655f  uper().__reduce_
+000157d0: 5f28 290a 2020 2020 2020 2020 2320 4372  _().        # Cr
+000157e0: 6561 7465 206f 7572 206f 776e 2074 7570  eate our own tup
+000157f0: 6c65 2074 6f20 7061 7373 2074 6f20 5f5f  le to pass to __
+00015800: 7365 7473 7461 7465 5f5f 0a20 2020 2020  setstate__.     
+00015810: 2020 206e 6577 5f73 7461 7465 203d 2070     new_state = p
+00015820: 6963 6b6c 6564 5f73 7461 7465 5b32 5d20  ickled_state[2] 
+00015830: 2b20 2828 7365 6c66 2e75 726c 732c 2073  + ((self.urls, s
+00015840: 656c 662e 6d65 7461 6461 7461 2c20 7365  elf.metadata, se
+00015850: 6c66 2e69 6e5f 6d65 6d6f 7279 292c 290a  lf.in_memory),).
+00015860: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00015870: 2061 2074 7570 6c65 2074 6861 7420 7265   a tuple that re
+00015880: 706c 6163 6573 2074 6865 2070 6172 656e  places the paren
+00015890: 7427 7320 5f5f 7365 7473 7461 7465 5f5f  t's __setstate__
+000158a0: 2074 7570 6c65 2077 6974 6820 6f75 7220   tuple with our 
+000158b0: 6f77 6e0a 2020 2020 2020 2020 7265 7475  own.        retu
+000158c0: 726e 2028 7069 636b 6c65 645f 7374 6174  rn (pickled_stat
+000158d0: 655b 305d 2c20 7069 636b 6c65 645f 7374  e[0], pickled_st
+000158e0: 6174 655b 315d 2c20 6e65 775f 7374 6174  ate[1], new_stat
+000158f0: 6529 0a0a 2020 2020 6465 6620 5f5f 7365  e)..    def __se
+00015900: 7473 7461 7465 5f5f 2873 656c 662c 2073  tstate__(self, s
+00015910: 7461 7465 293a 0a20 2020 2020 2020 2073  tate):.        s
+00015920: 656c 662e 7572 6c73 2c20 7365 6c66 2e6d  elf.urls, self.m
+00015930: 6574 6164 6174 612c 2073 656c 662e 696e  etadata, self.in
+00015940: 5f6d 656d 6f72 7920 3d20 7374 6174 655b  _memory = state[
+00015950: 2d31 5d20 2023 2053 6574 2074 6865 2061  -1]  # Set the a
+00015960: 7474 7269 6275 7465 730a 2020 2020 2020  ttributes.      
+00015970: 2020 7375 7065 7228 292e 5f5f 7365 7473    super().__sets
+00015980: 7461 7465 5f5f 2873 7461 7465 5b30 3a2d  tate__(state[0:-
+00015990: 315d 290a 0a20 2020 2064 6566 2073 746f  1])..    def sto
+000159a0: 705f 6f70 6572 6174 696f 6e28 7365 6c66  p_operation(self
+000159b0: 2c20 6f70 6572 6174 696f 6e3a 204f 7065  , operation: Ope
+000159c0: 7261 7469 6f6e 293a 0a20 2020 2020 2020  ration):.       
+000159d0: 2022 2222 0a20 2020 2020 2020 204d 6574   """.        Met
+000159e0: 686f 6420 7573 6564 2066 6f72 2063 6173  hod used for cas
+000159f0: 6573 2077 6865 7265 2074 6872 6561 6473  es where threads
+00015a00: 2061 7265 2063 7265 6174 6564 2074 6f20   are created to 
+00015a10: 6170 706c 7920 6675 6e63 7469 6f6e 7320  apply functions 
+00015a20: 746f 2074 6865 2064 6174 612e 0a20 2020  to the data..   
+00015a30: 2020 2020 2049 6620 6d65 7468 6f64 2069       If method i
+00015a40: 7320 6361 6c6c 6564 2c20 7468 6520 666c  s called, the fl
+00015a50: 6167 2063 6f6e 6365 726e 696e 6720 7468  ag concerning th
+00015a60: 6520 7374 6f70 2069 7320 7365 7420 746f  e stop is set to
+00015a70: 2030 2073 6f20 7468 6174 2069 6620 7468   0 so that if th
+00015a80: 6520 636f 6e63 6572 6e65 640a 2020 2020  e concerned.    
+00015a90: 2020 2020 6f70 6572 6174 696f 6e20 6973      operation is
+00015aa0: 2072 756e 6e69 6e67 2069 6e20 616e 6f74   running in anot
+00015ab0: 6865 7220 7468 7265 6164 2069 7420 6b6e  her thread it kn
+00015ac0: 6f77 7320 746f 2073 746f 702e 0a0a 2020  ows to stop...  
+00015ad0: 2020 2020 2020 3a70 6172 616d 2069 6e74        :param int
+00015ae0: 206f 7065 7261 7469 6f6e 3a20 6f70 6572   operation: oper
+00015af0: 6174 696f 6e20 746f 2073 746f 700a 2020  ation to stop.  
+00015b00: 2020 2020 2020 3a74 7970 6520 696e 743a        :type int:
+00015b10: 2055 6e69 6f6e 5b69 6e74 2c20 604f 7065   Union[int, `Ope
+00015b20: 7261 7469 6f6e 605d 0a20 2020 2020 2020  ration`].       
+00015b30: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00015b40: 6861 7361 7474 7228 7365 6c66 2c20 2273  hasattr(self, "s
+00015b50: 7461 7465 5f6f 665f 6f70 6572 6174 696f  tate_of_operatio
+00015b60: 6e73 2229 2061 6e64 2073 656c 662e 7374  ns") and self.st
+00015b70: 6174 655f 6f66 5f6f 7065 7261 7469 6f6e  ate_of_operation
+00015b80: 732e 6973 5f72 756e 6e69 6e67 280a 2020  s.is_running(.  
+00015b90: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
+00015ba0: 696f 6e0a 2020 2020 2020 2020 293a 0a20  ion.        ):. 
+00015bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015bc0: 7374 6174 655f 6f66 5f6f 7065 7261 7469  state_of_operati
+00015bd0: 6f6e 732e 7374 6f70 286f 7065 7261 7469  ons.stop(operati
+00015be0: 6f6e 290a 0a20 2020 2040 7072 6f70 6572  on)..    @proper
+00015bf0: 7479 0a20 2020 2064 6566 2073 6861 7065  ty.    def shape
+00015c00: 2873 656c 6629 202d 3e20 5475 706c 655b  (self) -> Tuple[
+00015c10: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+00015c20: 2254 6f74 616c 2073 6861 7065 203d 2073  "Total shape = s
+00015c30: 6361 6e20 7368 6170 6520 2b20 6672 616d  can shape + fram
+00015c40: 6520 7368 6170 6522 2222 0a20 2020 2020  e shape""".     
+00015c50: 2020 2073 6861 7065 203d 2073 7570 6572     shape = super
+00015c60: 2829 2e73 6861 7065 0a20 2020 2020 2020  ().shape.       
+00015c70: 2069 6620 7365 6c66 2e69 6e5f 6d65 6d6f   if self.in_memo
+00015c80: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00015c90: 7265 7475 726e 2073 6861 7065 0a20 2020  return shape.   
+00015ca0: 2020 2020 2072 6574 7572 6e20 7368 6170       return shap
+00015cb0: 6520 2b20 7365 6c66 2e66 7261 6d65 5f73  e + self.frame_s
+00015cc0: 6861 7065 0a0a 2020 2020 4070 726f 7065  hape..    @prope
+00015cd0: 7274 790a 2020 2020 6465 6620 7363 616e  rty.    def scan
+00015ce0: 5f73 6861 7065 2873 656c 6629 202d 3e20  _shape(self) -> 
+00015cf0: 5475 706c 655b 696e 745d 3a0a 2020 2020  Tuple[int]:.    
+00015d00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00015d10: 7368 6170 655b 3a2d 325d 0a0a 2020 2020  shape[:-2]..    
+00015d20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00015d30: 6620 6672 616d 655f 7368 6170 6528 7365  f frame_shape(se
+00015d40: 6c66 2920 2d3e 2054 7570 6c65 5b69 6e74  lf) -> Tuple[int
+00015d50: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+00015d60: 6966 2073 656c 662e 696e 5f6d 656d 6f72  if self.in_memor
+00015d70: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+00015d80: 6574 7572 6e20 7375 7065 7228 292e 7368  eturn super().sh
+00015d90: 6170 655b 2d32 3a5d 0a20 2020 2020 2020  ape[-2:].       
+00015da0: 2069 6620 7365 6c66 2e5f 696d 675f 7368   if self._img_sh
+00015db0: 6170 6520 6973 206e 6f74 204e 6f6e 653a  ape is not None:
+00015dc0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015dd0: 7572 6e20 7365 6c66 2e5f 696d 675f 7368  urn self._img_sh
+00015de0: 6170 650a 2020 2020 2020 2020 6966 2073  ape.        if s
+00015df0: 656c 662e 6e66 7261 6d65 7320 3d3d 2030  elf.nframes == 0
+00015e00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00015e10: 7475 726e 2030 2c20 300a 2020 2020 2020  turn 0, 0.      
+00015e20: 2020 696d 675f 7368 6170 6520 3d20 7574    img_shape = ut
+00015e30: 696c 732e 6765 745f 6461 7461 286e 6578  ils.get_data(nex
+00015e40: 7428 7365 6c66 2e75 726c 732e 666c 6174  t(self.urls.flat
+00015e50: 2929 2e73 6861 7065 0a20 2020 2020 2020  )).shape.       
+00015e60: 2073 656c 662e 5f69 6d67 5f73 6861 7065   self._img_shape
+00015e70: 203d 2069 6d67 5f73 6861 7065 0a20 2020   = img_shape.   
+00015e80: 2020 2020 2072 6574 7572 6e20 696d 675f       return img_
+00015e90: 7368 6170 650a 0a20 2020 2040 7072 6f70  shape..    @prop
+00015ea0: 6572 7479 0a20 2020 2064 6566 206e 6672  erty.    def nfr
+00015eb0: 616d 6573 2873 656c 6629 202d 3e20 696e  ames(self) -> in
+00015ec0: 743a 0a20 2020 2020 2020 2069 6620 7365  t:.        if se
+00015ed0: 6c66 2e75 726c 7320 6973 204e 6f6e 653a  lf.urls is None:
+00015ee0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015ef0: 7572 6e20 300a 2020 2020 2020 2020 7265  urn 0.        re
+00015f00: 7475 726e 2073 656c 662e 7572 6c73 2e73  turn self.urls.s
+00015f10: 697a 650a 0a20 2020 2040 7072 6f70 6572  ize..    @proper
+00015f20: 7479 0a20 2020 2064 6566 206e 6469 6d28  ty.    def ndim(
+00015f30: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+00015f40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015f50: 2020 4e75 6d62 6572 206f 6620 6172 7261    Number of arra
+00015f60: 7920 6469 6d65 6e73 696f 6e73 2e0a 2020  y dimensions..  
+00015f70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015f80: 2020 6966 2073 656c 662e 696e 5f6d 656d    if self.in_mem
+00015f90: 6f72 793a 0a20 2020 2020 2020 2020 2020  ory:.           
+00015fa0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00015fb0: 6e64 696d 0a20 2020 2020 2020 2072 6574  ndim.        ret
+00015fc0: 7572 6e20 7375 7065 7228 292e 6e64 696d  urn super().ndim
+00015fd0: 202b 2032 0a0a 2020 2020 6465 6620 6170   + 2..    def ap
+00015fe0: 706c 795f 6675 6e63 7328 0a20 2020 2020  ply_funcs(.     
+00015ff0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00016000: 2066 756e 6373 3d5b 5d2c 0a20 2020 2020   funcs=[],.     
+00016010: 2020 2069 6e64 6963 6573 3d4e 6f6e 652c     indices=None,
+00016020: 0a20 2020 2020 2020 2073 6176 653d 4661  .        save=Fa
+00016030: 6c73 652c 0a20 2020 2020 2020 2074 6578  lse,.        tex
+00016040: 743d 2222 2c0a 2020 2020 2020 2020 6f70  t="",.        op
+00016050: 6572 6174 696f 6e3d 4e6f 6e65 2c0a 2020  eration=None,.  
+00016060: 2020 2020 2020 6e65 775f 7368 6170 653d        new_shape=
+00016070: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00016080: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016090: 204d 6574 686f 6420 7468 6174 2061 7070   Method that app
+000160a0: 6c69 6573 2061 2073 6572 6965 7320 6f66  lies a series of
+000160b0: 2066 756e 6374 696f 6e73 2069 6e74 6f20   functions into 
+000160c0: 7468 6520 6461 7461 2e20 4974 2063 616e  the data. It can
+000160d0: 2073 6176 6520 7468 6520 696d 6167 6573   save the images
+000160e0: 0a20 2020 2020 2020 2069 6e74 6f20 6469  .        into di
+000160f0: 736b 206f 7220 7265 7475 726e 2074 6865  sk or return the
+00016100: 6d2e 0a0a 2020 2020 2020 2020 3a70 6172  m...        :par
+00016110: 616d 2066 756e 6373 3a20 4c69 7374 206f  am funcs: List o
+00016120: 6620 7475 7070 6c65 732e 2045 7665 7279  f tupples. Every
+00016130: 2074 7570 706c 6573 2063 6f6e 7461 696e   tupples contain
+00016140: 7320 7468 6520 6675 6e63 7469 6f6e 2074  s the function t
+00016150: 6f0a 2020 2020 2020 2020 2020 2020 6170  o.            ap
+00016160: 706c 7920 616e 6420 6974 7320 7061 7261  ply and its para
+00016170: 6d65 7465 7273 2c20 6465 6661 756c 7473  meters, defaults
+00016180: 2074 6f20 5b5d 0a20 2020 2020 2020 203a   to [].        :
+00016190: 7479 7065 2066 756e 6373 3a20 6172 7261  type funcs: arra
+000161a0: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
+000161b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000161c0: 696e 6469 6365 733a 2049 6e64 6963 6573  indices: Indices
+000161d0: 206f 6620 7468 6520 6461 7461 2074 6f20   of the data to 
+000161e0: 6170 706c 7920 7468 6520 6675 6e63 7469  apply the functi
+000161f0: 6f6e 7320 746f 2c0a 2020 2020 2020 2020  ons to,.        
+00016200: 2020 2020 6465 6661 756c 7473 2074 6f20      defaults to 
+00016210: 4e6f 6e65 0a20 2020 2020 2020 203a 7479  None.        :ty
+00016220: 7065 2069 6e64 6963 6573 3a20 556e 696f  pe indices: Unio
+00016230: 6e5b 4e6f 6e65 2c20 6172 7261 795f 6c69  n[None, array_li
+00016240: 6b65 5d2c 206f 7074 696f 6e61 6c0a 2020  ke], optional.  
+00016250: 2020 2020 2020 3a70 6172 616d 2073 6176        :param sav
+00016260: 653a 2049 6620 5472 7565 2c20 7361 7665  e: If True, save
+00016270: 7320 7468 6520 696d 6167 6573 2069 6e74  s the images int
+00016280: 6f20 6469 736b 2c20 6465 6661 756c 7473  o disk, defaults
+00016290: 2074 6f20 4661 6c73 650a 2020 2020 2020   to False.      
+000162a0: 2020 3a74 7970 6520 7361 7665 3a20 626f    :type save: bo
+000162b0: 6f6c 0a20 2020 2020 2020 203a 7061 7261  ol.        :para
+000162c0: 6d20 7374 7220 7465 7874 3a20 5465 7874  m str text: Text
+000162d0: 2074 6f20 7368 6f77 2069 6e20 7468 6520   to show in the 
+000162e0: 6164 7661 6e63 656d 656e 7420 6469 7370  advancement disp
+000162f0: 6c61 792e 0a20 2020 2020 2020 203a 7061  lay..        :pa
+00016300: 7261 6d20 696e 7420 6f70 6572 6174 696f  ram int operatio
+00016310: 6e3a 206f 7065 7261 7469 6f6e 2074 6f20  n: operation to 
+00016320: 7374 6f70 0a20 2020 2020 2020 203a 7479  stop.        :ty
+00016330: 7065 2069 6e74 3a20 556e 696f 6e5b 696e  pe int: Union[in
+00016340: 742c 2060 4f70 6572 6174 696f 6e60 5d0a  t, `Operation`].
+00016350: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00016360: 733a 2041 7272 6179 2077 6974 6820 7468  s: Array with th
+00016370: 6520 6e65 7720 7572 6c73 2028 6966 2064  e new urls (if d
+00016380: 6174 6120 7761 7320 7361 7665 6429 0a20  ata was saved). 
+00016390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000163a0: 2020 2069 6620 696e 6469 6365 7320 6973     if indices is
+000163b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000163c0: 2020 2069 6e64 6963 6573 203d 2072 616e     indices = ran
+000163d0: 6765 286c 656e 2873 656c 6629 290a 2020  ge(len(self)).  
+000163e0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000163f0: 6e63 6528 696e 6469 6365 732c 2069 6e74  nce(indices, int
+00016400: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00016410: 6e64 6963 6573 203d 205b 696e 6469 6365  ndices = [indice
+00016420: 735d 0a20 2020 2020 2020 2075 726c 7320  s].        urls 
+00016430: 3d20 5b5d 0a20 2020 2020 2020 2069 6f5f  = [].        io_
+00016440: 7574 696c 732e 6164 7661 6e63 656d 656e  utils.advancemen
+00016450: 745f 6469 7370 6c61 7928 302c 2073 656c  t_display(0, sel
+00016460: 662e 6e66 7261 6d65 732c 2074 6578 7429  f.nframes, text)
+00016470: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00016480: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
+00016490: 7374 6174 655f 6f66 5f6f 7065 7261 7469  state_of_operati
+000164a0: 6f6e 7322 293a 0a20 2020 2020 2020 2020  ons"):.         
+000164b0: 2020 2073 656c 662e 7374 6174 655f 6f66     self.state_of
+000164c0: 5f6f 7065 7261 7469 6f6e 7320 3d20 5f53  _operations = _S
+000164d0: 7461 7465 4f66 4f70 6572 6174 696f 6e73  tateOfOperations
+000164e0: 2829 0a0a 2020 2020 2020 2020 7769 7468  ()..        with
+000164f0: 2073 656c 662e 7374 6174 655f 6f66 5f6f   self.state_of_o
+00016500: 7065 7261 7469 6f6e 732e 7275 6e5f 636f  perations.run_co
+00016510: 6e74 6578 7428 6f70 6572 6174 696f 6e29  ntext(operation)
+00016520: 3a0a 2020 2020 2020 2020 2020 2020 5f66  :.            _f
+00016530: 696c 6520 3d20 4e6f 6e65 0a20 2020 2020  ile = None.     
+00016540: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00016550: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00016560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016570: 2020 2020 205f 6669 6c65 203d 2068 3570       _file = h5p
+00016580: 792e 4669 6c65 2873 6176 652c 2022 6122  y.File(save, "a"
+00016590: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000165a0: 2020 6578 6365 7074 204f 5345 7272 6f72    except OSError
+000165b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000165c0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+000165d0: 2e65 7869 7374 7328 7361 7665 293a 0a20  .exists(save):. 
+000165e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165f0: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
+00016600: 2873 6176 6529 0a20 2020 2020 2020 2020  (save).         
+00016610: 2020 2020 2020 2020 2020 205f 6669 6c65             _file
+00016620: 203d 2068 3570 792e 4669 6c65 2873 6176   = h5py.File(sav
+00016630: 652c 2022 7722 290a 0a20 2020 2020 2020  e, "w")..       
+00016640: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00016650: 5f6e 616d 6520 3d20 2264 6174 6173 6574  _name = "dataset
+00016660: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00016670: 2020 6e65 775f 7368 6170 6520 3d20 7365    new_shape = se
+00016680: 6c66 2e73 6861 7065 2069 6620 6e65 775f  lf.shape if new_
+00016690: 7368 6170 6520 6973 204e 6f6e 6520 656c  shape is None el
+000166a0: 7365 2074 7570 6c65 286e 6577 5f73 6861  se tuple(new_sha
+000166b0: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+000166c0: 2020 2020 6966 2022 6461 7461 7365 7422      if "dataset"
+000166d0: 2069 6e20 5f66 696c 653a 0a20 2020 2020   in _file:.     
+000166e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000166f0: 6620 6e65 775f 7368 6170 6520 213d 205f  f new_shape != _
+00016700: 6669 6c65 5b22 6461 7461 7365 7422 5d2e  file["dataset"].
+00016710: 7368 6170 653a 0a20 2020 2020 2020 2020  shape:.         
+00016720: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00016730: 6669 6c65 2e63 7265 6174 655f 6461 7461  file.create_data
+00016740: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
 00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016760: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00016770: 2020 2020 2020 2020 2020 2020 206f 7065               ope
-00016780: 7261 7469 6f6e 2069 7320 6e6f 7420 4e6f  ration is not No
-00016790: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-000167a0: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-000167b0: 6f74 2073 656c 662e 7374 6174 655f 6f66  ot self.state_of
-000167c0: 5f6f 7065 7261 7469 6f6e 732e 6973 5f72  _operations.is_r
-000167d0: 756e 6e69 6e67 286f 7065 7261 7469 6f6e  unning(operation
-000167e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000167f0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016810: 2069 6620 2275 7064 6174 655f 6461 7461   if "update_data
-00016820: 7365 7422 2069 6e20 5f66 696c 653a 0a20  set" in _file:. 
-00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016840: 2020 2020 2020 2020 2020 2064 656c 205f             del _
-00016850: 6669 6c65 5b22 7570 6461 7465 5f64 6174  file["update_dat
-00016860: 6173 6574 225d 0a20 2020 2020 2020 2020  aset"].         
-00016870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00016880: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00016890: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-000168a0: 6966 2073 6176 653a 0a20 2020 2020 2020  if save:.       
-000168b0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-000168c0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-000168d0: 696e 6469 6365 733a 0a20 2020 2020 2020  indices:.       
-000168e0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-000168f0: 2020 2020 2020 2020 2020 2069 6620 6a20             if j 
-00016900: 213d 2069 3a0a 2020 2020 2020 2020 2020  != i:.          
-00016910: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00016920: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00016930: 6e61 6d65 203d 2073 6176 6520 2b20 7374  name = save + st
-00016940: 7228 6a29 2e7a 6669 6c6c 2834 2920 2b20  r(j).zfill(4) + 
-00016950: 222e 6e70 7922 0a20 2020 2020 2020 2020  ".npy".         
-00016960: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00016970: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00016980: 7265 6d6f 7665 2866 696c 656e 616d 6529  remove(filename)
-00016990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169a0: 2020 2020 2023 2020 2020 2020 2020 2020       #          
-000169b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000169c0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-000169d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-000169e0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-000169f0: 2020 2020 2020 2020 2023 2020 2020 2072           #     r
-00016a00: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00016a10: 2020 2020 2020 2020 2020 696d 6720 3d20            img = 
-00016a20: 7365 6c66 5b69 6e74 2869 295d 0a20 2020  self[int(i)].   
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2066 6f72 2066 2c20 6172 6773 2069 6e20   for f, args in 
-00016a50: 6675 6e63 733a 0a20 2020 2020 2020 2020  funcs:.         
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016a70: 6d67 203d 2066 282a 285b 696d 675d 202b  mg = f(*([img] +
-00016a80: 2061 7267 7329 290a 2020 2020 2020 2020   args)).        
-00016a90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00016aa0: 6176 653a 0a20 2020 2020 2020 2020 2020  ave:.           
-00016ab0: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
-00016ac0: 6c65 5b64 6174 6173 6574 5f6e 616d 655d  le[dataset_name]
-00016ad0: 5b69 5d20 3d20 696d 670a 2020 2020 2020  [i] = img.      
-00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016af0: 2020 7572 6c73 2e61 7070 656e 6428 0a20    urls.append(. 
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 2020 2020 2020 2020 2044 6174 6155             DataU
-00016b20: 726c 280a 2020 2020 2020 2020 2020 2020  rl(.            
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b40: 2020 2020 6669 6c65 5f70 6174 683d 7361      file_path=sa
-00016b50: 7665 2c0a 2020 2020 2020 2020 2020 2020  ve,.            
-00016b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b70: 2020 2020 6461 7461 5f70 6174 683d 222f      data_path="/
-00016b80: 6461 7461 7365 7422 2c0a 2020 2020 2020  dataset",.      
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ba0: 2020 2020 2020 2020 2020 6461 7461 5f73            data_s
-00016bb0: 6c69 6365 3d69 2c0a 2020 2020 2020 2020  lice=i,.        
-00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bd0: 2020 2020 2020 2020 7363 6865 6d65 3d22          scheme="
-00016be0: 7369 6c78 222c 0a20 2020 2020 2020 2020  silx",.         
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00016c10: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 2020 2020 2020 2023 2066 696c 656e 616d         # filenam
-00016c40: 6520 3d20 7361 7665 202b 2073 7472 2869  e = save + str(i
-00016c50: 292e 7a66 696c 6c28 3429 202b 2022 2e6e  ).zfill(4) + ".n
-00016c60: 7079 220a 2020 2020 2020 2020 2020 2020  py".            
-00016c70: 2020 2020 2020 2020 2020 2020 2320 6e75              # nu
-00016c80: 6d70 792e 7361 7665 2866 696c 656e 616d  mpy.save(filenam
-00016c90: 652c 2069 6d67 290a 2020 2020 2020 2020  e, img).        
-00016ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cb0: 2320 7572 6c73 2e61 7070 656e 6428 4461  # urls.append(Da
-00016cc0: 7461 5572 6c28 6669 6c65 5f70 6174 683d  taUrl(file_path=
-00016cd0: 6669 6c65 6e61 6d65 2c20 7363 6865 6d65  filename, scheme
-00016ce0: 3d27 6661 6269 6f27 2929 0a20 2020 2020  ='fabio')).     
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016d00: 6f5f 7574 696c 732e 6164 7661 6e63 656d  o_utils.advancem
-00016d10: 656e 745f 6469 7370 6c61 7928 6920 2b20  ent_display(i + 
-00016d20: 312c 2073 656c 662e 6e66 7261 6d65 732c  1, self.nframes,
-00016d30: 2074 6578 7429 0a0a 2020 2020 2020 2020   text)..        
-00016d40: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00016d50: 7465 5f6f 665f 6f70 6572 6174 696f 6e73  te_of_operations
-00016d60: 2e73 746f 7028 6f70 6572 6174 696f 6e29  .stop(operation)
-00016d70: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016d80: 2020 6966 2064 6174 6173 6574 5f6e 616d    if dataset_nam
-00016d90: 6520 3d3d 2022 7570 6461 7465 5f64 6174  e == "update_dat
-00016da0: 6173 6574 223a 0a20 2020 2020 2020 2020  aset":.         
-00016db0: 2020 2020 2020 2020 2020 2064 656c 205f             del _
-00016dc0: 6669 6c65 5b22 6461 7461 7365 7422 5d0a  file["dataset"].
+00016760: 2022 7570 6461 7465 5f64 6174 6173 6574   "update_dataset
+00016770: 222c 206e 6577 5f73 6861 7065 2c20 6474  ", new_shape, dt
+00016780: 7970 653d 7365 6c66 2e64 7479 7065 0a20  ype=self.dtype. 
+00016790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000167b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000167c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000167d0: 2020 2020 2020 2020 2020 205f 6669 6c65             _file
+000167e0: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
+000167f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016800: 2020 2020 2020 2020 2020 2020 2022 7570               "up
+00016810: 6461 7465 5f64 6174 6173 6574 222c 0a20  date_dataset",. 
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00016840: 3d5f 6669 6c65 5b22 6461 7461 7365 7422  =_file["dataset"
+00016850: 5d2e 7368 6170 652c 0a20 2020 2020 2020  ].shape,.       
+00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016870: 2020 2020 2064 7479 7065 3d5f 6669 6c65       dtype=_file
+00016880: 5b22 6461 7461 7365 7422 5d2e 6474 7970  ["dataset"].dtyp
+00016890: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000168a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168c0: 2020 2020 2066 6f72 2069 2c20 696d 6720       for i, img 
+000168d0: 696e 2065 6e75 6d65 7261 7465 285f 6669  in enumerate(_fi
+000168e0: 6c65 5b22 6461 7461 7365 7422 5d29 3a0a  le["dataset"]):.
+000168f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016900: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
+00016910: 655b 2275 7064 6174 655f 6461 7461 7365  e["update_datase
+00016920: 7422 5d5b 695d 203d 2069 6d67 0a20 2020  t"][i] = img.   
+00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016940: 2064 6174 6173 6574 5f6e 616d 6520 3d20   dataset_name = 
+00016950: 2275 7064 6174 655f 6461 7461 7365 7422  "update_dataset"
+00016960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016970: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016980: 2020 2020 2020 2020 2020 205f 6669 6c65             _file
+00016990: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
+000169a0: 2264 6174 6173 6574 222c 206e 6577 5f73  "dataset", new_s
+000169b0: 6861 7065 2c20 6474 7970 653d 7365 6c66  hape, dtype=self
+000169c0: 2e64 7479 7065 290a 0a20 2020 2020 2020  .dtype)..       
+000169d0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000169e0: 6e20 696e 6469 6365 733a 0a20 2020 2020  n indices:.     
+000169f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00016a00: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00016a10: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
+00016a20: 6174 696f 6e20 6973 206e 6f74 204e 6f6e  ation is not Non
+00016a30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00016a40: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+00016a50: 7420 7365 6c66 2e73 7461 7465 5f6f 665f  t self.state_of_
+00016a60: 6f70 6572 6174 696f 6e73 2e69 735f 7275  operations.is_ru
+00016a70: 6e6e 696e 6728 6f70 6572 6174 696f 6e29  nning(operation)
+00016a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a90: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ab0: 6966 2022 7570 6461 7465 5f64 6174 6173  if "update_datas
+00016ac0: 6574 2220 696e 205f 6669 6c65 3a0a 2020  et" in _file:.  
+00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ae0: 2020 2020 2020 2020 2020 6465 6c20 5f66            del _f
+00016af0: 696c 655b 2275 7064 6174 655f 6461 7461  ile["update_data
+00016b00: 7365 7422 5d0a 2020 2020 2020 2020 2020  set"].          
+00016b10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00016b20: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00016b30: 2020 2020 2020 2020 2023 2020 2020 2069           #     i
+00016b40: 6620 7361 7665 3a0a 2020 2020 2020 2020  f save:.        
+00016b50: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00016b60: 2020 2020 2020 666f 7220 6a20 696e 2069        for j in i
+00016b70: 6e64 6963 6573 3a0a 2020 2020 2020 2020  ndices:.        
+00016b80: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00016b90: 2020 2020 2020 2020 2020 6966 206a 2021            if j !
+00016ba0: 3d20 693a 0a20 2020 2020 2020 2020 2020  = i:.           
+00016bb0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+00016bc0: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+00016bd0: 616d 6520 3d20 7361 7665 202b 2073 7472  ame = save + str
+00016be0: 286a 292e 7a66 696c 6c28 3429 202b 2022  (j).zfill(4) + "
+00016bf0: 2e6e 7079 220a 2020 2020 2020 2020 2020  .npy".          
+00016c00: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+00016c10: 2020 2020 2020 2020 2020 2020 6f73 2e72              os.r
+00016c20: 656d 6f76 6528 6669 6c65 6e61 6d65 290a  emove(filename).
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c40: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+00016c50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00016c60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00016c70: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00016c80: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00016c90: 2020 2020 2020 2020 2320 2020 2020 7265          #     re
+00016ca0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00016cb0: 2020 2020 2020 2020 2069 6d67 203d 2073           img = s
+00016cc0: 656c 665b 696e 7428 6929 5d0a 2020 2020  elf[int(i)].    
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ce0: 666f 7220 662c 2061 7267 7320 696e 2066  for f, args in f
+00016cf0: 756e 6373 3a0a 2020 2020 2020 2020 2020  uncs:.          
+00016d00: 2020 2020 2020 2020 2020 2020 2020 696d                im
+00016d10: 6720 3d20 6628 2a28 5b69 6d67 5d20 2b20  g = f(*([img] + 
+00016d20: 6172 6773 2929 0a20 2020 2020 2020 2020  args)).         
+00016d30: 2020 2020 2020 2020 2020 2069 6620 7361             if sa
+00016d40: 7665 3a0a 2020 2020 2020 2020 2020 2020  ve:.            
+00016d50: 2020 2020 2020 2020 2020 2020 5f66 696c              _fil
+00016d60: 655b 6461 7461 7365 745f 6e61 6d65 5d5b  e[dataset_name][
+00016d70: 695d 203d 2069 6d67 0a20 2020 2020 2020  i] = img.       
+00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d90: 2075 726c 732e 6170 7065 6e64 280a 2020   urls.append(.  
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 2020 2020 2020 2020 2020 4461 7461 5572            DataUr
+00016dc0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
 00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2020 2020 5f66 696c 655b 2264 6174 6173      _file["datas
-00016df0: 6574 225d 203d 205f 6669 6c65 5b22 7570  et"] = _file["up
-00016e00: 6461 7465 5f64 6174 6173 6574 225d 0a20  date_dataset"]. 
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2020 2064 656c 205f 6669 6c65 5b22 7570     del _file["up
-00016e30: 6461 7465 5f64 6174 6173 6574 225d 0a20  date_dataset"]. 
-00016e40: 2020 2020 2020 2020 2020 2066 696e 616c             final
-00016e50: 6c79 3a0a 2020 2020 2020 2020 2020 2020  ly:.            
-00016e60: 2020 2020 6966 205f 6669 6c65 2069 7320      if _file is 
-00016e70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00016e80: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
-00016e90: 696c 652e 636c 6f73 6528 290a 2020 2020  ile.close().    
-00016ea0: 2020 2020 7265 7475 726e 206e 756d 7079      return numpy
-00016eb0: 2e61 7272 6179 2875 726c 7329 0a0a 2020  .array(urls)..  
-00016ec0: 2020 6465 6620 7361 7665 2873 656c 662c    def save(self,
-00016ed0: 2070 6174 682c 2069 6e64 6963 6573 3d4e   path, indices=N
-00016ee0: 6f6e 652c 206e 6577 5f73 6861 7065 3d4e  one, new_shape=N
-00016ef0: 6f6e 652c 2069 6e5f 6d65 6d6f 7279 3d54  one, in_memory=T
-00016f00: 7275 6529 202d 3e20 4e6f 6e65 3a0a 2020  rue) -> None:.  
-00016f10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016f20: 2020 5361 7665 2074 6865 2064 6174 6120    Save the data 
-00016f30: 696e 746f 2060 7061 7468 6020 666f 6c64  into `path` fold
-00016f40: 6572 2061 6e64 2072 6570 6c61 6365 2044  er and replace D
-00016f50: 6174 6120 7572 6c73 2e0a 2020 2020 2020  ata urls..      
-00016f60: 2020 544f 444f 3a20 6368 6563 6b20 6966    TODO: check if
-00016f70: 2075 726c 7320 616c 7265 6164 7920 6578   urls already ex
-00016f80: 6973 7420 616e 642c 2069 6620 736f 2c20  ist and, if so, 
-00016f90: 6d6f 6469 6679 206f 6e6c 7920 7572 6c73  modify only urls
-00016fa0: 5b69 6e64 6963 6573 5d2e 0a0a 2020 2020  [indices]...    
-00016fb0: 2020 2020 3a70 6172 616d 2070 6174 683a      :param path:
-00016fc0: 2050 6174 6820 746f 2074 6865 2066 6f6c   Path to the fol
-00016fd0: 6465 720a 2020 2020 2020 2020 3a74 7970  der.        :typ
-00016fe0: 6520 7061 7468 3a20 7374 720a 2020 2020  e path: str.    
-00016ff0: 2020 2020 3a70 6172 616d 2069 6e64 6963      :param indic
-00017000: 6573 3a20 7468 6520 696e 6469 6365 7320  es: the indices 
-00017010: 6f66 2074 6865 2076 616c 7565 7320 746f  of the values to
-00017020: 2073 6176 652c 2064 6566 6175 6c74 7320   save, defaults 
-00017030: 746f 204e 6f6e 650a 2020 2020 2020 2020  to None.        
-00017040: 3a74 7970 6520 696e 6469 6365 733a 2055  :type indices: U
-00017050: 6e69 6f6e 5b4e 6f6e 652c 6172 7261 795f  nion[None,array_
-00017060: 6c69 6b65 5d2c 206f 7074 696f 6e61 6c0a  like], optional.
-00017070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017080: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
-00017090: 7472 2873 656c 662c 2022 696e 5f6d 656d  tr(self, "in_mem
-000170a0: 6f72 7922 2920 6f72 2073 656c 662e 696e  ory") or self.in
-000170b0: 5f6d 656d 6f72 7920 6973 204e 6f6e 653a  _memory is None:
-000170c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000170d0: 662e 696e 5f6d 656d 6f72 7920 3d20 5472  f.in_memory = Tr
-000170e0: 7565 0a20 2020 2020 2020 2075 726c 7320  ue.        urls 
-000170f0: 3d20 5b5d 0a0a 2020 2020 2020 2020 6966  = []..        if
-00017100: 2069 6e64 6963 6573 2069 7320 4e6f 6e65   indices is None
-00017110: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-00017120: 7461 203d 2073 656c 662e 666c 6174 7465  ta = self.flatte
-00017130: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00017140: 696e 6469 6365 7320 3d20 6e75 6d70 792e  indices = numpy.
-00017150: 6172 616e 6765 286c 656e 2864 6174 6129  arange(len(data)
-00017160: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00017170: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00017180: 203d 2073 656c 662e 666c 6174 7465 6e28   = self.flatten(
-00017190: 295b 696e 6469 6365 735d 0a0a 2020 2020  )[indices]..    
-000171a0: 2020 2020 5f66 696c 6520 3d20 4e6f 6e65      _file = None
-000171b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000171c0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-000171d0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000171e0: 6669 6c65 203d 2068 3570 792e 4669 6c65  file = h5py.File
-000171f0: 2870 6174 682c 2022 6122 290a 2020 2020  (path, "a").    
-00017200: 2020 2020 2020 2020 6578 6365 7074 204f          except O
-00017210: 5345 7272 6f72 3a0a 2020 2020 2020 2020  SError:.        
-00017220: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-00017230: 7468 2e65 7869 7374 7328 7061 7468 293a  th.exists(path):
-00017240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017250: 2020 2020 206f 732e 7265 6d6f 7665 2870       os.remove(p
-00017260: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-00017270: 2020 2020 205f 6669 6c65 203d 2068 3570       _file = h5p
-00017280: 792e 4669 6c65 2870 6174 682c 2022 7722  y.File(path, "w"
-00017290: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000172a0: 206e 6577 5f73 6861 7065 3a0a 2020 2020   new_shape:.    
-000172b0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-000172c0: 7368 6170 6520 3d20 7475 706c 6528 6e65  shape = tuple(ne
-000172d0: 775f 7368 6170 6529 0a20 2020 2020 2020  w_shape).       
-000172e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000172f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00017300: 6c66 2e6e 6469 6d20 3e20 333a 0a20 2020  lf.ndim > 3:.   
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 206e 6577 5f73 6861 7065 203d 2028 7365   new_shape = (se
-00017330: 6c66 2e6e 6672 616d 6573 2c29 202b 2073  lf.nframes,) + s
-00017340: 656c 662e 6672 616d 655f 7368 6170 650a  elf.frame_shape.
-00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017360: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00017370: 2020 2020 2020 2020 2020 6e65 775f 7368            new_sh
-00017380: 6170 6520 3d20 7365 6c66 2e73 6861 7065  ape = self.shape
-00017390: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000173a0: 2264 6174 6173 6574 2220 6e6f 7420 696e  "dataset" not in
-000173b0: 205f 6669 6c65 3a0a 2020 2020 2020 2020   _file:.        
-000173c0: 2020 2020 2020 2020 5f66 696c 652e 6372          _file.cr
-000173d0: 6561 7465 5f64 6174 6173 6574 2822 6461  eate_dataset("da
-000173e0: 7461 7365 7422 2c20 6e65 775f 7368 6170  taset", new_shap
-000173f0: 652c 2064 7479 7065 3d73 656c 662e 6474  e, dtype=self.dt
-00017400: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
-00017410: 2065 6c69 6620 6e65 775f 7368 6170 6520   elif new_shape 
-00017420: 213d 205f 6669 6c65 5b22 6461 7461 7365  != _file["datase
-00017430: 7422 5d2e 7368 6170 653a 0a20 2020 2020  t"].shape:.     
-00017440: 2020 2020 2020 2020 2020 2064 656c 205f             del _
-00017450: 6669 6c65 5b22 6461 7461 7365 7422 5d0a  file["dataset"].
-00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017470: 5f66 696c 652e 6372 6561 7465 5f64 6174  _file.create_dat
-00017480: 6173 6574 2822 6461 7461 7365 7422 2c20  aset("dataset", 
-00017490: 6e65 775f 7368 6170 652c 2064 7479 7065  new_shape, dtype
-000174a0: 3d73 656c 662e 6474 7970 6529 0a0a 2020  =self.dtype)..  
-000174b0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-000174c0: 206a 2069 6e20 656e 756d 6572 6174 6528   j in enumerate(
-000174d0: 696e 6469 6365 7329 3a0a 2020 2020 2020  indices):.      
-000174e0: 2020 2020 2020 2020 2020 5f66 696c 655b            _file[
-000174f0: 2264 6174 6173 6574 225d 5b6a 5d20 3d20  "dataset"][j] = 
-00017500: 6461 7461 5b69 5d0a 2020 2020 2020 2020  data[i].        
-00017510: 2020 2020 2020 2020 7572 6c73 2e61 7070          urls.app
-00017520: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-00017530: 2020 2020 2020 2020 2044 6174 6155 726c           DataUrl
-00017540: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00017550: 2020 2020 2020 2020 2020 6669 6c65 5f70            file_p
-00017560: 6174 683d 7061 7468 2c0a 2020 2020 2020  ath=path,.      
-00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017580: 2020 6461 7461 5f70 6174 683d 222f 6461    data_path="/da
-00017590: 7461 7365 7422 2c0a 2020 2020 2020 2020  taset",.        
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 6461 7461 5f73 6c69 6365 3d6a 2c0a 2020  data_slice=j,.  
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 2020 2020 7363 6865 6d65 3d22 7369        scheme="si
-000175e0: 6c78 222c 0a20 2020 2020 2020 2020 2020  lx",.           
-000175f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00017600: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00017610: 2020 2020 2020 2020 2023 2020 2020 2066           #     f
-00017620: 696c 656e 616d 6520 3d20 7061 7468 202b  ilename = path +
-00017630: 2073 7472 2869 292e 7a66 696c 6c28 3429   str(i).zfill(4)
-00017640: 202b 2022 2e6e 7079 220a 2020 2020 2020   + ".npy".      
-00017650: 2020 2020 2020 2320 2020 2020 6e75 6d70        #     nump
-00017660: 792e 7361 7665 2866 696c 656e 616d 652c  y.save(filename,
-00017670: 2069 6d67 290a 2020 2020 2020 2020 2020   img).          
-00017680: 2020 2320 2020 2020 7572 6c73 2e61 7070    #     urls.app
-00017690: 656e 6428 4461 7461 5572 6c28 6669 6c65  end(DataUrl(file
-000176a0: 5f70 6174 683d 6669 6c65 6e61 6d65 2c20  _path=filename, 
-000176b0: 7363 6865 6d65 3d27 6661 6269 6f27 2929  scheme='fabio'))
-000176c0: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
-000176d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000176e0: 205f 6669 6c65 2069 7320 6e6f 7420 4e6f   _file is not No
-000176f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00017700: 2020 2020 5f66 696c 652e 636c 6f73 6528      _file.close(
-00017710: 290a 2020 2020 2020 2020 7572 6c73 203d  ).        urls =
-00017720: 206e 756d 7079 2e61 7361 7272 6179 2875   numpy.asarray(u
-00017730: 726c 7329 0a20 2020 2020 2020 2069 6620  rls).        if 
-00017740: 7365 6c66 2e75 726c 7320 6973 206e 6f74  self.urls is not
-00017750: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017760: 2020 206e 6577 5f75 726c 7320 3d20 7365     new_urls = se
-00017770: 6c66 2e75 726c 732e 666c 6174 7465 6e28  lf.urls.flatten(
-00017780: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-00017790: 775f 7572 6c73 5b69 6e64 6963 6573 5d20  w_urls[indices] 
-000177a0: 3d20 7572 6c73 0a20 2020 2020 2020 2020  = urls.         
-000177b0: 2020 2073 656c 662e 7572 6c73 203d 206e     self.urls = n
-000177c0: 6577 5f75 726c 732e 7265 7368 6170 6528  ew_urls.reshape(
-000177d0: 7365 6c66 2e75 726c 732e 7368 6170 6529  self.urls.shape)
-000177e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000177f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017800: 7572 6c73 203d 206e 756d 7079 2e61 7361  urls = numpy.asa
-00017810: 7272 6179 2875 726c 7329 0a0a 2020 2020  rray(urls)..    
-00017820: 4063 6f6e 7465 7874 6d61 6e61 6765 720a  @contextmanager.
-00017830: 2020 2020 6465 6620 6f70 656e 5f61 735f      def open_as_
-00017840: 6864 6635 2873 656c 662c 205f 6469 7229  hdf5(self, _dir)
-00017850: 202d 3e20 4765 6e65 7261 746f 725b 6835   -> Generator[h5
-00017860: 7079 2e44 6174 6173 6574 2c20 4e6f 6e65  py.Dataset, None
-00017870: 2c20 4e6f 6e65 5d3a 0a20 2020 2020 2020  , None]:.       
-00017880: 2022 2222 0a20 2020 2020 2020 2043 6f6e   """.        Con
-00017890: 7665 7274 7320 7468 6520 6461 7461 2069  verts the data i
-000178a0: 6e74 6f20 616e 2048 4446 3520 6669 6c65  nto an HDF5 file
-000178b0: 2c20 7365 7474 696e 6720 666c 6174 7465  , setting flatte
-000178c0: 6e65 6420 696d 6167 6573 2069 6e20 7468  ned images in th
-000178d0: 6520 726f 7773 2e0a 2020 2020 2020 2020  e rows..        
-000178e0: 544f 444f 3a20 7061 7373 2066 696c 656e  TODO: pass filen
-000178f0: 616d 6520 7065 7220 7061 7261 6d65 7465  ame per paramete
-00017900: 723f 0a0a 2020 2020 2020 2020 3a70 6172  r?..        :par
-00017910: 616d 205f 6469 723a 2044 6972 6563 746f  am _dir: Directo
-00017920: 7279 2069 6e20 7768 6963 6820 746f 2073  ry in which to s
-00017930: 6176 6520 7468 6520 4844 4635 2066 696c  ave the HDF5 fil
-00017940: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-00017950: 205f 6469 723a 2073 7472 0a0a 2020 2020   _dir: str..    
-00017960: 2020 2020 3a72 6574 7572 6e3a 2048 4446      :return: HDF
-00017970: 3520 6461 7461 7365 740a 2020 2020 2020  5 dataset.      
-00017980: 2020 3a72 7479 7065 3a20 6068 3570 792e    :rtype: `h5py.
-00017990: 4461 7461 7365 7460 0a20 2020 2020 2020  Dataset`.       
-000179a0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-000179b0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-000179c0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-000179d0: 2020 2066 696c 656e 616d 6520 3d20 6f73     filename = os
-000179e0: 2e70 6174 682e 6a6f 696e 285f 6469 722c  .path.join(_dir,
-000179f0: 2022 6461 7461 2e68 6466 3522 290a 2020   "data.hdf5").  
-00017a00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017a10: 6c66 2e5f 6669 6c65 203d 2068 3570 792e  lf._file = h5py.
-00017a20: 4669 6c65 2866 696c 656e 616d 652c 2022  File(filename, "
-00017a30: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
-00017a40: 6578 6365 7074 204f 5345 7272 6f72 3a0a  except OSError:.
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a60: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-00017a70: 7328 6669 6c65 6e61 6d65 293a 0a20 2020  s(filename):.   
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 206f 732e 7265 6d6f 7665 2866 696c 656e   os.remove(filen
-00017aa0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00017ab0: 2020 2020 2073 656c 662e 5f66 696c 6520       self._file 
-00017ac0: 3d20 6835 7079 2e46 696c 6528 6669 6c65  = h5py.File(file
-00017ad0: 6e61 6d65 2c20 2277 2229 0a0a 2020 2020  name, "w")..    
-00017ae0: 2020 2020 2020 2020 6e66 7261 6d65 7320          nframes 
-00017af0: 3d20 7365 6c66 2e6e 6672 616d 6573 0a20  = self.nframes. 
-00017b00: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
-00017b10: 5f73 6861 7065 203d 2073 656c 662e 6672  _shape = self.fr
-00017b20: 616d 655f 7368 6170 650a 2020 2020 2020  ame_shape.      
-00017b30: 2020 2020 2020 6672 616d 655f 7369 7a65        frame_size
-00017b40: 203d 2066 7261 6d65 5f73 6861 7065 5b30   = frame_shape[0
-00017b50: 5d20 2a20 6672 616d 655f 7368 6170 655b  ] * frame_shape[
-00017b60: 315d 0a20 2020 2020 2020 2020 2020 2068  1].            h
-00017b70: 6466 355f 7368 6170 6520 3d20 286e 6672  df5_shape = (nfr
-00017b80: 616d 6573 2c20 6672 616d 655f 7369 7a65  ames, frame_size
-00017b90: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00017ba0: 6620 2264 6174 6173 6574 2220 696e 2073  f "dataset" in s
-00017bb0: 656c 662e 5f66 696c 6520 616e 6420 7365  elf._file and se
-00017bc0: 6c66 2e5f 6669 6c65 5b22 6461 7461 7365  lf._file["datase
-00017bd0: 7422 5d2e 7368 6170 6520 213d 2068 6466  t"].shape != hdf
-00017be0: 355f 7368 6170 653a 0a20 2020 2020 2020  5_shape:.       
-00017bf0: 2020 2020 2020 2020 2064 656c 2073 656c           del sel
-00017c00: 662e 5f66 696c 655b 2264 6174 6173 6574  f._file["dataset
-00017c10: 225d 0a20 2020 2020 2020 2020 2020 2069  "].            i
-00017c20: 6620 2264 6174 6173 6574 2220 6e6f 7420  f "dataset" not 
-00017c30: 696e 2073 656c 662e 5f66 696c 653a 0a20  in self._file:. 
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017c50: 656c 662e 5f66 696c 652e 6372 6561 7465  elf._file.create
-00017c60: 5f64 6174 6173 6574 2822 6461 7461 7365  _dataset("datase
-00017c70: 7422 2c20 7368 6170 653d 6864 6635 5f73  t", shape=hdf5_s
-00017c80: 6861 7065 2c20 6474 7970 653d 7365 6c66  hape, dtype=self
-00017c90: 2e64 7479 7065 290a 0a20 2020 2020 2020  .dtype)..       
-00017ca0: 2020 2020 2066 6f72 2069 6d61 6765 5f69       for image_i
-00017cb0: 6478 2c20 6672 616d 6520 696e 2065 6e75  dx, frame in enu
-00017cc0: 6d65 7261 7465 2873 656c 662e 5f69 7465  merate(self._ite
-00017cd0: 725f 6672 616d 6573 2829 293a 0a20 2020  r_frames()):.   
-00017ce0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017cf0: 662e 5f66 696c 655b 2264 6174 6173 6574  f._file["dataset
-00017d00: 225d 5b69 6d61 6765 5f69 6478 5d20 3d20  "][image_idx] = 
-00017d10: 6672 616d 652e 666c 6174 7465 6e28 290a  frame.flatten().
-00017d20: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-00017d30: 6c64 2073 656c 662e 5f66 696c 655b 2264  ld self._file["d
-00017d40: 6174 6173 6574 225d 0a20 2020 2020 2020  ataset"].       
-00017d50: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00017d60: 2020 2020 2020 6966 2073 656c 662e 5f66        if self._f
-00017d70: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
-00017d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d90: 2073 656c 662e 5f66 696c 652e 636c 6f73   self._file.clos
-00017da0: 6528 290a 0a20 2020 2064 6566 2072 6573  e()..    def res
-00017db0: 6861 7065 2873 656c 662c 2073 6861 7065  hape(self, shape
-00017dc0: 2c20 6f72 6465 723d 2243 2229 202d 3e20  , order="C") -> 
-00017dd0: 2244 6174 6122 3a0a 2020 2020 2020 2020  "Data":.        
-00017de0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-00017df0: 726e 7320 616e 2061 7272 6179 2063 6f6e  rns an array con
-00017e00: 7461 696e 696e 6720 7468 6520 7361 6d65  taining the same
-00017e10: 2064 6174 6120 7769 7468 2061 206e 6577   data with a new
-00017e20: 2073 6861 7065 206f 6620 7572 6c73 2061   shape of urls a
-00017e30: 6e64 206d 6574 6164 6174 612e 0a20 2020  nd metadata..   
-00017e40: 2020 2020 2053 6861 7065 2061 6c73 6f20       Shape also 
-00017e50: 636f 6e74 6169 6e73 2069 6d61 6765 2073  contains image s
-00017e60: 6861 7065 2061 7420 7468 6520 6c61 7374  hape at the last
-00017e70: 2074 776f 2070 6f73 6974 696f 6e73 2028   two positions (
-00017e80: 756e 7265 7368 6170 6162 6c65 292e 0a0a  unreshapable)...
-00017e90: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00017ea0: 6861 7065 3a20 4e65 7720 7368 6170 652c  hape: New shape,
-00017eb0: 2073 686f 756c 6420 6265 2063 6f6d 7061   should be compa
-00017ec0: 7469 626c 6520 7769 7468 2074 6865 206f  tible with the o
-00017ed0: 7269 6769 6e61 6c20 7368 6170 652e 0a20  riginal shape.. 
-00017ee0: 2020 2020 2020 203a 7479 7065 2073 6861         :type sha
-00017ef0: 7065 3a20 696e 7420 6f72 2074 7570 6c65  pe: int or tuple
-00017f00: 206f 6620 696e 7473 2e0a 2020 2020 2020   of ints..      
-00017f10: 2020 3a72 6574 7572 6e3a 206e 6577 2044    :return: new D
-00017f20: 6174 6120 6f62 6a65 6374 2077 6974 6820  ata object with 
-00017f30: 7572 6c73 2061 6e64 206d 6574 6164 6174  urls and metadat
-00017f40: 6120 7265 7368 6170 6564 2074 6f20 7368  a reshaped to sh
-00017f50: 6170 652e 0a20 2020 2020 2020 2022 2222  ape..        """
-00017f60: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00017f70: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00017f80: 7365 6c66 2e69 6e5f 6d65 6d6f 7279 3a0a  self.in_memory:.
-00017f90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00017fa0: 203d 2073 7570 6572 2829 2e72 6573 6861   = super().resha
-00017fb0: 7065 2873 6861 7065 2c20 6f72 6465 723d  pe(shape, order=
-00017fc0: 6f72 6465 7229 2e76 6965 7728 6e75 6d70  order).view(nump
-00017fd0: 792e 6e64 6172 7261 7929 0a20 2020 2020  y.ndarray).     
-00017fe0: 2020 2073 6361 6e5f 7368 6170 6520 3d20     scan_shape = 
-00017ff0: 7368 6170 655b 3a2d 325d 0a20 2020 2020  shape[:-2].     
-00018000: 2020 2072 6574 7572 6e20 4461 7461 280a     return Data(.
-00018010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018020: 2e75 726c 732e 7265 7368 6170 6528 7363  .urls.reshape(sc
-00018030: 616e 5f73 6861 7065 2c20 6f72 6465 723d  an_shape, order=
-00018040: 6f72 6465 7229 2c0a 2020 2020 2020 2020  order),.        
-00018050: 2020 2020 7365 6c66 2e6d 6574 6164 6174      self.metadat
-00018060: 612e 7265 7368 6170 6528 7363 616e 5f73  a.reshape(scan_s
-00018070: 6861 7065 2c20 6f72 6465 723d 6f72 6465  hape, order=orde
-00018080: 7229 2c0a 2020 2020 2020 2020 2020 2020  r),.            
-00018090: 7365 6c66 2e69 6e5f 6d65 6d6f 7279 2c0a  self.in_memory,.
-000180a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000180b0: 3d64 6174 612c 0a20 2020 2020 2020 2029  =data,.        )
-000180c0: 0a0a 2020 2020 6465 6620 7375 6d28 7365  ..    def sum(se
-000180d0: 6c66 2c20 6178 6973 3d4e 6f6e 652c 202a  lf, axis=None, *
-000180e0: 2a6b 7761 7267 7329 202d 3e20 556e 696f  *kwargs) -> Unio
-000180f0: 6e5b 6e75 6d70 792e 6e64 6172 7261 792c  n[numpy.ndarray,
-00018100: 2066 6c6f 6174 5d3a 0a20 2020 2020 2020   float]:.       
-00018110: 2022 2222 0a20 2020 2020 2020 2053 756d   """.        Sum
-00018120: 206f 6620 6172 7261 7920 656c 656d 656e   of array elemen
-00018130: 7473 206f 7665 7220 6120 6769 7665 6e20  ts over a given 
-00018140: 6178 6973 2e0a 0a20 2020 2020 2020 203a  axis...        :
-00018150: 7061 7261 6d20 6178 6973 3a20 4f6e 6c79  param axis: Only
-00018160: 2061 7869 7320 6163 6365 7074 6564 2061   axis accepted a
-00018170: 7265 2030 206f 7220 312e 0a20 2020 2020  re 0 or 1..     
-00018180: 2020 2020 2020 2057 6974 6820 302c 2074         With 0, t
-00018190: 6865 2073 756d 2069 7320 646f 6e65 2061  he sum is done a
-000181a0: 726f 756e 6420 7468 6520 7a20 6178 6973  round the z axis
-000181b0: 2c20 736f 2061 2072 6573 756c 7469 6e67  , so a resulting
-000181c0: 2069 6d61 6765 2069 7320 7265 7475 726e   image is return
-000181d0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-000181e0: 5769 7468 2031 2c20 6576 6572 7920 696d  With 1, every im
-000181f0: 6167 6573 2068 6173 2069 7473 2070 6978  ages has its pix
-00018200: 656c 7320 7375 6d6d 6564 2061 6e64 2074  els summed and t
-00018210: 6865 2072 6573 756c 7420 6973 2061 206c  he result is a l
-00018220: 6973 7420 7769 7468 0a20 2020 2020 2020  ist with.       
-00018230: 2020 2020 2074 6865 2069 6e74 656e 7369       the intensi
-00018240: 7479 206f 6620 6561 6368 2069 6d61 6765  ty of each image
-00018250: 2e0a 2020 2020 2020 2020 2020 2020 5769  ..            Wi
-00018260: 7468 204e 6f6e 652c 2061 2066 6c6f 6174  th None, a float
-00018270: 2069 7320 7468 6520 7265 7375 6c74 206f   is the result o
-00018280: 6620 7468 6520 7375 6d20 6f66 2061 6c6c  f the sum of all
-00018290: 2074 6865 2070 6978 656c 7320 616e 6420   the pixels and 
-000182a0: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
-000182b0: 7468 6520 696d 6167 6573 2e0a 2020 2020  the images..    
-000182c0: 2020 2020 3a74 7970 6520 6178 6973 3a20      :type axis: 
-000182d0: 556e 696f 6e5b 4e6f 6e65 2c20 696e 745d  Union[None, int]
-000182e0: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-000182f0: 6e3a 2053 756d 6d65 6420 6461 7461 0a20  n: Summed data. 
-00018300: 2020 2020 2020 203a 7274 7970 653a 2055         :rtype: U
-00018310: 6e69 6f6e 5b66 6c6f 6174 2c20 6c69 7374  nion[float, list
-00018320: 5d0a 2020 2020 2020 2020 2222 220a 2020  ].        """.  
-00018330: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-00018340: 662e 666c 6174 7465 6e28 290a 2020 2020  f.flatten().    
-00018350: 2020 2020 6966 2073 656c 662e 696e 5f6d      if self.in_m
-00018360: 656d 6f72 793a 0a20 2020 2020 2020 2020  emory:.         
-00018370: 2020 2069 6620 6178 6973 203d 3d20 303a     if axis == 0:
-00018380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018390: 2072 6574 7572 6e20 7375 7065 7228 4461   return super(Da
-000183a0: 7461 2c20 6461 7461 292e 7375 6d28 6178  ta, data).sum(ax
-000183b0: 6973 3d61 7869 7329 2e76 6965 7728 6e75  is=axis).view(nu
-000183c0: 6d70 792e 6e64 6172 7261 7929 0a20 2020  mpy.ndarray).   
-000183d0: 2020 2020 2020 2020 2069 6620 6178 6973           if axis
-000183e0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000183f0: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00018400: 7065 7228 4461 7461 2c20 6461 7461 292e  per(Data, data).
-00018410: 7669 6577 286e 756d 7079 2e6e 6461 7272  view(numpy.ndarr
-00018420: 6179 292e 7375 6d28 6178 6973 3d31 292e  ay).sum(axis=1).
-00018430: 7375 6d28 6178 6973 3d31 290a 2020 2020  sum(axis=1).    
-00018440: 2020 2020 2020 2020 6966 2061 7869 7320          if axis 
-00018450: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00018460: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00018470: 7375 7065 7228 4461 7461 2c20 6461 7461  super(Data, data
-00018480: 292e 7375 6d28 290a 2020 2020 2020 2020  ).sum().        
-00018490: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-000184a0: 726f 7228 2241 7869 7320 6d75 7374 2062  ror("Axis must b
-000184b0: 6520 4e6f 6e65 2c20 3020 6f72 2031 2229  e None, 0 or 1")
-000184c0: 0a20 2020 2020 2020 2069 6620 6178 6973  .        if axis
-000184d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000184e0: 2020 2069 6620 6461 7461 2e73 697a 6520     if data.size 
-000184f0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00018500: 2020 2020 2020 7265 7475 726e 206e 756d        return num
-00018510: 7079 2e61 7272 6179 285b 5d29 0a20 2020  py.array([]).   
-00018520: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00018530: 6461 7461 2e73 6861 7065 5b30 5d3a 0a20  data.shape[0]:. 
-00018540: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018550: 6574 7572 6e20 6e75 6d70 792e 7a65 726f  eturn numpy.zero
-00018560: 7328 6461 7461 5b30 5d2e 7368 6170 6529  s(data[0].shape)
-00018570: 0a20 2020 2020 2020 2020 2020 207a 7375  .            zsu
-00018580: 6d20 3d20 6e75 6d70 792e 6172 7261 7928  m = numpy.array(
-00018590: 6461 7461 5b30 5d2c 2064 7479 7065 3d6e  data[0], dtype=n
-000185a0: 756d 7079 2e66 6c6f 6174 3634 290a 2020  umpy.float64).  
-000185b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-000185c0: 696e 2072 616e 6765 2831 2c20 6c65 6e28  in range(1, len(
-000185d0: 6461 7461 2929 3a0a 2020 2020 2020 2020  data)):.        
-000185e0: 2020 2020 2020 2020 7a73 756d 202b 3d20          zsum += 
-000185f0: 6461 7461 5b69 5d0a 2020 2020 2020 2020  data[i].        
-00018600: 2020 2020 7265 7475 726e 207a 7375 6d0a      return zsum.
-00018610: 2020 2020 2020 2020 6966 2061 7869 7320          if axis 
-00018620: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00018630: 2020 7265 7475 726e 206e 756d 7079 2e61    return numpy.a
-00018640: 7272 6179 285b 692e 7375 6d28 2920 666f  rray([i.sum() fo
-00018650: 7220 6920 696e 2064 6174 615d 290a 2020  r i in data]).  
-00018660: 2020 2020 2020 6966 2061 7869 7320 6973        if axis is
-00018670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00018680: 2020 2069 6d67 5f73 756d 203d 2030 0a20     img_sum = 0. 
-00018690: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-000186a0: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-000186b0: 2020 2020 2020 2020 2020 696d 675f 7375            img_su
-000186c0: 6d20 2b3d 2069 2e73 756d 2829 0a20 2020  m += i.sum().   
-000186d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000186e0: 696d 675f 7375 6d0a 2020 2020 2020 2020  img_sum.        
-000186f0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00018700: 2241 7869 7320 6d75 7374 2062 6520 4e6f  "Axis must be No
-00018710: 6e65 2c20 3020 6f72 2031 2229 0a0a 2020  ne, 0 or 1")..  
-00018720: 2020 6465 6620 7461 6b65 2873 656c 662c    def take(self,
-00018730: 2069 6e64 6963 6573 2c20 6178 6973 3d4e   indices, axis=N
-00018740: 6f6e 652c 206f 7574 3d4e 6f6e 652c 206d  one, out=None, m
-00018750: 6f64 653d 2272 6169 7365 2229 202d 3e20  ode="raise") -> 
-00018760: 2244 6174 6122 3a0a 2020 2020 2020 2020  "Data":.        
-00018770: 2222 220a 2020 2020 2020 2020 5461 6b65  """.        Take
-00018780: 2065 6c65 6d65 6e74 7320 6672 6f6d 2075   elements from u
-00018790: 726c 7320 616e 6420 6d65 7461 6461 7461  rls and metadata
-000187a0: 2066 726f 6d20 616e 2061 7272 6179 2061   from an array a
-000187b0: 6c6f 6e67 2061 6e20 6178 6973 2e0a 0a20  long an axis... 
-000187c0: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-000187d0: 6469 6365 733a 2074 6865 2069 6e64 6963  dices: the indic
-000187e0: 6573 206f 6620 7468 6520 7661 6c75 6573  es of the values
-000187f0: 2074 6f20 6578 7472 6163 740a 2020 2020   to extract.    
-00018800: 2020 2020 3a74 7970 6520 696e 6469 6365      :type indice
-00018810: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
-00018820: 2020 2020 2020 3a70 6172 616d 2061 7869        :param axi
-00018830: 733a 2074 6865 2061 7869 7320 6f76 6572  s: the axis over
-00018840: 2077 6869 6368 2074 6f20 7365 6c65 6374   which to select
-00018850: 2076 616c 7565 732c 2064 6566 6175 6c74   values, default
-00018860: 7320 746f 204e 6f6e 650a 2020 2020 2020  s to None.      
-00018870: 2020 3a74 7970 6520 6178 6973 3a20 556e    :type axis: Un
-00018880: 696f 6e5b 4e20 6f6e 652c 2069 6e74 5d2c  ion[N one, int],
-00018890: 206f 7074 696f 6e61 6c0a 0a20 2020 2020   optional..     
-000188a0: 2020 203a 7265 7475 726e 3a20 466c 6174     :return: Flat
-000188b0: 7465 6e65 6420 6461 7461 2e0a 2020 2020  tened data..    
-000188c0: 2020 2020 3a72 7479 7065 3a20 3a63 6c61      :rtype: :cla
-000188d0: 7373 3a60 4461 7461 600a 2020 2020 2020  ss:`Data`.      
-000188e0: 2020 2222 220a 2020 2020 2020 2020 7572    """.        ur
-000188f0: 6c73 203d 206e 756d 7079 2e74 616b 6528  ls = numpy.take(
-00018900: 7365 6c66 2e75 726c 732c 2069 6e64 6963  self.urls, indic
-00018910: 6573 2c20 6178 6973 2c20 6d6f 6465 3d6d  es, axis, mode=m
-00018920: 6f64 6529 0a20 2020 2020 2020 206d 6574  ode).        met
-00018930: 6164 6174 6120 3d20 6e75 6d70 792e 7461  adata = numpy.ta
-00018940: 6b65 2873 656c 662e 6d65 7461 6461 7461  ke(self.metadata
-00018950: 2c20 696e 6469 6365 732c 2061 7869 732c  , indices, axis,
-00018960: 206d 6f64 653d 6d6f 6465 290a 2020 2020   mode=mode).    
-00018970: 2020 2020 6461 7461 203d 204e 6f6e 650a      data = None.
-00018980: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00018990: 696e 5f6d 656d 6f72 793a 0a20 2020 2020  in_memory:.     
-000189a0: 2020 2020 2020 2064 6174 6120 3d20 7375         data = su
-000189b0: 7065 7228 292e 7461 6b65 2869 6e64 6963  per().take(indic
-000189c0: 6573 2c20 6178 6973 2c20 6d6f 6465 3d6d  es, axis, mode=m
-000189d0: 6f64 6529 2e76 6965 7728 6e75 6d70 792e  ode).view(numpy.
-000189e0: 6e64 6172 7261 7929 0a20 2020 2020 2020  ndarray).       
-000189f0: 2072 6574 7572 6e20 4461 7461 2875 726c   return Data(url
-00018a00: 732c 206d 6574 6164 6174 612c 2073 656c  s, metadata, sel
-00018a10: 662e 696e 5f6d 656d 6f72 792c 2064 6174  f.in_memory, dat
-00018a20: 613d 6461 7461 290a 0a20 2020 2064 6566  a=data)..    def
-00018a30: 2066 6c61 7474 656e 2873 656c 6629 202d   flatten(self) -
-00018a40: 3e20 2244 6174 6122 3a0a 2020 2020 2020  > "Data":.      
-00018a50: 2020 2222 2246 6c61 7474 656e 7320 7468    """Flattens th
-00018a60: 6520 7363 616e 2064 696d 656e 7369 6f6e  e scan dimension
-00018a70: 732c 206e 6f74 2074 6865 2066 7261 6d65  s, not the frame
-00018a80: 2064 696d 656e 7369 6f6e 732e 0a20 2020   dimensions..   
-00018a90: 2020 2020 2054 4f44 4f3a 2074 6869 7320       TODO: this 
-00018aa0: 7368 6f75 6c64 2067 6574 2061 2064 6966  should get a dif
-00018ab0: 6665 7265 6e74 2066 756e 6374 696f 6e20  ferent function 
-00018ac0: 6e61 6d65 0a0a 2020 2020 2020 2020 3a72  name..        :r
-00018ad0: 6574 7572 6e3a 206e 6577 2064 6174 6120  eturn: new data 
-00018ae0: 7769 7468 2066 6c61 7474 656e 6564 2075  with flattened u
-00018af0: 726c 7320 616e 6420 6d65 7461 6461 7461  rls and metadata
-00018b00: 2028 6275 7420 6e6f 7420 6672 616d 6573   (but not frames
-00018b10: 292e 0a20 2020 2020 2020 203a 7274 7970  )..        :rtyp
-00018b20: 653a 203a 636c 6173 733a 6044 6174 6160  e: :class:`Data`
-00018b30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00018b40: 2020 2020 2069 6620 7365 6c66 2e6e 6672       if self.nfr
-00018b50: 616d 6573 203d 3d20 3020 6f72 2073 656c  ames == 0 or sel
-00018b60: 662e 6e64 696d 203c 3d20 333a 0a20 2020  f.ndim <= 3:.   
-00018b70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00018b80: 7365 6c66 0a20 2020 2020 2020 2064 6174  self.        dat
-00018b90: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
-00018ba0: 2069 6620 7365 6c66 2e69 6e5f 6d65 6d6f   if self.in_memo
-00018bb0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00018bc0: 6673 6861 7065 203d 2028 7365 6c66 2e6e  fshape = (self.n
-00018bd0: 6672 616d 6573 2c29 202b 2073 656c 662e  frames,) + self.
-00018be0: 6672 616d 655f 7368 6170 650a 2020 2020  frame_shape.    
-00018bf0: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00018c00: 6e6f 7420 7375 7265 2077 6879 2077 6520  not sure why we 
-00018c10: 6e65 6564 2074 6865 2076 6577 2068 6572  need the vew her
-00018c20: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00018c30: 6174 6120 3d20 7375 7065 7228 292e 7265  ata = super().re
-00018c40: 7368 6170 6528 6673 6861 7065 292e 7669  shape(fshape).vi
-00018c50: 6577 286e 756d 7079 2e6e 6461 7272 6179  ew(numpy.ndarray
-00018c60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00018c70: 2044 6174 6128 0a20 2020 2020 2020 2020   Data(.         
-00018c80: 2020 2073 656c 662e 7572 6c73 2e66 6c61     self.urls.fla
-00018c90: 7474 656e 2829 2c20 7365 6c66 2e6d 6574  tten(), self.met
-00018ca0: 6164 6174 612e 666c 6174 7465 6e28 292c  adata.flatten(),
-00018cb0: 2073 656c 662e 696e 5f6d 656d 6f72 792c   self.in_memory,
-00018cc0: 2064 6174 613d 6461 7461 0a20 2020 2020   data=data.     
-00018cd0: 2020 2029 0a0a 0a63 6c61 7373 2054 7261     )...class Tra
-00018ce0: 6e73 666f 726d 6174 696f 6e3a 0a20 2020  nsformation:.   
-00018cf0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00018d00: 6c66 2c20 6b69 6e64 3a20 7374 722c 2078  lf, kind: str, x
-00018d10: 3a20 6e75 6d70 792e 6e64 6172 7261 792c  : numpy.ndarray,
-00018d20: 2079 3a20 6e75 6d70 792e 6e64 6172 7261   y: numpy.ndarra
-00018d30: 792c 2072 6f74 6174 653a 2062 6f6f 6c29  y, rotate: bool)
-00018d40: 3a0a 2020 2020 2020 2020 7365 6c66 2e78  :.        self.x
-00018d50: 203d 2078 2020 2320 7368 6170 6520 2873   = x  # shape (s
-00018d60: 792c 2073 7829 0a20 2020 2020 2020 2073  y, sx).        s
-00018d70: 656c 662e 7920 3d20 7920 2023 2073 6861  elf.y = y  # sha
-00018d80: 7065 2028 7379 2c20 7378 290a 2020 2020  pe (sy, sx).    
-00018d90: 2020 2020 7365 6c66 2e72 6f74 6174 6520      self.rotate 
-00018da0: 3d20 726f 7461 7465 0a20 2020 2020 2020  = rotate.       
-00018db0: 2073 656c 662e 6b69 6e64 203d 206b 696e   self.kind = kin
-00018dc0: 640a 0a20 2020 2040 7072 6f70 6572 7479  d..    @property
-00018dd0: 0a20 2020 2064 6566 2073 6861 7065 2873  .    def shape(s
-00018de0: 656c 6629 202d 3e20 5475 706c 655b 696e  elf) -> Tuple[in
-00018df0: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
-00018e00: 2072 6574 7572 6e20 7365 6c66 2e78 2e73   return self.x.s
-00018e10: 6861 7065 0a0a 2020 2020 4070 726f 7065  hape..    @prope
-00018e20: 7274 790a 2020 2020 6465 6620 7378 2873  rty.    def sx(s
-00018e30: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00018e40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00018e50: 2e73 6861 7065 5b31 5d0a 0a20 2020 2040  .shape[1]..    @
-00018e60: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00018e70: 2073 7928 7365 6c66 2920 2d3e 2069 6e74   sy(self) -> int
-00018e80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00018e90: 2073 656c 662e 7368 6170 655b 305d 0a0a   self.shape[0]..
-00018ea0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00018eb0: 2020 6465 6620 6c61 6265 6c28 7365 6c66    def label(self
-00018ec0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00018ed0: 2020 7265 7475 726e 2022 6465 6772 6565    return "degree
-00018ee0: 7322 2069 6620 7365 6c66 2e6b 696e 6420  s" if self.kind 
-00018ef0: 3d3d 2022 7273 6d22 2065 6c73 6520 22c2  == "rsm" else ".
-00018f00: b56d 220a 0a20 2020 2040 7072 6f70 6572  .m"..    @proper
-00018f10: 7479 0a20 2020 2064 6566 2078 7265 6775  ty.    def xregu
-00018f20: 6c61 7228 7365 6c66 2920 2d3e 206e 756d  lar(self) -> num
-00018f30: 7079 2e6e 6461 7272 6179 3a0a 2020 2020  py.ndarray:.    
-00018f40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00018f50: 7873 6361 6c65 202a 206e 756d 7079 2e61  xscale * numpy.a
-00018f60: 7261 6e67 6528 7365 6c66 2e73 7829 202b  range(self.sx) +
-00018f70: 2073 656c 662e 786f 7269 6769 6e0a 0a20   self.xorigin.. 
-00018f80: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00018f90: 2064 6566 2079 7265 6775 6c61 7228 7365   def yregular(se
-00018fa0: 6c66 2920 2d3e 206e 756d 7079 2e6e 6461  lf) -> numpy.nda
-00018fb0: 7272 6179 3a0a 2020 2020 2020 2020 7265  rray:.        re
-00018fc0: 7475 726e 2073 656c 662e 7973 6361 6c65  turn self.yscale
-00018fd0: 202a 206e 756d 7079 2e61 7261 6e67 6528   * numpy.arange(
-00018fe0: 7365 6c66 2e73 7929 202b 2073 656c 662e  self.sy) + self.
-00018ff0: 796f 7269 6769 6e0a 0a20 2020 2040 7072  yorigin..    @pr
-00019000: 6f70 6572 7479 0a20 2020 2064 6566 2078  operty.    def x
-00019010: 6f72 6967 696e 2873 656c 6629 202d 3e20  origin(self) -> 
-00019020: 4e75 6d62 6572 3a0a 2020 2020 2020 2020  Number:.        
-00019030: 7265 7475 726e 2073 656c 662e 785b 305d  return self.x[0]
-00019040: 5b30 5d0a 0a20 2020 2040 7072 6f70 6572  [0]..    @proper
-00019050: 7479 0a20 2020 2064 6566 2079 6f72 6967  ty.    def yorig
-00019060: 696e 2873 656c 6629 202d 3e20 4e75 6d62  in(self) -> Numb
-00019070: 6572 3a0a 2020 2020 2020 2020 7265 7475  er:.        retu
-00019080: 726e 2073 656c 662e 795b 305d 5b30 5d0a  rn self.y[0][0].
-00019090: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000190a0: 2020 2064 6566 206f 7269 6769 6e28 7365     def origin(se
-000190b0: 6c66 2920 2d3e 2054 7570 6c65 5b4e 756d  lf) -> Tuple[Num
-000190c0: 6265 722c 204e 756d 6265 725d 3a0a 2020  ber, Number]:.  
-000190d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000190e0: 662e 786f 7269 6769 6e2c 2073 656c 662e  f.xorigin, self.
-000190f0: 796f 7269 6769 6e0a 0a20 2020 2040 7072  yorigin..    @pr
-00019100: 6f70 6572 7479 0a20 2020 2064 6566 2078  operty.    def x
-00019110: 7363 616c 6528 7365 6c66 2920 2d3e 204e  scale(self) -> N
-00019120: 756d 6265 723a 0a20 2020 2020 2020 2078  umber:.        x
-00019130: 203d 2073 656c 662e 780a 2020 2020 2020   = self.x.      
-00019140: 2020 7265 7475 726e 2028 785b 2d31 5d5b    return (x[-1][
-00019150: 2d31 5d20 2d20 785b 305d 5b30 5d29 202f  -1] - x[0][0]) /
-00019160: 2073 656c 662e 7378 0a0a 2020 2020 4070   self.sx..    @p
-00019170: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00019180: 7973 6361 6c65 2873 656c 6629 202d 3e20  yscale(self) -> 
-00019190: 4e75 6d62 6572 3a0a 2020 2020 2020 2020  Number:.        
-000191a0: 7920 3d20 7365 6c66 2e79 0a20 2020 2020  y = self.y.     
-000191b0: 2020 2072 6574 7572 6e20 2879 5b2d 315d     return (y[-1]
-000191c0: 5b2d 315d 202d 2079 5b30 5d5b 305d 2920  [-1] - y[0][0]) 
-000191d0: 2f20 7365 6c66 2e73 790a 0a20 2020 2040  / self.sy..    @
-000191e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000191f0: 2073 6361 6c65 2873 656c 6629 202d 3e20   scale(self) -> 
-00019200: 5475 706c 655b 4e75 6d62 6572 2c20 4e75  Tuple[Number, Nu
-00019210: 6d62 6572 5d3a 0a20 2020 2020 2020 2072  mber]:.        r
-00019220: 6574 7572 6e20 7365 6c66 2e78 7363 616c  eturn self.xscal
-00019230: 652c 2073 656c 662e 7973 6361 6c65 0a0a  e, self.yscale..
-00019240: 0a63 6c61 7373 205f 4844 4635 4d65 7461  .class _HDF5Meta
-00019250: 6461 7461 5265 6164 6572 3a0a 2020 2020  dataReader:.    
-00019260: 2222 220a 2020 2020 4571 7569 7661 6c65  """.    Equivale
-00019270: 6e74 206f 6620 7369 6c78 2e69 6f2e 6661  nt of silx.io.fa
-00019280: 6269 6f68 352e 4661 6269 6f52 6561 6465  bioh5.FabioReade
-00019290: 7220 746f 2067 6976 6520 6163 6365 7373  r to give access
-000192a0: 2074 6f20 4844 4635 206d 6574 6164 6174   to HDF5 metadat
-000192b0: 610a 0a20 2020 2046 4958 4d45 3a20 7265  a..    FIXME: re
-000192c0: 6d6f 7665 2074 6869 7320 636c 6173 732e  move this class.
-000192d0: 2053 746f 7261 6765 2061 6e64 2072 6561   Storage and rea
-000192e0: 6469 6e67 206f 6620 6d65 7461 6461 7461  ding of metadata
-000192f0: 2068 6173 2062 6565 6e20 6261 7365 6420   has been based 
-00019300: 6f6e 2045 4446 2e20 5468 6973 2063 6c61  on EDF. This cla
-00019310: 7373 2069 7320 6120 776f 726b 2d61 726f  ss is a work-aro
-00019320: 756e 640a 2020 2020 4465 7369 676e 206f  und.    Design o
-00019330: 6620 6861 6e64 6c65 206d 6574 6164 6174  f handle metadat
-00019340: 6120 7368 6f75 6c64 6e27 7420 6265 2062  a shouldn't be b
-00019350: 6173 6564 206f 6e20 7468 6520 6461 7461  ased on the data
-00019360: 2074 7970 6520 6275 7420 6d6f 7265 2061   type but more a
-00019370: 6273 7472 6163 7465 640a 2020 2020 2222  bstracted.    ""
-00019380: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00019390: 745f 5f28 7365 6c66 2c20 6d65 7461 6461  t__(self, metada
-000193a0: 7461 3a20 6469 6374 2920 2d3e 204e 6f6e  ta: dict) -> Non
-000193b0: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
-000193c0: 5f5f 6d65 7461 6461 7461 203d 206d 6574  __metadata = met
-000193d0: 6164 6174 610a 0a20 2020 2064 6566 2067  adata..    def g
-000193e0: 6574 5f76 616c 7565 2873 656c 662c 206b  et_value(self, k
-000193f0: 696e 642c 206e 616d 6529 3a0a 2020 2020  ind, name):.    
-00019400: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00019410: 5f5f 6d65 7461 6461 7461 2e67 6574 286e  __metadata.get(n
-00019420: 616d 652c 204e 6f6e 6529 0a0a 2020 2020  ame, None)..    
-00019430: 6465 6620 6765 745f 6b65 7973 2873 656c  def get_keys(sel
-00019440: 662c 206b 696e 6429 3a0a 2020 2020 2020  f, kind):.      
-00019450: 2020 7265 7475 726e 2074 7570 6c65 2873    return tuple(s
-00019460: 656c 662e 5f5f 6d65 7461 6461 7461 2e6b  elf.__metadata.k
-00019470: 6579 7328 2929 0a                        eys()).
+00016de0: 2020 2066 696c 655f 7061 7468 3d73 6176     file_path=sav
+00016df0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 2064 6174 615f 7061 7468 3d22 2f64     data_path="/d
+00016e20: 6174 6173 6574 222c 0a20 2020 2020 2020  ataset",.       
+00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e40: 2020 2020 2020 2020 2064 6174 615f 736c           data_sl
+00016e50: 6963 653d 692c 0a20 2020 2020 2020 2020  ice=i,.         
+00016e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e70: 2020 2020 2020 2073 6368 656d 653d 2273         scheme="s
+00016e80: 696c 7822 2c0a 2020 2020 2020 2020 2020  ilx",.          
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ea0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00016eb0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ed0: 2020 2020 2020 2320 6669 6c65 6e61 6d65        # filename
+00016ee0: 203d 2073 6176 6520 2b20 7374 7228 6929   = save + str(i)
+00016ef0: 2e7a 6669 6c6c 2834 2920 2b20 222e 6e70  .zfill(4) + ".np
+00016f00: 7922 0a20 2020 2020 2020 2020 2020 2020  y".             
+00016f10: 2020 2020 2020 2020 2020 2023 206e 756d             # num
+00016f20: 7079 2e73 6176 6528 6669 6c65 6e61 6d65  py.save(filename
+00016f30: 2c20 696d 6729 0a20 2020 2020 2020 2020  , img).         
+00016f40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00016f50: 2075 726c 732e 6170 7065 6e64 2844 6174   urls.append(Dat
+00016f60: 6155 726c 2866 696c 655f 7061 7468 3d66  aUrl(file_path=f
+00016f70: 696c 656e 616d 652c 2073 6368 656d 653d  ilename, scheme=
+00016f80: 2766 6162 696f 2729 290a 2020 2020 2020  'fabio')).      
+00016f90: 2020 2020 2020 2020 2020 2020 2020 696f                io
+00016fa0: 5f75 7469 6c73 2e61 6476 616e 6365 6d65  _utils.advanceme
+00016fb0: 6e74 5f64 6973 706c 6179 2869 202b 2031  nt_display(i + 1
+00016fc0: 2c20 7365 6c66 2e6e 6672 616d 6573 2c20  , self.nframes, 
+00016fd0: 7465 7874 290a 0a20 2020 2020 2020 2020  text)..         
+00016fe0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00016ff0: 655f 6f66 5f6f 7065 7261 7469 6f6e 732e  e_of_operations.
+00017000: 7374 6f70 286f 7065 7261 7469 6f6e 290a  stop(operation).
+00017010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017020: 2069 6620 6461 7461 7365 745f 6e61 6d65   if dataset_name
+00017030: 203d 3d20 2275 7064 6174 655f 6461 7461   == "update_data
+00017040: 7365 7422 3a0a 2020 2020 2020 2020 2020  set":.          
+00017050: 2020 2020 2020 2020 2020 6465 6c20 5f66            del _f
+00017060: 696c 655b 2264 6174 6173 6574 225d 0a20  ile["dataset"]. 
+00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017080: 2020 205f 6669 6c65 5b22 6461 7461 7365     _file["datase
+00017090: 7422 5d20 3d20 5f66 696c 655b 2275 7064  t"] = _file["upd
+000170a0: 6174 655f 6461 7461 7365 7422 5d0a 2020  ate_dataset"].  
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170c0: 2020 6465 6c20 5f66 696c 655b 2275 7064    del _file["upd
+000170d0: 6174 655f 6461 7461 7365 7422 5d0a 2020  ate_dataset"].  
+000170e0: 2020 2020 2020 2020 2020 6669 6e61 6c6c            finall
+000170f0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00017100: 2020 2069 6620 5f66 696c 6520 6973 206e     if _file is n
+00017110: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017120: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
+00017130: 6c65 2e63 6c6f 7365 2829 0a20 2020 2020  le.close().     
+00017140: 2020 2072 6574 7572 6e20 6e75 6d70 792e     return numpy.
+00017150: 6172 7261 7928 7572 6c73 290a 0a20 2020  array(urls)..   
+00017160: 2064 6566 2073 6176 6528 7365 6c66 2c20   def save(self, 
+00017170: 7061 7468 2c20 696e 6469 6365 733d 4e6f  path, indices=No
+00017180: 6e65 2c20 6e65 775f 7368 6170 653d 4e6f  ne, new_shape=No
+00017190: 6e65 2c20 696e 5f6d 656d 6f72 793d 5472  ne, in_memory=Tr
+000171a0: 7565 2920 2d3e 204e 6f6e 653a 0a20 2020  ue) -> None:.   
+000171b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000171c0: 2053 6176 6520 7468 6520 6461 7461 2069   Save the data i
+000171d0: 6e74 6f20 6070 6174 6860 2066 6f6c 6465  nto `path` folde
+000171e0: 7220 616e 6420 7265 706c 6163 6520 4461  r and replace Da
+000171f0: 7461 2075 726c 732e 0a20 2020 2020 2020  ta urls..       
+00017200: 2054 4f44 4f3a 2063 6865 636b 2069 6620   TODO: check if 
+00017210: 7572 6c73 2061 6c72 6561 6479 2065 7869  urls already exi
+00017220: 7374 2061 6e64 2c20 6966 2073 6f2c 206d  st and, if so, m
+00017230: 6f64 6966 7920 6f6e 6c79 2075 726c 735b  odify only urls[
+00017240: 696e 6469 6365 735d 2e0a 0a20 2020 2020  indices]...     
+00017250: 2020 203a 7061 7261 6d20 7061 7468 3a20     :param path: 
+00017260: 5061 7468 2074 6f20 7468 6520 666f 6c64  Path to the fold
+00017270: 6572 0a20 2020 2020 2020 203a 7479 7065  er.        :type
+00017280: 2070 6174 683a 2073 7472 0a20 2020 2020   path: str.     
+00017290: 2020 203a 7061 7261 6d20 696e 6469 6365     :param indice
+000172a0: 733a 2074 6865 2069 6e64 6963 6573 206f  s: the indices o
+000172b0: 6620 7468 6520 7661 6c75 6573 2074 6f20  f the values to 
+000172c0: 7361 7665 2c20 6465 6661 756c 7473 2074  save, defaults t
+000172d0: 6f20 4e6f 6e65 0a20 2020 2020 2020 203a  o None.        :
+000172e0: 7479 7065 2069 6e64 6963 6573 3a20 556e  type indices: Un
+000172f0: 696f 6e5b 4e6f 6e65 2c61 7272 6179 5f6c  ion[None,array_l
+00017300: 696b 655d 2c20 6f70 7469 6f6e 616c 0a20  ike], optional. 
+00017310: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017320: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
+00017330: 7228 7365 6c66 2c20 2269 6e5f 6d65 6d6f  r(self, "in_memo
+00017340: 7279 2229 206f 7220 7365 6c66 2e69 6e5f  ry") or self.in_
+00017350: 6d65 6d6f 7279 2069 7320 4e6f 6e65 3a0a  memory is None:.
+00017360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017370: 2e69 6e5f 6d65 6d6f 7279 203d 2054 7275  .in_memory = Tru
+00017380: 650a 2020 2020 2020 2020 7572 6c73 203d  e.        urls =
+00017390: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
+000173a0: 696e 6469 6365 7320 6973 204e 6f6e 653a  indices is None:
+000173b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000173c0: 6120 3d20 7365 6c66 2e66 6c61 7474 656e  a = self.flatten
+000173d0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+000173e0: 6e64 6963 6573 203d 206e 756d 7079 2e61  ndices = numpy.a
+000173f0: 7261 6e67 6528 6c65 6e28 6461 7461 2929  range(len(data))
+00017400: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00017410: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00017420: 3d20 7365 6c66 2e66 6c61 7474 656e 2829  = self.flatten()
+00017430: 5b69 6e64 6963 6573 5d0a 0a20 2020 2020  [indices]..     
+00017440: 2020 205f 6669 6c65 203d 204e 6f6e 650a     _file = None.
+00017450: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00017460: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00017470: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
+00017480: 696c 6520 3d20 6835 7079 2e46 696c 6528  ile = h5py.File(
+00017490: 7061 7468 2c20 2261 2229 0a20 2020 2020  path, "a").     
+000174a0: 2020 2020 2020 2065 7863 6570 7420 4f53         except OS
+000174b0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+000174c0: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+000174d0: 682e 6578 6973 7473 2870 6174 6829 3a0a  h.exists(path):.
+000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174f0: 2020 2020 6f73 2e72 656d 6f76 6528 7061      os.remove(pa
+00017500: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+00017510: 2020 2020 5f66 696c 6520 3d20 6835 7079      _file = h5py
+00017520: 2e46 696c 6528 7061 7468 2c20 2277 2229  .File(path, "w")
+00017530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017540: 6e65 775f 7368 6170 653a 0a20 2020 2020  new_shape:.     
+00017550: 2020 2020 2020 2020 2020 206e 6577 5f73             new_s
+00017560: 6861 7065 203d 2074 7570 6c65 286e 6577  hape = tuple(new
+00017570: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
+00017580: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017590: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000175a0: 662e 6e64 696d 203e 2033 3a0a 2020 2020  f.ndim > 3:.    
+000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175c0: 6e65 775f 7368 6170 6520 3d20 2873 656c  new_shape = (sel
+000175d0: 662e 6e66 7261 6d65 732c 2920 2b20 7365  f.nframes,) + se
+000175e0: 6c66 2e66 7261 6d65 5f73 6861 7065 0a20  lf.frame_shape. 
+000175f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017600: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00017610: 2020 2020 2020 2020 206e 6577 5f73 6861           new_sha
+00017620: 7065 203d 2073 656c 662e 7368 6170 650a  pe = self.shape.
+00017630: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00017640: 6461 7461 7365 7422 206e 6f74 2069 6e20  dataset" not in 
+00017650: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
+00017660: 2020 2020 2020 205f 6669 6c65 2e63 7265         _file.cre
+00017670: 6174 655f 6461 7461 7365 7428 2264 6174  ate_dataset("dat
+00017680: 6173 6574 222c 206e 6577 5f73 6861 7065  aset", new_shape
+00017690: 2c20 6474 7970 653d 7365 6c66 2e64 7479  , dtype=self.dty
+000176a0: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+000176b0: 656c 6966 206e 6577 5f73 6861 7065 2021  elif new_shape !
+000176c0: 3d20 5f66 696c 655b 2264 6174 6173 6574  = _file["dataset
+000176d0: 225d 2e73 6861 7065 3a0a 2020 2020 2020  "].shape:.      
+000176e0: 2020 2020 2020 2020 2020 6465 6c20 5f66            del _f
+000176f0: 696c 655b 2264 6174 6173 6574 225d 0a20  ile["dataset"]. 
+00017700: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00017710: 6669 6c65 2e63 7265 6174 655f 6461 7461  file.create_data
+00017720: 7365 7428 2264 6174 6173 6574 222c 206e  set("dataset", n
+00017730: 6577 5f73 6861 7065 2c20 6474 7970 653d  ew_shape, dtype=
+00017740: 7365 6c66 2e64 7479 7065 290a 0a20 2020  self.dtype)..   
+00017750: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00017760: 6a20 696e 2065 6e75 6d65 7261 7465 2869  j in enumerate(i
+00017770: 6e64 6963 6573 293a 0a20 2020 2020 2020  ndices):.       
+00017780: 2020 2020 2020 2020 205f 6669 6c65 5b22           _file["
+00017790: 6461 7461 7365 7422 5d5b 6a5d 203d 2064  dataset"][j] = d
+000177a0: 6174 615b 695d 0a20 2020 2020 2020 2020  ata[i].         
+000177b0: 2020 2020 2020 2075 726c 732e 6170 7065         urls.appe
+000177c0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+000177d0: 2020 2020 2020 2020 4461 7461 5572 6c28          DataUrl(
+000177e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000177f0: 2020 2020 2020 2020 2066 696c 655f 7061           file_pa
+00017800: 7468 3d70 6174 682c 0a20 2020 2020 2020  th=path,.       
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 2064 6174 615f 7061 7468 3d22 2f64 6174   data_path="/dat
+00017830: 6173 6574 222c 0a20 2020 2020 2020 2020  aset",.         
+00017840: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017850: 6174 615f 736c 6963 653d 6a2c 0a20 2020  ata_slice=j,.   
+00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017870: 2020 2020 2073 6368 656d 653d 2273 696c       scheme="sil
+00017880: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
+00017890: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000178a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000178b0: 2020 2020 2020 2020 2320 2020 2020 6669          #     fi
+000178c0: 6c65 6e61 6d65 203d 2070 6174 6820 2b20  lename = path + 
+000178d0: 7374 7228 6929 2e7a 6669 6c6c 2834 2920  str(i).zfill(4) 
+000178e0: 2b20 222e 6e70 7922 0a20 2020 2020 2020  + ".npy".       
+000178f0: 2020 2020 2023 2020 2020 206e 756d 7079       #     numpy
+00017900: 2e73 6176 6528 6669 6c65 6e61 6d65 2c20  .save(filename, 
+00017910: 696d 6729 0a20 2020 2020 2020 2020 2020  img).           
+00017920: 2023 2020 2020 2075 726c 732e 6170 7065   #     urls.appe
+00017930: 6e64 2844 6174 6155 726c 2866 696c 655f  nd(DataUrl(file_
+00017940: 7061 7468 3d66 696c 656e 616d 652c 2073  path=filename, s
+00017950: 6368 656d 653d 2766 6162 696f 2729 290a  cheme='fabio')).
+00017960: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
+00017970: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017980: 5f66 696c 6520 6973 206e 6f74 204e 6f6e  _file is not Non
+00017990: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000179a0: 2020 205f 6669 6c65 2e63 6c6f 7365 2829     _file.close()
+000179b0: 0a20 2020 2020 2020 2075 726c 7320 3d20  .        urls = 
+000179c0: 6e75 6d70 792e 6173 6172 7261 7928 7572  numpy.asarray(ur
+000179d0: 6c73 290a 2020 2020 2020 2020 6966 2073  ls).        if s
+000179e0: 656c 662e 7572 6c73 2069 7320 6e6f 7420  elf.urls is not 
+000179f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017a00: 2020 6e65 775f 7572 6c73 203d 2073 656c    new_urls = sel
+00017a10: 662e 7572 6c73 2e66 6c61 7474 656e 2829  f.urls.flatten()
+00017a20: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+00017a30: 5f75 726c 735b 696e 6469 6365 735d 203d  _urls[indices] =
+00017a40: 2075 726c 730a 2020 2020 2020 2020 2020   urls.          
+00017a50: 2020 7365 6c66 2e75 726c 7320 3d20 6e65    self.urls = ne
+00017a60: 775f 7572 6c73 2e72 6573 6861 7065 2873  w_urls.reshape(s
+00017a70: 656c 662e 7572 6c73 2e73 6861 7065 290a  elf.urls.shape).
+00017a80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00017a90: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00017aa0: 726c 7320 3d20 6e75 6d70 792e 6173 6172  rls = numpy.asar
+00017ab0: 7261 7928 7572 6c73 290a 0a20 2020 2040  ray(urls)..    @
+00017ac0: 636f 6e74 6578 746d 616e 6167 6572 0a20  contextmanager. 
+00017ad0: 2020 2064 6566 206f 7065 6e5f 6173 5f68     def open_as_h
+00017ae0: 6466 3528 7365 6c66 2c20 5f64 6972 2920  df5(self, _dir) 
+00017af0: 2d3e 2047 656e 6572 6174 6f72 5b68 3570  -> Generator[h5p
+00017b00: 792e 4461 7461 7365 742c 204e 6f6e 652c  y.Dataset, None,
+00017b10: 204e 6f6e 655d 3a0a 2020 2020 2020 2020   None]:.        
+00017b20: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
+00017b30: 6572 7473 2074 6865 2064 6174 6120 696e  erts the data in
+00017b40: 746f 2061 6e20 4844 4635 2066 696c 652c  to an HDF5 file,
+00017b50: 2073 6574 7469 6e67 2066 6c61 7474 656e   setting flatten
+00017b60: 6564 2069 6d61 6765 7320 696e 2074 6865  ed images in the
+00017b70: 2072 6f77 732e 0a20 2020 2020 2020 2054   rows..        T
+00017b80: 4f44 4f3a 2070 6173 7320 6669 6c65 6e61  ODO: pass filena
+00017b90: 6d65 2070 6572 2070 6172 616d 6574 6572  me per parameter
+00017ba0: 3f0a 0a20 2020 2020 2020 203a 7061 7261  ?..        :para
+00017bb0: 6d20 5f64 6972 3a20 4469 7265 6374 6f72  m _dir: Director
+00017bc0: 7920 696e 2077 6869 6368 2074 6f20 7361  y in which to sa
+00017bd0: 7665 2074 6865 2048 4446 3520 6669 6c65  ve the HDF5 file
+00017be0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00017bf0: 5f64 6972 3a20 7374 720a 0a20 2020 2020  _dir: str..     
+00017c00: 2020 203a 7265 7475 726e 3a20 4844 4635     :return: HDF5
+00017c10: 2064 6174 6173 6574 0a20 2020 2020 2020   dataset.       
+00017c20: 203a 7274 7970 653a 2060 6835 7079 2e44   :rtype: `h5py.D
+00017c30: 6174 6173 6574 600a 2020 2020 2020 2020  ataset`.        
+00017c40: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
+00017c50: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00017c60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017c70: 2020 6669 6c65 6e61 6d65 203d 206f 732e    filename = os.
+00017c80: 7061 7468 2e6a 6f69 6e28 5f64 6972 2c20  path.join(_dir, 
+00017c90: 2264 6174 612e 6864 6635 2229 0a20 2020  "data.hdf5").   
+00017ca0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017cb0: 662e 5f66 696c 6520 3d20 6835 7079 2e46  f._file = h5py.F
+00017cc0: 696c 6528 6669 6c65 6e61 6d65 2c20 2261  ile(filename, "a
+00017cd0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+00017ce0: 7863 6570 7420 4f53 4572 726f 723a 0a20  xcept OSError:. 
+00017cf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017d00: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+00017d10: 2866 696c 656e 616d 6529 3a0a 2020 2020  (filename):.    
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d30: 6f73 2e72 656d 6f76 6528 6669 6c65 6e61  os.remove(filena
+00017d40: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00017d50: 2020 2020 7365 6c66 2e5f 6669 6c65 203d      self._file =
+00017d60: 2068 3570 792e 4669 6c65 2866 696c 656e   h5py.File(filen
+00017d70: 616d 652c 2022 7722 290a 0a20 2020 2020  ame, "w")..     
+00017d80: 2020 2020 2020 206e 6672 616d 6573 203d         nframes =
+00017d90: 2073 656c 662e 6e66 7261 6d65 730a 2020   self.nframes.  
+00017da0: 2020 2020 2020 2020 2020 6672 616d 655f            frame_
+00017db0: 7368 6170 6520 3d20 7365 6c66 2e66 7261  shape = self.fra
+00017dc0: 6d65 5f73 6861 7065 0a20 2020 2020 2020  me_shape.       
+00017dd0: 2020 2020 2066 7261 6d65 5f73 697a 6520       frame_size 
+00017de0: 3d20 6672 616d 655f 7368 6170 655b 305d  = frame_shape[0]
+00017df0: 202a 2066 7261 6d65 5f73 6861 7065 5b31   * frame_shape[1
+00017e00: 5d0a 2020 2020 2020 2020 2020 2020 6864  ].            hd
+00017e10: 6635 5f73 6861 7065 203d 2028 6e66 7261  f5_shape = (nfra
+00017e20: 6d65 732c 2066 7261 6d65 5f73 697a 6529  mes, frame_size)
+00017e30: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00017e40: 2022 6461 7461 7365 7422 2069 6e20 7365   "dataset" in se
+00017e50: 6c66 2e5f 6669 6c65 2061 6e64 2073 656c  lf._file and sel
+00017e60: 662e 5f66 696c 655b 2264 6174 6173 6574  f._file["dataset
+00017e70: 225d 2e73 6861 7065 2021 3d20 6864 6635  "].shape != hdf5
+00017e80: 5f73 6861 7065 3a0a 2020 2020 2020 2020  _shape:.        
+00017e90: 2020 2020 2020 2020 6465 6c20 7365 6c66          del self
+00017ea0: 2e5f 6669 6c65 5b22 6461 7461 7365 7422  ._file["dataset"
+00017eb0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00017ec0: 2022 6461 7461 7365 7422 206e 6f74 2069   "dataset" not i
+00017ed0: 6e20 7365 6c66 2e5f 6669 6c65 3a0a 2020  n self._file:.  
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017ef0: 6c66 2e5f 6669 6c65 2e63 7265 6174 655f  lf._file.create_
+00017f00: 6461 7461 7365 7428 2264 6174 6173 6574  dataset("dataset
+00017f10: 222c 2073 6861 7065 3d68 6466 355f 7368  ", shape=hdf5_sh
+00017f20: 6170 652c 2064 7479 7065 3d73 656c 662e  ape, dtype=self.
+00017f30: 6474 7970 6529 0a0a 2020 2020 2020 2020  dtype)..        
+00017f40: 2020 2020 666f 7220 696d 6167 655f 6964      for image_id
+00017f50: 782c 2066 7261 6d65 2069 6e20 656e 756d  x, frame in enum
+00017f60: 6572 6174 6528 7365 6c66 2e5f 6974 6572  erate(self._iter
+00017f70: 5f66 7261 6d65 7328 2929 3a0a 2020 2020  _frames()):.    
+00017f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017f90: 2e5f 6669 6c65 5b22 6461 7461 7365 7422  ._file["dataset"
+00017fa0: 5d5b 696d 6167 655f 6964 785d 203d 2066  ][image_idx] = f
+00017fb0: 7261 6d65 2e66 6c61 7474 656e 2829 0a0a  rame.flatten()..
+00017fc0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00017fd0: 6420 7365 6c66 2e5f 6669 6c65 5b22 6461  d self._file["da
+00017fe0: 7461 7365 7422 5d0a 2020 2020 2020 2020  taset"].        
+00017ff0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+00018000: 2020 2020 2069 6620 7365 6c66 2e5f 6669       if self._fi
+00018010: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 7365 6c66 2e5f 6669 6c65 2e63 6c6f 7365  self._file.close
+00018040: 2829 0a0a 2020 2020 6465 6620 7265 7368  ()..    def resh
+00018050: 6170 6528 7365 6c66 2c20 7368 6170 652c  ape(self, shape,
+00018060: 206f 7264 6572 3d22 4322 2920 2d3e 2022   order="C") -> "
+00018070: 4461 7461 223a 0a20 2020 2020 2020 2022  Data":.        "
+00018080: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+00018090: 6e73 2061 6e20 6172 7261 7920 636f 6e74  ns an array cont
+000180a0: 6169 6e69 6e67 2074 6865 2073 616d 6520  aining the same 
+000180b0: 6461 7461 2077 6974 6820 6120 6e65 7720  data with a new 
+000180c0: 7368 6170 6520 6f66 2075 726c 7320 616e  shape of urls an
+000180d0: 6420 6d65 7461 6461 7461 2e0a 2020 2020  d metadata..    
+000180e0: 2020 2020 5368 6170 6520 616c 736f 2063      Shape also c
+000180f0: 6f6e 7461 696e 7320 696d 6167 6520 7368  ontains image sh
+00018100: 6170 6520 6174 2074 6865 206c 6173 7420  ape at the last 
+00018110: 7477 6f20 706f 7369 7469 6f6e 7320 2875  two positions (u
+00018120: 6e72 6573 6861 7061 626c 6529 2e0a 0a20  nreshapable)... 
+00018130: 2020 2020 2020 203a 7061 7261 6d20 7368         :param sh
+00018140: 6170 653a 204e 6577 2073 6861 7065 2c20  ape: New shape, 
+00018150: 7368 6f75 6c64 2062 6520 636f 6d70 6174  should be compat
+00018160: 6962 6c65 2077 6974 6820 7468 6520 6f72  ible with the or
+00018170: 6967 696e 616c 2073 6861 7065 2e0a 2020  iginal shape..  
+00018180: 2020 2020 2020 3a74 7970 6520 7368 6170        :type shap
+00018190: 653a 2069 6e74 206f 7220 7475 706c 6520  e: int or tuple 
+000181a0: 6f66 2069 6e74 732e 0a20 2020 2020 2020  of ints..       
+000181b0: 203a 7265 7475 726e 3a20 6e65 7720 4461   :return: new Da
+000181c0: 7461 206f 626a 6563 7420 7769 7468 2075  ta object with u
+000181d0: 726c 7320 616e 6420 6d65 7461 6461 7461  rls and metadata
+000181e0: 2072 6573 6861 7065 6420 746f 2073 6861   reshaped to sha
+000181f0: 7065 2e0a 2020 2020 2020 2020 2222 220a  pe..        """.
+00018200: 2020 2020 2020 2020 6461 7461 203d 204e          data = N
+00018210: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+00018220: 656c 662e 696e 5f6d 656d 6f72 793a 0a20  elf.in_memory:. 
+00018230: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00018240: 3d20 7375 7065 7228 292e 7265 7368 6170  = super().reshap
+00018250: 6528 7368 6170 652c 206f 7264 6572 3d6f  e(shape, order=o
+00018260: 7264 6572 292e 7669 6577 286e 756d 7079  rder).view(numpy
+00018270: 2e6e 6461 7272 6179 290a 2020 2020 2020  .ndarray).      
+00018280: 2020 7363 616e 5f73 6861 7065 203d 2073    scan_shape = s
+00018290: 6861 7065 5b3a 2d32 5d0a 2020 2020 2020  hape[:-2].      
+000182a0: 2020 7265 7475 726e 2044 6174 6128 0a20    return Data(. 
+000182b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000182c0: 7572 6c73 2e72 6573 6861 7065 2873 6361  urls.reshape(sca
+000182d0: 6e5f 7368 6170 652c 206f 7264 6572 3d6f  n_shape, order=o
+000182e0: 7264 6572 292c 0a20 2020 2020 2020 2020  rder),.         
+000182f0: 2020 2073 656c 662e 6d65 7461 6461 7461     self.metadata
+00018300: 2e72 6573 6861 7065 2873 6361 6e5f 7368  .reshape(scan_sh
+00018310: 6170 652c 206f 7264 6572 3d6f 7264 6572  ape, order=order
+00018320: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
+00018330: 656c 662e 696e 5f6d 656d 6f72 792c 0a20  elf.in_memory,. 
+00018340: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+00018350: 6461 7461 2c0a 2020 2020 2020 2020 290a  data,.        ).
+00018360: 0a20 2020 2064 6566 2073 756d 2873 656c  .    def sum(sel
+00018370: 662c 2061 7869 733d 4e6f 6e65 2c20 2a2a  f, axis=None, **
+00018380: 6b77 6172 6773 2920 2d3e 2055 6e69 6f6e  kwargs) -> Union
+00018390: 5b6e 756d 7079 2e6e 6461 7272 6179 2c20  [numpy.ndarray, 
+000183a0: 666c 6f61 745d 3a0a 2020 2020 2020 2020  float]:.        
+000183b0: 2222 220a 2020 2020 2020 2020 5375 6d20  """.        Sum 
+000183c0: 6f66 2061 7272 6179 2065 6c65 6d65 6e74  of array element
+000183d0: 7320 6f76 6572 2061 2067 6976 656e 2061  s over a given a
+000183e0: 7869 732e 0a0a 2020 2020 2020 2020 3a70  xis...        :p
+000183f0: 6172 616d 2061 7869 733a 204f 6e6c 7920  aram axis: Only 
+00018400: 6178 6973 2061 6363 6570 7465 6420 6172  axis accepted ar
+00018410: 6520 3020 6f72 2031 2e0a 2020 2020 2020  e 0 or 1..      
+00018420: 2020 2020 2020 5769 7468 2030 2c20 7468        With 0, th
+00018430: 6520 7375 6d20 6973 2064 6f6e 6520 6172  e sum is done ar
+00018440: 6f75 6e64 2074 6865 207a 2061 7869 732c  ound the z axis,
+00018450: 2073 6f20 6120 7265 7375 6c74 696e 6720   so a resulting 
+00018460: 696d 6167 6520 6973 2072 6574 7572 6e65  image is returne
+00018470: 642e 0a20 2020 2020 2020 2020 2020 2057  d..            W
+00018480: 6974 6820 312c 2065 7665 7279 2069 6d61  ith 1, every ima
+00018490: 6765 7320 6861 7320 6974 7320 7069 7865  ges has its pixe
+000184a0: 6c73 2073 756d 6d65 6420 616e 6420 7468  ls summed and th
+000184b0: 6520 7265 7375 6c74 2069 7320 6120 6c69  e result is a li
+000184c0: 7374 2077 6974 680a 2020 2020 2020 2020  st with.        
+000184d0: 2020 2020 7468 6520 696e 7465 6e73 6974      the intensit
+000184e0: 7920 6f66 2065 6163 6820 696d 6167 652e  y of each image.
+000184f0: 0a20 2020 2020 2020 2020 2020 2057 6974  .            Wit
+00018500: 6820 4e6f 6e65 2c20 6120 666c 6f61 7420  h None, a float 
+00018510: 6973 2074 6865 2072 6573 756c 7420 6f66  is the result of
+00018520: 2074 6865 2073 756d 206f 6620 616c 6c20   the sum of all 
+00018530: 7468 6520 7069 7865 6c73 2061 6e64 2061  the pixels and a
+00018540: 6c6c 0a20 2020 2020 2020 2020 2020 2074  ll.            t
+00018550: 6865 2069 6d61 6765 732e 0a20 2020 2020  he images..     
+00018560: 2020 203a 7479 7065 2061 7869 733a 2055     :type axis: U
+00018570: 6e69 6f6e 5b4e 6f6e 652c 2069 6e74 5d0a  nion[None, int].
+00018580: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00018590: 3a20 5375 6d6d 6564 2064 6174 610a 2020  : Summed data.  
+000185a0: 2020 2020 2020 3a72 7479 7065 3a20 556e        :rtype: Un
+000185b0: 696f 6e5b 666c 6f61 742c 206c 6973 745d  ion[float, list]
+000185c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000185d0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+000185e0: 2e66 6c61 7474 656e 2829 0a20 2020 2020  .flatten().     
+000185f0: 2020 2069 6620 7365 6c66 2e69 6e5f 6d65     if self.in_me
+00018600: 6d6f 7279 3a0a 2020 2020 2020 2020 2020  mory:.          
+00018610: 2020 6966 2061 7869 7320 3d3d 2030 3a0a    if axis == 0:.
+00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018630: 7265 7475 726e 2073 7570 6572 2844 6174  return super(Dat
+00018640: 612c 2064 6174 6129 2e73 756d 2861 7869  a, data).sum(axi
+00018650: 733d 6178 6973 292e 7669 6577 286e 756d  s=axis).view(num
+00018660: 7079 2e6e 6461 7272 6179 290a 2020 2020  py.ndarray).    
+00018670: 2020 2020 2020 2020 6966 2061 7869 7320          if axis 
+00018680: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00018690: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+000186a0: 6572 2844 6174 612c 2064 6174 6129 2e76  er(Data, data).v
+000186b0: 6965 7728 6e75 6d70 792e 6e64 6172 7261  iew(numpy.ndarra
+000186c0: 7929 2e73 756d 2861 7869 733d 3129 2e73  y).sum(axis=1).s
+000186d0: 756d 2861 7869 733d 3129 0a20 2020 2020  um(axis=1).     
+000186e0: 2020 2020 2020 2069 6620 6178 6973 2069         if axis i
+000186f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00018700: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018710: 7570 6572 2844 6174 612c 2064 6174 6129  uper(Data, data)
+00018720: 2e73 756d 2829 0a20 2020 2020 2020 2020  .sum().         
+00018730: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00018740: 6f72 2822 4178 6973 206d 7573 7420 6265  or("Axis must be
+00018750: 204e 6f6e 652c 2030 206f 7220 3122 290a   None, 0 or 1").
+00018760: 2020 2020 2020 2020 6966 2061 7869 7320          if axis 
+00018770: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00018780: 2020 6966 2064 6174 612e 7369 7a65 203d    if data.size =
+00018790: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000187a0: 2020 2020 2072 6574 7572 6e20 6e75 6d70       return nump
+000187b0: 792e 6172 7261 7928 5b5d 290a 2020 2020  y.array([]).    
+000187c0: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+000187d0: 6174 612e 7368 6170 655b 305d 3a0a 2020  ata.shape[0]:.  
+000187e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000187f0: 7475 726e 206e 756d 7079 2e7a 6572 6f73  turn numpy.zeros
+00018800: 2864 6174 615b 305d 2e73 6861 7065 290a  (data[0].shape).
+00018810: 2020 2020 2020 2020 2020 2020 7a73 756d              zsum
+00018820: 203d 206e 756d 7079 2e61 7272 6179 2864   = numpy.array(d
+00018830: 6174 615b 305d 2c20 6474 7970 653d 6e75  ata[0], dtype=nu
+00018840: 6d70 792e 666c 6f61 7436 3429 0a20 2020  mpy.float64).   
+00018850: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00018860: 6e20 7261 6e67 6528 312c 206c 656e 2864  n range(1, len(d
+00018870: 6174 6129 293a 0a20 2020 2020 2020 2020  ata)):.         
+00018880: 2020 2020 2020 207a 7375 6d20 2b3d 2064         zsum += d
+00018890: 6174 615b 695d 0a20 2020 2020 2020 2020  ata[i].         
+000188a0: 2020 2072 6574 7572 6e20 7a73 756d 0a20     return zsum. 
+000188b0: 2020 2020 2020 2069 6620 6178 6973 203d         if axis =
+000188c0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+000188d0: 2072 6574 7572 6e20 6e75 6d70 792e 6172   return numpy.ar
+000188e0: 7261 7928 5b69 2e73 756d 2829 2066 6f72  ray([i.sum() for
+000188f0: 2069 2069 6e20 6461 7461 5d29 0a20 2020   i in data]).   
+00018900: 2020 2020 2069 6620 6178 6973 2069 7320       if axis is 
+00018910: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00018920: 2020 696d 675f 7375 6d20 3d20 300a 2020    img_sum = 0.  
+00018930: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00018940: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
+00018950: 2020 2020 2020 2020 2069 6d67 5f73 756d           img_sum
+00018960: 202b 3d20 692e 7375 6d28 290a 2020 2020   += i.sum().    
+00018970: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00018980: 6d67 5f73 756d 0a20 2020 2020 2020 2072  mg_sum.        r
+00018990: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+000189a0: 4178 6973 206d 7573 7420 6265 204e 6f6e  Axis must be Non
+000189b0: 652c 2030 206f 7220 3122 290a 0a20 2020  e, 0 or 1")..   
+000189c0: 2064 6566 2074 616b 6528 7365 6c66 2c20   def take(self, 
+000189d0: 696e 6469 6365 732c 2061 7869 733d 4e6f  indices, axis=No
+000189e0: 6e65 2c20 6f75 743d 4e6f 6e65 2c20 6d6f  ne, out=None, mo
+000189f0: 6465 3d22 7261 6973 6522 2920 2d3e 2022  de="raise") -> "
+00018a00: 4461 7461 223a 0a20 2020 2020 2020 2022  Data":.        "
+00018a10: 2222 0a20 2020 2020 2020 2054 616b 6520  "".        Take 
+00018a20: 656c 656d 656e 7473 2066 726f 6d20 7572  elements from ur
+00018a30: 6c73 2061 6e64 206d 6574 6164 6174 6120  ls and metadata 
+00018a40: 6672 6f6d 2061 6e20 6172 7261 7920 616c  from an array al
+00018a50: 6f6e 6720 616e 2061 7869 732e 0a0a 2020  ong an axis...  
+00018a60: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
+00018a70: 6963 6573 3a20 7468 6520 696e 6469 6365  ices: the indice
+00018a80: 7320 6f66 2074 6865 2076 616c 7565 7320  s of the values 
+00018a90: 746f 2065 7874 7261 6374 0a20 2020 2020  to extract.     
+00018aa0: 2020 203a 7479 7065 2069 6e64 6963 6573     :type indices
+00018ab0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+00018ac0: 2020 2020 203a 7061 7261 6d20 6178 6973       :param axis
+00018ad0: 3a20 7468 6520 6178 6973 206f 7665 7220  : the axis over 
+00018ae0: 7768 6963 6820 746f 2073 656c 6563 7420  which to select 
+00018af0: 7661 6c75 6573 2c20 6465 6661 756c 7473  values, defaults
+00018b00: 2074 6f20 4e6f 6e65 0a20 2020 2020 2020   to None.       
+00018b10: 203a 7479 7065 2061 7869 733a 2055 6e69   :type axis: Uni
+00018b20: 6f6e 5b4e 206f 6e65 2c20 696e 745d 2c20  on[N one, int], 
+00018b30: 6f70 7469 6f6e 616c 0a0a 2020 2020 2020  optional..      
+00018b40: 2020 3a72 6574 7572 6e3a 2046 6c61 7474    :return: Flatt
+00018b50: 656e 6564 2064 6174 612e 0a20 2020 2020  ened data..     
+00018b60: 2020 203a 7274 7970 653a 203a 636c 6173     :rtype: :clas
+00018b70: 733a 6044 6174 6160 0a20 2020 2020 2020  s:`Data`.       
+00018b80: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+00018b90: 7320 3d20 6e75 6d70 792e 7461 6b65 2873  s = numpy.take(s
+00018ba0: 656c 662e 7572 6c73 2c20 696e 6469 6365  elf.urls, indice
+00018bb0: 732c 2061 7869 732c 206d 6f64 653d 6d6f  s, axis, mode=mo
+00018bc0: 6465 290a 2020 2020 2020 2020 6d65 7461  de).        meta
+00018bd0: 6461 7461 203d 206e 756d 7079 2e74 616b  data = numpy.tak
+00018be0: 6528 7365 6c66 2e6d 6574 6164 6174 612c  e(self.metadata,
+00018bf0: 2069 6e64 6963 6573 2c20 6178 6973 2c20   indices, axis, 
+00018c00: 6d6f 6465 3d6d 6f64 6529 0a20 2020 2020  mode=mode).     
+00018c10: 2020 2064 6174 6120 3d20 4e6f 6e65 0a20     data = None. 
+00018c20: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00018c30: 6e5f 6d65 6d6f 7279 3a0a 2020 2020 2020  n_memory:.      
+00018c40: 2020 2020 2020 6461 7461 203d 2073 7570        data = sup
+00018c50: 6572 2829 2e74 616b 6528 696e 6469 6365  er().take(indice
+00018c60: 732c 2061 7869 732c 206d 6f64 653d 6d6f  s, axis, mode=mo
+00018c70: 6465 292e 7669 6577 286e 756d 7079 2e6e  de).view(numpy.n
+00018c80: 6461 7272 6179 290a 2020 2020 2020 2020  darray).        
+00018c90: 7265 7475 726e 2044 6174 6128 7572 6c73  return Data(urls
+00018ca0: 2c20 6d65 7461 6461 7461 2c20 7365 6c66  , metadata, self
+00018cb0: 2e69 6e5f 6d65 6d6f 7279 2c20 6461 7461  .in_memory, data
+00018cc0: 3d64 6174 6129 0a0a 2020 2020 6465 6620  =data)..    def 
+00018cd0: 666c 6174 7465 6e28 7365 6c66 2920 2d3e  flatten(self) ->
+00018ce0: 2022 4461 7461 223a 0a20 2020 2020 2020   "Data":.       
+00018cf0: 2022 2222 466c 6174 7465 6e73 2074 6865   """Flattens the
+00018d00: 2073 6361 6e20 6469 6d65 6e73 696f 6e73   scan dimensions
+00018d10: 2c20 6e6f 7420 7468 6520 6672 616d 6520  , not the frame 
+00018d20: 6469 6d65 6e73 696f 6e73 2e0a 2020 2020  dimensions..    
+00018d30: 2020 2020 544f 444f 3a20 7468 6973 2073      TODO: this s
+00018d40: 686f 756c 6420 6765 7420 6120 6469 6666  hould get a diff
+00018d50: 6572 656e 7420 6675 6e63 7469 6f6e 206e  erent function n
+00018d60: 616d 650a 0a20 2020 2020 2020 203a 7265  ame..        :re
+00018d70: 7475 726e 3a20 6e65 7720 6461 7461 2077  turn: new data w
+00018d80: 6974 6820 666c 6174 7465 6e65 6420 7572  ith flattened ur
+00018d90: 6c73 2061 6e64 206d 6574 6164 6174 6120  ls and metadata 
+00018da0: 2862 7574 206e 6f74 2066 7261 6d65 7329  (but not frames)
+00018db0: 2e0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00018dc0: 3a20 3a63 6c61 7373 3a60 4461 7461 600a  : :class:`Data`.
+00018dd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00018de0: 2020 2020 6966 2073 656c 662e 6e66 7261      if self.nfra
+00018df0: 6d65 7320 3d3d 2030 206f 7220 7365 6c66  mes == 0 or self
+00018e00: 2e6e 6469 6d20 3c3d 2033 3a0a 2020 2020  .ndim <= 3:.    
+00018e10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018e20: 656c 660a 2020 2020 2020 2020 6461 7461  elf.        data
+00018e30: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00018e40: 6966 2073 656c 662e 696e 5f6d 656d 6f72  if self.in_memor
+00018e50: 793a 0a20 2020 2020 2020 2020 2020 2066  y:.            f
+00018e60: 7368 6170 6520 3d20 2873 656c 662e 6e66  shape = (self.nf
+00018e70: 7261 6d65 732c 2920 2b20 7365 6c66 2e66  rames,) + self.f
+00018e80: 7261 6d65 5f73 6861 7065 0a20 2020 2020  rame_shape.     
+00018e90: 2020 2020 2020 2023 2054 4f44 4f3a 206e         # TODO: n
+00018ea0: 6f74 2073 7572 6520 7768 7920 7765 206e  ot sure why we n
+00018eb0: 6565 6420 7468 6520 7665 7720 6865 7265  eed the vew here
+00018ec0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+00018ed0: 7461 203d 2073 7570 6572 2829 2e72 6573  ta = super().res
+00018ee0: 6861 7065 2866 7368 6170 6529 2e76 6965  hape(fshape).vie
+00018ef0: 7728 6e75 6d70 792e 6e64 6172 7261 7929  w(numpy.ndarray)
+00018f00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018f10: 4461 7461 280a 2020 2020 2020 2020 2020  Data(.          
+00018f20: 2020 7365 6c66 2e75 726c 732e 666c 6174    self.urls.flat
+00018f30: 7465 6e28 292c 2073 656c 662e 6d65 7461  ten(), self.meta
+00018f40: 6461 7461 2e66 6c61 7474 656e 2829 2c20  data.flatten(), 
+00018f50: 7365 6c66 2e69 6e5f 6d65 6d6f 7279 2c20  self.in_memory, 
+00018f60: 6461 7461 3d64 6174 610a 2020 2020 2020  data=data.      
+00018f70: 2020 290a 0a0a 636c 6173 7320 5472 616e    )...class Tran
+00018f80: 7366 6f72 6d61 7469 6f6e 3a0a 2020 2020  sformation:.    
+00018f90: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00018fa0: 662c 206b 696e 643a 2073 7472 2c20 783a  f, kind: str, x:
+00018fb0: 206e 756d 7079 2e6e 6461 7272 6179 2c20   numpy.ndarray, 
+00018fc0: 793a 206e 756d 7079 2e6e 6461 7272 6179  y: numpy.ndarray
+00018fd0: 2c20 726f 7461 7465 3a20 626f 6f6c 293a  , rotate: bool):
+00018fe0: 0a20 2020 2020 2020 2073 656c 662e 7820  .        self.x 
+00018ff0: 3d20 7820 2023 2073 6861 7065 2028 7379  = x  # shape (sy
+00019000: 2c20 7378 290a 2020 2020 2020 2020 7365  , sx).        se
+00019010: 6c66 2e79 203d 2079 2020 2320 7368 6170  lf.y = y  # shap
+00019020: 6520 2873 792c 2073 7829 0a20 2020 2020  e (sy, sx).     
+00019030: 2020 2073 656c 662e 726f 7461 7465 203d     self.rotate =
+00019040: 2072 6f74 6174 650a 2020 2020 2020 2020   rotate.        
+00019050: 7365 6c66 2e6b 696e 6420 3d20 6b69 6e64  self.kind = kind
+00019060: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00019070: 2020 2020 6465 6620 7368 6170 6528 7365      def shape(se
+00019080: 6c66 2920 2d3e 2054 7570 6c65 5b69 6e74  lf) -> Tuple[int
+00019090: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+000190a0: 7265 7475 726e 2073 656c 662e 782e 7368  return self.x.sh
+000190b0: 6170 650a 0a20 2020 2040 7072 6f70 6572  ape..    @proper
+000190c0: 7479 0a20 2020 2064 6566 2073 7828 7365  ty.    def sx(se
+000190d0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+000190e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000190f0: 7368 6170 655b 315d 0a0a 2020 2020 4070  shape[1]..    @p
+00019100: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00019110: 7379 2873 656c 6629 202d 3e20 696e 743a  sy(self) -> int:
+00019120: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019130: 7365 6c66 2e73 6861 7065 5b30 5d0a 0a20  self.shape[0].. 
+00019140: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00019150: 2064 6566 206c 6162 656c 2873 656c 6629   def label(self)
+00019160: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00019170: 2072 6574 7572 6e20 2264 6567 7265 6573   return "degrees
+00019180: 2220 6966 2073 656c 662e 6b69 6e64 203d  " if self.kind =
+00019190: 3d20 2272 736d 2220 656c 7365 2022 c2b5  = "rsm" else "..
+000191a0: 6d22 0a0a 2020 2020 4070 726f 7065 7274  m"..    @propert
+000191b0: 790a 2020 2020 6465 6620 7872 6567 756c  y.    def xregul
+000191c0: 6172 2873 656c 6629 202d 3e20 6e75 6d70  ar(self) -> nump
+000191d0: 792e 6e64 6172 7261 793a 0a20 2020 2020  y.ndarray:.     
+000191e0: 2020 2072 6574 7572 6e20 7365 6c66 2e78     return self.x
+000191f0: 7363 616c 6520 2a20 6e75 6d70 792e 6172  scale * numpy.ar
+00019200: 616e 6765 2873 656c 662e 7378 2920 2b20  ange(self.sx) + 
+00019210: 7365 6c66 2e78 6f72 6967 696e 0a0a 2020  self.xorigin..  
+00019220: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00019230: 6465 6620 7972 6567 756c 6172 2873 656c  def yregular(sel
+00019240: 6629 202d 3e20 6e75 6d70 792e 6e64 6172  f) -> numpy.ndar
+00019250: 7261 793a 0a20 2020 2020 2020 2072 6574  ray:.        ret
+00019260: 7572 6e20 7365 6c66 2e79 7363 616c 6520  urn self.yscale 
+00019270: 2a20 6e75 6d70 792e 6172 616e 6765 2873  * numpy.arange(s
+00019280: 656c 662e 7379 2920 2b20 7365 6c66 2e79  elf.sy) + self.y
+00019290: 6f72 6967 696e 0a0a 2020 2020 4070 726f  origin..    @pro
+000192a0: 7065 7274 790a 2020 2020 6465 6620 786f  perty.    def xo
+000192b0: 7269 6769 6e28 7365 6c66 2920 2d3e 204e  rigin(self) -> N
+000192c0: 756d 6265 723a 0a20 2020 2020 2020 2072  umber:.        r
+000192d0: 6574 7572 6e20 7365 6c66 2e78 5b30 5d5b  eturn self.x[0][
+000192e0: 305d 0a0a 2020 2020 4070 726f 7065 7274  0]..    @propert
+000192f0: 790a 2020 2020 6465 6620 796f 7269 6769  y.    def yorigi
+00019300: 6e28 7365 6c66 2920 2d3e 204e 756d 6265  n(self) -> Numbe
+00019310: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+00019320: 6e20 7365 6c66 2e79 5b30 5d5b 305d 0a0a  n self.y[0][0]..
+00019330: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00019340: 2020 6465 6620 6f72 6967 696e 2873 656c    def origin(sel
+00019350: 6629 202d 3e20 5475 706c 655b 4e75 6d62  f) -> Tuple[Numb
+00019360: 6572 2c20 4e75 6d62 6572 5d3a 0a20 2020  er, Number]:.   
+00019370: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00019380: 2e78 6f72 6967 696e 2c20 7365 6c66 2e79  .xorigin, self.y
+00019390: 6f72 6967 696e 0a0a 2020 2020 4070 726f  origin..    @pro
+000193a0: 7065 7274 790a 2020 2020 6465 6620 7873  perty.    def xs
+000193b0: 6361 6c65 2873 656c 6629 202d 3e20 4e75  cale(self) -> Nu
+000193c0: 6d62 6572 3a0a 2020 2020 2020 2020 7820  mber:.        x 
+000193d0: 3d20 7365 6c66 2e78 0a20 2020 2020 2020  = self.x.       
+000193e0: 2072 6574 7572 6e20 2878 5b2d 315d 5b2d   return (x[-1][-
+000193f0: 315d 202d 2078 5b30 5d5b 305d 2920 2f20  1] - x[0][0]) / 
+00019400: 7365 6c66 2e73 780a 0a20 2020 2040 7072  self.sx..    @pr
+00019410: 6f70 6572 7479 0a20 2020 2064 6566 2079  operty.    def y
+00019420: 7363 616c 6528 7365 6c66 2920 2d3e 204e  scale(self) -> N
+00019430: 756d 6265 723a 0a20 2020 2020 2020 2079  umber:.        y
+00019440: 203d 2073 656c 662e 790a 2020 2020 2020   = self.y.      
+00019450: 2020 7265 7475 726e 2028 795b 2d31 5d5b    return (y[-1][
+00019460: 2d31 5d20 2d20 795b 305d 5b30 5d29 202f  -1] - y[0][0]) /
+00019470: 2073 656c 662e 7379 0a0a 2020 2020 4070   self.sy..    @p
+00019480: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00019490: 7363 616c 6528 7365 6c66 2920 2d3e 2054  scale(self) -> T
+000194a0: 7570 6c65 5b4e 756d 6265 722c 204e 756d  uple[Number, Num
+000194b0: 6265 725d 3a0a 2020 2020 2020 2020 7265  ber]:.        re
+000194c0: 7475 726e 2073 656c 662e 7873 6361 6c65  turn self.xscale
+000194d0: 2c20 7365 6c66 2e79 7363 616c 650a 0a0a  , self.yscale...
+000194e0: 636c 6173 7320 5f48 4446 354d 6574 6164  class _HDF5Metad
+000194f0: 6174 6152 6561 6465 723a 0a20 2020 2022  ataReader:.    "
+00019500: 2222 0a20 2020 2045 7175 6976 616c 656e  "".    Equivalen
+00019510: 7420 6f66 2073 696c 782e 696f 2e66 6162  t of silx.io.fab
+00019520: 696f 6835 2e46 6162 696f 5265 6164 6572  ioh5.FabioReader
+00019530: 2074 6f20 6769 7665 2061 6363 6573 7320   to give access 
+00019540: 746f 2048 4446 3520 6d65 7461 6461 7461  to HDF5 metadata
+00019550: 0a0a 2020 2020 4649 584d 453a 2072 656d  ..    FIXME: rem
+00019560: 6f76 6520 7468 6973 2063 6c61 7373 2e20  ove this class. 
+00019570: 5374 6f72 6167 6520 616e 6420 7265 6164  Storage and read
+00019580: 696e 6720 6f66 206d 6574 6164 6174 6120  ing of metadata 
+00019590: 6861 7320 6265 656e 2062 6173 6564 206f  has been based o
+000195a0: 6e20 4544 462e 2054 6869 7320 636c 6173  n EDF. This clas
+000195b0: 7320 6973 2061 2077 6f72 6b2d 6172 6f75  s is a work-arou
+000195c0: 6e64 0a20 2020 2044 6573 6967 6e20 6f66  nd.    Design of
+000195d0: 2068 616e 646c 6520 6d65 7461 6461 7461   handle metadata
+000195e0: 2073 686f 756c 646e 2774 2062 6520 6261   shouldn't be ba
+000195f0: 7365 6420 6f6e 2074 6865 2064 6174 6120  sed on the data 
+00019600: 7479 7065 2062 7574 206d 6f72 6520 6162  type but more ab
+00019610: 7374 7261 6374 6564 0a20 2020 2022 2222  stracted.    """
+00019620: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00019630: 5f5f 2873 656c 662c 206d 6574 6164 6174  __(self, metadat
+00019640: 613a 2064 6963 7429 202d 3e20 4e6f 6e65  a: dict) -> None
+00019650: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00019660: 5f6d 6574 6164 6174 6120 3d20 6d65 7461  _metadata = meta
+00019670: 6461 7461 0a0a 2020 2020 6465 6620 6765  data..    def ge
+00019680: 745f 7661 6c75 6528 7365 6c66 2c20 6b69  t_value(self, ki
+00019690: 6e64 2c20 6e61 6d65 293a 0a20 2020 2020  nd, name):.     
+000196a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000196b0: 5f6d 6574 6164 6174 612e 6765 7428 6e61  _metadata.get(na
+000196c0: 6d65 2c20 4e6f 6e65 290a 0a20 2020 2064  me, None)..    d
+000196d0: 6566 2067 6574 5f6b 6579 7328 7365 6c66  ef get_keys(self
+000196e0: 2c20 6b69 6e64 293a 0a20 2020 2020 2020  , kind):.       
+000196f0: 2072 6574 7572 6e20 7475 706c 6528 7365   return tuple(se
+00019700: 6c66 2e5f 5f6d 6574 6164 6174 612e 6b65  lf.__metadata.ke
+00019710: 7973 2829 290a                           ys()).
```

### Comparing `darfix-1.0.1rc0/src/darfix/core/dimension.py` & `darfix-1.0.1rc1/src/darfix/core/dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                     )
                 else:
                     step = (v1 - v0) / (self.size - 1)
                     self.__unique_values = [
                         s for s in numpy.linspace(v0, v1, self.size)
                     ]
             else:
-                size = int(numpy.round((v1 - v0) / step)) + 1
+                size = int(numpy.round((v1 - v0) / step, 5)) + 1
                 self.__unique_values = [s for s in numpy.linspace(v0, v1, size)]
             self.set_range([v0, v1, step])
         elif self.size:
             self.__unique_values = self._values_with_step(values[: self.size])
         else:
             self.__unique_values = self._values_with_step(
                 self._find_unique_values(values)
```

### Comparing `darfix-1.0.1rc0/src/darfix/core/geneticShiftDetection.py` & `darfix-1.0.1rc1/src/darfix/core/geneticShiftDetection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/imageOperations.py` & `darfix-1.0.1rc1/src/darfix/core/imageOperations.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/imageRegistration.py` & `darfix-1.0.1rc1/src/darfix/core/imageRegistration.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/mapping.py` & `darfix-1.0.1rc1/src/darfix/core/mapping.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/process.py` & `darfix-1.0.1rc1/src/darfix/core/process.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/roi.py` & `darfix-1.0.1rc1/src/darfix/core/roi.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_components_matching.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_components_matching.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_data_selection.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_dataset.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import copy
 import unittest
 import numpy
 import tempfile
 import shutil
 import uuid
+import pytest
 
 from silx.io.url import DataUrl
 
 from darfix.test import utils
 from darfix.core.dataset import Data
 
 
@@ -856,9 +857,18 @@
         for i in range(4):
             numpy.testing.assert_array_equal(data.flatten()[i], self.data[i])
 
     def tearDown(self):
         shutil.rmtree(self._dir)
 
 
+@pytest.mark.parametrize("in_memory", (True, False), ids=["in_memory", "on_disk"])
+def test_empty_data(in_memory):
+    data = Data([], [], in_memory=in_memory)
+    assert data.size == 0
+    assert data.ndim == 3
+    assert data.shape == (0, 0, 0)
+    assert data.copy().tolist() == []
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_dimension.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_ga.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_ga.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_image_operations.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_image_operations.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_image_registration.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_image_registration.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_mapping.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_mapping.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_roi.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_roi.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/test/test_workflow.py` & `darfix-1.0.1rc1/src/darfix/core/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/core/utils.py` & `darfix-1.0.1rc1/src/darfix/core/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/base.py` & `darfix-1.0.1rc1/src/darfix/decomposition/base.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/ipca.py` & `darfix-1.0.1rc1/src/darfix/decomposition/ipca.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/nica.py` & `darfix-1.0.1rc1/src/darfix/decomposition/nica.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/nmf.py` & `darfix-1.0.1rc1/src/darfix/decomposition/nmf.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/pca.py` & `darfix-1.0.1rc1/src/darfix/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/test/test_base.py` & `darfix-1.0.1rc1/src/darfix/decomposition/test/test_base.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/test/test_ipca.py` & `darfix-1.0.1rc1/src/darfix/decomposition/test/test_ipca.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/test/test_nica.py` & `darfix-1.0.1rc1/src/darfix/decomposition/test/test_nica.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/test/test_nmf.py` & `darfix-1.0.1rc1/src/darfix/decomposition/test/test_nmf.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/decomposition/test/utils.py` & `darfix-1.0.1rc1/src/darfix/decomposition/test/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/dtypes.py` & `darfix-1.0.1rc1/src/darfix/dtypes.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/PCAWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/PCAWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/binningWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/binningWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/blindSourceSeparationWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/blindSourceSeparationWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/dataPartitionWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/dataPartitionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/datasetSelectionWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/datasetSelectionWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,16 @@
 
     def addFile(self, file):
         """
         Adds a file to the table.
 
         :param str file: filepath to add to the table.
         """
-        assert os.path.isfile(file)
+        if not os.path.isfile(file):
+            raise FileNotFoundError(file)
         item = qt.QTableWidgetItem()
         item.setText(file)
         row = self._table.rowCount()
         self._table.setRowCount(row + 1)
         self._table.setItem(row, 0, item)
         self._files.append(file)
 
@@ -381,15 +382,15 @@
     filenameChanged = qt.Signal()
 
     def __init__(self, parent=None):
         qt.QWidget.__init__(self, parent)
         self._isH5 = False
         self._filename = None
         self._filenameLE = qt.QLineEdit("", parent=self)
-        self._addButton = qt.QPushButton("Upload file", parent=self)
+        self._addButton = qt.QPushButton("Upload data", parent=self)
         # self._okButton =  qt.QPushButton("Ok", parent=self)
         self._addButton.pressed.connect(self._uploadFilename)
         # self._okButton.pressed.connect(self.close)
         self.setLayout(qt.QHBoxLayout())
 
         self.layout().addWidget(self._filenameLE)
         self.layout().addWidget(self._addButton)
```

### Comparing `darfix-1.0.1rc0/src/darfix/gui/dimensionsWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/dimensionsWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,23 +576,17 @@
 
     def remove(self):
         self.removed.emit(self)
 
     def showUniqueNames(self):
         title = "%s - %s" % (_METADATA_TYPES_I[self.kind], self.name)
         if len(self.unique_values):
-            ptp = float(self.unique_values[-1]) - float(self.unique_values[0])
-            unique_values_str = []
-            [unique_values_str.append(str(val)) for val in self.unique_values]
-            msg = (
-                "Unique values: ["
-                + ", ".join(unique_values_str)
-                + "]\n Ptp: "
-                + str(ptp)
-            )
+            total_range = float(self.unique_values[-1]) - float(self.unique_values[0])
+            unique_values = ", ".join([str(val) for val in self.unique_values])
+            msg = f"Unique values: [{unique_values}]\nTotal range: {total_range}"
             qt.QMessageBox.information(self, title, msg)
         else:
             qt.QMessageBox.information(self, title, "No values were found, try fitting")
 
     def setUniqueValues(self, values):
         super().set_unique_values(values)
         if values is None:
```

### Comparing `darfix-1.0.1rc0/src/darfix/gui/displayComponentsWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/displayComponentsWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/grainPlotWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/grainPlotWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/lineProfileWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/lineProfileWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/linkComponentsWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/linkComponentsWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/magnificationWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/magnificationWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/metadataWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/metadataWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,32 +67,31 @@
         self._table.clear()
         # v_header = [str(i) for i in range(self.__experiment.nslices)]
         metadata = self._dataset.get_data().metadata
         self._table.setRowCount(len(metadata))
         # self._table.setVerticalHeaderLabels(v_header)
 
         columnCount = None
-        if not self._dataset._isH5:
-            for row, metadata_frame in enumerate(metadata):
-                keys = metadata_frame.get_keys(kind=metadata_type)
-                if not row:
-                    if columnCount is None:
-                        self._table.setColumnCount(len(keys))
-                        self._table.setHorizontalHeaderLabels(keys)
-                    elif columnCount != len(metadata_frame):
-                        raise ValueError("Metadata keys are incoherent")
+        for row, metadata_frame in enumerate(metadata):
+            keys = metadata_frame.get_keys(kind=metadata_type)
+            if not row:
+                if columnCount is None:
+                    self._table.setColumnCount(len(keys))
+                    self._table.setHorizontalHeaderLabels(keys)
+                elif columnCount != len(metadata_frame):
+                    raise ValueError("Metadata keys are incoherent")
 
-                for column, key in enumerate(keys):
-                    _item = qt.QTableWidgetItem()
-                    try:
-                        txt = metadata_frame.get_value(kind=metadata_type, name=key)
-                    except KeyError:
-                        txt = "0"
-                    if type(txt) is numpy.ndarray and txt.size == 1:
-                        txt = txt[0]
-                    if hasattr(txt, "decode"):
-                        txt = txt.decode("utf-8")
-                    else:
-                        txt = str(txt)
-                    _item.setText(txt)
-                    _item.setFlags(qt.Qt.ItemIsEnabled | qt.Qt.ItemIsSelectable)
-                    self._table.setItem(row, column, _item)
+            for column, key in enumerate(keys):
+                _item = qt.QTableWidgetItem()
+                try:
+                    txt = metadata_frame.get_value(kind=metadata_type, name=key)
+                except KeyError:
+                    txt = "0"
+                if type(txt) is numpy.ndarray and txt.size == 1:
+                    txt = txt[0]
+                if hasattr(txt, "decode"):
+                    txt = txt.decode("utf-8")
+                else:
+                    txt = str(txt)
+                _item.setText(txt)
+                _item.setFlags(qt.Qt.ItemIsEnabled | qt.Qt.ItemIsSelectable)
+                self._table.setItem(row, column, _item)
```

### Comparing `darfix-1.0.1rc0/src/darfix/gui/noiseRemovalWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/noiseRemovalWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self.computeBS = qt.QPushButton("Compute")
         self.abortBS = qt.QPushButton("Abort")
         self.abortBS.hide()
         methodLabel = qt.QLabel("Method:")
         bgLabel = qt.QLabel("Background:")
         methodLabel.setMargin(0)
         # Step widget
+        # note: step wodget, ChunksWidget and ondist will be displayed if the dataset
+        # has been loaded with the `on disk` option in "DataSelectionWidgetOW"
         self.stepWidget = qt.QWidget()
         stepLayout = qt.QHBoxLayout()
         stepLayout.addWidget(qt.QLabel("Step:"))
         self.step = qt.QLineEdit("1")
         self.step.setSizePolicy(qt.QSizePolicy.Ignored, qt.QSizePolicy.Preferred)
         stepLayout.setContentsMargins(0, 0, 0, 0)
         stepLayout.addWidget(self.step)
```

### Comparing `darfix-1.0.1rc0/src/darfix/gui/operationThread.py` & `darfix-1.0.1rc1/src/darfix/gui/operationThread.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/projectionWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/projectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/rockingCurvesWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/rockingCurvesWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/roiLimitsToolbar.py` & `darfix-1.0.1rc1/src/darfix/gui/roiLimitsToolbar.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/roiSelectionWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/roiSelectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/rsmHistogramWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/rsmHistogramWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/rsmWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/rsmWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/shiftCorrectionWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/shiftCorrectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/showStackWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/showStackWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/utils.py` & `darfix-1.0.1rc1/src/darfix/gui/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/weakBeamWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/weakBeamWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/gui/zSumWidget.py` & `darfix-1.0.1rc1/src/darfix/gui/zSumWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/io/dataset_io.py` & `darfix-1.0.1rc1/src/darfix/io/dataset_io.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/io/utils.py` & `darfix-1.0.1rc1/src/darfix/io/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/curves.png` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/curves.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/curves.svg` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/curves.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/resize.png` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/resize.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/resize.svg` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/resize.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/scatter.png` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/scatter.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/resources/gui/icons/scatter.svg` & `darfix-1.0.1rc1/src/darfix/resources/gui/icons/scatter.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix/test/utils.py` & `darfix-1.0.1rc1/src/darfix/test/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/darfix.egg-info/PKG-INFO` & `darfix-1.0.1rc1/src/darfix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darfix
-Version: 1.0.1rc0
+Version: 1.0.1rc1
 Summary: Computer vision software for the interpretation of diffraction images
 Home-page: https://gitlab.esrf.fr/XRD/darfix
 Author: J.Garriga
 Author-email: julia.garriga@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/XRD/darfix/
 Project-URL: Documentation, http://www.edna-site.org/pub/doc/darfix/latest
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: silx<2.0.0,>=1.1.2
+Requires-Dist: matplotlib<3.9
 Requires-Dist: ewoks>=0.1.0
 Requires-Dist: ewokscore>=0.1.1
 Requires-Dist: chardet<5.0.0; python_version < "3.7"
 Requires-Dist: packaging
 Provides-Extra: full
 Requires-Dist: matplotlib>=1.2.0; extra == "full"
 Requires-Dist: opencv-python-headless<4.7,>=4.3.0.36; extra == "full"
```

### Comparing `darfix-1.0.1rc0/src/darfix.egg-info/SOURCES.txt` & `darfix-1.0.1rc1/src/darfix.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 src/darfix/resources/gui/icons/curves.png
 src/darfix/resources/gui/icons/curves.svg
 src/darfix/resources/gui/icons/resize.png
 src/darfix/resources/gui/icons/resize.svg
 src/darfix/resources/gui/icons/scatter.png
 src/darfix/resources/gui/icons/scatter.svg
 src/darfix/test/__init__.py
+src/darfix/test/conftest.py
 src/darfix/test/utils.py
 src/orangecontrib/darfix/__init__.py
 src/orangecontrib/darfix/test/__init__.py
 src/orangecontrib/darfix/test/test_ewoks.py
 src/orangecontrib/darfix/tutorials/__init__.py
 src/orangecontrib/darfix/tutorials/darfix_example1.ows
 src/orangecontrib/darfix/tutorials/darfix_example2.ows
@@ -159,8 +160,9 @@
 src/orangecontrib/darfix/widgets/icons/resize.png
 src/orangecontrib/darfix/widgets/icons/roi.png
 src/orangecontrib/darfix/widgets/icons/roi.svg
 src/orangecontrib/darfix/widgets/icons/save.svg
 src/orangecontrib/darfix/widgets/icons/shift_correction.svg
 src/orangecontrib/darfix/widgets/icons/upload.svg
 src/orangecontrib/darfix/widgets/icons/zsum.svg
-src/orangecontrib/darfix/widgets/test/test_data_selection.py
+src/orangecontrib/darfix/widgets/test/test_data_selection.py
+src/snippets/convert_edf_to_hdf5.py
```

### Comparing `darfix-1.0.1rc0/src/darfix.egg-info/requires.txt` & `darfix-1.0.1rc1/src/darfix.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 numpy
 silx<2.0.0,>=1.1.2
+matplotlib<3.9
 ewoks>=0.1.0
 ewokscore>=0.1.1
 packaging
 
 [:python_version < "3.7"]
 chardet<5.0.0
```

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/test/test_ewoks.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/test/test_ewoks.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/darfix_example1.ows` & `darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/darfix_example1.ows`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/darfix_example2.ows` & `darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/darfix_example2.ows`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/strain_0000.edf` & `darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/strain_0000.edf`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/tutorials/strain_0001.edf` & `darfix-1.0.1rc1/src/orangecontrib/darfix/tutorials/strain_0001.edf`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/__init__.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/binning.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/binning.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/blindsourceseparation.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/blindsourceseparation.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/datacopy.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/datacopy.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/datapartition.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/datapartition.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/dataselection.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/dataselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,18 @@
 
         self.controlArea.layout().addWidget(self._widget)
         self.controlArea.layout().addWidget(_buttons)
 
         _buttons.accepted.connect(self._getDataset)
 
         self.__updatingData = False
-        self.setDataset()
+        try:
+            self.setDataset()
+        except Exception as e:
+            _logger.exception(str(e))
 
     def setDataset(self):
         self._widget.setRawFilenames(self.filenames)
         self._widget.setRawFilename(self.raw_filename)
         self._widget.setDarkFilename(self.dark_filename)
         if self.on_disk:
             self._widget._onDiskCB.setChecked(True)
```

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/dimensions.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/dimensions.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/flash.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/flash.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/grainplot.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/grainplot.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/axes.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/axes.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/axes.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/axes.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/bss.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/bss.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/bss.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/bss.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/copy.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/copy.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/curves.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/curves.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/curves.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/curves.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/filter.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/filter.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/filter.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/flash.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/flash.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/gaussian.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/gaussian.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/gaussian.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/gaussian.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/grainplot.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/grainplot.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/grainplot.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/grainplot.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/image-select-box.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/image-select-box.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/line_profile.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/line_profile.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/line_profile.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/line_profile.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/link.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/link.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/link.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/link.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/metadata.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/metadata.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/metadata.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/metadata.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/mywidget.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/param_dims.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/param_dims.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/param_dims.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/param_dims.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/pca.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/pca.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/pca.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/pca.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/random.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/random.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/resize.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/resize.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/roi.png` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/roi.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/roi.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/save.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/save.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/shift_correction.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/shift_correction.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/upload.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/upload.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/icons/zsum.svg` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/icons/zsum.svg`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/lineprofile.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/lineprofile.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/linkcomponents.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/linkcomponents.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/metadata.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/metadata.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/noiseremoval.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/noiseremoval.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/pca.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/pca.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/projection.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/projection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/rockingcurves.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/rockingcurves.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/roiselection.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/roiselection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/rsmhistogram.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/rsmhistogram.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/shiftcorrection.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/shiftcorrection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/test/test_data_selection.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/test/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/transformation.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/transformation.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/weakbeam.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/weakbeam.py`

 * *Files identical despite different names*

### Comparing `darfix-1.0.1rc0/src/orangecontrib/darfix/widgets/zsum.py` & `darfix-1.0.1rc1/src/orangecontrib/darfix/widgets/zsum.py`

 * *Files identical despite different names*

