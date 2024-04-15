# Comparing `tmp/morphology-workflows-0.9.3.tar.gz` & `tmp/morphology-workflows-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphology-workflows-0.9.3.tar", last modified: Thu Feb 15 16:39:01 2024, max compression
+gzip compressed data, was "morphology-workflows-0.9.4.tar", last modified: Tue Mar 12 13:04:58 2024, max compression
```

## Comparing `morphology-workflows-0.9.3.tar` & `morphology-workflows-0.9.4.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.702569 morphology-workflows-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-02-15 16:39:01.702569 morphology-workflows-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.666569 morphology-workflows-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.666569 morphology-workflows-0.9.3/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/fetch_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.666569 morphology-workflows-0.9.3/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   239826 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/logo/BBP-Morphology-Workflows.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/luigi_cfg.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/docs/source/placeholders_config.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.670569 morphology-workflows-0.9.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      679 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/examples/logging.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/examples/luigi.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/examples/neuromorpho_config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      214 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 16:39:01.702569 morphology-workflows-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.654569 morphology-workflows-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.670569 morphology-workflows-0.9.3/src/morphology_workflows/
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.670569 morphology-workflows-0.9.3/src/morphology_workflows/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_data/default_placeholders.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.674569 morphology-workflows-0.9.3/src/morphology_workflows/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/allen_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.674569 morphology-workflows-0.9.3/src/morphology_workflows/_templates/config_templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/config_templates/default.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/config_templates/example_template_curate_dataset.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/logging.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/luigi.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/mouselight_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/neuromorpho_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/placeholder_config_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.674569 morphology-workflows-0.9.3/src/morphology_workflows/_templates/source_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/_templates/source_report/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10323 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    28054 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/marker_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/repair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.674569 morphology-workflows-0.9.3/src/morphology_workflows/tasks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      427 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/tasks/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/src/morphology_workflows/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.698569 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-15 16:39:01.000000 morphology-workflows-0.9.3/src/morphology_workflows.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/allen_config_download.json
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/mouselight_config_download.json
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/neuromorpho_config_download.json
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/placeholders.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.658569 morphology-workflows-0.9.3/tests/data/test_example_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/Annotate/
--rwxr-xr-x   0 runner    (1001) docker     (127)    25443 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/Annotate/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/ApicalPoint/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2765 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CollectCurated/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2645 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CollectCurated/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CutLeaves/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CutLeaves/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/HardLimit/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3554 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/HardLimit/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/MType/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1457 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/MType/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotApicalPoint/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3207 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotCutLeaves/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2804 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotHardLimit/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5108 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     7192 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/annotated_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Align/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Align/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/CheckNeurites/
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/CheckNeurites/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Collect/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Collect/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.678569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Curate/
--rw-r--r--   0 runner    (1001) docker     (127)    37582 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Curate/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/DetectErrors/
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/DetectErrors/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/ExtractMarkers/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Orient/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Orient/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotErrors/
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotErrors/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMarkers/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMarkers/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMorphologies/
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Recenter/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Recenter/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Sanitize/
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Sanitize/report.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/curated_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/CollectAnnotated/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2964 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/FixZeroDiameters/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeCollage/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeCollage/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeRelease/
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeRelease/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/PlotRepair/
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/PlotRepair/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Repair/
--rw-r--r--   0 runner    (1001) docker     (127)    43893 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Repair/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/RepairNeurites/
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Unravel/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Unravel/report.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/repaired_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-asc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.682569 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-h5/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-swc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-asc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-h5/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-swc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-asc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-h5/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-swc/
--rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)    57075 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_report/report_latexpdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)    16643 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_report/report_no_exception_rst2pdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   123901 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_report/report_rst2pdf.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.686569 morphology-workflows-0.9.3/tests/data/test_report_before_run/
--rwxr-xr-x   0 runner    (1001) docker     (127)    42350 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_report_before_run/report_latexpdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)    10085 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/data/test_report_before_run/report_rst2pdf.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.690569 morphology-workflows-0.9.3/tests/examples_test/
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/builder_recipe.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:01.698569 morphology-workflows-0.9.3/tests/examples_test/morphologies/
--rw-r--r--   0 runner    (1001) docker     (127)  1255757 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/C060114A5.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)   395836 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/C270106A.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/README
--rwxr-xr-x   0 runner    (1001) docker     (127)   589072 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/astrocyte.h5
--rwxr-xr-x   0 runner    (1001) docker     (127)    10180 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/circle_contour.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/complexe.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/disconnected_neurite.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/iterators.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/mono-type.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/multiple_point_section.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/multiple_soma.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/nested_single_children.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/neurite_wrong_root_point.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)   107856 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/nrn-order-already-sorted.h5
--rwxr-xr-x   0 runner    (1001) docker     (127)   165400 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/nrn_ordering.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/pia.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/reversed_NRN_neurite_order.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)   491711 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/rp100427-123_idC.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/sections-block.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      409 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/simple-with-font.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/simple-with-image-coord.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/simple.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/simple.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/simple2.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/soma_cylinders.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/soma_multiple_frustums.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/soma_single_frustum.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/soma_three_points_cylinder.swc
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/spine.asc
--rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/morphologies/three_point_soma.swc
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/mouse_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/placement_rules.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)    57762 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/report_CurateDataset.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   130944 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/report_example.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/run_curation.sh
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/examples_test/transform_rules.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/test_download_morphs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/test_example_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-15 16:38:53.000000 morphology-workflows-0.9.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.843337 morphology-workflows-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-03-12 13:04:58.839337 morphology-workflows-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.811337 morphology-workflows-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.811337 morphology-workflows-0.9.4/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/fetch_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.811337 morphology-workflows-0.9.4/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   239826 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/logo/BBP-Morphology-Workflows.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/luigi_cfg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/docs/source/placeholders_config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.815337 morphology-workflows-0.9.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      679 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/examples/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/examples/luigi.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/examples/neuromorpho_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      214 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 13:04:58.843337 morphology-workflows-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.799337 morphology-workflows-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.815337 morphology-workflows-0.9.4/src/morphology_workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.815337 morphology-workflows-0.9.4/src/morphology_workflows/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_data/default_placeholders.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.815337 morphology-workflows-0.9.4/src/morphology_workflows/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/allen_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/src/morphology_workflows/_templates/config_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/config_templates/default.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/config_templates/example_template_curate_dataset.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/luigi.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/mouselight_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/neuromorpho_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/placeholder_config_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/src/morphology_workflows/_templates/source_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/_templates/source_report/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10323 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28524 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/marker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/repair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/src/morphology_workflows/tasks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      427 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13802 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/tasks/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/src/morphology_workflows/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.839337 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-12 13:04:58.000000 morphology-workflows-0.9.4/src/morphology_workflows.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/allen_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/mouselight_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/neuromorpho_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/placeholders.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.807337 morphology-workflows-0.9.4/tests/data/test_example_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/Annotate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25443 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/Annotate/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.819337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/ApicalPoint/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2765 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CollectCurated/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2645 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CollectCurated/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CutLeaves/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3302 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CutLeaves/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/HardLimit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3554 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/HardLimit/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/MType/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1457 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/MType/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotApicalPoint/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3207 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotCutLeaves/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2804 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotHardLimit/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5108 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7192 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/annotated_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Align/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Align/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/CheckNeurites/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/CheckNeurites/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Collect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Collect/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Curate/
+-rw-r--r--   0 runner    (1001) docker     (127)    37582 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Curate/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/DetectErrors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/DetectErrors/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/ExtractMarkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Orient/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Orient/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotErrors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotErrors/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMarkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMarkers/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMorphologies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Recenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Recenter/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Sanitize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Sanitize/report.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/curated_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/CollectAnnotated/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2964 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/FixZeroDiameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.823337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeCollage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeCollage/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeRelease/
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeRelease/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/PlotRepair/
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/PlotRepair/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Repair/
+-rw-r--r--   0 runner    (1001) docker     (127)    43893 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Repair/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/RepairNeurites/
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Unravel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Unravel/report.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/repaired_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57075 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_report/report_latexpdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16643 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_report/report_no_exception_rst2pdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   123901 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_report/report_rst2pdf.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.827337 morphology-workflows-0.9.4/tests/data/test_report_before_run/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42350 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_report_before_run/report_latexpdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10085 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/data/test_report_before_run/report_rst2pdf.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.831337 morphology-workflows-0.9.4/tests/examples_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/builder_recipe.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:04:58.839337 morphology-workflows-0.9.4/tests/examples_test/morphologies/
+-rw-r--r--   0 runner    (1001) docker     (127)  1255757 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/C060114A5.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)   395836 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/C270106A.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/README
+-rwxr-xr-x   0 runner    (1001) docker     (127)   589072 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/astrocyte.h5
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10180 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/circle_contour.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/complexe.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/disconnected_neurite.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/iterators.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/mono-type.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/multiple_point_section.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/multiple_soma.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/nested_single_children.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/neurite_wrong_root_point.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)   107856 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/nrn-order-already-sorted.h5
+-rwxr-xr-x   0 runner    (1001) docker     (127)   165400 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/nrn_ordering.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/pia.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/reversed_NRN_neurite_order.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)   491711 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/rp100427-123_idC.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/sections-block.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      409 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/simple-with-font.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      574 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/simple-with-image-coord.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      591 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/simple.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/simple.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/simple2.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/soma_cylinders.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/soma_multiple_frustums.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      128 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/soma_single_frustum.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/soma_three_points_cylinder.swc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/spine.asc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/morphologies/three_point_soma.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/mouse_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/placement_rules.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57762 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/report_CurateDataset.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   130944 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/report_example.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/run_curation.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/examples_test/transform_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26137 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/test_download_morphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/test_example_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12569 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-12 13:04:51.000000 morphology-workflows-0.9.4/tox.ini
```

### Comparing `morphology-workflows-0.9.3/.auto-changelog` & `morphology-workflows-0.9.4/.auto-changelog`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/.auto-changelog-template.hbs` & `morphology-workflows-0.9.4/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/.copier-answers.yml` & `morphology-workflows-0.9.4/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/.gitignore` & `morphology-workflows-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/.pre-commit-config.yaml` & `morphology-workflows-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/.pylintrc` & `morphology-workflows-0.9.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/CHANGELOG.md` & `morphology-workflows-0.9.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [0.9.4](https://github.com/BlueBrain/morphology-workflows/compare/0.9.3..0.9.4)
+
+> 12 March 2024
+
+### New Features
+
+- Add sign flip in Orient (Alexis Arnaudon - [#144](https://github.com/BlueBrain/morphology-workflows/pull/144))
+
+### Fixes
+
+- The add_soma() function should work with no root point (Adrien Berchet - [#145](https://github.com/BlueBrain/morphology-workflows/pull/145))
+
 ## [0.9.3](https://github.com/BlueBrain/morphology-workflows/compare/0.9.2..0.9.3)
 
 > 15 February 2024
 
 ### Fixes
 
 - Use absolute paths in the dataset created by the Initialize workflow (Adrien Berchet - [#142](https://github.com/BlueBrain/morphology-workflows/pull/142))
```

