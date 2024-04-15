# Comparing `tmp/erlab-2.2.1.tar.gz` & `tmp/erlab-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.2.1.tar", last modified: Sun Apr 14 04:29:20 2024, max compression
+gzip compressed data, was "erlab-2.2.2.tar", last modified: Mon Apr 15 08:17:23 2024, max compression
```

## Comparing `erlab-2.2.1.tar` & `erlab-2.2.2.tar`

### file list

```diff
@@ -1,176 +1,178 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.480856 erlab-2.2.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-14 04:29:13.000000 erlab-2.2.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-14 04:29:13.000000 erlab-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-14 04:29:13.000000 erlab-2.2.1/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   107661 2024-04-14 04:29:16.000000 erlab-2.2.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-14 04:29:13.000000 erlab-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47789 2024-04-14 04:29:20.524856 erlab-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-14 04:29:13.000000 erlab-2.2.1/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-14 04:29:13.000000 erlab-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.492856 erlab-2.2.1/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    16040 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   321080 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   317804 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3357 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    22039 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     5063 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    50534 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379705 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    16293 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-14 04:29:13.000000 erlab-2.2.1/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4381 2024-04-14 04:29:13.000000 erlab-2.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-14 04:29:13.000000 erlab-2.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 04:29:20.524856 erlab-2.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.480856 erlab-2.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.504856 erlab-2.2.1/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-14 04:29:16.000000 erlab-2.2.1/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35514 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.504856 erlab-2.2.1/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      955 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10583 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     8402 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6510 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    11749 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15393 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10629 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21311 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22774 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9454 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19705 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54143 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2160 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31737 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.516856 erlab-2.2.1/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7594 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7804 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6777 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.516856 erlab-2.2.1/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18284 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    37209 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47789 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4752 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.484856 erlab-2.2.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.160388 erlab-2.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.116388 erlab-2.2.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.124389 erlab-2.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-15 08:17:16.000000 erlab-2.2.2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-15 08:17:16.000000 erlab-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.124389 erlab-2.2.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-15 08:17:16.000000 erlab-2.2.2/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-15 08:17:16.000000 erlab-2.2.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-15 08:17:16.000000 erlab-2.2.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-15 08:17:16.000000 erlab-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      785 2024-04-15 08:17:16.000000 erlab-2.2.2/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   109977 2024-04-15 08:17:19.000000 erlab-2.2.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-15 08:17:16.000000 erlab-2.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47831 2024-04-15 08:17:23.160388 erlab-2.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-15 08:17:16.000000 erlab-2.2.2/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-15 08:17:16.000000 erlab-2.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.124389 erlab-2.2.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.128389 erlab-2.2.2/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16114 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.136388 erlab-2.2.2/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   321080 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   317804 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.136388 erlab-2.2.2/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.136388 erlab-2.2.2/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    22039 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    51355 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379859 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16293 2024-04-15 08:17:16.000000 erlab-2.2.2/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-15 08:17:16.000000 erlab-2.2.2/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-15 08:17:16.000000 erlab-2.2.2/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-15 08:17:16.000000 erlab-2.2.2/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-15 08:17:16.000000 erlab-2.2.2/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     3955 2024-04-15 08:17:16.000000 erlab-2.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-15 08:17:16.000000 erlab-2.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 08:17:23.160388 erlab-2.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.116388 erlab-2.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.140388 erlab-2.2.2/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-15 08:17:19.000000 erlab-2.2.2/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35514 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.140388 erlab-2.2.2/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.144388 erlab-2.2.2/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.144388 erlab-2.2.2/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10583 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     8402 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6510 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    11749 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15393 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.144388 erlab-2.2.2/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.144388 erlab-2.2.2/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.148388 erlab-2.2.2/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21311 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22774 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9657 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.148388 erlab-2.2.2/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19705 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.148388 erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.148388 erlab-2.2.2/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40493 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.152388 erlab-2.2.2/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8022 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.152388 erlab-2.2.2/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.156388 erlab-2.2.2/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    37209 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.156388 erlab-2.2.2/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-15 08:17:16.000000 erlab-2.2.2/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.160388 erlab-2.2.2/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47831 2024-04-15 08:17:23.000000 erlab-2.2.2/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4780 2024-04-15 08:17:23.000000 erlab-2.2.2/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 08:17:23.000000 erlab-2.2.2/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-15 08:17:23.000000 erlab-2.2.2/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-15 08:17:23.000000 erlab-2.2.2/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.156388 erlab-2.2.2/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-15 08:17:16.000000 erlab-2.2.2/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-15 08:17:16.000000 erlab-2.2.2/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-15 08:17:16.000000 erlab-2.2.2/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.120388 erlab-2.2.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.160388 erlab-2.2.2/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 08:17:23.160388 erlab-2.2.2/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9348 2024-04-15 08:17:16.000000 erlab-2.2.2/tests/io/test_dataloader.py
```

### Comparing `erlab-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/.github/workflows/pr.yml` & `erlab-2.2.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/.github/workflows/release.yml` & `erlab-2.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/.gitignore` & `erlab-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/.pre-commit-config.yaml` & `erlab-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/.readthedocs.yaml` & `erlab-2.2.2/.readthedocs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 version: 2
 
 # Set the OS, Python version and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
     # python: "mambaforge-22.9"
-    python: "3.11"
+    python: "3.12"
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
   configuration: docs/source/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
-# formats:
-  # - pdf
-#   - epub
+formats:
+  - htmlzip
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
     - requirements: docs/requirements.txt
```

### Comparing `erlab-2.2.1/CHANGELOG.md` & `erlab-2.2.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,58 @@
 # CHANGELOG
 
 
 
