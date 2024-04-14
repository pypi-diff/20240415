# Comparing `tmp/elapi-1.0.7.dev1.tar.gz` & `tmp/elapi-1.0.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elapi-1.0.7.dev1.tar", max compression
+gzip compressed data, was "elapi-1.0.7.dev2.tar", max compression
```

## Comparing `elapi-1.0.7.dev1.tar` & `elapi-1.0.7.dev2.tar`

### file list

```diff
@@ -1,53 +1,57 @@
--rw-r--r--   0        0        0    34523 2023-11-30 00:33:35.195522 elapi-1.0.7.dev1/LICENSE
--rw-r--r--   0        0        0     4264 2024-01-26 23:55:44.251923 elapi-1.0.7.dev1/README.md
--rw-r--r--   0        0        0     1514 2024-03-19 01:49:05.033453 elapi-1.0.7.dev1/pyproject.toml
--rw-r--r--   0        0        0       11 2024-03-19 01:49:05.033793 elapi-1.0.7.dev1/src/elapi/VERSION
--rw-r--r--   0        0        0       48 2023-12-06 23:06:28.083147 elapi-1.0.7.dev1/src/elapi/__init__.py
--rw-r--r--   0        0        0     1594 2024-01-26 23:55:44.252809 elapi-1.0.7.dev1/src/elapi/_names.py
--rw-r--r--   0        0        0    17048 2024-03-19 01:49:00.645808 elapi-1.0.7.dev1/src/elapi/api.py
--rw-r--r--   0        0        0       73 2024-03-19 01:49:00.646161 elapi-1.0.7.dev1/src/elapi/cli/__init__.py
--rw-r--r--   0        0        0       47 2024-03-11 21:19:57.521288 elapi-1.0.7.dev1/src/elapi/cli/__main__.py
--rw-r--r--   0        0        0     1668 2024-03-19 01:49:00.646373 elapi-1.0.7.dev1/src/elapi/cli/_plugin_handler.py
--rw-r--r--   0        0        0     7054 2024-03-19 01:49:00.646673 elapi-1.0.7.dev1/src/elapi/cli/doc.py
--rwxr-xr-x   0        0        0    24262 2024-03-19 01:49:00.646954 elapi-1.0.7.dev1/src/elapi/cli/elapi.py
--rw-r--r--   0        0        0     2575 2024-03-19 01:49:00.647270 elapi-1.0.7.dev1/src/elapi/cli/helpers.py
--rw-r--r--   0        0        0      457 2024-03-19 01:49:00.647714 elapi-1.0.7.dev1/src/elapi/configuration/__init__.py
--rw-r--r--   0        0        0     3726 2023-11-30 00:33:35.198611 elapi-1.0.7.dev1/src/elapi/configuration/_config_history.py
--rw-r--r--   0        0        0     6876 2024-03-19 01:49:00.647983 elapi-1.0.7.dev1/src/elapi/configuration/config.py
--rw-r--r--   0        0        0     1090 2023-11-30 00:33:35.200032 elapi-1.0.7.dev1/src/elapi/configuration/log_file.py
--rw-r--r--   0        0        0     6502 2024-03-19 01:49:00.648240 elapi-1.0.7.dev1/src/elapi/endpoint.py
--rw-r--r--   0        0        0      418 2023-11-30 00:33:35.200347 elapi-1.0.7.dev1/src/elapi/loggers/__init__.py
--rw-r--r--   0        0        0     1226 2023-11-30 00:33:35.200496 elapi-1.0.7.dev1/src/elapi/loggers/base.py
--rw-r--r--   0        0        0      636 2023-11-30 00:33:35.200624 elapi-1.0.7.dev1/src/elapi/loggers/handlers/__init__.py
--rw-r--r--   0        0        0     2673 2023-11-30 00:33:35.200788 elapi-1.0.7.dev1/src/elapi/loggers/handlers/file.py
--rw-r--r--   0        0        0     1429 2024-01-26 23:55:44.254715 elapi-1.0.7.dev1/src/elapi/loggers/handlers/stderr.py
--rw-r--r--   0        0        0    11342 2024-03-19 01:49:00.648710 elapi-1.0.7.dev1/src/elapi/path.py
--rw-r--r--   0        0        0        0 2024-03-11 20:59:16.605191 elapi-1.0.7.dev1/src/elapi/plugins/__init__.py
--rw-r--r--   0        0        0       40 2024-03-19 01:49:00.649043 elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/__init__.py
--rw-r--r--   0        0        0      127 2024-03-19 01:49:00.649547 elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/_doc.py
--rw-r--r--   0        0        0     6092 2024-03-19 01:49:00.649695 elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/bill_teams.py
--rw-r--r--   0        0        0     4590 2024-03-19 01:49:00.649911 elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/cli.py
--rw-r--r--   0        0        0     2355 2024-01-26 23:55:44.255032 elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/invoice.py
--rw-r--r--   0        0        0      224 2024-03-19 01:49:00.650126 elapi-1.0.7.dev1/src/elapi/plugins/experiments/__init__.py
--rw-r--r--   0        0        0     1823 2024-03-19 01:49:00.650523 elapi-1.0.7.dev1/src/elapi/plugins/experiments/_doc.py
--rw-r--r--   0        0        0    10194 2024-03-19 01:49:00.650848 elapi-1.0.7.dev1/src/elapi/plugins/experiments/cli.py
--rw-r--r--   0        0        0     6225 2024-03-19 01:49:00.651136 elapi-1.0.7.dev1/src/elapi/plugins/experiments/experiments.py
--rw-r--r--   0        0        0     1931 2024-03-19 01:49:00.651360 elapi-1.0.7.dev1/src/elapi/plugins/experiments/formats.py
--rw-r--r--   0        0        0     3794 2024-03-19 01:49:00.651642 elapi-1.0.7.dev1/src/elapi/plugins/show_config.py
--rw-r--r--   0        0        0      137 2024-03-19 01:49:00.651862 elapi-1.0.7.dev1/src/elapi/plugins/utils/__init__.py
--rw-r--r--   0        0        0     2935 2024-03-19 01:49:00.652069 elapi-1.0.7.dev1/src/elapi/plugins/utils/export.py
--rw-r--r--   0        0        0      942 2024-03-19 01:49:00.652371 elapi-1.0.7.dev1/src/elapi/plugins/utils/get_location_from_headers.py
--rw-r--r--   0        0        0      294 2023-12-07 21:54:53.434352 elapi-1.0.7.dev1/src/elapi/plugins/version.py
--rw-r--r--   0        0        0      271 2024-01-26 23:55:44.255284 elapi-1.0.7.dev1/src/elapi/styles/__init__.py
--rw-r--r--   0        0        0     1639 2023-11-30 00:33:35.203150 elapi-1.0.7.dev1/src/elapi/styles/_markdown_doc.py
--rw-r--r--   0        0        0      731 2023-11-30 00:33:35.203288 elapi-1.0.7.dev1/src/elapi/styles/_missing.py
--rw-r--r--   0        0        0      138 2024-01-26 23:55:44.256419 elapi-1.0.7.dev1/src/elapi/styles/base.py
--rw-r--r--   0        0        0      628 2023-11-30 00:33:35.203406 elapi-1.0.7.dev1/src/elapi/styles/colors.py
--rw-r--r--   0        0        0     2954 2024-03-19 01:49:00.652654 elapi-1.0.7.dev1/src/elapi/styles/format.py
--rw-r--r--   0        0        0     1553 2023-11-30 00:33:35.203920 elapi-1.0.7.dev1/src/elapi/styles/highlight.py
--rw-r--r--   0        0        0      268 2023-11-30 00:33:35.204096 elapi-1.0.7.dev1/src/elapi/validators/__init__.py
--rw-r--r--   0        0        0      957 2023-11-30 00:33:35.204231 elapi-1.0.7.dev1/src/elapi/validators/base.py
--rw-r--r--   0        0        0     4167 2024-03-19 01:49:00.652927 elapi-1.0.7.dev1/src/elapi/validators/identity.py
--rw-r--r--   0        0        0     2413 2023-11-30 00:33:35.204669 elapi-1.0.7.dev1/src/elapi/validators/path.py
--rw-r--r--   0        0        0     2993 2024-03-19 01:49:00.653030 elapi-1.0.7.dev1/src/elapi/validators/permission.py
--rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 elapi-1.0.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-30 00:33:35.195522 elapi-1.0.7.dev2/LICENSE
+-rw-r--r--   0        0        0     6521 2024-04-14 21:48:47.364352 elapi-1.0.7.dev2/README.md
+-rw-r--r--   0        0        0     1416 2024-04-14 21:53:57.515760 elapi-1.0.7.dev2/pyproject.toml
+-rw-r--r--   0        0        0       11 2024-04-14 18:35:12.906558 elapi-1.0.7.dev2/src/elapi/VERSION
+-rw-r--r--   0        0        0       48 2023-12-06 23:06:28.083147 elapi-1.0.7.dev2/src/elapi/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-14 15:52:00.760366 elapi-1.0.7.dev2/src/elapi/_exceptions.py
+-rw-r--r--   0        0        0     1594 2024-01-26 23:55:44.252809 elapi-1.0.7.dev2/src/elapi/_names.py
+-rw-r--r--   0        0        0    17066 2024-04-02 15:08:46.197419 elapi-1.0.7.dev2/src/elapi/api.py
+-rw-r--r--   0        0        0       94 2024-04-14 15:52:00.760912 elapi-1.0.7.dev2/src/elapi/cli/__init__.py
+-rw-r--r--   0        0        0       47 2024-03-11 21:19:57.521288 elapi-1.0.7.dev2/src/elapi/cli/__main__.py
+-rw-r--r--   0        0        0     1668 2024-04-12 17:41:23.834798 elapi-1.0.7.dev2/src/elapi/cli/_plugin_handler.py
+-rw-r--r--   0        0        0     7105 2024-04-14 15:52:00.761360 elapi-1.0.7.dev2/src/elapi/cli/doc.py
+-rwxr-xr-x   0        0        0    24988 2024-04-14 18:35:05.962422 elapi-1.0.7.dev2/src/elapi/cli/elapi.py
+-rw-r--r--   0        0        0      457 2024-03-19 01:49:00.647714 elapi-1.0.7.dev2/src/elapi/configuration/__init__.py
+-rw-r--r--   0        0        0     3726 2023-11-30 00:33:35.198611 elapi-1.0.7.dev2/src/elapi/configuration/_config_history.py
+-rw-r--r--   0        0        0     6876 2024-04-12 22:37:26.173342 elapi-1.0.7.dev2/src/elapi/configuration/config.py
+-rw-r--r--   0        0        0     1090 2023-11-30 00:33:35.200032 elapi-1.0.7.dev2/src/elapi/configuration/log_file.py
+-rw-r--r--   0        0        0     6502 2024-03-19 01:49:00.648240 elapi-1.0.7.dev2/src/elapi/endpoint.py
+-rw-r--r--   0        0        0      418 2023-11-30 00:33:35.200347 elapi-1.0.7.dev2/src/elapi/loggers/__init__.py
+-rw-r--r--   0        0        0     1226 2023-11-30 00:33:35.200496 elapi-1.0.7.dev2/src/elapi/loggers/base.py
+-rw-r--r--   0        0        0      636 2023-11-30 00:33:35.200624 elapi-1.0.7.dev2/src/elapi/loggers/handlers/__init__.py
+-rw-r--r--   0        0        0     2673 2023-11-30 00:33:35.200788 elapi-1.0.7.dev2/src/elapi/loggers/handlers/file.py
+-rw-r--r--   0        0        0     1429 2024-01-26 23:55:44.254715 elapi-1.0.7.dev2/src/elapi/loggers/handlers/stderr.py
+-rw-r--r--   0        0        0    13866 2024-04-14 15:52:00.762713 elapi-1.0.7.dev2/src/elapi/path.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:59:16.605191 elapi-1.0.7.dev2/src/elapi/plugins/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-12 17:30:21.342171 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-14 15:52:00.763121 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/_doc.py
+-rw-r--r--   0        0        0     9119 2024-04-14 15:52:00.763919 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/bill_teams.py
+-rw-r--r--   0        0        0    12428 2024-04-14 15:52:00.764253 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/cli.py
+-rw-r--r--   0        0        0      795 2024-04-14 15:52:00.764505 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/format.py
+-rw-r--r--   0        0        0     2026 2024-04-14 15:52:00.764755 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/invoice.py
+-rw-r--r--   0        0        0     8517 2024-04-14 15:52:00.765133 elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/validator.py
+-rw-r--r--   0        0        0      214 2024-04-14 15:52:00.765753 elapi-1.0.7.dev2/src/elapi/plugins/commons/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-14 15:52:00.766203 elapi-1.0.7.dev2/src/elapi/plugins/commons/cli_helpers.py
+-rw-r--r--   0        0        0     2935 2024-04-14 15:52:00.766311 elapi-1.0.7.dev2/src/elapi/plugins/commons/export.py
+-rw-r--r--   0        0        0     4387 2024-04-14 15:52:00.766584 elapi-1.0.7.dev2/src/elapi/plugins/commons/get_information.py
+-rw-r--r--   0        0        0      942 2024-04-14 15:52:00.766686 elapi-1.0.7.dev2/src/elapi/plugins/commons/get_location_from_headers.py
+-rw-r--r--   0        0        0      224 2024-03-19 01:49:00.650126 elapi-1.0.7.dev2/src/elapi/plugins/experiments/__init__.py
+-rw-r--r--   0        0        0     3169 2024-04-14 15:52:00.766957 elapi-1.0.7.dev2/src/elapi/plugins/experiments/_doc.py
+-rw-r--r--   0        0        0    10192 2024-04-14 15:52:00.767324 elapi-1.0.7.dev2/src/elapi/plugins/experiments/cli.py
+-rw-r--r--   0        0        0     6295 2024-03-22 13:46:19.917268 elapi-1.0.7.dev2/src/elapi/plugins/experiments/experiments.py
+-rw-r--r--   0        0        0     1931 2024-04-13 23:29:32.885594 elapi-1.0.7.dev2/src/elapi/plugins/experiments/formats.py
+-rw-r--r--   0        0        0     3810 2024-03-22 13:46:19.918068 elapi-1.0.7.dev2/src/elapi/plugins/show_config.py
+-rw-r--r--   0        0        0      294 2023-12-07 21:54:53.434352 elapi-1.0.7.dev2/src/elapi/plugins/version.py
+-rw-r--r--   0        0        0      303 2024-04-14 15:52:00.767724 elapi-1.0.7.dev2/src/elapi/styles/__init__.py
+-rw-r--r--   0        0        0     1639 2023-11-30 00:33:35.203150 elapi-1.0.7.dev2/src/elapi/styles/_markdown_doc.py
+-rw-r--r--   0        0        0      731 2023-11-30 00:33:35.203288 elapi-1.0.7.dev2/src/elapi/styles/_missing.py
+-rw-r--r--   0        0        0      138 2024-01-26 23:55:44.256419 elapi-1.0.7.dev2/src/elapi/styles/base.py
+-rw-r--r--   0        0        0      628 2023-11-30 00:33:35.203406 elapi-1.0.7.dev2/src/elapi/styles/colors.py
+-rw-r--r--   0        0        0     4490 2024-04-14 15:52:00.768285 elapi-1.0.7.dev2/src/elapi/styles/format.py
+-rw-r--r--   0        0        0     1800 2024-04-14 15:52:00.768604 elapi-1.0.7.dev2/src/elapi/styles/highlight.py
+-rw-r--r--   0        0        0      299 2024-04-14 15:52:00.769441 elapi-1.0.7.dev2/src/elapi/validators/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-14 15:52:00.769763 elapi-1.0.7.dev2/src/elapi/validators/base.py
+-rw-r--r--   0        0        0     5952 2024-04-14 15:52:00.770524 elapi-1.0.7.dev2/src/elapi/validators/identity.py
+-rw-r--r--   0        0        0     2415 2024-04-14 18:35:05.962764 elapi-1.0.7.dev2/src/elapi/validators/path.py
+-rw-r--r--   0        0        0     5288 2024-04-14 15:52:00.771304 elapi-1.0.7.dev2/src/elapi/validators/permission.py
+-rw-r--r--   0        0        0     8133 1970-01-01 00:00:00.000000 elapi-1.0.7.dev2/PKG-INFO
```

### Comparing `elapi-1.0.7.dev1/LICENSE` & `elapi-1.0.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/README.md` & `elapi-1.0.7.dev2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # elAPI
 
