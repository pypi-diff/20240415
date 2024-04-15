# Comparing `tmp/gefyra-2.0.1.tar.gz` & `tmp/gefyra-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-2.0.1.tar", max compression
+gzip compressed data, was "gefyra-2.0.3.tar", max compression
```

## Comparing `gefyra-2.0.1.tar` & `gefyra-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2151 2023-09-28 13:17:40.330104 gefyra-2.0.1/README.md
--rw-r--r--   0        0        0        0 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/__init__.py
--rw-r--r--   0        0        0      239 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/__init__.py
--rw-r--r--   0        0        0     8859 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/bridge.py
--rw-r--r--   0        0        0     3980 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/clients.py
--rw-r--r--   0        0        0    10466 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/connect.py
--rw-r--r--   0        0        0     5845 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/install.py
--rw-r--r--   0        0        0     3066 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/list.py
--rw-r--r--   0        0        0     2797 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/reflect.py
--rw-r--r--   0        0        0     4361 2023-09-28 13:17:40.330104 gefyra-2.0.1/gefyra/api/run.py
--rw-r--r--   0        0        0     5375 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/api/status.py
--rw-r--r--   0        0        0     2177 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/__init__.py
--rw-r--r--   0        0        0     4298 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/bridge.py
--rw-r--r--   0        0        0     3763 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/clients.py
--rw-r--r--   0        0        0     5310 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/connections.py
--rw-r--r--   0        0        0      268 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/console.py
--rw-r--r--   0        0        0     2800 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/installation.py
--rw-r--r--   0        0        0     2937 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/list.py
--rw-r--r--   0        0        0     2293 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/main.py
--rw-r--r--   0        0        0     2239 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/run.py
--rw-r--r--   0        0        0      217 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/status.py
--rw-r--r--   0        0        0     4859 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/telemetry.py
--rw-r--r--   0        0        0     7341 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/updown.py
--rw-r--r--   0        0        0     7957 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/utils.py
--rw-r--r--   0        0        0     1024 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cli/version.py
--rw-r--r--   0        0        0        0 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     4642 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     5385 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/cluster/utils.py
--rw-r--r--   0        0        0    13270 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/configuration.py
--rw-r--r--   0        0        0      516 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/exceptions.py
--rw-r--r--   0        0        0      441 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6497 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/bridge.py
--rw-r--r--   0        0        0     1927 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/cargo.py
--rw-r--r--   0        0        0     4168 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/clients.py
--rw-r--r--   0        0        0     2237 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4594 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/networking.py
--rw-r--r--   0        0        0     4354 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/local/utils.py
--rw-r--r--   0        0        0        0 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/__init__.py
--rw-r--r--   0        0        0      214 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/__init__.py
--rw-r--r--   0        0        0     4741 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/deployment.py
--rw-r--r--   0        0        0      331 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/namespace.py
--rw-r--r--   0        0        0     3200 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/rbac.py
--rw-r--r--   0        0        0     2106 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/service.py
--rw-r--r--   0        0        0     4530 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/comps/webhook.py
--rw-r--r--   0        0        0     1583 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/install.py
--rw-r--r--   0        0        0     2887 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/uninstall.py
--rw-r--r--   0        0        0      486 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/misc/utils.py
--rw-r--r--   0        0        0    10557 2023-09-28 13:17:40.334104 gefyra-2.0.1/gefyra/types.py
--rw-r--r--   0        0        0     1840 2023-09-28 13:17:40.334104 gefyra-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 gefyra-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2151 2024-04-15 16:00:54.898460 gefyra-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     8859 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     3981 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/clients.py
+-rw-r--r--   0        0        0    10466 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/connect.py
+-rw-r--r--   0        0        0     5845 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/install.py
+-rw-r--r--   0        0        0     3066 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/list.py
+-rw-r--r--   0        0        0     2797 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     4422 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/run.py
+-rw-r--r--   0        0        0     5375 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/status.py
+-rw-r--r--   0        0        0     2179 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/__init__.py
+-rw-r--r--   0        0        0     4298 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/bridge.py
+-rw-r--r--   0        0        0     3763 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/clients.py
+-rw-r--r--   0        0        0     5310 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/connections.py
+-rw-r--r--   0        0        0      268 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/console.py
+-rw-r--r--   0        0        0     2800 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/installation.py
+-rw-r--r--   0        0        0     2937 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/list.py
+-rw-r--r--   0        0        0     2293 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/main.py
+-rw-r--r--   0        0        0     2261 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/run.py
+-rw-r--r--   0        0        0      217 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/status.py
+-rw-r--r--   0        0        0     4859 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/telemetry.py
+-rw-r--r--   0        0        0     7345 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/updown.py
+-rw-r--r--   0        0        0     7961 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/utils.py
+-rw-r--r--   0        0        0     1024 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/version.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     4642 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     5385 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0    13270 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/configuration.py
+-rw-r--r--   0        0        0      516 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/exceptions.py
+-rw-r--r--   0        0        0      441 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6579 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     1927 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/cargo.py
+-rw-r--r--   0        0        0     4167 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/clients.py
+-rw-r--r--   0        0        0     2237 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4594 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/networking.py
+-rw-r--r--   0        0        0     4354 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/utils.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/__init__.py
+-rw-r--r--   0        0        0     4741 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/deployment.py
+-rw-r--r--   0        0        0      331 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/namespace.py
+-rw-r--r--   0        0        0     3200 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/rbac.py
+-rw-r--r--   0        0        0     2106 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/service.py
+-rw-r--r--   0        0        0     4530 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/webhook.py
+-rw-r--r--   0        0        0     1583 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/install.py
+-rw-r--r--   0        0        0     2887 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/uninstall.py
+-rw-r--r--   0        0        0      486 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/utils.py
+-rw-r--r--   0        0        0    10557 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/types.py
+-rw-r--r--   0        0        0     1849 2024-04-15 16:00:54.902460 gefyra-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 gefyra-2.0.3/PKG-INFO
```

### Comparing `gefyra-2.0.1/README.md` & `gefyra-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/bridge.py` & `gefyra-2.0.3/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/clients.py` & `gefyra-2.0.3/gefyra/api/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ) -> bool:
     """
     Delete a GefyraClient configuration
     """
     config = ClientConfiguration(
         kube_config_file=kubeconfig,
         kube_context=kubecontext,
-        connection_name=connection_name if connection_name else "no-connection-name"
+        connection_name=connection_name if connection_name else "no-connection-name",
         # use no-connection-name to make sure you use admin access to the cluster
     )
     return handle_delete_gefyraclient(config, client_id, force, wait=wait)
 
 
 @stopwatch
 def write_client_file(
```

### Comparing `gefyra-2.0.1/gefyra/api/connect.py` & `gefyra-2.0.3/gefyra/api/connect.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/install.py` & `gefyra-2.0.3/gefyra/api/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/list.py` & `gefyra-2.0.3/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/reflect.py` & `gefyra-2.0.3/gefyra/api/reflect.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/run.py` & `gefyra-2.0.3/gefyra/api/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 
         _, active_context = kube_config.list_kube_config_contexts()
         namespace = active_context["context"].get("namespace") or "default"
         ns_source = "kubeconfig"
     else:
         ns_source = "--namespace argument"
 
-    dns_search = f"{namespace}.svc.cluster.local"
+    dns_search = (
+        f"{namespace}.svc.cluster.local svc.cluster.local cluster.local k8s".split(" ")
+    )
     #
     # Confirm the wireguard connection working
     #
     try:
         probe_wireguard_connection(config)
     except Exception as e:
         logger.error(e)
@@ -113,15 +115,15 @@
             env=env_dict,
             dns_search=dns_search,
             auto_remove=auto_remove,
             volumes=volumes,
         )
     except APIError as e:
         if e.status_code == 409:
