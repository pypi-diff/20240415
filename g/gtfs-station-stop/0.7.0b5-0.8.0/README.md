# Comparing `tmp/gtfs_station_stop-0.7.0b5.tar.gz` & `tmp/gtfs_station_stop-0.8.0.tar.gz`

## Comparing `gtfs_station_stop-0.7.0b5.tar` & `gtfs_station_stop-0.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.flake8
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.gitlab-ci.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/requirements-dev.txt
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/requirements.txt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/setup.cfg
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__init__.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__main__.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/alert.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/arrival.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/calendar.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/const.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/feed_subject.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/helpers.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_info.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_status.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/static_database.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop_info.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/trip_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/conftest.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/fixtures.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/mock_feed_server.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_arrival.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_calendar.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_feed_subject.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_helpers.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_route_info.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_route_status.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_station_stop.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_station_stop_info.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/test_trip_info.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/calendar.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/calendar_dates.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/routes.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/stops.txt
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/trips.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static_supl/stops.txt
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/tests/data/gtfs_static_supl/trips.txt
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/LICENSE
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/README.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/pyproject.toml
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 gtfs_station_stop-0.7.0b5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/.flake8
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/requirements-dev.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/setup.cfg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/__init__.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/__main__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/alert.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/arrival.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/calendar.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/const.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/feed_subject.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/helpers.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/route_info.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/route_status.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/static_database.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/station_stop.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/station_stop_info.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/src/gtfs_station_stop/trip_info.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/fixtures.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/mock_feed_server.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_arrival.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_calendar.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_feed_subject.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_route_info.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_route_status.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_station_stop.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_station_stop_info.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/test_trip_info.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static/calendar.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static/calendar_dates.txt
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static/routes.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static/stops.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static/trips.txt
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static_supl/stops.txt
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/tests/data/gtfs_static_supl/trips.txt
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 gtfs_station_stop-0.8.0/PKG-INFO
```

### Comparing `gtfs_station_stop-0.7.0b5/.gitlab-ci.yml` & `gtfs_station_stop-0.8.0/.gitlab-ci.yml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-stages:
-  - lint
-  - test
-  - build
-  - register
-  - release
-
-variables:
-  PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"
-  PRE_COMMIT_HOME: "/.cache/pre-commit"
-  TEST_RESULTS_FILE: "test_results.xml"
-  TEST_COVERAGE_FILE: "coverage.xml"
-  PYTHON_IMAGE: python:3
-
-default:
-  image: $PYTHON_IMAGE
-  cache:
-    paths:
-      - .cache/pip
-  before_script:
-    - python --version ; pip --version
-    - pip install --upgrade pip
-    - pip install -r requirements-dev.txt
-
-.doRelease:
-  rules:
-    - if: $CI_COMMIT_TAG
-
-include:
-  - template: Jobs/Secret-Detection.gitlab-ci.yml
-
-secret_detection:
-  inherit:
-    default: false
-  stage: lint
-
-check_formatting:
-  stage: lint
-  cache:
-    paths:
-      - $PRE_COMMIT_HOME
-  script:
-    - pre-commit run --all-files
-
-pytest:
-  stage: test
-  script:
-    - python -m pytest --junitxml=$TEST_RESULTS_FILE
-    - coverage report
-    - coverage xml -o $TEST_COVERAGE_FILE
-  coverage: '/TOTAL.*\s+(\d+%)$/'
-  artifacts:
-    when: always
-    paths:
-      - $TEST_RESULTS_FILE
-      - $TEST_COVERAGE_FILE
-    reports:
-      junit: $TEST_RESULTS_FILE
-      coverage_report:
-        coverage_format: cobertura
-        path: $TEST_COVERAGE_FILE
-
-module_test:
-  stage: test
-  image: $PYTHON_IMAGE
-  inherit:
-    default: false
-  script:
-    - pip install .
-    - echo "Running module version command to test module loading..."
-    - python -m gtfs_station_stop --version # output version
-    - python -m gtfs_station_stop # smoke test no input
-
-build:
-  stage: build
-  script:
-    - python -m build
-  artifacts:
-    paths:
-      - dist/
-
-register_package_gitlab_pypi:
-  extends: .doRelease
-  stage: register
-  variables:
-    TWINE_USERNAME: gitlab-ci-token
-    TWINE_PASSWORD: ${CI_JOB_TOKEN}
-  before_script:
-    - pip install --upgrade twine
-  script:
-    - |
-      python -m twine upload \
-      --verbose \
-      --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
-
-release_job:
-  extends: .doRelease
-  stage: release
-  image: registry.gitlab.com/gitlab-org/release-cli:latest
-  inherit:
-    default: false
-  rules:
-    - if: $CI_COMMIT_TAG
-  script:
-    - echo "Making Release $CI_COMMIT_TAG"
-  release:
-    tag_name: "$CI_COMMIT_TAG"
-    description: "$CI_COMMIT_TAG"
+stages:
+  - lint
+  - test
+  - build
+  - register
+  - release
+
+variables:
+  PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"
+  PRE_COMMIT_HOME: "/.cache/pre-commit"
+  TEST_RESULTS_FILE: "test_results.xml"
+  TEST_COVERAGE_FILE: "coverage.xml"
+  PYTHON_IMAGE: python:3
+
+default:
+  image: $PYTHON_IMAGE
+  cache:
+    paths:
+      - .cache/pip
+  before_script:
+    - python --version ; pip --version
+    - pip install --upgrade pip
+    - pip install -r requirements-dev.txt
+
+.doRelease:
+  rules:
+    - if: $CI_COMMIT_TAG
+
+include:
+  - template: Jobs/Secret-Detection.gitlab-ci.yml
+
+secret_detection:
+  inherit:
+    default: false
+  stage: lint
+
+check_formatting:
+  stage: lint
+  cache:
+    paths:
+      - $PRE_COMMIT_HOME
+  script:
+    - pre-commit run --all-files
+
+pytest:
+  stage: test
+  script:
+    - python -m pytest --junitxml=$TEST_RESULTS_FILE
+    - coverage report
+    - coverage xml -o $TEST_COVERAGE_FILE
+  coverage: '/TOTAL.*\s+(\d+%)$/'
+  artifacts:
+    when: always
+    paths:
+      - $TEST_RESULTS_FILE
+      - $TEST_COVERAGE_FILE
+    reports:
+      junit: $TEST_RESULTS_FILE
+      coverage_report:
+        coverage_format: cobertura
+        path: $TEST_COVERAGE_FILE
+
+module_test:
+  stage: test
+  image: $PYTHON_IMAGE
+  inherit:
+    default: false
+  script:
+    - pip install .
+    - echo "Running module version command to test module loading..."
+    - python -m gtfs_station_stop --version # output version
+    - python -m gtfs_station_stop # smoke test no input
+
+build:
+  stage: build
+  script:
+    - python -m build
+  artifacts:
+    paths:
+      - dist/
+
+register_package_gitlab_pypi:
+  extends: .doRelease
+  stage: register
+  variables:
+    TWINE_USERNAME: gitlab-ci-token
+    TWINE_PASSWORD: ${CI_JOB_TOKEN}
+  before_script:
+    - pip install --upgrade twine
+  script:
+    - |
+      python -m twine upload \
+      --verbose \
+      --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
+
+release_job:
+  extends: .doRelease
+  stage: release
+  image: registry.gitlab.com/gitlab-org/release-cli:latest
+  inherit:
+    default: false
+  rules:
+    - if: $CI_COMMIT_TAG
+  script:
+    - echo "Making Release $CI_COMMIT_TAG"
+  release:
+    tag_name: "$CI_COMMIT_TAG"
+    description: "$CI_COMMIT_TAG"
```

### Comparing `gtfs_station_stop-0.7.0b5/.pre-commit-config.yaml` & `gtfs_station_stop-0.8.0/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
-    hooks:
-      - id: check-yaml
-      - id: debug-statements
-      - id: trailing-whitespace
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.13.2
-    hooks:
-      - id: isort
-        args: ["--profile", "black"]
-  - repo: https://github.com/psf/black
-    rev: 23.12.1
-    hooks:
-      - id: black
-        exclude: tests/test_lowlevel.py
-  - repo: https://github.com/PyCQA/flake8
-    rev: 7.0.0
-    hooks:
-      - id: flake8
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.0
-    hooks:
-      - id: ruff
-      - id: ruff-format
-  - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
-    hooks:
-      - id: codespell
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v2.3.0
+    hooks:
+      - id: check-yaml
+      - id: debug-statements
+      - id: trailing-whitespace
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
+    hooks:
+      - id: isort
+        args: ["--profile", "black"]
+  - repo: https://github.com/psf/black
+    rev: 23.12.1
+    hooks:
+      - id: black
+        exclude: tests/test_lowlevel.py
+  - repo: https://github.com/PyCQA/flake8
+    rev: 7.0.0
+    hooks:
+      - id: flake8
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.0
+    hooks:
+      - id: ruff
+      - id: ruff-format
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
+    hooks:
+      - id: codespell
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/__main__.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/__main__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-#!/usr/bin/python
-import argparse
-import asyncio
-import os
-import time
-from pprint import pprint
-
-import dotenv
-
-import gtfs_station_stop.__about__
-from gtfs_station_stop.calendar import Calendar
-from gtfs_station_stop.feed_subject import FeedSubject
-from gtfs_station_stop.route_status import RouteStatus
-from gtfs_station_stop.static_database import (  # noqa: F401
-    GtfsStaticDatabase,
-    async_factory,
-)
-from gtfs_station_stop.station_stop import StationStop
-from gtfs_station_stop.station_stop_info import (  # noqa: F401
-    StationStopInfo,
-    StationStopInfoDatabase,
-)
-from gtfs_station_stop.trip_info import TripInfo, TripInfoDatabase  # noqa: F401
-
-dotenv.load_dotenv()
-
-parser = argparse.ArgumentParser(
-    prog="GTFS Station Stop", description="Use for static and realtime GTFS info"
-)
-
-parser.add_argument(
-    "-v", "--version", action="store_true", help="display the module version"
-)
-parser.add_argument(
-    "-i",
-    "--info-zip",
-    help="input GTFS zip file path of static data",
-    nargs="*",
-    default=[],
-)
-parser.add_argument("-k", "--api-key", help="API key for feed URLs")
-parser.add_argument("-u", "--feed-urls", help="feed URL list", nargs="*", default=[])
-parser.add_argument(
-    "-s",
-    "--stops",
-    help="list of stops to check for arrivals and alerts",
-    nargs="*",
-    default=[],
-)
-parser.add_argument(
-    "-r", "--routes", help="list of routes to check for alerts", nargs="*", default=[]
-)
-parser.add_argument(
-    "--lang", type=str, default="en", help="language to read alerts", nargs="?"
-)
-parser.add_argument(
-    "--do-async", action="store_true", help="update using asynchronous functions"
-)
-
-args = parser.parse_args()
-
-if args.version:
-    print(gtfs_station_stop.__about__.__version__)
-    exit(0)
-
-start_time = time.time()
-
-# Get the API Key, argument takes precedent of environment variable
-api_key = args.api_key or os.environ.get("API_KEY")
-headers = {"api-key": api_key, "x-api-key": api_key, "api_key": api_key}
-
-ssi_db = None
-ti_db = None
-calendar = None
-
-if args.do_async and args.info_zip:
-
-    async def async_get_static_info():
-        async with asyncio.TaskGroup() as tg:
-            ssi_db_task = tg.create_task(
-                async_factory(
-                    StationStopInfoDatabase,
-                    *args.info_zip,
-                    headers=headers,
-                )
-            )
-            ti_db_task = tg.create_task(
-                async_factory(
-                    TripInfoDatabase,
-                    *args.info_zip,
-                    headers=headers,
-                )
-            )
-            calendar_task = tg.create_task(
-                async_factory(
-                    Calendar,
-                    *args.info_zip,
-                    headers=headers,
-                )
-            )
-        return (ssi_db_task.result(), ti_db_task.result(), calendar_task.result())
-
-    ssi_db, ti_db, calendar = asyncio.run(async_get_static_info())
-elif args.info_zip:
-    ssi_db = StationStopInfoDatabase(*args.info_zip, headers=headers)
-    ti_db = TripInfoDatabase(*args.info_zip, headers=headers)
-    calendar = Calendar(*args.info_zip, headers=headers)
-
-if calendar is not None:
-    # Print out the current active service IDs
-    print()
-    print("SERVICES:")
-    print("=========")
-    exptabs: int = max(len(v.service_id) + 2 for v in calendar.services.values())
-    for s in calendar.get_active_services():
-        print(f"{s.service_id}:\t\033[92m active \033[00m".expandtabs(exptabs))
-    for s in calendar.get_inactive_services():
-        print(f"{s.service_id}:\t\033[91m inactive \033[00m".expandtabs(exptabs))
-
-feed_subject = FeedSubject(args.feed_urls, headers=headers)
-station_stops = [StationStop(id, feed_subject) for id in args.stops]
-route_statuses = [RouteStatus(id, feed_subject) for id in args.routes]
-
-if args.do_async:
-    asyncio.run(feed_subject.async_update())
-else:
-    station_stops = [StationStop(id, feed_subject) for id in args.stops]
-    route_statuses = [RouteStatus(id, feed_subject) for id in args.routes]
-    feed_subject.update()
-
-print()
-print("Arrival Status:")
-print("===============")
-if not len(station_stops):
-    print("none")
-for stop in station_stops:
-    if ssi_db is not None:
-        print(ssi_db[stop.id])
-        pprint(
-            [
-                [
-                    arrival.route,
-                    arrival.time,
-                    arrival.trip,
-                    ti_db.get_close_match(arrival.trip, calendar),
-                ]
-                for arrival in sorted(stop.get_time_to_arrivals())
-            ]
-        )
-        print(stop.alerts)
-
-print()
-print("Route Status:")
-print("===============")
-if not len(route_statuses):
-    print("none")
-for route in route_statuses:
-    for alert in route.alerts:
-        print(f"Alert! {route.id}")
-        print(alert.header_text.get(args.lang))
-        print(alert.description_text.get(args.lang))
-        print()
-        print()
-
-print(
-    f"Processed {len(args.feed_urls)} feeds and {len(args.info_zip)} static info zipfiles in {time.time() - start_time:.3f} seconds"
-)
+#!/usr/bin/python
+import argparse
+import asyncio
+import os
+import time
+from pprint import pprint
+
+import dotenv
+
+import gtfs_station_stop.__about__
+from gtfs_station_stop.calendar import Calendar
+from gtfs_station_stop.feed_subject import FeedSubject
+from gtfs_station_stop.route_status import RouteStatus
+from gtfs_station_stop.static_database import (  # noqa: F401
+    GtfsStaticDatabase,
+    async_factory,
+)
+from gtfs_station_stop.station_stop import StationStop
+from gtfs_station_stop.station_stop_info import (  # noqa: F401
+    StationStopInfo,
+    StationStopInfoDatabase,
+)
+from gtfs_station_stop.trip_info import TripInfo, TripInfoDatabase  # noqa: F401
+
+dotenv.load_dotenv()
+
+parser = argparse.ArgumentParser(
+    prog="GTFS Station Stop", description="Use for static and realtime GTFS info"
+)
+
+parser.add_argument(
+    "-v", "--version", action="store_true", help="display the module version"
+)
+parser.add_argument(
+    "-i",
+    "--info-zip",
+    help="input GTFS zip file path of static data",
+    nargs="*",
+    default=[],
+)
+parser.add_argument("-k", "--api-key", help="API key for feed URLs")
+parser.add_argument("-u", "--feed-urls", help="feed URL list", nargs="*", default=[])
+parser.add_argument(
+    "-s",
+    "--stops",
+    help="list of stops to check for arrivals and alerts",
+    nargs="*",
+    default=[],
+)
+parser.add_argument(
+    "-r", "--routes", help="list of routes to check for alerts", nargs="*", default=[]
+)
+parser.add_argument(
+    "--lang", type=str, default="en", help="language to read alerts", nargs="?"
+)
+parser.add_argument(
+    "--do-async", action="store_true", help="update using asynchronous functions"
+)
+
+args = parser.parse_args()
+
+if args.version:
+    print(gtfs_station_stop.__about__.__version__)
+    exit(0)
+
+start_time = time.time()
+
+# Get the API Key, argument takes precedent of environment variable
+api_key = args.api_key or os.environ.get("API_KEY")
+headers = {"api-key": api_key, "x-api-key": api_key, "api_key": api_key}
+
+ssi_db = None
+ti_db = None
+calendar = None
+
+if args.do_async and args.info_zip:
+
+    async def async_get_static_info():
+        async with asyncio.TaskGroup() as tg:
+            ssi_db_task = tg.create_task(
+                async_factory(
+                    StationStopInfoDatabase,
+                    *args.info_zip,
+                    headers=headers,
+                )
+            )
+            ti_db_task = tg.create_task(
+                async_factory(
+                    TripInfoDatabase,
+                    *args.info_zip,
+                    headers=headers,
+                )
+            )
+            calendar_task = tg.create_task(
+                async_factory(
+                    Calendar,
+                    *args.info_zip,
+                    headers=headers,
+                )
+            )
+        return (ssi_db_task.result(), ti_db_task.result(), calendar_task.result())
+
+    ssi_db, ti_db, calendar = asyncio.run(async_get_static_info())
+elif args.info_zip:
+    ssi_db = StationStopInfoDatabase(*args.info_zip, headers=headers)
+    ti_db = TripInfoDatabase(*args.info_zip, headers=headers)
+    calendar = Calendar(*args.info_zip, headers=headers)
+
+if calendar is not None:
+    # Print out the current active service IDs
+    print()
+    print("SERVICES:")
+    print("=========")
+    exptabs: int = max(len(v.service_id) + 2 for v in calendar.services.values())
+    for s in calendar.get_active_services():
+        print(f"{s.service_id}:\t\033[92m active \033[00m".expandtabs(exptabs))
+    for s in calendar.get_inactive_services():
+        print(f"{s.service_id}:\t\033[91m inactive \033[00m".expandtabs(exptabs))
+
+feed_subject = FeedSubject(args.feed_urls, headers=headers)
+station_stops = [StationStop(id, feed_subject) for id in args.stops]
+route_statuses = [RouteStatus(id, feed_subject) for id in args.routes]
+
+if args.do_async:
+    asyncio.run(feed_subject.async_update())
+else:
+    station_stops = [StationStop(id, feed_subject) for id in args.stops]
+    route_statuses = [RouteStatus(id, feed_subject) for id in args.routes]
+    feed_subject.update()
+
+print()
+print("Arrival Status:")
+print("===============")
+if not len(station_stops):
+    print("none")
+for stop in station_stops:
+    if ssi_db is not None:
+        print(ssi_db[stop.id])
+        pprint(
+            [
+                [
+                    arrival.route,
+                    arrival.time,
+                    arrival.trip,
+                    ti_db.get_close_match(arrival.trip, calendar),
+                ]
+                for arrival in sorted(stop.get_time_to_arrivals())
+            ]
+        )
+        print(stop.alerts)
+
+print()
+print("Route Status:")
+print("===============")
+if not len(route_statuses):
+    print("none")
+for route in route_statuses:
+    for alert in route.alerts:
+        print(f"Alert! {route.id}")
+        print(alert.header_text.get(args.lang))
+        print(alert.description_text.get(args.lang))
+        print()
+        print()
+
+print(
+    f"Processed {len(args.feed_urls)} feeds and {len(args.info_zip)} static info zipfiles in {time.time() - start_time:.3f} seconds"
+)
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/calendar.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/calendar.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import os
-from datetime import date, datetime
-from typing import NamedTuple
-
-from gtfs_station_stop.static_database import GtfsStaticDatabase
-
-SERVICE_EXCEPTION_TYPE_ADDED = "1"
-SERVICE_EXCEPTION_TYPE_REMOVED = "2"
-
-
-class ServiceDays(NamedTuple):
-    """Class for storing the days available with names."""
-
-    monday: bool
-    tuesday: bool
-    wednesday: bool
-    thursday: bool
-    friday: bool
-    saturday: bool
-    sunday: bool
-
-    def no_service():
-        return ServiceDays(*[False] * len(ServiceDays._fields))
-
-
-class Service:
-    """Class for keeping calendar service data."""
-
-    def __init__(
-        self, service_id: str, service_days: ServiceDays, start: date, end: date
-    ):
-        self.service_id = service_id
-        self.service_days = service_days
-        self.start = start
-        self.end = end
-        self.added_exceptions = set()
-        self.removed_exceptions = set()
-
-    def is_active_on(self, the_date: date = date.today()):
-        """Check if service is active on a given datetime, defaults to now."""
-        if isinstance(the_date, datetime):
-            the_date = the_date.date()
-        normally_active = (self.start <= the_date <= self.end) and self.service_days[
-            the_date.weekday()
-        ]
-        return (normally_active and the_date not in self.removed_exceptions) or (
-            not normally_active and the_date in self.added_exceptions
-        )
-
-    def no_regular_service(service_id: str):
-        return Service(service_id, ServiceDays.no_service(), date.min, date.min)
-
-
-class Calendar(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
-        self.services = {}
-        super().__init__(*gtfs_files, **kwargs)
-
-    def add_gtfs_data(self, zip_filelike):
-        for line in self._get_gtfs_record_iter(zip_filelike, "calendar.txt"):
-            self.services[line["service_id"]] = Service(
-                line["service_id"],
-                ServiceDays(
-                    line["monday"] == "1",
-                    line["tuesday"] == "1",
-                    line["wednesday"] == "1",
-                    line["thursday"] == "1",
-                    line["friday"] == "1",
-                    line["saturday"] == "1",
-                    line["sunday"] == "1",
-                ),
-                datetime.strptime(line["start_date"], "%Y%m%d").date(),
-                datetime.strptime(line["end_date"], "%Y%m%d").date(),
-            )
-        # Add in special services
-        for line in self._get_gtfs_record_iter(zip_filelike, "calendar_dates.txt"):
-            service_id = line["service_id"]
-            if self.services.get(service_id) is None:
-                # Create a blank calendar if it is missing
-                self.services[service_id] = Service.no_regular_service(service_id)
-            if line["exception_type"] == SERVICE_EXCEPTION_TYPE_ADDED:
-                self.services[service_id].added_exceptions.add(
-                    datetime.strptime(line["date"], "%Y%m%d").date()
-                )
-            elif line["exception_type"] == SERVICE_EXCEPTION_TYPE_REMOVED:
-                self.services[service_id].removed_exceptions.add(
-                    datetime.strptime(line["date"], "%Y%m%d").date()
-                )
-            else:
-                raise RuntimeError("Unsupported GTFS service exception type.")
-
-    def get_active_services(self, the_date: date = date.today()) -> list[str]:
-        return [s for s in self.services.values() if s.is_active_on(the_date)]
-
-    def get_inactive_services(self, the_date: date = date.today()) -> list[str]:
-        return [s for s in self.services.values() if not s.is_active_on(the_date)]
-
-    def __getitem__(self, key) -> Service:
-        return self.services[key]
+import os
+from datetime import date, datetime
+from typing import NamedTuple
+
+from gtfs_station_stop.static_database import GtfsStaticDatabase
+
+SERVICE_EXCEPTION_TYPE_ADDED = "1"
+SERVICE_EXCEPTION_TYPE_REMOVED = "2"
+
+
+class ServiceDays(NamedTuple):
+    """Class for storing the days available with names."""
+
+    monday: bool
+    tuesday: bool
+    wednesday: bool
+    thursday: bool
+    friday: bool
+    saturday: bool
+    sunday: bool
+
+    def no_service():
+        return ServiceDays(*[False] * len(ServiceDays._fields))
+
+
+class Service:
+    """Class for keeping calendar service data."""
+
+    def __init__(
+        self, service_id: str, service_days: ServiceDays, start: date, end: date
+    ):
+        self.service_id = service_id
+        self.service_days = service_days
+        self.start = start
+        self.end = end
+        self.added_exceptions = set()
+        self.removed_exceptions = set()
+
+    def is_active_on(self, the_date: date = date.today()):
+        """Check if service is active on a given datetime, defaults to now."""
+        if isinstance(the_date, datetime):
+            the_date = the_date.date()
+        normally_active = (self.start <= the_date <= self.end) and self.service_days[
+            the_date.weekday()
+        ]
+        return (normally_active and the_date not in self.removed_exceptions) or (
+            not normally_active and the_date in self.added_exceptions
+        )
+
+    def no_regular_service(service_id: str):
+        return Service(service_id, ServiceDays.no_service(), date.min, date.min)
+
+
+class Calendar(GtfsStaticDatabase):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
+        self.services = {}
+        super().__init__(*gtfs_files, **kwargs)
+
+    def add_gtfs_data(self, zip_filelike):
+        for line in self._get_gtfs_record_iter(zip_filelike, "calendar.txt"):
+            self.services[line["service_id"]] = Service(
+                line["service_id"],
+                ServiceDays(
+                    line["monday"] == "1",
+                    line["tuesday"] == "1",
+                    line["wednesday"] == "1",
+                    line["thursday"] == "1",
+                    line["friday"] == "1",
+                    line["saturday"] == "1",
+                    line["sunday"] == "1",
+                ),
+                datetime.strptime(line["start_date"], "%Y%m%d").date(),
+                datetime.strptime(line["end_date"], "%Y%m%d").date(),
+            )
+        # Add in special services
+        for line in self._get_gtfs_record_iter(zip_filelike, "calendar_dates.txt"):
+            service_id = line["service_id"]
+            if self.services.get(service_id) is None:
+                # Create a blank calendar if it is missing
+                self.services[service_id] = Service.no_regular_service(service_id)
+            if line["exception_type"] == SERVICE_EXCEPTION_TYPE_ADDED:
+                self.services[service_id].added_exceptions.add(
+                    datetime.strptime(line["date"], "%Y%m%d").date()
+                )
+            elif line["exception_type"] == SERVICE_EXCEPTION_TYPE_REMOVED:
+                self.services[service_id].removed_exceptions.add(
+                    datetime.strptime(line["date"], "%Y%m%d").date()
+                )
+            else:
+                raise RuntimeError("Unsupported GTFS service exception type.")
+
+    def get_active_services(self, the_date: date = date.today()) -> list[str]:
+        return [s for s in self.services.values() if s.is_active_on(the_date)]
+
+    def get_inactive_services(self, the_date: date = date.today()) -> list[str]:
+        return [s for s in self.services.values() if not s.is_active_on(the_date)]
+
+    def __getitem__(self, key) -> Service:
+        return self.services[key]
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/helpers.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/helpers.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import csv
-import os
-import time
-from datetime import datetime as dt
-from io import BytesIO, StringIO
-from urllib.parse import urlparse
-from zipfile import ZipFile
-
-import requests_cache
-from google.transit import gtfs_realtime_pb2
-
-from gtfs_station_stop.const import GTFS_STATIC_CACHE, GTFS_STATIC_CACHE_EXPIRY
-
-
-def is_none_or_ends_at(
-    alert: gtfs_realtime_pb2.FeedEntity, at_time: float | dt | None = None
-):
-    """Returns the 'ends at' time, else returns None if not active."""
-    if at_time is None:
-        at_time = time.time()
-        # fallthrough
-    if isinstance(at_time, float):
-        at_time = dt.fromtimestamp(at_time)
-
-    for time_range in alert.active_period:
-        start: dt = (
-            dt.fromtimestamp(time_range.start)
-            if time_range.HasField("start")
-            else dt.min
-        )
-        end: dt = (
-            dt.fromtimestamp(time_range.end) if time_range.HasField("end") else dt.max
-        )
-        if start <= at_time <= end:
-            return end
-
-    return None
-
-
-def is_url(url):
-    try:
-        result = urlparse(url)
-        return all([result.scheme, result.netloc])
-    except (ValueError, AttributeError):
-        return False
-
-
-def gtfs_record_iter(zip_filelike, target_txt: os.PathLike, **kwargs):
-    """Generates a line from a given GTFS table. Can handle local files or URLs."""
-
-    zip_data = zip_filelike
-    # If the data is a url, make the request for the file resource.
-    if is_url(zip_filelike):
-        # Make the request, check for good return code, and convert to IO object.
-        # As GTFS Static Data updates rarely, (most providers recommend pulling this once per day),
-        # we will use a cache to minimize unnecessary checks.
-        session = requests_cache.CachedSession(
-            GTFS_STATIC_CACHE,
-            expire_after=GTFS_STATIC_CACHE_EXPIRY,
-        )
-        res = session.get(zip_filelike, headers=kwargs.get("headers"))
-        if 200 <= res.status_code < 400:
-            zip_data = BytesIO(res.content)
-        else:
-            raise ConnectionRefusedError
-
-    with ZipFile(zip_data, "r") as zip:
-        # Find the stops.txt file
-        first_or_none: str = next(
-            (name for name in zip.namelist() if name == target_txt), None
-        )
-        if first_or_none is None:
-            raise RuntimeError(f"Did not find required {target_txt} file")
-        # Create the dictionary of IDs, parents should precede the children
-        with StringIO(
-            str(zip.read(first_or_none), encoding="utf-8-sig")
-        ) as stops_dot_txt:
-            reader = csv.DictReader(
-                stops_dot_txt,
-                delimiter=",",
-            )
-            for line in reader:
-                yield line
+import csv
+import os
+import time
+from datetime import datetime as dt
+from io import BytesIO, StringIO
+from urllib.parse import urlparse
+from zipfile import ZipFile
+
+import requests_cache
+from google.transit import gtfs_realtime_pb2
+
+from gtfs_station_stop.const import GTFS_STATIC_CACHE, GTFS_STATIC_CACHE_EXPIRY
+
+
+def is_none_or_ends_at(
+    alert: gtfs_realtime_pb2.FeedEntity, at_time: float | dt | None = None
+):
+    """Returns the 'ends at' time, else returns None if not active."""
+    if at_time is None:
+        at_time = time.time()
+        # fallthrough
+    if isinstance(at_time, float):
+        at_time = dt.fromtimestamp(at_time)
+
+    for time_range in alert.active_period:
+        start: dt = (
+            dt.fromtimestamp(time_range.start)
+            if time_range.HasField("start")
+            else dt.min
+        )
+        end: dt = (
+            dt.fromtimestamp(time_range.end) if time_range.HasField("end") else dt.max
+        )
+        if start <= at_time <= end:
+            return end
+
+    return None
+
+
+def is_url(url):
+    try:
+        result = urlparse(url)
+        return all([result.scheme, result.netloc])
+    except (ValueError, AttributeError):
+        return False
+
+
+def gtfs_record_iter(zip_filelike, target_txt: os.PathLike, **kwargs):
+    """Generates a line from a given GTFS table. Can handle local files or URLs."""
+
+    zip_data = zip_filelike
+    # If the data is a url, make the request for the file resource.
+    if is_url(zip_filelike):
+        # Make the request, check for good return code, and convert to IO object.
+        # As GTFS Static Data updates rarely, (most providers recommend pulling this once per day),
+        # we will use a cache to minimize unnecessary checks.
+        session = requests_cache.CachedSession(
+            GTFS_STATIC_CACHE,
+            expire_after=GTFS_STATIC_CACHE_EXPIRY,
+        )
+        res = session.get(zip_filelike, headers=kwargs.get("headers"))
+        if 200 <= res.status_code < 400:
+            zip_data = BytesIO(res.content)
+        else:
+            raise ConnectionRefusedError
+
+    with ZipFile(zip_data, "r") as zip:
+        # Find the stops.txt file
+        first_or_none: str = next(
+            (name for name in zip.namelist() if name == target_txt), None
+        )
+        if first_or_none is None:
+            raise RuntimeError(f"Did not find required {target_txt} file")
+        # Create the dictionary of IDs, parents should precede the children
+        with StringIO(
+            str(zip.read(first_or_none), encoding="utf-8-sig")
+        ) as stops_dot_txt:
+            reader = csv.DictReader(
+                stops_dot_txt,
+                delimiter=",",
+            )
+            for line in reader:
+                yield line
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_info.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/route_info.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import os
-from enum import Enum
-from typing import Any
-
-from gtfs_station_stop.static_database import GtfsStaticDatabase
-
-
-class RouteType(Enum):
-    UNKNOWN = -1
-
-    TRAM = 0
-    SUBWAY = 1
-    RAIL = 2
-    BUS = 3
-    FERRY = 4
-    CABLE_TRAM = 5
-    AERIAL_LIFT = 6
-    FUNICULAR = 7
-    TROLLEYBUS = 11
-
-    RAILWAY_SERVICE = 100
-    HIGH_SPEED_RAIL_SERVICE = 101
-    LONG_DISTANCE_TRAIN = 102
-    INTER_REGIONAL_RAIL_SERVICE = 103
-    CAR_TRANSPORT_RAIL_SERVICE = 104
-    SLEEPER_RAIL_SERVICE = 105
-    REGIONAL_RAIL_SERVICE = 106
-    TOURIST_RAIL_SERVICE = 107
-    RAIL_SHUTTLE_WITHIN_COMPLEX = 108
-    SUBURBAN_RAILWAY = 109
-    REPLACEMENT_RAIL_SERVICE = 110
-    SPECIAL_RAIL_SERVICE = 111
-    LORRY_TRANSPORT_RAIL = 112
-
-    BUS_SERVICE = 700
-    REGIONAL_BUS_SERVICE = 701
-    EXPRESS_BUS_SERVICE = 702
-    STOPPING_BUS_SERVICE = 703
-    LOCAL_BUS_SERVICE = 704
-    NIGHT_BUS_SERVICE = 705
-    POST_BUS_SERVICE = 706
-    SPECIAL_NEEDS_BUS = 707
-    MOBILITY_BUS_SERVICE = 708
-    MOBILITY_BUS_FOR_REGISTERED_DISABLED = 709
-    SIGHTSEEING_BUS = 710
-    SHUTTLE_BUS = 711
-    SCHOOL_BUS = 712
-    SCHOOL_AND_PUBLIC_SERVICE_BUS = 713
-    RAIL_REPLACEMENT_BUS_SERVICE = 714
-    DEMAND_AND_RESPONSE_BUS_SERVICE = 715
-    ALL_BUS_SERVICES = 716
-
-    @classmethod
-    def _missing_(cls, value):
-        if isinstance(value, str):
-            value = int(value)
-            for member in cls:
-                if member.value == value:
-                    return member
-        return cls.UNKNOWN
-
-    def pretty_name(self):
-        PRETTY_NAMES = {
-            RouteType.TRAM: "Tram",
-            RouteType.SUBWAY: "Subway",
-            RouteType.RAIL: "Rail",
-            RouteType.BUS: "Bus",
-            RouteType.FERRY: "Ferry",
-            RouteType.CABLE_TRAM: "Cable Tram",
-            RouteType.AERIAL_LIFT: "Aerial Lift",
-            RouteType.FUNICULAR: "Funicular",
-            RouteType.TROLLEYBUS: "Trolleybus",
-            RouteType.SHUTTLE_BUS: "Shuttle Bus",
-        }
-        return PRETTY_NAMES.get(self) or self.name
-
-
-class RouteInfo:
-    def __init__(self, route_data_dict: dict):
-        self.agency_id = route_data_dict.get("agency_id")
-        self.id = route_data_dict["route_id"]
-        self.short_name = route_data_dict.get("route_short_name")
-        self.long_name = route_data_dict.get("route_long_name")
-        if self.short_name is None and self.long_name is None:
-            raise ValueError(
-                "Either 'route_short_name' or 'route_long_name' must be provided."
-            )
-        self.type = RouteType(int(route_data_dict["route_type"]))
-        self.desc = route_data_dict.get("route_desc")
-        self.url = route_data_dict.get("route_url")
-        self.color = route_data_dict.get("route_color")
-        self.text_color = route_data_dict.get("route_text_color")
-
-
-class RouteInfoDatabase(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
-        self.route_infos = {}
-        super().__init__(*gtfs_files, **kwargs)
-
-    def add_gtfs_data(self, zip_filelike: os.PathLike):
-        for line in self._get_gtfs_record_iter(zip_filelike, "routes.txt"):
-            id = line["route_id"]
-            self.route_infos[id] = RouteInfo(line)
-
-    def get_routes(self):
-        return self.route_infos.keys()
-
-    def __getitem__(self, key):
-        return self.route_infos[key]
-
-    def get(self, key: str | None, default: Any | None = None):
-        return self.route_infos.get(key, default)
+import os
+from enum import Enum
+from typing import Any
+
+from gtfs_station_stop.static_database import GtfsStaticDatabase
+
+
+class RouteType(Enum):
+    UNKNOWN = -1
+
+    TRAM = 0
+    SUBWAY = 1
+    RAIL = 2
+    BUS = 3
+    FERRY = 4
+    CABLE_TRAM = 5
+    AERIAL_LIFT = 6
+    FUNICULAR = 7
+    TROLLEYBUS = 11
+
+    RAILWAY_SERVICE = 100
+    HIGH_SPEED_RAIL_SERVICE = 101
+    LONG_DISTANCE_TRAIN = 102
+    INTER_REGIONAL_RAIL_SERVICE = 103
+    CAR_TRANSPORT_RAIL_SERVICE = 104
+    SLEEPER_RAIL_SERVICE = 105
+    REGIONAL_RAIL_SERVICE = 106
+    TOURIST_RAIL_SERVICE = 107
+    RAIL_SHUTTLE_WITHIN_COMPLEX = 108
+    SUBURBAN_RAILWAY = 109
+    REPLACEMENT_RAIL_SERVICE = 110
+    SPECIAL_RAIL_SERVICE = 111
+    LORRY_TRANSPORT_RAIL = 112
+
+    BUS_SERVICE = 700
+    REGIONAL_BUS_SERVICE = 701
+    EXPRESS_BUS_SERVICE = 702
+    STOPPING_BUS_SERVICE = 703
+    LOCAL_BUS_SERVICE = 704
+    NIGHT_BUS_SERVICE = 705
+    POST_BUS_SERVICE = 706
+    SPECIAL_NEEDS_BUS = 707
+    MOBILITY_BUS_SERVICE = 708
+    MOBILITY_BUS_FOR_REGISTERED_DISABLED = 709
+    SIGHTSEEING_BUS = 710
+    SHUTTLE_BUS = 711
+    SCHOOL_BUS = 712
+    SCHOOL_AND_PUBLIC_SERVICE_BUS = 713
+    RAIL_REPLACEMENT_BUS_SERVICE = 714
+    DEMAND_AND_RESPONSE_BUS_SERVICE = 715
+    ALL_BUS_SERVICES = 716
+
+    @classmethod
+    def _missing_(cls, value):
+        if isinstance(value, str):
+            value = int(value)
+            for member in cls:
+                if member.value == value:
+                    return member
+        return cls.UNKNOWN
+
+    def pretty_name(self):
+        PRETTY_NAMES = {
+            RouteType.TRAM: "Tram",
+            RouteType.SUBWAY: "Subway",
+            RouteType.RAIL: "Rail",
+            RouteType.BUS: "Bus",
+            RouteType.FERRY: "Ferry",
+            RouteType.CABLE_TRAM: "Cable Tram",
+            RouteType.AERIAL_LIFT: "Aerial Lift",
+            RouteType.FUNICULAR: "Funicular",
+            RouteType.TROLLEYBUS: "Trolleybus",
+            RouteType.SHUTTLE_BUS: "Shuttle Bus",
+        }
+        return PRETTY_NAMES.get(self) or self.name
+
+
+class RouteInfo:
+    def __init__(self, route_data_dict: dict):
+        self.agency_id = route_data_dict.get("agency_id")
+        self.id = route_data_dict["route_id"]
+        self.short_name = route_data_dict.get("route_short_name")
+        self.long_name = route_data_dict.get("route_long_name")
+        if self.short_name is None and self.long_name is None:
+            raise ValueError(
+                "Either 'route_short_name' or 'route_long_name' must be provided."
+            )
+        self.type = RouteType(int(route_data_dict["route_type"]))
+        self.desc = route_data_dict.get("route_desc")
+        self.url = route_data_dict.get("route_url")
+        self.color = route_data_dict.get("route_color")
+        self.text_color = route_data_dict.get("route_text_color")
+
+
+class RouteInfoDatabase(GtfsStaticDatabase):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
+        self.route_infos = {}
+        super().__init__(*gtfs_files, **kwargs)
+
+    def add_gtfs_data(self, zip_filelike: os.PathLike):
+        for line in self._get_gtfs_record_iter(zip_filelike, "routes.txt"):
+            id = line["route_id"]
+            self.route_infos[id] = RouteInfo(line)
+
+    def get_routes(self):
+        return self.route_infos.keys()
+
+    def __getitem__(self, key):
+        return self.route_infos[key]
+
+    def get(self, key: str | None, default: Any | None = None):
+        return self.route_infos.get(key, default)
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/route_status.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/route_status.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import time
-
-from gtfs_station_stop.alert import Alert
-from gtfs_station_stop.feed_subject import FeedSubject
-
-
-class RouteStatus:
-    def __init__(self, route_id: str, updater: FeedSubject):
-        self.id = route_id
-        self.updater = updater
-        self.updater.subscribe(self)
-        self.alerts: list[Alert] = []
-        self._last_updated = None
-
-    @property
-    def last_updated(self):
-        """Last update triggered by updater."""
-        return self._last_updated
-
-    def begin_update(self, timestamp: float | None):
-        self.alerts.clear()
-        self._last_updated = timestamp if timestamp is not None else time.time()
+import time
+
+from gtfs_station_stop.alert import Alert
+from gtfs_station_stop.feed_subject import FeedSubject
+
+
+class RouteStatus:
+    def __init__(self, route_id: str, updater: FeedSubject):
+        self.id = route_id
+        self.updater = updater
+        self.updater.subscribe(self)
+        self.alerts: list[Alert] = []
+        self._last_updated = None
+
+    @property
+    def last_updated(self):
+        """Last update triggered by updater."""
+        return self._last_updated
+
+    def begin_update(self, timestamp: float | None):
+        self.alerts.clear()
+        self._last_updated = timestamp if timestamp is not None else time.time()
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/station_stop.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import time
-
-from gtfs_station_stop.alert import Alert
-from gtfs_station_stop.arrival import Arrival
-from gtfs_station_stop.feed_subject import FeedSubject
-
-
-class StationStop:
-    def __init__(self, stop_id: str, updater: FeedSubject):
-        self.id = stop_id
-        self.updater = updater
-        self.updater.subscribe(self)
-        self.arrivals: list[Arrival] = []
-        self.alerts: list[Alert] = []
-        self._last_updated = None
-
-    @property
-    def last_updated(self):
-        return self._last_updated
-
-    def begin_update(self, timestamp: float | None = None):
-        if timestamp is None:
-            timestamp = time.time()
-        self.alerts.clear()
-        self.arrivals.clear()
-        self._last_updated = timestamp
-
-    def get_time_to_arrivals(self, the_time: float | None = None):
-        if the_time is None:
-            the_time = time.time()
-        return [Arrival(a.time - the_time, a.route, a.trip) for a in self.arrivals]
+import time
+
+from gtfs_station_stop.alert import Alert
+from gtfs_station_stop.arrival import Arrival
+from gtfs_station_stop.feed_subject import FeedSubject
+
+
+class StationStop:
+    def __init__(self, stop_id: str, updater: FeedSubject):
+        self.id = stop_id
+        self.updater = updater
+        self.updater.subscribe(self)
+        self.arrivals: list[Arrival] = []
+        self.alerts: list[Alert] = []
+        self._last_updated = None
+
+    @property
+    def last_updated(self):
+        return self._last_updated
+
+    def begin_update(self, timestamp: float | None = None):
+        if timestamp is None:
+            timestamp = time.time()
+        self.alerts.clear()
+        self.arrivals.clear()
+        self._last_updated = timestamp
+
+    def get_time_to_arrivals(self, the_time: float | None = None):
+        if the_time is None:
+            the_time = time.time()
+        return [Arrival(a.time - the_time, a.route, a.trip) for a in self.arrivals]
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/station_stop_info.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/station_stop_info.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import os
-from enum import Enum
-from typing import Any
-
-from gtfs_station_stop.static_database import GtfsStaticDatabase
-
-
-class LocationType(Enum):
-    STOP = 0
-    STATION = 1
-    ENTRANCE = 2
-    GENERIC_NODE = 3
-    BOARDING_AREA = 4
-
-
-class StationStopInfo:
-    pass
-
-
-class StationStopInfo:
-    def __init__(
-        self, station_data_dict: dict, parent: StationStopInfo | None = None
-    ) -> None:
-        parent_station = station_data_dict.get("parent_station")
-        if parent_station and not parent:
-            ValueError("Parent station reference not provided.")
-        self.location_type = StationStopInfo._get_location_type(
-            station_data_dict.get("location_type", "")
-        )
-        self.id = station_data_dict["stop_id"]
-        self.code = station_data_dict.get("stop_code")
-        self.name = station_data_dict.get("stop_name")
-        self.desc = station_data_dict.get("stop_desc")
-        self.lat = station_data_dict.get("stop_lat")
-        self.lon = station_data_dict.get("stop_lon")
-        self.url = station_data_dict.get("stop_url")
-
-        self.parent = parent
-
-    def _get_location_type(raw: str) -> LocationType:
-        if raw == "":
-            return LocationType.STOP
-        return LocationType(int(raw))
-
-    def __repr__(self):
-        return f"{self.id}: {self.name}, lat: {self.lat}, long: {self.lon}{f', parent: {self.parent.id}' if self.parent else ''}"
-
-
-class StationStopInfoDatabase(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
-        self.station_stop_infos = {}
-        super().__init__(*gtfs_files, **kwargs)
-
-    def add_gtfs_data(self, zip_filelike):
-        for line in self._get_gtfs_record_iter(zip_filelike, "stops.txt"):
-            id = line["stop_id"]
-            parent = None
-            if line.get("parent_station"):
-                parent = self.station_stop_infos.get(line["parent_station"])
-            self.station_stop_infos[id] = StationStopInfo(line, parent)
-
-    def get_stop_ids(self) -> list[str]:
-        return self.station_stop_infos.keys()
-
-    def __getitem__(self, key) -> StationStopInfo:
-        return self.station_stop_infos[key]
-
-    def get(self, key: Any, default: Any | None = None):
-        return self.station_stop_infos.get(key, default)
+import os
+from enum import Enum
+from typing import Any
+
+from gtfs_station_stop.static_database import GtfsStaticDatabase
+
+
+class LocationType(Enum):
+    STOP = 0
+    STATION = 1
+    ENTRANCE = 2
+    GENERIC_NODE = 3
+    BOARDING_AREA = 4
+
+
+class StationStopInfo:
+    pass
+
+
+class StationStopInfo:
+    def __init__(
+        self, station_data_dict: dict, parent: StationStopInfo | None = None
+    ) -> None:
+        parent_station = station_data_dict.get("parent_station")
+        if parent_station and not parent:
+            ValueError("Parent station reference not provided.")
+        self.location_type = StationStopInfo._get_location_type(
+            station_data_dict.get("location_type", "")
+        )
+        self.id = station_data_dict["stop_id"]
+        self.code = station_data_dict.get("stop_code")
+        self.name = station_data_dict.get("stop_name")
+        self.desc = station_data_dict.get("stop_desc")
+        self.lat = station_data_dict.get("stop_lat")
+        self.lon = station_data_dict.get("stop_lon")
+        self.url = station_data_dict.get("stop_url")
+
+        self.parent = parent
+
+    def _get_location_type(raw: str) -> LocationType:
+        if raw == "":
+            return LocationType.STOP
+        return LocationType(int(raw))
+
+    def __repr__(self):
+        return f"{self.id}: {self.name}, lat: {self.lat}, long: {self.lon}{f', parent: {self.parent.id}' if self.parent else ''}"
+
+
+class StationStopInfoDatabase(GtfsStaticDatabase):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
+        self.station_stop_infos = {}
+        super().__init__(*gtfs_files, **kwargs)
+
+    def add_gtfs_data(self, zip_filelike):
+        for line in self._get_gtfs_record_iter(zip_filelike, "stops.txt"):
+            id = line["stop_id"]
+            parent = None
+            if line.get("parent_station"):
+                parent = self.station_stop_infos.get(line["parent_station"])
+            self.station_stop_infos[id] = StationStopInfo(line, parent)
+
+    def get_stop_ids(self) -> list[str]:
+        return self.station_stop_infos.keys()
+
+    def __getitem__(self, key) -> StationStopInfo:
+        return self.station_stop_infos[key]
+
+    def get(self, key: Any, default: Any | None = None):
+        return self.station_stop_infos.get(key, default)
```

### Comparing `gtfs_station_stop-0.7.0b5/src/gtfs_station_stop/trip_info.py` & `gtfs_station_stop-0.8.0/src/gtfs_station_stop/trip_info.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import os
-from collections.abc import Iterable
-from datetime import date, datetime
-from typing import Any
-
-from gtfs_station_stop.calendar import Calendar
-from gtfs_station_stop.static_database import GtfsStaticDatabase
-
-
-class TripInfo:
-    def __init__(self, trip_data_dict: dict):
-        self.route_id = trip_data_dict["route_id"]
-        self.trip_id = trip_data_dict["trip_id"]
-        self.service_id = trip_data_dict["service_id"]
-        self.trip_headsign = trip_data_dict.get("trip_headsign", "")
-        self.trip_short_name = trip_data_dict.get("trip_short_name", "")
-        self.direction_id = trip_data_dict.get("direction_id")
-        self.shape_id = trip_data_dict.get("shape_id")
-
-    def __repr__(self):
-        return f"{self.trip_id}: {self.route_id} to {self.trip_headsign}"
-
-
-class TripInfoDatabase(GtfsStaticDatabase):
-    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
-        self.trip_infos = {}
-        self.__cached_route_ids = None
-        super().__init__(*gtfs_files, **kwargs)
-
-    def add_gtfs_data(self, zip_filepath: os.PathLike):
-        for line in self._get_gtfs_record_iter(zip_filepath, "trips.txt"):
-            id = line["trip_id"]
-            self.trip_infos[id] = TripInfo(line)
-        # invalidate the cache
-        self.__cached_route_ids = None
-
-    def get_close_match(
-        self,
-        key,
-        service_finder: str | Calendar | Iterable[str] | None = None,
-        the_date: date | datetime = date.today(),
-    ) -> TripInfo | None:
-        """Gets the first close match for a given trip ID using either none, a specific service ID, or a calendar and date. When using Calendar, a date can be provided, defaults to today."""
-        active_services: set[str] = set()
-        if isinstance(service_finder, str):
-            active_services = [service_finder]
-        elif isinstance(service_finder, Calendar):
-            active_services = set(
-                s.service_id for s in service_finder.get_active_services(the_date)
-            )
-
-        if isinstance(the_date, datetime):
-            the_date = the_date.date()
-
-        return next(
-            (
-                trip_info
-                for trip_id, trip_info in self.trip_infos.items()
-                if key in trip_id
-                and (
-                    len(active_services) == 0 or trip_info.service_id in active_services
-                )
-            ),
-            None,
-        )
-
-    def get_route_ids(self) -> list[str]:
-        # cache this as it may be expensive to rerun the querey
-        if self.__cached_route_ids is None:
-            self.__cached_route_ids = list(
-                set(ti.route_id for ti in self.trip_infos.values() if ti.route_id)
-            )
-        return self.__cached_route_ids
-
-    def __getitem__(self, key) -> TripInfo:
-        return self.trip_infos[key]
-
-    def get(self, key: Any, default: Any | None = None):
-        return self.trip_infos.get(key, default)
+import os
+from collections.abc import Iterable
+from datetime import date, datetime
+from typing import Any
+
+from gtfs_station_stop.calendar import Calendar
+from gtfs_station_stop.static_database import GtfsStaticDatabase
+
+
+class TripInfo:
+    def __init__(self, trip_data_dict: dict):
+        self.route_id = trip_data_dict["route_id"]
+        self.trip_id = trip_data_dict["trip_id"]
+        self.service_id = trip_data_dict["service_id"]
+        self.trip_headsign = trip_data_dict.get("trip_headsign", "")
+        self.trip_short_name = trip_data_dict.get("trip_short_name", "")
+        self.direction_id = trip_data_dict.get("direction_id")
+        self.shape_id = trip_data_dict.get("shape_id")
+
+    def __repr__(self):
+        return f"{self.trip_id}: {self.route_id} to {self.trip_headsign}"
+
+
+class TripInfoDatabase(GtfsStaticDatabase):
+    def __init__(self, *gtfs_files: os.PathLike, **kwargs):
+        self.trip_infos = {}
+        self.__cached_route_ids = None
+        super().__init__(*gtfs_files, **kwargs)
+
+    def add_gtfs_data(self, zip_filepath: os.PathLike):
+        for line in self._get_gtfs_record_iter(zip_filepath, "trips.txt"):
+            id = line["trip_id"]
+            self.trip_infos[id] = TripInfo(line)
+        # invalidate the cache
+        self.__cached_route_ids = None
+
+    def get_close_match(
+        self,
+        key,
+        service_finder: str | Calendar | Iterable[str] | None = None,
+        the_date: date | datetime = date.today(),
+    ) -> TripInfo | None:
+        """Gets the first close match for a given trip ID using either none, a specific service ID, or a calendar and date. When using Calendar, a date can be provided, defaults to today."""
+        active_services: set[str] = set()
+        if isinstance(service_finder, str):
+            active_services = [service_finder]
+        elif isinstance(service_finder, Calendar):
+            active_services = set(
+                s.service_id for s in service_finder.get_active_services(the_date)
+            )
+
+        if isinstance(the_date, datetime):
+            the_date = the_date.date()
+
+        return next(
+            (
+                trip_info
+                for trip_id, trip_info in self.trip_infos.items()
+                if key in trip_id
+                and (
+                    len(active_services) == 0 or trip_info.service_id in active_services
+                )
+            ),
+            None,
+        )
+
+    def get_route_ids(self) -> list[str]:
+        # cache this as it may be expensive to rerun the querey
+        if self.__cached_route_ids is None:
+            self.__cached_route_ids = list(
+                set(ti.route_id for ti in self.trip_infos.values() if ti.route_id)
+            )
+        return self.__cached_route_ids
+
+    def __getitem__(self, key) -> TripInfo:
+        return self.trip_infos[key]
+
+    def get(self, key: Any, default: Any | None = None):
+        return self.trip_infos.get(key, default)
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/fixtures.py` & `gtfs_station_stop-0.8.0/tests/fixtures.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import os
-import pathlib
-
-import dotenv
-import pytest
-from mock_feed_server import create_mock_feed_server
-
-from gtfs_station_stop.calendar import Calendar
-from gtfs_station_stop.feed_subject import FeedSubject
-from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
-from gtfs_station_stop.trip_info import TripInfoDatabase
-
-
-@pytest.fixture(scope="session")
-def test_directory():
-    return pathlib.Path(__file__).parent.resolve()
-
-
-@pytest.fixture(scope="session")
-def good_trip_info_database(test_directory):
-    return TripInfoDatabase(test_directory / "data" / "gtfs_static.zip")
-
-
-@pytest.fixture
-def good_station_stop_info_db(test_directory):
-    return StationStopInfoDatabase(test_directory / "data" / "gtfs_static.zip")
-
-
-@pytest.fixture(scope="session")
-def mock_feed_server(test_directory):
-    server = create_mock_feed_server(test_directory / "data")
-
-    yield server
-
-    server.clear()
-    if server.is_running():
-        server.stop()
-
-    server.check_assertions()
-    server.clear()
-
-
-@pytest.fixture
-def mock_feed_subject(mock_feed_server):
-    return FeedSubject(mock_feed_server.realtime_urls)
-
-
-@pytest.fixture
-def nyct_feed_subject():
-    feed_urls = [
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs",
-        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/camsys%2Fsubway-alerts",
-    ]
-    dotenv.load_dotenv()
-    return FeedSubject(
-        feed_urls,
-        headers={"x-api-key": os.environ.get("API_KEY")},
-    )
-
-
-@pytest.fixture
-def feed_subject(mock_feed_subject, nyct_feed_subject):
-    # Set the feed server to use either mock data read from the tests/data directory, or to use real data
-    # By default, use mock data
-    feed_dict = {"MOCK": mock_feed_subject, "NYCT": nyct_feed_subject}
-    feed_key = os.environ.get("GTFS_SOURCE", "MOCK")
-    print(f"Using feed subject {feed_key}")
-    return feed_dict.get(feed_key)
-
-
-@pytest.fixture
-def gtfs_calendar(test_directory):
-    return Calendar(test_directory / "data" / "gtfs_static.zip")
+import os
+import pathlib
+
+import dotenv
+import pytest
+from mock_feed_server import create_mock_feed_server
+
+from gtfs_station_stop.calendar import Calendar
+from gtfs_station_stop.feed_subject import FeedSubject
+from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
+from gtfs_station_stop.trip_info import TripInfoDatabase
+
+
+@pytest.fixture(scope="session")
+def test_directory():
+    return pathlib.Path(__file__).parent.resolve()
+
+
+@pytest.fixture(scope="session")
+def good_trip_info_database(test_directory):
+    return TripInfoDatabase(test_directory / "data" / "gtfs_static.zip")
+
+
+@pytest.fixture
+def good_station_stop_info_db(test_directory):
+    return StationStopInfoDatabase(test_directory / "data" / "gtfs_static.zip")
+
+
+@pytest.fixture(scope="session")
+def mock_feed_server(test_directory):
+    server = create_mock_feed_server(test_directory / "data")
+
+    yield server
+
+    server.clear()
+    if server.is_running():
+        server.stop()
+
+    server.check_assertions()
+    server.clear()
+
+
+@pytest.fixture
+def mock_feed_subject(mock_feed_server):
+    return FeedSubject(mock_feed_server.realtime_urls)
+
+
+@pytest.fixture
+def nyct_feed_subject():
+    feed_urls = [
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-bdfm",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-g",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-jz",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-nqrw",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs-l",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/nyct%2Fgtfs",
+        "https://api-endpoint.mta.info/Dataservice/mtagtfsfeeds/camsys%2Fsubway-alerts",
+    ]
+    dotenv.load_dotenv()
+    return FeedSubject(
+        feed_urls,
+        headers={"x-api-key": os.environ.get("API_KEY")},
+    )
+
+
+@pytest.fixture
+def feed_subject(mock_feed_subject, nyct_feed_subject):
+    # Set the feed server to use either mock data read from the tests/data directory, or to use real data
+    # By default, use mock data
+    feed_dict = {"MOCK": mock_feed_subject, "NYCT": nyct_feed_subject}
+    feed_key = os.environ.get("GTFS_SOURCE", "MOCK")
+    print(f"Using feed subject {feed_key}")
+    return feed_dict.get(feed_key)
+
+
+@pytest.fixture
+def gtfs_calendar(test_directory):
+    return Calendar(test_directory / "data" / "gtfs_static.zip")
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/mock_feed_server.py` & `gtfs_station_stop-0.8.0/tests/mock_feed_server.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import glob
-import os
-import pathlib
-
-import pytest_httpserver
-
-
-def create_mock_feed_server(data_directory: os.PathLike):
-    """Creates a Mock Feed using local files."""
-    server = pytest_httpserver.HTTPServer()
-    server.start()
-
-    # Install the requests that point to realtime files
-    MOCK_REALTIME_DATA_MAP = dict(
-        (f"/{path.name}", path.read_bytes())
-        for path in (
-            pathlib.Path(x)
-            for x in glob.glob(str(pathlib.Path(data_directory) / "*.dat"))
-        )
-    )
-    server.realtime_urls = []
-    for endpoint, data in MOCK_REALTIME_DATA_MAP.items():
-        server.expect_request(endpoint).respond_with_data(data)
-        server.realtime_urls.append(server.url_for(endpoint))
-
-    # Install the requests that point to static files
-    MOCK_STATIC_DATA_MAP = dict(
-        (f"/{path.name}", path.read_bytes())
-        for path in (
-            pathlib.Path(x)
-            for x in glob.glob(str(pathlib.Path(data_directory) / "*.zip"))
-        )
-    )
-    server.static_urls = []
-    for endpoint, data in MOCK_STATIC_DATA_MAP.items():
-        server.expect_request(endpoint).respond_with_data(data)
-        server.static_urls.append(server.url_for(endpoint))
-
-    return server
+import glob
+import os
+import pathlib
+
+import pytest_httpserver
+
+
+def create_mock_feed_server(data_directory: os.PathLike):
+    """Creates a Mock Feed using local files."""
+    server = pytest_httpserver.HTTPServer()
+    server.start()
+
+    # Install the requests that point to realtime files
+    MOCK_REALTIME_DATA_MAP = dict(
+        (f"/{path.name}", path.read_bytes())
+        for path in (
+            pathlib.Path(x)
+            for x in glob.glob(str(pathlib.Path(data_directory) / "*.dat"))
+        )
+    )
+    server.realtime_urls = []
+    for endpoint, data in MOCK_REALTIME_DATA_MAP.items():
+        server.expect_request(endpoint).respond_with_data(data)
+        server.realtime_urls.append(server.url_for(endpoint))
+
+    # Install the requests that point to static files
+    MOCK_STATIC_DATA_MAP = dict(
+        (f"/{path.name}", path.read_bytes())
+        for path in (
+            pathlib.Path(x)
+            for x in glob.glob(str(pathlib.Path(data_directory) / "*.zip"))
+        )
+    )
+    server.static_urls = []
+    for endpoint, data in MOCK_STATIC_DATA_MAP.items():
+        server.expect_request(endpoint).respond_with_data(data)
+        server.static_urls.append(server.url_for(endpoint))
+
+    return server
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_calendar.py` & `gtfs_station_stop-0.8.0/tests/test_calendar.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from datetime import date, datetime
-
-import pytest
-
-from gtfs_station_stop.calendar import Calendar
-
-
-def test_invalid_gtfs_zip(test_directory):
-    with pytest.raises(RuntimeError):
-        Calendar(test_directory / "data" / "gtfs_static_nocalendar.zip")
-
-
-def test_get_station_stop_info_from_zip_calendar_txt(gtfs_calendar):
-    service = gtfs_calendar["Regular"]
-    # GTFS Data for test has Regular Service active on all weekdays, but not weekends
-    assert (
-        service.is_active_on(datetime(year=2024, month=3, day=4)) is True
-    ), "Regular Service active on a weekday."
-    assert (
-        service.is_active_on(datetime(year=2024, month=3, day=9)) is False
-    ), "Regular Service not active on a weekend."
-    # Test with date too
-    assert (
-        service.is_active_on(date(year=2024, month=3, day=4)) is True
-    ), "Regular Service active on a weekday."
-    assert (
-        service.is_active_on(date(year=2024, month=3, day=9)) is False
-    ), "Regular Service not active on a weekend."
-
-
-def test_get_station_stop_info_from_zip_calendar_dates_txt(gtfs_calendar):
-    assert (
-        gtfs_calendar["Regular"].is_active_on(date(year=2024, month=12, day=25))
-        is False
-    ), "No Regular service on Christmas."
-    assert (
-        gtfs_calendar["PiDaySpecial"].is_active_on(date(year=2024, month=3, day=14))
-        is True
-    ), "Service 'PiDaySpecial' should be added for 2024-03-14."
-
-    assert (
-        gtfs_calendar["PiDaySpecial"].is_active_on(date(year=2024, month=3, day=13))
-        is False
-    ), "Service PiDaySpecial should not be active for 2024-03-13."
+from datetime import date, datetime
+
+import pytest
+
+from gtfs_station_stop.calendar import Calendar
+
+
+def test_invalid_gtfs_zip(test_directory):
+    with pytest.raises(RuntimeError):
+        Calendar(test_directory / "data" / "gtfs_static_nocalendar.zip")
+
+
+def test_get_station_stop_info_from_zip_calendar_txt(gtfs_calendar):
+    service = gtfs_calendar["Regular"]
+    # GTFS Data for test has Regular Service active on all weekdays, but not weekends
+    assert (
+        service.is_active_on(datetime(year=2024, month=3, day=4)) is True
+    ), "Regular Service active on a weekday."
+    assert (
+        service.is_active_on(datetime(year=2024, month=3, day=9)) is False
+    ), "Regular Service not active on a weekend."
+    # Test with date too
+    assert (
+        service.is_active_on(date(year=2024, month=3, day=4)) is True
+    ), "Regular Service active on a weekday."
+    assert (
+        service.is_active_on(date(year=2024, month=3, day=9)) is False
+    ), "Regular Service not active on a weekend."
+
+
+def test_get_station_stop_info_from_zip_calendar_dates_txt(gtfs_calendar):
+    assert (
+        gtfs_calendar["Regular"].is_active_on(date(year=2024, month=12, day=25))
+        is False
+    ), "No Regular service on Christmas."
+    assert (
+        gtfs_calendar["PiDaySpecial"].is_active_on(date(year=2024, month=3, day=14))
+        is True
+    ), "Service 'PiDaySpecial' should be added for 2024-03-14."
+
+    assert (
+        gtfs_calendar["PiDaySpecial"].is_active_on(date(year=2024, month=3, day=13))
+        is False
+    ), "Service PiDaySpecial should not be active for 2024-03-13."
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_route_info.py` & `gtfs_station_stop-0.8.0/tests/test_route_info.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import pytest
-
-from gtfs_station_stop.route_info import RouteInfoDatabase, RouteType
-
-
-def test_invalid_gtfs_zip(test_directory):
-    with pytest.raises(RuntimeError):
-        RouteInfoDatabase(test_directory / "data" / "gtfs_static_noroutes.zip")
-
-
-def test_get_route_info_from_zip(test_directory):
-    ri_db = RouteInfoDatabase(test_directory / "data" / "gtfs_static.zip")
-    assert ri_db.route_infos["X"].long_name == "X Test Route"
-    assert ri_db.route_infos["Y"].long_name == "Y Test Route"
-    assert ri_db.route_infos["X"].color == "EE352E"
-    assert ri_db.route_infos["X"].type == RouteType.SUBWAY
-
-
-def test_route_info_has_pretty_name():
-    assert RouteType.SUBWAY.pretty_name() == "Subway"
-
-
-def test_route_info_pretty_name_fallback():
-    assert RouteType.RAILWAY_SERVICE.pretty_name() == "RAILWAY_SERVICE"
-
-
-def test_route_info_default_unknown():
-    assert RouteType(-42) == RouteType.UNKNOWN
+import pytest
+
+from gtfs_station_stop.route_info import RouteInfoDatabase, RouteType
+
+
+def test_invalid_gtfs_zip(test_directory):
+    with pytest.raises(RuntimeError):
+        RouteInfoDatabase(test_directory / "data" / "gtfs_static_noroutes.zip")
+
+
+def test_get_route_info_from_zip(test_directory):
+    ri_db = RouteInfoDatabase(test_directory / "data" / "gtfs_static.zip")
+    assert ri_db.route_infos["X"].long_name == "X Test Route"
+    assert ri_db.route_infos["Y"].long_name == "Y Test Route"
+    assert ri_db.route_infos["X"].color == "EE352E"
+    assert ri_db.route_infos["X"].type == RouteType.SUBWAY
+
+
+def test_route_info_has_pretty_name():
+    assert RouteType.SUBWAY.pretty_name() == "Subway"
+
+
+def test_route_info_pretty_name_fallback():
+    assert RouteType.RAILWAY_SERVICE.pretty_name() == "RAILWAY_SERVICE"
+
+
+def test_route_info_default_unknown():
+    assert RouteType(-42) == RouteType.UNKNOWN
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_route_status.py` & `gtfs_station_stop-0.8.0/tests/test_route_status.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from gtfs_station_stop.feed_subject import FeedSubject
-from gtfs_station_stop.route_status import RouteStatus
-
-
-def test_create_route_status():
-    rs = RouteStatus("Z", FeedSubject([]))
-    assert hasattr(rs, "alerts")
-
-
-def test_subscribe_to_feed(feed_subject):
-    rs = RouteStatus("Z", feed_subject)
-    assert len(feed_subject.subscribers) == 1
-    del rs
-
-
-def test_update_feed(feed_subject):
-    rs = RouteStatus("Z", feed_subject)
-    assert rs.last_updated is None
-    feed_subject.update()
-    assert len(rs.alerts) == 1
-    assert rs.last_updated is not None
+from gtfs_station_stop.feed_subject import FeedSubject
+from gtfs_station_stop.route_status import RouteStatus
+
+
+def test_create_route_status():
+    rs = RouteStatus("Z", FeedSubject([]))
+    assert hasattr(rs, "alerts")
+
+
+def test_subscribe_to_feed(feed_subject):
+    rs = RouteStatus("Z", feed_subject)
+    assert len(feed_subject.subscribers) == 1
+    del rs
+
+
+def test_update_feed(feed_subject):
+    rs = RouteStatus("Z", feed_subject)
+    assert rs.last_updated is None
+    feed_subject.update()
+    assert len(rs.alerts) == 1
+    assert rs.last_updated is not None
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_station_stop.py` & `gtfs_station_stop-0.8.0/tests/test_station_stop.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import datetime
-import time
-
-import pytest
-from freezegun import freeze_time
-
-from gtfs_station_stop.feed_subject import FeedSubject
-from gtfs_station_stop.station_stop import StationStop
-
-
-def test_create_station_stop():
-    ss = StationStop("L20N", FeedSubject([]))
-    assert hasattr(ss, "alerts")
-    assert hasattr(ss, "arrivals")
-
-
-def test_subscribe_to_feed(feed_subject):
-    ss = StationStop("L20N", feed_subject)
-    assert len(feed_subject.subscribers) == 1
-    del ss
-
-
-@freeze_time(datetime.datetime.now())
-def test_update_feed(feed_subject):
-    ss = StationStop("101N", feed_subject)
-    assert ss.last_updated is None
-    feed_subject.update()
-    assert len(ss.arrivals) == 2
-    assert ss.last_updated == time.time()
-    arrival_routes = [a.route for a in ss.arrivals]
-    assert "X" in arrival_routes
-    assert "Y" in arrival_routes
-
-
-@pytest.mark.asyncio
-@freeze_time(datetime.datetime.now())
-async def test_async_update_feed(feed_subject):
-    """Asynchronous version of update."""
-    ss = StationStop("101N", feed_subject)
-    assert ss.last_updated is None
-    await feed_subject.async_update()
-    assert len(ss.arrivals) == 2
-    assert ss.last_updated == time.time()
-    arrival_routes = [a.route for a in ss.arrivals]
-    assert "X" in arrival_routes
-    assert "Y" in arrival_routes
-
-
-def test_multiple_subscribers(feed_subject):
-    ss1 = StationStop("103N", feed_subject)
-    ss2 = StationStop("103S", feed_subject)
-    assert ss1.last_updated is None
-    assert ss2.last_updated is None
-    feed_subject.unsubscribe(ss2)
-    feed_subject.update()
-    assert ss1.last_updated is not None
-    assert ss2.last_updated is None
-    assert len(ss1.arrivals) == 3
-    assert len(ss2.arrivals) == 0
+import datetime
+import time
+
+import pytest
+from freezegun import freeze_time
+
+from gtfs_station_stop.feed_subject import FeedSubject
+from gtfs_station_stop.station_stop import StationStop
+
+
+def test_create_station_stop():
+    ss = StationStop("L20N", FeedSubject([]))
+    assert hasattr(ss, "alerts")
+    assert hasattr(ss, "arrivals")
+
+
+def test_subscribe_to_feed(feed_subject):
+    ss = StationStop("L20N", feed_subject)
+    assert len(feed_subject.subscribers) == 1
+    del ss
+
+
+@freeze_time(datetime.datetime.now())
+def test_update_feed(feed_subject):
+    ss = StationStop("101N", feed_subject)
+    assert ss.last_updated is None
+    feed_subject.update()
+    assert len(ss.arrivals) == 2
+    assert ss.last_updated == time.time()
+    arrival_routes = [a.route for a in ss.arrivals]
+    assert "X" in arrival_routes
+    assert "Y" in arrival_routes
+
+
+@pytest.mark.asyncio
+@freeze_time(datetime.datetime.now())
+async def test_async_update_feed(feed_subject):
+    """Asynchronous version of update."""
+    ss = StationStop("101N", feed_subject)
+    assert ss.last_updated is None
+    await feed_subject.async_update()
+    assert len(ss.arrivals) == 2
+    assert ss.last_updated == time.time()
+    arrival_routes = [a.route for a in ss.arrivals]
+    assert "X" in arrival_routes
+    assert "Y" in arrival_routes
+
+
+def test_multiple_subscribers(feed_subject):
+    ss1 = StationStop("103N", feed_subject)
+    ss2 = StationStop("103S", feed_subject)
+    assert ss1.last_updated is None
+    assert ss2.last_updated is None
+    feed_subject.unsubscribe(ss2)
+    feed_subject.update()
+    assert ss1.last_updated is not None
+    assert ss2.last_updated is None
+    assert len(ss1.arrivals) == 3
+    assert len(ss2.arrivals) == 0
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_station_stop_info.py` & `gtfs_station_stop-0.8.0/tests/test_station_stop_info.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import pytest
-
-from gtfs_station_stop.static_database import async_factory
-from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
-
-pytest_plugins = ("pytest_asyncio",)
-
-
-def test_invalid_gtfs_zip(test_directory):
-    with pytest.raises(RuntimeError):
-        StationStopInfoDatabase(test_directory / "data" / "gtfs_static_nostops.zip")
-
-
-def test_get_station_stop_info_from_zip(good_station_stop_info_db):
-    ssi = good_station_stop_info_db
-    assert ssi["101"].name == "Test Station Main St"
-    assert ssi["101N"].name == "Test Station Main St"
-    assert ssi["102S"].parent == ssi["102"]
-
-
-def test_conatenated_station_stop_info_from_zip(test_directory):
-    gtfs_static_zips = [
-        test_directory / "data" / "gtfs_static.zip",
-        test_directory / "data" / "gtfs_static_supl.zip",
-    ]
-    ssi = StationStopInfoDatabase(*gtfs_static_zips)
-    assert ssi["101"].name == "Test Station Main St"
-    assert ssi["201"].name == "Test Station Last St"
-
-
-def test_get_station_stop_info_from_url(mock_feed_server):
-    ssi = StationStopInfoDatabase(
-        *[
-            url
-            for url in mock_feed_server.static_urls
-            if url.endswith("gtfs_static.zip")
-        ]
-    )
-    assert ssi["101"].name == "Test Station Main St"
-    assert ssi["101N"].name == "Test Station Main St"
-    assert ssi["102S"].parent == ssi["102"]
-
-
-@pytest.mark.asyncio
-async def test_async_get_station_stop_info_from_url(mock_feed_server):
-    ssi = await async_factory(
-        StationStopInfoDatabase,
-        *[
-            url
-            for url in mock_feed_server.static_urls
-            if url.endswith("gtfs_static.zip")
-        ],
-        headers={"api-key": "TEST_KEY"},
-    )
-    assert ssi["101"].name == "Test Station Main St"
-    assert ssi["101N"].name == "Test Station Main St"
-    assert ssi["102S"].parent == ssi["102"]
-
-
-def test_get_stop_ids(good_station_stop_info_db):
-    ssi = good_station_stop_info_db
-    assert set(ssi.get_stop_ids()) == set(
-        ["101", "101N", "101S", "102", "102S", "102N", "103", "103N", "103S"]
-    )
+import pytest
+
+from gtfs_station_stop.static_database import async_factory
+from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
+
+pytest_plugins = ("pytest_asyncio",)
+
+
+def test_invalid_gtfs_zip(test_directory):
+    with pytest.raises(RuntimeError):
+        StationStopInfoDatabase(test_directory / "data" / "gtfs_static_nostops.zip")
+
+
+def test_get_station_stop_info_from_zip(good_station_stop_info_db):
+    ssi = good_station_stop_info_db
+    assert ssi["101"].name == "Test Station Main St"
+    assert ssi["101N"].name == "Test Station Main St"
+    assert ssi["102S"].parent == ssi["102"]
+
+
+def test_conatenated_station_stop_info_from_zip(test_directory):
+    gtfs_static_zips = [
+        test_directory / "data" / "gtfs_static.zip",
+        test_directory / "data" / "gtfs_static_supl.zip",
+    ]
+    ssi = StationStopInfoDatabase(*gtfs_static_zips)
+    assert ssi["101"].name == "Test Station Main St"
+    assert ssi["201"].name == "Test Station Last St"
+
+
+def test_get_station_stop_info_from_url(mock_feed_server):
+    ssi = StationStopInfoDatabase(
+        *[
+            url
+            for url in mock_feed_server.static_urls
+            if url.endswith("gtfs_static.zip")
+        ]
+    )
+    assert ssi["101"].name == "Test Station Main St"
+    assert ssi["101N"].name == "Test Station Main St"
+    assert ssi["102S"].parent == ssi["102"]
+
+
+@pytest.mark.asyncio
+async def test_async_get_station_stop_info_from_url(mock_feed_server):
+    ssi = await async_factory(
+        StationStopInfoDatabase,
+        *[
+            url
+            for url in mock_feed_server.static_urls
+            if url.endswith("gtfs_static.zip")
+        ],
+        headers={"api-key": "TEST_KEY"},
+    )
+    assert ssi["101"].name == "Test Station Main St"
+    assert ssi["101N"].name == "Test Station Main St"
+    assert ssi["102S"].parent == ssi["102"]
+
+
+def test_get_stop_ids(good_station_stop_info_db):
+    ssi = good_station_stop_info_db
+    assert set(ssi.get_stop_ids()) == set(
+        ["101", "101N", "101S", "102", "102S", "102N", "103", "103N", "103S"]
+    )
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/test_trip_info.py` & `gtfs_station_stop-0.8.0/tests/test_trip_info.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import pathlib
-
-import pytest
-
-from gtfs_station_stop.trip_info import TripInfoDatabase
-
-TEST_DIRECTORY = pathlib.Path(__file__).parent.resolve()
-
-
-def test_invalid_gtfs_zip():
-    with pytest.raises(RuntimeError):
-        TripInfoDatabase(TEST_DIRECTORY / "data" / "gtfs_static_notrips.zip")
-
-
-def test_get_trip_info_from_zip(good_trip_info_database):
-    assert good_trip_info_database["456_X..N04R"].service_id == "Weekday"
-    assert good_trip_info_database["456_X..N04R"].shape_id == "X..N04R"
-    assert good_trip_info_database["456_Y..N05R"].trip_headsign == "Northbound Y"
-
-
-def test_get_close_match_trip_info_from_zip(good_trip_info_database):
-    assert (
-        good_trip_info_database.get_close_match("456_X..N").trip_headsign
-        == "Northbound X"
-    )
-    assert good_trip_info_database.get_close_match("321_Z..S").route_id == "Z"
-
-
-def test_get_close_match_trip_with_service_id_from_zip(good_trip_info_database):
-    assert good_trip_info_database.get_close_match("456_X..N", "Special") is None
-    assert good_trip_info_database.get_close_match("456_X..N", "Weekday") is not None
-
-
-def test_concatenated_trip_info_from_zips():
-    gtfs_static_zips = [
-        TEST_DIRECTORY / "data" / "gtfs_static.zip",
-        TEST_DIRECTORY / "data" / "gtfs_static_supl.zip",
-    ]
-    ti = TripInfoDatabase(*gtfs_static_zips)
-    assert ti.get_close_match("456_X..N").trip_headsign == "Northbound X"
-    assert ti.get_close_match("987_X..S21R").trip_headsign == "Southbound Special X"
-
-
-def test_get_trip_info_from_url(mock_feed_server):
-    ti = TripInfoDatabase(
-        *[
-            url
-            for url in mock_feed_server.static_urls
-            if url.endswith("gtfs_static.zip")
-        ]
-    )
-    assert ti["456_X..N04R"].service_id == "Weekday"
-    assert ti["456_X..N04R"].shape_id == "X..N04R"
-    assert ti["456_Y..N05R"].trip_headsign == "Northbound Y"
-
-
-def test_get_route_ids(good_trip_info_database):
-    ti = good_trip_info_database
-    assert set(ti.get_route_ids()) == set(["X", "Y", "Z"])
+import pathlib
+
+import pytest
+
+from gtfs_station_stop.trip_info import TripInfoDatabase
+
+TEST_DIRECTORY = pathlib.Path(__file__).parent.resolve()
+
+
+def test_invalid_gtfs_zip():
+    with pytest.raises(RuntimeError):
+        TripInfoDatabase(TEST_DIRECTORY / "data" / "gtfs_static_notrips.zip")
+
+
+def test_get_trip_info_from_zip(good_trip_info_database):
+    assert good_trip_info_database["456_X..N04R"].service_id == "Weekday"
+    assert good_trip_info_database["456_X..N04R"].shape_id == "X..N04R"
+    assert good_trip_info_database["456_Y..N05R"].trip_headsign == "Northbound Y"
+
+
+def test_get_close_match_trip_info_from_zip(good_trip_info_database):
+    assert (
+        good_trip_info_database.get_close_match("456_X..N").trip_headsign
+        == "Northbound X"
+    )
+    assert good_trip_info_database.get_close_match("321_Z..S").route_id == "Z"
+
+
+def test_get_close_match_trip_with_service_id_from_zip(good_trip_info_database):
+    assert good_trip_info_database.get_close_match("456_X..N", "Special") is None
+    assert good_trip_info_database.get_close_match("456_X..N", "Weekday") is not None
+
+
+def test_concatenated_trip_info_from_zips():
+    gtfs_static_zips = [
+        TEST_DIRECTORY / "data" / "gtfs_static.zip",
+        TEST_DIRECTORY / "data" / "gtfs_static_supl.zip",
+    ]
+    ti = TripInfoDatabase(*gtfs_static_zips)
+    assert ti.get_close_match("456_X..N").trip_headsign == "Northbound X"
+    assert ti.get_close_match("987_X..S21R").trip_headsign == "Southbound Special X"
+
+
+def test_get_trip_info_from_url(mock_feed_server):
+    ti = TripInfoDatabase(
+        *[
+            url
+            for url in mock_feed_server.static_urls
+            if url.endswith("gtfs_static.zip")
+        ]
+    )
+    assert ti["456_X..N04R"].service_id == "Weekday"
+    assert ti["456_X..N04R"].shape_id == "X..N04R"
+    assert ti["456_Y..N05R"].trip_headsign == "Northbound Y"
+
+
+def test_get_route_ids(good_trip_info_database):
+    ti = good_trip_info_database
+    assert set(ti.get_route_ids()) == set(["X", "Y", "Z"])
```

### Comparing `gtfs_station_stop-0.7.0b5/tests/data/gtfs_static/trips.txt` & `gtfs_station_stop-0.8.0/tests/data/gtfs_static/trips.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-route_id,trip_id,service_id,trip_headsign,direction_id,shape_id
-X,123_X..N01R,Weekday,Northbound X,0,X..N01R
-X,321_X..S01R,Weekday,Southbound X,1,X..S01R
-X,456_X..N04R,Weekday,Northbound X,0,X..N04R
-X,654_X..S04R,Weekday,Southbound X,1,X..S04R
-Y,123_Y..N02R,Weekday,Northbound Y,0,Y..N02R
-Y,321_Y..S02R,Weekday,Southbound Y,1,Y..S02R
-Y,456_Y..N05R,Weekday,Northbound Y,0,Y..N05R
-Y,654_Y..S05R,Weekday,Southbound Y,1,Y..S05R
-Z,123_Z..N03R,Weekday,Northbound Z,0,Z..N03R
-Z,321_Z..S03R,Weekday,Southbound Z,1,Z..S03R
-Z,456_Z..N06R,Weekday,Northbound Z,0,Z..N06R
-Z,654_Z..S06R,Weekday,Southbound Z,1,Z..S06R
+route_id,trip_id,service_id,trip_headsign,direction_id,shape_id
+X,123_X..N01R,Weekday,Northbound X,0,X..N01R
+X,321_X..S01R,Weekday,Southbound X,1,X..S01R
+X,456_X..N04R,Weekday,Northbound X,0,X..N04R
+X,654_X..S04R,Weekday,Southbound X,1,X..S04R
+Y,123_Y..N02R,Weekday,Northbound Y,0,Y..N02R
+Y,321_Y..S02R,Weekday,Southbound Y,1,Y..S02R
+Y,456_Y..N05R,Weekday,Northbound Y,0,Y..N05R
+Y,654_Y..S05R,Weekday,Southbound Y,1,Y..S05R
+Z,123_Z..N03R,Weekday,Northbound Z,0,Z..N03R
+Z,321_Z..S03R,Weekday,Southbound Z,1,Z..S03R
+Z,456_Z..N06R,Weekday,Northbound Z,0,Z..N06R
+Z,654_Z..S06R,Weekday,Southbound Z,1,Z..S06R
 ,bad,unknown,Eastbound ?,2,u..EXXR
```

### Comparing `gtfs_station_stop-0.7.0b5/README.md` & `gtfs_station_stop-0.8.0/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# GTFS Station Stop
-
-A project for organizing GTFS Real-Time data for use as a homeassistant sensor.
-
-## Usage
-
-This is designed for use with [Home Assistant GTFS Realtime Custom Component](https://github.com/bcpearce/homeassistant-gtfs-realtime).
-
-It can also be used for general GTFS update purposes.
-
-### Feed Subjects and Station Stops
-
-All updates go through the Feed Subject which is setup to call updates from one or more feed URLS.
-
-Create a feed subject like so, then pass it in the constructor for a Station Stop
-
-```python
-from gtfs_station_stop.feed_subject import FeedSubject
-from gtfs_station_stop.station_stop import StationStop
-
-# Obtain the API keep from your GTFS provider if needed, otherwise leave blank.
-api_key = "YOUR_API_KEY_HERE"
-urls = ["https://gtfs.example.com/feed1", "https://gtfs.example.com/feed2"]
-feed_subject = FeedSubject(urls, api_key)
-
-# Obtain the Stop ID from GTFS static data from your provider.
-# This must match those provided by the realtime feed.
-station_stop_nb = StationStop("STOP_ID_NORTHBOUND", feed_subject)
-station_stop_sb = StationStop("STOP_ID_SOUTHBOUND", feed_subject)
-```
-
-Calling `feed_subject.update()` will update all registered listeners.
-
-```python
-feed_subject.update()
-
-for arrival in station_stop_nb.arrivals:
-    minutes_to = (arrival.time - time.time()) / 60.0
-    print(f"{arrival.route} in {minutes_to}")
-```
-
-Active service alerts are also supported for station stops and for routes.
-
-```python
-route_status = RouteStatus("Line 1", feed_subject)
-
-feed_subject.update()
-
-for alert in route_status.alerts:
-    print(f"{route_status.id} alert {alert.header_text['en']}")
-
-for alert in station_stop_nb.alerts:
-    print(f"{station_stop_nb.id} alert {alert.header_text['en']}")
-```
-
-As the update will make one or more http requests, this may improve performance or integrate better with an asynchronous project.
-
-### GTFS Static Info
-
-Static data can be loaded into a database for convenient lookup to use alongside GTFS Realtime data. GTFS data can be read from a file or a URL from your service provider. The GTFS file must be provided as a .zip containing the requisite .txt files as defined by [GTFS Static Reference](https://developers.google.com/transit/gtfs/reference).
-
-```python
-from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
-
-station_stop_info_db = StationStopInfoDatabase("gtfs_static.zip")
-print(f"{station_stop_info_db['STOP_ID']}")
-```
-
-Static info can be queried through the `station_stop_info`, `route_info`, `calendar`, and `trip_info` submodules.
-
-GTFS providers will regularly update their static feeds.  In order to account for this, the library will attempt to cache zip file downloads for static info.
-
-### Async Updates
-
-Asynchronous updates are also supported through the `async_update()` method.
-
-```python
-await feed_subject.async_update()
-```
-
-Static data can also be obtained similarly with `gtfs_station_stop.static_database.async_factory`.
-
-```python
-station_stop_info_database = await async_get_gtfs_database(StationStopInfoDatabase, "https://gtfsprovider.example.com/static.zip")
-```
-
-### Command Line Interface
-
-This can be run as a Python module on the command line using
-
-`python -m gtfs_station_stop`
-
-Use `python -m gtfs_station_stop --help` for details.
-
-## Development Setup
-
-Install all development dependencies with:
-
-```bash
-$ pip install -r requirements-dev.txt
-```
-
-Run tests with:
-
-```bash
-$ pytest
-```
+# GTFS Station Stop
+
+A project for organizing GTFS Real-Time data for use as a homeassistant sensor.
+
+## Usage
+
+This is designed for use with [Home Assistant GTFS Realtime Custom Component](https://github.com/bcpearce/homeassistant-gtfs-realtime).
+
+It can also be used for general GTFS update purposes.
+
+### Feed Subjects and Station Stops
+
+All updates go through the Feed Subject which is setup to call updates from one or more feed URLS.
+
+Create a feed subject like so, then pass it in the constructor for a Station Stop
+
+```python
+from gtfs_station_stop.feed_subject import FeedSubject
+from gtfs_station_stop.station_stop import StationStop
+
+# Obtain the API keep from your GTFS provider if needed, otherwise leave blank.
+api_key = "YOUR_API_KEY_HERE"
+urls = ["https://gtfs.example.com/feed1", "https://gtfs.example.com/feed2"]
+feed_subject = FeedSubject(urls, api_key)
+
+# Obtain the Stop ID from GTFS static data from your provider.
+# This must match those provided by the realtime feed.
+station_stop_nb = StationStop("STOP_ID_NORTHBOUND", feed_subject)
+station_stop_sb = StationStop("STOP_ID_SOUTHBOUND", feed_subject)
+```
+
+Calling `feed_subject.update()` will update all registered listeners.
+
+```python
+feed_subject.update()
+
+for arrival in station_stop_nb.arrivals:
+    minutes_to = (arrival.time - time.time()) / 60.0
+    print(f"{arrival.route} in {minutes_to}")
+```
+
+Active service alerts are also supported for station stops and for routes.
+
+```python
+route_status = RouteStatus("Line 1", feed_subject)
+
+feed_subject.update()
+
+for alert in route_status.alerts:
+    print(f"{route_status.id} alert {alert.header_text['en']}")
+
+for alert in station_stop_nb.alerts:
+    print(f"{station_stop_nb.id} alert {alert.header_text['en']}")
+```
+
+As the update will make one or more http requests, this may improve performance or integrate better with an asynchronous project.
+
+### GTFS Static Info
+
+Static data can be loaded into a database for convenient lookup to use alongside GTFS Realtime data. GTFS data can be read from a file or a URL from your service provider. The GTFS file must be provided as a .zip containing the requisite .txt files as defined by [GTFS Static Reference](https://developers.google.com/transit/gtfs/reference).
+
+```python
+from gtfs_station_stop.station_stop_info import StationStopInfoDatabase
+
+station_stop_info_db = StationStopInfoDatabase("gtfs_static.zip")
+print(f"{station_stop_info_db['STOP_ID']}")
+```
+
+Static info can be queried through the `station_stop_info`, `route_info`, `calendar`, and `trip_info` submodules.
+
+GTFS providers will regularly update their static feeds.  In order to account for this, the library will attempt to cache zip file downloads for static info.
+
+### Async Updates
+
+Asynchronous updates are also supported through the `async_update()` method.
+
+```python
+await feed_subject.async_update()
+```
+
+Static data can also be obtained similarly with `gtfs_station_stop.static_database.async_factory`.
+
+```python
+station_stop_info_database = await async_get_gtfs_database(StationStopInfoDatabase, "https://gtfsprovider.example.com/static.zip")
+```
+
+### Command Line Interface
+
+This can be run as a Python module on the command line using
+
+`python -m gtfs_station_stop`
+
+Use `python -m gtfs_station_stop --help` for details.
+
+## Development Setup
+
+Install all development dependencies with:
+
+```bash
+$ pip install -r requirements-dev.txt
+```
+
+Run tests with:
+
+```bash
+$ pytest
+```
```

### Comparing `gtfs_station_stop-0.7.0b5/pyproject.toml` & `gtfs_station_stop-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "gtfs_station_stop"
-dynamic = ["version"]
-authors = [
-  { name="Benjamin Pearce", email="gtfs@bcpearce.com" },
-]
-description = "Package for reading and organizing GTFS data for a given station stop."
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-  "python-dotenv==1.0.1",
-  "gtfs-realtime-bindings==1.0.0",
-  "requests==2.31.0",
-  "requests-cache==1.2.0",
-  "aiohttp[speedups]==3.9.3",
-  "aiohttp-client-cache[sqlite]==0.11.0",
-]
-[tool.hatch.version]
-path = "src/gtfs_station_stop/__about__.py"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "gtfs_station_stop"
+dynamic = ["version"]
+authors = [
+  { name="Benjamin Pearce", email="gtfs@bcpearce.com" },
+]
+description = "Package for reading and organizing GTFS data for a given station stop."
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+  "python-dotenv>=1.0.1",
+  "gtfs-realtime-bindings>=1.0.0",
+  "requests>=2.31.0",
+  "requests-cache>=1.2.0",
+  "aiohttp[speedups]>=3.9.3",
+  "aiohttp-client-cache[sqlite]>=0.11.0",
+]
+[tool.hatch.version]
+path = "src/gtfs_station_stop/__about__.py"
```

### Comparing `gtfs_station_stop-0.7.0b5/PKG-INFO` & `gtfs_station_stop-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: gtfs_station_stop
-Version: 0.7.0b5
+Version: 0.8.0
 Summary: Package for reading and organizing GTFS data for a given station stop.
 Author-email: Benjamin Pearce <gtfs@bcpearce.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: aiohttp-client-cache[sqlite]==0.11.0
-Requires-Dist: aiohttp[speedups]==3.9.3
-Requires-Dist: gtfs-realtime-bindings==1.0.0
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: requests-cache==1.2.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: aiohttp-client-cache[sqlite]>=0.11.0
+Requires-Dist: aiohttp[speedups]>=3.9.3
+Requires-Dist: gtfs-realtime-bindings>=1.0.0
+Requires-Dist: python-dotenv>=1.0.1
+Requires-Dist: requests-cache>=1.2.0
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # GTFS Station Stop
 
 A project for organizing GTFS Real-Time data for use as a homeassistant sensor.
 
 ## Usage
```

