# Comparing `tmp/gnssrefl-3.1.4.tar.gz` & `tmp/gnssrefl-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-3.1.4.tar", last modified: Fri Mar 22 16:52:55 2024, max compression
+gzip compressed data, was "gnssrefl-3.1.5.tar", last modified: Mon Apr 15 18:28:21 2024, max compression
```

## Comparing `gnssrefl-3.1.4.tar` & `gnssrefl-3.1.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:52:55.054345 gnssrefl-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-22 16:52:55.054345 gnssrefl-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:52:55.026345 gnssrefl-3.1.4/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24097 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:52:55.030345 gnssrefl-3.1.4/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/filesizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18742 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnssir_cl_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41964 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (127)   196720 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    24691 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/make_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/max_resolve_RH_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/mjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18749 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57200 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25784 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinex_coords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/sd_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    61061 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:52:55.026345 gnssrefl-3.1.4/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 16:52:54.000000 gnssrefl-3.1.4/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 16:52:55.054345 gnssrefl-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:52:55.054345 gnssrefl-3.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-22 16:52:47.000000 gnssrefl-3.1.4/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.756948 gnssrefl-3.1.5/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.760948 gnssrefl-3.1.5/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/filesizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_cl_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41964 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50903 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)    50899 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (127)   199207 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40525 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21773344 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/make_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/max_resolve_RH_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/mjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34201 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51554 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18818 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5978 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19877 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57267 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinex_coords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24490 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38571 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/sd_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61061 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32950 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.760948 gnssrefl-3.1.5/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 18:28:21.000000 gnssrefl-3.1.5/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.784948 gnssrefl-3.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 18:28:13.000000 gnssrefl-3.1.5/test/test_rinex2snr.py
```

### Comparing `gnssrefl-3.1.4/LICENSE` & `gnssrefl-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/PKG-INFO` & `gnssrefl-3.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.1.4
+Version: 3.1.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.1.4 
+# gnssrefl v3.1.5 
+
+If you use this code in any presentation or publication, you are expected to cite either 
+this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
 
 
 gnssrefl is an open source software package for GNSS interferometric reflectometry (GNSS-IR). 
 
 ![](docs/myAnimation.gif)
 
+I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
+a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
+and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
```

### Comparing `gnssrefl-3.1.4/README.md` & `gnssrefl-3.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-# gnssrefl v3.1.4 
+# gnssrefl v3.1.5 
+
+If you use this code in any presentation or publication, you are expected to cite either 
+this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
 
 
 gnssrefl is an open source software package for GNSS interferometric reflectometry (GNSS-IR). 
 
 ![](docs/myAnimation.gif)
 
+I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
+a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
+and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
```

### Comparing `gnssrefl-3.1.4/gnssrefl/EGM96.py` & `gnssrefl-3.1.5/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/check_rinex_file.py` & `gnssrefl-3.1.5/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/computemp1mp2.py` & `gnssrefl-3.1.5/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/daily_avg.py` & `gnssrefl-3.1.5/gnssrefl/daily_avg.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,21 +183,25 @@
     allrh.write(" {0:s}  \n".format('% (1), (2),(3), (4),(5),  (6), (7), (8), (9),  (10), (11)' ))
 
     fs = 12
     NotEnough = 0
     tv = np.empty(shape=[0, 8])
     tv_median = np.empty(shape=[0, 9])
     tvall = np.empty(shape=[0, 7])
+    tv_list = []
+    tv_median_list = []
     #
     ngps = []; nglo = [] ; ngal = []; nbei = []
     obstimes = []; medRH = []; meanRH = [] ; alltimes = []; meanAmp = []
     tttimes = []
     fig,ax=plt.subplots()
     year_list = np.arange(year1, year2+1, 1)
     NumFiles = 0
+    test_alltimes = []
+    test_good = []
     s1 = time.time()
     for yr in year_list:
         direc = xdir + '/' + str(yr) + '/results/' + station + '/' + extension + '/'
         # counter for the legends
         nle = 0
         # i understand why python people like this - but then the results are not sorted ...
         if os.path.isdir(direc):
@@ -265,14 +269,19 @@
                                 #filler = datetime.datetime(year=yr, month=d.month, day=d.day, hour = hrr, minute=mm, second = ss)
                                 for w in range(0,len(good)):
                                     hrr = int(np.floor(gutcTime[w])) # 
                                     mm = int(60*(gutcTime[w] - hrr )); ss = 0
                                     filler = datetime.datetime(year=yr, month=d.month, day=d.day, hour = hrr, minute=mm, second = ss)
                                     alltimes.append(filler)
                                 # 
+                                # this probably should not be inside the loop
+                                # maybe this makes it slow? will try accumulating it all and plot outside the loop
+                                #test_alltimes.append(alltimes)
+                                #test_good.append(good)
+
                                 ax.plot(alltimes,good,'b.')
 
                                 # this are stats for the daily averages - is this slowing it down? - apparently not
                                 # turned off for now
                                 if True:
                                     ijk = (gsat  < 100); 
                                     ngps = np.append(ngps, len(gsat[ijk]))
@@ -301,39 +310,50 @@
                                 #meanAmp = np.append(meanAmp, np.mean(goodAmp))
                                 # updated this to include mean amplitude 2021 november 8
                                 meanAmp.append(np.mean(goodAmp))
                                 newl = [yr, doy, meanRHtoday, len(rh), d.month, d.day, stdRHtoday, np.mean(goodAmp)]
                                 # a new variable is not really needed - but I did not want to oerwrite working code
                                 newl_plus_median = [yr, doy, meanRHtoday, len(rh), d.month, d.day, stdRHtoday, np.mean(goodAmp),medv]
 
-                                tv = np.append(tv, [newl],axis=0)
-                                tv_median = np.append(tv_median, [newl_plus_median],axis=0)
+                                # maybe this is slow??
+                                #tv = np.append(tv, [newl],axis=0)
+                                #tv_median = np.append(tv_median, [newl_plus_median],axis=0)
+                                # see if this works
+                                tv_list.append(newl)
+                                tv_median_list.append(newl_plus_median)
 
                                 k += 1
                             else:
                                 NotEnough = NotEnough + 1
                     except:
                         okok = 1;
+            #ax.plot(test_alltimes,test_good,'b.')
         else:
             abc = 0; # dummy line
     #meanRH = np.asarray(meanRH)
+
     s2 = time.time()
+    #print(s2-s1, ' seconds')
+    tv = np.asarray(tv_list)
+    tv_median = np.asarray(tv_median_list)
 
     # not sure you can sort obstimes
     dumb_time = tv_median[:,0] + tv_median[:,1]/365.25
     # sort it ...
     ii = np.argsort(dumb_time)
     tv_median = tv_median[ii,:]
+    # i have a function for this now - though it asks for MJD
     for www in range(0,len(tv_median)):
         filler = datetime.datetime(year=int(tv_median[www,0]), 
                 month=int(tv_median[www,4]), day=int(tv_median[www,5]), hour = 12, minute=0, second = 0)
         tttimes.append(filler)
 
     # plot the median 
-    ax.plot(tttimes, tv_median[:,8],'ks',markerfacecolor='white',label='median value')
+    #ax.plot(tttimes, tv_median[:,8],'k.',label='median value')
+    ax.plot(tttimes, tv_median[:,8],'ks',markerfacecolor='white',label='median value',markersize=4)
     # if requested, also show the limits for the median filter
     if plot_limits:
         ax.plot(tttimes, tv_median[:,8]+howBig,'-',color='gray',label='median+limit')
         ax.plot(tttimes, tv_median[:,8]-howBig,'-',color='gray',label='median-limit')
 
     plt.ylabel('meters',fontsize=fs)
     plt.title('All Reflector Heights for ' + station.upper() + ' when QC is applied: ' ,fontsize=fs)
```

### Comparing `gnssrefl-3.1.4/gnssrefl/daily_avg_cl.py` & `gnssrefl-3.1.5/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-3.1.5/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/decipher_argt.py` & `gnssrefl-3.1.5/gnssrefl/decipher_argt.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     station : str
         4 char id
     filename : str
         NMEA output from Argentina
     idec : int
         decimation interval, sec
     snrname : str
-        ultimaet output file
+        ultimate output file
     orbfile : str
         sp3 filename
     recx : list of floats
         Cartesian station coordinates in meters
     csnr: str
         2 ch snr file choice, i.e. '66' or '99'
     year : int
@@ -87,32 +87,33 @@
                             freq.append(1)
                             t.append(sod) ; snr.append(dat) ; az.append(azimA) ; elv.append(eleA)
 
             except:
                 iii = 0
     #print(igal,igps,iglo)
     message = 'None '
+    xdir = os.environ['REFL_CODE']
+    logdir = xdir + '/logs'
     # make sure this directory exists
-    if not os.path.isdir('logs'):
-        subprocess.call(['mkdir', 'logs'])
+    if not os.path.isdir(logdir):
+        subprocess.call(['mkdir', logdir])
 
     # temporary file - will be deleted
-    outputfile = 'logs/' + station + 'tmp.txt'
+    outputfile = logdir + '/' + station + 'tmp.txt'
     # write to file tod, iprn, s1, freq
     fout = open(outputfile, 'w+')
     fout.write('{0:15.4f}{1:15.4f}{2:15.4f} \n'.format(recx[0], recx[1],recx[2]) )
     fout.write('{0:6.0f}{1:6.0f}{2:6.0f} \n'.format(year, month, day) )
     for i in range(0,len(t)):
         # might as well decimate
         if ( (int(t[i]) % idec) == 0):
             fout.write('{0:8.0f} {1:3.0f} {2:6.2f} {3:1.0f} \n'.format(t[i], prn[i], snr[i],freq[i]) )
     fout.close()
 
-
-    errorlog = 'logs/' + station + '_nmea2snr_error.txt'
+    errorlog = logdir + '/' + station + '_nmea2snr_error.txt'
 
     in1 = g.binary(outputfile)
     in2 = g.binary(snrname)
     in3 = g.binary(orbfile)
     in4 = g.binary(csnr)
     in5 = g.binary(errorlog)
     xnmeasnr.foo(in1,in2,in3,in4,in5)
