# Comparing `tmp/adafruit-circuitpython-httpserver-4.5.7.tar.gz` & `tmp/adafruit_circuitpython_httpserver-4.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-4.5.7.tar", last modified: Mon Apr  1 15:19:35 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_httpserver-4.5.8.tar", last modified: Mon Apr 15 15:54:51 2024, max compression
```

## Comparing `adafruit-circuitpython-httpserver-4.5.7.tar` & `adafruit_circuitpython_httpserver-4.5.8.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.083020 adafruit-circuitpython-httpserver-4.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.087020 adafruit-circuitpython-httpserver-4.5.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 15:19:35.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.091020 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    28371 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.095020 adafruit-circuitpython-httpserver-4.5.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.095020 adafruit-circuitpython-httpserver-4.5.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/examples/directory_listing.tpl.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/examples/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_ethernet_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_form_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_handler_serves_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_multiple_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_redirects.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_connectionmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_static_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/examples/settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-01 15:19:32.000000 adafruit-circuitpython-httpserver-4.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 15:19:23.000000 adafruit-circuitpython-httpserver-4.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:19:35.099020 adafruit-circuitpython-httpserver-4.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.498462 adafruit_circuitpython_httpserver-4.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.486462 adafruit_circuitpython_httpserver-4.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.486462 adafruit_circuitpython_httpserver-4.5.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.486462 adafruit_circuitpython_httpserver-4.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.490462 adafruit_circuitpython_httpserver-4.5.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 15:54:51.498462 adafruit_circuitpython_httpserver-4.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.498462 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 15:54:51.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-15 15:54:51.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:54:51.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 15:54:51.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 15:54:51.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.490462 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28371 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.494462 adafruit_circuitpython_httpserver-4.5.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.494462 adafruit_circuitpython_httpserver-4.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/starting_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/docs/starting_methods.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:54:51.498462 adafruit_circuitpython_httpserver-4.5.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/examples/directory_listing.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_form_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_auto_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_auto_settings_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_manual_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_manual_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_manual_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_start_and_poll_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-15 15:54:48.000000 adafruit_circuitpython_httpserver-4.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 15:54:40.000000 adafruit_circuitpython_httpserver-4.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:54:51.498462 adafruit_circuitpython_httpserver-4.5.8/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_httpserver-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/.gitignore` & `adafruit_circuitpython_httpserver-4.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/.pre-commit-config.yaml` & `adafruit_circuitpython_httpserver-4.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/.pylintrc` & `adafruit_circuitpython_httpserver-4.5.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_httpserver-4.5.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/LICENSE` & `adafruit_circuitpython_httpserver-4.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_httpserver-4.5.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/LICENSES/MIT.txt` & `adafruit_circuitpython_httpserver-4.5.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/LICENSES/Unlicense.txt` & `adafruit_circuitpython_httpserver-4.5.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/PKG-INFO` & `adafruit_circuitpython_httpserver-4.5.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.5.7
+Version: 4.5.8
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/README.rst` & `adafruit_circuitpython_httpserver-4.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.5.7
+Version: 4.5.8
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,35 +38,38 @@
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
+docs/starting_methods.rst
+docs/starting_methods.rst.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/directory_listing.tpl.html
 examples/home.html
 examples/httpserver_authentication_handlers.py
 examples/httpserver_authentication_server.py
 examples/httpserver_chunked.py
 examples/httpserver_cookies.py
 examples/httpserver_cpu_information.py
 examples/httpserver_cpython.py
-examples/httpserver_ethernet_simpletest.py
 examples/httpserver_form_data.py
 examples/httpserver_handler_serves_file.py
 examples/httpserver_mdns.py
 examples/httpserver_methods.py
 examples/httpserver_multiple_servers.py
 examples/httpserver_neopixel.py
 examples/httpserver_redirects.py