### Comparing `morphology-workflows-0.9.3/CONTRIBUTING.md` & `morphology-workflows-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/LICENSE.txt` & `morphology-workflows-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/PKG-INFO` & `morphology-workflows-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphology-workflows
-Version: 0.9.3
+Version: 0.9.4
 Summary: Workflows used for morphology processing.
 Home-page: https://morphology-workflows.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/morphology-workflows/issues
 Project-URL: Source, https://github.com/BlueBrain/morphology-workflows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morphology-workflows-0.9.3/README.md` & `morphology-workflows-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/commitlint.config.js` & `morphology-workflows-0.9.4/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/docs/Makefile` & `morphology-workflows-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/docs/source/conf.py` & `morphology-workflows-0.9.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/docs/source/fetch_config.rst` & `morphology-workflows-0.9.4/docs/source/fetch_config.rst`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/docs/source/logo/BBP-Morphology-Workflows.jpg` & `morphology-workflows-0.9.4/docs/source/logo/BBP-Morphology-Workflows.jpg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/docs/source/placeholders_config.rst` & `morphology-workflows-0.9.4/docs/source/placeholders_config.rst`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/examples/logging.conf` & `morphology-workflows-0.9.4/examples/logging.conf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/examples/luigi.cfg` & `morphology-workflows-0.9.4/examples/luigi.cfg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/package.json` & `morphology-workflows-0.9.4/package.json`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/pyproject.toml` & `morphology-workflows-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/setup.py` & `morphology-workflows-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/_data/default_placeholders.csv` & `morphology-workflows-0.9.4/src/morphology_workflows/_data/default_placeholders.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/_templates/logging.conf` & `morphology-workflows-0.9.4/src/morphology_workflows/_templates/logging.conf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/_templates/luigi.cfg` & `morphology-workflows-0.9.4/src/morphology_workflows/_templates/luigi.cfg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/_templates/placeholder_config_schema.json` & `morphology-workflows-0.9.4/src/morphology_workflows/_templates/placeholder_config_schema.json`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/_templates/source_report/conf.py` & `morphology-workflows-0.9.4/src/morphology_workflows/_templates/source_report/conf.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/annotation.py` & `morphology-workflows-0.9.4/src/morphology_workflows/annotation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/curation.py` & `morphology-workflows-0.9.4/src/morphology_workflows/curation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Curation functions."""
