# Comparing `tmp/fbnconfig-0.0.38.tar.gz` & `tmp/fbnconfig-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbnconfig-0.0.38.tar", max compression
+gzip compressed data, was "fbnconfig-0.0.40.tar", max compression
```

## Comparing `fbnconfig-0.0.38.tar` & `fbnconfig-0.0.40.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      176 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/__init__.py
--rw-r--r--   0        0        0     6600 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/access.py
--rw-r--r--   0        0        0     6513 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/configuration.py
--rw-r--r--   0        0        0     4167 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/deploy.py
--rw-r--r--   0        0        0     8124 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/drive.py
--rw-r--r--   0        0        0     7488 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/identity.py
--rw-r--r--   0        0        0     1057 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/load_module.py
--rw-r--r--   0        0        0     9681 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/log.py
--rw-r--r--   0        0        0     8126 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/main.py
--rw-r--r--   0        0        0     6618 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/property.py
--rw-r--r--   0        0        0      771 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/resource_abc.py
--rw-r--r--   0        0        0    14708 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/scheduler.py
--rw-r--r--   0        0        0     8107 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig.md
--rw-r--r--   0        0        0     1070 2024-04-09 09:58:52.151540 fbnconfig-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     8639 1970-01-01 00:00:00.000000 fbnconfig-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/access.py
+-rw-r--r--   0        0        0     9838 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/configuration.py
+-rw-r--r--   0        0        0     4191 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/deploy.py
+-rw-r--r--   0        0        0     8124 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/drive.py
+-rw-r--r--   0        0        0     7488 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/identity.py
+-rw-r--r--   0        0        0     1057 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/load_module.py
+-rw-r--r--   0        0        0     9681 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/log.py
+-rw-r--r--   0        0        0     8283 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/main.py
+-rw-r--r--   0        0        0     6618 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/property.py
+-rw-r--r--   0        0        0      771 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/resource_abc.py
+-rw-r--r--   0        0        0    14708 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/scheduler.py
+-rw-r--r--   0        0        0     9716 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig.md
+-rw-r--r--   0        0        0     1070 2024-04-15 07:48:05.118508 fbnconfig-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0    10248 1970-01-01 00:00:00.000000 fbnconfig-0.0.40/PKG-INFO
```

### Comparing `fbnconfig-0.0.38/fbnconfig/access.py` & `fbnconfig-0.0.40/fbnconfig/access.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/configuration.py` & `fbnconfig-0.0.40/fbnconfig/configuration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 import httpx
 from .resource_abc import Resource, Ref
 from pydantic import BaseModel, Field, computed_field
 from enum import Enum
-from typing import Dict, Any
+from typing import Dict, Any, Union
+
 
 class SetType(str, Enum):
     PERSONAL = "personal"
     SHARED = "shared"
 
+
 class SetRef(BaseModel, Ref):
     """ Refer to an existing configuration set """
     id: str = Field(None, exclude=True, init=True)
     scope: str = Field(exclude=True, init=True)
     code: str = Field(exclude=True, init=True)
     type: SetType
 
@@ -33,15 +35,15 @@
 class SetResource(BaseModel, Resource):
     """ Manage a configuration set """
     id: str = Field(None, exclude=True, init=True)
     scope: str = Field(exclude=True, init=True)
     code: str = Field(exclude=True, init=True)
     description: str
     type: SetType
-    _remote: Dict[str, Any]|None = None
+    _remote: Dict[str, Any] | None = None
 
     @computed_field(alias="id")
     def setId(self) -> Dict[str, str]:
         return {"scope": self.scope, "code": self.code}
 
     def read(self, client, old_state):
         scope = self.scope
@@ -58,35 +60,36 @@
     @staticmethod
     def delete(client, old_state):
         type = old_state.type
         scope = old_state.scope
         code = old_state.code
         client.request("delete", f"/configuration/api/sets/{type}/{scope}/{code}")
 
-    def update(self, client, old_state) -> Dict[str, Any]|None:
+    def update(self, client, old_state) -> Dict[str, Any] | None:
         if [old_state.scope, old_state.code, old_state.type] != [self.scope, self.code, self.type.value]:
             raise RuntimeError("Cannot change the scope, code or type on a config set")
         self.read(client, old_state)
         assert self._remote is not None
         current = {"description": self._remote["description"]}
         desired = self.model_dump(mode="json", exclude_none=True, by_alias=True)
         desired.pop("id")
         desired.pop("type")
-        if(desired == current):
+        if (desired == current):
             return None
         client.put(f"/configuration/api/sets/{self.type.value}/{self.scope}/{self.code}", json=desired)
         return {"scope": self.scope, "code": self.code, "type": self.type.value}
 
     def deps(self):
         return []
 
+
 class ItemRef(BaseModel, Ref):
     """ Reference an existing configuration item with a set """
     id: str = Field(None, exclude=True, init=True)
-    set: SetRef|SetResource
+    set: SetRef | SetResource
     key: str
     ref: str = Field(None, exclude=False, init=False)
 
     def attach(self, client):
         type = self.set.type.value
         scope = self.set.scope
         code = self.set.code
@@ -96,21 +99,23 @@
             self.ref = get.json()["ref"]
         except httpx.HTTPStatusError as ex:
             if ex.response.status_code == 404:
                 raise RuntimeError("Config item not found")
             else:
                 raise ex
 
+
 class ValueType(str, Enum):
     TEXT = "text"
 
