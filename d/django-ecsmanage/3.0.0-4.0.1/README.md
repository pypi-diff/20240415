# Comparing `tmp/django-ecsmanage-3.0.0.tar.gz` & `tmp/django_ecsmanage-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ecsmanage-3.0.0.tar", last modified: Mon Dec 18 19:52:53 2023, max compression
+gzip compressed data, was "django_ecsmanage-4.0.1.tar", last modified: Mon Apr 15 15:52:17 2024, max compression
```

## Comparing `django-ecsmanage-3.0.0.tar` & `django_ecsmanage-4.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.180065 django-ecsmanage-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2023-12-18 19:52:53.180065 django-ecsmanage-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2023-12-18 19:52:52.000000 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-18 19:52:53.000000 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 19:52:53.000000 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-18 19:52:53.000000 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-18 19:52:53.000000 django-ecsmanage-3.0.0/django_ecsmanage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/ecsmanage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/ecsmanage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/ecsmanage/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/ecsmanage/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/ecsmanage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/ecsmanage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/ecsmanage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/ecsmanage/management/commands/ecsmanage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1038 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/scripts/test
--rwxr-xr-x   0 runner    (1001) docker     (127)      700 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/scripts/update
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-18 19:52:53.180065 django-ecsmanage-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:53.176066 django-ecsmanage-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/tests/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-12-18 19:52:40.000000 django-ecsmanage-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.806401 django_ecsmanage-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-04-15 15:52:17.806401 django_ecsmanage-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.806401 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-04-15 15:52:17.000000 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-15 15:52:17.000000 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:52:17.000000 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 15:52:17.000000 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 15:52:17.000000 django_ecsmanage-4.0.1/django_ecsmanage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/ecsmanage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/ecsmanage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/ecsmanage/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/ecsmanage/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/ecsmanage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/ecsmanage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/ecsmanage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/ecsmanage/management/commands/ecsmanage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.802401 django_ecsmanage-4.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1038 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/scripts/test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      700 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/scripts/update
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 15:52:17.806401 django_ecsmanage-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:17.806401 django_ecsmanage-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/tests/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 15:52:08.000000 django_ecsmanage-4.0.1/tox.ini
```

### Comparing `django-ecsmanage-3.0.0/.github/workflows/continuous_integration.yml` & `django_ecsmanage-4.0.1/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/.github/workflows/release.yml` & `django_ecsmanage-4.0.1/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,30 @@
     tags:
       - "*"
 
 jobs:
   release:
     name: release
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
     steps:
       - name: Checkout commit and fetch tag history
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.x
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
 
       - name: Install release dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools wheel twine
+          pip install setuptools wheel
 