-            logger.warning(e.explanation)
+            logger.error(e.explanation)
             return True
         else:
             raise RuntimeError(e.explanation)
 
     logger.info(
         f"Container image '{', '.join(container.image.tags)}' started with name"
         f" '{container.name}' in Kubernetes namespace '{namespace}' (from {ns_source})"
```

### Comparing `gefyra-2.0.1/gefyra/api/status.py` & `gefyra-2.0.3/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/api/utils.py` & `gefyra-2.0.3/gefyra/api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 
 def stopwatch(func):
     def wrapper(*args, **kwargs):
         tic = time.perf_counter()
         result = func(*args, **kwargs)
         toc = time.perf_counter()
         logger.debug(
-            f"Operation time for '{func.__name__}(...)' was {(toc - tic)*1000:0.4f}ms"
+            f"Operation time for '{func.__name__}(...)' was {(toc - tic) * 1000:0.4f}ms"
         )
         return result
 
     return wrapper
```

### Comparing `gefyra-2.0.1/gefyra/cli/bridge.py` & `gefyra-2.0.3/gefyra/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/clients.py` & `gefyra-2.0.3/gefyra/cli/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             c.state_transitions.get("CREATING", "Creating..."),
         ]
         for c in gefyraclients
     ]
     click.echo(tabulate(clients, headers=["ID", "STATE", "CREATED"], tablefmt="plain"))
 
 