+
 class ItemResource(BaseModel, Resource):
     """ Manage a configuration item with a set """
     id: str = Field(None, exclude=True, init=True)
-    set: SetRef|SetResource = Field(exclude=True, init=True)
+    set: SetRef | SetResource = Field(exclude=True, init=True)
     key: str
     ref: str = Field(None, exclude=False, init=False)
     value: Any
     valueType: ValueType
     isSecret: bool
     description: str
     _remote: Dict[str, Any] = {}
@@ -157,17 +162,104 @@
             return self.create(client)
         self.read(client, old_state)
         # can't update these using PUT
         if self.isSecret != self._remote["isSecret"] or self.valueType != self._remote["valueType"]:
             self.delete(client, old_state)
             return self.create(client)
         self.ref = self._remote["ref"]
-        current = {k: v for k,v in self._remote.items() if k in ["description", "value"]}
+        current = {k: v for k, v in self._remote.items() if k in ["description", "value"]}
         desired = self.model_dump(mode="json", exclude_none=True, by_alias=True)
-        desired = {k: v for k,v in desired.items() if k in ["description", "value"]}
+        desired = {k: v for k, v in desired.items() if k in ["description", "value"]}
         if desired == current:
             return None
         client.put(f"/configuration/api/sets/{type}/{scope}/{code}/items/{key}", json=desired)
         return {"scope": scope, "code": code, "type": type, "key": self.key}
 
     def deps(self):
         return [self.set]
+
+
+class SystemConfigResource(BaseModel, Resource):
+    """ Manage a system configuration item
+
+        The default value is used to reset the system configuration value when the resource is deleted
+
+       Example
+       -------
+           >>> from fbnconfig import Deployment
+           >>> from fbnconfig.configuration import SystemConfigResource
+           >>> validate_instruments = SystemConfigResource(
+                    id="validate-instr",
+                    code="TransactionBooking",
+                    key="ValidateInstruments",
+                    value=True,
+                    description="Test from fbnconfig",
+                    default_value=False)
+           >>> Deployment("myDeployment", [validate_instruments])
+
+       Attributes
+       ----------
+       id : str
+         Resource identifier; this will be used in the log to reference the item resource
+       code : str
+         Code of the system configuration set; System configurations exist in the 'system' scope
+       key: str
+           Key of the set to use
+       value: Any
+           Configuration item value
+       default_value: Any
+         The value this configuration item will be set to when the resource is deleted
+         """
+    id: str = Field(None, exclude=True, init=True)
+    code: str = Field(None, exclude=True, init=True)
+    key: str
+    value: str
+    default_value: Any = Field(None, exclude=True, init=True)
+    description: str
+    _remote: Dict[str, Any] = {}
+
+    def read(self, client, old_state):
+        code = old_state.code
+        key = old_state.key
+        get = client.get(f"/configuration/api/sets/system/{code}/items/{key}")
+        self._remote = get.json()["values"][0]
+
+    def create(self, client):
+        desired = self.model_dump(mode="json", exclude_none=True)
+        result = client.put(
+            f"/configuration/api/sets/shared/system/{self.code}/items/{self.key}",
+            json=desired
+        )
+        if result is None:
+            raise RuntimeError("Something wrong creating config item")
+        return {"code": self.code, "key": self.key, "default_value": self.default_value}
+
+    @staticmethod
+    def delete(client, old_state):
+        if old_state.default_value is None:
+            pass
+        else:
+            desired = {"value": old_state.default_value}
+            client.put(
+                f"/configuration/api/sets/shared/system/{old_state.code}/items/{old_state.key}",
+                json=desired)
+
+    def update(self, client, old_state) -> Union[None, Dict[str, Any]]:
+        code = self.code
+        key = self.key
+
+        if self.key != old_state.key or code != old_state.code:
+            self.delete(client, old_state)
+            return self.create(client)
+
+        self.read(client, old_state)
+
+        current = {k: v for k, v in self._remote.items() if k in ["description", "value"]}
+        desired = self.model_dump(mode="json", exclude_none=True, by_alias=True)
+        desired = {k: v for k, v in desired.items() if k in ["description", "value"]}
+        if desired == current:
+            return None
+        client.put(f"/configuration/api/sets/shared/system/{code}/items/{key}", json=desired)
+        return {"code": code, "key": self.key, "default_value": self.default_value}
+
+    def deps(self):
+        return []
```

### Comparing `fbnconfig-0.0.38/fbnconfig/deploy.py` & `fbnconfig-0.0.40/fbnconfig/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from .resource_abc import Resource, Ref
 
 # import all resources here, so they are available in globals()
 from .drive import FolderResource, FileResource  # noqa: F401
 from .scheduler import ImageResource, JobResource, ScheduleResource  # noqa: F401
 from .access import PolicyResource, RoleResource  # noqa: F401
 from .identity import IdentityRoleResource, UserResource, RoleAssignment  # noqa: F401
-from .configuration import SetResource, ItemResource # noqa: F401
-from .property import DefinitionResource # noqa: F401
+from .configuration import SetResource, ItemResource, SystemConfigResource  # noqa: F401
+from .property import DefinitionResource  # noqa: F401
 
 Deployment = NamedTuple("Deployment", [("id", str), ("resources", List[Union[Resource, Ref]])])
 deployments = []
 
 
 def deployment(id, resources):
     d = Deployment(id, resources)
