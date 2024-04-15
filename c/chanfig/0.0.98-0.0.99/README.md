# Comparing `tmp/chanfig-0.0.98.tar.gz` & `tmp/chanfig-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanfig-0.0.98.tar", last modified: Thu Mar 28 13:13:42 2024, max compression
+gzip compressed data, was "chanfig-0.0.99.tar", last modified: Mon Apr 15 13:10:54 2024, max compression
```

## Comparing `chanfig-0.0.98.tar` & `chanfig-0.0.99.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.152243 chanfig-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 13:13:36.000000 chanfig-0.0.98/.codespell-whitelist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.128244 chanfig-0.0.98/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-28 13:13:36.000000 chanfig-0.0.98/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.128244 chanfig-0.0.98/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-28 13:13:36.000000 chanfig-0.0.98/.github/workflows/push.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     7031 2024-03-28 13:13:36.000000 chanfig-0.0.98/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-28 13:13:36.000000 chanfig-0.0.98/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.132243 chanfig-0.0.98/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.AGPL
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.Apache
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.BSD
--rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.GPLv2
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.GPLv3
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-28 13:13:36.000000 chanfig-0.0.98/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-03-28 13:13:42.152243 chanfig-0.0.98/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    11142 2024-03-28 13:13:36.000000 chanfig-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-03-28 13:13:36.000000 chanfig-0.0.98/README.zh.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.132243 chanfig-0.0.98/chanfig/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2329 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-28 13:13:41.000000 chanfig-0.0.98/chanfig/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20268 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/configclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/default_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    48291 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/flat_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    30651 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-03-28 13:13:36.000000 chanfig-0.0.98/chanfig/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.152243 chanfig-0.0.98/chanfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-03-28 13:13:42.000000 chanfig-0.0.98/chanfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-28 13:13:42.000000 chanfig-0.0.98/chanfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:13:42.000000 chanfig-0.0.98/chanfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 13:13:42.000000 chanfig-0.0.98/chanfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 13:13:42.000000 chanfig-0.0.98/chanfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-28 13:13:36.000000 chanfig-0.0.98/demo/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-28 13:13:36.000000 chanfig-0.0.98/demo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-28 13:13:36.000000 chanfig-0.0.98/demo/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/docs/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/configclass.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/default_dict.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/flat_dict.md
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/functional.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/index.zh.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/nested_dict.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/parser.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/registry.md
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/utils.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/docs/variable.md
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.128244 chanfig-0.0.98/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.136243 chanfig-0.0.98/docs/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.148244 chanfig-0.0.98/docs/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.148244 chanfig-0.0.98/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.152243 chanfig-0.0.98/docs/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-28 13:13:36.000000 chanfig-0.0.98/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-28 13:13:36.000000 chanfig-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-28 13:13:36.000000 chanfig-0.0.98/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:13:42.152243 chanfig-0.0.98/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-28 13:13:36.000000 chanfig-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:13:42.152243 chanfig-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/interpolate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_configclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_flat_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_nested_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-28 13:13:36.000000 chanfig-0.0.98/tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-28 13:13:36.000000 chanfig-0.0.98/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.852487 chanfig-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 13:10:51.000000 chanfig-0.0.99/.codespell-whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.824487 chanfig-0.0.99/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 13:10:51.000000 chanfig-0.0.99/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.828487 chanfig-0.0.99/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-15 13:10:51.000000 chanfig-0.0.99/.github/workflows/push.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7031 2024-04-15 13:10:51.000000 chanfig-0.0.99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-15 13:10:51.000000 chanfig-0.0.99/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.828487 chanfig-0.0.99/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.AGPL
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.Apache
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.BSD
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.GPLv2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.GPLv3
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 13:10:51.000000 chanfig-0.0.99/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-15 13:10:54.852487 chanfig-0.0.99/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11491 2024-04-15 13:10:51.000000 chanfig-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-04-15 13:10:51.000000 chanfig-0.0.99/README.zh.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.832487 chanfig-0.0.99/chanfig/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2329 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20268 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/configclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/default_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48291 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/flat_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30651 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-15 13:10:51.000000 chanfig-0.0.99/chanfig/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.852487 chanfig-0.0.99/chanfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 13:10:54.000000 chanfig-0.0.99/chanfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.832487 chanfig-0.0.99/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 13:10:51.000000 chanfig-0.0.99/demo/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-15 13:10:51.000000 chanfig-0.0.99/demo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 13:10:51.000000 chanfig-0.0.99/demo/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.832487 chanfig-0.0.99/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.836487 chanfig-0.0.99/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.836487 chanfig-0.0.99/docs/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/configclass.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/default_dict.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/flat_dict.md
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/functional.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/index.zh.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/nested_dict.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/parser.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/registry.md
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/docs/variable.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.836487 chanfig-0.0.99/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.824487 chanfig-0.0.99/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.836487 chanfig-0.0.99/docs/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.848487 chanfig-0.0.99/docs/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.848487 chanfig-0.0.99/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.848487 chanfig-0.0.99/docs/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-15 13:10:51.000000 chanfig-0.0.99/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-15 13:10:51.000000 chanfig-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:10:51.000000 chanfig-0.0.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:10:54.852487 chanfig-0.0.99/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-15 13:10:51.000000 chanfig-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:10:54.852487 chanfig-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/interpolate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_configclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_flat_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_nested_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-15 13:10:51.000000 chanfig-0.0.99/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 13:10:51.000000 chanfig-0.0.99/tox.ini
```

### Comparing `chanfig-0.0.98/.github/workflows/push.yaml` & `chanfig-0.0.99/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/.gitignore` & `chanfig-0.0.99/.gitignore`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/.pre-commit-config.yaml` & `chanfig-0.0.99/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.AGPL` & `chanfig-0.0.99/LICENSES/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.Apache` & `chanfig-0.0.99/LICENSES/LICENSE.Apache`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.BSD` & `chanfig-0.0.99/LICENSES/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.GPLv2` & `chanfig-0.0.99/LICENSES/LICENSE.GPLv2`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.GPLv3` & `chanfig-0.0.99/LICENSES/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.MIT` & `chanfig-0.0.99/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/LICENSES/LICENSE.Unlicense` & `chanfig-0.0.99/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/PKG-INFO` & `chanfig-0.0.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chanfig
-Version: 0.0.98
+Version: 0.0.99
 Summary: Easier Configuration
 Author-email: Zhiyuan Chen <this@zyc.ai>, "Evian C. Liu" <evian.liu@outlook.com>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
 Project-URL: documentation, https://chanfig.danling.org
 Project-URL: homepage, https://chanfig.danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/CHANfiG
@@ -136,14 +136,17 @@
 
 Note that [`Config`][chanfig.Config] also has `default_factory=Config()` by default for convenience.
 
 ### Registry
 
 [`Registry`][chanfig.Registry] extends the [`NestedDict`][chanfig.NestedDict] and supports [`register`][chanfig.Registry.register], [`lookup`][chanfig.Registry.lookup], and [`build`][chanfig.Registry.build] to help you register constructors and build objects from a [`Config`][chanfig.Config].
 
+[`ConfigRegistry`][chanfig.ConfigRegistry] is a subclass of [`Registry`][chanfig.Registry] that is specifically designed for building objects from a [`Config`][chanfig.Config] or a [`dataclass`][dataclasses.dataclass].
+Just specify the `key` when creating the registry and pass `config` to the `build` method, and you will get the object you want.
+
 ### Variable
 
 Have one value for multiple names at multiple places? We got you covered.
 
 Just wrap the value with [`Variable`][chanfig.Variable], and one alteration will be reflected everywhere.
 
 [`Variable`][chanfig.Variable] supports `type`, `choices`, `validator`, and `required` to ensure the correctness of the value.
```

