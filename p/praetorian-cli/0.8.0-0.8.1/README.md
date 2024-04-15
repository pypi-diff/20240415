# Comparing `tmp/praetorian_cli-0.8.tar.gz` & `tmp/praetorian_cli-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praetorian_cli-0.8.tar", last modified: Fri Apr 12 20:26:35 2024, max compression
+gzip compressed data, was "praetorian_cli-0.8.1.tar", last modified: Mon Apr 15 19:12:40 2024, max compression
```

## Comparing `praetorian_cli-0.8.tar` & `praetorian_cli-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.256895 praetorian_cli-0.8/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-12 20:26:35.256725 praetorian_cli-0.8/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian_cli-0.8/README.md
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.246191 praetorian_cli-0.8/praetorian_cli/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian_cli-0.8/praetorian_cli/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)      674 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/cli.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.249585 praetorian_cli-0.8/praetorian_cli/handlers/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian_cli-0.8/praetorian_cli/handlers/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2843 2024-04-12 20:26:25.000000 praetorian_cli-0.8/praetorian_cli/handlers/account.py
--rw-r--r--   0 privateducky   (501) staff       (20)     5002 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/handlers/backend.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1186 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/handlers/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.250637 praetorian_cli-0.8/praetorian_cli/sdk/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian_cli-0.8/praetorian_cli/sdk/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3125 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/sdk/chaos.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian_cli-0.8/praetorian_cli/sdk/keychain.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.255509 praetorian_cli-0.8/praetorian_cli/sdk/test/
--rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_file_upload.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2484 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_job_capabilities.py
--rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_link_account.py
--rw-r--r--   0 privateducky   (501) staff       (20)      741 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_manual_risk.py
--rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_nvd.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1831 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_seed.py
--rw-r--r--   0 privateducky   (501) staff       (20)      988 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.256394 praetorian_cli-0.8/praetorian_cli.egg-info/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/SOURCES.txt
--rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/dependency_links.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/entry_points.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/requires.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/top_level.txt
--rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian_cli-0.8/pyproject.toml
--rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-12 20:26:35.257398 praetorian_cli-0.8/setup.cfg
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.745303 praetorian_cli-0.8.1/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-15 19:12:40.745166 praetorian_cli-0.8.1/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/README.md
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.722090 praetorian_cli-0.8.1/praetorian_cli/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian_cli-0.8.1/praetorian_cli/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      674 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/cli.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.734631 praetorian_cli-0.8.1/praetorian_cli/handlers/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2833 2024-04-13 14:46:54.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     5145 2024-04-15 11:06:17.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/backend.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1186 2024-04-11 14:42:01.000000 praetorian_cli-0.8.1/praetorian_cli/handlers/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.735740 praetorian_cli-0.8.1/praetorian_cli/sdk/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3424 2024-04-14 13:45:08.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/chaos.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/keychain.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.744310 praetorian_cli-0.8.1/praetorian_cli/sdk/test/
+-rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_file_upload.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2539 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_job_capabilities.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-10 11:11:30.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_link_account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      757 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_manual_risk.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-08 21:35:19.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_nvd.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1848 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_seed.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      909 2024-04-15 14:23:33.000000 praetorian_cli-0.8.1/praetorian_cli/sdk/test/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-15 19:12:40.744859 praetorian_cli-0.8.1/praetorian_cli.egg-info/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/entry_points.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/requires.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-15 19:12:40.000000 praetorian_cli-0.8.1/praetorian_cli.egg-info/top_level.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian_cli-0.8.1/pyproject.toml
+-rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-15 19:12:40.746073 praetorian_cli-0.8.1/setup.cfg
```

### Comparing `praetorian_cli-0.8/PKG-INFO` & `praetorian_cli-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `praetorian_cli-0.8/README.md` & `praetorian_cli-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/cli.py` & `praetorian_cli-0.8.1/praetorian_cli/cli.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/handlers/account.py` & `praetorian_cli-0.8.1/praetorian_cli/handlers/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 def my_accounts(controller):
     """ Fetch my associated accounts """
     result = controller.my(dict(key=f'#account'))
     for hit in result.get('accounts', []):
         print(f"{hit['key']}")
 
 
-@chaos.command('link-account')
+@chaos.command('link-chaos')
 @click.pass_obj
 @handle_api_error
 @click.argument('username')
 @click.option('-config', '--config', default="", help="Add an optional configuration")
 def link_account(controller, username, config):
     """ Link another Chaos account to yours """
     result = controller.link_account(username=username, config=config)
     print(f"{result['key']}")
 
 
-@chaos.command('unlink-account')
+@chaos.command('unlink')
 @click.pass_obj
 @handle_api_error
 @click.argument('username')
 def unlink_account(controller, username):
     """ Unlink a Chaos account from yours """
     result = controller.unlink_account(username=username)
     print(f"{result['key']}")
```

### Comparing `praetorian_cli-0.8/praetorian_cli/handlers/backend.py` & `praetorian_cli-0.8.1/praetorian_cli/handlers/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,38 +11,37 @@
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_seeds(controller, seed):
     """ Fetch seed domains """
     result = controller.my(dict(key=f'#seed#{seed}'))
     for hit in result.get('seeds', []):
         print(f"{hit['key']}")
-        print(hit)
 
 
 @chaos.command('assets')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_assets(controller, seed):
     """ Fetch existing assets """
     result = controller.my(dict(key=f'#asset#{seed}'))
     for hit in result.get('assets', []):
         print(f"{hit['key']}")
-        print(hit)
+
 
 @chaos.command('risks')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_risks(controller, seed):
     """ Fetch current risks """
     result = controller.my(dict(key=f'#risk#{seed}'))
     for hit in result.get('risks', []):
         print(f"{hit['key']}")
