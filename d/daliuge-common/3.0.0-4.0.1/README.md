# Comparing `tmp/daliuge-common-3.0.0.tar.gz` & `tmp/daliuge-common-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-common-3.0.0.tar", last modified: Thu May 18 12:49:51 2023, max compression
+gzip compressed data, was "daliuge-common-4.0.1.tar", last modified: Mon Apr 15 07:01:39 2024, max compression
```

## Comparing `daliuge-common-3.0.0.tar` & `daliuge-common-4.0.1.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      321 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      654 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/README.md
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/daliuge_common.egg-info/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      321 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      779 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       44 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       29 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/daliuge_common.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9571 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/clients.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/common/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8417 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1109 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/deployment_methods.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1451 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/k8s_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6305 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/network.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1987 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/osutils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/dlg/common/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/__init__.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4420 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7505 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reprodata_compare.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33879 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8979 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility_fields.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5843 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/streams.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5123 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/common/tool.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      199 2023-05-18 12:49:51.000000 daliuge-common-3.0.0/dlg/common/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1850 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/constants.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4834 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/exceptions.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7029 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/restutils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16698 2023-05-18 12:40:21.000000 daliuge-common-3.0.0/dlg/utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2210 2023-05-18 12:38:53.000000 daliuge-common-3.0.0/dlg/version_helper.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-05-18 12:49:51.340462 daliuge-common-3.0.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2454 2023-05-18 12:43:13.000000 daliuge-common-3.0.0/setup.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      321 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      654 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/README.md
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1896 2023-06-29 09:21:30.000000 daliuge-common-4.0.1/build_common.sh
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.928615 daliuge-common-4.0.1/daliuge_common.egg-info/
+-rw-r--r--   0 awicenec  (1000) awicenec  (1000)      321 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      906 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       44 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      168 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        4 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/daliuge_common.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.928615 daliuge-common-4.0.1/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9558 2024-04-12 16:12:35.000000 daliuge-common-4.0.1/dlg/clients.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/dlg/common/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8417 2023-06-29 08:45:39.000000 daliuge-common-4.0.1/dlg/common/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1109 2023-05-09 13:46:34.000000 daliuge-common-4.0.1/dlg/common/deployment_methods.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1451 2023-05-09 13:46:34.000000 daliuge-common-4.0.1/dlg/common/k8s_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6305 2023-05-09 13:46:34.000000 daliuge-common-4.0.1/dlg/common/network.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1987 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/common/osutils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/dlg/common/reproducibility/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        0 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/common/reproducibility/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4420 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/common/reproducibility/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7505 2023-05-09 13:02:30.000000 daliuge-common-4.0.1/dlg/common/reproducibility/reprodata_compare.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33879 2023-06-29 08:45:39.000000 daliuge-common-4.0.1/dlg/common/reproducibility/reproducibility.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8979 2023-06-29 08:45:39.000000 daliuge-common-4.0.1/dlg/common/reproducibility/reproducibility_fields.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5843 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/common/streams.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5123 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/common/tool.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      199 2024-04-15 07:01:39.000000 daliuge-common-4.0.1/dlg/common/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1850 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/constants.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4834 2023-05-09 13:46:34.000000 daliuge-common-4.0.1/dlg/exceptions.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7052 2024-04-12 16:12:35.000000 daliuge-common-4.0.1/dlg/restutils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16836 2024-03-18 15:04:41.000000 daliuge-common-4.0.1/dlg/utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2210 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/dlg/version_helper.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/docker/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      585 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/docker/Dockerfile
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1957 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/docker/Dockerfile.casa
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      711 2024-04-12 16:12:35.000000 daliuge-common-4.0.1/docker/Dockerfile.dev
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1423 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/docker/Dockerfile.devcuda
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      632 2022-11-30 13:05:02.000000 daliuge-common-4.0.1/docker/Dockerfile.ray
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2024-04-15 07:01:39.932615 daliuge-common-4.0.1/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2694 2024-04-15 06:59:37.000000 daliuge-common-4.0.1/setup.py
```

### Comparing `daliuge-common-3.0.0/README.md` & `daliuge-common-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/daliuge_common.egg-info/SOURCES.txt` & `daliuge-common-4.0.1/daliuge_common.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+build_common.sh
 setup.py
 daliuge_common.egg-info/PKG-INFO
 daliuge_common.egg-info/SOURCES.txt
 daliuge_common.egg-info/dependency_links.txt
 daliuge_common.egg-info/entry_points.txt
 daliuge_common.egg-info/requires.txt
 daliuge_common.egg-info/top_level.txt
