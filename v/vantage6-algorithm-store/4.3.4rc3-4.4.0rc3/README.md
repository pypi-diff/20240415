# Comparing `tmp/vantage6-algorithm-store-4.3.4rc3.tar.gz` & `tmp/vantage6-algorithm-store-4.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-store-4.3.4rc3.tar", last modified: Mon Mar 25 11:02:01 2024, max compression
+gzip compressed data, was "vantage6-algorithm-store-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:20 2024, max compression
```

## Comparing `vantage6-algorithm-store-4.3.4rc3.tar` & `vantage6-algorithm-store-4.4.0rc3.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.883176 vantage6-algorithm-store-4.3.4rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-03-25 11:02:01.883176 vantage6-algorithm-store-4.3.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:02:01.883176 vantage6-algorithm-store-4.3.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.875177 vantage6-algorithm-store-4.3.4rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.875177 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.879176 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.879176 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.879176 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/developer_algorithm_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/review.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.879176 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18548 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.883176 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/schema/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/schema/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/vantage6_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-25 11:01:46.000000 vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.883176 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-03-25 11:02:01.000000 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-25 11:02:01.000000 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:02:01.000000 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-25 11:02:01.000000 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 11:02:01.000000 vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.815519 vantage6-algorithm-store-4.4.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.815519 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.815519 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/common/ui_visualization_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/developer_algorithm_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/ui_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/vantage6_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 13:15:06.000000 vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.819520 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-15 13:15:20.000000 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-15 13:15:20.000000 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:20.000000 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:15:20.000000 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:15:20.000000 vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/PKG-INFO` & `vantage6-algorithm-store-4.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.3.4rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.4.0rc3 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/setup.py` & `vantage6-algorithm-store-4.4.0rc3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         "flasgger==0.9.5",
         "flask==2.2.5",
         "Flask-Cors==3.0.10",
         "Flask-Principal==0.4.0",
         "flask-marshmallow==0.15.0",
         "Flask-RESTful==0.3.10",
         "gevent==23.9.1",
+        "jsonschema==4.21.1",
         "marshmallow==3.19.0",
         "requests==2.31.0",
         "schema==0.7.5",
         "SQLAlchemy==1.4.46",
         "werkzeug==3.0.1",
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-common == {version_ns["__version__"]}',
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/__init__.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,20 @@
 from flask_principal import Principal
 from flasgger import Swagger
 from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import APPNAME
 from vantage6.backend.common.resource.output_schema import BaseHATEOASModelSchema
+from vantage6.backend.common.globals import HOST_URI_ENV
 
 # TODO move this to common, then remove dependency on CLI in algorithm store
 from vantage6.cli.context.algorithm_store import AlgorithmStoreContext
 from vantage6.algorithm.store._version import __version__