```

### Comparing `gnssrefl-3.1.4/gnssrefl/download_ioc.py` & `gnssrefl-3.1.5/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_noaa.py` & `gnssrefl-3.1.5/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_orbits.py` & `gnssrefl-3.1.5/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_psmsl.py` & `gnssrefl-3.1.5/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_rinex.py` & `gnssrefl-3.1.5/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_teqc.py` & `gnssrefl-3.1.5/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_tides.py` & `gnssrefl-3.1.5/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_unr.py` & `gnssrefl-3.1.5/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/download_wsv.py` & `gnssrefl-3.1.5/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/filesizes.py` & `gnssrefl-3.1.5/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gnssir_cl.py` & `gnssrefl-3.1.5/gnssrefl/gnssir_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,21 +88,24 @@
         Analyzes data from day of year 15 to day of year 20
     gnssir p041 2021 15 -dec 5
         before computing periodograms, decimates the SNR file contents to 5 seconds
     gnssir p041 2021 15 -gzip T
         gzips the SNR file after you run the code. Big space saver (now the default)
 
     Parameters
-    ----------
+    --------
     station : str
         lowercase 4 character ID of the station
     year : int
         full Year
     doy : integer
         Day of year
+
+    Optional parameters (requires hyphen prefix)
+    ----------
     snr : int, optional
         SNR format. This tells the code what elevation angles to save data for. Input is the snr file ending.
         Value options:
 
             66 (default) : saves all data with elevation angles less than 30 degress
 
             99 : saves all data with elevation angles between 5 and 30 degrees
```

### Comparing `gnssrefl-3.1.4/gnssrefl/gnssir_cl_old.py` & `gnssrefl-3.1.5/gnssrefl/gnssir_cl_old.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gnssir_input.py` & `gnssrefl-3.1.5/gnssrefl/gnssir_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gnssir_v2.py` & `gnssrefl-3.1.5/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gnsssnr.f` & `gnssrefl-3.1.5/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gnsssnrbigger.f` & `gnssrefl-3.1.5/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gps.py` & `gnssrefl-3.1.5/gnssrefl/gps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1985,14 +1985,15 @@
 
 def open_outputfile(station,year,doy,extension):
     """
     opens an output file in 
     $REFL_CODE/year/results/station/extension directory
     for lomb scargle periodogram results
 
+
     Parameters
     ----------
     station : str
         4 ch station name
     year : int
         full year
     doy : int
@@ -2003,24 +2004,24 @@
     Returns
     -------
     fileID : ?
         I don't know the proper name of this - but what comes out
         when you open a file so you can keep writing to it
 
     """
-    if os.path.isdir('logs'):
-        skippingxist = True
-    else:
-        subprocess.call(['mkdir', 'logs'])
+    xdir = os.environ['REFL_CODE']
+    logdir = xdir + '/logs'
+
+    if not os.path.isdir(logdir):
+        subprocess.call(['mkdir', logdir])
     fout = 0
 #   primary reflector height output goes to this directory
-    xdir = os.environ['REFL_CODE']
     cdoy = '{:03d}'.format(doy)
 #   extra file with rejected arcs
-    w = 'logs/reject.' + str(year) + '_' + cdoy  + station + '.txt'
+    w = logdir + '/reject.' + str(year) + '_' + cdoy  + station + '.txt'
 
     filedir = xdir + '/' + str(year)  + '/results/' + station 
 #   changed to a function
     filepath1,fexit = LSPresult_name(station,year,doy,extension)
     #print('Output will go to:', filepath1)
     versionNumber = 'v' + str(version('gnssrefl'))
     #versionNumber = 'working-on-it'
@@ -4689,36 +4690,54 @@
 def get_obstimes_plus(tvd):
     """
     send a LSP results file, so the variable created when you read
     in the results file.  return obstimes for matplotlib plotting purposes
     2022jun10 - added MJD output
 
     See get_obstimes 
+    2024apr06 too slow because I was using np.append
 
+    Parameters
+    ----------
+    tvd : numpy array
+        contents of Lomb Scargle data processing
+    Returns
+    -------
+    obstimes: list of datetime objects
+        times of observations 
+    modjulian : list of floats
+        modified julian days
 
     """
     nr,nc = tvd.shape
     obstimes = []
-    modjulian = np.empty(shape=[0,1])
+    #modjulian = np.empty(shape=[0,1])
+    modjulian = []
 
     if nr > 0:
         for ijk in range(0,nr):
             dtime, iyear,imon,iday,ihour,imin,isec = ymd_hhmmss(tvd[ijk,0],tvd[ijk,1],tvd[ijk,4],True)
             obstimes.append(dtime)
             m,f = mjd(iyear,imon,iday,ihour,imin,isec)
             x=[m+f]
-            modjulian = np.append(modjulian, [x],axis=0 )
+            xx = m+f
+            #modjulian = np.append(modjulian, [x],axis=0 )
+            modjulian.append(xx)
     else:
         print('empty file')
 
+    # afterwards change to np array - but probably best to keep them as lists for now
+    #modjulian = np.asarray(modjulian)
+
     return obstimes, modjulian
 
 
 def confused_obstimes(tvd):
     """
+    this will be slow (and should be fixed)
 
     Parameters
     ----------
     tvd : numpy array
         results of LSP results
 
     Returns
@@ -4736,14 +4755,15 @@
     else:
         print('empty file')
 
     return modifiedjulian
 
 def more_confused_obstimes(tvd):
     """
+    too slow
 
     Parameters
     ----------
     tvd : numpy array of floats
         lsp results from a loadtxt command
 
     Returns
@@ -4881,15 +4901,16 @@
     Parameters
     ----------
     t : list of integers
         year, month, day, hour, minute, second 
 
     Returns
     -------
-    obstimes : datetime 
+    obstimes : list
+        datetime format
 
     """
     nr,nc = t.shape
     obstimes = []
 
     # if i read in the file better, would not have to change from float
     # year mon day hour min sealevel doy mjd seconds
@@ -4911,49 +4932,62 @@
     ----------
     t : numpy array
         our water level format
         where year, month, day, hour, minute, second are in the first columns
 
     Returns
     -------
-    obstimes : datetime obj
-        timetags 
+    obstimes : list of datetime obj
+        list of timetags 
 
-    modjulian : numpy array of floats
-        modified julian date array 
+    modjulian : list of floats
+        modified julian date 
 
     """
     time_format = kwargs.get('time_format','new')
     if time_format == 'new':
         tt = True
     else:
         tt = False
 
     nr,nc = t.shape
+
     obstimes = []
-    modjulian = np.empty(shape=[0,1])
-    #modjulian=[]
+    # was doing this
+    #modjulian = np.empty(shape=[0,1])
+    # now try this
+    modjulian=[]
 
     # if i read in the file better, would not have to change from float
+    # slow because i am using np.append
     if nr > 0:
         for i in range(0,nr):
             # new fileformat
             if tt:
                 year = int(t[i,0]); month=int(t[i,1]); day=int(t[i,2]); hour=int(t[i,3]); minute=int(t[i,4]); second = int(t[i,5])
             else:
                 year = int(t[i,0]); month=int(t[i,1]); day=int(t[i,2]); hour=int(t[i,3]); minute=int(t[i,4]); second = int(t[i,8])
 
             dtime = datetime.datetime(year=year, month=month, day=day, hour=hour, minute=minute, second=second)
             obstimes.append(dtime)
             imjd, fr = mjd(year,month,day,hour,minute,second)
             x = [imjd+fr]
-            modjulian = np.append(modjulian, x)
+            #modjulian = np.append(modjulian, x)
+            xx = float(imjd+fr)
+            modjulian.append(xx)
     else:
         print('you sent me an empty variable')
 
+    # change modjulian to numpy array at the append
+    #modjulian = np.asarray(modjulian)
+    #nr,nc=modjulian.shape
+    #print('mjd', nr,nc)
+    #nr,nc=obstimes.shape
+    #print('obstimes ' , nr,nc)
+
     return obstimes, modjulian
 
 
 def final_gfz_orbits(year,month,day):
     """
     downloads gfz final orbit and stores in $ORBITS
 
@@ -6739,14 +6773,87 @@
     return year, doy
 
 
 def randomfilename():
     """
     makes a string -length 9 - using random number
     generator.  useful for filenames
+
+    Returns
+    -------
+    rname : str
+        filename with nine random numerical characters
+
     """
     a=math.modf(random())
     xx = int(math.floor(a[0]*1000000000))
     # make sure it is length 9
     rname = '{:09d}'.format(xx)
     return rname
 
+
+def replace_wget(url,f):
+    """
+    use requests instead of wget to download files
+    this cannot be used for ftp addresses.
+
+    Parameters
+    ----------
+    url : str
+        full path to file
+    f : str
+        filename
+
+    Returns
+    -------
+    success : bool
+        whether file was found or not
+    """
+    # use a try in case the website is down
+    try:
+        response = requests.get(url)
+        #print(response.status_code)
+        if response.status_code == 200:
+            with open(f, "wb") as file:
+                file. write(response.content)
+            success = True
+        else:
+            success = False
+    except:
+        print('No file downloaded')
+        success = False
+
+    if success: 
+        print("Successful download:", f)
+
+    return success
+
+def define_logdir(station,year,doy):
+    """
+    creates logfile name and directory (for rinex2snr) 
+    given a station, year and day of year
+
+    Parameters
+    ----------
+    station : str
+        4 ch station name
+    year : int
+        full year
+    doy : int
+        day of year
+    """
+    cyyyy,cyy,cdoy = ydoych(year,doy)
+
+    xdir = os.environ['REFL_CODE']
+
+    # universal location for the log directory
+    logdir = xdir + '/logs/' + station + '/' + cyyyy + '/'
+
+    # define directory for the 
+    if not os.path.isdir(logdir):
+        subprocess.call(['mkdir', '-p',logdir])
+
+    logname = cdoy + '_translation.txt'
+
+    return logdir, logname
+
+
```

### Comparing `gnssrefl-3.1.4/gnssrefl/gpssnr.f` & `gnssrefl-3.1.5/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gpsweek.py` & `gnssrefl-3.1.5/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/gpt_1wA.pickle` & `gnssrefl-3.1.5/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/highrate.py` & `gnssrefl-3.1.5/gnssrefl/highrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,28 +215,28 @@
 def bkg_highrate(station, year, month, day,stream,dec_rate,bkg):
     """
     picks up a highrate RINEX 3 file from BKG, merges and decimates it.
     requires gfzrnx
 
     Parameters
     ----------
-    inputs: string
+    station : str
         9 ch station name 
-    year : integer
+    year : int
         full year
     month : integer
         month or day of year if day set to 0
-    day : integer
+    day : int
         day of the month
     stream : str
         R or S
-    dec_rate : integer
+    dec_rate : int
         decimation rate in seconds
     bkg : str
-        file directory at BKG
+        file directory at BKG (igs or euref)
 
     Returns
     -------
     file_name24 : str
         name of merged rinex file
     fexist : boolean
         whether file exists
