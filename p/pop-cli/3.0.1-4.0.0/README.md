# Comparing `tmp/pop_cli-3.0.1.tar.gz` & `tmp/pop_cli-4.0.0.tar.gz`

## Comparing `pop_cli-3.0.1.tar` & `pop_cli-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-3.0.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/__main__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/config.yaml
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/config.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/console.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/init.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/ref.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pop_cli-3.0.1/src/hub/state.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_ref.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-3.0.1/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-3.0.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-3.0.1/README.rst
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pop_cli-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pop_cli-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-4.0.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/__main__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/config.yaml
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/config.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/console.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/init.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/ref.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 pop_cli-4.0.0/src/hub/state.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.0.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.0.0/README.rst
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-4.0.0/PKG-INFO
```

### Comparing `pop_cli-3.0.1/.pre-commit-config.yaml` & `pop_cli-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/src/config.yaml` & `pop_cli-4.0.0/src/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,16 @@
 dyne:
   cli:
     - hub
 
 # python imports to put on the hub for this plugin
 import:
   - aioconsole
-  - aiopath
   - asyncio
   - builtins
-  - pdb
   - pickle
   - pprint
   - prompt_toolkit
   - readline
   - rlcompleter
   - sys
   - typing
```

### Comparing `pop_cli-3.0.1/src/hub/cli.py` & `pop_cli-4.0.0/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/src/hub/config.py` & `pop_cli-4.0.0/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/src/hub/console.py` & `pop_cli-4.0.0/src/hub/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,18 @@
         except EOFError:
             # Exit handling...
             break
         except KeyboardInterrupt:
             # Keyboard interrupt handling...
             continue
         except Exception:
+            # Capture the current exception info
+            exc_type, exc_value, exc_traceback = hub.lib.sys.exc_info()
             # Error handling...
-            await hub.log.error(hub.lib.traceback.format_exc())
+            hub.lib.sys.excepthook(exc_type, exc_value, exc_traceback)
             continue
 
 
 async def get_completer(hub, **kwargs):
     """
     Creates a completer for the interactive console that provides completion suggestions for the 'hub' namespace.
```

### Comparing `pop_cli-3.0.1/src/hub/init.py` & `pop_cli-4.0.0/src/hub/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,22 @@
     else:
         # Treat all the extra args as parameters for the named ref
         args, kwargs = await hub.cli.cli.parameters(OPT)
         await hub.log.debug(f"Args: {' '.join(args)}")
         await hub.log.debug(f"Kwargs: {' '.join(kwargs.keys())}")
 
     # Get the named reference from the hub
-    finder = hub.lib.cpop.ref.find(hub, ref)
-
-    # Call or retrieve the object at the given ref
-    ret = await hub.cli.ref.resolve(finder, *args, **kwargs)
-
-    # output the results of finder to the console
-    await hub.cli.ref.output(ret)
+    finder = await hub.cli.ref.find(ref)
 
     if OPT.cli.interactive:
         # Start an asynchronous interactive console
         await hub.cli.console.run(OPT=OPT, ref=finder)
+    else:
+        # Call or retrieve the object at the given ref
+        ret = await hub.cli.ref.resolve(finder, *args, **kwargs)
+
+        # output the results of finder to the console
+        await hub.cli.ref.output(ret)
 
     if hub_state_file:
         # Write the serialized hub to a file
         hub_state_file = await hub.cli.state.save(hub_state_file)
```

### Comparing `pop_cli-3.0.1/src/hub/state.py` & `pop_cli-4.0.0/src/hub/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 async def restore(hub, opts: dict) -> str:
     # Try to get a saved hub
-    if opts.cli.hub_state:
-        hub_state = await hub.cli.cli.parse_value(opts.cli.hub_state)
+    try:
+        if opts.cli.hub_state:
+            hub_state = await hub.cli.cli.parse_value(opts.cli.hub_state)
+
+            # Load the saved state of the hub from a file in memory
+            hub_state_file = await hub.lib.aiopath.Path(hub_state).expanduser()
+            await hub.log.debug(f"Restoring hub from {hub_state_file}")
+            await hub.cli.state.load(hub_state_file)
+            return hub_state_file
+    except Exception as e:
+        await hub.log.error(f"Could not restore hub from '{hub_state_file}': {e}")
 
-        # Load the saved state of the hub from a file in memory
-        hub_state_file = str(await hub.lib.aiopath.Path(hub_state).expanduser())
-        await hub.log.debug(f"Restoring hub from {hub_state_file}")
-        await hub.cli.state.load(hub_state_file)
-        return hub_state_file
 
-
-async def load(hub, state_file: str):
-    """
+async def load(hub, state_file):
+    """_summary_
     Read a hub state from a pickle file and add its attributes to the current hub.
 
     Args:
         hub (pop.hub.Hub): The global namespace
         state_file (str): A pickle file that contains serialized hub data
         cli (str): The cli config to load on the new hub
     """
     state_file = hub.lib.aiopath.Path(state_file)
     if await state_file.exists():
         try:
             async with state_file.open("rb") as f:
-                contents = await f.read()
-                state = hub.lib.pickle.loads(contents)
-        except Exception as e:
-            await hub.log.error(f"Error loading hub state: {e}")
+                state = hub.lib.pickle.loads(await f.read())
+        except Exception:
             return
 
         if not state:
             return
 
         hub.__setstate__(state)
 
 
-async def save(hub, state_file: str):
+async def save(hub, state_file):
     """_summary_
     Serialize the hub and write it to a file.
 
     Args:
         hub (pop.hub.Hub): The global namespace
         state_file (str): A pickle file to writ ethe serialized hub to.
     """
```

### Comparing `pop_cli-3.0.1/tests/conftest.py` & `pop_cli-4.0.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+import pathlib
 import sys
-import unittest.mock as mock
+from unittest import mock
 
-import aiopath
 import cpop.hub
 import pytest
 
 
 @pytest.fixture(name="hub")
 async def testing_hub():
-    yield await cpop.hub.AsyncHub()
+    async with cpop.hub.Hub() as hub:
+        yield hub
 
 
 @pytest.fixture(autouse=True, scope="session")
-async def tpath():
-    code_dir = await aiopath.AsyncPath(__file__).parent.parent.absolute()
-    assert await code_dir.exists()
+def tpath():
+    code_dir = pathlib.Path(__file__).parent.parent.absolute()
+    assert code_dir.exists()
 
     tpath_dir = code_dir / "tests" / "tpath"
-    assert await tpath_dir.exists()
+    assert tpath_dir.exists()
 
     NEW_PATH = [str(code_dir), str(tpath_dir)]
 
     for p in sys.path:
         if p not in NEW_PATH:
             NEW_PATH.append(p)
```

### Comparing `pop_cli-3.0.1/tests/integration/test_cli.py` & `pop_cli-4.0.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/tests/integration/test_config.py` & `pop_cli-4.0.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/tests/integration/test_console.py` & `pop_cli-4.0.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/tests/integration/test_init.py` & `pop_cli-4.0.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/tests/integration/test_ref.py` & `pop_cli-4.0.0/tests/integration/test_ref.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Test find
 async def test_find(hub):
     # Set up a nested attribute on the hub for testing
     hub.nested = hub.lib.cpop.data.NamespaceDict({"level1": {"level2": "value"}})
 
     # Test finding a nested attribute
-    result = hub.lib.cpop.ref.find(hub, "nested.level1.level2")
+    result = await hub.cli.ref.find("nested.level1.level2")
     assert result == "value"
 
     # Test finding a non-existent attribute
     with hub.lib.pytest.raises(KeyError):
-        hub.lib.cpop.ref.find(hub, "nonexistent.attribute")
+        await hub.cli.ref.find("nonexistent.attribute")
 
 
 # Test resolve
 async def test_resolve_function(hub):
     # Set up a function on the hub for testing
     async def test_func():
         return "result"
```

### Comparing `pop_cli-3.0.1/.gitignore` & `pop_cli-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/README.rst` & `pop_cli-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-3.0.1/pyproject.toml` & `pop_cli-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "3.0.1"
+version = "4.0.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -16,25 +16,23 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "aiopath",
-    "cPop>=33.0.0",
+    "cPop>=35.0.0",
     "aioconsole",
     "uvloop; sys_platform != 'win32'",
     "prompt-toolkit",
 ]
 
 
 [project.optional-dependencies]
 test = [
-    "cpop[test]",
     "pexpect",
     "pytest",
     "pytest-asyncio",
 ]
 
 [project.scripts]
 hub = "hub.__main__:main"
```

### Comparing `pop_cli-3.0.1/PKG-INFO` & `pop_cli-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 3.0.1
+Version: 4.0.0
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
-Requires-Dist: aiopath
-Requires-Dist: cpop>=33.0.0
+Requires-Dist: cpop>=35.0.0
 Requires-Dist: prompt-toolkit
 Requires-Dist: uvloop; sys_platform != 'win32'
 Provides-Extra: test
-Requires-Dist: cpop[test]; extra == 'test'
 Requires-Dist: pexpect; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
 
 =======
 Pop-cli
```

