# Comparing `tmp/microsoft_kiota_serialization_json-1.1.0.tar.gz` & `tmp/microsoft_kiota_serialization_json-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_serialization_json-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_serialization_json-1.1.0.tar` & `microsoft_kiota_serialization_json-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       82 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      619 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      605 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      240 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2617 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/policies/resourceManagement.yml
--rw-r--r--   0        0        0      514 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      792 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1121 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2538 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1324 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1357 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.gitignore
--rw-r--r--   0        0        0    15976 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/.pylintrc
--rw-r--r--   0        0        0     1963 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      444 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/LICENSE
--rw-r--r--   0        0        0    71086 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/Pipfile.lock
--rw-r--r--   0        0        0     2545 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/README.md
--rw-r--r--   0        0        0     2757 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/SECURITY.md
--rw-r--r--   0        0        0     1244 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/SUPPORT.md
--rw-r--r--   0        0        0      119 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    12082 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1410 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    19300 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1268 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      795 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/requirements-dev.txt
--rw-r--r--   0        0        0        0 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      119 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1569 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/entity.py
--rw-r--r--   0        0        0     2692 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/intersection_type.py
--rw-r--r--   0        0        0       94 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/office_location.py
--rw-r--r--   0        0        0     3077 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/union_type.py
--rw-r--r--   0        0        0     3133 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/user.py
--rw-r--r--   0        0        0     2169 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/helpers/user2.py
--rw-r--r--   0        0        0        0 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     2062 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/conftest.py
--rw-r--r--   0        0        0     5236 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_intersection_wrapper.py
--rw-r--r--   0        0        0     4900 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1679 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0    11445 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1018 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     5873 2024-03-05 00:45:36.003411 microsoft_kiota_serialization_json-1.1.0/tests/unit/test_union_wrapper.py
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      619 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      605 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      240 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2617 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/policies/resourceManagement.yml
+-rw-r--r--   0        0        0      514 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      792 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1121 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1324 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1357 2024-04-15 13:08:19.874150 microsoft_kiota_serialization_json-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/.gitignore
+-rw-r--r--   0        0        0    15976 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/.pylintrc
+-rw-r--r--   0        0        0     2096 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/LICENSE
+-rw-r--r--   0        0        0    71086 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/README.md
+-rw-r--r--   0        0        0     2757 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/SECURITY.md
+-rw-r--r--   0        0        0     1244 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/SUPPORT.md
+-rw-r--r--   0        0        0      119 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    12021 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1410 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    19300 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1268 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      794 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1569 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/entity.py
+-rw-r--r--   0        0        0     2692 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/intersection_type.py
+-rw-r--r--   0        0        0       94 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     3077 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/union_type.py
+-rw-r--r--   0        0        0     3133 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/user.py
+-rw-r--r--   0        0        0     2169 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/helpers/user2.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2062 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     5236 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_intersection_wrapper.py
+-rw-r--r--   0        0        0     5123 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1679 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0    11445 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1018 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     5873 2024-04-15 13:08:19.878150 microsoft_kiota_serialization_json-1.2.0/tests/unit/test_union_wrapper.py
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-1.2.0/PKG-INFO
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `microsoft_kiota_serialization_json-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `microsoft_kiota_serialization_json-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/policies/resourceManagement.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/policies/resourceManagement.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/pull_request_template.md` & `microsoft_kiota_serialization_json-1.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/workflows/auto-merge-dependabot.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.6.0
+        uses: dependabot/fetch-metadata@v2.0.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/workflows/build.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.github/workflows/publish.yml` & `microsoft_kiota_serialization_json-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.gitignore` & `microsoft_kiota_serialization_json-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/.pylintrc` & `microsoft_kiota_serialization_json-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/CHANGELOG.md` & `microsoft_kiota_serialization_json-1.2.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.0] - 2024-04-09
+
+### Added
+
+### Changed
+- Enhanced error handling: Enabled silent failure when an enum key is not available
+
 ## [1.1.0] - 2024-02-29
 
 ### Added
 
 ### Changed
 - Support objects and collections when writing additional data.
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/LICENSE` & `microsoft_kiota_serialization_json-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/Pipfile.lock` & `microsoft_kiota_serialization_json-1.2.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/README.md` & `microsoft_kiota_serialization_json-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/SECURITY.md` & `microsoft_kiota_serialization_json-1.2.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/SUPPORT.md` & `microsoft_kiota_serialization_json-1.2.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_parse_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             camel_case_key = "None_"
         else:
             camel_case_key = raw_key[0].upper() + raw_key[1:]
 
         try:
             return enum_class[camel_case_key]  # type: ignore
         except KeyError:
-            raise Exception(f'Invalid key: {camel_case_key} for enum {enum_class}.')
+            return None
 
     def get_object_value(self, factory: ParsableFactory) -> U:
         """Gets the model object value of the node
         Returns:
             Parsable: The model object value of the node
         """
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-1.2.0/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/pyproject.toml` & `microsoft_kiota_serialization_json-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/requirements-dev.txt` & `microsoft_kiota_serialization_json-1.2.0/requirements-dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,77 +2,77 @@
 
 astroid==3.1.0
 
 certifi==2024.2.2
 
 charset-normalizer==3.3.2
 
