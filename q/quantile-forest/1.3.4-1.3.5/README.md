# Comparing `tmp/quantile-forest-1.3.4.tar.gz` & `tmp/quantile_forest-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantile-forest-1.3.4.tar", last modified: Thu Feb 22 05:49:49 2024, max compression
+gzip compressed data, was "quantile_forest-1.3.5.tar", last modified: Mon Apr 15 14:27:24 2024, max compression
```

## Comparing `quantile-forest-1.3.4.tar` & `quantile_forest-1.3.5.tar`

### file list

```diff
@@ -1,64 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/css/gallery.css
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/css/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (127)    34494 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/js/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/quantile-forest-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_static/quantile-forest-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_templates/navbar-project.html
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/_templates/sidebar-logo.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     6865 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2087 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/make.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/references.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      268 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/sphinx_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.866102 quantile-forest-1.3.4/docs/sphinxext/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/sphinxext/gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/sphinxext/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14739 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      776 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9428 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_conformalized.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5054 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6415 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_extrapolation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4069 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_interpolation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6850 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_intervals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_multioutput.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3291 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_vs_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/examples/plot_quantile_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/quantile_forest/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/_min_dependencies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58939 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/_quantile_forest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1173 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/_quantile_forest_fast.pxd
--rwxr-xr-x   0 runner    (1001) docker     (127)    39096 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/_quantile_forest_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/quantile_forest/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51498 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/tests/test_quantile_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/quantile_forest/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/quantile_forest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 05:49:49.000000 quantile-forest-1.3.4/quantile_forest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-22 05:49:49.870102 quantile-forest-1.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3917 2024-02-22 05:49:31.000000 quantile-forest-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3382 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.976945 quantile_forest-1.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.976945 quantile_forest-1.3.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/css/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/css/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34494 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/js/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/quantile-forest-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_static/quantile-forest-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_templates/navbar-project.html
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/_templates/sidebar-logo.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6921 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/getting_started/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      894 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/getting_started/developers.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      412 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/getting_started/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2163 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/make.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/references.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      268 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/refs.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/releases/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3401 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/releases/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/sphinx_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/sphinxext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/sphinxext/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/sphinxext/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/sphinxext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/docs/user_guide/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8987 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/user_guide/fit_predict.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3456 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/user_guide/introduction.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1520 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/user_guide/proximities.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1202 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/docs/user_guide/quantile_ranks.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.980945 quantile_forest-1.3.5/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      776 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4123 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_predict_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9428 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_conformalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5054 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20218 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_extrapolation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4069 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_interpolation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6850 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_intervals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_multioutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3291 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/examples/plot_quantile_vs_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/quantile_forest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/_min_dependencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63292 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/_quantile_forest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1173 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/_quantile_forest_fast.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39186 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/_quantile_forest_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/quantile_forest/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52823 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/tests/test_quantile_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/quantile_forest/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/quantile_forest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 14:27:24.000000 quantile_forest-1.3.5/quantile_forest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 14:27:24.984945 quantile_forest-1.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3917 2024-04-15 14:27:16.000000 quantile_forest-1.3.5/setup.py
```

### Comparing `quantile-forest-1.3.4/LICENSE` & `quantile_forest-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/PKG-INFO` & `quantile_forest-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.3.4
+Version: 1.3.5
 Summary: scikit-learn compatible quantile forests.
 Home-page: https://zillow.github.io/quantile-forest
 Download-URL: https://pypi.org/project/quantile-forest/#files
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Project-URL: Documentation, https://zillow.github.io/quantile-forest
 Project-URL: Source, https://github.com/zillow/quantile-forest
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantile-forest Version: 1.3.4 Summary: scikit-
+Metadata-Version: 2.1 Name: quantile-forest Version: 1.3.5 Summary: scikit-
 learn compatible quantile forests. Home-page: https://zillow.github.io/
 quantile-forest Download-URL: https://pypi.org/project/quantile-forest/#files
 Maintainer: Zillow Group AI Team License: Apache License 2.0 Project-URL:
 Documentation, https://zillow.github.io/quantile-forest Project-URL: Source,
 https://github.com/zillow/quantile-forest Project-URL: Tracker, https://
 github.com/zillow/quantile-forest/issues Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `quantile-forest-1.3.4/README.md` & `quantile_forest-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/Makefile` & `quantile_forest-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/css/gallery.css` & `quantile_forest-1.3.5/docs/_static/css/gallery.css`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/css/theme_overrides.css` & `quantile_forest-1.3.5/docs/_static/css/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/favicon.ico` & `quantile_forest-1.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/js/copybutton.js` & `quantile_forest-1.3.5/docs/_static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/quantile-forest-logo-white.png` & `quantile_forest-1.3.5/docs/_static/quantile-forest-logo-white.png`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/_static/quantile-forest-logo.png` & `quantile_forest-1.3.5/docs/_static/quantile-forest-logo.png`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/conf.py` & `quantile_forest-1.3.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "sphinx.ext.doctest",
     "sphinx.ext.githubpages",
     "sphinx.ext.intersphinx",
     "numpydoc",
     "sphinx_design",
     "sphinxcontrib.bibtex",
     "sphinxext_altair.altairplot",
+    "sphinxext.directives",
     "sphinxext.gallery",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
@@ -152,14 +153,15 @@
 html_css_files = [
     "css/gallery.css",
 ]
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
     "index": [],
