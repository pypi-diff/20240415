# Comparing `tmp/pytest-inmanta-lsm-3.2.0.tar.gz` & `tmp/pytest_inmanta_lsm-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-inmanta-lsm-3.2.0.tar", last modified: Tue Feb 20 13:05:33 2024, max compression
+gzip compressed data, was "pytest_inmanta_lsm-3.3.0.tar", last modified: Mon Apr 15 13:33:15 2024, max compression
```

## Comparing `pytest-inmanta-lsm-3.2.0.tar` & `pytest_inmanta_lsm-3.3.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.007984 pytest-inmanta-lsm-3.2.0/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     5499 2024-02-20 13:05:24.000000 pytest-inmanta-lsm-3.2.0/CHANGELOG.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       86 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/LICENSE
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       12 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/MANIFEST.in
--rw-r--r--   0 jenkins    (988) jenkins    (986)    13328 2024-02-20 13:05:33.007984 pytest-inmanta-lsm-3.2.0/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    12394 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/README.md
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      228 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/pyproject.toml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      610 2024-02-20 13:05:33.007984 pytest-inmanta-lsm-3.2.0/setup.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1818 2024-02-20 13:05:24.000000 pytest-inmanta-lsm-3.2.0/setup.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.003983 pytest-inmanta-lsm-3.2.0/src/
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.005983 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      775 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/__init__.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1847 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/exceptions.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     2635 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/failed_resources_logs.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    12309 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/lsm_project.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    18070 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/managed_service_instance.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     9638 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/orchestrator_container.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     6798 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/parameters.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    18147 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/plugin.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/py.typed
--rw-rw-r--   0 jenkins    (988) jenkins    (986)    31896 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/remote_orchestrator.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.006983 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)      773 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/docker-compose.yml
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       25 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/my-env-file
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     3444 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     3517 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/setup_project.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     7957 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/wait_for_state.py
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.006983 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/
--rw-r--r--   0 jenkins    (988) jenkins    (986)    13328 2024-02-20 13:05:32.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1091 2024-02-20 13:05:33.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-02-20 13:05:32.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       51 2024-02-20 13:05:32.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       41 2024-02-20 13:05:32.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (988) jenkins    (986)       19 2024-02-20 13:05:32.000000 pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-02-20 13:05:33.006983 pytest-inmanta-lsm-3.2.0/tests/
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1014 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/tests/test_basic_example.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     2516 2024-02-20 13:05:13.000000 pytest-inmanta-lsm-3.2.0/tests/test_containerized_orchestrator.py
--rw-rw-r--   0 jenkins    (988) jenkins    (986)     1893 2024-02-20 13:05:22.000000 pytest-inmanta-lsm-3.2.0/tests/test_partial.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     6731 2024-04-15 13:33:11.000000 pytest_inmanta_lsm-3.3.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       86 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/LICENSE
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       12 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (988) jenkins    (986)    20261 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    19327 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/README.md
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      228 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      610 2024-04-15 13:33:15.755594 pytest_inmanta_lsm-3.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1818 2024-04-15 13:33:11.000000 pytest_inmanta_lsm-3.3.0/setup.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.751594 pytest_inmanta_lsm-3.3.0/src/
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.753594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      775 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/__init__.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1847 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/exceptions.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2635 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/failed_resources_logs.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    42233 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/lsm_project.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    18098 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/managed_service_instance.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     9905 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/orchestrator_container.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     7956 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/parameters.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    19222 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/plugin.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/py.typed
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    36800 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_orchestrator.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2915 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     9257 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance.pyi
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)    23508 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_service_instance_async.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      773 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/docker-compose.yml
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       25 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-env-file
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3444 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3517 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/setup_project.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     3421 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/util.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     7957 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/wait_for_state.py
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/
+-rw-r--r--   0 jenkins    (988) jenkins    (986)    20261 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1279 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)        1 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       51 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       41 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)       19 2024-04-15 13:33:15.000000 pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (988) jenkins    (986)        0 2024-04-15 13:33:15.754594 pytest_inmanta_lsm-3.3.0/tests/
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)      840 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/tests/test_basic_example.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     2342 2024-04-15 13:33:09.000000 pytest_inmanta_lsm-3.3.0/tests/test_containerized_orchestrator.py
+-rw-rw-r--   0 jenkins    (988) jenkins    (986)     1893 2024-04-15 13:32:59.000000 pytest_inmanta_lsm-3.3.0/tests/test_partial.py
```

### Comparing `pytest-inmanta-lsm-3.2.0/CHANGELOG.md` & `pytest_inmanta_lsm-3.3.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# v 3.3.0 (2024-04-15)
+Changes in this release:
+- Better logs when `docker-compose` in not installed
+- Add async `RemoteServiceInstance` class, for async service testing.
+- Add `export_service_entities` helper to `LsmProject` class.  Allowing to test the definition of a service.  (#352)
+- Allow to easily reuse model used in `export_service_entities` for all later compiles.
+- Validate that any service added to the `LsmProject` object using `add_service` method is part of one of the exported services. (#354)
+- Add `LsmProject` helpers to facilitate partial compile testing (#380)
+- Add `LsmProject` helpers to facilitate service creation and update:
+    - Fill in default attribute values.
+    - Determine initial state automatically.
+    - Follow the first "auto" state transfers, running the corresponding compiles, and applying the corresponding attribute operations.
+- Extend `LsmProject` mocking capability to allow partial compile selection testing.
+- Add `--lsm-rsh` and `--lsm-rh` to support remote access to a local container without ssh.
+- Add `remote_orchestrator_access` fixture, which sets up a remote orchestrator object allowing us to interact with the remote environment, but doesn't do any cleanup on its own.
+
 # v 3.2.0 (2024-02-20)
 Changes in this release:
 - Update default tags of ISO and postgres containers
 
 # v 3.1.0 (2023-11-29)
 Changes in this release:
 - Ignore `__pycache__` dirs when rsyncing the project to the remote orchestrator
```

### Comparing `pytest-inmanta-lsm-3.2.0/PKG-INFO` & `pytest_inmanta_lsm-3.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-lsm
-Version: 3.2.0
+Version: 3.3.0
 Summary: Common fixtures for inmanta LSM related modules
 Home-page: https://github.com/inmanta/pytest-inmanta-lsm
 Author: Inmanta
 Author-email: code@inmanta.com
 License: inmanta EULA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -22,14 +22,16 @@
 License-File: LICENSE
 Requires-Dist: pytest-inmanta~=2.5
 Requires-Dist: inmanta-lsm
 Requires-Dist: devtools
 
 # pytest-inmanta-lsm
 
+[![pypi version](https://img.shields.io/pypi/v/pytest-inmanta-lsm.svg)](https://pypi.python.org/pypi/pytest-inmanta-lsm/)
+
 A pytest plugin to test inmanta modules that use lsm, it is built on top of `pytest-inmanta` and `pytest-inmanta-extensions`
 
 ## Installation
 
 ```bash
 pip install pytest-inmanta-lsm
 ```
@@ -39,97 +41,243 @@
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
 ### First case: using a remote orchestrator
 
-This plugin is built around the remote_orchestrator fixture.
+This plugin is built around the remote_orchestrator fixture and the `RemoteServiceInstance` class.
 
-A typical testcase using this plugin looks as follows:
+You can easily write a test case that sends your project to a remote orchestrator, exports its service catalog, then deploy a service.  
 ```python
-
-def test_full_cycle(project, remote_orchestrator):
+def test_deploy_service(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
 
     # setup project
-    project.compile(
-        """
-        import quickstart
-        """
-    )
+    project.compile("import quickstart")
 
     # sync project and export service entities
     remote_orchestrator.export_service_entities()
 
     # verify the service is in the catalog
     result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
     assert result.code == 200
 
-    # get a ManagedInstance object, to simplifies interacting with a specific service instance
-    service_instance = remote_orchestrator.get_managed_instance(SERVICE_NAME)
+    # Test the synchronous service instance class
+    instance = remote_service_instance.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
+    )
 
-    # create an instance and wait for it to be up
-    service_instance.create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="up",
+    # Create the service instance and stop waiting in a transient state
+    created = instance.create(
+        {
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        wait_for_state="creating",
+        timeout=60,
+    )
+
+    # Wait for up state, we provide here the version from which we should follow the
+    # service, which is the version in which we last stopped following the service.  This
+    # guarantees that we don't "miss" the target state, in case it is a transient one, and
+    # don't confuse the start state for the target one in case it is the same one.
+    # The start version should always be the last version in which we know our service has
+    # been, BEFORE the target state we expect our service to go into.
+    instance.wait_for_state(
+        target_state="up",
+        start_version=created.version,
+        timeout=60,
+    )
+
+    # Delete the instance
+    instance.delete(wait_for_state="terminated", timeout=60)
+```
+> source: [test_quickstart.py::test_transient_state](./examples/quickstart/tests/test_quickstart.py)
+
+For a more advanced test case, you might also want to deploy multiple services.  You could either test them one by one, or, parallelize them, in order to:
+1. speed up the test case.
+2. test interference in between the services.
+
+In that case, the recommended way is to create an `async` helper, which follows the progress of your service, and instantiate multiple services with it, in a `sync` test case.
+```python
+async def service_full_cycle(
+    remote_orchestrator: remote_orchestrator.RemoteOrchestrator,
+    router_ip: str,
+    interface_name: str,
+    address: str,
+    vlan_id: int,
+    vlan_id_update: int,
+) -> None:
+    # Create an async service instance object
+    instance = remote_service_instance_async.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
     )
 
-    # make validation fail by creating a duplicate
-    remote_orchestrator.get_managed_instance(SERVICE_NAME).create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="rejected",
+    # Create the service instance on the remote orchestrator
+    await instance.create(
+        {
+            "router_ip": router_ip,
+            "interface_name": interface_name,
+            "address": address,
+            "vlan_id": vlan_id,
+        },
+        wait_for_state="up",
+        timeout=60,
     )
 
-    service_instance.update(
-        attribute_updates={"vlan_id": 42},
+    # Update the vlan id
+    await instance.update(
+        [
+            inmanta_lsm.model.PatchCallEdit(
+                edit_id=str(uuid.uuid4()),
+                operation=inmanta_lsm.model.EditOperation.replace,
+                target="vlan_id",
+                value=vlan_id_update,
+            ),
+        ],
         wait_for_state="up",
+        timeout=60,
+    )
+
+    # Delete the instance
+    await instance.delete(wait_for_state="terminated", timeout=60)
+
+
+def test_full_cycle(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
+    # get connection to remote_orchestrator
+    client = remote_orchestrator.client
+
+    # setup project
+    project.compile("import quickstart")
+
+    # sync project and export service entities
+    remote_orchestrator.export_service_entities()
+
+    # verify the service is in the catalog
+    result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
+    assert result.code == 200
+
+    # Create a first service that should be deployed
+    first_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.17",
+        interface_name="eth1",
+        address="10.0.0.254/24",
+        vlan_id=14,
+        vlan_id_update=42,
     )
 
-    # break it down
-    service_instance.delete()
+    # Create another valid service
+    another_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.18",
+        interface_name="eth2",
+        address="10.0.0.253/24",
+        vlan_id=15,
+        vlan_id_update=52,
+    )
 
+    # Run all the services
+    util.sync_execute_scenarios(first_service, another_service, timeout=60)
 ```
+> source: [test_quickstart.py::test_full_cycle](./examples/quickstart/tests/test_quickstart.py)
+
 
 ### Second case: mocking the lsm api
 
 This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
  - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
  - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
  - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
 
 A simple usage would be as follow:
 ```python
-def test_model(lsm_project: lsm_project.LsmProject) -> None:
-    # Create a service object, you can modify it as you wish, depending on what you are trying to test
-    service = inmanta_lsm.model.ServiceInstance(
-        id=uuid.uuid4(),
-        environment=lsm_project.environment,
-        service_entity="vlan-assignment",
-        version=1,
-        config={},
-        state="start",
-        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        active_attributes=None,
-        rollback_attributes=None,
-        created_at=datetime.datetime.now(),
-        last_updated=datetime.datetime.now(),
-        callback=[],
-        deleted=False,
-        deployment_progress=None,
-        service_identity_attribute_value=None,
-    )
-
-    # Add the service to the mocked server.  From now on it will be taken into account
-    # for EACH compile
-    lsm_project.add_service(service)
+def test_model(lsm_project: pytest_inmanta_lsm.lsm_project.LsmProject) -> None:
+    # Export the service entities
+    lsm_project.export_service_entities("import quickstart")
+
+    # Create a service.  This will add it to our inventory, in its initial state
+    # (as defined in the lifecycle), and fill in any default attributes we didn't
+    # provide.
+    service = lsm_project.create_service(
+        service_entity_name="vlan-assignment",
+        attributes={
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        # With auto_transfer=True, we follow the first auto transfers of the service's
+        # lifecycle, triggering a compile (validating compile when appropriate) for
+        # each state we meets.
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been created and is now in creating state
+    assert service.state == "creating"
+
+    # Assert that the default value has been added to our attributes
+    assert "value_with_default" in service.active_attributes
+
+    # Do a second compile, in the non-validating creating state
+    lsm_project.compile(service_id=service.id)
+
+    # Move to the up state
+    service.state = "up"
+    lsm_project.compile(service_id=service.id)
+
+    # Trigger an update on our service from the up state.  Change the vlan id
+    new_attributes = copy.deepcopy(service.active_attributes)
+    new_attributes["vlan_id"] = 15
+    lsm_project.update_service(
+        service_id=service.id,
+        attributes=new_attributes,
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been updated and is now in update_inprogress state
+    assert service.state == "update_inprogress"
+
+```
+
+### Third case: development on an active environment.
+
+In some cases, (i.e. PoC) you might want to update the code of your module that is currently deployed in an environment.
+You can either start a new test case with pytest-inmanta-lsm's `remote_orchestrator` fixture, which will clear up everything
+and allow you to start from scratch.  Or you can use the similar `remote_orchestrator_access` fixture, which gives you the
+same handy `RemoteOrchestrator` object, but doesn't clear the environment of any existing services, or resources.  This allows
+you for example to re-export the service catalog, or re-synchronize your module's source code and keep all the existing services.
+
+To do so, simply create a test case using the `remote_orchestrator_access` fixture, and the same cli/env var options as used for
+normal pytest-inmanta-lsm test cases.
+```python
+def test_update_existing_environment(
+    project: plugin.Project,
+    remote_orchestrator_access: remote_orchestrator.RemoteOrchestrator,
+) -> None:
+    """
+    Make sure that it is possible to simply run a compile and export service entities,
+    without initially cleaning up the environment.
+    """
+
+    # Setup the compiler config
+    remote_orchestrator_access.setup_config()
+
+    # Do a local compile of our model
+    project.compile("import quickstart")
+
+    # Export service entities (and update the project)
+    remote_orchestrator_access.export_service_entities()
 
-    # Run a compile, with central focus the service we just created
-    lsm_project.compile("import quickstart", service_id=service.id)
 ```
 
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
@@ -184,23 +332,36 @@
                         A path to a public key that should be set in the
                         container (overrides INMANTA_LSM_CONTAINER_PUB_KEY_FILE,
                         defaults to $HOME/.ssh/id_rsa.pub)
   --lsm-environment
                         The environment to use on the remote server (is created
                         if it doesn't exist) (overrides INMANTA_LSM_ENVIRONMENT,
                         defaults to 719c7ad5-6657-444b-b536-a27174cb7498)
-  --lsm-host=LSM_HOST   Remote orchestrator to use for the remote_inmanta
-                        fixture (overrides INMANTA_LSM_HOST, defaults to
-                        127.0.0.1)
+  --lsm-host=LSM_HOST   IP address or domain name of the remote orchestrator api we
+                        wish to use in our test. It will be picked up and used by the
+                        remote_orchestrator fixture.  This is also the default remote
+                        hostname, if it is not specified in the --lsm-rh option.
+                        (overrides INMANTA_LSM_HOST, defaults to 127.0.0.1)
   --lsm-no-clean        Don't cleanup the orchestrator after tests (for
                         debugging purposes) (overrides INMANTA_LSM_NO_CLEAN,
                         defaults to False)
   --lsm-srv-port
                         Port the orchestrator api is listening to (overrides
                         INMANTA_LSM_SRV_PORT, defaults to 8888)
+  --lsm-rsh=LSM_RSH     A command which allows us to start a shell on the remote
+                        orchestrator or send file to it.  When sending files, this value
+                        will be passed to the `-e` argument of rsync.  When running a
+                        command, we will append the host name and `sh` to this value,
+                        and pass the command to execute as input to the open remote
+                        shell. (overrides INMANTA_LSM_REMOTE_SHELL)
+  --lsm-rh=LSM_RH       The name of the host that we should try to open the remote
+                        shell on, as recognized by the remote shell command.  This
+                        doesn't have to strictly be a hostname, as long as it is a
+                        valid host identifier to the chosen rsh protocol. (overrides
+                        INMANTA_LSM_REMOTE_HOST)
   --lsm-ssh-port
                         Port to use to ssh to the remote orchestrator (overrides
                         INMANTA_LSM_SSH_PORT, defaults to 22)
   --lsm-ssh-user
                         Username to use to ssh to the remote orchestrator
                         (overrides INMANTA_LSM_SSH_USER, defaults to centos)
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
```

### Comparing `pytest-inmanta-lsm-3.2.0/README.md` & `pytest_inmanta_lsm-3.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pytest-inmanta-lsm
 
+[![pypi version](https://img.shields.io/pypi/v/pytest-inmanta-lsm.svg)](https://pypi.python.org/pypi/pytest-inmanta-lsm/)
+
 A pytest plugin to test inmanta modules that use lsm, it is built on top of `pytest-inmanta` and `pytest-inmanta-extensions`
 
 ## Installation
 
 ```bash
 pip install pytest-inmanta-lsm
 ```
@@ -13,97 +15,243 @@
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
 ### First case: using a remote orchestrator
 
-This plugin is built around the remote_orchestrator fixture.
+This plugin is built around the remote_orchestrator fixture and the `RemoteServiceInstance` class.
 
-A typical testcase using this plugin looks as follows:
+You can easily write a test case that sends your project to a remote orchestrator, exports its service catalog, then deploy a service.  
 ```python
-
-def test_full_cycle(project, remote_orchestrator):
+def test_deploy_service(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
 
     # setup project
-    project.compile(
-        """
-        import quickstart
-        """
-    )
+    project.compile("import quickstart")
 
     # sync project and export service entities
     remote_orchestrator.export_service_entities()
 
     # verify the service is in the catalog
     result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
     assert result.code == 200
 
-    # get a ManagedInstance object, to simplifies interacting with a specific service instance
-    service_instance = remote_orchestrator.get_managed_instance(SERVICE_NAME)
+    # Test the synchronous service instance class
+    instance = remote_service_instance.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
+    )
 
-    # create an instance and wait for it to be up
-    service_instance.create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="up",
+    # Create the service instance and stop waiting in a transient state
+    created = instance.create(
+        {
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        wait_for_state="creating",
+        timeout=60,
+    )
+
+    # Wait for up state, we provide here the version from which we should follow the
+    # service, which is the version in which we last stopped following the service.  This
+    # guarantees that we don't "miss" the target state, in case it is a transient one, and
+    # don't confuse the start state for the target one in case it is the same one.
+    # The start version should always be the last version in which we know our service has
+    # been, BEFORE the target state we expect our service to go into.
+    instance.wait_for_state(
+        target_state="up",
+        start_version=created.version,
+        timeout=60,
+    )
+
+    # Delete the instance
+    instance.delete(wait_for_state="terminated", timeout=60)
+```
+> source: [test_quickstart.py::test_transient_state](./examples/quickstart/tests/test_quickstart.py)
+
+For a more advanced test case, you might also want to deploy multiple services.  You could either test them one by one, or, parallelize them, in order to:
+1. speed up the test case.
+2. test interference in between the services.
+
+In that case, the recommended way is to create an `async` helper, which follows the progress of your service, and instantiate multiple services with it, in a `sync` test case.
+```python
+async def service_full_cycle(
+    remote_orchestrator: remote_orchestrator.RemoteOrchestrator,
+    router_ip: str,
+    interface_name: str,
+    address: str,
+    vlan_id: int,
+    vlan_id_update: int,
+) -> None:
+    # Create an async service instance object
+    instance = remote_service_instance_async.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
     )
 
-    # make validation fail by creating a duplicate
-    remote_orchestrator.get_managed_instance(SERVICE_NAME).create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="rejected",
+    # Create the service instance on the remote orchestrator
+    await instance.create(
+        {
+            "router_ip": router_ip,
+            "interface_name": interface_name,
+            "address": address,
+            "vlan_id": vlan_id,
+        },
+        wait_for_state="up",
+        timeout=60,
     )
 
-    service_instance.update(
-        attribute_updates={"vlan_id": 42},
+    # Update the vlan id
+    await instance.update(
+        [
+            inmanta_lsm.model.PatchCallEdit(
+                edit_id=str(uuid.uuid4()),
+                operation=inmanta_lsm.model.EditOperation.replace,
+                target="vlan_id",
+                value=vlan_id_update,
+            ),
+        ],
         wait_for_state="up",
+        timeout=60,
+    )
+
+    # Delete the instance
+    await instance.delete(wait_for_state="terminated", timeout=60)
+
+
+def test_full_cycle(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
+    # get connection to remote_orchestrator
+    client = remote_orchestrator.client
+
+    # setup project
+    project.compile("import quickstart")
+
+    # sync project and export service entities
+    remote_orchestrator.export_service_entities()
+
+    # verify the service is in the catalog
+    result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
+    assert result.code == 200
+
+    # Create a first service that should be deployed
+    first_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.17",
+        interface_name="eth1",
+        address="10.0.0.254/24",
+        vlan_id=14,
+        vlan_id_update=42,
     )
 
-    # break it down
-    service_instance.delete()
+    # Create another valid service
+    another_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.18",
+        interface_name="eth2",
+        address="10.0.0.253/24",
+        vlan_id=15,
+        vlan_id_update=52,
+    )
 
+    # Run all the services
+    util.sync_execute_scenarios(first_service, another_service, timeout=60)
 ```
+> source: [test_quickstart.py::test_full_cycle](./examples/quickstart/tests/test_quickstart.py)
+
 
 ### Second case: mocking the lsm api
 
 This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
  - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
  - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
  - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
 
 A simple usage would be as follow:
 ```python
-def test_model(lsm_project: lsm_project.LsmProject) -> None:
-    # Create a service object, you can modify it as you wish, depending on what you are trying to test
-    service = inmanta_lsm.model.ServiceInstance(
-        id=uuid.uuid4(),
-        environment=lsm_project.environment,
-        service_entity="vlan-assignment",
-        version=1,
-        config={},
-        state="start",
-        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        active_attributes=None,
-        rollback_attributes=None,
-        created_at=datetime.datetime.now(),
-        last_updated=datetime.datetime.now(),
-        callback=[],
-        deleted=False,
-        deployment_progress=None,
-        service_identity_attribute_value=None,
-    )
-
-    # Add the service to the mocked server.  From now on it will be taken into account
-    # for EACH compile
-    lsm_project.add_service(service)
+def test_model(lsm_project: pytest_inmanta_lsm.lsm_project.LsmProject) -> None:
+    # Export the service entities
+    lsm_project.export_service_entities("import quickstart")
+
+    # Create a service.  This will add it to our inventory, in its initial state
+    # (as defined in the lifecycle), and fill in any default attributes we didn't
+    # provide.
+    service = lsm_project.create_service(
+        service_entity_name="vlan-assignment",
+        attributes={
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        # With auto_transfer=True, we follow the first auto transfers of the service's
+        # lifecycle, triggering a compile (validating compile when appropriate) for
+        # each state we meets.
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been created and is now in creating state
+    assert service.state == "creating"
+
+    # Assert that the default value has been added to our attributes
+    assert "value_with_default" in service.active_attributes
+
+    # Do a second compile, in the non-validating creating state
+    lsm_project.compile(service_id=service.id)
+
+    # Move to the up state
+    service.state = "up"
+    lsm_project.compile(service_id=service.id)
+
+    # Trigger an update on our service from the up state.  Change the vlan id
+    new_attributes = copy.deepcopy(service.active_attributes)
+    new_attributes["vlan_id"] = 15
+    lsm_project.update_service(
+        service_id=service.id,
+        attributes=new_attributes,
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been updated and is now in update_inprogress state
+    assert service.state == "update_inprogress"
+
+```
+
+### Third case: development on an active environment.
+
+In some cases, (i.e. PoC) you might want to update the code of your module that is currently deployed in an environment.
+You can either start a new test case with pytest-inmanta-lsm's `remote_orchestrator` fixture, which will clear up everything
+and allow you to start from scratch.  Or you can use the similar `remote_orchestrator_access` fixture, which gives you the
+same handy `RemoteOrchestrator` object, but doesn't clear the environment of any existing services, or resources.  This allows
+you for example to re-export the service catalog, or re-synchronize your module's source code and keep all the existing services.
+
+To do so, simply create a test case using the `remote_orchestrator_access` fixture, and the same cli/env var options as used for
+normal pytest-inmanta-lsm test cases.
+```python
+def test_update_existing_environment(
+    project: plugin.Project,
+    remote_orchestrator_access: remote_orchestrator.RemoteOrchestrator,
+) -> None:
+    """
+    Make sure that it is possible to simply run a compile and export service entities,
+    without initially cleaning up the environment.
+    """
+
+    # Setup the compiler config
+    remote_orchestrator_access.setup_config()
+
+    # Do a local compile of our model
+    project.compile("import quickstart")
+
+    # Export service entities (and update the project)
+    remote_orchestrator_access.export_service_entities()
 
-    # Run a compile, with central focus the service we just created
-    lsm_project.compile("import quickstart", service_id=service.id)
 ```
 
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
@@ -158,23 +306,36 @@
                         A path to a public key that should be set in the
                         container (overrides INMANTA_LSM_CONTAINER_PUB_KEY_FILE,
                         defaults to $HOME/.ssh/id_rsa.pub)
   --lsm-environment
                         The environment to use on the remote server (is created
                         if it doesn't exist) (overrides INMANTA_LSM_ENVIRONMENT,
                         defaults to 719c7ad5-6657-444b-b536-a27174cb7498)
-  --lsm-host=LSM_HOST   Remote orchestrator to use for the remote_inmanta
-                        fixture (overrides INMANTA_LSM_HOST, defaults to
-                        127.0.0.1)
+  --lsm-host=LSM_HOST   IP address or domain name of the remote orchestrator api we
+                        wish to use in our test. It will be picked up and used by the
+                        remote_orchestrator fixture.  This is also the default remote
+                        hostname, if it is not specified in the --lsm-rh option.
+                        (overrides INMANTA_LSM_HOST, defaults to 127.0.0.1)
   --lsm-no-clean        Don't cleanup the orchestrator after tests (for
                         debugging purposes) (overrides INMANTA_LSM_NO_CLEAN,
                         defaults to False)
   --lsm-srv-port
                         Port the orchestrator api is listening to (overrides
                         INMANTA_LSM_SRV_PORT, defaults to 8888)
+  --lsm-rsh=LSM_RSH     A command which allows us to start a shell on the remote
+                        orchestrator or send file to it.  When sending files, this value
+                        will be passed to the `-e` argument of rsync.  When running a
+                        command, we will append the host name and `sh` to this value,
+                        and pass the command to execute as input to the open remote
+                        shell. (overrides INMANTA_LSM_REMOTE_SHELL)
+  --lsm-rh=LSM_RH       The name of the host that we should try to open the remote
+                        shell on, as recognized by the remote shell command.  This
+                        doesn't have to strictly be a hostname, as long as it is a
+                        valid host identifier to the chosen rsh protocol. (overrides
+                        INMANTA_LSM_REMOTE_HOST)
   --lsm-ssh-port
                         Port to use to ssh to the remote orchestrator (overrides
                         INMANTA_LSM_SSH_PORT, defaults to 22)
   --lsm-ssh-user
                         Username to use to ssh to the remote orchestrator
                         (overrides INMANTA_LSM_SSH_USER, defaults to centos)
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
```

### Comparing `pytest-inmanta-lsm-3.2.0/setup.cfg` & `pytest_inmanta_lsm-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/setup.py` & `pytest_inmanta_lsm-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-inmanta-lsm",
-    version="3.2.0",
+    version="3.3.0",
     python_requires=">=3.6",  # also update classifiers
     author="Inmanta",
     author_email="code@inmanta.com",
     license="inmanta EULA",
     url="https://github.com/inmanta/pytest-inmanta-lsm",
     description="Common fixtures for inmanta LSM related modules",
     long_description=read("README.md"),
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/__init__.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/exceptions.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/failed_resources_logs.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/failed_resources_logs.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/managed_service_instance.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/managed_service_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import logging
 from pprint import pformat
 from typing import Any, Collection, Dict, List, Optional, Union
 from uuid import UUID
 
 from inmanta_lsm.diagnose.model import FullDiagnosis
 
-from pytest_inmanta_lsm import remote_orchestrator as r_orchestrator
-from pytest_inmanta_lsm.exceptions import VersionExceededError, VersionMismatchError
-from pytest_inmanta_lsm.wait_for_state import State, WaitForState
+from pytest_inmanta_lsm import exceptions, remote_orchestrator, wait_for_state
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ManagedServiceInstance:
     """Object that represents a service instance that contains the method to
     push it through its lifecycle and verify its status
@@ -42,15 +40,15 @@
 
     ALL_BAD_STATES = list(set(CREATE_FLOW_BAD_STATES + UPDATE_FLOW_BAD_STATES + DELETE_FLOW_BAD_STATES))
 
     DEFAULT_TIMEOUT = 600
 
     def __init__(
         self,
-        remote_orchestrator: "r_orchestrator.RemoteOrchestrator",
+        remote_orchestrator: "remote_orchestrator.RemoteOrchestrator",
         service_entity_name: str,
         service_id: Optional[UUID] = None,
         lookback_depth: int = 1,
     ) -> None:
         """
         :param remote_orchestrator: remote_orchestrator to create the service instance  on
         :param service_entity_name: name of the service entity
@@ -248,30 +246,30 @@
             bad_states=bad_states,
             start_version=current_version,
             timeout=timeout,
         )
 
     def get_state(
         self,
-    ) -> State:
+    ) -> wait_for_state.State:
         """Get the current state of the service instance"""
         response = self.remote_orchestrator.client.lsm_services_get(
             tid=self.remote_orchestrator.environment,
             service_entity=self.service_entity_name,
             service_id=self.instance_id,
         )
         assert (
             response.code == 200
         ), f"Wrong response code while trying to get state, got {response.code} (expected 200): \n{response}"
         instance_state = response.result["data"]["state"]
         instance_version = int(response.result["data"]["version"])
 
-        return State(name=instance_state, version=instance_version)
+        return wait_for_state.State(name=instance_state, version=instance_version)
 
-    def get_states(self, after_version: int = 0) -> List[State]:
+    def get_states(self, after_version: int = 0) -> List[wait_for_state.State]:
         """
         Get all the states the managed instance went through after the given version
 
         :param after_version: The version all returned states should be greater than
         """
         response = self.remote_orchestrator.client.lsm_service_log_list(
             tid=self.remote_orchestrator.environment,
@@ -280,15 +278,17 @@
         )
         assert (
             response.code == 200
         ), f"Wrong response code while trying to get state logs, got {response.code} (expected 200): \n{response}"
 
         logs = response.result["data"]
 
-        return [State(name=log["state"], version=log["version"]) for log in logs if log["version"] > after_version]
+        return [
+            wait_for_state.State(name=log["state"], version=log["version"]) for log in logs if log["version"] > after_version
+        ]
 
     def wait_for_state(
         self,
         state: Optional[str] = None,
         states: Optional[Collection[str]] = None,
         version: Optional[int] = None,
         versions: Optional[Collection[int]] = None,
@@ -328,38 +328,38 @@
         if version is None and versions is not None:
             desired_versions.extend(versions)
         elif version is not None and versions is None:
             desired_versions.append(version)
         elif version is not None and versions is not None:
             raise ValueError("Both 'version' and 'versions' arguments can not be set")
 
-        def compare_states(current_state: State, wait_for_states: List[str]) -> bool:
+        def compare_states(current_state: wait_for_state.State, wait_for_states: List[str]) -> bool:
             if current_state.name in wait_for_states:
                 if len(desired_versions) == 0:
                     # Version is not given, so version does not need to be verified
                     return True
                 elif current_state.version not in desired_versions:
-                    raise VersionMismatchError(self, desired_versions, current_state.version)
+                    raise exceptions.VersionMismatchError(self, desired_versions, current_state.version)
                 else:
                     return True
             elif (
                 len(desired_versions) > 0
                 and current_state.version is not None
                 and max(desired_versions) <= current_state.version
             ):
-                raise VersionExceededError(self, desired_versions, current_state.version)
+                raise exceptions.VersionExceededError(self, desired_versions, current_state.version)
 
             return False
 
-        def check_start_state(current_state: State) -> bool:
+        def check_start_state(current_state: wait_for_state.State) -> bool:
             if start_version is None:
                 return False
             return current_state.version == start_version
 
-        def get_bad_state_error(current_state: State) -> FullDiagnosis:
+        def get_bad_state_error(current_state: wait_for_state.State) -> FullDiagnosis:
             result = self.remote_orchestrator.client.lsm_services_diagnose(
                 tid=self.remote_orchestrator.environment,
                 service_entity=self.service_entity_name,
                 service_id=self.instance_id,
                 version=current_state.version,
                 rejection_lookbehind=self._lookback - 1,
                 failure_lookbehind=self._lookback,
@@ -367,15 +367,15 @@
             assert result.code == 200, (
                 f"Wrong response code while trying to get the service diagnostic, got {result.code} (expected 200):\n"
                 f"{json.dumps(result.result or {}, indent=4)}"
             )
 
             return FullDiagnosis(**result.result["data"])
 
-        wait_for_obj = WaitForState(
+        wait_for_obj = wait_for_state.WaitForState(
             "Instance lifecycle",
             get_states_method=self.get_states,
             compare_states_method=compare_states,
             check_start_state_method=check_start_state,
             get_bad_state_error_method=get_bad_state_error,
         )
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/orchestrator_container.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/orchestrator_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,30 @@
     """
     Helper function to run command and log the results.  Raises a CalledProcessError
     if the command failed.
     """
     LOGGER.info(f"Running command: {cmd}")
     env_vars = dict(os.environ)
     env_vars.pop("PYTHONPATH", None)
-    result = subprocess.run(
-        args=cmd,
-        cwd=str(cwd),
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        text=True,
-        universal_newlines=True,
-        env=env_vars,
-    )
+    try:
+        result = subprocess.run(
+            args=cmd,
+            cwd=str(cwd),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            encoding="utf-8",
+            text=True,
+            universal_newlines=True,
+            env=env_vars,
+        )
+    except FileNotFoundError as e:
+        if e.filename == "docker-compose":
+            raise FileNotFoundError("The `docker-compose` command is not found. You need it to have a local orchestrator.")
+        raise e
+
     LOGGER.debug(f"Return code: {result.returncode}")
     LOGGER.debug("Stdout: %s", result.stdout)
     LOGGER.debug("Stderr: %s", result.stderr)
     result.check_returncode()
     return result.stdout, result.stderr
 
 
@@ -215,15 +221,14 @@
     def orchestrator_port(self) -> int:
         return int(self.config.get("server", "bind-port", vars={"fallback": "8888"}))
 
     def _up(self) -> None:
         # Pull container images
         cmd = ["docker-compose", "--verbose", "pull"]
         run_cmd(cmd=cmd, cwd=self.cwd)
-
         # Starting the lab
         cmd = ["docker-compose", "--verbose", "up", "-d"]
         run_cmd(cmd=cmd, cwd=self.cwd)
 
         # Getting the containers ids
         cmd = ["docker-compose", "--verbose", "ps", "-q"]
         stdout, _ = run_cmd(cmd=cmd, cwd=self.cwd)
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/parameters.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/parameters.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,27 +16,53 @@
 )
 
 param_group = "pytest-inmanta-lsm"
 
 inm_lsm_host = StringTestParameter(
     argument="--lsm-host",
     environment_variable="INMANTA_LSM_HOST",
-    usage="Remote orchestrator to use for the remote_inmanta fixture",
+    usage=(
+        "IP address or domain name of the remote orchestrator api we wish to use in our test. It "
+        "will be picked up and used by the remote_orchestrator fixture.  This is also the default "
+        "remote hostname, if it is not specified in the --lsm-rh option."
+    ),
     default="127.0.0.1",
     group=param_group,
 )
 
 inm_lsm_srv_port = IntegerTestParameter(
     argument="--lsm-srv-port",
     environment_variable="INMANTA_LSM_SRV_PORT",
     usage="Port the orchestrator api is listening to",
     default=8888,
     group=param_group,
 )
 
+inm_lsm_remote_shell = StringTestParameter(
+    argument="--lsm-rsh",
+    environment_variable="INMANTA_LSM_REMOTE_SHELL",
+    usage=(
+        "A command which allows us to start a shell on the remote orchestrator or send file to it.  "
+        "When sending files, this value will be passed to the `-e` argument of rsync.  When running a command, we will "
+        "append the host name and `sh` to this value, and pass the command to execute as input to the open remote shell."
+    ),
+    group=param_group,
+)
+
+inm_lsm_remote_host = StringTestParameter(
+    argument="--lsm-rh",
+    environment_variable="INMANTA_LSM_REMOTE_HOST",
+    usage=(
+        "The name of the host that we should try to open the remote shell on, "
+        "as recognized by the remote shell command.  This doesn't have to strictly be "
+        "a hostname, as long as it is a valid host identifier to the chosen rsh protocol."
+    ),
+    group=param_group,
+)
+
 inm_lsm_ssh_user = StringTestParameter(
     argument="--lsm-ssh-user",
     environment_variable="INMANTA_LSM_SSH_USER",
     usage="Username to use to ssh to the remote orchestrator",
     default="centos",
     group=param_group,
 )
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/plugin.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,34 @@
     :copyright: 2020 Inmanta
     :contact: code@inmanta.com
     :license: Inmanta EULA
 """
 
 import logging
 import os
+import shlex
 import shutil
 import textwrap
 import time
 import uuid
 from typing import Dict, Generator, Iterator, Optional, Tuple, Union
 from uuid import UUID
 
 import pkg_resources
 import pytest
 import pytest_inmanta.plugin
 import requests
 from inmanta import module
 from packaging import version
 from pytest_inmanta.plugin import Project
-from pytest_inmanta.test_parameter import ParameterNotSetException, StringTestParameter
+from pytest_inmanta.test_parameter import (
+    ParameterNotSetException,
+    ParameterType,
+    TestParameter,
+)
 
 from pytest_inmanta_lsm import lsm_project
 from pytest_inmanta_lsm.orchestrator_container import (
     DoNotCleanOrchestratorContainer,
     OrchestratorContainer,
 )
 from pytest_inmanta_lsm.parameters import (
@@ -44,14 +49,16 @@
     inm_lsm_env,
     inm_lsm_env_name,
     inm_lsm_host,
     inm_lsm_no_clean,
     inm_lsm_no_halt,
     inm_lsm_partial_compile,
     inm_lsm_project_name,
+    inm_lsm_remote_host,
+    inm_lsm_remote_shell,
     inm_lsm_srv_port,
     inm_lsm_ssh_port,
     inm_lsm_ssh_user,
     inm_lsm_ssl,
     inm_lsm_token,
 )
 from pytest_inmanta_lsm.remote_orchestrator import (
@@ -217,15 +224,15 @@
 
     # mod object is constructed from the source dir: it does not contain all installation metadata
     installed: Optional[module.ModuleV2] = module.ModuleV2Source(urls=[]).get_installed_module(None, mod.name)
 
     # Generic message to help fix any of the problems reported below
     how_to_fix = (
         "To ensure the remote orchestrator uses the same code as the local project, please install the module"
-        " with `inmanta module install -e .` before running the tests."
+        " with `pip install -e .` before running the tests."
     )
 
     if installed is None:
         # Make sure that the module v2 source can be found, it should always be the case, unless
         # this fixture is used outside of the context of a module test suite.
         LOGGER.error("The module being tested is not installed.  %s", how_to_fix)
     elif not installed.is_editable():
@@ -249,86 +256,106 @@
         return
 
     # We didn't exit, there was a failure, so we raise an exception
     raise RuntimeError(f"Module at {mod.path} should be installed in editable mode.  See logs for details.")
 
 
 @pytest.fixture(scope="session")
-def remote_orchestrator_shared(
+def remote_orchestrator_access(
     request: pytest.FixtureRequest,
     project_shared: Project,
     remote_orchestrator_container: Optional[OrchestratorContainer],
     remote_orchestrator_environment: str,
-    remote_orchestrator_no_clean: bool,
-    remote_orchestrator_no_halt: bool,
-    remote_orchestrator_host: Tuple[str, int],
-) -> Iterator[RemoteOrchestrator]:
+    remote_orchestrator_host: tuple[str, int],
+) -> RemoteOrchestrator:
     """
-    Session fixture to setup the `RemoteOrchestrator` object that will be used to sync our project
-    to the remote orchestrator environment.  This fixture also makes sure that if the module being
-    tested is v2, it is installed in editable mode, as it is required to send it to the remote
-    orchestrator.
+    This fixture allows to get the remote orchestrator object, without any of the initial cleanup.
+    This allows to easily build helper tests that simply sync a remote environment with our local
+    project, without clearing its service inventory.
     """
-    # no need to do anything if this version of inmanta does not support v2 modules
-    if hasattr(module, "ModuleV2"):
-        verify_v2_editable_install()
-
     LOGGER.info("Setting up remote orchestrator")
 
     host, port = remote_orchestrator_host
 
+    def get_optional_option(option: TestParameter[ParameterType]) -> Optional[ParameterType]:
+        try:
+            return option.resolve(request.config)
+        except ParameterNotSetException:
+            return None
+
     if remote_orchestrator_container is None:
-        ssh_user = inm_lsm_ssh_user.resolve(request.config)
-        ssh_port = inm_lsm_ssh_port.resolve(request.config)
         container_env = inm_lsm_container_env.resolve(request.config)
+        remote_shell = get_optional_option(inm_lsm_remote_shell)
+        remote_host = get_optional_option(inm_lsm_remote_host)
+        ssh_user = get_optional_option(inm_lsm_ssh_user) if remote_shell is None else None
+        ssh_port = get_optional_option(inm_lsm_ssh_port) if remote_shell is None else None
     else:
         # If the orchestrator is running in a container we deployed ourself, we overwrite
         # a few configuration parameters with what matches the deployed orchestrator
         # If the container image behaves differently than assume, those value won't work,
         # no mechanism exists currently to work around this.
-        ssh_user = "inmanta"
-        ssh_port = 22
+        ssh_user = None
+        ssh_port = None
         container_env = True
+        remote_shell = "docker exec -w /var/lib/inmanta -u inmanta -i"
+        remote_host = remote_orchestrator_container.orchestrator["Config"]["Hostname"]
 
     ssl = inm_lsm_ssl.resolve(request.config)
     ca_cert: Optional[str] = None
     if ssl:
         ca_cert = str(inm_lsm_ca_cert.resolve(request.config))
         if (
             remote_orchestrator_container is not None
             and remote_orchestrator_container.compose_file == inm_lsm_ctr_compose.default
         ):
             LOGGER.warning("SSL currently doesn't work with the default docker-compose file.")
 
-    def get_optional_option(option: StringTestParameter) -> Optional[str]:
-        try:
-            return option.resolve(request.config)
-        except ParameterNotSetException:
-            return None
-
     token = get_optional_option(inm_lsm_token)
     environment_name = get_optional_option(inm_lsm_env_name)
     project_name = get_optional_option(inm_lsm_project_name)
 
-    remote_orchestrator = RemoteOrchestrator(
+    return RemoteOrchestrator(
         OrchestratorEnvironment(
             id=UUID(remote_orchestrator_environment),
             name=environment_name,
             project=project_name,
         ),
         host=host,
         port=port,
         ssh_user=ssh_user,
         ssh_port=ssh_port,
         ssl=ssl,
         token=token,
         ca_cert=ca_cert,
         container_env=container_env,
+        remote_shell=shlex.split(remote_shell) if remote_shell is not None else None,
+        remote_host=remote_host,
     )
 
+
+@pytest.fixture(scope="session")
+def remote_orchestrator_shared(
+    request: pytest.FixtureRequest,
+    project_shared: Project,
+    remote_orchestrator_access: RemoteOrchestrator,
+    remote_orchestrator_no_clean: bool,
+    remote_orchestrator_no_halt: bool,
+) -> Iterator[RemoteOrchestrator]:
+    """
+    Session fixture to setup the `RemoteOrchestrator` object that will be used to sync our project
+    to the remote orchestrator environment.  This fixture also makes sure that if the module being
+    tested is v2, it is installed in editable mode, as it is required to send it to the remote
+    orchestrator.
+    """
+    # no need to do anything if this version of inmanta does not support v2 modules
+    if hasattr(module, "ModuleV2"):
+        verify_v2_editable_install()
+
+    remote_orchestrator = remote_orchestrator_access
+
     # Make sure we start our test suite with a clean environment
     remote_orchestrator.clear_environment()
 
     # Get the former cached modules back into the project to speed up
     # subsequent test cases
     remote_orchestrator.restore_libs_folder()
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/remote_orchestrator.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/remote_orchestrator.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import uuid
 from pprint import pformat
 from uuid import UUID
 
 import inmanta.data.model
 import inmanta.module
 import inmanta.protocol.endpoints
+import pydantic
 from inmanta.agent import config as inmanta_config
 from inmanta.protocol.common import Result
 from packaging.version import Version
 
 from pytest_inmanta_lsm import managed_service_instance, retry_limited
 
 LOGGER = logging.getLogger(__name__)
@@ -158,62 +159,98 @@
             assert result.code in range(200, 300), str(result.result)
             assert result.result is not None
             return inmanta.data.model.Environment(**result.result["data"])
         else:
             return current_environment
 
 
+T = typing.TypeVar("T")
+
+
 class RemoteOrchestrator:
     """
     This class helps to interact with a real remote orchestrator.  Its main focus is to help
     sync a local project to this remote orchestrator, into the environment specified by the
     user.  This class should be usable independently from any testing artifacts (like the Project
     object from the `pytest_inmanta.plugin.project` fixture.)
     """
 
     def __init__(
         self,
         orchestrator_environment: OrchestratorEnvironment,
         *,
         host: str = "localhost",
         port: int = 8888,
-        ssh_user: str = "inmanta",
-        ssh_port: int = 22,
+        ssh_user: typing.Optional[str] = "inmanta",
+        ssh_port: typing.Optional[int] = 22,
         token: typing.Optional[str] = None,
         ssl: bool = False,
         ca_cert: typing.Optional[str] = None,
         container_env: bool = False,
+        remote_shell: typing.Optional[typing.Sequence[str]] = None,
+        remote_host: typing.Optional[str] = None,
     ) -> None:
         """
         :param environment: The environment that should be configured on the remote orchestrator
             and that this project should be sync to.
 
         :param host: the host to connect to, the orchestrator should be on port 8888
         :param port: The port the server is listening to
         :param ssh_user: the username to log on to the machine, should have sudo rights
         :param ssh_port: the port to use to log on to the machine
         :param token: Token used for authentication
         :param ssl: Option to indicate whether SSL should be used or not. Defaults to false
         :param ca_cert: Certificate used for authentication
         :param container_env: Whether the remote orchestrator is running in a container, without a systemd init process.
+        :param remote_shell: A command which allows us to start a shell on the remote orchestrator or send file to it.
+            When sending files, this value will be passed to the `-e` argument of rsync.  When running a command, we will
+            append the host name and `sh` to this value, and pass the command to execute as input to the open remote shell.
+        :param remote_host: The name of the remote host we can execute command on or send files to.  Defaults
+            to the value of the host parameter.
         """
         self.orchestrator_environment = orchestrator_environment
         self.environment = self.orchestrator_environment.id
 
         self.host = host
         self.port = port
         self.ssh_user = ssh_user
         self.ssh_port = ssh_port
         self.ssl = ssl
         self.token = token
         self.ca_cert = ca_cert
         self.container_env = container_env
 
+        self.remote_shell: typing.Sequence[str]
+        if remote_shell is not None:
+            # We got a remote shell command, allowing us to access the remote orchestrator
+            self.remote_shell = remote_shell
+        elif ssh_user is None or ssh_port is None:
+            # No remote shell command and no ssh user and port, we have no
+            # way of accessing the remote orchestrator
+            raise ValueError("Either the remote shell or the ssh access should be provided")
+        else:
+            # Compose the remote shell command based on the ssh user and port
+            self.remote_shell = [
+                *SSH_CMD,
+                "-p",
+                str(ssh_port),
+                "-l",
+                ssh_user,
+            ]
+
+        # Cached value of the name of the user we have on the remote orchestrator
+        self._whoami: typing.Optional[str] = None
+
+        # Allow to change the remote host, as the access to the remote shell or to the
+        # remote api might be different (i.e. podman exec -i <container-name> vs curl <container-ip>)
+        self.remote_host = remote_host if remote_host is not None else host
+
         # Build the client once, it loads the config on every call
         self.client = inmanta.protocol.endpoints.SyncClient("client")
+        self.async_client = inmanta.protocol.endpoints.Client("client")
 
         # Setting up the client when the config is loaded
         self.setup_config()
 
         self.orchestrator_environment.configure_environment(self.client)
         self.server_version = self._get_server_version()
 
@@ -254,88 +291,138 @@
             if self.ssl:
                 inmanta_config.Config.set(section, "ssl", str(self.ssl))
                 if self.ca_cert:
                     inmanta_config.Config.set(section, "ssl_ca_cert_file", self.ca_cert)
             if self.token:
                 inmanta_config.Config.set(section, "token", self.token)
 
+    @typing.overload
+    async def request(self, method: str, returned_type: None = None, **kwargs: object) -> None:
+        pass
+
+    @typing.overload
+    async def request(self, method: str, returned_type: type[T], **kwargs: object) -> T:
+        pass
+
+    async def request(
+        self,
+        method: str,
+        returned_type: typing.Optional[type[T]] = None,
+        **kwargs: object,
+    ) -> typing.Optional[T]:
+        """
+        Helper method to send a request to the orchestrator, which we expect to succeed with 20X code and
+        return an object of a given type.
+
+        :param method: The name of the method to execute
+        :param returned_type: The type of the object that the api should return
+        :param **kwargs: Parameters to pass to the method we are calling
+        """
+        response: Result = await getattr(self.async_client, method)(**kwargs)
+        assert response.code in range(200, 300), str(response.result)
+        if returned_type is not None:
+            assert response.result is not None, str(response)
+            try:
+                return pydantic.TypeAdapter(returned_type).validate_python(response.result["data"])
+            except AttributeError:
+                # Handle pydantic v1
+                return pydantic.parse_obj_as(returned_type, response.result["data"])
+        else:
+            return None
+
     def _get_server_version(self) -> Version:
         """
         Get the version of the remote orchestrator
         """
         server_status: Result = self.client.get_server_status()
         if server_status.code != 200:
             raise Exception(f"Failed to get server status for {self.host}")
         try:
             assert server_status.result is not None
             return Version(server_status.result["data"]["version"])
         except (KeyError, TypeError):
             raise Exception(f"Unexpected response for server status API call: {server_status.result}")
 
+    @property
+    def remote_user(self) -> str:
+        """
+        Execute the whoami command in the remote shell, to discover which user we have access to
+        in this shell and returns its name.  The result is cached, as we don't expect the remote
+        shell to change within the lifecycle of this remote orchestrator object.
+        """
+        if self._whoami is None:
+            self._whoami = self.run_command(["whoami"], user=None, stderr=subprocess.PIPE).strip()
+            LOGGER.debug("Remote user at %s (accessed via %s) is %s", self.remote_host, self.remote_shell, repr(self._whoami))
+        return self._whoami
+
     def run_command(
         self,
         args: typing.Sequence[str],
         *,
         shell: bool = False,
         cwd: typing.Optional[str] = None,
         env: typing.Optional[typing.Mapping[str, str]] = None,
-        user: str = "inmanta",
+        user: typing.Optional[str] = "inmanta",
+        stderr: int = subprocess.STDOUT,
     ) -> str:
         """
         Helper method to execute a command on the remote orchestrator host as the specified user.
         This methods tries to mimic the interface of subprocess.check_output as closely as it can
         but taking some liberties regarding the typing or parameters.  This should be kept in mind
         for future expansion.
 
         :param args: A sequence of string, which should be executed as a single command, on the
             remote orchestrator.  If shell is True, the sequence should contain exactly one element.
         :param shell: Whether to execute the argument in a shell (bash).
         :param cwd: The directory on the remote orchestrator in which the command should be executed.
         :param env: A mapping of environment variables that should be available to the process
             running on the remote orchestrator.
-        :param user: The user that should be running the process on the remote orchestrator.
+        :param user: The user that should be running the process on the remote orchestrator.  If set to
+            None, keep whichever user is used when opening the remote shell on the orchestrator.
+        :param stderr: The file descriptor number where stderr for the given command should be sent to.
+            Defaults to stdout, which is returned by this command.
         """
         if shell:
             assert len(args) == 1, "When running command in a shell, only one arg should be provided"
             cmd = args[0]
         else:
             # Join the command, safely escape all spaces
             cmd = shlex.join(args)
 
         # If required, add env var prefix to the command
         if env is not None:
+            shell = True
             env_prefix = [f"{k}={shlex.quote(v)}" for k, v in env.items()]
             cmd = " ".join(env_prefix + [cmd])
 
         if cwd is not None:
             # Pretend that the command is a shell, and add a cd ... prefix to it
             shell = True
             cmd = shlex.join(["cd", cwd]) + "; " + cmd
 
         if shell:
             # The command we received should be run in a shell
             cmd = shlex.join(["bash", "-l", "-c", cmd])
 
-        # If we need to change user, prefix the command with a sudo
-        if self.ssh_user != user:
-            # Make sure the user is a safe value to use
-            user = shlex.quote(user)
-            cmd = f"sudo --login --user={user} -- {cmd}"
+        if user is not None and user != self.remote_user:
+            # If we need to change user, prefix the command with a sudo
+            cmd = shlex.join(["sudo", "--login", "--user", user, "--", *shlex.split(cmd)])
 
         LOGGER.debug("Running command on remote orchestrator: %s", cmd)
         try:
+            # The command we execute on the remote host is always "sh", and we provide
+            # the desired command to run as input.  We do this because 'ssh' and 'docker exec'
+            # don't expect the same format of argument for the command to execute on the
+            # remote host.  The former expects the command and its arguments as a single string.
+            # The latter expects the command and its arguments to be space-separated arguments to
+            # the exec command.
             return subprocess.check_output(
-                SSH_CMD
-                + [
-                    "-p",
-                    str(self.ssh_port),
-                    f"{self.ssh_user}@{self.host}",
-                    cmd,
-                ],
-                stderr=subprocess.STDOUT,
+                [*self.remote_shell, self.remote_host, "sh"],
+                input=cmd,
+                stderr=stderr,
                 universal_newlines=True,
             )
         except subprocess.CalledProcessError as e:
             LOGGER.error("Failed to execute command: %s", cmd)
             LOGGER.error("Subprocess exited with code %d: %s", e.returncode, str(e.stdout))
             raise e
 
@@ -398,75 +485,78 @@
             shell = True
             cmd = shlex.join(["cd", cwd]) + "; " + cmd
 
         if shell:
             # The command we received should be run in a shell
             cmd = shlex.join(["bash", "-l", "-c", cmd])
 
-        return self.run_command(args=[base_cmd + " " + cmd], shell=True, user=self.ssh_user)
+        return self.run_command(args=[base_cmd + " " + cmd], shell=True, user=None)
 
     def sync_local_folder(
         self,
         local_folder: pathlib.Path,
         remote_folder: pathlib.Path,
         *,
         excludes: typing.Sequence[str],
-        user: str = "inmanta",
+        user: typing.Optional[str] = "inmanta",
     ) -> None:
         """
         Sync a local folder with a remote orchestrator folder, exclude the provided sub folder
         as well as anything that would be ignored by git (if a .gitignore file is found in the
         folder) and make sure that the remote folder is owned by the specified user.
 
         :param local_folder: The folder on this machine that should be sent to the remote
             orchestrator.
         :param remote_folder: The folder on the remote orchestrator that should contain our
             local folder content after the sync.
         :param excludes: A list of exclude values to provide to rsync.
-        :param user: The user that should own the file on the remote orchestrator.
+        :param user: The user that should own the file on the remote orchestrator.  If set to None,
+            keep whichever user is used when opening the remote shell on the orchestrator.
         """
-        if self.ssh_user != user:
+        if user is not None and user != self.remote_user:
             # Syncing the folder would not give us the correct permission on the folder
             # So we sync the folder in a temporary location, then move it
             temporary_remote_folder = pathlib.Path(f"/tmp/{self.environment}/tmp-{remote_folder.name}")
             self.run_command(["mkdir", "-p", str(remote_folder)], user=user)
 
             # Package a few commands together in a script to speed things up
             src_folder = shlex.quote(str(remote_folder))
             tmp_folder = shlex.quote(str(temporary_remote_folder))
             tmp_folder_parent = shlex.quote(str(temporary_remote_folder.parent))
             move_folder_to_tmp = (
                 f"mkdir -p {tmp_folder_parent} && "
                 f"sudo rm -rf {tmp_folder} && "
                 f"sudo mv {src_folder} {tmp_folder} && "
-                f"sudo chown -R {self.ssh_user}:{self.ssh_user} {tmp_folder}"
+                f"sudo chown -R {shlex.quote(self.remote_user)}:{shlex.quote(self.remote_user)} {tmp_folder}"
             )
-            self.run_command([move_folder_to_tmp], shell=True, user=self.ssh_user)
+            self.run_command([move_folder_to_tmp], shell=True, user=None)
 
             # Do the sync with the temporary folder
-            self.sync_local_folder(local_folder, temporary_remote_folder, excludes=excludes, user=self.ssh_user)
+            self.sync_local_folder(local_folder, temporary_remote_folder, excludes=excludes, user=None)
 
             # Move the temporary folder back into its original location
-            move_tmp_to_folder = f"sudo chown -R {user}:{user} {tmp_folder} && sudo mv {tmp_folder} {src_folder}"
-            self.run_command([move_tmp_to_folder], shell=True, user=self.ssh_user)
+            move_tmp_to_folder = (
+                f"sudo chown -R {shlex.quote(user)}:{shlex.quote(user)} {tmp_folder} && sudo mv {tmp_folder} {src_folder}"
+            )
+            self.run_command([move_tmp_to_folder], shell=True, user=None)
             return
 
-        # Make sure target dir exists
-        self.run_command(["mkdir", "-p", str(remote_folder)])
+        # Make sure target dir exists and it belongs to the user that will be used for the sync
+        self.run_command(["mkdir", "-p", str(remote_folder)], user=None)
 
         cmd = [
             "rsync",
             "--exclude=.git",
             *[f"--exclude={exc}" for exc in excludes],
             "--delete",
             "-e",
-            " ".join(SSH_CMD + [f"-p {self.ssh_port}"]),
+            shlex.join(self.remote_shell),
             "-rl",
             f"{local_folder}/",
-            f"{self.ssh_user}@{self.host}:{remote_folder}/",
+            f"{self.remote_host}:{remote_folder}/",
         ]
         gitignore = local_folder / ".gitignore"
         if not gitignore.exists():
             LOGGER.warning("%s does not have a .gitignore file, it will be synced entirely", str(local_folder))
         else:
             cmd.insert(1, f"--filter=:- {gitignore}")
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/docker-compose.yml` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/my-server-conf.cfg`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/resources/setup_project.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/resources/setup_project.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm/wait_for_state.py` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm/wait_for_state.py`

 * *Files identical despite different names*

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-inmanta-lsm
-Version: 3.2.0
+Version: 3.3.0
 Summary: Common fixtures for inmanta LSM related modules
 Home-page: https://github.com/inmanta/pytest-inmanta-lsm
 Author: Inmanta
 Author-email: code@inmanta.com
 License: inmanta EULA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -22,14 +22,16 @@
 License-File: LICENSE
 Requires-Dist: pytest-inmanta~=2.5
 Requires-Dist: inmanta-lsm
 Requires-Dist: devtools
 
 # pytest-inmanta-lsm
 
+[![pypi version](https://img.shields.io/pypi/v/pytest-inmanta-lsm.svg)](https://pypi.python.org/pypi/pytest-inmanta-lsm/)
+
 A pytest plugin to test inmanta modules that use lsm, it is built on top of `pytest-inmanta` and `pytest-inmanta-extensions`
 
 ## Installation
 
 ```bash
 pip install pytest-inmanta-lsm
 ```
@@ -39,97 +41,243 @@
 This plugin is used to push code to a remote orchestrator and interact with it, via the LSM north-bound-api
 It requires an LSM enabled orchestrator, with no ssl or authentication enabled, in a default setup and ssh access to the orchestrator machine, with a user that has sudo permissions.
 
 ## Usage
 
 ### First case: using a remote orchestrator
 
-This plugin is built around the remote_orchestrator fixture.
+This plugin is built around the remote_orchestrator fixture and the `RemoteServiceInstance` class.
 
-A typical testcase using this plugin looks as follows:
+You can easily write a test case that sends your project to a remote orchestrator, exports its service catalog, then deploy a service.  
 ```python
-
-def test_full_cycle(project, remote_orchestrator):
+def test_deploy_service(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
     # get connection to remote_orchestrator
     client = remote_orchestrator.client
 
     # setup project
-    project.compile(
-        """
-        import quickstart
-        """
-    )
+    project.compile("import quickstart")
 
     # sync project and export service entities
     remote_orchestrator.export_service_entities()
 
     # verify the service is in the catalog
     result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
     assert result.code == 200
 
-    # get a ManagedInstance object, to simplifies interacting with a specific service instance
-    service_instance = remote_orchestrator.get_managed_instance(SERVICE_NAME)
+    # Test the synchronous service instance class
+    instance = remote_service_instance.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
+    )
 
-    # create an instance and wait for it to be up
-    service_instance.create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="up",
+    # Create the service instance and stop waiting in a transient state
+    created = instance.create(
+        {
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        wait_for_state="creating",
+        timeout=60,
+    )
+
+    # Wait for up state, we provide here the version from which we should follow the
+    # service, which is the version in which we last stopped following the service.  This
+    # guarantees that we don't "miss" the target state, in case it is a transient one, and
+    # don't confuse the start state for the target one in case it is the same one.
+    # The start version should always be the last version in which we know our service has
+    # been, BEFORE the target state we expect our service to go into.
+    instance.wait_for_state(
+        target_state="up",
+        start_version=created.version,
+        timeout=60,
+    )
+
+    # Delete the instance
+    instance.delete(wait_for_state="terminated", timeout=60)
+```
+> source: [test_quickstart.py::test_transient_state](./examples/quickstart/tests/test_quickstart.py)
+
+For a more advanced test case, you might also want to deploy multiple services.  You could either test them one by one, or, parallelize them, in order to:
+1. speed up the test case.
+2. test interference in between the services.
+
+In that case, the recommended way is to create an `async` helper, which follows the progress of your service, and instantiate multiple services with it, in a `sync` test case.
+```python
+async def service_full_cycle(
+    remote_orchestrator: remote_orchestrator.RemoteOrchestrator,
+    router_ip: str,
+    interface_name: str,
+    address: str,
+    vlan_id: int,
+    vlan_id_update: int,
+) -> None:
+    # Create an async service instance object
+    instance = remote_service_instance_async.RemoteServiceInstance(
+        remote_orchestrator=remote_orchestrator,
+        service_entity_name=SERVICE_NAME,
     )
 
-    # make validation fail by creating a duplicate
-    remote_orchestrator.get_managed_instance(SERVICE_NAME).create(
-        attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        wait_for_state="rejected",
+    # Create the service instance on the remote orchestrator
+    await instance.create(
+        {
+            "router_ip": router_ip,
+            "interface_name": interface_name,
+            "address": address,
+            "vlan_id": vlan_id,
+        },
+        wait_for_state="up",
+        timeout=60,
     )
 
-    service_instance.update(
-        attribute_updates={"vlan_id": 42},
+    # Update the vlan id
+    await instance.update(
+        [
+            inmanta_lsm.model.PatchCallEdit(
+                edit_id=str(uuid.uuid4()),
+                operation=inmanta_lsm.model.EditOperation.replace,
+                target="vlan_id",
+                value=vlan_id_update,
+            ),
+        ],
         wait_for_state="up",
+        timeout=60,
+    )
+
+    # Delete the instance
+    await instance.delete(wait_for_state="terminated", timeout=60)
+
+
+def test_full_cycle(project: plugin.Project, remote_orchestrator: remote_orchestrator.RemoteOrchestrator) -> None:
+    # get connection to remote_orchestrator
+    client = remote_orchestrator.client
+
+    # setup project
+    project.compile("import quickstart")
+
+    # sync project and export service entities
+    remote_orchestrator.export_service_entities()
+
+    # verify the service is in the catalog
+    result = client.lsm_service_catalog_get_entity(remote_orchestrator.environment, SERVICE_NAME)
+    assert result.code == 200
+
+    # Create a first service that should be deployed
+    first_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.17",
+        interface_name="eth1",
+        address="10.0.0.254/24",
+        vlan_id=14,
+        vlan_id_update=42,
     )
 
-    # break it down
-    service_instance.delete()
+    # Create another valid service
+    another_service = service_full_cycle(
+        remote_orchestrator=remote_orchestrator,
+        router_ip="10.1.9.18",
+        interface_name="eth2",
+        address="10.0.0.253/24",
+        vlan_id=15,
+        vlan_id_update=52,
+    )
 
+    # Run all the services
+    util.sync_execute_scenarios(first_service, another_service, timeout=60)
 ```
+> source: [test_quickstart.py::test_full_cycle](./examples/quickstart/tests/test_quickstart.py)
+
 
 ### Second case: mocking the lsm api
 
 This toolbox comes with one more fixture: `lsm_project`.  This fixture allows to run compile using the lsm model locally.  It has as advantage that:
  - You get a more fined grained control about what you want to see in your compile (choose the value of attributes, state, version, etc of your service).
  - If you only care about testing one specific case it is much faster than going through the full lifecycle on the remote orchestrator.
  - You don't need a running remote orchestrator, so you won't need to synchronize the full project anywhere.
 
 A simple usage would be as follow:
 ```python
-def test_model(lsm_project: lsm_project.LsmProject) -> None:
-    # Create a service object, you can modify it as you wish, depending on what you are trying to test
-    service = inmanta_lsm.model.ServiceInstance(
-        id=uuid.uuid4(),
-        environment=lsm_project.environment,
-        service_entity="vlan-assignment",
-        version=1,
-        config={},
-        state="start",
-        candidate_attributes={"router_ip": "10.1.9.17", "interface_name": "eth1", "address": "10.0.0.254/24", "vlan_id": 14},
-        active_attributes=None,
-        rollback_attributes=None,
-        created_at=datetime.datetime.now(),
-        last_updated=datetime.datetime.now(),
-        callback=[],
-        deleted=False,
-        deployment_progress=None,
-        service_identity_attribute_value=None,
-    )
-
-    # Add the service to the mocked server.  From now on it will be taken into account
-    # for EACH compile
-    lsm_project.add_service(service)
+def test_model(lsm_project: pytest_inmanta_lsm.lsm_project.LsmProject) -> None:
+    # Export the service entities
+    lsm_project.export_service_entities("import quickstart")
+
+    # Create a service.  This will add it to our inventory, in its initial state
+    # (as defined in the lifecycle), and fill in any default attributes we didn't
+    # provide.
+    service = lsm_project.create_service(
+        service_entity_name="vlan-assignment",
+        attributes={
+            "router_ip": "10.1.9.17",
+            "interface_name": "eth1",
+            "address": "10.0.0.254/24",
+            "vlan_id": 14,
+        },
+        # With auto_transfer=True, we follow the first auto transfers of the service's
+        # lifecycle, triggering a compile (validating compile when appropriate) for
+        # each state we meets.
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been created and is now in creating state
+    assert service.state == "creating"
+
+    # Assert that the default value has been added to our attributes
+    assert "value_with_default" in service.active_attributes
+
+    # Do a second compile, in the non-validating creating state
+    lsm_project.compile(service_id=service.id)
+
+    # Move to the up state
+    service.state = "up"
+    lsm_project.compile(service_id=service.id)
+
+    # Trigger an update on our service from the up state.  Change the vlan id
+    new_attributes = copy.deepcopy(service.active_attributes)
+    new_attributes["vlan_id"] = 15
+    lsm_project.update_service(
+        service_id=service.id,
+        attributes=new_attributes,
+        auto_transfer=True,
+    )
+
+    # Assert that the service has been updated and is now in update_inprogress state
+    assert service.state == "update_inprogress"
+
+```
+
+### Third case: development on an active environment.
+
+In some cases, (i.e. PoC) you might want to update the code of your module that is currently deployed in an environment.
+You can either start a new test case with pytest-inmanta-lsm's `remote_orchestrator` fixture, which will clear up everything
+and allow you to start from scratch.  Or you can use the similar `remote_orchestrator_access` fixture, which gives you the
+same handy `RemoteOrchestrator` object, but doesn't clear the environment of any existing services, or resources.  This allows
+you for example to re-export the service catalog, or re-synchronize your module's source code and keep all the existing services.
+
+To do so, simply create a test case using the `remote_orchestrator_access` fixture, and the same cli/env var options as used for
+normal pytest-inmanta-lsm test cases.
+```python
+def test_update_existing_environment(
+    project: plugin.Project,
+    remote_orchestrator_access: remote_orchestrator.RemoteOrchestrator,
+) -> None:
+    """
+    Make sure that it is possible to simply run a compile and export service entities,
+    without initially cleaning up the environment.
+    """
+
+    # Setup the compiler config
+    remote_orchestrator_access.setup_config()
+
+    # Do a local compile of our model
+    project.compile("import quickstart")
+
+    # Export service entities (and update the project)
+    remote_orchestrator_access.export_service_entities()
 
-    # Run a compile, with central focus the service we just created
-    lsm_project.compile("import quickstart", service_id=service.id)
 ```
 
 ## Options and environment variables
 
 The following options are available, each with a corresponding environment variable.
 
 
@@ -184,23 +332,36 @@
                         A path to a public key that should be set in the
                         container (overrides INMANTA_LSM_CONTAINER_PUB_KEY_FILE,
                         defaults to $HOME/.ssh/id_rsa.pub)
   --lsm-environment
                         The environment to use on the remote server (is created
                         if it doesn't exist) (overrides INMANTA_LSM_ENVIRONMENT,
                         defaults to 719c7ad5-6657-444b-b536-a27174cb7498)
-  --lsm-host=LSM_HOST   Remote orchestrator to use for the remote_inmanta
-                        fixture (overrides INMANTA_LSM_HOST, defaults to
-                        127.0.0.1)
+  --lsm-host=LSM_HOST   IP address or domain name of the remote orchestrator api we
+                        wish to use in our test. It will be picked up and used by the
+                        remote_orchestrator fixture.  This is also the default remote
+                        hostname, if it is not specified in the --lsm-rh option.
+                        (overrides INMANTA_LSM_HOST, defaults to 127.0.0.1)
   --lsm-no-clean        Don't cleanup the orchestrator after tests (for
                         debugging purposes) (overrides INMANTA_LSM_NO_CLEAN,
                         defaults to False)
   --lsm-srv-port
                         Port the orchestrator api is listening to (overrides
                         INMANTA_LSM_SRV_PORT, defaults to 8888)
+  --lsm-rsh=LSM_RSH     A command which allows us to start a shell on the remote
+                        orchestrator or send file to it.  When sending files, this value
+                        will be passed to the `-e` argument of rsync.  When running a
+                        command, we will append the host name and `sh` to this value,
+                        and pass the command to execute as input to the open remote
+                        shell. (overrides INMANTA_LSM_REMOTE_SHELL)
+  --lsm-rh=LSM_RH       The name of the host that we should try to open the remote
+                        shell on, as recognized by the remote shell command.  This
+                        doesn't have to strictly be a hostname, as long as it is a
+                        valid host identifier to the chosen rsh protocol. (overrides
+                        INMANTA_LSM_REMOTE_HOST)
   --lsm-ssh-port
                         Port to use to ssh to the remote orchestrator (overrides
                         INMANTA_LSM_SSH_PORT, defaults to 22)
   --lsm-ssh-user
                         Username to use to ssh to the remote orchestrator
                         (overrides INMANTA_LSM_SSH_USER, defaults to centos)
   --lsm-ssl             [True | False] Choose whether to use SSL/TLS or not when
```

### Comparing `pytest-inmanta-lsm-3.2.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt` & `pytest_inmanta_lsm-3.3.0/src/pytest_inmanta_lsm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 src/pytest_inmanta_lsm/lsm_project.py
 src/pytest_inmanta_lsm/managed_service_instance.py
 src/pytest_inmanta_lsm/orchestrator_container.py
 src/pytest_inmanta_lsm/parameters.py
 src/pytest_inmanta_lsm/plugin.py
 src/pytest_inmanta_lsm/py.typed
 src/pytest_inmanta_lsm/remote_orchestrator.py
+src/pytest_inmanta_lsm/remote_service_instance.py
+src/pytest_inmanta_lsm/remote_service_instance.pyi
+src/pytest_inmanta_lsm/remote_service_instance_async.py
+src/pytest_inmanta_lsm/util.py
 src/pytest_inmanta_lsm/wait_for_state.py
 src/pytest_inmanta_lsm.egg-info/PKG-INFO
 src/pytest_inmanta_lsm.egg-info/SOURCES.txt
 src/pytest_inmanta_lsm.egg-info/dependency_links.txt
 src/pytest_inmanta_lsm.egg-info/entry_points.txt
 src/pytest_inmanta_lsm.egg-info/requires.txt
 src/pytest_inmanta_lsm.egg-info/top_level.txt
```

### Comparing `pytest-inmanta-lsm-3.2.0/tests/test_containerized_orchestrator.py` & `pytest_inmanta_lsm-3.3.0/tests/test_containerized_orchestrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 import os
 import shutil
 import subprocess
 from pathlib import Path
 
 import utils
-import versions
-from packaging import version
 from pytest import Testdir, fixture
 
 HOME = os.getenv("HOME", "")
 
 
 @fixture
 def testdir(testdir: Testdir) -> Testdir:
@@ -77,12 +75,8 @@
     """Make sure that our plugin works."""
 
     testdir.copy_example("quickstart")
 
     utils.add_version_constraint_to_project(testdir.tmpdir)
 
     result = testdir.runpytest("tests/test_quickstart.py", "--lsm-ctr")
-
-    if versions.INMANTA_CORE_VERSION < version.Version("6"):
-        result.assert_outcomes(passed=2, skipped=1)
-    else:
-        result.assert_outcomes(passed=3)
+    result.assert_outcomes(passed=5)
```

### Comparing `pytest-inmanta-lsm-3.2.0/tests/test_partial.py` & `pytest_inmanta_lsm-3.3.0/tests/test_partial.py`

 * *Files identical despite different names*

