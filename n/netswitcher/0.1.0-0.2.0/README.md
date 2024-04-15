# Comparing `tmp/netswitcher-0.1.0.tar.gz` & `tmp/netswitcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netswitcher-0.1.0.tar", max compression
+gzip compressed data, was "netswitcher-0.2.0.tar", max compression
```

## Comparing `netswitcher-0.1.0.tar` & `netswitcher-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     2016 2024-04-15 14:16:50.088914 netswitcher-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-23 11:20:27.437174 netswitcher-0.1.0/core/__init__.py
--rw-r--r--   0        0        0     3278 2024-04-15 13:46:20.572397 netswitcher-0.1.0/core/acl.py
--rw-r--r--   0        0        0     2827 2024-04-15 13:46:22.396353 netswitcher-0.1.0/core/lacp.py
--rw-r--r--   0        0        0     1333 2024-04-15 13:46:24.316307 netswitcher-0.1.0/core/speed.py
--rw-r--r--   0        0        0     1074 2024-04-15 13:46:26.680250 netswitcher-0.1.0/core/state.py
--rw-r--r--   0        0        0     2021 2024-04-15 13:46:28.660202 netswitcher-0.1.0/core/status.py
--rw-r--r--   0        0        0      492 2024-04-15 12:19:34.018554 netswitcher-0.1.0/core/utils.py
--rw-r--r--   0        0        0      449 2024-04-15 13:02:49.943549 netswitcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 netswitcher-0.1.0/setup.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 netswitcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2016 2024-04-15 14:16:50.088914 netswitcher-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-23 11:20:27.437174 netswitcher-0.2.0/core/__init__.py
+-rw-r--r--   0        0        0     3278 2024-04-15 13:46:20.572397 netswitcher-0.2.0/core/acl.py
+-rw-r--r--   0        0        0     2827 2024-04-15 13:46:22.396353 netswitcher-0.2.0/core/lacp.py
+-rw-r--r--   0        0        0      863 2024-04-15 14:08:02.053593 netswitcher-0.2.0/core/main.py
+-rw-r--r--   0        0        0     1333 2024-04-15 13:46:24.316307 netswitcher-0.2.0/core/speed.py
+-rw-r--r--   0        0        0     1074 2024-04-15 13:46:26.680250 netswitcher-0.2.0/core/state.py
+-rw-r--r--   0        0        0     2021 2024-04-15 13:46:28.660202 netswitcher-0.2.0/core/status.py
+-rw-r--r--   0        0        0      492 2024-04-15 12:19:34.018554 netswitcher-0.2.0/core/utils.py
+-rw-r--r--   0        0        0      454 2024-04-15 14:26:26.387076 netswitcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 netswitcher-0.2.0/setup.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 netswitcher-0.2.0/PKG-INFO
```

### Comparing `netswitcher-0.1.0/README.md` & `netswitcher-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/core/acl.py` & `netswitcher-0.2.0/core/acl.py`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/core/lacp.py` & `netswitcher-0.2.0/core/lacp.py`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/core/speed.py` & `netswitcher-0.2.0/core/speed.py`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/core/state.py` & `netswitcher-0.2.0/core/state.py`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/core/status.py` & `netswitcher-0.2.0/core/status.py`

 * *Files identical despite different names*

### Comparing `netswitcher-0.1.0/setup.py` & `netswitcher-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['netmiko>=4.3.0,<5.0.0', 'typer-slim>=0.12.3,<0.13.0']
 
 entry_points = \
-{'console_scripts': ['nt = main:create_app']}
+{'console_scripts': ['nt = core.main:create_app']}
 
 setup_kwargs = {
     'name': 'netswitcher',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# netswitcher (nt)\n\n```console\nUsage: nt [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n\nCommands:\n  acl\n  lacp\n  speed\n  state\n  status\n```\n\n## Installation\n```console\npip install nt\n```\n\nor\n\n```console\ngit clone https://github.com/Fearkin/netswitcher/tree/master\n\npoetry install\n```\n## Usage:\n**`nt acl` [action]** - команда для работы с ACL\n\nName of interface should be ge-(0-9)/(0-9)/(0-9)\n\n- add     *ACL_name* *interface_name* - Adds ACL rule with given name to interface\n\n- create  *name* IP - Creates ACL rule with given name\n\n- delete  *name* IP - Deletes IP from ACL with given name\n\n- find    *name* - Shows ACL with given name\n\n- prune   *name* - Deletes ACL rule with given name\n\n- remove  *ACL_name* *interface_name* - Removes ACL rule with given name from interface\n\n\n**`nt status` [action]** - команда для проверки интерфейсов\n\n- int   *name* - Shows current state of interface\n\n- lacp  *name* - Shows active LACP with given name and all created LACP\n\n- show  *name* OR show --mac *MAC* - Shows current configuration of interface\n\n\n**`nt speed` [action]** - команда для изменения скорости\n\n- desc  *name* *description* - Set description for interface\n\n- set   *name* *speed* (10m|100m|1g) - Set speed for interface\n\n**`nt lacp` [action]** - команда для работы с LACP\n\n\n- create  *port (0-9)* *description* *interface1* *interface2* - Creates LACP\n\n- delete  *port (0-9)* - Deletes LACP\n\n- remove  *name* - Removes interface from LACP\n\n**`nt state` on/off *name*** - включить/выключить интерфейс\n',
     'author': 'Fearkin',
     'author_email': 'aloneWorker@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `netswitcher-0.1.0/PKG-INFO` & `netswitcher-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netswitcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Fearkin
 Author-email: aloneWorker@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