+    "releases/changes": [],
     "**": ["sidebar-nav-bs"],
 }
 
 # -- Options for autodoc ------------------------------------------------------
 
 autodoc_default_options = {
     "members": True,
```

### Comparing `quantile-forest-1.3.4/docs/index.rst` & `quantile_forest-1.3.5/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       :link: install
       :link-type: ref
       :link-alt: Getting started
 
       A guide that provides installation requirements and instructions, as well as procedures for developers.
 
    .. grid-item-card:: User Guide
-      :link: user_guide
+      :link: user-guide-intro
       :link-type: ref
       :link-alt: User guide
 
       Information on the key concepts behind quantile forests and how they apply to this package.
 
    .. grid-item-card:: Examples
       :link: example-gallery
@@ -46,13 +46,14 @@
 
       Information on all of the package methods and classes, for when you want just the details.
 
 .. toctree::
    :maxdepth: 1
    :hidden:
 
-   Getting Started <install>
-   User Guide <user_guide>
+   Getting Started <getting_started/installation>
+   User Guide <user_guide/introduction>
    Examples <gallery/index>
    API <api>
+   Release Notes <releases/changes>
 
 .. _GitHub: http://github.com/zillow/quantile-forest
```

### Comparing `quantile-forest-1.3.4/docs/install.rst` & `quantile_forest-1.3.5/docs/getting_started/developers.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,46 @@
-.. _install:
+.. _developers:
 
-Getting Started
-===============
-
-Prerequisites
--------------
-
-The quantile-forest package requires the following dependencies:
-
-* python (>=3.8)
-* numpy (>=1.23)
-* scikit-learn (>=1.0)
-* scipy (>=1.4)
-
-Install
--------
-
-quantile-forest can be installed using `pip`::
-
-  pip install quantile-forest
-
-Developer Install
+Developer's Guide
 -----------------
 
+Development Installation
+~~~~~~~~~~~~~~~~~~~~~~~~
+
 Building the package from source additionally requires the following dependencies:
 
 * cython (>=3.0a4)
 
 To manually build and install the package, run::
 
   pip install --verbose --editable .
 
 Troubleshooting
----------------
+~~~~~~~~~~~~~~~
 
 If the build fails because SciPy is not installed, ensure OpenBLAS and LAPACK are available and accessible.
 
 On macOS, run::
 
   brew install openblas
   brew install lapack
   export SYSTEM_VERSION_COMPAT=1
 
 Test and Coverage
------------------
+~~~~~~~~~~~~~~~~~
 
 To test the code::
 
   $ python -m pytest quantile_forest -v
 
 To test the documentation::
 
-  $ python -m pytest docs/*rst
+  $ python -m pytest docs/user_guide/*rst
 
 Documentation
--------------
+~~~~~~~~~~~~~
 
 To build the documentation, run::
 
   $ pip install -r ./docs/sphinx_requirements.txt
   $ mkdir -p ./docs/_images
   $ sphinx-build -b html ./docs ./docs/_build
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Install
-   :hidden:
-
-   Getting Started <self>
```

### Comparing `quantile-forest-1.3.4/docs/make.bat` & `quantile_forest-1.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/sphinxext/gallery.py` & `quantile_forest-1.3.5/docs/sphinxext/gallery.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/docs/sphinxext/utils.py` & `quantile_forest-1.3.5/docs/sphinxext/utils.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/__init__.py` & `quantile_forest-1.3.5/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_conformalized.py` & `quantile_forest-1.3.5/examples/plot_quantile_conformalized.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_example.py` & `quantile_forest-1.3.5/examples/plot_quantile_example.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_interpolation.py` & `quantile_forest-1.3.5/examples/plot_quantile_interpolation.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_intervals.py` & `quantile_forest-1.3.5/examples/plot_quantile_intervals.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_multioutput.py` & `quantile_forest-1.3.5/examples/plot_quantile_multioutput.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/examples/plot_quantile_vs_standard.py` & `quantile_forest-1.3.5/examples/plot_quantile_vs_standard.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/pyproject.toml` & `quantile_forest-1.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "Cython>=3.0a4",
     "numpy>=1.23",
     "scipy>=1.4",
     "scikit-learn>=1.0",
 ]
 
 [tool.black]
-line-length = 100
+line-length = 99
 target_version = ['py38', 'py39', 'py310', 'py311', 'py312']
 preview = true
 exclude = '''
 /(
     \.eggs         # exclude a few common directories in the
   | \.git          # root of the project
   | \.mypy_cache
@@ -22,7 +22,18 @@
   | build
   | dist
   | doc/tutorial
   | doc/_build
   | doc/auto_examples
 )/
 '''
+
+[tool.cython-lint]
+max-line-length = 99
+ignore = ['E741']
+
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+line_length = 99
```

### Comparing `quantile-forest-1.3.4/quantile_forest/__init__.py` & `quantile_forest-1.3.5/quantile_forest/__init__.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/quantile_forest/_min_dependencies.py` & `quantile_forest-1.3.5/quantile_forest/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/quantile_forest/_quantile_forest.py` & `quantile_forest-1.3.5/quantile_forest/_quantile_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 from sklearn.utils.validation import check_is_fitted
 
 from ._quantile_forest_fast import QuantileForest, generate_unsampled_indices
 
 sklearn_version = parse_version(sklearn.__version__)
 
 
-def _generate_unsampled_indices(sample_indices, duplicates=None):
+def _generate_unsampled_indices(sample_indices, n_total_samples, duplicates=None):
     """Private function used by forest._get_y_train_leaves function."""
     if duplicates is None:
         duplicates = []
-    return generate_unsampled_indices(sample_indices, duplicates)
+    return generate_unsampled_indices(sample_indices, n_total_samples, duplicates)
 
 
 def _group_by_value(a):
     """Private function used by forest._get_y_train_leaves function."""
     sort_idx = np.argsort(a)
     a_sorted = a[sort_idx]
     unq_first = np.concatenate(([True], a_sorted[1:] != a_sorted[:-1]))
@@ -258,28 +258,31 @@
                 f"got {type(self.max_samples_leaf)}."
             )
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
             X_leaves = self.apply(X)
 
-        shape = (n_samples, self.n_estimators)
+        if self.bootstrap:
+            n_samples_bootstrap = _get_n_samples_bootstrap(n_samples, self.max_samples)
+
+        shape = (n_samples if not self.bootstrap else n_samples_bootstrap, self.n_estimators)
         bootstrap_indices = np.empty(shape, dtype=np.int64)
+        X_leaves_bootstrap = np.empty(shape, dtype=np.int64)
         for i, estimator in enumerate(self.estimators_):
             # Get bootstrap indices.
             if self.bootstrap:
-                n_samples_bootstrap = _get_n_samples_bootstrap(n_samples, self.max_samples)
                 bootstrap_indices[:, i] = _generate_sample_indices(
                     estimator.random_state, n_samples, n_samples_bootstrap
                 )
             else:
                 bootstrap_indices[:, i] = np.arange(n_samples)
 
             # Get predictions on bootstrap indices.
-            X_leaves[:, i] = X_leaves[bootstrap_indices[:, i], i]
+            X_leaves_bootstrap[:, i] = X_leaves[bootstrap_indices[:, i], i]
 
         if sorter is not None:
             # Reassign bootstrap indices to account for target sorting.
             bootstrap_indices = np.argsort(sorter, axis=0)[bootstrap_indices]
             if bootstrap_indices.shape[-1] == 1:
                 bootstrap_indices = np.squeeze(bootstrap_indices, -1)
 
@@ -290,25 +293,25 @@
         max_node_count = 0
         max_samples_leaf = 0 if not leaf_subsample else max_samples_leaf
         for i, estimator in enumerate(self.estimators_):
             node_count = estimator.tree_.node_count
             if node_count > max_node_count:
                 max_node_count = node_count
             if not leaf_subsample:
-                sample_count = np.max(np.bincount(X_leaves[:, i]))
+                sample_count = np.max(np.bincount(X_leaves_bootstrap[:, i]))
                 if sample_count > max_samples_leaf:
                     max_samples_leaf = sample_count
 
         # Initialize NumPy array (more efficient serialization than dict/list).
         shape = (self.n_estimators, max_node_count, y_dim, max_samples_leaf)
         y_train_leaves = np.zeros(shape, dtype=np.int64)
 
         for i, estimator in enumerate(self.estimators_):
             # Group training indices by leaf node.
-            leaf_indices, leaf_values_list = _group_by_value(X_leaves[:, i])
+            leaf_indices, leaf_values_list = _group_by_value(X_leaves_bootstrap[:, i])
 
             if leaf_subsample:
                 random.seed(estimator.random_state)
 
             # Map each leaf node to its list of training indices.
             for leaf_idx, leaf_values in zip(leaf_indices, leaf_values_list):
                 y_indices = bootstrap_indices[:, i][leaf_values]
@@ -435,15 +438,17 @@
             warn("Unsampled indices only exist if bootstrap=True.")
             return np.array([])
         n_train_samples = self.n_train_samples_
         n_samples_bootstrap = _get_n_samples_bootstrap(n_train_samples, self.max_samples)
         sample_indices = _generate_sample_indices(
             estimator.random_state, n_train_samples, n_samples_bootstrap
         )
-        unsampled_indices = _generate_unsampled_indices(sample_indices, duplicates=duplicates)
+        unsampled_indices = _generate_unsampled_indices(
+            sample_indices, n_train_samples, duplicates=duplicates
+        )
         return np.asarray(unsampled_indices)
 
     def predict(
         self,
         X,
         quantiles=None,
         interpolation="linear",
@@ -612,15 +617,15 @@
         oob_score=False,
         indices=None,
         duplicates=None,
     ):
         """Return quantile ranks for X with scores y.
 
         A quantile rank of, for example, 0.8 means that 80% of the scores in
-        `inputs` are below the given score.
+        the frequency distribution of the inputs are below the given score.
 
         In the case of gaps or ties, the exact definition depends on the
         optional keyword `kind`.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
@@ -856,29 +861,31 @@
 
 class RandomForestQuantileRegressor(BaseForestQuantileRegressor):
     """A random forest regressor that provides quantile estimates.
 
     A quantile random forest is a meta estimator that fits a number of
     decision trees on various sub-samples of the dataset, keeps the values of
     samples that reach each node, and assesses the conditional distribution
-    based on this information. The sub-sample size is controlled with the
+    based on this information [1]. The sub-sample size is controlled with the
     `max_samples` parameter if `bootstrap=True` (default), otherwise the whole
     dataset is used to build each tree. The leaf-sample size is controlled
     with the `max_samples_leaf` parameter.
 
     Parameters
     ----------
     n_estimators : int, default=100
         The number of trees in the forest.
 
     default_quantiles : float, list, or "mean", default=0.5
         The default quantile or list of quantiles that the model tries to
         predict. Each quantile must be strictly between 0 and 1. If "mean",
         the model predicts the mean.
 
+        .. versionadded:: 1.2
+
     criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
             default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
         variance reduction as feature selection criterion and minimizes the L2
         loss using the mean of each terminal node, "friedman_mse", which uses
         mean squared error with Friedman's improvement score for potential
@@ -928,25 +935,27 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `round(max_features * n_features)` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
+          `max(1, int(max_features * n_features_in_))` features are considered
+          at each split.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
             The default of 1.0 is equivalent to bagged trees and more
             randomness can be achieved by setting smaller values, e.g. 0.3.
 
+        .. sklearn-versionchanged:: 1.1
+            The default of `max_features` changed from `"auto"` to 1.0.
+
         Note: the search for a split does not stop until at least one
         valid partition of the node samples is found, even if it requires to
         effectively inspect more than ``max_features`` features.
 
     max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
@@ -1008,20 +1017,37 @@
         to train each base estimator.
 
         - If None (default), then draw `X.shape[0]` samples.
         - If int, then draw `max_samples` samples.
         - If float, then draw `max(round(n_samples * max_samples), 1)` samples.
           Thus, `max_samples` should be in the interval `(0.0, 1.0]`.
 
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        .. sklearn-versionadded:: 1.4
+
     Attributes
     ----------
-    estimator_ : DecisionTreeRegressor
+    estimator_ : :class:`~sklearn.tree.DecisionTreeRegressor`
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
+        .. sklearn-versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
@@ -1045,25 +1071,55 @@
         Score of the training dataset obtained using an out-of-bag estimate.
         This attribute exists only when ``oob_score`` is True.
 
     oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
         This attribute exists only when ``oob_score`` is True.
 
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
+
+        .. sklearn-versionadded:: 1.4
+
     See Also
     --------
     ExtraTreesQuantileRegressor : Quantile ensemble of extremely randomized
         tree regressors.
 
+    Notes
+    -----
+    The default values for the parameters controlling the size of the trees
+    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
+    unpruned trees which can potentially be very large on some data sets. To
+    reduce memory consumption, the complexity and size of the trees should be
+    controlled by setting those parameter values.
+
+    The features are always randomly permuted at each split. Therefore,
+    the best found split may vary, even with the same training data,
+    ``max_features=n_features`` and ``bootstrap=False``, if the improvement
+    of the criterion is identical for several splits enumerated during the
+    search of the best split. To obtain a deterministic behaviour during
+    fitting, ``random_state`` has to be fixed.
+
+    The default value ``max_features=1.0`` uses ``n_features``
+    rather than ``n_features / 3``. The latter was originally suggested in
+    [2], whereas the former was more recently justified empirically in [3].
+
     References
     ----------
     .. [1] N. Meinshausen, "Quantile Regression Forests", Journal of Machine
            Learning Research, 7(Jun), 983-999, 2006.
            http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 
+    .. [2] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
+
+    .. [3] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized
+           trees", Machine Learning, 63(1), 3-42, 2006.
+
     Examples
     --------
     >>> from quantile_forest import RandomForestQuantileRegressor
     >>> from sklearn.datasets import fetch_california_housing
     >>> X, y = fetch_california_housing(return_X_y=True)
     >>> qrf = RandomForestQuantileRegressor(random_state=0)
     >>> qrf.fit(X[:1000], y[:1000])
@@ -1090,14 +1146,15 @@
         oob_score=False,
         n_jobs=None,
         random_state=None,
         verbose=0,
         warm_start=False,
         ccp_alpha=0.0,
         max_samples=None,
+        monotonic_cst=None,
     ):
         """Initialize random forest quantile regressor."""
         init_dict = {
             "estimator": DecisionTreeRegressor(),
             "n_estimators": n_estimators,
             "estimator_params": (
                 "criterion",
@@ -1116,27 +1173,30 @@
             "n_jobs": n_jobs,
             "random_state": random_state,
             "verbose": verbose,
             "warm_start": warm_start,
             "max_samples": max_samples,
             "max_samples_leaf": max_samples_leaf,
         }
+        if sklearn_version >= parse_version("1.4.0"):
+            init_dict["estimator_params"] += ("monotonic_cst",)
         super(RandomForestQuantileRegressor, self).__init__(**init_dict)
 
         self.default_quantiles = default_quantiles
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_samples_leaf = max_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
 
     def _more_tags(self):
         return {
             "multioutput": True,
             "_xfail_checks": {
                 "check_dataframe_column_names_consistency": "Internal calls.",
             },
@@ -1145,27 +1205,29 @@
 
 class ExtraTreesQuantileRegressor(BaseForestQuantileRegressor):
     """An extra-trees regressor that provides quantile estimates.
 
     A quantile extra trees regressor is a meta estimator that fits a number of
     randomized decision trees (a.k.a. extra-trees) on various sub-samples of
     the dataset, keeps the values of samples that reach each node, and
-    assesses the conditional distribution based on this information. The
+    assesses the conditional distribution based on this information [1]. The
     leaf-sample size is controlled with the `max_samples_leaf` parameter.
 
     Parameters
     ----------
     n_estimators : int, default=100
         The number of trees in the forest.
 
     default_quantiles : float, list, or "mean", default=0.5
         The default quantile or list of quantiles that the model tries to
         predict. Each quantile must be strictly between 0 and 1. If "mean",
         the model predicts the mean.
 
+        .. versionadded:: 1.2
+
     criterion : {"squared_error", "absolute_error", "friedman_mse", "poisson"}, \
             default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
         variance reduction as feature selection criterion and minimizes the L2
         loss using the mean of each terminal node, "friedman_mse", which uses
         mean squared error with Friedman's improvement score for potential
@@ -1215,25 +1277,27 @@
         equal weight when sample_weight is not provided.
 
     max_features : {"sqrt", "log2", None}, int or float, default=1.0
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a fraction and
-          `round(max_features * n_features)` features are considered at each
-          split.
-        - If "auto", then `max_features=n_features`.
+          `max(1, int(max_features * n_features_in_))` features are considered
+          at each split.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None or 1.0, then `max_features=n_features`.
 
         .. note::
             The default of 1.0 is equivalent to bagged trees and more
             randomness can be achieved by setting smaller values, e.g. 0.3.
 
+        .. sklearn-versionchanged:: 1.1
+            The default of `max_features` changed from `"auto"` to `"sqrt"`.
+
         Note: the search for a split does not stop until at least one
         valid partition of the node samples is found, even if it requires to
         effectively inspect more than ``max_features`` features.
 
     max_leaf_nodes : int, default=None
         Grow trees with ``max_leaf_nodes`` in best-first fashion.
         Best nodes are defined as relative reduction in impurity.
@@ -1257,15 +1321,15 @@
 
     bootstrap : bool, default=False
         Whether bootstrap samples are used when building trees. If False, the
         whole dataset is used to build each tree.
 
     oob_score : bool or callable, default=False
         Whether to use out-of-bag samples to estimate the generalization score.
-        By default, :func:`~sklearn.metrics.accuracy_score` is used.
+        By default, :func:`~sklearn.metrics.r2_score` is used.
         Provide a callable with signature `metric(y_true, y_pred)` to use a
         custom metric. Only available if `bootstrap=True`.
 
     n_jobs : int, default=None
         The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
         :meth:`decision_path` and :meth:`apply` are all parallelized over the
         trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
@@ -1298,20 +1362,37 @@
         to train each base estimator.
 
         - If None (default), then draw `X.shape[0]` samples.
         - If int, then draw `max_samples` samples.
         - If float, then draw `max_samples * X.shape[0]` samples. Thus,
           `max_samples` should be in the interval `(0.0, 1.0]`.
 
+    monotonic_cst : array-like of int of shape (n_features), default=None
+        Indicates the monotonicity constraint to enforce on each feature.
+          - 1: monotonically increasing
+          - 0: no constraint
+          - -1: monotonically decreasing
+
+        If monotonic_cst is None, no constraints are applied.
+
+        Monotonicity constraints are not supported for:
+          - multioutput regressions (i.e. when `n_outputs_ > 1`),
+          - regressions trained on data with missing values.
+
+        .. sklearn-versionadded:: 1.4
+
     Attributes
     ----------
-    estimator_ : ExtraTreeRegressor
+    estimator_ : :class:`~sklearn.tree.ExtraTreeRegressor`
         The child estimator template used to create the collection of fitted
         sub-estimators.
 
+        .. sklearn-versionadded:: 1.2
+           `base_estimator_` was renamed to `estimator_`.
+
     estimators_ : list of DecisionTreeRegressor
         The collection of fitted sub-estimators.
 
     feature_importances_ : ndarray of shape (n_features,)
         The impurity-based feature importances.
         The higher, the more important the feature.
         The importance of a feature is computed as the (normalized)
@@ -1335,25 +1416,41 @@
         Score of the training dataset obtained using an out-of-bag estimate.
         This attribute exists only when ``oob_score`` is True.
 
     oob_prediction_ : ndarray of shape (n_samples,) or (n_samples, n_outputs)
         Prediction computed with out-of-bag estimate on the training set.
         This attribute exists only when ``oob_score`` is True.
 
+    estimators_samples_ : list of arrays
+        The subset of drawn samples (i.e., the in-bag samples) for each base
+        estimator. Each subset is defined by an array of the indices selected.
+
+        .. sklearn-versionadded:: 1.4
+
     See Also
     --------
-    RandomForestQuantileRegressor : Quantile ensemble regressor using trees
-        with optimal splits.
+    RandomForestQuantileRegressor : Quantile ensemble regressor using trees.
+
+    Notes
+    -----
+    The default values for the parameters controlling the size of the trees
+    (e.g. ``max_depth``, ``min_samples_leaf``, etc.) lead to fully grown and
+    unpruned trees which can potentially be very large on some data sets. To
+    reduce memory consumption, the complexity and size of the trees should be
+    controlled by setting those parameter values.
 
     References
     ----------
     .. [1] N. Meinshausen, "Quantile Regression Forests", Journal of Machine
            Learning Research, 7(Jun), 983-999, 2006.
            http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 
+    .. [2] P. Geurts, D. Ernst., and L. Wehenkel, "Extremely randomized trees",
+           Machine Learning, 63(1), 3-42, 2006.
+
     Examples
     --------
     >>> from quantile_forest import ExtraTreesQuantileRegressor
     >>> from sklearn.datasets import fetch_california_housing
     >>> X, y = fetch_california_housing(return_X_y=True)
     >>> qrf = ExtraTreesQuantileRegressor(random_state=0)
     >>> qrf.fit(X[:1000], y[:1000])
@@ -1380,14 +1477,15 @@
         oob_score=False,
         n_jobs=None,
         random_state=None,
         verbose=0,
         warm_start=False,
         ccp_alpha=0.0,
         max_samples=None,
+        monotonic_cst=None,
     ):
         """Initialize extra trees quantile regressor."""
         init_dict = {
             "estimator": ExtraTreeRegressor(),
             "n_estimators": n_estimators,
             "estimator_params": (
                 "criterion",
@@ -1406,27 +1504,30 @@
             "n_jobs": n_jobs,
             "random_state": random_state,
             "verbose": verbose,
             "warm_start": warm_start,
             "max_samples": max_samples,
             "max_samples_leaf": max_samples_leaf,
         }
+        if sklearn_version >= parse_version("1.4.0"):
+            init_dict["estimator_params"] += ("monotonic_cst",)
         super(ExtraTreesQuantileRegressor, self).__init__(**init_dict)
 
         self.default_quantiles = default_quantiles
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_samples_leaf = max_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
+        self.monotonic_cst = monotonic_cst
 
     def _more_tags(self):
         return {
             "multioutput": True,
             "_xfail_checks": {
                 "check_dataframe_column_names_consistency": "Internal calls.",
             },
```

### Comparing `quantile-forest-1.3.4/quantile_forest/_quantile_forest_fast.pxd` & `quantile_forest-1.3.5/quantile_forest/_quantile_forest_fast.pxd`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/quantile_forest/_quantile_forest_fast.pyx` & `quantile_forest-1.3.5/quantile_forest/_quantile_forest_fast.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -503,22 +503,26 @@
         out = (left + right) * 0.5 / n_inputs
 
     return out
 
 
 cpdef vector[intp_t] generate_unsampled_indices(
     vector[intp_t] sample_indices,
+    intp_t n_total_samples,
     vector[set[intp_t]] duplicates,
 ) noexcept nogil:
     """Return a list of every unsampled index, accounting for duplicates.
 
     Parameters
     ----------
     sample_indices : array-like of shape (n_samples)
-        Sample indices for which to get duplicates.
+        Sampled indices.
+
+    n_total_samples : int
+        Number of total samples, sampled and unsampled.
 
     duplicates : list of sets
         List of sets of functionally identical indices.
 
     Returns
     -------
     unsampled_indices : array-like
@@ -539,15 +543,15 @@
     # Account for duplicates of sampled indices.
     for i in range(n_duplicates):
         for sampled_idx in duplicates[i]:
             if sampled_set.count(sampled_idx):
                 sampled_set.insert(duplicates[i].begin(), duplicates[i].end())
 
     # If the index is not in `sampled_set`, it is unsampled.
-    for i in range(n_samples):
+    for i in range(n_total_samples):
         if not sampled_set.count(i):
             unsampled_indices.push_back(i)
 
     return unsampled_indices
 
 
 cdef class QuantileForest:
```

### Comparing `quantile-forest-1.3.4/quantile_forest/tests/test_quantile_forest.py` & `quantile_forest-1.3.5/quantile_forest/tests/test_quantile_forest.py`

 * *Files 3% similar despite different names*

```diff
@@ -268,14 +268,15 @@
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
 def test_predict_quantiles_toy(name):
     check_predict_quantiles_toy(name)
 
 
 def check_predict_quantiles(
     name,
+    max_samples,
     max_samples_leaf,
     quantiles,
     weighted_quantile,
     aggregate_leaves_first,
 ):
     ForestRegressor = FOREST_REGRESSORS[name]
 
@@ -291,15 +292,21 @@
 
     X_test = x2.reshape(-1, 1)
     y_test = np.squeeze(X_test * 2)
 
     y_train = y_train.astype(np.float64)
     y_test = y_test.astype(np.float64)
 
-    est = ForestRegressor(n_estimators=10, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=10,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         y_pred = est.predict(
             X_test,
             quantiles=quantiles,
             weighted_quantile=weighted_quantile,
@@ -313,15 +320,21 @@
         assert_array_almost_equal(y_pred, y_test, -e1_high)
 
     # Check predicted quantiles on the California Housing Prices dataset.
     X_train, X_test, y_train, y_test = train_test_split(
         X_california, y_california, test_size=0.25, random_state=0
     )
 
-    est = ForestRegressor(n_estimators=10, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=10,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         y_pred = est.predict(
             X_test,
             quantiles=quantiles,
             weighted_quantile=weighted_quantile,
@@ -334,15 +347,21 @@
 
     if isinstance(quantiles, list):
         # Check that predicted values are monotonic.
         assert np.all(np.less_equal(y_pred[:, 0], y_pred[:, 1]))
         assert np.all(np.less_equal(y_pred[:, 1], y_pred[:, 2]))
 
     # Check that weighted and unweighted quantiles are all equal.
-    est = ForestRegressor(n_estimators=10, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=10,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     y_pred_1 = est.predict(
         X_test,
         quantiles=quantiles,
         weighted_quantile=True,
         weighted_leaves=False,
         aggregate_leaves_first=aggregate_leaves_first,
@@ -353,15 +372,21 @@
         weighted_quantile=False,
         weighted_leaves=False,
         aggregate_leaves_first=aggregate_leaves_first,
     )
     assert_allclose(y_pred_1, y_pred_2)
 
     # Check that weighted and unweighted leaves are all equal.
-    est = ForestRegressor(n_estimators=1, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=1,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         y_pred_1 = est.predict(
             X_test,
             quantiles=quantiles,
             weighted_quantile=weighted_quantile,
@@ -374,15 +399,21 @@
             weighted_quantile=weighted_quantile,
             weighted_leaves=False,
             aggregate_leaves_first=False,
         )
     assert_allclose(y_pred_1, y_pred_2)
 
     # Check that aggregated and unaggregated quantiles are all equal.
-    est = ForestRegressor(n_estimators=1, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=1,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     y_pred_1 = est.predict(
         X_test,
         quantiles=quantiles,
         weighted_quantile=weighted_quantile,
         weighted_leaves=False,
         aggregate_leaves_first=True,
@@ -393,15 +424,21 @@
         weighted_quantile=weighted_quantile,
         weighted_leaves=False,
         aggregate_leaves_first=False,
     )
     assert_allclose(y_pred_1, y_pred_2)
 
     # Check that omitting quantiles is the same as setting to 0.5.
-    est = ForestRegressor(n_estimators=1, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=1,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     y_pred_1 = est.predict(
         X_test,
         weighted_quantile=weighted_quantile,
         weighted_leaves=False,
         aggregate_leaves_first=True,
     )
@@ -452,71 +489,93 @@
         X = np.linspace(-1, 0.3, 500)
         y = np.empty((len(X), 2))
         y[:, 0] = (X**3) + 3 * np.exp(-6 * (X - 0.3) ** 2)
         y[:, 0] += np.random.normal(0, 0.2 * np.abs(X), len(X))
         y[:, 1] = np.log1p(X + 1)
         y[:, 1] += np.log1p(X + 1) * np.random.uniform(size=len(X))
 
-        est = ForestRegressor(n_estimators=1, max_samples_leaf=max_samples_leaf, random_state=0)
+        est = ForestRegressor(
+            n_estimators=1,
+            max_samples_leaf=max_samples_leaf,
+            max_samples=max_samples,
+            bootstrap=True,
+            random_state=0,
+        )
         est.fit(X.reshape(-1, 1), y)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
             y_pred = est.predict(
                 X.reshape(-1, 1),
                 quantiles=quantiles,
                 weighted_quantile=weighted_quantile,
                 aggregate_leaves_first=aggregate_leaves_first,
             )
         score = est.score(X.reshape(-1, 1), y, quantiles=0.5)
         assert y_pred.ndim == (3 if isinstance(quantiles, list) else 2)
         assert y_pred.shape[1] == y.shape[1]
         assert np.any(y_pred[:, 0, ...] != y_pred[:, 1, ...])
-        assert score > 0.97
+        assert score > 0.95
 
     # Check that specifying `quantiles` overwrites `default_quantiles`.
-    est1 = ForestRegressor(n_estimators=1, max_samples_leaf=max_samples_leaf, random_state=0)
+    est1 = ForestRegressor(
+        n_estimators=1,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est1.fit(X_train, y_train)
     y_pred_1 = est1.predict(X_test, quantiles=0.5)
     est2 = ForestRegressor(
         n_estimators=1,
         default_quantiles=[0.25, 0.5, 0.75],
         max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
         random_state=0,
     )
     est2.fit(X_train, y_train)
     y_pred_2 = est2.predict(X_test, quantiles=0.5)
     assert_allclose(y_pred_1, y_pred_2)
 
     # Check that specifying `interpolation` changes outputs.
-    est = ForestRegressor(n_estimators=10, max_samples_leaf=max_samples_leaf, random_state=0)
+    est = ForestRegressor(
+        n_estimators=10,
+        max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
+        bootstrap=True,
+        random_state=0,
+    )
     est.fit(X_train, y_train)
     y_pred_1 = est.predict(X_test, quantiles=0.5, interpolation="linear")
     y_pred_2 = est.predict(X_test, quantiles=0.5, interpolation="nearest")
     assert np.any(y_pred_1 != y_pred_2)
 
     # Check error if invalid quantiles.
     assert_raises(ValueError, est.predict, X_test, -0.01)
     assert_raises(ValueError, est.predict, X_test, 1.01)
 
 
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
+@pytest.mark.parametrize("max_samples", [None, 0.5, 1.0, 100])
 @pytest.mark.parametrize("max_samples_leaf", [None, 1])
 @pytest.mark.parametrize("quantiles", [None, "mean", 0.5, [0.2, 0.5, 0.8]])
 @pytest.mark.parametrize("weighted_quantile", [True, False])
 @pytest.mark.parametrize("aggregate_leaves_first", [True, False])
 def test_predict_quantiles(
     name,
+    max_samples,
     max_samples_leaf,
     quantiles,
     weighted_quantile,
     aggregate_leaves_first,
 ):
     check_predict_quantiles(
-        name, max_samples_leaf, quantiles, weighted_quantile, aggregate_leaves_first
+        name, max_samples, max_samples_leaf, quantiles, weighted_quantile, aggregate_leaves_first
     )
 
 
 def check_quantile_ranks_toy(name):
     # Check rank predictions on toy data.
     ForestRegressor = FOREST_REGRESSORS[name]
 
@@ -825,28 +884,30 @@
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
 def test_oob_samples_duplicates(name):
     check_oob_samples_duplicates(name)
 
 
 def check_predict_oob(
     name,
+    max_samples,
     max_samples_leaf,
     quantiles,
     weighted_quantile,
     aggregate_leaves_first,
 ):
     # Check OOB predictions.
     X = X_california
     y = y_california
 
     ForestRegressor = FOREST_REGRESSORS[name]
 
     est = ForestRegressor(
         n_estimators=20,
         max_samples_leaf=max_samples_leaf,
+        max_samples=max_samples,
         bootstrap=True,
         oob_score=True,
         random_state=0,
     )
     est.fit(X, y)
 
     n_quantiles = None
@@ -973,15 +1034,21 @@
         X,
         oob_score=True,
         indices=-np.ones(len(X) - 1),
     )
 
     # Check warning if not enough estimators.
     with np.errstate(divide="ignore", invalid="ignore"):
-        est = ForestRegressor(n_estimators=4, bootstrap=True, oob_score=True, random_state=0)
+        est = ForestRegressor(
+            n_estimators=4,
+            max_samples=max_samples,
+            bootstrap=True,
+            oob_score=True,
+            random_state=0,
+        )
         with pytest.warns():
             est.fit(X, y)
             est.predict(
                 X,
                 quantiles=quantiles,
                 weighted_quantile=weighted_quantile,
                 aggregate_leaves_first=aggregate_leaves_first,
@@ -1024,27 +1091,30 @@
             weighted_quantile=weighted_quantile,
             aggregate_leaves_first=aggregate_leaves_first,
             oob_score=True,
         )
 
 
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
+@pytest.mark.parametrize("max_samples", [None, 0.5, 1.0, 100])
 @pytest.mark.parametrize("max_samples_leaf", [None, 1])
 @pytest.mark.parametrize("quantiles", [None, "mean", 0.5, [0.2, 0.5, 0.8]])
 @pytest.mark.parametrize("weighted_quantile", [True, False])
 @pytest.mark.parametrize("aggregate_leaves_first", [True, False])
 def test_predict_oob(
     name,
+    max_samples,
     max_samples_leaf,
     quantiles,
     weighted_quantile,
     aggregate_leaves_first,
 ):
     check_predict_oob(
         name,
+        max_samples,
         max_samples_leaf,
         quantiles,
         weighted_quantile,
         aggregate_leaves_first,
     )
 
 
@@ -1460,28 +1530,29 @@
 
 
 def test_generate_unsampled_indices():
     # Check unsampled indices generation.
     max_index = 20
     duplicates = [[1, 4], [19, 10], [2, 3, 5], [6, 13]]
 
-    def _generate_unsampled_indices(sample_indices):
+    def _generate_unsampled_indices(sample_indices, n_total_samples):
         return generate_unsampled_indices(
             np.array(sample_indices, dtype=np.int64),
+            n_total_samples=n_total_samples,
             duplicates=duplicates,
         )
 
     # If all indices are sampled, there are no unsampled indices.
     indices = [idx for idx in range(max_index)]
     expected = np.array([], dtype=np.int64)
-    assert_array_equal(_generate_unsampled_indices(indices), expected)
+    assert_array_equal(_generate_unsampled_indices(indices, max_index), expected)
 
     # Index 7 has no duplicates, and thus should be the only unsampled index.
     indices = [7 for _ in range(max_index)]
     expected = np.array([idx for idx in range(max_index) if idx != 7])
-    assert_array_equal(_generate_unsampled_indices(indices), expected)
+    assert_array_equal(_generate_unsampled_indices(indices, max_index), expected)
 
     # Check sample indices [0, 1, 2] with duplicates set(1, 4) + set(2, 3, 5),
     # which excludes [0, 1, 2, 3, 4, 5] (i.e., range(6)) from unsampled.
     indices = [idx % 3 for idx in range(max_index)]
     expected = [x for x in range(max_index) if x not in range(6)]
-    assert_array_equal(_generate_unsampled_indices(indices), expected)
+    assert_array_equal(_generate_unsampled_indices(indices, max_index), expected)
```

### Comparing `quantile-forest-1.3.4/quantile_forest.egg-info/PKG-INFO` & `quantile_forest-1.3.5/quantile_forest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.3.4
+Version: 1.3.5
 Summary: scikit-learn compatible quantile forests.
 Home-page: https://zillow.github.io/quantile-forest
 Download-URL: https://pypi.org/project/quantile-forest/#files
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Project-URL: Documentation, https://zillow.github.io/quantile-forest
 Project-URL: Source, https://github.com/zillow/quantile-forest
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantile-forest Version: 1.3.4 Summary: scikit-
+Metadata-Version: 2.1 Name: quantile-forest Version: 1.3.5 Summary: scikit-
 learn compatible quantile forests. Home-page: https://zillow.github.io/
 quantile-forest Download-URL: https://pypi.org/project/quantile-forest/#files
 Maintainer: Zillow Group AI Team License: Apache License 2.0 Project-URL:
 Documentation, https://zillow.github.io/quantile-forest Project-URL: Source,
 https://github.com/zillow/quantile-forest Project-URL: Tracker, https://
 github.com/zillow/quantile-forest/issues Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `quantile-forest-1.3.4/quantile_forest.egg-info/SOURCES.txt` & `quantile_forest-1.3.5/quantile_forest.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,41 +4,47 @@
 pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
-docs/install.rst
 docs/make.bat
 docs/references.rst
 docs/refs.bib
 docs/sphinx_requirements.txt
-docs/user_guide.rst
 docs/_static/favicon.ico
 docs/_static/quantile-forest-logo-white.png
 docs/_static/quantile-forest-logo.png
 docs/_static/css/gallery.css
 docs/_static/css/theme_overrides.css
 docs/_static/js/copybutton.js
 docs/_templates/class.rst
 docs/_templates/navbar-project.html
 docs/_templates/sidebar-logo.html
+docs/getting_started/developers.rst
+docs/getting_started/installation.rst
+docs/releases/changes.rst
 docs/sphinxext/__init__.py
+docs/sphinxext/directives.py
 docs/sphinxext/gallery.py
 docs/sphinxext/utils.py
+docs/user_guide/fit_predict.rst
+docs/user_guide/introduction.rst
+docs/user_guide/proximities.rst
+docs/user_guide/quantile_ranks.rst
 examples/__init__.py
+examples/plot_predict_custom.py
 examples/plot_quantile_conformalized.py
 examples/plot_quantile_example.py
 examples/plot_quantile_extrapolation.py
 examples/plot_quantile_interpolation.py
 examples/plot_quantile_intervals.py
 examples/plot_quantile_multioutput.py
 examples/plot_quantile_vs_standard.py
-examples/plot_quantile_weighting.py
 quantile_forest/__init__.py
 quantile_forest/_min_dependencies.py
 quantile_forest/_quantile_forest.py
 quantile_forest/_quantile_forest_fast.pxd
 quantile_forest/_quantile_forest_fast.pyx
 quantile_forest/version.py
 quantile_forest/version.txt
```

### Comparing `quantile-forest-1.3.4/setup.cfg` & `quantile_forest-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.3.4/setup.py` & `quantile_forest-1.3.5/setup.py`

 * *Files identical despite different names*

