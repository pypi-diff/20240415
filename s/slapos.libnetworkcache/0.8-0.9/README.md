# Comparing `tmp/slapos.libnetworkcache-0.8.tar.gz` & `tmp/slapos.libnetworkcache-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slapos.libnetworkcache-0.8.tar", last modified: Fri Sep  2 09:27:08 2011, max compression
+gzip compressed data, was "dist/slapos.libnetworkcache-0.9.tar", last modified: Fri Sep  2 12:33:42 2011, max compression
```

## Comparing `slapos.libnetworkcache-0.8.tar` & `slapos.libnetworkcache-0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/
-drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos/
--rw-r--r--   0 luke      (1000) users      (100)    30482 2011-09-02 08:38:43.000000 slapos.libnetworkcache-0.8/slapos/libnetworkcachetests.py
--rw-r--r--   0 luke      (1000) users      (100)     1818 2011-09-02 08:54:01.000000 slapos.libnetworkcache-0.8/slapos/signature.py
--rw-r--r--   0 luke      (1000) users      (100)     9077 2011-08-31 13:02:31.000000 slapos.libnetworkcache-0.8/slapos/separatedssltestserver.py
--rw-r--r--   0 luke      (1000) users      (100)      244 2011-07-18 08:34:58.000000 slapos.libnetworkcache-0.8/slapos/__init__.py
--rw-r--r--   0 luke      (1000) users      (100)    10517 2011-09-02 09:25:26.000000 slapos.libnetworkcache-0.8/slapos/libnetworkcache.py
--rw-r--r--   0 luke      (1000) users      (100)     1273 2011-09-02 09:26:31.000000 slapos.libnetworkcache-0.8/CHANGES.txt
--rw-r--r--   0 luke      (1000) users      (100)     1321 2011-09-02 09:26:31.000000 slapos.libnetworkcache-0.8/setup.py
--rw-r--r--   0 luke      (1000) users      (100)       20 2011-07-18 08:34:58.000000 slapos.libnetworkcache-0.8/MANIFEST.in
-drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/
--rw-r--r--   0 luke      (1000) users      (100)        7 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/top_level.txt
--rw-r--r--   0 luke      (1000) users      (100)       65 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/entry_points.txt
--rw-r--r--   0 luke      (1000) users      (100)        1 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/dependency_links.txt
--rw-r--r--   0 luke      (1000) users      (100)      546 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/SOURCES.txt
--rw-r--r--   0 luke      (1000) users      (100)        1 2011-08-03 13:38:42.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/zip-safe
--rw-r--r--   0 luke      (1000) users      (100)        7 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/namespace_packages.txt
--rw-r--r--   0 luke      (1000) users      (100)       10 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/requires.txt
--rw-r--r--   0 luke      (1000) users      (100)     2842 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/PKG-INFO
--rw-r--r--   0 luke      (1000) users      (100)       59 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/setup.cfg
--rw-r--r--   0 luke      (1000) users      (100)     2842 2011-09-02 09:27:08.000000 slapos.libnetworkcache-0.8/PKG-INFO
--rw-r--r--   0 luke      (1000) users      (100)      513 2011-08-25 13:26:17.000000 slapos.libnetworkcache-0.8/README.txt
+drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/
+drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos/
+-rw-r--r--   0 luke      (1000) users      (100)    33313 2011-09-02 12:30:38.000000 slapos.libnetworkcache-0.9/slapos/libnetworkcachetests.py
+-rw-r--r--   0 luke      (1000) users      (100)     1818 2011-09-02 08:54:01.000000 slapos.libnetworkcache-0.9/slapos/signature.py
+-rw-r--r--   0 luke      (1000) users      (100)     9077 2011-08-31 13:02:31.000000 slapos.libnetworkcache-0.9/slapos/separatedssltestserver.py
+-rw-r--r--   0 luke      (1000) users      (100)      244 2011-07-18 08:34:58.000000 slapos.libnetworkcache-0.9/slapos/__init__.py
+-rw-r--r--   0 luke      (1000) users      (100)    11017 2011-09-02 12:26:35.000000 slapos.libnetworkcache-0.9/slapos/libnetworkcache.py
+-rw-r--r--   0 luke      (1000) users      (100)     1367 2011-09-02 12:32:19.000000 slapos.libnetworkcache-0.9/CHANGES.txt
+-rw-r--r--   0 luke      (1000) users      (100)     1321 2011-09-02 12:32:20.000000 slapos.libnetworkcache-0.9/setup.py
+-rw-r--r--   0 luke      (1000) users      (100)       20 2011-07-18 08:34:58.000000 slapos.libnetworkcache-0.9/MANIFEST.in
+drwxr-xr-x   0 luke      (1000) users      (100)        0 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/
+-rw-r--r--   0 luke      (1000) users      (100)        7 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/top_level.txt
+-rw-r--r--   0 luke      (1000) users      (100)       65 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/entry_points.txt
+-rw-r--r--   0 luke      (1000) users      (100)        1 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/dependency_links.txt
+-rw-r--r--   0 luke      (1000) users      (100)      546 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/SOURCES.txt
+-rw-r--r--   0 luke      (1000) users      (100)        1 2011-08-03 13:38:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/zip-safe
+-rw-r--r--   0 luke      (1000) users      (100)        7 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/namespace_packages.txt
+-rw-r--r--   0 luke      (1000) users      (100)       10 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/requires.txt
+-rw-r--r--   0 luke      (1000) users      (100)     2976 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/PKG-INFO
+-rw-r--r--   0 luke      (1000) users      (100)       59 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/setup.cfg
+-rw-r--r--   0 luke      (1000) users      (100)     2976 2011-09-02 12:33:42.000000 slapos.libnetworkcache-0.9/PKG-INFO
+-rw-r--r--   0 luke      (1000) users      (100)      513 2011-08-25 13:26:17.000000 slapos.libnetworkcache-0.9/README.txt
```

### Comparing `slapos.libnetworkcache-0.8/slapos/libnetworkcachetests.py` & `slapos.libnetworkcache-0.9/slapos/libnetworkcachetests.py`

 * *Files 2% similar despite different names*

```diff
@@ -554,14 +554,93 @@
     open(f, 'w').write(json.dumps([]))
     try:
       nc.select(key)
     except slapos.libnetworkcache.DirectoryNotFound, msg:
       # empty content in shadir so usual exception is raised
       self.assertEqual(str(msg), 'Could not find a trustable entry.')
 