-coverage[toml]==7.4.3
+coverage[toml]==7.4.4
 
 dill==0.3.8
 
 docutils==0.20.1
 
 flit==3.9.0
 
 flit-core==3.9.0
 
-idna==3.6
+idna==3.7
 
 importlib-metadata==6.8.0 ; python_version >= '3.8'
 
 iniconfig==2.0.0
 
 isort==5.13.2
 
 lazy-object-proxy==1.10.0
 
 mccabe==0.7.0
 
-mypy==1.8.0
+mypy==1.9.0
 
 mypy-extensions==1.0.0
 
-packaging==23.2
+packaging==24.0
 
 platformdirs==4.2.0
 
 pluggy==1.4.0
 
 pylint==3.1.0
 
-pytest==8.1.0
+pytest==8.1.1
 
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 
 requests==2.31.0
 
 toml==0.10.2
 
 tomli==2.0.1
 
 tomlkit==0.12.4
 
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
 
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 
 urllib3==2.2.1
 
 wrapt==1.16.0
 
 yapf==0.40.2
 
-zipp==3.17.0 ; python_version >= '3.8'
+zipp==3.18.1 ; python_version >= '3.8'
 
 colorama==0.4.6
 
 exceptiongroup==1.2.0
 
-microsoft-kiota-abstractions==1.3.0
+microsoft-kiota-abstractions==1.3.2
 
 pendulum==3.0.0
 
 six==1.16.0
 
 uritemplate==4.1.1
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-1.2.0/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/helpers/intersection_type.py` & `microsoft_kiota_serialization_json-1.2.0/tests/helpers/intersection_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/helpers/union_type.py` & `microsoft_kiota_serialization_json-1.2.0/tests/helpers/union_type.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/helpers/user.py` & `microsoft_kiota_serialization_json-1.2.0/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/helpers/user2.py` & `microsoft_kiota_serialization_json-1.2.0/tests/helpers/user2.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/conftest.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_intersection_wrapper.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_intersection_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_parse_node.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_parse_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,37 +95,48 @@
 def test_get_enum_value():
     parse_node = JsonParseNode("dunhill")
     result = parse_node.get_enum_value(OfficeLocation)
     assert isinstance(result, OfficeLocation)
     assert result == OfficeLocation.Dunhill
 
 
+def test_get_enum_value_for_key_not_found():
+    parse_node = JsonParseNode("whitehouse")
+    result = parse_node.get_enum_value(OfficeLocation)
+    assert result is None
+
+
 def test_get_object_value(user1_json):
     parse_node = JsonParseNode(json.loads(user1_json))
     result = parse_node.get_object_value(User)
     assert isinstance(result, User)
     assert result.id == UUID("8f841f30-e6e3-439a-a812-ebd369559c36")
     assert result.office_location == OfficeLocation.Dunhill
     assert isinstance(result.updated_at, datetime)
     assert isinstance(result.birthday, date)
     assert result.business_phones == ["+1 205 555 0108"]
     assert result.is_active is True
     assert result.mobile_phone is None
-    assert result.additional_data["additional_data"]["@odata.context"] == "https://graph.microsoft.com/v1.0/$metadata#users/$entity"
+    assert result.additional_data["additional_data"][
+        "@odata.context"] == "https://graph.microsoft.com/v1.0/$metadata#users/$entity"
     assert result.additional_data["additional_data"]["manager"] == {
         "id": UUID('8f841f30-e6e3-439a-a812-ebd369559c36'),
-        "updated_at": DateTime(2022, 1, 27, 12, 59, 45, 596117, tzinfo=FixedTimezone(0, name="+00:00")),
-        "is_active": True}
+        "updated_at":
+        DateTime(2022, 1, 27, 12, 59, 45, 596117, tzinfo=FixedTimezone(0, name="+00:00")),
+        "is_active": True
+    }
     assert result.additional_data["additional_data"]["approvers"] == [
         {
-            "id": UUID('8f841f30-e6e3-439a-a812-ebd369559c36'),
-            "updated_at": DateTime(2022, 1, 27, 12, 59, 45, 596117, tzinfo=FixedTimezone(0, name="+00:00")),
-            "is_active": True
-        },
-        {
+            "id":
+            UUID('8f841f30-e6e3-439a-a812-ebd369559c36'),
+            "updated_at":
+            DateTime(2022, 1, 27, 12, 59, 45, 596117, tzinfo=FixedTimezone(0, name="+00:00")),
+            "is_active":
+            True
+        }, {
             "display_name": "John Doe",
             "age": 32
         }
     ]
 
 
 def test_get_collection_of_object_values(users_json):
```

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/tests/unit/test_union_wrapper.py` & `microsoft_kiota_serialization_json-1.2.0/tests/unit/test_union_wrapper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-1.1.0/PKG-INFO` & `microsoft_kiota_serialization_json-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 1.1.0
+Version: 1.2.0
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