### Comparing `chanfig-0.0.98/README.md` & `chanfig-0.0.99/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
 
 Note that [`Config`][chanfig.Config] also has `default_factory=Config()` by default for convenience.
 
 ### Registry
 
 [`Registry`][chanfig.Registry] extends the [`NestedDict`][chanfig.NestedDict] and supports [`register`][chanfig.Registry.register], [`lookup`][chanfig.Registry.lookup], and [`build`][chanfig.Registry.build] to help you register constructors and build objects from a [`Config`][chanfig.Config].
 
+[`ConfigRegistry`][chanfig.ConfigRegistry] is a subclass of [`Registry`][chanfig.Registry] that is specifically designed for building objects from a [`Config`][chanfig.Config] or a [`dataclass`][dataclasses.dataclass].
+Just specify the `key` when creating the registry and pass `config` to the `build` method, and you will get the object you want.
+
 ### Variable
 
 Have one value for multiple names at multiple places? We got you covered.
 
 Just wrap the value with [`Variable`][chanfig.Variable], and one alteration will be reflected everywhere.
 
 [`Variable`][chanfig.Variable] supports `type`, `choices`, `validator`, and `required` to ensure the correctness of the value.
```

### Comparing `chanfig-0.0.98/README.zh.md` & `chanfig-0.0.99/README.zh.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
 注意[`Config`][chanfig.Config]默认设置`default_factory=Config()`来提供便利。
 
 ### Registry
 
 [`Registry`][chanfig.Registry]继承自[`NestedDict`][chanfig.NestedDict]，并且提供[`register`][chanfig.Registry.register]、[`lookup`][chanfig.Registry.lookup]和[`build`][chanfig.Registry.build]来帮助你注册构造函数并从[`Config`][chanfig.Config]来创建对象。
 
