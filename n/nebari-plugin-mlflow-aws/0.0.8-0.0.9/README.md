# Comparing `tmp/nebari_plugin_mlflow_aws-0.0.8.tar.gz` & `tmp/nebari_plugin_mlflow_aws-0.0.9.tar.gz`

## Comparing `nebari_plugin_mlflow_aws-0.0.8.tar` & `nebari_plugin_mlflow_aws-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/.github/workflows/publish-docker-image.yaml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/docker/Dockerfile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/__about__.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/__init__.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/outputs.tf
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/variables.tf
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/versions.tf
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/main.tf
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/outputs.tf
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/variables.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/versions.tf
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/outputs.tf
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/.helmignore
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/Chart.yaml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/values.yaml
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/deployment.yaml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/hpa.yaml
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/ingress.yaml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/postgres.yaml
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/service.yaml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/traefik.yaml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/tests/integration/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/tests/unit/__init__.py
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/tests/unit/test_plugin.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/.gitignore
--rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/README.md
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/.github/workflows/publish-docker-image.yaml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/docker/.dockerignore
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/docker/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/__about__.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/__init__.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/outputs.tf
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/variables.tf
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/versions.tf
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/main.tf
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/outputs.tf
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/variables.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/versions.tf
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/outputs.tf
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/.helmignore
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/Chart.yaml
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/values.yaml
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/deployment.yaml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/hpa.yaml
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/postgres.yaml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/service.yaml
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/traefik.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/tests/unit/test_plugin.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/.gitignore
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/README.md
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 nebari_plugin_mlflow_aws-0.0.9/PKG-INFO
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/.github/workflows/publish-pypi.yaml` & `nebari_plugin_mlflow_aws-0.0.9/.github/workflows/publish-pypi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 name: build and publish
+
 'on':
   workflow_dispatch: {}
   push:
     branches:
     - main
+
 jobs:
   pypi-publish:
     name: Upload release to PyPI
+
     runs-on: ubuntu-latest
+
     environment:
       name: pypi
       url: https://pypi.org/p/nebari-plugin-mlflow-aws
+
     permissions:
       id-token: write
+
     steps:
     - name: Checkout Image
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
+
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.10'
+
     - name: Install Hatch
       run: pip install hatch
+
     - name: Build
       run: hatch build
