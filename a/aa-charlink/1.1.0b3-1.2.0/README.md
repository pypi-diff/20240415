# Comparing `tmp/aa_charlink-1.1.0b3.tar.gz` & `tmp/aa_charlink-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_charlink-1.1.0b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_charlink-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_charlink-1.1.0b3.tar` & `aa_charlink-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rwxr-xr-x   0        0        0    35149 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/LICENSE
--rwxr-xr-x   0        0        0     3945 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/README.md
--rwxr-xr-x   0        0        0      129 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/__init__.py
--rw-r--r--   0        0        0     2713 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/app_imports/__init__.py
--rw-r--r--   0        0        0     5216 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/app_imports/utils.py
--rwxr-xr-x   0        0        0      108 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/app_settings.py
--rwxr-xr-x   0        0        0      148 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/apps.py
--rwxr-xr-x   0        0        0      754 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/auth_hooks.py
--rwxr-xr-x   0        0        0      494 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/decorators.py
--rwxr-xr-x   0        0        0      652 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/forms.py
--rwxr-xr-x   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/__init__.py
--rw-r--r--   0        0        0     2882 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/afat.py
--rwxr-xr-x   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/allianceauth/__init__.py
--rwxr-xr-x   0        0        0     1777 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/allianceauth/corputils.py
--rw-r--r--   0        0        0     1788 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/corpstats.py
--rwxr-xr-x   0        0        0     4001 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/corptools.py
--rwxr-xr-x   0        0        0     2058 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/memberaudit.py
--rwxr-xr-x   0        0        0     1548 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/miningtaxes.py
--rwxr-xr-x   0        0        0     2600 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/moonmining.py
--rwxr-xr-x   0        0        0     1689 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/moonstuff.py
--rwxr-xr-x   0        0        0     3962 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/imports/structures.py
--rw-r--r--   0        0        0      810 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/migrations/__init__.py
--rwxr-xr-x   0        0        0      435 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/models.py
--rw-r--r--   0        0        0       62 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/static/charlink/css/added-icons.css
--rw-r--r--   0        0        0     4278 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/app_audit.html
--rwxr-xr-x   0        0        0     4080 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/audit.html
--rw-r--r--   0        0        0      746 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/base.html
--rwxr-xr-x   0        0        0     6096 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/charlink.html
--rw-r--r--   0        0        0      532 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/dashboard_login.html
--rw-r--r--   0        0        0      903 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/menu-left.html
--rw-r--r--   0        0        0      431 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/menu-right.html
--rw-r--r--   0        0        0     2711 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/search.html
--rw-r--r--   0        0        0     3004 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templates/charlink/user_audit.html
--rw-r--r--   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templatetags/__init__.py
--rw-r--r--   0        0        0      837 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/templatetags/charlinkutils.py
--rw-r--r--   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/__init__.py
--rw-r--r--   0        0        0     3943 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_afat.py
--rw-r--r--   0        0        0     3060 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_allianceauth_corputils.py
--rw-r--r--   0        0        0     2980 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_corpstats.py
--rw-r--r--   0        0        0     3798 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_corptools.py
--rw-r--r--   0        0        0     3213 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_memberaudit.py
--rw-r--r--   0        0        0     2272 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_miningtaxes.py
--rw-r--r--   0        0        0     3710 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_moonmining.py
--rw-r--r--   0        0        0     2440 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_moonstuff.py
--rw-r--r--   0        0        0     5986 2024-03-14 15:49:52.780784 aa_charlink-1.1.0b3/charlink/tests/imports/test_structures.py
--rw-r--r--   0        0        0     7861 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_app_imports.py
--rwxr-xr-x   0        0        0     1234 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1323 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_decorators.py
--rw-r--r--   0        0        0     1261 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_forms.py
--rw-r--r--   0        0        0     2241 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_templatetags.py
--rw-r--r--   0        0        0     5488 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_utils.py
--rw-r--r--   0        0        0    20489 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/tests/test_views.py
--rwxr-xr-x   0        0        0      520 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/urls.py
--rw-r--r--   0        0        0     2703 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/utils.py
--rwxr-xr-x   0        0        0     8267 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/charlink/views.py
--rwxr-xr-x   0        0        0     1530 2024-03-14 15:49:52.784784 aa_charlink-1.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     5417 1970-01-01 00:00:00.000000 aa_charlink-1.1.0b3/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/LICENSE
+-rwxr-xr-x   0        0        0     3945 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/README.md
+-rwxr-xr-x   0        0        0      127 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/__init__.py
+-rw-r--r--   0        0        0     2713 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_imports/__init__.py
+-rw-r--r--   0        0        0     5216 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_imports/utils.py
+-rwxr-xr-x   0        0        0      108 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/app_settings.py
+-rwxr-xr-x   0        0        0      148 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/apps.py
+-rwxr-xr-x   0        0        0      754 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/auth_hooks.py
+-rwxr-xr-x   0        0        0      494 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/decorators.py
+-rwxr-xr-x   0        0        0      652 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/forms.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/afat.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0        0        0     1777 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0        0        0     1788 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/corpstats.py
+-rwxr-xr-x   0        0        0     4001 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/corptools.py
+-rwxr-xr-x   0        0        0     2058 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/memberaudit.py
+-rwxr-xr-x   0        0        0     1548 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0        0        0     2600 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/moonmining.py
+-rwxr-xr-x   0        0        0     1689 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/moonstuff.py
+-rwxr-xr-x   0        0        0     3962 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/imports/structures.py
+-rw-r--r--   0        0        0      810 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/migrations/__init__.py
+-rwxr-xr-x   0        0        0      435 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/models.py
+-rw-r--r--   0        0        0       62 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/static/charlink/css/added-icons.css
+-rw-r--r--   0        0        0     4306 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/app_audit.html
+-rwxr-xr-x   0        0        0     4080 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/audit.html
+-rw-r--r--   0        0        0      746 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/base.html
+-rwxr-xr-x   0        0        0     6124 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0        0        0      532 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/dashboard_login.html
+-rw-r--r--   0        0        0      903 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/menu-left.html
+-rw-r--r--   0        0        0      431 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/menu-right.html
+-rw-r--r--   0        0        0     2711 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/search.html
+-rw-r--r--   0        0        0     3032 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templates/charlink/user_audit.html
+-rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/charlink_versioned_static.py
+-rw-r--r--   0        0        0      837 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/templatetags/charlinkutils.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/__init__.py
+-rw-r--r--   0        0        0     3943 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_afat.py
+-rw-r--r--   0        0        0     3060 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_allianceauth_corputils.py
+-rw-r--r--   0        0        0     2980 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_corpstats.py
+-rw-r--r--   0        0        0     3798 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_corptools.py
+-rw-r--r--   0        0        0     3213 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_memberaudit.py
+-rw-r--r--   0        0        0     2272 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_miningtaxes.py
+-rw-r--r--   0        0        0     3710 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_moonmining.py
+-rw-r--r--   0        0        0     2440 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_moonstuff.py
+-rw-r--r--   0        0        0     5986 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/imports/test_structures.py
+-rw-r--r--   0        0        0     7861 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_app_imports.py
+-rwxr-xr-x   0        0        0     1265 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1323 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_decorators.py
+-rw-r--r--   0        0        0     1261 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_forms.py
+-rw-r--r--   0        0        0     2241 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_templatetags.py
+-rw-r--r--   0        0        0     5488 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_utils.py
+-rw-r--r--   0        0        0    20489 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/tests/test_views.py
+-rwxr-xr-x   0        0        0      520 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/urls.py
+-rw-r--r--   0        0        0     2703 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/utils.py
+-rwxr-xr-x   0        0        0     8267 2024-04-15 20:22:47.868466 aa_charlink-1.2.0/charlink/views.py
+-rwxr-xr-x   0        0        0     1519 2024-04-15 20:22:47.872466 aa_charlink-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 aa_charlink-1.2.0/PKG-INFO
```

### Comparing `aa_charlink-1.1.0b3/LICENSE` & `aa_charlink-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/README.md` & `aa_charlink-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/app_imports/__init__.py` & `aa_charlink-1.2.0/charlink/app_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/app_imports/utils.py` & `aa_charlink-1.2.0/charlink/app_imports/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/auth_hooks.py` & `aa_charlink-1.2.0/charlink/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/forms.py` & `aa_charlink-1.2.0/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/afat.py` & `aa_charlink-1.2.0/charlink/imports/afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/allianceauth/corputils.py` & `aa_charlink-1.2.0/charlink/imports/allianceauth/corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/corpstats.py` & `aa_charlink-1.2.0/charlink/imports/corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/corptools.py` & `aa_charlink-1.2.0/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/memberaudit.py` & `aa_charlink-1.2.0/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/miningtaxes.py` & `aa_charlink-1.2.0/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/moonmining.py` & `aa_charlink-1.2.0/charlink/imports/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/moonstuff.py` & `aa_charlink-1.2.0/charlink/imports/moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/imports/structures.py` & `aa_charlink-1.2.0/charlink/imports/structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/migrations/0001_initial.py` & `aa_charlink-1.2.0/charlink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/app_audit.html` & `aa_charlink-1.2.0/charlink/templates/charlink/app_audit.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'charlink/base.html' %}
 {% load charlinkutils %}
