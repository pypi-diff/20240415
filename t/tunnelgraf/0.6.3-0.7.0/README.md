# Comparing `tmp/tunnelgraf-0.6.3.tar.gz` & `tmp/tunnelgraf-0.7.0.tar.gz`

## Comparing `tunnelgraf-0.6.3.tar` & `tunnelgraf-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/Makefile
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/README.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/cli.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/tunnelgraf.spec
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tests/test_tunnel_def.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/__init__.py
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/__main__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/lastpass_secrets.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/tunnel_builder.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/tunnel_definition.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/src/tunnelgraf/tunnels.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/LICENSE
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/Makefile
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/README.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/cli.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/tunnelgraf.spec
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tests/test_tunnel_def.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/__init__.py
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/__main__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/lastpass_secrets.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/nslookup.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/run_remote.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnel_builder.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnel_definition.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/src/tunnelgraf/tunnels.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 tunnelgraf-0.7.0/PKG-INFO
```

### Comparing `tunnelgraf-0.6.3/Makefile` & `tunnelgraf-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/README.md` & `tunnelgraf-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -195,7 +195,30 @@
 ```json
 {
   "jumpbox": ["ssh://<ip address>:22"],
   "jumpbox2": ["ssh://<domain name>:2224"],
   "load_balancer": ["https://<fqdn>.local:8443", "https://<fqdn2>:8443"]
 }
 ```
+
+## Resolve Remote DNS
+
+Often, especially in cloud/kubernetes environments, the remote IP is unknown and
+the nameserver to resolve it with (e.g. coredns) is not configured in the remote
+host's dns client configuration. In such examples, use "hostlookup" and
+"nameserver" to dynamically fetch the remote IP address of the endpoint.
+
+```yaml
+---
+id: staging_env_bastion
+port: 22
+sshuser: <some user>
+sshkeyfile: <path to some key file>
+localbindport: 2223 # top layer takes precedence
+nexthops:
+  - id: an_app_node
+    hostlookup: <some fqdn>
+    nameserver: <an address of the nameserver>
+    port: 443
+    localbindport: 8443
+    hosts_file_entry: <some fqdn>
+```
```

### Comparing `tunnelgraf-0.6.3/tunnelgraf.spec` & `tunnelgraf-0.7.0/tunnelgraf.spec`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/src/tests/test_tunnel_def.py` & `tunnelgraf-0.7.0/src/tests/test_tunnel_def.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/src/tunnelgraf/__init__.py` & `tunnelgraf-0.7.0/src/tunnelgraf/__init__.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/src/tunnelgraf/lastpass_secrets.py` & `tunnelgraf-0.7.0/src/tunnelgraf/lastpass_secrets.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/src/tunnelgraf/tunnel_builder.py` & `tunnelgraf-0.7.0/src/tunnelgraf/tunnel_builder.py`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/src/tunnelgraf/tunnel_definition.py` & `tunnelgraf-0.7.0/src/tunnelgraf/tunnel_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     port: Optional[int] = Field(22, alias="port")  # Not Required
     localbindaddress: Optional[str] = Field("127.0.0.1", alias="localbindaddress")
     localbindport: int = Field(..., alias="localbindport")  # Required field
     protocol: Optional[str] = Field("ssh", alias="protocol")  # Not required
     sshuser: Optional[str] = Field(None, alias="sshuser")  # Not required
     sshpass: Optional[str] = Field(None, alias="sshpass")  # Not required
     sshkeyfile: Optional[str] = Field(None, alias="sshkeyfile")  # Not required