```

### Comparing `fbnconfig-0.0.38/fbnconfig/drive.py` & `fbnconfig-0.0.40/fbnconfig/drive.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/identity.py` & `fbnconfig-0.0.40/fbnconfig/identity.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/load_module.py` & `fbnconfig-0.0.40/fbnconfig/load_module.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/log.py` & `fbnconfig-0.0.40/fbnconfig/log.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/main.py` & `fbnconfig-0.0.40/fbnconfig/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from . import log as deployment_log
 from httpx import RequestError, HTTPStatusError
 from json import dumps
 from .load_module import load_module
 
 help_footer = "environment defaults to $LUSID_ENV and token defaults to $FBN_ACCESS_TOKEN"
 
+
 def http_exception_handler(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except RequestError as exc:
             msg = f"An error occurred while requesting {exc.request.url!r} before we got a response"
@@ -21,39 +22,44 @@
         except HTTPStatusError as exc:
             status = exc.response.status_code
             base_msg = " ".join([
                 f"The server responded with {exc.response.status_code}",
                 f"while requesting {exc.request.method} {exc.request.url!r}",
             ])
             if exc.response.is_server_error:
-                detail = [ exc.response.text ]
+                detail = [exc.response.text]
             elif exc.response.json().get("name", "") == "AccessDenied":
                 detail = [
                     exc.response.json().get("detail"),
                     exc.response.json().get("instance")
                 ]
             elif status == 400:
-                detail = [ exc.response.text ]
+                detail = [exc.response.text]
+            elif status == 404:
+                error_detail = exc.response.json().get("detail", None)
+                detail = [error_detail if not None else exc.response.text]
             else:
-                detail = [ exc.response.text ]
+                detail = [exc.response.text]
             msg_str = "\n".join([base_msg] + detail)
             raise click.ClickException(msg_str)
 
     return wrapper
 
+
 def runtime_error_handler(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except RuntimeError as exc:
-            raise click.ClickException("Runtime Error: " + str(exc))
+            raise click.ClickException(str(exc))
 
     return wrapper
 
+
 @click.group()
 @click.version_option(message="%(version)s")
 def cli():
     pass
 
 
 @cli.command(epilog=help_footer)
@@ -167,14 +173,15 @@
     else:
         deployment_log.remove(client, deployment, resource_id)
         click.echo(f"   Removed entry for '{resource_id}' in deployment '{deployment}'")
 
 
 cli.add_command(log)
 
+
 @cli.command(epilog=help_footer)
 @click.option("-e", "--environment", type=str, envvar="LUSID_ENV")
 @click.option("-t", "--access-token", type=str, envvar="FBN_ACCESS_TOKEN")
 @click.option("-v", "--vars_file", type=click.File("r"))
 @click.argument("script_path", type=click.Path(readable=True))
 @http_exception_handler
 @click.pass_context
@@ -195,9 +202,10 @@
             )
 
         d = module.configure(host_vars)
     except ImportError as e:
         raise click.ClickException(f"Failed importing user config: [{script_path}]. Error : \n{e}")
     deploy(d, environment, access_token)
 
+
 if __name__ == "__main__":
     cli()
```

### Comparing `fbnconfig-0.0.38/fbnconfig/property.py` & `fbnconfig-0.0.40/fbnconfig/property.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/resource_abc.py` & `fbnconfig-0.0.40/fbnconfig/resource_abc.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig/scheduler.py` & `fbnconfig-0.0.40/fbnconfig/scheduler.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.38/fbnconfig.md` & `fbnconfig-0.0.40/fbnconfig.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,254 @@
 # fbnconfig
+
 [![pypi](https://img.shields.io/pypi/v/fbnconfig)](https://pypi.org/project/fbnconfig/)
 [![python](https://img.shields.io/pypi/pyversions/fbnconfig.svg)](https://pypi.python.org/pypi/fbnconfig)
 
-fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID
-environment setup. It allows you to specify the desired state and, when you deploy, it will converge
-the LUSID env to that state by creating, updating or deleting entities within lusid so that the
-lusid environment and the desired state match.
+fbnconfig is a Python library (and commandline tool) to allow a declarative description of a LUSID
+environment. It allows you to specify the desired state and, when you deploy, it converges the
+LUSID environment to your desired state by creating, updating, or deleting entities within LUSID
+so that the LUSID environment and the desired state match.
 
 ## Getting started
+
 fbnconfig is available from PyPi
-```
+
+```cli
 pip install fbnconfig
 ```
 
 ## Running the command
 
-```
+```cli
 fbnconfig -e https://foo.lusid.com -t <token> run path/to/script.py
 ```
 
 This will apply the deployment script (script.py) to the foo.lusid.com domain.
 
-There are other commands for viewing what has been deployed.  Use `fbnconfig --help`.
+For a list of commands that let you view what's already deployed, use `fbnconfig --help`.
 
 ## Authentication
 
-fbnconfig needs a lusid url and a valid token. These can be passed on the commandline:
-
-```
-fbnconfig -e https://foo.lusid.com -t xyzabc1234 ...
-```
+fbnconfig needs a valid LUSID url and a token to create and modify a LUSID environment.
+The token will most likely be a personal access token (PAT), but could be a token from an
+authentication exchange. For more information on PATs and how to create them, start by reading
+[What is a personal access token?](https://support.lusid.com/knowledgebase/article/KA-01911/) on
+FINBOURNE's Knowledge Base.
 
-or as environment variables (this is the best way to deal with the token):
+We recommend configuring the url and token as environment variables:
 
-```
+```environment
 FBN_ACCESS_TOKEN=xyzabc1234
 LUSID_ENV=https://foo.lusid.com
 fbnconfig ...
 ```
 
-The token needs to be a valid token from an authentication exchange or, more likely, a personal
-access token (PAT).
+Alternatively, you can use the commandline:
+
+```cli
+fbnconfig -e https://foo.lusid.com -t xyzabc1234 ...
+```
 
 ## Writing the deployment script
 
-Using fbnconfig is about defining one or more "Deployments". A Deployment is a list of "Resources"
+A fbnconfig configure script is a Python file that includes the `configure(env):` function. When you
+create an fbnconfig configure script, you must define one or more `Deployments`.
 
-```
+For example, the following code is a valid fbnconfig configure script. The configure script defines
+the desired state, and running it changes the remote LUSID environment to match.
+
+```Python
 from fbnconfig import drive
 from fbnconfig import Deployment
 
 
 def configure(env):
     f1 = drive.FolderResource(id="base_folder", name="my_folder", parent=drive.root)
     return Deployment("my_deployment", [f1])
 ```
 
-
-* Configure scripts are python files. They need to import references resource like a normal python
-  script would
-* The entrypoint is a function called `configure` which should return a `Deployment`
-* Deployments contain one or more resources. In this case, a `FolderResource`
-
-When we run this script the first time it will create a folder in Drive called `my_folder`. The
-second time we run it, it knows the folder already exists and will not make any changes. If we
-change the name of the folder `name="another_name"` and run fbnconfig again it will rename the
-folder in drive. The script defines the desired state, fbnconfig makes the changes to bring the
-remote lusid state to match.
-
-## Deployment and Resource Ids
-
-fbnconfig uses the `id` provided to keep track of what needs changing. We can change the `name` of a
-folder and it will get renamed because it has the same `id`. If we change the `id` then the existing
-folder will get deleted and a new one will be created.
-
-* A `Deployment` has an `id` which is used to identify it in the system. fbnconfig tracks resources
-  using the deployment `id`. These `id`s need to be unique across all deployments within lusid.
-* Resources have an `id`. This is how resources within a deployment are tracked. These ids need to
-  be unique within a deployment
-* The folder also has python variable that references it, `f1`. This is used to identify the
-  resource within the script, but it's not used for tracking changes in lusid.
-
-Changing the ID of an existing resource means deleting the old one and creating a new one.
-
-Changing the ID of a deployment will leave the old deployment and create a new one with new
-resources.
-
-Changing the python variable names will not affect what gets deployed.
+* Configure scripts need to import references resource like a normal Python
+  script would.
+* The `configure(env):`  function is the entrypoint, which should return a `Deployment`.
+* `Deployments` contain one or more resources. In this case, the `Deployment` contains a single
+  `FolderResource` Resource that's saved in the `f1` variable.
+
+When we run this script the first time it will create a folder in LUSID Drive called `my_folder`.
+The second time we run it, fbnconfig knows the folder already exists and will not make any changes.
+If we change the name of the folder (for example `name="another_name"`) and run fbnconfig again it
+will rename the folder in LUSID Drive.
+
+### Deployment and Resource Ids
+
+Deployments require an `id`. In this example we define a value of `my_deployment` for the
+Deployment's `id` when we return the Deployment object.  
+
+Be careful if you change the ID of a Deployment. If you change the ID and re-run the configure
+script, fbnconfig creates a new LUSID environment with a new Deployment ID and new Resources.
+The previous Deployment's Resources are not automatically removed.
+
+Each Resource must also have an `id` and these `id`s must be unique within the fbnconfig Deployment.
+In this example, we use `id="base_folder"` to uniquely identify the folder Resource we create.
+
+* We can change the `name` of a folder and it will get renamed
+  because it has the same `id`.
+* If we change the `id` then the existing folder will be deleted and a new one will be created. Note
+  that the original folder does not persist, because fbnconfig configure scripts are declarative
+  fbnconfig makes the LUSID state match the configure file state. If the original folder disappears
+  from the configure file, fbnconfig makes the original folder disappear from the corresponding
+  LUSID environment.
+* The Python variable `f1` that references the folder is only used to identify the resource within
+  the Python configure script. This variable is not used for tracking changes in LUSID, therefore
+  changing the Python variable names does not affect what gets deployed.
 
 ## Dependencies
 
-Resources may need to reference other resources:
+Resources may need to reference other resources. For example, the following code creates the nested
+folder Resources.
 
-```
+```Python
 def configure(env):
     f1 = drive.FolderResource(id="base_folder", name="my_folder", parent=drive.root)
     f2 = drive.FolderResource(id="sub_folder", name="my_subfolder", parent=f1)
     return Deployment("my_deployment", [f1, f2])
 ```
 
-If we run this it will create the structure `/my_folder/my_subfolder`. Using the python variable
-names we say that `my_subfolder` (`f1` in the script) is a subfolder of it's parent `my_folder`
-(`f2` in the script).  Relationships are defined by the python variables.
-
-The deployment can reference `[f1, f2]` including both folders or it can reference `[f2]`. Because
-`f2` depends on `f1`, `f1` will be implicitly included.
+If we run this it will create the structure `/my_folder/my_subfolder`. Using the Python variable
+names we say that `my_subfolder` (`f1` in the script) is a subfolder of its parent `my_folder`
+(`f2` in the script).  Relationships are defined by the Python variables, in this case `parent=f1`.
+
+When we have nested structures like this, fbnconfig creates the parents before the children. For
+example, `f1` would get created (or updated) before `f2`, and if they are removed from the
+deployment then `f2` will be deleted before `f1`.
 
-fbnconfig will make sure that `f1` gets created (or updated) before `f2`, if they are removed
-from the deployment, then `f2` will be deleted before `f1`
+This example references both folders (`[f1, f2]`), however we could instead reference just the
+subfolder (`[f2]`). Because `f2` depends on `f1`, `f1` will be implicitly included.
 
 ## Dependencies outside the deployment
 
-When we put resources in a deployment they are fully managed by fbnconfig. Removing a resource from
-the deployment will delete it from lusid. This means, we mostly want to manage all related resources
-within a single deployment.
-
-However, if there are existing resources and we need to establish a relationship we can use a `Ref`.
-Suppose that `downloads` folder already exists because it has been created manually or is part of
-another deployment.
+When we define a Deployment in a configure script and use fbnconfig to create the corresponding
+LUSID environment, all the underlying Resources are fully managed by fbnconfig. This means we want
+to use fbnconfig to manage all related Resources within a single Deployment.
+
+However, if we need to establish a relationship between existing Resources and our configure script,
+we can use a `Ref`. In the following example, we account for the `downloads` folder which already
+exists because it has been created manually or is part of another Deployment.
 
-```
+```Python
 def configure(env):
     f1 = drive.FolderRef(id="downloads", name="downloads")
     f2 = drive.FolderResource(id="sub_folder", name="my_subfolder", parent=f1)
     return Deployment("my_deployment", [f1, f2])
 ```
 
-will create `sub_folder` within `downloads`. The downloads folder will be the parent, but it won't
-be managed within this deployment. If it doesn't exist at the time this is run, then it will error.
-If `f1` is removed, it won't get deleted because it is not being managed in this deployment.
+* This code will create `sub_folder` within the existing `downloads` Resource. We tell fbnconfig
+  that `downloads` already exists by using the `drive.FolderRef()` function instead of
+  `drive.FolderResource()`.
+* If `downloads` doesn't exist at the time this is run, we get an error.
+* The `downloads` folder will be the parent of `sub_folder`, but it won't be managed within this
+  Deployment.
+* If `f1` is removed, it won't get deleted because it is not being managed in this deployment.
 
 ## The vars file
 
-To aid with using the same script for dev, uat and prod, `fbnconfig` takes a commandline argument to
-a json file called the "vars file". The vars file is parsed and passed into the configure function
-(called `env` in the examples above).
+To aid with using the same script for dev, uat, and prod, fbnconfig takes a commandline argument to
+a json file called the "vars file". The vars file (called `env` in the examples above) is
+parsed and passed into the configure function.
 
-Say we wanted to use different email for dev and prod (like the environment variable example above):
+For example, suppose we wanted to use different email for dev and prod (like the environment
+variable example above).
 
-We would create two vars files
+We would:
 
-```
+1. Create two vars files.
+
+```json
 // prod.json                                    // dev.json
 {                                               {
     "email": "prod@company.com"                     "email": "dev@company.com"
 }                                               }
 ```
 
-reference them from the script var env:
-
-```
-def configure(env):
-    export_user = identity.UserResource(
-        id="user2",
-        ...
-        emailAddress=env.email,
-    )
-```
-
-Then running:
-
-```
-fbnconfig -e https://dev.lusid.com -v dev.json script.py
-```
+1. Reference the files from the script var env.
 
-Will use the `dev@company.com` email.
+    ```Python
+    def configure(env):
+        export_user = identity.UserResource(
+            id="user2",
+            ...
+            emailAddress=env.email,
+        )
+    ```
+
+1. Run the following command to use the `dev@company.com` email..
+
+    ```cli
+    fbnconfig -e https://dev.lusid.com -v dev.json script.py
+    ```
 
 These vars files can be comitted to the repo to capture variations between environments. For
-secrets, it's better to use explicit environment variables in the script (see below)
+secrets, it's better to use explicit environment variables in the script (see below).
 
-## Using python in the script
+## Using Python in the script
 
-A deployment script is normal python so python language features are available. Variables,
-f-strings, os.environ can all be used within the script:
+A deployment script is normal Python, so Python language features are available. For example
+variables and f-strings. To allow values to depend on the environment, you can use `os.environ` to
+initialise the variables. This is useful when setting up secrets in the config store.
 
-To allow values to depend on the environment use `os.environ` to initialise the variables:
+For example, the following code:
 
-```
+1. Passes the secret as an environment variable.
+2. Makes an http request or use a library from a vault provider to source the
+secret.
+3. Uses the secret inside the configure function.
+
+```Python
 import os
 
 company = os.environ["company"]
 
 def configure(env):
     export_user = identity.UserResource(
         id="user2",
         ...
         emailAddress=f"exports@{company}",
         login=f"exports@{company}",
     )
 ```
 
-This is useful when setting up secrets in the config store. Pass the secret as an
-environment variable, make a http request or use a library from a vault provider to source the
-secret then use it inside the configure function.
-
-You can even create resources in a loop:
+You can even create resources in a loop, for example:
 
-```
+```Python
 def configure(env):
     folders = [
         drive.FolderResource(id=f"folder_{i}", name="i", parent=drive.root)
         for i in range(0, 10)
     ]
     return Deployment('ten-folders', folders)
 ```
 
-The python variables for the resources need to be added to the deployment
-and each resource must have a unique `id`.
+The Python variables for the Resources need to be added to the deployment and each Resource must
+have a unique `id`.
 
 ## Using fbnconfig as a library
 
-Using fbnconfig from the commandline dyamically loads your python script and executes the
-deployment. In some cases (eg using fbnconfig as part of another application) you can call it from
-python as well.
+Using fbnconfig from the commandline dyamically loads your Python script and executes the
+Deployment. In some cases (for example using fbnconfig as part of another application) you can call
+it from Python as well.
+
+The following example creates an empty deployment called "my-jobs":
+
+```Python
+from os import environ
+from fbnconfig import Deployment, deploy
 
-This creates an empty deployment called "my-jobs":
-
-```
-import fbnconfig
-import os
 
 def configure(env):
     return Deployment("my-jobs", [])
 
 
 host_vars = {}
 lusid_url = "https://foo.lusid.com"
-token = os.environ["MY_TOKEN_VAR"])
+token = environ["MY_TOKEN_VAR"]
 deployment = configure(host_vars)
-fbnconfig.deploy(deployment, lusid_url, token)
+deploy(deployment, lusid_url, token)
 ```
-
-
```

### Comparing `fbnconfig-0.0.38/pyproject.toml` & `fbnconfig-0.0.40/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbnconfig"
-version = "0.0.38"
+version = "0.0.40"
 description = "fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment"
 authors = ["FINBOURNE Technology <engineering@finbourne.com>"]
 readme = "fbnconfig.md"
 
 [tool.poetry.scripts]
 fbnconfig = 'fbnconfig.main:cli'
 
@@ -16,15 +16,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest-xdist = "^3.5.0"
 coverage= "^7.4.1"
 ruff = "^0.3.3"
 respx = "^0.20.2"
 pytest = "^8.1.1"
-pyright = "^1.1.354"
+pyright = "^1.1.355"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `fbnconfig-0.0.38/PKG-INFO` & `fbnconfig-0.0.40/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,249 +1,269 @@
 Metadata-Version: 2.1
 Name: fbnconfig
-Version: 0.0.38
+Version: 0.0.40
 Summary: fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment
 Author: FINBOURNE Technology
 Author-email: engineering@finbourne.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.25.2,<0.26.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # fbnconfig
+
 [![pypi](https://img.shields.io/pypi/v/fbnconfig)](https://pypi.org/project/fbnconfig/)
 [![python](https://img.shields.io/pypi/pyversions/fbnconfig.svg)](https://pypi.python.org/pypi/fbnconfig)
 
-fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID
-environment setup. It allows you to specify the desired state and, when you deploy, it will converge
-the LUSID env to that state by creating, updating or deleting entities within lusid so that the
-lusid environment and the desired state match.
+fbnconfig is a Python library (and commandline tool) to allow a declarative description of a LUSID
+environment. It allows you to specify the desired state and, when you deploy, it converges the
+LUSID environment to your desired state by creating, updating, or deleting entities within LUSID
+so that the LUSID environment and the desired state match.
 
 ## Getting started
+
 fbnconfig is available from PyPi
-```
+
+```cli
 pip install fbnconfig
 ```
 
 ## Running the command
 
-```
+```cli
 fbnconfig -e https://foo.lusid.com -t <token> run path/to/script.py
 ```
 
 This will apply the deployment script (script.py) to the foo.lusid.com domain.
 
-There are other commands for viewing what has been deployed.  Use `fbnconfig --help`.
+For a list of commands that let you view what's already deployed, use `fbnconfig --help`.
 
 ## Authentication
 
-fbnconfig needs a lusid url and a valid token. These can be passed on the commandline:
-
-```
-fbnconfig -e https://foo.lusid.com -t xyzabc1234 ...
-```
+fbnconfig needs a valid LUSID url and a token to create and modify a LUSID environment.
+The token will most likely be a personal access token (PAT), but could be a token from an
+authentication exchange. For more information on PATs and how to create them, start by reading
+[What is a personal access token?](https://support.lusid.com/knowledgebase/article/KA-01911/) on
+FINBOURNE's Knowledge Base.
 
-or as environment variables (this is the best way to deal with the token):
+We recommend configuring the url and token as environment variables:
 
-```
+```environment
 FBN_ACCESS_TOKEN=xyzabc1234
 LUSID_ENV=https://foo.lusid.com
 fbnconfig ...
 ```
 
-The token needs to be a valid token from an authentication exchange or, more likely, a personal
-access token (PAT).
+Alternatively, you can use the commandline:
+
+```cli
+fbnconfig -e https://foo.lusid.com -t xyzabc1234 ...
+```
 
 ## Writing the deployment script
 
-Using fbnconfig is about defining one or more "Deployments". A Deployment is a list of "Resources"
+A fbnconfig configure script is a Python file that includes the `configure(env):` function. When you
+create an fbnconfig configure script, you must define one or more `Deployments`.
 
-```
+For example, the following code is a valid fbnconfig configure script. The configure script defines
+the desired state, and running it changes the remote LUSID environment to match.
+
+```Python
 from fbnconfig import drive
 from fbnconfig import Deployment
 
 
 def configure(env):
     f1 = drive.FolderResource(id="base_folder", name="my_folder", parent=drive.root)
     return Deployment("my_deployment", [f1])
 ```
 
-
-* Configure scripts are python files. They need to import references resource like a normal python
-  script would
-* The entrypoint is a function called `configure` which should return a `Deployment`
-* Deployments contain one or more resources. In this case, a `FolderResource`
-
-When we run this script the first time it will create a folder in Drive called `my_folder`. The
-second time we run it, it knows the folder already exists and will not make any changes. If we
-change the name of the folder `name="another_name"` and run fbnconfig again it will rename the
-folder in drive. The script defines the desired state, fbnconfig makes the changes to bring the
-remote lusid state to match.
-
-## Deployment and Resource Ids
-
-fbnconfig uses the `id` provided to keep track of what needs changing. We can change the `name` of a
-folder and it will get renamed because it has the same `id`. If we change the `id` then the existing
-folder will get deleted and a new one will be created.
-
-* A `Deployment` has an `id` which is used to identify it in the system. fbnconfig tracks resources
-  using the deployment `id`. These `id`s need to be unique across all deployments within lusid.
-* Resources have an `id`. This is how resources within a deployment are tracked. These ids need to
-  be unique within a deployment
-* The folder also has python variable that references it, `f1`. This is used to identify the
-  resource within the script, but it's not used for tracking changes in lusid.
-
-Changing the ID of an existing resource means deleting the old one and creating a new one.
-
-Changing the ID of a deployment will leave the old deployment and create a new one with new
-resources.
-
-Changing the python variable names will not affect what gets deployed.
+* Configure scripts need to import references resource like a normal Python
+  script would.
+* The `configure(env):`  function is the entrypoint, which should return a `Deployment`.
+* `Deployments` contain one or more resources. In this case, the `Deployment` contains a single
+  `FolderResource` Resource that's saved in the `f1` variable.
+
+When we run this script the first time it will create a folder in LUSID Drive called `my_folder`.
+The second time we run it, fbnconfig knows the folder already exists and will not make any changes.
+If we change the name of the folder (for example `name="another_name"`) and run fbnconfig again it
+will rename the folder in LUSID Drive.
+
+### Deployment and Resource Ids
+
+Deployments require an `id`. In this example we define a value of `my_deployment` for the
+Deployment's `id` when we return the Deployment object.  
+
+Be careful if you change the ID of a Deployment. If you change the ID and re-run the configure
+script, fbnconfig creates a new LUSID environment with a new Deployment ID and new Resources.
+The previous Deployment's Resources are not automatically removed.
+
+Each Resource must also have an `id` and these `id`s must be unique within the fbnconfig Deployment.
+In this example, we use `id="base_folder"` to uniquely identify the folder Resource we create.
+
+* We can change the `name` of a folder and it will get renamed
+  because it has the same `id`.
+* If we change the `id` then the existing folder will be deleted and a new one will be created. Note
+  that the original folder does not persist, because fbnconfig configure scripts are declarative
+  fbnconfig makes the LUSID state match the configure file state. If the original folder disappears
+  from the configure file, fbnconfig makes the original folder disappear from the corresponding
+  LUSID environment.
+* The Python variable `f1` that references the folder is only used to identify the resource within
+  the Python configure script. This variable is not used for tracking changes in LUSID, therefore
+  changing the Python variable names does not affect what gets deployed.
 
 ## Dependencies
 
-Resources may need to reference other resources:
+Resources may need to reference other resources. For example, the following code creates the nested
+folder Resources.
 
-```
+```Python
 def configure(env):
     f1 = drive.FolderResource(id="base_folder", name="my_folder", parent=drive.root)
     f2 = drive.FolderResource(id="sub_folder", name="my_subfolder", parent=f1)
     return Deployment("my_deployment", [f1, f2])
 ```
 
-If we run this it will create the structure `/my_folder/my_subfolder`. Using the python variable
-names we say that `my_subfolder` (`f1` in the script) is a subfolder of it's parent `my_folder`
-(`f2` in the script).  Relationships are defined by the python variables.
-
-The deployment can reference `[f1, f2]` including both folders or it can reference `[f2]`. Because
-`f2` depends on `f1`, `f1` will be implicitly included.
+If we run this it will create the structure `/my_folder/my_subfolder`. Using the Python variable
+names we say that `my_subfolder` (`f1` in the script) is a subfolder of its parent `my_folder`
+(`f2` in the script).  Relationships are defined by the Python variables, in this case `parent=f1`.
+
+When we have nested structures like this, fbnconfig creates the parents before the children. For
+example, `f1` would get created (or updated) before `f2`, and if they are removed from the
+deployment then `f2` will be deleted before `f1`.
 
-fbnconfig will make sure that `f1` gets created (or updated) before `f2`, if they are removed
-from the deployment, then `f2` will be deleted before `f1`
+This example references both folders (`[f1, f2]`), however we could instead reference just the
+subfolder (`[f2]`). Because `f2` depends on `f1`, `f1` will be implicitly included.
 
 ## Dependencies outside the deployment
 
-When we put resources in a deployment they are fully managed by fbnconfig. Removing a resource from
-the deployment will delete it from lusid. This means, we mostly want to manage all related resources
-within a single deployment.
-
-However, if there are existing resources and we need to establish a relationship we can use a `Ref`.
-Suppose that `downloads` folder already exists because it has been created manually or is part of
-another deployment.
+When we define a Deployment in a configure script and use fbnconfig to create the corresponding
+LUSID environment, all the underlying Resources are fully managed by fbnconfig. This means we want
+to use fbnconfig to manage all related Resources within a single Deployment.
+
+However, if we need to establish a relationship between existing Resources and our configure script,
+we can use a `Ref`. In the following example, we account for the `downloads` folder which already
+exists because it has been created manually or is part of another Deployment.
 
-```
+```Python
 def configure(env):
     f1 = drive.FolderRef(id="downloads", name="downloads")
     f2 = drive.FolderResource(id="sub_folder", name="my_subfolder", parent=f1)
     return Deployment("my_deployment", [f1, f2])
 ```
 
-will create `sub_folder` within `downloads`. The downloads folder will be the parent, but it won't
-be managed within this deployment. If it doesn't exist at the time this is run, then it will error.
-If `f1` is removed, it won't get deleted because it is not being managed in this deployment.
+* This code will create `sub_folder` within the existing `downloads` Resource. We tell fbnconfig
+  that `downloads` already exists by using the `drive.FolderRef()` function instead of
+  `drive.FolderResource()`.
+* If `downloads` doesn't exist at the time this is run, we get an error.
+* The `downloads` folder will be the parent of `sub_folder`, but it won't be managed within this
+  Deployment.
+* If `f1` is removed, it won't get deleted because it is not being managed in this deployment.
 
 ## The vars file
 
-To aid with using the same script for dev, uat and prod, `fbnconfig` takes a commandline argument to
-a json file called the "vars file". The vars file is parsed and passed into the configure function
-(called `env` in the examples above).
+To aid with using the same script for dev, uat, and prod, fbnconfig takes a commandline argument to
+a json file called the "vars file". The vars file (called `env` in the examples above) is
+parsed and passed into the configure function.
 
-Say we wanted to use different email for dev and prod (like the environment variable example above):
+For example, suppose we wanted to use different email for dev and prod (like the environment
+variable example above).
 
-We would create two vars files
+We would:
 
-```
+1. Create two vars files.
+
+```json
 // prod.json                                    // dev.json
 {                                               {
     "email": "prod@company.com"                     "email": "dev@company.com"
 }                                               }
 ```
 
-reference them from the script var env:
-
-```
-def configure(env):
-    export_user = identity.UserResource(
-        id="user2",
-        ...
-        emailAddress=env.email,
-    )
-```
-
-Then running:
-
-```
-fbnconfig -e https://dev.lusid.com -v dev.json script.py
-```
+1. Reference the files from the script var env.
 
-Will use the `dev@company.com` email.
+    ```Python
+    def configure(env):
+        export_user = identity.UserResource(
+            id="user2",
+            ...
+            emailAddress=env.email,
+        )
+    ```
+
+1. Run the following command to use the `dev@company.com` email..
+
+    ```cli
+    fbnconfig -e https://dev.lusid.com -v dev.json script.py
+    ```
 
 These vars files can be comitted to the repo to capture variations between environments. For
-secrets, it's better to use explicit environment variables in the script (see below)
+secrets, it's better to use explicit environment variables in the script (see below).
 
-## Using python in the script
+## Using Python in the script
 
-A deployment script is normal python so python language features are available. Variables,
-f-strings, os.environ can all be used within the script:
+A deployment script is normal Python, so Python language features are available. For example
+variables and f-strings. To allow values to depend on the environment, you can use `os.environ` to
+initialise the variables. This is useful when setting up secrets in the config store.
 
-To allow values to depend on the environment use `os.environ` to initialise the variables:
+For example, the following code:
 
-```
+1. Passes the secret as an environment variable.
+2. Makes an http request or use a library from a vault provider to source the
+secret.
+3. Uses the secret inside the configure function.
+
+```Python
 import os
 
 company = os.environ["company"]
 
 def configure(env):
     export_user = identity.UserResource(
         id="user2",
         ...
         emailAddress=f"exports@{company}",
         login=f"exports@{company}",
     )
 ```
 
-This is useful when setting up secrets in the config store. Pass the secret as an
-environment variable, make a http request or use a library from a vault provider to source the
-secret then use it inside the configure function.
-
-You can even create resources in a loop:
+You can even create resources in a loop, for example:
 
-```
+```Python
 def configure(env):
     folders = [
         drive.FolderResource(id=f"folder_{i}", name="i", parent=drive.root)
         for i in range(0, 10)
     ]
     return Deployment('ten-folders', folders)
 ```
 
-The python variables for the resources need to be added to the deployment
-and each resource must have a unique `id`.
+The Python variables for the Resources need to be added to the deployment and each Resource must
+have a unique `id`.
 
 ## Using fbnconfig as a library
 
-Using fbnconfig from the commandline dyamically loads your python script and executes the
-deployment. In some cases (eg using fbnconfig as part of another application) you can call it from
-python as well.
+Using fbnconfig from the commandline dyamically loads your Python script and executes the
+Deployment. In some cases (for example using fbnconfig as part of another application) you can call
+it from Python as well.
+
+The following example creates an empty deployment called "my-jobs":
+
+```Python
+from os import environ
+from fbnconfig import Deployment, deploy
 
-This creates an empty deployment called "my-jobs":
-
-```
-import fbnconfig
-import os
 
 def configure(env):
     return Deployment("my-jobs", [])
 
 
 host_vars = {}
 lusid_url = "https://foo.lusid.com"
-token = os.environ["MY_TOKEN_VAR"])
+token = environ["MY_TOKEN_VAR"]
 deployment = configure(host_vars)
-fbnconfig.deploy(deployment, lusid_url, token)
+deploy(deployment, lusid_url, token)
 ```
 
-
-
```