+
     - name: Publish package distributions to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/__init__.py` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 from typing import Any, Dict, List, Optional
 
 NUM_ATTEMPTS = 10
 TIMEOUT = 10
 
 CLIENT_NAME = "mlflow"
 
-#TODO this only works for AWS.  How to check
+# TODO this only works for AWS.  How to check
+
 
 class MlflowConfig(Base):
     name: Optional[str] = "mlflow"
     namespace: Optional[str] = None
     values: Optional[Dict[str, Any]] = {}
 
+
 class InputSchema(Base):
     mlflow: MlflowConfig = MlflowConfig()
 
+
 class MlflowStage(NebariTerraformStage):
     name = "mlflow"
     priority = 102
-    wait = True # wait for install to complete on nebari deploy
+    wait = True  # wait for install to complete on nebari deploy
     input_schema = InputSchema
 
     @property
     def template_directory(self):
         return Path(inspect.getfile(self.__class__)).parent / "terraform"
-    
+
     def _attempt_keycloak_connection(
         self,
         keycloak_url,
         username,
         password,
         master_realm_name,
         client_id,
@@ -54,134 +57,140 @@
                     keycloak_url,
                     username=username,
                     password=password,
                     realm_name=master_realm_name,
                     client_id=client_id,
                     verify=verify,
                 )
-                realm_admin.realm_name = client_realm_name # switch to nebari realm
-                c = realm_admin.get_client_id(CLIENT_NAME) # lookup client guid
-                existing_client = realm_admin.get_client(c) # query client info
+                realm_admin.realm_name = client_realm_name  # switch to nebari realm
+                c = realm_admin.get_client_id(CLIENT_NAME)  # lookup client guid
+                existing_client = realm_admin.get_client(c)  # query client info
                 if existing_client != None and existing_client["name"] == CLIENT_NAME:
-                    print(
-                        f"Attempt {i+1} succeeded connecting to keycloak and nebari client={CLIENT_NAME} exists"
-                    )
+                    print(f"Attempt {i+1} succeeded connecting to keycloak and nebari client={CLIENT_NAME} exists")
                     return True
                 else:
                     print(
                         f"Attempt {i+1} succeeded connecting to keycloak but nebari client={CLIENT_NAME} did not exist"
                     )
             except KeycloakError as e:
                 print(f"Attempt {i+1} failed connecting to keycloak {client_realm_name} realm -- {e}")
             time.sleep(timeout)
         return False
-    
+
     def check(self, stage_outputs: Dict[str, Dict[str, Any]], disable_prompt=False) -> bool:
-                
         # TODO: Module requires EKS cluster is configured for IRSA.  Once Nebari version with IRSA is released, should update
         # this error message and also minimum Nebari version in pyproject.toml
         try:
             _ = stage_outputs["stages/02-infrastructure"]["cluster_oidc_issuer_url"]["value"]
-            
+
         except KeyError:
             print(
                 "\nPrerequisite stage output(s) not found in stages/02-infrastructure: cluster_oidc_issuer_url.  Please ensure Nebari version is at least XX."
             )
             return False
-        
+
         try:
             _ = self.config.escaped_project_name
             _ = self.config.provider
-            
+
         except KeyError:
-            print(
-                "\nBase config values not found: escaped_project_name, provider"
-            )
+            print("\nBase config values not found: escaped_project_name, provider")
             return False
-        
-        if not self.config.provider == ProviderEnum.aws:
-            raise KeyError("Plugin nebari_plugin_mlflow_aws developed for aws only.  Detected provider is {}.".format(self.config.provider))
 
+        if not self.config.provider == ProviderEnum.aws:
+            raise KeyError(
+                "Plugin nebari_plugin_mlflow_aws developed for aws only.  Detected provider is {}.".format(
+                    self.config.provider
+                )
+            )
 
         keycloak_config = self.get_keycloak_config(stage_outputs)
 
         if not self._attempt_keycloak_connection(
-            keycloak_url = keycloak_config["keycloak_url"],
-            username = keycloak_config["username"],
-            password = keycloak_config["password"],
-            master_realm_name = keycloak_config["master_realm_id"],
-            client_id = keycloak_config["master_client_id"],
-            client_realm_name = keycloak_config["realm_id"],
+            keycloak_url=keycloak_config["keycloak_url"],
+            username=keycloak_config["username"],
+            password=keycloak_config["password"],
+            master_realm_name=keycloak_config["master_realm_id"],
+            client_id=keycloak_config["master_client_id"],
+            client_realm_name=keycloak_config["realm_id"],
             verify=False,
         ):
             print(
                 f"ERROR: unable to connect to keycloak master realm and ensure that nebari client={CLIENT_NAME} exists"
             )
             sys.exit(1)
 
         print(f"Keycloak successfully configured with {CLIENT_NAME} client")
         return True
 
     def input_vars(self, stage_outputs: Dict[str, Dict[str, Any]]):
         keycloak_config = self.get_keycloak_config(stage_outputs)
 
         if not self.config.provider == ProviderEnum.aws:
-            raise KeyError("Plugin nebari_plugin_mlflow_aws developed for aws only.  Detected provider is {}.".format(self.config.provider))
+            raise KeyError(
+                "Plugin nebari_plugin_mlflow_aws developed for aws only.  Detected provider is {}.".format(
+                    self.config.provider
+                )
+            )
 
         # TODO: Module requires EKS cluster is configured for IRSA.  Once Nebari version with IRSA is released, should update
         # this error message and also minimum Nebari version in pyproject.toml
         try:
             _ = stage_outputs["stages/02-infrastructure"]["cluster_oidc_issuer_url"]["value"]
-            
+
         except KeyError:
-            raise Exception("Prerequisite stage output(s) not found in stages/02-infrastructure: cluster_oidc_issuer_url.  Please ensure Nebari version is at least XX.")
-                    
+            raise Exception(
+                "Prerequisite stage output(s) not found in stages/02-infrastructure: cluster_oidc_issuer_url.  Please ensure Nebari version is at least XX."
+            )
+
         try:
             domain = stage_outputs["stages/04-kubernetes-ingress"]["domain"]
             cluster_oidc_issuer_url = stage_outputs["stages/02-infrastructure"]["cluster_oidc_issuer_url"]["value"]
-            
+
         except KeyError:
-            raise Exception("Prerequisite stage output(s) not found: stages/02-infrastructure, stages/04-kubernetes-ingress")
+            raise Exception(
+                "Prerequisite stage output(s) not found: stages/02-infrastructure, stages/04-kubernetes-ingress"
+            )
 
         chart_ns = self.config.mlflow.namespace
         create_ns = True
         if chart_ns == None or chart_ns == "" or chart_ns == self.config.namespace:
             chart_ns = self.config.namespace
             create_ns = False
 
         return {
             "chart_name": self.config.mlflow.name,
             "project_name": self.config.escaped_project_name,
             "realm_id": keycloak_config["realm_id"],
             "client_id": CLIENT_NAME,
-                        "base_url": f"https://{keycloak_config['domain']}/mlflow",
+            "base_url": f"https://{keycloak_config['domain']}/mlflow",
             "external_url": keycloak_config["keycloak_url"],
             "valid_redirect_uris": [f"https://{keycloak_config['domain']}/mlflow/_oauth"],
             "signing_key_ref": {
                 "name": "forwardauth-deployment",
                 "kind": "Deployment",
                 "namespace": self.config.namespace,
-                },
+            },
             "create_namespace": create_ns,
             "namespace": chart_ns,
             "ingress_host": domain,
             "cluster_oidc_issuer_url": cluster_oidc_issuer_url,
-            "overrides": self.config.mlflow.values
-
+            "overrides": self.config.mlflow.values,
         }
 
     def get_keycloak_config(self, stage_outputs: Dict[str, Dict[str, Any]]):
         directory = "stages/05-kubernetes-keycloak"
 
         return {
             "domain": stage_outputs["stages/04-kubernetes-ingress"]["domain"],
             "keycloak_url": f"{stage_outputs[directory]['keycloak_credentials']['value']['url']}/auth/",
             "username": stage_outputs[directory]["keycloak_credentials"]["value"]["username"],
             "password": stage_outputs[directory]["keycloak_credentials"]["value"]["password"],
             "master_realm_id": stage_outputs[directory]["keycloak_credentials"]["value"]["realm"],
             "master_client_id": stage_outputs[directory]["keycloak_credentials"]["value"]["client_id"],
             "realm_id": stage_outputs["stages/06-kubernetes-keycloak-configuration"]["realm_id"]["value"],
         }
-    
+
+
 @hookimpl
 def nebari_stage() -> List[NebariStage]:
-    return [ MlflowStage ]
+    return [MlflowStage]
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/main.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/variables.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/main.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/outputs.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/variables.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/keycloak/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/main.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/main.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/variables.tf` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/Chart.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/Chart.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # a dependency of application charts to inject those utilities and functions into the rendering
 # pipeline. Library charts do not define any templates and therefore cannot be deployed.
 type: application
 
 # This is the chart version. This version number should be incremented each time you make changes
 # to the chart and its templates, including the app version.
 # Versions are expected to follow Semantic Versioning (https://semver.org/)