+
 import json
 import logging
 import shutil
 from functools import partial
 from pathlib import Path
 
 import matplotlib as mpl
@@ -190,19 +191,21 @@
     except CorruptedMorphology as exc:
         return ValidationResult(is_valid=False, comment=exc, morph_path=None)
     return ValidationResult(is_valid=True, morph_path=new_morph_path)
 
 
 def _center_root_points(morph):
     root_points = np.array([section.points[0, COLS.XYZ] for section in morph.root_sections])
-    center = np.mean(root_points, axis=0)
     if len(root_points) > 0:
+        center = np.mean(root_points, axis=0)
         dists = np.linalg.norm(root_points - center, axis=1)
         radius = max(1.0, dists.mean())
     else:
+        root_points = np.zeros((1, 3), dtype=float)
+        center = np.zeros(3, dtype=float)
         radius = 1.0
     return center, radius, root_points
 
 
 def _create_intermediate_angles_xy(points, missing_pts):
     relative_pts_xy = points.copy()
     relative_pts_xy[:, 2] = 0
@@ -542,19 +545,30 @@
         is_valid=True, morph_path=new_morph_path, soma_location=json.dumps(location.tolist())
     )
 
 
 def orient(row, data_dir, pia_direction="y"):
     """Orient a morphology such that the original pia_direcion is along y."""
     new_morph_path = data_dir / Path(row.morph_path).name