@@ -275,34 +275,37 @@
     for h in range(0,24):
         # subdirectory
         ch = '{:02d}'.format(h)
         print('Hour: ', ch)
         for e in ['00', '15', '30', '45']:
             file_name = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.crx.gz'
             dirname = gns + '/' + alpha[h] + '/'
-            print('looking for', dirname + file_name)
+            #print('looking for', dirname + file_name)
             crnx_name = file_name[:-3] 
             oname = file_name[:-6] + 'rnx'
 
             if os.path.isfile(oname):
                 fileF = fileF + 1
-                print('already have ', oname)
+                print('You already have ', oname, ' so no need to download')
             else:
                 try:
-                    wget.download(dirname+file_name,file_name)
-                    subprocess.call(['gunzip',file_name]) # unzip
-                    subprocess.call([crnxpath, crnx_name]) # hatanaka
-                    subprocess.call(['rm',crnx_name]) # remove old file
+                    s = g.replace_wget(dirname+file_name, file_name)
+                    #wget.download(dirname+file_name,file_name)
+                    if os.path.isfile(file_name):
+                        subprocess.call(['gunzip',file_name]) # unzip
+                        subprocess.call([crnxpath, crnx_name]) # hatanaka
+                        subprocess.call(['rm',crnx_name]) # remove old file
                 except:
                     okok = 1
+                    print('Could not find ', file_name, ' at BKG')
                 if os.path.isfile(oname):
-                    print('successful download ', oname)
+                    #print('successful download ', oname)
                     fileF = fileF + 1
-                else:
-                    print('unsuccessful download ', oname)
+                #else:
+                #    print('unsuccessful download ', oname)
 
     searchP = station.upper() + streamID + cyyyy + cdoy + '*15M*MO.rnx'
     print('Found ', fileF,' 15 minute files')
 
     outfile = station.upper() + cyyyy + cdoy + '.tmp'
     crate = '{:02d}'.format(dec_rate)
 
@@ -386,33 +389,33 @@
     s1 = time.time()
     for h in range(0,23):
         # subdirectory
         ch = '{:02d}'.format(h)
         print('Hour: ', ch)
         file_name = station.upper() + streamID + cyyyy + cdoy + ch + '00_01H_01S_MO.crx.gz'
         dirname = gns + '/' + ch + '/'
-        print('looking for', dirname + file_name)
+        #print('looking for', dirname + file_name)
         crnx_name = file_name[:-3] 
         oname = file_name[:-6] + 'rnx'
         if os.path.isfile(oname):
             fileF = fileF + 1
             print('already have ', oname)
         else:
             try:
                 wget.download(dirname+file_name,file_name)
                 subprocess.call(['gunzip',file_name]) # gunzip
                 subprocess.call([crnxpath, crnx_name]) # hatanaka
                 subprocess.call(['rm',crnx_name]) # remove old file
             except:
                 okok = 1
             if os.path.isfile(oname):
-                print('successful download ', oname)
+                print('Successful download ', oname)
                 fileF = fileF + 1
             else:
-                print('unsuccessful download ', oname)
+                print('Unsuccessful download ', oname)
 
     searchP = station.upper() + streamID + cyyyy + cdoy + '*01H*MO.rnx'
     print(searchP)
     print('Found ', fileF,' one hour files')
 
     outfile = station.upper() + '.tmp'
     crate = '{:02d}'.format(dec_rate)
```

### Comparing `gnssrefl-3.1.4/gnssrefl/installexe_cl.py` & `gnssrefl-3.1.5/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/invsnr_cl.py` & `gnssrefl-3.1.5/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/invsnr_input.py` & `gnssrefl-3.1.5/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/karnak_libraries.py` & `gnssrefl-3.1.5/gnssrefl/karnak_libraries.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,28 +89,31 @@
     cdoy: str
         three character day of year
 
     file_name: str
         expected RINEX filename
 
     """
+    # BKG has two separate archives - 
     dir1 = 'https://igs.bkg.bund.de/root_ftp/IGS/obs/' + cyyyy + '/' + cdoy + '/'
     dir2 = 'https://igs.bkg.bund.de/root_ftp/EUREF/obs/' + cyyyy + '/' + cdoy + '/'
     print('>>> Trying first : ',dir1+file_name)
     fexist = False
     try:
-        wget.download(dir1+file_name,file_name)
-        fexist = True
+        fexist = g.replace_wget(dir1+file_name, file_name)
+        #wget.download(dir1+file_name,file_name)
+        #fexist = True
     except:
-        print('did not find the file')
+        print('did not find the RINEX 3 file')
     if (not fexist):
         print('>>> Now trying: ',dir2+file_name)
         try:
-            wget.download(dir2+file_name,file_name)
-            fexist = True
+            fexist = g.replace_wget(dir2+file_name, file_name)
+            #wget.download(dir2+file_name,file_name)
+            #fexist = True
         except:
             print('did not find it there either')
 
     return
 
 def universal(station9ch, year, doy, archive,srate,stream,debug=False):
     """
@@ -203,18 +206,19 @@
         elif (archive == 'sonel'):
             dir1='ftp://ftp.sonel.org/gps/data/' + cyyyy + '/' + cdoy + '/'
             wget.download(dir1+file_name,file_name)
         elif archive == 'bkg':
             just_bkg(cyyyy, cdoy, file_name)
         elif (archive == 'bev'):
             dir1 = 'https://gnss.bev.gv.at/at.gv.bev.dc/data/obs/' + cyyyy + '/' + cdoy + '/'
-            wget.download(dir1+file_name,file_name)
+            #wget.download(dir1+file_name,file_name)
+            fex = g.replace_wget(dir1+file_name, file_name)
         elif (archive == 'epn'):
             dir1 = 'https://epncb.oma.be/ftp/obs/' + cyyyy + '/' + cdoy + '/'
-            print(dir1)
+            #print(dir1)
             wget.download(dir1+file_name,file_name)
         elif (archive == 'ignes'):
            # if someone wanted to help by adding this to the high rate
            # https://datos-geodesia.ign.es/ERGNSS/horario_1s/YYYYMMDD/HH/file
             dir1 = 'https://datos-geodesia.ign.es/ERGNSS/diario_30s/' + cyyyy + '/' + cyyyy + cmm + cdd + '/'
             #print(dir1)
             wget.download(dir1+file_name,file_name)
@@ -224,25 +228,24 @@
             request = requests.get(API_URL, QUERY_PARAMS, headers=headers)
         #request.raise_for_status()
         # i don't know how to read this - so doing it the dumb way
             if len(json.loads(request.content)) == 1:
                 for query_response_item in json.loads(request.content):
                     file_url = query_response_item['fileLocation']
                     file_name = urlparse(file_url).path.rsplit('/', 1)[1]
-                    wget.download(file_url,file_name)
+                    fex = g.replace_wget(file_url, file_name)
+                    #wget.download(file_url,file_name)
         elif (archive == 'nrcan'):
             dir1 = 'https://cacsa.nrcan.gc.ca/gps/data/gpsdata/' + cyy + cdoy  + '/' + cyy + 'd' + '/'
             wget.download(dir1+file_name,file_name)
-        elif (archive == 'unavco-old'):
-            dir1 = 'https://data.unavco.org/archive/gnss/rinex3/obs/' + cyyyy + '/' + cdoy + '/'
-            wget.download(dir1+file_name,file_name)
+        #elif (archive == 'unavco-old'):
+        #    dir1 = 'https://data.unavco.org/archive/gnss/rinex3/obs/' + cyyyy + '/' + cdoy + '/'
+        #    wget.download(dir1+file_name,file_name)
         elif (archive == 'gfz'):
-            # no idea
             dir1 = 'ftp://isdcftp.gfz-potsdam.de/gnss/data/daily/' + cyyyy + '/' + cdoy + '/'
-            #print(dir1+file_name)
             wget.download(dir1+file_name,file_name)
         elif (archive == 'cddis'):
             new_way_dir = '/gnss/data/daily/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/'
             g.cddis_download_2022B(file_name,new_way_dir)
         else:
             return '', ''
     except:
@@ -266,30 +269,26 @@
 def filename_plus(station9ch,year,doy,srate,stream):
     """
     function to create RINEX 3 filenames for one day files.
 
     Parameters
     ----------
     station9ch : str
-         9 character station name
-
+        9 character station name
     year : int
-
+        full year
     doy : int
         day of year
-
     srate : int
-         receiver sample rate 
-
+        receiver sample rate 
     stream : str 
-         R or S ; latter means the file was streamed.
-
+        R or S ; latter means the file was streamed.
     output : str
-         compliant filename with crx.gz on the end as this is how the files 
-         are stored at GNSS archives as far as I know.
+        compliant filename with crx.gz on the end as this is how the files 
+        are stored at GNSS archives as far as I know.
 
     Returns
     -------
     file_name : str
         filename of the RINEX 3 file
     cyyyy : str
         4ch year 
@@ -320,17 +319,17 @@
     doy : int
         day of year
     rinexv : int
         rinex version        
 
     Returns
     -------
-    QUERY_PARAMS : json
+    QUERY_PARAMS : dict
         I think
-    headers : json
+    headers : dict
         I think
 
     """
     d = datetime.datetime(year, 1, 1) + datetime.timedelta(days=(doy-1))
     month = int(d.month); day = int(d.day)
     cmonth = '{:02d}'.format(month); cday = '{:02d}'.format(day)
 
@@ -440,15 +439,15 @@
         name of the GNSS archive
     screenstats : bool
         whether print statements come to scree
 
     Returns
     -------
     file_name : str
