# Comparing `tmp/pop_cli-4.0.0.tar.gz` & `tmp/pop_cli-4.0.1.tar.gz`

## Comparing `pop_cli-4.0.0.tar` & `pop_cli-4.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-4.0.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/__main__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/config.yaml
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/config.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/console.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/init.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/ref.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/state.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_ref.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.0.0/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.0.0/README.rst
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-4.0.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/__main__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/config.yaml
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/config.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/console.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/init.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.0.1/src/hub/state.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.0.1/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.0.1/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.0.1/README.rst
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pop_cli-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pop_cli-4.0.1/PKG-INFO
```

### Comparing `pop_cli-4.0.0/.pre-commit-config.yaml` & `pop_cli-4.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/src/__main__.py` & `pop_cli-4.0.1/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/src/config.yaml` & `pop_cli-4.0.1/src/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 dyne:
   cli:
     - hub
 
 # python imports to put on the hub for this plugin
 import:
   - aioconsole
+  - aiopath
   - asyncio
   - builtins
+  - pdb
   - pickle
   - pprint
   - prompt_toolkit
   - readline
   - rlcompleter
   - sys
   - typing
```

### Comparing `pop_cli-4.0.0/src/hub/cli.py` & `pop_cli-4.0.1/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/src/hub/config.py` & `pop_cli-4.0.1/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/src/hub/console.py` & `pop_cli-4.0.1/src/hub/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/src/hub/init.py` & `pop_cli-4.0.1/src/hub/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,22 @@
     else:
         # Treat all the extra args as parameters for the named ref
         args, kwargs = await hub.cli.cli.parameters(OPT)
         await hub.log.debug(f"Args: {' '.join(args)}")
         await hub.log.debug(f"Kwargs: {' '.join(kwargs.keys())}")
 
     # Get the named reference from the hub
-    finder = await hub.cli.ref.find(ref)
+    finder = hub.lib.cpop.ref.find(hub, ref)
+
+    # Call or retrieve the object at the given ref
+    ret = await hub.cli.ref.resolve(finder, *args, **kwargs)
+
+    # output the results of finder to the console
+    await hub.cli.ref.output(ret)
 
     if OPT.cli.interactive:
         # Start an asynchronous interactive console
         await hub.cli.console.run(OPT=OPT, ref=finder)
-    else:
-        # Call or retrieve the object at the given ref
-        ret = await hub.cli.ref.resolve(finder, *args, **kwargs)
-
-        # output the results of finder to the console
-        await hub.cli.ref.output(ret)
 
     if hub_state_file:
         # Write the serialized hub to a file
         hub_state_file = await hub.cli.state.save(hub_state_file)
```

### Comparing `pop_cli-4.0.0/src/hub/state.py` & `pop_cli-4.0.1/src/hub/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,18 @@
         state_file (str): A pickle file that contains serialized hub data
         cli (str): The cli config to load on the new hub
     """
     state_file = hub.lib.aiopath.Path(state_file)
     if await state_file.exists():
         try:
             async with state_file.open("rb") as f:
-                state = hub.lib.pickle.loads(await f.read())
-        except Exception:
+                contents = await f.read()
+                state = hub.lib.pickle.loads(contents)
+        except Exception as e:
+            await hub.log.error(f"Error loading hub state: {e}")
             return
 
         if not state:
             return
 
         hub.__setstate__(state)
 
@@ -41,12 +43,16 @@
     Serialize the hub and write it to a file.
 
     Args:
         hub (pop.hub.Hub): The global namespace
         state_file (str): A pickle file to writ ethe serialized hub to.
     """
     state_file = hub.lib.aiopath.Path(state_file)
+    state_file = hub.lib.aiopath.Path(state_file)
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     await state_file.parent.mkdir(parents=True, exist_ok=True)
     async with state_file.open("wb") as f:
         await f.write(hub.lib.pickle.dumps(state))
+    await state_file.parent.mkdir(parents=True, exist_ok=True)
+    async with state_file.open("wb") as f:
+        await f.write(hub.lib.pickle.dumps(state))
```

### Comparing `pop_cli-4.0.0/tests/conftest.py` & `pop_cli-4.0.1/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import pathlib
 import sys
 from unittest import mock
 
+import aiopath
 import cpop.hub
 import pytest
 
 
 @pytest.fixture(name="hub")
 async def testing_hub():
     async with cpop.hub.Hub() as hub:
         yield hub
 
 
 @pytest.fixture(autouse=True, scope="session")