-    _convert = {"x": [1.0, 0, 0], "z": [0.0, 0.0, 1.0]}
+    _convert = {"x": [1.0, 0, 0], "y": [0.0, 1.0, 0.0], "z": [0.0, 0.0, 1.0]}
+    _convert_id = {"x": 0, "y": 1, "z": 2}
     morph = Morphology(row.morph_path)
-    if pia_direction != "y":
-        rotation_matrix = rotation_matrix_from_vectors(_convert[pia_direction], [0.0, 1.0, 0.0])
-        rotate(morph, rotation_matrix)
+
+    flip = False
+    if "-" in pia_direction[0]:
+        flip = True
+        pia_direction = pia_direction[1]
+    elif len(pia_direction) > 1:
+        msg = f"Invalid 'pia_direction' argument: '{pia_direction}'"
+        raise ValueError(msg)
+
+    rotation_matrix = rotation_matrix_from_vectors(_convert[pia_direction], [0.0, 1.0, 0.0])
+    if flip:
+        rotation_matrix[_convert_id[pia_direction], _convert_id[pia_direction]] *= -1
+    rotate(morph, rotation_matrix)
     morph.write(new_morph_path)
     return ValidationResult(is_valid=True, morph_path=new_morph_path)
 
 
 def align(
     row,
     data_dir,
```

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/marker_helper.py` & `morphology-workflows-0.9.4/src/morphology_workflows/marker_helper.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/placeholders.py` & `morphology-workflows-0.9.4/src/morphology_workflows/placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/repair.py` & `morphology-workflows-0.9.4/src/morphology_workflows/repair.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/annotation.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/annotation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/cli.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/curation.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/curation.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
 
     Sometimes, morphologies are oriented along non-standard axis. At BBP, the standard axis is
         - ``y`` for pia direction (apical trunk, minus main axon, etc...)
         - ``z`` is the slice direction is invitro
         - ``x`` the other direction
 
     If ``y`` is provided (default value), no oriention will be applied.
+    One can also use minus sign, as ``-y`` to flip y axis.
     """
 
     output_columns = {"morph_path": None}
     validation_function = orient
 
     pia_direction = luigi.Parameter(
         default="y", description=":str: Axis of pia direction, x, y or z"
```

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/fetch.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/fetch.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/placeholders.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/repair.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/repair.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/tasks/workflows.py` & `morphology-workflows-0.9.4/src/morphology_workflows/tasks/workflows.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows/utils.py` & `morphology-workflows-0.9.4/src/morphology_workflows/utils.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows.egg-info/PKG-INFO` & `morphology-workflows-0.9.4/src/morphology_workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphology-workflows
-Version: 0.9.3
+Version: 0.9.4
 Summary: Workflows used for morphology processing.
 Home-page: https://morphology-workflows.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/morphology-workflows/issues
 Project-URL: Source, https://github.com/BlueBrain/morphology-workflows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows.egg-info/SOURCES.txt` & `morphology-workflows-0.9.4/src/morphology_workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/src/morphology_workflows.egg-info/requires.txt` & `morphology-workflows-0.9.4/src/morphology_workflows.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/__init__.py` & `morphology-workflows-0.9.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/conftest.py` & `morphology-workflows-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/placeholders.csv` & `morphology-workflows-0.9.4/tests/data/placeholders.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/Annotate/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/Annotate/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CollectCurated/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CollectCurated/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/CutLeaves/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/CutLeaves/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/HardLimit/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/HardLimit/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/MType/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/MType/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_annotated/annotated_dataset.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_annotated/annotated_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Align/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Align/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/CheckNeurites/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/CheckNeurites/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Collect/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Collect/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Curate/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Curate/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/DetectErrors/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/DetectErrors/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Orient/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Orient/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotErrors/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotErrors/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMarkers/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMarkers/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Recenter/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Recenter/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/Sanitize/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/Sanitize/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_curated/curated_dataset.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_curated/curated_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeCollage/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeCollage/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/MakeRelease/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/MakeRelease/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/PlotRepair/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/PlotRepair/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Repair/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Repair/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/Unravel/report.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/Unravel/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/out_repaired/repaired_dataset.csv` & `morphology-workflows-0.9.4/tests/data/test_example_1/out_repaired/repaired_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-asc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-h5/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/repair_release-swc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/repair_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-asc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-h5/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/unravel_release-swc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/unravel_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml` & `morphology-workflows-0.9.4/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_report/report_latexpdf.pdf` & `morphology-workflows-0.9.4/tests/data/test_report/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_report/report_no_exception_rst2pdf.pdf` & `morphology-workflows-0.9.4/tests/data/test_report/report_no_exception_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_report/report_rst2pdf.pdf` & `morphology-workflows-0.9.4/tests/data/test_report/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_report_before_run/report_latexpdf.pdf` & `morphology-workflows-0.9.4/tests/data/test_report_before_run/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/data/test_report_before_run/report_rst2pdf.pdf` & `morphology-workflows-0.9.4/tests/data/test_report_before_run/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/builder_recipe.xml` & `morphology-workflows-0.9.4/tests/examples_test/builder_recipe.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/dataset.csv` & `morphology-workflows-0.9.4/tests/examples_test/dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/C060114A5.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/C060114A5.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/C270106A.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/C270106A.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/README` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/README`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/astrocyte.h5` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/astrocyte.h5`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/circle_contour.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/circle_contour.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/complexe.swc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/complexe.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/nrn-order-already-sorted.h5` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/nrn-order-already-sorted.h5`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/nrn_ordering.swc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/nrn_ordering.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/pia.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/pia.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/rp100427-123_idC.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/rp100427-123_idC.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/sections-block.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/sections-block.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/simple-with-image-coord.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/simple-with-image-coord.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/simple.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/simple.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/simple.swc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/simple.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/spine.asc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/spine.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/morphologies/three_point_soma.swc` & `morphology-workflows-0.9.4/tests/examples_test/morphologies/three_point_soma.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/placement_rules.xml` & `morphology-workflows-0.9.4/tests/examples_test/placement_rules.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/report_CurateDataset.pdf` & `morphology-workflows-0.9.4/tests/examples_test/report_CurateDataset.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/report_example.pdf` & `morphology-workflows-0.9.4/tests/examples_test/report_example.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/examples_test/transform_rules.xml` & `morphology-workflows-0.9.4/tests/examples_test/transform_rules.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/test_cli.py` & `morphology-workflows-0.9.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/test_curation.py` & `morphology-workflows-0.9.4/tests/test_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,15 +598,16 @@
                 [0.20710672, -0.20710684, 0],
                 [0, 1, 0],
                 [-1.2071068, 1.2071067, 0],
             ],
         )
 
     @pytest.mark.parametrize("nb_root_points", list(range(6)))