-elAPI is a powerful, extensible API interface to eLabFTW. It supports serving almost all kinds of requests documented in
+elAPI is a powerful, extensible API client for eLabFTW built for
+the [University Computing Centre](https://www.urz.uni-heidelberg.de/en) (
+URZ, [FIRE](https://www.urz.uni-heidelberg.de/en/node/64/organisation/future-it-research-education) division) at
+Universität Heidelberg. It supports serving almost all kinds of requests documented on
 [eLabFTW API documentation](https://doc.elabftw.net/api/v2/) with ease. elAPI treats eLabFTW API endpoints as its
 arguments.
 
 **Example:**
 
 From [the documentation](https://doc.elabftw.net/api/v2/#/Users/read-user):
 > GET /users/{id}
@@ -13,133 +16,186 @@
 
 ```sh
 $ elapi get users --id <id>
 ```
 
 ## Installation
 
-Support for installing packages with `pip install --user` has been deprecated with the adoption of [PEP 688](https://peps.python.org/pep-0668/) on many systems like [Debian 12](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1030335#5).
-We recommend [`pipx`](https://pipx.pypa.io/stable/) for installing elAPI.
+elAPI can be used both as a CLI tool and as a Python library. If you are interested in simply using elAPI's
+off-the-shelf features from the command-line, install elAPI as a CLI tool. If you intend to write automation script for
+eLabFTW, you should install elAPI as a library inside a virtual environment. Of course, if you're interested in
+both, you can have elAPI installed in both ways.
+
+### Install elAPI as a CLI tool
+
+Support for installing Python packages with `pip install --user` has been deprecated with the adoption
+of [PEP 688](https://peps.python.org/pep-0668/) on many systems
+like [Debian 12](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1030335#5).
+We recommend [`pipx`](https://pipx.pypa.io/stable/) for installing elAPI for use of its CLI functionalities. Pipx
+installs packages in isolated virtual environments, so Pipx-installed elAPI should not conflict with elAPI installed
+inside other virtual environments.
 
 ```shell
 $ pipx install elapi
 ```
 
-Of course, `pip install --user elapi` might continue to work on some systems.
+After installation with Pipx is complete, you would also be able to run elAPI just by entering the `elapi` command on
+the
+terminal.
+
+### Install elAPI as a library
+
+It is recommended to install elAPI inside a Python virtual environment for use of its rich APIs for
+working with eLabFTW. From inside a virtual environment, elAPI CLI can be invoked with `python -m elapi.cli`.
+At the moment, though, the documentation about using elAPI as a library is severely lacking.
 
 ## Configuration
 
-elAPI needs to be configured first before we can do anything useful with it. elAPI supports a YAML configuration file in
+elAPI needs to be configured first before you can do anything useful with it. Mainly, elAPI needs to know your eLabFTW
+server's API URL and your API key (or token) for access.
+
+### Quick configuration
+
+You can run `elapi init` to simplify the configuration process. You will be prompted with questions
+about your eLabFTW server with examples to help you fill in the answers.
+
+### Advanced configuration
+
+elAPI supports a YAML configuration file in
 the following locations.
 
 - Current directory: `./elapi.yml`
 - User directory: `$HOME/.config/elapi.yml`
 - Root directory: `/etc/elapi.yml`
 
 elAPI supports configuration overloading. I.e., a keyword set in root configuration file `/etc/elapi.yml` can be
-overriden by setting a different value in user configuration file `$HOME/.config/elapi.yml`. In terms of precedence,
+overridden by setting a different value in user configuration file `$HOME/.config/elapi.yml`. In terms of precedence,
 configuration file present in the currently active directory has the highest priority, and configuration in root
 directory has the lowest.
 
 The following parameters are currently configurable, with `host` and `api_token` being the required fields. For testing
-purposes it would be safe to store everything in the user configuration file.
+purposes it would be safe to store everything in `$HOME/.config/elapi.yml`.
 
 ```yaml
 # elAPI configuration
 # Saved in `$HOME/.config/elapi.yml`
 
 host: <host API url>
 # Example: https://demo.elabftw.net/api/v2/
 # Note the host URL ends with the API endpoint
 api_token: <token with at least read-access>
 # You can generate an API token from eLabFTW user panel -> API keys tab.
 export_dir: ~/Downloads/elAPI
 unsafe_api_token_warning: yes
 ```
 
-We can get an overview of detected configurations.
+You can get an overview of detected configurations.
 
 ```shell
 $ elapi show-config
 ```
 
-If both `host` and `api_token` are detected, we are good to go!
+If both `host` and `api_token` are detected, you are good to go!
 
 ## Usage
 
 elAPI can be invoked from the command-line.
 
 ```shell
 $ elapi --help 
 ```
 
 ### `GET` requests
 
-We can request an overview of running eLabFTW server.
+Request an overview of running eLabFTW server:
 
 ```shell
 $ elapi get info -F yml
 # Here -F (or --format) defines the output format
 ```
 
-We can request a list o all active experiments and export it to a `JSON` file.
+You can request a list o all active experiments and export it to a `JSON` file.
 
 ```shell
 $ elapi get experiments --export ~/Downoads/experiments.json
 ```
 
 ### `POST` requests
 
-We can create a new user by the name 'John Doe'.
+Create a new user by the name 'John Doe':
 
 ```shell
 $ elapi post users --id <user id> -d '{"firstname": "John", "lastname": "Doe", "email": "test_test@itnerd.de"}'
 ```
 
 ### `PATCH` requests
 
-We can update an existing user's email address.
+Update an existing user's email address:
 
 ```shell
 $ elapi patch users --id <user id> -d '{"email": "new_email@itnerd.de"}'
 ```
 
-`patch` command allows us to make changes to eLabFTW server settings. E.g., we can update the time (in minutes)
+`patch` command allows us to make changes to eLabFTW server settings. E.g., you can update the time (in minutes)
 after which the authentication cookie will expire.
 
 ```shell
 $ elapi patch config -d '{"cookie_validity_time": 43200}'
 ```
 
-We can publish an announcement to all the members.
+You can publish an announcement to all the members.
 
 ```shell
 $ elapi patch config -d '{"announcement": "Notice: Server will be down tomorrow at midnight due to scheduled maintenance."}'
 ```
 
-### Bill teams
+### `DELETE` requests
 
-We can generate invoice for eLabFTW teams.
+Delete all the tags associated to an experiment:
 
 ```shell
-$ elapi bill-teams generate-invoice
+$ elapi delete experiments -i <experiment ID> --sub tags
 ```
 
-We may just want to have a look at the billing information without generating invoice.
+You can reset the configuration to default values.
 
 ```shell
-$ elapi bill-teams info -F yaml
+$ elapi delete config
 ```
 
-We can also export this information as a `YAML` file to the export directory defined in configuration
-file (`export_dir`).
+### `experiments` plugin
+
+`experiments` plugin enables experiments-specific actions. You can download an experiment in PDF by its "Unique eLabID"
+to `~/Downloads` directory.
 
 ```shell
-elapi bill-teams info -F yaml --export
+$ elapi experiments get -i <experiment unique elabid> -F pdf --export ~/Downloads/
 ```
 
+Append text in markdown to an existing experiment by its ID:
+
+```shell
+$ elapi experiments append --id <experiment ID> -M -t "**New content.**"
+```
+
+You can also upload an attachment to an experiment.
+
+```shell
+$ elapi experiments upload-attachment --id <experiment ID> --path <path to attachment file> --comment <comment for your attachment>
+```
+
+### Bill teams
+
+You can get a list of all teams and its users for billing purposes and export it to home directory.
+
+```shell
+$ elapi bill-teams teams-info --export ~
+```
+
+Most sub-commands available under `elapi bill-teams` plugin are for Universität Heidelberg specific use-cases.
+
 ## Open-source
 
 elAPI is open-source and published under AGPLv3 license. The repository is however hosted internally within
 Universität Heidelberg's network. The codebase can still be accessed from [PyPI](https://pypi.org/project/elapi/#files).
 If you express interest in having the repository made completely public, or if you have any question, feel free
 to [contact us](mailto:elabftw@uni-heidelberg.de).
```

### Comparing `elapi-1.0.7.dev1/pyproject.toml` & `elapi-1.0.7.dev2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tool.poetry]
 name = "elapi"
-version = "1.0.7-dev1"
-description = """elAPI is a powerful, extensible API interface to eLabFTW built for \
-the University Computing Centre (URZ, FIRE division) at Universität Heidelberg."""
+version = "1.0.7-dev2"
+description = "elAPI is a powerful, extensible API client for eLabFTW."
 authors = [
     "Alexander Haller <alexander.haller@urz.uni-heidelberg.de>",
     "Mahadi Xion <mahadi.xion@urz.uni-heidelberg.de>",
 ]
 maintainers = [
     "Mahadi Xion <mahadi.xion@urz.uni-heidelberg.de>",
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `elapi-1.0.7.dev1/src/elapi/_names.py` & `elapi-1.0.7.dev2/src/elapi/_names.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/api.py` & `elapi-1.0.7.dev2/src/elapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     @property
     def endpoint_id(self) -> Union[int, str, None]:
         return self._endpoint_id
 
     @endpoint_id.setter
     def endpoint_id(self, value):
         if value is not None:
-            if not re.match(r"^\w+$", value := str(value)):
+            if not re.match(r"^(\d+)$|^(me)$", value := str(value)):
                 # Although, eLabFTW primarily supports integer-only IDs, there are exceptions, like the alias
                 # ID "me" for receiving one's own user information.
                 raise ElabFTWURLError("Invalid endpoint ID (or entity ID).")
             self._endpoint_id = value
         else:
             self._endpoint_id = ""
 
@@ -169,15 +169,15 @@
     @sub_endpoint_id.setter
     def sub_endpoint_id(self, value):
         if self.sub_endpoint_name is None:
             raise ElabFTWURLError(
                 "Sub-endpoint ID cannot be defined without first specifying its sub-endpoint name."
             )
         if value is not None:
-            if not re.match(r"^\w+$", value := str(value)):
+            if not re.match(r"^(\d+)$|^(me)$", value := str(value)):
                 raise ElabFTWURLError("Invalid sub-endpoint ID (or entity sub-ID).")
             self._sub_endpoint_id = value
         else:
             self._sub_endpoint_id = ""
             # Similar to an empty endpoint_id, an empty sub_endpoint_id sends back
             # the whole list of available resources for a given sub-endpoint as response.
```

### Comparing `elapi-1.0.7.dev1/src/elapi/cli/_plugin_handler.py` & `elapi-1.0.7.dev2/src/elapi/cli/_plugin_handler.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/cli/doc.py` & `elapi-1.0.7.dev2/src/elapi/cli/doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,16 @@
               f"If _--format/-F_ is also present, then file extension is ignored, "
               f"and --format value takes precedence.\n",
     "data_format": f"Format style for the output. Supported values are: {supported_highlighting_formats}. "
               f"The values are case insensitive. The default format is `{DEFAULT_EXPORT_DATA_FORMAT.upper()}`. "
               "When 'txt' is used, the response will be sent in *original*, un-formatted (almost), "
               "without syntax highlighting. This can be utilized if one wishes to pipe the output "
               " to some external formatting program like `less`. "
-              "If an unsupported format value is provided then the output format falls back to 'txt'.",
+              "If an unsupported format value is provided then the output format "
+              f"falls back to `{DEFAULT_EXPORT_DATA_FORMAT.upper()}`.",
     "no_keys": "Do not show the names of configuration keywords.",
     "init_host": 'The host URL of your eLabFTW instance. It will look like \"https://demo.elabftw.net/api/v2\".',
     "init_api_token": 'API token (or API key) of your eLabFTW instance. You can generate it from eLabFTW "User Panel". '
                       'Make sure your API key has proper permission for your future tasks.',
     "init_export_dir": f"Preferred export directory. If '--export-dir' isn't passed, {EXPORT_DIR} will be "
                         "set as the export directory."
 }
```

### Comparing `elapi-1.0.7.dev1/src/elapi/cli/elapi.py` & `elapi-1.0.7.dev2/src/elapi/cli/elapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import typer
 from rich import pretty
 from rich.markdown import Markdown
 from typing_extensions import Annotated
 
 from ._plugin_handler import internal_plugin_typer_apps
 from .doc import __PARAMETERS__doc__ as docs
-from .helpers import OrderedCommands
 from .. import APP_NAME
 from ..configuration import EXPORT_DIR
 from ..loggers import Logger
+from ..plugins.commons.cli_helpers import OrderedCommands
 from ..styles import get_custom_help_text
 from ..styles import stdin_console, stderr_console
 
 logger = Logger()
 
 
 pretty.install()
@@ -97,14 +97,15 @@
     With arguments: `elapi init --host <host> --api-token <api-token> --export-dir <export-directory>`
 
     """
     from .._names import CONFIG_FILE_NAME
     from ..configuration import LOCAL_CONFIG_LOC
     from ..validators import Validate, ValidationError
     from ..validators import PathValidator
+    from ..path import ProperPath
     from time import sleep
 
     with stdin_console.status(
         f"Creating configuration file {CONFIG_FILE_NAME}...", refresh_per_second=15
     ):
         sleep(0.5)
         typer.echo()  # mainly for a newline!
@@ -115,35 +116,50 @@
             logger.error(
                 f"{APP_NAME} couldn't validate path '{LOCAL_CONFIG_LOC}' for writing configuration! "
                 f"Please make sure you have write and read access to '{LOCAL_CONFIG_LOC}'. "
                 "Configuration initialization has failed!"
             )
             raise typer.Exit(1)
         else:
-            with LOCAL_CONFIG_LOC.open(mode="r+") as f:
-                if f.read():
-                    logger.error(
-                        f"A configuration file '{LOCAL_CONFIG_LOC}' already exists and it's not empty! "
-                        f"It's ambiguous what to do in this situation. {APP_NAME} will abort. "
-                        f"Configuration initialization has failed!"
-                    )
-                    raise typer.Exit(1)
+            path = ProperPath(LOCAL_CONFIG_LOC)
+            try:
+                with path.open(mode="r") as f:
+                    if f.read():
+                        logger.error(
+                            f"A configuration file '{LOCAL_CONFIG_LOC}' already exists and it's not empty! "
+                            f"It's ambiguous what to do in this situation."
+                        )
+                        logger.error("Configuration initialization has failed!")
+                        raise typer.Exit(1)
+            except path.PathException as e:
+                if isinstance(e, FileNotFoundError):
+                    path.create()
                 else:
+                    logger.error(e)
+                    logger.error("Configuration initialization has failed!")
+                    raise typer.Exit(1)
+            try:
+                with path.open(mode="w") as f:
                     _configuration_yaml_text = f"""host: {host_url}
-api_token: {api_token}
-export_dir: {export_directory}
-unsafe_api_token_warning: yes
-"""
+    api_token: {api_token}
+    export_dir: {export_directory}
+    unsafe_api_token_warning: yes
+    """
                     f.write(_configuration_yaml_text)
-            stdin_console.print(
-                "Configuration file has been successfully created! "
-                f"Run '{APP_NAME} show-config' to see the configuration path "
-                "and more configuration details.",
-                style="green",
-            )
+            except path.PathException as e:
+                logger.error(e)
+                logger.error("Configuration initialization has failed!")
+                raise typer.Exit(1)
+            else:
+                stdin_console.print(
+                    "Configuration file has been successfully created! "
+                    f"Run '{APP_NAME} show-config' to see the configuration path "
+                    "and more configuration details.",
+                    style="green",
+                )
 
 
 @app.command(short_help="Make `GET` requests to eLabFTW endpoints.")
 def get(
     endpoint_name: Annotated[
         str, typer.Argument(help=docs["endpoint_name"], show_default=False)
     ],
@@ -196,17 +212,17 @@
     <br/>
     `$ elapi get users --id <id>` will return information about the specific user `<id>`.
     """
     import ast
     import re
     from .. import APP_NAME
     from ..api import GETRequest, ElabFTWURLError
-    from .helpers import CLIExport, CLIFormat
+    from ..plugins.commons.cli_helpers import CLIExport, CLIFormat
     from ..validators import Validate, HostIdentityValidator
-    from ..plugins.utils import Export
+    from ..plugins.commons import Export
     from ..styles import Highlight
 
     validate_config = Validate(HostIdentityValidator())
     validate_config()
 
     if export is False:
         _export_dest = None
@@ -320,23 +336,23 @@
     **Example**:
     <br/>
     From [the official documentation about `POST users`](https://doc.elabftw.net/api/v2/#/Users/post-user),
     > POST /users/{id}
 
     With `elapi` you can do the following:
     <br/>
-    `$ elapi post users --id <user id> -d '{"firstname": "John", "lastname": "Doe", "email": "test_test@itnerd.de"}'`
+    `$ elapi post users -d '{"firstname": "John", "lastname": "Doe", "email": "test_test@itnerd.de"}'`
     will create a new user.
     """
     import ast
     from .. import APP_NAME
     from ..api import POSTRequest, ElabFTWURLError
     from json import JSONDecodeError
     from ..validators import Validate, HostIdentityValidator
-    from ..plugins.utils import get_location_from_headers
+    from ..plugins.commons import get_location_from_headers
     from ..styles import Format, Highlight
     from ..path import ProperPath
 
     validate_config = Validate(HostIdentityValidator())
     validate_config()
 
     try:
@@ -666,15 +682,15 @@
 
 
 @app.command(name="show-config")
 def show_config(
     no_keys: Annotated[
         Optional[bool],
         typer.Option("--no-keys", help=docs["no_keys"], show_default=True),
-    ] = True,
+    ] = False,
 ) -> None:
     """
     Get information about detected configuration values.
     """
     from ..plugins.show_config import show
 
     md = Markdown(show(no_keys))
```

### Comparing `elapi-1.0.7.dev1/src/elapi/cli/helpers.py` & `elapi-1.0.7.dev2/src/elapi/plugins/commons/cli_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from collections.abc import Iterable
 from typing import Optional
 
 from click import Context
 from typer.core import TyperGroup
 
-from ..configuration import APP_NAME, DEFAULT_EXPORT_DATA_FORMAT
-from ..loggers import Logger
-from ..path import ProperPath
+from ...configuration import APP_NAME, DEFAULT_EXPORT_DATA_FORMAT
+from ...loggers import Logger
+from ...path import ProperPath
 
 logger = Logger()
 
 
 class CLIExport:
     def __new__(
         cls, data_format: Optional[str] = None, export_dest: Optional[str] = None
     ):
         from collections import namedtuple
-        from ..validators import Validate
-        from ..plugins.utils import ExportValidator
+        from ...validators import Validate
+        from .export import ExportValidator
 
         validate_export = Validate(ExportValidator(export_dest))
         export_dest: ProperPath = validate_export.get()
 
         _export_file_ext: str = (
             export_dest.expanded.suffix.removeprefix(".")
             if export_dest.kind == "file"
@@ -40,19 +40,19 @@
     FALLBACK_DATA_FORMAT = DEFAULT_EXPORT_DATA_FORMAT
 
     def __new__(
         cls,
         data_format: str,
         export_file_ext: Optional[str] = None,
     ):
-        from ..styles import Format
+        from ...styles import Format, FormatError
 
         try:
             format = Format(data_format)
-        except ValueError as e:
+        except FormatError as e:
             logger.error(e)
             logger.info(
                 f"{APP_NAME} will fallback to '{cls.FALLBACK_DATA_FORMAT}' format."
             )
             format = Format(
                 cls.FALLBACK_DATA_FORMAT
             )  # Falls back to DEFAULT_EXPORT_DATA_FORMAT
```

### Comparing `elapi-1.0.7.dev1/src/elapi/configuration/_config_history.py` & `elapi-1.0.7.dev2/src/elapi/configuration/_config_history.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/configuration/config.py` & `elapi-1.0.7.dev2/src/elapi/configuration/config.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/configuration/log_file.py` & `elapi-1.0.7.dev2/src/elapi/configuration/log_file.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/endpoint.py` & `elapi-1.0.7.dev2/src/elapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/loggers/base.py` & `elapi-1.0.7.dev2/src/elapi/loggers/base.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/loggers/handlers/__init__.py` & `elapi-1.0.7.dev2/src/elapi/loggers/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/loggers/handlers/file.py` & `elapi-1.0.7.dev2/src/elapi/loggers/handlers/file.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/loggers/handlers/stderr.py` & `elapi-1.0.7.dev2/src/elapi/loggers/handlers/stderr.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/path.py` & `elapi-1.0.7.dev2/src/elapi/path.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import os
 import re
 from contextlib import contextmanager
 from pathlib import Path
 from shutil import rmtree
 from typing import Union, TextIO, Generator
 
+from ._exceptions import NoException
 from .loggers import SimpleLogger
 
 
 class ProperPath:
     def __init__(
         self,
-        name: Union[str, Path, None],
+        name: Union[str, Path, None, "ProperPath"],
         env_var: bool = False,
         kind: Union[str, None] = "",
         err_logger: logging.Logger = SimpleLogger(),
     ):
         self.name = name
         self.env_var = env_var
         self.kind = kind
         self.err_logger = err_logger
+        self.PathException = NoException
 
     def __str__(self):
         return str(self.expanded)
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}(name={self.name}, env_var={self.env_var}, kind={self.kind}, "
@@ -59,14 +61,32 @@
     @err_logger.setter
     def err_logger(self, value):
         if not isinstance(value, logging.Logger):
             raise ValueError("'err_logger' must be a logging.Logger instance!")
         self._err_logger = value
 
     @property
+    def PathException(self) -> type:
+        return self._PathException
+
+    # noinspection PyAttributeOutsideInit
+    @PathException.setter
+    def PathException(self, value: type) -> None:
+        if not issubclass(value, (Exception, BaseException)):
+            raise ValueError(
+                "Only an instance of Exception or BaseException can be "
+                "assigned to descriptor PathException."
+            )
+        self._PathException = value
+
+    @PathException.deleter
+    def PathException(self):
+        raise AttributeError("PathException cannot be deleted!")
+
+    @property
     def expanded(self) -> Path:
         if self.env_var:
             try:
                 return Path(os.environ[self.name]).expanduser()
             except KeyError as e:
                 raise ValueError(
                     f"Environment variable {self.name} doesn't exist."
@@ -130,18 +150,32 @@
         try:
             if self.kind == "file":
                 path_parent, path_file = path.parent, path.name
                 path_parent.mkdir(parents=True, exist_ok=True)
                 (path_parent / path_file).touch(exist_ok=True)
             elif self.kind == "dir":
                 path.mkdir(parents=True, exist_ok=True)
-        except PermissionError as e:
+        except (exception := PermissionError) as e:
             message = f"Permission to create {self._error_helper_compare_path_source(self.name, path)} is denied."
             self.err_logger.error(message)
+            self.PathException = exception
+            raise e
+        except (exception := NotADirectoryError) as e:
+            # Both "file" and "dir" cases are handled, but when path is under special files like
+            # /dev/null/<directory name>, os.mkdir() will throw NotADirectoryError.
+            message = f"Couldn't create {self._error_helper_compare_path_source(self.name, path)}."
+            self.err_logger.error(message)
+            self.PathException = exception
             raise e
+        except (exception := OSError) as os_err:
+            # When an attempt to create a file or directory inside root (e.g., '/foo')
+            # is made, OS can throw OSError with error no. 30 instead of PermissionError.
+            self.err_logger.error(os_err)
+            self.PathException = exception
+            raise os_err
         else:
             return path
 
     def _remove_file(self, _file: Path = None, verbose: bool = False) -> None:
         file = _file if _file else self.expanded
         if not isinstance(file, Path):
             raise ValueError(
@@ -149,18 +183,20 @@
                 f"Check instance attribute 'expanded'."
             )
 
         try:
             file.unlink()
         except FileNotFoundError as e:
             # unlink() throws FileNotFoundError when a directory is passed as it expects files only
-            raise ValueError(f"{file} doesn't exist or isn't a valid file!") from e
-        except PermissionError as e:
+            self.PathException = exception = ValueError
+            raise exception(f"{file} doesn't exist or isn't a valid file!") from e
+        except (exception := PermissionError) as e:
             message = f"Permission to remove {self._error_helper_compare_path_source(self.name, file)} is denied."
             self.err_logger.warning(message)
+            self.PathException = exception
             raise e
         if verbose:
             self.err_logger.info(f"Deleted: {file}")
 
     def remove(self, parent_only: bool = False, verbose: bool = False) -> None:
         # removes everything (if parent_only is False) found inside a ProperPath except the parent directory of the path
         # if the ProperPath isn't a directory then it just removes the file
@@ -183,50 +219,61 @@
                     ) if verbose else ...
                     # rmtree deletes files and directories recursively.
                     # So in case of permission error with rmtree(ref), shutil.rmtree() might give better
                     # traceback message. I.e., which file or directory exactly
 
     @contextmanager
     def open(
-        self, mode="r", encoding: Union[str, None] = None
+        self,
+        mode="r",
+        encoding: Union[str, None] = None,
+        **kwargs,
     ) -> Generator[TextIO, None, None]:
         path = self.expanded.resolve()
         file: Union[TextIO, None] = None
         try:
             # this try block doesn't yield anything yet. Here, we want to catch possible errors that occur
             # before the file is opened. E.g., FileNotFoundError
-            file: TextIO = path.open(mode=mode, encoding=encoding)
-        except FileNotFoundError as e:
+            file: TextIO = path.open(mode=mode, encoding=encoding, **kwargs)
+        except (exception := FileNotFoundError) as e:
             message = f"File in {path} couldn't be found while trying to open it with mode '{mode}'!"
             self.err_logger.warning(message)
+            self.PathException = exception
             raise e
 
-        except PermissionError as e:
+        except (exception := PermissionError) as e:
             message = (
                 f"Permission denied while trying to open file with mode '{mode}' for "
                 f"{self._error_helper_compare_path_source(self.name, path)}."
             )
             self.err_logger.error(message)
+            self.PathException = exception
 
             try:
                 yield  # Without yield (yield None) Python throws RuntimeError: generator didn't yield.
                 # I.e., contextmanager always expects a yield?
-            except AttributeError as attribute_err:
+            except (exception := AttributeError) as attribute_err:
                 # However, yielding None leads to attribute calls to None
                 # (e.g., yield None -> file = None -> file.read() -> None.read()!! So we also catch that error.
                 attribute_in_error = str(attribute_err).split()[-1]
                 message = (
-                    f"An attempt to access attribute {attribute_in_error} "
-                    f"of the file object was made, "
+                    f"An attempt to access attribute {attribute_in_error} was made,"
                     f"but there was a problem opening the file {path}."
                 )
                 self.err_logger.warning(message)
+                self.PathException = exception
                 raise attribute_err
             else:
                 raise e
+        except (exception := OSError) as os_err:
+            # When an attempt to create a file or directory inside root (e.g., '/foo')
+            # is made, OS can throw OSError with error no. 30 instead of PermissionError.
+            self.err_logger.error(os_err)
+            self.PathException = exception
+            raise os_err
 
         else:
             try:
                 # Now we yield the contextmanager expected yield
                 yield file
             except AttributeError as e:
                 # This is useful for catching AttributeError when the file object is valid but the attributes being
@@ -234,42 +281,49 @@
                 attribute_in_error = str(e).split()[-1]
                 message = (
                     f"An attempt to access unknown/private attribute {attribute_in_error} "
                     f"of the file object {file} was made."
                 )
                 self.err_logger.warning(message)
                 raise e
-            except MemoryError as e:
+            except (exception := MemoryError) as e:
                 message = (
                     f"Out of memory while trying to use mode '{mode}' with "
                     f"{self._error_helper_compare_path_source(self.name, path)}."
                 )
                 self.err_logger.critical(message)
+                self.PathException = exception
                 raise e
-            except IOError as io_err:
+            except (exception := IOError) as io_err:
                 # We catch "No disk space left" error which will likely be triggered during a write attempt on the file
                 if io_err.errno == errno.ENOSPC:
                     message = (
                         f"Not enough disk space left while trying to use mode '{mode}' with "
                         f"{self._error_helper_compare_path_source(self.name, path)}."
                     )
                     self.err_logger.critical(message)
+                    self.PathException = exception
                 raise io_err
+            except (exception := OSError) as os_err:
+                self.err_logger.error(os_err)
+                self.PathException = exception
+                raise os_err
         finally:
             if file:
                 try:
                     file.close()
                 # This behavior was noticed during an experiment with "/dev/full" on Debian/Linux.
                 # f = open("/dev/full", mode="w"); f.write("hello"); <- This won't trigger ENOSPC error yet.
                 # But the error is triggered immediately after when closing with f.close()!*
                 # f = open("/dev/full", mode="w");f.write("hello" * 10_000); <- Opening f again.
                 # The above will trigger ENOSPC error, and will be captured by previous ENOSPC IOError exception.
                 # Because of *, we again need to catch the error during close().
-                except IOError as io_err:
+                except (exception := IOError) as io_err:
                     if io_err.errno == errno.ENOSPC:
                         message = (
                             f"An 'ENOSPC' error (not enough disk space left) is received while trying to"
                             f"close the file before using it with '{mode}'. Data may have been lost."
                             f"{self._error_helper_compare_path_source(self.name, path)}."
                         )
                         self.err_logger.critical(message)
+                    self.PathException = exception
                     raise io_err
```

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/bill_teams/invoice.py` & `elapi-1.0.7.dev2/src/elapi/plugins/bill_teams/invoice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from datetime import datetime
 
-from ...styles import stdin_console
-
 
 class InvoiceGenerator:
     __slots__ = ("data",)
 
     def __init__(self, teams_data: dict):
         self.data = teams_data
 
@@ -21,31 +19,26 @@
     def MONTHLY_FEE(self):
         raise TypeError("MONTHLY_FEE cannot be deleted!")
 
     @staticmethod
     def _template(
         team_id: int,
         team_name: str,
-        owners: list,
         member_count: int,
         bill_amount: int,
     ):
         def _owner_template(owners_: list):
             trunc_owners = [
                 (value["owner_name"], value["owner_email"])
                 for owner in owners_
                 for value in owner.values()
             ]
             return "\n".join([f"|{owner[0]}|{owner[1]}|" for owner in trunc_owners])
 
         return f"""◆ **Team:** {team_name}                      ◇ **Team ID:** {team_id}
-
-|Owner Name| Owner Email|
-|:----------|------------:|
-{_owner_template(owners)}
         
 **Number of members:** {member_count}
 
 **💲 Amount due:** {member_count * bill_amount:.2f} EUR
 
 ---
 
@@ -67,20 +60,16 @@
 """
 
     def generate(self):
         total_bill_amount = 0
         breakdown = """## Breakdown
 
 """
-        with stdin_console.status(status="Generating invoice..."):
-            for team in self.data.values():
-                team_id = team["team_id"]
-                team_name = team["team_name"]
-                owners = team["owners"]
-                member_count = team["members"]["member_count"]
-                bill_amount = 0 if team["on_trial"] else self.MONTHLY_FEE
-                total_bill_amount += bill_amount * member_count
-                team_invoice = self._template(
-                    team_id, team_name, owners, member_count, bill_amount
-                )
-                breakdown += team_invoice
+        for team in self.data.values():
+            team_id = team["team_id"]
+            team_name = team["team_name"]
+            member_count = team["active_member_count"]
+            bill_amount = 0 if team["on_trial"] else self.MONTHLY_FEE
+            total_bill_amount += bill_amount * member_count
+            team_invoice = self._template(team_id, team_name, member_count, bill_amount)
+            breakdown += team_invoice
         return self._header(len(self.data.values()), total_bill_amount) + breakdown
```

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/experiments/cli.py` & `elapi-1.0.7.dev2/src/elapi/plugins/experiments/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Annotated, Optional
 
 import typer
 
 from ._doc import __PARAMETERS__doc__ as docs
 from ...cli.doc import __PARAMETERS__doc__ as elapi_docs
-from ...cli.helpers import CLIExport, CLIFormat, OrderedCommands
 from ...loggers import Logger
+from ...plugins.commons.cli_helpers import CLIExport, CLIFormat, OrderedCommands
 from ...plugins.experiments.experiments import (
     ExperimentIDValidator,
     FixedExperimentEndpoint,
     append_to_experiment,
 )
 from ...styles import stdin_console, stderr_console
 from ...validators import ValidationError
@@ -31,17 +31,15 @@
 @app.command(short_help="Read or download an experiment.")
 def get(
     experiment_id: Annotated[
         str, typer.Option("--id", "-i", help=docs["experiment_id"], show_default=False)
     ],
     data_format: Annotated[
         Optional[str],
-        typer.Option(
-            "--format", "-F", help=elapi_docs["data_format"], show_default=False
-        ),
+        typer.Option("--format", "-F", help=docs["data_format"], show_default=False),
     ] = None,
     export: Annotated[
         Optional[bool],
         typer.Option(
             "--export",
             "-e",
             help=elapi_docs["export"] + elapi_docs["export_details"],
@@ -52,15 +50,15 @@
     ] = False,
     _export_dest: Annotated[Optional[str], typer.Argument(hidden=True)] = None,
 ) -> dict:
     """
     Read or download an experiment.
     """
     from ...validators import Validate, HostIdentityValidator
-    from ..utils import Export
+    from ..commons import Export
     from ...styles import Highlight
     from . import (
         formats,
     )  # must be imported for all formats to be registered by BaseFormat
 
     validate_config = Validate(HostIdentityValidator())
     validate_config()
@@ -258,15 +256,15 @@
     ] = False,
     _export_dest: Annotated[Optional[str], typer.Argument(hidden=True)] = None,
 ) -> None:
     """
     Download an attachment from an experiment.
     """
     from ...validators import Validate, HostIdentityValidator
-    from ...plugins.utils import Export
+    from ...plugins.commons import Export
     from .experiments import download_attachment
 
     validate_config = Validate(HostIdentityValidator())
     validate_config()
 
     if export is False:
         _export_dest = None
@@ -284,15 +282,15 @@
                 attachment_name,
                 attachment_extension,
                 attachment_hash,
                 attachment_creation_date,
             ) = download_attachment(experiment_id, attachment_id)
         except ValueError as e:
             logger.error(e)
-            typer.Exit(1)
+            raise typer.Exit(1)
         else:
             data_format, export_dest, export_file_ext = CLIExport(
                 attachment_extension, _export_dest
             )
             _is_real_id = attachment_id == attachment_real_id
             if export:
                 if export_file_ext and export_file_ext != attachment_extension:
```

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/experiments/experiments.py` & `elapi-1.0.7.dev2/src/elapi/plugins/experiments/experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,25 +52,25 @@
         if re.match(r"^\d+-\w+$", self.experiment_id, re.IGNORECASE):
             try:
                 elab_id = (
                     _experiment_data := self._experiment_endpoint.get(
                         query={"q": self.experiment_id}
                     ).json()[0]
                 )["elabid"]
-            except KeyError:
+            except (KeyError, IndexError):
                 self._experiment_endpoint.close()
                 raise ValidationError(
-                    f"Experiment ID '{self.experiment_id}' could not be found!"
+                    f"Experiment ID (detected as Unique eLabID) '{self.experiment_id}' could not be found!"
                 )
             else:
                 self._experiment_endpoint.close()
                 if elab_id == self.experiment_id:
                     return _experiment_data["id"]
                 raise ValidationError(
-                    f"Experiment ID '{self.experiment_id}' could not be found!"
+                    f"Experiment ID (detected as Unique eLabID) '{self.experiment_id}' could not be found!"
                 )
         raise ValidationError(
             f"Experiment ID '{self.experiment_id}' could not be validated "
             "because it didn't match any valid pattern for experiment IDs!"
         )
```

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/experiments/formats.py` & `elapi-1.0.7.dev2/src/elapi/plugins/experiments/formats.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/show_config.py` & `elapi-1.0.7.dev2/src/elapi/plugins/show_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,56 +60,56 @@
 
 - {ColorText('Log file path').colorize(LIGHTGREEN)}: {LOG_FILE_PATH}
 """
         + (
             f"- {ColorText('Host address').colorize(LIGHTGREEN)}"
             + (
                 f" **[{ColorText(KEY_HOST.lower()).colorize(YELLOW)}]**"
-                if no_keys
+                if not no_keys
                 else ""
             )
             + ":"
             + (
                 f" {host_value} ← `{host_source}`"
                 if host_source
                 else f" _{host_value.colorize(RED)}_\n"
             )
         )
         + "\n"
         + (
             f"- {ColorText('API Token').colorize(LIGHTGREEN)}"
             + (
                 f" **[{ColorText(KEY_API_TOKEN.lower()).colorize(YELLOW)}]**"
-                if no_keys
+                if not no_keys
                 else ""
             )
             + ":"
             + (
                 f" {api_token_masked} ← `{api_token_source}`"
                 if api_token_source
                 else f" _{api_token_masked.colorize(RED)}_\n"
             )
         )
         + "\n"
         + f"- {ColorText('Export directory').colorize(LIGHTGREEN)}"
         + (
             f" **[{ColorText(KEY_EXPORT_DIR.lower()).colorize(YELLOW)}]**"
-            if no_keys
+            if not no_keys
             else ""
         )
         + f": {EXPORT_DIR} ← `{export_dir_source}`"
         + f"""
 - {ColorText('App data directory').colorize(LIGHTGREEN)}: {APP_DATA_DIR}
 - {ColorText('Caching directory').colorize(LIGHTGREEN)}: {TMP_DIR}
 """
         + "\n"
         + f"- {ColorText('Unsafe API token use warning').colorize(LIGHTGREEN)}"
         + (
             f" **[{ColorText(KEY_UNSAFE_TOKEN_WARNING.lower()).colorize(YELLOW)}]**"
-            if no_keys
+            if not no_keys
             else ""
         )
         + f": {unsafe_token_use_value} ← `{unsafe_token_use_source}`"
         + f"""
 
 
 {ColorText("Detected configuration files that are in use:").colorize(BLUE)}
```

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/utils/export.py` & `elapi-1.0.7.dev2/src/elapi/plugins/commons/export.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/plugins/utils/get_location_from_headers.py` & `elapi-1.0.7.dev2/src/elapi/plugins/commons/get_location_from_headers.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/styles/_markdown_doc.py` & `elapi-1.0.7.dev2/src/elapi/styles/_markdown_doc.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/styles/_missing.py` & `elapi-1.0.7.dev2/src/elapi/styles/_missing.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/styles/colors.py` & `elapi-1.0.7.dev2/src/elapi/styles/colors.py`

 * *Files identical despite different names*

### Comparing `elapi-1.0.7.dev1/src/elapi/styles/highlight.py` & `elapi-1.0.7.dev2/src/elapi/styles/highlight.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 class BaseHighlight(ABC):
     @classmethod
     def __subclasshook__(cls, subclass) -> bool:
         return issubclass(subclass, Syntax) or super().__subclasshook__(cls, subclass)
 
     @abstractmethod
-    def __call__(self, *args, **kwargs):
-        ...
+    def __call__(self, *args, **kwargs): ...
 
 
 class Highlight(BaseHighlight):
     def __init__(self, language: str, /, theme: str = "lightbulb"):
         validator = ValidateLanguage(language)
         self.name = validator.name
         self.theme = theme
@@ -52,7 +51,16 @@
             raise TypeError(
                 "text value must be an object that implements '__str__' attribute!"
             )
         self._text = str(value)
 
     def colorize(self, ansi_color: str) -> str:
         return f"{ansi_color}{self.text}{Fore.RESET}"
+
+
+def print_typer_error(error_message: str) -> None:
+    import click
+    from typer.rich_utils import rich_format_error
+
+    exception = click.ClickException(error_message)
+    exception.ctx = click.get_current_context()
+    rich_format_error(exception)
```

### Comparing `elapi-1.0.7.dev1/src/elapi/validators/base.py` & `elapi-1.0.7.dev2/src/elapi/validators/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,47 @@
+import sys
 from abc import abstractmethod, ABC
 from typing import Any
 
 import typer
 
 
-class ValidationError(Exception):
-    ...
+class ValidationError(Exception): ...
 
 
 class RuntimeValidationError(typer.Exit):
     def __init__(self, *args) -> None:
         super().__init__(*args or (1,))  # default error code is always 1
 
 
-class CriticalValidationError(BaseException):
-    SYSTEM_EXIT: bool = True
+class Exit(BaseException):
+    if (
+        hasattr(sys, "ps1")
+        or hasattr(sys, "ps2")
+        or sys.modules.get(
+            "ptpython", False
+        )  # hasattr(sys, "ps1") doesn't work with ptpython.
+        or sys.modules.get("bpython", False)
+    ):
+        SYSTEM_EXIT: bool = False
+    else:
+        SYSTEM_EXIT: bool = True
 
     def __new__(cls, *args, **kwargs):
         if cls.SYSTEM_EXIT:
             return SystemExit(*args)
         return super().__new__(cls, *args, **kwargs)  # cls == CriticalValidationError
 
 
+class CriticalValidationError(Exit): ...
+
+
 class Validator(ABC):
     @abstractmethod
-    def validate(self):
-        ...
+    def validate(self): ...
 
 
 class Validate:
     def __init__(self, *_typ: (Validator, ...)):
         self.typ = _typ
 
     def __call__(self, *args, **kwargs) -> None:
```

### Comparing `elapi-1.0.7.dev1/src/elapi/validators/identity.py` & `elapi-1.0.7.dev2/src/elapi/validators/identity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from json import JSONDecodeError
+from typing import Union, Iterable
 
 import httpx
 
 from .base import Validator, RuntimeValidationError, CriticalValidationError
 from ..styles import stdin_console
 from ..styles.highlight import NoteText
 
@@ -17,14 +18,35 @@
     TimeoutError,
 )
 
 
 class HostIdentityValidator(Validator):
     __slots__ = ()
 
+    def __init__(self, restrict_to: Union[str, Iterable[str], None] = None):
+        self.restrict_to = restrict_to
+
+    @property
+    def restrict_to(self) -> Iterable[str]:
+        return self._restrict_to
+
+    @restrict_to.setter
+    def restrict_to(self, value):
+        if value is None:
+            self._restrict_to = None
+        elif isinstance(value, str):
+            self._restrict_to = [value]
+        elif isinstance(value, Iterable):
+            self._restrict_to = value
+        else:
+            raise AttributeError(
+                "restrict_to must be a string of target host URL, or an iterable of strings where "
+                f"each string is a host URL that {HostIdentityValidator.__name__} validation will be restricted to."
+            )
+
     @staticmethod
     def check_endpoint():
         from ..api import GETRequest
 
         session = GETRequest()
         return session(endpoint_name="apikeys", endpoint_id=None)
 
@@ -50,36 +72,57 @@
                     "Host is the URL of the root API endpoint. Example:"
                     f"\n{_HOST_EXAMPLE}",
                 )
             )
             raise CriticalValidationError
         else:
             if not HOST:
-                logger.critical("'host' is detected on configuration file but it's empty.")
+                logger.critical(
+                    "'host' is detected on configuration file but it's empty."
+                )
                 stdin_console.print(
                     NoteText(
                         "Host contains the URL of the root API endpoint. Example:"
                         f"\n{_HOST_EXAMPLE}",
                     )
                 )
                 raise CriticalValidationError
-
+        if self.restrict_to is not None:
+            if HOST not in self.restrict_to:
+                logger.error(
+                    "Detected 'host' is different from the restricted host. 'host' could not be validated!"
+                )
+                try:
+                    stdin_console.print(
+                        NoteText(
+                            f"Detected 'host': '{HOST}'. "
+                            f"Host(s) restricted by {HostIdentityValidator.__name__}: '{', '.join(self.restrict_to)}'."
+                        )
+                    )
+                except TypeError as e:
+                    raise ValueError(
+                        f"An invalid value might have been given to restrict_to "
+                        f"attribute of {HostIdentityValidator.__name__}. Validation could not be completed!"
+                    ) from e
+                raise CriticalValidationError
         try:
             inspect.applied_config[KEY_API_TOKEN]
         except KeyError:
             logger.critical("'api_token' is missing from configuration file.")
             stdin_console.print(
                 NoteText(
                     "An API token with at least read-access is required to make requests."
                 )
             )
             raise CriticalValidationError
         else:
             if not API_TOKEN:
-                logger.critical("'api_token' is detected on configuration file but it's empty.")
+                logger.critical(
+                    "'api_token' is detected on configuration file but it's empty."
+                )
                 stdin_console.print(
                     NoteText(
                         "An API token with at least read-access is required to make requests.",
                     )
                 )
                 raise CriticalValidationError
```

### Comparing `elapi-1.0.7.dev1/src/elapi/validators/path.py` & `elapi-1.0.7.dev2/src/elapi/validators/path.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,14 @@
 from pathlib import Path
 from random import choices
 from typing import Union, Iterable
 
 from .base import Validator, ValidationError
 from ..path import ProperPath
 
-COMMON_PATH_ERRORS: tuple = (
-    FileNotFoundError,
-    PermissionError,
-    MemoryError,
-    IOError,
-    ValueError,
-    AttributeError,
-)
-
 
 class PathValidator(Validator):
     def __init__(
         self,
         path: Union[Iterable, Union[None, str, ProperPath, Path]],
         **kwargs,
     ):
@@ -50,28 +41,31 @@
     def validate(self):
         for p in self.path:
             if not isinstance(p, ProperPath):
                 try:
                     p = ProperPath(p, err_logger=self.err_logger)
                 except (ValueError, TypeError):
                     continue
+            p_child = (
+                ProperPath(p / self.TMP_FILE, kind="file", err_logger=self.err_logger)
+                if p.kind == "dir"
+                else p
+            )
             try:
                 p.create()
-                with (p / self.TMP_FILE if p.kind == "dir" else p).open(
-                    mode="ba+"
-                ) as f:
+                with p_child.open(mode="ba+") as f:
                     f.write(
                         b"\x06"
                     )  # Throwback: \x06 is the ASCII "Acknowledge" character
                     f.seek(f.tell() - 1)
                     if (
                         not f.read(1) == b"\x06"
                     ):  # This checks for /dev/null-type special files!
                         continue  # It'd not be possible to read from those files.
                     f.seek(f.tell() - 1)
                     f.truncate()
-            except COMMON_PATH_ERRORS:
+            except (p.PathException, p_child.PathException, ValueError, AttributeError):
                 continue
             else:
-                (p / self.TMP_FILE).remove() if p.kind == "dir" else ...
+                p_child.remove() if p.kind == "dir" else ...
                 return p.expanded
         raise ValidationError("Given path(s) could not be validated!")
```

### Comparing `elapi-1.0.7.dev1/PKG-INFO` & `elapi-1.0.7.dev2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: elapi
-Version: 1.0.7.dev1
-Summary: elAPI is a powerful, extensible API interface to eLabFTW built for the University Computing Centre (URZ, FIRE division) at Universität Heidelberg.
+Version: 1.0.7.dev2
+Summary: elAPI is a powerful, extensible API client for eLabFTW.
 Home-page: https://www.urz.uni-heidelberg.de/en/service-catalogue/software-and-applications/elabftw
 License: AGPL-3.0-only
 Keywords: elabftw,api
 Author: Alexander Haller
 Author-email: alexander.haller@urz.uni-heidelberg.de
 Maintainer: Mahadi Xion
 Maintainer-email: mahadi.xion@urz.uni-heidelberg.de
@@ -34,15 +34,18 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # elAPI
 
-elAPI is a powerful, extensible API interface to eLabFTW. It supports serving almost all kinds of requests documented in
+elAPI is a powerful, extensible API client for eLabFTW built for
+the [University Computing Centre](https://www.urz.uni-heidelberg.de/en) (
+URZ, [FIRE](https://www.urz.uni-heidelberg.de/en/node/64/organisation/future-it-research-education) division) at
+Universität Heidelberg. It supports serving almost all kinds of requests documented on
 [eLabFTW API documentation](https://doc.elabftw.net/api/v2/) with ease. elAPI treats eLabFTW API endpoints as its
 arguments.
 
 **Example:**
 
 From [the documentation](https://doc.elabftw.net/api/v2/#/Users/read-user):
 > GET /users/{id}
@@ -51,133 +54,186 @@
 
 ```sh
 $ elapi get users --id <id>
 ```
 
 ## Installation
 
-Support for installing packages with `pip install --user` has been deprecated with the adoption of [PEP 688](https://peps.python.org/pep-0668/) on many systems like [Debian 12](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1030335#5).
-We recommend [`pipx`](https://pipx.pypa.io/stable/) for installing elAPI.
+elAPI can be used both as a CLI tool and as a Python library. If you are interested in simply using elAPI's
+off-the-shelf features from the command-line, install elAPI as a CLI tool. If you intend to write automation script for
+eLabFTW, you should install elAPI as a library inside a virtual environment. Of course, if you're interested in
+both, you can have elAPI installed in both ways.
+
+### Install elAPI as a CLI tool
+
+Support for installing Python packages with `pip install --user` has been deprecated with the adoption
+of [PEP 688](https://peps.python.org/pep-0668/) on many systems
+like [Debian 12](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1030335#5).
+We recommend [`pipx`](https://pipx.pypa.io/stable/) for installing elAPI for use of its CLI functionalities. Pipx
+installs packages in isolated virtual environments, so Pipx-installed elAPI should not conflict with elAPI installed
+inside other virtual environments.
 
 ```shell
 $ pipx install elapi
 ```
 
-Of course, `pip install --user elapi` might continue to work on some systems.
+After installation with Pipx is complete, you would also be able to run elAPI just by entering the `elapi` command on
+the
+terminal.
+
+### Install elAPI as a library
+
+It is recommended to install elAPI inside a Python virtual environment for use of its rich APIs for
+working with eLabFTW. From inside a virtual environment, elAPI CLI can be invoked with `python -m elapi.cli`.
+At the moment, though, the documentation about using elAPI as a library is severely lacking.
 
 ## Configuration
 
-elAPI needs to be configured first before we can do anything useful with it. elAPI supports a YAML configuration file in
+elAPI needs to be configured first before you can do anything useful with it. Mainly, elAPI needs to know your eLabFTW
+server's API URL and your API key (or token) for access.
+
+### Quick configuration
+
+You can run `elapi init` to simplify the configuration process. You will be prompted with questions
+about your eLabFTW server with examples to help you fill in the answers.
+
+### Advanced configuration
+
+elAPI supports a YAML configuration file in
 the following locations.
 
 - Current directory: `./elapi.yml`
 - User directory: `$HOME/.config/elapi.yml`
 - Root directory: `/etc/elapi.yml`
 
 elAPI supports configuration overloading. I.e., a keyword set in root configuration file `/etc/elapi.yml` can be
-overriden by setting a different value in user configuration file `$HOME/.config/elapi.yml`. In terms of precedence,
+overridden by setting a different value in user configuration file `$HOME/.config/elapi.yml`. In terms of precedence,
 configuration file present in the currently active directory has the highest priority, and configuration in root
 directory has the lowest.
 
 The following parameters are currently configurable, with `host` and `api_token` being the required fields. For testing
-purposes it would be safe to store everything in the user configuration file.
+purposes it would be safe to store everything in `$HOME/.config/elapi.yml`.
 
 ```yaml
 # elAPI configuration
 # Saved in `$HOME/.config/elapi.yml`
 
 host: <host API url>
 # Example: https://demo.elabftw.net/api/v2/
 # Note the host URL ends with the API endpoint
 api_token: <token with at least read-access>
 # You can generate an API token from eLabFTW user panel -> API keys tab.
 export_dir: ~/Downloads/elAPI
 unsafe_api_token_warning: yes
 ```
 
-We can get an overview of detected configurations.
+You can get an overview of detected configurations.
 
 ```shell
 $ elapi show-config
 ```
 
-If both `host` and `api_token` are detected, we are good to go!
+If both `host` and `api_token` are detected, you are good to go!
 
 ## Usage
 
 elAPI can be invoked from the command-line.
 
 ```shell
 $ elapi --help 
 ```
 
 ### `GET` requests
 
-We can request an overview of running eLabFTW server.
+Request an overview of running eLabFTW server:
 
 ```shell
 $ elapi get info -F yml
 # Here -F (or --format) defines the output format
 ```
 
-We can request a list o all active experiments and export it to a `JSON` file.
+You can request a list o all active experiments and export it to a `JSON` file.
 
 ```shell
 $ elapi get experiments --export ~/Downoads/experiments.json
 ```
 
 ### `POST` requests
 
-We can create a new user by the name 'John Doe'.
+Create a new user by the name 'John Doe':
 
 ```shell
 $ elapi post users --id <user id> -d '{"firstname": "John", "lastname": "Doe", "email": "test_test@itnerd.de"}'
 ```
 
 ### `PATCH` requests
 
-We can update an existing user's email address.
+Update an existing user's email address:
 
 ```shell
 $ elapi patch users --id <user id> -d '{"email": "new_email@itnerd.de"}'
 ```
 
-`patch` command allows us to make changes to eLabFTW server settings. E.g., we can update the time (in minutes)
+`patch` command allows us to make changes to eLabFTW server settings. E.g., you can update the time (in minutes)
 after which the authentication cookie will expire.
 
 ```shell
 $ elapi patch config -d '{"cookie_validity_time": 43200}'
 ```
 
-We can publish an announcement to all the members.
+You can publish an announcement to all the members.
 
 ```shell
 $ elapi patch config -d '{"announcement": "Notice: Server will be down tomorrow at midnight due to scheduled maintenance."}'
 ```
 
-### Bill teams
+### `DELETE` requests
 
-We can generate invoice for eLabFTW teams.
+Delete all the tags associated to an experiment:
 
 ```shell
-$ elapi bill-teams generate-invoice
+$ elapi delete experiments -i <experiment ID> --sub tags
 ```
 
-We may just want to have a look at the billing information without generating invoice.
+You can reset the configuration to default values.
 
 ```shell
-$ elapi bill-teams info -F yaml
+$ elapi delete config
 ```
 
-We can also export this information as a `YAML` file to the export directory defined in configuration
-file (`export_dir`).
+### `experiments` plugin
+
+`experiments` plugin enables experiments-specific actions. You can download an experiment in PDF by its "Unique eLabID"
+to `~/Downloads` directory.
 
 ```shell
-elapi bill-teams info -F yaml --export
+$ elapi experiments get -i <experiment unique elabid> -F pdf --export ~/Downloads/
 ```
 
+Append text in markdown to an existing experiment by its ID:
+
+```shell
+$ elapi experiments append --id <experiment ID> -M -t "**New content.**"
+```
+
+You can also upload an attachment to an experiment.
+
+```shell
+$ elapi experiments upload-attachment --id <experiment ID> --path <path to attachment file> --comment <comment for your attachment>
+```
+
+### Bill teams
+
+You can get a list of all teams and its users for billing purposes and export it to home directory.
+
+```shell
+$ elapi bill-teams teams-info --export ~
+```
+
+Most sub-commands available under `elapi bill-teams` plugin are for Universität Heidelberg specific use-cases.
+
 ## Open-source
 
 elAPI is open-source and published under AGPLv3 license. The repository is however hosted internally within
 Universität Heidelberg's network. The codebase can still be accessed from [PyPI](https://pypi.org/project/elapi/#files).
 If you express interest in having the repository made completely public, or if you have any question, feel free
 to [contact us](mailto:elabftw@uni-heidelberg.de).
```