-      - name: Build and publish package
-        env:
-          TWINE_USERNAME: ${{ secrets.PYPI_AZAVEA_USERNAME }}
-          TWINE_PASSWORD: ${{ secrets.PYPI_AZAVEA_PASSWORD }}
-        run: |
-          python setup.py sdist bdist_wheel
-          twine upload dist/*
+      - name: Build package
+        run: python setup.py sdist bdist_wheel
+
+      - name: Upload release to TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `django-ecsmanage-3.0.0/.gitignore` & `django_ecsmanage-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/CHANGELOG.md` & `django_ecsmanage-4.0.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [4.0.1] - 2024-04-15
+### Changed
+- Update PyPI Integration for Publishing [#36](https://github.com/azavea/django-ecsmanage/issues/36)
+
+## [4.0.0] - 2024-01-05
+### Changed
+- Return task ARN from the handle command [#34](https://github.com/azavea/django-ecsmanage/pull/34)
+
 ## [3.0.0] - 2023-12-18
 ### Added
 - Add support for Django 3.2, 4.2, 5.0 [#33](https://github.com/azavea/django-ecsmanage/pull/33)
 
 ### Changed
 - Support default network modes [#33](https://github.com/azavea/django-ecsmanage/pull/33)
 - Upgrade CI to use newer GitHub Actions for `checkout` and `setup-python` [#33](https://github.com/azavea/django-ecsmanage/pull/33)
@@ -66,15 +74,16 @@
 - Fixed reference to taskDefinition in describe_task_definition response [#5](https://github.com/azavea/django-ecsmanage/pull/5)
 
 ## [0.1.0] - 2019-04-10
 ### Added
 - Update PyPi credentials [#4](https://github.com/azavea/django-ecsmanage/pull/4)
 - Initialize Django module for one-off management commands [#2](https://github.com/azavea/django-ecsmanage/pull/2)
 
-[Unreleased]: https://github.com/azavea/django-ecsmanage/compare/3.0.0...HEAD
+[Unreleased]: https://github.com/azavea/django-ecsmanage/compare/4.0.0...HEAD
+[4.0.0]: https://github.com/azavea/django-ecsmanage/compare/3.0.0...4.0.0
 [3.0.0]: https://github.com/azavea/django-ecsmanage/compare/2.0.1...3.0.0
 [2.0.1]: https://github.com/azavea/django-ecsmanage/compare/2.0.0...2.0.1
 [2.0.0]: https://github.com/azavea/django-ecsmanage/compare/1.1.0...2.0.0
 [1.1.0]: https://github.com/:azavea/django-ecsmanage/compare/1.0.1...1.1.0
 [1.0.1]: https://github.com/:azavea/django-ecsmanage/compare/1.0.0...1.0.1
 [1.0.0]: https://github.com/azavea/django-ecsmanage/compare/0.1.0...1.0.0
 [0.1.0]: https://github.com/azavea/django-ecsmanage/releases/tag/0.1.0
```

### Comparing `django-ecsmanage-3.0.0/LICENSE` & `django_ecsmanage-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/PKG-INFO` & `django_ecsmanage-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ecsmanage
-Version: 3.0.0
+Version: 4.0.1
 Summary: Run any Django management command on an AWS Elastic Container Service (ECS) cluster.
 Home-page: https://github.com/azavea/django-ecsmanage/
 Author: Azavea, Inc.
 Author-email: systems@azavea.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-ecsmanage-3.0.0/README.rst` & `django_ecsmanage-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/django_ecsmanage.egg-info/PKG-INFO` & `django_ecsmanage-4.0.1/django_ecsmanage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ecsmanage
-Version: 3.0.0
+Version: 4.0.1
 Summary: Run any Django management command on an AWS Elastic Container Service (ECS) cluster.
 Home-page: https://github.com/azavea/django-ecsmanage/
 Author: Azavea, Inc.
 Author-email: systems@azavea.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-ecsmanage-3.0.0/django_ecsmanage.egg-info/SOURCES.txt` & `django_ecsmanage-4.0.1/django_ecsmanage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/ecsmanage/management/commands/ecsmanage.py` & `django_ecsmanage-4.0.1/ecsmanage/management/commands/ecsmanage.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             nargs=REMAINDER,
             help="Command override for the ECS container (e.g. 'migrate')",
         )
 
     def handle(self, *args, **options):
         """
         Run the given command on the latest app CLI task definition and print
-        out a URL to view the status.
+        out a URL to view the status. Returns the task ARN of the started task.
         """
         self.env = options["env"]
         cmd = options["cmd"]
 
         config = self.parse_config()
 
         aws_region = config["AWS_REGION"]
@@ -41,27 +41,37 @@
         self.ecs_client = boto3.client("ecs", region_name=aws_region)
         self.ec2_client = boto3.client("ec2", region_name=aws_region)
 
         task_def_arn = self.get_task_def(config["TASK_DEFINITION_NAME"])
         security_group_id = self.get_security_group(config["SECURITY_GROUP_TAGS"])
         subnet_id = self.get_subnet(config["SUBNET_TAGS"])
 
-        task_id = self.run_task(config, task_def_arn, security_group_id, subnet_id, cmd)
+        task_arn = self.run_task(config, task_def_arn, security_group_id, subnet_id, cmd)
+
+        # Task ARNs have at least two formats:
+        #
+        #  - Old: arn:aws:ecs:region:aws_account_id:task/task-id
+        #  - New: arn:aws:ecs:region:aws_account_id:task/cluster-name/task-id
+        #
+        # See: https://docs.aws.amazon.com/AmazonECS/latest/userguide/ecs-account-settings.html#ecs-resource-ids  # NOQA
+        task_id = task_arn.split("/")[-1]
 
         cluster_name = config["CLUSTER_NAME"]
 
         url = (
             f"https://console.aws.amazon.com/ecs/home?region={aws_region}#"
             f"/clusters/{cluster_name}/tasks/{task_id}/details"  # NOQA
         )
 
         self.stdout.write(
             self.style.SUCCESS(f"Task started! View here:\n{url}")
         )  # NOQA
 
+        return task_arn
+
     def parse_config(self):
         """
         Parse configuration settings for the app, checking to make sure that
         they're valid.
         """
         if getattr(settings, "ECSMANAGE_ENVIRONMENTS") is None:
             raise CommandError(
@@ -161,15 +171,15 @@
 
         subnet = self.parse_response(subnet_response, "Subnets", 0)
         return subnet["SubnetId"]
 
     def run_task(self, config, task_def_arn, security_group_id, subnet_id, cmd):
         """
         Run a task for a given task definition ARN using the given security
-        group and subnets, and return the task ID.
+        group and subnets, and return the task ARN of the started task.
         """
         task_def = self.ecs_client.describe_task_definition(
             taskDefinition=task_def_arn
         )["taskDefinition"]
 
         kwargs = {
             "cluster": config["CLUSTER_NAME"],
@@ -196,15 +206,8 @@
 
         # Setting platformVersion of only relevant if launchType is FARGATE.
         if config["LAUNCH_TYPE"] == "FARGATE":
             kwargs["platformVersion"] = config["PLATFORM_VERSION"]
 
         task = self.parse_response(self.ecs_client.run_task(**kwargs), "tasks", 0)
 
-        # Task ARNs have at least two formats:
-        #
-        #  - Old: arn:aws:ecs:region:aws_account_id:task/task-id
-        #  - New: arn:aws:ecs:region:aws_account_id:task/cluster-name/task-id
-        #
-        # See: https://docs.aws.amazon.com/AmazonECS/latest/userguide/ecs-account-settings.html#ecs-resource-ids  # NOQA
-        task_id = task["taskArn"].split("/")[-1]
-        return task_id
+        return task["taskArn"]
```

### Comparing `django-ecsmanage-3.0.0/scripts/test` & `django_ecsmanage-4.0.1/scripts/test`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/scripts/update` & `django_ecsmanage-4.0.1/scripts/update`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/setup.cfg` & `django_ecsmanage-4.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/tests/test_configuration.py` & `django_ecsmanage-4.0.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `django-ecsmanage-3.0.0/tox.ini` & `django_ecsmanage-4.0.1/tox.ini`

 * *Files identical despite different names*