+[`ConfigRegistry`][chanfig.ConfigRegistry]是一个[`Registry`][chanfig.Registry]的子类，他专为从一个[`Config`][chanfig.Config]或者一个[`dataclass`][dataclasses.dataclass]来构建一个对象而设计。
+只需在创建注册表时指定`key`，然后在调用`build`方法时传入`config`，你就会得到你想要的对象。
+
 ### Variable
 
 有一个值在多个地方以多个名字出现？我们给你提供掩护。
 
 只要将值以[`Variable`][chanfig.Variable]包装，然后每处更改都会在处处体现。
 
 [`Variable`][chanfig.Variable]支持`type`、`choices`、`validator`、`required`来确保值的正确性。
```

### Comparing `chanfig-0.0.98/chanfig/__init__.py` & `chanfig-0.0.99/chanfig/__init__.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/config.py` & `chanfig-0.0.99/chanfig/config.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/configclasses.py` & `chanfig-0.0.99/chanfig/configclasses.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/default_dict.py` & `chanfig-0.0.99/chanfig/default_dict.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/flat_dict.py` & `chanfig-0.0.99/chanfig/flat_dict.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/functional.py` & `chanfig-0.0.99/chanfig/functional.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/nested_dict.py` & `chanfig-0.0.99/chanfig/nested_dict.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/parser.py` & `chanfig-0.0.99/chanfig/parser.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/registry.py` & `chanfig-0.0.99/chanfig/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from collections.abc import Callable, MutableMapping
 from copy import deepcopy
 from functools import wraps
 from typing import Any
 
 from .nested_dict import NestedDict
+from .utils import NULL, Null
 
 
 class Registry(NestedDict):
     """
     `Registry` for components.
 
     `Registry` provides 3 core functionalities:
@@ -57,15 +58,15 @@
 
     See Also:
         [`ConfigRegistry`][chanfig.ConfigRegistry]: Optimised for components that can be initialised with a `config`.
 
     Examples:
         >>> registry = Registry()
         >>> @registry.register
-        ... @registry.register("Module1")
+        ... @registry.register("Module1", default=True)
         ... class Module:
         ...     def __init__(self, a, b):
         ...         self.a = a
         ...         self.b = b
         >>> module = registry.register(Module, "Module2")
         >>> registry
         Registry(
@@ -74,34 +75,41 @@
           ('Module2'): <class 'chanfig.registry.Module'>
         )
         >>> module = registry.register(Module, "Module")
         Traceback (most recent call last):
         ValueError: Component with name Module already registered.
         >>> registry.lookup("Module")
         <class 'chanfig.registry.Module'>
-        >>> config = {"module": {"name": "Module", "a": 1, "b": 2}}
+        >>> config = {"module": {"name": "Module", "a": 0, "b": 1}}
         >>> # registry.register(Module)
         >>> module = registry.build(config["module"])
         >>> type(module)
         <class 'chanfig.registry.Module'>
-        >>> module.a
-        1
-        >>> module.b
-        2
+        >>> module.a, module.b
+        (0, 1)
+        >>> config = {"module": {"name": "NE", "a": 1, "b": 0}}
+        >>> module = registry.build(config["module"])
+        >>> module.a, module.b
+        (1, 0)
     """
 
     override: bool = False
+    key: str = "name"
+    default: Any = None
 
     def __init__(self, override: bool | None = None, key: str = "name", fallback: bool | None = None):
         super().__init__(fallback=fallback)
-        self.setattr("key", key)
         if override is not None:
             self.setattr("override", override)
+        self.setattr("key", key)
+        self.setattr("default", Null)
 