-        print(hit)
+
 
 @chaos.command('services')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_services(controller, seed):
     """ Fetch recently seen services """
@@ -91,14 +90,23 @@
 @click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
 @click.option('-comment', '--comment', default="", help="Add a comment")
 def add_seed(controller, seed, status, comment=""):
     """ Add a new seed domain """
     controller.add_asset(seed, status=status, comment=comment)
 
 
+@chaos.command('delete-seed')
+@click.pass_obj
+@handle_api_error
+@click.argument('seed')
+def delete_seed(controller, seed):
+    """ Delete any seed """
+    controller.delete_asset(f'#seed#{seed}')
+
+
 @chaos.command('update-asset')
 @click.pass_obj
 @handle_api_error
 @click.argument('key')
 @click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
 @click.option('-comment', '--comment', help="Add a comment")
 def update_asset(controller, key, status, comment=''):
```

### Comparing `praetorian_cli-0.8/praetorian_cli/handlers/utils.py` & `praetorian_cli-0.8.1/praetorian_cli/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/chaos.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/chaos.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 
         resp = requests.put(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
+    def delete_asset(self, key: str) -> {}:
+        resp = requests.delete(f"{self.keychain.api}/asset", json={'key': key}, headers=self.keychain.headers)
+        if not resp.ok:
+            raise Exception(f'[{resp.status_code}] Request failed')
+        return resp.json()
+
+    @verify_credentials
     def link_account(self, username: str, config: str):
         resp = requests.post(f"{self.keychain.api}/account/{username}", json={'config':config}, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
```

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/keychain.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/keychain.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_file_upload.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_job_capabilities.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_job_capabilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,9 +45,10 @@
         assert response.get('risks'), "Received empty response for my risks"
 
         for my_risk in response.get('risks', []):
             assert my_risk['username'] == self.username, f"Job did not have username = {self.username}"
             assert self.seed in my_risk['key'], "Service key does not have seed"
 
     def test_delete_seed(self):
-        response = self.utils.freeze_seed(self.seed)
-        assert response['seed'] == self.seed
+        self.chaos.delete_asset(key=f'#seed#{self.seed}')
+        response = self.chaos.my(dict(key=f'#seed#{self.seed}'))
+        assert response == {}
```

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_link_account.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_link_account.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_manual_risk.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_manual_risk.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,8 +14,8 @@
         self.utils.add_seed(self.seed)
         response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'))
         assert response, "Received empty response for my Assets"
 
         self.chaos.add_risk(key=f'#asset#{self.seed}', name=self.name)
         my_risk = self.chaos.my(dict(key=f'#risk#{self.seed}'))
         assert my_risk is not None
-        self.utils.freeze_seed(self.seed)
+        self.chaos.delete_asset(key=f'#seed#{self.seed}')
```

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_nvd.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_nvd.py`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/test_seed.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/test_seed.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,33 +15,33 @@
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
         self.utils = Utils(self.chaos)
 
     def test_add_seed(self):
         response = self.utils.add_seed(self.seed)
         assert response['seed'] == self.seed, "Response does not have correct seed"
-        assert response['status'] is 0
+        assert response['status'] == "AA"
 
     def test_my_seed(self):
         response = self.chaos.my(dict(key=f'#seed#{self.seed}'))
         for my_seed in response['seeds']:
             assert my_seed['username'] == self.username, f"Seed did not have username = {self.username}"
             assert my_seed['seed'] in self.seed
 
     def test_my_job(self):
-        response = self.utils.wait_for_key(dict(key=f'#job#{threshold()}'))
+        response = self.utils.wait_for_key(dict(key=f'#job#{self.seed}'))
         assert response is not None, "Received empty response for my Jobs"
         for job in response['jobs']:
             assert job['source'] is not '', "Job Capability is empty"
             assert job['status'] is not None, "Job Status is empty"
 
     def test_my_asset(self):
         response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'))
         assert response is not None, "Received empty response for my Assets"
         for asset in response['assets']:
             assert asset['seed'] == self.seed, "Seed is empty"
             assert asset['name'] or asset['dns'], "Asset fields IP and DNS are both empty"
 
     def test_delete_seed(self):
-        response = self.utils.freeze_seed(self.seed)
-        assert response['seed'] == self.seed
-        assert response['status'] is 1
+        self.chaos.delete_asset(key=f'#seed#{self.seed}')
+        response = self.chaos.my(dict(key=f'#seed#{self.seed}'))
+        assert response == {}
```

### Comparing `praetorian_cli-0.8/praetorian_cli/sdk/test/utils.py` & `praetorian_cli-0.8.1/praetorian_cli/sdk/test/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,11 +24,9 @@
             print(f"Trying to get response for my {key}")
             response = self.chaos.my(key)
             if response:
                 return response
             time.sleep(interval)
 
     def add_seed(self, seed):
-        return self.chaos.upsert_seed(seed, 0)
+        return self.chaos.add_asset(seed, "AA")
 
-    def freeze_seed(self, seed):
-        return self.chaos.upsert_seed(seed, 1)
```

### Comparing `praetorian_cli-0.8/praetorian_cli.egg-info/PKG-INFO` & `praetorian_cli-0.8.1/praetorian_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.8.0
+Version: 0.8.1
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `praetorian_cli-0.8/praetorian_cli.egg-info/SOURCES.txt` & `praetorian_cli-0.8.1/praetorian_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `praetorian_cli-0.8/setup.cfg` & `praetorian_cli-0.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = praetorian-cli
-version = 0.8.0
+version = 0.8.1
 author = Praetorian Labs
 author_email = research@praetorian.com
 description = For interacting with the Chaos API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/praetorian-inc/praetorian-cli
 classifiers =
```

