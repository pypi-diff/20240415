# Comparing `tmp/LimeNDAdecoder-1.2.7.tar.gz` & `tmp/limendadecoder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LimeNDAdecoder-1.2.7.tar", last modified: Thu Feb  1 07:11:00 2024, max compression
+gzip compressed data, was "limendadecoder-1.3.0.tar", last modified: Mon Apr 15 09:59:18 2024, max compression
```

## Comparing `LimeNDAdecoder-1.2.7.tar` & `limendadecoder-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 07:11:00.216386 LimeNDAdecoder-1.2.7/
--rw-rw-rw-   0        0        0     1980 2024-02-01 07:11:00.211616 LimeNDAdecoder-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1390 2023-07-14 06:40:04.000000 LimeNDAdecoder-1.2.7/README.md
--rw-rw-rw-   0        0        0      728 2024-01-09 13:08:33.000000 LimeNDAdecoder-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-01 07:11:00.217383 LimeNDAdecoder-1.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-01 07:11:00.130632 LimeNDAdecoder-1.2.7/src/
-drwxrwxrwx   0        0        0        0 2024-02-01 07:11:00.158550 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/
--rw-rw-rw-   0        0        0      347 2023-12-27 10:04:49.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/__init__.py
--rw-rw-rw-   0        0        0    25278 2023-12-27 10:05:38.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/nda_functions.py
--rw-rw-rw-   0        0        0    15318 2024-01-09 12:59:17.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/nda_version_8_0.py
-drwxrwxrwx   0        0        0        0 2024-02-01 07:11:00.206613 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/
--rw-rw-rw-   0        0        0     1980 2024-02-01 07:11:00.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-02-01 07:11:00.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 07:11:00.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-02-01 07:11:00.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-01 07:11:00.000000 LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 09:59:18.163087 limendadecoder-1.3.0/
+-rw-rw-rw-   0        0        0     1980 2024-04-15 09:59:18.158087 limendadecoder-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1390 2023-07-14 06:40:04.000000 limendadecoder-1.3.0/README.md
+-rw-rw-rw-   0        0        0      728 2024-04-15 09:25:49.000000 limendadecoder-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:59:18.165076 limendadecoder-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 09:59:18.071878 limendadecoder-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 09:59:18.108064 limendadecoder-1.3.0/src/LimeNDAdecoder/
+-rw-rw-rw-   0        0        0      347 2023-12-27 10:04:49.000000 limendadecoder-1.3.0/src/LimeNDAdecoder/__init__.py
+-rw-rw-rw-   0        0        0    26021 2024-04-15 07:12:23.000000 limendadecoder-1.3.0/src/LimeNDAdecoder/nda_functions.py
+-rw-rw-rw-   0        0        0    15890 2024-04-15 07:15:00.000000 limendadecoder-1.3.0/src/LimeNDAdecoder/nda_version_8_0.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:59:18.154197 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/
+-rw-rw-rw-   0        0        0     1980 2024-04-15 09:59:18.000000 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-04-15 09:59:18.000000 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:59:18.000000 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-15 09:59:18.000000 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 09:59:18.000000 limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/top_level.txt
```

### Comparing `LimeNDAdecoder-1.2.7/PKG-INFO` & `limendadecoder-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LimeNDAdecoder
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime AI Celltesting <celltesting@lime.ai>
 Project-URL: Homepage, https://github.com/limeaicell/LimeNDAdecoder
 Project-URL: Bug Tracker, https://github.com/limeaicell/LimeNDAdecoder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `LimeNDAdecoder-1.2.7/README.md` & `limendadecoder-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `LimeNDAdecoder-1.2.7/pyproject.toml` & `limendadecoder-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy","pandas","xlsxwriter"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LimeNDAdecoder"
-version = "1.2.7"
+version = "1.3.0"
 authors = [
   { name="Lime AI Celltesting", email="celltesting@lime.ai" },
 ]
 description = 'Python Package for working with NDA files, specifically for people at Lime.AI' 
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/nda_functions.py` & `limendadecoder-1.3.0/src/LimeNDAdecoder/nda_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,36 +86,66 @@
     """
     ## Parameters
 
     #### nda
         Path to the nda file.\n
     ----------
     ----------
-    returns barcode entered during the test for the passed nda file
+    Returns barcode entered during the test for the passed nda file
     """
     if nda.split(".")[-1] != "nda":
         raise ValueError("File passed in function is not an nda file")
     return nda_version_8_0.get_barcode(nda)
 
 
+def get_channel_number(nda):
+    """
+    ## Parameters
+
+    #### nda
+        Path to the nda file.\n
+    ----------
+    ----------
+    Returns channel number for the nda file
+    """
+    if nda.split(".")[-1] != "nda":
+        raise ValueError("File passed in function is not an nda file")
+    return nda_version_8_0.get_channel(nda)
+
+def get_end_time(nda):
+    """
+    ## Parameters
+
+    #### nda
+        Path to the nda file.\n
+    ----------
+    ----------
+    Returns the end time for the passed nda file. If it isn't available, it returns "N/A"
+    """
+    if nda.split(".")[-1] != "nda":
+        raise ValueError("File passed in function is not an nda file")
+    return nda_version_8_0.get_end_time(nda)
+
 def get_start_time(nda):
     """
     ## Parameters
 
     #### nda
         Path to the nda file.\n
     ----------
     ----------
-    returns start time for the passed nda file
+    Returns start time for the passed nda file
     """
     if nda.split(".")[-1] != "nda":
         raise ValueError("File passed in function is not an nda file")
     return nda_version_8_0.get_st_time(nda)
 
 
+
+
 def get_process_name(nda):
     """
     ## Parameters
 
     #### nda
         Path to the nda file.\n
     ----------
```

### Comparing `LimeNDAdecoder-1.2.7/src/LimeNDAdecoder/nda_version_8_0.py` & `limendadecoder-1.3.0/src/LimeNDAdecoder/nda_version_8_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,32 @@
             if data[i : i + 1] == b"\x00":
                 t = i
                 break
         remarks = data[x8 - 376 : t]
     return remarks.decode()
 
 
+def get_channel(inpath):
+    with open(inpath, "rb") as f:
+        data = f.read()
+        pos = data.find(b"BTS Client")
+        [dev_id, unit_id, ch_id] = struct.unpack("<bbb", data[pos - 603 : pos - 600])
+    return str(dev_id) + "-" + str(unit_id) + "-" + str(ch_id)
+
+
+def get_end_time(inpath):
+    with open(inpath, "rb") as f:
+        data = f.read()
+        pos = data.find(b"BTS Client")
+        if data[pos - 546 : pos - 545] == b"\x00":
+            return "N/A"
+        end_time = data[pos - 546 : pos - 527].decode()
+        return end_time
+
+
 def ValidFile(inpath):
     with open(inpath, "rb") as f:
         data = f.read()
         pos = data.find(b"BTS Client")
         if pos == -1:
             return False
         else:
```

### Comparing `LimeNDAdecoder-1.2.7/src/LimeNDAdecoder.egg-info/PKG-INFO` & `limendadecoder-1.3.0/src/LimeNDAdecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LimeNDAdecoder
-Version: 1.2.7
+Version: 1.3.0
 Summary: Python Package for working with NDA files, specifically for people at Lime.AI
 Author-email: Lime AI Celltesting <celltesting@lime.ai>
 Project-URL: Homepage, https://github.com/limeaicell/LimeNDAdecoder
 Project-URL: Bug Tracker, https://github.com/limeaicell/LimeNDAdecoder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