@@ -21,8 +22,13 @@
 dlg/common/streams.py
 dlg/common/tool.py
 dlg/common/version.py
 dlg/common/reproducibility/__init__.py
 dlg/common/reproducibility/constants.py
 dlg/common/reproducibility/reprodata_compare.py
 dlg/common/reproducibility/reproducibility.py
-dlg/common/reproducibility/reproducibility_fields.py
+dlg/common/reproducibility/reproducibility_fields.py
+docker/Dockerfile
+docker/Dockerfile.casa
+docker/Dockerfile.dev
+docker/Dockerfile.devcuda
+docker/Dockerfile.ray
```

### Comparing `daliuge-common-3.0.0/dlg/__init__.py` & `daliuge-common-4.0.1/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/clients.py` & `daliuge-common-4.0.1/dlg/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 from .restutils import RestClient
 
 logger = logging.getLogger(__name__)
 compress = os.environ.get("DALIUGE_COMPRESSED_JSON", True)
 
 quote = urllib.parse.quote
 
-default_host = "localhost" # localhost now binds to IPv6 address on some distros
+default_host = "localhost"  # localhost now binds to IPv6 address on some distros
+
 
 class BaseDROPManagerClient(RestClient):
     """
     Base class for REST clients that talk to the DROP managers.
     """
 
     def _request(self, url, method, content=None, headers={}):