-        filename that was downloaded
+        RINEX filename that was downloaded
     foundit : bool
         whether file was found
 
     """
     # define the file name
 
     foundit = False; dir1 = ''; file_name = ''
@@ -467,45 +466,53 @@
     s1 = time.time()
     if (archive == 'jp'):
         # i did not want to rewrite the code
         gsi_data(station, year, doy)
         file_name = oname
         if os.path.exists(file_name):
             foundit = True
-    elif (archive == 'unavco-old'):
-        dir1 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy
-        foundit, file_name = gogetit(dir1, dname, '.Z'); 
-        if not foundit:
-            foundit, file_name = gogetit(dir1, oname, '.Z')
+    #elif (archive == 'unavco-old'):
+    #    dir1 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy
+    #    foundit, file_name = gogetit(dir1, dname, '.Z'); 
+    #    if not foundit:
+    #        foundit, file_name = gogetit(dir1, oname, '.Z')
     elif (archive == 'unavco'):
         #url1 = 'https://data-idm.unavco.org/archive/gnss/rinex/obs/' + cydoy + dname + '.Z'
         url1 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy + dname + '.Z'
-        print(url1)
+        if screenstats:
+            print(url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1, dname + '.Z')
         if not foundit:
             url2 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy + oname + '.Z'
-            print(url2)
+            if screenstats:
+                print(url2)
             foundit,file_name = kelly.the_kelly_simple_way(url2, oname + '.Z')
     elif (archive == 'special'):
         #print('testing out new protocol at unavco')
         url1 = 'https://data.unavco.org/archive/gnss/products/reflectometry/' + cydoy + oname + '.gz'
         if screenstats:
             print(url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1, oname + '.gz')
         # old way
         #foundit, file_name = gogetit(dir1, oname, '.gz'); 
     elif archive == 'sopac':
         dir1 = 'ftp://garner.ucsd.edu/pub/rinex/' + cydoy
+        file_name = dname + '.Z'
+        url = dir1 + '/' + file_name
         foundit, file_name = gogetit(dir1, dname, '.Z');
     elif archive == 'sonel':
         dir1 = 'ftp://ftp.sonel.org/gps/data/' + cydoy
         foundit, file_name = gogetit(dir1, dname, '.Z');
     elif archive == 'nz':
-        dir1 =  'https://data.geonet.org.nz/gnss/rinex/' + cydoy
-        foundit, file_name = gogetit(dir1, oname, '.gz'); 
+        dir1 =  'https://data.geonet.org.nz/gnss/rinex/' + cydoy + '/'
+        # try using requests
+        file_name = oname + '.gz'
+        url = dir1 + file_name
+        foundit = g.replace_wget(url, file_name)
+        #foundit, file_name = gogetit(dir1, oname, '.gz'); 
     elif archive == 'bkg':
         # are the old data with Z instead of gz?
         dir1 = 'https://igs.bkg.bund.de/root_ftp/IGS/obs/' + cydoy
         dir2 = 'https://igs.bkg.bund.de/root_ftp/EUREF/obs/' + cydoy
 
         foundit, file_name = gogetit(dir1, dname, '.Z');
         if not os.path.exists(file_name):
@@ -523,17 +530,21 @@
             dir1 = 'ftp://gps.alaska.edu/pub/gpsdata/permanent/C2/' + cydoy
             foundit, file_name = gogetit(dir1, oname, '.gz');
         else:
             dir1 = 'ftp://gps.alaska.edu/pub/gpsdata/CoopCORS/' + cydoy + '/' + station.upper() + '/'
             foundit, file_name = gogetit(dir1, oname, '.gz');
     elif (archive == 'ngs'):
         dir1 = 'https://geodesy.noaa.gov/corsdata/rinex/' + cydoy + '/' + station + '/'
-        foundit, file_name = gogetit(dir1, oname, '.gz');
+        file_name = oname + '.gz' ; url = dir1 + file_name
+        foundit = g.replace_wget(url,file_name)
+        #foundit, file_name = gogetit(dir1, oname, '.gz');
         if not foundit:
-            foundit, file_name = gogetit(dir1, dname, '.gz')
+            file_name = dname + '.gz'; url = dir1 + file_name
+            foundit = g.replace_wget(url,file_name)
+            #foundit, file_name = gogetit(dir1, dname, '.gz')
     elif (archive == 'cddis'):
         foundit,file_name = serial_cddis_files(dname,cyyyy,cdoy); 
     elif (archive == 'ga'):
         QUERY_PARAMS, headers = ga_stuff(station, year, doy)
         API_URL = 'https://data.gnss.ga.gov.au/api/rinexFiles/'
         QUERY_PARAMS['rinexVersion'] = '2'
         request = requests.get(API_URL, QUERY_PARAMS, headers=headers)
```

### Comparing `gnssrefl-3.1.4/gnssrefl/kelly.py` & `gnssrefl-3.1.5/gnssrefl/kelly.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     s1 = time.time()
     token = device_flow.access_token
     s2 = time.time()
     #print('Time it took doing whatever ', s2-s1)
 
     headers = {}
     headers['authorization'] = 'Bearer ' + token
+    #print('In the kelly function')
 
     s1 = time.time()
     r = requests.get(url, headers=headers)
     s2 = time.time()
     # Opens a local file of same name as remote file for writing to
     # check to see that the file exists
     if (r.status_code == requests.codes.ok):
```

### Comparing `gnssrefl-3.1.4/gnssrefl/llh2xyz.py` & `gnssrefl-3.1.5/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/make_meta.py` & `gnssrefl-3.1.5/gnssrefl/make_meta.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/max_resolve_RH_cl.py` & `gnssrefl-3.1.5/gnssrefl/max_resolve_RH_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/nmea2snr.py` & `gnssrefl-3.1.5/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/nmea2snr_cl.py` & `gnssrefl-3.1.5/gnssrefl/nmea2snr_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station name", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("doy", help="start day of year", type=int)
 
-    parser.add_argument("-snr", default='66', help="snr file ending, 99: 5-30 deg.; 66: < 30 deg.; 88: all data; 50: < 10 deg", type=str)
+    parser.add_argument("-snr", default='66', help="snr file type, 99: 5-30 deg.; 66: < 30 deg.; 88: all data; 50: < 10 deg", type=str)
     parser.add_argument("-year_end", default=None, help="end year", type=int)
     parser.add_argument("-doy_end", default=None, help="end day of year", type=int)
     parser.add_argument("-overwrite", default=None, help="boolean", type=str)
     parser.add_argument("-dec", default=None, help="decimation, seconds", type=int)
     parser.add_argument("-lat", default=None, help="latitude, degrees", type=float)
     parser.add_argument("-lon", default=None, help="longitude, degrees", type=float)
     parser.add_argument("-height", default=None, help="ellipsoid height, m", type=float)
-    parser.add_argument("-risky", default=None, help="boolean for whether sp3 orbits are used", type=str)
+    parser.add_argument("-risky", default=None, help="boolean for whether low quality orbits are used instead of precise sp3", type=str)
     parser.add_argument("-gzip", default=None, help="gzip SNR file after creation. Default is true.", type=str)
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
     boolean_args = ['risky', 'gzip', 'overwrite']
     args = str2bool(args, boolean_args)
@@ -73,15 +73,15 @@
     station : str
         4 ch name of station
     year : int
         full year
     doy : int
         day of year
     snr : int, optional
-        snr file type, default is 66
+        snr file type (default is 66); 99: 5-30 deg.; 66: < 30 deg.; 88: all data; 50: < 10 deg
     year_end : int, optional
         final year
     doy_end : int, optional
         final day of year
     overwrite : bool, optional
         whether make a new SNR file even if one already exists
     dec : int, optional
```

### Comparing `gnssrefl-3.1.4/gnssrefl/nyquist_libs.py` & `gnssrefl-3.1.5/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/phase_functions.py` & `gnssrefl-3.1.5/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/prn2gps.py` & `gnssrefl-3.1.5/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/query_unr.py` & `gnssrefl-3.1.5/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/quickLook_cl.py` & `gnssrefl-3.1.5/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/quickLook_function2.py` & `gnssrefl-3.1.5/gnssrefl/quickLook_function2.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,19 @@
     # dictionary for key
     datakey = {'NW':{},'SW':{},'NE':{},'SE':{},'fNW':{},'fSW':{},'fNE':{},'fSE': {} }
 
     # make sure environment variables exist
     g.check_environ_variables()
 
     # make sure logs directory exists
-    if not os.path.isdir('logs'):
-        subprocess.call(['mkdir', 'logs'])
+    xdir = os.environ['REFL_CODE']
+    logdir = xdir + '/logs'
+
+    if not os.path.isdir(logdir):
+        subprocess.call(['mkdir', logdir])
 
     # if it finds the station coordinates, it will return irefr as 1
     quick_p,quick_T,irefr, quick_e = quick_refraction(station)
 
     webapp = False 
     # orbit directories
     ann = g.make_nav_dirs(year)
@@ -139,15 +142,15 @@
     allGood, snrD, nrows, ncols = gnssir_v2.read_snr(obsfile)
 
     if allGood == 0:
         print('file does not exist'); sys.exit()
     else:
         # make output file for the quickLook RRH values, just so you can give them a quick look see
         # also used in the azimuth QC plot
-        quicklog = 'logs/rh_' + station + '.txt'
+        quicklog = logdir + '/rh_' + station + '.txt'
         rhout = open(quicklog,'w+')
         amax = 0
         minEdataset = min(snrD[:,1])
         print('minimum elevation angle (degrees) for this dataset: ', minEdataset)
         if minEdataset > (e1+0.5):
             print('It looks like the receiver had an elevation mask. Overriding e1 to this value.')
             e1 = minEdataset
```

### Comparing `gnssrefl-3.1.4/gnssrefl/quickPhase.py` & `gnssrefl-3.1.5/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/quicklib.py` & `gnssrefl-3.1.5/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/quickplt.py` & `gnssrefl-3.1.5/gnssrefl/quickplt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import argparse
 from astropy.time import Time
 import datetime
-import matplotlib.pyplot as plt
+import matplotlib.pyplot as myplt
 import numpy as np
 import os
 import subprocess
 import sys
 
 
 import gnssrefl.quicklib as q
@@ -14,71 +14,95 @@
 
 from gnssrefl.utils import validate_input_datatypes, str2bool
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
 
     parser.add_argument("filename", help="filename", type=str)
-    parser.add_argument("xcol", help="x-column", type=int)
-    parser.add_argument("ycol",   help="y-column", type=int)
-    parser.add_argument("-errorcol",   help="error bar for y-values", type=int,default=None)
-    parser.add_argument("-mjd", help="if x-values are MJD ", type=str,default=None)
+    parser.add_argument("xcol", help="x-axis column number", type=str)
+    parser.add_argument("ycol",   help="y-axis column number", type=str)
+    parser.add_argument("-errorcol",   help="column for errors for y-axis values", type=int,default=None)
+    parser.add_argument("-mjd", help="True/T for when x-values are MJD ", type=str,default=None)
     parser.add_argument("-reverse", help="reverse the y-axis", type=str,default=None)
-    parser.add_argument("-ymd", help="columns 1-3 are year mon day ", type=str,default=None)
-    parser.add_argument("-ymdhm", help="columns 1-5 are year mon day hour minute", type=str,default=None)
+    parser.add_argument("-ymd", help="True/T for when columns 1-3 are year month day ", type=str,default=None)
+    parser.add_argument("-ymdhm", help="True/T for when columns 1-5 are year month day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
-    parser.add_argument("-symbol", help="plot symbol ", type=str,default=None)
+    parser.add_argument("-symbol", help="plot symbol, e.g. * or -", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot. Must end in png", type=str,default=None)
-    parser.add_argument("-xlimits", nargs="*",type=float, help="optional xlimits", default=None)
-    parser.add_argument("-ylimits", nargs="*",type=float, help="optional ylimits", default=None)
-    parser.add_argument("-ydoy", help="if True/T, columns 1-2 are year and doy", type=str,default=None)
+    parser.add_argument("-xlimits", nargs="*",type=float, help="optional x-axis limits", default=None)
+    parser.add_argument("-ylimits", nargs="*",type=float, help="optional y-axis limits", default=None)
+    parser.add_argument("-ydoy", help="True/T for when columns 1-2 are year and doy", type=str,default=None)
     parser.add_argument("-filename2", help="second filename", type=str, default=None)
     parser.add_argument("-freq", help="spec freq, column 11 in a LSP file ", type=int,default=None)
     parser.add_argument("-utc_offset", help="offset from UTC, hours  ", type=int,default=None)
     parser.add_argument("-yoffset", help="offset for y-axis values", type=float,default=None)
-    parser.add_argument("-keepzeros", help="keep zeros (default is to remove)", type=str,default=None)
-    parser.add_argument("-sat", help="print only this satellite (only for SNR file)", type=int,default=None)
+    parser.add_argument("-yoffset2", help="offset for y-axis values in file 2", type=float,default=None)
+    parser.add_argument("-keepzeros", help="True/T if you want to keep zero y-values (default is to remove)", type=str,default=None)
+    parser.add_argument("-sat", help="Only use this satellite (can also input gps, glonass, galileo, and beidou) SNR file", type=str,default=None)
+    parser.add_argument("-scale", help="scale factor for first file", type=float,default=None)
+    parser.add_argument("-scale2", help="scale factor for file 2", type=float,default=None)
+    parser.add_argument("-elimits", nargs="*",type=float, help="optional elevation angle limits for SNR file", default=None)
+    parser.add_argument("-azlimits", nargs="*",type=float, help="optional azimuth angle limits for SNR file", default=None)
+    parser.add_argument("-plt", help="Set to False/F if you do not want the plot to come to the screen ", type=str,default=None)
 
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['mjd', 'reverse', 'ymdhm', 'ydoy','ymd','keepzeros']
+    boolean_args = ['mjd', 'reverse', 'ymdhm', 'ydoy','ymd','keepzeros','plt']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def run_quickplt (filename: str, xcol: int, ycol: int, errorcol: int=None, mjd: bool=False, xlabel: str=None, 
+def run_quickplt (filename: str, xcol: str, ycol: str, errorcol: int=None, mjd: bool=False, xlabel: str=None, 
                   ylabel: str=None, symbol: str=None, reverse:bool=False,title:str=None,outfile: str=None,
                   xlimits: float=[], ylimits: float=[], ydoy:bool=False, ymd:bool=False, ymdhm:bool=False, 
                   filename2: str=None, freq:int=None, utc_offset: int=None, yoffset: float=None, 
-                  keepzeros: bool=False, sat: int=None):
+                  keepzeros: bool=False, sat: str=None,yoffset2: float=None,scale: float=1.0, 
+                  scale2: float=1.0, elimits: float=[0], azlimits:float=[0], plt:bool=True):
 
     """
     quick file plotting using matplotlib
 
     A png file is saved as temp.png or to your preferred
     filename if outfile is given. In either case, it goes to REFL_CODE/Files
 
     Allows you to set x and y-axis limits with a title and various axes labels, symbols etc.
     
     Someone could easily update this to include different filetypes (e.g. jpeg)
 
     I rewrote this recently to take advantage of our boolean argument translator.  Let me know 
     if things have broken or submit a PR.
 