+  def test_select_no_json_response(self):
+    key = 'somekey' + str(random.random())
+    urlmd5 = str(random.random())
+    file_name = 'my file'
+    test_data = tempfile.TemporaryFile()
+    test_string = str(random.random())
+    test_data.write(test_string)
+    test_data.seek(0)
+    key_file = tempfile.NamedTemporaryFile()
+    key_file.write(self.key)
+    key_file.flush()
+    key_file.seek(0)
+
+    nc = slapos.libnetworkcache.NetworkcacheClient(
+      self.shacache, self.shadir)
+    self.assertEqual(True, nc.upload(self.test_data, key, urlmd5=urlmd5,
+        file_name=file_name))
+    f = os.path.join(self.tree, 'shadir', key)
+    # now remove the entry from shacache
+    open(f, 'w').write('This is not a json.')
+    try:
+      nc.select(key)
+    except slapos.libnetworkcache.DirectoryNotFound, msg:
+      self.assertTrue(str(msg).startswith('It was impossible to parse json '
+        'response'))
+
+  def test_select_json_no_in_json_response(self):
+    key = 'somekey' + str(random.random())
+    urlmd5 = str(random.random())
+    file_name = 'my file'
+    test_data = tempfile.TemporaryFile()
+    test_string = str(random.random())
+    test_data.write(test_string)
+    test_data.seek(0)
+    key_file = tempfile.NamedTemporaryFile()
+    key_file.write(self.key)
+    key_file.flush()
+    key_file.seek(0)
+
+    nc = slapos.libnetworkcache.NetworkcacheClient(
+      self.shacache, self.shadir)
+    self.assertEqual(True, nc.upload(self.test_data, key, urlmd5=urlmd5,
+        file_name=file_name))
+    f = os.path.join(self.tree, 'shadir', key)
+    # now remove the entry from shacache
+    open(f, 'w').write(json.dumps([['This is not a json.', 'signature']]))
+    try:
+      nc.select(key)
+    except slapos.libnetworkcache.DirectoryNotFound, msg:
+      self.assertTrue(str(msg).startswith('It was impossible to parse '
+        'json-in-json response'))
+
+  def test_select_json_in_json_no_dict(self):
+    key = 'somekey' + str(random.random())
+    urlmd5 = str(random.random())
+    file_name = 'my file'
+    test_data = tempfile.TemporaryFile()
+    test_string = str(random.random())
+    test_data.write(test_string)
+    test_data.seek(0)
+    key_file = tempfile.NamedTemporaryFile()
+    key_file.write(self.key)
+    key_file.flush()
+    key_file.seek(0)
+
+    nc = slapos.libnetworkcache.NetworkcacheClient(
+      self.shacache, self.shadir)
+    self.assertEqual(True, nc.upload(self.test_data, key, urlmd5=urlmd5,
+        file_name=file_name))
+    f = os.path.join(self.tree, 'shadir', key)
+    # now remove the entry from shacache
+    open(f, 'w').write(json.dumps([[json.dumps('This is a string'),
+      'signature']]))
+    try:
+      nc.select(key)
+    except slapos.libnetworkcache.DirectoryNotFound, msg:
+      self.assertTrue(str(msg).startswith('It was impossible to fetch sha512 '
+        'from directory response'))
+
   def test_select_signed_content_server_hacked(self):
     key = 'somekey' + str(random.random())
     urlmd5 = str(random.random())
     file_name = 'my file'
     test_data = tempfile.TemporaryFile()
     test_string = str(random.random())
     test_data.write(test_string)
