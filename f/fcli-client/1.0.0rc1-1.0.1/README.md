# Comparing `tmp/fcli_client-1rc1.tar.gz` & `tmp/fcli_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcli_client-1rc1.tar", last modified: Fri Apr 12 18:48:07 2024, max compression
+gzip compressed data, was "fcli_client-1.0.1.tar", last modified: Mon Apr 15 19:18:07 2024, max compression
```

## Comparing `fcli_client-1rc1.tar` & `fcli_client-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:48:07.447929 fcli_client-1rc1/
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     1068 2023-11-25 20:33:36.000000 fcli_client-1rc1/LICENSE
--rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3777 2024-04-12 18:48:07.443930 fcli_client-1rc1/PKG-INFO
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     3147 2024-03-31 17:16:45.000000 fcli_client-1rc1/README.md
-drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:48:07.443930 fcli_client-1rc1/fcli_client.egg-info/
--rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3777 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/PKG-INFO
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      206 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/SOURCES.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/dependency_links.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       31 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/requires.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/top_level.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      673 2024-04-12 18:46:28.000000 fcli_client-1rc1/pyproject.toml
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       38 2024-04-12 18:48:07.447929 fcli_client-1rc1/setup.cfg
+drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-15 19:18:07.835371 fcli_client-1.0.1/
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     1068 2023-11-25 20:33:36.000000 fcli_client-1.0.1/LICENSE
+-rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3363 2024-04-15 19:18:07.835371 fcli_client-1.0.1/PKG-INFO
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     2736 2024-04-12 19:00:56.000000 fcli_client-1.0.1/README.md
+drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-15 19:18:07.835371 fcli_client-1.0.1/fcli_client.egg-info/
+-rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3363 2024-04-15 19:18:07.000000 fcli_client-1.0.1/fcli_client.egg-info/PKG-INFO
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      206 2024-04-15 19:18:07.000000 fcli_client-1.0.1/fcli_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-15 19:18:07.000000 fcli_client-1.0.1/fcli_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       31 2024-04-15 19:18:07.000000 fcli_client-1.0.1/fcli_client.egg-info/requires.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-15 19:18:07.000000 fcli_client-1.0.1/fcli_client.egg-info/top_level.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      670 2024-04-15 19:17:39.000000 fcli_client-1.0.1/pyproject.toml
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       38 2024-04-15 19:18:07.835371 fcli_client-1.0.1/setup.cfg
```

### Comparing `fcli_client-1rc1/LICENSE` & `fcli_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fcli_client-1rc1/PKG-INFO` & `fcli_client-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcli-client
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: A workflow oriented, command line Mastodon client
 Author-email: Phil Cowans <phil-fcli@philcowans.com>
 Project-URL: Homepage, https://github.com/philcowans/fcli
 Project-URL: Issues, https://github.com/philcowans/fcli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,54 +71,31 @@
 Finally, you'll need to create some directories to store state:
 
 ```
 {$HOME}/.fcli/cache
 {$HOME}/.fcli/outbox
 {$HOME}/.fcli/processed/actionable
 {$HOME}/.fcli/processed/actioned
+{$HOME}/.fcli/processed/boostable
+{$HOME}/.fcli/processed/boosted
 {$HOME}/.fcli/processed/interesting
 {$HOME}/.fcli/processed/not_interesting
 {$HOME}/.fcli/processed/skipped
 {$HOME}/.fcli/sent
 {$HOME}/.fcli/staging
 ```
 
 There are probably other things you need to do - my isntallation has evolved
 with the codebase, so let me know if you run into any problems.
 
 ## Usage
 
-First of all, sync the local state with the server:
+Kick off the workflow using the default entry point:
 
 ```
-python -m fcli sync
+python -m fcli
 ```
 
 You'll be asked to authenticate via an OAuth 2.0 code. This step will also post
-the content of any files in `{$HOME}/.fcli/outbox`. Once you've done this, you
-can start the review workflow:
+the content of any files in `{$HOME}/.fcli/outbox`.
 