-from vantage6.algorithm.store.globals import API_PATH, HOST_URI_ENV
+from vantage6.algorithm.store.globals import API_PATH
 from vantage6.algorithm.store.globals import RESOURCES, SERVER_MODULE_NAME
 
 # TODO the following are simply copies of the same files in the server - refactor
 from vantage6.algorithm.store.model.base import Base, DatabaseSessionManager, Database
 from vantage6.algorithm.store import db
 
 # TODO move server imports to common / refactor
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/_version.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 3, 4, "candidate", __build__, 0)
+version_info = (4, 4, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/db.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/default_roles.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/globals.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/globals.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,10 +13,7 @@
 # URL extension for the API endpoints
 API_PATH = "/api"
 
 # TODO: this should be done differently
 # Which resources should be initialized. These names correspond to the
 # file-names in the resource directory
 RESOURCES = ["version", "algorithm", "vantage6_server", "role", "rule", "user"]
-
-# environment variable name for host URI
-HOST_URI_ENV = "HOST_URI_ENV_VAR"
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/__init__.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,7 +9,8 @@
 from vantage6.algorithm.store.model.role_rule_association import role_rule_association
 from vantage6.algorithm.store.model.permission import Permission
 from vantage6.algorithm.store.model.user import User
 from vantage6.algorithm.store.model.developer_algorithm_association import (
     developer_algorithm_association,
 )
 from vantage6.algorithm.store.model.review import Review
+from vantage6.algorithm.store.model.ui_visualization import UIVisualization
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/algorithm.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 from sqlalchemy import Column, String
 from sqlalchemy.orm import relationship
 
 from vantage6.algorithm.store.model.base import Base
 
 
 class Algorithm(Base):
@@ -20,14 +19,18 @@
     partitioning : str
         Type of partitioning
     vantage6_version : str
         Version of vantage6 that the algorithm is built with
 
     functions : list[:class:`~.model.function.function`]
         List of functions that are available in the algorithm
+    developer : list[:class:`~.model.user.User`]
+        List of users that have developed the algorithm
+    review : :class:`~.model.review.Review`
+        Review of the algorithm
     """
 
     # fields
     name = Column(String)
     description = Column(String)
     image = Column(String)
     # status = Column(String)
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/argument.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/argument.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     ----------
     name : str
         Name of the argument
     description : str
         Description of the argument
     function_id : int
         ID of the algorithm that this function belongs to
-    function : :class:`~.model.algorithm.algorithm`
-        Algorithm function that this argument belongs to
     type_ : str
         Type of the argument
+    function : :class:`~.model.algorithm.algorithm`
+        Algorithm function that this argument belongs to
     """
 
     # fields
     name = Column(String)
     description = Column(String)
     function_id = Column(Integer, ForeignKey("function.id"))
     type_ = Column("type", String)
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/base.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/common/enums.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/common/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,22 +15,31 @@
     FEDERATED = "federated"
 
 
 class ArgumentType(str, enum.Enum):
     """Enum for argument types"""
 
     COLUMN = "column"
+    COLUMNS = "column_list"
     STRING = "string"
+    STRINGS = "string_list"
     INTEGER = "integer"
+    INTEGERS = "integer_list"
     FLOAT = "float"
+    FLOATS = "float_list"
     BOOLEAN = "boolean"
-    DATE = "date"
     JSON = "json"
-    ORGANIZATIONS = "organizations"
     ORGANIZATION = "organization"
+    ORGANIZATIONS = "organization_list"
+
+
+class VisualizationType(str, enum.Enum):
+    """Enum for visualization types"""
+
+    TABLE = "table"
 
 
 class ReviewStatus(str, enum.Enum):
     """Enum for review status"""
 
     DRAFT = "draft"
     UNDER_REVIEW = "under review"
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/database.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/database.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/function.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/function.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 from sqlalchemy import Column, String, ForeignKey, Integer
 from sqlalchemy.orm import relationship
 
 from vantage6.algorithm.store.model.base import Base
 
 
 class Function(Base):
@@ -18,26 +17,28 @@
         Name of the function
     description : str
         Description of the function
     type_ : str
         Type of function
     algorithm_id : int
         ID of the algorithm that this function belongs to
-    algorithm : :class:`~.model.algorithm.algorithm`
+    algorithm : :class:`~.model.algorithm.Algorithm`
         Algorithm that this function belongs to
-    databases : list[:class:`~.model.database.database`]
+    databases : list[:class:`~.model.database.Database`]
         List of databases that this function uses
-    arguments : list[:class:`~.model.argument.argument`]
+    arguments : list[:class:`~.model.argument.Argument`]
         List of arguments that this function uses
+    ui_visualizations : list[:class:`~.model.ui_visualization.UIVisualization`]
+        List of user interface visualizations that this function produces
     """
 
     # fields
     name = Column(String)
     description = Column(String)
     type_ = Column("type", String)
     algorithm_id = Column(Integer, ForeignKey("algorithm.id"))
 
     # relationships
     algorithm = relationship("Algorithm", back_populates="functions")
     databases = relationship("Database", back_populates="function")
     arguments = relationship("Argument", back_populates="function")
-    # output = relationship("Output", back_populates='function')
+    ui_visualizations = relationship("UIVisualization", back_populates="function")
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/permission.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/review.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/review.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     ----------
     algorithm_id : int
         Id of the algorithm
     reviewer_id : int
         Id of the user appointed as reviewer
     status : str
         Review status
+    reviewers : list[:class:`~.model.user.User`]
+        List of users that have written reviews
+    algorithm : :class:`~.model.algorithm.Algorithm`
+        Algorithm that the review is linked to
     """
 
     # fields
     algorithm_id = Column(Integer, ForeignKey("algorithm.id"))
     reviewer_id = Column(Integer, ForeignKey("user.id"))
     status = Column(Text)
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/role.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/role_rule_association.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/role_rule_association.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/rule.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/user.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
     Attributes
     ----------
     username : str
         Username
     v6_server_id : int
         Id of the whitelisted server through which the user is authenticated
+    server : :class:`~.model.vantage6_server.Vantage6Server`
+        Server through which the user is authenticated
+    roles : list[:class:`~.model.role.Role`]
+        List of roles that the user has
+    algorithms : list[:class:`~.model.algorithm.Algorithm`]
+        List of algorithms that the user has developed
+    reviews : list[:class:`~.model.review.Review`]
+        List of reviews that the user has written
     """
 
     # fields
     # link with the v6 server. This is a temporary solution
     username = Column(String)
     v6_server_id = Column(Integer, ForeignKey("vantage6server.id"))
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/model/vantage6_server.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/model/vantage6_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     linked to. It essentially serves as a whitelist of servers that are allowed
     to use this algorithm store.
 
     Attributes
     ----------
     url : str
         URL of the vantage6 server
+    users : list[:class:`~.model.user.User`]
+        List of known vantage6 users from that server
     """
 
     # fields
     url = Column(String, unique=True)
 
     # relationships
     users = relationship("User", back_populates="server")
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/permission.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/__init__.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/algorithm.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/algorithm.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from flask import g, request
 from flask_restful import Api
 from http import HTTPStatus
 
 from vantage6.algorithm.store import db
 from vantage6.algorithm.store.model.rule import Operation
 from vantage6.common import logger_name
+from vantage6.algorithm.store.model.ui_visualization import UIVisualization
 from vantage6.algorithm.store.resource.schema.input_schema import AlgorithmInputSchema
 from vantage6.algorithm.store.resource.schema.output_schema import AlgorithmOutputSchema
 from vantage6.algorithm.store.model.algorithm import Algorithm as db_Algorithm
 from vantage6.algorithm.store.model.argument import Argument
 from vantage6.algorithm.store.model.database import Database
 from vantage6.algorithm.store.model.function import Function
 from vantage6.algorithm.store.resource import (
@@ -140,17 +141,27 @@
             description: Unauthorized
 
         security:
           - bearerAuth: []
 
         tags: ["Algorithm"]
         """
-        # TODO add filtering
         q = g.session.query(db_Algorithm)
 
+        # filter on properties
+        for field in [
+            "name",
+            "description",
+            "image",
+            "partitioning",
+            "vantage6_version",
+        ]:
+            if (value := request.args.get(field)) is not None:
+                q = q.filter(getattr(db_Algorithm, field).like(f"%{value}%"))
+
         # paginate results
         try:
             page = Pagination.from_query(q, request, db.Algorithm)
         except (ValueError, AttributeError) as e:
             return {"msg": str(e)}, HTTPStatus.BAD_REQUEST
 
         # model serialization
@@ -230,14 +241,32 @@
                                 type: string
                                 description: Description of the argument
                               type:
                                 type: string
                                 description: Type of argument. Can be 'string',
                                   'integer', 'float', 'boolean', 'json',
                                   'column', 'organizations' or 'organization'
+                        ui_visualizations:
+                          type: array
+                          description: List of visualizations that are available in
+                            the algorithm
+                          items:
+                            properties:
+                              name:
+                                type: string
+                                description: Name of the visualization
+                              description:
+                                type: string
+                                description: Description of the visualization
+                              type:
+                                type: string
+                                description: Type of visualization.
+                              schema:
+                                type: object
+                                description: Schema that describes the visualization
 
         responses:
           201:
             description: Algorithm created successfully
           400:
             description: Invalid input
           401:
@@ -275,34 +304,40 @@
                 name=function["name"],
                 description=function.get("description", ""),
                 type_=function["type"],
                 algorithm_id=algorithm.id,
             )
             func.save()
             # create the arguments
-            arguments = function.get("arguments")
-            if arguments:
-                for argument in arguments:
-                    arg = Argument(
-                        name=argument["name"],
-                        description=argument.get("description", ""),
-                        type_=argument["type"],
-                        function_id=func.id,
-                    )
-                    arg.save()
+            for argument in function.get("arguments", []):
+                arg = Argument(
+                    name=argument["name"],
+                    description=argument.get("description", ""),
+                    type_=argument["type"],
+                    function_id=func.id,
+                )
+                arg.save()
             # create the databases
-            databases = function.get("databases")
-            if databases:
-                for database in databases:
-                    db = Database(
-                        name=database["name"],
-                        description=database.get("description", ""),
-                        function_id=func.id,
-                    )
-                    db.save()
+            for database in function.get("databases", []):
+                db = Database(
+                    name=database["name"],
+                    description=database.get("description", ""),
+                    function_id=func.id,
+                )
+                db.save()
+            # create the visualizations
+            for visualization in function.get("ui_visualizations", []):
+                vis = UIVisualization(
+                    name=visualization["name"],
+                    description=visualization.get("description", ""),
+                    type_=visualization["type"],
+                    schema=visualization.get("schema", {}),
+                    function_id=func.id,
+                )
+                vis.save()
 
         return algorithm_output_schema.dump(algorithm, many=False), HTTPStatus.CREATED
 
 
 class Algorithm(AlgorithmStoreResources):
     """Resource for /algorithm/<id>"""
 
@@ -370,14 +405,16 @@
 
         # delete all subresources and finally the algorithm itself
         for function in algorithm.functions:
             for database in function.databases:
                 database.delete()
             for argument in function.arguments:
                 argument.delete()
+            for visualization in function.ui_visualizations:
+                visualization.delete()
             function.delete()
         algorithm.delete()
 
         return {"msg": f"Algorithm id={id} was successfully deleted"}, HTTPStatus.OK
 
     @with_permission(module_name, Operation.EDIT)
     def patch(self, id):
@@ -490,51 +527,56 @@
                 "msg": "Request body is incorrect",
                 "errors": errors,
             }, HTTPStatus.BAD_REQUEST
 
         fields = ["name", "description", "image", "partitioning", "vantage6_version"]
         for field in fields:
             if field in data and data.get(field) is not None:
-                setattr(algorithm, field, data.get("name"))
+                setattr(algorithm, field, data.get(field))
 
         if (functions := data.get("functions")) is not None:
             for function in algorithm.functions:
                 for argument in function.arguments:
                     argument.delete()
                 for db in function.databases:
                     db.delete()
+                for visualization in function.ui_visualizations:
+                    visualization.delete()
                 function.delete()
 
             for new_function in functions:
                 func = Function(
                     name=new_function["name"],
                     description=new_function.get("description", ""),
                     type_=new_function["type"],
                     algorithm_id=id,
                 )
                 func.save()
 
-                arguments = new_function.get("arguments")
-                if arguments:
-                    for argument in arguments:
-                        arg = Argument(
-                            name=argument["name"],
-                            description=argument.get("description", ""),
-                            type_=argument["type"],
-                            function_id=func.id,
-                        )
-                        arg.save()
-
-                # create the databases
-                databases = new_function.get("databases")
-                if databases:
-                    for database in databases:
-                        db = Database(
-                            name=database["name"],
-                            description=database.get("description", ""),
-                            function_id=func.id,
-                        )
-                        db.save()
+                for argument in new_function.get("arguments", []):
+                    arg = Argument(
+                        name=argument["name"],
+                        description=argument.get("description", ""),
+                        type_=argument["type"],
+                        function_id=func.id,
+                    )
+                    arg.save()
+                for database in new_function.get("databases", []):
+                    db = Database(
+                        name=database["name"],
+                        description=database.get("description", ""),
+                        function_id=func.id,
+                    )
+                    db.save()
+                for visualization in new_function.get("ui_visualizations", []):
+                    vis = UIVisualization(
+                        name=visualization["name"],
+                        description=visualization.get("description", ""),
+                        type_=visualization["type"],
+                        schema=visualization.get("schema", {}),
+                        function_id=func.id,
+                    )
+                    vis.save()
 
         algorithm.save()
 
         return algorithm_output_schema.dump(algorithm, many=False), HTTPStatus.OK
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/role.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/rule.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/schema/input_schema.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/schema/input_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from marshmallow import Schema, fields, ValidationError, validates
+from marshmallow import Schema, fields, ValidationError, validates, validates_schema
 from marshmallow.validate import Range
+from jsonschema import validate as json_validate
 
 from vantage6.algorithm.store.model.common.enums import (
     Partitioning,
     FunctionType,
     ArgumentType,
+    VisualizationType,
+)
+from vantage6.algorithm.store.model.common.ui_visualization_schemas import (
+    get_schema_for_visualization,
 )
 
 
 class _NameDescriptionSchema(Schema):
     """
     Schema for the name and description fields.
     """
@@ -40,19 +45,20 @@
 
 
 class FunctionInputSchema(_NameDescriptionSchema):
     """
     Schema for the input of a function.
     """
 
-    type = fields.String(required=True)
+    type_ = fields.String(required=True, data_key="type")
     databases = fields.Nested("DatabaseInputSchema", many=True)
     arguments = fields.Nested("ArgumentInputSchema", many=True)
+    ui_visualizations = fields.Nested("UIVisualizationInputSchema", many=True)
 
-    @validates("type")
+    @validates("type_")
     def validate_type(self, value):
         """
         Validate that the type is one of the allowed values.
         """
         types = [f.value for f in FunctionType]
         if value not in types:
             raise ValidationError(
@@ -70,28 +76,65 @@
 
 
 class ArgumentInputSchema(_NameDescriptionSchema):
     """
     Schema for the input of an argument.
     """
 
-    type = fields.String(required=True)
+    type_ = fields.String(required=True, data_key="type")
 
-    @validates("type")
+    @validates("type_")
     def validate_type(self, value):
         """
         Validate that the type is one of the allowed values.
         """
         types = [a.value for a in ArgumentType]
         if value not in types:
             raise ValidationError(
-                f"Argument type '{value}' is not one of the allowed values " f"{types}"
+                f"Argument type '{value}' is not one of the allowed values: {types}"
             )
 
 
+class UIVisualizationInputSchema(_NameDescriptionSchema):
+    """
+    Schema for the input of a UI visualization.
+    """
+
+    type_ = fields.String(required=True, data_key="type")
+    schema = fields.Dict()
+
+    @validates("type_")
+    def validate_type(self, value):
+        """
+        Validate that the type is one of the allowed values.
+        """
+        types = [v.value for v in VisualizationType]
+        if value not in types:
+            raise ValidationError(
+                f"UI visualization type '{value}' is not one of the allowed values "
+                f"{types}"
+            )
+
+    @validates_schema
+    def validate_schema(self, data, **kwargs):
+        """
+        Validate that the schema is a valid JSON schema.
+        """
+        schema = data.get("schema")
+        type_ = data.get("type_")
+        if schema and type_:
+            try:
+                json_validate(schema, get_schema_for_visualization(type_))
+            except Exception as exc:
+                raise ValidationError(
+                    "Schema does not match requirements for that visualization type: "
+                    f"{exc}",
+                ) from exc
+
+
 class UserInputSchema(Schema):
     """Schema for validating input for creating a user."""
 
     roles = fields.List(fields.Integer(validate=Range(min=1)))
     username = fields.String()
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/schema/output_schema.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/schema/output_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from vantage6.algorithm.store.model.algorithm import Algorithm
 from vantage6.algorithm.store.model.argument import Argument
 from vantage6.algorithm.store.model.database import Database
 from vantage6.algorithm.store.model.function import Function
 from vantage6.algorithm.store.model import Base
 from vantage6.algorithm.store.model.role import Role
 from vantage6.algorithm.store.model.rule import Rule
+from vantage6.algorithm.store.model.ui_visualization import UIVisualization
 from vantage6.algorithm.store.model.user import User
 from vantage6.algorithm.store.model.review import Review
 from vantage6.algorithm.store.model.vantage6_server import Vantage6Server
 
 
 # TODO: Remove duplicated code
 def create_one_to_many_link(obj: Base, link_to: str, link_from: str) -> str:
@@ -76,37 +77,47 @@
 
 
 class FunctionOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Function model"""
 
     class Meta:
         model = Function
-        exclude = ["type_"]
 
-    type = fields.String(attribute="type_")
+    type_ = fields.String(data_key="type")
 
     databases = fields.Nested("DatabaseOutputSchema", many=True, exclude=["id"])
     arguments = fields.Nested("ArgumentOutputSchema", many=True, exclude=["id"])
+    ui_visualizations = fields.Nested(
+        "UIVisualizationOutputSchema", many=True, exclude=["id"]
+    )
 
 
 class DatabaseOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Database model"""
 
     class Meta:
         model = Database
 
 
 class ArgumentOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Argument model"""
 
     class Meta:
         model = Argument
-        exclude = ["type_"]
 
-    type = fields.String(attribute="type_")
+    type_ = fields.String(data_key="type")
+
+
+class UIVisualizationOutputSchema(HATEOASModelSchema):
+    """Marshmallow output schema to serialize the UIVisualization model"""
+
+    class Meta:
+        model = UIVisualization
+
+    type_ = fields.String(data_key="type")
 
 
 class Vantage6ServerOutputSchema(HATEOASModelSchema):
     """Marshmallow output schema to serialize the Vantage6Server model"""
 
     class Meta:
         model = Vantage6Server
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/user.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/vantage6_server.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/vantage6_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6/algorithm/store/resource/version.py` & `vantage6-algorithm-store-4.4.0rc3/vantage6/algorithm/store/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/PKG-INFO` & `vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-store
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 algorithm store
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.3.4rc3 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-store Version: 4.4.0rc3 Summary:
 Vantage6 algorithm store Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-store-4.3.4rc3/vantage6_algorithm_store.egg-info/SOURCES.txt` & `vantage6-algorithm-store-4.4.0rc3/vantage6_algorithm_store.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 vantage6/algorithm/store/model/developer_algorithm_association.py
 vantage6/algorithm/store/model/function.py
 vantage6/algorithm/store/model/permission.py
 vantage6/algorithm/store/model/review.py
 vantage6/algorithm/store/model/role.py
 vantage6/algorithm/store/model/role_rule_association.py
 vantage6/algorithm/store/model/rule.py
+vantage6/algorithm/store/model/ui_visualization.py
 vantage6/algorithm/store/model/user.py
 vantage6/algorithm/store/model/vantage6_server.py
 vantage6/algorithm/store/model/common/enums.py
+vantage6/algorithm/store/model/common/ui_visualization_schemas.py
 vantage6/algorithm/store/resource/__init__.py
 vantage6/algorithm/store/resource/algorithm.py
 vantage6/algorithm/store/resource/role.py
 vantage6/algorithm/store/resource/rule.py
 vantage6/algorithm/store/resource/user.py
 vantage6/algorithm/store/resource/vantage6_server.py
 vantage6/algorithm/store/resource/version.py
```

