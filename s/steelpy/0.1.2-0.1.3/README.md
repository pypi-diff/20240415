# Comparing `tmp/steelpy-0.1.2.tar.gz` & `tmp/steelpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelpy-0.1.2.tar", max compression
+gzip compressed data, was "steelpy-0.1.3.tar", max compression
```

## Comparing `steelpy-0.1.2.tar` & `steelpy-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      376 2024-04-15 00:07:39.229557 steelpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-0.1.2/README.md
--rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-0.1.2/steelpy/__init__.py
--rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-0.1.2/steelpy/shape files/.DS_Store
--rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-0.1.2/steelpy/shape files/C_shapes.xlsx
--rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-0.1.2/steelpy/shape files/DBL_L_shapes.xlsx
--rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-0.1.2/steelpy/shape files/HP_shapes.xlsx
--rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-0.1.2/steelpy/shape files/HSS_R_shapes.xlsx
--rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-0.1.2/steelpy/shape files/HSS_shapes.xlsx
--rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-0.1.2/steelpy/shape files/L_shapes.xlsx
--rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-0.1.2/steelpy/shape files/M_shapes.xlsx
--rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-0.1.2/steelpy/shape files/MC_shapes.xlsx
--rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-0.1.2/steelpy/shape files/MT_shapes.xlsx
--rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-0.1.2/steelpy/shape files/PIPE_shapes.xlsx
--rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-0.1.2/steelpy/shape files/S_shapes.xlsx
--rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-0.1.2/steelpy/shape files/ST_shapes.xlsx
--rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-0.1.2/steelpy/shape files/W_shapes.xlsx
--rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-0.1.2/steelpy/shape files/WT_shapes.xlsx
--rw-r--r--   0        0        0     1829 2024-04-15 00:07:31.541137 steelpy-0.1.2/steelpy/steelpy.py
--rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 steelpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-0.1.3/license.txt
+-rw-r--r--   0        0        0      376 2024-04-15 00:15:57.617540 steelpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-0.1.3/README.md
+-rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-0.1.3/steelpy/__init__.py
+-rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-0.1.3/steelpy/shape files/.DS_Store
+-rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-0.1.3/steelpy/shape files/C_shapes.xlsx
+-rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-0.1.3/steelpy/shape files/DBL_L_shapes.xlsx
+-rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-0.1.3/steelpy/shape files/HP_shapes.xlsx
+-rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-0.1.3/steelpy/shape files/HSS_R_shapes.xlsx
+-rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-0.1.3/steelpy/shape files/HSS_shapes.xlsx
+-rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-0.1.3/steelpy/shape files/L_shapes.xlsx
+-rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-0.1.3/steelpy/shape files/M_shapes.xlsx
+-rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-0.1.3/steelpy/shape files/MC_shapes.xlsx
+-rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-0.1.3/steelpy/shape files/MT_shapes.xlsx
+-rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-0.1.3/steelpy/shape files/PIPE_shapes.xlsx
+-rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-0.1.3/steelpy/shape files/S_shapes.xlsx
+-rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-0.1.3/steelpy/shape files/ST_shapes.xlsx
+-rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-0.1.3/steelpy/shape files/W_shapes.xlsx
+-rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-0.1.3/steelpy/shape files/WT_shapes.xlsx
+-rw-r--r--   0        0        0     1829 2024-04-15 00:07:31.541137 steelpy-0.1.3/steelpy/steelpy.py
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 steelpy-0.1.3/PKG-INFO
```

### Comparing `steelpy-0.1.2/README.md` & `steelpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/.DS_Store` & `steelpy-0.1.3/steelpy/shape files/.DS_Store`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/C_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/C_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/DBL_L_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/DBL_L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/HP_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/HP_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/HSS_R_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/HSS_R_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/HSS_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/HSS_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/L_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/M_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/M_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/MC_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/MC_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/MT_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/MT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/PIPE_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/PIPE_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/S_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/S_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/ST_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/ST_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/W_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/W_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/shape files/WT_shapes.xlsx` & `steelpy-0.1.3/steelpy/shape files/WT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/steelpy/steelpy.py` & `steelpy-0.1.3/steelpy/steelpy.py`

 * *Files identical despite different names*

### Comparing `steelpy-0.1.2/PKG-INFO` & `steelpy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steelpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple library for section properties of AISC steel shapes
 Author: evanfaler
 Author-email: emfaler@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```

