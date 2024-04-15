# Comparing `tmp/ansar_connect-0.1.166.tar.gz` & `tmp/ansar_connect-0.1.167.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.166.tar", last modified: Mon Apr 15 03:02:14 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.167.tar", last modified: Mon Apr 15 06:32:29 2024, max compression
```

## Comparing `ansar_connect-0.1.166.tar` & `ansar_connect-0.1.167.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.022271 ansar_connect-0.1.166/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.166/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 03:02:14.022271 ansar_connect-0.1.166/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.166/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.166/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-15 03:02:14.022271 ansar_connect-0.1.166/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.166/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.018271 ansar_connect-0.1.166/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.018271 ansar_connect-0.1.166/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.018271 ansar_connect-0.1.166/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.166/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.166/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.166/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.166/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.022271 ansar_connect-0.1.166/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-15 03:02:10.000000 ansar_connect-0.1.166/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-14 15:15:11.000000 ansar_connect-0.1.166/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.166/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.166/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.166/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.166/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.166/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.166/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.166/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.166/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.166/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.166/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.166/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.166/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38734 2024-04-15 03:01:31.000000 ansar_connect-0.1.166/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.166/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.166/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.166/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 03:02:14.022271 ansar_connect-0.1.166/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-15 03:02:14.000000 ansar_connect-0.1.166/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.401489 ansar_connect-0.1.167/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.167/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.167/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar_connect-0.1.167/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-15 06:32:29.401489 ansar_connect-0.1.167/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar_connect-0.1.167/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.167/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.167/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.167/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.167/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-15 06:32:26.000000 ansar_connect-0.1.167/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.167/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.167/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.167/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.167/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.167/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.167/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.167/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.167/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.167/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.167/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.167/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.167/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.167/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38749 2024-04-15 06:31:16.000000 ansar_connect-0.1.167/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.167/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.167/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.167/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-15 06:32:29.397489 ansar_connect-0.1.167/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-15 06:32:29.000000 ansar_connect-0.1.167/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.166/LICENSE` & `ansar_connect-0.1.167/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/PKG-INFO` & `ansar_connect-0.1.167/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.166
+Version: 0.1.167
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.166/README.md` & `ansar_connect-0.1.167/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/pyproject.toml` & `ansar_connect-0.1.167/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/setup.py` & `ansar_connect-0.1.167/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.167/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.167/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.167/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.167/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/__init__.py` & `ansar_connect-0.1.167/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 1f0f8e5d089e8d6a254fcce5a6e4c988f94c6ef9
-Version: 0.1.165 (2024-04-15@15:02:10+NZST)
+Commit: f513078edcb11c0a0410aeaea4f5a64de19055c4
+Version: 0.1.166 (2024-04-15@18:32:26+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.166/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.167/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/directory.py` & `ansar_connect-0.1.167/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.167/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.167/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/group_if.py` & `ansar_connect-0.1.167/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/grouping.py` & `ansar_connect-0.1.167/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/moving.py` & `ansar_connect-0.1.167/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/networking.py` & `ansar_connect-0.1.167/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.167/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/node.py` & `ansar_connect-0.1.167/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.167/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/procedure.py` & `ansar_connect-0.1.167/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/product.py` & `ansar_connect-0.1.167/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/socketry.py` & `ansar_connect-0.1.167/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -995,17 +995,17 @@
 		try:
 			stream.receive_and_route(scrap, self)
 		except (ar.CodecFailed, OverflowError, ValueError) as e:
 			value = ar.Faulted(condition='cannot start inbound', explanation=str(e))
 			close_session(stream, value, s)
 		return
 
-	except ssl.SSLError as e:
-		self.trace(f'SSL error "{e}" (in receive event for incomplete connect)')
-		return
+	#except ssl.SSLError as e:
+	#	self.trace(f'SSL error "{e}" (in receive event for incomplete connect)')
+	#	return
 	except socket.error as e:
 		self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), selector.controller_address)
 		self.clear(s, TcpClient)
 		#self.send(NotConnected(request.requested_ipp, e.errno, str(e), request.tag), stream.controller_address)
 		#self.send(ar.Stop(), stream.remote_address)
 		#self.clear(s, TcpStream)
 		return
@@ -1072,18 +1072,18 @@
 		if stream.send_a_block(s):
 			return
 	except (ar.CodecFailed, OverflowError, ValueError) as e:
 		value = ar.Faulted(condition='cannot stream outbound', explanation=str(e))
 		self.warning(str(value))
 		close_session(stream, value, s)
 		return
-	except ssl.SSLError as e:
-		# Seems to occur as a natural part of negotiation.
-		# self.trace(f'SSL error [2] "{e}"')
-		return
+		#except ssl.SSLError as e:
+		#	# Seems to occur as a natural part of negotiation.
+		#	# self.trace(f'SSL error [2] "{e}"')
+		#	return
 
 	try:
 		self.sending.remove(s)
 	except KeyError:
 		pass
 
 # A network transport for the purpose of exchanging
@@ -1100,18 +1100,18 @@
 			stream.receive_and_route(scrap, self)
 		except (ar.CodecFailed, OverflowError, ValueError) as e:
 			value = ar.Faulted(condition='cannot stream inbound', explanation=str(e))
 			self.warning(str(value))
 			close_session(stream, value, s)
 		return
 
-	except ssl.SSLError as e:
-		# Seems to occur as a natural part of negotiation.
-		# self.trace(f'SSL error [3] "{e}"')
-		return
+	#except ssl.SSLError as e:
+	#	# Seems to occur as a natural part of negotiation.
+	#	# self.trace(f'SSL error [3] "{e}"')
+	#	return
 	except socket.error as e:
 		if e.errno == errno.ECONNREFUSED:
 			self.fault('Unexpected connection refused')
 		elif e.errno not in SOCKET_DOWN:
 			self.fault('Unexpected socket termination [%d] %s' % (e.errno, e.strerror))
 		end_of_session(self, stream, s)
 		return
@@ -1323,15 +1323,15 @@
 		for f in F:
 			try:
 				h = id(f)
 				if h in self.handshaking:
 					f.do_handshake()
 					self.handshaking.discard(h)
 					continue
-				a = self.networking[s]
+				a = self.networking[f]
 				c = a.__class__
 				j = select_table[(c, ReceiveBlock)]
 			except (ssl.SSLWantReadError, ssl.SSLWantWriteError):
 				continue
 			except KeyError:
 				continue
 			except ValueError:
```

### Comparing `ansar_connect-0.1.166/src/ansar/connect/standard.py` & `ansar_connect-0.1.167/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/transporting.py` & `ansar_connect-0.1.167/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar/connect/wan.py` & `ansar_connect-0.1.167/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.166/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.167/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.166
+Version: 0.1.167
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.166/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.167/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