```

### Comparing `slapos.libnetworkcache-0.8/slapos/signature.py` & `slapos.libnetworkcache-0.9/slapos/signature.py`

 * *Files identical despite different names*

### Comparing `slapos.libnetworkcache-0.8/slapos/separatedssltestserver.py` & `slapos.libnetworkcache-0.9/slapos/separatedssltestserver.py`

 * *Files identical despite different names*

### Comparing `slapos.libnetworkcache-0.8/slapos/libnetworkcache.py` & `slapos.libnetworkcache-0.9/slapos/libnetworkcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,19 @@
     Raise DirectoryNotFound if multiple files are found.
     '''
     url = os.path.join(self.shadir_url, key)
     request = urllib2.Request(url=url, data=None,
       headers=self.shadir_header_dict)
     data = urllib2.urlopen(request).read()
     # Filtering...
-    data_list = json.loads(data)
+    try:
+      data_list = json.loads(data)
+    except Exception:
+      raise DirectoryNotFound('It was impossible to parse json response:\n%s'%
+        traceback.format_exc())
     filtered_data_list = []
     if self.signature_certificate_list is not None:
       for data in data_list:
         if len(data[1]):
           if self._verifySignatureInCertificateList(data[0], data[1]):
             filtered_data_list.append(data)
     else:
@@ -223,16 +227,25 @@
       raise DirectoryNotFound('Could not find a trustable entry.')
 
     if len(filtered_data_list) > 1:
       raise DirectoryNotFound('Too many entries for a given key %r. ' \
                'Entries: %s.' % (key, str(data_list)))
 
     information_json, signature = filtered_data_list[0]
-    information_dict = json.loads(information_json)
-    sha512 = information_dict.get('sha512')
+    try:
+      information_dict = json.loads(information_json)
+    except Exception:
+      raise DirectoryNotFound('It was impossible to parse json-in-json '
+        'response:\n%s' % traceback.format_exc())
+    try:
+      sha512 = information_dict.get('sha512')
+    except Exception:
+      raise DirectoryNotFound('It was impossible to fetch sha512 from '
+        'directory response (%r):\n%s' % (information_dict,
+          traceback.format_exc()))
     return self.download(sha512)
 
   def _getSignatureString(self, content):
     """
       Return the signature based on certification file.
     """
     if self.signature_private_key_file is None:
```

### Comparing `slapos.libnetworkcache-0.8/CHANGES.txt` & `slapos.libnetworkcache-0.9/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changes
 =======
 
+0.9 (2011-09-02)
+----------------
+
+ * Bugfix: Do not trust received content. [Łukasz Nowak]
+
 0.8 (2011-09-02)
 ----------------
 
  * Bugfix: Do not try to validate against empty signatures. [Łukasz Nowak]
 
 0.7 (2011-09-02)
 ----------------
```

### Comparing `slapos.libnetworkcache-0.8/setup.py` & `slapos.libnetworkcache-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 name = "slapos.libnetworkcache"
-version = '0.8'
+version = '0.9'
 
 
 def read(*rnames):
   return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
```

### Comparing `slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/SOURCES.txt` & `slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slapos.libnetworkcache-0.8/slapos.libnetworkcache.egg-info/PKG-INFO` & `slapos.libnetworkcache-0.9/slapos.libnetworkcache.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: slapos.libnetworkcache
-Version: 0.8
+Version: 0.9
 Summary: libnetworkcache - Client for ShaCache and ShaDir HTTP Server
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: GPLv3
 Description: Introduction
         ============
@@ -28,14 +28,19 @@
         ===
         
         Please see slapos/libnetworkcache.py and slapos/libnetworkcachetests.py
         
         Changes
         =======
         
+        0.9 (2011-09-02)
+        ----------------
+        
+         * Bugfix: Do not trust received content. [Łukasz Nowak]
+        
         0.8 (2011-09-02)
         ----------------
         
          * Bugfix: Do not try to validate against empty signatures. [Łukasz Nowak]
         
         0.7 (2011-09-02)
         ----------------
```

### Comparing `slapos.libnetworkcache-0.8/PKG-INFO` & `slapos.libnetworkcache-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: slapos.libnetworkcache
-Version: 0.8
+Version: 0.9
 Summary: libnetworkcache - Client for ShaCache and ShaDir HTTP Server
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: GPLv3
 Description: Introduction
         ============
@@ -28,14 +28,19 @@
         ===
         
         Please see slapos/libnetworkcache.py and slapos/libnetworkcachetests.py
         
         Changes
         =======
         
+        0.9 (2011-09-02)
+        ----------------
+        
+         * Bugfix: Do not trust received content. [Łukasz Nowak]
+        
         0.8 (2011-09-02)
         ----------------
         
          * Bugfix: Do not try to validate against empty signatures. [Łukasz Nowak]
         
         0.7 (2011-09-02)
         ----------------
```

### Comparing `slapos.libnetworkcache-0.8/README.txt` & `slapos.libnetworkcache-0.9/README.txt`

 * *Files identical despite different names*