-{% load static %}
+{% load charlink_versioned_static %}
 
 {% block page_title %}Charlink App Audit{% endblock page_title %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% static 'charlink/css/added-icons.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% charlink_static 'charlink/css/added-icons.css' %}">
     {% include "bundles/datatables-css-bs5.html" %}
 {% endblock extra_css %}
 
 {% block charlink_page_header %}<h1 class="page-header text-center">Links Audit</h1>{% endblock charlink_page_header %}
 
 {% block charlink_content %}
     <div class="card">
```

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/audit.html` & `aa_charlink-1.2.0/charlink/templates/charlink/audit.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/base.html` & `aa_charlink-1.2.0/charlink/templates/charlink/base.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/charlink.html` & `aa_charlink-1.2.0/charlink/templates/charlink/charlink.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends 'charlink/base.html' %}
 {% load django_bootstrap5 %}
 {% load charlinkutils %}
-{% load static %}
+{% load charlink_versioned_static %}
 
 {% block page_title %}Charlink{% endblock page_title %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% static 'charlink/css/added-icons.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% charlink_static 'charlink/css/added-icons.css' %}">
 {% endblock extra_css %}
 
 {% block charlink_page_header %}<h1 class="page-header text-center">Character Linking</h1>{% endblock charlink_page_header %}
 
 {% block charlink_content %}
     <div class="card">
         <div class="card-header">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'charlink/base.html' %} {% load django_bootstrap5 %} {% load
-charlinkutils %} {% load static %} {% block page_title %}Charlink{% endblock
-page_title %} {% block extra_css %}
+charlinkutils %} {% load charlink_versioned_static %} {% block page_title
+%}Charlink{% endblock page_title %} {% block extra_css %}
 {% endblock extra_css %} {% block charlink_page_header %}
 ************ CChhaarraacctteerr LLiinnkkiinngg ************
 {% endblock charlink_page_header %} {% block charlink_content %}
     * Login Form
     * Linked Characters
 Select the apps you want to link from the list. You will be redirected to
 eveonline website to authenticate and provide the token with all the scopes
```

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/dashboard_login.html` & `aa_charlink-1.2.0/charlink/templates/charlink/dashboard_login.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/menu-left.html` & `aa_charlink-1.2.0/charlink/templates/charlink/menu-left.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/search.html` & `aa_charlink-1.2.0/charlink/templates/charlink/search.html`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/templates/charlink/user_audit.html` & `aa_charlink-1.2.0/charlink/templates/charlink/user_audit.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'charlink/base.html' %}
 {% load charlinkutils %}
-{% load static %}
+{% load charlink_versioned_static %}
 
 {% block page_title %}Charlink User Audit{% endblock page_title %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% static 'charlink/css/added-icons.css' %}">
+    <link rel="stylesheet" type="text/css" href="{% charlink_static 'charlink/css/added-icons.css' %}">
     {% include "bundles/datatables-css-bs5.html" %}
 {% endblock extra_css %}
 
 {% block charlink_page_header %}<h1 class="page-header text-center">Links Audit</h1>{% endblock charlink_page_header %}
 
 {% block charlink_content %}
     <div class="card">
```

### Comparing `aa_charlink-1.1.0b3/charlink/templatetags/charlinkutils.py` & `aa_charlink-1.2.0/charlink/templatetags/charlinkutils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_afat.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_afat.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_allianceauth_corputils.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_allianceauth_corputils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_corpstats.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_corpstats.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_corptools.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_corptools.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_memberaudit.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_miningtaxes.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_moonmining.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_moonstuff.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_moonstuff.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/imports/test_structures.py` & `aa_charlink-1.2.0/charlink/tests/imports/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_app_imports.py` & `aa_charlink-1.2.0/charlink/tests/test_app_imports.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_auth_hooks.py` & `aa_charlink-1.2.0/charlink/tests/test_auth_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
                 <i class="nav-link fas fa-link fa-fw align-self-center me-3 active"></i>
-                <a class="nav-link flex-fill align-self-center me-auto" href="{reverse('charlink:index')}">
+                <a class="nav-link flex-fill align-self-center me-auto active" href="{reverse('charlink:index')}">
                     CharLink
                 </a>
             </li>
         """
-        cls.html_dashboard = f'<form method="post" action="{reverse("charlink:dashboard_post")}">'
+        cls.html_dashboard = (
+            f'<form method="post" action="{reverse("charlink:dashboard_post")}">'
+        )
 
     def test_menu_hook(self):
         self.client.force_login(self.testuser)
 
-        response = self.client.get(reverse('charlink:index'))
+        response = self.client.get(reverse("charlink:index"))
         self.assertContains(response, self.html_menu, html=True)
 
     def test_dashboard_hook(self):
         self.client.force_login(self.testuser)
 
-        response = self.client.get(reverse('authentication:dashboard'))
+        response = self.client.get(reverse("authentication:dashboard"))
         self.assertContains(response, self.html_dashboard, status_code=200)
```

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_decorators.py` & `aa_charlink-1.2.0/charlink/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_forms.py` & `aa_charlink-1.2.0/charlink/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_templatetags.py` & `aa_charlink-1.2.0/charlink/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_utils.py` & `aa_charlink-1.2.0/charlink/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/tests/test_views.py` & `aa_charlink-1.2.0/charlink/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/urls.py` & `aa_charlink-1.2.0/charlink/urls.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/utils.py` & `aa_charlink-1.2.0/charlink/utils.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/charlink/views.py` & `aa_charlink-1.2.0/charlink/views.py`

 * *Files identical despite different names*

### Comparing `aa_charlink-1.1.0b3/pyproject.toml` & `aa_charlink-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "allianceauth",
     "eveonline",
 	"allianceauth_charlink",
     "charlink",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "allianceauth>=4.0.0b2,<5.0.0",
+    "allianceauth~=4.0",
     "allianceauth-app-utils~=1.14",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Maestro-Zacht/aa-charlink"
 Source = "https://github.com/Maestro-Zacht/aa-charlink"
 Tracker = "https://github.com/Maestro-Zacht/aa-charlink/issues"
```

### Comparing `aa_charlink-1.1.0b3/PKG-INFO` & `aa_charlink-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 1.1.0b3
+Version: 1.2.0
 Summary: Character Linker for Alliance Auth
 Keywords: allianceauth,eveonline,allianceauth_charlink,charlink
 Author-email: Matteo Ghia <matteo.ghia@yahoo.it>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: allianceauth>=4.0.0b2,<5.0.0
+Requires-Dist: allianceauth~=4.0
 Requires-Dist: allianceauth-app-utils~=1.14
 Project-URL: Changelog, https://github.com/Maestro-Zacht/aa-charlink/releases
 Project-URL: Homepage, https://github.com/Maestro-Zacht/aa-charlink
 Project-URL: Source, https://github.com/Maestro-Zacht/aa-charlink
 Project-URL: Tracker, https://github.com/Maestro-Zacht/aa-charlink/issues
 
 # AllianceAuth CharLink
```

