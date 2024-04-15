# Comparing `tmp/pretix-ldap-0.1.2.tar.gz` & `tmp/pretix_ldap-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-ldap-0.1.2.tar", last modified: Sun Apr  3 15:10:04 2022, max compression
+gzip compressed data, was "pretix_ldap-0.2.5.tar", last modified: Mon Apr 15 12:21:23 2024, max compression
```

## Comparing `pretix-ldap-0.1.2.tar` & `pretix_ldap-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 15:10:04.293740 pretix-ldap-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-04-03 15:10:04.293740 pretix-ldap-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 15:10:04.293740 pretix-ldap-0.1.2/pretix_ldap/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-04-03 15:09:54.000000 pretix-ldap-0.1.2/pretix_ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-04-03 15:09:54.000000 pretix-ldap-0.1.2/pretix_ldap/ldap_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 15:10:04.293740 pretix-ldap-0.1.2/pretix_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-04-03 15:10:03.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-04-03 15:10:04.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 15:10:03.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-03 15:10:03.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-03 15:10:04.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-03 15:10:04.000000 pretix-ldap-0.1.2/pretix_ldap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-04-03 15:10:04.293740 pretix-ldap-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-04-03 15:09:54.000000 pretix-ldap-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:21:23.188083 pretix_ldap-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-15 12:21:23.188083 pretix_ldap-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:21:23.184083 pretix_ldap-0.2.5/pretix_ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/pretix_ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/pretix_ldap/ldap_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:21:23.188083 pretix_ldap-0.2.5/pretix_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 12:21:23.000000 pretix_ldap-0.2.5/pretix_ldap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-15 12:21:23.188083 pretix_ldap-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:21:23.188083 pretix_ldap-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-15 12:20:51.000000 pretix_ldap-0.2.5/tests/test_pretix-ldap.py
```

### Comparing `pretix-ldap-0.1.2/PKG-INFO` & `pretix_ldap-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pretix-ldap
-Version: 0.1.2
+Version: 0.2.5
 Summary: LDAP authentication backend for pretix
 Home-page: https://github.com/Sohalt/pretix-ldap
 Author: sohalt
 Author-email: sohalt@sohalt.net
 License: Apache Software License
-Platform: UNKNOWN
+License-File: LICENSE
+Requires-Dist: ldap3
 
 pretix LDAP
 ==========================
 
 LDAP authentication plugin for `pretix`_.
 
 Installation
@@ -77,26 +78,32 @@
 
 5. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 Running CI linter and tests locally
 -----------------------------------
 
-1. Set up docker
+1. `Install nix`_
 
-2. Install test dependencies: `pip install -r src/tests/requirements.txt`
+2. Enter devshell: `nix develop`
 
-3. Run linter::
+3. Build package::
+
+    python -m build
+
+4. Run linter::
 
-    cd src/
     flake8
 
-4. Run tests::
+5. Run tests::
+
+    cp -r dist tests
+
+    cd tests
 
-    cd src/tests
     pytest
 
 
 License
 -------
 
 
@@ -104,9 +111,8 @@
 
 Released under the terms of the Apache License 2.0
 
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
-
-
+.. _Install nix: https://github.com/DeterminateSystems/nix-installer
```

### Comparing `pretix-ldap-0.1.2/pretix_ldap/__init__.py` & `pretix_ldap-0.2.5/pretix_ldap/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .ldap_connector import LDAPAuthBackend  # noqa
-from django.utils.translation import ugettext_lazy
+from django.utils.translation import gettext_lazy
 
 try:
     from pretix.base.plugins import PluginConfig
 except ImportError:
     raise RuntimeError("Please use pretix 2.7 or above to run this plugin!")
 
 
 class PluginApp(PluginConfig):
     name = "pretix_ldap"
     verbose_name = "pretix LDAP"
 
     class PretixPluginMeta:
-        name = ugettext_lazy("pretix LDAP")
+        name = gettext_lazy("pretix LDAP")
         author = "sohalt"
-        description = ugettext_lazy("LDAP authentication backend for pretix")
+        description = gettext_lazy("LDAP authentication backend for pretix")
         visible = True
-        version = "0.1.2"
-        compatibility = "pretix>=4.7.0"
+        version = "0.2.5"
+        compatibility = "pretix>=2023.06.0"
 
 
 default_app_config = "pretix_ldap.PluginApp"
```

### Comparing `pretix-ldap-0.1.2/pretix_ldap/ldap_connector.py` & `pretix_ldap-0.2.5/pretix_ldap/ldap_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ldap3 import Server, Connection
 from ldap3.utils.conv import escape_filter_chars
 import re
 import logging
 from django import forms
 from django.contrib import messages
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from pretix.settings import config
 from pretix.base.auth import BaseAuthBackend
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `pretix-ldap-0.1.2/pretix_ldap.egg-info/PKG-INFO` & `pretix_ldap-0.2.5/pretix_ldap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pretix-ldap
-Version: 0.1.2
+Version: 0.2.5
 Summary: LDAP authentication backend for pretix
 Home-page: https://github.com/Sohalt/pretix-ldap
 Author: sohalt
 Author-email: sohalt@sohalt.net
 License: Apache Software License
-Platform: UNKNOWN
+License-File: LICENSE
+Requires-Dist: ldap3
 
 pretix LDAP
 ==========================
 
 LDAP authentication plugin for `pretix`_.
 
 Installation
@@ -77,26 +78,32 @@
 
 5. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 Running CI linter and tests locally
 -----------------------------------
 
-1. Set up docker
+1. `Install nix`_
 
-2. Install test dependencies: `pip install -r src/tests/requirements.txt`
+2. Enter devshell: `nix develop`
 
-3. Run linter::
+3. Build package::
+
+    python -m build
+
+4. Run linter::
 
-    cd src/
     flake8
 
-4. Run tests::
+5. Run tests::
+
+    cp -r dist tests
+
+    cd tests
 
-    cd src/tests
     pytest
 
 
 License
 -------
 
 
@@ -104,9 +111,8 @@
 
 Released under the terms of the Apache License 2.0
 
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
-
-
+.. _Install nix: https://github.com/DeterminateSystems/nix-installer
```

### Comparing `pretix-ldap-0.1.2/setup.py` & `pretix_ldap-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from setuptools import setup, find_packages
 
 
 try:
     with open(
-        os.path.join(os.path.dirname(__file__), "../README.rst"), encoding="utf-8"
+        os.path.join(os.path.dirname(__file__), "README.rst"), encoding="utf-8"
     ) as f:
         long_description = f.read()
 except:  # NOQA
     long_description = ""
 
 
 setup(
     name="pretix-ldap",
-    version="0.1.2",
+    version="0.2.5",
     description="LDAP authentication backend for pretix",
     long_description=long_description,
     url="https://github.com/Sohalt/pretix-ldap",
     author="sohalt",
     author_email="sohalt@sohalt.net",
     license="Apache Software License",
     install_requires=["ldap3"],
```

