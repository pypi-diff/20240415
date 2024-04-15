# Comparing `tmp/vantage6-node-4.3.4rc3.tar.gz` & `tmp/vantage6-node-4.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.3.4rc3.tar", last modified: Mon Mar 25 11:02:00 2024, max compression
+gzip compressed data, was "vantage6-node-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:19 2024, max compression
```

## Comparing `vantage6-node-4.3.4rc3.tar` & `vantage6-node-4.4.0rc3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.611180 vantage6-node-4.3.4rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.611180 vantage6-node-4.3.4rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.611180 vantage6-node-4.3.4rc3/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    41843 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.611180 vantage6-node-4.3.4rc3/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27826 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24517 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-25 11:01:46.000000 vantage6-node-4.3.4rc3/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.615180 vantage6-node-4.3.4rc3/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 11:02:00.000000 vantage6-node-4.3.4rc3/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.507510 vantage6-node-4.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.507510 vantage6-node-4.4.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    41932 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27826 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25123 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-15 13:15:06.000000 vantage6-node-4.4.0rc3/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.511510 vantage6-node-4.4.0rc3/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 13:15:19.000000 vantage6-node-4.4.0rc3/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-4.3.4rc3/PKG-INFO` & `vantage6-node-4.4.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.3.4rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.4.0rc3 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-node-4.3.4rc3/setup.py` & `vantage6-node-4.4.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/__init__.py` & `vantage6-node-4.4.0rc3/vantage6/node/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,17 +494,18 @@
     def __print_connection_error_logs(self):
         """Print error message when node cannot find the server"""
         self.log.warning("Could not connect to the server. Retrying in 10 seconds")
         if self.client.host == "http://localhost" and running_in_docker():
             self.log.warn(
                 f"You are trying to reach the server at {self.client.host}."
                 " As your node is running inside a Docker container, it cannot"
-                " reach localhost on your host system. Probably, you have to "
-                "change your serverl URL to http://host.docker.internal "
-                "(Windows/MacOS) or http://172.17.0.1 (Linux)."
+                " reach localhost on your host system. Probably, you have to"
+                " change your server URL to http://host.docker.internal (Windows/MacOS)"
+                ' or look into node config option "node_extra_hosts" if using'
+                " http://172.17.0.1 does not work (Linux)."
             )
         else:
             self.log.debug(
                 "Are you sure the server can be reached at " f"{self.client.base_path}?"
             )
 
     def authenticate(self) -> None:
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/_version.py` & `vantage6-node-4.4.0rc3/vantage6/node/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 3, 4, "candidate", __build__, 0)
+version_info = (4, 4, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/cli/node.py` & `vantage6-node-4.4.0rc3/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/context.py` & `vantage6-node-4.4.0rc3/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/docker_base.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/docker_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/exceptions.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/squid.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/squid.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.common.docker.addons import (
     remove_container,
     running_in_docker,
     remove_container_if_exists,
-    pull_if_newer,
+    pull_image,
 )
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.docker_manager import NetworkManager
 from vantage6.node.globals import SQUID_IMAGE, PACKAGE_FOLDER
 from vantage6.node._version import major_minor
 
 log = logging.getLogger(logger_name(__name__))
@@ -86,33 +86,35 @@
         )
 
         # hostname of the squid which can be used by the algorithm containers
         self.hostname = "squid"
         # This is the default port of the squid container, which is exposed
         # to the algorithm containers.
         self.port = 3128
-        log.debug(f"Squid hostname: {self.hostname}, port: {self.port}")
+        log.debug("Squid hostname: %s, port: %s", self.hostname, self.port)
 
         try:
             # Create squid configuration, which can later be mounted by the
             # squid container
             self.squid_config = self.read_config(config)
         except KeyError as e:
             # parent class should handle this
             raise KeyError(f"Invalid Squid configuration: {e}")
 
-        log.debug(f"Squid configuration: {self.squid_config}")
+        log.debug("Squid configuration: %s", self.squid_config)
 
         # Check if the whitelist is safe, if not, log a warning
         self.check_safety_of_whitelist(self.squid_config)
 
         # The image is overridable by the user configuration
         self.image = squid_image if squid_image else f"{SQUID_IMAGE}:{major_minor}"
-        pull_if_newer(self.docker, self.image, log)
-        log.debug(f"Squid image: {self.image}")
+        log.info("Pulling Squid image: %s", self.image)
+        pull_image(self.docker, self.image)
+
+        log.debug("Squid image: %s", self.image)
 
         # Create the SSH configuration files
         self.create_squid_config_file(self.squid_config)
 
         self.start()
         log.info("Squid started")
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/task_manager.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from pathlib import Path
 from docker import DockerClient
 
 from vantage6.common.globals import APPNAME, ENV_VAR_EQUALS_REPLACEMENT, STRING_ENCODING
 from vantage6.common.docker.addons import (
     remove_container_if_exists,
     remove_container,
-    pull_if_newer,
     running_in_docker,
 )
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.common.task_status import TaskStatus
 from vantage6.node.util import get_parent_id
 from vantage6.node.globals import ALPINE_IMAGE, ENV_VARS_NOT_SETTABLE_BY_NODE
 from vantage6.node.docker.vpn_manager import VPNManager
