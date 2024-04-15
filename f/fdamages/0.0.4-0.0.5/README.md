# Comparing `tmp/fdamages-0.0.4.tar.gz` & `tmp/fdamages-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdamages-0.0.4.tar", last modified: Fri Apr 12 09:42:34 2024, max compression
+gzip compressed data, was "fdamages-0.0.5.tar", last modified: Mon Apr 15 07:51:15 2024, max compression
```

## Comparing `fdamages-0.0.4.tar` & `fdamages-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.360581 fdamages-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      469 2024-04-12 09:42:34.360077 fdamages-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 09:42:34.360581 fdamages-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      844 2024-04-12 09:42:32.000000 fdamages-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.350511 fdamages-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.354021 fdamages-0.0.4/src/fdamages/
--rw-rw-rw-   0        0        0       41 2024-04-12 09:42:30.000000 fdamages-0.0.4/src/fdamages/__init__.py
--rw-rw-rw-   0        0        0     1968 2024-04-12 08:29:52.000000 fdamages-0.0.4/src/fdamages/module_fdamage.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.359027 fdamages-0.0.4/src/fdamages.egg-info/
--rw-rw-rw-   0        0        0      469 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 07:51:15.574733 fdamages-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-04-15 07:51:15.573605 fdamages-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:51:15.574733 fdamages-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      846 2024-04-15 07:51:13.000000 fdamages-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:51:15.565088 fdamages-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 07:51:15.568599 fdamages-0.0.5/src/fdamages/
+-rw-rw-rw-   0        0        0       41 2024-04-12 09:42:30.000000 fdamages-0.0.5/src/fdamages/__init__.py
+-rw-rw-rw-   0        0        0     2298 2024-04-15 07:49:56.000000 fdamages-0.0.5/src/fdamages/module_fdamage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:51:15.572604 fdamages-0.0.5/src/fdamages.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-15 07:51:15.000000 fdamages-0.0.5/src/fdamages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-15 07:51:15.000000 fdamages-0.0.5/src/fdamages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:51:15.000000 fdamages-0.0.5/src/fdamages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 07:51:15.000000 fdamages-0.0.5/src/fdamages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 07:51:15.000000 fdamages-0.0.5/src/fdamages.egg-info/top_level.txt
```

### Comparing `fdamages-0.0.4/LICENSE` & `fdamages-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fdamages-0.0.4/setup.py` & `fdamages-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 PACKAGE_NAME = "fdamages"
 AUTHOR = "Valerio Luzzi"
 EMAIL = "valerio.luzzi@gecosistema.com"
 GITHUB = f"https://github.com/valluzzi/{PACKAGE_NAME}.git"
 DESCRIPTION = "A fdamage utility for reading damage functions"
 
 setup(
@@ -31,12 +31,13 @@
 
 
 
 
 
 
 
+
```

### Comparing `fdamages-0.0.4/src/fdamages/module_fdamage.py` & `fdamages-0.0.5/src/fdamages/module_fdamage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import boto3
 from botocore.response import StreamingBody
 
 # fdamage text format
 f_example = """wd,dmg #header is optional
 #0,0.0
 0.5,0.25
 1,0.4
@@ -33,14 +34,18 @@
 
 def normalize_text(text):
     """
     Normalize text
     """
     if text is None:
         text = ""
+    elif isinstance(text, str) and text.startswith("s3://"):
+        s3 = boto3.client('s3')
+        bucket, key = text.split('s3://')[1].split('/', 1)
+        text = normalize_text(s3.get_object(Bucket=bucket, Key=key))
     elif isinstance(text, str):
         text = text.replace('\r\n', '\n').replace('\r', '\n')
     elif isinstance(text, bytes):
         text = normalize_text(text.decode('utf-8'))
     elif isinstance(text, StreamingBody):
         text = normalize_text(text.read())
     elif isinstance(text, dict) and "Body" in text:
@@ -76,9 +81,12 @@
         res.insert(0, (0,0))
 
     return res
 
 
 if __name__ == '__main__':
     text = f_example
-    arr = parse_fdamage(text)
-    print(arr) 
+    #arr = parse_fdamage(text)
+    
+    arr = parse_fdamage("s3://saferplaces.co/fdamage/shared/residential.csv")
+    
+    print(arr)
```