-version: 1.1.1
+version: 1.2.0
 
 # This is the version number of the application being deployed. This version number should be
 # incremented each time you make changes to the application. Versions are not expected to
 # follow Semantic Versioning. They should reflect the version the application is using.
 # It is recommended to use it with quotes.
-appVersion: "2.4.1"
+appVersion: "2.9.2"
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/values.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/values.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 replicaCount: 1
 
 image:
   repository: ghcr.io/metrostar/nebari-mlflow-aws
   pullPolicy: IfNotPresent
   # Overrides the image tag whose default is the chart appVersion.
-  tag: "20231211-2144"
+  tag: "2.9.2-20231229-1941"
 
 imagePullSecrets: []
 nameOverride: ""
 fullnameOverride: ""
 
 serviceAccount:
   # Specifies whether a service account should be created
@@ -75,15 +75,23 @@
   targetCPUUtilizationPercentage: 80
   # targetMemoryUtilizationPercentage: 80
 
 nodeSelector: {}
 
 tolerations: []
 
-affinity: {}
+affinity:
+  nodeAffinity:
+    requiredDuringSchedulingIgnoredDuringExecution:
+      nodeSelectorTerms:
+      - matchExpressions:
+        - key: eks.amazonaws.com/nodegroup
+          operator: In
+          values:
+          - general
 
 args: []
 
 env: []
 
 envFrom: []
 
