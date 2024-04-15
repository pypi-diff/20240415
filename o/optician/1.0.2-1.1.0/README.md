# Comparing `tmp/optician-1.0.2.tar.gz` & `tmp/optician-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optician-1.0.2.tar", max compression
+gzip compressed data, was "optician-1.1.0.tar", max compression
```

## Comparing `optician-1.0.2.tar` & `optician-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-04-12 14:52:15.821613 optician-1.0.2/LICENSE
--rw-r--r--   0        0        0     9317 2024-04-12 14:52:15.821953 optician-1.0.2/README.md
--rw-r--r--   0        0        0     1289 2024-04-15 09:36:03.228785 optician-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       76 2023-11-29 17:40:14.310907 optician-1.0.2/src/optician/__main__.py
--rw-r--r--   0        0        0        0 2023-11-29 17:40:14.311039 optician-1.0.2/src/optician/cli/__init__.py
--rw-r--r--   0        0        0     7146 2024-04-03 13:48:52.141182 optician-1.0.2/src/optician/cli/commands.py
--rw-r--r--   0        0        0       25 2023-11-29 17:40:14.311431 optician-1.0.2/src/optician/db_client/__init__.py
--rw-r--r--   0        0        0     5688 2024-04-03 13:48:52.141698 optician-1.0.2/src/optician/db_client/db_client.py
--rw-r--r--   0        0        0       28 2023-11-29 17:40:14.311780 optician-1.0.2/src/optician/diff_tracker/__init__.py
--rw-r--r--   0        0        0     1860 2024-04-03 13:48:52.142156 optician-1.0.2/src/optician/diff_tracker/diff_tracker.py
--rw-r--r--   0        0        0     1804 2024-04-03 13:48:52.142496 optician-1.0.2/src/optician/logger.py
--rw-r--r--   0        0        0       32 2023-11-29 17:40:14.312115 optician-1.0.2/src/optician/lookml_generator/__init__.py
--rw-r--r--   0        0        0    11114 2024-04-03 13:48:52.142973 optician-1.0.2/src/optician/lookml_generator/lookml_generator.py
--rw-r--r--   0        0        0       25 2023-11-29 17:40:14.312533 optician-1.0.2/src/optician/vc_client/__init__.py
--rw-r--r--   0        0        0     5112 2024-04-03 13:48:52.143444 optician-1.0.2/src/optician/vc_client/vc_client.py
--rw-r--r--   0        0        0    10574 1970-01-01 00:00:00.000000 optician-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 14:52:15.821613 optician-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9319 2024-04-15 10:47:15.590912 optician-1.1.0/README.md
+-rw-r--r--   0        0        0     1298 2024-04-15 10:51:41.003174 optician-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-11-29 17:40:14.310907 optician-1.1.0/src/optician/__main__.py
+-rw-r--r--   0        0        0        0 2023-11-29 17:40:14.311039 optician-1.1.0/src/optician/cli/__init__.py
+-rw-r--r--   0        0        0     7146 2024-04-03 13:48:52.141182 optician-1.1.0/src/optician/cli/commands.py
+-rw-r--r--   0        0        0       25 2023-11-29 17:40:14.311431 optician-1.1.0/src/optician/db_client/__init__.py
+-rw-r--r--   0        0        0     5688 2024-04-03 13:48:52.141698 optician-1.1.0/src/optician/db_client/db_client.py
+-rw-r--r--   0        0        0       28 2023-11-29 17:40:14.311780 optician-1.1.0/src/optician/diff_tracker/__init__.py
+-rw-r--r--   0        0        0     1860 2024-04-03 13:48:52.142156 optician-1.1.0/src/optician/diff_tracker/diff_tracker.py
+-rw-r--r--   0        0        0     1804 2024-04-03 13:48:52.142496 optician-1.1.0/src/optician/logger.py
+-rw-r--r--   0        0        0       32 2023-11-29 17:40:14.312115 optician-1.1.0/src/optician/lookml_generator/__init__.py
+-rw-r--r--   0        0        0    11114 2024-04-03 13:48:52.142973 optician-1.1.0/src/optician/lookml_generator/lookml_generator.py
+-rw-r--r--   0        0        0       25 2023-11-29 17:40:14.312533 optician-1.1.0/src/optician/vc_client/__init__.py
+-rw-r--r--   0        0        0     5112 2024-04-03 13:48:52.143444 optician-1.1.0/src/optician/vc_client/vc_client.py
+-rw-r--r--   0        0        0    10603 1970-01-01 00:00:00.000000 optician-1.1.0/PKG-INFO
```

### Comparing `optician-1.0.2/LICENSE` & `optician-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/README.md` & `optician-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation
 
 You can install optician from a PyPi repository. We suggest you install it into a virtual environment.
 Please specify which database (or databases) you will be using, as in the example below.
 
 ```shell
-pip install optician[bigquery]
+pip install "optician[bigquery]"
 ```
 
 ## Setup
 1. Create the Optician configuration file `.optician/config.json` (you can name it another way) somewhere in your computer (we suggest inside the dbt or Looker repo)
 2. Create the environment variable `OPTICIAN_CONFIG_FILE` which will be the absolute path to the file created in 1
 3. You need to be able to connect to your database. For BigQuery, you can connect either by Oauth or Service Account.
 4. [Optional] Create an environment variable `GH_TOKEN` for your GitHub personal token. You need to create this token in [GitHub](https://github.com/settings/tokens) with read:project, repo, user:email permissions. This will allow you to commit your Looker views directly to the Looker repository.
```

### Comparing `optician-1.0.2/pyproject.toml` & `optician-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [tool.poetry]
 name = "optician"
-version = "1.0.2"
+version = "1.1.0"
 description = "Sync your data warehouse tables to Looker"
 authors = [
     "GetGround <bi@getground.co.uk>"
 ]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/getground/optician"
@@ -22,19 +22,19 @@
 
 [project.urls]
 Homepage = "https://github.com/getground/optician"
 
 [tool.poetry.dependencies]
 # These packages are mandatory
 python = "^3.9"
-PyGithub = "^1.59.0"
+PyGithub = "^2.3.0"
 # The packages are optional dependencies
-google-cloud-bigquery = {version = "3.*", optional = true }
-psycopg2 = {version = "2.*", optional = true}
-snowflake-connector-python = {version = "3.*", optional = true}
+google-cloud-bigquery = {version = "^3.10.0", optional = true }
+psycopg2 = {version = "^2.9.9", optional = true}
+snowflake-connector-python = {version = "^3.8.1", optional = true}
 
 [tool.poetry.extras]
 bigquery = ["google-cloud-bigquery"]
 redshift = ["psycopg2"]
 postgres = ["psycopg2"]
 snowflake = ["snowflake-connector-python"]
```

### Comparing `optician-1.0.2/src/optician/cli/commands.py` & `optician-1.1.0/src/optician/cli/commands.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/src/optician/db_client/db_client.py` & `optician-1.1.0/src/optician/db_client/db_client.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/src/optician/diff_tracker/diff_tracker.py` & `optician-1.1.0/src/optician/diff_tracker/diff_tracker.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/src/optician/logger.py` & `optician-1.1.0/src/optician/logger.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/src/optician/lookml_generator/lookml_generator.py` & `optician-1.1.0/src/optician/lookml_generator/lookml_generator.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/src/optician/vc_client/vc_client.py` & `optician-1.1.0/src/optician/vc_client/vc_client.py`

 * *Files identical despite different names*

### Comparing `optician-1.0.2/PKG-INFO` & `optician-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optician
-Version: 1.0.2
+Version: 1.1.0
 Summary: Sync your data warehouse tables to Looker
 Home-page: https://github.com/getground/optician
 License: MIT
 Keywords: optician,looker,sync,lookml,dbt,data warehouse
 Author: GetGround
 Author-email: bi@getground.co.uk
 Requires-Python: >=3.9,<4.0
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: bigquery
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
-Requires-Dist: PyGithub (>=1.59.0,<2.0.0)
-Requires-Dist: google-cloud-bigquery (==3.*) ; extra == "bigquery"
-Requires-Dist: psycopg2 (==2.*) ; extra == "redshift" or extra == "postgres"
-Requires-Dist: snowflake-connector-python (==3.*) ; extra == "snowflake"
+Requires-Dist: PyGithub (>=2.3.0,<3.0.0)
+Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0) ; extra == "bigquery"
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0) ; extra == "redshift" or extra == "postgres"
+Requires-Dist: snowflake-connector-python (>=3.8.1,<4.0.0) ; extra == "snowflake"
 Project-URL: Repository, https://github.com/getground/optician
 Description-Content-Type: text/markdown
 
 # Optician
 Optician automatically generates your LookML views from your database models.
 
 Optician was created at [GetGround](https://www.getground.co.uk/), where we use dbt, BigQuery and Looker, so you may realise that its usage may be aligned with this data stack paradigm.
@@ -45,15 +45,15 @@
 
 ## Installation
 
 You can install optician from a PyPi repository. We suggest you install it into a virtual environment.
 Please specify which database (or databases) you will be using, as in the example below.
 
 ```shell
-pip install optician[bigquery]
+pip install "optician[bigquery]"
 ```
 
 ## Setup
 1. Create the Optician configuration file `.optician/config.json` (you can name it another way) somewhere in your computer (we suggest inside the dbt or Looker repo)
 2. Create the environment variable `OPTICIAN_CONFIG_FILE` which will be the absolute path to the file created in 1
 3. You need to be able to connect to your database. For BigQuery, you can connect either by Oauth or Service Account.
 4. [Optional] Create an environment variable `GH_TOKEN` for your GitHub personal token. You need to create this token in [GitHub](https://github.com/settings/tokens) with read:project, repo, user:email permissions. This will allow you to commit your Looker views directly to the Looker repository.
```