-```
-python -m fcli review
-```
-
-Finally, upload any actionable posts as inbox items in Everdo. Make sure the
-Everdo API is up when you run this step:
-
-```
-python -m fcli actions
-```
-
-You'll also need to manually move some files around:
-
-```
-mv ~/.fcli/processed/actionable/* ~/.fcli/processed/actioned/
-mv ~/.fcli/cache/* ~/.fcli/processed/skipped/
-```
-
-Finally, update the stats databases ussed by the algorithm:
-
-```
-python -m fcli stats
-```
-
-At somepoint soon I'll combine these steps into a single workflow.
+There are a few command line options you'll find if you look at the code, but they're obsolete.
```

### Comparing `fcli_client-1rc1/README.md` & `fcli_client-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -52,54 +52,31 @@
 Finally, you'll need to create some directories to store state:
 
 ```
 {$HOME}/.fcli/cache
 {$HOME}/.fcli/outbox
 {$HOME}/.fcli/processed/actionable
 {$HOME}/.fcli/processed/actioned
+{$HOME}/.fcli/processed/boostable
+{$HOME}/.fcli/processed/boosted
 {$HOME}/.fcli/processed/interesting
 {$HOME}/.fcli/processed/not_interesting
 {$HOME}/.fcli/processed/skipped
 {$HOME}/.fcli/sent
 {$HOME}/.fcli/staging
 ```
 
 There are probably other things you need to do - my isntallation has evolved
 with the codebase, so let me know if you run into any problems.
 
 ## Usage
 
-First of all, sync the local state with the server:
+Kick off the workflow using the default entry point:
 
 ```
-python -m fcli sync
+python -m fcli
 ```
 
 You'll be asked to authenticate via an OAuth 2.0 code. This step will also post
-the content of any files in `{$HOME}/.fcli/outbox`. Once you've done this, you
-can start the review workflow:
+the content of any files in `{$HOME}/.fcli/outbox`.
 
-```
-python -m fcli review
-```
-
-Finally, upload any actionable posts as inbox items in Everdo. Make sure the
-Everdo API is up when you run this step:
-
-```
-python -m fcli actions
-```
-
-You'll also need to manually move some files around:
-
-```
-mv ~/.fcli/processed/actionable/* ~/.fcli/processed/actioned/
-mv ~/.fcli/cache/* ~/.fcli/processed/skipped/
-```
-
-Finally, update the stats databases ussed by the algorithm:
-
-```
-python -m fcli stats
-```
-
-At somepoint soon I'll combine these steps into a single workflow.
+There are a few command line options you'll find if you look at the code, but they're obsolete.
```

### Comparing `fcli_client-1rc1/fcli_client.egg-info/PKG-INFO` & `fcli_client-1.0.1/fcli_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcli-client
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: A workflow oriented, command line Mastodon client
 Author-email: Phil Cowans <phil-fcli@philcowans.com>
 Project-URL: Homepage, https://github.com/philcowans/fcli
 Project-URL: Issues, https://github.com/philcowans/fcli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -71,54 +71,31 @@
 Finally, you'll need to create some directories to store state:
 
 ```
 {$HOME}/.fcli/cache
 {$HOME}/.fcli/outbox
 {$HOME}/.fcli/processed/actionable
 {$HOME}/.fcli/processed/actioned
+{$HOME}/.fcli/processed/boostable
+{$HOME}/.fcli/processed/boosted
 {$HOME}/.fcli/processed/interesting
 {$HOME}/.fcli/processed/not_interesting
 {$HOME}/.fcli/processed/skipped
 {$HOME}/.fcli/sent
 {$HOME}/.fcli/staging
 ```
 
 There are probably other things you need to do - my isntallation has evolved
 with the codebase, so let me know if you run into any problems.
 
 ## Usage
 
-First of all, sync the local state with the server:
+Kick off the workflow using the default entry point:
 
 ```
-python -m fcli sync
+python -m fcli
 ```
 
 You'll be asked to authenticate via an OAuth 2.0 code. This step will also post
-the content of any files in `{$HOME}/.fcli/outbox`. Once you've done this, you
-can start the review workflow:
+the content of any files in `{$HOME}/.fcli/outbox`.
 
-```
-python -m fcli review
-```
-
-Finally, upload any actionable posts as inbox items in Everdo. Make sure the
-Everdo API is up when you run this step:
-
-```
-python -m fcli actions
-```
-
-You'll also need to manually move some files around:
-
-```
-mv ~/.fcli/processed/actionable/* ~/.fcli/processed/actioned/
-mv ~/.fcli/cache/* ~/.fcli/processed/skipped/
-```
-
-Finally, update the stats databases ussed by the algorithm:
-
-```
-python -m fcli stats
-```
-
-At somepoint soon I'll combine these steps into a single workflow.
+There are a few command line options you'll find if you look at the code, but they're obsolete.
```

### Comparing `fcli_client-1rc1/pyproject.toml` & `fcli_client-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fcli-client"
-version = "1.0.0rc1"
+version = "1.0.1"
 authors = [
   { name="Phil Cowans", email="phil-fcli@philcowans.com" },
 ]
 description = "A workflow oriented, command line Mastodon client"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