-def tpath():
-    code_dir = pathlib.Path(__file__).parent.parent.absolute()
-    assert code_dir.exists()
+async def tpath():
+    code_dir = await aiopath.AsyncPath(__file__).parent.parent.absolute()
+    assert await code_dir.exists()
 
     tpath_dir = code_dir / "tests" / "tpath"
-    assert tpath_dir.exists()
+    assert await tpath_dir.exists()
 
     NEW_PATH = [str(code_dir), str(tpath_dir)]
 
     for p in sys.path:
         if p not in NEW_PATH:
             NEW_PATH.append(p)
```

### Comparing `pop_cli-4.0.0/tests/integration/test_cli.py` & `pop_cli-4.0.1/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/tests/integration/test_config.py` & `pop_cli-4.0.1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/tests/integration/test_console.py` & `pop_cli-4.0.1/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/tests/integration/test_init.py` & `pop_cli-4.0.1/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/tests/integration/test_ref.py` & `pop_cli-4.0.1/tests/integration/test_ref.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Test find
 async def test_find(hub):
     # Set up a nested attribute on the hub for testing
     hub.nested = hub.lib.cpop.data.NamespaceDict({"level1": {"level2": "value"}})
 
     # Test finding a nested attribute
-    result = await hub.cli.ref.find("nested.level1.level2")
+    result = hub.lib.cpop.ref.find(hub, "nested.level1.level2")
     assert result == "value"
 
     # Test finding a non-existent attribute
     with hub.lib.pytest.raises(KeyError):
-        await hub.cli.ref.find("nonexistent.attribute")
+        hub.lib.cpop.ref.find(hub, "nonexistent.attribute")
 
 
 # Test resolve
 async def test_resolve_function(hub):
     # Set up a function on the hub for testing
     async def test_func():
         return "result"
```

### Comparing `pop_cli-4.0.0/tests/integration/test_state.py` & `pop_cli-4.0.1/tests/integration/test_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 async def test_save_and_load(hub, tmp_path):
-    state_file = tmp_path / "state.pkl"
+    state_file = str(tmp_path / "state.pkl")
 
     # Set some initial state on the hub
     hub.some_attribute = "test_value"
 
     # Save the hub state to a file
     await hub.cli.state.save(state_file)
-    await hub.lib.asyncio.sleep(0)
 
     # Clear the hub of these attributes
     hub._clear()
     hub._attrs.clear()
 
     # Set the state option to point to the state file
-    opts = hub.lib.cpop.data.ImmutableNamespaceDict(
-        {"cli": {"hub_state": str(state_file)}}
-    )
+    opts = hub.lib.cpop.data.ImmutableNamespaceDict({"cli": {"hub_state": state_file}})
 
     # Restore the hub state
     restored_file = await hub.cli.state.restore(opts)
-    await hub.lib.asyncio.sleep(0)
 
     # Verify that the hub's state is restored and the correct file path is returned
     assert str(restored_file) == str(state_file)
 
     # Verify that the attribute from earlier made it back onto the hub
     assert hub.some_attribute == "test_value"
```

### Comparing `pop_cli-4.0.0/.gitignore` & `pop_cli-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/README.rst` & `pop_cli-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-4.0.0/pyproject.toml` & `pop_cli-4.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "4.0.0"
+version = "4.0.1"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -16,23 +16,25 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
+    "aiopath",
     "cPop>=35.0.0",
     "aioconsole",
     "uvloop; sys_platform != 'win32'",
     "prompt-toolkit",
 ]
 
 
 [project.optional-dependencies]
 test = [
+    "cpop[test]",
     "pexpect",
     "pytest",
     "pytest-asyncio",
 ]
 
 [project.scripts]
 hub = "hub.__main__:main"
```

### Comparing `pop_cli-4.0.0/PKG-INFO` & `pop_cli-4.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 4.0.0
+Version: 4.0.1
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
+Requires-Dist: aiopath
 Requires-Dist: cpop>=35.0.0
 Requires-Dist: prompt-toolkit
 Requires-Dist: uvloop; sys_platform != 'win32'
 Provides-Extra: test
+Requires-Dist: cpop[test]; extra == 'test'
 Requires-Dist: pexpect; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
 
 =======
 Pop-cli
```