+    hostlookup: Optional[str] = Field(None, alias="hostlookup")  # Not required
+    nameserver: Optional[str] = Field(None, alias="nameserver")  # Not required
     lastpass: Optional[str] = Field(
         None, alias="lastpass"
     )  # Required or None allowed with alias
     hosts_file_entry: Optional[str] = Field(
         None, alias="hosts_file_entry"
     )  # Not required
     hosts_file_entries: List[Optional[str]] = Field(
```

### Comparing `tunnelgraf-0.6.3/src/tunnelgraf/tunnels.py` & `tunnelgraf-0.7.0/src/tunnelgraf/tunnels.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from pathlib import Path
 
 import yaml
 from python_hosts import Hosts, HostsEntry, HostsException
 
 from tunnelgraf.tunnel_builder import TunnelBuilder
 from tunnelgraf.tunnel_definition import TunnelDefinition
+from tunnelgraf.run_remote import RunCommand
+from tunnelgraf.nslookup import NSLookup
 
 
 class Tunnels:
     """
     Creates an ssh tunnel, connecting a remote endpoint through a bastion
     and binding it to a local port, as specified in the provided config file.
     """
@@ -114,17 +116,20 @@
             for tunnel in self.tunnel_defs:
                 self.make_tunnel(tunnel)
         if isinstance(self.tunnel_defs, TunnelDefinition):
             self.make_tunnel(self.tunnel_defs)
 
     def make_tunnel(self, this_tunnel_def: TunnelDefinition):
         """Creates a tunnel from the provided config."""
+
         self._add_to_processed_configs(this_tunnel_def)
         if this_tunnel_def.nexthop is not None:
             if self._connect_tunnels:
+                if this_tunnel_def.nexthop.hostlookup is not None:
+                    this_tunnel_def.nexthop.host = self._lookup_host(this_tunnel_def)
                 self.tunnels.append(TunnelBuilder(this_tunnel_def))
                 tc = self.tunnels[-1].tunnel
                 print(
                     f"Created tunnel {this_tunnel_def.id}: {tc.local_bind_host}:{tc.local_bind_port} to {tc._remote_binds[0][0]}:{tc._remote_binds[0][1]}"
                 )
             self._add_to_hosts(
                 this_tunnel_def.nexthop.id,
@@ -139,14 +144,29 @@
             for tunnel in this_tunnel_def.nexthops:
                 nexthop_config = this_tunnel_def
                 nexthop_config.nexthop = tunnel
                 nexthop_config.nexthops = None
                 nexthop_config = self._update_bastion_address(nexthop_config)
                 self.make_tunnel(nexthop_config)
 
+    def _lookup_host(self, this_tunnel_def: TunnelDefinition) -> str | None:
+        print(f"Looking up {this_tunnel_def.nexthop.hostlookup}...")
+        this_connection = RunCommand(
+            host=this_tunnel_def.host,
+            user=this_tunnel_def.sshuser,
+            identityfile=this_tunnel_def.sshkeyfile,
+            password=this_tunnel_def.sshpass,
+            port=this_tunnel_def.localbindport,
+        )
+        return NSLookup(
+            record=this_tunnel_def.nexthop.hostlookup,
+            nameserver=this_tunnel_def.nexthop.nameserver,
+            connection=this_connection,
+        ).host_ip
+
     def _add_to_processed_configs(self, this_tunnel_def: TunnelDefinition):
         """Adds a tunnel to the processed configs."""
         if not any(this_tunnel_def.id == t["id"] for t in self.tunnel_configs):
             self.tunnel_configs.append(
                 this_tunnel_def.model_dump(exclude=self._excluded_fields)
             )
```

### Comparing `tunnelgraf-0.6.3/LICENSE` & `tunnelgraf-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tunnelgraf-0.6.3/pyproject.toml` & `tunnelgraf-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tunnelgraf"
-version = "0.6.3"
+version = "0.7.0"
 dependencies = [
   "click~=8.0.0",
   "sshtunnel~=0.4.0",
   "pyyaml~=6.0.0",
   "python-hosts~=1.0.5",
   "pydantic~=2.5.0",
   "paramiko~=3.4.0",
```

### Comparing `tunnelgraf-0.6.3/PKG-INFO` & `tunnelgraf-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tunnelgraf
-Version: 0.6.3
+Version: 0.7.0
 Summary: Hierarchical SSH tunnel management made easy. Securely define and share multihop connection profiles that expose a graph of remote endpoints as localhost.
 Project-URL: Homepage, https://github.com/denniswalker/tunnelgraf
 Project-URL: Documentation, https://github.com/denniswalker/tunnelgraf/blob/main/README.md
 Project-URL: Repository, https://github.com/denniswalker/tunnelgraf
 Project-URL: Issues, https://github.com/denniswalker/tunnelgraf/issues
 Author-email: Dennis Walker <denniswalker@me.com>
 Maintainer-email: Dennis Walker <denniswalker@me.com>
```