+    To make simple plots of observables in SNR files, the x-axis can be either time or elevation.
+    The latter is short for elevation angle. To pick this option set -sat to a specific satellite
+    nubmer or a constellation (gps, glonass, etc). You can also set elimits and azlimits for simple
+    elevation angle and azimuth angle limits. Only for SNR files, you can send the name of the SNR file
+    without the directory, i.e. sc021500.22.snr66 instead of /Users/Files/2022/snr/sc02/sc021500.22.snr66
+
+    You may submit a filename that has been gzipped. The code will checked to see if the gzip version
+    is there and gunzip it for you.
+
+
     Examples
     --------
     quickplt txtfile 1 16
         would plot column 1 on the x-axis and column 16 on the y-axis
 
+    quickplt sc021500.22.snr66 time L1 -sat gps
+        would plot all the GPS L1 SNR data for the given SNR file, with time on the 
+        x-axis column 1 on the x-axis and SNR data on the y-axis
+        You have to set -sat or it will not work. For a specific satellite number,
+        provide that instead of gps. The other allowed x-axis option is elevation which
+        is short for elevation angle.
+
     quickplt txtfile 1 16 -xlabel Time
         would plot column 1 on the x-axis and column 16 on the y-axis
         and add Time on the x-axis label
 
     quickplt txtfile 1 16 -xlabel "Time (sec)"
         would plot column 1 on the x-axis and column 16 on the y-axis
         and add Time (sec) on the x-axis label, but need quote marks since you 
@@ -122,18 +146,20 @@
         Assuming you submitted a standard SNR file, it would plot the 
         data for Glonass satellite 22 for L2 data (column 8) vs time (seconds of the day in column 4). 
 
     Parameters
     ----------
     filename : str
         name of file to be plotted 
-    xcol : int
+    xcol : str
         column number in the file for the x-axis parameter
-    ycol : int
+        for snrfiles, you can say time or elevation
+    ycol : str
         column number in the file for the y-axis parameter
+        for snrfiles, you can say L1, L2, or L5
     errorcol : int, optional
         column number for the error bars
     mjd : bool, optional
         code will convert MJD to datetime (for xcol) 
     xlabel : str, optional
         label for x-axis 
     ylabel : str
@@ -167,42 +193,105 @@
     utc_offset: int, optional
         offset time axis by this number of hours (for local time)
         this only is used when the mjd option is used  
     yoffset : float
         add or subtract to the y-axis values
     keepzeros: bool, optional
         keep/remove zeros, default is to remove