-    def register(self, component: Any = None, name: Any | None = None, override: bool = False) -> Callable:
+    def register(
+        self, component: Any = Null, name: Any = Null, override: bool = False, default: bool = False
+    ) -> Callable:
         r"""
         Register a new component.
 
         Args:
             component: The component to register.
             name: The name of the component.
 
@@ -129,30 +137,36 @@
             )
         """
 
         if name in self and not (override or self.override):
             raise ValueError(f"Component with name {name} already registered.")
 
         # Registry.register()
-        if name is not None:
+        if name is not Null:
             self.set(name, component)
+            if default:
+                self.setattr("default", component)
             return component
         # @Registry.register
-        if callable(component) and name is None:
+        if callable(component) and name is Null:
             self.set(component.__name__, component)
+            if default:
+                self.setattr("default", component)
             return component
 
         # @Registry.register()
-        def decorator(name: Any | None = None):
+        def decorator(name: Any = Null):
             @wraps(self.register)
             def wrapper(component):
-                if name is None:
+                if name is Null:
                     self.set(component.__name__, component)
                 else:
                     self.set(name, component)
+                if default:
+                    self.setattr("default", component)
                 return component
 
             return wrapper
 
         return decorator(component)
 
     def lookup(self, name: str) -> Any:
@@ -175,15 +189,15 @@
             ...     def __init__(self, a, b):
             ...         self.a = a
             ...         self.b = b
             >>> registry.lookup("Module")
             <class 'chanfig.registry.Module'>
         """
 
-        return self[name]
+        return self.get(name, self.getattr("default", Null))
 
     @staticmethod
     def init(cls: Callable, *args: Any, **kwargs: Any) -> Any:  # pylint: disable=W0211
         r"""
         Constructor of component.
 
         Args:
@@ -195,27 +209,25 @@
             (Any):
 
         Examples:
             >>> class Module:
             ...     def __init__(self, a, b):
             ...         self.a = a
             ...         self.b = b
-            >>> kwargs = {"a": 1, "b": 2}
+            >>> kwargs = {"a": 0, "b": 1}
             >>> module = Registry.init(Module, **kwargs)
             >>> type(module)
             <class 'chanfig.registry.Module'>
-            >>> module.a
-            1
-            >>> module.b
-            2
+            >>> module.a, module.b
+            (0, 1)
         """
 
         return cls(*args, **kwargs)
 
-    def build(self, name: str | MutableMapping | None = None, *args: Any, **kwargs: Any) -> Any:
+    def build(self, name: str | MutableMapping | NULL = Null, *args: Any, **kwargs: Any) -> Any:
         r"""
         Build a component.
 
         Args:
             name (str | MutableMapping):
                 If its a `MutableMapping`, it must contain `key` as a member, the rest will be treated as `**kwargs`.
                 Note that values in `kwargs` will override values in `name` if its a `MutableMapping`.
@@ -248,24 +260,24 @@
             >>> module.a
             2
         """
 
         if isinstance(name, MutableMapping):
             name = deepcopy(name)
             name, kwargs = name.pop(self.getattr("key", "name")), dict(name, **kwargs)  # type: ignore[arg-type]
-        if name is None:
+        if name is Null:
             name, kwargs = kwargs.pop(self.getattr("key")), dict(**kwargs)
         return self.init(self.lookup(name), *args, **kwargs)  # type: ignore[arg-type]
 
 
 class ConfigRegistry(Registry):
     """
     `ConfigRegistry` for components that can be initialised with a `config`.
 
-    `ConfigRegistry` is purcutularly useful when you want to construct a component from a configuration, such as a
+    `ConfigRegistry` is particularly useful when you want to construct a component from a configuration, such as a
     Hugginface Transformers model.
 
     See Also:
         [`Registry`][chanfig.Registry]: General purpose Registry.
 
     Examples:
         >>> from dataclasses import dataclass, field
