# Comparing `tmp/ceotr_config-1.0.8.tar.gz` & `tmp/ceotr_config-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceotr_config-1.0.8.tar", last modified: Fri Apr  5 14:49:44 2024, max compression
+gzip compressed data, was "ceotr_config-1.0.9.tar", last modified: Mon Apr 15 02:45:43 2024, max compression
```

## Comparing `ceotr_config-1.0.8.tar` & `ceotr_config-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      336 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2326 2024-04-05 14:34:18.000000 ceotr_config-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.846637 ceotr_config-1.0.8/ceotr_config/
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10977 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/config_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/ceotr_config/template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/default_django_setting.yml-tpl
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/default_setting.yml-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/ceotr_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      336 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      568 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-05 14:47:42.000000 ceotr_config-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/test/ceotr_conifg_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/test/ceotr_conifg_test/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16730 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.245051 ceotr_config-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-15 02:45:43.245051 ceotr_config-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2024-04-08 15:33:34.000000 ceotr_config-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.243051 ceotr_config-1.0.9/ceotr_config/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-15 02:41:47.000000 ceotr_config-1.0.9/ceotr_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10977 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/ceotr_config/config_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.244051 ceotr_config-1.0.9/ceotr_config/template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/ceotr_config/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-15 02:41:47.000000 ceotr_config-1.0.9/ceotr_config/template/default_django_setting.yml-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-15 02:41:47.000000 ceotr_config-1.0.9/ceotr_config/template/default_setting.yml-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.244051 ceotr_config-1.0.9/ceotr_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 02:45:43.000000 ceotr_config-1.0.9/ceotr_config.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 02:45:43.245051 ceotr_config-1.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-15 02:43:01.000000 ceotr_config-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.244051 ceotr_config-1.0.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.244051 ceotr_config-1.0.9/test/ceotr_conifg_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/test/ceotr_conifg_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 02:45:43.245051 ceotr_config-1.0.9/test/ceotr_conifg_test/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.9/test/ceotr_conifg_test/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16679 2024-04-15 02:41:47.000000 ceotr_config-1.0.9/test/ceotr_conifg_test/tests.py
```

### Comparing `ceotr_config-1.0.8/README.md` & `ceotr_config-1.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,19 @@
 PROJECT_ROOT="PATH_TO_THE_PROJECT_ROOT"
 
 # if this is a Python project only
 # it will auto generate  setting YML from setting template if it not alreadt exist
 config_agenet.load(setting_path = SETTING_PATH, setting_template=SETTING_TEMPLATE_PATH)
 
 # if this is a docker python project
-# make sure in your environment variable ENVIRONMENT=docker, otherwise
-# it won't read config from .env
-config_agenet.load(setting_path = SETTING_PATH, setting_template=SETTING_TEMPLATE_PATH, docker_dot_env_path=PATH_TO_DOCKER)
+# make sure in your environment variable ENVIRONMENT=docker, otherwise it won’t read variable from environment
+config_agenet.load(setting_path = SETTING_PATH, setting_template=SETTING_TEMPLATE_PATH)
 #or
-config_agenet.load(setting_path = SETTING_PATH, setting_template=SETTING_TEMPLATE_PATH, project_root=PATH_TO_DOCKER)
+config_agenet.load(setting_path = SETTING_PATH, setting_template=SETTING_TEMPLATE_PATH)
 
-# if you give variable from docker_dot_env_path, it will read value from docker_dot_env_path
-# if you specific value for project_root and not for docker_dot_env_path, it will assign docker_dot_env_path as {project_root}/docker/.env
 ```
 
 
 # update the PyPI
 
 ## This repo will auto update the PyPI package when there is a push to master
 ### for trouble shooting look at steps below
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ceotr_config-1.0.8/ceotr_config/__init__.py` & `ceotr_config-1.0.9/ceotr_config/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     def __init__(self, default_template):
         self._debug = True
         self._config_yml = None
         self.default_template = default_template
 
     @property
     def debug(self):
-        if hasattr(self, 'general_info'):
-            return self.general_info['ENVIRONMENT'] != 'prod'
+        if hasattr(self, 'general'):
+            return self.general['ENVIRONMENT'] != 'prod'
         return self._debug
 
     def load(self, setting_path=None, setting_template=None):
         self._config_yml = ConfigHandler(setting_path, setting_template, self.default_template).build_or_load()
         self._load(self._config_yml)
 
     def _load(self, config_yml):
```

### Comparing `ceotr_config-1.0.8/ceotr_config/config_handler.py` & `ceotr_config-1.0.9/ceotr_config/config_handler.py`

 * *Files identical despite different names*

### Comparing `ceotr_config-1.0.8/ceotr_config.egg-info/SOURCES.txt` & `ceotr_config-1.0.9/ceotr_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ceotr_config-1.0.8/setup.py` & `ceotr_config-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 install_requires = [
     "PyYAML",
       "python-dotenv"
 ]
 packages = find_packages(exclude=['tests'])
 
 setup(name='ceotr_config',
-      version='1.0.8',
+      version='1.0.9',
       description="Common python library for CEOTR data team",
       author="CEOTR",
       author_email="support@ceotr.ca",
       url="https://gitlab.oceantrack.org/ceotr-public/ceotr_app_common/ceotr_config",
       packages=packages,
       include_package_data=True,
       license="GNU General Public License v3 (GPLv3)",
```

### Comparing `ceotr_config-1.0.8/test/ceotr_conifg_test/tests.py` & `ceotr_config-1.0.9/test/ceotr_conifg_test/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,16 +362,15 @@
 
         setting_path = os.path.join(self.output_path, "config.yml")
         self.config_obj.setting_path = setting_path
         self.config_obj.check_value_update = False
         res = self.config_obj.build_or_load()
         expected = {'bugs': {'HOST': 'bugs_host', 'SLOCUM_DELAY_BINARY_DATA_DIR': '', 'SLOCUM_LIVE_BINARY_DATA_DIR': '',
                              'USER': 'bugs_user', 'WEB_HOOK_TOKEN': ''},
-                    'django_settings': {'SECRET_KEY': 'SECRET_KEY'},
-                    'general_info': {'ENVIRONMENT': 'ENVIRONMENT'}}
+                    'general': {'SECRET_KEY': 'SECRET_KEY', 'ENVIRONMENT': 'ENVIRONMENT'}}
         self.assertEqual(expected, res)
 
     def test_load_environment_variable(self):
         ret_dict = {
             "database": {
                 "name": "",
                 "db": ""
@@ -429,15 +428,15 @@
         self.output_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "output")
         self.resource = os.path.join(os.path.dirname(os.path.abspath(__file__)), "resource")
         self.setting_path = os.path.join(self.resource, "passwd/pw_info.yml")
         self.tpl_path = os.path.join(self.resource, 'default_setting.yml-tpl')
 
     def test_load(self):
         self.agent.load(self.setting_path, self.tpl_path)
-        self.assertTrue(hasattr(self.agent, 'general_info'))
+        self.assertTrue(hasattr(self.agent, 'general'))
         self.assertTrue(hasattr(self.agent, 'bugs'))
 
     def test_DEBBUG_value_for_prod(self):
         self.agent.load(self.setting_path, self.tpl_path)
         self.assertFalse(self.agent.debug)
 
     def test_DEBUG_value_before_load(self):
```