-examples/httpserver_simpletest_auto.py
-examples/httpserver_simpletest_connectionmanager.py
-examples/httpserver_simpletest_manual.py
+examples/httpserver_simpletest_auto_connection_manager.py
+examples/httpserver_simpletest_auto_settings_toml.py
+examples/httpserver_simpletest_manual_ap.py
+examples/httpserver_simpletest_manual_ethernet.py
+examples/httpserver_simpletest_manual_wifi.py
 examples/httpserver_sse.py
 examples/httpserver_start_and_poll.py
 examples/httpserver_start_and_poll_asyncio.py
 examples/httpserver_static_files_serving.py
 examples/httpserver_templates.py
 examples/httpserver_url_parameters.py
 examples/httpserver_websocket.py
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/__init__.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "4.5.7"
+__version__ = "4.5.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
 
 
 from .authentication import (
     Basic,
     Token,
     Bearer,
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/authentication.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/authentication.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/exceptions.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/headers.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/interfaces.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/interfaces.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/mime_types.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/mime_types.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/request.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/response.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/response.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/route.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/route.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/server.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/adafruit_httpserver/status.py` & `adafruit_circuitpython_httpserver-4.5.8/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/docs/_static/favicon.ico` & `adafruit_circuitpython_httpserver-4.5.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/docs/api.rst` & `adafruit_circuitpython_httpserver-4.5.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/docs/conf.py` & `adafruit_circuitpython_httpserver-4.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/docs/examples.rst` & `adafruit_circuitpython_httpserver-4.5.8/docs/examples.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,25 @@
-Simple Test
------------
+.. note::
+    All examples in this document are using ``Server`` in ``debug`` mode.
+    This mode is useful for development, but it is not recommended to use it in production.
+    More about Debug mode at the end of Examples section.
 
-**All examples in this document are using** ``Server`` **in** ``debug`` **mode.**
-**This mode is useful for development, but it is not recommended to use it in production.**
-**More about Debug mode at the end of Examples section.**
+Different ways of starting the server
+-------------------------------------
 
-This is the minimal example of using the library with CircuitPython.
-This example is serving a simple static text message.
+There are several ways to start the server on CircuitPython, mostly depending on the device you are using and
+whether you have access to external network.
 
-It also manually connects to the WiFi network.
+Functionally, all of them are the same, not features of the server are limited or disabled in any way.
 
-.. literalinclude:: ../examples/httpserver_simpletest_manual.py
-    :caption: examples/httpserver_simpletest_manual.py
-    :emphasize-lines: 12-17
-    :linenos:
-
-It is also possible to use Ethernet instead of WiFi.
-The only difference in usage is related to configuring the ``socket_source`` differently.
-
-.. literalinclude:: ../examples/httpserver_ethernet_simpletest.py
-    :caption: examples/httpserver_ethernet_simpletest.py
-    :emphasize-lines: 13-23
-    :linenos:
-
-Although there is nothing wrong with this approach, from the version 8.0.0 of CircuitPython,
-`it is possible to use the environment variables <https://docs.circuitpython.org/en/latest/docs/environment.html#circuitpython-behavior>`_
-defined in ``settings.toml`` file to store secrets and configure the WiFi network.
-
-By default the library uses ``0.0.0.0`` and port ``5000`` for the server, as port ``80`` is reserved for the CircuitPython Web Workflow.
-If you want to use port ``80`` , you need to set ``CIRCUITPY_WEB_API_PORT`` to any other port, and then set ``port`` parameter in ``Server`` constructor to ``80`` .
+Below you can find examples of different ways to start the server:
 
-This is the same example as above, but it uses the ``settings.toml`` file to configure the WiFi network.
+.. toctree::
 
-**From now on, all the examples will use the** ``settings.toml`` **file to configure the WiFi network.**
-
-.. literalinclude:: ../examples/settings.toml
-    :caption: settings.toml
-    :lines: 5-
-    :linenos:
-
-Note that we still need to import ``socketpool`` and ``wifi`` modules.
-
-.. literalinclude:: ../examples/httpserver_simpletest_auto.py
-    :caption: examples/httpserver_simpletest_auto.py
-    :emphasize-lines: 11
-    :linenos:
+    starting_methods
 
 CPython usage
 --------------------
 
 Library can also be used in CPython, no changes other than changing the ``socket_source`` are necessary.
 
 .. literalinclude:: ../examples/httpserver_cpython.py
@@ -206,15 +177,15 @@
     :language: django
     :lines: 9-
     :emphasize-lines: 1-2,6,10,15-23,27
     :linenos:
 
 .. literalinclude:: ../examples/httpserver_templates.py
     :caption: examples/httpserver_templates.py
-    :emphasize-lines: 12-15,49-55
+    :emphasize-lines: 12-15,51-59
     :linenos:
 
 Form data parsing
 ---------------------
 
 Another way to pass data to the handler function is to use form data.
 Remember that it is only possible to use it with ``POST`` method.
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/docs/index.rst` & `adafruit_circuitpython_httpserver-4.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/directory_listing.tpl.html` & `adafruit_circuitpython_httpserver-4.5.8/examples/directory_listing.tpl.html`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_handlers.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_authentication_handlers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_authentication_server.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_authentication_server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_chunked.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cookies.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpu_information.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_cpython.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_ethernet_simpletest.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_manual_ethernet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # SPDX-FileCopyrightText: 2023 Tim C for Adafruit Industries
+#
 # SPDX-License-Identifier: MIT
 
 import board
 import digitalio
 
 from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
+from adafruit_wiznet5k import adafruit_wiznet5k_socket as socket
 from adafruit_httpserver import Server, Request, Response
 
-print("Wiznet5k HTTPServer Test")
 
 # For Adafruit Ethernet FeatherWing
 cs = digitalio.DigitalInOut(board.D10)
+
 # For Particle Ethernet FeatherWing
 # cs = digitalio.DigitalInOut(board.D5)
+
 spi_bus = board.SPI()
 
 # Initialize ethernet interface with DHCP
 eth = WIZNET5K(spi_bus, cs)
 
 # Set the interface on the socket source
 socket.set_interface(eth)
 
-# Initialize the server
 server = Server(socket, "/static", debug=True)
 
 
 @server.route("/")
 def base(request: Request):
     """
     Serve a default static plain text message.
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_form_data.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_form_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_handler_serves_file.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_handler_serves_file.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_mdns.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_methods.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_multiple_servers.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_multiple_servers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_neopixel.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_redirects.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_redirects.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_auto.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_auto_settings_toml.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_simpletest_manual.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_simpletest_manual_ap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2024 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
-import os
-
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response
 
-ssid = os.getenv("WIFI_SSID")
-password = os.getenv("WIFI_PASSWORD")
 
-print("Connecting to", ssid)
-wifi.radio.connect(ssid, password)
-print("Connected to", ssid)
+AP_SSID = "..."
+AP_PASSWORD = "..."
+
+print("Creating access point...")
+wifi.radio.start_ap(ssid=AP_SSID, password=AP_PASSWORD)
+print(f"Created access point {AP_SSID}")
 
 pool = socketpool.SocketPool(wifi.radio)
 server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
 def base(request: Request):
     """
     Serve a default static plain text message.
     """
     return Response(request, "Hello from the CircuitPython HTTP Server!")
 
 
-server.serve_forever(str(wifi.radio.ipv4_address))
+server.serve_forever(str(wifi.radio.ipv4_address_ap))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_sse.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_sse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_start_and_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_start_and_poll_asyncio.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_start_and_poll_asyncio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_static_files_serving.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_static_files_serving.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_templates.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_templates.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_url_parameters.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_url_parameters.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/examples/httpserver_websocket.py` & `adafruit_circuitpython_httpserver-4.5.8/examples/httpserver_websocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.5.7/pyproject.toml` & `adafruit_circuitpython_httpserver-4.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "4.5.7"
+version = "4.5.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