-@clients.command("inspect", alias=["show", "get"], help="Discribe a Gefyra client")
+@clients.command("inspect", alias=["show", "get"], help="Describe a Gefyra client")
 @click.argument("client_id")
 @click.pass_context
 @standard_error_handler
 def inspect_client(ctx, client_id):
     from gefyra import api
 
     client = api.get_client(
```

### Comparing `gefyra-2.0.1/gefyra/cli/connections.py` & `gefyra-2.0.3/gefyra/cli/connections.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/installation.py` & `gefyra-2.0.3/gefyra/cli/installation.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/list.py` & `gefyra-2.0.3/gefyra/cli/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/main.py` & `gefyra-2.0.3/gefyra/cli/main.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/run.py` & `gefyra-2.0.3/gefyra/cli/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,17 @@
     help="The name of the container running in Gefyra",
     type=str,
     required=True,
 )
 @click.option(
     "-i", "--image", help="The docker image to run in Gefyra", type=str, required=True
 )
-@click.option("--connection-name", type=str, callback=check_connection_name)
+@click.option(
+    "--connection-name", type=str, callback=check_connection_name, required=False
+)
 def run(
     detach,
     auto_remove,
     expose,
     env_from,
     volume,
     env,
```

### Comparing `gefyra-2.0.1/gefyra/cli/telemetry.py` & `gefyra-2.0.3/gefyra/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cli/updown.py` & `gefyra-2.0.3/gefyra/cli/updown.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             except ClientConfigurationError as e:
                 logger.warning(e)
                 sleep(1)
                 _i += 1
         else:
             raise ClientConfigurationError(
                 f"Could not set up the client '{client_id}'. This is most probably a problem of Gefyra operator. \n"
-                f"Try running 'gefyra up{' --preset '+preset if preset else ''}' again after some time."
+                f"Try running 'gefyra up{' --preset ' + preset if preset else ''}' again after some time."
             )
 
         # create a temporary file with the client config
         loc = os.path.join(
             get_gefyra_config_location(),
             f"{connection_name}_client.json",
         )
@@ -159,15 +159,15 @@
                 probe_timeout=180,
             )
         except GefyraConnectionError as e:
             raise GefyraConnectionError(
                 f"Gefyra could not successfully establish the connection to '{config.CARGO_ENDPOINT.split(':')[0]}'.\n"
                 "If you have run 'gefyra up' with a remote cluster, a newly created route may not be working "
                 "immediately.\n"
-                f"Try running 'gefyra up{' --preset '+preset if preset else ''}' again after some time. "
+                f"Try running 'gefyra up{' --preset ' + preset if preset else ''}' again after some time. "
                 f"Error: {e}"
             ) from None
         fh.close()
         os.remove(loc)
         bar()
         bar.title = "Gefyra is ready"
```

### Comparing `gefyra-2.0.1/gefyra/cli/utils.py` & `gefyra-2.0.3/gefyra/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             if cmd.hidden:
                 continue
 
             if hasattr(acmd, "alias"):
                 alias = ",".join(acmd.alias)
             else:
                 alias = None
-            commands.append((f"{subcommand} {'('+alias+')' if alias else ''}", cmd))
+            commands.append((f"{subcommand} {'(' + alias + ')' if alias else ''}", cmd))
 
         # allow for 3 times the default spacing
         if len(commands):
             limit = formatter.width - 6 - max(len(cmd[0]) for cmd in commands)
 
             rows = []
             for subcommand, cmd in commands:
```

### Comparing `gefyra-2.0.1/gefyra/cli/version.py` & `gefyra-2.0.3/gefyra/cli/version.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cluster/resources.py` & `gefyra-2.0.3/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/cluster/utils.py` & `gefyra-2.0.3/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/configuration.py` & `gefyra-2.0.3/gefyra/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     CARGO_ENDPOINT_LABEL,
     ACTIVE_KUBECONFIG_LABEL,
     CLIENT_ID_LABEL,
 )
 
 logger = logging.getLogger("gefyra")
 
-__VERSION__ = "2.0.1"
+__VERSION__ = "2.0.3"
 USER_HOME = os.path.expanduser("~")
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
```

### Comparing `gefyra-2.0.1/gefyra/exceptions.py` & `gefyra-2.0.3/gefyra/exceptions.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/local/bridge.py` & `gefyra-2.0.3/gefyra/local/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             plural="gefyrabridges",
             version="v1",
         )
     except ApiException as e:
         if e.status == 409:
             raise RuntimeError(f"Workload {target} already bridged.")
         logger.error(
-            f"A Kubernetes API Error occured. \nReason:{e.reason} \nBody:{e.body}"
+            f"A Kubernetes API Error occured. \nReason: {e.reason} \nBody: {e.body}"
         )
         raise e from None
     return ireq
 
 
 def handle_delete_gefyrabridge(config: ClientConfiguration, name: str) -> bool:
     from kubernetes.client import ApiException
@@ -135,34 +135,37 @@
     image: str,
     name: str = "",
     command: str = "",
     volumes: Optional[List] = None,
     ports: Optional[Dict] = None,
     env: Optional[Dict] = None,
     auto_remove: bool = False,