-    def test__add_soma_contour(self, nb_root_points):
+    @pytest.mark.parametrize("soma_type", ["contour", "spherical"])
+    def test__add_soma(self, nb_root_points, soma_type):
         """Test _add_soma for contour type with multiple numbers of root sections."""
         # pylint: disable=protected-access
         morph = Morphology()
         morph.soma.type = SomaType.SOMA_UNDEFINED
         morph.soma.points = np.array([], dtype=morph.soma.points.dtype).reshape((0, 3))
         morph.soma.diameters = np.array([], dtype=morph.soma.diameters.dtype)
 
@@ -615,21 +616,26 @@
             angle = i * interval
             x = np.cos(angle)
             y = np.sin(angle)
             z = 0
             stub = PointLevel([np.array([x, y, z]), 2 * np.array([x, y, z])], [1, 1])
             morph.append_root_section(stub, SectionType.axon)
 
-        if nb_root_points < 2:
-            with pytest.raises(ValueError, match="At least 2 root points are needed"):
+        if soma_type == "contour":
+            if nb_root_points < 2:
+                with pytest.raises(ValueError, match="At least 2 root points are needed"):
+                    curation._add_soma(morph, soma_type="contour")  # noqa: SLF001
+            else:
                 curation._add_soma(morph, soma_type="contour")  # noqa: SLF001
+
+                assert len(morph.soma.points) == max(4, nb_root_points)
         else:
-            curation._add_soma(morph, soma_type="contour")  # noqa: SLF001
+            curation._add_soma(morph, soma_type="spherical")  # noqa: SLF001
 
-            assert len(morph.soma.points) == max(4, nb_root_points)
+            assert len(morph.soma.points) == 1
 
     def test_no_mock_but_stub(self, simple_morph, res_path):
         """Check neurites with no mock soma but with stub axon."""
         row = pd.Series({"morph_path": simple_morph}, name="test_name")
         res = curation.check_neurites(
             row,
             res_path,
```

### Comparing `morphology-workflows-0.9.3/tests/test_download_morphs.py` & `morphology-workflows-0.9.4/tests/test_download_morphs.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/test_example_1.py` & `morphology-workflows-0.9.4/tests/test_example_1.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tests/test_placeholders.py` & `morphology-workflows-0.9.4/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.9.3/tox.ini` & `morphology-workflows-0.9.4/tox.ini`

 * *Files identical despite different names*

