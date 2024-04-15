# Comparing `tmp/codecov-cli-0.5.0.tar.gz` & `tmp/codecov-cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.5.0.tar", last modified: Tue Apr  9 17:20:47 2024, max compression
+gzip compressed data, was "codecov-cli-0.5.1.tar", last modified: Mon Apr 15 17:30:21 2024, max compression
```

## Comparing `codecov-cli-0.5.0.tar` & `codecov-cli-0.5.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.847977 codecov-cli-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/empty_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/send_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/upload_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.831977 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.831977 codecov-cli-0.5.0/codecov_cli/helpers/git_services/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git_services/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/compress_pycoverage_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/pytest_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/empty_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/empty_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/upload_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/upload_completion/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload_completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:20:47.847977 codecov-cli-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.588699 codecov-cli-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-15 17:30:21.588699 codecov-cli-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.568699 codecov-cli-0.5.1/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.572699 codecov-cli-0.5.1/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/empty_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/send_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/commands/upload_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.572699 codecov-cli-0.5.1/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/helpers/git_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/git_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/git_services/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/compress_pycoverage_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/runners/pytest_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/services/empty_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/empty_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.576699 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload/upload_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/codecov_cli/services/upload_completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/services/upload_completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.568699 codecov-cli-0.5.1/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 17:30:21.000000 codecov-cli-0.5.1/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.580699 codecov-cli-0.5.1/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.568699 codecov-cli-0.5.1/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.584699 codecov-cli-0.5.1/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-04-15 17:30:07.000000 codecov-cli-0.5.1/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-15 17:30:07.000000 codecov-cli-0.5.1/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.584699 codecov-cli-0.5.1/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-15 17:30:07.000000 codecov-cli-0.5.1/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.568699 codecov-cli-0.5.1/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.588699 codecov-cli-0.5.1/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-04-15 17:30:09.000000 codecov-cli-0.5.1/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-15 17:30:09.000000 codecov-cli-0.5.1/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:30:21.588699 codecov-cli-0.5.1/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-15 17:30:09.000000 codecov-cli-0.5.1/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:30:21.588699 codecov-cli-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-15 17:30:04.000000 codecov-cli-0.5.1/setup.py
```

### Comparing `codecov-cli-0.5.0/LICENSE` & `codecov-cli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/PKG-INFO` & `codecov-cli-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.5.0/README.md` & `codecov-cli-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/base_picking.py` & `codecov-cli-0.5.1/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/commit.py` & `codecov-cli-0.5.1/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.5.1/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/empty_upload.py` & `codecov-cli-0.5.1/codecov_cli/commands/empty_upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.5.1/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.5.1/codecov_cli/commands/labelanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/report.py` & `codecov-cli-0.5.1/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/send_notifications.py` & `codecov-cli-0.5.1/codecov_cli/commands/send_notifications.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.5.1/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/upload.py` & `codecov-cli-0.5.1/codecov_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/commands/upload_process.py` & `codecov-cli-0.5.1/codecov_cli/commands/upload_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                 report_code=report_code,
                 build_code=build_code,
                 build_url=build_url,
                 job_code=job_code,
                 env_vars=env_vars,
                 flags=flags,
                 name=name,
+                network_filter=network_filter,
+                network_prefix=network_prefix,
                 network_root_folder=network_root_folder,
                 files_search_root_folder=files_search_root_folder,
                 files_search_exclude_folders=files_search_exclude_folders,
                 files_search_explicitly_listed_files=files_search_explicitly_listed_files,
                 plugin_names=plugin_names,
                 token=token,
                 branch=branch,
@@ -109,14 +111,16 @@
         report_code=report_code,
         build_code=build_code,
         build_url=build_url,
         job_code=job_code,
         env_vars=env_vars,
         flags=flags,
         name=name,
+        network_filter=network_filter,
+        network_prefix=network_prefix,
         network_root_folder=network_root_folder,
         files_search_root_folder=files_search_root_folder,
         files_search_exclude_folders=files_search_exclude_folders,
         files_search_explicitly_listed_files=files_search_explicitly_listed_files,
         disable_search=disable_search,
         token=token,
         plugin_names=plugin_names,
```

### Comparing `codecov-cli-0.5.0/codecov_cli/fallbacks.py` & `codecov-cli-0.5.1/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.5.1/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/config.py` & `codecov-cli-0.5.1/codecov_cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/encoder.py` & `codecov-cli-0.5.1/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.5.1/codecov_cli/helpers/folder_searcher.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/git.py` & `codecov-cli-0.5.1/codecov_cli/helpers/git.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/git_services/github.py` & `codecov-cli-0.5.1/codecov_cli/helpers/git_services/github.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.5.1/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/options.py` & `codecov-cli-0.5.1/codecov_cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/request.py` & `codecov-cli-0.5.1/codecov_cli/helpers/request.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.5.1/codecov_cli/helpers/versioning_systems.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/main.py` & `codecov-cli-0.5.1/codecov_cli/main.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/plugins/__init__.py` & `codecov-cli-0.5.1/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/plugins/compress_pycoverage_contexts.py` & `codecov-cli-0.5.1/codecov_cli/plugins/compress_pycoverage_contexts.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/plugins/gcov.py` & `codecov-cli-0.5.1/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.5.1/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/plugins/xcode.py` & `codecov-cli-0.5.1/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/runners/__init__.py` & `codecov-cli-0.5.1/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.5.1/codecov_cli/runners/dan_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/runners/pytest_standard_runner.py` & `codecov-cli-0.5.1/codecov_cli/runners/pytest_standard_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/runners/types.py` & `codecov-cli-0.5.1/codecov_cli/runners/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.5.1/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/empty_upload/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/empty_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/report/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/general.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/general.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.5.1/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/file_finder.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/file_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/network_finder.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/network_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/upload_collector.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.5.1/codecov_cli/services/upload/upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/services/upload_completion/__init__.py` & `codecov-cli-0.5.1/codecov_cli/services/upload_completion/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli/types.py` & `codecov-cli-0.5.1/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.5.1/codecov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.5.0/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.5.1/codecov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.5.1/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.5.1/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.5.1/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterpython/src/parser.c` & `codecov-cli-0.5.1/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.5.1/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.5.1/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.5.0/setup.py` & `codecov-cli-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.5.0",
+    version="0.5.1",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=[
```