@@ -319,15 +331,42 @@
         ...         self.b = config.module.a
         >>> nested_config = NestedConfig()
         >>> module = nested_registry.build(nested_config)
         >>> module.a, module.b
         (0, 1)
     """
 
-    def build(self, config) -> Any:  # type: ignore[override]
+    @staticmethod
+    def init(cls: Callable, config, *args: Any, **kwargs: Any) -> Any:  # pylint: disable=W0211
+        r"""
+        Constructor of component.
+
+        Args:
+            cls: The component to construct.
+            *args: The arguments to pass to the component.
+            **kwargs: The keyword arguments to pass to the component.
+
+        Returns:
+            (Any):
+
+        Examples:
+            >>> class Module:
+            ...     def __init__(self, config, a=None, b=None):
+            ...         self.config = config
+            ...         self.a = config.a if a is None else a
+            ...         self.b = config.b if b is None else b
+            >>> config = NestedDict({"a": 0, "b": 1})
+            >>> module = ConfigRegistry.init(Module, config, b=2)
+            >>> module.a, module.b
+            (0, 2)
+        """
+
+        return cls(config, *args, **kwargs)
+
+    def build(self, config, *args, **kwargs) -> Any:  # type: ignore[override]
         r"""
         Build a component.
 
         Args:
             config
 
         Returns:
@@ -371,11 +410,11 @@
         config_ = deepcopy(config)
 
         while "." in key:
             key, rest = key.split(".", 1)
             config_, key = getattr(config_, key), rest
         name = getattr(config_, key)
 
-        return self.init(self.lookup(name), config)  # type: ignore[arg-type]
+        return self.init(self.lookup(name), config, *args, **kwargs)  # type: ignore[arg-type]
 
 
 GlobalRegistry = Registry()
```

### Comparing `chanfig-0.0.98/chanfig/utils.py` & `chanfig-0.0.99/chanfig/utils.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig/variable.py` & `chanfig-0.0.99/chanfig/variable.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/chanfig.egg-info/PKG-INFO` & `chanfig-0.0.99/chanfig.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chanfig
-Version: 0.0.98
+Version: 0.0.99
 Summary: Easier Configuration
 Author-email: Zhiyuan Chen <this@zyc.ai>, "Evian C. Liu" <evian.liu@outlook.com>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
 Project-URL: documentation, https://chanfig.danling.org
 Project-URL: homepage, https://chanfig.danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/CHANfiG
@@ -136,14 +136,17 @@
 
 Note that [`Config`][chanfig.Config] also has `default_factory=Config()` by default for convenience.
 
 ### Registry
 
 [`Registry`][chanfig.Registry] extends the [`NestedDict`][chanfig.NestedDict] and supports [`register`][chanfig.Registry.register], [`lookup`][chanfig.Registry.lookup], and [`build`][chanfig.Registry.build] to help you register constructors and build objects from a [`Config`][chanfig.Config].
 
+[`ConfigRegistry`][chanfig.ConfigRegistry] is a subclass of [`Registry`][chanfig.Registry] that is specifically designed for building objects from a [`Config`][chanfig.Config] or a [`dataclass`][dataclasses.dataclass].
+Just specify the `key` when creating the registry and pass `config` to the `build` method, and you will get the object you want.
+
 ### Variable
 
 Have one value for multiple names at multiple places? We got you covered.
 
 Just wrap the value with [`Variable`][chanfig.Variable], and one alteration will be reflected everywhere.
 
 [`Variable`][chanfig.Variable] supports `type`, `choices`, `validator`, and `required` to ensure the correctness of the value.
```

### Comparing `chanfig-0.0.98/chanfig.egg-info/SOURCES.txt` & `chanfig-0.0.99/chanfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/demo/config.py` & `chanfig-0.0.99/demo/config.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/docs/utils.md` & `chanfig-0.0.99/docs/docs/utils.md`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/mkdocs.yml` & `chanfig-0.0.99/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/fonts/CascadiaCodePL.woff2` & `chanfig-0.0.99/docs/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/fonts/HYQiHei.ttf` & `chanfig-0.0.99/docs/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/fonts/HelveticaNowDisplay.otf` & `chanfig-0.0.99/docs/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/fonts/HelveticaWorld.ttf` & `chanfig-0.0.99/docs/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/images/favicon.ico` & `chanfig-0.0.99/docs/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/assets/images/logo.png` & `chanfig-0.0.99/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/docs/overrides/main.html` & `chanfig-0.0.99/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/pyproject.toml` & `chanfig-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_config.py` & `chanfig-0.0.99/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_configclass.py` & `chanfig-0.0.99/tests/test_configclass.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_flat_dict.py` & `chanfig-0.0.99/tests/test_flat_dict.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_misc.py` & `chanfig-0.0.99/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_nested_dict.py` & `chanfig-0.0.99/tests/test_nested_dict.py`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.98/tests/test_variable.py` & `chanfig-0.0.99/tests/test_variable.py`

 * *Files identical despite different names*