-    sat : int
-        satellite number for SNR file plotting (i.e. column 1)
+    sat : str
+        satellite number for SNR file plotting 
+        for all gps satellites, say gps instead of a number
+        similar for glonass, galileo, and beidou
+    yoffset2 : float
+        add or subtract to the y-axis values in filename2
+    scale : float
+        multiply all y-axis values in file 1 by this value
+    scale2 : float
+        multiply all y-axis values in file 2 by this value
+    elimits : list of floats
+        if SNR file is plotted, elevation angle limits are applied
+    azlimits : list of floats
+        if SNR file is plotted, azimuth angle limits are applied
+    plt: bool
+         whether you want the plot to be displayed on the screen.
+         png file is always created.
 
     """
+    snrfile = False
+    if sat is not None:
+        snrfile = True
+
+        if xcol == 'elevation':
+            xcol = 1 # python column
+        elif xcol == 'time':
+            xcol = 3 # python column
+        else:
+            xcol = int(xcol) - 1
+
+        if (ycol.upper() == 'L1'):
+            ycolT = 'L1'
+            ycol = 6
+        elif (ycol.upper() == 'L2'):
+            ycolT = 'L2'
+            ycol = 7
+        elif (ycol.upper() == 'L5'):
+            ycolT = 'L5'
+            ycol = 8
+        else:
+            ycolT = ''
+            ycol = int(ycol) - 1
+    else:
+        # change strings to integers and change to python column
+        if (xcol == 'time'):
+            print('You cannot chose time for the xcolumn unless you invoke -sat mode. xcol must be an integer. Exit')
+            sys.exit()
+        elif (xcol == 'elevation'):
+            print('You cannot chose elevation for the xcolumn. Unless you invoke -sat mode. xcol must be an integer. Exit')
+            sys.exit()
+        else:
+            xcol = int(xcol) - 1
+            ycol = int(ycol) - 1
+
 
-    # change column numbers to pythonese
-    xcol = xcol - 1
-    ycol = ycol - 1
     if errorcol is None:
         yerrors = False
     else:
         yerrors = True
         errorcol = errorcol - 1
 
     if ylabel is None:
         ylabel = 'Unknown'
 
     secondFile = False
 
     if yoffset is None:
         yoffset = 0
+    if yoffset2 is None:
+        yoffset2 = 0
 
     reverse_sign = reverse
 
     convert_mjd = mjd
-
     commentsign = '%'
 
+    basename = os.path.basename(filename)
+    station = basename[0:4]
+    cyear = '20' + basename[9:11]  
+    if snrfile:
+        xdir = os.environ['REFL_CODE']
+        longfile = xdir + '/' + cyear + '/snr/' + station + '/' + basename
+        longfile_gz = longfile + '.gz'
+        if not os.path.isfile(filename) and os.path.isfile(longfile):
+            filename = longfile
+            print('using ', longfile)
+        elif not os.path.isfile(filename) and os.path.isfile(longfile_gz):
+            subprocess.call(['gunzip', longfile_gz])
+            filename = longfile
+            print('now using ', longfile)
+
     if (not os.path.isfile(filename)) & os.path.isfile(filename + '.gz'):
         print('I will be nice and gunzip the file for you ...')
         subprocess.call(['gunzip', filename + '.gz'])
 
     if os.path.isfile(filename):
         tvd = np.loadtxt(filename,comments=commentsign)
         if len(tvd) == 0:
@@ -218,32 +307,77 @@
                     return
                 else:
                     tvd = tvd[ii,:]
             if not keepzeros:
                 print('Remove zero values')
                 ii = (tvd[:,ycol] != 0)
                 tvd = tvd[ii,:]
-            if (sat is not None):
-                print('Only show satellite ', sat)
-                ii = (tvd[:,0] == sat)
-                tvd = tvd[ii,:]
+            if snrfile:
+                if sat.lower() == 'gps':
+                    print('Show all GPS satellites')
+                    print('initial nmber of observations:', len(tvd))
+                    ii = (tvd[:,0] < 33)
+                    tvd = tvd[ii,:]
+                    print('after editing:', len(tvd))
+                elif sat.lower() == 'glonass':
+                    print('Show all Glonass satellites')
+                    print('initial nmber of observations:', len(tvd))
+                    ii = (tvd[:,0] > 100) & (tvd[:,0] <= 199)
+                    tvd = tvd[ii,:]
+                    print('after editing:', len(tvd))
+                elif sat.lower() == 'galileo':
+                    print('Show all Galileo satellites')
+                    print('initial nmber of observations:', len(tvd))
+                    ii = (tvd[:,0] > 200) & (tvd[:,0] <= 299)
+                    tvd = tvd[ii,:]
+                    print('after editing:', len(tvd))
+                elif sat.lower() == 'beidou':
+                    print('Show all Beidou satellites')
+                    print('initial nmber of observations:', len(tvd))
+                    ii = (tvd[:,0] > 300) & (tvd[:,0] <= 399)
+                    tvd = tvd[ii,:]
+                    print('after editing:', len(tvd))
+                else:
+                    sat = int(sat)
+                    print('Only show satellite ', sat)
+                    ii = (tvd[:,0] == sat)
+                    tvd = tvd[ii,:]
             if len(tvd) == 0:
                 print('No data are left. Exiting')
                 sys.exit()
 
+            if snrfile:
+                # this means it is a SNR file
+                if len(elimits) == 2:
+                    print('Apply elevation angle limits')
+                    e1 = elimits[0]
+                    e2 = elimits[1]
+                    i= (tvd[:,1] >= e1) & (tvd[:,1] <= e2)
+                    tvd=tvd[i,:]
+                if len(azlimits) == 2:
+                    print('Apply azimuth angle limits')
+                    a1 = azlimits[0]
+                    a2 = azlimits[1]
+                    i= (tvd[:,2] >= a1) & (tvd[:,2] <= a2)
+                    tvd=tvd[i,:]
+                if len(tvd) == 0:
+                    print('no data for this satellite and these editing choices.')
+                    print('exiting '); sys.exit()
+
         tval = []
         yval = []
     else:
         print('input file does not exist')
         sys.exit()
 
 
     tvd2=[]
     secondFile = False
     if filename2 is not None:
+        print('Warning: filename2 does not allow SNR file options')
         if os.path.isfile(filename2):
             tvd2 = np.loadtxt(filename2,comments=commentsign)
             if len(tvd2) == 0:
                 print('empty input for filenumber 2')
                 return
             else:
                 secondFile = True
@@ -261,25 +395,27 @@
 
     tval,yval = q.trans_time(tvd, ymd, ymdhm, convert_mjd, ydoy,xcol,ycol,utc_offset)
 
     yval = yval + yoffset
 
     if secondFile:
         tval2,yval2 = q.trans_time(tvd2, ymd, ymdhm, convert_mjd, ydoy,xcol,ycol,utc_offset)
-        yval2 = yval2 + yoffset
+        yval2 = yval2 + yoffset2
+        yval2 = yval2*scale2
+
 
     # supercedes previous trans_time ... ??? 
     if ydoy:
         print('Making obstimes for ydoy x-axis')
         tval = g.ydoy2datetime(tvd[:,0], tvd[:,1])
     if ydoy & secondFile:
         print('Making obstimes for second ydoy x-axis')
         tval2 = g.ydoy2datetime(tvd2[:,0], tvd2[:,1])
 
-    fig,ax=plt.subplots()
+    fig,ax=myplt.subplots()
 
     # i.e. using default
     if symbol is None:
         if yerrors:
             ax.errorbar(tval, yval, yerr=tvd[:,errorcol], fmt='.',color='blue')
         else:
             ax.plot(tval, yval, 'b.')
@@ -287,61 +423,79 @@
         if yerrors:
             ax.errorbar(tval, yval, yerr=tvd[:,errorcol],fmt=symbol)
         else:
             ax.plot(tval, yval, symbol)
 
     # is second file currently supported???
     if secondFile:
-        ax.plot(tval2, yval2, symbol)
+        if symbol is None:
+            ax.plot(tval2, yval2, 'r.')
+        else:
+            ax.plot(tval2, yval2, color='red', fmt=symbol)
 
-    plt.grid()
-    plt.ylabel(ylabel)
+    myplt.grid()
+    myplt.ylabel(ylabel)
 
     if xlabel is not None:
-        plt.xlabel(xlabel)
+        myplt.xlabel(xlabel)
+    else:
+        if snrfile:
+            if (xcol == 1): # python column name
+                myplt.xlabel('elevation angle (degrees)')
+            if (xcol == 3): # using python column name
+                myplt.xlabel('seconds of the day')
+            myplt.ylabel(ycolT + ' SNR, dBHz')
+
 
     if title is None:
-        ax.set_title(os.path.basename(filename) )
+        if snrfile:
+            sname = os.path.basename(filename)
+            ytitle = sname[0:4] + ' 20' + sname[9:11] + ' ' + sname[4:7]
+            ax.set_title('sat ' + str(sat) + '/' + ytitle  )
+        else:
+            ax.set_title(os.path.basename(filename) )
     else:
         ax.set_title(title)
 
 
 
     if len(ylimits) == 2:
         print('found y-axis limits')
-        plt.ylim((ylimits))
+        myplt.ylim((ylimits))
     if len(xlimits) == 2:
         print('found x-axis limits')
         if convert_mjd:
             t1 = Time(xlimits[0],format='mjd')
             t1_utc = t1.utc # change to UTC
             tvalues1 =  t1_utc.datetime # change to datetime
             t2 = Time(xlimits[1],format='mjd')
             t2_utc = t2.utc # change to UTC
             tvalues2 =  t2_utc.datetime # change to datetime
-            plt.xlim((tvalues1,tvalues2))
+            myplt.xlim((tvalues1,tvalues2))
             if utc_offset is not None:
                 cc = '{:02d}'.format(abs(utc_offset)) + ':00'
                 if utc_offset < 0:
-                    plt.xlabel('UTC-' + cc)
+                    myplt.xlabel('UTC-' + cc)
                 else:
-                    plt.xlabel('UTC+' + cc)
+                    myplt.xlabel('UTC+' + cc)
         else:
             if ydoy:
                 t1,t2 = q.set_xlimits_ydoy(xlimits)
-                plt.xlim((t1,t2))
+                myplt.xlim((t1,t2))
             else:
-                plt.xlim((xlimits))
+                myplt.xlim((xlimits))
+
 
     if reverse_sign:
         ax.invert_yaxis()
     fig.autofmt_xdate() # obstimes
 
     q.save_plot(outfile)
-    plt.show()
+    if plt:
+        myplt.show()
 
 
 def main():
     args = parse_arguments()
     run_quickplt(**args)
 
 if __name__ == "__main__":
```

### Comparing `gnssrefl-3.1.4/gnssrefl/read_snr_files.py` & `gnssrefl-3.1.5/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/refl_zones.py` & `gnssrefl-3.1.5/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/refl_zones_cl.py` & `gnssrefl-3.1.5/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/refraction.py` & `gnssrefl-3.1.5/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rh_plot.py` & `gnssrefl-3.1.5/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rinex2snr.py` & `gnssrefl-3.1.5/gnssrefl/rinex2snr.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     """
     xdir  = os.environ['REFL_CODE'] + '/'
     fname =  xdir + str(year) + '/snr/' + station + '/' + station + cdoy + '0.' + cyy + '.snr' + csnr
 
     return fname
 