-    dns_search: str = "default",
+    dns_search: Optional[List[str]] = None,
 ) -> Container:
     import docker
 
+    if not dns_search:
+        dns_search = ["default"]
+
     gefyra_net = config.DOCKER.networks.get(f"{config.NETWORK_NAME}")
 
     net_add = gefyra_net.attrs["IPAM"]["Config"][0]["Subnet"].split("/")[0]
     cargo_ip = get_cargo_ip_from_netaddress(net_add)
     all_kwargs = {
         "network": config.NETWORK_NAME,
         "name": name,
         "command": command,
         "volumes": volumes,
         "ports": ports,
         "detach": True,
         "dns": [config.STOWAWAY_IP],
-        "dns_search": [dns_search],
+        "dns_search": dns_search,
         "auto_remove": auto_remove,
         "environment": env,
-        "pid_mode": f"container:{config.CARGO_CONTAINER_NAME}",
+        "pid_mode": f"container:{config.CARGO_CONTAINER_NAME}",  # noqa: E231
     }
     not_none_kwargs = {k: v for k, v in all_kwargs.items() if v is not None}
 
     container = handle_docker_run_container(config, image, **not_none_kwargs)
 
     cargo = config.DOCKER.containers.get(config.CARGO_CONTAINER_NAME)
```

### Comparing `gefyra-2.0.1/gefyra/local/cargo.py` & `gefyra-2.0.3/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/local/clients.py` & `gefyra-2.0.3/gefyra/local/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             name=client_id,
             group="gefyra.dev",
             plural="gefyraclients",
             version="v1",
         )
     except ApiException as e:
         if e.status in [404, 403]:
-            raise GefyraClientNotFound(f"Client {client_id} does not exists.")
+            raise GefyraClientNotFound(f"Client {client_id} does not exist.")
         else:
             logger.error(
                 f"A Kubernetes API Error occured. \nReason:{e.reason} \nBody:{e.body}"
             )
             raise e
     except urllib3.exceptions.MaxRetryError as e:
         # this connection does not work (at the moment)
```

### Comparing `gefyra-2.0.1/gefyra/local/minikube.py` & `gefyra-2.0.3/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/local/networking.py` & `gefyra-2.0.3/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/local/utils.py` & `gefyra-2.0.3/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/comps/deployment.py` & `gefyra-2.0.3/gefyra/misc/comps/deployment.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/comps/rbac.py` & `gefyra-2.0.3/gefyra/misc/comps/rbac.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/comps/service.py` & `gefyra-2.0.3/gefyra/misc/comps/service.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/comps/webhook.py` & `gefyra-2.0.3/gefyra/misc/comps/webhook.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/install.py` & `gefyra-2.0.3/gefyra/misc/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/misc/uninstall.py` & `gefyra-2.0.3/gefyra/misc/uninstall.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/gefyra/types.py` & `gefyra-2.0.3/gefyra/types.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.1/pyproject.toml` & `gefyra-2.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "2.0.1"
+version = "2.0.3"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@blueshoe.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
@@ -18,27 +18,27 @@
     "Topic :: Software Development :: Build Tools",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-kubernetes = ">=24.2,<29.0"
-docker = "^6.0.0"
+kubernetes = ">=24.2,<30.0"
+docker = ">=6,<8"
 
 [tool.poetry.group.cli.dependencies]
 cli-tracker = ">=0.2.7,<0.4.0"
 tabulate = ">=0.8.10,<0.10.0"
 alive-progress = "^3.1.4"
 click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
-flake8-bugbear = "^23.3.12"
-black = "^23.1.0"
-flake8 = "^6.0.0"
+flake8-bugbear = ">=23.3.12,<25.0.0"
+black = "^24.2.0"
+flake8 = "^7.0.0"
 flake8-black = "^0.3.6"
 pytest = "^7.2.2"
 coverage = {extras = ["toml"], version = "^6.5.0"}
 coveralls = "^3.3.1"
 pytest-kubernetes = ">=0.2,<0.4"
 mypy = "^1.3.0"
 types-tabulate = "^0.9.0.2"
```

### Comparing `gefyra-2.0.1/PKG-INFO` & `gefyra-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: Gefyra
-Version: 2.0.1
+Version: 2.0.3
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@blueshoe.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Dist: docker (>=6.0.0,<7.0.0)
-Requires-Dist: kubernetes (>=24.2,<29.0)
+Requires-Dist: docker (>=6,<8)
+Requires-Dist: kubernetes (>=24.2,<30.0)
 Project-URL: Documentation, https://gefyra.dev
 Project-URL: Repository, https://github.com/gefyrahq/gefyra
 Project-URL: issues, https://github.com/gefyrahq/gefyra/issues
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/Schille/gefyra/raw/main/docs/static/img/logo.png" alt="Gefyra Logo"/>
```