@@ -98,31 +106,27 @@
 timeout: 300
 
 storage:
   artifacts:
     artifactsDestination: ""
     defaultArtifactRoot: ""
     proxyArtifacts: false
-#    minio:
-#      bucketName: mlflow
-#      namespace: minio
-#      service:
-#        name: minio
-#        port: 9000
-#      existingSecret:
-#        name: minio-root-credentials
   db:
     enabled: true
+    existingSecret: ""
     selfHosted: true
+    autoUpgrade: false
     image:
       name: postgres
       tag: 11
     resources:
       requests:
         memory: "200Mi"
         cpu: "500m"
     volume:
       size: 100Mi
       accessMode: ReadWriteOnce
+    server: ""
+    port: 5432
     dbName: "mlflow_db"
     username: "mlflow_user"
     password: ""
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/NOTES.txt` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/_helpers.tpl` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/deployment.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/deployment.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,40 @@
       {{- with .Values.imagePullSecrets }}
       imagePullSecrets:
         {{- toYaml . | nindent 8 }}
       {{- end }}
       serviceAccountName: {{ include "mlflow.serviceAccountName" . }}
       securityContext:
         {{- toYaml .Values.podSecurityContext | nindent 8 }}
+      {{- if and .Values.storage.db.enabled .Values.storage.db.autoUpgrade }}
+      initContainers:
+        - name: db-upgrade
+          command:
+          - mlflow
+          args:
+          - db
+          - upgrade
+          - "postgresql://$(POSTGRES_USER):$(POSTGRES_PASSWORD)@$(POSTGRES_SERVER):$(POSTGRES_PORT)/$(POSTGRES_DB)"
+          {{- if .Values.env }}
+          env:
+          {{ toYaml .Values.env | nindent 10 }}
+          {{- end }}
+          envFrom:
+          {{- if .Values.storage.db.existingSecret }}
+          - secretRef:
+              name: {{ .Values.storage.db.existingSecret }}
+          {{- else }}
+          - secretRef:
+              name: {{ .Release.Name }}-postgres-env
+          {{- end }}
+          securityContext:
+            {{- toYaml .Values.securityContext | nindent 12 }}
+          image: "{{ .Values.image.repository }}:{{ .Values.image.tag | default .Chart.AppVersion }}"
+          imagePullPolicy: {{ .Values.image.pullPolicy }}
+      {{- end }}
       containers:
         - name: {{ .Chart.Name }}
           command:
           - mlflow
           args:
           - server
           - --host
@@ -41,15 +67,15 @@
           - --gunicorn-opts
           - "--log-level {{ .Values.logLevel }} --timeout {{ .Values.timeout }}"
           {{- if .Values.storage.backendStoreUri }}
           - --backend-store-uri
           - {{ .Values.storage.backendStoreUri }}
           {{- else if and .Values.storage.db.enabled .Values.storage.db.selfHosted }}
           - --backend-store-uri
-          - "postgresql://$(POSTGRES_USER):$(POSTGRES_PASSWORD)@{{ .Release.Name }}-postgres:5432/$(POSTGRES_DB)"
+          - "postgresql://$(POSTGRES_USER):$(POSTGRES_PASSWORD)@$(POSTGRES_SERVER):$(POSTGRES_PORT)/$(POSTGRES_DB)"
           {{- end }}
           {{- if .Values.storage.artifacts.artifactsDestination }}
           - --artifacts-destination
           - {{ .Values.storage.artifacts.artifactsDestination }}
           {{- else if .Values.storage.artifacts.minio }}
           - --artifacts-destination
           - "s3://{{ .Values.storage.artifacts.minio.bucketName }}"
@@ -71,27 +97,28 @@
           {{- range $a := .Values.args }}
           - {{ $a }}
           {{- end }}
           {{- if .Values.env }}
           env:
           {{ toYaml .Values.env | nindent 10 }}
           {{- end }}
-          {{- if and .Values.storage.db.enabled .Values.storage.db.selfHosted }}
-          - name: POSTGRES_USER
-            value: {{ .Values.db.username }}
-          - name: POSTGRES_PASSWORD
-            value: {{ .Values.db.password }}
-          - name: POSTGRES_DB
-            value: {{ .Values.db.dbName }}
-          {{- end }}
-          {{- if or .Values.envFrom .Values.storage.artifacts.minio  }}
+          {{- if or .Values.envFrom .Values.storage.artifacts.minio .Values.storage.db.enabled }}
           envFrom:
           {{- if .Values.storage.artifacts.minio }}
           - secretRef:
-              name: minio-env
+              name: {{ .Release.Name }}-minio-env
+          {{- end }}
+          {{- if .Values.storage.db.enabled }}
+          {{- if .Values.storage.db.existingSecret }}
+          - secretRef:
+              name: {{ .Values.storage.db.existingSecret }}
+          {{- else }}
+          - secretRef:
+              name: {{ .Release.Name }}-postgres-env
+          {{- end }}
           {{- end }}
           {{- if .Values.envFrom }}
           {{ toYaml .Values.envFrom | nindent 10 }}
           {{- end }}
           {{- end }}
           securityContext:
             {{- toYaml .Values.securityContext | nindent 12 }}
@@ -176,14 +203,26 @@
         - name: SECRET
           valueFrom:
             secretKeyRef:
               name: {{ .Release.Name }}-traefik-forward-auth
               key: signing_key
         - name: DEFAULT_PROVIDER
           value: "oidc"
+      {{- with .Values.nodeSelector }}
+      nodeSelector:
+        {{- toYaml . | nindent 8 }}
+      {{- end }}
+      {{- with .Values.affinity }}
+      affinity:
+        {{- toYaml . | nindent 8 }}
+      {{- end }}
+      {{- with .Values.tolerations }}
+      tolerations:
+        {{- toYaml . | nindent 8 }}
+      {{- end }}
 
 ---
 apiVersion: v1
 kind: Secret
 metadata:
   name: {{ .Release.Name }}-traefik-forward-auth
   namespace: {{ .Release.Namespace }}
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/hpa.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/ingress.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/service.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/traefik.yaml` & `nebari_plugin_mlflow_aws-0.0.9/src/nebari_plugin_mlflow_aws/terraform/modules/mlflow/chart/templates/traefik.yaml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/tests/unit/test_plugin.py` & `nebari_plugin_mlflow_aws-0.0.9/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/.gitignore` & `nebari_plugin_mlflow_aws-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/LICENSE.md` & `nebari_plugin_mlflow_aws-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/README.md` & `nebari_plugin_mlflow_aws-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Nebari Plugin MLflow AWS
 
-[![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-mlflow-chart.svg)](https://pypi.org/project/nebari-plugin-mlflow-chart)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-mlflow-chart.svg)](https://pypi.org/project/nebari-plugin-mlflow-chart)
+[![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-mlflow-aws.svg)](https://pypi.org/project/nebari-plugin-mlflow-aws)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-mlflow-aws.svg)](https://pypi.org/project/nebari-plugin-mlflow-aws)
 
 -----
 
 **Table of Contents**
 
 - [Features](#features)
 - [Installation](#installation)
```

### Comparing `nebari_plugin_mlflow_aws-0.0.8/pyproject.toml` & `nebari_plugin_mlflow_aws-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari_plugin_mlflow_aws-0.0.8/PKG-INFO` & `nebari_plugin_mlflow_aws-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari-plugin-mlflow-aws
-Version: 0.0.8
+Version: 0.0.9
 Summary: MetroStar - MLFlow Plugin for AWS Nebari Platform
 Project-URL: Documentation, https://github.com/MetroStar/nebari-mlflow-aws#readme
 Project-URL: Issues, https://github.com/MetroStar/nebari-mlflow-aws/issues
 Project-URL: Source, https://github.com/MetroStar/nebari-mlflow-aws
 Author-email: Scott Blair <sblair@metrostar.com>, Ken Foster <kfoster@metrostar.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: nebari
 Description-Content-Type: text/markdown
 
 # Nebari Plugin MLflow AWS
 
-[![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-mlflow-chart.svg)](https://pypi.org/project/nebari-plugin-mlflow-chart)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-mlflow-chart.svg)](https://pypi.org/project/nebari-plugin-mlflow-chart)
+[![PyPI - Version](https://img.shields.io/pypi/v/nebari-plugin-mlflow-aws.svg)](https://pypi.org/project/nebari-plugin-mlflow-aws)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nebari-plugin-mlflow-aws.svg)](https://pypi.org/project/nebari-plugin-mlflow-aws)
 
 -----
 
 **Table of Contents**
 
 - [Features](#features)
 - [Installation](#installation)
```