-def run_rinex2snr(station, year, doy,  isnr, orbtype, rate,dec_rate,archive,fortran,nol,overwrite,translator,srate, 
+def run_rinex2snr(station, year, doy,  isnr, orbtype, rate,dec_rate,archive, nol,overwrite,translator,srate, 
                   mk, stream,strip,bkg,screenstats,gzip):
     """
     main code to convert RINEX files into SNR files 
     now works on a single year and doy
 
     Parameters
     ----------
@@ -88,18 +88,14 @@
 
     dec_rate : integer
          decimation value
 
     archive : str
         choice of GNSS archive
 
-    fortran : bool
-        whether the fortran rinex translator is to be used
-        default: false
-
     nol: bool
         True: assumes RINEX files are in local directory
         False (default): will look at multiple - or specific archive
 
     overwrite: bool
         False (default): if SNR file exists, SNR file not made
         True: make a new SNR file
@@ -167,15 +163,15 @@
             fname =  quickname(station,year,cyy,cdoy,csnr)
             if screenstats:
                 print(fname)
             # now it unzips if that version exists
             snre = g.snr_exist(station,year,doy,csnr)
             if snre:
                 if overwrite:
-                    print('File exists, ', fname, ' and you requested overwriting, so will delete existing file')
+                    print('SNR file exists/you requested overwriting, existing file will be deleted')
                     if os.path.isfile(fname):
                         subprocess.call(['rm', fname]); 
                     if os.path.isfile(fname + '.gz'):
                         subprocess.call(['rm', fname + '.gz']); 
                     snre = False
                 else:
                     print('SNR file already exists', fname, '\n')
@@ -214,15 +210,15 @@
 
                             if screenstats:
                                 print('Found the RINEX 2.11 file', r)
                             if strip:
                                 if screenstats:
                                     print('Testing out stripping the RINEX 2 file here')
                                 k.strip_rinexfile(r)
-                            conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
+                            conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,translator)
                         else:
                             print('You Chose the No Look Option, but did not provide the needed RINEX file.')
                     if version == 3:
                         if rate == 'high':
                             csrate = '01' # high rate assumes 1-sec
                         else:
                             csrate = '{:02d}'.format(srate)
@@ -262,15 +258,15 @@
                                 print('Your file is not RINEX v3 or higher which is I was expecting. Exiting.')
                                 sys.exit()
                             if screenstats: 
                                 print('The RINEX 3 file exists locally', r3)
                             # convert to RINEX 2.11
                             fexists = g.new_rinex3_rinex2(r3,r2,dec_rate)
                             if fexists:
-                                conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
+                                conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,translator)
                             else:
                                 print('Something about the RINEX 3-2 conversion did not work')
                         else:
                             print('You Chose the No Look Option, but did not provide the needed RINEX3 file ', r3)
                             print('I looked for files ending with rnx, rnx.gz, and crx.gz in the local directory')
                             print('I looked for files ending with rnx and crx.gz in $REFL_CODE/YYYY/rinex for your station')
 
@@ -346,78 +342,89 @@
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                                     #subprocess.call(['rm', '-f',rnx_filename]) # rnx
                         # this means the rinex 2 version exists
                         if fexists:
                              if screenstats:
                                  print('RINEX 2 created from v3', year, doy, ' Now remove RINEX 3 files and convert')
                              subprocess.call(['rm', '-f',rnx_filename]) # rnx
-                             conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
+                             conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,translator)
                         else:
                             print('Unsuccessful RINEX 3 retrieval/translation', year, doy)
                     else:
                         print(station, ' year:', year, ' doy:', doy, ' from: ', archive, ' rate:', rate, ' orb:', orbtype)
                         # this is rinex version 2 - finds rinex and converts it
-                        conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
+                        conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,translator)
 
 
-def conv2snr(year, doy, station, option, orbtype,receiverrate,dec_rate,archive,fortran,translator):
+def conv2snr(year, doy, station, option, orbtype,receiverrate,dec_rate,archive,translator):
     """
     convert RINEX files to SNR files
 
+    2024 March 29: change location of logs directory to below REFL_CODE
+
     Parameters
     ----------
     year : int
         full year
-
     doy : int
         day of year
-
     option : int
         snr choice (66, 99 etc)
-
     orbtype : str
         orbit source (nav, gps, gnss, etc)
-
     receiverrate : int
         sampling interval of the GPS receiver, e.g. 1, 30, 15
-
     dec_rate : int
         decimation value to reduce file size
-
     archive : str
         external location (archive) of the rinex files
-
-    fortran : bool
-         whether fortran translator to be used.  this is here for backwards compatability
-
     translator : str
          hybrid, python, or fortran
 
     """
+    xdir = os.environ['REFL_CODE']
+
+    # universal location for the log directory
+    logdir, logname = g.define_logdir(station,year,doy)
+
+    exedir = os.environ['EXE'] # location of executables for fortran people
+
     screenstats = False # for now
-    # define directory for the conversion executables
-    if not os.path.isdir('logs'):
-        subprocess.call(['mkdir', 'logs'])
-    logname = 'logs/' + station + '.txt'
-    log = open(logname, 'w+')
+
+    general_log = logdir + '/' + logname + '.gen'
+    print('Minimal feedback is written to ', general_log)
+    errorlog = logdir + '/' + logname
+
+    log = open(general_log, 'w+')
     log.write("Receiver rate: {0:5s} \n".format(receiverrate))
     log.write("Decimation rate: {0:3.0f} \n".format(dec_rate))
     log.write("Archive: {0:10s} \n".format(archive))
     log.write("Orbits : {0:10s} \n".format(orbtype))
-    exedir = os.environ['EXE']
+    log.write("Translator : {0:10s} \n".format(translator))
     csnr = str(option)
-    cdoy = '{:03d}'.format(doy)
-    cyy = str(year)[2:4]
+    # should be using a function for this
+    cyyyy,cyy,cdoy = g.ydoych(year,doy)
+
     snrname_full =  quickname(station,year,cyy,cdoy,csnr)
-    print('Creating ', snrname_full)
+    log.write("Creating : {0:s} \n".format(snrname_full))
+
     snrname_compressed = ''
 
     # if it exists, you should not have gotten to this code...
     snre = False
     #snrname_full, snrname_compressed, snre = g.define_and_xz_snr(station,year,doy,option)
+
+    # use a local definition of fortran now that we are only using translator variable from
+    # the functions that call conv2snr
+    # 
+    fortran = False
+    if translator == 'fortran':
+        fortran == True
+
+
     if (snre == True):
         log.write("The snrfile already exists: {0:50s} \n".format(snrname_full))
         print("The snrfile already exists: ", snrname_full)
     else:
         log.write("The snrfile does not exist: {0:50s} \n".format(snrname_full))
         d = g.doy2ymd(year,doy);
         month = d.month; day = d.day
@@ -462,15 +469,16 @@
                     subprocess.call([exc, '-O.dec', cdec, rinexfile],stdout=fout)
                     fout.close() # needed?
                     status = subprocess.call(['mv','-f', rinexout, rinexfile])
             # if orbits and rinexfile exist
             if (oexist) and (rexist):
                 snrname = g.snr_name(station, year,month,day,option)
                 orbfile = orbdir + '/' + f
-                #print('translator',translator)
+                # almost everyone uses hybrid. python only is heavily discouraged because
+                # it is too slow. 
                 if translator == 'hybrid':
                     g.make_snrdir(year,station) # make sure output directory exists
                     in1 = g.binary(rinexfile)
                     in2 = g.binary(snrname) # this file is made locally and moved later
                     in3 = g.binary(orbfile)
                     if (len(snrname) > 132) or (len(orbfile) > 132):
                         print('The orbit or SNR file name is too long.')
@@ -479,15 +487,15 @@
                     in4 = g.binary(str(option))
                     if (dec_rate > 0):
                         decr = str(dec_rate)
                     else:
                         decr = '0'
                     in5 = g.binary(decr) # decimation can be used in hybrid option
                     message = 'None '
-                    errorlog = 'logs/' + station + '_hybrid_error.txt'
+
                     in6 = g.binary(errorlog)
                     log.write('SNR file {0:50s} \n will use hybrid of python and fortran to make \n'.format( snrname))
                     # these are calls to the fortran codes that have been ported to be called from python
                     if (orbtype  == 'gps') or ('nav' in orbtype):
                         gpssnr.foo(in1,in2,in3,in4,in5,in6)
                     else:
                         if orbtype in ['ultra', 'wum', 'wum2']:
@@ -497,32 +505,30 @@
                             gnsssnr.foo(in1,in2,in3,in4,in5,in6)
                 else:
                     if (translator == 'fortran'):
                         t1=time.time()
                         try:
                             #subprocess.call([snrexe, rinexfile, snrname, orbfile, str(option)])
                             log.write('Using standalone fortran for translation  - separate log is used for stdout \n')
-                            flogname = 'logs/' + station + '_fortran.txt'
+                            flogname = errorlog
+
                             flog = open(flogname, 'w+')
                             a=subprocess.run([snrexe, rinexfile, snrname, orbfile, str(option)],capture_output=True,text=True)
                             ddd = a.stdout; flog.write(ddd); flog.close()
                             status = subprocess.call(['rm','-f', rinexfile ])
                             status = subprocess.call(['xz', orbfile])
                         except:
-                            log.write('Problem with making SNR file, check fortran specific log {0:50s} \n'.format(flogname))
+                            log.write('Problem with making SNR file, check log {0:50s} \n'.format(flogname))
                         t2=time.time()
-#                        print(' Exec time:', '{0:4.2f}'.format(t2-t1) )
-#                      this is for people that want to use slow python code
                     else:
                         log.write('SNR file {0:50s} \n will use python to make \n'.format( snrname))
                         log.write('Decimating will be done here instead of using teqc \n')
                         t1=time.time()
                         rnx2snr(rinexfile, orbfile,snrname,option,year,month,day,dec_rate,log)
                         t2=time.time()
-#                        print(' Exec time:', '{0:4.2f}'.format(t2-t1) )
 
                 # remove the rinex file
                 subprocess.call(['rm', '-f',rinexfile])
 
                 if os.path.isfile(snrname):
 #                make sure it exists and is non-zero size before moving it
                     if (os.stat(snrname).st_size == 0):
@@ -533,23 +539,23 @@
                         log.write('A SNR file was created : {0:50s}  \n'.format(snrname_full))
                         print('\n')
                         print('SUCCESS: SNR file was created \n', snrname_full)
                         g.store_snrfile(snrname,year,station)
                         subprocess.call(['gzip', snrname_full])
 
                 else:
-                    logfile = 'logs/' + station + '_hybrid_error.txt'
-                    print('No SNR file created - check ', logfile, ' for why it failed.')
+                    # not sure why this is made here??? wasn't it created earlier?
+                    print('No SNR file created - check ', errorlog, ' or ')
+                    print( general_log , ' for why it failed.')
             else:
                 print('Either the RINEX file or orbit file does not exist, so there is nothing to convert')
                 log.write('Either the RINEX file or orbit file does not exist, so there is nothing to convert \n')
         else:
             print('The orbit file you requested does not exist.')
 
-    # close the log file
     log.close()
 
     return True
 
 def satorb(week, sec_of_week, ephem):
     """
     Calculate GPS satellite orbits
```

### Comparing `gnssrefl-3.1.4/gnssrefl/rinex2snr_cl.py` & `gnssrefl-3.1.5/gnssrefl/rinex2snr_cl.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     parser.add_argument("-snr", default=None, help="snr file ending, 99: 5-30 deg.; 66: < 30 deg.; 88: all data; 50: < 10 deg.", type=int)
     parser.add_argument("-orb", default=None, type=str,
                         help="orbit type, e.g. gps, gps+glo, gnss, rapid, ultra, gnss3")
     parser.add_argument("-rate", default=None, metavar='low', type=str, help="low or high (tells code which folder to search).  If samplerate is 1, this is set automatically to high.") 
     parser.add_argument("-dec", default=None, type=int, help="decimate (seconds)")
     parser.add_argument("-nolook", default=None, metavar='False', type=str,
                         help="True means only use RINEX files on local machine")
-    parser.add_argument("-fortran", default=None, metavar='False', type=str,
-                        help="True means use Fortran RINEX translators ")
+    # remove fortran as an option
+    #parser.add_argument("-fortran", default=None, metavar='False', type=str,
+    #                    help="True means use Fortran RINEX translators ")
     parser.add_argument("-archive", default=None, metavar='all',
                         help="specify archive", type=str)
     parser.add_argument("-doy_end", default=None, help="end day of year", type=int)
     parser.add_argument("-year_end", default=None, help="end year", type=int)
     parser.add_argument("-overwrite", default=None, help="boolean", type=str)
     parser.add_argument("-translator", default=None, help="translator(fortran,hybrid,python)", type=str)
     parser.add_argument("-samplerate", default=None, help="sample rate in sec (RINEX 3 only)", type=int)
@@ -57,23 +58,23 @@
     parser.add_argument("-screenstats", default=None, help="set to T see more info printed to screen", type=str)
     parser.add_argument("-gzip", default=None, help="boolean, default is SNR files are gzipped after creation", type=str)
     parser.add_argument("-par", default=None, help="parallel processes allowed", type=int)
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['nolook', 'fortran', 'overwrite', 'mk', 'weekly','strip','screenstats','gzip','monthly']
+    boolean_args = ['nolook', 'overwrite', 'mk', 'weekly','strip','screenstats','gzip','monthly']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def rinex2snr(station: str, year: int, doy: int, snr: int = 66, orb: str = None, rate: str = 'low', dec: int = 0,
-              fortran: bool = False, nolook: bool = False, archive: str = 'all', doy_end: int = None,
+              nolook: bool = False, archive: str = 'all', doy_end: int = None,
               year_end: int = None, overwrite: bool = False, translator: str = 'hybrid', samplerate: int = 30,
               stream: str = 'R', mk: bool = False, weekly: bool = False, strip: bool = False, 
               screenstats : bool = False, gzip : bool = True, monthly : bool = False, par : int=None ):
     """
     rinex2snr translates RINEX files to a new file in SNR format. This function will also fetch orbit files for you.
     RINEX obs files are provided by the user or fetched from a long list of archives. Although RINEX 3 is supported, 
     the default is RINEX 2.11 files
@@ -237,17 +238,14 @@
             low (default) : standard rate data. Usually 30 sec, but sometimes 15 sec.
 
             high : high-rate data
 
     dec : int, optional
         Decimation rate. 0 is default.
 
-    fortran : bool, optional
-        Whether to use fortran to translate the rinex files. 
-
     nolook : bool, optional
         tells the code to retrieve RINEX files from your local machine. default is False
 
     archive : str, optional
         Select which archive to get the files from. Default is all
         value options:
 
@@ -298,15 +296,15 @@
     overwrite : bool, optional
         Make a new SNR file even if one already exists (overwrite existing file).
         Default is False.
 
     translator : str, optional
         hybrid (default) : uses a combination of python and fortran to translate the files.
 
-        fortran : uses fortran to translate (requires the fortran translator executable)
+        fortran : uses fortran to translate (requires the fortran translator executable to exist)
 
         python : uses python to translate. (Warning: This can be very slow)
 
     srate : int, optional
         sample rate for RINEX 3 files only. Default is 30.
 
     mk : bool, optional
@@ -335,14 +333,15 @@
     monthly : bool, optional
         default is false. snr files created every 30 days instead of every day
 
     par : int, optional
         default is NOne.  parallel processing, valid up to 10
 
     """
+
     archive_list_rinex3 = ['unavco', 'epn','cddis', 'bev', 'bkg', 'ga', 'epn', 'bfg','sonel','all','unavco2','nrcan','gfz','ignes']
     archive_list = ['sopac', 'unavco', 'sonel',  'nz', 'ga', 'bkg', 'jeff',
                     'ngs', 'nrcan', 'special', 'bev', 'jp', 'all','unavco2','cddis']
 
     archive_list_no_parallel = ['sopac','cddis','jeff']
 
     if False:
@@ -357,15 +356,17 @@
     #
     if doy_end is None:
         doy_end = doy
     if year_end is None:
         year_end = year
 
     # make sure directories are there for orbit files and snr files
+    # and for logs
     for y in range(year, year_end+1):
+        tmp1, tmp2 = g.define_logdir(station,y,1)
         ann = g.make_nav_dirs(y)
         f1 = xdir + '/' + str(y) + '/snr/' + station[0:4]
         if not os.path.isdir(f1):
             print('make output directory for snr files in ', y)
             subprocess.call(['mkdir','-p',f1])
 
     # when multi-GNSS orbits are reliably available
@@ -428,51 +429,36 @@
             print('found GFZ orbits at IGN - warning, only a single file at a time')
 
     # if you choose GPS+GLO, you get the JAXA sp3 file 
     if orb == 'gps+glo':
         orb = 'jax'
 
     # default is to use hybrid for RINEX translator - UNLESS You chose fortran
-    if translator is None:
-        # the case when someone sets fortran to true and doesn't set translator also
-        # but i do not think this happens because Kelly has made hybrid the default
-        if fortran:
-            translator = 'fortran'
-        else:
-            translator = 'hybrid'
-    elif translator == 'hybrid':
-        # override
-        if fortran:
-            translator = 'fortran'     
-    elif translator == 'python':
-        fortran = False  
-    elif translator == 'fortran':
-        fortran = True
-    translator_accepted = [None, 'fortran', 'hybrid', 'python']
+
+    # these are currently accepted
+    translator_accepted = ['fortran', 'hybrid', 'python']
     if translator not in translator_accepted:
         print(f'translator option must be one of {translator_accepted}. Exiting.')
         sys.exit()
 
     # check that the fortran exe exist
-    if fortran:
+    if translator == 'fortran':
         if orb == 'nav':
             snrexe = g.gpsSNR_version()
             if not os.path.isfile(snrexe):
                 print('You have selected the fortran and GPS only options.')
-                print('However, the fortran translator gpsSNR.e has not been properly installed.')
+                print('However, the fortran translator gpsSNR.e does not exist.')
                 print('We are changing your choice to the hybrid translator option.')
-                fortran = False
                 translator = 'hybrid'
         else:
             snrexe = g.gnssSNR_version()
             if not os.path.isfile(snrexe):
                 print('You have selected the fortran and GNSS options.')
                 print('However, the fortran translator gnssSNR.e has not been properly installed.')
                 print('We are changing your choice to hybrid option.')
-                fortran = False
                 translator = 'hybrid'
 
     rate = rate.lower()
     # default is set to low.  set to high for 1sec files so the user doesn't have to
     if samplerate == 1:
         rate = 'high'
     rate_accepted = ['low', 'high']
@@ -544,28 +530,28 @@
     if mk:
         print('You have invoked the Makan option')
 
     if stream not in ['R', 'S']:
         stream = 'R'
 
     args = {'station': station, 'year':year, 'doy':doy, 'isnr': snr, 'orbtype': orb, 'rate': rate, 
-            'dec_rate': dec, 'archive': archive, 'fortran': fortran, 'nol': nolook, 'overwrite': overwrite, 
+            'dec_rate': dec, 'archive': archive, 'nol': nolook, 'overwrite': overwrite, 
             'translator': translator, 'srate': samplerate, 'mk': mk, 'stream': stream, 
             'strip': strip, 'bkg': bkg, 'screenstats': screenstats, 'gzip' : gzip}
     MJD1 = int(g.ydoy2mjd(year,doy))
     MJD2 = int(g.ydoy2mjd(year_end,doy_end))
 
 
     # queue which handles any exceptions any of the processes encounter
     manager = multiprocessing.Manager()
     error_queue = manager.Queue()
 
 
     if MJD1 == MJD2:
-        print('requested parallel processing, but only asked for one day of analysis')
+        print('Only one day being analyzed, parallel processing turned off')
         par = None
     if archive in archive_list_no_parallel:
         print('You have chosen an archive that is unfriendly to multiple simultaneous download')
         print('requests. Your request for parallel processing has been declined.')
         par = None
 
     if not par:
@@ -630,15 +616,15 @@
         for mjd in mjd_list:
             y, d = g.modjul_to_ydoy(mjd)
             args['year'] = y
             args['doy'] = d
             rnx.run_rinex2snr(**args)
 
     except Exception as e:
-        print(y, d)
+        print('Error of some kind processing year/doy ', y, d)
         error_queue.put(e)
 
     return
 
 def process_jobs(mjd_list, args):
     """
     this is not being used - calls should be sent to function above instead
```

### Comparing `gnssrefl-3.1.4/gnssrefl/rinex3_rinex2.py` & `gnssrefl-3.1.5/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rinex3_snr.py` & `gnssrefl-3.1.5/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rinex_coords.py` & `gnssrefl-3.1.5/gnssrefl/rinex_coords.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rinpy.py` & `gnssrefl-3.1.5/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-3.1.5/gnssrefl/rt_rinex3_snr.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     year = rinex3[12:16]
     iyear = int(year)
     cdoy = rinex3[16:19] 
     idoy = int(cdoy)
     iyear,month,day=g.ydoy2ymd(iyear, idoy)
 
+    maindir = os.environ['REFL_CODE']
     # where rinex data are
     xdir = os.environ['REFL_CODE'] + '/rinex/' + STATION + '/' + year + '/'
     # where snr data will go
     snrdir =  os.environ['REFL_CODE'] + '/' + year + '/snr/' + STATION + '/'
     print(xdir)
 
 
@@ -100,15 +101,15 @@
     in4 = g.binary(str(option))
     if (dec_rate > 0):
         decr = str(dec_rate)
     else:
         decr = '0'
     in5 = g.binary(decr) # decimation can be used in hybrid option
     message = 'None '
-    errorlog = 'logs/' + station + '_hybrid_error.txt'
+    errorlog = maindir + '/logs/' + station + '_hybrid_error.txt'
     in6 = g.binary(errorlog)
     gnsssnrbigger.foo(in1,in2,in3,in4,in5,in6)
     # clean up - remove the rinex2 file
     print('Output file written to: ', snrname)
     subprocess.call(['rm','-f',rinex2])
 
 if __name__ == "__main__":
```

### Comparing `gnssrefl-3.1.4/gnssrefl/sd_libs.py` & `gnssrefl-3.1.5/gnssrefl/sd_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/smoosh.py` & `gnssrefl-3.1.5/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/smoosh_snr.py` & `gnssrefl-3.1.5/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/snow_functions.py` & `gnssrefl-3.1.5/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/snowdepth_cl.py` & `gnssrefl-3.1.5/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/spline_functions.py` & `gnssrefl-3.1.5/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/subdaily.py` & `gnssrefl-3.1.5/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/subdaily_cl.py` & `gnssrefl-3.1.5/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/utils.py` & `gnssrefl-3.1.5/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/veg_multiyr.py` & `gnssrefl-3.1.5/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/vwc_cl.py` & `gnssrefl-3.1.5/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/vwc_input.py` & `gnssrefl-3.1.5/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/xnmeasnr.f` & `gnssrefl-3.1.5/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/xyz2llh.py` & `gnssrefl-3.1.5/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/ydoy.py` & `gnssrefl-3.1.5/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl/ymd.py` & `gnssrefl-3.1.5/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-3.1.5/gnssrefl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 3.1.4
+Version: 3.1.5
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# gnssrefl v3.1.4 
+# gnssrefl v3.1.5 
+
+If you use this code in any presentation or publication, you are expected to cite either 
+this github repository or the gnssrefl DOI, which is given just below.
 
 [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) 
 
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601494.svg)](http://dx.doi.org/10.5281/zenodo.5601494) 
 
 
 gnssrefl is an open source software package for GNSS interferometric reflectometry (GNSS-IR). 
 
 ![](docs/myAnimation.gif)
 
+I made this animation ages ago - so it is in Matlab.  I would be happy to host a link to 
+a version in python.  The main code is [snr_simulation](docs/pages/snr_simulation.m) 
+and the helper function is [setFrame.m](docs/pages/set_Frame.m). 
 
 Documentation:
 
 - [online](https://gnssrefl.readthedocs.io/en/latest/)
 
 - [pdf](https://gnssrefl.readthedocs.io/_/downloads/en/latest/pdf/)
```

### Comparing `gnssrefl-3.1.4/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-3.1.5/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-3.1.5/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/pyproject.toml` & `gnssrefl-3.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-3.1.4/setup.py` & `gnssrefl-3.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "simplekml",
     "earthscope-sdk",
     "jupyterlab",
     "ipywidgets"
 ]
 setup(
     name="gnssrefl",
-    version="3.1.4",
+    version="3.1.5",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-3.1.4/test/test_gps.py` & `gnssrefl-3.1.5/test/test_gps.py`

 * *Files identical despite different names*

