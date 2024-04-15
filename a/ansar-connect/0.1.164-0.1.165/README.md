# Comparing `tmp/ansar_connect-0.1.164.tar.gz` & `tmp/ansar_connect-0.1.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.164.tar", last modified: Mon Apr 15 02:04:31 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.165.tar", last modified: Mon Apr 15 02:27:22 2024, max compression
```

## Comparing `ansar_connect-0.1.164.tar` & `ansar_connect-0.1.165.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.164/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.164/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.164/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.164/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.730384 ansar_connect-0.1.164/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.730384 ansar_connect-0.1.164/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.164/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.164/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.164/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.164/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-15 02:04:28.000000 ansar_connect-0.1.164/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 15:15:11.000000 ansar_connect-0.1.164/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.164/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.164/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.164/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.164/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.164/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.164/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.164/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.164/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.164/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.164/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.164/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.164/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38859 2024-04-15 01:59:03.000000 ansar_connect-0.1.164/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.164/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.164/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.164/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:04:31.734384 ansar_connect-0.1.164/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-15 02:04:31.000000 ansar_connect-0.1.164/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.945850 ansar_connect-0.1.165/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.165/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 02:27:22.945850 ansar_connect-0.1.165/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.165/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.165/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-15 02:27:22.945850 ansar_connect-0.1.165/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.165/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.941851 ansar_connect-0.1.165/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.941851 ansar_connect-0.1.165/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.941851 ansar_connect-0.1.165/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.165/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.165/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.165/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.165/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.945850 ansar_connect-0.1.165/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-15 02:27:19.000000 ansar_connect-0.1.165/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 15:15:11.000000 ansar_connect-0.1.165/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.165/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.165/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.165/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.165/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.165/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.165/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.165/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.165/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.165/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.165/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.165/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.165/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    39075 2024-04-15 02:26:18.000000 ansar_connect-0.1.165/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.165/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.165/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.165/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 02:27:22.945850 ansar_connect-0.1.165/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-15 02:27:22.000000 ansar_connect-0.1.165/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.164/LICENSE` & `ansar_connect-0.1.165/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/PKG-INFO` & `ansar_connect-0.1.165/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.164
+Version: 0.1.165
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.164/README.md` & `ansar_connect-0.1.165/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/pyproject.toml` & `ansar_connect-0.1.165/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/setup.py` & `ansar_connect-0.1.165/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.165/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.165/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.165/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.165/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/__init__.py` & `ansar_connect-0.1.165/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: ddfe8b7790966c395f5b0fd7f748f11c5a918366
-Version: 0.1.163 (2024-04-15@14:04:28+NZST)
+Commit: bdd7483a8b63a9b550355ab6c38c2511b13b906c
+Version: 0.1.164 (2024-04-15@14:27:19+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.164/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.165/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/directory.py` & `ansar_connect-0.1.165/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.165/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.165/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/group_if.py` & `ansar_connect-0.1.165/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/grouping.py` & `ansar_connect-0.1.165/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/moving.py` & `ansar_connect-0.1.165/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/networking.py` & `ansar_connect-0.1.165/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.165/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/node.py` & `ansar_connect-0.1.165/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.165/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/procedure.py` & `ansar_connect-0.1.165/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/product.py` & `ansar_connect-0.1.165/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/socketry.py` & `ansar_connect-0.1.165/src/ansar/connect/socketry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1282,20 +1282,22 @@
 		# for every socket in every list --- select([sock],[],[],0)
 		# to find which one has failed.
 
 		for r in R:
 			try:
 				h = id(r)
 				if h in self.handshaking:
-					try:
-						r.do_handshake()
-					except ssl.SSLWantReadError:
-						continue
-					except ssl.SSLWantWriteError:
-						continue
+					while True:
+						try:
+							r.do_handshake()
+							break
+						except ssl.SSLWantReadError:
+							select.select([r], [], [])
+						except ssl.SSLWantWriteError:
+							select.select([], [r], [])
 					self.handshaking.discard(h)
 					continue
 
 				a = self.networking[r]
 				c = a.__class__
 				j = select_table[(c, ReceiveBlock)]
 			except KeyError:
@@ -1305,20 +1307,22 @@
 				continue
 			j(self, a, r)
 
 		for s in S:
 			try:
 				h = id(s)
 				if h in self.handshaking:
-					try:
-						s.do_handshake()
-					except ssl.SSLWantReadError:
-						continue
-					except ssl.SSLWantWriteError:
-						continue
+					while True:
+						try:
+							s.do_handshake()
+							break
+						except ssl.SSLWantReadError:
+							select.select([s], [], [])
+						except ssl.SSLWantWriteError:
+							select.select([], [s], [])
 					self.handshaking.discard(h)
 					continue
 
 				a = self.networking[s]
 				c = a.__class__
 				j = select_table[(c, ReadyToSend)]
 			except KeyError:
@@ -1328,20 +1332,22 @@
 				continue
 			j(self, a, s)
 
 		for f in F:
 			try:
 				h = id(f)
 				if h in self.handshaking:
-					try:
-						f.do_handshake()
-					except ssl.SSLWantReadError:
-						continue
-					except ssl.SSLWantWriteError:
-						continue
+					while True:
+						try:
+							f.do_handshake()
+							break
+						except ssl.SSLWantReadError:
+							select.select([f], [], [])
+						except ssl.SSLWantWriteError:
+							select.select([], [f], [])
 					self.handshaking.discard(h)
 					continue
 
 				a = self.networking[f]
 				c = a.__class__
 				j = select_table[(c, BrokenTransport)]
 			except KeyError:
```

### Comparing `ansar_connect-0.1.164/src/ansar/connect/standard.py` & `ansar_connect-0.1.165/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/transporting.py` & `ansar_connect-0.1.165/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar/connect/wan.py` & `ansar_connect-0.1.165/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.164/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.165/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.164
+Version: 0.1.165
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.164/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.165/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

