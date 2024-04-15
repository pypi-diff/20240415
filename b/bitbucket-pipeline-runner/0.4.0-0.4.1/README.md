# Comparing `tmp/bitbucket_pipeline_runner-0.4.0.tar.gz` & `tmp/bitbucket_pipeline_runner-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_pipeline_runner-0.4.0.tar", max compression
+gzip compressed data, was "bitbucket_pipeline_runner-0.4.1.tar", max compression
```

## Comparing `bitbucket_pipeline_runner-0.4.0.tar` & `bitbucket_pipeline_runner-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/LICENSE
--rw-r--r--   0        0        0     1046 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/README.md
--rw-r--r--   0        0        0       29 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/__init__.py
--rw-r--r--   0        0        0       61 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/__main__.py
--rw-r--r--   0        0        0     3057 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/artifacts.py
--rw-r--r--   0        0        0    10673 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/cache.py
--rw-r--r--   0        0        0     5267 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/cli.py
--rw-r--r--   0        0        0     3227 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/config.py
--rw-r--r--   0        0        0    17004 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/container.py
--rw-r--r--   0        0        0     5831 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/context.py
--rw-r--r--   0        0        0      608 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/errors.py
--rw-r--r--   0        0        0    14158 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/models.py
--rw-r--r--   0        0        0      357 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/parse.py
--rw-r--r--   0        0        0        0 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/py.typed
--rw-r--r--   0        0        0     4193 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/repository.py
--rw-r--r--   0        0        0    15676 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/runner.py
--rw-r--r--   0        0        0     9283 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/service.py
--rw-r--r--   0        0        0        0 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/static/__init__.py
--rw-r--r--   0        0        0     1665 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/static/known_hosts
--rwxr-xr-x   0        0        0      451 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/static/runit.sh
--rw-r--r--   0        0        0     4331 2024-03-26 19:14:53.286164 bitbucket_pipeline_runner-0.4.0/pipeline_runner/utils.py
--rw-r--r--   0        0        0     2844 2024-03-26 19:14:53.290165 bitbucket_pipeline_runner-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-15 21:35:07.074115 bitbucket_pipeline_runner-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1046 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/README.md
+-rw-r--r--   0        0        0       29 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/__main__.py
+-rw-r--r--   0        0        0     3057 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/artifacts.py
+-rw-r--r--   0        0        0    10673 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/cache.py
+-rw-r--r--   0        0        0     5267 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/cli.py
+-rw-r--r--   0        0        0     3227 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/config.py
+-rw-r--r--   0        0        0    17315 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/container.py
+-rw-r--r--   0        0        0     5831 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/context.py
+-rw-r--r--   0        0        0      608 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/errors.py
+-rw-r--r--   0        0        0    14998 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/models.py
+-rw-r--r--   0        0        0      357 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/parse.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/py.typed
+-rw-r--r--   0        0        0     4193 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/repository.py
+-rw-r--r--   0        0        0    15676 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/runner.py
+-rw-r--r--   0        0        0     9283 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/service.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/known_hosts
+-rwxr-xr-x   0        0        0      451 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/runit.sh
+-rw-r--r--   0        0        0     4331 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/utils.py
+-rw-r--r--   0        0        0     2844 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.1/PKG-INFO
```

### Comparing `bitbucket_pipeline_runner-0.4.0/LICENSE` & `bitbucket_pipeline_runner-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/README.md` & `bitbucket_pipeline_runner-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/artifacts.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/artifacts.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/cache.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/cache.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/cli.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/cli.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/config.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/config.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/container.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,21 +212,25 @@
             raise Exception(f"Error creating root ssh config: {output}")
 
     def _insert_ssh_known_hosts(self) -> None:
         if not self._ssh_private_key:
             return
 
         private_key_file_path = os.path.join(config.ssh_key_dir, "id_rsa")
+        known_hosts_file_path = os.path.join(config.ssh_key_dir, "known_hosts")
 
         cmd = " && ".join(
             [
                 "install -d -m 700 ~/.ssh",
                 f'echo "IdentityFile {private_key_file_path}\nServerAliveInterval 180" > ~/.ssh/config',
                 f"install -m 600 /dev/null {private_key_file_path}",
                 f'echo "{self._ssh_private_key}" > {private_key_file_path}',
+                # The default ssh key with open perms readable by alt uids
+                f"install -m 644 {private_key_file_path} {private_key_file_path}_tmp",
+                f"install -m 644 /dev/null {known_hosts_file_path}",
             ]
         )
         exit_code, output = self.run_command(cmd, user=0)
         if exit_code != 0:
             raise Exception(f"Error creating root ssh config: {output}")
 
     def _get_volumes(self) -> dict[str, dict[str, str]]:
```

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/context.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/context.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/errors.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/errors.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/models.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,22 +193,47 @@
 
     def as_int(self) -> int:
         return {self.Simple: 1, self.Double: 2}[self]
 
 
 class Pipe(BaseModel):
     pipe: str
-    variables: dict[str, str] = Field(default_factory=dict)
+    variables: dict[str, str | list[str]] = Field(default_factory=dict)
 
     def as_cmd(self) -> str:
-        cmd = "docker run --rm"
-        if self.variables:
-            cmd += " " + " ".join(f'-e {k}="{self._escape_value(v)}"' for k, v in self.variables.items())
+        cmd = [
+            "docker",
+            "run",
+            "--rm",
+            "--volume=/opt/atlassian/pipelines/agent/build:/opt/atlassian/pipelines/agent/build",
+            "--volume=/opt/atlassian/pipelines/agent/ssh:/opt/atlassian/pipelines/agent/ssh:ro",
+            "--volume=/opt/atlassian/pipelines/bin/docker:/usr/local/bin/docker:ro",
+        ]
+
+        variables = self.expand_variables()
+        if variables:
+            cmd += [f'-e {k}="{self._escape_value(v)}"' for k, v in variables.items()]
+
+        cmd.append(self.get_image())
+
+        return " ".join(cmd)
+
+    def expand_variables(self) -> dict[str, str]:
+        expanded_variables = {}
+
+        for key, value in self.variables.items():
+            if isinstance(value, list):
+                for i, v in enumerate(value):
+                    expanded_variables[f"{key}_{i}"] = v
+
+                expanded_variables[f"{key}_COUNT"] = str(len(value))
+            else:
+                expanded_variables[key] = value
 
-        return f"{cmd} {self.get_image()}"
+        return expanded_variables
 
     @staticmethod
     def _escape_value(v: str) -> str:
         return v.replace('"', '\\"')
 
     def get_image(self) -> str:
         if self.pipe.startswith("atlassian/"):
```

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/repository.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/repository.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/runner.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/runner.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/service.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/service.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/static/known_hosts` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/known_hosts`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pipeline_runner/utils.py` & `bitbucket_pipeline_runner-0.4.1/pipeline_runner/utils.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.0/pyproject.toml` & `bitbucket_pipeline_runner-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bitbucket-pipeline-runner"
-version = "0.4.0"
+version = "0.4.1"
 description = "Run a bitbucket pipeline locally"
 authors = ["Mathieu Lemay <acidrain1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mathieu-lemay/pipeline-runner"
 packages = [
     {include = "pipeline_runner"}
```

### Comparing `bitbucket_pipeline_runner-0.4.0/PKG-INFO` & `bitbucket_pipeline_runner-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipeline-runner
-Version: 0.4.0
+Version: 0.4.1
 Summary: Run a bitbucket pipeline locally
 Home-page: https://github.com/mathieu-lemay/pipeline-runner
 License: MIT
 Author: Mathieu Lemay
 Author-email: acidrain1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

