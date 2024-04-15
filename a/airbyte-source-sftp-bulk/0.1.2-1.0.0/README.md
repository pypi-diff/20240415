# Comparing `tmp/airbyte-source-sftp-bulk-0.1.2.tar.gz` & `tmp/airbyte_source_sftp_bulk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-sftp-bulk-0.1.2.tar", last modified: Wed Jan 31 18:01:30 2024, max compression
+gzip compressed data, was "airbyte_source_sftp_bulk-1.0.0.tar", max compression
```

## Comparing `airbyte-source-sftp-bulk-0.1.2.tar` & `airbyte_source_sftp_bulk-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.092225 airbyte-source-sftp-bulk-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     5640 2024-01-31 18:01:30.092225 airbyte-source-sftp-bulk-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5450 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.088225 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5640 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-01-31 18:01:30.000000 airbyte-source-sftp-bulk-0.1.2/airbyte_source_sftp_bulk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.088225 airbyte-source-sftp-bulk-0.1.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      912 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      676 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/configured_catalog.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.088225 airbyte-source-sftp-bulk-0.1.2/integration_tests/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.088225 airbyte-source-sftp-bulk-0.1.2/integration_tests/files/empty/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/files/empty/empty.json
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/files/test_1.json
--rw-r--r--   0 root         (0) root         (0)       40 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/files/test_2.json
--rw-r--r--   0 root         (0) root         (0)     9446 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/integration_test.py
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      175 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)      236 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/integration_tests/valid_config.json
--rw-r--r--   0 root         (0) root         (0)     5354 2024-01-31 18:01:30.092225 airbyte-source-sftp-bulk-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1028 2024-01-31 18:01:28.000000 airbyte-source-sftp-bulk-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:01:30.088225 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8194 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/client.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/run.py
--rw-r--r--   0 root         (0) root         (0)     5165 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/source.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/spec.json
--rw-r--r--   0 root         (0) root         (0)     2646 2024-01-31 17:51:56.000000 airbyte-source-sftp-bulk-0.1.2/source_sftp_bulk/streams.py
+-rw-r--r--   0        0        0     4550 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/README.md
+-rw-r--r--   0        0        0      857 2024-04-15 16:02:51.847530 airbyte_source_sftp_bulk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/client.py
+-rw-r--r--   0        0        0      670 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/run.py
+-rw-r--r--   0        0        0     1001 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/source.py
+-rw-r--r--   0        0        0     2053 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/spec.py
+-rw-r--r--   0        0        0     3273 2024-04-15 15:20:35.000000 airbyte_source_sftp_bulk-1.0.0/source_sftp_bulk/stream_reader.py
+-rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 airbyte_source_sftp_bulk-1.0.0/PKG-INFO
```

### Comparing `airbyte-source-sftp-bulk-0.1.2/PKG-INFO` & `airbyte_source_sftp_bulk-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 Metadata-Version: 2.1
 Name: airbyte-source-sftp-bulk
-Version: 0.1.2
+Version: 1.0.0
 Summary: Source implementation for SFTP Bulk.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk[file-based] (>=0,<1)
+Requires-Dist: paramiko (==3.4.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/sftp-bulk
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.2
-Requires-Dist: paramiko==2.11.0
-Requires-Dist: backoff==1.8.0
-Requires-Dist: terminaltables==3.1.0
-Requires-Dist: pandas==1.5.0
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: docker==5.0.3; extra == "tests"
 
-# SFTP Bulk Source
+# Sftp-Bulk source connector
 
-This is the repository for the FTP source connector, written in Python, that helps you bulk ingest files with the same data format from an FTP server into a single stream.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/sftp-bulk).
 
+This is the repository for the Sftp-Bulk source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/sftp-bulk).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/sftp-bulk)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_sftp_bulk/spec.json` file.
-Note that the `secrets` directory is gitignored by default, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/sftp-bulk)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_sftp_bulk/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source ftp test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-sftp-bulk spec
+poetry run source-sftp-bulk check --config secrets/config.json
+poetry run source-sftp-bulk discover --config secrets/config.json
+poetry run source-sftp-bulk read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-sftp-bulk build
 ```
 
-An image will be built with the tag `airbyte/source-sftp-bulk:dev`.
+An image will be available on your host with the tag `airbyte/source-sftp-bulk:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-sftp-bulk:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-sftp-bulk:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-sftp-bulk:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-sftp-bulk:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-sftp-bulk:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-sftp-bulk test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-sftp-bulk test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/sftp-bulk.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/sftp-bulk.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-sftp-bulk-0.1.2/README.md` & `airbyte_source_sftp_bulk-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,91 @@
-# SFTP Bulk Source
+# Sftp-Bulk source connector
 
-This is the repository for the FTP source connector, written in Python, that helps you bulk ingest files with the same data format from an FTP server into a single stream.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/sftp-bulk).
+
+This is the repository for the Sftp-Bulk source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/sftp-bulk).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
-
-#### Minimum Python version required `= 3.9.0`
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/sftp-bulk)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_sftp_bulk/spec.json` file.
-Note that the `secrets` directory is gitignored by default, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/sftp-bulk)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_sftp_bulk/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source ftp test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-sftp-bulk spec
+poetry run source-sftp-bulk check --config secrets/config.json
+poetry run source-sftp-bulk discover --config secrets/config.json
+poetry run source-sftp-bulk read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-sftp-bulk build
 ```
 
-An image will be built with the tag `airbyte/source-sftp-bulk:dev`.
+An image will be available on your host with the tag `airbyte/source-sftp-bulk:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-sftp-bulk:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-sftp-bulk:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-sftp-bulk:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-sftp-bulk:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-sftp-bulk:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-sftp-bulk test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-sftp-bulk test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/sftp-bulk.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/sftp-bulk.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