+## v2.2.2 (2024-04-15)
+
+### Chore
+
+* cleanup pyproject.toml ([`0331132`](https://github.com/kmnhan/erlabpy/commit/033113247ea5d8fa8bc4afb9513b349b95080bed))
+
+* (**deps**) add ipywidgets to optional dependency group viz ([`0062966`](https://github.com/kmnhan/erlabpy/commit/00629663742ada02ade556cb19ca0b14bd864fec))
+
+### Ci
+
+* (**readthdocs**) update build python version and add zip format ([`b2cc6fc`](https://github.com/kmnhan/erlabpy/commit/b2cc6fc1f732bab8904f90e10e194d4dffee5d57))
+
+### Documentation
+
+* (**io**) add tutorial for writing advanced plugins ([`11f289e`](https://github.com/kmnhan/erlabpy/commit/11f289edd451e10773d99ae1c9fc47cde22b06dc))
+
+* add ipywidgets to intersphinx mapping ([`0ee46f8`](https://github.com/kmnhan/erlabpy/commit/0ee46f8c6d783f2ee63cad807abf5e8582cfaa31))
+
+### Fix
+
+* (**io**) unify call signature for summarize ([`e2782c8`](https://github.com/kmnhan/erlabpy/commit/e2782c898d5aaaa1443b2bc82bb61fb40a28d232))
+
+* resolve failing tests due to changes in sample data generation ([`80f0045`](https://github.com/kmnhan/erlabpy/commit/80f004574950834e42dbfa7677031d0f9f113bda))
+
+* (**interactive.exampledata**) properly generate 2D data ([`825260c`](https://github.com/kmnhan/erlabpy/commit/825260c8ceb0a79b8c071750003529b91cda3573))
+
+### Performance
+
+* (**io**) speedup merlin summary generation by excluding duplicates ([`d6b4253`](https://github.com/kmnhan/erlabpy/commit/d6b42537ce48232b5112daef8f31e5cf86ea921a))
+
+### Refactor
+
+* (**io**) allow for more complex setups ([`f67b2e4`](https://github.com/kmnhan/erlabpy/commit/f67b2e4c7b092b7ca2db00ce02a23647879c514b))
+
+  LoaderBase.infer_index now returns a second argument, which is a dictionary containing optional keyword arguments to load.
+
+* (**io**) provide rich interactive summary ([`b075a9e`](https://github.com/kmnhan/erlabpy/commit/b075a9ee59b61892462fc475e78b036a54408099))
+
+* (**io**) include &#34;Path&#34; column in ssrl loader summary ([`ae1d8ae`](https://github.com/kmnhan/erlabpy/commit/ae1d8aee051aa71563f6a6009ce9672e56edfae7))
+
+* (**io**) improve array formatting in summary ([`1718529`](https://github.com/kmnhan/erlabpy/commit/171852957db7fe53ff6a5c5c5f843530078d4b46))
+
+### Test
+
+* add test for dataloader ([`64cde09`](https://github.com/kmnhan/erlabpy/commit/64cde099dbb13d8b148e67d1fe23a8849041dae4))
+
+
 ## v2.2.1 (2024-04-14)
 
 ### Chore
 
 * (**deps**) pin lmfit&lt;1.3.0 ([`915fc60`](https://github.com/kmnhan/erlabpy/commit/915fc60e8e7e8a2dfc9a56bbc1afd1c737bcc3d5))
 
 ### Documentation
```

### Comparing `erlab-2.2.1/LICENSE` & `erlab-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/PKG-INFO` & `erlab-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -730,14 +730,15 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: viz
 Requires-Dist: cmasher; extra == "viz"
 Requires-Dist: cmocean; extra == "viz"
 Requires-Dist: colorcet; extra == "viz"
 Requires-Dist: hvplot; extra == "viz"
+Requires-Dist: ipywidgets; extra == "viz"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/erlab.svg)](https://anaconda.org/conda-forge/erlab)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
```

### Comparing `erlab-2.2.1/PythonInterface.ipf` & `erlab-2.2.2/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/README.md` & `erlab-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/Makefile` & `erlab-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/environment.yml` & `erlab-2.2.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/make.bat` & `erlab-2.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/conf.py` & `erlab-2.2.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "pyqtgraph": ("https://pyqtgraph.readthedocs.io/en/latest/", None),
     "csaps": ("https://csaps.readthedocs.io/en/latest/", None),
     "iminuit": ("https://scikit-hep.org/iminuit/", None),
     "cmasher": ("https://cmasher.readthedocs.io/", None),
+    "ipywidgets": ("https://ipywidgets.readthedocs.io/en/stable/", None),
 }
 
 
 # -- Plot configuration ------------------------------------------------------
 
 plot_formats = ["pdf"]
 plot_basedir = "pyplots"
```

### Comparing `erlab-2.2.1/docs/source/contributing.rst` & `erlab-2.2.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/getting-started.rst` & `erlab-2.2.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/flowchart_multiple.pdf` & `erlab-2.2.2/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/flowchart_single.pdf` & `erlab-2.2.2/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/imagetool_dark.png` & `erlab-2.2.2/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/imagetool_light.png` & `erlab-2.2.2/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/ktool_1_dark.png` & `erlab-2.2.2/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/ktool_1_light.png` & `erlab-2.2.2/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/ktool_2_dark.png` & `erlab-2.2.2/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/images/ktool_2_light.png` & `erlab-2.2.2/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/index.rst` & `erlab-2.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/pyplots/norms.py` & `erlab-2.2.2/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/reference.rst` & `erlab-2.2.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/refs.bib` & `erlab-2.2.2/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.2.2/docs/source/user-guide/curve-fitting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/user-guide/index.rst` & `erlab-2.2.2/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/user-guide/indexing.ipynb` & `erlab-2.2.2/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/docs/source/user-guide/kconv.ipynb` & `erlab-2.2.2/docs/source/user-guide/kconv.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989870931537599%*

 * *Differences: {"'cells'": "{0: {'metadata': {'vscode': OrderedDict([('languageId', 'raw')])}, 'source': {insert: "*

 * *            "[(3, 'Momentum conversion in ERLabPy is exact with no small angle approximation, but "*

 * *            "is also\\n'), (4, 'very fast, thanks to the numba-accelerated trilinear interpolation "*

 * *            "in\\n'), (6, '\\n'), (7, '.. _nomenclature:\\n'), (12, 'Momentum conversion in "*

 * *            "ERLabPy follows the nomenclature from :cite:t:`ishida2018kconv`.\\n'), (13, 'All "*

 * *            'experim […]*

```diff
@@ -4,32 +4,42 @@
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
-                "tags": []
+                "tags": [],
+                "vscode": {
+                    "languageId": "raw"
+                }
             },
             "source": [
                 "Momentum conversion\n",
                 "===================\n",
                 "\n",
-                "Momentum conversion in ERLabPy is exact with no small angle approximation, but\n",
-                "is also very fast, thanks to the numba-accelerated trilinear interpolation in\n",
+                "Momentum conversion in ERLabPy is exact with no small angle approximation, but is also\n",
+                "very fast, thanks to the numba-accelerated trilinear interpolation in\n",
                 ":mod:`erlab.analysis.interpolate`\\ .\n",
                 "\n",
+                ".. _nomenclature:\n",
+                "\n",
                 "Nomenclature\n",
                 "------------\n",
                 "\n",
-                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`ishida2018kconv`. All experimental geometry are classified into 4 types. Definition of angles differ for each geometry.\n",
+                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`ishida2018kconv`.\n",
+                "All experimental geometry are classified into 4 types. Definition of angles differ for\n",
+                "each geometry.\n",
                 "\n",
-                "For instance, image a typical Type 1 setup with a vertical slit that acquires maps by rotating about the `z` axis in the lab frame. In this case, the polar angle (rotation about `z`) is :math:`\u03b2`, and the tilt angle is :math:`\u03be`.\n",
+                "For instance, imagine a typical Type 1 setup with a vertical slit that acquires maps by\n",
+                "rotating about the `z` axis in the lab frame. In this case, the polar angle (rotation\n",
+                "about `z`) is :math:`\u03b2`, and the tilt angle is :math:`\u03be`.\n",
                 "\n",
-                "In all cases, :math:`\u03b4` is the azimuthal angle that indicates in-plane rotation, and :math:`\u03b1` is the angle along the slit."
+                "In all cases, :math:`\u03b4` is the azimuthal angle that indicates in-plane rotation, and\n",
+                ":math:`\u03b1` is the angle along the slit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "editable": true,
@@ -580,15 +590,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from erlab.interactive.exampledata import generate_data_angles\n",
                 "\n",
-                "dat = generate_data_angles().T\n",
+                "dat = generate_data_angles(assign_attributes=True).T\n",
                 "dat"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `erlab-2.2.1/docs/source/user-guide/plotting.ipynb` & `erlab-2.2.2/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/environment.yml` & `erlab-2.2.2/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/environment_apple.yml` & `erlab-2.2.2/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/environment_nogit.yml` & `erlab-2.2.2/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/environment_nogit_mkl.yml` & `erlab-2.2.2/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/pyproject.toml` & `erlab-2.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 dev = [
     "pytest",
     "pytest-xdist",
     "python-semantic-release",
     "ruff",
     "pre-commit",
 ]
-viz = ["cmasher", "cmocean", "colorcet", "hvplot"]
+viz = ["cmasher", "cmocean", "colorcet", "hvplot", "ipywidgets"]
 
 [project.urls]
 Documentation = "https://erlabpy.readthedocs.io"
 Repository = "https://github.com/kmnhan/erlabpy.git"
 Issues = "https://github.com/kmnhan/erlabpy/issues"
 Changelog = "https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md"
 
@@ -79,44 +79,27 @@
 [tool.setuptools_scm]
 
 [tool.semantic_release]
 assets = []
 build_command = "pip install build && python -m build"
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
-logging_use_named_masks = false
-major_on_zero = true
-allow_zero_version = true
 tag_format = "v{version}"
 version_variables = ["src/erlab/__init__.py:__version__"]
 
 [tool.semantic_release.branches.main]
 match = "(main|master)"
 prerelease_token = "rc"
 prerelease = false
 
 [tool.semantic_release.changelog]
 template_dir = "templates"
 changelog_file = "CHANGELOG.md"
 exclude_commit_patterns = []
 
-[tool.semantic_release.changelog.environment]
-block_start_string = "{%"
-block_end_string = "%}"
-variable_start_string = "{{"
-variable_end_string = "}}"
-comment_start_string = "{#"
-comment_end_string = "#}"
-trim_blocks = false
-lstrip_blocks = false
-newline_sequence = "\n"
-keep_trailing_newline = false
-extensions = []
-autoescape = true
-
 [tool.semantic_release.commit_author]
 env = "GIT_COMMIT_AUTHOR"
 default = "semantic-release <semantic-release>"
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
     "build",
@@ -129,29 +112,27 @@
     "style",
     "refactor",
     "test",
     "tests",
 ]
 minor_tags = ["feat"]
 patch_tags = ["fix", "perf"]
-default_bump_level = 0
 
 [tool.semantic_release.remote]
 name = "origin"
 type = "github"
 ignore_token_for_push = false
 
 [tool.semantic_release.remote.token]
 env = "GH_TOKEN"
 
 [tool.semantic_release.publish]
 dist_glob_patterns = ["dist/*"]
 upload_to_vcs_release = true
 
-
 [tool.ruff]
 line-length = 88
 indent-width = 4
 
 [tool.ruff.lint]
 select = [
     "E4",
```

### Comparing `erlab-2.2.1/src/erlab/accessors.py` & `erlab-2.2.2/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/__init__.py` & `erlab-2.2.2/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/correlation.py` & `erlab-2.2.2/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.2.2/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.2.2/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/functions/general.py` & `erlab-2.2.2/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/minuit.py` & `erlab-2.2.2/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/models.py` & `erlab-2.2.2/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/fit/spline.py` & `erlab-2.2.2/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/gold.py` & `erlab-2.2.2/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/image.py` & `erlab-2.2.2/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/interpolate.py` & `erlab-2.2.2/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/kspace.py` & `erlab-2.2.2/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/mask/__init__.py` & `erlab-2.2.2/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/mask/polygon.py` & `erlab-2.2.2/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/transform.py` & `erlab-2.2.2/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/analysis/utilities.py` & `erlab-2.2.2/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/characterization/resistance.py` & `erlab-2.2.2/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/characterization/xrd.py` & `erlab-2.2.2/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/constants.py` & `erlab-2.2.2/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/__init__.py` & `erlab-2.2.2/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/bzplot.py` & `erlab-2.2.2/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/colors.py` & `erlab-2.2.2/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/curvefittingtool.py` & `erlab-2.2.2/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/derivative.py` & `erlab-2.2.2/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/dtool.ui` & `erlab-2.2.2/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/exampledata.py` & `erlab-2.2.2/src/erlab/interactive/exampledata.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,14 @@
     else:
         kx = np.linspace(*krange, shape[0])
         ky = np.linspace(*krange, shape[1])
 
     eV = np.linspace(*Erange, shape[2])
 
     dE = eV[1] - eV[0]
-    dk = ((kx[1] - kx[0]) + (ky[1] - ky[0])) / 2
 
     point_iter = np.array(np.meshgrid(kx, ky)).T.reshape(-1, 2)
 
     Eij = band(point_iter, t, a).reshape(*shape[:-1], 1)
 
     Akw_p = spectral_function(eV[None, None, :], Eij + bandshift, Sreal, Simag)
     Akw_m = spectral_function(eV[None, None, :], -Eij + bandshift, Sreal, Simag)
@@ -130,23 +129,24 @@
 
     if noise:
         rng = np.random.default_rng()
         out = rng.poisson(out).astype(float)
 
     broadened = scipy.ndimage.gaussian_filter(
         out,
-        sigma=[kres / dk, kres / dk, Eres / dE],
+        sigma=[kres / (k[1] - k[0]) if len(k) > 1 else 0 for k in (kx, ky)]
+        + [Eres / dE],
         truncate=10.0,
     )
     if noise:
         broadened = scipy.ndimage.gaussian_filter(
             rng.poisson(broadened).astype(float), ccd_sigma, truncate=10.0
         )
 
-    return xr.DataArray(broadened, coords={"kx": kx, "ky": ky, "eV": eV})
+    return xr.DataArray(broadened, coords={"kx": kx, "ky": ky, "eV": eV}).squeeze()
 
 
 def generate_data_angles(
     shape: tuple[int, int, int] = (500, 60, 500),
     angrange: float | tuple[float, float] | dict[str, tuple[float, float]] = 15.0,
     Erange: tuple[float, float] = (-0.45, 0.12),
     hv: float = 50.0,
@@ -160,14 +160,15 @@
     Sreal: float = 0.0,
     Simag: float = 0.03,
     angres: float = 0.1,
     Eres: float = 10.0e-3,
     noise: bool = True,
     count: int = 10000,
     ccd_sigma: float = 0.6,
+    assign_attributes: bool = False,
 ) -> xr.DataArray:
     """
     Generate simulated data for a given shape.
 
     Parameters
     ----------
     shape
@@ -202,14 +203,16 @@
         Broadening in energy in electronvolts, by default 2.0e-3
     noise
         Whether to add noise to the generated data, by default `True`
     count
         Determines the signal-to-noise ratio when `noise` is `True`, by default 10000
     ccd_sigma
         The sigma value for CCD noise generation when `noise` is `True`, by default 0.6
+    assign_attributes
+        Whether to assign attributes to the generated data, by default `False`
 
     Returns
     -------
     xarray.DataArray
         The generated data with coordinates for alpha, beta, and eV.
 
     """
@@ -231,15 +234,14 @@
 
     Ekin = hv - 4.5 + eV[None, None, :]
     forward_func, _ = erlab.analysis.kspace.get_kconv_func(
         Ekin, configuration=configuration, angle_params={}
     )
 
     dE = eV[1] - eV[0]
-    dalpha, dbeta = (alpha[1] - alpha[0]), (beta[1] - beta[0])
 
     a_mesh, b_mesh = np.meshgrid(alpha, beta, indexing="ij")
     kxv, kyv = forward_func(a_mesh[:, :, None], b_mesh[:, :, None])
     point_iter = np.stack([kxv, kyv], axis=3)
 
     Eij = band(point_iter, t, a)
 
@@ -255,15 +257,16 @@
 
     if noise:
         rng = np.random.default_rng()
         out = rng.poisson(out).astype(float)
 
     out = scipy.ndimage.gaussian_filter(
         out,
-        sigma=[angres / dalpha, angres / dbeta, Eres / dE],
+        sigma=[angres / (a[1] - a[0]) if len(a) > 1 else 0 for a in (alpha, beta)]
+        + [Eres / dE],
         truncate=10.0,
     )
     if noise:
         out = scipy.ndimage.gaussian_filter(
             rng.poisson(out).astype(float), ccd_sigma, truncate=10.0, axes=(0, 2)
         )
 
@@ -273,19 +276,22 @@
     match configuration:
         case (
             erlab.analysis.kspace.AxesConfiguration.Type1DA
             | erlab.analysis.kspace.AxesConfiguration.Type2DA
         ):
             out = out.assign_coords(chi=0.0)
 
-    return out.assign_attrs(
-        configuration=int(configuration),
-        temp_sample=temp,
-        sample_workfunction=4.5,
-    )
+    if assign_attributes:
+        out = out.assign_attrs(
+            configuration=int(configuration),
+            temp_sample=temp,
+            sample_workfunction=4.5,
+        )
+
+    return out.squeeze()
 
 
 if __name__ == "__main__":
     # out = generate_data(
     #     shape=(201, 202, 203),
     #     krange=1.4,
     #     Erange=(-0.45, 0.09),
```

### Comparing `erlab-2.2.1/src/erlab/interactive/fermiedge.py` & `erlab-2.2.2/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/controls.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/core.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.2.2/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/kspace.py` & `erlab-2.2.2/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/ktool.ui` & `erlab-2.2.2/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/masktool.py` & `erlab-2.2.2/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/interactive/utilities.py` & `erlab-2.2.2/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/__init__.py` & `erlab-2.2.2/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/dataloader.py` & `erlab-2.2.2/src/erlab/io/dataloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 This module provides a base class `LoaderBase` for implementing data loaders. Data
 loaders are plugins used to load data from various file formats. Each data loader that
 subclasses `LoaderBase` is registered on import in `loaders`.
 
 Loaded ARPES data must contain several attributes and coordinates. See the
 implementation of `LoaderBase.validate` for details.
 
-For any data loader plugin subclassing `LoaderBase`, the following attributes and
-methods must be defined: `LoaderBase.name`, `LoaderBase.aliases`, `LoaderBase.name_map`,
-`LoaderBase.coordinate_attrs`, `LoaderBase.additional_attrs`,
-`LoaderBase.always_single`, `LoaderBase.skip_validate`, :func:`LoaderBase.load_single`,
-:func:`LoaderBase.identify`, :func:`LoaderBase.infer_index`, and
-:func:`LoaderBase.generate_summary`.
-
 A detailed guide on how to implement a data loader can be found in
 :doc:`../user-guide/io`.
 
 If additional post-processing is required, the :func:`LoaderBase.post_process` method
 can be extended to include the necessary functionality.
 
 """
 
 from __future__ import annotations
 
 import contextlib
 import datetime
+import importlib
 import itertools
 import os
 import warnings
 from typing import TYPE_CHECKING
 
 import joblib
 import numpy as np
@@ -175,25 +169,26 @@
 
         - For numpy arrays:
             - If the array has a size of 1, the value is recursively formatted using
               `formatter(val.item())`.
             - If the array can be squeezed to a 1-dimensional array, the following are
               applied.
 
-                - If the array is evenly spaced, the start, end, and step values are
-                  formatted and returned as a string in the format "start→end (step)".
+                - If the array is evenly spaced, the start, end, step, and length values
+                  are formatted and returned as a string in the format "start→end (step,
+                  length)".
                 - If the array is monotonic increasing or decreasing but not evenly
-                  spaced, the start and end values are formatted and returned as a
-                  string in the format "start→end".
+                  spaced, the start, end, and length values are formatted and returned
+                  as a string in the format "start→end (length)".
                 - If all elements are equal, the value is recursively formatted using
                   `formatter(val[0])`.
-                - If the array is not monotonic, the mean and standard deviation values
-                  are formatted and returned as a string in the format "mean±std".
+                - If the array is not monotonic, the minimum and maximum values are
+                  formatted and returned as a string in the format "min~max".
 
-            - For other dimensions, the array is returned as is.
+            - For arrays with more dimensions, the array is returned as is.
 
         - For lists:
             The list is grouped by consecutive equal elements, and the count of each
             element is formatted and returned as a string in the format
             "[element]×count".
 
         - For floating-point numbers:
@@ -212,28 +207,31 @@
         - For other types:
             The value is returned as is.
 
         Examples
         --------
 
         >>> formatter(np.array([0.1, 0.15, 0.2]))
-        '0.1→0.2 (0.05)'
+        '0.1→0.2 (0.05, 3)'
 
         >>> formatter(np.array([1.0, 2.0, 2.1]))
-        '1→2.1'
+        '1→2.1 (3)'
 
         >>> formatter(np.array([1.0, 2.1, 2.0]))
-        '1.7±0.4967'
+        '1~2.1 (3)'
 
         >>> formatter([1, 1, 2, 2, 2, 3, 3, 3, 3])
         '[1]×2, [2]×3, [3]×4'
 
         >>> formatter(3.14159)
         '3.1416'
 
+        >>> formatter(42.0)
+        '42'
+
         >>> formatter(42)
         '42'
 
         >>> formatter(datetime.datetime(2024, 1, 1, 12, 0, 0, 0))
         '2024-01-01 12:00:00'
         """
         if isinstance(val, np.ndarray):
@@ -243,24 +241,27 @@
             elif val.squeeze().ndim == 1:
                 val = val.squeeze()
 
                 if _is_uniform(val):
                     start, end, step = tuple(
                         cls.formatter(v) for v in (val[0], val[-1], val[1] - val[0])
                     )
-                    return f"{start}→{end} ({step})".replace("-", "−")
+                    return f"{start}→{end} ({step}, {len(val)})".replace("-", "−")
 
                 elif _is_monotonic(val):
                     if val[0] == val[-1]:
                         return cls.formatter(val[0])
 
-                    return f"{cls.formatter(val[0])}→{cls.formatter(val[-1])}"
+                    return (
+                        f"{cls.formatter(val[0])}→{cls.formatter(val[-1])} ({len(val)})"
+                    )
 
                 else:
-                    return f"{cls.formatter(np.mean(val))}±{cls.formatter(np.std(val))}"
+                    mn, mx = tuple(cls.formatter(v) for v in (np.min(val), np.max(val)))
+                    return f"{mn}~{mx} ({len(val)})"
 
             else:
                 return val
 
         elif isinstance(val, list):
             return ", ".join(
                 [f"[{k}]×{len(tuple(g))}" for k, g in itertools.groupby(val)]
@@ -297,16 +298,19 @@
         Returns
         -------
         pandas.io.formats.style.Styler
             The styler to be displayed.
 
         """
         style = df.style.format(cls.formatter)
-        if "Time" in df.columns:
-            style = style.hide(["Time"], axis="columns")
+
+        hidden = [c for c in ("Time", "Path") if c in df.columns]
+        if len(hidden) > 0:
+            style = style.hide(hidden, axis="columns")
+
         return style
 
     def load(
         self,
         identifier: str | os.PathLike | int | None,
         data_dir: str | os.PathLike | None = None,
         **kwargs: dict,
@@ -371,20 +375,24 @@
                 identifier = os.path.join(data_dir, identifier)
 
             if not single:
                 # Get file name without extension and path
                 basename_no_ext: str = os.path.splitext(os.path.basename(identifier))[0]
 
                 # Infer index from file name
-                new_identifier: int | None = self.infer_index(basename_no_ext)
+                new_identifier, additional_kwargs = self.infer_index(basename_no_ext)
 
                 if new_identifier is not None:
                     # On success, load with the index
                     new_dir: str = os.path.dirname(identifier)
-                    return self.load(new_identifier, new_dir, single=single, **kwargs)
+
+                    new_kwargs = kwargs | additional_kwargs
+                    return self.load(
+                        new_identifier, new_dir, single=single, **new_kwargs
+                    )
                 else:
                     # On failure, assume single file
                     single = True
 
             data = self.load_single(identifier)
 
         data = self.post_process_general(data)
@@ -393,39 +401,52 @@
             self.validate(data)
 
         data.attrs["data_loader_name"] = str(self.name)
 
         return data
 
     def summarize(
-        self, data_dir: str | os.PathLike, usecache: bool = True, **kwargs
-    ) -> pandas.DataFrame:
+        self,
+        data_dir: str | os.PathLike,
+        usecache: bool = True,
+        *,
+        display: bool = True,
+        **kwargs,
+    ) -> pandas.DataFrame | pandas.io.formats.style.Styler | None:
         """
-        Takes a path to a directory and summarizes the data in the directory to a
+        Takes a path to a directory and summarizes the data in the directory to a table
         `pandas.DataFrame`, much like a log file. This is useful for quickly inspecting
         the contents of a directory.
 
         The dataframe is formatted using the style from :meth:`get_styler
         <erlab.io.dataloader.LoaderBase.get_styler>` and displayed in the IPython shell.
         Results are cached in a pickle file in the directory.
 
         Parameters
         ----------
         data_dir
             Directory to summarize.
         usecache
             Whether to use the cached summary if available. If `False`, the summary will
             be regenerated and the cache will be updated.
+        display
+            Whether to display the formatted dataframe using the IPython shell. If
+            `False`, the dataframe will be returned without formatting. If `True` but
+            the IPython shell is not detected, the dataframe styler will be returned.
         **kwargs
             Additional keyword arguments to be passed to `generate_summary`.
 
         Returns
         -------
-        pandas.DataFrame
-            Summary of the data in the directory.
+        df : pandas.DataFrame or pandas.io.formats.style.Styler or None
+            Summary of the data in the directory. If `display` is `False`, the DataFrame
+            is returned. If `display` is `True` and the IPython shell is detected, the
+            summary will be displayed, and `None` will be returned. If `display` is
+            `True` but the IPython shell is not detected, the styler for the summary
+            DataFrame will be returned.
 
         """
         if not os.path.isdir(data_dir):
             raise FileNotFoundError(f"Directory {data_dir} not found")
 
         pkl_path = os.path.join(data_dir, ".summary.pkl")
         df = None
@@ -436,27 +457,253 @@
             except FileNotFoundError:
                 pass
 
         if df is None:
             df = self.generate_summary(data_dir, **kwargs)
             df.to_pickle(pkl_path)
 
+        if not display:
+            return df
+
+        styled = self.get_styler(df)
+
         try:
             shell = get_ipython().__class__.__name__  # type: ignore
-            if shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]:
+            if display and (
+                shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]
+            ):
                 from IPython.display import display
 
                 with pandas.option_context(
                     "display.max_rows", len(df), "display.max_columns", len(df.columns)
                 ):
-                    display(self.get_styler(df))
+                    display(styled)
+
+                if importlib.util.find_spec("ipywidgets"):
+                    display(self.isummarize(df=df))
+
+                return None
+
         except NameError:
             pass
 
-        return df
+        return styled
+
+    def isummarize(self, df: pandas.DataFrame | None = None, **kwargs):
+        """Display an interactive summary.
+
+        This method provides an interactive summary of the data using ipywidgets and
+        matplotlib.
+
+        Parameters
+        ----------
+        df
+            A summary dataframe as returned by `generate_summary`. If None, a dataframe
+            will be generated using `summarize`. Defaults to None.
+        **kwargs
+            Additional keyword arguments to be passed to `summarize` if `df` is None.
+
+        Note
+        ----
+        This method requires `ipywidgets` to be installed. If not found, an
+        `ImportError` will be raised.
+
+        """
+        if not importlib.util.find_spec("ipywidgets"):
+            raise ImportError(
+                "ipywidgets and IPython is required for interactive summaries"
+            )
+        if df is None:
+            kwargs.setdefault("display", False)
+            df = self.summarize(**kwargs)
+
+        import matplotlib.pyplot as plt
+        import erlab.plotting.erplot as eplt
+
+        from ipywidgets import (
+            HTML,
+            Button,
+            Dropdown,
+            FloatSlider,
+            HBox,
+            Layout,
+            Output,
+            Select,
+            VBox,
+        )
+        from ipywidgets.widgets.interaction import show_inline_matplotlib_plots
+
+        self._temp_data: xr.DataArray | None = None
+
+        def _format_data_info(series) -> str:
+            table = ""
+            table += (
+                "<div class='widget-inline-hbox widget-select' "
+                "style='height:220px;overflow-y:auto;'>"
+            )
+            table += "<table class='widget-select'>"
+            table += "<tbody>"
+
+            for k, v in series.items():
+                if k == "Path":
+                    continue
+                table += "<tr>"
+                table += f"<td style='text-align:left;'><b>{k}</b></td>"
+                table += f"<td style='text-align:left;'>{self.formatter(v)}</td>"
+                table += "</tr>"
+
+            table += "</tbody></table>"
+            table += "</div>"
+            return table
+
+        def _update_data(_, *, full: bool = False):
+            series = df.loc[data_select.value]
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+
+                path = series["Path"]
+
+                full_button.disabled = True
+
+                if not self.always_single:
+                    idx, _ = self.infer_index(
+                        os.path.splitext(os.path.basename(path))[0]
+                    )
+                    if idx is not None:
+                        n_scans = len(self.identify(idx, os.path.dirname(path))[0])
+                        if n_scans > 1 and not full:
+                            full_button.disabled = False
+
+                self._temp_data = self.load(path, single=not full)
+
+                data_info.value = _format_data_info(series)
+
+            if self._temp_data.ndim == 4:
+                # If the data is 4D, average over the last dimension, making it 3D
+                self._temp_data = self._temp_data.mean(self._temp_data.dims[-1])
+
+            if self._temp_data.ndim == 3:
+                dim_sel.unobserve(_update_sliders, "value")
+                coord_sel.unobserve(_update_plot, "value")
+
+                dim_sel.options = self._temp_data.dims
+                # Set the default dimension to the one with the smallest size
+                dim_sel.value = self._temp_data.dims[np.argmin(self._temp_data.shape)]
+
+                coord_sel.observe(_update_plot, "value")
+                dim_sel.observe(_update_sliders, "value")
+
+                dim_sel.disabled = False
+                dim_sel.layout.visibility = "visible"
+                coord_sel.disabled = False
+                coord_sel.layout.visibility = "visible"
+
+                _update_sliders(None)
+
+            else:
+                # 2D or 1D data, disable and hide dimension selection
+                dim_sel.disabled = True
+                dim_sel.layout.visibility = "hidden"
+                coord_sel.disabled = True
+                coord_sel.layout.visibility = "hidden"
+
+            _update_plot(None)
+
+        def _update_sliders(_):
+            if out.block:
+                return
+            if self._temp_data is None:
+                return
+
+            scan_coords = self._temp_data[dim_sel.value].values
+
+            dim_sel.unobserve(_update_sliders, "value")
+            coord_sel.unobserve(_update_plot, "value")
+
+            coord_sel.step = abs(scan_coords[1] - scan_coords[0])
+            coord_sel.max = 1e100  # To ensure max > min always
+            coord_sel.min = scan_coords.min()
+            coord_sel.max = scan_coords.max()
+
+            coord_sel.observe(_update_plot, "value")
+            dim_sel.observe(_update_sliders, "value")
+
+        def _update_plot(_):
+            if self._temp_data is None:
+                return
+            if not coord_sel.disabled:
+                plot_data = self._temp_data.qsel({dim_sel.value: coord_sel.value})
+            else:
+                plot_data = self._temp_data
+
+            out.clear_output(wait=True)
+            with out:
+                plot_data.qplot(ax=plt.gca())
+                # Remove automatic title from xarray
+                plt.title("")
+
+                # Add line at Fermi level if the data is 2D and has an energy dimension
+                if plot_data.ndim == 2 and "eV" in plot_data.dims:
+                    if plot_data["eV"].values[0] * plot_data["eV"].values[-1] < 0:
+                        eplt.fermiline(
+                            orientation="h" if plot_data.dims[0] == "eV" else "v"
+                        )
+
+                show_inline_matplotlib_plots()
+
+        def _next(_):
+            idx = list(df.index).index(data_select.value)
+            if idx + 1 < len(df.index):
+                data_select.value = list(df.index)[idx + 1]
+
+        def _prev(_):
+            idx = list(df.index).index(data_select.value)
+            if idx - 1 >= 0:
+                data_select.value = list(df.index)[idx - 1]
+
+        prev_button = Button(description="Prev", layout=Layout(width="50px"))
+        prev_button.on_click(_prev)
+
+        next_button = Button(description="Next", layout=Layout(width="50px"))
+        next_button.on_click(_next)
+
+        full_button = Button(description="Load full", layout=Layout(width="100px"))
+        full_button.on_click(lambda _: _update_data(None, full=True))
+
+        buttons = [prev_button, next_button]
+        if not self.always_single:
+            buttons.append(full_button)
+
+        data_select = Select(options=list(df.index), value=next(iter(df.index)))
+        data_select.observe(_update_data, "value")
+
+        data_info = HTML()
+
+        dim_sel = Dropdown()
+        dim_sel.observe(_update_sliders, "value")
+
+        coord_sel = FloatSlider(continuous_update=True, readout_format=".3f")
+        coord_sel.observe(_update_plot, "value")
+
+        ui = VBox([HBox(buttons), data_select, data_info, dim_sel, coord_sel])
+
+        out = Output()
+        out.block = False
+
+        show_inline_matplotlib_plots()
+        _update_data(None)
+
+        return HBox(
+            [ui, out],
+            layout=Layout(
+                display="grid",
+                grid_template_columns="auto auto",
+                grid_template_rows="auto",
+            ),
+        )
 
     def load_single(
         self, file_path: str | os.PathLike
     ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
         r"""Load a single file and return it in applicable format.
 
         Any scan-specific postprocessing should be implemented in this method. When the
@@ -504,29 +751,32 @@
             over multiple files, the coordinates will be iterables corresponding to each
             file in the `files` list. For single file scans, an empty dictionary is
             returned.
 
         """
         raise NotImplementedError("method must be implemented in the subclass")
 
-    def infer_index(self, name: str) -> int | None:
+    def infer_index(self, name: str) -> tuple[int | None, dict | None]:
         """Infer the index for the given file name.
 
         This method takes a file name and tries to infer the scan index from it. If the
         index can be inferred, it is returned; otherwise, `None` should be returned.
 
         Parameters
         ----------
         name
             The base name of the file without the path and extension.
 
         Returns
         -------
         index
             The inferred index if found, otherwise None.
+        additional_kwargs
+            Additional keyword arguments to be passed to `load` when the index is found.
+            This argument is useful when the index alone is not enough to load the data.
 
         Note
         ----
         This method is used to determine all files for a given scan. Hence, for loaders
         with `always_single` set to `True`, this method does not have to be implemented.
 
         """
@@ -868,22 +1118,27 @@
         if not isinstance(identifier, int) and os.path.isfile(identifier):
             # If the identifier is a path to a file, ignore data_dir
             data_dir = None
 
         return loader.load(identifier, data_dir=data_dir, **kwargs)
 
     def summarize(
-        self, data_dir: str | os.PathLike | None = None, usecache: bool = True, **kwargs
+        self,
+        data_dir: str | os.PathLike | None = None,
+        usecache: bool = True,
+        *,
+        display: bool = True,
+        **kwargs,
     ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
         loader, default_dir = self._get_current_defaults()
 
         if data_dir is None:
             data_dir = default_dir
 
-        return loader.summarize(data_dir, usecache, **kwargs)
+        return loader.summarize(data_dir, usecache, display=display, **kwargs)
 
     def _get_current_defaults(self):
         if self.current_loader is None:
             raise ValueError(
                 "No loader has been set. Set a loader with `erlab.io.set_loader` first"
             )
         return self.current_loader, self.default_data_dir
```

### Comparing `erlab-2.2.1/src/erlab/io/igor.py` & `erlab-2.2.2/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/plugins/__init__.py` & `erlab-2.2.2/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/plugins/da30.py` & `erlab-2.2.2/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/plugins/kriss.py` & `erlab-2.2.2/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/io/plugins/merlin.py` & `erlab-2.2.2/src/erlab/io/plugins/merlin.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,34 +26,37 @@
         "xi": "Tilt",
         "x": "Sample X",
         "y": "Sample Y (Vert)",
         "z": "Sample Z",
         "hv": "BL Energy",
         "polarization": "EPU POL",
         "temp_sample": "Temperature Sensor B",
-        "photon_flux": "Mesh Current",
+        "mesh_current": "Mesh Current",
     }
     coordinate_attrs: tuple[str, ...] = (
         "beta",
         "delta",
         "xi",
         "hv",
         "x",
         "y",
         "z",
         "polarization",
-        "photon_flux",
+        "mesh_current",
     )
     additional_attrs: dict[str, str | int | float] = {
         "configuration": 1,
         "sample_workfunction": 4.44,
     }
     always_single: bool = False
 
     def load_single(self, file_path: str | os.PathLike) -> xr.DataArray:
+        if os.path.splitext(file_path)[1] == ".ibw":
+            return self.load_live(file_path)
+
         data = load_experiment(file_path)
         # One file always corresponds to single region, so assume only one data variable
         data: xr.DataArray = data.data_vars[next(iter(data.data_vars.keys()))]
 
         return self.process_keys(data)
 
     def identify(
@@ -97,24 +100,24 @@
         if len(files) == 0:
             raise FileNotFoundError(f"No files found for scan {num} in {data_dir}")
 
         files = [os.path.join(data_dir, f) for f in files]
 
         return files, coord_dict
 
-    def infer_index(self, name: str) -> int | None:
+    def infer_index(self, name: str) -> tuple[int | None, dict]:
         try:
             scan_num: str = re.match(r".*?(\d{3})(?:_S\d{3})?", name).group(1)
         except (AttributeError, IndexError):
-            return None
+            return None, None
 
         if scan_num.isdigit():
-            return int(scan_num)
+            return int(scan_num), {}
         else:
-            return None
+            return None, None
 
     def post_process(self, data: xr.DataArray) -> xr.DataArray:
         data = super().post_process(data)
 
         if "eV" in data.coords:
             data = data.assign_coords(eV=-data.eV.values)
 
@@ -134,20 +137,20 @@
         return self.post_process(wave)
 
     def generate_summary(
         self, data_dir: str | os.PathLike, exclude_live: bool = False
     ) -> pd.DataFrame:
         files: dict[str, str] = {}
 
-        for pth in erlab.io.utilities.get_files(data_dir, extensions=(".pxt",)):
-            data_name = os.path.splitext(os.path.basename(pth))[0]
+        for path in erlab.io.utilities.get_files(data_dir, extensions=(".pxt",)):
+            data_name = os.path.splitext(os.path.basename(path))[0]
             name_match = re.match(r"(.*?_\d{3})_(?:_S\d{3})?", data_name)
             if name_match is not None:
                 data_name = name_match.group(1)
-            files[data_name] = pth
+            files[data_name] = path
 
         if not exclude_live:
             for file in os.listdir(data_dir):
                 if file.endswith(".ibw"):
                     data_name = os.path.splitext(file)[0]
                     path = os.path.join(data_dir, file)
                     files[data_name] = path
@@ -166,43 +169,51 @@
             "y": "y",
             "z": "z",
             "polar": "beta",
             "tilt": "xi",
             "azi": "delta",
         }
 
-        cols = ["Time", "File Name", "Type", *summary_attrs.keys()]
+        cols = ["File Name", "Path", "Time", "Type", *summary_attrs.keys()]
 
-        data: list[dict] = []
         data_info = []
 
+        processed_indices: list[int] = []
+
         for name, path in files.items():
             if os.path.splitext(path)[1] == ".ibw":
                 data = self.load_live(path)
                 if "beta" in data.dims:
                     data_type = "LP"
                 else:
                     data_type = "LXY"
             else:
+                idx, _ = self.infer_index(os.path.splitext(os.path.basename(path))[0])
+                if idx in processed_indices:
+                    continue
+
+                if idx is not None:
+                    processed_indices.append(idx)
                 data = self.load(path)
                 data_type = "core"
                 if "alpha" in data.dims:
                     data_type = "cut"
                 if "beta" in data.dims:
                     data_type = "map"
                 if "hv" in data.dims:
                     data_type = "hvdep"
 
             data_info.append(
                 [
+                    name,
+                    path,
                     datetime.datetime.strptime(
                         f"{data.attrs['Date']} {data.attrs['Time']}",
                         "%d/%m/%Y %I:%M:%S %p",
                     ),
-                    name,
                     data_type,
                 ]
             )
 
             for k, v in summary_attrs.items():
                 try:
                     val = data.attrs[v]
```

### Comparing `erlab-2.2.1/src/erlab/io/plugins/ssrl52.py` & `erlab-2.2.2/src/erlab/io/plugins/ssrl52.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,25 +184,26 @@
             "z": "z",
             "polar": "chi",
             "tilt": "xi",
             "azi": "delta",
             "DA": "beta",
         }
 
-        cols = ["Time", "File Name", *summary_attrs.keys()]
+        cols = ["File Name", "Path", "Time", *summary_attrs.keys()]
 
         data_info = []
 
         for name, path in files.items():
             data = self.load(path)
 
             data_info.append(
                 [
-                    datetime.datetime.fromtimestamp(data.attrs["CreationTimeStamp"]),
                     name,
+                    path,
+                    datetime.datetime.fromtimestamp(data.attrs["CreationTimeStamp"]),
                 ]
             )
 
             for k, v in summary_attrs.items():
                 try:
                     val = data.attrs[v]
                 except KeyError:
```

### Comparing `erlab-2.2.1/src/erlab/io/utilities.py` & `erlab-2.2.2/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/lattice.py` & `erlab-2.2.2/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/parallel.py` & `erlab-2.2.2/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.2.2/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/__init__.py` & `erlab-2.2.2/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/annotations.py` & `erlab-2.2.2/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/atoms.py` & `erlab-2.2.2/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/bz.py` & `erlab-2.2.2/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/colors.py` & `erlab-2.2.2/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/erplot.py` & `erlab-2.2.2/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/general.py` & `erlab-2.2.2/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/plot3d.py` & `erlab-2.2.2/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.2.2/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/src/erlab.egg-info/PKG-INFO` & `erlab-2.2.2/src/erlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -730,14 +730,15 @@
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: viz
 Requires-Dist: cmasher; extra == "viz"
 Requires-Dist: cmocean; extra == "viz"
 Requires-Dist: colorcet; extra == "viz"
 Requires-Dist: hvplot; extra == "viz"
+Requires-Dist: ipywidgets; extra == "viz"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/erlab.svg)](https://anaconda.org/conda-forge/erlab)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
```

### Comparing `erlab-2.2.1/src/erlab.egg-info/SOURCES.txt` & `erlab-2.2.2/src/erlab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,9 @@
 tests/analysis/test_fastbinning.py
 tests/analysis/test_fit_functions_dynamic.py
 tests/analysis/test_fit_functions_general.py
 tests/analysis/test_fit_models.py
 tests/analysis/test_image.py
 tests/analysis/test_interpolate.py
 tests/analysis/test_kspace.py
-tests/analysis/test_utilities.py
+tests/analysis/test_utilities.py
+tests/io/test_dataloader.py
```

### Comparing `erlab-2.2.1/src/erlab.egg-info/requires.txt` & `erlab-2.2.2/src/erlab.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -37,7 +37,8 @@
 sphinx-design
 
 [viz]
 cmasher
 cmocean
 colorcet
 hvplot
+ipywidgets
```

### Comparing `erlab-2.2.1/templates/.macros.j2` & `erlab-2.2.2/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_fastbinning.py` & `erlab-2.2.2/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.2.2/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_fit_functions_general.py` & `erlab-2.2.2/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_fit_models.py` & `erlab-2.2.2/tests/analysis/test_fit_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_image.py` & `erlab-2.2.2/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_interpolate.py` & `erlab-2.2.2/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2.1/tests/analysis/test_kspace.py` & `erlab-2.2.2/tests/analysis/test_kspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         assert kx.size == ky.size == k_tot.size
         assert np.allclose(kx, 0.1)
         assert np.allclose(ky, 0.2)
 
 
 @pytest.fixture()
 def angle_data():
-    return generate_data_angles(shape=(10, 10, 10))
+    return generate_data_angles(shape=(10, 10, 10), assign_attributes=True)
 
 
 def test_offsets(angle_data):
     angle_data.kspace.offsets.reset()
     angle_data.kspace.offsets = {"xi": 10.0}
     answer = dict.fromkeys(angle_data.kspace.valid_offset_keys, 0.0)
     answer["xi"] = 10.0
```

### Comparing `erlab-2.2.1/tests/analysis/test_utilities.py` & `erlab-2.2.2/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