@@ -133,15 +134,15 @@
         Returns a list of all the sessions currently held by the DROP Manager
         """
         sessions = self._get_json("/sessions")
         logger.debug(
             "Successfully read %d sessions from %s:%s",
             len(sessions),
             self.host,
-            self.port
+            self.port,
         )
         return sessions
 
     def session(self, sessionId):
         """
         Returns the details of sessions `sessionId`
         """
@@ -219,15 +220,15 @@
 
 class NodeManagerClient(BaseDROPManagerClient):
     """
     A NodeManager REST client
     """
 
     def __init__(
-            self, host=default_host, port=constants.NODE_DEFAULT_REST_PORT, timeout=10
+        self, host=default_host, port=constants.NODE_DEFAULT_REST_PORT, timeout=10
     ):
         super(NodeManagerClient, self).__init__(host=host, port=port, timeout=timeout)
 
     def add_node_subscriptions(self, sessionId, node_subscriptions):
         self._post_json(
             f"/sessions/{quote(sessionId)}/subscriptions", node_subscriptions
         )
@@ -238,58 +239,56 @@
     def shutdown_node_manager(self):
         self._GET("/shutdown")
 
     def get_log_file(self, sessionId):
         return self._request(f"/sessions/{sessionId}/logs", "GET")
 
     def get_submission_method(self):
-        return self._get_json("/submission_method")
+        return self._get_json("submission_method")
 
 
 class CompositeManagerClient(BaseDROPManagerClient):
     def nodes(self):
         return self._get_json("/nodes")
 
     def add_node(self, node):
         self._POST(f"/node/{node}", content=None)
 
     def remove_node(self, node):
         self._DELETE(f"/node/{node}")
 
     def get_submission_method(self):
-        return self._get_json("/submission_method")
+        return self._get_json("submission_method")
 
 
 class DataIslandManagerClient(CompositeManagerClient):
     """
     A DataIslandManager REST client
     """
 
     def __init__(
-            self, host=default_host, port=constants.ISLAND_DEFAULT_REST_PORT, timeout=10
+        self, host=default_host, port=constants.ISLAND_DEFAULT_REST_PORT, timeout=10
     ):
         super(DataIslandManagerClient, self).__init__(
             host=host, port=port, timeout=timeout
         )
 
 
 class MasterManagerClient(CompositeManagerClient):
     """
     A MasterManager REST client
     """
 
     def __init__(
-            self, host=default_host, port=constants.MASTER_DEFAULT_REST_PORT, timeout=10
+        self, host=default_host, port=constants.MASTER_DEFAULT_REST_PORT, timeout=10
     ):
         super(MasterManagerClient, self).__init__(host=host, port=port, timeout=timeout)
 
     def create_island(self, island_host, nodes):
-        self._post_json(
-            f"/managers/{quote(island_host)}/island", {"nodes": nodes}
-        )
+        self._post_json(f"/managers/{quote(island_host)}/island", {"nodes": nodes})
 
     def dims(self):
         return self._get_json("/islands")
 
     def add_dim(self, dim):
         self._POST(f"/island/{dim}", content=None)
 
@@ -297,14 +296,16 @@
         self._DELETE(f"/island/{dim}")
 
     def add_node_to_dim(self, dim, nm):
         """
         Adds a nm to a dim
         """
         self._POST(
-            f"/managers/{dim}/node/{nm}", content=None, )
+            f"/managers/{dim}/node/{nm}",
+            content=None,
+        )
 
     def remove_node_from_dim(self, dim, nm):
         """
         Removes a nm from a dim
         """
         self._DELETE(f"/managers/{dim}/node/{nm}")
```

### Comparing `daliuge-common-3.0.0/dlg/common/__init__.py` & `daliuge-common-4.0.1/dlg/common/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/deployment_methods.py` & `daliuge-common-4.0.1/dlg/common/deployment_methods.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/k8s_utils.py` & `daliuge-common-4.0.1/dlg/common/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/network.py` & `daliuge-common-4.0.1/dlg/common/network.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/osutils.py` & `daliuge-common-4.0.1/dlg/common/osutils.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/reproducibility/constants.py` & `daliuge-common-4.0.1/dlg/common/reproducibility/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/reproducibility/reprodata_compare.py` & `daliuge-common-4.0.1/dlg/common/reproducibility/reprodata_compare.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility.py` & `daliuge-common-4.0.1/dlg/common/reproducibility/reproducibility.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/reproducibility/reproducibility_fields.py` & `daliuge-common-4.0.1/dlg/common/reproducibility/reproducibility_fields.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/streams.py` & `daliuge-common-4.0.1/dlg/common/streams.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/common/tool.py` & `daliuge-common-4.0.1/dlg/common/tool.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/constants.py` & `daliuge-common-4.0.1/dlg/constants.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/exceptions.py` & `daliuge-common-4.0.1/dlg/exceptions.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/dlg/restutils.py` & `daliuge-common-4.0.1/dlg/restutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 class RestClient(object):
     """
     The base class for our REST clients
     """
 
-    def __init__(self, host, port, url_prefix="", timeout=None):
+    def __init__(self, host, port, url_prefix="", timeout=10):
         self.host = host
         self.port = port
         self.url_prefix = url_prefix
         self.timeout = timeout
         self._conn = None
         self._resp = None
 
@@ -140,17 +140,15 @@
     def _get_json(self, url):
         ret = self._GET(url)
         return json.load(ret) if ret else None
 
     def _post_form(self, url, content=None):
         if content is not None:
             content = urllib.parse.urlencode(content)
-        ret = self._POST(
-            url, content, content_type="application/x-www-form-urlencoded"
-        )
+        ret = self._POST(url, content, content_type="application/x-www-form-urlencoded")
         return json.load(ret) if ret else None
 
     def _post_json(self, url, content, compress=False):
         if not isinstance(content, (str, bytes)):
             content = common.JSONStream(content)
         ret = self._POST(
             url, content, content_type="application/json", compress=compress
@@ -175,29 +173,28 @@
         stream, _ = self._request(url, "POST", content, headers)
         return stream
 
     def _DELETE(self, url):
         stream, _ = self._request(url, "DELETE")
         return stream
 
-    def _request(self, url, method, content=None, headers={}):
+    def _request(self, url, method, content=None, headers={}, timeout=10):
         # Do the HTTP stuff...
         url = self.url_prefix + url
-        logger.debug(
-            "Sending %s request to %s:%d%s", method, self.host, self.port, url
-        )
+        logger.debug("Sending %s request to %s:%d%s", method, self.host, self.port, url)
 
-        if not common.portIsOpen(self.host, self.port, self.timeout):
+        if not common.portIsOpen(self.host, self.port, timeout):
             raise RestClientException(
                 "Cannot connect to %s:%d after %.2f [s]"
                 % (self.host, self.port, self.timeout)
             )
 
         if content and hasattr(content, "read"):
             headers["Transfer-Encoding"] = "chunked"
+            headers["Origin"] = "http://dlg-trans.local:8084"
             content = chunked(content)
 
         self._conn = http.client.HTTPConnection(self.host, self.port)
         self._conn.request(method, url, content, headers)
         self._resp = self._conn.getresponse()
 
         # Server errors are encoded in the body as json content
```

### Comparing `daliuge-common-3.0.0/dlg/utils.py` & `daliuge-common-4.0.1/dlg/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #    License along with this library; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 #
 """
 Module containing miscellaneous utility classes and functions.
 """
-
+import base64
 import errno
 import functools
 import importlib
 import io
 import logging
 import os
 import signal
@@ -34,42 +34,39 @@
 import threading
 import time
 from typing import Tuple
 import zlib
 import re
 import grp
 import pwd
+import pickle
 
 import netifaces
 
 from . import common
 
 logger = logging.getLogger(__name__)
 
 
 def timed_import(module_name):
     """Imports `module_name` and log how long it took to import it"""
     start = time.time()
     module = importlib.import_module(module_name)
-    logger.info(
-        "Imported %s in %.3f seconds", module_name, time.time() - start
-    )
+    logger.info("Imported %s in %.3f seconds", module_name, time.time() - start)
     return module
 
 
 def get_local_ip_addr():
     """
     Enumerate all interfaces and return bound IP addresses (exclude localhost)
     """
     PROTO = netifaces.AF_INET
     ifaces = netifaces.interfaces()
     if_addrs = [(netifaces.ifaddresses(iface), iface) for iface in ifaces]
-    if_inet_addrs = [
-        (tup[0][PROTO], tup[1]) for tup in if_addrs if PROTO in tup[0]
-    ]
+    if_inet_addrs = [(tup[0][PROTO], tup[1]) for tup in if_addrs if PROTO in tup[0]]
     iface_addrs = [
         (s["addr"], tup[1])
         for tup in if_inet_addrs
         for s in tup[0]
         if "addr" in s and not s["addr"].startswith("127.")
     ]
     return iface_addrs
@@ -84,17 +81,15 @@
         for iface_proto, addrs in netifaces.ifaddresses(iface).items()
         if proto == iface_proto
         for addr in addrs
         if "addr" in addr
     ]
 
 
-def register_service(
-    zc, service_type_name, service_name, ipaddr, port, protocol="tcp"
-):
+def register_service(zc, service_type_name, service_name, ipaddr, port, protocol="tcp"):
     """
     ZeroConf: Register service type, protocol, ipaddr and port
 
     Returns ZeroConf object and ServiceInfo object
     """
     import zeroconf
 
@@ -400,17 +395,15 @@
         to_decompress = decompressor.unconsumed_tail + compressed
 
         while True:
             decompressed = decompressor.decompress(to_decompress)
             if not decompressed:
                 break
             response.write(decompressed)
-            to_decompress = decompressor.unconsumed_tail + content.read(
-                blocksize
-            )
+            to_decompress = decompressor.unconsumed_tail + content.read(blocksize)
 
         response.write(decompressor.flush())
         self.decompressor = None
         return response.getvalue()
 
     def read(self, n=-1):
         if n == -1:
@@ -514,32 +507,38 @@
         raise
     template_dir = os.path.dirname(__file__)
     # get current user info
     pw = pwd.getpwuid(os.getuid())
     gr = grp.getgrgid(pw.pw_gid)
     dgr = grp.getgrnam("docker")
     with open(os.path.join(workdir, "passwd"), "wt") as file:
-        file.write(
-            open(os.path.join(template_dir, "passwd.template"), "rt").read()
-        )
+        file.write(open(os.path.join(template_dir, "passwd.template"), "rt").read())
         file.write(
             f"{pw.pw_name}:x:{pw.pw_uid}:{pw.pw_gid}:{pw.pw_gecos}:{DLG_ROOT}:/bin/bash\n"
         )
         logger.debug(f"passwd file written {file.name}")
     with open(os.path.join(workdir, "group"), "wt") as file:
-        file.write(
-            open(os.path.join(template_dir, "group.template"), "rt").read()
-        )
+        file.write(open(os.path.join(template_dir, "group.template"), "rt").read())
         file.write(f"{gr.gr_name}:x:{gr.gr_gid}:\n")
         file.write(f"docker:x:{dgr.gr_gid}\n")
         logger.debug(f"Group file written {file.name}")
 
     return dgr.gr_gid
 
 
+def serialize_data(d):
+    # return pickle.dumps(d)
+    return b2s(base64.b64encode(pickle.dumps(d)))
+
+
+def deserialize_data(d):
+    # return pickle.loads()
+    return pickle.loads(base64.b64decode(d.encode("utf8")))
+
+
 # Backwards compatibility
 terminate_or_kill = common.osutils.terminate_or_kill
 wait_or_kill = common.osutils.wait_or_kill
 b2s = common.b2s
 
 check_port = common.check_port
 connect_to = common.connect_to
```

### Comparing `daliuge-common-3.0.0/dlg/version_helper.py` & `daliuge-common-4.0.1/dlg/version_helper.py`

 * *Files identical despite different names*

### Comparing `daliuge-common-3.0.0/setup.py` & `daliuge-common-4.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,37 +26,53 @@
 
 # Version information
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
-MAJOR = 3
+MAJOR = 4
 MINOR = 0
-PATCH = 0
+PATCH = 1
 VERSION = (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/common/version.py"
 RELEASE = True
 
 
 def do_versioning():
     # Avoid importing, the package doesn't exist as such yet
     with open(os.path.join("dlg", "version_helper.py")) as f:
         code = f.read()
     _globals = {}
     exec(code, _globals)
     return _globals["write_version_info"](VERSION, VERSION_FILE, RELEASE)
 
 
-install_requires = ["gputil>=1.4.0", "merklelib>=1.0"]
+install_requires = [
+    "gputil>=1.4.0",
+    "merklelib>=1.0",
+    "pyzmq==25.1.0",
+    "pydantic==1.10.7",
+    "boto3",
+    "phonenumbers",
+    "mailchecker",
+    "ftfy",
+    "toml",
+    "pyyaml",
+    "beautifulsoup4",
+    "openpyxl",
+    "xlrd",
+    "xmltodict",
+    "python-benedict[all]",
+]
 
 setup(
     name="daliuge-common",
     version=do_versioning(),
-    description=u"Data Activated \uF9CA (flow) Graph Engine - Common functionality",
+    description="Data Activated \uF9CA (flow) Graph Engine - Common functionality",
     long_description="The SKA-SDK prototype for the Execution Framework component",
     author="ICRAR DIA Group",
     author_email="dfms_prototype@googlegroups.com",
     url="https://github.com/ICRAR/daliuge",
     license="LGPLv2+",
     packages=find_packages(),
     test_suite="test",
```