@@ -180,30 +179,47 @@
         bytes:
             Results of the algorithm container
         """
         with open(self.output_file, "rb") as fp:
             results = fp.read()
         return results
 
-    def pull(self):
-        """Pull the latest docker image."""
+    def pull(self, local_exists: bool) -> None:
+        """
+        Pull the latest docker image.
+
+        Parameters
+        ----------
+        local_exists: bool
+            Whether the image already exists locally
+
+        Raises
+        ------
+        PermanentAlgorithmStartFail
+            If the image could not be pulled and does not exist locally
+        """
         try:
             self.log.info(f"Retrieving latest image: '{self.image}'")
-            pull_if_newer(self.docker, self.image, self.log)
-
+            self.docker.images.pull(self.image)
         except docker.errors.APIError as e:
-            self.log.debug("Failed to pull image: could not find image")
-            self.log.exception(e)
-            self.status = TaskStatus.NO_DOCKER_IMAGE
-            raise PermanentAlgorithmStartFail
+            self.log.warning("Failed to pull image: could not find image")
+            if not local_exists:
+                self.log.exception(e)
+                self.status = TaskStatus.NO_DOCKER_IMAGE
+                raise PermanentAlgorithmStartFail
+            else:
+                self.log.info("Using local image")
         except Exception as e:
-            self.log.debug("Failed to pull image")
-            self.log.exception(e)
-            self.status = TaskStatus.FAILED
-            raise PermanentAlgorithmStartFail
+            self.log.warning("Failed to pull image")
+            if not local_exists:
+                self.log.exception(e)
+                self.status = TaskStatus.FAILED
+                raise PermanentAlgorithmStartFail
+            else:
+                self.log.info("Using local image")
 
     def run(
         self,
         docker_input: bytes,
         tmp_vol_name: str,
         token: str,
         algorithm_env: dict,
@@ -270,15 +286,16 @@
             the algo container. None if VPN is inactive
         """
         vpn_ports = None
         container_name = f"{APPNAME}-{self.node_name}-run-{self.run_id}"
         helper_container_name = container_name + "-helper"
 
         # Try to pull the latest image
-        self.pull()
+        local_exists = len(self.docker.images.list(name=self.image)) > 0
+        self.pull(local_exists=local_exists)
 
         # remove algorithm containers if they were already running
         self.log.debug("Check if algorithm container is already running")
         remove_container_if_exists(docker_client=self.docker, name=container_name)
         remove_container_if_exists(
             docker_client=self.docker, name=helper_container_name
         )
@@ -655,9 +672,9 @@
                 .replace("=", ENV_VAR_EQUALS_REPLACEMENT)
             )
 
         self.log.debug("Encoding environment variables")
 
         encoded_environment_variables = {}
         for key, val in environment_variables.items():
-            encoded_environment_variables[key] = _encode(val)
+            encoded_environment_variables[key] = _encode(str(val))
         return encoded_environment_variables
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.4.0rc3/vantage6/node/docker/vpn_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from docker.models.containers import Container
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME, VPN_CONFIG_FILE
 from vantage6.common.docker.addons import (
     remove_container_if_exists,
     remove_container,
-    pull_if_newer,
+    pull_image,
 )
 from vantage6.common.docker.network_manager import NetworkManager
 from vantage6.node.globals import (
     MAX_CHECK_VPN_ATTEMPTS,
     NETWORK_CONFIG_IMAGE,
     VPN_CLIENT_IMAGE,
     FREE_PORT_RANGE,
@@ -97,17 +97,20 @@
         self.log.debug(f"  Config: {self.network_config_image}")
 
         self.has_vpn = False
 
     def _update_images(self) -> None:
         """Pulls the latest version of the VPN images"""
         self.log.info("Updating VPN images...")
-        pull_if_newer(self.docker, self.alpine_image, self.log)
-        pull_if_newer(self.docker, self.vpn_client_image, self.log)
-        pull_if_newer(self.docker, self.network_config_image, self.log)
+        self.log.debug("Pulling Alpine image")
+        pull_image(self.docker, self.alpine_image)
+        self.log.debug("Pulling VPN client image")
+        pull_image(self.docker, self.vpn_client_image)
+        self.log.debug("Pulling network config image")
+        pull_image(self.docker, self.network_config_image)
         self.log.info("Done updating VPN images")
 
     def connect_vpn(self) -> None:
         """
         Start VPN client container and configure network to allow
         algorithm-to-algoritm communication
         """
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/globals.py` & `vantage6-node-4.4.0rc3/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/proxy_server.py` & `vantage6-node-4.4.0rc3/vantage6/node/proxy_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,18 @@
     url = f"{server_url}/{endpoint}"
     for i in range(RETRY):
         try:
             response: Response = method(url, json=json, params=params, headers=headers)
             # verify that the server gave us a valid response, else we
             # would want to try again
             if response.status_code > 210:
-                log.warn("Proxy server received status code:" f"{response.status_code}")
+                log.warning(
+                    "Proxy server received status code %s", response.status_code
+                )
+                log.warning("Error messages: %s", response.json())
                 log.debug(
                     f"method: {request.method}, url: {url}, json: {json}"
                     f", params: {params}, headers: {headers}"
                 )
                 if "application/json" in response.headers.get("Content-Type"):
                     log.debug(response.json().get("msg", "no description..."))
```

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/socket.py` & `vantage6-node-4.4.0rc3/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6/node/util/colorer.py` & `vantage6-node-4.4.0rc3/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.3.4rc3/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.4.0rc3/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.3.4rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.4.0rc3 Summary: vantage6
 node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-node-4.3.4rc3/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.4.0rc3/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

